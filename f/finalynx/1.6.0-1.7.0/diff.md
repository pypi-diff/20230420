# Comparing `tmp/finalynx-1.6.0.tar.gz` & `tmp/finalynx-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalynx-1.6.0.tar", max compression
+gzip compressed data, was "finalynx-1.7.0.tar", max compression
```

## Comparing `finalynx-1.6.0.tar` & `finalynx-1.7.0.tar`

### file list

```diff
@@ -1,77 +1,81 @@
--rw-r--r--   0        0        0    35149 2023-03-31 18:54:01.877124 finalynx-1.6.0/LICENSE
--rw-r--r--   0        0        0     6652 2023-03-31 18:54:01.877124 finalynx-1.6.0/README.md
--rw-r--r--   0        0        0     1261 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/__init__.py
--rw-r--r--   0        0        0      770 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/__main__.py
--rw-r--r--   0        0        0      662 2023-03-31 18:54:03.493129 finalynx-1.6.0/finalynx/__meta__.py
--rw-r--r--   0        0        0      993 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/analyzer/__init__.py
--rw-r--r--   0        0        0      579 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/analyzer/analyzer.py
--rw-r--r--   0        0        0     5465 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/assistant.py
--rw-r--r--   0        0        0      273 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/console.py
--rw-r--r--   0        0        0      424 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/copilot/__init__.py
--rw-r--r--   0        0        0      593 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/copilot/copilot.py
--rw-r--r--   0        0        0      427 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/dashboard/__init__.py
--rw-r--r--   0        0        0     5013 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/dashboard/dashboard.py
--rw-r--r--   0        0        0      891 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/fetch/__init__.py
--rw-r--r--   0        0        0     1095 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/fetch/fetch.py
--rw-r--r--   0        0        0    16256 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/fetch/fetch_finary.py
--rw-r--r--   0        0        0       47 2023-03-31 18:54:02.529125 finalynx-1.6.0/finalynx/finary_api/.git
--rw-r--r--   0        0        0      222 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/.github/dependabot.yml
--rw-r--r--   0        0        0     1905 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/.gitignore
--rw-r--r--   0        0        0     1064 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/LICENSE
--rw-r--r--   0        0        0     5099 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/README.md
--rwxr-xr-x   0        0        0      170 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/check.sh
--rw-r--r--   0        0        0       32 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/credentials.json.tpl
--rw-r--r--   0        0        0      691 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/__init__.py
--rw-r--r--   0        0        0    15625 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/__main__.py
--rw-r--r--   0        0        0      323 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/auth.py
--rw-r--r--   0        0        0      694 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/bank_account_types.py
--rw-r--r--   0        0        0      118 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/constants.py
--rw-r--r--   0        0        0      241 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/crypto_chains.py
--rw-r--r--   0        0        0      824 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/currencies.py
--rw-r--r--   0        0        0      308 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/generic_asset_categories.py
--rw-r--r--   0        0        0     1310 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py
--rw-r--r--   0        0        0     3244 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/importers/cryptocom.py
--rw-r--r--   0        0        0     1204 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py
--rw-r--r--   0        0        0      391 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/institutions.py
--rw-r--r--   0        0        0      511 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/precious_metals.py
--rw-r--r--   0        0        0      494 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/scpis.py
--rw-r--r--   0        0        0     3276 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/securities.py
--rw-r--r--   0        0        0     2308 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/signin.py
--rw-r--r--   0        0        0     4177 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/user_cryptos.py
--rw-r--r--   0        0        0      246 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/user_fonds_euro.py
--rw-r--r--   0        0        0     2024 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/user_generic_assets.py
--rw-r--r--   0        0        0     3653 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/user_holdings_accounts.py
--rw-r--r--   0        0        0      411 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/user_me.py
--rw-r--r--   0        0        0     1670 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/user_portfolio.py
--rw-r--r--   0        0        0     1865 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/user_precious_metals.py
--rw-r--r--   0        0        0      222 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/user_real_estates.py
--rw-r--r--   0        0        0      208 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/user_scpis.py
--rw-r--r--   0        0        0     5680 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/user_securities.py
--rw-r--r--   0        0        0      221 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/user_startups.py
--rw-r--r--   0        0        0      196 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/utils.py
--rw-r--r--   0        0        0     3253 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/finary_api/views.py
--rw-r--r--   0        0        0      478 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/mypy.ini
--rw-r--r--   0        0        0      195 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/requirements-tests.txt
--rw-r--r--   0        0        0       60 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/requirements.txt
--rw-r--r--   0        0        0      224 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/setup.cfg
--rw-r--r--   0        0        0       50 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/tests/data/cryptos.csv
--rw-r--r--   0        0        0      172 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/tests/data/stocks.csv
--rw-r--r--   0        0        0      340 2023-03-31 18:54:02.537125 finalynx-1.6.0/finalynx/finary_api/tests/data/stocks.json
--rw-r--r--   0        0        0      153 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/parse/__init__.py
--rw-r--r--   0        0        0      739 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/parse/json.py
--rw-r--r--   0        0        0     1007 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/parse/parser.py
--rw-r--r--   0        0        0     1921 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/portfolio/__init__.py
--rw-r--r--   0        0        0     3829 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/portfolio/bucket.py
--rw-r--r--   0        0        0      951 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/portfolio/constants.py
--rw-r--r--   0        0        0     5943 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/portfolio/folder.py
--rw-r--r--   0        0        0      422 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/portfolio/hierarchy.py
--rw-r--r--   0        0        0     1709 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/portfolio/line.py
--rw-r--r--   0        0        0     6406 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/portfolio/node.py
--rw-r--r--   0        0        0     1195 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/portfolio/portfolio.py
--rw-r--r--   0        0        0     3529 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/portfolio/render.py
--rw-r--r--   0        0        0    10020 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/portfolio/targets.py
--rw-r--r--   0        0        0      419 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/simulator/__init__.py
--rw-r--r--   0        0        0      720 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/simulator/simulator.py
--rw-r--r--   0        0        0     1705 2023-03-31 18:54:01.897124 finalynx-1.6.0/finalynx/usage.py
--rw-r--r--   0        0        0     1713 2023-03-31 18:54:03.493129 finalynx-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     7539 1970-01-01 00:00:00.000000 finalynx-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-20 08:07:53.173183 finalynx-1.7.0/LICENSE
+-rw-r--r--   0        0        0     6652 2023-04-20 08:07:53.173183 finalynx-1.7.0/README.md
+-rw-r--r--   0        0        0     1340 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/__init__.py
+-rw-r--r--   0        0        0      770 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/__main__.py
+-rw-r--r--   0        0        0      662 2023-04-20 08:07:54.501173 finalynx-1.7.0/finalynx/__meta__.py
+-rw-r--r--   0        0        0      993 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/analyzer/__init__.py
+-rw-r--r--   0        0        0     1101 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/analyzer/analyzer.py
+-rw-r--r--   0        0        0     3187 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/analyzer/asset_class.py
+-rw-r--r--   0        0        0     2398 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/analyzer/envelopes.py
+-rw-r--r--   0        0        0     2858 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/analyzer/investment_state.py
+-rw-r--r--   0        0        0     5506 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/assistant.py
+-rw-r--r--   0        0        0      273 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/console.py
+-rw-r--r--   0        0        0      424 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/copilot/__init__.py
+-rw-r--r--   0        0        0      593 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/copilot/copilot.py
+-rw-r--r--   0        0        0      427 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/dashboard/__init__.py
+-rw-r--r--   0        0        0    11345 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/dashboard/dashboard.py
+-rw-r--r--   0        0        0      891 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/fetch/__init__.py
+-rw-r--r--   0        0        0     1095 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/fetch/fetch.py
+-rw-r--r--   0        0        0    16256 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/fetch/fetch_finary.py
+-rw-r--r--   0        0        0       47 2023-04-20 08:07:53.689179 finalynx-1.7.0/finalynx/finary_api/.git
+-rw-r--r--   0        0        0      222 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/.github/dependabot.yml
+-rw-r--r--   0        0        0     1905 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/.gitignore
+-rw-r--r--   0        0        0     1064 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/LICENSE
+-rw-r--r--   0        0        0     5099 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/README.md
+-rwxr-xr-x   0        0        0      170 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/check.sh
+-rw-r--r--   0        0        0       32 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/credentials.json.tpl
+-rw-r--r--   0        0        0      691 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/__init__.py
+-rw-r--r--   0        0        0    15625 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/__main__.py
+-rw-r--r--   0        0        0      323 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/auth.py
+-rw-r--r--   0        0        0      694 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/bank_account_types.py
+-rw-r--r--   0        0        0      118 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/constants.py
+-rw-r--r--   0        0        0      241 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/crypto_chains.py
+-rw-r--r--   0        0        0      824 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/currencies.py
+-rw-r--r--   0        0        0      308 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/generic_asset_categories.py
+-rw-r--r--   0        0        0     1310 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py
+-rw-r--r--   0        0        0     3244 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/importers/cryptocom.py
+-rw-r--r--   0        0        0     1204 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py
+-rw-r--r--   0        0        0      391 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/institutions.py
+-rw-r--r--   0        0        0      511 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/precious_metals.py
+-rw-r--r--   0        0        0      494 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/scpis.py
+-rw-r--r--   0        0        0     3276 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/securities.py
+-rw-r--r--   0        0        0     2308 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/signin.py
+-rw-r--r--   0        0        0     4177 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_cryptos.py
+-rw-r--r--   0        0        0      246 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_fonds_euro.py
+-rw-r--r--   0        0        0     2024 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_generic_assets.py
+-rw-r--r--   0        0        0     3653 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_holdings_accounts.py
+-rw-r--r--   0        0        0      411 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_me.py
+-rw-r--r--   0        0        0     1670 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_portfolio.py
+-rw-r--r--   0        0        0     1865 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_precious_metals.py
+-rw-r--r--   0        0        0      222 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_real_estates.py
+-rw-r--r--   0        0        0      208 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_scpis.py
+-rw-r--r--   0        0        0     5680 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_securities.py
+-rw-r--r--   0        0        0      221 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/user_startups.py
+-rw-r--r--   0        0        0      196 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/utils.py
+-rw-r--r--   0        0        0     3253 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/finary_api/views.py
+-rw-r--r--   0        0        0      478 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/mypy.ini
+-rw-r--r--   0        0        0      195 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/requirements-tests.txt
+-rw-r--r--   0        0        0       60 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/requirements.txt
+-rw-r--r--   0        0        0      224 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/setup.cfg
+-rw-r--r--   0        0        0       50 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/tests/data/cryptos.csv
+-rw-r--r--   0        0        0      172 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/tests/data/stocks.csv
+-rw-r--r--   0        0        0      340 2023-04-20 08:07:53.697179 finalynx-1.7.0/finalynx/finary_api/tests/data/stocks.json
+-rw-r--r--   0        0        0      153 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/parse/__init__.py
+-rw-r--r--   0        0        0      739 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/parse/json.py
+-rw-r--r--   0        0        0     1007 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/parse/parser.py
+-rw-r--r--   0        0        0     2016 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/__init__.py
+-rw-r--r--   0        0        0     4675 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/bucket.py
+-rw-r--r--   0        0        0      860 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/constants.py
+-rw-r--r--   0        0        0     2133 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/envelope.py
+-rw-r--r--   0        0        0     6934 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/folder.py
+-rw-r--r--   0        0        0      422 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/hierarchy.py
+-rw-r--r--   0        0        0     2436 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/line.py
+-rw-r--r--   0        0        0     6833 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/node.py
+-rw-r--r--   0        0        0     1195 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/portfolio.py
+-rw-r--r--   0        0        0     3529 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/render.py
+-rw-r--r--   0        0        0    11163 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/portfolio/targets.py
+-rw-r--r--   0        0        0      419 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/simulator/__init__.py
+-rw-r--r--   0        0        0     2262 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/simulator/simulator.py
+-rw-r--r--   0        0        0     1705 2023-04-20 08:07:53.193183 finalynx-1.7.0/finalynx/usage.py
+-rw-r--r--   0        0        0     1713 2023-04-20 08:07:54.501173 finalynx-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7539 1970-01-01 00:00:00.000000 finalynx-1.7.0/PKG-INFO
```

### Comparing `finalynx-1.6.0/LICENSE` & `finalynx-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/README.md` & `finalynx-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/__init__.py` & `finalynx-1.7.0/finalynx/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 # Add finary_api submodule to path to allow imports to work
 sys.path.append(os.path.join(os.path.dirname(__file__), "finary_api"))
 
 # Portfolio
 from .portfolio import TargetRange, TargetMin, TargetMax, TargetRatio, TargetGlobalRatio
 from .portfolio import Line, Folder, Bucket, SharedFolder, Portfolio, FolderDisplay
