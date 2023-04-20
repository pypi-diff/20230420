# Comparing `tmp/adafruit-circuitpython-bno08x-1.1.9.tar.gz` & `tmp/adafruit-circuitpython-bno08x-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bno08x-1.1.9.tar", last modified: Mon Nov 28 18:14:46 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-bno08x-1.2.0.tar", last modified: Thu Apr 20 19:39:42 2023, max compression
```

## Comparing `adafruit-circuitpython-bno08x-1.1.9.tar` & `adafruit-circuitpython-bno08x-1.2.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:46.411184 adafruit-circuitpython-bno08x-1.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:46.403184 adafruit-circuitpython-bno08x-1.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:46.403184 adafruit-circuitpython-bno08x-1.1.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:46.407184 adafruit-circuitpython-bno08x-1.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6140 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:46.407184 adafruit-circuitpython-bno08x-1.1.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2022-11-28 18:14:46.411184 adafruit-circuitpython-bno08x-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2969 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:46.407184 adafruit-circuitpython-bno08x-1.1.9/adafruit_bno08x/
--rw-r--r--   0 runner    (1001) docker     (122)    38547 2022-11-28 18:14:37.000000 adafruit-circuitpython-bno08x-1.1.9/adafruit_bno08x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3701 2022-11-28 18:14:37.000000 adafruit-circuitpython-bno08x-1.1.9/adafruit_bno08x/debug.py
--rw-r--r--   0 runner    (1001) docker     (122)     4236 2022-11-28 18:14:37.000000 adafruit-circuitpython-bno08x-1.1.9/adafruit_bno08x/i2c.py
--rw-r--r--   0 runner    (1001) docker     (122)     5919 2022-11-28 18:14:37.000000 adafruit-circuitpython-bno08x-1.1.9/adafruit_bno08x/spi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5374 2022-11-28 18:14:37.000000 adafruit-circuitpython-bno08x-1.1.9/adafruit_bno08x/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:46.407184 adafruit-circuitpython-bno08x-1.1.9/adafruit_circuitpython_bno08x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2022-11-28 18:14:46.000000 adafruit-circuitpython-bno08x-1.1.9/adafruit_circuitpython_bno08x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1263 2022-11-28 18:14:46.000000 adafruit-circuitpython-bno08x-1.1.9/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:14:46.000000 adafruit-circuitpython-bno08x-1.1.9/adafruit_circuitpython_bno08x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 18:14:46.000000 adafruit-circuitpython-bno08x-1.1.9/adafruit_circuitpython_bno08x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-28 18:14:46.000000 adafruit-circuitpython-bno08x-1.1.9/adafruit_circuitpython_bno08x.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:46.407184 adafruit-circuitpython-bno08x-1.1.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:46.407184 adafruit-circuitpython-bno08x-1.1.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      265 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5553 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:46.411184 adafruit-circuitpython-bno08x-1.1.9/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1878 2022-11-28 18:14:37.000000 adafruit-circuitpython-bno08x-1.1.9/examples/bno08x_calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2022-11-28 18:14:37.000000 adafruit-circuitpython-bno08x-1.1.9/examples/bno08x_find_heading.py
--rw-r--r--   0 runner    (1001) docker     (122)     4327 2022-11-28 18:14:37.000000 adafruit-circuitpython-bno08x-1.1.9/examples/bno08x_more_reports.py
--rw-r--r--   0 runner    (1001) docker     (122)     1270 2022-11-28 18:14:37.000000 adafruit-circuitpython-bno08x-1.1.9/examples/bno08x_quaternion_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     1431 2022-11-28 18:14:37.000000 adafruit-circuitpython-bno08x-1.1.9/examples/bno08x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      962 2022-11-28 18:14:37.000000 adafruit-circuitpython-bno08x-1.1.9/examples/bno08x_simpletest_spi.py
--rw-r--r--   0 runner    (1001) docker     (122)     4835 2022-11-28 18:14:37.000000 adafruit-circuitpython-bno08x-1.1.9/examples/bno08x_simpletest_uart.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2022-11-28 18:14:37.000000 adafruit-circuitpython-bno08x-1.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      158 2022-11-28 18:14:27.000000 adafruit-circuitpython-bno08x-1.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:14:46.411184 adafruit-circuitpython-bno08x-1.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.732784 adafruit-circuitpython-bno08x-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.724784 adafruit-circuitpython-bno08x-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-20 19:39:42.732784 adafruit-circuitpython-bno08x-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/
+-rw-r--r--   0 runner    (1001) docker     (123)    38913 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-20 19:39:42.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-20 19:39:42.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:39:42.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 19:39:42.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 19:39:42.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_find_heading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_more_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_quaternion_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_simpletest_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_simpletest_uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:39:42.732784 adafruit-circuitpython-bno08x-1.2.0/setup.cfg
```

### Comparing `adafruit-circuitpython-bno08x-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bno08x-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/.gitignore` & `adafruit-circuitpython-bno08x-1.2.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-bno08x-1.1.9/.pre-commit-config.yaml` & `adafruit-circuitpython-bno08x-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/.pylintrc` & `adafruit-circuitpython-bno08x-1.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bno08x-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/LICENSE` & `adafruit-circuitpython-bno08x-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bno08x-1.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/LICENSES/MIT.txt` & `adafruit-circuitpython-bno08x-1.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bno08x-1.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/PKG-INFO` & `adafruit-circuitpython-bno08x-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bno08x
-Version: 1.1.9
+Version: 1.2.0
 Summary: Helper library for the Hillcrest Laboratories BNO08x IMUs
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BNO08x
 Keywords: adafruit,blinka,circuitpython,micropython,bno080,IMU,BNO055,SENSOR,FUSION,VR,MOTION,TRACK,BNO085
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bno08x-1.1.9/README.rst` & `adafruit-circuitpython-bno08x-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/adafruit_bno08x/__init__.py` & `adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https:# github.com/adafruit/circuitpython/releases
 
 * `Adafruit's Bus Device library <https:# github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
 """
-__version__ = "1.1.9"
+__version__ = "1.2.0"
 __repo__ = "https:# github.com/adafruit/Adafruit_CircuitPython_BNO08x.git"
 
 from struct import unpack_from, pack_into
 from collections import namedtuple
 import time
 from micropython import const
 
@@ -77,14 +77,17 @@
 BNO_REPORT_GYROSCOPE = const(0x02)
 # Magnetic field calibrated (in µTesla). The fully calibrated magnetic field measurement.
 BNO_REPORT_MAGNETOMETER = const(0x03)
 # Linear acceleration (m/s2). Acceleration of the device with gravity removed
 BNO_REPORT_LINEAR_ACCELERATION = const(0x04)
 # Rotation Vector
 BNO_REPORT_ROTATION_VECTOR = const(0x05)
+# Gravity Vector (m/s2). Vector direction of gravity
+BNO_REPORT_GRAVITY = const(0x06)
+# Game Rotation Vector
 BNO_REPORT_GAME_ROTATION_VECTOR = const(0x08)
 
 BNO_REPORT_GEOMAGNETIC_ROTATION_VECTOR = const(0x09)
 
 BNO_REPORT_STEP_COUNTER = const(0x11)
 
 BNO_REPORT_RAW_ACCELEROMETER = const(0x14)
@@ -135,14 +138,15 @@
 _RAW_REPORTS = {
     BNO_REPORT_RAW_ACCELEROMETER: BNO_REPORT_ACCELEROMETER,
     BNO_REPORT_RAW_GYROSCOPE: BNO_REPORT_GYROSCOPE,
     BNO_REPORT_RAW_MAGNETOMETER: BNO_REPORT_MAGNETOMETER,
 }
 _AVAIL_SENSOR_REPORTS = {
     BNO_REPORT_ACCELEROMETER: (_Q_POINT_8_SCALAR, 3, 10),
+    BNO_REPORT_GRAVITY: (_Q_POINT_8_SCALAR, 3, 10),
     BNO_REPORT_GYROSCOPE: (_Q_POINT_9_SCALAR, 3, 10),
     BNO_REPORT_MAGNETOMETER: (_Q_POINT_4_SCALAR, 3, 10),
     BNO_REPORT_LINEAR_ACCELERATION: (_Q_POINT_8_SCALAR, 3, 10),
     BNO_REPORT_ROTATION_VECTOR: (_Q_POINT_14_SCALAR, 4, 14),
     BNO_REPORT_GEOMAGNETIC_ROTATION_VECTOR: (_Q_POINT_12_SCALAR, 4, 14),
     BNO_REPORT_GAME_ROTATION_VECTOR: (_Q_POINT_14_SCALAR, 4, 12),
     BNO_REPORT_STEP_COUNTER: (1, 1, 12),
@@ -366,23 +370,14 @@
         # add a slice to the list that was passed in
         report_slice = packet.data[next_byte_index : next_byte_index + required_bytes]
 
         report_slices.append([report_slice[0], report_slice])
         next_byte_index = next_byte_index + required_bytes
 
 
-# class Report:
-#     _buffer = bytearray(DATA_BUFFER_SIZE)
-#     _report_obj = Report(_buffer)
-
-#     @classmethod
-#     def get_report(cls)
-#         return cls._report_obj
-
-
 class Packet:
     """A class representing a Hillcrest LaboratorySensor Hub Transport packet"""
 
     def __init__(self, packet_bytes):
         self.header = self.header_from_buffer(packet_bytes)
         data_end_index = self.header.data_length + _BNO_HEADER_LEN
         self.data = packet_bytes[_BNO_HEADER_LEN:data_end_index]
@@ -594,14 +589,24 @@
         self._process_available_packets()
         try:
             return self._readings[BNO_REPORT_ACCELEROMETER]
         except KeyError:
             raise RuntimeError("No accel report found, is it enabled?") from None
 
     @property
+    def gravity(self):
+        """A tuple representing the gravity vector in the X, Y, and Z components
+        axes in meters per second squared"""
+        self._process_available_packets()
+        try:
+            return self._readings[BNO_REPORT_GRAVITY]
+        except KeyError:
+            raise RuntimeError("No gravity report found, is it enabled?") from None
+
+    @property
     def gyro(self):
         """A tuple representing Gyro's rotation measurements on the X, Y, and Z
         axes in radians per second"""
         self._process_available_packets()
         try:
             return self._readings[BNO_REPORT_GYROSCOPE]
         except KeyError:
```

