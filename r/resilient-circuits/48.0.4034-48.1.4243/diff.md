# Comparing `tmp/resilient_circuits-48.0.4034.tar.gz` & `tmp/resilient_circuits-48.1.4243.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_circuits-48.0.4034.tar", last modified: Tue Feb 28 15:23:45 2023, max compression
+gzip compressed data, was "resilient_circuits-48.1.4243.tar", last modified: Thu Apr 20 19:35:25 2023, max compression
```

## Comparing `resilient_circuits-48.0.4034.tar` & `resilient_circuits-48.1.4243.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:45.602444 resilient_circuits-48.0.4034/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12006 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2023-02-28 15:23:45.602444 resilient_circuits-48.0.4034/PKG-INFO
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2095 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:45.598444 resilient_circuits-48.0.4034/resilient_circuits/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1057 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/LICENSE
--rwxrwxr-x   0 travis    (2000) travis    (2000)      129 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/README
--rwxrwxr-x   0 travis    (2000) travis    (2000)      742 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    15525 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/action_message.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    59349 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/actions_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    11127 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/actions_test_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    10195 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/app.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11010 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/app_argument_parser.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6029 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/app_function_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6381 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/app_restartable.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:45.598444 resilient_circuits-48.0.4034/resilient_circuits/bin/
--rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/bin/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     9741 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/bin/res_action_test.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    17085 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/bin/resilient_circuits_cmd.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2996 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/bin/service_wrapper.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:45.598444 resilient_circuits-48.0.4034/resilient_circuits/cmds/
--rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13670 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/cmds/selftest.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6750 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/component_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2610 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:45.598444 resilient_circuits-48.0.4034/resilient_circuits/data/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2641 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/data/app.config.base
--rwxrwxr-x   0 travis    (2000) travis    (2000)    20046 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11921 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/helpers.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      313 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/keyring_arguments.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3395 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/rest_helper.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    14446 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/stomp_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3606 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/stomp_events.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3991 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/stomp_transport.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      760 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/template_functions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:45.598444 resilient_circuits-48.0.4034/resilient_circuits/util/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      559 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/util/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      725 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/util/resilient_config.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    16321 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/util/resilient_customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      498 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/resilient_circuits/validate_configs.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:45.598444 resilient_circuits-48.0.4034/resilient_circuits.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2023-02-28 15:23:45.000000 resilient_circuits-48.0.4034/resilient_circuits.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2581 2023-02-28 15:23:45.000000 resilient_circuits-48.0.4034/resilient_circuits.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:23:45.000000 resilient_circuits-48.0.4034/resilient_circuits.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-02-28 15:23:45.000000 resilient_circuits-48.0.4034/resilient_circuits.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      176 2023-02-28 15:23:45.000000 resilient_circuits-48.0.4034/resilient_circuits.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-02-28 15:23:45.000000 resilient_circuits-48.0.4034/resilient_circuits.egg-info/top_level.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1511 2023-02-28 15:23:45.606444 resilient_circuits-48.0.4034/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)      199 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:45.602444 resilient_circuits-48.0.4034/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      287 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:45.602444 resilient_circuits-48.0.4034/tests/cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3691 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/cmds/test_selftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3803 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2045 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:45.602444 resilient_circuits-48.0.4034/tests/selftest_tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/selftest_tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/selftest_tests/mocked_fail_script.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      276 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/selftest_tests/mocked_success_script.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      282 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/selftest_tests/mocked_unimplemented_script.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:45.602444 resilient_circuits-48.0.4034/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2050 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/shared_mock_data/mock_app_config
--rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/shared_mock_data/mock_app_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2094 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/shared_mock_data/mock_commented_app_config
--rw-rw-r--   0 travis    (2000) travis    (2000)     2246 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/shared_mock_data/mock_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1710 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/shared_mock_data/mock_constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/shared_mock_data/mock_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    55022 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/shared_mock_data/mock_import_definition.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      545 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/shared_mock_data/mock_paths.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1787 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/test_action_message.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3049 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/test_actions_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/test_app_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1663 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/test_app_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1488 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/test_app_restartable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2311 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/test_component_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7756 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/test_decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3486 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/test_errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7974 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/test_resilient_circuits_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/test_rest_helper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3484 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/test_stomp_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/test_templates.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:45.602444 resilient_circuits-48.0.4034/tests/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1744 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tests/util/test_resilient_customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2023-02-28 15:22:43.000000 resilient_circuits-48.0.4034/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.019501 resilient_circuits-48.1.4243/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12364 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2023-04-20 19:35:25.019501 resilient_circuits-48.1.4243/PKG-INFO
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2095 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.011501 resilient_circuits-48.1.4243/resilient_circuits/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1057 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/LICENSE
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      129 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/README
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      742 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    15525 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/action_message.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    59349 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/actions_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    11127 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/actions_test_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    10353 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/app.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11847 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/app_argument_parser.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6029 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/app_function_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7793 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/app_restartable.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.015501 resilient_circuits-48.1.4243/resilient_circuits/bin/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/bin/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     9741 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/bin/res_action_test.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    17085 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/bin/resilient_circuits_cmd.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2996 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/bin/service_wrapper.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.015501 resilient_circuits-48.1.4243/resilient_circuits/cmds/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13670 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/cmds/selftest.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6750 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/component_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2755 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.015501 resilient_circuits-48.1.4243/resilient_circuits/data/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3063 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/data/app.config.base
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    20046 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11921 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/helpers.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      313 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/keyring_arguments.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3395 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/rest_helper.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    14446 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/stomp_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3606 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/stomp_events.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3991 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/stomp_transport.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      760 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/template_functions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.015501 resilient_circuits-48.1.4243/resilient_circuits/util/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      559 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/util/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      725 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/util/resilient_config.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    16321 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/util/resilient_customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1128 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/validate_configs.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.015501 resilient_circuits-48.1.4243/resilient_circuits.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2023-04-20 19:35:24.000000 resilient_circuits-48.1.4243/resilient_circuits.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2581 2023-04-20 19:35:25.000000 resilient_circuits-48.1.4243/resilient_circuits.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:35:24.000000 resilient_circuits-48.1.4243/resilient_circuits.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-04-20 19:35:24.000000 resilient_circuits-48.1.4243/resilient_circuits.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      176 2023-04-20 19:35:24.000000 resilient_circuits-48.1.4243/resilient_circuits.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-04-20 19:35:24.000000 resilient_circuits-48.1.4243/resilient_circuits.egg-info/top_level.txt
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1511 2023-04-20 19:35:25.019501 resilient_circuits-48.1.4243/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      199 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.015501 resilient_circuits-48.1.4243/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      287 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.015501 resilient_circuits-48.1.4243/tests/cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3691 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/cmds/test_selftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3803 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2045 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.019501 resilient_circuits-48.1.4243/tests/selftest_tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/selftest_tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       43 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/selftest_tests/mocked_fail_script.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      276 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/selftest_tests/mocked_success_script.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      282 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/selftest_tests/mocked_unimplemented_script.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.019501 resilient_circuits-48.1.4243/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2093 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_app_config
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_app_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2141 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_commented_app_config
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2246 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1710 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    55022 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_import_definition.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      545 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_paths.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1787 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_action_message.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3049 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_actions_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4280 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_app_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1663 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_app_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_app_restartable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2311 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_component_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7756 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3486 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7974 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_resilient_circuits_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_rest_helper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3207 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_stomp_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_templates.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.019501 resilient_circuits-48.1.4243/tests/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1744 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/util/test_resilient_customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tox.ini
```

### Comparing `resilient_circuits-48.0.4034/CHANGES` & `resilient_circuits-48.1.4243/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+**2023-04: version 48.1**
+
+* Better log handling for errors upon restart
+* Added new configs for log rotation. ``log_max_bytes`` sets the maximum bytes per log file; defaults to ``10000000``. 
+  ``log_backup_count`` sets the maximum number of log files to keep as backups while files rotate; defaults to ``10``
+* Improved log filtering for sensitive values
+
 **2023-02: version 48.0**
 
 * Include ``threadName`` in the app logs
 * Display SOAR server version in startup logs. Note: for CP4S this displays the underlying SOAR version, not the platform version
 * Updated project to use ``pyproject.toml`` and ``setup.cfg`` metadata files. Build backend continues to use ``setuptools``.
   Instead of directly invoking setup.py to get a sdist or wheel, use ``build`` as a build frontend:
```

### Comparing `resilient_circuits-48.0.4034/PKG-INFO` & `resilient_circuits-48.1.4243/resilient_circuits.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: resilient_circuits
-Version: 48.0.4034
+Name: resilient-circuits
+Version: 48.1.4243
 Summary: Framework used to run IBM SOAR Apps and Integrations
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_circuits-48.0.4034/README.md` & `resilient_circuits-48.1.4243/README.md`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/LICENSE` & `resilient_circuits-48.1.4243/resilient_circuits/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/__init__.py` & `resilient_circuits-48.1.4243/resilient_circuits/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/action_message.py` & `resilient_circuits-48.1.4243/resilient_circuits/action_message.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/actions_component.py` & `resilient_circuits-48.1.4243/resilient_circuits/actions_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/actions_test_component.py` & `resilient_circuits-48.1.4243/resilient_circuits/actions_test_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/app.py` & `resilient_circuits-48.1.4243/resilient_circuits/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         super(RedactingFilter, self).__init__()
 
     def filter(self, record):
         # Best effort regex filter pattern to redact password logging.
         if isinstance(record.msg, string_types):
             for p in constants.PASSWD_PATTERNS:
                 if p in record.msg.lower():
-                    regex = r"{0}(?=.*?':\s)(None,|.+?,|.+?'}})".format(p)
+                    regex = r"{0}(?=.*?'|\":\s)(None,|.+?,|.+?'|.+\"|}})".format(p)
                     record.msg = re.sub(regex, r"***", record.msg)
 
         return True
 
 
 # Main component for our application
 class App(Component):
@@ -68,15 +68,15 @@
         self.auto_load_components = auto_load_components
         self.config_file = config_file or get_config_file()
         self.do_initialization()
 
     def do_initialization(self):
         self.opts = helpers.get_configs(path_config_file=self.config_file, ALLOW_UNRECOGNIZED=self.ALLOW_UNRECOGNIZED)
 
-        self.config_logging(self.opts["logdir"], self.opts["loglevel"], self.opts['logfile'])
+        self.config_logging(self.opts["logdir"], self.opts["loglevel"], self.opts["logfile"], self.opts[constants.APP_CONFIG_LOG_MAX_BYTES], self.opts[constants.APP_CONFIG_LOG_BACKUP_COUNT])
         LOG.info("Configuration file: %s", self.config_file)
         LOG.info("Resilient server: %s", self.opts.get("host"))
         if self.opts.get("email", None):
             LOG.info("Resilient user: %s", self.opts.get("email"))
         if self.opts.get("api_key_id", None):
             LOG.info("Resilient api key id: %s", self.opts.get("api_key_id"))
         if self.opts.get("api_key_id", None) and self.opts.get("email", None):
@@ -113,15 +113,15 @@
             if not self.component_loader:
                 self.component_loader = ComponentLoader(self.opts)
             else:
                 LOG.info("Updating and re-registering ComponentLoader")
                 self.component_loader.opts = self.opts
             self.component_loader.register(self)
 
-    def config_logging(self, logdir, loglevel, logfile):
+    def config_logging(self, logdir, loglevel, logfile, log_max_bytes, log_backup_count):
         """ set up some logging """
         global LOG_PATH, LOG, logging_initialized
 
         LOG_PATH = os.path.join(logdir, logfile)
         LOG_PATH = os.path.expanduser(LOG_PATH)
         LOG = logging.getLogger(__name__)
 
@@ -139,16 +139,16 @@
             logging.getLogger().setLevel(numeric_level)
         except AttributeError as e:
             logging.getLogger().setLevel(logging.INFO)
             LOG.warning("Invalid logging level specified. Using INFO level")
 
         LOG.addFilter(RedactingFilter())
 
-        file_handler = RotatingFileHandler(LOG_PATH, maxBytes=10000000,
-                                           backupCount=10)
+        file_handler = RotatingFileHandler(LOG_PATH, maxBytes=log_max_bytes,
+                                           backupCount=log_backup_count)
         file_handler.setFormatter(logging.Formatter(self.FILE_LOG_FORMAT))
         file_handler.addFilter(RedactingFilter())
         logging.getLogger().addHandler(file_handler)
 
         syslog = logging.handlers.SysLogHandler()
         syslog.setFormatter(logging.Formatter(self.SYSLOG_LOG_FORMAT))
         syslog.addFilter(RedactingFilter())
```

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/app_argument_parser.py` & `resilient_circuits-48.1.4243/resilient_circuits/app_argument_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 class AppArgumentParser(keyring_arguments.ArgumentParser):
     """Helper to parse command line arguments."""
     DEFAULT_APP_SECTION = "resilient"
     DEFAULT_STOMP_PORT = 65001
     DEFAULT_COMPONENTS_DIR = ''
     DEFAULT_LOG_LEVEL = 'INFO'
     DEFAULT_LOG_FILE = 'app.log'
