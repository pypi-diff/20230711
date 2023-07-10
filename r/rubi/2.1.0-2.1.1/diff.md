# Comparing `tmp/rubi-2.1.0.tar.gz` & `tmp/rubi-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.1.0.tar", max compression
+gzip compressed data, was "rubi-2.1.1.tar", max compression
```

## Comparing `rubi-2.1.0.tar` & `rubi-2.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11357 2023-07-06 01:41:13.434500 rubi-2.1.0/LICENSE
--rw-r--r--   0        0        0     2757 2023-07-06 01:41:13.434500 rubi-2.1.0/README.md
--rw-r--r--   0        0        0     6735 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      721 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      745 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      648 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      721 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0     1729 2023-07-06 01:41:53.450427 rubi-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-06 01:41:13.438500 rubi-2.1.0/rubi/__init__.py
--rw-r--r--   0        0        0    28087 2023-07-06 01:41:13.438500 rubi-2.1.0/rubi/client.py
--rw-r--r--   0        0        0      163 2023-07-06 01:41:13.438500 rubi-2.1.0/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    61077 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/aid.py
--rw-r--r--   0        0        0    11860 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0       74 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/contract_types/__init__.py
--rw-r--r--   0        0        0    15968 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/contract_types/events.py
--rw-r--r--   0        0        0     2708 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/contract_types/transaction_reciept.py
--rw-r--r--   0        0        0    18474 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24668 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/market.py
--rw-r--r--   0        0        0    14847 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/router.py
--rw-r--r--   0        0        0       77 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/data/README.md
--rw-r--r--   0        0        0       31 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/data/__init__.py
--rw-r--r--   0        0        0     9355 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/data/market.py
--rw-r--r--   0        0        0       72 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/network/__init__.py
--rw-r--r--   0        0        0     8181 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/network/network.py
--rw-r--r--   0        0        0       93 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/rubicon_types/__init__.py
--rw-r--r--   0        0        0    15638 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/rubicon_types/order.py
--rw-r--r--   0        0        0    10670 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/rubicon_types/order_query.py
--rw-r--r--   0        0        0     6410 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/rubicon_types/orderbook.py
--rw-r--r--   0        0        0     2776 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/rubicon_types/pair.py
--rw-r--r--   0        0        0     3595 1970-01-01 00:00:00.000000 rubi-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-10 23:49:14.175642 rubi-2.1.1/LICENSE
+-rw-r--r--   0        0        0     2757 2023-07-10 23:49:14.175642 rubi-2.1.1/README.md
+-rw-r--r--   0        0        0     6735 2023-07-10 23:49:14.175642 rubi-2.1.1/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-07-10 23:49:14.175642 rubi-2.1.1/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      721 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      745 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      648 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      721 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0     1729 2023-07-10 23:49:41.515647 rubi-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/__init__.py
+-rw-r--r--   0        0        0    28087 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/client.py
+-rw-r--r--   0        0        0      163 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    61077 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    12008 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0       74 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/contract_types/__init__.py
+-rw-r--r--   0        0        0    15968 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/contract_types/events.py
+-rw-r--r--   0        0        0     2708 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/contract_types/transaction_reciept.py
+-rw-r--r--   0        0        0    18524 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24736 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14865 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/router.py
+-rw-r--r--   0        0        0       77 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/data/README.md
+-rw-r--r--   0        0        0       31 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/data/__init__.py
+-rw-r--r--   0        0        0     9355 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/data/market.py
+-rw-r--r--   0        0        0       72 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/network/__init__.py
+-rw-r--r--   0        0        0     8181 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/network/network.py
+-rw-r--r--   0        0        0       93 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/rubicon_types/__init__.py
+-rw-r--r--   0        0        0    15639 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/rubicon_types/order.py
+-rw-r--r--   0        0        0    10670 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/rubicon_types/order_query.py
+-rw-r--r--   0        0        0     6411 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/rubicon_types/orderbook.py
+-rw-r--r--   0        0        0     2776 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/rubicon_types/pair.py
+-rw-r--r--   0        0        0     3595 1970-01-01 00:00:00.000000 rubi-2.1.1/PKG-INFO
```

### Comparing `rubi-2.1.0/LICENSE` & `rubi-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/README.md` & `rubi-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/network_config/ERC20.json` & `rubi-2.1.1/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/network_config/README.md` & `rubi-2.1.1/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/network_config/abitrum_goerli/abis/market.json` & `rubi-2.1.1/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/network_config/abitrum_goerli/abis/router.json` & `rubi-2.1.1/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/network_config/abitrum_goerli/network.yaml` & `rubi-2.1.1/network_config/abitrum_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/network_config/optimism/abis/market.json` & `rubi-2.1.1/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/network_config/optimism/abis/router.json` & `rubi-2.1.1/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/network_config/optimism/network.yaml` & `rubi-2.1.1/network_config/optimism/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/network_config/optimism_goerli/abis/market.json` & `rubi-2.1.1/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/network_config/optimism_goerli/abis/router.json` & `rubi-2.1.1/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/network_config/optimism_goerli/network.yaml` & `rubi-2.1.1/network_config/optimism_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/network_config/polygon_mumbai/abis/market.json` & `rubi-2.1.1/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/network_config/polygon_mumbai/abis/router.json` & `rubi-2.1.1/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/network_config/polygon_mumbai/network.yaml` & `rubi-2.1.1/network_config/polygon_mumbai/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/pyproject.toml` & `rubi-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.1.0"
+version = "2.1.1"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `rubi-2.1.0/rubi/client.py` & `rubi-2.1.1/rubi/client.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/rubi/contracts/aid.py` & `rubi-2.1.1/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/rubi/contracts/base_contract.py` & `rubi-2.1.1/rubi/contracts/base_contract.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,29 +176,29 @@
     ######################################################################
     # helper methods
     ######################################################################
 
     def _default_transaction_handler(
         self,
         instantiated_contract_function: ContractFunction,
-        gas: int,
-        nonce: Optional[int] = None,
-        max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        gas: Optional[int],
+        nonce: Optional[int],
+        max_fee_per_gas: Optional[int],
+        max_priority_fee_per_gas: Optional[int],
     ) -> TransactionReceipt:
         """Default transaction handler for executing transactions against this contract. This function will build, sign
         and execute a transaction with reasonable defaults (mostly from the web3py library).
 
         Note: if a nonce is not passed then this function will query to the wallet to get the nonce and also wait for
         the transaction receipt before returning.
 
         :param instantiated_contract_function: The instantiated contract function to call.
         :type instantiated_contract_function: ContractFunction
-        :param gas: The gas limit for the transaction.
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param nonce: Optional nonce value for the transaction (optional, default is None).
         :type nonce: Optional[int]
         :param max_fee_per_gas: Optional maximum fee per gas for the transaction (optional, default is None).
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: Optional maximum priority fee per gas for the transaction.
             (optional, default is None).
         :type max_priority_fee_per_gas: Optional[int]
@@ -229,25 +229,25 @@
         self.w3.eth.send_raw_transaction(signed_txn.rawTransaction)
 
         return self._wait_for_transaction_receipt(transaction=signed_txn)
 
     def _transaction_params(
         self,
         nonce: Optional[Nonce],
-        gas: int,
+        gas: Optional[int],
         max_fee_per_gas: Optional[int],
         max_priority_fee_per_gas: Optional[int]
     ) -> Dict:
         """Build transaction parameters Dict for a transaction. If a key is associated with a None value after building
         the Dict then this key will be removed before returning the dict.
 
         :param nonce: Optional nonce value for the transaction (optional, default is None).
         :type nonce: Optional[Nonce]
-        :param gas: The gas limit for the transaction.
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: Optional maximum fee per gas for the transaction (optional, default is None).
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: Optional maximum priority fee per gas for the transaction.
             (optional, default is None).
         :type max_priority_fee_per_gas: Optional[int]
         :return: The transaction parameters dictionary.
         :rtype: Dict
@@ -258,14 +258,15 @@
 
         transaction = {
             'chainId': self.chain_id,
             'gas': gas,
             'maxFeePerGas': max_fee_per_gas,
             'maxPriorityFeePerGas': max_priority_fee_per_gas,
             'nonce': nonce,
+            'from': self.wallet
         }
 
         return {key: value for key, value in transaction.items() if value is not None}
 
     def _wait_for_transaction_receipt(self, transaction: SignedTransaction) -> TransactionReceipt:
         """Wait for the transaction receipt and check if the transaction was successful.
```

