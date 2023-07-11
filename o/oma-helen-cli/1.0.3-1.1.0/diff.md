# Comparing `tmp/oma-helen-cli-1.0.3.tar.gz` & `tmp/oma-helen-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oma-helen-cli-1.0.3.tar", last modified: Mon Apr 24 19:09:42 2023, max compression
+gzip compressed data, was "oma-helen-cli-1.1.0.tar", last modified: Tue Jul 11 06:10:29 2023, max compression
```

## Comparing `oma-helen-cli-1.0.3.tar` & `oma-helen-cli-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 caro       (501) staff       (20)        0 2023-04-24 19:09:42.323016 oma-helen-cli-1.0.3/
--rw-r--r--   0 caro       (501) staff       (20)     1079 2022-09-09 11:17:34.000000 oma-helen-cli-1.0.3/LICENSE
--rw-r--r--   0 caro       (501) staff       (20)     6648 2023-04-24 19:09:42.322884 oma-helen-cli-1.0.3/PKG-INFO
--rw-r--r--   0 caro       (501) staff       (20)     5846 2023-04-24 19:04:33.000000 oma-helen-cli-1.0.3/README.md
-drwxr-xr-x   0 caro       (501) staff       (20)        0 2023-04-24 19:09:42.310481 oma-helen-cli-1.0.3/helenservice/
--rw-r--r--   0 caro       (501) staff       (20)        0 2022-09-18 16:57:21.000000 oma-helen-cli-1.0.3/helenservice/__init__.py
--rw-r--r--   0 caro       (501) staff       (20)    13751 2023-04-24 18:00:21.000000 oma-helen-cli-1.0.3/helenservice/api_client.py
--rw-r--r--   0 caro       (501) staff       (20)       54 2023-04-24 17:38:45.000000 oma-helen-cli-1.0.3/helenservice/api_exceptions.py
--rw-r--r--   0 caro       (501) staff       (20)     1038 2023-01-17 18:10:03.000000 oma-helen-cli-1.0.3/helenservice/api_response.py
--rwxr-xr-x   0 caro       (501) staff       (20)     6486 2023-04-24 18:48:11.000000 oma-helen-cli-1.0.3/helenservice/cli.py
--rw-r--r--   0 caro       (501) staff       (20)       22 2022-09-19 18:41:34.000000 oma-helen-cli-1.0.3/helenservice/const.py
--rw-r--r--   0 caro       (501) staff       (20)     5538 2022-09-20 16:14:21.000000 oma-helen-cli-1.0.3/helenservice/helen_session.py
--rw-r--r--   0 caro       (501) staff       (20)     5324 2023-04-24 17:25:36.000000 oma-helen-cli-1.0.3/helenservice/price_client.py
--rw-r--r--   0 caro       (501) staff       (20)      447 2023-01-14 21:51:15.000000 oma-helen-cli-1.0.3/helenservice/utils.py
-drwxr-xr-x   0 caro       (501) staff       (20)        0 2023-04-24 19:09:42.322728 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/
--rw-r--r--   0 caro       (501) staff       (20)     6648 2023-04-24 19:09:42.000000 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/PKG-INFO
--rw-r--r--   0 caro       (501) staff       (20)      521 2023-04-24 19:09:42.000000 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/SOURCES.txt
--rw-r--r--   0 caro       (501) staff       (20)        1 2023-04-24 19:09:42.000000 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/dependency_links.txt
--rw-r--r--   0 caro       (501) staff       (20)       56 2023-04-24 19:09:42.000000 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/entry_points.txt
--rw-r--r--   0 caro       (501) staff       (20)        1 2023-01-14 22:28:51.000000 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/not-zip-safe
--rw-r--r--   0 caro       (501) staff       (20)      121 2023-04-24 19:09:42.000000 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/requires.txt
--rw-r--r--   0 caro       (501) staff       (20)       13 2023-04-24 19:09:42.000000 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/top_level.txt
--rw-r--r--   0 caro       (501) staff       (20)       38 2023-04-24 19:09:42.323050 oma-helen-cli-1.0.3/setup.cfg
--rw-r--r--   0 caro       (501) staff       (20)     1562 2023-04-24 19:08:01.000000 oma-helen-cli-1.0.3/setup.py
+drwxr-xr-x   0 caro       (501) staff       (20)        0 2023-07-11 06:10:29.654856 oma-helen-cli-1.1.0/
+-rw-r--r--   0 caro       (501) staff       (20)     1079 2022-09-09 11:17:34.000000 oma-helen-cli-1.1.0/LICENSE
+-rw-r--r--   0 caro       (501) staff       (20)     7208 2023-07-11 06:10:29.654724 oma-helen-cli-1.1.0/PKG-INFO
+-rw-r--r--   0 caro       (501) staff       (20)     6406 2023-07-11 06:09:10.000000 oma-helen-cli-1.1.0/README.md
+drwxr-xr-x   0 caro       (501) staff       (20)        0 2023-07-11 06:10:29.652361 oma-helen-cli-1.1.0/helenservice/
+-rw-r--r--   0 caro       (501) staff       (20)        0 2022-09-18 16:57:21.000000 oma-helen-cli-1.1.0/helenservice/__init__.py
+-rw-r--r--   0 caro       (501) staff       (20)    18446 2023-07-11 06:09:10.000000 oma-helen-cli-1.1.0/helenservice/api_client.py
+-rw-r--r--   0 caro       (501) staff       (20)       54 2023-04-24 19:11:17.000000 oma-helen-cli-1.1.0/helenservice/api_exceptions.py
+-rw-r--r--   0 caro       (501) staff       (20)     1038 2023-01-17 18:10:03.000000 oma-helen-cli-1.1.0/helenservice/api_response.py
+-rwxr-xr-x   0 caro       (501) staff       (20)     8170 2023-07-11 06:09:10.000000 oma-helen-cli-1.1.0/helenservice/cli.py
+-rw-r--r--   0 caro       (501) staff       (20)       22 2022-09-19 18:41:34.000000 oma-helen-cli-1.1.0/helenservice/const.py
+-rw-r--r--   0 caro       (501) staff       (20)     5538 2022-09-20 16:14:21.000000 oma-helen-cli-1.1.0/helenservice/helen_session.py
+-rw-r--r--   0 caro       (501) staff       (20)     5324 2023-04-24 19:11:17.000000 oma-helen-cli-1.1.0/helenservice/price_client.py
+-rw-r--r--   0 caro       (501) staff       (20)      447 2023-01-14 21:51:15.000000 oma-helen-cli-1.1.0/helenservice/utils.py
+drwxr-xr-x   0 caro       (501) staff       (20)        0 2023-07-11 06:10:29.654555 oma-helen-cli-1.1.0/oma_helen_cli.egg-info/
+-rw-r--r--   0 caro       (501) staff       (20)     7208 2023-07-11 06:10:29.000000 oma-helen-cli-1.1.0/oma_helen_cli.egg-info/PKG-INFO
+-rw-r--r--   0 caro       (501) staff       (20)      521 2023-07-11 06:10:29.000000 oma-helen-cli-1.1.0/oma_helen_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 caro       (501) staff       (20)        1 2023-07-11 06:10:29.000000 oma-helen-cli-1.1.0/oma_helen_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 caro       (501) staff       (20)       56 2023-07-11 06:10:29.000000 oma-helen-cli-1.1.0/oma_helen_cli.egg-info/entry_points.txt
+-rw-r--r--   0 caro       (501) staff       (20)        1 2023-01-14 22:28:51.000000 oma-helen-cli-1.1.0/oma_helen_cli.egg-info/not-zip-safe
+-rw-r--r--   0 caro       (501) staff       (20)      121 2023-07-11 06:10:29.000000 oma-helen-cli-1.1.0/oma_helen_cli.egg-info/requires.txt
+-rw-r--r--   0 caro       (501) staff       (20)       13 2023-07-11 06:10:29.000000 oma-helen-cli-1.1.0/oma_helen_cli.egg-info/top_level.txt
+-rw-r--r--   0 caro       (501) staff       (20)       38 2023-07-11 06:10:29.654893 oma-helen-cli-1.1.0/setup.cfg
+-rw-r--r--   0 caro       (501) staff       (20)     1562 2023-07-11 06:09:10.000000 oma-helen-cli-1.1.0/setup.py
```

### Comparing `oma-helen-cli-1.0.3/LICENSE` & `oma-helen-cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oma-helen-cli-1.0.3/PKG-INFO` & `oma-helen-cli-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oma-helen-cli
-Version: 1.0.3
+Version: 1.1.0
 Summary: Oma Helen API library and CLI
 Home-page: https://github.com/carohauta/oma-helen-cli
 Author: carohauta
 Author-email: carosoft.dev@gmail.com
 License: MIT license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -59,18 +59,21 @@
 | get_api_access_token          | Get the access token to the Oma Helen API. With the token, you can make queries to your own contracts and data in Oma Helen |
 | get_contract_base_price       | Get the monthly base price of your current electricity contract |
 | get_contract_data_json        | Returns the whole contract data as JSON. Will return all active contracts you have with Helen |
 | get_contract_delivery_site_id | Get the delivery site id from the contract data |
 | get_daily_measurements_json   | Returns your daily energy consumption for the on-going month of the on-going year as JSON |
 | get_market_prices_json        | Returns the prices for the Market Price Electricity contract as JSON. The JSON includes the price for last month, the current month and next month if available |
 | get_monthly_measurements_json | Returns your monthly energy consumption for the on-going year as JSON |