+    DEFAULT_LOG_MAX_BYTES = 10000000
+    DEFAULT_LOG_BACKUP_COUNT = 10
     DEFAULT_NO_PROMPT_PASS = "False"
     DEFAULT_STOMP_TIMEOUT = 60
     DEFAULT_STOMP_MAX_RETRIES = 3
     DEFAULT_MAX_CONNECTION_RETRIES = res_constants.APP_CONFIG_MAX_CONNECTION_RETRIES_DEFAULT
     DEFAULT_NUM_WORKERS = 25
     DEFAULT_APP_EXCEPTION = False
     DEFAULT_HEARTBEAT_TIMEOUT_THRESHOLD = None
@@ -38,14 +40,16 @@
         super(AppArgumentParser, self).__init__(config_file=config_file)
 
         default_components_dir = self.getopt(self.DEFAULT_APP_SECTION, "componentsdir") or self.DEFAULT_COMPONENTS_DIR
         default_noload = self.getopt(self.DEFAULT_APP_SECTION, "noload") or ""
         default_log_dir = self.getopt(self.DEFAULT_APP_SECTION, "logdir") or constants.APP_LOG_DIR
         default_log_level = self.getopt(self.DEFAULT_APP_SECTION, "loglevel") or self.DEFAULT_LOG_LEVEL
         default_log_file = self.getopt(self.DEFAULT_APP_SECTION, "logfile") or self.DEFAULT_LOG_FILE
