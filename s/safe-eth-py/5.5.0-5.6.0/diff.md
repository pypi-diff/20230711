# Comparing `tmp/safe-eth-py-5.5.0.tar.gz` & `tmp/safe-eth-py-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe-eth-py-5.5.0.tar", last modified: Thu Jun 22 15:02:46 2023, max compression
+gzip compressed data, was "safe-eth-py-5.6.0.tar", last modified: Tue Jul 11 11:06:00 2023, max compression
```

## Comparing `safe-eth-py-5.5.0.tar` & `safe-eth-py-5.6.0.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.551445 safe-eth-py-5.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-22 15:02:46.551445 safe-eth-py-5.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.507445 safe-eth-py-5.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.511445 safe-eth-py-5.5.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.eth.clients.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.eth.contracts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.eth.django.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.eth.eip712.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.eth.oracles.abis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.eth.oracles.rst
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.eth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.safe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.511445 safe-eth-py-5.5.0/gnosis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.511445 safe-eth-py-5.5.0/gnosis/eth/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.515445 safe-eth-py-5.5.0/gnosis/eth/abis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/abis/multicall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.515445 safe-eth-py-5.5.0/gnosis/eth/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/clients/blockscout_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/clients/contract_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/clients/etherscan_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/clients/sourcify.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.527445 safe-eth-py-5.5.0/gnosis/eth/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)   328664 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/CPKFactory.json
--rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/DelegateConstructorProxy.json
--rw-r--r--   0 runner    (1001) docker     (123)    29068 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/ERC1155.json
--rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/ERC20.json
--rw-r--r--   0 runner    (1001) docker     (123)    89890 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/ERC20TestToken.json
--rw-r--r--   0 runner    (1001) docker     (123)   622260 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/ERC721.json
--rw-r--r--   0 runner    (1001) docker     (123)   983403 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
--rw-r--r--   0 runner    (1001) docker     (123)  1158944 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)  1347363 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/MultiSend.json
--rw-r--r--   0 runner    (1001) docker     (123)    78793 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/PayingProxy.json
--rw-r--r--   0 runner    (1001) docker     (123)   136946 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)   288861 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/Proxy_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/Proxy_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/Proxy_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/kyber_network_proxy.json
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_exchange.json
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_factory.json
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_v2_factory.json
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_v2_pair.json
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_v2_router.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.527445 safe-eth-py-5.5.0/gnosis/eth/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.527445 safe-eth-py-5.5.0/gnosis/eth/django/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.527445 safe-eth-py-5.5.0/gnosis/eth/eip712/
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77429 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/ethereum_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20891 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/ethereum_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/multicall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.531445 safe-eth-py-5.5.0/gnosis/eth/oracles/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.531445 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/aave_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/balancer_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    29731 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/cream_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/curve_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/mooniswap_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/superfluid_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/yearn_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/zerion_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/cowswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.535445 safe-eth-py-5.5.0/gnosis/eth/oracles/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/helpers/curve_gauge_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/kyber.py
--rw-r--r--   0 runner    (1001) docker     (123)    32229 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/superfluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/sushiswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.535445 safe-eth-py-5.5.0/gnosis/eth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.535445 safe-eth-py-5.5.0/gnosis/eth/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   107062 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/clients/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/clients/test_blockscout_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/clients/test_etherscan_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/clients/test_sourcify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.535445 safe-eth-py-5.5.0/gnosis/eth/tests/eip712/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/eip712/test_eip712.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/ethereum_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.539445 safe-eth-py-5.5.0/gnosis/eth/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_internal_txs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_log_receipts.py
--rw-r--r--   0 runner    (1001) docker     (123)   793149 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_trace_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    92795 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_trace_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)   171076 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_trace_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.539445 safe-eth-py-5.5.0/gnosis/eth/tests/oracles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/oracles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_cowswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_kyber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_superfluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_sushiswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    61046 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/test_ethereum_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/test_multicall.py
--rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/test_oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.539445 safe-eth-py-5.5.0/gnosis/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/protocol/gnosis_protocol_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/protocol/order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.543445 safe-eth-py-5.5.0/gnosis/protocol/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/protocol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/protocol/tests/test_gnosis_protocol_api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.543445 safe-eth-py-5.5.0/gnosis/safe/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32683 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.547445 safe-eth-py-5.5.0/gnosis/safe/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/api/base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/api/relay_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/api/transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/multi_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/proxy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    42768 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/safe_create2_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/safe_creation_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/safe_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/safe_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/signatures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.547445 safe-eth-py-5.5.0/gnosis/safe/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.547445 safe-eth-py-5.5.0/gnosis/safe/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/api/test_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/safe_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_multi_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_proxy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    34197 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_create2_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_creation_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.547445 safe-eth-py-5.5.0/gnosis/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.551445 safe-eth-py-5.5.0/safe_eth_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-22 15:02:46.000000 safe-eth-py-5.5.0/safe_eth_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-22 15:02:46.000000 safe-eth-py-5.5.0/safe_eth_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:02:46.000000 safe-eth-py-5.5.0/safe_eth_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-22 15:02:46.000000 safe-eth-py-5.5.0/safe_eth_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 15:02:46.000000 safe-eth-py-5.5.0/safe_eth_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-22 15:02:46.551445 safe-eth-py-5.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.099037 safe-eth-py-5.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-11 11:06:00.103037 safe-eth-py-5.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.055036 safe-eth-py-5.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.059036 safe-eth-py-5.6.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/source/gnosis.eth.clients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/source/gnosis.eth.contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/source/gnosis.eth.django.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/source/gnosis.eth.eip712.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/source/gnosis.eth.oracles.abis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/source/gnosis.eth.oracles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/source/gnosis.eth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/source/gnosis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/source/gnosis.safe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/docs/source/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.059036 safe-eth-py-5.6.0/gnosis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.063036 safe-eth-py-5.6.0/gnosis/eth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.063036 safe-eth-py-5.6.0/gnosis/eth/abis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/abis/multicall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.063036 safe-eth-py-5.6.0/gnosis/eth/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/clients/blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/clients/contract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/clients/etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/clients/sourcify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.075036 safe-eth-py-5.6.0/gnosis/eth/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)   328664 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/CPKFactory.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/DelegateConstructorProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29068 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/ERC1155.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/ERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)    89890 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/ERC20TestToken.json
+-rw-r--r--   0 runner    (1001) docker     (123)   622260 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/ERC721.json
+-rw-r--r--   0 runner    (1001) docker     (123)   983403 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1158944 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1347363 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/MultiSend.json
+-rw-r--r--   0 runner    (1001) docker     (123)    78793 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/PayingProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)   136946 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)   288861 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/Proxy_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/Proxy_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/Proxy_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/kyber_network_proxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/uniswap_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/uniswap_factory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/uniswap_v2_factory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/uniswap_v2_pair.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/contracts/uniswap_v2_router.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.079037 safe-eth-py-5.6.0/gnosis/eth/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/django/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/django/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.079037 safe-eth-py-5.6.0/gnosis/eth/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/django/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/django/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/django/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/django/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/django/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.079037 safe-eth-py-5.6.0/gnosis/eth/eip712/
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77429 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20968 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/ethereum_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/multicall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.083037 safe-eth-py-5.6.0/gnosis/eth/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.083037 safe-eth-py-5.6.0/gnosis/eth/oracles/abis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/abis/aave_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/abis/balancer_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29731 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/abis/cream_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/abis/curve_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/abis/mooniswap_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/abis/superfluid_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/abis/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/abis/yearn_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/abis/zerion_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.083037 safe-eth-py-5.6.0/gnosis/eth/oracles/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/helpers/curve_gauge_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/kyber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32229 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/oracles/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.087036 safe-eth-py-5.6.0/gnosis/eth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.087036 safe-eth-py-5.6.0/gnosis/eth/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107062 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/clients/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/clients/test_blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/clients/test_etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/clients/test_sourcify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.087036 safe-eth-py-5.6.0/gnosis/eth/tests/eip712/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/eip712/test_eip712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/ethereum_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.091037 safe-eth-py-5.6.0/gnosis/eth/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/mocks/mock_internal_txs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/mocks/mock_log_receipts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   793149 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/mocks/mock_trace_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92795 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/mocks/mock_trace_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171076 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/mocks/mock_trace_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.091037 safe-eth-py-5.6.0/gnosis/eth/tests/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/oracles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/oracles/test_cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/oracles/test_kyber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/oracles/test_superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/oracles/test_sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/oracles/test_uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61046 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/test_ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/test_multicall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/test_oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/eth/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.091037 safe-eth-py-5.6.0/gnosis/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/protocol/gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/protocol/order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.091037 safe-eth-py-5.6.0/gnosis/protocol/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/protocol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/protocol/tests/test_gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.095037 safe-eth-py-5.6.0/gnosis/safe/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35479 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.095037 safe-eth-py-5.6.0/gnosis/safe/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/api/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/api/relay_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/api/transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42768 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/safe_creation_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.099037 safe-eth-py-5.6.0/gnosis/safe/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.099037 safe-eth-py-5.6.0/gnosis/safe/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/api/test_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/safe_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/test_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/test_multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/test_proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34197 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/test_safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/test_safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/test_safe_creation_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/test_safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/test_safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/test_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/safe/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.099037 safe-eth-py-5.6.0/gnosis/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/gnosis/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:00.099037 safe-eth-py-5.6.0/safe_eth_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-11 11:06:00.000000 safe-eth-py-5.6.0/safe_eth_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-11 11:06:00.000000 safe-eth-py-5.6.0/safe_eth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:06:00.000000 safe-eth-py-5.6.0/safe_eth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-11 11:06:00.000000 safe-eth-py-5.6.0/safe_eth_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 11:06:00.000000 safe-eth-py-5.6.0/safe_eth_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-11 11:06:00.103037 safe-eth-py-5.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 11:05:43.000000 safe-eth-py-5.6.0/setup.py
```

### Comparing `safe-eth-py-5.5.0/LICENSE` & `safe-eth-py-5.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/PKG-INFO` & `safe-eth-py-5.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-eth-py
-Version: 5.5.0
+Version: 5.6.0
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `safe-eth-py-5.5.0/README.rst` & `safe-eth-py-5.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/docs/Makefile` & `safe-eth-py-5.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/docs/make.bat` & `safe-eth-py-5.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/docs/source/conf.py` & `safe-eth-py-5.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/docs/source/gnosis.eth.clients.rst` & `safe-eth-py-5.6.0/docs/source/gnosis.eth.clients.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/docs/source/gnosis.eth.django.rst` & `safe-eth-py-5.6.0/docs/source/gnosis.eth.django.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/docs/source/gnosis.eth.oracles.abis.rst` & `safe-eth-py-5.6.0/docs/source/gnosis.eth.oracles.abis.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/docs/source/gnosis.eth.rst` & `safe-eth-py-5.6.0/docs/source/gnosis.eth.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/docs/source/gnosis.safe.rst` & `safe-eth-py-5.6.0/docs/source/gnosis.safe.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/docs/source/index.rst` & `safe-eth-py-5.6.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/docs/source/quickstart.rst` & `safe-eth-py-5.6.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/__init__.py` & `safe-eth-py-5.6.0/gnosis/eth/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/abis/multicall.py` & `safe-eth-py-5.6.0/gnosis/eth/abis/multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/clients/__init__.py` & `safe-eth-py-5.6.0/gnosis/eth/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/clients/blockscout_client.py` & `safe-eth-py-5.6.0/gnosis/eth/clients/blockscout_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class BlockScoutConfigurationProblem(BlockscoutClientException):
     pass
 
 
 class BlockscoutClient:
     NETWORK_WITH_URL = {
-        EthereumNetwork.GNOSIS: "https://blockscout.com/poa/xdai/",
+        EthereumNetwork.GNOSIS: "https://gnosis.blockscout.com/graphiql",
         EthereumNetwork.POLYGON: "https://polygon-explorer-mainnet.chainstacklabs.com/",
         EthereumNetwork.MUMBAI: "https://polygon-explorer-mumbai.chainstacklabs.com/",
         EthereumNetwork.ENERGY_WEB_CHAIN: "https://explorer.energyweb.org/",
         EthereumNetwork.ENERGY_WEB_VOLTA_TESTNET: "https://volta-explorer.energyweb.org/",
         EthereumNetwork.POLIS_MAINNET: "https://explorer.polis.tech",
         EthereumNetwork.BOBABEAM: "https://blockexplorer.bobabeam.boba.network/",
         EthereumNetwork.BOBA_NETWORK_RINKEBY_TESTNET: "https://blockexplorer.rinkeby.boba.network/",
```

