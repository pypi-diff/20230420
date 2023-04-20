# Comparing `tmp/resilient_lib-48.0.4034.tar.gz` & `tmp/resilient_lib-48.1.4243.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_lib-48.0.4034.tar", last modified: Tue Feb 28 15:23:25 2023, max compression
+gzip compressed data, was "resilient_lib-48.1.4243.tar", last modified: Thu Apr 20 19:35:10 2023, max compression
```

## Comparing `resilient_lib-48.0.4034.tar` & `resilient_lib-48.1.4243.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:25.858444 resilient_lib-48.0.4034/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6131 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2023-02-28 15:23:25.858444 resilient_lib-48.0.4034/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1727 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:25.850444 resilient_lib-48.0.4034/resilient_lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)      871 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:25.854444 resilient_lib-48.0.4034/resilient_lib/components/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/components/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1400 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/components/function_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/components/function_result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10468 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/components/html2markdown.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      573 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/components/integration_errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8828 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/components/oauth2_client_credentials_session.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26296 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/components/poller_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19335 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/components/requests_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24255 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/components/resilient_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23208 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/components/templates_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1530 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/components/workflow_status.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:25.854444 resilient_lib-48.0.4034/resilient_lib/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/ui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5694 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/ui/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/ui/conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1717 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/ui/elements.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3855 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/ui/tab.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:25.854444 resilient_lib-48.0.4034/resilient_lib/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      518 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/util/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      410 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/resilient_lib/util/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:25.854444 resilient_lib-48.0.4034/resilient_lib.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2023-02-28 15:23:25.000000 resilient_lib-48.0.4034/resilient_lib.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1628 2023-02-28 15:23:25.000000 resilient_lib-48.0.4034/resilient_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:23:25.000000 resilient_lib-48.0.4034/resilient_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2023-02-28 15:23:25.000000 resilient_lib-48.0.4034/resilient_lib.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      145 2023-02-28 15:23:25.000000 resilient_lib-48.0.4034/resilient_lib.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-02-28 15:23:25.000000 resilient_lib-48.0.4034/resilient_lib.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1356 2023-02-28 15:23:25.858444 resilient_lib-48.0.4034/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:25.858444 resilient_lib-48.0.4034/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:25.858444 resilient_lib-48.0.4034/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      119 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/data/default_template.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/data/override_template.jinja
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:25.858444 resilient_lib-48.0.4034/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/shared_mock_data/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:25.858444 resilient_lib-48.0.4034/tests/shared_mock_data/mock_certs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/shared_mock_data/mock_certs/cert.pem
--rw-rw-r--   0 travis    (2000) travis    (2000)     3247 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/shared_mock_data/mock_certs/key.open.pem
--rw-rw-r--   0 travis    (2000) travis    (2000)      418 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/shared_mock_data/mock_paths.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17000 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/test_function_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11263 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/test_html2markdown.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6802 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/test_oauth2_client_credentials_session.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1193 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/test_payload.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10945 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/test_poller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30802 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/test_requests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10291 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/test_templates.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:25.858444 resilient_lib-48.0.4034/tests/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/ui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5394 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/ui/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      699 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/ui/test_conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2323 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/ui/test_permissions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3634 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tests/ui/test_tab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      933 2023-02-28 15:22:43.000000 resilient_lib-48.0.4034/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6221 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1727 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.635501 resilient_lib-48.1.4243/resilient_lib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      871 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/resilient_lib/components/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1400 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/function_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/function_result.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10468 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/html2markdown.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      573 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/integration_errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8828 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/oauth2_client_credentials_session.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26850 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/poller_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19335 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/requests_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24255 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/resilient_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23208 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/templates_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1530 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/workflow_status.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/resilient_lib/ui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/ui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5694 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/ui/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/ui/conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1717 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/ui/elements.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3855 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/ui/tab.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/resilient_lib/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      518 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/util/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      410 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/util/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.635501 resilient_lib-48.1.4243/resilient_lib.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2023-04-20 19:35:10.000000 resilient_lib-48.1.4243/resilient_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1628 2023-04-20 19:35:10.000000 resilient_lib-48.1.4243/resilient_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:35:10.000000 resilient_lib-48.1.4243/resilient_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       89 2023-04-20 19:35:10.000000 resilient_lib-48.1.4243/resilient_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      145 2023-04-20 19:35:10.000000 resilient_lib-48.1.4243/resilient_lib.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-04-20 19:35:10.000000 resilient_lib-48.1.4243/resilient_lib.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1356 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      119 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/data/default_template.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/data/override_template.jinja
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/shared_mock_data/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/tests/shared_mock_data/mock_certs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/shared_mock_data/mock_certs/cert.pem
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3247 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/shared_mock_data/mock_certs/key.open.pem
+-rw-rw-r--   0 travis    (2000) travis    (2000)      418 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/shared_mock_data/mock_paths.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17000 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_function_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11263 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_html2markdown.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6802 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_oauth2_client_credentials_session.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1193 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_payload.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12012 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_poller.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31154 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_requests.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10291 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_templates.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/tests/ui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/ui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5394 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/ui/test_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      699 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/ui/test_conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2323 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/ui/test_permissions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3634 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/ui/test_tab.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      933 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tox.ini
```

### Comparing `resilient_lib-48.0.4034/CHANGES` & `resilient_lib-48.1.4243/CHANGES`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**2023-04: version 48.1**
+
+* Updated SOAR case default filters for poller helper methods
+
 **2023-02: version 48.0**
 
 * Added support for ``verify`` config in app.config when using
   :class:`resilient_lib.RequestsCommon.execute() <resilient_lib.components.requests_common.RequestsCommon.execute>`.
   ``verify`` now can be set to ``True``, ``False``, or ``<path_to_your_custom_CA_bundle>`` to control the value used
   when verifying SSL certificates. This change is backward compatible with any apps that use ``RequestsCommon.execute()``
   so any apps updated to run on v48.0 will pull in these changes and the ``verify`` configuration will be supported for that app
```