-| calculate_the_impact_of_usage_between_dates | Calculates your impact of usage between given dates for the Helen Smart Electricity Guarantee |
-| calculate_spot_cost_between_dates | Calculates the total costs between given dates of a spot price contract in an hourly precision |
+| calculate_the_impact_of_usage_between_dates | Calculates your impact of usage (in c/kwh) between given dates for the Helen Smart Electricity Guarantee |
+| calculate_spot_cost_between_dates | Calculates the total costs (eur) between given dates of a spot price contract in an hourly precision |
 | get_exchange_margin_price_json | Get the margin price of the Exchange Electricity contract |
-| get_contract_energy_unit_price | Get the energy unit price (c/kwh) from your contract data |
+| get_contract_energy_unit_price | Get the energy unit price (c/kwh) from your contract data. Note that this only works for fixed price contracts. For spot electricity contract, this returns 0.0 |
+| get_contract_transfer_fee      | Get the transfer fees (c/kwh) from your contract. Note that if Helen is not your transfer company, this returns 0.0 |
+| calculate_transfer_fees_between_dates | Calculates total transfer fees (eur) based on your consumption between dates |
+| get_contract_transfer_base_price | Get the monthly transfer base price (eur) from your contract. Note that if Helen is not your transfer company, this returns 0.0 |
 
 ### Oma Helen API example
 
 In this example, in addition to the `access-token`, you are going to need your delivery site id (`Consumption` or `Käyttöpaikka`) from Oma Helen. You can get it with the CLI tool's `get_contract_delivery_site_id` function.
 
 #### Making a request