### Comparing `safe-eth-py-5.5.0/gnosis/eth/clients/etherscan_client.py` & `safe-eth-py-5.6.0/gnosis/eth/clients/etherscan_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         EthereumNetwork.POLYGON: "https://polygonscan.com",
         EthereumNetwork.POLYGON_ZKEVM: "https://zkevm.polygonscan.com",
         EthereumNetwork.OPTIMISM: "https://optimistic.etherscan.io",
         EthereumNetwork.ARBITRUM_ONE: "https://arbiscan.io",
         EthereumNetwork.ARBITRUM_NOVA: "https://nova.arbiscan.io",
         EthereumNetwork.ARBITRUM_GOERLI: "https://goerli.arbiscan.io",
         EthereumNetwork.AVALANCHE_C_CHAIN: "https://snowtrace.io",
+        EthereumNetwork.GNOSIS: "https://gnosisscan.io",
         EthereumNetwork.MOONBEAM: "https://moonscan.io",
         EthereumNetwork.MOONRIVER: "https://moonriver.moonscan.io",
         EthereumNetwork.MOONBASE_ALPHA: "https://moonbase.moonscan.io",
         EthereumNetwork.CRONOS_MAINNET_BETA: "https://cronoscan.com",
         EthereumNetwork.CRONOS_TESTNET: "https://testnet.cronoscan.com",
         EthereumNetwork.CELO_MAINNET: "https://celoscan.io",
         EthereumNetwork.BASE_GOERLI_TESTNET: "https://goerli.basescan.org",