### Comparing `resilient_lib-48.0.4034/PKG-INFO` & `resilient_lib-48.1.4243/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient_lib
-Version: 48.0.4034
+Version: 48.1.4243
 Summary: Python module with library calls which facilitate the development of Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-lib
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_lib-48.0.4034/README.md` & `resilient_lib-48.1.4243/README.md`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/__init__.py` & `resilient_lib-48.1.4243/resilient_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/components/function_metrics.py` & `resilient_lib-48.1.4243/resilient_lib/components/function_metrics.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/components/function_result.py` & `resilient_lib-48.1.4243/resilient_lib/components/function_result.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/components/html2markdown.py` & `resilient_lib-48.1.4243/resilient_lib/components/html2markdown.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/components/integration_errors.py` & `resilient_lib-48.1.4243/resilient_lib/components/integration_errors.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/components/oauth2_client_credentials_session.py` & `resilient_lib-48.1.4243/resilient_lib/components/oauth2_client_credentials_session.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/components/poller_common.py` & `resilient_lib-48.1.4243/resilient_lib/components/poller_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 LOG = logging.getLogger(__name__)
 
 TYPES_URI = "/types"
 INCIDENTS_URI = "/incidents"
 ARTIFACTS_URI = "/artifacts"
 ARTIFACT_FILE_URI = "/".join([ARTIFACTS_URI, "files"])
 
+DEFAULT_CASES_QUERY_FILTER = "return_level=normal"
+
 # P O L L E R   L O G I C
 def poller(named_poller_interval, named_last_poller_time):
     """
     Decorator to wrap a function as the logic for a poller.
 
     **Example:**
 
@@ -154,25 +156,23 @@
                     field_search['method'] = "equals"
                     field_search['value'] = search_value
 
                 query['filters'][0]['conditions'].append(field_search)
 
         return query
 
-    def _query_cases(self, query):
+    def _query_cases(self, query, filters=DEFAULT_CASES_QUERY_FILTER):
         """ run a query to find case(s) which match the query string
-
         Args:
             query [str]: query string to find cases
-
+            filters [str]: Filters for the end of the uri
         Returns:
             query_results [list]: List of query results
         """
-        query_uri = "/".join([INCIDENTS_URI, "query?return_level=normal"])
-
+        query_uri = "/".join([INCIDENTS_URI, "query?{}".format(filters)])
         try:
             return self.rest_client.post(query_uri, query), None
         except SimpleHTTPException as err:
             LOG.error(str(err))
             LOG.error(query)
             return None, str(err)
 
@@ -259,24 +259,25 @@
                                        This will be a mix of comments sync'd from SOAR and new comments]
             filter_soar_header ([str]): [title added to SOAR comments to be filtered]
         Returns:
             new_comments ([list])
         """
 
         if filter_soar_header:
-            # filter entity comments with our SOAR header
+            # Filter entity comments with our SOAR header
             staged_entity_comments = [comment for comment in entity_comments \
                                         if clean_html(filter_soar_header) not in clean_html(comment)]
         else:
             staged_entity_comments = entity_comments.copy()
 
         # filter out the comments already sync'd to SOAR
         if soar_comment_list:
-            new_entity_comments = [comment for comment in staged_entity_comments \
-                if not any([clean_html(comment) in clean_html(already_synced) for already_synced in soar_comment_list])]
+            already_synced = [clean_html(soar_comment) for soar_comment in soar_comment_list]
+            new_entity_comments = [comment for comment in staged_entity_comments\
+                if clean_html(comment) not in already_synced]
         else:
             new_entity_comments = staged_entity_comments
 
         return new_entity_comments
 
     def _chk_status(self, resp, rc=200):
         """
@@ -296,75 +297,75 @@
             elif resp.status_code != rc:
                 raise IntegrationError("status code failure: {0}".format(resp.status_code))
 
             return resp.json()
 
         return {}
 
-    def get_soar_case(self, search_fields, open_cases=True):
-        """Find a SOAR case which contains custom field(s) associated with the associated endpoint.
+    def get_soar_case(self, search_fields, open_cases=True, uri_filters=DEFAULT_CASES_QUERY_FILTER):
+        """
+        Find a SOAR case which contains custom field(s) associated with the associated endpoint.
         Returns only one case. See :class:`SOARCommon.get_soar_cases()` for examples.
 
         .. note::
 
             ``search_fields`` only supports custom fields.
 
         :param search_fields: Dictionary containing key/value pairs to search for a case match.
             Field values can be True/False for ``has_a_value`` or ``does_not_have_a_value``,
             otherwise a field will use ``equals`` for the value.
         :type search_fields: dict
+        :param uri_filters: Filters for the end of the uri. Default is "return_level=normal"
+        :type uri_filters: str
         :param open_cases: True if only querying open cases.
         :type open_cases: bool
-
         :return: A tuple with the matching case, if any, and any associated error message if something went wrong.
             Returns ``None`` if no associated case was found.
         :rtype: tuple(dict, str)
         """
-        r_cases, error_msg = self.get_soar_cases(search_fields, open_cases=open_cases)
+        r_cases, error_msg = self.get_soar_cases(search_fields, open_cases=open_cases, uri_filters=uri_filters)
         if error_msg:
             return None, error_msg
-
         # return first case
         return (r_cases[0] if r_cases else None, None)
 
-    def get_soar_cases(self, search_fields, open_cases=True):
+    def get_soar_cases(self, search_fields, open_cases=True, uri_filters=DEFAULT_CASES_QUERY_FILTER):
         """
         Get all IBM SOAR cases that match the given search fields.
         To find all cases that are synced from the endpoint platform,
         provide the unique search field that matches the unique id of your
         endpoint solution.
 
         **Example:**
 
         .. code-block:: python
 
             from resilient_lib import SOARCommon
 
             soar_common = SOARCommon(res_client)
-
             found_id = get_id_from_endpoint_query_result()
             cases = soar_common.get_soar_cases({ "endpoint_id": found_id }, open_cases=False)
 
         .. note::
 
             ``search_fields`` only supports custom fields.
-
         :param search_fields: Dictionary containing key/value pairs to search for a case match.
             Field values can be True/False for ``has_a_value`` or ``does_not_have_a_value``,
             otherwise a field will use ``equals`` for the value.
         :type search_fields: dict
+        :param uri_filters: Filters for the end of the uri. Default is "return_level=normal"
+        :type uri_filters: str
         :param open_cases: True if only querying open cases.
         :type open_cases: bool
 
         :return: A tuple with a list of cases whose values match the ``search_fields`` and any associated error message.
         :rtype: tuple(dict, str)
         """
         query = self._build_search_query(search_fields, open_cases=open_cases)
-
-        return self._query_cases(query)
+        return self._query_cases(query, filters=uri_filters)
 
     def create_soar_case(self, case_payload):
         """
         Create a new IBM SOAR case based on a payload formatted for the API call.
 
         :param case_payload: Fields to use for creating a SOAR case
         :type case_payload: dict
```