-from .portfolio import console
+from .portfolio import AssetClass, EnvelopeClass
+from .portfolio import Envelope, EnvelopeState, PEA, AV, PER
 
 # Fetch
 from .fetch import FetchFinary
 
 # Advisor
 from .copilot import Copilot
```

### Comparing `finalynx-1.6.0/finalynx/__main__.py` & `finalynx-1.7.0/finalynx/__main__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/__meta__.py` & `finalynx-1.7.0/finalynx/__meta__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ```{warning}
 Do not manually change this information.
 ```
 
 Metadata information about Finalynx. This file is used by Fynalinx and updated by the CI/CD pipeline.
 """
 
-__version__ = "1.6.0"
+__version__ = "1.7.0"
 
 __author__ = "Pierre Laclau (MadeInPierre)"
 
 __copyright__ = """
 Copyright (c) 2023, MadeInPierre
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
```

### Comparing `finalynx-1.6.0/finalynx/analyzer/__init__.py` & `finalynx-1.7.0/finalynx/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/assistant.py` & `finalynx-1.7.0/finalynx/assistant.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Optional
 
 from docopt import docopt
-from finalynx import console
 from finalynx import Copilot
 from finalynx import Dashboard
 from finalynx import FetchFinary
 from finalynx import Portfolio
 from finalynx import Simulator
 from rich import inspect  # noqa F401
 from rich import pretty
 from rich import print  # noqa F401
 from rich import traceback
 from rich.columns import Columns
 from rich.panel import Panel
 
 from .__meta__ import __version__
