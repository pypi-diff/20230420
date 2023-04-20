# Comparing `tmp/conflux-web3-1.0.2.tar.gz` & `tmp/conflux-web3-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conflux-web3-1.0.2.tar", last modified: Tue Feb 28 09:06:52 2023, max compression
+gzip compressed data, was "conflux-web3-1.1.0.tar", last modified: Thu Apr 20 02:24:57 2023, max compression
```

## Comparing `conflux-web3-1.0.2.tar` & `conflux-web3-1.1.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-02-28 09:06:52.465832 conflux-web3-1.0.2/
--rw-r--r--   0 conflux-y   (501) staff       (20)       55 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/MANIFEST.in
--rw-r--r--   0 conflux-y   (501) staff       (20)     3819 2023-02-28 09:06:52.465574 conflux-web3-1.0.2/PKG-INFO
--rw-r--r--   0 conflux-y   (501) staff       (20)     3008 2023-02-01 03:42:18.000000 conflux-web3-1.0.2/README.md
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-02-28 09:06:52.421139 conflux-web3-1.0.2/_web3_hook/
--rw-r--r--   0 conflux-y   (501) staff       (20)     4927 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/_web3_hook/__init__.py
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-02-28 09:06:52.423666 conflux-web3-1.0.2/cfxpm/
--rw-r--r--   0 conflux-y   (501) staff       (20)       55 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/cfxpm/__init__.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     2215 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/cfxpm/contract.py
--rw-r--r--   0 conflux-y   (501) staff       (20)      635 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/cfxpm/package.py
--rw-r--r--   0 conflux-y   (501) staff       (20)        0 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/cfxpm/py.typed
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-02-28 09:06:52.425887 conflux-web3-1.0.2/cns/
--rw-r--r--   0 conflux-y   (501) staff       (20)       88 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/cns/__init__.py
--rw-r--r--   0 conflux-y   (501) staff       (20)    12876 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/cns/cns.py
--rw-r--r--   0 conflux-y   (501) staff       (20)      142 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/cns/exceptions.py
--rw-r--r--   0 conflux-y   (501) staff       (20)        0 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/cns/py.typed
--rw-r--r--   0 conflux-y   (501) staff       (20)     1700 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/cns/utils.py
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-02-28 09:06:52.431135 conflux-web3-1.0.2/conflux_web3/
--rw-r--r--   0 conflux-y   (501) staff       (20)      429 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/__init__.py
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-02-28 09:06:52.439276 conflux-web3-1.0.2/conflux_web3/_utils/
--rw-r--r--   0 conflux-y   (501) staff       (20)        0 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/_utils/__init__.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     1227 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/_utils/abi.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     1000 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/_utils/cns.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     1912 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/_utils/contracts.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     2579 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/_utils/decorators.py
--rw-r--r--   0 conflux-y   (501) staff       (20)      778 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/_utils/disabled_eth_apis.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     4691 2023-02-01 03:42:18.000000 conflux-web3-1.0.2/conflux_web3/_utils/events.py
--rw-r--r--   0 conflux-y   (501) staff       (20)    19314 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/_utils/method_formatters.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     1116 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/_utils/normalizers.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     5835 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/_utils/rpc_abi.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     2223 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/_utils/transactions.py
--rw-r--r--   0 conflux-y   (501) staff       (20)    60379 2023-02-01 03:42:18.000000 conflux-web3-1.0.2/conflux_web3/client.py
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-02-28 09:06:52.441684 conflux-web3-1.0.2/conflux_web3/contract/
--rw-r--r--   0 conflux-y   (501) staff       (20)     6122 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/contract/__init__.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     1629 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/contract/caller.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     1458 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/contract/constructor.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     7379 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/contract/event.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     4167 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/contract/function.py
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-02-28 09:06:52.456170 conflux-web3-1.0.2/conflux_web3/contract/metadata/
--rw-r--r--   0 conflux-y   (501) staff       (20)     1422 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/contract/metadata/AdminControl.json
--rw-r--r--   0 conflux-y   (501) staff       (20)      865 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/contract/metadata/Create2Factory.json
--rw-r--r--   0 conflux-y   (501) staff       (20)     5456 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/contract/metadata/CrossSpaceCall.json
--rw-r--r--   0 conflux-y   (501) staff       (20)     3375 2023-02-28 05:56:59.000000 conflux-web3-1.0.2/conflux_web3/contract/metadata/ENS.json
--rw-r--r--   0 conflux-y   (501) staff       (20)     4850 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/contract/metadata/ERC1820.json
--rw-r--r--   0 conflux-y   (501) staff       (20)    19262 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/contract/metadata/ERC20.json
--rw-r--r--   0 conflux-y   (501) staff       (20)    24033 2023-02-28 06:42:24.000000 conflux-web3-1.0.2/conflux_web3/contract/metadata/ETHRegistrarController.json
--rw-r--r--   0 conflux-y   (501) staff       (20)     3294 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/contract/metadata/Faucet.json
--rw-r--r--   0 conflux-y   (501) staff       (20)    33016 2023-02-28 06:42:24.000000 conflux-web3-1.0.2/conflux_web3/contract/metadata/NameWrapper.json
--rw-r--r--   0 conflux-y   (501) staff       (20)     4148 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/contract/metadata/ParamsControl.json
--rw-r--r--   0 conflux-y   (501) staff       (20)     3876 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/contract/metadata/PoSRegister.json
--rw-r--r--   0 conflux-y   (501) staff       (20)     6599 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/contract/metadata/SponsorWhitelistControl.json
--rw-r--r--   0 conflux-y   (501) staff       (20)     3147 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/contract/metadata/Staking.json
--rw-r--r--   0 conflux-y   (501) staff       (20)     4590 2023-02-28 06:42:24.000000 conflux-web3-1.0.2/conflux_web3/contract/metadata/__init__.py
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-02-28 09:06:52.456496 conflux-web3-1.0.2/conflux_web3/dev/
--rw-r--r--   0 conflux-y   (501) staff       (20)      301 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/dev/__init__.py
--rw-r--r--   0 conflux-y   (501) staff       (20)      239 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/exceptions.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     5864 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/main.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     1354 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/method.py
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-02-28 09:06:52.459309 conflux-web3-1.0.2/conflux_web3/middleware/
--rw-r--r--   0 conflux-y   (501) staff       (20)      970 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/middleware/__init__.py
--rw-r--r--   0 conflux-y   (501) staff       (20)      437 2023-02-01 03:42:18.000000 conflux-web3-1.0.2/conflux_web3/middleware/cache.py
--rw-r--r--   0 conflux-y   (501) staff       (20)      740 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/middleware/names.py
--rw-r--r--   0 conflux-y   (501) staff       (20)      809 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/middleware/pending.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     6744 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/middleware/wallet.py
--rw-r--r--   0 conflux-y   (501) staff       (20)        0 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/py.typed
--rw-r--r--   0 conflux-y   (501) staff       (20)      473 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/conflux_web3/txpool.py
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-02-28 09:06:52.460214 conflux-web3-1.0.2/conflux_web3/types/
--rw-r--r--   0 conflux-y   (501) staff       (20)    13377 2023-02-01 03:42:18.000000 conflux-web3-1.0.2/conflux_web3/types/__init__.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     2048 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/types/transaction_hash.py
--rw-r--r--   0 conflux-y   (501) staff       (20)      153 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/conflux_web3/utils.py
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-02-28 09:06:52.433754 conflux-web3-1.0.2/conflux_web3.egg-info/
--rw-r--r--   0 conflux-y   (501) staff       (20)     3819 2023-02-28 09:06:52.000000 conflux-web3-1.0.2/conflux_web3.egg-info/PKG-INFO
--rw-r--r--   0 conflux-y   (501) staff       (20)     2233 2023-02-28 09:06:52.000000 conflux-web3-1.0.2/conflux_web3.egg-info/SOURCES.txt
--rw-r--r--   0 conflux-y   (501) staff       (20)        1 2023-02-28 09:06:52.000000 conflux-web3-1.0.2/conflux_web3.egg-info/dependency_links.txt
--rw-r--r--   0 conflux-y   (501) staff       (20)      404 2023-02-28 09:06:52.000000 conflux-web3-1.0.2/conflux_web3.egg-info/requires.txt
--rw-r--r--   0 conflux-y   (501) staff       (20)       40 2023-02-28 09:06:52.000000 conflux-web3-1.0.2/conflux_web3.egg-info/top_level.txt
--rw-r--r--   0 conflux-y   (501) staff       (20)      532 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/pyproject.toml
--rw-r--r--   0 conflux-y   (501) staff       (20)       38 2023-02-28 09:06:52.465928 conflux-web3-1.0.2/setup.cfg
--rw-r--r--   0 conflux-y   (501) staff       (20)     3347 2023-02-28 08:42:51.000000 conflux-web3-1.0.2/setup.py
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-02-28 09:06:52.462033 conflux-web3-1.0.2/tests/
--rw-r--r--   0 conflux-y   (501) staff       (20)        1 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/tests/__init__.py
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-02-28 09:06:52.464582 conflux-web3-1.0.2/tests/_test_helpers/
--rw-r--r--   0 conflux-y   (501) staff       (20)      575 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/tests/_test_helpers/ENV_SETTING.py
--rw-r--r--   0 conflux-y   (501) staff       (20)        0 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/tests/_test_helpers/__init__.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     6598 2023-02-01 03:42:18.000000 conflux-web3-1.0.2/tests/_test_helpers/node.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     3048 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/tests/_test_helpers/type_check.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     2894 2022-12-30 09:15:10.000000 conflux-web3-1.0.2/tests/conftest.py
--rw-r--r--   0 conflux-y   (501) staff       (20)      192 2022-09-19 09:17:55.000000 conflux-web3-1.0.2/tests/test_node.py
+drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-04-20 02:24:57.882749 conflux-web3-1.1.0/
+-rw-r--r--   0 conflux-y   (501) staff       (20)       55 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/MANIFEST.in
+-rw-r--r--   0 conflux-y   (501) staff       (20)     3819 2023-04-20 02:24:57.882326 conflux-web3-1.1.0/PKG-INFO
+-rw-r--r--   0 conflux-y   (501) staff       (20)     3008 2023-02-01 03:42:18.000000 conflux-web3-1.1.0/README.md
+drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-04-20 02:24:57.761344 conflux-web3-1.1.0/_web3_hook/
+-rw-r--r--   0 conflux-y   (501) staff       (20)     5037 2023-04-19 07:46:46.000000 conflux-web3-1.1.0/_web3_hook/__init__.py
+drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-04-20 02:24:57.766520 conflux-web3-1.1.0/cfxpm/
+-rw-r--r--   0 conflux-y   (501) staff       (20)       55 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/cfxpm/__init__.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     2215 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/cfxpm/contract.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)      635 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/cfxpm/package.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)        0 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/cfxpm/py.typed
+drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-04-20 02:24:57.773587 conflux-web3-1.1.0/cns/
+-rw-r--r--   0 conflux-y   (501) staff       (20)       88 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/cns/__init__.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)    12876 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/cns/cns.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)      142 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/cns/exceptions.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)        0 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/cns/py.typed
+-rw-r--r--   0 conflux-y   (501) staff       (20)     1700 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/cns/utils.py
+drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-04-20 02:24:57.797610 conflux-web3-1.1.0/conflux_web3/
+-rw-r--r--   0 conflux-y   (501) staff       (20)      429 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/conflux_web3/__init__.py
+drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-04-20 02:24:57.829312 conflux-web3-1.1.0/conflux_web3/_utils/
+-rw-r--r--   0 conflux-y   (501) staff       (20)        0 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/_utils/__init__.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     1233 2023-04-18 10:20:48.000000 conflux-web3-1.1.0/conflux_web3/_utils/abi.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     1000 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/conflux_web3/_utils/cns.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     1912 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/conflux_web3/_utils/contracts.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     2579 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/conflux_web3/_utils/decorators.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)      778 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/_utils/disabled_eth_apis.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     4691 2023-02-01 03:42:18.000000 conflux-web3-1.1.0/conflux_web3/_utils/events.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)    19314 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/conflux_web3/_utils/method_formatters.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     1116 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/conflux_web3/_utils/normalizers.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     5835 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/_utils/rpc_abi.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     2223 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/conflux_web3/_utils/transactions.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)    60748 2023-04-19 03:22:17.000000 conflux-web3-1.1.0/conflux_web3/client.py
+drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-04-20 02:24:57.836184 conflux-web3-1.1.0/conflux_web3/contract/
+-rw-r--r--   0 conflux-y   (501) staff       (20)     6237 2023-04-19 07:40:53.000000 conflux-web3-1.1.0/conflux_web3/contract/__init__.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     2652 2023-04-19 07:41:05.000000 conflux-web3-1.1.0/conflux_web3/contract/caller.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     1458 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/contract/constructor.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     7336 2023-04-18 10:12:30.000000 conflux-web3-1.1.0/conflux_web3/contract/event.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     4676 2023-04-19 07:38:58.000000 conflux-web3-1.1.0/conflux_web3/contract/function.py
+drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-04-20 02:24:57.860307 conflux-web3-1.1.0/conflux_web3/contract/metadata/
+-rw-r--r--   0 conflux-y   (501) staff       (20)     1422 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/contract/metadata/AdminControl.json
+-rw-r--r--   0 conflux-y   (501) staff       (20)      865 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/contract/metadata/Create2Factory.json
+-rw-r--r--   0 conflux-y   (501) staff       (20)     5456 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/contract/metadata/CrossSpaceCall.json
+-rw-r--r--   0 conflux-y   (501) staff       (20)     3375 2023-02-28 05:56:59.000000 conflux-web3-1.1.0/conflux_web3/contract/metadata/ENS.json
+-rw-r--r--   0 conflux-y   (501) staff       (20)     4850 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/contract/metadata/ERC1820.json
+-rw-r--r--   0 conflux-y   (501) staff       (20)    19262 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/contract/metadata/ERC20.json
+-rw-r--r--   0 conflux-y   (501) staff       (20)    24033 2023-02-28 06:42:24.000000 conflux-web3-1.1.0/conflux_web3/contract/metadata/ETHRegistrarController.json
+-rw-r--r--   0 conflux-y   (501) staff       (20)     3294 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/contract/metadata/Faucet.json
+-rw-r--r--   0 conflux-y   (501) staff       (20)    33016 2023-02-28 06:42:24.000000 conflux-web3-1.1.0/conflux_web3/contract/metadata/NameWrapper.json
+-rw-r--r--   0 conflux-y   (501) staff       (20)     4148 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/contract/metadata/ParamsControl.json
+-rw-r--r--   0 conflux-y   (501) staff       (20)     3876 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/contract/metadata/PoSRegister.json
+-rw-r--r--   0 conflux-y   (501) staff       (20)     6599 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/contract/metadata/SponsorWhitelistControl.json
+-rw-r--r--   0 conflux-y   (501) staff       (20)     3147 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/contract/metadata/Staking.json
+-rw-r--r--   0 conflux-y   (501) staff       (20)     4590 2023-02-28 06:42:24.000000 conflux-web3-1.1.0/conflux_web3/contract/metadata/__init__.py
+drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-04-20 02:24:57.863177 conflux-web3-1.1.0/conflux_web3/dev/
+-rw-r--r--   0 conflux-y   (501) staff       (20)      301 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/dev/__init__.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)      239 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/conflux_web3/exceptions.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     5864 2023-04-19 02:44:44.000000 conflux-web3-1.1.0/conflux_web3/main.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     1354 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/conflux_web3/method.py
+drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-04-20 02:24:57.870995 conflux-web3-1.1.0/conflux_web3/middleware/
+-rw-r--r--   0 conflux-y   (501) staff       (20)      970 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/conflux_web3/middleware/__init__.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)      437 2023-02-01 03:42:18.000000 conflux-web3-1.1.0/conflux_web3/middleware/cache.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)      740 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/conflux_web3/middleware/names.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)      809 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/middleware/pending.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     6744 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/conflux_web3/middleware/wallet.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)        0 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/conflux_web3/py.typed
+-rw-r--r--   0 conflux-y   (501) staff       (20)      473 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/conflux_web3/txpool.py
+drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-04-20 02:24:57.873690 conflux-web3-1.1.0/conflux_web3/types/
+-rw-r--r--   0 conflux-y   (501) staff       (20)    13377 2023-02-01 03:42:18.000000 conflux-web3-1.1.0/conflux_web3/types/__init__.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     2048 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/types/transaction_hash.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)      153 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/conflux_web3/utils.py
+drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-04-20 02:24:57.803483 conflux-web3-1.1.0/conflux_web3.egg-info/
+-rw-r--r--   0 conflux-y   (501) staff       (20)     3819 2023-04-20 02:24:57.000000 conflux-web3-1.1.0/conflux_web3.egg-info/PKG-INFO
+-rw-r--r--   0 conflux-y   (501) staff       (20)     2233 2023-04-20 02:24:57.000000 conflux-web3-1.1.0/conflux_web3.egg-info/SOURCES.txt
+-rw-r--r--   0 conflux-y   (501) staff       (20)        1 2023-04-20 02:24:57.000000 conflux-web3-1.1.0/conflux_web3.egg-info/dependency_links.txt
+-rw-r--r--   0 conflux-y   (501) staff       (20)      402 2023-04-20 02:24:57.000000 conflux-web3-1.1.0/conflux_web3.egg-info/requires.txt
+-rw-r--r--   0 conflux-y   (501) staff       (20)       40 2023-04-20 02:24:57.000000 conflux-web3-1.1.0/conflux_web3.egg-info/top_level.txt
+-rw-r--r--   0 conflux-y   (501) staff       (20)      532 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/pyproject.toml
+-rw-r--r--   0 conflux-y   (501) staff       (20)       38 2023-04-20 02:24:57.882986 conflux-web3-1.1.0/setup.cfg
+-rw-r--r--   0 conflux-y   (501) staff       (20)     3345 2023-04-19 08:04:36.000000 conflux-web3-1.1.0/setup.py
+drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-04-20 02:24:57.877786 conflux-web3-1.1.0/tests/
+-rw-r--r--   0 conflux-y   (501) staff       (20)        1 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/tests/__init__.py
+drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2023-04-20 02:24:57.881089 conflux-web3-1.1.0/tests/_test_helpers/
+-rw-r--r--   0 conflux-y   (501) staff       (20)      575 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/tests/_test_helpers/ENV_SETTING.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)        0 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/tests/_test_helpers/__init__.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     6598 2023-02-01 03:42:18.000000 conflux-web3-1.1.0/tests/_test_helpers/node.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     3048 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/tests/_test_helpers/type_check.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)     2894 2022-12-30 09:15:10.000000 conflux-web3-1.1.0/tests/conftest.py
+-rw-r--r--   0 conflux-y   (501) staff       (20)      192 2022-09-19 09:17:55.000000 conflux-web3-1.1.0/tests/test_node.py
```

### Comparing `conflux-web3-1.0.2/PKG-INFO` & `conflux-web3-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflux-web3
-Version: 1.0.2
+Version: 1.1.0
 Summary: Python SDK for Conflux network
 Home-page: https://github.com/conflux-chain/python-conflux-sdk
 Author: Conflux-Dev
 Author-email: wenda.zhang@confluxnetwork.org
 Keywords: python,conflux,blockchain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `conflux-web3-1.0.2/README.md` & `conflux-web3-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/_web3_hook/__init__.py` & `conflux-web3-1.1.0/_web3_hook/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # so make sure this module is executed before any module of conflux_web3 or web3 is executed
 # or the hook might not take effect
 # else try directly importing the package to hook
 
 from typing import (
     TYPE_CHECKING,
     Callable,
-    Dict
+    Dict,
+    Union,
 )
 from cfx_utils.post_import_hook import (
     when_imported
 )
 from cfx_address import (
     Base32Address
 )
@@ -97,16 +98,18 @@
     "safe": "latest_confirmed",
     "finalized": "latest_finalized",
 }
 
 # used to hook web3.contract.parse_block_identifier
 # hook is activated in _web3_hook
 def cfx_parse_block_identifier(
-    w3: "Web3", block_identifier: "EpochNumberParam"
+    w3: "Web3", block_identifier: Union["EpochNumberParam", None]
 ) -> "EpochNumberParam":
+    if block_identifier is None:
+        return w3.cfx.default_block
     if isinstance(block_identifier, int):
         return block_identifier
     elif block_identifier in ['earliest', 'latest_checkpoint', 'latest_finalized', 'latest_confirmed', 'latest_state', 'latest_mined']: # get_args("EpochLiteral")
         return block_identifier
     elif isinstance(block_identifier, bytes) or (
         isinstance(block_identifier, str) and block_identifier.startswith("0x")
     ):
@@ -114,18 +117,18 @@
         # assert r is not None
         return w3.cfx.get_block_by_hash(block_identifier)["epochNumber"] # type: ignore
     elif block_identifier in eth_to_cfx_tag_mapping:
         return eth_to_cfx_tag_mapping[block_identifier]
     else:
         raise InvalidEpochNumebrParam
 
-@when_imported("web3.contract")
+@when_imported("web3._utils.contracts")
 def hook_parse_block_identifier(mod):
     # from conflux_web3.contract import cfx_parse_block_identifier
-    if mod.__name__ == "web3.contract":
+    if mod.__name__ == "web3._utils.contracts":
         mod.parse_block_identifier = conditional_func(
             cfx_parse_block_identifier,
             cfx_web3_condition
         )(mod.parse_block_identifier)
     
 @when_imported("ethpm.package")
 def hook_ethpm_package(mod):
```