@@ -57,14 +58,15 @@
         EthereumNetwork.POLYGON: "https://api.polygonscan.com",
         EthereumNetwork.POLYGON_ZKEVM: "https://api-zkevm.polygonscan.com",
         EthereumNetwork.OPTIMISM: "https://api-optimistic.etherscan.io",
         EthereumNetwork.ARBITRUM_ONE: "https://api.arbiscan.io",
         EthereumNetwork.ARBITRUM_NOVA: "https://api-nova.arbiscan.io",
         EthereumNetwork.ARBITRUM_GOERLI: "https://api-goerli.arbiscan.io",
         EthereumNetwork.AVALANCHE_C_CHAIN: "https://api.snowtrace.io",
+        EthereumNetwork.GNOSIS: "https://api.gnosisscan.io",
         EthereumNetwork.MOONBEAM: "https://api-moonbeam.moonscan.io",
         EthereumNetwork.MOONRIVER: "https://api-moonriver.moonscan.io",
         EthereumNetwork.MOONBASE_ALPHA: "https://api-moonbase.moonscan.io",
         EthereumNetwork.CRONOS_MAINNET_BETA: "https://api.cronoscan.com",
         EthereumNetwork.CRONOS_TESTNET: "https://api-testnet.cronoscan.com",
         EthereumNetwork.CELO_MAINNET: "https://api.celoscan.io",
         EthereumNetwork.BASE_GOERLI_TESTNET: "https://api-goerli.basescan.org",