+from .console import console
 from .usage import __doc__
 
 # Enable rich's features
 
 traceback.install()
 pretty.install()
 
@@ -113,15 +113,17 @@
         # Get recommendations for immediate investment operations
         recommentations = self.copilot.rich_recommendations(self.portfolio)  # noqa TODO
 
         # Final set of results to be displayed
         panels = [
             Panel(
                 self.portfolio.tree(
-                    output_format=self.output_format, hide_root=self.hide_root, hide_amounts=self.hide_amounts
+                    output_format=self.output_format,
+                    hide_root=self.hide_root,
+                    hide_amounts=self.hide_amounts,
                 ),
                 title=self.portfolio.name,
                 padding=(1, 4),
             ),
             # Panel(simulation, title='Simulation'),   # TODO Coming soon
             # Panel(recommendations, title='Advisor'), # TODO Coming soon
         ]
```

### Comparing `finalynx-1.6.0/finalynx/copilot/copilot.py` & `finalynx-1.7.0/finalynx/copilot/copilot.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/fetch/__init__.py` & `finalynx-1.7.0/finalynx/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/fetch/fetch.py` & `finalynx-1.7.0/finalynx/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/fetch/fetch_finary.py` & `finalynx-1.7.0/finalynx/fetch/fetch_finary.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/.gitignore` & `finalynx-1.7.0/finalynx/finary_api/.gitignore`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/LICENSE` & `finalynx-1.7.0/finalynx/finary_api/LICENSE`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/README.md` & `finalynx-1.7.0/finalynx/finary_api/README.md`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/__init__.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/__main__.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/__main__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/bank_account_types.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/bank_account_types.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/currencies.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/currencies.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/importers/cryptocom.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/importers/cryptocom.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/securities.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/securities.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/signin.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/signin.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/user_cryptos.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/user_cryptos.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/user_generic_assets.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/user_generic_assets.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/user_holdings_accounts.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/user_holdings_accounts.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/user_portfolio.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/user_portfolio.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/user_precious_metals.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/user_precious_metals.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/user_securities.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/user_securities.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/finary_api/finary_api/views.py` & `finalynx-1.7.0/finalynx/finary_api/finary_api/views.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/parse/json.py` & `finalynx-1.7.0/finalynx/parse/json.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/parse/parser.py` & `finalynx-1.7.0/finalynx/parse/parser.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/portfolio/__init__.py` & `finalynx-1.7.0/finalynx/portfolio/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 `constants` is not used for now, but may soon be the basis of future `Envelope` objects.
 ```
 """
 # flake8: noqa
 from ..console import console
 from .bucket import Bucket
 from .bucket import SharedFolder
+from .constants import AssetClass
+from .constants import EnvelopeClass
+from .envelope import *
 from .folder import Folder
 from .folder import FolderDisplay
 from .hierarchy import Hierarchy
 from .line import Line
 from .node import Node
 from .portfolio import Portfolio
 from .targets import *
```

### Comparing `finalynx-1.6.0/finalynx/portfolio/bucket.py` & `finalynx-1.7.0/finalynx/portfolio/bucket.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import TYPE_CHECKING
 
 import numpy as np
 
+from .constants import AssetClass
 from .folder import Folder
 from .folder import FolderDisplay
+from .line import Line
 
 if TYPE_CHECKING:
     from .targets import Target
-    from .line import Line
 
 
 class Bucket:
     """
     Holds a list of `Line` objects to represent a group of investments that hold the same purpose.
 
     Once defined with a list of lines, there is nothing else to do from a user perspective.