### Comparing `adafruit-circuitpython-bno08x-1.1.9/adafruit_bno08x/debug.py` & `adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/debug.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/adafruit_bno08x/i2c.py` & `adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/i2c.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/adafruit_bno08x/spi.py` & `adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/adafruit_bno08x/uart.py` & `adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/uart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/adafruit_circuitpython_bno08x.egg-info/PKG-INFO` & `adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bno08x
-Version: 1.1.9
+Version: 1.2.0
 Summary: Helper library for the Hillcrest Laboratories BNO08x IMUs
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BNO08x
 Keywords: adafruit,blinka,circuitpython,micropython,bno080,IMU,BNO055,SENSOR,FUSION,VR,MOTION,TRACK,BNO085
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bno08x-1.1.9/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt` & `adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/docs/_static/favicon.ico` & `adafruit-circuitpython-bno08x-1.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/docs/conf.py` & `adafruit-circuitpython-bno08x-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/docs/index.rst` & `adafruit-circuitpython-bno08x-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/examples/bno08x_calibration.py` & `adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_calibration.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/examples/bno08x_find_heading.py` & `adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_find_heading.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 # SPDX-License-Identifier: Unlicense
 
 import time
 from math import atan2, sqrt, pi
 from board import SCL, SDA
 from busio import I2C
 from adafruit_bno08x import (
-    BNO_REPORT_STEP_COUNTER,
     BNO_REPORT_ROTATION_VECTOR,
     BNO_REPORT_GEOMAGNETIC_ROTATION_VECTOR,
 )
 from adafruit_bno08x.i2c import BNO08X_I2C
 
 i2c = I2C(SCL, SDA, frequency=800000)
 bno = BNO08X_I2C(i2c)
-bno.enable_feature(BNO_REPORT_STEP_COUNTER)
 bno.enable_feature(BNO_REPORT_ROTATION_VECTOR)
 bno.enable_feature(BNO_REPORT_GEOMAGNETIC_ROTATION_VECTOR)
 
 # quat_real, quat_i, quat_j, quat_k
 
 
 def find_heading(dqw, dqx, dqy, dqz):
```

### Comparing `adafruit-circuitpython-bno08x-1.1.9/examples/bno08x_more_reports.py` & `adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_more_reports.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/examples/bno08x_quaternion_service.py` & `adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_quaternion_service.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/examples/bno08x_simpletest.py` & `adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/examples/bno08x_simpletest_spi.py` & `adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_simpletest_spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/examples/bno08x_simpletest_uart.py` & `adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_simpletest_uart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.1.9/pyproject.toml` & `adafruit-circuitpython-bno08x-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bno08x"
 description = "Helper library for the Hillcrest Laboratories BNO08x IMUs"
-version = "1.1.9"
+version = "1.2.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BNO08x"}
 keywords = [
     "adafruit",
```