### Comparing `resilient_lib-48.0.4034/resilient_lib/components/requests_common.py` & `resilient_lib-48.1.4243/resilient_lib/components/requests_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/components/resilient_common.py` & `resilient_lib-48.1.4243/resilient_lib/components/resilient_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/components/templates_common.py` & `resilient_lib-48.1.4243/resilient_lib/components/templates_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/components/workflow_status.py` & `resilient_lib-48.1.4243/resilient_lib/components/workflow_status.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/ui/common.py` & `resilient_lib-48.1.4243/resilient_lib/ui/common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/ui/conditions.py` & `resilient_lib-48.1.4243/resilient_lib/ui/conditions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/ui/elements.py` & `resilient_lib-48.1.4243/resilient_lib/ui/elements.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/ui/tab.py` & `resilient_lib-48.1.4243/resilient_lib/ui/tab.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib/util/config.py` & `resilient_lib-48.1.4243/resilient_lib/util/config.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/resilient_lib.egg-info/PKG-INFO` & `resilient_lib-48.1.4243/resilient_lib.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient-lib
-Version: 48.0.4034
+Version: 48.1.4243
 Summary: Python module with library calls which facilitate the development of Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-lib
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_lib-48.0.4034/resilient_lib.egg-info/SOURCES.txt` & `resilient_lib-48.1.4243/resilient_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/setup.cfg` & `resilient_lib-48.1.4243/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient      >= 48.0
+	resilient      >= 48.1
 	
 	pytz           ~= 2022.1
 	deprecated     ~= 1.2
 	beautifulsoup4 ~= 4.9
 	
 	jinja2         ~= 3.0; python_version >= "3.6"