@@ -79,27 +80,46 @@
 
 
 class SharedFolder(Folder):
     def __init__(
         self,
         name: str,
         bucket: Bucket,
+        asset_class: AssetClass = AssetClass.UNKNOWN,
         target_amount: float = np.inf,
         parent: Optional["Folder"] = None,
         target: Optional["Target"] = None,
         newline: bool = False,
         display: FolderDisplay = FolderDisplay.EXPANDED,
     ):
-        super().__init__(name, parent, target, bucket.lines, newline=False, display=display)  # type: ignore # TODO couldn't fix the mypy error
+        super().__init__(name, asset_class, parent, target, bucket.lines, newline=False, display=display)  # type: ignore # TODO couldn't fix the mypy error
         self.target_amount = target_amount
         self.newline = newline
         self.bucket = bucket
 
     def process(self) -> None:
         super().process()  # Process children
         self.children = self.bucket.use_amount(self.target_amount)  # type: ignore # TODO couldn't fix the mypy error
 
         for child in self.children:
             child.set_parent(self)
 
         if self.children:
             self.children[-1].newline = self.newline
+
+    def set_child_amount(self, key: str, amount: float) -> bool:
+        """Used by the `fetch` subpackage to
+
+        This method passes down the vey:value pair corresponding to an investment fetched online
+        (e.g. in your Finary account) to its children until a match is found.
+
+        :param key: Name of the line in the online account.
+        :param amount: Fetched amount in the online account.
+        """
+        success = False
+        for child in self.children:
+            if isinstance(child, Line) and child.key == key:
+                child.amount = amount
+                success = True
+            elif isinstance(child, Folder) and child.set_child_amount(key, amount):
+                success = True
+        return success
```

### Comparing `finalynx-1.6.0/finalynx/portfolio/constants.py` & `finalynx-1.7.0/finalynx/portfolio/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,35 +4,30 @@
 These enumerations are not yet used in Finalynx, but will serve as the basis for the `Analyzer`
 subpackage to classify lines and show relevant statistics.
 ```
 """
 from enum import Enum
 
 
-class AssetType(Enum):
+class AssetClass(Enum):
     """Enumeration that defines the asset class for each line."""
 
-    CCP = "CCP"
-    LIVRET = "Livret"
+    CASH = "Cash"
+    LIVRET = "Livrets"
     FOND_EURO = "Fonds euro"
-    ETF = "ETF"
-    STOCK = "Action"
-    OBLIGATION = "Obligation"
-    CROWDFUNDING = "Crowdfunding"
+    BOND = "Obligations"
+    STOCK = "Actions"
+    REAL_ESTATE = "Immobilier"
     GOLD = "Or"
-    SILVER = "Argent"
-    PILOTED = "Gestion pilotee"
     CRYPTO = "Cryptos"
-    FOREST = "Forets"
-    SCPI = "SCPI"
-    HOUSING = "Immobilier"
-    PASSIVE = "Passif"
+    PASSIVE = "Passifs"
+    UNKNOWN = "Inconnu"
 
 
-class EnvelopeType(Enum):
+class EnvelopeClass(Enum):  # TODO use or remove?
     """Enumeration that defines the envelope types that hold each line."""
 
     CCP = "CCP"
     LIVRET = "Livret"
     AV = "AV"
     PEA = "PEA"
     CTO = "CTO"
```

