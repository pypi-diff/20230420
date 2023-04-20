# Comparing `tmp/resilient_sdk-48.0.4034.tar.gz` & `tmp/resilient_sdk-48.1.4243.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_sdk-48.0.4034.tar", last modified: Tue Feb 28 15:24:18 2023, max compression
+gzip compressed data, was "resilient_sdk-48.1.4243.tar", last modified: Thu Apr 20 19:35:53 2023, max compression
```

## Comparing `resilient_sdk-48.0.4034.tar` & `resilient_sdk-48.1.4243.tar`

### file list

```diff
@@ -1,252 +1,256 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:18.178444 resilient_sdk-48.0.4034/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8344 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     3152 2023-02-28 15:24:18.178444 resilient_sdk-48.0.4034/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2385 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.778444 resilient_sdk-48.0.4034/assets/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    62353 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/assets/IBM_Security_lockup_pos_RGB.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.778444 resilient_sdk-48.0.4034/resilient_sdk/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6105 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/app.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.778444 resilient_sdk-48.0.4034/resilient_sdk/cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)      456 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8183 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/cmds/base_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36429 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/cmds/clone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35159 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/cmds/codegen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10010 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/cmds/dev.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21294 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/cmds/docgen.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.778444 resilient_sdk-48.0.4034/resilient_sdk/cmds/ext/
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/cmds/ext/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8445 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/cmds/ext/ext_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7602 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/cmds/extract.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48148 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/cmds/validate.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.770444 resilient_sdk-48.0.4034/resilient_sdk/data/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.770444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.770444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.778444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2663 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      454 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/MANIFEST.in.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      342 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/README.md.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      534 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.770444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/doc/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/
--rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      743 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/entrypoint.sh.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/LICENSE.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      145 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/__init__.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/components/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/components/__init__.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3082 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/lib/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/lib/__init__.py.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     7886 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/poller/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/poller/__init__.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/poller/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_close_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_update_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)    10722 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/util/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/util/__init__.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      913 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4885 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/util/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/util/data/export.res.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      975 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.770444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/payload_samples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/blank.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_fail.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_success.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     2256 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/tests/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3132 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      750 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.770444 resilient_sdk-48.0.4034/resilient_sdk/data/docgen/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/docgen/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15077 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/docgen/templates/README.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.770444 resilient_sdk-48.0.4034/resilient_sdk/data/ext/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/ext/icons/
--rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/ext/icons/app_logo.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/ext/icons/company_logo.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/validate/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18106 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/validate/.pylintrc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.782444 resilient_sdk-48.0.4034/resilient_sdk/data/validate/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/data/validate/templates/validate_report.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.786444 resilient_sdk-48.0.4034/resilient_sdk/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5890 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/util/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3006 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/util/jinja2_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53165 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/util/package_file_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2464 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/util/resilient_objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/util/sdk_argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      817 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/util/sdk_exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3168 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/util/sdk_genson_overwrites.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    58497 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/util/sdk_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28324 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/util/sdk_validate_configs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    86157 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/util/sdk_validate_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3388 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/resilient_sdk/util/sdk_validate_issue.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.778444 resilient_sdk-48.0.4034/resilient_sdk.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3152 2023-02-28 15:24:17.000000 resilient_sdk-48.0.4034/resilient_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    15453 2023-02-28 15:24:17.000000 resilient_sdk-48.0.4034/resilient_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:24:17.000000 resilient_sdk-48.0.4034/resilient_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2023-02-28 15:24:17.000000 resilient_sdk-48.0.4034/resilient_sdk.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      108 2023-02-28 15:24:17.000000 resilient_sdk-48.0.4034/resilient_sdk.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-02-28 15:24:17.000000 resilient_sdk-48.0.4034/resilient_sdk.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1171 2023-02-28 15:24:18.178444 resilient_sdk-48.0.4034/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.786444 resilient_sdk-48.0.4034/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15506 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3772 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.786444 resilient_sdk-48.0.4034/tests/integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/integration/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1227 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/integration/test_installation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.790444 resilient_sdk-48.0.4034/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      721 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/.mock_sdk_settings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        3 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)    23891 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_app.log
--rw-rw-r--   0 travis    (2000) travis    (2000)      292 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   224427 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    58851 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_export.resz
--rw-rw-r--   0 travis    (2000) travis    (2000)   223680 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_export_corrupt.res
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.790444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/
--rw-rw-r--   0 travis    (2000) travis    (2000)      627 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    57247 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   191223 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/customize_old.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.790444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_app_zip_files/
--rw-rw-r--   0 travis    (2000) travis    (2000)    66751 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    41671 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    41951 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     2773 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   539154 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.774444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.794444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile
--rw-rw-r--   0 travis    (2000) travis    (2000)      214 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     5843 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1619 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.794444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      712 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.774444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.794444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/
--rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      566 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.794444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      145 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.866444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2254 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2061 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3465 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2355 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.866444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6889 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.866444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.866444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_close_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_update_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)    10660 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.942444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      591 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.946444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    49696 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.946444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/
--rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:17.774444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:18.014444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:18.014444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:18.014444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:18.098444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2005 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:18.098444 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2325 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2381 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      741 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)    53354 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     2352 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/setup_callable_data.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1798 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/setup_py_lines.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2795 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_paths.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   413882 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_reload_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     1102 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/mock_xml_test_report.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:18.106444 resilient_sdk-48.0.4034/tests/shared_mock_data/resilient_api_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)  3241462 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)   594886 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/resilient_api_data/export.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     1449 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/resilient_api_data/orgs.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/resilient_api_data/session.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     2056 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/shared_mock_data/resilient_api_mock.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:18.106444 resilient_sdk-48.0.4034/tests/unit/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1830 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_app.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:18.174444 resilient_sdk-48.0.4034/tests/unit/test_cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_cmds/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:18.178444 resilient_sdk-48.0.4034/tests/unit/test_cmds/ext/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_cmds/ext/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6916 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_cmds/ext/test_ext_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2070 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_cmds/test_base_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20782 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_cmds/test_clone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32103 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_cmds/test_codegen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2736 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_cmds/test_dev.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10659 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_cmds/test_docgen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1145 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_cmds/test_extract.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23815 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_cmds/test_validate.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:24:18.178444 resilient_sdk-48.0.4034/tests/unit/test_util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2148 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_util/test_jinja_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18754 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_util/test_package_file_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_util/test_resilient_objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      470 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_util/test_sdk_argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      947 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_util/test_sdk_exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26709 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_util/test_sdk_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3988 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_util/test_sdk_validate_configs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47944 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_util/test_sdk_validate_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tests/unit/test_util/test_sdk_validate_issue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      943 2023-02-28 15:22:43.000000 resilient_sdk-48.0.4034/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:53.227501 resilient_sdk-48.1.4243/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8523 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3152 2023-04-20 19:35:53.227501 resilient_sdk-48.1.4243/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2385 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.911501 resilient_sdk-48.1.4243/assets/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    62353 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/assets/IBM_Security_lockup_pos_RGB.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.911501 resilient_sdk-48.1.4243/resilient_sdk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6354 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/app.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.911501 resilient_sdk-48.1.4243/resilient_sdk/cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      507 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8183 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/cmds/base_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36429 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/cmds/clone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35393 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/cmds/codegen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10010 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/cmds/dev.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21294 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/cmds/docgen.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.911501 resilient_sdk-48.1.4243/resilient_sdk/cmds/ext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/cmds/ext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8445 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/cmds/ext/ext_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7602 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/cmds/extract.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5757 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/cmds/run_init.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48148 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/cmds/validate.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.907501 resilient_sdk-48.1.4243/resilient_sdk/data/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.907501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.907501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.911501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2853 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      454 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/MANIFEST.in.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      342 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/README.md.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.911501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      534 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.907501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/doc/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.911501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      743 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/entrypoint.sh.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.915501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/LICENSE.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      145 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/__init__.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.915501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/components/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/components/__init__.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3082 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.915501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/lib/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/lib/__init__.py.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7886 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.915501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/poller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/poller/__init__.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.915501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/poller/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_close_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      351 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_update_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10722 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.915501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/util/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/util/__init__.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      913 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4885 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.915501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/util/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/util/data/export.res.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      975 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.907501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/payload_samples/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.915501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/blank.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_fail.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_success.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2018 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.915501 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/tests/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3132 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      750 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.907501 resilient_sdk-48.1.4243/resilient_sdk/data/docgen/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.915501 resilient_sdk-48.1.4243/resilient_sdk/data/docgen/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15077 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/docgen/templates/README.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.907501 resilient_sdk-48.1.4243/resilient_sdk/data/ext/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.915501 resilient_sdk-48.1.4243/resilient_sdk/data/ext/icons/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/ext/icons/app_logo.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/ext/icons/company_logo.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.915501 resilient_sdk-48.1.4243/resilient_sdk/data/run_init/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      773 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/run_init/sdk_settings.json.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.915501 resilient_sdk-48.1.4243/resilient_sdk/data/validate/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18106 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/validate/.pylintrc
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.915501 resilient_sdk-48.1.4243/resilient_sdk/data/validate/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/data/validate/templates/validate_report.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.919501 resilient_sdk-48.1.4243/resilient_sdk/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8225 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/util/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3006 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/util/jinja2_filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53165 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/util/package_file_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2464 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/util/resilient_objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/util/sdk_argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      817 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/util/sdk_exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3168 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/util/sdk_genson_overwrites.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58615 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/util/sdk_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28324 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/util/sdk_validate_configs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86171 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/util/sdk_validate_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3388 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/resilient_sdk/util/sdk_validate_issue.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.911501 resilient_sdk-48.1.4243/resilient_sdk.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3152 2023-04-20 19:35:52.000000 resilient_sdk-48.1.4243/resilient_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15575 2023-04-20 19:35:52.000000 resilient_sdk-48.1.4243/resilient_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:35:52.000000 resilient_sdk-48.1.4243/resilient_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       57 2023-04-20 19:35:52.000000 resilient_sdk-48.1.4243/resilient_sdk.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      108 2023-04-20 19:35:52.000000 resilient_sdk-48.1.4243/resilient_sdk.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-04-20 19:35:52.000000 resilient_sdk-48.1.4243/resilient_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1171 2023-04-20 19:35:53.227501 resilient_sdk-48.1.4243/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.919501 resilient_sdk-48.1.4243/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16619 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3772 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.919501 resilient_sdk-48.1.4243/tests/integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/tests/integration/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1227 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/tests/integration/test_installation.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.923501 resilient_sdk-48.1.4243/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      806 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/.mock_sdk_settings.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        3 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24687 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_app.log
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2023-04-20 19:34:28.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   224427 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58851 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_export.resz
+-rw-rw-r--   0 travis    (2000) travis    (2000)   223680 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_export_corrupt.res
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.927501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      627 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    57247 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   191223 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/customize_old.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.931501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_app_zip_files/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    66751 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41671 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41951 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2773 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   539154 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.907501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.931501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile
+-rw-rw-r--   0 travis    (2000) travis    (2000)      214 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5843 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1619 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.931501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      712 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.907501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.931501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      566 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.931501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       30 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      145 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.995501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2254 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2061 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3465 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2355 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.995501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6889 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.999501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.999501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_close_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      351 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_update_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10660 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.999501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      591 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:53.055501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49696 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:53.055501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:52.907501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:53.119501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:53.119501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:53.119501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)       56 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:53.171501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_schema.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2005 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:53.171501 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2325 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2381 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      741 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53354 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2352 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/setup_callable_data.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1798 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/setup_py_lines.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2795 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_paths.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   413882 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_reload_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1102 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/mock_xml_test_report.xml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:53.175501 resilient_sdk-48.1.4243/tests/shared_mock_data/resilient_api_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  3241462 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)   594886 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/resilient_api_data/export.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1449 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/resilient_api_data/orgs.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/resilient_api_data/session.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2056 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/shared_mock_data/resilient_api_mock.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:53.175501 resilient_sdk-48.1.4243/tests/unit/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1830 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_app.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:53.179501 resilient_sdk-48.1.4243/tests/unit/test_cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_cmds/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:53.223501 resilient_sdk-48.1.4243/tests/unit/test_cmds/ext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_cmds/ext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6916 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_cmds/ext/test_ext_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2070 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_cmds/test_base_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20782 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_cmds/test_clone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32212 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_cmds/test_codegen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2736 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_cmds/test_dev.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10659 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_cmds/test_docgen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1145 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_cmds/test_extract.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5876 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_cmds/test_run_init.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23815 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_cmds/test_validate.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:53.227501 resilient_sdk-48.1.4243/tests/unit/test_util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2148 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_util/test_jinja_filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18754 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_util/test_package_file_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_util/test_resilient_objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      470 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_util/test_sdk_argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      947 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_util/test_sdk_exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27286 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_util/test_sdk_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3988 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_util/test_sdk_validate_configs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48045 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_util/test_sdk_validate_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tests/unit/test_util/test_sdk_validate_issue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      943 2023-04-20 19:34:29.000000 resilient_sdk-48.1.4243/tox.ini
```

### Comparing `resilient_sdk-48.0.4034/CHANGES` & `resilient_sdk-48.1.4243/CHANGES`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+**2023-04: version 48.1**
+
+* Added new ``init`` functionality to the SDK
+* Added ``--settings`` option for ``codegen``, ``docgen``, and ``validate``
+* Bug fixes for ``validate``
+
 **2023-02: version 48.0**
 
 * ``clone`` command fixed when cloning subplaybooks with multiple input fields
 * ``resilient-sdk`` version is now added as a comment to all files generated or updated by the SDK
 * Added new ``--poller`` flag to ``docgen`` to support documentation for poller-based apps generated
   with ``resilient-sdk codegen [...] --poller``, including automatically formatting the poller template file contents
   into the README file
```