```

### Comparing `resilient_lib-48.0.4034/tests/shared_mock_data/mock_certs/cert.pem` & `resilient_lib-48.1.4243/tests/shared_mock_data/mock_certs/cert.pem`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/tests/shared_mock_data/mock_certs/key.open.pem` & `resilient_lib-48.1.4243/tests/shared_mock_data/mock_certs/key.open.pem`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/tests/test_common.py` & `resilient_lib-48.1.4243/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/tests/test_function_metrics.py` & `resilient_lib-48.1.4243/tests/test_function_metrics.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/tests/test_html2markdown.py` & `resilient_lib-48.1.4243/tests/test_html2markdown.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/tests/test_oauth2_client_credentials_session.py` & `resilient_lib-48.1.4243/tests/test_oauth2_client_credentials_session.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/tests/test_payload.py` & `resilient_lib-48.1.4243/tests/test_payload.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/tests/test_poller.py` & `resilient_lib-48.1.4243/tests/test_poller.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,24 @@
 import sys
 import time
 from collections import namedtuple
 from threading import Thread
 
 import mock
 import pytest
-from resilient import SimpleHTTPException
-from resilient_lib.components.poller_common import (IntegrationError, SOARCommon, b_to_s, eval_mapping,
-                           get_last_poller_date, poller, s_to_b)
+from resilient_lib.components.poller_common import (DEFAULT_CASES_QUERY_FILTER,
+                                                    IntegrationError,
+                                                    SOARCommon, b_to_s,
+                                                    eval_mapping,
+                                                    get_last_poller_date,
+                                                    poller, s_to_b)
 from resilient_lib.util import constants
 