### Comparing `finalynx-1.6.0/finalynx/portfolio/folder.py` & `finalynx-1.7.0/finalynx/portfolio/folder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from enum import Enum
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import TYPE_CHECKING
 
 import numpy as np
+from finalynx.console import console
+from finalynx.portfolio.targets import TargetRatio
 from rich.tree import Tree
 
+from .constants import AssetClass
 from .line import Line
 from .node import Node
 
 if TYPE_CHECKING:
     from .targets import Target
 
 
@@ -30,14 +33,15 @@
 
 class Folder(Node):
     """Holds a group of `Node` objects to build the portfolio hierarchy."""
 
     def __init__(
         self,
         name: str,
+        asset_class: AssetClass = AssetClass.UNKNOWN,
         parent: Optional["Folder"] = None,
         target: Optional["Target"] = None,
         children: Optional[List["Node"]] = None,
         newline: bool = False,
         display: FolderDisplay = FolderDisplay.EXPANDED,
     ):
         """
@@ -57,14 +61,16 @@
         super().__init__(name, parent, target, newline)
         self.children = [] if children is None else children
         self.display = display
 
         for child in self.children:
             child.set_parent(self)
 
+        self.set_children_class(asset_class)
+
     def add_child(self, child: Node) -> None:
         """Manually add a child at the end of the existing children in this folder.
         :param child: Any `Node` object to add as a child.
         :returns: Nohing to return.
         """
         child.set_parent(self)
         self.children.append(child)
@@ -76,15 +82,15 @@
         return float(np.sum([child.get_amount() for child in self.children]) if self.children else 0)
 
     def tree(
         self,
         output_format: str = "[console]",
         _tree: Optional[Tree] = None,
         hide_root: bool = False,
-        **render_args: Any
+        **render_args: Any,
     ) -> Tree:
         """Generate a fully rendered `Tree` object from the `rich` package using the
 
         This `Tree` can either be manipulated for further operations or directly printed
         to the console using rich's `print` method.
 
         :param hide_amount: Replace the amoutns by simple dots (easier to share the result), defaults to False.
@@ -101,45 +107,62 @@
         return node
 
     def process(self) -> None:
         """Some `Node` or `Target` objects might need to process some data once the investment
         values have been fetched from Finary. Folders do not have any processing procedure.
         Here, we only call the `process()` method of all children.
         """
+        total_ratio = 0.0
+
         for child in self.children:
             child.process()
 