### Comparing `conflux-web3-1.0.2/cfxpm/contract.py` & `conflux-web3-1.1.0/cfxpm/contract.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/cfxpm/package.py` & `conflux-web3-1.1.0/cfxpm/package.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/cns/cns.py` & `conflux-web3-1.1.0/cns/cns.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/cns/utils.py` & `conflux-web3-1.1.0/cns/utils.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/_utils/abi.py` & `conflux-web3-1.1.0/conflux_web3/_utils/abi.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from eth_abi.decoding import (
     AddressDecoder
 )
 from eth_abi.exceptions import (
     EncodingError
 )
 from web3._utils.abi import (
-    build_default_registry, 
+    build_non_strict_registry, 
     AddressEncoder,
 )
 from cfx_address import (
     Base32Address,
     validate_base32
 )
 from cfx_utils.exceptions import (
@@ -37,15 +37,15 @@
         except InvalidBase32Address:
             raise EncodingError(InvalidBase32Address)
 
 class CfxAddressDecoder(AddressDecoder):
     decode_fn = lambda x: x
 
 def build_cfx_default_registry() -> ABIRegistry:
-    registry = build_default_registry()
+    registry = build_non_strict_registry()
     
     registry.unregister('address')
     registry.register(
         BaseEquals('address'),
         Base32AddressEncoder, CfxAddressDecoder,
         label='address',
     )
```

### Comparing `conflux-web3-1.0.2/conflux_web3/_utils/cns.py` & `conflux-web3-1.1.0/conflux_web3/_utils/cns.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/_utils/contracts.py` & `conflux-web3-1.1.0/conflux_web3/_utils/contracts.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/_utils/decorators.py` & `conflux-web3-1.1.0/conflux_web3/_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/_utils/disabled_eth_apis.py` & `conflux-web3-1.1.0/conflux_web3/_utils/disabled_eth_apis.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/_utils/events.py` & `conflux-web3-1.1.0/conflux_web3/_utils/events.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/_utils/method_formatters.py` & `conflux-web3-1.1.0/conflux_web3/_utils/method_formatters.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/_utils/normalizers.py` & `conflux-web3-1.1.0/conflux_web3/_utils/normalizers.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/_utils/rpc_abi.py` & `conflux-web3-1.1.0/conflux_web3/_utils/rpc_abi.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/_utils/transactions.py` & `conflux-web3-1.1.0/conflux_web3/_utils/transactions.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/client.py` & `conflux-web3-1.1.0/conflux_web3/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,22 @@
 
 class BaseCfx(BaseEth):
     _default_block: EpochNumberParam = "latest_state"
     _default_account: Union[AddressParam, Empty] = empty
     w3: "Web3"
     
     @property
+    def default_block(self) -> EpochNumberParam:
+        return self._default_block
+
+    @default_block.setter
+    def default_block(self, value: EpochNumberParam) -> None:
+        self._default_block = value
+    
+    @property
     def default_account(self) -> Base32Address:
         """default account address, this address will be used as default `from` address if transaction `from` field is empty
         """
         return self._default_account # type: ignore
     
 
     @default_account.setter
@@ -252,14 +260,18 @@
         RPC.cfx_getConfirmationRiskByHash,
     )
     
     _get_transaction_receipt: ConfluxMethod[Callable[[_Hash32], TxReceipt]] = ConfluxMethod(
         RPC.cfx_getTransactionReceipt
     )
     
