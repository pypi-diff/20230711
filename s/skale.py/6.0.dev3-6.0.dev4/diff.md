# Comparing `tmp/skale.py-6.0.dev3.tar.gz` & `tmp/skale.py-6.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skale.py-6.0.dev3.tar", last modified: Fri Jul  7 12:56:58 2023, max compression
+gzip compressed data, was "dist/skale.py-6.0.dev4.tar", last modified: Tue Jul 11 10:56:16 2023, max compression
```

## Comparing `skale.py-6.0.dev3.tar` & `skale.py-6.0.dev4.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-07 12:56:56.000000 skale.py-6.0.dev3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale/contracts/allocator/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/allocator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/allocator/allocator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/allocator/escrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/base_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/contract_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale/contracts/ima/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/ima/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/ima/linker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale/contracts/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/bounty_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/constants_holder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale/contracts/manager/delegation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/delegation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/delegation/delegation_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/delegation/delegation_period_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/delegation/distributor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/delegation/slashing_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/delegation/token_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/delegation/validator_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/dkg.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/key_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/node_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/punisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/schains.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/schains_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/sync_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale/contracts/manager/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/test/time_helpers_with_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/contracts/manager/wallets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale/dataclasses/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/dataclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/dataclasses/delegation_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/dataclasses/node_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/dataclasses/schain_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/dataclasses/skaled_ports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale/schain_config/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/schain_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/schain_config/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/schain_config/ports_allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/schain_config/rotation_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/skale_allocator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/skale_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/skale_ima.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/skale_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/transactions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/transactions/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/transactions/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/abi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/account_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/contract_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/contract_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale/utils/contracts_provision/
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/contracts_provision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/contracts_provision/allocator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/contracts_provision/fake_multisig_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/contracts_provision/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/contracts_provision/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale/utils/random_names/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/random_names/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/random_names/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/random_names/vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/utils/web3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale/wallets/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/wallets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/wallets/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/wallets/ledger_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/wallets/redis_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/wallets/rpc_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/wallets/sgx_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/skale/wallets/web3_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-07 12:56:57.000000 skale.py-6.0.dev3/skale.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/skale.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:56:57.000000 skale.py-6.0.dev3/skale.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-07 12:56:57.000000 skale.py-6.0.dev3/skale.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 12:56:57.000000 skale.py-6.0.dev3/skale.py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:56:58.000000 skale.py-6.0.dev3/tests/schain_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/tests/schain_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/tests/schain_config/generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-07 12:54:44.000000 skale.py-6.0.dev3/tests/schain_config/ports_allocation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-11 10:56:15.000000 skale.py-6.0.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale/contracts/allocator/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/allocator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/allocator/allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/allocator/escrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/base_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/contract_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale/contracts/ima/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/ima/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/ima/linker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale/contracts/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/bounty_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/constants_holder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale/contracts/manager/delegation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/delegation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/delegation/delegation_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/delegation/delegation_period_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/delegation/distributor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/delegation/slashing_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/delegation/token_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/delegation/validator_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/dkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/key_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/node_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/punisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/schains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/schains_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/sync_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale/contracts/manager/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/test/time_helpers_with_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/contracts/manager/wallets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale/dataclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/dataclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/dataclasses/delegation_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/dataclasses/node_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/dataclasses/schain_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/dataclasses/skaled_ports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale/schain_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/schain_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/schain_config/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/schain_config/ports_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/schain_config/rotation_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/skale_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/skale_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/skale_ima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/skale_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/transactions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/transactions/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/transactions/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/abi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/account_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/contract_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/contract_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale/utils/contracts_provision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/contracts_provision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/contracts_provision/allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/contracts_provision/fake_multisig_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/contracts_provision/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/contracts_provision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale/utils/random_names/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/random_names/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/random_names/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/random_names/vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/utils/web3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale/wallets/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/wallets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/wallets/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/wallets/ledger_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/wallets/redis_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/wallets/rpc_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/wallets/sgx_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/skale/wallets/web3_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/skale.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:56:16.000000 skale.py-6.0.dev4/tests/schain_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/tests/schain_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/tests/schain_config/generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-11 10:54:37.000000 skale.py-6.0.dev4/tests/schain_config/ports_allocation_test.py
```

### Comparing `skale.py-6.0.dev3/LICENSE` & `skale.py-6.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/PKG-INFO` & `skale.py-6.0.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale.py
-Version: 6.0.dev3
+Version: 6.0.dev4
 Summary: SKALE client tools
 Home-page: https://github.com/skalenetwork/skale.py
 Author: SKALE Labs
 Author-email: support@skalelabs.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: skale