+            if isinstance(child.target, TargetRatio):
+                total_ratio += child.target.target_ratio
+
+        if total_ratio != 0 and total_ratio != 100:
+            console.log(f"[yellow][bold]WARNING:[/] Folder '{self.name}' total ratio should sum to 100.")
+
     def set_child_amount(self, key: str, amount: float) -> bool:
         """Used by the `fetch` subpackage to
 
         This method passes down the vey:value pair corresponding to an investment fetched online
         (e.g. in your Finary account) to its children until a match is found.
 
         :param key: Name of the line in the online account.
         :param amount: Fetched amount in the online account.
         """
         success = False
         for child in self.children:
             if isinstance(child, Line) and child.key == key:
-                child.amount = amount
+                child.amount += amount
                 success = True
             elif isinstance(child, Folder) and child.set_child_amount(key, amount):
                 success = True
         return success
 
+    def set_children_class(self, asset_class: AssetClass) -> None:
+        for child in self.children:
+            if isinstance(child, Line):
+                child.asset_class = asset_class if child.asset_class is AssetClass.UNKNOWN else child.asset_class
+            elif isinstance(child, Folder):
+                child.set_children_class(asset_class)
+            else:
+                raise ValueError("Unrecognized node type.")
+
     def _render_name_color(self) -> str:
         """Internal method that overrides the superclass' render method to display
         the folder name with a bold font of different color.
         """
         if self.display == FolderDisplay.EXPANDED:
-            return "[blue bold]"
+            return "[dodger_blue2 bold]"
         elif self.display == FolderDisplay.COLLAPSED:
-            return "[blue]"
+            return "[dodger_blue2]"
         elif self.display == FolderDisplay.LINE:
-            return "[white]"
+            return super()._render_name_color()
         else:
             raise ValueError("Display mode '{self.display}' not recognized.")
 
     def _render_newline(self) -> str:
         """Internal method that overrides the superclass' render method to display
         a new line after the folder has rendered.
         :returns: The newline character depending on the user configuration.
```

### Comparing `finalynx-1.6.0/finalynx/portfolio/node.py` & `finalynx-1.7.0/finalynx/portfolio/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,24 +46,28 @@
 
         if target is not None:
             target.set_parent(self)
 
         # Setup custom aliases for node rendering
         render_aliases: Dict[str, str] = {
             "[text]": "[target_text][prehint] [name] [hint][newline]",
-            "[console]": "[target][dim white][prehint][/] [name_color][name][/] [dim white][hint][/][newline]",
-            "[dashboard]": "[amount] [currency] [name]",
-            "[target_text]": "[target_symbol] [amount] [currency]",
+            "[console]": "[target][dim white][prehint][/] [account_code][name_color][name][/] [dim white][hint][/][newline]",
+            "[console_targets]": "[bold green][goal][/][account_code][name_color][name][/][newline]",
+            "[text_targets]": "[goal][name][newline]",
+            "[dashboard_tree]": "[amount] [currency] [name]",
+            "[dashboard_console]": "[bold][target][/][bright_black][prehint][/] [name_color][name][/] [bright_black][hint][/][newline]",
             "[target]": "[[target_color]][target_text][/]",
+            "[target_text]": "[target_symbol] [amount] [currency]",
         }
         render_agents: Dict[str, Callable[..., str]] = {
             "name": self._render_name,
             "name_color": self._render_name_color,
             "newline": self._render_newline,
             "amount": self._render_amount,
+            "goal": self._render_goal,
             "hint": self._render_hint,
             "prehint": self._render_prehint,
             "currency": self._render_currency,
             "target_symbol": self.target._render_target_symbol,
             "target_color": self.target._render_target_color,
         }
         render_aliases.update(aliases if aliases else {})
@@ -109,36 +113,39 @@
     def _render_hint(self) -> str:
         """:returns: A formatted rendering of a hint message (at the end by default)."""
         return self.target.hint() if self.target.check() != Target.RESULT_NONE else ""
 
     def _render_prehint(self) -> str:
         """:returns: A formatted rendering of a pre-hint message (next to the amount by default)."""
         prehint = self.target.prehint()
-        return f" ({prehint})" if prehint else ""
+        return " " + prehint if prehint else ""
 
     def _render_amount(self, hide_amounts: bool = False) -> str:
         """:returns: A formatted rendering of the node amount aligned with the other
         elements in the same parent.
         :param hide_amounts: Replaces amoutn with a dummy amount with dots instead of
         the real amount (easier to share).
         """
         max_length = (
             np.max([len(str(round(c.get_amount()))) for c in self.parent.children])
             if (self.parent and self.parent.children)
             else 0
         )
         return "···" if hide_amounts else f"{round(self.get_amount()):>{max_length}}"
 
+    def _render_goal(self) -> str:
+        return self.target.render_goal()
+
     def _render_name(self) -> str:
         """:returns: A formatted rendering of the node name."""
         return self.name
 
     def _render_name_color(self) -> str:
         """:returns: A formatted rendering of the node name."""
-        return "[white]"
+        return "[black]"
 
     def _render_newline(self) -> str:
         """:returns: A rendering of the newline if set by the user."""
         return "\n" if self.newline else ""
 
     def __repr__(self) -> str:
         """:returns: A console representation of this node for debugging."""
```

### Comparing `finalynx-1.6.0/finalynx/portfolio/portfolio.py` & `finalynx-1.7.0/finalynx/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/portfolio/render.py` & `finalynx-1.7.0/finalynx/portfolio/render.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/finalynx/portfolio/targets.py` & `finalynx-1.7.0/finalynx/portfolio/targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 if TYPE_CHECKING:
     from .node import Node
 
 
 class Target(Hierarchy):
     """Abstract class that defines an objective for a `Node` in the Portfolio tree."""
 
-    RESULT_NOK = {"name": "Not OK", "symbol": "×", "color": "red"}
+    RESULT_NOK = {"name": "NOK", "symbol": "×", "color": "red"}
     RESULT_OK = {"name": "OK", "symbol": "✓", "color": "green"}
     RESULT_TOLERATED = {"name": "Tolerated", "symbol": "≈", "color": "yellow"}
     RESULT_INVEST = {"name": "Invest", "symbol": "↗", "color": "red"}
     RESULT_DEVEST = {"name": "Devest", "symbol": "↘", "color": "magenta"}
     RESULT_START = {"name": "Start", "symbol": "↯", "color": "cyan"}
-    RESULT_NONE = {"name": "No target", "symbol": "‣", "color": "blue"}
+    RESULT_NONE = {"name": "No target", "symbol": "‣", "color": "black"}
 
     def __init__(self) -> None:
         """Abstract Target class that holds the Node parent using this instance and provides
         a common logic for rendering the amounts."""
         super().__init__(parent=None)
         self.parent: Node = self.parent  # Tell mypy this class only has Nodes as parents.
 
@@ -44,27 +44,32 @@
 
     def prehint(self) -> str:
         """Virtual method for information to be printed between the amoutn and the name."""
         return ""
 
     def hint(self) -> str:
         """Virtual method for information to be printed at the end of the parent's description."""
