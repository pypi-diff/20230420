# Comparing `tmp/bsl-appcli-1.4.0.tar.gz` & `tmp/bsl-appcli-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsl-appcli-1.4.0.tar", last modified: Wed Apr 19 04:06:31 2023, max compression
+gzip compressed data, was "bsl-appcli-1.5.0.tar", last modified: Thu Apr 20 02:01:06 2023, max compression
```

## Comparing `bsl-appcli-1.4.0.tar` & `bsl-appcli-1.5.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.539481 bsl-appcli-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    36266 2023-04-19 04:06:31.539481 bsl-appcli-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35907 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/appcli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/appcli/backup_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/backup_manager/backup_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/backup_manager/remote_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/cli_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/appcli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/appcli_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/backup_manager_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/configure_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/configure_template_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/debug_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/encrypt_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/init_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/install_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/launcher_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/migrate_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/service_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/task_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/version_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/appcli/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/common/data_class_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/appcli/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/configuration/configuration_dir_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    25435 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/appcli/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/crypto/cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/crypto/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/appcli/git_repositories/
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/git_repositories/git_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/keycloak_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/appcli/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/models/cli_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/models/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    28248 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/orchestrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/string_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/appcli/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/templates/installer.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/templates/launcher.j2
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/variables_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/bsl_appcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36266 2023-04-19 04:06:31.000000 bsl-appcli-1.4.0/bsl_appcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-19 04:06:31.000000 bsl-appcli-1.4.0/bsl_appcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 04:06:31.000000 bsl-appcli-1.4.0/bsl_appcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-19 04:06:31.000000 bsl-appcli-1.4.0/bsl_appcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 04:06:31.000000 bsl-appcli-1.4.0/bsl_appcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 04:06:31.539481 bsl-appcli-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/backup_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/backup_manager/test_backup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/cipher/
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/cipher/test_cipher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/commands/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/commands/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/commands/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/commands/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/commands/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/commands/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/commands/test_install_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/commands_task/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/commands_task/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/commands_task/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/commands_task/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/commands_task/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/commands_task/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/commands_task/test_commands_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/configuration/test_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/configuration_manager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/configuration_manager/expected_generated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/configuration_manager/expected_generated/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/configuration_manager/expected_generated/nesting/nested_baseline_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/configuration_manager/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/configuration_manager/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/configuration_manager/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/configuration_manager/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/configuration_manager/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/configuration_manager/test_configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/configuration_state/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/configuration_state/test_configuration_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/crypto/test_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/git_repositories/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/git_repositories/test_git_repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/string_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/string_transformer/test_string_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/variables_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/variables_manager/test_variables_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/version/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/version/test_version.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.522488 bsl-appcli-1.5.0/
+-rw-r--r--   0 al        (1000) al        (1000)     1085 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/LICENSE
+-rw-r--r--   0 al        (1000) al        (1000)       30 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/MANIFEST.in
+-rw-r--r--   0 al        (1000) al        (1000)    36266 2023-04-20 02:01:06.522488 bsl-appcli-1.5.0/PKG-INFO
+-rw-r--r--   0 al        (1000) al        (1000)    35907 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/README.md
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.515821 bsl-appcli-1.5.0/appcli/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.515821 bsl-appcli-1.5.0/appcli/backup_manager/
+-rw-r--r--   0 al        (1000) al        (1000)    22873 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/backup_manager/backup_manager.py
+-rw-r--r--   0 al        (1000) al        (1000)     8376 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/appcli/backup_manager/remote_strategy.py
+-rw-r--r--   0 al        (1000) al        (1000)    13220 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/cli_builder.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/appcli/commands/
+-rw-r--r--   0 al        (1000) al        (1000)     1368 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/appcli/commands/appcli_command.py
+-rw-r--r--   0 al        (1000) al        (1000)     8349 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/commands/backup_manager_cli.py
+-rw-r--r--   0 al        (1000) al        (1000)    10246 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/appcli/commands/configure_cli.py
+-rw-r--r--   0 al        (1000) al        (1000)     8018 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/commands/configure_template_cli.py
+-rw-r--r--   0 al        (1000) al        (1000)     2340 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/appcli/commands/debug_cli.py
+-rw-r--r--   0 al        (1000) al        (1000)     1914 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/commands/encrypt_cli.py
+-rw-r--r--   0 al        (1000) al        (1000)     2415 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/commands/init_cli.py
+-rw-r--r--   0 al        (1000) al        (1000)     4304 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/commands/install_cli.py
+-rw-r--r--   0 al        (1000) al        (1000)     3336 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/commands/launcher_cli.py
+-rw-r--r--   0 al        (1000) al        (1000)     2064 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/commands/migrate_cli.py
+-rw-r--r--   0 al        (1000) al        (1000)    10273 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/commands/service_cli.py
+-rw-r--r--   0 al        (1000) al        (1000)     2804 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/commands/task_cli.py
+-rw-r--r--   0 al        (1000) al        (1000)     1303 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/commands/version_cli.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/appcli/common/
+-rw-r--r--   0 al        (1000) al        (1000)     1556 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/appcli/common/data_class_extensions.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/appcli/configuration/
+-rw-r--r--   0 al        (1000) al        (1000)    13861 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/configuration/configuration_dir_state.py
+-rw-r--r--   0 al        (1000) al        (1000)    25435 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/configuration_manager.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/appcli/crypto/
+-rw-r--r--   0 al        (1000) al        (1000)     3987 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/appcli/crypto/cipher.py
+-rw-r--r--   0 al        (1000) al        (1000)     2372 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/appcli/crypto/crypto.py
+-rw-r--r--   0 al        (1000) al        (1000)     3086 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/appcli/functions.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/appcli/git_repositories/
+-rw-r--r--   0 al        (1000) al        (1000)     8026 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/appcli/git_repositories/git_repositories.py
+-rw-r--r--   0 al        (1000) al        (1000)     9981 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/keycloak_manager.py
+-rw-r--r--   0 al        (1000) al        (1000)     1157 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/appcli/logger.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/appcli/models/
+-rw-r--r--   0 al        (1000) al        (1000)     5719 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/models/cli_context.py
+-rw-r--r--   0 al        (1000) al        (1000)     9179 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/models/configuration.py
+-rw-r--r--   0 al        (1000) al        (1000)    28248 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/orchestrators.py
+-rw-r--r--   0 al        (1000) al        (1000)     3669 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/string_transformer.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/appcli/templates/
+-rw-r--r--   0 al        (1000) al        (1000)      196 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/appcli/templates/__init__.py
+-rw-r--r--   0 al        (1000) al        (1000)     4998 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/templates/installer.j2
+-rw-r--r--   0 al        (1000) al        (1000)     3559 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/appcli/templates/launcher.j2
+-rw-r--r--   0 al        (1000) al        (1000)    10966 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/appcli/variables_manager.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/bsl_appcli.egg-info/
+-rw-r--r--   0 al        (1000) al        (1000)    36266 2023-04-20 02:01:06.000000 bsl-appcli-1.5.0/bsl_appcli.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) al        (1000)     2104 2023-04-20 02:01:06.000000 bsl-appcli-1.5.0/bsl_appcli.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) al        (1000)        1 2023-04-20 02:01:06.000000 bsl-appcli-1.5.0/bsl_appcli.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) al        (1000)      321 2023-04-20 02:01:06.000000 bsl-appcli-1.5.0/bsl_appcli.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) al        (1000)       18 2023-04-20 02:01:06.000000 bsl-appcli-1.5.0/bsl_appcli.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) al        (1000)       38 2023-04-20 02:01:06.522488 bsl-appcli-1.5.0/setup.cfg
+-rw-r--r--   0 al        (1000) al        (1000)     2390 2023-04-19 04:04:30.000000 bsl-appcli-1.5.0/setup.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.512488 bsl-appcli-1.5.0/tests/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/tests/backup_manager/
+-rw-r--r--   0 al        (1000) al        (1000)    36535 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/tests/backup_manager/test_backup_manager.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/tests/cipher/
+-rw-r--r--   0 al        (1000) al        (1000)     1870 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/tests/cipher/test_cipher.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/tests/commands/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.512488 bsl-appcli-1.5.0/tests/commands/resources/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.512488 bsl-appcli-1.5.0/tests/commands/resources/templates/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.512488 bsl-appcli-1.5.0/tests/commands/resources/templates/baseline/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/tests/commands/resources/templates/baseline/nesting/
+-rw-r--r--   0 al        (1000) al        (1000)        0 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/tests/commands/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 al        (1000) al        (1000)    17566 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/tests/commands/test_commands.py
+-rw-r--r--   0 al        (1000) al        (1000)     1816 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/tests/commands/test_install_script.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/tests/commands_task/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.512488 bsl-appcli-1.5.0/tests/commands_task/resources/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.512488 bsl-appcli-1.5.0/tests/commands_task/resources/templates/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.512488 bsl-appcli-1.5.0/tests/commands_task/resources/templates/baseline/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/tests/commands_task/resources/templates/baseline/nesting/
+-rw-r--r--   0 al        (1000) al        (1000)        0 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/tests/commands_task/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 al        (1000) al        (1000)     6570 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/tests/commands_task/test_commands_task.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.519154 bsl-appcli-1.5.0/tests/configuration/
+-rw-r--r--   0 al        (1000) al        (1000)     1942 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/tests/configuration/test_configuration.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.522488 bsl-appcli-1.5.0/tests/configuration_manager/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.512488 bsl-appcli-1.5.0/tests/configuration_manager/expected_generated/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.522488 bsl-appcli-1.5.0/tests/configuration_manager/expected_generated/nesting/
+-rw-r--r--   0 al        (1000) al        (1000)        0 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/tests/configuration_manager/expected_generated/nesting/nested_baseline_file.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.512488 bsl-appcli-1.5.0/tests/configuration_manager/resources/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.512488 bsl-appcli-1.5.0/tests/configuration_manager/resources/templates/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.512488 bsl-appcli-1.5.0/tests/configuration_manager/resources/templates/baseline/
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.522488 bsl-appcli-1.5.0/tests/configuration_manager/resources/templates/baseline/nesting/
+-rw-r--r--   0 al        (1000) al        (1000)        0 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/tests/configuration_manager/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 al        (1000) al        (1000)     9109 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/tests/configuration_manager/test_configuration_manager.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.522488 bsl-appcli-1.5.0/tests/configuration_state/
+-rw-r--r--   0 al        (1000) al        (1000)     2463 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/tests/configuration_state/test_configuration_state.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.522488 bsl-appcli-1.5.0/tests/crypto/
+-rw-r--r--   0 al        (1000) al        (1000)     2004 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/tests/crypto/test_crypto.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.522488 bsl-appcli-1.5.0/tests/git_repositories/
+-rw-r--r--   0 al        (1000) al        (1000)     3466 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/tests/git_repositories/test_git_repositories.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.522488 bsl-appcli-1.5.0/tests/string_transformer/
+-rw-r--r--   0 al        (1000) al        (1000)     2676 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/tests/string_transformer/test_string_transformer.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.522488 bsl-appcli-1.5.0/tests/variables_manager/
+-rw-r--r--   0 al        (1000) al        (1000)    10415 2022-10-10 02:56:22.000000 bsl-appcli-1.5.0/tests/variables_manager/test_variables_manager.py
+drwxr-sr-x   0 al        (1000) al        (1000)        0 2023-04-20 02:01:06.522488 bsl-appcli-1.5.0/tests/version/
+-rw-r--r--   0 al        (1000) al        (1000)     1459 2023-04-19 03:29:47.000000 bsl-appcli-1.5.0/tests/version/test_version.py
```

### Comparing `bsl-appcli-1.4.0/LICENSE` & `bsl-appcli-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/PKG-INFO` & `bsl-appcli-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsl-appcli
-Version: 1.4.0
+Version: 1.5.0
 Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
 Home-page: https://www.brightsparklabs.com
 Author: brightSPARK Labs
 Author-email: enquire@brightsparklabs.com
 License: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `bsl-appcli-1.4.0/README.md` & `bsl-appcli-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/backup_manager/backup_manager.py` & `bsl-appcli-1.5.0/appcli/backup_manager/backup_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/backup_manager/remote_strategy.py` & `bsl-appcli-1.5.0/appcli/backup_manager/remote_strategy.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/cli_builder.py` & `bsl-appcli-1.5.0/appcli/cli_builder.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/commands/appcli_command.py` & `bsl-appcli-1.5.0/appcli/commands/appcli_command.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/commands/backup_manager_cli.py` & `bsl-appcli-1.5.0/appcli/commands/backup_manager_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/commands/configure_cli.py` & `bsl-appcli-1.5.0/appcli/commands/configure_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/commands/configure_template_cli.py` & `bsl-appcli-1.5.0/appcli/commands/configure_template_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/commands/debug_cli.py` & `bsl-appcli-1.5.0/appcli/commands/debug_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/commands/encrypt_cli.py` & `bsl-appcli-1.5.0/appcli/commands/encrypt_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/commands/init_cli.py` & `bsl-appcli-1.5.0/appcli/commands/init_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/commands/install_cli.py` & `bsl-appcli-1.5.0/appcli/commands/install_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/commands/launcher_cli.py` & `bsl-appcli-1.5.0/appcli/commands/launcher_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/commands/migrate_cli.py` & `bsl-appcli-1.5.0/appcli/commands/migrate_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/commands/service_cli.py` & `bsl-appcli-1.5.0/appcli/commands/service_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/commands/task_cli.py` & `bsl-appcli-1.5.0/appcli/commands/task_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/commands/version_cli.py` & `bsl-appcli-1.5.0/appcli/commands/version_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/common/data_class_extensions.py` & `bsl-appcli-1.5.0/appcli/common/data_class_extensions.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/configuration/configuration_dir_state.py` & `bsl-appcli-1.5.0/appcli/configuration/configuration_dir_state.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/configuration_manager.py` & `bsl-appcli-1.5.0/appcli/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/crypto/cipher.py` & `bsl-appcli-1.5.0/appcli/crypto/cipher.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/crypto/crypto.py` & `bsl-appcli-1.5.0/appcli/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/functions.py` & `bsl-appcli-1.5.0/appcli/functions.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/git_repositories/git_repositories.py` & `bsl-appcli-1.5.0/appcli/git_repositories/git_repositories.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/keycloak_manager.py` & `bsl-appcli-1.5.0/appcli/keycloak_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/logger.py` & `bsl-appcli-1.5.0/appcli/logger.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/models/cli_context.py` & `bsl-appcli-1.5.0/appcli/models/cli_context.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/models/configuration.py` & `bsl-appcli-1.5.0/appcli/models/configuration.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/orchestrators.py` & `bsl-appcli-1.5.0/appcli/orchestrators.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/string_transformer.py` & `bsl-appcli-1.5.0/appcli/string_transformer.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/templates/installer.j2` & `bsl-appcli-1.5.0/appcli/templates/installer.j2`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/templates/launcher.j2` & `bsl-appcli-1.5.0/appcli/templates/launcher.j2`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/appcli/variables_manager.py` & `bsl-appcli-1.5.0/appcli/variables_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/bsl_appcli.egg-info/PKG-INFO` & `bsl-appcli-1.5.0/bsl_appcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsl-appcli
-Version: 1.4.0
+Version: 1.5.0
 Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
 Home-page: https://www.brightsparklabs.com
 Author: brightSPARK Labs
 Author-email: enquire@brightsparklabs.com
 License: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `bsl-appcli-1.4.0/bsl_appcli.egg-info/SOURCES.txt` & `bsl-appcli-1.5.0/bsl_appcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/setup.py` & `bsl-appcli-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/tests/backup_manager/test_backup_manager.py` & `bsl-appcli-1.5.0/tests/backup_manager/test_backup_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/tests/cipher/test_cipher.py` & `bsl-appcli-1.5.0/tests/cipher/test_cipher.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/tests/commands/test_commands.py` & `bsl-appcli-1.5.0/tests/commands/test_commands.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/tests/commands/test_install_script.py` & `bsl-appcli-1.5.0/tests/commands/test_install_script.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/tests/commands_task/test_commands_task.py` & `bsl-appcli-1.5.0/tests/commands_task/test_commands_task.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/tests/configuration/test_configuration.py` & `bsl-appcli-1.5.0/tests/configuration/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/tests/configuration_manager/test_configuration_manager.py` & `bsl-appcli-1.5.0/tests/configuration_manager/test_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/tests/configuration_state/test_configuration_state.py` & `bsl-appcli-1.5.0/tests/configuration_state/test_configuration_state.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/tests/crypto/test_crypto.py` & `bsl-appcli-1.5.0/tests/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/tests/git_repositories/test_git_repositories.py` & `bsl-appcli-1.5.0/tests/git_repositories/test_git_repositories.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/tests/string_transformer/test_string_transformer.py` & `bsl-appcli-1.5.0/tests/string_transformer/test_string_transformer.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/tests/variables_manager/test_variables_manager.py` & `bsl-appcli-1.5.0/tests/variables_manager/test_variables_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.4.0/tests/version/test_version.py` & `bsl-appcli-1.5.0/tests/version/test_version.py`

 * *Files identical despite different names*