```

### Comparing `skale.py-6.0.dev3/README.md` & `skale.py-6.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/setup.py` & `skale.py-6.0.dev4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 extras_require['dev'] = (
     extras_require['linter'] + extras_require['dev'] + extras_require['hw-wallet']
 )
 
 setup(
     name='skale.py',
-    version='6.0dev3',
+    version='6.0dev4',
     description='SKALE client tools',
     long_description_markdown_filename='README.md',
     author='SKALE Labs',
     author_email='support@skalelabs.com',
     url='https://github.com/skalenetwork/skale.py',
     include_package_data=True,
     install_requires=[
```

### Comparing `skale.py-6.0.dev3/skale/config.py` & `skale.py-6.0.dev4/skale/config.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/allocator/allocator.py` & `skale.py-6.0.dev4/skale/contracts/allocator/allocator.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/allocator/escrow.py` & `skale.py-6.0.dev4/skale/contracts/allocator/escrow.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/base_contract.py` & `skale.py-6.0.dev4/skale/contracts/base_contract.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/contract_manager.py` & `skale.py-6.0.dev4/skale/contracts/contract_manager.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/ima/linker.py` & `skale.py-6.0.dev4/skale/contracts/ima/linker.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/__init__.py` & `skale.py-6.0.dev4/skale/contracts/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/bounty_v2.py` & `skale.py-6.0.dev4/skale/contracts/manager/bounty_v2.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/constants_holder.py` & `skale.py-6.0.dev4/skale/contracts/manager/constants_holder.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/delegation/delegation_controller.py` & `skale.py-6.0.dev4/skale/contracts/manager/delegation/delegation_controller.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/delegation/delegation_period_manager.py` & `skale.py-6.0.dev4/skale/contracts/manager/delegation/delegation_period_manager.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/delegation/distributor.py` & `skale.py-6.0.dev4/skale/contracts/manager/delegation/distributor.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/delegation/slashing_table.py` & `skale.py-6.0.dev4/skale/contracts/manager/delegation/slashing_table.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/delegation/token_state.py` & `skale.py-6.0.dev4/skale/contracts/manager/delegation/token_state.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/delegation/validator_service.py` & `skale.py-6.0.dev4/skale/contracts/manager/delegation/validator_service.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/dkg.py` & `skale.py-6.0.dev4/skale/contracts/manager/dkg.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/groups.py` & `skale.py-6.0.dev4/skale/contracts/manager/groups.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/key_storage.py` & `skale.py-6.0.dev4/skale/contracts/manager/key_storage.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/manager.py` & `skale.py-6.0.dev4/skale/contracts/manager/manager.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/node_rotation.py` & `skale.py-6.0.dev4/skale/contracts/manager/node_rotation.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/nodes.py` & `skale.py-6.0.dev4/skale/contracts/manager/nodes.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/punisher.py` & `skale.py-6.0.dev4/skale/contracts/manager/punisher.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/schains.py` & `skale.py-6.0.dev4/skale/contracts/manager/schains.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/schains_internal.py` & `skale.py-6.0.dev4/skale/contracts/manager/schains_internal.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/sync_manager.py` & `skale.py-6.0.dev4/skale/contracts/manager/sync_manager.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/test/time_helpers_with_debug.py` & `skale.py-6.0.dev4/skale/contracts/manager/test/time_helpers_with_debug.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/token.py` & `skale.py-6.0.dev4/skale/contracts/manager/token.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/contracts/manager/wallets.py` & `skale.py-6.0.dev4/skale/contracts/manager/wallets.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/dataclasses/__init__.py` & `skale.py-6.0.dev4/skale/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/dataclasses/delegation_status.py` & `skale.py-6.0.dev4/skale/dataclasses/delegation_status.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/dataclasses/node_info.py` & `skale.py-6.0.dev4/skale/dataclasses/node_info.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/dataclasses/schain_options.py` & `skale.py-6.0.dev4/skale/dataclasses/schain_options.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/dataclasses/skaled_ports.py` & `skale.py-6.0.dev4/skale/dataclasses/skaled_ports.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/schain_config/__init__.py` & `skale.py-6.0.dev4/skale/schain_config/__init__.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/schain_config/generator.py` & `skale.py-6.0.dev4/skale/schain_config/generator.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/schain_config/ports_allocation.py` & `skale.py-6.0.dev4/skale/schain_config/ports_allocation.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/schain_config/rotation_history.py` & `skale.py-6.0.dev4/skale/schain_config/rotation_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,31 +28,26 @@
 RotationNodeData = namedtuple('RotationNodeData', ['index', 'node_id', 'public_key'])
 
 
 def get_previous_schain_groups(
     skale: Skale,
     schain_name: str,
     leaving_node_id=None,
-    include_keys=True
 ) -> dict:
     """
     Returns all previous node groups with public keys and finish timestamps.
     In case of no rotations returns the current state.
     """
     logger.info(f'Collecting rotation history for {schain_name}...')
     node_groups = {}
 
     group_id = skale.schains.name_to_group_id(schain_name)
 
-    previous_public_keys = None
-    current_public_key = None
-
-    if include_keys:
-        previous_public_keys = skale.key_storage.get_all_previous_public_keys(group_id)
-        current_public_key = skale.key_storage.get_common_public_key(group_id)
+    previous_public_keys = skale.key_storage.get_all_previous_public_keys(group_id)
+    current_public_key = skale.key_storage.get_common_public_key(group_id)
 
     rotation = skale.node_rotation.get_rotation_obj(schain_name)
 
     logger.info(f'Rotation data for {schain_name}: {rotation}')
 
     _add_current_schain_state(skale, node_groups, rotation, schain_name, current_public_key)
     if rotation.rotation_counter == 0:
@@ -134,16 +129,18 @@
         nodes[previous_node_id] = RotationNodeData(
             nodes[new_node_id].index,
             previous_node_id,
             public_key
         )
         del nodes[new_node_id]
 
-        if not next_dkg_is_failed and previous_public_keys is not None:
-            bls_public_key = _pop_previous_bls_public_key(previous_public_keys)
+        bls_public_key = None
+        if not next_dkg_is_failed:
+            if len(previous_public_keys) > 0:
+                bls_public_key = _pop_previous_bls_public_key(previous_public_keys)
         else:
             bls_public_key = node_groups[rotation_id + 1]['bls_public_key']
             node_groups[rotation_id + 1]['finish_ts'] = None
             node_groups[rotation_id + 1]['bls_public_key'] = None
 
         logger.info(f'Adding rotation: {previous_node_id} -> {new_node_id}')
```

### Comparing `skale.py-6.0.dev3/skale/skale_allocator.py` & `skale.py-6.0.dev4/skale/skale_allocator.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/skale_base.py` & `skale.py-6.0.dev4/skale/skale_base.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/skale_ima.py` & `skale.py-6.0.dev4/skale/skale_ima.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/skale_manager.py` & `skale.py-6.0.dev4/skale/skale_manager.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/transactions/result.py` & `skale.py-6.0.dev4/skale/transactions/result.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/transactions/tools.py` & `skale.py-6.0.dev4/skale/transactions/tools.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/abi_utils.py` & `skale.py-6.0.dev4/skale/utils/abi_utils.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/account_tools.py` & `skale.py-6.0.dev4/skale/utils/account_tools.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/constants.py` & `skale.py-6.0.dev4/skale/utils/constants.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/contract_info.py` & `skale.py-6.0.dev4/skale/utils/contract_info.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/contract_types.py` & `skale.py-6.0.dev4/skale/utils/contract_types.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/contracts_provision/__init__.py` & `skale.py-6.0.dev4/skale/utils/contracts_provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/contracts_provision/allocator.py` & `skale.py-6.0.dev4/skale/utils/contracts_provision/allocator.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/contracts_provision/fake_multisig_contract.py` & `skale.py-6.0.dev4/skale/utils/contracts_provision/fake_multisig_contract.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/contracts_provision/main.py` & `skale.py-6.0.dev4/skale/utils/contracts_provision/main.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/contracts_provision/utils.py` & `skale.py-6.0.dev4/skale/utils/contracts_provision/utils.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/exceptions.py` & `skale.py-6.0.dev4/skale/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/helper.py` & `skale.py-6.0.dev4/skale/utils/helper.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/random_names/generator.py` & `skale.py-6.0.dev4/skale/utils/random_names/generator.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/random_names/vocabulary.py` & `skale.py-6.0.dev4/skale/utils/random_names/vocabulary.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/utils/web3_utils.py` & `skale.py-6.0.dev4/skale/utils/web3_utils.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/wallets/common.py` & `skale.py-6.0.dev4/skale/wallets/common.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/wallets/ledger_wallet.py` & `skale.py-6.0.dev4/skale/wallets/ledger_wallet.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/wallets/redis_wallet.py` & `skale.py-6.0.dev4/skale/wallets/redis_wallet.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/wallets/rpc_wallet.py` & `skale.py-6.0.dev4/skale/wallets/rpc_wallet.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/wallets/sgx_wallet.py` & `skale.py-6.0.dev4/skale/wallets/sgx_wallet.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale/wallets/web3_wallet.py` & `skale.py-6.0.dev4/skale/wallets/web3_wallet.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/skale.py.egg-info/PKG-INFO` & `skale.py-6.0.dev4/skale.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale.py
-Version: 6.0.dev3
+Version: 6.0.dev4
 Summary: SKALE client tools
 Home-page: https://github.com/skalenetwork/skale.py
 Author: SKALE Labs
 Author-email: support@skalelabs.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: skale
```

### Comparing `skale.py-6.0.dev3/skale.py.egg-info/SOURCES.txt` & `skale.py-6.0.dev4/skale.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/tests/schain_config/generator_test.py` & `skale.py-6.0.dev4/tests/schain_config/generator_test.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.0.dev3/tests/schain_config/ports_allocation_test.py` & `skale.py-6.0.dev4/tests/schain_config/ports_allocation_test.py`

 * *Files identical despite different names*