### Comparing `rubi-2.1.0/rubi/contracts/contract_types/events.py` & `rubi-2.1.1/rubi/contracts/contract_types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/rubi/contracts/contract_types/transaction_reciept.py` & `rubi-2.1.1/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/rubi/contracts/erc20.py` & `rubi-2.1.1/rubi/contracts/erc20.py`

 * *Files 4% similar despite different names*

```diff
@@ -212,29 +212,29 @@
 
     # approve(spender (address), amount (uint256)) -> bool
     def approve(
         self,
         spender: ChecksumAddress,
         amount: int,
         nonce: Optional[int] = None,
-        gas: int = 100000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Approves the spender to spend the amount of the erc20 token from the signer's wallet
 
         :param spender: address of the spender
         :type spender: ChecksumAddress
         :param amount: amount of the erc20 token to approve the spender to spend
         :type amount: int
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
         :type nonce: Optional[int]
-        :param gas: gas limit of the transaction, defaults to a very high estimate made when writing the class
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
@@ -252,28 +252,28 @@
 
     # transfer(recipient (address), amount (uint256)) -> bool
     def transfer(
         self,
         recipient: ChecksumAddress,
         amount: int,
         nonce: Optional[int] = None,
-        gas: int = 100000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Transfers the amount of the erc20 token to the recipient
 
         :param recipient: address of the recipient
         :type recipient: ChecksumAddress
         :param amount: amount of the erc20 token to transfer
         :type amount: int
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce
         :type nonce: Optional[int]
-        :param gas: gas limit of the transaction, defaults to a very high estimate made when writing the class
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
@@ -292,31 +292,31 @@
     # transferFrom(sender (address), recipient (address), amount (uint256)) -> bool
     def transfer_from(
         self,
         sender: ChecksumAddress,
         recipient: ChecksumAddress,
         amount: int,
         nonce: Optional[int] = None,
-        gas: int = 100000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Transfers the amount of the erc20 token from the sender to the recipient
 
         :param sender: address of the sender
         :type sender: ChecksumAddress
         :param recipient: address of the recipient
         :type recipient: ChecksumAddress
         :param amount: amount of the erc20 token to transfer
         :type amount: int
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
         :type nonce: Optional[int]
-        :param gas: gas limit of the transaction, defaults to a very high estimate made when writing the class
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
@@ -335,29 +335,29 @@
 
     # increaseAllowance(spender (address), addedValue (uint256)) -> bool
     def increase_allowance(
         self,
         spender: ChecksumAddress,
         added_value: int,
         nonce: Optional[int] = None,
-        gas: int = 100000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Increases the allowance of the spender by the added_value
 
         :param spender: address of the spender
         :type spender: ChecksumAddress
         :param added_value: amount to increase the allowance by, in the integer representation of the erc20 token
         :type added_value: int
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
         :type nonce: Optional[int]
-        :param gas: gas limit of the transaction, defaults to a very high estimate made when writing the class
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
@@ -375,29 +375,29 @@
 
     # decreaseAllowance(spender (address), subtractedValue (uint256)) -> bool
     def decrease_allowance(
         self,
         spender: ChecksumAddress,
         subtracted_value: int,
         nonce: Optional[int] = None,
-        gas: int = 100000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Decreases the allowance of the spender by the subtracted_value
 
         :param spender: address of the spender
         :type spender: ChecksumAddress
         :param subtracted_value: amount to decrease the allowance by, in the integer representation of the erc20 token
         :type subtracted_value: int
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
         :type nonce: Optional[int]
-        :param gas: gas limit of the transaction, defaults to a very high estimate made when writing the class
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
```