### Comparing `resilient_sdk-48.0.4034/PKG-INFO` & `resilient_sdk-48.1.4243/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient_sdk
-Version: 48.0.4034
+Version: 48.1.4243
 Summary: Python SDK for developing Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-sdk
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
 Project-URL: Change Log, https://ibm.biz/resilient-sdk-changes
```

### Comparing `resilient_sdk-48.0.4034/README.md` & `resilient_sdk-48.1.4243/README.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/assets/IBM_Security_lockup_pos_RGB.png` & `resilient_sdk-48.1.4243/assets/IBM_Security_lockup_pos_RGB.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/LICENSE` & `resilient_sdk-48.1.4243/resilient_sdk/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/app.py` & `resilient_sdk-48.1.4243/resilient_sdk/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """ TODO: module docstring """
 
 import logging
 import os
 import sys
 
 from resilient_sdk.cmds import (CmdClone, CmdCodegen, CmdDev, CmdDocgen,
-                                CmdExtPackage, CmdExtract, CmdValidate)
+                                CmdExtPackage, CmdExtract, CmdValidate, CmdRunInit)
 from resilient_sdk.util import constants, sdk_helpers, package_file_helpers
 from resilient_sdk.util.sdk_argparse import SDKArgumentParser
 from resilient_sdk.util.sdk_exception import SDKException
 
 # Setup logging
 LOG = logging.getLogger(constants.LOGGER_NAME)
 LOG.setLevel(logging.INFO)