```

### Comparing `safe-eth-py-5.5.0/gnosis/eth/clients/sourcify.py` & `safe-eth-py-5.6.0/gnosis/eth/clients/sourcify.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/constants.py` & `safe-eth-py-5.6.0/gnosis/eth/constants.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/CPKFactory.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/CPKFactory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/DelegateConstructorProxy.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/DelegateConstructorProxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/ERC1155.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/ERC1155.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/ERC20.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/ERC20.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/ERC20TestToken.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/ERC20TestToken.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/ERC721.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/ERC721.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V0_0_1.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/GnosisSafe_V0_0_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V1_0_0.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/GnosisSafe_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V1_1_1.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/GnosisSafe_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V1_3_0.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/GnosisSafe_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/MultiSend.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/MultiSend.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/PayingProxy.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/PayingProxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/ProxyFactory_V1_0_0.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/ProxyFactory_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/ProxyFactory_V1_1_1.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/ProxyFactory_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/ProxyFactory_V1_3_0.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/ProxyFactory_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/Proxy_V1_0_0.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/Proxy_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/Proxy_V1_1_1.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/Proxy_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/Proxy_V1_3_0.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/Proxy_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/__init__.py` & `safe-eth-py-5.6.0/gnosis/eth/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/kyber_network_proxy.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/kyber_network_proxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_exchange.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/uniswap_exchange.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_factory.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/uniswap_factory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_v2_factory.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/uniswap_v2_factory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_v2_pair.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/uniswap_v2_pair.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_v2_router.json` & `safe-eth-py-5.6.0/gnosis/eth/contracts/uniswap_v2_router.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/django/admin.py` & `safe-eth-py-5.6.0/gnosis/eth/django/admin.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/django/forms.py` & `safe-eth-py-5.6.0/gnosis/eth/django/forms.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/django/models.py` & `safe-eth-py-5.6.0/gnosis/eth/django/models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/django/serializers.py` & `safe-eth-py-5.6.0/gnosis/eth/django/serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/django/tests/models.py` & `safe-eth-py-5.6.0/gnosis/eth/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/django/tests/test_forms.py` & `safe-eth-py-5.6.0/gnosis/eth/django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/django/tests/test_models.py` & `safe-eth-py-5.6.0/gnosis/eth/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/django/tests/test_serializers.py` & `safe-eth-py-5.6.0/gnosis/eth/django/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/eip712/__init__.py` & `safe-eth-py-5.6.0/gnosis/eth/eip712/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/ethereum_client.py` & `safe-eth-py-5.6.0/gnosis/eth/ethereum_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/ethereum_network.py` & `safe-eth-py-5.6.0/gnosis/eth/ethereum_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -555,14 +555,15 @@
     GTON_TESTNET = 50021
     SARDIS_MAINNET = 51712
     DFK_CHAIN = 53935
     HAQQ_CHAIN_TESTNET = 54211
     REI_CHAIN_MAINNET = 55555
     REI_CHAIN_TESTNET = 55556
     BOBA_BNB_MAINNET = 56288