### Comparing `rubi-2.1.0/rubi/contracts/market.py` & `rubi-2.1.1/rubi/contracts/market.py`

 * *Files 8% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         buy_amt: int,
         buy_gem: ChecksumAddress,
         pos: int = 0,
         rounding: bool = True,
         owner: Optional[ChecksumAddress] = None,
         recipient: Optional[ChecksumAddress] = None,
         nonce: Optional[int] = None,
-        gas: int = 400000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Make a new offer to buy the buy_amt of the buy_gem token in exchange for the pay_amt of the pay_gem token
 
         :param pay_amt: the amount of the token being sold
         :type pay_amt: int
@@ -251,16 +251,16 @@
         :type owner: Optional[ChecksumAddress]
         :param recipient: the recipient of the offer's fill, defaults to the wallet that was provided in instantiating
             this class (optional, default is None)
         :type recipient: Optional[ChecksumAddress]
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
         :type nonce: Optional[int]
-        :param gas: gas limit of the transaction, defaults to a very high estimate made when writing the class
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
@@ -285,27 +285,27 @@
         )
 
     # cancel(id (uint256)) -> bool
     def cancel(
         self,
         id: int,
         nonce: Optional[int] = None,
-        gas: int = 350000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Cancel an offer by offer id
 
         :param id: the id of the offer to cancel
         :type id: int
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
         :type nonce: Optional[int]
-        :param gas: gas limit of the transaction, defaults to a very high estimate made when writing the class
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
@@ -326,15 +326,15 @@
     def batch_offer(
         self,
         pay_amts: List[int],
         pay_gems: List[ChecksumAddress],
         buy_amts: List[int],
         buy_gems: List[ChecksumAddress],
         nonce: Optional[int] = None,
-        gas: int = 3500000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Batch the placement of a set of offers in one transaction
 
         :param pay_amts: the amounts of the token being sold
         :type pay_amts: List[int]
@@ -343,16 +343,16 @@
         :param buy_amts: the amounts of the token being bought
         :type buy_amts: List[int]
         :param buy_gems: the addresses of the tokens being bought
         :type buy_gems: List[ChecksumAddress]
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
         :type nonce: Optional[int]
-        :param gas: gas limit of the transaction, defaults to a very high estimate made when writing the class
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
@@ -372,27 +372,27 @@
         )
 
     # batchCancel (ids (uint256[])) -> bool[]
     def batch_cancel(
         self,
         ids: List[int],
         nonce: Optional[int] = None,
-        gas: int = 3500000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Cancel a set offer by offer id in a single transaction
 
         :param ids: the ids of the offers to cancel
         :type ids: List[int]
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
         :type nonce: Optional[int]
-        :param gas: gas limit of the transaction, defaults to a very high estimate made when writing the class
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
@@ -414,15 +414,15 @@
         self,
         ids: List[int],
         pay_amts: List[int],
         pay_gems: List[ChecksumAddress],
         buy_amts: List[int],
         buy_gems: List[ChecksumAddress],
         nonce: Optional[int] = None,
-        gas: int = 800000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Batch update a set of offers in a single transaction and return a list of new offer ids
 
         :param ids: the ids of the offers to cancel
         :type ids: List[int]
@@ -433,16 +433,16 @@
         :param buy_amts: the amounts of the token being bought
         :type buy_amts: List[int]
         :param buy_gems: the addresses of the tokens being bought
         :type buy_gems: List[ChecksumAddress]
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
         :type nonce: Optional[int]
-        :param gas: gas limit of the transaction, defaults to a very high estimate made when writing the class
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
@@ -463,15 +463,15 @@
     def sell_all_amount(
         self,
         pay_gem: ChecksumAddress,
         pay_amt: int,
         buy_gem: ChecksumAddress,
         min_fill_amount: int,
         nonce: Optional[int] = None,
-        gas: int = 500000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Sell the pay_amt of the pay_gem token in exchange for buy_gem, on the condition that you receive at least the
         min_fill_amount of the buy_gem token
 
         :param pay_gem: the address of the tokens being sold
@@ -481,16 +481,16 @@
         :param buy_gem: the address of the tokens being bought
         :type buy_gem: ChecksumAddress
         :param min_fill_amount: minimum amount of the buy_gem token you want to receive
         :type min_fill_amount: int
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
         :type nonce: Optional[int]
-        :param gas: gas limit of the transaction, defaults to a very high estimate made when writing the class
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
@@ -510,15 +510,15 @@
     def buy_all_amount(
         self,
         buy_gem: ChecksumAddress,
         buy_amt: int,
         pay_gem: ChecksumAddress,
         max_fill_amount: int,
         nonce: Optional[int] = None,
-        gas: int = 500000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Buy the buy_amt of the buy_gem token in exchange for pay_gem, on the condition that it does not exceed the
         max_fill_amount of the pay_gem token
 
         :param buy_gem: the address of the tokens being bought
@@ -528,16 +528,16 @@
         :param pay_gem: the address of the tokens being sold
         :type pay_gem: ChecksumAddress
         :param max_fill_amount: maximum amount of the pay_gem token you want to pay
         :type max_fill_amount: int
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
         :type nonce: Optional[int]
-        :param gas: gas limit of the transaction, defaults to a very high estimate made when writing the class
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
```

### Comparing `rubi-2.1.0/rubi/contracts/router.py` & `rubi-2.1.1/rubi/contracts/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     def multiswap(
         self,
         routes: List[List[ChecksumAddress]],
         pay_amts: List[int],
         buy_amts_min: List[int],
         to: ChecksumAddress,
         nonce: Optional[int] = None,
-        gas: int = 350000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Perform a multiple swaps for the specified payment amounts using the specified routes. Reverts with an
         exception if any of the swaps cannot achieve the buy_amt_min along the specified route.
 
         :param routes: The list of routes, where each route is a list of addresses representing the swap path.
@@ -254,16 +254,16 @@
         :param buy_amts_min: The list of minimum buy amounts for each swap.
         :type buy_amts_min: List[int]
         :param to: The address of the recipient.
         :type to: ChecksumAddress
         :param nonce: Nonce of the transaction. Defaults to calling the chain state to get the nonce.
             (optional, default is None).
         :type nonce: Optional[int]
-        :param gas: Gas limit of the transaction. Defaults to a very high estimate made when writing the class.
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: Max fee that can be paid for gas. Defaults to max_priority_fee (from chain)
             + (2 * base fee per gas of latest block) (optional, default is None).
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: Max priority fee that can be paid for gas. Defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None).
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
@@ -284,15 +284,15 @@
     def swap(
         self,
         pay_amt: int,
         buy_amt_min: int,
         route: List[ChecksumAddress],
         to: ChecksumAddress,
         nonce: Optional[int] = None,
-        gas: int = 350000,
+        gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Perform a swap operation with the specified payment amount using the specified route and paying out to the
         recipient. Reverts if the swap does not result in the buy_min_amount.
 
         :param pay_amt: The payment amount.
@@ -302,16 +302,16 @@
         :param route: The route, represented as a list of addresses representing the swap path.
         :type route: List[ChecksumAddress]
         :param to: The address of the recipient.
         :type to: ChecksumAddress
         :param nonce: Nonce of the transaction. Defaults to calling the chain state to get the nonce.
             (optional, default is None).
         :type nonce: Optional[int]
-        :param gas: Gas limit of the transaction. Defaults to a very high estimate made when writing the class.
-        :type gas: int
+        :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
+        :type gas: Optional[int]
         :param max_fee_per_gas: Max fee that can be paid for gas. Defaults to max_priority_fee (from chain)
             + (2 * base fee per gas of latest block) (optional, default is None).
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: Max priority fee that can be paid for gas. Defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None).
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
```

### Comparing `rubi-2.1.0/rubi/data/market.py` & `rubi-2.1.1/rubi/data/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/rubi/network/network.py` & `rubi-2.1.1/rubi/network/network.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/rubi/rubicon_types/order.py` & `rubi-2.1.1/rubi/rubicon_types/order.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,15 @@
             pair_name=pair_name,
             order_type=OrderType.LIMIT,
             order_side=OrderSide.NEUTRAL,
         )
 
         self.order_id = order_id
 
+
 # TODO: add a new class for a limit order object that is returned from the subgraph
 
 class Transaction:
     """
     Class representing a transaction to be executed on chain
 
     :param orders: The list of orders to include in the transaction.
```

### Comparing `rubi-2.1.0/rubi/rubicon_types/order_query.py` & `rubi-2.1.1/rubi/rubicon_types/order_query.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/rubi/rubicon_types/orderbook.py` & `rubi-2.1.1/rubi/rubicon_types/orderbook.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,8 +196,8 @@
 
         return self.best_ask() - self.best_bid()
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
 
-# TODO: add a DetailedORderBook class that contains the full order book composed of LimitOrder instances
+# TODO: add a DetailedOrderBook class that contains the full order book composed of LimitOrder instances
```

### Comparing `rubi-2.1.0/rubi/rubicon_types/pair.py` & `rubi-2.1.1/rubi/rubicon_types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.0/PKG-INFO` & `rubi-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.1.0
+Version: 2.1.1
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