-        return "- Invest!" if self.check() == Target.RESULT_START else "- No target"
+        return "- Invest!" if self.check() == Target.RESULT_START else ""
 
     def render_amount(self, hide_amount: bool = False, n_characters: int = 0) -> str:
         """Check for the parent's amount against the target logic and format the amount based on the target recommendation.
         :param hide_amount: Replace the amounts by simple dots (easier to share the result), defaults to False.
         :param n_characters: Used by `Node` objects to align the amount with other nodes' renders.
         :returns: A string with a righ-formatted render of the parent's amount based on the target recommendation.
         """
         result = self.check()
         result = result if result != True else Target.RESULT_START  # type: ignore # noqa: E712 TODO weird bug??? Workaround for now
         number = f"{round(self.get_amount()):>{n_characters}}" if not hide_amount else "···"
         return f'[{result["color"]}]{result["symbol"]} {number} €[/][dim white]{self.prehint()}[/]'
 
+    def render_goal(self) -> str:
+        """Ideal amount to be reached based on the current target and node
+        position in the tree. Must be overridden by subclasses."""
+        return ""
+
     def _render_target_name(self) -> str:
         """:returns: The name of the target recommentation."""
         return self.check()["name"]
 
     def _render_target_symbol(self) -> str:
         """:returns: The UFT-8 symbol associated to the target recommentation."""
         return self.check()["symbol"]
@@ -100,14 +105,19 @@
             return Target.RESULT_TOLERATED
         elif self._get_variable() <= self.target_max:
             return Target.RESULT_OK
         elif self._get_variable() <= self.target_max + self.tolerance:
             return Target.RESULT_TOLERATED
         return Target.RESULT_DEVEST
 
+    def render_goal(self) -> str:
+        """:returns: The average between target boundaries."""
+        goal_amount = round((self.target_min + self.target_max) / 2)
+        return f"{goal_amount} € "
+
     def _get_variable(self) -> float:
         """Internal method that gives the value to be checked (overriden by subclasses)."""
         return self.get_amount()
 
     def hint(self) -> str:
         """:returns: A formatted description of the target."""
         return f"- Range {self.target_min}-{self.target_max} €"
@@ -119,14 +129,18 @@
     def __init__(self, target_max: float, tolerance: float = 0):
         """This target checks if the amount is below a specified threshold (with an optional tolerance).
         :param target_max: Maximum threshold to get a `RESULT_OK`.
         :param tolerance: If the amount is at most `target_max + tolerance`, the check will return a `RESULT_TOLERATED`.
         """
         super().__init__(0, target_max, tolerance)
 