@@ -115,14 +115,15 @@
     # Add any subcommands to main app parser here
     cmd_validate = CmdValidate(sub_parser)
     cmd_codegen = CmdCodegen(sub_parser)
     cmd_clone = CmdClone(sub_parser)
     cmd_docgen = CmdDocgen(sub_parser)
     cmd_extract = CmdExtract(sub_parser)
     cmd_ext_package = CmdExtPackage(sub_parser, cmd_validate=cmd_validate)
+    cmd_run_init = CmdRunInit(sub_parser)
 
     try:
         # Parse the arguments
         args = parser.parse_args()
 
         if args.cmd is None:
             parser.print_help()
@@ -154,14 +155,17 @@
 
             elif main_cmd == cmd_validate.CMD_NAME:
                 cmd_validate.parser.print_usage()
 
             elif sdk_dev and main_cmd == cmd_dev.CMD_NAME:
                 cmd_dev.parser.print_usage()
 
+            elif main_cmd == cmd_run_init.CMD_NAME:
+                cmd_run_init.parser.print_usage()
+
             else:
                 parser.print_help()
 
         # Exit
         sys.exit()
 
     # If -v was specified, set the log level to DEBUG
@@ -188,11 +192,14 @@
     elif args.cmd == cmd_ext_package.CMD_NAME:
         cmd_ext_package.execute_command(args)
 
     elif args.cmd == cmd_validate.CMD_NAME:
         cmd_validate.execute_command(args)
     elif sdk_dev and args.cmd == cmd_dev.CMD_NAME:
         cmd_dev.execute_command(args)