+    LINEA_TESTNET = 59140
     THINKIUM_TESTNET_CHAIN_0 = 60000
     THINKIUM_TESTNET_CHAIN_1 = 60001
     THINKIUM_TESTNET_CHAIN_2 = 60002
     THINKIUM_TESTNET_CHAIN_103 = 60103
     ETICA_MAINNET = 61803
     DOKEN_SUPER_CHAIN_MAINNET = 61916
     CELO_BAKLAVA_TESTNET = 62320
@@ -581,14 +582,15 @@
     ENERGY_WEB_VOLTA_TESTNET = 73799
     MIXIN_VIRTUAL_MACHINE = 73927
     RESINCOIN_MAINNET = 75000
     VENTION_SMART_CHAIN_MAINNET = 77612
     FIRENZE_TEST_NETWORK = 78110
     GOLD_SMART_CHAIN_TESTNET = 79879
     MUMBAI = 80001
+    BASE_MAINNET = 8453
     BASE_GOERLI_TESTNET = 84531
     IVAR_CHAIN_MAINNET = 88888
     BEVERLY_HILLS = 90210
     LAMBDA_TESTNET = 92001
     BOBA_BNB_MAINNET_OLD = 97288
     UB_SMART_CHAIN_TESTNET = 99998
     UB_SMART_CHAIN = 99999
