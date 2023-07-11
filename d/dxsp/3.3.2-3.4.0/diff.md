# Comparing `tmp/dxsp-3.3.2.tar.gz` & `tmp/dxsp-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.3.2.tar", max compression
+gzip compressed data, was "dxsp-3.4.0.tar", max compression
```

## Comparing `dxsp-3.3.2.tar` & `dxsp-3.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-10 10:06:14.418350 dxsp-3.3.2/LICENSE
--rw-r--r--   0        0        0     2697 2023-07-10 10:06:14.418350 dxsp-3.3.2/README.md
--rw-r--r--   0        0        0      115 2023-07-10 10:06:15.142357 dxsp-3.3.2/dxsp/__init__.py
--rw-r--r--   0        0        0      417 2023-07-10 10:06:14.418350 dxsp-3.3.2/dxsp/config.py
--rw-r--r--   0        0        0    10489 2023-07-10 10:06:14.418350 dxsp-3.3.2/dxsp/default_settings.toml
--rw-r--r--   0        0        0    17229 2023-07-10 10:06:14.418350 dxsp-3.3.2/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-10 10:06:14.418350 dxsp-3.3.2/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-10 10:06:14.418350 dxsp-3.3.2/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1773 2023-07-10 10:06:14.418350 dxsp-3.3.2/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      990 2023-07-10 10:06:14.418350 dxsp-3.3.2/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2328 2023-07-10 10:06:15.142357 dxsp-3.3.2/pyproject.toml
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 dxsp-3.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-11 19:36:15.202038 dxsp-3.4.0/LICENSE
+-rw-r--r--   0        0        0     2697 2023-07-11 19:36:15.202038 dxsp-3.4.0/README.md
+-rw-r--r--   0        0        0      115 2023-07-11 19:36:15.970050 dxsp-3.4.0/dxsp/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-11 19:36:15.202038 dxsp-3.4.0/dxsp/config.py
+-rw-r--r--   0        0        0    10713 2023-07-11 19:36:15.202038 dxsp-3.4.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    16465 2023-07-11 19:36:15.202038 dxsp-3.4.0/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-11 19:36:15.206039 dxsp-3.4.0/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-11 19:36:15.206039 dxsp-3.4.0/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1773 2023-07-11 19:36:15.206039 dxsp-3.4.0/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      990 2023-07-11 19:36:15.206039 dxsp-3.4.0/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2328 2023-07-11 19:36:15.970050 dxsp-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 dxsp-3.4.0/PKG-INFO
```

### Comparing `dxsp-3.3.2/LICENSE` & `dxsp-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.2/README.md` & `dxsp-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.2/dxsp/default_settings.toml` & `dxsp-3.4.0/dxsp/default_settings.toml`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 trading_asset = "USDT"
 trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
 trading_risk_amount = 10 # 10% of the position
 dex_trading_slippage = 2 # 2% slippage
-
+dex_notify_invalid_token = true
 
 
 
 
 
 
 ##############
@@ -47,14 +47,15 @@
 dex_factory_contract_addr = "0x5C69bEe701ef814a2B6a3EDD4B1652CB9cc5aA6f"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
 trading_asset = "USDT"
 trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
 trading_risk_amount = 10 
 dex_trading_slippage = 2
+dex_notify_invalid_token = true
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
 [zerox]
 VALUE = "test_zerox"
@@ -70,14 +71,15 @@
 dex_factory_contract_addr = ""
 dex_router_abi_url = "https://raw.githubusercontent.com/0xProject/protocol/development/packages/contract-artifacts/artifacts/Exchange.json"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
 trading_asset = "USDT"
 trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
 trading_risk_amount = 10
 dex_trading_slippage = 2
+dex_notify_invalid_token = true
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
 [testnet]
 VALUE = "On Testnet"
@@ -92,14 +94,15 @@
 dex_factory_contract_addr = "0x5C69bEe701ef814a2B6a3EDD4B1652CB9cc5aA6f"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
 trading_asset = "USDC"
 trading_asset_address = "0xa3726f2e6423caF1824cD7721B543B29b621fB4f"
 trading_risk_amount = 10
 dex_trading_slippage = 2
+dex_notify_invalid_token = true
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
 [bsc]
 VALUE = "chain_56"
@@ -111,14 +114,15 @@
 dex_rpc = "https://rpc.ankr.com/bsc"
 dex_router_contract_addr = "0x10ED43C718714eb63d5aA57B78B54704E256024E"
 dex_factory_contract_addr = "0xcA143Ce32Fe78f1f7019d7d551a6402fC5350c73"
 trading_asset = "BUSD"
 trading_asset_address = "0xe9e7cea3dedca5984780bafc599bd69add087d56"
 trading_risk_amount = 10 
 dex_trading_slippage = 2
+dex_notify_invalid_token = false
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
 [uniswap3]
 VALUE = "On uniswap3"
@@ -133,14 +137,15 @@
 dex_factory_contract_addr = "0x68b3465833fb72A70ecDF485E0e4C7bD8665Fc45"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
 trading_asset = "USDT"
 trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
 trading_risk_amount = 10 
 dex_trading_slippage = 2
+dex_notify_invalid_token = true
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
 [pancake3]
 VALUE = "On pancake3"
@@ -155,14 +160,15 @@
 dex_factory_contract_addr = "0x13f4EA83D0bd40E75C8222255bc855a974568Dd4"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
 trading_asset = "BUSD"
 trading_asset_address = "0xe9e7cea3dedca5984780bafc599bd69add087d56"
 trading_risk_amount = 10 
 dex_trading_slippage = 2
+dex_notify_invalid_token = true
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
```