+        default_log_max_bytes = self.getopt(self.DEFAULT_APP_SECTION, constants.APP_CONFIG_LOG_MAX_BYTES) or self.DEFAULT_LOG_MAX_BYTES
+        default_log_backup_count = self.getopt(self.DEFAULT_APP_SECTION, constants.APP_CONFIG_LOG_BACKUP_COUNT) or self.DEFAULT_LOG_BACKUP_COUNT
 
         # STOMP port is usually 65001
         default_stomp_port = self.getopt(self.DEFAULT_APP_SECTION, "stomp_port") or self.DEFAULT_STOMP_PORT
         # For some environments the STOMP TLS certificate will be different from the REST API cert
         default_stomp_cafile = self.getopt(self.DEFAULT_APP_SECTION, "stomp_cafile") or None
 
         default_stomp_url = self.getopt(self.DEFAULT_APP_SECTION, "stomp_host") or self.getopt(self.DEFAULT_APP_SECTION, "host")
@@ -121,14 +125,22 @@
                           type=str,
                           default=default_log_level,
                           help="Log level")
         self.add_argument("--logfile",
                           type=str,
                           default=default_log_file,
                           help="File to log to")
+        self.add_argument("--{0}".format(constants.APP_CONFIG_LOG_MAX_BYTES),
+                          type=int,
+                          default=default_log_max_bytes,
+                          help="Maximum bytes per log file")
+        self.add_argument("--{0}".format(constants.APP_CONFIG_LOG_BACKUP_COUNT),
+                          type=int,
+                          default=default_log_backup_count,
+                          help="Number of log files to create in rotation")
         self.add_argument("--no-prompt-password",
                           type=bool,
                           default=default_no_prompt_password,
                           help="Never prompt for password on stdin")
         self.add_argument("--test-actions",
                           action="store_true",
                           default=default_test_actions,
```

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/app_function_component.py` & `resilient_circuits-48.1.4243/resilient_circuits/app_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/app_restartable.py` & `resilient_circuits-48.1.4243/resilient_circuits/app_restartable.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 """Action Module server - restartable version of App"""
 
 from __future__ import print_function
 
 import logging
 import os
+
 import filelock
-import resilient
 from circuits import Event, Timer
-from watchdog.observers import Observer
+from resilient_circuits.app import (App, AppArgumentParser,
+                                    RotatingFileHandler, constants, get_lock,
+                                    helpers)
 from watchdog.events import PatternMatchingEventHandler
+from watchdog.observers import Observer
 
-from resilient_circuits.app import App, AppArgumentParser
-from resilient_circuits.app import get_lock
-
+import resilient
 
 application = None
 LOG = logging.getLogger(__name__)
 
 
 class reload(Event):
     """Notify components of updates to config"""
@@ -63,17 +64,19 @@
 
         if self.app.reloading:
             LOG.warning("Configuration file change ignored because reload already in progress")
             return
 
         LOG.info("Configuration file has changed! Notify components to reload")
         self.app.reloading = True
-        opts = AppArgumentParser().parse_args()
+        opts = helpers.get_configs(path_config_file=self.app.config_file, ALLOW_UNRECOGNIZED=self.app.ALLOW_UNRECOGNIZED)
         # See if we need to reset root loglevel on reload
         self.reset_loglevel(opts)
+        # check if we need to reset rotating file handler opts
+        self.reset_filehandler(opts)
         reload_event = reload(opts=opts)
         self.app.reload_timer = Timer(self.max_reload_time, Event.create("reload_timeout"))
         self.app.fire(reload_event)
         self.app.reload_timer.register(self.app)
 
     def reset_loglevel(self, opts):
         """ Reset the loglevel if it has changed in the config file. """
@@ -89,14 +92,37 @@
                 root_logger = logging.getLogger()
                 # If level is different set loglevel to new value.
                 if logging.getLevelName(root_logger.level) != config_loglevel.upper():
                     root_logger.setLevel(config_loglevel.upper())
             else:
                 LOG.error("Invalid app.config setting for loglevel %s", config_loglevel)
 
+    def reset_filehandler(self, opts):
+        """
+        Reset ``log_max_bytes`` and ``log_backup_count`` if changed on reload
+        """
+
+        log_max_bytes = opts.get(constants.APP_CONFIG_LOG_MAX_BYTES)
+        log_backup_count = opts.get(constants.APP_CONFIG_LOG_BACKUP_COUNT)
+
+        # loop through handlers and find the RotatingFileHandler
+        # (it will be there -- just need to find it in the list)
+        handlers = getattr(logging.getLogger(), "handlers", [])
+        for handler in handlers:
+            if isinstance(handler, RotatingFileHandler):
+
+                # update values as appropriate
+                if log_backup_count is not None and handler.backupCount != log_backup_count:
+                    LOG.debug("Reloaded 'log_backup_count' to '%s'",log_backup_count)
+                    handler.backupCount = log_backup_count
+                if log_max_bytes is not None and handler.maxBytes != log_max_bytes:
+                    LOG.debug("Reloaded 'log_max_bytes' to '%s'", log_max_bytes)
+                    handler.maxBytes = log_max_bytes
+                break # break the loop as we only needed the RotatingFileHandler
+
 # Main component for our application
 class AppRestartable(App):
     """Our main app component, which sets up the Resilient services and other components"""
 
     def __init__(self, *args, **kwargs):
         super(AppRestartable, self).__init__(*args, **kwargs)
         self.reloading = False
```

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/bin/res_action_test.py` & `resilient_circuits-48.1.4243/resilient_circuits/bin/res_action_test.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/bin/resilient_circuits_cmd.py` & `resilient_circuits-48.1.4243/resilient_circuits/bin/resilient_circuits_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/bin/service_wrapper.py` & `resilient_circuits-48.1.4243/resilient_circuits/bin/service_wrapper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/cmds/selftest.py` & `resilient_circuits-48.1.4243/resilient_circuits/cmds/selftest.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/component_loader.py` & `resilient_circuits-48.1.4243/resilient_circuits/component_loader.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/constants.py` & `resilient_circuits-48.1.4243/resilient_circuits/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 
 import os
 
 import pkg_resources
 
 PACKAGE_NAME = "resilient-circuits"
 
-PASSWD_PATTERNS = ['pass', 'secret', 'pin', 'key', 'id']
+PASSWD_PATTERNS = ['token', 'pass', 'secret', 'pin', 'key', 'id']
 
 INBOUND_MSG_DEST_PREFIX = "inbound_destinations"
 
 APP_FUNCTION_PAYLOAD_VERSION = 2.0
 
 MIN_NUM_WORKERS = 1
 MAX_NUM_WORKERS = 500
+MIN_LOG_BYTES = 100000
+MIN_BACKUP_COUNT = 0
 DEFAULT_SELFTEST_TIMEOUT_VALUE = 10
 
 APP_LOG_DIR = os.environ.get("APP_LOG_DIR", "logs")
 CMDS_LOGGER_NAME = "resilient_circuits_cmd_logger"
 LOG_DIVIDER = "\n------------------------\n"
 
 DEFAULT_NONE_STR = "Not found"
@@ -34,14 +36,16 @@
 SELFTEST_UNIMPLEMENTED_STATE = "unimplemented"
 
 # app configs
 INBOUND_MSG_APP_CONFIG_Q_NAME = "inbound_destination_api_name"
 APP_CONFIG_TRAP_EXCEPTION = "trap_exception"
 APP_CONFIG_SELFTEST_TIMEOUT = "selftest_timeout"
 APP_CONFIG_HEARTBEAT_TIMEOUT_THRESHOLD = "heartbeat_timeout_threshold"
+APP_CONFIG_LOG_MAX_BYTES = "log_max_bytes"
+APP_CONFIG_LOG_BACKUP_COUNT = "log_backup_count"
 
 # Headers
 HEADER_CIRCUITS_VER_KEY = "Resilient-Circuits-Version"
 HEADER_CIRCUITS_VER_VALUE = pkg_resources.get_distribution(PACKAGE_NAME).version
 
 # Exit Codes
 EXIT_SELFTEST_ERROR = 1             # Error running App's selftest
@@ -55,8 +59,8 @@
 EXIT_STOMP_ERROR = 30               # STOMP: Generic connection error
 EXIT_STOMP_UNAUTHORIZED_CONN = 31   # STOMP: Not authorized to instansiate STOMP connection
 EXIT_STOMP_UNAUTHORIZED_Q = 32      # STOMP: Not authorized to read from queue
 EXIT_STOMP_Q_TIMEOUT = 33           # STOMP: Timed out trying to see if resilient-circuits is subscribed to a message destination
 EXIT_STOMP_HEARTBEAT_TIMEOUT = 34   # STOMP: The delta of the current HeartbeatTimeout event and the first HeartbeatTimeout event is greater than the 'heartbeat_timeout_threshold'
 
 # STOMP connection constants
-STOMP_MAX_CONNECTION_ERRORS = 2     # default number of errors when heartbeat is lost
+STOMP_MAX_CONNECTION_ERRORS = 1     # default number of errors when heartbeat is lost
```

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/data/app.config.base` & `resilient_circuits-48.1.4243/resilient_circuits/data/app.config.base`

 * *Files 10% similar despite different names*

```diff
@@ -41,14 +41,23 @@
 
 # Directory containing additional components to load
 # componentsdir=components
 # Existing directory to write logs to, or set with $APP_LOG_DIR
 logdir=/tmp
 logfile=app.log
 loglevel=INFO
+# Optional override the default values for maximum bytes per log file
+# and maximum backup count. These default to 10000000 and 10
+# respectively.
+# Setting log_max_bytes to 0 is unlimited.
+# Setting log_backup_count to 0 means no backups will be used.
+# NOTE: if either log_max_bytes or log_backup_count are zero,
+# the log file will never roll over and will continue to grow
+#log_max_bytes=10000000
+#log_backup_count=10
 
 # The number of Functions to run concurrently (within the range: 1 <= 500)
 num_workers=50
 
 # Timeout value in seconds for selftest to wait for a response from SOAR
 selftest_timeout=10
```

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/decorators.py` & `resilient_circuits-48.1.4243/resilient_circuits/decorators.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/helpers.py` & `resilient_circuits-48.1.4243/resilient_circuits/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/rest_helper.py` & `resilient_circuits-48.1.4243/resilient_circuits/rest_helper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/stomp_component.py` & `resilient_circuits-48.1.4243/resilient_circuits/stomp_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/stomp_events.py` & `resilient_circuits-48.1.4243/resilient_circuits/stomp_events.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/stomp_transport.py` & `resilient_circuits-48.1.4243/resilient_circuits/stomp_transport.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/template_functions.py` & `resilient_circuits-48.1.4243/resilient_circuits/template_functions.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/util/__init__.py` & `resilient_circuits-48.1.4243/resilient_circuits/util/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/util/resilient_config.py` & `resilient_circuits-48.1.4243/resilient_circuits/util/resilient_config.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits/util/resilient_customize.py` & `resilient_circuits-48.1.4243/resilient_circuits/util/resilient_customize.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/resilient_circuits.egg-info/PKG-INFO` & `resilient_circuits-48.1.4243/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: resilient-circuits
-Version: 48.0.4034
+Name: resilient_circuits
+Version: 48.1.4243
 Summary: Framework used to run IBM SOAR Apps and Integrations
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_circuits-48.0.4034/resilient_circuits.egg-info/SOURCES.txt` & `resilient_circuits-48.1.4243/resilient_circuits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/setup.cfg` & `resilient_circuits-48.1.4243/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient     >= 48.0
-	resilient-lib >= 48.0
+	resilient     >= 48.1
+	resilient-lib >= 48.1
 	
 	stompest      ~= 2.3
 	circuits      ~= 3.2
 	pysocks       ~= 1.6
 	filelock      ~= 3.2
 	
 	watchdog      ~= 2.1;  python_version >= "3.6"
```

### Comparing `resilient_circuits-48.0.4034/tests/cmds/test_selftest.py` & `resilient_circuits-48.1.4243/tests/cmds/test_selftest.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/conftest.py` & `resilient_circuits-48.1.4243/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/helpers.py` & `resilient_circuits-48.1.4243/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/shared_mock_data/mock_app_config` & `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_app_config`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 
 # Directory containing additional components to load
 # componentsdir=components
 # Existing directory to write logs to, or set with $APP_LOG_DIR
 logdir=/tmp
 logfile=app.log
 loglevel=INFO
+log_max_bytes=20000000
+log_backup_count=11
 
 # The number of Functions to run in parallel
 num_workers=50
 
 heartbeat_timeout_threshold=5
 
 # If your Resilient server uses a self-signed TLS certificate, or some
```

### Comparing `resilient_circuits-48.0.4034/tests/shared_mock_data/mock_app_function_component.py` & `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_app_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/shared_mock_data/mock_commented_app_config` & `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_commented_app_config`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
 # Directory containing additional components to load
 # componentsdir=components
 # Existing directory to write logs to, or set with $APP_LOG_DIR
 logdir=/tmp
 logfile=app.log
 loglevel=INFO
+# log_max_bytes=10000000
+# log_backup_count=10
 
 # The number of Functions to run in parallel
 #num_workers=5
 
 # If your Resilient server uses a self-signed TLS certificate, or some
 # other certificate that is not automatically trusted by your machine,
 # you need to explicitly tell the Python scripts that it should be trusted.
```

### Comparing `resilient_circuits-48.0.4034/tests/shared_mock_data/mock_component.py` & `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/shared_mock_data/mock_constants.py` & `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_constants.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/shared_mock_data/mock_function_component.py` & `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/shared_mock_data/mock_import_definition.txt` & `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_import_definition.txt`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/shared_mock_data/mock_paths.py` & `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_paths.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/test_action_message.py` & `resilient_circuits-48.1.4243/tests/test_action_message.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/test_actions_component.py` & `resilient_circuits-48.1.4243/tests/test_actions_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/test_app_function_component.py` & `resilient_circuits-48.1.4243/tests/test_app_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/test_app_restartable.py` & `resilient_circuits-48.1.4243/tests/test_app_restartable.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 def test_reload_config_not_already_loading():
     magic_app = MagicMock()
     config_update_handler = ConfigFileUpdateHandler(magic_app)
     with patch("resilient_circuits.app_restartable.AppArgumentParser.parse_args") as mock_parse_args:
         mock_parse_args.return_value = {"loglevel": "DEBUG"}
         magic_app.reloading = False
+        magic_app.config_file = None
         config_update_handler.reload_config()
         assert config_update_handler.app.reloading
 
 def test_reload_config_is_already_loading():
     magic_app = MagicMock()
     config_update_handler = ConfigFileUpdateHandler(magic_app)
     with patch("resilient_circuits.app_restartable.AppArgumentParser.parse_args") as mock_parse_args:
```

### Comparing `resilient_circuits-48.0.4034/tests/test_component_loader.py` & `resilient_circuits-48.1.4243/tests/test_component_loader.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/test_decorators.py` & `resilient_circuits-48.1.4243/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/test_errors.py` & `resilient_circuits-48.1.4243/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/test_helpers.py` & `resilient_circuits-48.1.4243/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/test_resilient_circuits_cmd.py` & `resilient_circuits-48.1.4243/tests/test_resilient_circuits_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/test_rest_helper.py` & `resilient_circuits-48.1.4243/tests/test_rest_helper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/test_stomp_component.py` & `resilient_circuits-48.1.4243/tests/test_stomp_component.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,31 +20,26 @@
     with patch("resilient_circuits.stomp_component.Stomp.connect") as patch_stomp_library_connect:
         with patch("resilient_circuits.stomp_component.StompClient.connected") as patch_connected_state:
             patch_stomp_library_connect.side_effect = None
             patch_connected_state.return_value = True
             client.connect(mock_evt)
 
 
-            # first StompConnectionError with "no more data" error
-            patch_stomp_library_connect.side_effect = StompConnectionError("No more data received from STOMP")
-            client.connect(mock_evt)
-            assert client._stomp_connection_errors == 1
-
-            # now a StompConnectionError with a different error (this could be possible in real world)
+            # first a StompConnectionError with a different error (this could be possible in real world)
             patch_stomp_library_connect.side_effect = StompConnectionError("A different STOMP error")
             client.connect(mock_evt)
-            assert client._stomp_connection_errors == 1
+            assert client._stomp_connection_errors == 0
 
-            # now a second StompConnectionError with "no more data" error
+            # now a StompConnectionError with "no more data" error
             # this should trigger the max, and throw a sys.exit(1)
             patch_stomp_library_connect.side_effect = StompConnectionError("Some preamble. No more data received from STOMP")
             with pytest.raises(SystemExit):
                 client.connect(mock_evt)
                 assert "Exiting due to unrecoverable error" in caplog.text
-            assert client._stomp_connection_errors == 2
+            assert client._stomp_connection_errors == 1
 
 def test_stomp_reconnect_one_failure_followed_by_successful_reconnect(caplog):
 
     max_connection_errors_override = 5
     client = StompClient(host="example.com", port=443, stomp_max_connection_errors=max_connection_errors_override)
 
     assert client._stomp_max_connection_errors == max_connection_errors_override
```

### Comparing `resilient_circuits-48.0.4034/tests/test_templates.py` & `resilient_circuits-48.1.4243/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tests/util/test_resilient_customize.py` & `resilient_circuits-48.1.4243/tests/util/test_resilient_customize.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.0.4034/tox.ini` & `resilient_circuits-48.1.4243/tox.ini`

 * *Files identical despite different names*