@@ -671,14 +673,15 @@
     PLATON_DEV_TESTNET2 = 2206132
     FILECOIN_BUTTERFLY_TESTNET = 3141592
     IMVERSED_MAINNET = 5555555
     IMVERSED_TESTNET = 5555558
     OPENVESSEL = 7355310
     QL1_TESTNET = 7668378
     MUSICOIN = 7762959
+    ZORA_NETWORK = 7777777
     PLIAN_MAINNET_SUBCHAIN_1 = 8007736
     PLIAN_TESTNET_SUBCHAIN_1 = 10067275
     SOVERUN_MAINNET = 10101010
     SEPOLIA = 11155111
     PEPCHAIN_CHURCHILL = 13371337
     ANDUSCHAIN_MAINNET = 14288640
     PLIAN_TESTNET_MAIN = 16658437
```

### Comparing `safe-eth-py-5.5.0/gnosis/eth/exceptions.py` & `safe-eth-py-5.6.0/gnosis/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/multicall.py` & `safe-eth-py-5.6.0/gnosis/eth/multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/__init__.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/aave_abis.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/abis/aave_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/balancer_abis.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/abis/balancer_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/cream_abis.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/abis/cream_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/curve_abis.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/abis/curve_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/mooniswap_abis.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/abis/mooniswap_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/uniswap_v3.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/abis/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/yearn_abis.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/abis/yearn_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/zerion_abis.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/abis/zerion_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/cowswap.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/cowswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/helpers/curve_gauge_list.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/helpers/curve_gauge_list.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/kyber.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/kyber.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/oracles.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/oracles.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/superfluid.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/superfluid.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/sushiswap.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/sushiswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/uniswap_v3.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/oracles/utils.py` & `safe-eth-py-5.6.0/gnosis/eth/oracles/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/clients/mocks.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/clients/mocks.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/clients/test_blockscout_client.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/clients/test_blockscout_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/clients/test_etherscan_client.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/clients/test_etherscan_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/clients/test_sourcify.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/clients/test_sourcify.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/eip712/test_eip712.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/eip712/test_eip712.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/ethereum_test_case.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/ethereum_test_case.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_internal_txs.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/mocks/mock_internal_txs.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_log_receipts.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/mocks/mock_log_receipts.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_trace_block.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/mocks/mock_trace_block.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_trace_filter.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/mocks/mock_trace_filter.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_trace_transaction.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/mocks/mock_trace_transaction.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_cowswap.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/oracles/test_cowswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_kyber.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/oracles/test_kyber.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_superfluid.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/oracles/test_superfluid.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_sushiswap.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/oracles/test_sushiswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_uniswap_v3.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/oracles/test_uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/test_ethereum_client.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/test_ethereum_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/test_multicall.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/test_multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/test_oracles.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/test_oracles.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/test_utils.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/tests/utils.py` & `safe-eth-py-5.6.0/gnosis/eth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/eth/utils.py` & `safe-eth-py-5.6.0/gnosis/eth/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/protocol/gnosis_protocol_api.py` & `safe-eth-py-5.6.0/gnosis/protocol/gnosis_protocol_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/protocol/order.py` & `safe-eth-py-5.6.0/gnosis/protocol/order.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/protocol/tests/test_gnosis_protocol_api.py` & `safe-eth-py-5.6.0/gnosis/protocol/tests/test_gnosis_protocol_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/__init__.py` & `safe-eth-py-5.6.0/gnosis/safe/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/addresses.py` & `safe-eth-py-5.6.0/gnosis/safe/addresses.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,14 +373,18 @@
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 53901616, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 53901624, "1.3.0"),
     ],
     EthereumNetwork.XDC_APOTHEM_NETWORK: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 42293309, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 42293315, "1.3.0"),
     ],
