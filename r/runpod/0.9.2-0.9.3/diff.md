# Comparing `tmp/runpod-0.9.2.tar.gz` & `tmp/runpod-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runpod-0.9.2.tar", last modified: Wed Apr 12 04:23:09 2023, max compression
+gzip compressed data, was "runpod-0.9.3.tar", last modified: Thu Apr 20 18:46:34 2023, max compression
```

## Comparing `runpod-0.9.2.tar` & `runpod-0.9.3.tar`

### file list

```diff
@@ -1,79 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.613602 runpod-0.9.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.589601 runpod-0.9.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-12 04:22:56.000000 runpod-0.9.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.593601 runpod-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-12 04:22:56.000000 runpod-0.9.2/.github/workflows/CD_publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-12 04:22:56.000000 runpod-0.9.2/.github/workflows/CI_codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-12 04:22:56.000000 runpod-0.9.2/.github/workflows/CI_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 04:22:56.000000 runpod-0.9.2/.github/workflows/ci_pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-12 04:22:56.000000 runpod-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-12 04:22:56.000000 runpod-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-12 04:23:09.613602 runpod-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-12 04:22:56.000000 runpod-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.581601 runpod-0.9.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.593601 runpod-0.9.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    28325 2023-04-12 04:22:56.000000 runpod-0.9.2/docs/images/env_var_location.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.593601 runpod-0.9.2/docs/serverless/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.597601 runpod-0.9.2/docs/serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-12 04:22:56.000000 runpod-0.9.2/docs/serverless/utils/rp_cleanup.md
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-12 04:22:56.000000 runpod-0.9.2/docs/serverless/utils/rp_download.md
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-12 04:22:56.000000 runpod-0.9.2/docs/serverless/utils/rp_upload.md
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-12 04:22:56.000000 runpod-0.9.2/docs/serverless/utils/rp_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-12 04:22:56.000000 runpod-0.9.2/docs/serverless/worker.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.597601 runpod-0.9.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-12 04:22:56.000000 runpod-0.9.2/examples/call_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-12 04:22:56.000000 runpod-0.9.2/examples/call_endpoint_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-12 04:22:56.000000 runpod-0.9.2/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-12 04:22:56.000000 runpod-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 04:22:56.000000 runpod-0.9.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.597601 runpod-0.9.2/runpod/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.601601 runpod-0.9.2/runpod/api_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/api_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.601601 runpod-0.9.2/runpod/api_wrapper/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/api_wrapper/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/api_wrapper/queries/cpu_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.601601 runpod-0.9.2/runpod/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.601601 runpod-0.9.2/runpod/endpoint/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/endpoint/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/endpoint/asyncio/asyncio_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/endpoint/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.605601 runpod-0.9.2/runpod/serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.605601 runpod-0.9.2/runpod/serverless/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/rp_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/rp_tips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/worker_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.609602 runpod-0.9.2/runpod/serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/utils/rp_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/utils/rp_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/utils/rp_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/utils/rp_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/work_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.601601 runpod-0.9.2/runpod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-12 04:23:09.000000 runpod-0.9.2/runpod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-12 04:23:09.000000 runpod-0.9.2/runpod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 04:23:09.000000 runpod-0.9.2/runpod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 04:23:09.000000 runpod-0.9.2/runpod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 04:23:09.000000 runpod-0.9.2/runpod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-12 04:23:09.613602 runpod-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-12 04:22:56.000000 runpod-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.609602 runpod-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.609602 runpod-0.9.2/tests/test_endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/test_endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/test_endpoint/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.613602 runpod-0.9.2/tests/test_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/test_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/test_serverless/test_module_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/test_serverless/test_pod_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/test_serverless/test_util_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/test_whatever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/whatever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.162383 runpod-0.9.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.150383 runpod-0.9.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-20 18:46:19.000000 runpod-0.9.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.150383 runpod-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-20 18:46:19.000000 runpod-0.9.3/.github/workflows/CD_publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-20 18:46:19.000000 runpod-0.9.3/.github/workflows/CI_codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-20 18:46:19.000000 runpod-0.9.3/.github/workflows/CI_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-20 18:46:19.000000 runpod-0.9.3/.github/workflows/ci_pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-20 18:46:19.000000 runpod-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-20 18:46:19.000000 runpod-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-20 18:46:34.162383 runpod-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-20 18:46:19.000000 runpod-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.146382 runpod-0.9.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.150383 runpod-0.9.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/api/quries.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.150383 runpod-0.9.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    28325 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/images/env_var_location.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.154383 runpod-0.9.3/docs/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/serverless/local_testing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.154383 runpod-0.9.3/docs/serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/serverless/utils/rp_cleanup.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/serverless/utils/rp_download.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/serverless/utils/rp_upload.md
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/serverless/utils/rp_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/serverless/worker.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.154383 runpod-0.9.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-20 18:46:19.000000 runpod-0.9.3/examples/call_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-20 18:46:19.000000 runpod-0.9.3/examples/call_endpoint_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-20 18:46:19.000000 runpod-0.9.3/examples/graphql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-20 18:46:19.000000 runpod-0.9.3/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-20 18:46:19.000000 runpod-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-20 18:46:19.000000 runpod-0.9.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.154383 runpod-0.9.3/runpod/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.154383 runpod-0.9.3/runpod/api_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/api_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/api_wrapper/ctl_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/api_wrapper/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.154383 runpod-0.9.3/runpod/api_wrapper/mutations/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/api_wrapper/mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/api_wrapper/mutations/pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.158383 runpod-0.9.3/runpod/api_wrapper/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/api_wrapper/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/api_wrapper/queries/gpus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.158383 runpod-0.9.3/runpod/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.158383 runpod-0.9.3/runpod/endpoint/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/endpoint/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/endpoint/asyncio/asyncio_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/endpoint/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.158383 runpod-0.9.3/runpod/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.158383 runpod-0.9.3/runpod/serverless/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/rp_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/rp_tips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/worker_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.158383 runpod-0.9.3/runpod/serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/utils/rp_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/utils/rp_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/utils/rp_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/utils/rp_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/work_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.154383 runpod-0.9.3/runpod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-20 18:46:34.000000 runpod-0.9.3/runpod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-20 18:46:34.000000 runpod-0.9.3/runpod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:46:34.000000 runpod-0.9.3/runpod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-20 18:46:34.000000 runpod-0.9.3/runpod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 18:46:34.000000 runpod-0.9.3/runpod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-20 18:46:34.162383 runpod-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-20 18:46:19.000000 runpod-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.162383 runpod-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.162383 runpod-0.9.3/tests/test_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/test_endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/test_endpoint/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.162383 runpod-0.9.3/tests/test_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/test_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/test_serverless/test_module_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/test_serverless/test_pod_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/test_serverless/test_util_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/test_whatever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/whatever.py
```

### Comparing `runpod-0.9.2/.github/workflows/CD_publish-to-pypi.yml` & `runpod-0.9.3/.github/workflows/CD_publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/.github/workflows/CI_codeql.yml` & `runpod-0.9.3/.github/workflows/CI_codeql.yml`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/.github/workflows/CI_tests.yml` & `runpod-0.9.3/.github/workflows/CI_tests.yml`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/.github/workflows/ci_pylint.yml` & `runpod-0.9.3/.github/workflows/ci_pylint.yml`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/.gitignore` & `runpod-0.9.3/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 env
 .env
 .vscode
+test_wrapper.py
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `runpod-0.9.2/LICENSE` & `runpod-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/PKG-INFO` & `runpod-0.9.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: runpod
-Version: 0.9.2
-Summary: Official Python library for RunPod API & SDK.
-Home-page: https://github.com/runpod/runpod-python
-Author: RunPod
-Author-email: support@runpod.io
-License: MIT
-Project-URL: Bug Tracker, https://github.com/runpod/runpod-python/issues
-Keywords: runpod,ai,gpu,serverless,SDK,API,python,library
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 <div align="center">
 <h1>RunPod | Python Library </h1>
 
 [![CI | Code Quality](https://github.com/runpod/runpod-python/actions/workflows/ci_pylint.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/ci_pylint.yml)
 &nbsp;
 [![CI | Unit Tests](https://github.com/runpod/runpod-python/actions/workflows/CI_tests.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/CI_tests.yml)
 
@@ -36,14 +13,15 @@
 
 - [Table of Contents](#table-of-contents)
 - [Installation](#installation)
 - [SDK - Serverless Worker](#sdk---serverless-worker)
   - [Quick Start](#quick-start)
 - [API Language Library](#api-language-library)
   - [Endpoints](#endpoints)
+  - [GPU Pod Control](#gpu-pod-control)
 - [Directory](#directory)
 - [Community and Contributing](#community-and-contributing)
 
 ## Installation
 
 ```bash
 pip install runpod
@@ -115,14 +93,34 @@
     {"your_model_input_key": "your_model_input_value"}
 )
 
 # Returns the job results if completed within 90 seconds, otherwise, returns the job status.
 print(run_request )
 ```
 
+### GPU Pod Control
+
+```python
+import runpod
+
+runpod.api_key = "your_runpod_api_key_found_under_settings"
+
+# Create a pod
+pod = runpod.create_pod("test", "runpod/stack", "NVIDIA GeForce RTX 3070")
+
+# Stop the pod
+runpod.stop_pod(pod.id)
+
+# Start the pod
+runpod.start_pod(pod.id)
+
+# Terminate the pod
+runpod.terminate_pod(pod.id)
+```
+
 ## Directory
 
 ```BASH
 .
 ├── docs               # Documentation
 ├── runpod             # Package source code
 │   ├── endpoint       # Language library - Endpoints
```

### Comparing `runpod-0.9.2/README.md` & `runpod-0.9.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: runpod
+Version: 0.9.3
+Summary: Official Python library for RunPod API & SDK.
+Home-page: https://github.com/runpod/runpod-python
+Author: RunPod
+Author-email: support@runpod.io
+License: MIT
+Project-URL: Bug Tracker, https://github.com/runpod/runpod-python/issues
+Keywords: runpod,ai,gpu,serverless,SDK,API,python,library
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 <div align="center">
 <h1>RunPod | Python Library </h1>
 
 [![CI | Code Quality](https://github.com/runpod/runpod-python/actions/workflows/ci_pylint.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/ci_pylint.yml)
 &nbsp;
 [![CI | Unit Tests](https://github.com/runpod/runpod-python/actions/workflows/CI_tests.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/CI_tests.yml)
 
@@ -13,14 +36,15 @@
 
 - [Table of Contents](#table-of-contents)
 - [Installation](#installation)
 - [SDK - Serverless Worker](#sdk---serverless-worker)
   - [Quick Start](#quick-start)
 - [API Language Library](#api-language-library)
   - [Endpoints](#endpoints)
+  - [GPU Pod Control](#gpu-pod-control)
 - [Directory](#directory)
 - [Community and Contributing](#community-and-contributing)
 
 ## Installation
 
 ```bash
 pip install runpod
@@ -92,14 +116,34 @@
     {"your_model_input_key": "your_model_input_value"}
 )
 
 # Returns the job results if completed within 90 seconds, otherwise, returns the job status.
 print(run_request )
 ```
 
+### GPU Pod Control
+
+```python
+import runpod
+
+runpod.api_key = "your_runpod_api_key_found_under_settings"
+
+# Create a pod
+pod = runpod.create_pod("test", "runpod/stack", "NVIDIA GeForce RTX 3070")
+
+# Stop the pod
+runpod.stop_pod(pod.id)
+
+# Start the pod
+runpod.start_pod(pod.id)
+
+# Terminate the pod
+runpod.terminate_pod(pod.id)
+```
+
 ## Directory
 
 ```BASH
 .
 ├── docs               # Documentation
 ├── runpod             # Package source code
 │   ├── endpoint       # Language library - Endpoints
```

### Comparing `runpod-0.9.2/docs/images/env_var_location.png` & `runpod-0.9.3/docs/images/env_var_location.png`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/docs/serverless/utils/rp_download.md` & `runpod-0.9.3/docs/serverless/utils/rp_download.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/docs/serverless/utils/rp_upload.md` & `runpod-0.9.3/docs/serverless/utils/rp_upload.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/docs/serverless/utils/rp_validator.md` & `runpod-0.9.3/docs/serverless/utils/rp_validator.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/docs/serverless/worker.md` & `runpod-0.9.3/docs/serverless/worker.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/examples/call_endpoint_asyncio.py` & `runpod-0.9.3/examples/call_endpoint_asyncio.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/infer.py` & `runpod-0.9.3/infer.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/endpoint/asyncio/asyncio_runner.py` & `runpod-0.9.3/runpod/endpoint/asyncio/asyncio_runner.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/endpoint/runner.py` & `runpod-0.9.3/runpod/endpoint/runner.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/serverless/__init__.py` & `runpod-0.9.3/runpod/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/serverless/modules/heartbeat.py` & `runpod-0.9.3/runpod/serverless/modules/heartbeat.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/serverless/modules/job.py` & `runpod-0.9.3/runpod/serverless/modules/job.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/serverless/modules/logging.py` & `runpod-0.9.3/runpod/serverless/modules/logging.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/serverless/modules/retry.py` & `runpod-0.9.3/runpod/serverless/modules/retry.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/serverless/modules/rp_fastapi.py` & `runpod-0.9.3/runpod/serverless/modules/rp_fastapi.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/serverless/modules/rp_tips.py` & `runpod-0.9.3/runpod/serverless/modules/rp_tips.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/serverless/modules/worker_state.py` & `runpod-0.9.3/runpod/serverless/modules/worker_state.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/serverless/utils/rp_cleanup.py` & `runpod-0.9.3/runpod/serverless/utils/rp_cleanup.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/serverless/utils/rp_download.py` & `runpod-0.9.3/runpod/serverless/utils/rp_download.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/serverless/utils/rp_upload.py` & `runpod-0.9.3/runpod/serverless/utils/rp_upload.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/serverless/utils/rp_validator.py` & `runpod-0.9.3/runpod/serverless/utils/rp_validator.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod/serverless/work_loop.py` & `runpod-0.9.3/runpod/serverless/work_loop.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/runpod.egg-info/PKG-INFO` & `runpod-0.9.3/runpod.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runpod
-Version: 0.9.2
+Version: 0.9.3
 Summary: Official Python library for RunPod API & SDK.
 Home-page: https://github.com/runpod/runpod-python
 Author: RunPod
 Author-email: support@runpod.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/runpod/runpod-python/issues
 Keywords: runpod,ai,gpu,serverless,SDK,API,python,library
@@ -36,14 +36,15 @@
 
 - [Table of Contents](#table-of-contents)
 - [Installation](#installation)
 - [SDK - Serverless Worker](#sdk---serverless-worker)
   - [Quick Start](#quick-start)
 - [API Language Library](#api-language-library)
   - [Endpoints](#endpoints)
+  - [GPU Pod Control](#gpu-pod-control)
 - [Directory](#directory)
 - [Community and Contributing](#community-and-contributing)
 
 ## Installation
 
 ```bash
 pip install runpod
@@ -115,14 +116,34 @@
     {"your_model_input_key": "your_model_input_value"}
 )
 
 # Returns the job results if completed within 90 seconds, otherwise, returns the job status.
 print(run_request )
 ```
 
+### GPU Pod Control
+
+```python
+import runpod
+
+runpod.api_key = "your_runpod_api_key_found_under_settings"
+
+# Create a pod
+pod = runpod.create_pod("test", "runpod/stack", "NVIDIA GeForce RTX 3070")
+
+# Stop the pod
+runpod.stop_pod(pod.id)
+
+# Start the pod
+runpod.start_pod(pod.id)
+
+# Terminate the pod
+runpod.terminate_pod(pod.id)
+```
+
 ## Directory
 
 ```BASH
 .
 ├── docs               # Documentation
 ├── runpod             # Package source code
 │   ├── endpoint       # Language library - Endpoints
```

### Comparing `runpod-0.9.2/runpod.egg-info/SOURCES.txt` & `runpod-0.9.3/runpod.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,31 +7,38 @@
 setup.cfg
 setup.py
 .github/dependabot.yml
 .github/workflows/CD_publish-to-pypi.yml
 .github/workflows/CI_codeql.yml
 .github/workflows/CI_tests.yml
 .github/workflows/ci_pylint.yml
+docs/api/quries.md
 docs/images/env_var_location.png
+docs/serverless/local_testing.md
 docs/serverless/worker.md
 docs/serverless/utils/rp_cleanup.md
 docs/serverless/utils/rp_download.md
 docs/serverless/utils/rp_upload.md
 docs/serverless/utils/rp_validator.md
 examples/call_endpoint.py
 examples/call_endpoint_asyncio.py
+examples/graphql_wrapper.py
 runpod/__init__.py
 runpod.egg-info/PKG-INFO
 runpod.egg-info/SOURCES.txt
 runpod.egg-info/dependency_links.txt
 runpod.egg-info/requires.txt
 runpod.egg-info/top_level.txt
 runpod/api_wrapper/__init__.py
+runpod/api_wrapper/ctl_commands.py
+runpod/api_wrapper/graphql.py
+runpod/api_wrapper/mutations/__init__.py
+runpod/api_wrapper/mutations/pods.py
 runpod/api_wrapper/queries/__init__.py
-runpod/api_wrapper/queries/cpu_types.py
+runpod/api_wrapper/queries/gpus.py
 runpod/endpoint/__init__.py
 runpod/endpoint/runner.py
 runpod/endpoint/asyncio/__init__.py
 runpod/endpoint/asyncio/asyncio_runner.py
 runpod/serverless/__init__.py
 runpod/serverless/work_loop.py
 runpod/serverless/modules/__init__.py
```

### Comparing `runpod-0.9.2/setup.cfg` & `runpod-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/tests/test_endpoint/test_runner.py` & `runpod-0.9.3/tests/test_endpoint/test_runner.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/tests/test_serverless/test_module_download.py` & `runpod-0.9.3/tests/test_serverless/test_module_download.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/tests/test_serverless/test_pod_worker.py` & `runpod-0.9.3/tests/test_serverless/test_pod_worker.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/tests/test_serverless/test_util_upload.py` & `runpod-0.9.3/tests/test_serverless/test_util_upload.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/tests/test_whatever.py` & `runpod-0.9.3/tests/test_whatever.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.2/tests/whatever.py` & `runpod-0.9.3/tests/whatever.py`

 * *Files identical despite different names*

