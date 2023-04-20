# Comparing `tmp/cairo-nile-0.9.0.tar.gz` & `tmp/cairo-nile-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cairo-nile-0.9.0.tar", last modified: Fri Sep  9 23:35:15 2022, max compression
+gzip compressed data, was "cairo-nile-0.9.1.tar", last modified: Mon Oct  3 21:30:00 2022, max compression
```

## Comparing `cairo-nile-0.9.0.tar` & `cairo-nile-0.9.1.tar`

### file list

```diff
@@ -1,82 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.881386 cairo-nile-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.869386 cairo-nile-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.873386 cairo-nile-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3045 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15990 2022-09-09 23:35:15.881386 cairo-nile-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15544 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/RELEASING.md
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/example.env
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-09-09 23:35:15.881386 cairo-nile-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.869386 cairo-nile-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.873386 cairo-nile-0.9.0/src/cairo_nile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15990 2022-09-09 23:35:15.000000 cairo-nile-0.9.0/src/cairo_nile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-09-09 23:35:15.000000 cairo-nile-0.9.0/src/cairo_nile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 23:35:15.000000 cairo-nile-0.9.0/src/cairo_nile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-09 23:35:15.000000 cairo-nile-0.9.0/src/cairo_nile.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 23:34:10.000000 cairo-nile-0.9.0/src/cairo_nile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-09 23:35:15.000000 cairo-nile-0.9.0/src/cairo_nile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-09 23:35:15.000000 cairo-nile-0.9.0/src/cairo_nile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.873386 cairo-nile-0.9.0/src/nile/
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.873386 cairo-nile-0.9.0/src/nile/artifacts/
--rw-r--r--   0 runner    (1001) docker     (121)  1331396 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/artifacts/Account.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.877386 cairo-nile-0.9.0/src/nile/artifacts/abis/
--rw-r--r--   0 runner    (1001) docker     (121)     3761 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/artifacts/abis/Account.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.877386 cairo-nile-0.9.0/src/nile/base_project/
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/base_project/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.877386 cairo-nile-0.9.0/src/nile/base_project/contracts/
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/base_project/contracts/contract.cairo
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.877386 cairo-nile-0.9.0/src/nile/base_project/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/base_project/tests/test_contract.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6628 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3062 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/common.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.877386 cairo-nile-0.9.0/src/nile/core/
--rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/core/account.py
--rw-r--r--   0 runner    (1001) docker     (121)     2061 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/core/call_or_invoke.py
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/core/clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     2349 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/core/compile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/core/declare.py
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/core/deploy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/core/init.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/core/install.py
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/core/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/core/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/core/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/core/test.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/core/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/deployments.py
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/nre.py
--rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/signer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.877386 cairo-nile-0.9.0/src/nile/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     2944 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3310 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/src/nile/utils/get_accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.881386 cairo-nile-0.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.881386 cairo-nile-0.9.0/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     3905 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/commands/test_account.py
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/commands/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     3778 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/commands/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/commands/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/commands/test_declare.py
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/commands/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3898 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/commands/test_get_accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/commands/test_node.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.881386 cairo-nile-0.9.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/core/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.869386 cairo-nile-0.9.0/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 23:35:15.881386 cairo-nile-0.9.0/tests/resources/contracts/
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/resources/contracts/contract.cairo
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/resources/contracts/contract_with_unwhitelisted_hints.cairo
--rw-r--r--   0 runner    (1001) docker     (121)     5529 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/test_nre.py
--rw-r--r--   0 runner    (1001) docker     (121)     3579 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tests/test_signer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-09-09 23:33:59.000000 cairo-nile-0.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.172683 cairo-nile-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.160683 cairo-nile-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.164683 cairo-nile-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     3045 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    18166 2022-10-03 21:30:00.172683 cairo-nile-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    17720 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/RELEASING.md
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/example.env
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-10-03 21:30:00.172683 cairo-nile-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.160683 cairo-nile-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.164683 cairo-nile-0.9.1/src/cairo_nile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    18166 2022-10-03 21:30:00.000000 cairo-nile-0.9.1/src/cairo_nile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1726 2022-10-03 21:30:00.000000 cairo-nile-0.9.1/src/cairo_nile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 21:30:00.000000 cairo-nile-0.9.1/src/cairo_nile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-03 21:30:00.000000 cairo-nile-0.9.1/src/cairo_nile.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 21:29:02.000000 cairo-nile-0.9.1/src/cairo_nile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-03 21:30:00.000000 cairo-nile-0.9.1/src/cairo_nile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-03 21:30:00.000000 cairo-nile-0.9.1/src/cairo_nile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.164683 cairo-nile-0.9.1/src/nile/
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.164683 cairo-nile-0.9.1/src/nile/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (121)  1331396 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/artifacts/Account.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.168683 cairo-nile-0.9.1/src/nile/artifacts/abis/
+-rw-r--r--   0 runner    (1001) docker     (121)     3761 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/artifacts/abis/Account.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.168683 cairo-nile-0.9.1/src/nile/base_project/
+-rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/base_project/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.168683 cairo-nile-0.9.1/src/nile/base_project/contracts/
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/base_project/contracts/contract.cairo
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.168683 cairo-nile-0.9.1/src/nile/base_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      936 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/base_project/tests/test_contract.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7641 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3306 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/common.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.168683 cairo-nile-0.9.1/src/nile/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     3644 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/core/account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2288 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/core/call_or_invoke.py
+-rw-r--r--   0 runner    (1001) docker     (121)      761 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/core/clean.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2349 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/core/compile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/core/declare.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/core/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/core/init.py
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/core/install.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/core/test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3222 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/nre.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/signer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.168683 cairo-nile-0.9.1/src/nile/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     3563 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3354 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2989 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/utils/get_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/src/nile/utils/get_nonce.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.168683 cairo-nile-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.172683 cairo-nile-0.9.1/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     3416 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/commands/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/commands/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3778 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/commands/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2927 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/commands/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2592 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/commands/test_declare.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2398 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/commands/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6687 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/commands/test_get_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/commands/test_get_nonce.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/commands/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.172683 cairo-nile-0.9.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/core/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.172683 cairo-nile-0.9.1/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/mocks/mock_response.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.160683 cairo-nile-0.9.1/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 21:30:00.172683 cairo-nile-0.9.1/tests/resources/contracts/
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/resources/contracts/contract.cairo
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/resources/contracts/contract_with_unwhitelisted_hints.cairo
+-rw-r--r--   0 runner    (1001) docker     (121)     5529 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1626 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/test_nre.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tests/test_signer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-10-03 21:28:55.000000 cairo-nile-0.9.1/tox.ini
```

### Comparing `cairo-nile-0.9.0/.github/workflows/ci.yml` & `cairo-nile-0.9.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/.gitignore` & `cairo-nile-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/CONTRIBUTING.md` & `cairo-nile-0.9.1/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,17 @@
     ```
 
 5. Go to [github.com/OpenZeppelin/nile](https://github.com/OpenZeppelin/nile) in your web browser and issue a new pull request.
     Begin the body of the PR with "Fixes #123" or "Resolves #123" to link the PR to the issue that it is resolving.
     *IMPORTANT* Read the PR template very carefully and make sure to follow all the instructions. These instructions
     refer to some very important conditions that your PR must meet in order to be accepted, such as making sure that all PR checks pass.
 
-6. Maintainers will review your code and possibly ask for changes before your code is pulled in to the main repository. We'll check that all tests pass, review the coding style, and check for general code correctness. If everything is OK, we'll merge your pull request and your code will be part of OpenZeppelin Nile.
+6. Maintainers will review your code and possibly ask for changes before your code is pulled into the main repository. We'll check that all tests pass, review the coding style, and check for general code correctness. If everything is OK, we'll merge your pull request and your code will be part of OpenZeppelin Nile.
 
-    *IMPORTANT* Please pay attention to the maintainer's feedback, since its a necessary step to keep up with the standards OpenZeppelin Nile attains to.
+    *IMPORTANT* Please pay attention to the maintainer's feedback, since it's a necessary step to keep up with the standards OpenZeppelin Nile attains to.
 
 ## All set
 
 If you have any questions, feel free to post them to github.com/OpenZeppelin/nile/issues.
 
 Finally, if you're looking to collaborate and want to find easy tasks to start, look at the issues we marked as ["Good first issue"](https://github.com/OpenZeppelin/nile/labels/good%20first%20issue).
```