+    EthereumNetwork.BASE_MAINNET: [
+        ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 595207, "1.3.0+L2"),
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 595211, "1.3.0"),
+    ],
     EthereumNetwork.BASE_GOERLI_TESTNET: [
         ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 938848, "1.3.0+L2"),
         ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 939064, "1.3.0"),
     ],
     EthereumNetwork.KAVA_EVM: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 2116303, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 2116307, "1.3.0"),
@@ -468,14 +472,52 @@
         ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 885391, "1.3.0+L2"),
         ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 885392, "1.3.0"),
     ],
     EthereumNetwork.TENET: [
         ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 727470, "1.3.0+L2"),
         ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 727472, "1.3.0"),
     ],
+    EthereumNetwork.LINEA_TESTNET: [
+        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 363132, "1.3.0+L2"),
+        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 363135, "1.3.0"),
+    ],
+    EthereumNetwork.ASTAR: [
+        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 1106426, "1.3.0+L2"),
+        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 1106429, "1.3.0"),
+    ],
+    EthereumNetwork.SHIDEN: [
+        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 1634935, "1.3.0+L2"),
+        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 1634935, "1.3.0"),
+    ],
+    EthereumNetwork.DARWINIA_NETWORK: [
+        (
+            "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
+            491175,
+            "1.3.0+L2",
+        )
+    ],
+    EthereumNetwork.DARWINIA_CRAB_NETWORK: [
+        (
+            "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
+            739900,
+            "1.3.0+L2",
+        )
+    ],
+    EthereumNetwork.ZORA_NETWORK: [
+        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 11932, "1.3.0+L2"),
+        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 11934, "1.3.0"),
+    ],
+    EthereumNetwork.ZKSYNC_ALPHA_TESTNET: [
+        ("0x1727c2c531cf966f902E5927b98490fDFb3b2b70", 8619879, "1.3.0+L2"),
+        ("0xB00ce5CCcdEf57e539ddcEd01DF43a13855d9910", 8619884, "1.3.0"),
+    ],
+    EthereumNetwork.ZKSYNC_V2: [
+        ("0x1727c2c531cf966f902E5927b98490fDFb3b2b70", 7259224, "1.3.0+L2"),
+        ("0xB00ce5CCcdEf57e539ddcEd01DF43a13855d9910", 7259230, "1.3.0"),
+    ],
 }
 
 PROXY_FACTORIES: Dict[EthereumNetwork, List[Tuple[str, int]]] = {
     EthereumNetwork.MAINNET: [
         (
             "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
             14981216,
@@ -714,14 +756,17 @@
     ],
     EthereumNetwork.XINFIN_XDC_NETWORK: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 53901564),  # v1.3.0
     ],
     EthereumNetwork.XDC_APOTHEM_NETWORK: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 42293264),  # v1.3.0
     ],
+    EthereumNetwork.BASE_MAINNET: [
+        ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 595181),  # v1.3.0
+    ],
     EthereumNetwork.BASE_GOERLI_TESTNET: [
         ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 938696),  # v1.3.0
     ],
     EthereumNetwork.KAVA_EVM: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 2116356),  # v1.3.0
     ],
     EthereumNetwork.CROSSBELL: [
@@ -779,8 +824,38 @@
     ],
     EthereumNetwork.TENET_TESTNET: [
         ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 885379),  # v1.3.0
     ],
     EthereumNetwork.TENET: [
         ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 727457),  # v1.3.0
     ],