+    _transaction_receipt: ConfluxMethod[Callable[[_Hash32], TxReceipt]] = ConfluxMethod(
+        RPC.cfx_getTransactionReceipt
+    )
+    
     _get_transaction_by_hash: ConfluxMethod[Callable[[_Hash32], TxData]] = ConfluxMethod(
         RPC.cfx_getTransactionByHash
     )
     
     _get_block_by_hash: ConfluxMethod[Callable[[_Hash32, bool], BlockData]] = ConfluxMethod(
         RPC.cfx_getBlockByHash
     )
@@ -456,15 +468,15 @@
             kwargs["address"] = address
         return super().contract(**kwargs)  # type: ignore
 
 class ConfluxClient(BaseCfx, Eth):
     """RPC entry defined provides friendlier APIs for users
     """
     account: Account
-    defaultContractFactory: Type[ConfluxContract] = ConfluxContract
+    _default_contract_factory: Type[ConfluxContract] = ConfluxContract
     
     def __init__(self, w3: "Web3") -> None:
         super().__init__(w3)
         self.account = Account()
         self.account.set_w3(w3)
         self._disable_eth_methods(disabled_method_list)
```

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/__init__.py` & `conflux-web3-1.1.0/conflux_web3/contract/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     List,
     Callable,
     Union,
 )
 
 from web3.contract import (
     Contract,
-    find_functions_by_identifier,
 )
 
-from web3._utils.blocks import (
-    is_hex_encoded_block_hash,
+from web3.contract.utils import (
+    find_functions_by_identifier,
 )
+
 from web3._utils.normalizers import (
     normalize_abi,
     normalize_bytecode,
 )
 from web3._utils.datatypes import (
     PropertyCheckingFactory,
 )
@@ -116,16 +116,16 @@
                 raise Base32AddressNotMatch(f"expected an address of contract type or builtin type"
                                             f"receives {address} of {address.address_type}")
             self.address = Base32Address(address, self.w3.cfx.chain_id, verbose=True)
 
         if not self.address:
             raise TypeError("The address argument is required to instantiate a contract.")
 
-        self.functions = ConfluxContractFunctions(self.abi, self.w3, self.address)
-        self.caller = ConfluxContractCaller(self.abi, self.w3, self.address)
+        self.functions = ConfluxContractFunctions(self.abi, self.w3, self.address, decode_tuples=self.decode_tuples)
+        self.caller = ConfluxContractCaller(self.abi, self.w3, self.address, decode_tuples=self.decode_tuples)
         self.events = ConfluxContractEvents(self.abi, self.w3, self.address)
         self.fallback = Contract.get_fallback_function(self.abi, self.w3, ConfluxContractFunction, self.address) # type: ignore
         self.receive = Contract.get_receive_function(self.abi, self.w3, ConfluxContractFunction, self.address) # type: ignore
 
     @classmethod
     def factory(cls, w3: "Web3", class_name: Optional[str] = None, **kwargs: Any) -> "Contract":
         kwargs["w3"] = w3
@@ -142,16 +142,16 @@
             PropertyCheckingFactory(
                 class_name or cls.__name__,
                 (cls,),
                 kwargs,
                 normalizers=normalizers,
             ),
         )
-        contract.functions = ConfluxContractFunctions(contract.abi, contract.w3)
-        contract.caller = ConfluxContractCaller(contract.abi, contract.w3, contract.address)
+        contract.functions = ConfluxContractFunctions(contract.abi, contract.w3, decode_tuples=contract.decode_tuples)
+        contract.caller = ConfluxContractCaller(contract.abi, contract.w3, contract.address, decode_tuples=contract.decode_tuples)
         contract.events = ConfluxContractEvents(contract.abi, contract.w3)
         contract.fallback = Contract.get_fallback_function(
             contract.abi,
             contract.w3,
             ConfluxContractFunction,
         )
         contract.receive = Contract.get_receive_function(
```

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/constructor.py` & `conflux-web3-1.1.0/conflux_web3/contract/constructor.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/event.py` & `conflux-web3-1.1.0/conflux_web3/contract/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     cast,
 )
 from hexbytes import HexBytes
 
 from eth_utils.functional import (
     to_tuple,
 )