```

### Comparing `oma-helen-cli-1.0.3/README.md` & `oma-helen-cli-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -37,18 +37,21 @@
 | get_api_access_token          | Get the access token to the Oma Helen API. With the token, you can make queries to your own contracts and data in Oma Helen |
 | get_contract_base_price       | Get the monthly base price of your current electricity contract |
 | get_contract_data_json        | Returns the whole contract data as JSON. Will return all active contracts you have with Helen |
 | get_contract_delivery_site_id | Get the delivery site id from the contract data |
 | get_daily_measurements_json   | Returns your daily energy consumption for the on-going month of the on-going year as JSON |
 | get_market_prices_json        | Returns the prices for the Market Price Electricity contract as JSON. The JSON includes the price for last month, the current month and next month if available |
 | get_monthly_measurements_json | Returns your monthly energy consumption for the on-going year as JSON |
-| calculate_the_impact_of_usage_between_dates | Calculates your impact of usage between given dates for the Helen Smart Electricity Guarantee |
-| calculate_spot_cost_between_dates | Calculates the total costs between given dates of a spot price contract in an hourly precision |
+| calculate_the_impact_of_usage_between_dates | Calculates your impact of usage (in c/kwh) between given dates for the Helen Smart Electricity Guarantee |
+| calculate_spot_cost_between_dates | Calculates the total costs (eur) between given dates of a spot price contract in an hourly precision |
 | get_exchange_margin_price_json | Get the margin price of the Exchange Electricity contract |