### Comparing `dxsp-3.3.2/dxsp/main.py` & `dxsp-3.4.0/dxsp/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
  DEX SWAP Main
 """
 
 import logging
 from typing import Optional
-from datetime import datetime
+from datetime import datetime, timedelta
 import requests
 from pycoingecko import CoinGeckoAPI
 from web3 import Web3
 from web3.gas_strategies.time_based import medium_gas_price_strategy
 from dxsp import __version__
 from dxsp.config import settings
 
@@ -20,15 +20,16 @@
         self.w3 = w3 or Web3(Web3.HTTPProvider(settings.dex_rpc))
         if self.w3.net.listening:
             self.logger.info("connected %s", self.w3)
             self.w3.eth.set_gas_price_strategy(medium_gas_price_strategy)
             self.chain_id = self.w3.net.version
             self.wallet_address = self.w3.to_checksum_address(
                 settings.dex_wallet_address)
-            self.account = f"{str(self.w3.net.version)} - {str(self.wallet_address[-8:])}"
+            self.account = (f"{str(self.w3.net.version)} - "
+                            f"{str(self.wallet_address[-8:])}")
             self.private_key = settings.dex_private_key
             self.trading_asset_address = self.w3.to_checksum_address(
                 settings.trading_asset_address)
 
             self.protocol_type = settings.dex_protocol_type
             self.protocol_version = settings.dex_protocol_version
             self.dex_swap = None
@@ -80,16 +81,18 @@
             if not buy_token_address.startswith("0x"):
                 buy_token_address = await self.search_contract_address(buy_token)
             sell_amount = await self.calculate_sell_amount(sell_token_address, quantity)
             sell_token_amount_wei = sell_amount * (10 ** (
                 await self.get_token_decimals(sell_token_address)))
             await self.get_approve(sell_token_address)
 
-            order_amount = int(sell_token_amount_wei * (settings.dex_trading_slippage / 100))
-            order = await self.dex_swap.get_swap(sell_token_address, buy_token_address, order_amount)
+            order_amount = int(
+                sell_token_amount_wei * (settings.dex_trading_slippage / 100))
+            order = await self.dex_swap.get_swap(
+                sell_token_address, buy_token_address, order_amount)
 
             if not order:
                 raise ValueError("swap order not executed")
 
             signed_order = await self.get_sign(order)
             order_hash = str(self.w3.to_hex(signed_order))
             receipt = self.w3.wait_for_transaction_receipt(order_hash)
@@ -169,17 +172,19 @@
         except Exception as error:
             raise error
 
     async def calculate_sell_amount(self, sell_token_address, quantity):
         """Returns amount based on risk percentage."""
         sell_balance = await self.get_token_balance(sell_token_address)
         sell_contract = await self.get_token_contract(sell_token_address)
-        sell_decimals = sell_contract.functions.decimals().call() if sell_contract is not None else 18
+        sell_decimals = (sell_contract.functions.decimals().call() 
+        if sell_contract is not None else 18)
         risk_percentage = settings.trading_risk_amount
-        return (sell_balance / (risk_percentage * 10 ** sell_decimals)) * (float(quantity) / 100)
+        return (sell_balance / 
+        (risk_percentage * 10 ** sell_decimals)) * (float(quantity) / 100)
 
     async def get_confirmation(self, transactionHash):
         """Returns trade confirmation."""
         try:
             transaction = self.w3.eth.get_transaction(transactionHash)
             block = self.w3.eth.get_block(transaction["blockNumber"])
             return {
@@ -231,15 +236,17 @@
                 token
             )
             if token_address is not None:
                 return self.w3.to_checksum_address(token_address)
 
         token_address = await self.search_cg_contract(token)
         if token_address is None:
-            raise ValueError("Invalid Token")
+            if settings.dex_notify_invalid_token:
+                raise ValueError("Invalid Token")
+            return
         return self.w3.to_checksum_address(token_address)
 
     async def search_cg_platform(self):
         """search coingecko platform"""
         asset_platforms = self.cg.get_asset_platforms()
         output_dict = next(
             x for x in asset_platforms
@@ -310,15 +317,15 @@
         """Get token balance"""
         contract = await self.get_token_contract(token_address)
         if contract is None or contract.functions is None:
             raise ValueError("No Balance")
         balance = contract.functions.balanceOf(self.wallet_address).call()
         if balance is None:
             raise ValueError("No Balance")
-        return balance
+        return round(balance,5)
 
     async def get_explorer_abi(self, address):
         if not settings.dex_block_explorer_api:
             return None
 
         params = {
             "module": "contract",
@@ -331,26 +338,31 @@
         if resp['status'] == "1":
             self.logger.debug("ABI found %s", resp)
             return resp["result"]
         else:
             return None
 
 # 🔒 USER RELATED
-    async def get_name(self):
-        return settings.dex_router_contract_addr[-8:]
-
     async def get_info(self):
-        return f"{__class__.__name__} {__version__}\n💱 {await self.get_name()}\n🪪 {self.account}"
+        return (f"ℹ️ {__class__.__name__} {__version__}\n"
+                f"💱 {await self.get_name()}\n"
+                f"🪪 {self.account}")
+
+    async def get_name(self):
+        if settings.dex_router_contract_addr:
+            return settings.dex_router_contract_addr[-8:]
+        else:
+            return self.protocol_type
 
     async def get_account_balance(self):
         account_balance = self.w3.eth.get_balance(
             self.w3.to_checksum_address(self.wallet_address))
         account_balance = self.w3.from_wei(account_balance, 'ether') or 0
         trading_asset_balance = await self.get_trading_asset_balance() or 0
-        return f"₿ {account_balance}\n💵 {trading_asset_balance}"
+        return f"₿ {round(account_balance,5)}\n💵 {trading_asset_balance}"
 
     async def get_trading_asset_balance(self):
         trading_asset_balance = await self.get_token_balance(
             self.trading_asset_address)
         return trading_asset_balance if trading_asset_balance else 0
 
     async def get_account_position(self):
@@ -358,52 +370,38 @@
         position = "📊 Position\n" + str(open_positions)
         position += "\n" + str(await self.get_account_margin())
         return position
 
     async def get_account_margin(self):
         return 0
 
-    async def get_account_pnl(self, frequency="daily"):
-
-        latest_tx_date = await self.get_block_timestamp(self.w3.eth.get_block('latest'))
-
-        #total_profit_loss = 0
+    async def get_account_pnl(self, period=24):
+        """
+        Retrieves the profit and loss (PnL) information for the account.
+        WIP not ready
+        """
+        transaction_list = await self.get_account_transactions(period)
+        return {
+            "latest block": transaction_list['latest block'],
+            "instrument": 0,
+            "Total PnL": 0,
+            "OpenPnl": 0
+            }
 
-        # for tx in transactions:
-        #     # Retrieve the transaction details
-        #     tx_value = tx['value']
-        #     tx_status = tx['status']
-        #     tx_timestamp = datetime.fromtimestamp(tx['timestamp'])
-
-        #     # Check if the transaction falls within the desired frequency
-        #     if frequency == "daily":
-        #         start_date = datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)
-        #         end_date = datetime.now()
-        #     elif frequency == "weekly":
-        #         start_date = datetime.now().replace(hour=0, minute=0, second=0, microsecond=0) - timedelta(days=datetime.now().weekday())
-        #         end_date = datetime.now()
-        #     elif frequency == "monthly":
-        #         start_date = datetime.now().replace(day=1, hour=0, minute=0, second=0, microsecond=0)
-        #         end_date = datetime.now()
-        #     elif frequency == "quarterly":
-        #         quarter = (datetime.now().month - 1) // 3
-        #         start_date = datetime(datetime.now().year, 3 * quarter + 1, 1).replace(hour=0, minute=0, second=0, microsecond=0)
-        #         end_date = datetime.now()
-        #     elif frequency == "yearly":
-        #         start_date = datetime(datetime.now().year, 1, 1).replace(hour=0, minute=0, second=0, microsecond=0)
-        #         end_date = datetime.now()
-
-        #     if start_date <= tx_timestamp <= end_date:
-        #         # Check if the transaction was successful
-        #         if tx_status == 1:
-        #             # Check if the transaction resulted in profit or loss
-        #             if tx_value > 0:
-        #                 total_profit_loss += tx_value
-        #             else:
-        #                 total_profit_loss -= tx_value
-
-        # if total_profit_loss > 0:
-        #     return f"Transactions made. Profit ({frequency}): {total_profit_loss}"
-        # elif total_profit_loss < 0:
-        #     return f"Transactions made. Loss ({frequency}): {abs(total_profit_loss)}"
-        # else:
-        #     return f"Transactions made ({frequency}), but no profit or loss."
+    async def get_account_transactions(self, period=24):
+        """
+        Retrieves the account transactions within a specified time period.
+        WIP not ready
+        """
+        latest_block = self.w3.eth.get_block_number()
+        latest_transaction_timestamp = await self.get_block_timestamp(latest_block)
+        time_difference = datetime.utcnow() - latest_transaction_timestamp
+        print(time_difference)        
+        if time_difference <= timedelta(hours=period):
+            # TODO
+            # Get user transaction history
+            # for a given transaction withing the time period
+            # consolidate the pnl per instrument and return it
+            return {
+                    "latest block": latest_transaction_timestamp,
+                    }
+        return None
```

### Comparing `dxsp-3.3.2/dxsp/protocols/oneinch.py` & `dxsp-3.4.0/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.2/dxsp/protocols/uniswap.py` & `dxsp-3.4.0/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.2/dxsp/protocols/zerox.py` & `dxsp-3.4.0/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.2/pyproject.toml` & `dxsp-3.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "3.3.2"
+version = "3.4.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-3.3.2/PKG-INFO` & `dxsp-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 3.3.2
+Version: 3.4.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dxsp Version: 3.3.2 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 3.4.0 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: pycoingecko (>=3.1.0,<4.0.0) Requires-Dist:
 uniswap-python (>=0.7.0,<0.8.0) Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-
```