-from web3.contract import (
+from web3.contract.base_contract import (
     BaseContractEvent,
     BaseContractEvents,
 )
 from web3.datastructures import (
     AttributeDict,
     MutableAttributeDict,
 )
@@ -28,17 +28,14 @@
 )
 from web3.logs import (
     DISCARD,
     IGNORE,
     STRICT,
     WARN,
 )
-from web3.contract import (
-    check_for_forbidden_api_filter_arguments
-)
 from web3._utils.events import (
     EventLogErrorFlags,
 )
 from web3._utils.filters import (
     construct_event_filter_params
 )
 from web3.exceptions import (
@@ -165,15 +162,15 @@
         if argument_filters is None:
             argument_filters = kwargs
 
         _filters = dict(**argument_filters)
 
         event_abi = self._get_event_abi()
 
-        check_for_forbidden_api_filter_arguments(event_abi, _filters)
+        BaseContractEvent.check_for_forbidden_api_filter_arguments(event_abi, _filters)
 
         _, event_filter_params = construct_event_filter_params(
             self._get_event_abi(),
             self.w3.codec,
             argument_filters=_filters,
         )
         return event_filter_params["topics"] # type: ignore
```

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/function.py` & `conflux-web3-1.1.0/conflux_web3/contract/function.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from typing import (
     TYPE_CHECKING,
+    cast,
     Any,
     Optional,
 )
 
-from web3.contract import (
+from web3._utils.datatypes import (
+    PropertyCheckingFactory,
+)
+
+from web3.contract.contract import (
     BaseContractFunctions,
     ContractFunction,
+)
+
+from web3.contract.contract import (
     call_contract_function
 )
+
 from web3.types import (
     ABI,
     ABIFunction,
     FunctionIdentifier,
     CallOverride
 )
 
@@ -109,28 +118,40 @@
             self.function_identifier,
             call_transaction,
             block_identifier, # type: ignore
             self.contract_abi,
             self.abi,
             state_override,
             ccip_read_enabled,
+            self.decode_tuples,
             *self.args,
             **self.kwargs,
         )
 
     def transact(self, transaction: Optional[TxParam] = None) -> "TransactionHash":
         if transaction and "value" in transaction:
             transaction["value"] = to_int_if_drip_units(transaction["value"])
         return super().transact(transaction) # type: ignore
 
+    @classmethod
+    def factory(cls, class_name: str, **kwargs: Any) -> "ConfluxContractFunction":
+        return cast(ConfluxContractFunction, PropertyCheckingFactory(class_name, (cls,), kwargs)(kwargs.get("abi")))
+
 
 class ConfluxContractFunctions(BaseContractFunctions):
     def __init__(
         self,
         abi: ABI,
         w3: "Web3",
         address: Optional[AddressParam] = None,
+        decode_tuples: Optional[bool] = False,
     ) -> None:
-        super().__init__(abi, w3, ConfluxContractFunction, address)  # type: ignore
+        super().__init__(
+            abi,
+            w3,
+            ConfluxContractFunction,
+            address, # type: ignore
+            decode_tuples
+        )
     
     def __getattr__(self, function_name: str) -> "ConfluxContractFunction":
         return super().__getattr__(function_name) # type: ignore
```

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/metadata/AdminControl.json` & `conflux-web3-1.1.0/conflux_web3/contract/metadata/AdminControl.json`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/metadata/Create2Factory.json` & `conflux-web3-1.1.0/conflux_web3/contract/metadata/Create2Factory.json`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/metadata/CrossSpaceCall.json` & `conflux-web3-1.1.0/conflux_web3/contract/metadata/CrossSpaceCall.json`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/metadata/ENS.json` & `conflux-web3-1.1.0/conflux_web3/contract/metadata/ENS.json`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/metadata/ERC1820.json` & `conflux-web3-1.1.0/conflux_web3/contract/metadata/ERC1820.json`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/metadata/ERC20.json` & `conflux-web3-1.1.0/conflux_web3/contract/metadata/ERC20.json`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/metadata/ETHRegistrarController.json` & `conflux-web3-1.1.0/conflux_web3/contract/metadata/ETHRegistrarController.json`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/metadata/Faucet.json` & `conflux-web3-1.1.0/conflux_web3/contract/metadata/Faucet.json`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/metadata/NameWrapper.json` & `conflux-web3-1.1.0/conflux_web3/contract/metadata/NameWrapper.json`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/metadata/ParamsControl.json` & `conflux-web3-1.1.0/conflux_web3/contract/metadata/ParamsControl.json`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/metadata/PoSRegister.json` & `conflux-web3-1.1.0/conflux_web3/contract/metadata/PoSRegister.json`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/metadata/SponsorWhitelistControl.json` & `conflux-web3-1.1.0/conflux_web3/contract/metadata/SponsorWhitelistControl.json`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/metadata/Staking.json` & `conflux-web3-1.1.0/conflux_web3/contract/metadata/Staking.json`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/contract/metadata/__init__.py` & `conflux-web3-1.1.0/conflux_web3/contract/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/main.py` & `conflux-web3-1.1.0/conflux_web3/main.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/method.py` & `conflux-web3-1.1.0/conflux_web3/method.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/middleware/__init__.py` & `conflux-web3-1.1.0/conflux_web3/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/middleware/names.py` & `conflux-web3-1.1.0/conflux_web3/middleware/names.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/middleware/pending.py` & `conflux-web3-1.1.0/conflux_web3/middleware/pending.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/middleware/wallet.py` & `conflux-web3-1.1.0/conflux_web3/middleware/wallet.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/types/__init__.py` & `conflux-web3-1.1.0/conflux_web3/types/__init__.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3/types/transaction_hash.py` & `conflux-web3-1.1.0/conflux_web3/types/transaction_hash.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/conflux_web3.egg-info/PKG-INFO` & `conflux-web3-1.1.0/conflux_web3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflux-web3
-Version: 1.0.2
+Version: 1.1.0
 Summary: Python SDK for Conflux network
 Home-page: https://github.com/conflux-chain/python-conflux-sdk
 Author: Conflux-Dev
 Author-email: wenda.zhang@confluxnetwork.org
 Keywords: python,conflux,blockchain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `conflux-web3-1.0.2/conflux_web3.egg-info/SOURCES.txt` & `conflux-web3-1.1.0/conflux_web3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/pyproject.toml` & `conflux-web3-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/setup.py` & `conflux-web3-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import (
     find_packages,
     setup,
 )
 
-VERSION = "1.0.2"
+VERSION = "1.1.0"
 DESCRIPTION = 'Python SDK for Conflux network'
 with open('./README.md') as readme:
     long_description = readme.read()
 
 extras_require = {
     'tester': [
         "docker>=5.0.0,<6",
@@ -88,15 +88,15 @@
     long_description=long_description,
     packages=find_packages(),
     package_data={"conflux_web3": ["contract/metadata/*.json", "py.typed"],
                   "cns": ["py.typed"],
                   "cfxpm": ["py.typed"]},
     url='https://github.com/conflux-chain/python-conflux-sdk',
     install_requires=[
-        "web3==6.0.0b9",
+        "web3==6.2.0",
         "cfx-address>=1.0.0",
         "cfx-account>=1.0.0",
         "cfx-utils>=1.0.0",
         # "cached_property==1.5.2", # required by cfx-account
         # "eth-account>=0.6.0,<0.7.0"
     ],  # add any additional packages that
     # needs to be installed along with your package. Eg: 'caer'
```

### Comparing `conflux-web3-1.0.2/tests/_test_helpers/ENV_SETTING.py` & `conflux-web3-1.1.0/tests/_test_helpers/ENV_SETTING.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/tests/_test_helpers/node.py` & `conflux-web3-1.1.0/tests/_test_helpers/node.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/tests/_test_helpers/type_check.py` & `conflux-web3-1.1.0/tests/_test_helpers/type_check.py`

 * *Files identical despite different names*

### Comparing `conflux-web3-1.0.2/tests/conftest.py` & `conflux-web3-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