-| get_contract_energy_unit_price | Get the energy unit price (c/kwh) from your contract data |
+| get_contract_energy_unit_price | Get the energy unit price (c/kwh) from your contract data. Note that this only works for fixed price contracts. For spot electricity contract, this returns 0.0 |
+| get_contract_transfer_fee      | Get the transfer fees (c/kwh) from your contract. Note that if Helen is not your transfer company, this returns 0.0 |
+| calculate_transfer_fees_between_dates | Calculates total transfer fees (eur) based on your consumption between dates |
+| get_contract_transfer_base_price | Get the monthly transfer base price (eur) from your contract. Note that if Helen is not your transfer company, this returns 0.0 |
 
 ### Oma Helen API example
 
 In this example, in addition to the `access-token`, you are going to need your delivery site id (`Consumption` or `Käyttöpaikka`) from Oma Helen. You can get it with the CLI tool's `get_contract_delivery_site_id` function.
 
 #### Making a request
```

### Comparing `oma-helen-cli-1.0.3/helenservice/api_response.py` & `oma-helen-cli-1.1.0/helenservice/api_response.py`

 * *Files identical despite different names*

### Comparing `oma-helen-cli-1.0.3/helenservice/cli.py` & `oma-helen-cli-1.1.0/helenservice/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,14 +30,37 @@
     def do_exit(self, input=None):
         """Exit the CLI"""
 
         self.api_client.close()
         print("Bye")
         return True
 