+from resilient import SimpleHTTPException
+
 NEW_CASE_PAYLOAD = {
   "name": "test case",
   "description": u"a short description  ฑ ฒ ณ ด ต ถ ท ธ น ",
   "discovered_date": str(datetime.datetime.now()),
   "start_date": str(datetime.datetime.now()),
   "plan_status": "A"
 }
@@ -119,28 +124,31 @@
 def test_get_soar_case(fx_mock_resilient_client):
     soar_common = SOARCommon(fx_mock_resilient_client)
 
     case, _err_msg = soar_common.get_soar_case({ "id": 2314 }, open_cases=False)
 
     assert case["plan_status"] == "A"
     assert case["id"] == 2314
+    assert fx_mock_resilient_client.session.adapters.get("https://").last_request.query == DEFAULT_CASES_QUERY_FILTER
 
 
 
 
 @pytest.mark.livetest
 @pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY_VERSION, reason="poller common requires python3.6 or higher")
-def test_get_soar_cases_success(fx_mock_resilient_client):
+def test_get_soar_cases_success(fx_mock_resilient_client, caplog):
     soar_common = SOARCommon(fx_mock_resilient_client)
 
-    cases, _err_msg = soar_common.get_soar_cases({ "id": 2314, "bad_field": True }, open_cases=True)
+    mock_query = "return_level=notnormal"
+    cases, _err_msg = soar_common.get_soar_cases({ "id": 2314, "bad_field": True }, open_cases=True, uri_filters=mock_query)
 
     assert cases
     assert len(cases) == 1
     assert cases[0]["id"] == 2314
+    assert fx_mock_resilient_client.session.adapters.get("https://").last_request.query == mock_query
 
 @pytest.mark.livetest
 @pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY_VERSION, reason="poller common requires python3.6 or higher")
 def test_get_soar_cases_failure(fx_mock_resilient_client):
     old_post = fx_mock_resilient_client.post
     fx_mock_resilient_client.post = _raise_http_exception
     soar_common = SOARCommon(fx_mock_resilient_client)
@@ -272,14 +280,25 @@
     soar_common = SOARCommon(fx_mock_resilient_client)
 
     resp = soar_common.lookup_artifact_type("artifact")
 
     assert resp == "my artifact"
 
 
+@pytest.mark.livetest
+@pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY_VERSION, reason="poller common requires python3.6 or higher")
+def test_filter_soar_comments(fx_mock_resilient_client):
+    soar_common = SOARCommon(fx_mock_resilient_client)
+
+    mock_entity_comments = ["new comment to add here", "comment to add"]
+    mock_soar_comments = ["new comment to add here"]
+    resp = soar_common._filter_comments(mock_soar_comments, mock_entity_comments)
+
+    assert resp == ["comment to add"]
+
 
 
 def test_eval_mapping(caplog):
     # test convert str to dict
     mock_config = '"source":"A","tags":["tagA"],"priorities":[40,50]'
     parsed_config = eval_mapping(mock_config, "{{ {} }}")
     assert parsed_config == { "source": "A", "tags": ["tagA"], "priorities": [40, 50] }
```

### Comparing `resilient_lib-48.0.4034/tests/test_requests.py` & `resilient_lib-48.1.4243/tests/test_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import logging
 import os
 import time
 import unittest
 
