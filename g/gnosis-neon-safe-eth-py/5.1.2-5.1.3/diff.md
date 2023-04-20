# Comparing `tmp/gnosis-neon-safe-eth-py-5.1.2.tar.gz` & `tmp/gnosis-neon-safe-eth-py-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnosis-neon-safe-eth-py-5.1.2.tar", last modified: Thu Apr 20 10:39:57 2023, max compression
+gzip compressed data, was "gnosis-neon-safe-eth-py-5.1.3.tar", last modified: Thu Apr 20 13:37:48 2023, max compression
```

## Comparing `gnosis-neon-safe-eth-py-5.1.2.tar` & `gnosis-neon-safe-eth-py-5.1.3.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.894083 gnosis-neon-safe-eth-py-5.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-20 10:39:57.894083 gnosis-neon-safe-eth-py-5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.866083 gnosis-neon-safe-eth-py-5.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.866083 gnosis-neon-safe-eth-py-5.1.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/source/gnosis.eth.clients.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/source/gnosis.eth.contracts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/source/gnosis.eth.django.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/source/gnosis.eth.eip712.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/source/gnosis.eth.oracles.abis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/source/gnosis.eth.oracles.rst
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/source/gnosis.eth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/source/gnosis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/source/gnosis.safe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.866083 gnosis-neon-safe-eth-py-5.1.2/gnosis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.866083 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.870083 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/clients/blockscout_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/clients/contract_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/clients/etherscan_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/clients/sourcify.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.878083 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)   328664 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/CPKFactory.json
--rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/DelegateConstructorProxy.json
--rw-r--r--   0 runner    (1001) docker     (123)    29068 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/ERC1155.json
--rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/ERC20.json
--rw-r--r--   0 runner    (1001) docker     (123)    89890 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/ERC20TestToken.json
--rw-r--r--   0 runner    (1001) docker     (123)   622260 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/ERC721.json
--rw-r--r--   0 runner    (1001) docker     (123)   983403 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
--rw-r--r--   0 runner    (1001) docker     (123)  1158944 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)  1347363 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/MultiSend.json
--rw-r--r--   0 runner    (1001) docker     (123)    78793 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/PayingProxy.json
--rw-r--r--   0 runner    (1001) docker     (123)   136946 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)   288861 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/Proxy_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/Proxy_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/Proxy_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/kyber_network_proxy.json
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/uniswap_exchange.json
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/uniswap_factory.json
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/uniswap_v2_factory.json
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/uniswap_v2_pair.json
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/uniswap_v2_router.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.878083 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.878083 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.878083 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/eip712/
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    81858 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/ethereum_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/ethereum_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/multicall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.882083 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.882083 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/aave_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/balancer_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    29731 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/cream_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/curve_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/makerdao.py
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/mooniswap_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/superfluid_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/yearn_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/zerion_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/cowswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.882083 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/helpers/curve_gauge_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/kyber.py
--rw-r--r--   0 runner    (1001) docker     (123)    32311 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/superfluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/sushiswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.886083 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.886083 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   107062 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/clients/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/clients/test_blockscout_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/clients/test_etherscan_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/clients/test_sourcify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.886083 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/eip712/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/eip712/test_eip712.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/ethereum_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.886083 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/mocks/mock_internal_txs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/mocks/mock_log_receipts.py
--rw-r--r--   0 runner    (1001) docker     (123)   753187 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/mocks/mock_trace_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    92731 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/mocks/mock_trace_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)   169556 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/mocks/mock_trace_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.886083 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/oracles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/oracles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/oracles/test_cowswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/oracles/test_kyber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/oracles/test_superfluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/oracles/test_sushiswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/oracles/test_uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    71326 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/test_ethereum_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/test_multicall.py
--rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/test_oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.890083 gnosis-neon-safe-eth-py-5.1.2/gnosis/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/protocol/gnosis_protocol_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/protocol/order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.890083 gnosis-neon-safe-eth-py-5.1.2/gnosis/protocol/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/protocol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/protocol/tests/test_gnosis_protocol_api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.890083 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21902 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.890083 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/api/base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/api/relay_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/api/transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/multi_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/proxy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    42010 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/safe_create2_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/safe_creation_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/safe_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/safe_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/signatures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.894083 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.894083 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/api/test_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/safe_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_multi_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_proxy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    32576 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_safe_create2_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_safe_creation_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_safe_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_safe_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.894083 gnosis-neon-safe-eth-py-5.1.2/gnosis/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:39:57.894083 gnosis-neon-safe-eth-py-5.1.2/gnosis_neon_safe_eth_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-20 10:39:57.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis_neon_safe_eth_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-20 10:39:57.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis_neon_safe_eth_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:39:57.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis_neon_safe_eth_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-20 10:39:57.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis_neon_safe_eth_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 10:39:57.000000 gnosis-neon-safe-eth-py-5.1.2/gnosis_neon_safe_eth_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-20 10:39:57.894083 gnosis-neon-safe-eth-py-5.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 10:39:41.000000 gnosis-neon-safe-eth-py-5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.157707 gnosis-neon-safe-eth-py-5.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-20 13:37:48.157707 gnosis-neon-safe-eth-py-5.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.117707 gnosis-neon-safe-eth-py-5.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.121707 gnosis-neon-safe-eth-py-5.1.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/source/gnosis.eth.clients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/source/gnosis.eth.contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/source/gnosis.eth.django.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/source/gnosis.eth.eip712.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/source/gnosis.eth.oracles.abis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/source/gnosis.eth.oracles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/source/gnosis.eth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/source/gnosis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/source/gnosis.safe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/docs/source/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.121707 gnosis-neon-safe-eth-py-5.1.3/gnosis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.125707 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.125707 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/clients/blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/clients/contract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/clients/etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/clients/sourcify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.141707 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)   328664 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/CPKFactory.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/DelegateConstructorProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29068 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/ERC1155.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/ERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)    89890 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/ERC20TestToken.json
+-rw-r--r--   0 runner    (1001) docker     (123)   622260 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/ERC721.json
+-rw-r--r--   0 runner    (1001) docker     (123)   983403 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1158944 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1347363 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/MultiSend.json
+-rw-r--r--   0 runner    (1001) docker     (123)    78793 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/PayingProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)   136946 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)   288861 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/Proxy_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/Proxy_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/Proxy_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/kyber_network_proxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/uniswap_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/uniswap_factory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/uniswap_v2_factory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/uniswap_v2_pair.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/uniswap_v2_router.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.141707 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.145707 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.145707 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/eip712/
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81858 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/ethereum_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/multicall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.145707 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.145707 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/aave_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/balancer_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29731 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/cream_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/curve_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/makerdao.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/mooniswap_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/superfluid_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/yearn_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/zerion_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.145707 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/helpers/curve_gauge_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/kyber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32311 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.149707 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.149707 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107062 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/clients/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/clients/test_blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/clients/test_etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/clients/test_sourcify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.149707 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/eip712/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/eip712/test_eip712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/ethereum_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.149707 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/mocks/mock_internal_txs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/mocks/mock_log_receipts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   753187 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/mocks/mock_trace_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92731 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/mocks/mock_trace_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169556 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/mocks/mock_trace_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.153707 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/oracles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/oracles/test_cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/oracles/test_kyber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/oracles/test_superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/oracles/test_sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/oracles/test_uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71326 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/test_ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/test_multicall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/test_oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.153707 gnosis-neon-safe-eth-py-5.1.3/gnosis/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/protocol/gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/protocol/order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.153707 gnosis-neon-safe-eth-py-5.1.3/gnosis/protocol/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/protocol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/protocol/tests/test_gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.153707 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.153707 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/api/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/api/relay_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/api/transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42010 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/safe_creation_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.157707 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.157707 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/api/test_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/safe_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32576 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_safe_creation_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.157707 gnosis-neon-safe-eth-py-5.1.3/gnosis/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:48.157707 gnosis-neon-safe-eth-py-5.1.3/gnosis_neon_safe_eth_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-20 13:37:48.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis_neon_safe_eth_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-20 13:37:48.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis_neon_safe_eth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:37:48.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis_neon_safe_eth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-20 13:37:48.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis_neon_safe_eth_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 13:37:48.000000 gnosis-neon-safe-eth-py-5.1.3/gnosis_neon_safe_eth_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-20 13:37:48.157707 gnosis-neon-safe-eth-py-5.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 13:37:33.000000 gnosis-neon-safe-eth-py-5.1.3/setup.py
```

### Comparing `gnosis-neon-safe-eth-py-5.1.2/LICENSE` & `gnosis-neon-safe-eth-py-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/PKG-INFO` & `gnosis-neon-safe-eth-py-5.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnosis-neon-safe-eth-py
-Version: 5.1.2
+Version: 5.1.3
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `gnosis-neon-safe-eth-py-5.1.2/README.rst` & `gnosis-neon-safe-eth-py-5.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/docs/Makefile` & `gnosis-neon-safe-eth-py-5.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/docs/make.bat` & `gnosis-neon-safe-eth-py-5.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/docs/source/conf.py` & `gnosis-neon-safe-eth-py-5.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/docs/source/gnosis.eth.clients.rst` & `gnosis-neon-safe-eth-py-5.1.3/docs/source/gnosis.eth.clients.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/docs/source/gnosis.eth.django.rst` & `gnosis-neon-safe-eth-py-5.1.3/docs/source/gnosis.eth.django.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/docs/source/gnosis.eth.oracles.abis.rst` & `gnosis-neon-safe-eth-py-5.1.3/docs/source/gnosis.eth.oracles.abis.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/docs/source/gnosis.eth.rst` & `gnosis-neon-safe-eth-py-5.1.3/docs/source/gnosis.eth.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/docs/source/gnosis.safe.rst` & `gnosis-neon-safe-eth-py-5.1.3/docs/source/gnosis.safe.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/docs/source/index.rst` & `gnosis-neon-safe-eth-py-5.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/docs/source/quickstart.rst` & `gnosis-neon-safe-eth-py-5.1.3/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/__init__.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/__init__.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/clients/__init__.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/clients/blockscout_client.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/clients/blockscout_client.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/clients/etherscan_client.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/clients/etherscan_client.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/clients/sourcify.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/clients/sourcify.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/constants.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/constants.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/CPKFactory.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/CPKFactory.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/DelegateConstructorProxy.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/DelegateConstructorProxy.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/ERC1155.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/ERC1155.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/ERC20.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/ERC20.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/ERC20TestToken.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/ERC20TestToken.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/ERC721.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/ERC721.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/GnosisSafe_V0_0_1.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/GnosisSafe_V0_0_1.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/GnosisSafe_V1_0_0.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/GnosisSafe_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/GnosisSafe_V1_1_1.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/GnosisSafe_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/GnosisSafe_V1_3_0.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/GnosisSafe_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/MultiSend.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/MultiSend.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/PayingProxy.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/PayingProxy.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/ProxyFactory_V1_0_0.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/ProxyFactory_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/ProxyFactory_V1_1_1.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/ProxyFactory_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/ProxyFactory_V1_3_0.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/ProxyFactory_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/Proxy_V1_0_0.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/Proxy_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/Proxy_V1_1_1.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/Proxy_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/Proxy_V1_3_0.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/Proxy_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/__init__.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/kyber_network_proxy.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/kyber_network_proxy.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/uniswap_exchange.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/uniswap_exchange.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/uniswap_factory.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/uniswap_factory.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/uniswap_v2_factory.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/uniswap_v2_factory.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/uniswap_v2_pair.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/uniswap_v2_pair.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/contracts/uniswap_v2_router.json` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/contracts/uniswap_v2_router.json`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/admin.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/admin.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/forms.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/forms.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/models.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/models.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/serializers.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/serializers.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/tests/models.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/tests/test_forms.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/tests/test_models.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/django/tests/test_serializers.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/django/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/eip712/__init__.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/eip712/__init__.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/ethereum_client.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/ethereum_client.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/ethereum_network.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/ethereum_network.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/exceptions.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/multicall.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/multicall.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/__init__.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/__init__.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/aave_abis.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/aave_abis.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/balancer_abis.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/balancer_abis.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/cream_abis.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/cream_abis.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/curve_abis.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/curve_abis.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/makerdao.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/makerdao.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/mooniswap_abis.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/mooniswap_abis.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/uniswap_v3.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/yearn_abis.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/yearn_abis.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/abis/zerion_abis.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/abis/zerion_abis.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/cowswap.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/cowswap.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/helpers/curve_gauge_list.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/helpers/curve_gauge_list.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/kyber.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/kyber.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/oracles.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/oracles.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/superfluid.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/superfluid.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/sushiswap.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/sushiswap.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/uniswap_v3.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/oracles/utils.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/oracles/utils.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/clients/mocks.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/clients/mocks.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/clients/test_blockscout_client.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/clients/test_blockscout_client.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/clients/test_etherscan_client.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/clients/test_etherscan_client.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/clients/test_sourcify.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/clients/test_sourcify.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/eip712/test_eip712.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/eip712/test_eip712.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/ethereum_test_case.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/ethereum_test_case.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/mocks/mock_internal_txs.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/mocks/mock_internal_txs.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/mocks/mock_log_receipts.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/mocks/mock_log_receipts.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/mocks/mock_trace_block.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/mocks/mock_trace_block.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/mocks/mock_trace_filter.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/mocks/mock_trace_filter.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/mocks/mock_trace_transaction.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/mocks/mock_trace_transaction.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/oracles/test_cowswap.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/oracles/test_cowswap.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/oracles/test_kyber.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/oracles/test_kyber.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/oracles/test_superfluid.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/oracles/test_superfluid.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/oracles/test_sushiswap.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/oracles/test_sushiswap.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/oracles/test_uniswap_v3.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/oracles/test_uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/test_ethereum_client.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/test_ethereum_client.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/test_multicall.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/test_multicall.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/test_oracles.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/test_oracles.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/test_utils.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/tests/utils.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/eth/utils.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/eth/utils.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/protocol/gnosis_protocol_api.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/protocol/gnosis_protocol_api.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/protocol/order.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/protocol/order.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/protocol/tests/test_gnosis_protocol_api.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/protocol/tests/test_gnosis_protocol_api.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/__init__.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/__init__.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/addresses.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/addresses.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,20 +259,20 @@
     EthereumNetwork.KAVA_EVM: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 2116303, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 2116307, "1.3.0"),
     ],
     EthereumNetwork.NEON_EVM_DEVNET: [
         (
             "0x69f4D1788e39c87893C980c06EdF4b7f686e2938",
-            12504268,
+            205147021,
             "1.3.0+L2",
         ),  # need to change block number
         (
             "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
-            12504268,
+            205147000,
             "1.3.0",
         ),  # need to change block number
     ],
 }
 
 PROXY_FACTORIES: Dict[EthereumNetwork, List[Tuple[str, int]]] = {
     EthereumNetwork.MAINNET: [
@@ -461,11 +461,11 @@
     ],
     EthereumNetwork.KAVA_EVM: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 2116356),  # v1.3.0
     ],
     EthereumNetwork.NEON_EVM_DEVNET: [
         (
             "0xc22834581ebc8527d974f8a1c97e1bea4ef910bc",
-            205634872,
+            205146874,
         ),  # v1.3.0. need to change block number
     ],
 }
```

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/api/base_api.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/api/base_api.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/api/relay_service_api.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/api/relay_service_api.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/api/transaction_service_api.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/api/transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/exceptions.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/exceptions.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/multi_send.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/multi_send.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/proxy_factory.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/safe.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/safe.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/safe_create2_tx.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/safe_creation_tx.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/safe_creation_tx.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/safe_signature.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/safe_signature.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/safe_tx.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/safe_tx.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/serializers.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/serializers.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/signatures.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/signatures.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/api/test_transaction_service_api.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/api/test_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/safe_test_case.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/safe_test_case.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_multi_send.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_multi_send.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_proxy_factory.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_safe.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_safe.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_safe_create2_tx.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_safe_creation_tx.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_safe_creation_tx.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_safe_signature.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_safe_signature.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_safe_tx.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_safe_tx.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_serializers.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/test_signatures.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis/safe/tests/utils.py` & `gnosis-neon-safe-eth-py-5.1.3/gnosis/safe/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis_neon_safe_eth_py.egg-info/PKG-INFO` & `gnosis-neon-safe-eth-py-5.1.3/gnosis_neon_safe_eth_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnosis-neon-safe-eth-py
-Version: 5.1.2
+Version: 5.1.3
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `gnosis-neon-safe-eth-py-5.1.2/gnosis_neon_safe_eth_py.egg-info/SOURCES.txt` & `gnosis-neon-safe-eth-py-5.1.3/gnosis_neon_safe_eth_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnosis-neon-safe-eth-py-5.1.2/setup.cfg` & `gnosis-neon-safe-eth-py-5.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gnosis-neon-safe-eth-py
-version = 5.1.2
+version = 5.1.3
 description = Safe Ecosystem Foundation utilities for Ethereum projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 keywords = 
 	ethereum
 	web3
 	django
```