+    def render_goal(self) -> str:
+        """:returns: The maximum target value."""
+        return f"{self.target_max} € "
+
     def hint(self) -> str:
         """:returns: A formatted description of the target."""
         return f"- Maximum {self.target_max} €"
 
 
 class TargetMin(TargetRange):
     """Target to make sure your node does not go under a specified value."""
@@ -134,14 +148,18 @@
     def __init__(self, target_min: float, tolerance: float = 0):
         """This target checks if the amount is above a specified threshold (with an optional tolerance).
         :param target_min: Minimum threshold to get a `RESULT_OK`.
         :param tolerance: If the amount is at least `target_min - tolerance`, the check will return a `RESULT_TOLERATED`.
         """
         super().__init__(target_min, np.inf, tolerance)
 
+    def render_goal(self) -> str:
+        """:returns: The minimum target value."""
+        return f"{self.target_min} € "
+
     def hint(self) -> str:
         """:returns: A formatted description of the target."""
         return f"- Minimum {self.target_min} €"
 
 
 class TargetRatio(TargetRange):
     """Target to make sure your node represents a specified ratio in a folder."""
@@ -164,14 +182,18 @@
         total = self._get_reference_amount()
         return 100 * self.get_amount() / total if total > 0 else 0
 
     def get_ideal(self) -> int:
         """:returns: How much this amount represents agains the reference in percentage (0-100%)."""
         return round(self._get_reference_amount() * self.target_ratio / 100)
 
+    def render_goal(self) -> str:
+        """:returns: The target ratio as a string."""
+        return f"{self.target_ratio:>2} % "
+
     def _get_variable(self) -> float:
         """:returns: The value to be checked."""
         return self.get_ratio()
 
     def _get_reference_amount(self) -> float:
         """:returns: The value to be checked against (parent's amount)."""
         if not self.parent.parent:
@@ -182,19 +204,27 @@
             return self.parent.parent.target.get_ideal()
 
         # Otherwise, simply get the parent's value
         return self.parent.parent.get_amount()
 
     def prehint(self) -> str:
         """:returns: A rich-formatted view of the calculated percentage."""
-        return f"{round(self.get_ratio()):>2}%"
+        if not self.parent or not self.parent.parent:
+            raise ValueError("Target's parent must be set.")
+
+        max_length = 0
+        for child in self.parent.parent.children:
+            if isinstance(child.target, TargetRatio):
+                max_length = max(max_length, len(str(round(child.target.get_ideal()))))
+
+        return f"→ {self.get_ideal():>{max_length}} €"
 
     def hint(self) -> str:
         """:returns: A formatted description of the target."""
-        return f"→ {self.get_ideal()} € - {self.target_ratio}%"
+        return f"{round(self.get_ratio())}% → {self.target_ratio}%"
 
 
 class TargetGlobalRatio(TargetRatio):
     """Target to make sure your node represents a specified ratio in your portfolio."""
 
     def __init__(self, target_ratio: float, zone: float = 4, tolerance: float = 0):
         """This target checks if the amount represents a specified ratio of the total amount of your entire portfolio.
@@ -210,8 +240,8 @@
         root = self.parent
         while root.parent is not None:
             root = root.parent
         return root.get_amount()
 
     def hint(self) -> str:
         """:returns: A formatted description of the target."""
-        return f"→ Global {self.target_ratio}%"
+        return f"Global {round(self.get_ratio())}% → {self.target_ratio}%"
```

### Comparing `finalynx-1.6.0/finalynx/usage.py` & `finalynx-1.7.0/finalynx/usage.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.6.0/pyproject.toml` & `finalynx-1.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finalynx"
-version = "1.6.0"
+version = "1.7.0"
 description = "A command line investment assistant to organize your portfolio and simulate its future to reach your life goals."
 authors = ["MadeInPierre <pielaclau@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "finalynx"}]
 include = [{ path = "finalynx/finary_api/**/*" }]
 
@@ -48,15 +48,15 @@
 upload_to_pypi = true
 upload_to_release = true
 commit_subject = "chore(release): auto bump version to {version}"
 build_command = "pip install poetry && poetry build"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.6.0"
+version = "1.7.0"
 tag_format = "v$version"
 
 [tool.mypy]
 exclude = [
     "finary_api/*",
     "docs/*",
     "tests/*.py"
```

### Comparing `finalynx-1.6.0/PKG-INFO` & `finalynx-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalynx
-Version: 1.6.0
+Version: 1.7.0
 Summary: A command line investment assistant to organize your portfolio and simulate its future to reach your life goals.
 License: GPLv3
 Author: MadeInPierre
 Author-email: pielaclau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finalynx Version: 1.6.0 Summary: A command line
+Metadata-Version: 2.1 Name: finalynx Version: 1.7.0 Summary: A command line
 investment assistant to organize your portfolio and simulate its future to
 reach your life goals. License: GPLv3 Author: MadeInPierre Author-email:
 pielaclau@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: docopt (==0.6.2)
```