+    
+    elif args.cmd == cmd_run_init.CMD_NAME:
+        cmd_run_init.execute_command(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/cmds/base_cmd.py` & `resilient_sdk-48.1.4243/resilient_sdk/cmds/base_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/cmds/clone.py` & `resilient_sdk-48.1.4243/resilient_sdk/cmds/clone.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/cmds/codegen.py` & `resilient_sdk-48.1.4243/resilient_sdk/cmds/codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,21 +342,22 @@
         jinja_data["poller_flag"] = args.poller
 
         # add ::CHANGE_ME:: to jinja data
         jinja_data["change_me_str"] = constants.DOCGEN_PLACEHOLDER_STRING
 
         # add license name, author, author_email, url
         settings_file_contents_setup = settings_file_contents.get("setup", {})
-        jinja_data["license"] = settings_file_contents_setup.get("license", "<<insert here>>")
-        jinja_data["author"] = settings_file_contents_setup.get("author", "<<your name here>>")
-        jinja_data["author_email"] = settings_file_contents_setup.get("author_email", "you@example.com")
-        jinja_data["url"] = settings_file_contents_setup.get("url", "<<your company url>>")
+        jinja_data["license"] = settings_file_contents_setup.get("license", constants.CODEGEN_DEFAULT_SETUP_PY_LICENSE)
+        jinja_data["author"] = settings_file_contents_setup.get("author", constants.CODEGEN_DEFAULT_SETUP_PY_AUTHOR)
+        jinja_data["author_email"] = settings_file_contents_setup.get("author_email", constants.CODEGEN_DEFAULT_SETUP_PY_EMAIL)
+        jinja_data["url"] = settings_file_contents_setup.get("url", constants.CODEGEN_DEFAULT_SETUP_PY_URL)
+        jinja_data["long_description"] = settings_file_contents_setup.get("long_description", constants.CODEGEN_DEFAULT_SETUP_PY_LONG_DESC)
 
         # add license_content to jinja_data
-        jinja_data["license_content"] = settings_file_contents.get("license_content", "<<PUT YOUR LICENSE TEXT HERE>>")
+        jinja_data["license_content"] = settings_file_contents.get("license_content", constants.CODEGEN_DEFAULT_LICENSE_CONTENT)
         # add current SDK version to jinja data
         jinja_data["sdk_version"] = sdk_helpers.get_resilient_sdk_version()
 
         # Validate we have write permissions
         sdk_helpers.validate_dir_paths(os.W_OK, output_base)
 
         if not args.reload:
```

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/cmds/dev.py` & `resilient_sdk-48.1.4243/resilient_sdk/cmds/dev.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/cmds/docgen.py` & `resilient_sdk-48.1.4243/resilient_sdk/cmds/docgen.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/cmds/ext/ext_package.py` & `resilient_sdk-48.1.4243/resilient_sdk/cmds/ext/ext_package.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/cmds/extract.py` & `resilient_sdk-48.1.4243/resilient_sdk/cmds/extract.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/cmds/validate.py` & `resilient_sdk-48.1.4243/resilient_sdk/cmds/validate.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 # install the base package
 COPY ./dist /tmp/packages
 RUN pip install /tmp/packages/${APPLICATION}-*.tar.gz
 
 # uncomment and replicate if additional pypi packages are needed
 #RUN pip install <package>
 
+# uncomment and replicate if additional pypi packages in requirements file are needed
+#COPY /path/to/<requirements.txt> /tmp/packages/.
+#RUN pip install -r /tmp/packages/<requirements.txt>
+
 # uncomment and replicate if additional local packages are needed
 #COPY /path/to/extra_package /tmp/packages/.
 #RUN pip install /tmp/packages/<extra_package>*.tar.gz
 
 ## ---- end section for changes ----
 
 # set up configuration and log locations using /etc and /var/log, the conventional locations for config and logs
```

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/entrypoint.sh.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/entrypoint.sh.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2`

 * *Files 18% similar despite different names*

```diff
@@ -26,18 +26,15 @@
     display_name="<<display name of your app here>>",
     version="1.0.0",
     license="{{license}}",
     author="{{author}}",
     author_email="{{author_email}}",
     url="{{url}}",
     description="<<{{change_me_str}}>>Enter a short description of the App",
-    long_description="""<<{{change_me_str}}>>Enter a long description, including the key features of the App. \
-Multiple continuation lines are supported with a backslash. Line breaks are supported too:
-<br>- This will be rendered like a list
-<br>- once the App is installed in SOAR""",
+    long_description="""{{long_description}}""",
     install_requires=[
         "resilient-circuits>={{resilient_libraries_version}}"
     ],
     python_requires='>=3.6',
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
```

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/docgen/templates/README.md.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/docgen/templates/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/ext/icons/app_logo.png` & `resilient_sdk-48.1.4243/resilient_sdk/data/ext/icons/app_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/ext/icons/company_logo.png` & `resilient_sdk-48.1.4243/resilient_sdk/data/ext/icons/company_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/validate/.pylintrc` & `resilient_sdk-48.1.4243/resilient_sdk/data/validate/.pylintrc`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/data/validate/templates/validate_report.md.jinja2` & `resilient_sdk-48.1.4243/resilient_sdk/data/validate/templates/validate_report.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/util/jinja2_filters.py` & `resilient_sdk-48.1.4243/resilient_sdk/util/jinja2_filters.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/util/package_file_helpers.py` & `resilient_sdk-48.1.4243/resilient_sdk/util/package_file_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/util/resilient_objects.py` & `resilient_sdk-48.1.4243/resilient_sdk/util/resilient_objects.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/util/sdk_argparse.py` & `resilient_sdk-48.1.4243/resilient_sdk/util/sdk_argparse.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/util/sdk_exception.py` & `resilient_sdk-48.1.4243/resilient_sdk/util/sdk_exception.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/util/sdk_genson_overwrites.py` & `resilient_sdk-48.1.4243/resilient_sdk/util/sdk_genson_overwrites.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/util/sdk_helpers.py` & `resilient_sdk-48.1.4243/resilient_sdk/util/sdk_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,33 +18,35 @@
 import shutil
 import subprocess
 import sys
 import tempfile
 import time
 import uuid
 import xml.etree.ElementTree as ET
+from argparse import SUPPRESS
 from zipfile import BadZipfile, ZipFile, is_zipfile
 
 import pkg_resources
 import requests
 import requests.exceptions
 from jinja2 import Environment, PackageLoader
-from resilient import ArgumentParser
-from resilient import constants as res_constants
-from resilient import get_client, get_config_file
-from resilient.helpers import remove_tag
 from resilient_sdk.util import constants
 from resilient_sdk.util.jinja2_filters import add_filters_to_jinja_env
 from resilient_sdk.util.resilient_objects import (DEFAULT_INCIDENT_FIELD,
                                                   DEFAULT_INCIDENT_TYPE,
                                                   ResilientFieldTypes,
                                                   ResilientObjMap,
                                                   ResilientTypeIds)
 from resilient_sdk.util.sdk_exception import SDKException
 
+from resilient import ArgumentParser
+from resilient import constants as res_constants
+from resilient import get_client, get_config_file
+from resilient.helpers import remove_tag
+
 if sys.version_info.major < 3:
     # Handle PY 2 specific imports
     # JSONDecodeError is not available in PY2.7 so we set it to None
     JSONDecodeError = None
 else:
     # Handle PY 3 specific imports
     # reload(package) in PY2.7, importlib.reload(package) in PY3.6
@@ -1417,14 +1419,18 @@
     :return: Formatted string
     :rtype: str
     """
     parsed_optionals = []
 
     for option in optionals:
 
+        # skipped any suppressed options
+        if option.help == SUPPRESS:
+            continue
+
         option_strings = ", ".join(option.option_strings)
 
         tabs = "\t\t\t"
 
         if len(option_strings) >= 16:
             tabs = "\t\t"
 
@@ -1533,15 +1539,15 @@
 
     log_file_contents = read_file(path_log_file)
 
     regex_line = re.compile(r'\[[\w]+\] Result\:')       # Looking for line that contains [<fn_name>] Result: {'version': 2.0, 'success': True...
     regex_fn_name = re.compile(r'\[([\w]+)\] Result\:')  # Getting <fn_name> from [<fn_name>] Result: {'version': 2.0, 'success': True...
 
     for l in reversed(log_file_contents):
-        match = regex_line.search(l, endpos=120)
+        match = regex_line.search(l)
 
         if match:
             fn_name_group_index = 0
 
             fn_name_match = match.group(fn_name_group_index)
             fn_name_match_endpos = match.end(fn_name_group_index)
```

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/util/sdk_validate_configs.py` & `resilient_sdk-48.1.4243/resilient_sdk/util/sdk_validate_configs.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/util/sdk_validate_helpers.py` & `resilient_sdk-48.1.4243/resilient_sdk/util/sdk_validate_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,26 +637,26 @@
         # ignore and return an empty list
         return []
 
     issues = []
 
     # validate GLOBAL scripts are all python3 only.
     # for each non-python3 script we find, create an issue
-    for script in export_res.get("scripts", []):
+    for script in export_res.get("scripts") or []:
         if script.get("language", "") not in constants.EXPORT_RES_SCRIPTS_ALLOWED_LANGUAGE_TYPES:
             issues.append(SDKValidateIssue(
                 name=attr_dict.get("name"),
                 description=attr_dict.get("fail_msg").format(script.get("name", "UNKNOWN SCRIPT NAME")),
                 severity=attr_dict.get("fail_severity"),
                 solution=attr_dict.get("fail_solution")
             ))
 
     # do very similar check for local scripts in playbooks
-    for playbook in export_res.get("playbooks", []):
-        for local_script in playbook.get("local_scripts", []):
+    for playbook in export_res.get("playbooks") or []:
+        for local_script in playbook.get("local_scripts") or []:
             if local_script.get("language", "") not in constants.EXPORT_RES_SCRIPTS_ALLOWED_LANGUAGE_TYPES:
                 issues.append(SDKValidateIssue(
                     name=attr_dict.get("name"),
                     description=attr_dict.get("fail_msg_playbooks").format(
                         local_script.get("name", "UNKNOWN SCRIPT NAME"), playbook.get("display_name", "UNKNOWN PLAYBOOK NAME")),
                     severity=attr_dict.get("fail_severity"),
                     solution=attr_dict.get("fail_solution")
@@ -679,15 +679,15 @@
                 solution=attr_dict.get("fail_solution")
             ))
 
     # workflows are harder, but we can simply look into the XML for what we know should be there:
     # there should be a line in there that says "post_processing_script_language":"python3" for PY3
     # or "post_processing_script_language":"python" for Python 2 scripts (same goes for pre_processing...)
     # so we scan the workflows and their xml properties
-    for workflow in export_res.get("workflows", []):
+    for workflow in export_res.get("workflows") or []:
         # check for bad pre processing scripts
         if constants.EXPORT_RES_WORKFLOW_PRE_PROCESSING_UNALLOWED_LANGUAGE in workflow.get("content", {}).get("xml", ""):
             issues.append(SDKValidateIssue(
                 name=attr_dict.get("name"),
                 description=attr_dict.get("fail_msg_pre_processing").format(workflow.get("name", "UNKNOWN SCRIPT NAME")),
                 severity=attr_dict.get("fail_severity"),
                 solution=attr_dict.get("fail_solution")
@@ -797,15 +797,15 @@
     :rtype: list[SDKValidateIssue]
     """
 
     # render jinja file of LICENSE
     template_rendered = sdk_helpers.setup_env_and_render_jinja_file(
         constants.PACKAGE_TEMPLATE_PACKAGE_DIR,
         filename,
-        sdk_version=sdk_helpers.get_resilient_sdk_version()
+        license_content=constants.CODEGEN_DEFAULT_LICENSE_CONTENT
     )
 
     # read the contents of the package's LICENSE file
     file_contents = "".join(sdk_helpers.read_file(path_file))
 
     if template_rendered in file_contents:
         # the template is still in the file
```

### Comparing `resilient_sdk-48.0.4034/resilient_sdk/util/sdk_validate_issue.py` & `resilient_sdk-48.1.4243/resilient_sdk/util/sdk_validate_issue.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/resilient_sdk.egg-info/PKG-INFO` & `resilient_sdk-48.1.4243/resilient_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient-sdk
-Version: 48.0.4034
+Version: 48.1.4243
 Summary: Python SDK for developing Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-sdk
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
 Project-URL: Change Log, https://ibm.biz/resilient-sdk-changes
```

### Comparing `resilient_sdk-48.0.4034/resilient_sdk.egg-info/SOURCES.txt` & `resilient_sdk-48.1.4243/resilient_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 resilient_sdk/cmds/__init__.py
 resilient_sdk/cmds/base_cmd.py
 resilient_sdk/cmds/clone.py
 resilient_sdk/cmds/codegen.py
 resilient_sdk/cmds/dev.py
 resilient_sdk/cmds/docgen.py
 resilient_sdk/cmds/extract.py
+resilient_sdk/cmds/run_init.py
 resilient_sdk/cmds/validate.py
 resilient_sdk/cmds/ext/__init__.py
 resilient_sdk/cmds/ext/ext_package.py
 resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2
 resilient_sdk/data/codegen/templates/package_template/MANIFEST.in.jinja2
 resilient_sdk/data/codegen/templates/package_template/README.md.jinja2
 resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2
@@ -52,14 +53,15 @@
 resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/blank.json.jinja2
 resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_fail.json.jinja2
 resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_success.json.jinja2
 resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2
 resilient_sdk/data/docgen/templates/README.md.jinja2
 resilient_sdk/data/ext/icons/app_logo.png
 resilient_sdk/data/ext/icons/company_logo.png
+resilient_sdk/data/run_init/sdk_settings.json.jinja2
 resilient_sdk/data/validate/.pylintrc
 resilient_sdk/data/validate/templates/validate_report.md.jinja2
 resilient_sdk/util/__init__.py
 resilient_sdk/util/constants.py
 resilient_sdk/util/jinja2_filters.py
 resilient_sdk/util/package_file_helpers.py
 resilient_sdk/util/resilient_objects.py
@@ -173,14 +175,15 @@
 tests/unit/test_cmds/__init__.py
 tests/unit/test_cmds/test_base_cmd.py
 tests/unit/test_cmds/test_clone.py
 tests/unit/test_cmds/test_codegen.py
 tests/unit/test_cmds/test_dev.py
 tests/unit/test_cmds/test_docgen.py
 tests/unit/test_cmds/test_extract.py
+tests/unit/test_cmds/test_run_init.py
 tests/unit/test_cmds/test_validate.py
 tests/unit/test_cmds/ext/__init__.py
 tests/unit/test_cmds/ext/test_ext_package.py
 tests/unit/test_util/__init__.py
 tests/unit/test_util/test_jinja_filters.py
 tests/unit/test_util/test_package_file_helpers.py
 tests/unit/test_util/test_resilient_objects.py
```

### Comparing `resilient_sdk-48.0.4034/setup.cfg` & `resilient_sdk-48.1.4243/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient >= 48.0
+	resilient >= 48.1
 	
 	genson    ~= 1.2
 	
 	jinja2    ~= 3.0; python_version >= "3.6"
 	
 	jinja2    ~= 2.0; python_version == "2.7"
```

### Comparing `resilient_sdk-48.0.4034/tests/conftest.py` & `resilient_sdk-48.1.4243/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -381,14 +381,55 @@
 
     _add_to_cmd_line_args(args_to_add)
 
     yield
 
     sys.argv = original_cmd_line
 
+@pytest.fixture
+def fx_cmd_line_args_init():
+    """
+    Before: adds args_to_add to cmd line so can be accessed by ArgParsers
+    After: Set the cmd line args back to its original value
+    """
+    original_cmd_line = copy.deepcopy(sys.argv)
+
+    args_to_add = [
+        "init"
+    ]
+
+    _add_to_cmd_line_args(args_to_add)
+
+    yield
+
+    sys.argv = original_cmd_line
+
+@pytest.fixture
+def fx_mock_settings_file_path():
+    """
+    Before: Change the settings file path to point to the test temp directory
+    After: Change the settings file path back to the original value
+    """
+    old_sdk_settings_path = constants.SDK_SETTINGS_FILE_PATH
+    constants.SDK_SETTINGS_FILE_PATH = "{}/test_settings.json".format(mock_paths.TEST_TEMP_DIR)
+    
+    yield
+    
+    constants.SDK_SETTINGS_FILE_PATH = old_sdk_settings_path
+
+@pytest.fixture
+def fx_create_mock_settings_file():
+    """
+    Before: Create a temporary file with the default settings file name
+    """
+    fake_settings_json = "{}/test_settings.json".format(mock_paths.TEST_TEMP_DIR)
+    with open(fake_settings_json, "w") as f:
+        pass
+
+    yield
 
 @pytest.fixture
 def fx_cmd_line_args_docgen():
     """
     Before: adds args_to_add to cmd line so can be accessed by ArgParsers
     After: Set the cmd line args back to its original value
     """
```

### Comparing `resilient_sdk-48.0.4034/tests/helpers.py` & `resilient_sdk-48.1.4243/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/integration/test_installation.py` & `resilient_sdk-48.1.4243/tests/integration/test_installation.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/.mock_sdk_settings.json` & `resilient_sdk-48.1.4243/resilient_sdk/data/run_init/sdk_settings.json.jinja2`

 * *Files 18% similar despite different names*

```diff
@@ -10,37 +10,40 @@
 00000090: 5f73 6574 7469 6e67 7322 2c0a 2020 2020  _settings",.    
 000000a0: 2020 2020 2020 2020 2272 6573 696c 6965          "resilie
 000000b0: 6e74 5f68 6f73 7422 3a20 2265 7861 6d70  nt_host": "examp
 000000c0: 6c65 2e6f 7267 222c 0a20 2020 2020 2020  le.org",.       
 000000d0: 2020 2020 2022 7265 7369 6c69 656e 745f       "resilient_
 000000e0: 6f72 6722 3a20 2265 7861 6d70 6c65 206f  org": "example o
 000000f0: 7267 2066 726f 6d20 7365 7474 696e 6773  rg from settings
-00000100: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00000110: 6d22 3a20 226e 6f74 206c 6976 6574 6573  m": "not livetes
-00000120: 7422 0a20 2020 2020 2020 207d 2c0a 2020  t".        },.  
-00000130: 2020 2020 2020 2270 796c 696e 7422 3a20        "pylint": 
-00000140: 5b0a 2020 2020 2020 2020 2020 2020 222d  [.            "-
-00000150: 2d65 6e61 626c 653d 452c 4622 0a20 2020  -enable=E,F".   
-00000160: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00000170: 2262 616e 6469 7422 3a20 5b0a 2020 2020  "bandit": [.    
-00000180: 2020 2020 2020 2020 222d 6c6c 220a 2020          "-ll".  
-00000190: 2020 2020 2020 5d0a 2020 2020 7d2c 0a20        ].    },. 
-000001a0: 2020 2022 646f 6367 656e 223a 207b 0a20     "docgen": {. 
-000001b0: 2020 2020 2020 2022 7375 7070 6f72 7465         "supporte
-000001c0: 645f 6170 7022 3a20 7472 7565 0a20 2020  d_app": true.   
-000001d0: 207d 2c0a 2020 2020 2263 6f64 6567 656e   },.    "codegen
-000001e0: 223a 7b0a 2020 2020 2020 2020 2273 6574  ":{.        "set
-000001f0: 7570 223a 207b 0a20 2020 2020 2020 2020  up": {.         
-00000200: 2020 2022 6c69 6365 6e73 6522 3a20 224d     "license": "M
-00000210: 4954 222c 0a20 2020 2020 2020 2020 2020  IT",.           
-00000220: 2022 6175 7468 6f72 223a 2022 6175 7468   "author": "auth
-00000230: 6f72 206e 616d 6522 2c0a 2020 2020 2020  or name",.      
-00000240: 2020 2020 2020 2261 7574 686f 725f 656d        "author_em
-00000250: 6169 6c22 3a20 2279 6f75 4065 7861 6d70  ail": "you@examp
-00000260: 6c65 2e63 6f6d 222c 0a20 2020 2020 2020  le.com",.       
-00000270: 2020 2020 2022 7572 6c22 3a20 2265 7861       "url": "exa
-00000280: 6d70 6c65 2e63 6f6d 220a 2020 2020 2020  mple.com".      
-00000290: 2020 7d2c 0a20 2020 2020 2020 2022 6c69    },.        "li
-000002a0: 6365 6e73 655f 636f 6e74 656e 7422 3a20  cense_content": 
-000002b0: 2254 6869 7320 6973 2061 2074 6573 7420  "This is a test 
-000002c0: 6c69 6365 6e73 652e 220a 2020 2020 7d0a  license.".    }.
-000002d0: 7d                                       }
+00000100: 220a 2020 2020 2020 2020 7d2c 0a20 2020  ".        },.   
+00000110: 2020 2020 2022 7079 6c69 6e74 223a 205b       "pylint": [
+00000120: 0a20 2020 2020 2020 2020 2020 2022 2d2d  .            "--
+00000130: 656e 6162 6c65 3d45 2c46 220a 2020 2020  enable=E,F".    
+00000140: 2020 2020 5d2c 0a20 2020 2020 2020 2022      ],.        "
+00000150: 6261 6e64 6974 223a 205b 0a20 2020 2020  bandit": [.     
+00000160: 2020 2020 2020 2022 2d6c 6c22 0a20 2020         "-ll".   
+00000170: 2020 2020 205d 0a20 2020 207d 2c0a 2020       ].    },.  
+00000180: 2020 2264 6f63 6765 6e22 3a20 7b0a 2020    "docgen": {.  
+00000190: 2020 2020 2020 2273 7570 706f 7274 6564        "supported
+000001a0: 5f61 7070 223a 207b 7b20 7375 7070 6f72  _app": {{ suppor
+000001b0: 7465 645f 6170 7020 7d7d 0a20 2020 207d  ted_app }}.    }
+000001c0: 2c0a 2020 2020 2263 6f64 6567 656e 223a  ,.    "codegen":
+000001d0: 207b 0a20 2020 2020 2020 2022 7365 7475   {.        "setu
+000001e0: 7022 3a20 7b0a 2020 2020 2020 2020 2020  p": {.          
+000001f0: 2020 226c 6963 656e 7365 223a 2022 7b7b    "license": "{{
+00000200: 206c 6963 656e 7365 207d 7d22 2c0a 2020   license }}",.  
+00000210: 2020 2020 2020 2020 2020 2261 7574 686f            "autho
+00000220: 7222 3a20 227b 7b20 6175 7468 6f72 207d  r": "{{ author }
+00000230: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
+00000240: 2261 7574 686f 725f 656d 6169 6c22 3a20  "author_email": 
+00000250: 227b 7b20 6175 7468 6f72 5f65 6d61 696c  "{{ author_email
+00000260: 207d 7d22 2c0a 2020 2020 2020 2020 2020   }}",.          
+00000270: 2020 2275 726c 223a 2022 7b7b 2075 726c    "url": "{{ url
+00000280: 207d 7d22 2c0a 2020 2020 2020 2020 2020   }}",.          
+00000290: 2020 226c 6f6e 675f 6465 7363 7269 7074    "long_descript
+000002a0: 696f 6e22 3a20 227b 7b20 6c6f 6e67 5f64  ion": "{{ long_d
+000002b0: 6573 6372 6970 7469 6f6e 207d 7d22 0a20  escription }}". 
+000002c0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000002d0: 2020 226c 6963 656e 7365 5f63 6f6e 7465    "license_conte
+000002e0: 6e74 223a 2022 7b7b 206c 6963 656e 7365  nt": "{{ license
+000002f0: 5f63 6f6e 7465 6e74 207d 7d22 0a20 2020  _content }}".   
+00000300: 207d 0a7d 0a                              }.}.
```

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_app.log` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_app.log`

 * *Files 2% similar despite different names*

```diff
@@ -316,14 +316,15 @@
 2021-12-02 14:48:46,904 DEBUG [debugger] <task_done[*] ([<resilient_circuits.action_message.FunctionResult object at 0x10e72ae10>] )>
 2021-12-02 14:48:46,905 DEBUG [debugger] <task_success[*] (<task[*] (<function app_function.__call__.<locals>.app_function_decorator.<locals>._invoke_app_function at 0x10e959510>, <mock_function_one[functions.mock_function_one] (*** workflow=mock_workflow_one, user=admin@example.com) 2021-12-02 14:48:43.659000> mock_input_text_with_value_string={'format': 'text', 'content': 'data value one  ล ฦ ว ศ ษ ส ห ฬ อ'}, mock_input_text='abc  à¸¥ à¸¦ à¸§ à¸¨ à¸© à¸ª à¸« à¸¬ à¸\xad abc', mock_input_boolean=True, mock_input_multiselect=[{'*** 'name': 'value one'}, {'*** 'name': 'value two'}], mock_input_select={'*** 'name': 'select two'}, mock_input_number=1630407352685)>, [<resilient_circuits.action_message.FunctionResult object at 0x10e72ae10>] )>
 2021-12-02 14:48:47,116 DEBUG [debugger] <mock_function_one_success[functions.mock_function_one] (<mock_function_one[functions.mock_function_one] (id=3, workflow=mock_workflow_one, user=admin@example.com) 2021-12-02 14:48:43.659000>, [<resilient_circuits.action_message.FunctionResult object at 0x10e72ae10>] )>
 2021-12-02 14:48:47,117 DEBUG [actions_component] success! [<resilient_circuits.action_message.FunctionResult object at 0x10e72ae10>], <mock_function_one[functions.mock_function_one] (id=3, workflow=mock_workflow_one, user=admin@example.com) 2021-12-02 14:48:43.659000>
 2021-12-02 14:48:47,118 DEBUG [actions_component] Message: Completed
 2021-12-02 14:48:47,120 DEBUG [actions_component] Ack ID:xxx.xxx.xxx-35545-1634461020363-3:2:2287:1:1
 2021-12-02 14:48:47,121 DEBUG [actions_component] [mock_function_one] Result: {'version': 2.1, 'success': True, 'reason': None, 'content': {'mock_key': 'Mock Value!'}, 'raw': None, 'inputs': {'mock_input_text_with_value_string': 'data value one  ล ฦ ว ศ ษ ส ห ฬ อ', 'mock_input_text': 'abc  à¸¥ à¸¦ à¸§ à¸¨ à¸© à¸ª à¸« à¸¬ à¸\xad abc', 'mock_input_boolean': True, 'mock_input_multiselect': ['value one', 'value two'], 'mock_input_select': 'select two', 'mock_input_number': 1630407352685}, 'metrics': {'version': '1.0', 'package': 'fn-main-mock-integration', 'package_version': '1.0.3', 'host': 'xxxs-MacBook-Pro-2.local', 'execution_time_ms': 3233, 'timestamp': '2021-12-02 14:48:45'}}
+2021-12-02 14:48:47,121 DEBUG [actions_component] [mock_function_one_but_really_really_really_really_really_really_really_really_long] Result: {'version': 2.1, 'success': True, 'reason': None, 'content': {'mock_key': 'Mock Value!'}, 'raw': None, 'inputs': {'mock_input_text_with_value_string': 'data value one  ล ฦ ว ศ ษ ส ห ฬ อ', 'mock_input_text': 'abc  à¸¥ à¸¦ à¸§ à¸¨ à¸© à¸ª à¸« à¸¬ à¸\xad abc', 'mock_input_boolean': True, 'mock_input_multiselect': ['value one', 'value two'], 'mock_input_select': 'select two', 'mock_input_number': 1630407352685}, 'metrics': {'version': '1.0', 'package': 'fn-main-mock-integration', 'package_version': '1.0.3', 'host': 'xxxs-MacBook-Pro-2.local', 'execution_time_ms': 3233, 'timestamp': '2021-12-02 14:48:45'}}
 2021-12-02 14:48:47,123 DEBUG [debugger] <Ack[*] ()>
 2021-12-02 14:48:47,125 DEBUG [stomp_component] ack_frame()
 2021-12-02 14:48:47,127 DEBUG [client] Sending ACK frame [headers={'*** version=1.2]
 2021-12-02 14:48:47,129 DEBUG [stomp_component] Ack Sent
 2021-12-02 14:48:47,130 DEBUG [debugger] <Send[*] ()>
 2021-12-02 14:48:47,131 DEBUG [stomp_component] send()
 2021-12-02 14:48:47,132 DEBUG [client] Sending SEND frame [headers={'correlation-*** 'destination': '/queue/acks.201.fn_main_mock_integration'}, body=b'{\n  "message_type": ...', version=1.2]
```

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_export.res` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_export.resz` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_export.resz`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_export_corrupt.res` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_export_corrupt.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/config.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/config.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/customize.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/customize.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/customize_old.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/customize_old.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/setup.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/setup.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/setup_callable_data.txt` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/setup_callable_data.txt`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_package_files/setup_py_lines.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_package_files/setup_py_lines.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_paths.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_paths.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_reload_export.res` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_reload_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/mock_xml_test_report.xml` & `resilient_sdk-48.1.4243/tests/shared_mock_data/mock_xml_test_report.xml`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON` & `resilient_sdk-48.1.4243/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/resilient_api_data/export.JSON` & `resilient_sdk-48.1.4243/tests/shared_mock_data/resilient_api_data/export.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/resilient_api_data/orgs.JSON` & `resilient_sdk-48.1.4243/tests/shared_mock_data/resilient_api_data/orgs.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/resilient_api_data/session.JSON` & `resilient_sdk-48.1.4243/tests/shared_mock_data/resilient_api_data/session.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/shared_mock_data/resilient_api_mock.py` & `resilient_sdk-48.1.4243/tests/shared_mock_data/resilient_api_mock.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_app.py` & `resilient_sdk-48.1.4243/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_cmds/ext/test_ext_package.py` & `resilient_sdk-48.1.4243/tests/unit/test_cmds/ext/test_ext_package.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_cmds/test_base_cmd.py` & `resilient_sdk-48.1.4243/tests/unit/test_cmds/test_base_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_cmds/test_clone.py` & `resilient_sdk-48.1.4243/tests/unit/test_cmds/test_clone.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_cmds/test_codegen.py` & `resilient_sdk-48.1.4243/tests/unit/test_cmds/test_codegen.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,15 @@
         cmd_codegen.execute_command(args)
 
         setup_py = sdk_helpers.read_file(os.path.join(mock_paths.TEST_TEMP_DIR, mock_paths.MOCK_INT_FN_MAIN_MOCK_INTEGRATION_NAME, "setup.py"))
         assert '    license="MIT",\n' in setup_py
         assert '    author="author name",\n' in setup_py
         assert '    author_email="you@example.com",\n' in setup_py
         assert '    url="example.com",\n' in setup_py
+        assert '    long_description="""<<CHANGE ME>> this is an example long description""",\n' in setup_py
 
         license = sdk_helpers.read_file(os.path.join(mock_paths.TEST_TEMP_DIR, mock_paths.MOCK_INT_FN_MAIN_MOCK_INTEGRATION_NAME,
                         mock_paths.MOCK_INT_FN_MAIN_MOCK_INTEGRATION_NAME, "LICENSE"))
         assert 'This is a test license.' in license
 
 
 def test_merge_codegen_params():
```

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_cmds/test_dev.py` & `resilient_sdk-48.1.4243/tests/unit/test_cmds/test_dev.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_cmds/test_docgen.py` & `resilient_sdk-48.1.4243/tests/unit/test_cmds/test_docgen.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_cmds/test_extract.py` & `resilient_sdk-48.1.4243/tests/unit/test_cmds/test_extract.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_cmds/test_validate.py` & `resilient_sdk-48.1.4243/tests/unit/test_cmds/test_validate.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_util/test_jinja_filters.py` & `resilient_sdk-48.1.4243/tests/unit/test_util/test_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_util/test_package_file_helpers.py` & `resilient_sdk-48.1.4243/tests/unit/test_util/test_package_file_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_util/test_resilient_objects.py` & `resilient_sdk-48.1.4243/tests/unit/test_util/test_resilient_objects.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_util/test_sdk_exception.py` & `resilient_sdk-48.1.4243/tests/unit/test_util/test_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_util/test_sdk_helpers.py` & `resilient_sdk-48.1.4243/tests/unit/test_util/test_sdk_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -632,14 +632,26 @@
     assert isinstance(mock_function_one_results, dict)
 
     # There are two Results for mock_function_one
     # in the mock_app.log file, so this ensures we get the latest
     assert mock_function_one_results.get("version") == 2.1
     assert mock_function_one_results.get("reason") == None
 
+def test_scrape_results_really_long_function_name():
+
+    results_scraped = sdk_helpers.scrape_results_from_log_file(mock_paths.MOCK_APP_LOG_PATH)
+    mock_function_one_results = results_scraped.get("mock_function_one_but_really_really_really_really_really_really_really_really_long")
+
+    assert isinstance(mock_function_one_results, dict)
+
+    # There are two Results for mock_function_one
+    # in the mock_app.log file, so this ensures we get the latest
+    assert mock_function_one_results.get("version") == 2.1
+    assert mock_function_one_results.get("reason") == None
+
 
 def test_scrape_results_from_log_file_not_found():
     with pytest.raises(SDKException, match=constants.ERROR_NOT_FIND_FILE):
         sdk_helpers.scrape_results_from_log_file("mock_path_non_existent")
 
 
 def test_handle_file_not_found_error(caplog):
```

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_util/test_sdk_validate_configs.py` & `resilient_sdk-48.1.4243/tests/unit/test_util/test_sdk_validate_configs.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_util/test_sdk_validate_helpers.py` & `resilient_sdk-48.1.4243/tests/unit/test_util/test_sdk_validate_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,15 +549,21 @@
         assert result.severity == SDKValidateIssue.SEVERITY_LEVEL_CRITICAL
         assert u"Pre-processing script for workflow 'Shouldnt Pass Δ, Й, ק ,م, ๗, あ, 叶' packaged with this app is written in Python 2" in result.description
         result = results[3]
         assert isinstance(result, SDKValidateIssue)
         assert result.severity == SDKValidateIssue.SEVERITY_LEVEL_CRITICAL
         assert u"Post-processing script for workflow 'Shouldnt Pass Δ, Й, ק ,م, ๗, あ, 叶' packaged with this app is written in Python 2" in result.description
 
-def test_package_files_validate_python_versions_in_scripts_pass(fx_copy_fn_main_mock_integration, fx_get_package_files_config):
+@pytest.mark.parametrize("playbook_input", [
+    [{"display_name": "My PB", "local_scripts":
+       [{"language": "python3", "name": u"Should Pass Δ, Й, ק ,م, ๗, あ, 叶",}]}],
+    [], # ensure empty playbook list works
+    None # ensure None playbook object works
+])
+def test_package_files_validate_python_versions_in_scripts_pass(playbook_input, fx_copy_fn_main_mock_integration, fx_get_package_files_config):
     """add scripts everywhere they could be found, but make them all pass as py3 scripts"""
 
     filename = "export.res"
     i = fx_get_package_files_config[filename]
     attr_dict = sdk_validate_configs.package_files[i][1]
     path_file = os.path.join(fx_copy_fn_main_mock_integration[1], attr_dict.get("path").format(fx_copy_fn_main_mock_integration[0]))
 
@@ -570,18 +576,15 @@
                 "name": u"Should Pass Δ, Й, ק ,م, ๗, あ, 叶"
             },], 
             "workflows": [{
                 "name": u"Should Pass Δ, Й, ק ,م, ๗, あ, 叶",
                 "content": {"xml":
                     "\u003c?xml version=\"1.0\" encoding=\"UTF-8\"?\u003e\u003c{\"multiselect_value\":[\"8b8b22d4-b20c-4d10-abac-a65211a5b9cd\",\"bf8e34a8-79aa-4ec4-b4c9-b8f1f0f7135e\"]}}},\"post_processing_script\":\"# post process of mock  \u0e25 \u0e26 \u0e27 \u0e28 \u0e29 \u0e2a \u0e2b \u0e2c \u0e2d workflow two\\n\\nincident.addNote(u\\\" \u0e25 \u0e26 \u0e27 \u0e28 \u0e29 \u0e2a \u0e2b \u0e2c \u0e2d\\\")\",\"post_processing_script_language\":\"python3\",\"pre_processing_script\":\"# A mock pre-process script for mock_workflow_one\\n\\ninputs.mock_input_number = 123\\ninputs.mock_input_boolean = True\\ninputs.mock_input_text = \\\"abc  \u0e25 \u0e26 \u0e27 \u0e28 \u0e29 \u0e2a \u0e2b \u0e2c \u0e2d abc\\\"\",\"pre_processing_script_language\":\"python3\",\"result_name\":\"output_of_mock_function_one\"}\u003c/resilient:function\u003e\u003c/"
             }}],
-            "playbooks": [{"display_name": "My PB", "local_scripts": [{
-                "language": "python3",
-                "name": u"Should Pass Δ, Й, ק ,م, ๗, あ, 叶",
-            }]}]
+            "playbooks": playbook_input
         }
 
         results = sdk_validate_helpers.package_files_validate_script_python_versions(path_file, attr_dict)
 
         assert len(results) == 1
         result = results[0]
         assert isinstance(result, SDKValidateIssue)
@@ -667,17 +670,17 @@
 def test_package_files_validate_license_is_not_default(fx_copy_fn_main_mock_integration,fx_get_package_files_config):
 
     filename = "LICENSE"
     i = fx_get_package_files_config[filename]
     attr_dict = sdk_validate_configs.package_files[i][1]
     path_file = os.path.join(fx_copy_fn_main_mock_integration[1], attr_dict.get("path").format(fx_copy_fn_main_mock_integration[0]))
 
-    with patch("resilient_sdk.util.sdk_validate_helpers.sdk_helpers.setup_env_and_render_jinja_file") as mock_jinja_render:
+    with patch("resilient_sdk.util.sdk_validate_helpers.sdk_helpers.read_file") as mock_read_file:
 
-        mock_jinja_render.return_value = "A sample LICENSE\n\nThis should still be validated manually to ensure proper license type"
+        mock_read_file.return_value = "A sample LICENSE\n\nThis should still be validated manually to ensure proper license type"
 
         result = sdk_validate_helpers.package_files_validate_license(path_file, attr_dict, filename)
 
     assert len(result) == 2
     assert isinstance(result[0], SDKValidateIssue)
     assert result[0].severity == SDKValidateIssue.SEVERITY_LEVEL_INFO
     assert "'LICENSE' file is valid" == result[0].description
@@ -780,15 +783,15 @@
     with patch("resilient_sdk.util.sdk_validate_helpers.sdk_helpers.run_subprocess") as mock_tox_sub_process:
 
         mock_tox_sub_process.return_value = (None, "bad run")
 
         result = sdk_validate_helpers.tox_tests_run_tox_tests(path_package, attr_dict, args, None)
 
         assert "Using mock args" in caplog.text
-        assert "'-m', '\"not livetest\"'" in caplog.text
+        assert "'-m', 'not livetest'" in caplog.text
         assert "Something went wrong..." in result[1].description
         assert "bad run" in result[1].description
         assert result[0] == 0
 
 def test_tox_tests_run_tox_tests_with_pytest_args(fx_copy_fn_main_mock_integration, caplog):
 
     path_package = fx_copy_fn_main_mock_integration[1]
```

### Comparing `resilient_sdk-48.0.4034/tests/unit/test_util/test_sdk_validate_issue.py` & `resilient_sdk-48.1.4243/tests/unit/test_util/test_sdk_validate_issue.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.0.4034/tox.ini` & `resilient_sdk-48.1.4243/tox.ini`

 * *Files identical despite different names*