+import pytest
 import requests
 import requests_mock
 from parameterized import parameterized
 from resilient_lib import (IntegrationError, RequestsCommon,
                            RequestsCommonWithoutSession)
 from resilient_lib.components.requests_common import (
     get_case_insensitive_key_value, is_payload_in_json)
@@ -133,14 +134,15 @@
 
         # R E S P O N S E  Object
         response = rc.execute_call_v2("get", "{}?format=json".format(IPIFY))
 
         self.assertTrue(isinstance(response, requests.models.Response))
 
     @parameterized.expand(REQUESTS_COMMON_CLASSES)
+    @pytest.mark.livetest
     def test_verbs(self, RCObjectType):
         URL = TestFunctionRequests.URL_TEST_HTTP_VERBS
 
         headers = {
             "Content-type": "application/json; charset=UTF-8"
         }
 
@@ -202,14 +204,15 @@
         self.assertEqual(resp.get("url"), DEL_URL)
 
         # bad verb
         with self.assertRaises(IntegrationError):
             resp = rc.execute_call("bad", URL, None, log=TestFunctionRequests.LOG)
 
     @parameterized.expand(REQUESTS_COMMON_CLASSES)
+    @pytest.mark.livetest
     def test_verbs_v2(self, RCObjectType):
         URL = TestFunctionRequests.URL_TEST_HTTP_VERBS
 
         headers = {
             "Content-type": "application/json; charset=UTF-8"
         }
 
@@ -280,98 +283,107 @@
         self.assertEqual(resp.json().get("url"), DEL_URL)
 
         # bad verb
         with self.assertRaises(IntegrationError):
             resp = rc.execute_call_v2("bad", URL)
 
     @parameterized.expand(REQUESTS_COMMON_CLASSES)
+    @pytest.mark.livetest
     def test_statuscode(self, RCObjectType):
         URL = TestFunctionRequests.URL_TEST_HTTP_STATUS_CODES
 
         rc = RCObjectType(None, None)
 
         resp = rc.execute_call("get", "/".join((URL, "200")), None, resp_type='text')
 
         with self.assertRaises(IntegrationError):
             resp = rc.execute_call("get", "/".join((URL, "300")), None, resp_type='text')
 
     @parameterized.expand(REQUESTS_COMMON_CLASSES)
+    @pytest.mark.livetest
     def test_statuscode_v2(self, RCObjectType):
         URL = TestFunctionRequests.URL_TEST_HTTP_STATUS_CODES
 
         rc = RCObjectType(None, None)
 
         resp = rc.execute_call_v2("get", "/".join((URL, "200")))
 
         with self.assertRaises(IntegrationError):
             resp = rc.execute_call_v2("get", "/".join((URL, "400")))
 
     @parameterized.expand(REQUESTS_COMMON_CLASSES)
+    @pytest.mark.livetest
     def test_statuscode_callback(self, RCObjectType):
         URL = "/".join((TestFunctionRequests.URL_TEST_HTTP_STATUS_CODES, "300"))
 
         def callback(resp):
             if resp.status_code != 300:
                 raise ValueError(resp.status_code)
 
         rc = RCObjectType(None, None)
 
         resp = rc.execute_call("get", URL, None, resp_type='text', callback=callback)
 
     @parameterized.expand(REQUESTS_COMMON_CLASSES)
+    @pytest.mark.livetest
     def test_statuscode_callback_v2(self, RCObjectType):
         URL = "/".join((TestFunctionRequests.URL_TEST_HTTP_STATUS_CODES, "300"))
 
         def callback(resp):
             if resp.status_code != 300:
                 raise ValueError(resp.status_code)
 
         rc = RCObjectType(None, None)
 
         resp = rc.execute_call_v2("get", URL, callback=callback)
 
     @parameterized.expand(REQUESTS_COMMON_CLASSES)