+    EthereumNetwork.LINEA_TESTNET: [
+        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 363118),  # v1.3.0
+    ],
+    EthereumNetwork.ASTAR: [
+        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 1106417),  # v1.3.0
+    ],
+    EthereumNetwork.SHIDEN: [
+        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 1634935),  # v1.3.0
+    ],
+    EthereumNetwork.DARWINIA_NETWORK: [
+        (
+            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
+            491157,
+        )
+    ],
+    EthereumNetwork.DARWINIA_CRAB_NETWORK: [
+        (
+            "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
+            739882,
+        )
+    ],
+    EthereumNetwork.ZORA_NETWORK: [
+        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 11914),  # v1.3.0
+    ],
+    EthereumNetwork.ZKSYNC_ALPHA_TESTNET: [
+        ("0xDAec33641865E4651fB43181C6DB6f7232Ee91c2", 8619849),  # v1.3.0
+    ],
+    EthereumNetwork.ZKSYNC_V2: [
+        ("0xDAec33641865E4651fB43181C6DB6f7232Ee91c2", 7259190),  # v1.3.0
+    ],
 }
```

### Comparing `safe-eth-py-5.5.0/gnosis/safe/api/base_api.py` & `safe-eth-py-5.6.0/gnosis/safe/api/base_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/api/relay_service_api.py` & `safe-eth-py-5.6.0/gnosis/safe/api/relay_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/api/transaction_service_api.py` & `safe-eth-py-5.6.0/gnosis/safe/api/transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/exceptions.py` & `safe-eth-py-5.6.0/gnosis/safe/exceptions.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/multi_send.py` & `safe-eth-py-5.6.0/gnosis/safe/multi_send.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/proxy_factory.py` & `safe-eth-py-5.6.0/gnosis/safe/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/safe.py` & `safe-eth-py-5.6.0/gnosis/safe/safe.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/safe_create2_tx.py` & `safe-eth-py-5.6.0/gnosis/safe/safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/safe_creation_tx.py` & `safe-eth-py-5.6.0/gnosis/safe/safe_creation_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/safe_signature.py` & `safe-eth-py-5.6.0/gnosis/safe/safe_signature.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/safe_tx.py` & `safe-eth-py-5.6.0/gnosis/safe/safe_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/serializers.py` & `safe-eth-py-5.6.0/gnosis/safe/serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/signatures.py` & `safe-eth-py-5.6.0/gnosis/safe/signatures.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/tests/api/test_transaction_service_api.py` & `safe-eth-py-5.6.0/gnosis/safe/tests/api/test_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/tests/safe_test_case.py` & `safe-eth-py-5.6.0/gnosis/safe/tests/safe_test_case.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/tests/test_addresses.py` & `safe-eth-py-5.6.0/gnosis/safe/tests/test_addresses.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/tests/test_multi_send.py` & `safe-eth-py-5.6.0/gnosis/safe/tests/test_multi_send.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/tests/test_proxy_factory.py` & `safe-eth-py-5.6.0/gnosis/safe/tests/test_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/tests/test_safe.py` & `safe-eth-py-5.6.0/gnosis/safe/tests/test_safe.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_create2_tx.py` & `safe-eth-py-5.6.0/gnosis/safe/tests/test_safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_creation_tx.py` & `safe-eth-py-5.6.0/gnosis/safe/tests/test_safe_creation_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_signature.py` & `safe-eth-py-5.6.0/gnosis/safe/tests/test_safe_signature.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_tx.py` & `safe-eth-py-5.6.0/gnosis/safe/tests/test_safe_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/tests/test_serializers.py` & `safe-eth-py-5.6.0/gnosis/safe/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/tests/test_signatures.py` & `safe-eth-py-5.6.0/gnosis/safe/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/gnosis/safe/tests/utils.py` & `safe-eth-py-5.6.0/gnosis/safe/tests/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/safe_eth_py.egg-info/PKG-INFO` & `safe-eth-py-5.6.0/safe_eth_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-eth-py
-Version: 5.5.0
+Version: 5.6.0
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `safe-eth-py-5.5.0/safe_eth_py.egg-info/SOURCES.txt` & `safe-eth-py-5.6.0/safe_eth_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.5.0/setup.cfg` & `safe-eth-py-5.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = safe-eth-py
-version = 5.5.0
+version = 5.6.0
 description = Safe Ecosystem Foundation utilities for Ethereum projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 keywords = 
 	ethereum
 	web3
 	django
```