### Comparing `cairo-nile-0.9.0/LICENSE` & `cairo-nile-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/PKG-INFO` & `cairo-nile-0.9.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: cairo-nile
-Version: 0.9.0
-Summary: StarkNet/Cairo development toolbelt
-Home-page: https://github.com/martriay/nile
-Author: Martin Triay
-Author-email: martriay@gmail.com
-License: MIT
-Platform: any
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: testing
-License-File: LICENSE
-
 # OpenZeppelin Nile ⛵
 
 [![Tests and linter](https://github.com/OpenZeppelin/nile/actions/workflows/ci.yml/badge.svg)](https://github.com/OpenZeppelin/nile/actions/workflows/ci.yml)
 
 _Navigate your [StarkNet](https://www.cairo-lang.org/docs/hello_starknet/index.html) projects written in [Cairo](https://cairo-lang.org)._
 
 ## Getting started
@@ -133,16 +117,17 @@
 📦 Registering deployment as my_contract in localhost.deployments.txt
 ```
 
 A few things to notice here:
 
 1. `nile deploy <contract_name>` looks for an artifact with the same name
 2. This created a `localhost.deployments.txt` file storing all data related to my deployment
-3. The `--alias` parameter lets me create an unique identifier for future interactions, if no alias is set then the contract's address can be used as identifier
+3. The `--alias` parameter lets me create a unique identifier for future interactions, if no alias is set then the contract's address can be used as identifier
 4. By default Nile works on local, but you can use the `--network` parameter to interact with `mainnet`, `goerli`, and the default `localhost`.
+5. By default, the ABI corresponding to the contract will be registered with the deployment. To register a different ABI file, use the `--abi` parameter.
 
 ### `declare`
 
 ```sh
 nile declare contract --alias my_contract
 
 🚀 Declaring contract
@@ -150,15 +135,15 @@
 📦 Registering declaration as my_contract in localhost.declarations.txt
 ```
 
 A few things to notice here:
 
 1. `nile declare <contract_name>` looks for an artifact with the same name
 2. This created a `localhost.declarations.txt` file storing all data related to my declarations
-3. The `--alias` parameter lets me create an unique identifier for future interactions, if no alias is set then the contract's address can be used as identifier
+3. The `--alias` parameter lets me create a unique identifier for future interactions, if no alias is set then the contract's address can be used as identifier
 4. By default Nile works on local, but you can use the `--network` parameter to interact with `mainnet`, `goerli`, and the default `localhost`.
 
 ### `setup`
 
 Deploy an Account associated with a given private key.
 
 To avoid accidentally leaking private keys, this command takes an alias instead of the actual private key. This alias is associated with an environmental variable of the same name, whose value is the actual private key.
@@ -400,42 +385,102 @@
 
     # or
     alice, bob, *_ = accounts
     alice.send(...)
     bob.send(...)
 ```
 
-> Please note that the list of accounts include only those that exist in the local `<network>.accounts.json` file.
+> Please note that the list of accounts includes only those that exist in the local `<network>.accounts.json` file. In a recent release we added a flag to the command, to get predeployed accounts if the network you are connected to is a [starknet-devnet](https://github.com/Shard-Labs/starknet-devnet) instance.
+
+### `get-accounts --predeployed`
+
+This flag retrieves the predeployed accounts if the network you are connecting to is a [starknet-devnet](https://github.com/Shard-Labs/starknet-devnet) instance.
+
+You can use it either from the cli:
+
+```sh
+nile get-accounts --predeployed
+```
+
+Or from the nile runtime environment for scripting:
+
+```python
+def run(nre):
+
+    # fetch the list of pre-deployed accounts from devnet
+    accounts = nre.get_accounts(predeployed=True)
+
+    # then
+    accounts[0].send(...)
+
+    # or
+    alice, bob, *_ = accounts
+    alice.send(...)
+    bob.send(...)
+```
+
+### `get-nonce`
+
+Retrieves the nonce for the given contract address (usually an account).
+
+```sh
+nile get-nonce <contract_address>
+```
+
+## Short string literals
+
+From [cairo-lang docs](https://www.cairo-lang.org/docs/how_cairo_works/consts.html#short-string-literals): A short string is a string whose length is at most 31 characters, and therefore can fit into a single field element.
+
+In Nile, arguments to contract calls (calldata) that are neither int nor hex, are treated as short strings and converted automatically to the corresponding felt representation. Because of this, you can run the following from the CLI:
+
+```sh
+nile deploy MyToken 'MyToken name' 'MyToken symbol' (...)
+```
+
+And this is equivalent to passing the felt representation directly like this:
+
+```sh
+nile deploy MyToken 0x4d79546f6b656e206e616d65 0x4d79546f6b656e2073796d626f6c (...)
+```
+
+Note that if you want to pass the token name as a hex or an int, you need to provide the felt representation directly because these values are not interpreted as short strings. You can open a python terminal, and import and use the `str_to_felt` util like this:
+
+```python
+>>> from nile.utils import str_to_felt
+>>>
+>>> str_to_felt('any string')
+460107418789485453340263
+```
 
 ## Extending Nile with plugins
 
 Nile has the possibility of extending its CLI and `NileRuntimeEnvironment` functionalities through plugins. For developing plugins for Nile fork [this plugin example](https://github.com/franalgaba/nile-plugin-example) boilerplate and implement your desired functionality with the provided instructions.
 
 ### How it works
 
 This implementation takes advantage of the native extensibility features of [click](https://click.palletsprojects.com/). Using click and leveraging the Python [entrypoints](https://packaging.python.org/en/latest/specifications/entry-points/) we have a simple manner of handling extension natively on Python environments through dependencies. The plugin implementation on Nile looks for specific Python entrypoints constraints for adding commands.
 
 In order for this implementation to be functional, it is needed by the plugin developer to follow some development guidelines defined in this simple plugin example extending Nile for a dummy greet extension. In a brief explanation the guidelines are as follows:
 
-1. Define a Python module that implement a click command or group:
+1. Define a Python module that implements a click command or group:
 
    ```python
    # First, import click dependency
    import click
 
    # Decorate the method that will be the command name with `click.command`
    @click.command()
    # You can define custom parameters as defined in `click`: https://click.palletsprojects.com/en/7.x/options/
    def my_command():
        # Help message to show with the command
        """
        Subcommand plugin that does something.
        """
        # Done! Now implement your custom functionality in the command
-       click.echo("I'm a plugin overiding a command!")
+       click.echo("I'm a plugin overriding a command!")
    ```
 
 2. Define the plugin entrypoint. In this case using Poetry features in the pyproject.toml file:
 
    ```sh
    # We need to specify that click commands are Poetry entrypoints of type `nile_plugins`. Do not modify this
    [tool.poetry.plugins."nile_plugins"]
```

### Comparing `cairo-nile-0.9.0/README.md` & `cairo-nile-0.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: cairo-nile
+Version: 0.9.1
+Summary: StarkNet/Cairo development toolbelt
+Home-page: https://github.com/martriay/nile
+Author: Martin Triay
+Author-email: martriay@gmail.com
+License: MIT
+Platform: any
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: testing
+License-File: LICENSE
+
 # OpenZeppelin Nile ⛵
 
 [![Tests and linter](https://github.com/OpenZeppelin/nile/actions/workflows/ci.yml/badge.svg)](https://github.com/OpenZeppelin/nile/actions/workflows/ci.yml)
 
 _Navigate your [StarkNet](https://www.cairo-lang.org/docs/hello_starknet/index.html) projects written in [Cairo](https://cairo-lang.org)._
 
 ## Getting started
@@ -117,16 +133,17 @@
 📦 Registering deployment as my_contract in localhost.deployments.txt
 ```
 
 A few things to notice here:
 
 1. `nile deploy <contract_name>` looks for an artifact with the same name
 2. This created a `localhost.deployments.txt` file storing all data related to my deployment
-3. The `--alias` parameter lets me create an unique identifier for future interactions, if no alias is set then the contract's address can be used as identifier
+3. The `--alias` parameter lets me create a unique identifier for future interactions, if no alias is set then the contract's address can be used as identifier
 4. By default Nile works on local, but you can use the `--network` parameter to interact with `mainnet`, `goerli`, and the default `localhost`.
+5. By default, the ABI corresponding to the contract will be registered with the deployment. To register a different ABI file, use the `--abi` parameter.
 
 ### `declare`
 
 ```sh
 nile declare contract --alias my_contract
 
 🚀 Declaring contract
@@ -134,15 +151,15 @@
 📦 Registering declaration as my_contract in localhost.declarations.txt
 ```
 
 A few things to notice here:
 
 1. `nile declare <contract_name>` looks for an artifact with the same name
 2. This created a `localhost.declarations.txt` file storing all data related to my declarations
-3. The `--alias` parameter lets me create an unique identifier for future interactions, if no alias is set then the contract's address can be used as identifier
+3. The `--alias` parameter lets me create a unique identifier for future interactions, if no alias is set then the contract's address can be used as identifier
 4. By default Nile works on local, but you can use the `--network` parameter to interact with `mainnet`, `goerli`, and the default `localhost`.
 
 ### `setup`
 
 Deploy an Account associated with a given private key.
 
 To avoid accidentally leaking private keys, this command takes an alias instead of the actual private key. This alias is associated with an environmental variable of the same name, whose value is the actual private key.
@@ -384,42 +401,102 @@
 
     # or
     alice, bob, *_ = accounts
     alice.send(...)
     bob.send(...)
 ```
 
-> Please note that the list of accounts include only those that exist in the local `<network>.accounts.json` file.
+> Please note that the list of accounts includes only those that exist in the local `<network>.accounts.json` file. In a recent release we added a flag to the command, to get predeployed accounts if the network you are connected to is a [starknet-devnet](https://github.com/Shard-Labs/starknet-devnet) instance.
+
+### `get-accounts --predeployed`
+
+This flag retrieves the predeployed accounts if the network you are connecting to is a [starknet-devnet](https://github.com/Shard-Labs/starknet-devnet) instance.
+
+You can use it either from the cli:
+
+```sh
+nile get-accounts --predeployed
+```
+
+Or from the nile runtime environment for scripting:
+
+```python
+def run(nre):
+
+    # fetch the list of pre-deployed accounts from devnet
+    accounts = nre.get_accounts(predeployed=True)
+
+    # then
+    accounts[0].send(...)
+
+    # or
+    alice, bob, *_ = accounts
+    alice.send(...)
+    bob.send(...)
+```
+
+### `get-nonce`
+
+Retrieves the nonce for the given contract address (usually an account).
+
+```sh
+nile get-nonce <contract_address>
+```
+
+## Short string literals
+
+From [cairo-lang docs](https://www.cairo-lang.org/docs/how_cairo_works/consts.html#short-string-literals): A short string is a string whose length is at most 31 characters, and therefore can fit into a single field element.
+
+In Nile, arguments to contract calls (calldata) that are neither int nor hex, are treated as short strings and converted automatically to the corresponding felt representation. Because of this, you can run the following from the CLI:
+
+```sh
+nile deploy MyToken 'MyToken name' 'MyToken symbol' (...)
+```
+
+And this is equivalent to passing the felt representation directly like this:
+
+```sh
+nile deploy MyToken 0x4d79546f6b656e206e616d65 0x4d79546f6b656e2073796d626f6c (...)
+```
+
+Note that if you want to pass the token name as a hex or an int, you need to provide the felt representation directly because these values are not interpreted as short strings. You can open a python terminal, and import and use the `str_to_felt` util like this:
+
+```python
+>>> from nile.utils import str_to_felt
+>>>
+>>> str_to_felt('any string')
+460107418789485453340263
+```
 
 ## Extending Nile with plugins
 
 Nile has the possibility of extending its CLI and `NileRuntimeEnvironment` functionalities through plugins. For developing plugins for Nile fork [this plugin example](https://github.com/franalgaba/nile-plugin-example) boilerplate and implement your desired functionality with the provided instructions.
 
 ### How it works
 
 This implementation takes advantage of the native extensibility features of [click](https://click.palletsprojects.com/). Using click and leveraging the Python [entrypoints](https://packaging.python.org/en/latest/specifications/entry-points/) we have a simple manner of handling extension natively on Python environments through dependencies. The plugin implementation on Nile looks for specific Python entrypoints constraints for adding commands.
 
 In order for this implementation to be functional, it is needed by the plugin developer to follow some development guidelines defined in this simple plugin example extending Nile for a dummy greet extension. In a brief explanation the guidelines are as follows:
 
-1. Define a Python module that implement a click command or group:
+1. Define a Python module that implements a click command or group:
 
    ```python
    # First, import click dependency
    import click
 
    # Decorate the method that will be the command name with `click.command`
    @click.command()
    # You can define custom parameters as defined in `click`: https://click.palletsprojects.com/en/7.x/options/
    def my_command():
        # Help message to show with the command
        """
        Subcommand plugin that does something.
        """
        # Done! Now implement your custom functionality in the command
-       click.echo("I'm a plugin overiding a command!")
+       click.echo("I'm a plugin overriding a command!")
    ```
 
 2. Define the plugin entrypoint. In this case using Poetry features in the pyproject.toml file:
 
    ```sh
    # We need to specify that click commands are Poetry entrypoints of type `nile_plugins`. Do not modify this
    [tool.poetry.plugins."nile_plugins"]
```

### Comparing `cairo-nile-0.9.0/RELEASING.md` & `cairo-nile-0.9.1/RELEASING.md`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/setup.cfg` & `cairo-nile-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/src/cairo_nile.egg-info/PKG-INFO` & `cairo-nile-0.9.1/src/cairo_nile.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cairo-nile
-Version: 0.9.0
+Version: 0.9.1
 Summary: StarkNet/Cairo development toolbelt
 Home-page: https://github.com/martriay/nile
 Author: Martin Triay
 Author-email: martriay@gmail.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3.8
@@ -133,16 +133,17 @@
 📦 Registering deployment as my_contract in localhost.deployments.txt
 ```
 
 A few things to notice here:
 
 1. `nile deploy <contract_name>` looks for an artifact with the same name
 2. This created a `localhost.deployments.txt` file storing all data related to my deployment
-3. The `--alias` parameter lets me create an unique identifier for future interactions, if no alias is set then the contract's address can be used as identifier
+3. The `--alias` parameter lets me create a unique identifier for future interactions, if no alias is set then the contract's address can be used as identifier
 4. By default Nile works on local, but you can use the `--network` parameter to interact with `mainnet`, `goerli`, and the default `localhost`.
+5. By default, the ABI corresponding to the contract will be registered with the deployment. To register a different ABI file, use the `--abi` parameter.
 
 ### `declare`
 
 ```sh
 nile declare contract --alias my_contract
 
 🚀 Declaring contract
@@ -150,15 +151,15 @@
 📦 Registering declaration as my_contract in localhost.declarations.txt
 ```
 
 A few things to notice here:
 
 1. `nile declare <contract_name>` looks for an artifact with the same name
 2. This created a `localhost.declarations.txt` file storing all data related to my declarations
-3. The `--alias` parameter lets me create an unique identifier for future interactions, if no alias is set then the contract's address can be used as identifier
+3. The `--alias` parameter lets me create a unique identifier for future interactions, if no alias is set then the contract's address can be used as identifier
 4. By default Nile works on local, but you can use the `--network` parameter to interact with `mainnet`, `goerli`, and the default `localhost`.
 
 ### `setup`
 
 Deploy an Account associated with a given private key.
 
 To avoid accidentally leaking private keys, this command takes an alias instead of the actual private key. This alias is associated with an environmental variable of the same name, whose value is the actual private key.
@@ -400,42 +401,102 @@
 
     # or
     alice, bob, *_ = accounts
     alice.send(...)
     bob.send(...)
 ```
 
-> Please note that the list of accounts include only those that exist in the local `<network>.accounts.json` file.
+> Please note that the list of accounts includes only those that exist in the local `<network>.accounts.json` file. In a recent release we added a flag to the command, to get predeployed accounts if the network you are connected to is a [starknet-devnet](https://github.com/Shard-Labs/starknet-devnet) instance.
+
+### `get-accounts --predeployed`
+
+This flag retrieves the predeployed accounts if the network you are connecting to is a [starknet-devnet](https://github.com/Shard-Labs/starknet-devnet) instance.
+
+You can use it either from the cli:
+
+```sh
+nile get-accounts --predeployed
+```
+
+Or from the nile runtime environment for scripting:
+
+```python
+def run(nre):
+
+    # fetch the list of pre-deployed accounts from devnet
+    accounts = nre.get_accounts(predeployed=True)
+
+    # then
+    accounts[0].send(...)
+
+    # or
+    alice, bob, *_ = accounts
+    alice.send(...)
+    bob.send(...)
+```
+
+### `get-nonce`
+
+Retrieves the nonce for the given contract address (usually an account).
+
+```sh
+nile get-nonce <contract_address>
+```
+
+## Short string literals
+
+From [cairo-lang docs](https://www.cairo-lang.org/docs/how_cairo_works/consts.html#short-string-literals): A short string is a string whose length is at most 31 characters, and therefore can fit into a single field element.
+
+In Nile, arguments to contract calls (calldata) that are neither int nor hex, are treated as short strings and converted automatically to the corresponding felt representation. Because of this, you can run the following from the CLI:
+
+```sh
+nile deploy MyToken 'MyToken name' 'MyToken symbol' (...)
+```
+
+And this is equivalent to passing the felt representation directly like this:
+
+```sh
+nile deploy MyToken 0x4d79546f6b656e206e616d65 0x4d79546f6b656e2073796d626f6c (...)
+```
+
+Note that if you want to pass the token name as a hex or an int, you need to provide the felt representation directly because these values are not interpreted as short strings. You can open a python terminal, and import and use the `str_to_felt` util like this:
+
+```python
+>>> from nile.utils import str_to_felt
+>>>
+>>> str_to_felt('any string')
+460107418789485453340263
+```
 
 ## Extending Nile with plugins
 
 Nile has the possibility of extending its CLI and `NileRuntimeEnvironment` functionalities through plugins. For developing plugins for Nile fork [this plugin example](https://github.com/franalgaba/nile-plugin-example) boilerplate and implement your desired functionality with the provided instructions.
 
 ### How it works
 
 This implementation takes advantage of the native extensibility features of [click](https://click.palletsprojects.com/). Using click and leveraging the Python [entrypoints](https://packaging.python.org/en/latest/specifications/entry-points/) we have a simple manner of handling extension natively on Python environments through dependencies. The plugin implementation on Nile looks for specific Python entrypoints constraints for adding commands.
 
 In order for this implementation to be functional, it is needed by the plugin developer to follow some development guidelines defined in this simple plugin example extending Nile for a dummy greet extension. In a brief explanation the guidelines are as follows:
 
-1. Define a Python module that implement a click command or group:
+1. Define a Python module that implements a click command or group:
 
    ```python
    # First, import click dependency
    import click
 
    # Decorate the method that will be the command name with `click.command`
    @click.command()
    # You can define custom parameters as defined in `click`: https://click.palletsprojects.com/en/7.x/options/
    def my_command():
        # Help message to show with the command
        """
        Subcommand plugin that does something.
        """
        # Done! Now implement your custom functionality in the command
-       click.echo("I'm a plugin overiding a command!")
+       click.echo("I'm a plugin overriding a command!")
    ```
 
 2. Define the plugin entrypoint. In this case using Poetry features in the pyproject.toml file:
 
    ```sh
    # We need to specify that click commands are Poetry entrypoints of type `nile_plugins`. Do not modify this
    [tool.poetry.plugins."nile_plugins"]
```

### Comparing `cairo-nile-0.9.0/src/cairo_nile.egg-info/SOURCES.txt` & `cairo-nile-0.9.1/src/cairo_nile.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -41,23 +41,27 @@
 src/nile/core/plugins.py
 src/nile/core/run.py
 src/nile/core/test.py
 src/nile/core/version.py
 src/nile/utils/__init__.py
 src/nile/utils/debug.py
 src/nile/utils/get_accounts.py
+src/nile/utils/get_nonce.py
+tests/__init__.py
 tests/conftest.py
 tests/test_cli.py
 tests/test_common.py
 tests/test_nre.py
 tests/test_signer.py
 tests/commands/test_account.py
 tests/commands/test_clean.py
 tests/commands/test_compile.py
 tests/commands/test_debug.py
 tests/commands/test_declare.py
 tests/commands/test_deploy.py
 tests/commands/test_get_accounts.py
+tests/commands/test_get_nonce.py
 tests/commands/test_node.py
 tests/core/test_plugins.py
+tests/mocks/mock_response.py
 tests/resources/contracts/contract.cairo
 tests/resources/contracts/contract_with_unwhitelisted_hints.cairo
```

### Comparing `cairo-nile-0.9.0/src/nile/accounts.py` & `cairo-nile-0.9.1/src/nile/accounts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 """nile common module."""
 import json
 import os
 
 from nile.common import ACCOUNTS_FILENAME
+from nile.utils import hex_address, normalize_number
 
 
 def register(pubkey, address, index, alias, network):
     """Register a new account."""
     file = f"{network}.{ACCOUNTS_FILENAME}"
 
     if exists(pubkey, network):
         raise Exception(f"account-{index} already exists in {file}")
 
     with open(file, "r") as fp:
         accounts = json.load(fp)
-        accounts[pubkey] = {"address": address, "index": index, "alias": alias}
+        # Save public key as hex
+        pubkey = hex(pubkey)
+        accounts[pubkey] = {
+            "address": hex_address(address),
+            "index": index,
+            "alias": alias,
+        }
     with open(file, "w") as file:
         json.dump(accounts, file)
 
 
 def exists(pubkey, network):
     """Return whether an account exists or not."""
     account = next(load(pubkey, network), None)
@@ -31,15 +38,18 @@
 
     if not os.path.exists(file):
         with open(file, "w") as fp:
             json.dump({}, fp)
 
     with open(file) as fp:
         accounts = json.load(fp)
+        # pubkey in file is in hex format
+        pubkey = hex(pubkey)
         if pubkey in accounts:
+            accounts[pubkey]["address"] = normalize_number(accounts[pubkey]["address"])
             yield accounts[pubkey]
 
 
 def current_index(network):
     """Return the length of the accounts. Used as the next index."""
     file = f"{network}.{ACCOUNTS_FILENAME}"
```

### Comparing `cairo-nile-0.9.0/src/nile/artifacts/Account.json` & `cairo-nile-0.9.1/src/nile/artifacts/Account.json`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/src/nile/artifacts/abis/Account.json` & `cairo-nile-0.9.1/src/nile/artifacts/abis/Account.json`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/src/nile/base_project/.gitignore` & `cairo-nile-0.9.1/src/nile/base_project/.gitignore`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/src/nile/base_project/contracts/contract.cairo` & `cairo-nile-0.9.1/src/nile/base_project/contracts/contract.cairo`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/src/nile/base_project/tests/test_contract.py` & `cairo-nile-0.9.1/src/nile/base_project/tests/test_contract.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,13 +19,13 @@
 
     # Deploy the contract.
     contract = await starknet.deploy(
         source=CONTRACT_FILE,
     )
 
     # Invoke increase_balance() twice.
-    await contract.increase_balance(amount=10).invoke()
-    await contract.increase_balance(amount=20).invoke()
+    await contract.increase_balance(amount=10).execute()
+    await contract.increase_balance(amount=20).execute()
 
     # Check the result of get_balance().
     execution_info = await contract.get_balance().call()
     assert execution_info.result == (30,)
```

### Comparing `cairo-nile-0.9.0/src/nile/common.py` & `cairo-nile-0.9.1/src/nile/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 """nile common module."""
 import json
 import os
 import re
 import subprocess
 
+from nile.utils import normalize_number, str_to_felt
+
 CONTRACTS_DIRECTORY = "contracts"
 BUILD_DIRECTORY = "artifacts"
 TEMP_DIRECTORY = ".temp"
 ABIS_DIRECTORY = f"{BUILD_DIRECTORY}/abis"
 DEPLOYMENTS_FILENAME = "deployments.txt"
 DECLARATIONS_FILENAME = "declarations.txt"
 ACCOUNTS_FILENAME = "accounts.json"
 NODE_FILENAME = "node.json"
 RETRY_AFTER_SECONDS = 30
 
 
-def _get_gateway():
+def get_gateway():
     """Get the StarkNet node details."""
     try:
         with open(NODE_FILENAME, "r") as f:
             gateway = json.load(f)
             return gateway
 
     except FileNotFoundError:
         with open(NODE_FILENAME, "w") as f:
             f.write('{"localhost": "http://127.0.0.1:5050/"}')
 
 
-GATEWAYS = _get_gateway()
+GATEWAYS = get_gateway()
 
 
 def get_all_contracts(ext=None, directory=None):
     """Get all cairo contracts in the default contract directory."""
     if ext is None:
         ext = ".cairo"
 
@@ -68,41 +70,55 @@
         command.append(f"--gateway_url={GATEWAYS.get(network)}")
 
     command.append("--no_wallet")
 
     return subprocess.check_output(command)
 
 
-def get_nonce(contract_address, network):
-    """Get the current nonce for contract address in a given network."""
-    command = ["starknet", "get_nonce", "--contract_address", contract_address]
-
-    if network == "mainnet":
-        os.environ["STARKNET_NETWORK"] = "alpha-mainnet"
-    elif network == "goerli":
-        os.environ["STARKNET_NETWORK"] = "alpha-goerli"
-    else:
-        command.append(f"--feeder_gateway_url={GATEWAYS.get(network)}")
-
-    return int(subprocess.check_output(command).strip())
-
-
 def parse_information(x):
     """Extract information from deploy/declare command."""
     # address is 64, tx_hash is 64 chars long
     address, tx_hash = re.findall("0x[\\da-f]{1,64}", str(x))
-    return address, tx_hash
+    return normalize_number(address), normalize_number(tx_hash)
 
 
-def stringify(x):
+def stringify(x, process_short_strings=False):
     """Recursively convert list or tuple elements to strings."""
     if isinstance(x, list) or isinstance(x, tuple):
-        return [stringify(y) for y in x]
+        return [stringify(y, process_short_strings) for y in x]
     else:
+        if process_short_strings and is_string(x):
+            return str(str_to_felt(x))
         return str(x)
 
 
 def prepare_params(params):
     """Sanitize call, invoke, and deploy parameters."""
     if params is None:
         params = []
-    return stringify(params)
+    return stringify(params, True)
+
+
+def is_string(param):
+    """Identify a param as string if is not int or hex."""
+    is_int = True
+    is_hex = True
+
+    # convert to integer
+    try:
+        int(param)
+    except Exception:
+        is_int = False
+
+    # convert to hex (starting with 0x)
+    try:
+        assert param.startswith("0x")
+        int(param, 16)
+    except Exception:
+        is_hex = False
+
+    return not is_int and not is_hex
+
+
+def is_alias(param):
+    """Identiy param as alias (instead of address)."""
+    return is_string(param)
```

### Comparing `cairo-nile-0.9.0/src/nile/core/account.py` & `cairo-nile-0.9.1/src/nile/core/account.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,59 @@
 """Command to call or invoke StarkNet smart contracts."""
 import logging
 import os
 
 from dotenv import load_dotenv
 
 from nile import accounts, deployments
-from nile.common import get_nonce
+from nile.common import is_alias
 from nile.core.call_or_invoke import call_or_invoke
 from nile.core.deploy import deploy
+from nile.utils import normalize_number
+from nile.utils.get_nonce import get_nonce_without_log as get_nonce
 
 try:
     from nile.signer import Signer
 except ImportError:
     pass
 
 load_dotenv()
 
 
 class Account:
     """Account contract abstraction."""
 
-    def __init__(self, signer, network):
+    def __init__(self, signer, network, predeployed_info=None):
         """Get or deploy an Account contract for the given private key."""
         try:
-            self.signer = Signer(int(os.environ[signer]))
-            self.alias = signer
+            if predeployed_info is None:
+                self.signer = Signer(normalize_number(os.environ[signer]))
+                self.alias = signer
+            else:
+                self.signer = Signer(signer)
+                self.alias = predeployed_info["alias"]
+
             self.network = network
         except KeyError:
             logging.error(
                 f"\n❌ Cannot find {signer} in env."
                 "\nCheck spelling and that it exists."
                 "\nTry moving the .env to the root of your project."
             )
             return
 
-        if accounts.exists(str(self.signer.public_key), network):
-            signer_data = next(accounts.load(str(self.signer.public_key), network))
+        self.abi_path = os.path.dirname(os.path.realpath(__file__)).replace(
+            "/core", "/artifacts/abis/Account.json"
+        )
+
+        if predeployed_info is not None:
+            self.address = predeployed_info["address"]
+            self.index = predeployed_info["index"]
+        elif accounts.exists(self.signer.public_key, network):
+            signer_data = next(accounts.load(self.signer.public_key, network))
             self.address = signer_data["address"]
             self.index = signer_data["index"]
         else:
             address, index = self.deploy()
             self.address = address
             self.index = index
 
@@ -47,29 +61,36 @@
         """Deploy an Account contract for the given private key."""
         index = accounts.current_index(self.network)
         pt = os.path.dirname(os.path.realpath(__file__)).replace("/core", "")
         overriding_path = (f"{pt}/artifacts", f"{pt}/artifacts/abis")
 
         address, _ = deploy(
             "Account",
-            [str(self.signer.public_key)],
+            [self.signer.public_key],
             self.network,
             f"account-{index}",
             overriding_path,
         )
 
         accounts.register(
             self.signer.public_key, address, index, self.alias, self.network
         )
 
         return address, index
 
-    def send(self, to, method, calldata, max_fee, nonce=None):
+    def send(self, address_or_alias, method, calldata, max_fee, nonce=None):
         """Execute a tx going through an Account contract."""
-        target_address, _ = next(deployments.load(to, self.network)) or to
+        if not is_alias(address_or_alias):
+            address_or_alias = normalize_number(address_or_alias)
+
+        target_address, _ = (
+            next(deployments.load(address_or_alias, self.network), None)
+            or address_or_alias
+        )
+
         calldata = [int(x) for x in calldata]
 
         if nonce is None:
             nonce = get_nonce(self.address, self.network)
 
         if max_fee is None:
             max_fee = 0
@@ -80,15 +101,15 @@
             sender=self.address,
             calls=[[target_address, method, calldata]],
             nonce=nonce,
             max_fee=max_fee,
         )
 
         return call_or_invoke(
-            contract=self.address,
+            contract=self,
             type="invoke",
             method="__execute__",
             params=calldata,
             network=self.network,
             signature=[str(sig_r), str(sig_s)],
             max_fee=str(max_fee),
         )
```

### Comparing `cairo-nile-0.9.0/src/nile/core/call_or_invoke.py` & `cairo-nile-0.9.1/src/nile/core/call_or_invoke.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 """Command to call or invoke StarkNet smart contracts."""
 import logging
 import os
 import subprocess
 
 from nile import deployments
 from nile.common import GATEWAYS, prepare_params
+from nile.core import account
+from nile.utils import hex_address
 
 
 def call_or_invoke(
     contract, type, method, params, network, signature=None, max_fee=None
 ):
     """Call or invoke functions of StarkNet smart contracts."""
-    address, abi = next(deployments.load(contract, network))
+    if isinstance(contract, account.Account):
+        address = contract.address
+        abi = contract.abi_path
+    else:
+        address, abi = next(deployments.load(contract, network))
 
+    address = hex_address(address)
     command = [
         "starknet",
         type,
         "--address",
         address,
         "--abi",
         abi,
```

### Comparing `cairo-nile-0.9.0/src/nile/core/clean.py` & `cairo-nile-0.9.1/src/nile/core/clean.py`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/src/nile/core/compile.py` & `cairo-nile-0.9.1/src/nile/core/compile.py`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/src/nile/core/declare.py` & `cairo-nile-0.9.1/src/nile/core/declare.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 
     if alias_exists(alias, network):
         file = f"{network}.{DECLARATIONS_FILENAME}"
         raise Exception(f"Alias {alias} already exists in {file}")
 
     output = run_command(contract_name, network, overriding_path, operation="declare")
     class_hash, tx_hash = parse_information(output)
-    logging.info(f"⏳ Declaration of {contract_name} successfully sent at {class_hash}")
-    logging.info(f"🧾 Transaction hash: {tx_hash}")
+    logging.info(
+        f"⏳ Declaration of {contract_name} successfully sent at {hex(class_hash)}"
+    )
+    logging.info(f"🧾 Transaction hash: {hex(tx_hash)}")
 
     deployments.register_class_hash(class_hash, network, alias)
     return class_hash
 
 
 def alias_exists(alias, network):
     """Return whether an alias exists or not."""
```

### Comparing `cairo-nile-0.9.0/src/nile/core/deploy.py` & `cairo-nile-0.9.1/src/nile/core/deploy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Command to deploy StarkNet smart contracts."""
 import logging
 
 from nile import deployments
 from nile.common import ABIS_DIRECTORY, BUILD_DIRECTORY, parse_information, run_command
+from nile.utils import hex_address
 
 
-def deploy(contract_name, arguments, network, alias, overriding_path=None):
+def deploy(contract_name, arguments, network, alias, overriding_path=None, abi=None):
     """Deploy StarkNet smart contracts."""
     logging.info(f"🚀 Deploying {contract_name}")
     base_path = (
         overriding_path if overriding_path else (BUILD_DIRECTORY, ABIS_DIRECTORY)
     )
-    abi = f"{base_path[1]}/{contract_name}.json"
+    register_abi = abi if abi is not None else f"{base_path[1]}/{contract_name}.json"
 
     output = run_command(contract_name, network, overriding_path, arguments=arguments)
 
     address, tx_hash = parse_information(output)
-    logging.info(f"⏳ ️Deployment of {contract_name} successfully sent at {address}")
-    logging.info(f"🧾 Transaction hash: {tx_hash}")
+    logging.info(
+        f"⏳ ️Deployment of {contract_name} successfully sent at {hex_address(address)}"
+    )
+    logging.info(f"🧾 Transaction hash: {hex(tx_hash)}")
 
-    deployments.register(address, abi, network, alias)
-    return address, abi
+    deployments.register(address, register_abi, network, alias)
+    return address, register_abi
```

### Comparing `cairo-nile-0.9.0/src/nile/core/init.py` & `cairo-nile-0.9.1/src/nile/core/init.py`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/src/nile/core/node.py` & `cairo-nile-0.9.1/src/nile/core/node.py`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/src/nile/core/plugins.py` & `cairo-nile-0.9.1/src/nile/core/plugins.py`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/src/nile/core/test.py` & `cairo-nile-0.9.1/src/nile/core/test.py`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/src/nile/deployments.py` & `cairo-nile-0.9.1/src/nile/deployments.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """nile common module."""
 import logging
 import os
 
 from nile.common import DECLARATIONS_FILENAME, DEPLOYMENTS_FILENAME
+from nile.utils import hex_address, normalize_number
 
 
 def register(address, abi, network, alias):
     """Register a new deployment."""
     file = f"{network}.{DEPLOYMENTS_FILENAME}"
 
     if alias is not None:
         if exists(alias, network):
             raise Exception(f"Alias {alias} already exists in {file}")
 
     with open(file, "a") as fp:
+        # Save address as hex
+        address = hex_address(address)
         if alias is not None:
             logging.info(f"📦 Registering deployment as {alias} in {file}")
         else:
             logging.info(f"📦 Registering {address} in {file}")
 
         fp.write(f"{address}:{abi}")
         if alias is not None:
@@ -29,58 +32,84 @@
     """Register a new deployment."""
     file = f"{network}.{DECLARATIONS_FILENAME}"
 
     if class_hash_exists(hash, network):
         raise Exception(f"Hash {hash[:6]}...{hash[-6:]} already exists in {file}")
 
     with open(file, "a") as fp:
+        # Save class_hash as hex
+        hash = hex(hash)
         if alias is not None:
             logging.info(f"📦 Registering {alias} in {file}")
         else:
             logging.info(f"📦 Registering {hash} in {file}")
 
         fp.write(f"{hash}")
         if alias is not None:
             fp.write(f":{alias}")
         fp.write("\n")
 
 
-def exists(identifier, network):
-    """Return whether a deployment exists or not."""
-    foo = next(load(identifier, network), None)
-    return foo is not None
+def exists(address_or_alias, network):
+    """
+    Return whether a deployment exists or not.
+
+    If address_or_alias is an int, address is assumed.
+
+    If address_or_alias is a str, alias is assumed.
+    """
+    deployment = next(load(address_or_alias, network), None)
+    return deployment is not None
 
 
 def class_hash_exists(hash, network):
     """Return whether a class declaration exists or not."""
     if hash in load_class(hash, network):
         return True
 
 
-def load(identifier, network):
-    """Load deployments that matches an identifier (address or alias)."""
+def load(address_or_alias, network):
+    """
+    Load deployments that matches an identifier (address or alias).
+
+    If address_or_alias is an int, address is assumed.
+
+    If address_or_alias is a str, alias is assumed.
+    """
     file = f"{network}.{DEPLOYMENTS_FILENAME}"
 
     if not os.path.exists(file):
         return
 
     with open(file) as fp:
         for line in fp:
             [address, abi, *alias] = line.strip().split(":")
-            identifiers = [x for x in [address] + alias]
-            if identifier in identifiers:
+            address = normalize_number(address)
+            identifiers = [address]
+            if type(address_or_alias) is not int:
+                identifiers = alias
+            if address_or_alias in identifiers:
                 yield address, abi
 
 
-def load_class(identifier, network):
-    """Load declaration class that matches an identifier (hash or alias)."""
+def load_class(hash_or_alias, network):
+    """
+    Load declaration class that matches an identifier (hash or alias).
+
+    If hash_or_alias is an int, class_hash is assumed.
+
+    If hash_or_alias is a str, alias is assumed.
+    """
     file = f"{network}.{DECLARATIONS_FILENAME}"
 
     if not os.path.exists(file):
         return
 
     with open(file) as fp:
         for line in fp:
             [hash, *alias] = line.strip().split(":")
-            identifiers = [x for x in [hash] + alias]
-            if identifier in identifiers:
+            hash = normalize_number(hash)
+            identifiers = [hash]
+            if type(hash_or_alias) is not int:
+                identifiers = alias
+            if hash_or_alias in identifiers:
                 yield hash
```

### Comparing `cairo-nile-0.9.0/src/nile/nre.py` & `cairo-nile-0.9.1/src/nile/nre.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """nile runtime environment."""
 from nile import deployments
+from nile.common import is_alias
 from nile.core.account import Account
 from nile.core.call_or_invoke import call_or_invoke
 from nile.core.compile import compile
 from nile.core.declare import declare
 from nile.core.deploy import deploy
 from nile.core.plugins import get_installed_plugins, skip_click_exit
-from nile.utils.get_accounts import get_accounts
+from nile.utils import normalize_number
+from nile.utils.get_accounts import get_accounts, get_predeployed_accounts
+from nile.utils.get_nonce import get_nonce
 
 
 class NileRuntimeEnvironment:
     """The NileRuntimeEnvironment exposes Nile functionality when running a script."""
 
     def __init__(self, network="localhost"):
         """Construct NRE object."""
@@ -22,36 +25,55 @@
         """Compile a list of contracts."""
         return compile(contracts)
 
     def declare(self, contract, alias=None, overriding_path=None):
         """Declare a smart contract class."""
         return declare(contract, self.network, alias)
 
-    def deploy(self, contract, arguments=None, alias=None, overriding_path=None):
+    def deploy(
+        self, contract, arguments=None, alias=None, overriding_path=None, abi=None
+    ):
         """Deploy a smart contract."""
-        return deploy(contract, arguments, self.network, alias, overriding_path)
+        return deploy(
+            contract, arguments, self.network, alias, overriding_path, abi=abi
+        )
 
-    def call(self, contract, method, params=None):
+    def call(self, address_or_alias, method, params=None):
         """Call a view function in a smart contract."""
+        if not is_alias(address_or_alias):
+            address_or_alias = normalize_number(address_or_alias)
         return str(
-            call_or_invoke(contract, "call", method, params, self.network)
+            call_or_invoke(address_or_alias, "call", method, params, self.network)
         ).split()
 
-    def invoke(self, contract, method, params=None):
+    def invoke(self, address_or_alias, method, params=None):
         """Invoke a mutable function in a smart contract."""
-        return call_or_invoke(contract, "invoke", method, params, self.network)
+        if not is_alias(address_or_alias):
+            address_or_alias = normalize_number(address_or_alias)
+        return call_or_invoke(address_or_alias, "invoke", method, params, self.network)
 
-    def get_deployment(self, identifier):
+    def get_deployment(self, address_or_alias):
         """Get a deployment by its identifier (address or alias)."""
-        return next(deployments.load(identifier, self.network))
+        if not is_alias(address_or_alias):
+            address_or_alias = normalize_number(address_or_alias)
+        return next(deployments.load(address_or_alias, self.network))
 
-    def get_declaration(self, identifier):
+    def get_declaration(self, address_or_alias):
         """Get a declared class by its identifier (class hash or alias)."""
-        return next(deployments.load_class(identifier, self.network))
+        if not is_alias(address_or_alias):
+            address_or_alias = normalize_number(address_or_alias)
+        return next(deployments.load_class(address_or_alias, self.network))
 
     def get_or_deploy_account(self, signer):
         """Get or deploy an Account contract."""
         return Account(signer, self.network)
 
-    def get_accounts(self):
+    def get_accounts(self, predeployed=False):
         """Retrieve and manage deployed accounts."""
-        return get_accounts(self.network)
+        if not predeployed:
+            return get_accounts(self.network)
+        else:
+            return get_predeployed_accounts(self.network)
+
+    def get_nonce(self, contract_address):
+        """Retrieve the nonce for a contract."""
+        return get_nonce(contract_address, self.network)
```

### Comparing `cairo-nile-0.9.0/src/nile/signer.py` & `cairo-nile-0.9.1/src/nile/signer.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 def from_call_to_call_array(calls):
     """Transform from Call to CallArray."""
     call_array = []
     calldata = []
     for _, call in enumerate(calls):
         assert len(call) == 3, "Invalid call parameters"
         entry = (
-            int(call[0], 16),
+            call[0],
             get_selector_from_name(call[1]),
             len(calldata),
             len(call[2]),
         )
         call_array.append(entry)
         calldata.extend(call[2])
     return (call_array, calldata)
```

### Comparing `cairo-nile-0.9.0/src/nile/utils/__init__.py` & `cairo-nile-0.9.1/src/nile/utils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -112,7 +112,29 @@
         Event(
             from_address=from_address,
             keys=[get_selector_from_name(name)],
             data=data,
         )
         in tx_exec_info.raw_events
     )
+
+
+def normalize_number(number):
+    """Normalize hex or int to int."""
+    if type(number) == str and number.startswith("0x"):
+        return int(number, 16)
+    else:
+        return int(number)
+
+
+def hex_address(number):
+    """Return the 64 hexadecimal characters length address."""
+    if type(number) == str and number.startswith("0x"):
+        return _pad_hex_to_64(number)
+    else:
+        return _pad_hex_to_64(hex(int(number)))
+
+
+def _pad_hex_to_64(hexadecimal):
+    if len(hexadecimal) < 66:
+        missing_zeros = 66 - len(hexadecimal)
+        return hexadecimal[:2] + missing_zeros * "0" + hexadecimal[2:]
```

### Comparing `cairo-nile-0.9.0/src/nile/utils/debug.py` & `cairo-nile-0.9.1/src/nile/utils/debug.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     GATEWAYS,
     RETRY_AFTER_SECONDS,
 )
 
 
 def debug(tx_hash, network, contracts_file=None):
     """Use available contracts to help locate the error in a rejected transaction."""
-    command = ["starknet", "tx_status", "--hash", tx_hash]
+    # Starknet CLI expects hex strings
+    command = ["starknet", "tx_status", "--hash", hex(tx_hash)]
 
     if network == "mainnet":
         os.environ["STARKNET_NETWORK"] = "alpha-mainnet"
     elif network == "goerli":
         os.environ["STARKNET_NETWORK"] = "alpha-goerli"
     else:
         command.append(f"--feeder_gateway_url={GATEWAYS.get(network)}")
```

### Comparing `cairo-nile-0.9.0/tests/commands/test_account.py` & `cairo-nile-0.9.1/tests/commands/test_account.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for account commands."""
 import logging
-from unittest.mock import MagicMock, patch
+from unittest.mock import ANY, MagicMock, patch
 
 import pytest
 
 from nile.core.account import Account
 
 KEY = "TEST_KEY"
 NETWORK = "goerli"
@@ -35,41 +35,27 @@
     assert (
         "\n❌ Cannot find BAD_KEY in env."
         "\nCheck spelling and that it exists."
         "\nTry moving the .env to the root of your project."
     ) in caplog.text
 
 
-def test_account_multiple_inits_with_same_key():
-    account = Account(KEY, NETWORK)
-    account.deploy()
-    account2 = Account(KEY, NETWORK)
-
-    # Check addresses don't match
-    assert account.address != account2.address
-    # Check indexing
-    assert account.index == 0
-    assert account2.index == 1
-
-
 @patch("nile.core.account.deploy", return_value=(1, 2))
 def test_deploy(mock_deploy):
     account = Account(KEY, NETWORK)
     with patch("nile.core.account.os.path.dirname") as mock_path:
         test_path = "/overriding_path"
         mock_path.return_value.replace.return_value = test_path
 
-        account.deploy()
-
         mock_deploy.assert_called_with(
             "Account",
-            [str(account.signer.public_key)],
+            [account.signer.public_key],
             NETWORK,
-            f"account-{account.index + 1}",
-            (f"{test_path}/artifacts", f"{test_path}/artifacts/abis"),
+            f"account-{account.index}",
+            ANY,
         )
 
 
 @patch("nile.core.account.deploy", return_value=(MOCK_ADDRESS, MOCK_INDEX))
 @patch("nile.core.account.accounts.register")
 def test_deploy_accounts_register(mock_register, mock_deploy):
     account = Account(KEY, NETWORK)
@@ -79,51 +65,49 @@
     )
 
 
 @patch("nile.core.account.get_nonce", return_value=0)
 @patch("nile.core.account.call_or_invoke")
 def test_send_nonce_call(mock_call, mock_nonce):
     account = Account(KEY, NETWORK)
-    contract_address, _ = account.deploy()
 
     # Instead of creating and populating a tmp .txt file, this uses the
     # deployed account address (contract_address) as the target
-    account.send(contract_address, "method", [1, 2, 3], max_fee=1)
+    account.send(account.address, "method", [1, 2, 3], max_fee=1)
 
     # 'call_or_invoke' is called once for '__execute__'
     assert mock_call.call_count == 1
 
     # Check 'get_nonce' call
     mock_nonce.assert_called_once_with(account.address, NETWORK)
 
 
 def test_send_sign_transaction_and_execute():
     account = Account(KEY, NETWORK)
-    contract_address, _ = account.deploy()
 
     calldata = ["111", "222", "333"]
     sig_r, sig_s = [999, 888]
     return_signature = [calldata, sig_r, sig_s]
 
     account.signer.sign_transaction = MagicMock(return_value=return_signature)
 
     with patch("nile.core.account.call_or_invoke") as mock_call:
-        send_args = [contract_address, "method", [1, 2, 3]]
+        send_args = [account.address, "method", [1, 2, 3]]
         nonce = 4
         max_fee = 1
         account.send(*send_args, max_fee, nonce)
 
         # Check values are correctly passed to 'sign_transaction'
         account.signer.sign_transaction.assert_called_once_with(
             calls=[send_args], nonce=nonce, sender=account.address, max_fee=1
         )
 
         # Check values are correctly passed to '__execute__'
         mock_call.assert_called_with(
-            contract=account.address,
+            contract=account,
             max_fee=str(max_fee),
             method="__execute__",
             network=NETWORK,
             params=calldata,
             signature=[str(sig_r), str(sig_s)],
             type="invoke",
         )
```

### Comparing `cairo-nile-0.9.0/tests/commands/test_clean.py` & `cairo-nile-0.9.1/tests/commands/test_clean.py`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/tests/commands/test_compile.py` & `cairo-nile-0.9.1/tests/commands/test_compile.py`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/tests/commands/test_debug.py` & `cairo-nile-0.9.1/tests/commands/test_debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from unittest.mock import patch
 
 import pytest
 
 from nile.common import BUILD_DIRECTORY
 from nile.utils.debug import _abi_to_build_path, _locate_error_lines_with_abis, debug
 
-MOCK_HASH = "0x1234"
+MOCK_HASH = 1234
 NETWORK = "goerli"
 ERROR_MESSAGE = "Error at pc=0:1:\nAn ASSERT_EQ instruction failed: 3 != 0."
 DEBUG_ADDRESS = "0x07826b88e404632d9835ab1ec2076c6cf1910e6ecb2ed270647fc211ff55e76f"
 ABI_PATH = "path/to/abis/test_contract.json"
 ALIAS = "contract_alias"
 MOCK_FILE = 123
```

### Comparing `cairo-nile-0.9.0/tests/commands/test_declare.py` & `cairo-nile-0.9.1/tests/commands/test_declare.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,18 @@
     # check internals
     mock_run_cmd.assert_called_once_with(*exp_command, operation="declare")
     mock_parse.assert_called_once_with(RUN_OUTPUT)
     mock_register.assert_called_once_with(*exp_register)
 
     # check logs
     assert f"🚀 Declaring {CONTRACT}" in caplog.text
-    assert f"⏳ Declaration of {CONTRACT} successfully sent at {HASH}" in caplog.text
-    assert f"🧾 Transaction hash: {TX_HASH}" in caplog.text
+    assert (
+        f"⏳ Declaration of {CONTRACT} successfully sent at {hex(HASH)}" in caplog.text
+    )
+    assert f"🧾 Transaction hash: {hex(TX_HASH)}" in caplog.text
 
 
 @patch("nile.core.declare.alias_exists", return_value=True)
 def test_declare_duplicate_hash(mock_alias_check):
 
     with pytest.raises(Exception) as err:
         declare(ALIAS, NETWORK)
```

### Comparing `cairo-nile-0.9.0/tests/commands/test_deploy.py` & `cairo-nile-0.9.1/tests/commands/test_deploy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,78 @@
 """Tests for deploy command."""
 import logging
 from unittest.mock import patch
 
 import pytest
 
 from nile.core.deploy import ABIS_DIRECTORY, BUILD_DIRECTORY, deploy
+from nile.utils import hex_address
 
 
 @pytest.fixture(autouse=True)
 def tmp_working_dir(monkeypatch, tmp_path):
     monkeypatch.chdir(tmp_path)
     return tmp_path
 
 
 CONTRACT = "contract"
 NETWORK = "goerli"
 ALIAS = "alias"
 ABI = f"{ABIS_DIRECTORY}/{CONTRACT}.json"
+ABI_OVERRIDE = f"{ABIS_DIRECTORY}/override.json"
 BASE_PATH = (BUILD_DIRECTORY, ABIS_DIRECTORY)
 PATH_OVERRIDE = ("artifacts2", ABIS_DIRECTORY)
 RUN_OUTPUT = b"output"
 ARGS = [1, 2, 3]
 ADDRESS = 999
 TX_HASH = 222
 
 
 @pytest.mark.parametrize(
-    "args, exp_command",
+    "args, exp_command, exp_abi",
     [
         (
             [CONTRACT, ARGS, NETWORK, ALIAS],  # args
             [CONTRACT, NETWORK, None],  # expected command
+            ABI,  # expected ABI
         ),
         (
             [CONTRACT, ARGS, NETWORK, ALIAS, PATH_OVERRIDE],  # args
             [CONTRACT, NETWORK, PATH_OVERRIDE],  # expected command
+            ABI,  # expected ABI
+        ),
+        (
+            [CONTRACT, ARGS, NETWORK, ALIAS, None, ABI_OVERRIDE],  # args
+            [CONTRACT, NETWORK, None],  # expected command
+            ABI_OVERRIDE,  # expected ABI
+        ),
+        (
+            [CONTRACT, ARGS, NETWORK, ALIAS, PATH_OVERRIDE, ABI_OVERRIDE],  # args
+            [CONTRACT, NETWORK, PATH_OVERRIDE],  # expected command
+            ABI_OVERRIDE,  # expected ABI
         ),
     ],
 )
 @patch("nile.core.deploy.run_command", return_value=RUN_OUTPUT)
 @patch("nile.core.deploy.parse_information", return_value=[ADDRESS, TX_HASH])
 @patch("nile.core.deploy.deployments.register")
-def test_deploy(mock_register, mock_parse, mock_run_cmd, caplog, args, exp_command):
+def test_deploy(
+    mock_register, mock_parse, mock_run_cmd, caplog, args, exp_command, exp_abi
+):
     logging.getLogger().setLevel(logging.INFO)
 
     # check return values
     res = deploy(*args)
-    assert res == (ADDRESS, ABI)
+    assert res == (ADDRESS, exp_abi)
 
     # check internals
     mock_run_cmd.assert_called_once_with(*exp_command, arguments=ARGS)
     mock_parse.assert_called_once_with(RUN_OUTPUT)
-    mock_register.assert_called_once_with(ADDRESS, ABI, NETWORK, ALIAS)
+    mock_register.assert_called_once_with(ADDRESS, exp_abi, NETWORK, ALIAS)
 
     # check logs
     assert f"🚀 Deploying {CONTRACT}" in caplog.text
-    assert f"⏳ ️Deployment of {CONTRACT} successfully sent at {ADDRESS}" in caplog.text
-    assert f"🧾 Transaction hash: {TX_HASH}" in caplog.text
+    assert (
+        f"⏳ ️Deployment of {CONTRACT} successfully sent at {hex_address(ADDRESS)}"
+        in caplog.text
+    )
+    assert f"🧾 Transaction hash: {hex(TX_HASH)}" in caplog.text
```

### Comparing `cairo-nile-0.9.0/tests/commands/test_get_accounts.py` & `cairo-nile-0.9.1/tests/commands/test_get_accounts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 """Tests for get-accounts command."""
 import logging
 from unittest.mock import MagicMock, patch
 
 import pytest
+from requests.exceptions import MissingSchema
 
 from nile.core.account import Account
-from nile.utils.get_accounts import _check_and_return_account, get_accounts
+from nile.utils import hex_address
+from nile.utils import normalize_number as normalize
+from nile.utils.get_accounts import (
+    _check_and_return_account,
+    get_accounts,
+    get_predeployed_accounts,
+)
+from tests.mocks.mock_response import MockResponse
 
 NETWORK = "goerli"
+GATEWAYS = {"localhost": "http://127.0.0.1:5050/"}
 PUBKEYS = [
-    "883045738439352841478194533192765345509759306772397516907181243450667673002",
-    "661519931401775515888740911132355225260405929679788917190706536765421826262",
+    883045738439352841478194533192765345509759306772397516907181243450667673002,
+    661519931401775515888740911132355225260405929679788917190706536765421826262,
 ]
 ADDRESSES = ["333", "444"]
 INDEXES = [0, 1]
 ALIASES = ["TEST_KEY", "TEST_KEY_2"]
 
 MOCK_ACCOUNTS = {
     PUBKEYS[0]: {
@@ -24,14 +33,26 @@
     },
     PUBKEYS[1]: {
         "address": ADDRESSES[1],
         "index": INDEXES[1],
         "alias": ALIASES[1],
     },
 }
+JSON_DATA = [
+    {
+        "address": normalize("0xaaa1"),
+        "private_key": normalize("0xbbb1"),
+        "public_key": normalize("0xbbb2"),
+    },
+    {
+        "address": normalize("0xaaa2"),
+        "private_key": normalize("0xbbb3"),
+        "public_key": normalize("0xbbb4"),
+    },
+]
 
 
 @pytest.fixture(autouse=True)
 def tmp_working_dir(monkeypatch, tmp_path):
     monkeypatch.chdir(tmp_path)
     return tmp_path
 
@@ -95,15 +116,15 @@
     get_accounts(NETWORK)
 
     # Check total accounts log
     assert f"\nTotal registered accounts: {len(PUBKEYS)}\n" in caplog.text
 
     # Check index/address log
     for i in range(len(PUBKEYS)):
-        assert f"{INDEXES[i]}: {ADDRESSES[i]}" in caplog.text
+        assert f"{INDEXES[i]}: {hex_address(ADDRESSES[i])}" in caplog.text
 
     # Check final success log
     assert "\n🚀 Successfully retrieved deployed accounts" in caplog.text
 
 
 @patch("nile.utils.get_accounts.current_index", MagicMock(return_value=len(PUBKEYS)))
 @patch("nile.utils.get_accounts.open", MagicMock())
@@ -118,9 +139,72 @@
         # Check correct args are passed to `_check_and_receive_account`
         for i in range(len(PUBKEYS)):
             mock_return_account.assert_any_call(ALIASES[i], PUBKEYS[i], NETWORK)
 
         # Assert call count equals correct number of accounts
         assert mock_return_account.call_count == len(PUBKEYS)
 
-        # assert returned accounts array equals correct number of accounts
+        # Assert returned accounts array equals correct number of accounts
         assert len(result) == len(PUBKEYS)
+
+
+@patch("nile.common.get_gateway", return_value=GATEWAYS)
+@patch("nile.utils.get_accounts._check_and_return_account")
+@patch("requests.get", return_value=MockResponse(JSON_DATA, 200))
+def test_get_predeployed_accounts(mock_response, mock_return_account, mock_gateways):
+    result = get_predeployed_accounts("localhost")
+
+    # Assert the correct endpoint is used
+    mock_response.assert_called_once_with(
+        f"{GATEWAYS.get('localhost')}/predeployed_accounts"
+    )
+
+    # Check correct args are passed to `_check_and_receive_account`
+    for i in range(len(JSON_DATA)):
+        predeployed_info = {
+            "address": JSON_DATA[i]["address"],
+            "alias": f"account-{i}",
+            "index": i,
+        }
+        mock_return_account.assert_any_call(
+            JSON_DATA[i]["private_key"],
+            JSON_DATA[i]["public_key"],
+            "localhost",
+            predeployed_info,
+        )
+
+    # Assert call count equals correct number of accounts
+    assert mock_return_account.call_count == len(JSON_DATA)
+
+    # Assert returned accounts array equals correct number of accounts
+    assert len(result) == len(JSON_DATA)
+
+
+@patch("nile.common.get_gateway", return_value=GATEWAYS)
+@patch("nile.utils.get_accounts._check_and_return_account")
+@patch("requests.get", return_value=MockResponse(JSON_DATA, 200))
+def test_get_predeployed_accounts_logging(
+    mock_response, mock_return_account, mock_gateways, caplog
+):
+    # make logs visible to test
+    logger = logging.getLogger()
+
+    logger.setLevel(logging.INFO)
+    get_predeployed_accounts("localhost")
+
+    assert "🚀 Successfully retrieved pre-deployed accounts" in caplog.text
+
+    # test exceptions
+    logger.setLevel(logging.ERROR)
+
+    # test missing schema first
+    mock_response.side_effect = MissingSchema
+    get_predeployed_accounts("localhost")
+
+    assert "❌ Failed to retrieve gateway from provided network" in caplog.text
+
+    # test generic exceptions
+    mock_response.side_effect = Exception
+    get_predeployed_accounts("localhost")
+
+    assert "❌ Error querying the account from the gateway" in caplog.text
+    assert "Check you are connected to a starknet-devnet implementation" in caplog.text
```

### Comparing `cairo-nile-0.9.0/tests/commands/test_node.py` & `cairo-nile-0.9.1/tests/commands/test_node.py`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/tests/core/test_plugins.py` & `cairo-nile-0.9.1/tests/core/test_plugins.py`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/tests/resources/contracts/contract.cairo` & `cairo-nile-0.9.1/tests/resources/contracts/contract.cairo`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/tests/resources/contracts/contract_with_unwhitelisted_hints.cairo` & `cairo-nile-0.9.1/tests/resources/contracts/contract_with_unwhitelisted_hints.cairo`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/tests/test_cli.py` & `cairo-nile-0.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/tests/test_common.py` & `cairo-nile-0.9.1/tests/test_common.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,11 +49,16 @@
 
 
 @pytest.mark.parametrize(
     "args, expected",
     [
         ([], []),
         ([LIST1], [["1", "2", "3"]]),
+        (
+            ["MyToken name", "MyToken symbol"],
+            ["23977024514528806274181721445", "1571358278584159847990373933805420"],
+        ),
+        (["0xbad", 1234, "1234", "bad"], ["0xbad", "1234", "1234", "6447460"]),
     ],
 )
 def test_prepare_params(args, expected):
     assert prepare_params(args) == expected
```

### Comparing `cairo-nile-0.9.0/tests/test_nre.py` & `cairo-nile-0.9.1/tests/test_nre.py`

 * *Files identical despite different names*

### Comparing `cairo-nile-0.9.0/tests/test_signer.py` & `cairo-nile-0.9.1/tests/test_signer.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,28 +28,23 @@
     return await send_transactions(
         signer, account, [(to, selector_name, calldata)], nonce, max_fee
     )
 
 
 async def send_transactions(signer, account, calls, nonce=None, max_fee=0):
     # hexify address before passing to from_call_to_call_array
-    build_calls = []
-    for call in calls:
-        build_call = list(call)
-        build_call[0] = hex(build_call[0])
-        build_calls.append(build_call)
-    raw_invocation = get_raw_invoke(account, build_calls)
+    raw_invocation = get_raw_invoke(account, calls)
     state = raw_invocation.state
 
     if nonce is None:
         nonce = await state.state.get_nonce_at(account.contract_address)
 
     # get signature
     calldata, sig_r, sig_s = signer.sign_transaction(
-        account.contract_address, build_calls, nonce, max_fee
+        account.contract_address, calls, nonce, max_fee
     )
 
     # craft invoke and execute tx
     external_tx = InvokeFunction(
         contract_address=account.contract_address,
         calldata=calldata,
         entry_point_selector=None,
```

### Comparing `cairo-nile-0.9.0/tox.ini` & `cairo-nile-0.9.1/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     TEST_KEY_2 = 4321
 passenv =
     HOME
 extras =
     testing
 deps =
     cairo-lang==0.10.0
-    starknet-devnet==0.3.0
+    starknet-devnet==0.3.1
     # See https://github.com/starkware-libs/cairo-lang/issues/52
     marshmallow-dataclass==8.5.3
 commands =
     pytest {posargs}
 
 [testenv:unit]
 description = Invoke pytest to run unit tests
```