+    @pytest.mark.livetest
     def test_timeout(self, RCObjectType):
         URL = "/".join((TestFunctionRequests.URL_TEST_HTTP_STATUS_CODES, "200?sleep=30000"))
 
         rc = RCObjectType(None, None)
 
         with self.assertRaises(IntegrationError):
             resp = rc.execute_call("get", URL, None, resp_type='text', timeout=2)
 
     @parameterized.expand(REQUESTS_COMMON_CLASSES)
+    @pytest.mark.livetest
     def test_timeout_v2(self, RCObjectType):
         URL = "/".join((TestFunctionRequests.URL_TEST_HTTP_STATUS_CODES, "200?sleep=30000"))
 
         rc = RCObjectType(None, None)
 
         with self.assertRaises(IntegrationError):
             resp = rc.execute_call_v2("get", URL, timeout=2)
 
     @parameterized.expand(REQUESTS_COMMON_CLASSES)
+    @pytest.mark.livetest
     def test_basicauth(self, RCObjectType):
         URL = "/".join((TestFunctionRequests.URL_TEST_HTTP_VERBS, "basic-auth"))
         basicauth = ("postman", "password")
 
         rc = RCObjectType(None, None)
 
         resp = rc.execute_call("get", URL, None, basicauth=basicauth)
         self.assertTrue(resp.get("authenticated"))
 
     @parameterized.expand(REQUESTS_COMMON_CLASSES)
+    @pytest.mark.livetest
     def test_basicauth_v2(self, RCObjectType):
         URL = "/".join((TestFunctionRequests.URL_TEST_HTTP_VERBS, "basic-auth"))
         basicauth = ("postman", "password")
 
         rc = RCObjectType(None, None)
 
         resp = rc.execute_call_v2("get", URL, auth=basicauth)
         self.assertTrue(resp.json().get("authenticated"))
 
     @parameterized.expand(REQUESTS_COMMON_CLASSES)
+    @pytest.mark.livetest
     def test_proxy_override(self, RCObjectType):
         rc = RCObjectType(None, None)
         proxies = rc.get_proxies()
         self.assertIsNone(proxies)
 
         # test only integration proxies
         integrations_xyz =  {
@@ -484,28 +496,30 @@
 
         rc = RequestsCommon(opts=integrations)
         response = rc.execute_call_v2("get", URL)
         json_result = response.json()
         self.assertTrue(json_result.get("ip"))
 
     @parameterized.expand(REQUESTS_COMMON_CLASSES)
+    @pytest.mark.livetest
     def test_headers(self, RCObjectType):
         # G E T with headers
         headers = {
             "Content-type": "application/json; charset=UTF-8",
             "my-sample-header": "my header"
         }
         URL = "/".join((TestFunctionRequests.URL_TEST_HTTP_VERBS, "headers"))
 
         rc = RCObjectType()
 
         json_result = rc.execute_call("get", URL, None, headers=headers)
         self.assertEqual(json_result['headers'].get("my-sample-header"), "my header")
 
     @parameterized.expand(REQUESTS_COMMON_CLASSES)
+    @pytest.mark.livetest
     def test_headers_v2(self, RCObjectType):
         # G E T with headers
         headers = {
             "Content-type": "application/json; charset=UTF-8",
             "my-sample-header": "my header"
         }
         URL = "/".join((TestFunctionRequests.URL_TEST_HTTP_VERBS, "headers"))
```

### Comparing `resilient_lib-48.0.4034/tests/test_templates.py` & `resilient_lib-48.1.4243/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/tests/ui/test_common.py` & `resilient_lib-48.1.4243/tests/ui/test_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/tests/ui/test_conditions.py` & `resilient_lib-48.1.4243/tests/ui/test_conditions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/tests/ui/test_permissions.py` & `resilient_lib-48.1.4243/tests/ui/test_permissions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/tests/ui/test_tab.py` & `resilient_lib-48.1.4243/tests/ui/test_tab.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.0.4034/tox.ini` & `resilient_lib-48.1.4243/tox.ini`

 * *Files identical despite different names*