+    def do_calculate_transfer_fees_between_dates(self, input=None):
+        """Calculate the transfer fees between a start date and an end date
+        The provided dates should be presented in format 'YYYY-mm-dd'
+
+        Usage example:
+        calculate_transfer_fee_between_dates 2022-12-01 2022-12-31
+        """
+
+        if input is None:
+            print("Please provide proper start and end dates in format 'YYYY-mm-dd'")
+        else:
+            try:
+                start_date_str, end_date_str = str(input).split(' ')
+                start_date = datetime.strptime(start_date_str, '%Y-%m-%d').date()
+                end_date = datetime.strptime(end_date_str, '%Y-%m-%d').date()
+                if start_date > end_date: 
+                    print("Start date must be before end date")
+                    raise ValueError()
+                price = self.api_client.calculate_transfer_fees_between_dates(start_date, end_date)
+                print(price)
+            except ValueError:
+                print("Please provide proper start and end dates in format 'YYYY-mm-dd'")
+
     def do_calculate_spot_cost_between_dates(self, input=None):
         """Calculate the price of your Exchange Electricity (spot) contract between a start date and an end date
         The provided dates should be presented in format 'YYYY-mm-dd'
 
         Includes 10% tax. The price returned is in euros.
 
         Usage example:
@@ -128,14 +151,26 @@
 
     def do_get_contract_base_price(self, input=None):
         """Helper to get the contract base price from your contract data. To see the whole contract data as JSON, use get_contract_data_json"""
         
         base_price = self.api_client.get_contract_base_price()
         print(base_price)
 
+    def do_get_contract_transfer_fee(self, input=None):
+        """Helper to get the transfer fee price from your contract data. To see the whole contract data as JSON, use get_contract_data_json"""
+        
+        base_price = self.api_client.get_transfer_fee()
+        print(base_price)
+
+    def do_get_contract_transfer_base_price(self, input=None):
+        """Helper to get the transfer base price from your contract data. To see the whole contract data as JSON, use get_contract_data_json"""
+        
+        base_price = self.api_client.get_transfer_base_price()
+        print(base_price)
+
     def do_get_api_access_token(self, input=None):
         """Get your access token for the Oma Helen API."""
         
         access_token = self.api_client.get_api_access_token()
         print(access_token)
 
     def do_get_contract_energy_unit_price(self, input=None):
```

### Comparing `oma-helen-cli-1.0.3/helenservice/helen_session.py` & `oma-helen-cli-1.1.0/helenservice/helen_session.py`

 * *Files identical despite different names*

### Comparing `oma-helen-cli-1.0.3/helenservice/price_client.py` & `oma-helen-cli-1.1.0/helenservice/price_client.py`

 * *Files identical despite different names*

### Comparing `oma-helen-cli-1.0.3/oma_helen_cli.egg-info/PKG-INFO` & `oma-helen-cli-1.1.0/oma_helen_cli.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oma-helen-cli
-Version: 1.0.3
+Version: 1.1.0
 Summary: Oma Helen API library and CLI
 Home-page: https://github.com/carohauta/oma-helen-cli
 Author: carohauta
 Author-email: carosoft.dev@gmail.com
 License: MIT license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -59,18 +59,21 @@
 | get_api_access_token          | Get the access token to the Oma Helen API. With the token, you can make queries to your own contracts and data in Oma Helen |
 | get_contract_base_price       | Get the monthly base price of your current electricity contract |
 | get_contract_data_json        | Returns the whole contract data as JSON. Will return all active contracts you have with Helen |
 | get_contract_delivery_site_id | Get the delivery site id from the contract data |
 | get_daily_measurements_json   | Returns your daily energy consumption for the on-going month of the on-going year as JSON |
 | get_market_prices_json        | Returns the prices for the Market Price Electricity contract as JSON. The JSON includes the price for last month, the current month and next month if available |
 | get_monthly_measurements_json | Returns your monthly energy consumption for the on-going year as JSON |
-| calculate_the_impact_of_usage_between_dates | Calculates your impact of usage between given dates for the Helen Smart Electricity Guarantee |
-| calculate_spot_cost_between_dates | Calculates the total costs between given dates of a spot price contract in an hourly precision |
+| calculate_the_impact_of_usage_between_dates | Calculates your impact of usage (in c/kwh) between given dates for the Helen Smart Electricity Guarantee |
+| calculate_spot_cost_between_dates | Calculates the total costs (eur) between given dates of a spot price contract in an hourly precision |
 | get_exchange_margin_price_json | Get the margin price of the Exchange Electricity contract |
-| get_contract_energy_unit_price | Get the energy unit price (c/kwh) from your contract data |
+| get_contract_energy_unit_price | Get the energy unit price (c/kwh) from your contract data. Note that this only works for fixed price contracts. For spot electricity contract, this returns 0.0 |
+| get_contract_transfer_fee      | Get the transfer fees (c/kwh) from your contract. Note that if Helen is not your transfer company, this returns 0.0 |
+| calculate_transfer_fees_between_dates | Calculates total transfer fees (eur) based on your consumption between dates |
+| get_contract_transfer_base_price | Get the monthly transfer base price (eur) from your contract. Note that if Helen is not your transfer company, this returns 0.0 |
 
 ### Oma Helen API example
 
 In this example, in addition to the `access-token`, you are going to need your delivery site id (`Consumption` or `Käyttöpaikka`) from Oma Helen. You can get it with the CLI tool's `get_contract_delivery_site_id` function.
 
 #### Making a request
```

### Comparing `oma-helen-cli-1.0.3/oma_helen_cli.egg-info/SOURCES.txt` & `oma-helen-cli-1.1.0/oma_helen_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oma-helen-cli-1.0.3/setup.py` & `oma-helen-cli-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,10 +43,10 @@
     install_requires=requirements,
     license="MIT license",
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
     packages=find_packages(include=['helenservice', 'helenservice.*']),
     url='https://github.com/carohauta/oma-helen-cli',
-    version='1.0.3',
+    version='1.1.0',
     zip_safe=False,
 )
```

