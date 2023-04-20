# Comparing `tmp/tabpy-2.6.0.tar.gz` & `tmp/tabpy-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/dleskosky/Documents/Repos/TabPy/dist/.tmp-_25w9uit/tabpy-2.6.0.tar", last modified: Mon Jan 30 22:54:55 2023, max compression
+gzip compressed data, was "tabpy-2.7.0.tar", last modified: Thu Apr 20 19:39:01 2023, max compression
```

## Comparing `tabpy-2.6.0.tar` & `tabpy-2.7.0.tar`

### file list

```diff
@@ -1,145 +1,149 @@
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.885362 tabpy-2.6.0/
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     4875 2023-01-30 22:53:44.000000 tabpy-2.6.0/CHANGELOG
--rw-r--r--   0 dleskosky   (503) staff       (20)     1078 2023-01-30 22:41:27.000000 tabpy-2.6.0/LICENSE
--rwxr-xr-x   0 dleskosky   (503) staff       (20)      549 2023-01-30 22:41:27.000000 tabpy-2.6.0/MANIFEST.in
--rw-r--r--   0 dleskosky   (503) staff       (20)     6390 2023-01-30 22:54:55.885622 tabpy-2.6.0/PKG-INFO
--rw-r--r--   0 dleskosky   (503) staff       (20)      131 2023-01-30 22:41:27.000000 tabpy-2.6.0/Procfile
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     3280 2023-01-30 22:41:27.000000 tabpy-2.6.0/README.md
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.765412 tabpy-2.6.0/docs/
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     7524 2023-01-30 22:41:27.000000 tabpy-2.6.0/docs/TableauConfiguration.md
--rwxr-xr-x   0 dleskosky   (503) staff       (20)      869 2023-01-30 22:41:27.000000 tabpy-2.6.0/docs/about.md
--rw-r--r--   0 dleskosky   (503) staff       (20)      413 2023-01-30 22:41:27.000000 tabpy-2.6.0/docs/deploy-to-heroku.md
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.767142 tabpy-2.6.0/docs/img/
--rwxr-xr-x   0 dleskosky   (503) staff       (20)   136889 2023-01-30 22:41:27.000000 tabpy-2.6.0/docs/img/Example1-SimpleFunctionCall.png
--rwxr-xr-x   0 dleskosky   (503) staff       (20)   188230 2023-01-30 22:41:27.000000 tabpy-2.6.0/docs/img/Example2-MultipleFunctionCalls.png
--rwxr-xr-x   0 dleskosky   (503) staff       (20)    43399 2023-01-30 22:41:27.000000 tabpy-2.6.0/docs/img/python-calculated-field.png
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     1206 2023-01-30 22:41:27.000000 tabpy-2.6.0/docs/security.md
--rwxr-xr-x   0 dleskosky   (503) staff       (20)    11228 2023-01-30 22:41:27.000000 tabpy-2.6.0/docs/server-config.md
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     1357 2023-01-30 22:41:27.000000 tabpy-2.6.0/docs/server-install.md
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     4089 2023-01-30 22:41:27.000000 tabpy-2.6.0/docs/server-rest.md
--rwxr-xr-x   0 dleskosky   (503) staff       (20)    16573 2023-01-30 22:41:27.000000 tabpy-2.6.0/docs/tabpy-tools.md
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     2174 2023-01-30 22:41:27.000000 tabpy-2.6.0/docs/tabpy-virtualenv.md
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.768719 tabpy-2.6.0/misc/
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     3567 2023-01-30 22:41:27.000000 tabpy-2.6.0/misc/TabPy.postman_collection.json
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     7855 2023-01-30 22:41:27.000000 tabpy-2.6.0/misc/TabPy.yml
--rw-r--r--   0 dleskosky   (503) staff       (20)       88 2023-01-30 22:41:27.000000 tabpy-2.6.0/requirements.txt
--rwxr-xr-x   0 dleskosky   (503) staff       (20)        6 2023-01-30 22:41:27.000000 tabpy-2.6.0/requirements_dev.txt
--rw-r--r--   0 dleskosky   (503) staff       (20)      308 2023-01-30 22:54:55.886834 tabpy-2.6.0/setup.cfg
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     3577 2023-01-30 22:41:27.000000 tabpy-2.6.0/setup.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.770573 tabpy-2.6.0/tabpy/
--rwxr-xr-x   0 dleskosky   (503) staff       (20)        6 2023-01-30 22:54:04.000000 tabpy-2.6.0/tabpy/VERSION
--rwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/__init__.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.776269 tabpy-2.6.0/tabpy/models/
--rwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/models/__init__.py
--rw-r--r--   0 dleskosky   (503) staff       (20)      794 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/models/deploy_models.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.780146 tabpy-2.6.0/tabpy/models/scripts/
--rw-r--r--   0 dleskosky   (503) staff       (20)      693 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/models/scripts/ANOVA.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     2198 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/models/scripts/PCA.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     1424 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/models/scripts/SentimentAnalysis.py
--rwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/models/scripts/__init__.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     1377 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/models/scripts/tTest.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.781675 tabpy-2.6.0/tabpy/models/utils/
--rw-r--r--   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/models/utils/__init__.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     1731 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/models/utils/setup_utils.py
--rwxr-xr-x   0 dleskosky   (503) staff       (20)      841 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.783562 tabpy-2.6.0/tabpy/tabpy_server/
--rw-r--r--   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/__init__.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.787465 tabpy-2.6.0/tabpy/tabpy_server/app/
--rw-r--r--   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/app/__init__.py
--rw-r--r--   0 dleskosky   (503) staff       (20)    17069 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/app/app.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     1313 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/app/app_parameters.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     2635 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/app/util.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.792936 tabpy-2.6.0/tabpy/tabpy_server/common/
--rw-r--r--   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/common/__init__.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     1916 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/common/default.conf
--rw-r--r--   0 dleskosky   (503) staff       (20)     2916 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/common/endpoint_file_mgr.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     3656 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/common/messages.py
--rw-r--r--   0 dleskosky   (503) staff       (20)      104 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/common/util.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.804707 tabpy-2.6.0/tabpy/tabpy_server/handlers/
--rw-r--r--   0 dleskosky   (503) staff       (20)      803 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/handlers/__init__.py
--rw-r--r--   0 dleskosky   (503) staff       (20)    15107 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/handlers/base_handler.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     4926 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/handlers/endpoint_handler.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     2522 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/handlers/endpoints_handler.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     5906 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/handlers/evaluation_plane_handler.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     5690 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/handlers/management_handler.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     8060 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/handlers/query_plane_handler.py
--rw-r--r--   0 dleskosky   (503) staff       (20)      975 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/handlers/service_info_handler.py
--rw-r--r--   0 dleskosky   (503) staff       (20)      892 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/handlers/status_handler.py
--rw-r--r--   0 dleskosky   (503) staff       (20)      700 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/handlers/upload_destination_handler.py
--rw-r--r--   0 dleskosky   (503) staff       (20)      967 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/handlers/util.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.807936 tabpy-2.6.0/tabpy/tabpy_server/management/
--rw-r--r--   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/management/__init__.py
--rw-r--r--   0 dleskosky   (503) staff       (20)    20688 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/management/state.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     1479 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/management/util.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.810923 tabpy-2.6.0/tabpy/tabpy_server/psws/
--rw-r--r--   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/psws/__init__.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     7159 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/psws/callbacks.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     9457 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/psws/python_service.py
--rw-r--r--   0 dleskosky   (503) staff       (20)      254 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/state.ini.template
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.814061 tabpy-2.6.0/tabpy/tabpy_server/static/
--rw-r--r--   0 dleskosky   (503) staff       (20)     1768 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/static/TabPy_logo.png
--rw-r--r--   0 dleskosky   (503) staff       (20)     1548 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/static/index.html
--rw-r--r--   0 dleskosky   (503) staff       (20)    33575 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_server/static/tableau.png
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.822098 tabpy-2.6.0/tabpy/tabpy_tools/
--rw-r--r--   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_tools/__init__.py
--rw-r--r--   0 dleskosky   (503) staff       (20)    11782 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_tools/client.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     2346 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_tools/custom_query_object.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     2944 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_tools/query_object.py
--rw-r--r--   0 dleskosky   (503) staff       (20)    13098 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_tools/rest.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     7031 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_tools/rest_client.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     4133 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/tabpy_tools/schema.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.823787 tabpy-2.6.0/tabpy/utils/
--rwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/utils/__init__.py
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     4394 2023-01-30 22:41:27.000000 tabpy-2.6.0/tabpy/utils/tabpy_user.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.774843 tabpy-2.6.0/tabpy.egg-info/
--rw-r--r--   0 dleskosky   (503) staff       (20)     6390 2023-01-30 22:54:55.000000 tabpy-2.6.0/tabpy.egg-info/PKG-INFO
--rw-r--r--   0 dleskosky   (503) staff       (20)     4218 2023-01-30 22:54:55.000000 tabpy-2.6.0/tabpy.egg-info/SOURCES.txt
--rw-r--r--   0 dleskosky   (503) staff       (20)        1 2023-01-30 22:54:55.000000 tabpy-2.6.0/tabpy.egg-info/dependency_links.txt
--rw-r--r--   0 dleskosky   (503) staff       (20)      138 2023-01-30 22:54:55.000000 tabpy-2.6.0/tabpy.egg-info/entry_points.txt
--rw-r--r--   0 dleskosky   (503) staff       (20)      210 2023-01-30 22:54:55.000000 tabpy-2.6.0/tabpy.egg-info/requires.txt
--rw-r--r--   0 dleskosky   (503) staff       (20)       12 2023-01-30 22:54:55.000000 tabpy-2.6.0/tabpy.egg-info/top_level.txt
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.824658 tabpy-2.6.0/tests/
--rw-r--r--   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/__init__.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.839434 tabpy-2.6.0/tests/integration/
--rw-r--r--   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/__init__.py
--rwxr-xr-x   0 dleskosky   (503) staff       (20)    10362 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/integ_test_base.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.846794 tabpy-2.6.0/tests/integration/resources/
--rw-r--r--   0 dleskosky   (503) staff       (20)     1375 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/resources/2019_04_24_to_3018_08_25.crt
--rw-r--r--   0 dleskosky   (503) staff       (20)     1679 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/resources/2019_04_24_to_3018_08_25.key
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     1512 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/resources/deploy_and_evaluate_model.conf
--rw-r--r--   0 dleskosky   (503) staff       (20)     1525 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/resources/deploy_and_evaluate_model_auth.conf
--rwxr-xr-x   0 dleskosky   (503) staff       (20)      136 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/resources/pwdfile.txt
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     2461 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/test_auth.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     1223 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/test_custom_evaluate_timeout.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     1038 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/test_deploy_and_evaluate_model.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     1233 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/test_deploy_and_evaluate_model_auth_on.py
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     1463 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/test_deploy_and_evaluate_model_ssl.py
--rw-r--r--   0 dleskosky   (503) staff       (20)      716 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/test_deploy_model_ssl_off_auth_off.py
--rw-r--r--   0 dleskosky   (503) staff       (20)      924 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/test_deploy_model_ssl_off_auth_on.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     1082 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/test_deploy_model_ssl_on_auth_off.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     2965 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/test_deploy_model_ssl_on_auth_on.py
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     3295 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/test_evaluate.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     3275 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/test_gzip.py
--rwxr-xr-x   0 dleskosky   (503) staff       (20)      725 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/test_url.py
--rwxr-xr-x   0 dleskosky   (503) staff       (20)      986 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/integration/test_url_ssl.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.848911 tabpy-2.6.0/tests/unit/
--rw-r--r--   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/__init__.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.869712 tabpy-2.6.0/tests/unit/server_tests/
--rw-r--r--   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/server_tests/__init__.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.878221 tabpy-2.6.0/tests/unit/server_tests/resources/
--rwxr-xr-x   0 dleskosky   (503) staff       (20)      745 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/server_tests/resources/expired.crt
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     4258 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/server_tests/resources/future.crt
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     1387 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/server_tests/resources/valid.crt
--rw-r--r--   0 dleskosky   (503) staff       (20)    13347 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/server_tests/test_config.py
--rw-r--r--   0 dleskosky   (503) staff       (20)      473 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/server_tests/test_endpoint_file_manager.py
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     5347 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/server_tests/test_endpoint_handler.py
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     4729 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/server_tests/test_endpoints_handler.py
--rwxr-xr-x   0 dleskosky   (503) staff       (20)    16279 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/server_tests/test_evaluation_plane_handler.py
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     5711 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/server_tests/test_pwd_file.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     5330 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/server_tests/test_service_info_handler.py
-drwxr-xr-x   0 dleskosky   (503) staff       (20)        0 2023-01-30 22:54:55.884495 tabpy-2.6.0/tests/unit/tools_tests/
--rw-r--r--   0 dleskosky   (503) staff       (20)       96 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/tools_tests/__init__.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     3170 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/tools_tests/test_client.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     7431 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/tools_tests/test_rest.py
--rw-r--r--   0 dleskosky   (503) staff       (20)     1896 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/tools_tests/test_rest_object.py
--rwxr-xr-x   0 dleskosky   (503) staff       (20)     1049 2023-01-30 22:41:27.000000 tabpy-2.6.0/tests/unit/tools_tests/test_schema.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.581994 tabpy-2.7.0/
+-rw-rw-rw-   0        0        0     5217 2023-04-20 19:29:50.000000 tabpy-2.7.0/CHANGELOG
+-rw-rw-rw-   0        0        0     1099 2023-02-17 14:44:24.000000 tabpy-2.7.0/LICENSE
+-rw-rw-rw-   0        0        0      549 2023-02-17 14:44:24.000000 tabpy-2.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6773 2023-04-20 19:39:01.582994 tabpy-2.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2023-02-17 14:44:24.000000 tabpy-2.7.0/Procfile
+-rw-rw-rw-   0        0        0     3334 2023-02-17 14:44:24.000000 tabpy-2.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.283341 tabpy-2.7.0/docs/
+-rw-rw-rw-   0        0        0     7688 2023-02-17 14:44:24.000000 tabpy-2.7.0/docs/TableauConfiguration.md
+-rw-rw-rw-   0        0        0      887 2023-02-17 14:44:24.000000 tabpy-2.7.0/docs/about.md
+-rw-rw-rw-   0        0        0      426 2023-02-17 14:44:24.000000 tabpy-2.7.0/docs/deploy-to-heroku.md
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.293338 tabpy-2.7.0/docs/img/
+-rw-rw-rw-   0        0        0   136889 2023-02-17 14:44:24.000000 tabpy-2.7.0/docs/img/Example1-SimpleFunctionCall.png
+-rw-rw-rw-   0        0        0   188230 2023-02-17 14:44:24.000000 tabpy-2.7.0/docs/img/Example2-MultipleFunctionCalls.png
+-rw-rw-rw-   0        0        0    43399 2023-02-17 14:44:24.000000 tabpy-2.7.0/docs/img/python-calculated-field.png
+-rw-rw-rw-   0        0        0     1229 2023-02-17 14:44:24.000000 tabpy-2.7.0/docs/security.md
+-rw-rw-rw-   0        0        0    13360 2023-04-20 19:20:47.000000 tabpy-2.7.0/docs/server-config.md
+-rw-rw-rw-   0        0        0     1422 2023-02-17 14:44:24.000000 tabpy-2.7.0/docs/server-install.md
+-rw-rw-rw-   0        0        0     4268 2023-02-17 14:44:24.000000 tabpy-2.7.0/docs/server-rest.md
+-rw-rw-rw-   0        0        0    17022 2023-02-17 14:44:24.000000 tabpy-2.7.0/docs/tabpy-tools.md
+-rw-rw-rw-   0        0        0     2174 2023-02-17 14:44:24.000000 tabpy-2.7.0/docs/tabpy-virtualenv.md
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.299340 tabpy-2.7.0/misc/
+-rw-rw-rw-   0        0        0     3747 2023-02-17 14:44:24.000000 tabpy-2.7.0/misc/TabPy.postman_collection.json
+-rw-rw-rw-   0        0        0     7855 2023-02-17 14:44:24.000000 tabpy-2.7.0/misc/TabPy.yml
+-rw-rw-rw-   0        0        0       90 2023-02-17 14:44:24.000000 tabpy-2.7.0/requirements.txt
+-rw-rw-rw-   0        0        0        6 2023-02-17 14:44:24.000000 tabpy-2.7.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0      337 2023-04-20 19:39:01.584994 tabpy-2.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     3708 2023-04-20 19:20:47.000000 tabpy-2.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.306337 tabpy-2.7.0/tabpy/
+-rw-rw-rw-   0        0        0        7 2023-04-20 19:29:50.000000 tabpy-2.7.0/tabpy/VERSION
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.326342 tabpy-2.7.0/tabpy/models/
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/models/__init__.py
+-rw-rw-rw-   0        0        0      820 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/models/deploy_models.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.339339 tabpy-2.7.0/tabpy/models/scripts/
+-rw-rw-rw-   0        0        0      715 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/models/scripts/ANOVA.py
+-rw-rw-rw-   0        0        0     2258 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/models/scripts/PCA.py
+-rw-rw-rw-   0        0        0     1476 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/models/scripts/SentimentAnalysis.py
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/models/scripts/__init__.py
+-rw-rw-rw-   0        0        0     1416 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/models/scripts/tTest.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.344339 tabpy-2.7.0/tabpy/models/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/models/utils/__init__.py
+-rw-rw-rw-   0        0        0     1789 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/models/utils/setup_utils.py
+-rw-rw-rw-   0        0        0      889 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.349338 tabpy-2.7.0/tabpy/tabpy_server/
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.363338 tabpy-2.7.0/tabpy/tabpy_server/app/
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/app/__init__.py
+-rw-rw-rw-   0        0        0    20045 2023-04-20 19:20:47.000000 tabpy-2.7.0/tabpy/tabpy_server/app/app.py
+-rw-rw-rw-   0        0        0     1560 2023-04-20 19:20:47.000000 tabpy-2.7.0/tabpy/tabpy_server/app/app_parameters.py
+-rw-rw-rw-   0        0        0     5396 2023-04-20 19:20:47.000000 tabpy-2.7.0/tabpy/tabpy_server/app/arrow_server.py
+-rw-rw-rw-   0        0        0     2723 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/app/util.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.377338 tabpy-2.7.0/tabpy/tabpy_server/common/
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/common/__init__.py
+-rw-rw-rw-   0        0        0     1985 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/common/default.conf
+-rw-rw-rw-   0        0        0     3010 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/common/endpoint_file_mgr.py
+-rw-rw-rw-   0        0        0     3828 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/common/messages.py
+-rw-rw-rw-   0        0        0      107 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/common/util.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.414355 tabpy-2.7.0/tabpy/tabpy_server/handlers/
+-rw-rw-rw-   0        0        0     1014 2023-04-20 19:20:47.000000 tabpy-2.7.0/tabpy/tabpy_server/handlers/__init__.py
+-rw-rw-rw-   0        0        0    15551 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/handlers/base_handler.py
+-rw-rw-rw-   0        0        0     1735 2023-04-20 19:20:47.000000 tabpy-2.7.0/tabpy/tabpy_server/handlers/basic_auth_server_middleware_factory.py
+-rw-rw-rw-   0        0        0     5068 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/handlers/endpoint_handler.py
+-rw-rw-rw-   0        0        0     2598 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/handlers/endpoints_handler.py
+-rw-rw-rw-   0        0        0     8200 2023-04-20 19:20:47.000000 tabpy-2.7.0/tabpy/tabpy_server/handlers/evaluation_plane_handler.py
+-rw-rw-rw-   0        0        0     5840 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/handlers/management_handler.py
+-rw-rw-rw-   0        0        0      211 2023-04-20 19:20:47.000000 tabpy-2.7.0/tabpy/tabpy_server/handlers/no_op_auth_handler.py
+-rw-rw-rw-   0        0        0     8294 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/handlers/query_plane_handler.py
+-rw-rw-rw-   0        0        0      998 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/handlers/service_info_handler.py
+-rw-rw-rw-   0        0        0      921 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/handlers/status_handler.py
+-rw-rw-rw-   0        0        0      721 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/handlers/upload_destination_handler.py
+-rw-rw-rw-   0        0        0     1005 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/handlers/util.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.424338 tabpy-2.7.0/tabpy/tabpy_server/management/
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/management/__init__.py
+-rw-rw-rw-   0        0        0    21331 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/management/state.py
+-rw-rw-rw-   0        0        0     1524 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/management/util.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.432337 tabpy-2.7.0/tabpy/tabpy_server/psws/
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/psws/__init__.py
+-rw-rw-rw-   0        0        0     7364 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/psws/callbacks.py
+-rw-rw-rw-   0        0        0     9732 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/psws/python_service.py
+-rw-rw-rw-   0        0        0      269 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/state.ini.template
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.440339 tabpy-2.7.0/tabpy/tabpy_server/static/
+-rw-rw-rw-   0        0        0     1768 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/static/TabPy_logo.png
+-rw-rw-rw-   0        0        0     1619 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/static/index.html
+-rw-rw-rw-   0        0        0    33575 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_server/static/tableau.png
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.461339 tabpy-2.7.0/tabpy/tabpy_tools/
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_tools/__init__.py
+-rw-rw-rw-   0        0        0    12171 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_tools/client.py
+-rw-rw-rw-   0        0        0     2429 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_tools/custom_query_object.py
+-rw-rw-rw-   0        0        0     3052 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_tools/query_object.py
+-rw-rw-rw-   0        0        0    13521 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_tools/rest.py
+-rw-rw-rw-   0        0        0     7283 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_tools/rest_client.py
+-rw-rw-rw-   0        0        0     4241 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/tabpy_tools/schema.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.466338 tabpy-2.7.0/tabpy/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/utils/__init__.py
+-rw-rw-rw-   0        0        0     4394 2023-02-17 14:44:24.000000 tabpy-2.7.0/tabpy/utils/tabpy_user.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.321337 tabpy-2.7.0/tabpy.egg-info/
+-rw-rw-rw-   0        0        0     6773 2023-04-20 19:39:01.000000 tabpy-2.7.0/tabpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4414 2023-04-20 19:39:01.000000 tabpy-2.7.0/tabpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 19:39:01.000000 tabpy-2.7.0/tabpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-04-20 19:39:01.000000 tabpy-2.7.0/tabpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      218 2023-04-20 19:39:01.000000 tabpy-2.7.0/tabpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 19:39:01.000000 tabpy-2.7.0/tabpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.469339 tabpy-2.7.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.514989 tabpy-2.7.0/tests/integration/
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/__init__.py
+-rw-rw-rw-   0        0        0    10362 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/integ_test_base.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.528991 tabpy-2.7.0/tests/integration/resources/
+-rw-rw-rw-   0        0        0     1398 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/resources/2019_04_24_to_3018_08_25.crt
+-rw-rw-rw-   0        0        0     1706 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/resources/2019_04_24_to_3018_08_25.key
+-rw-rw-rw-   0        0        0     1569 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/resources/deploy_and_evaluate_model.conf
+-rw-rw-rw-   0        0        0     1582 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/resources/deploy_and_evaluate_model_auth.conf
+-rw-rw-rw-   0        0        0      136 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/resources/pwdfile.txt
+-rw-rw-rw-   0        0        0     2246 2023-04-20 19:20:47.000000 tabpy-2.7.0/tests/integration/test_arrow_server.py
+-rw-rw-rw-   0        0        0     2461 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/test_auth.py
+-rw-rw-rw-   0        0        0     1261 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/test_custom_evaluate_timeout.py
+-rw-rw-rw-   0        0        0     1067 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/test_deploy_and_evaluate_model.py
+-rw-rw-rw-   0        0        0     1267 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/test_deploy_and_evaluate_model_auth_on.py
+-rw-rw-rw-   0        0        0     1506 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/test_deploy_and_evaluate_model_ssl.py
+-rw-rw-rw-   0        0        0      736 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/test_deploy_model_ssl_off_auth_off.py
+-rw-rw-rw-   0        0        0      950 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/test_deploy_model_ssl_off_auth_on.py
+-rw-rw-rw-   0        0        0     1112 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/test_deploy_model_ssl_on_auth_off.py
+-rw-rw-rw-   0        0        0     3045 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/test_deploy_model_ssl_on_auth_on.py
+-rw-rw-rw-   0        0        0     3295 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/test_evaluate.py
+-rw-rw-rw-   0        0        0     3376 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/test_gzip.py
+-rw-rw-rw-   0        0        0      725 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/test_url.py
+-rw-rw-rw-   0        0        0      986 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/integration/test_url_ssl.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.531993 tabpy-2.7.0/tests/unit/
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.553993 tabpy-2.7.0/tests/unit/server_tests/
+-rw-rw-rw-   0        0        0        0 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/server_tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.563993 tabpy-2.7.0/tests/unit/server_tests/resources/
+-rw-rw-rw-   0        0        0      758 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/server_tests/resources/expired.crt
+-rw-rw-rw-   0        0        0     4330 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/server_tests/resources/future.crt
+-rw-rw-rw-   0        0        0     1410 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/server_tests/resources/valid.crt
+-rw-rw-rw-   0        0        0    13712 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/server_tests/test_config.py
+-rw-rw-rw-   0        0        0      486 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/server_tests/test_endpoint_file_manager.py
+-rw-rw-rw-   0        0        0     5347 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/server_tests/test_endpoint_handler.py
+-rw-rw-rw-   0        0        0     4729 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/server_tests/test_endpoints_handler.py
+-rw-rw-rw-   0        0        0    16279 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/server_tests/test_evaluation_plane_handler.py
+-rw-rw-rw-   0        0        0     5711 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/server_tests/test_pwd_file.py
+-rw-rw-rw-   0        0        0     5519 2023-04-20 19:20:47.000000 tabpy-2.7.0/tests/unit/server_tests/test_service_info_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:39:01.578990 tabpy-2.7.0/tests/unit/tools_tests/
+-rw-rw-rw-   0        0        0      100 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/tools_tests/__init__.py
+-rw-rw-rw-   0        0        0     3262 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/tools_tests/test_client.py
+-rw-rw-rw-   0        0        0     7665 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/tools_tests/test_rest.py
+-rw-rw-rw-   0        0        0     1959 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/tools_tests/test_rest_object.py
+-rw-rw-rw-   0        0        0     1082 2023-02-17 14:44:24.000000 tabpy-2.7.0/tests/unit/tools_tests/test_schema.py
```

### Comparing `tabpy-2.6.0/CHANGELOG` & `tabpy-2.7.0/CHANGELOG`

 * *Files 20% similar despite different names*

```diff
@@ -1,221 +1,228 @@
-# Changelog
-
-## v2.6.0
-
-### Improvements
-
-- Fixes deprecation of sklearn in favor of current package name
-scikit-learn
-
-## v2.5.1
-
-### Improvements
-
-- Gzip encoded requests are now supported by default. This can be disabled in
-the config file.
-- The INFO method will return the enabled status of features.
-
-## v2.5.0
-
-### Improvements
-
-- A server with Adhoc Disabled Flag on with the wrong credentials will now
-  return wrong credentials error instead of telling the user
-  that Adhoc Scripts are not allowed on this server.
-- Added documentation for how to run TabPy projects with local changes
-
-### Breaking changes
-
-- Discontinued support for Python 3.6
-- Added support for Python 3.9
-
-## v2.4.0
-
-### Improvements
-
-- Add toggle to turn off evaluate API.
-
-### Breaking changes
-
-- Changing error code to 406 when server not configured for authentication
-  but credentials are provided by client.
-
-## v2.3.2
-
-### Improvements
-
-- Test files added to tar.gz and zip releases.
-
-## v2.3.1
-
-### Bug fixes
-
-- Overriding deployed models.
-
-## v2.3.0
-
-### Improvements
-
-- Fixed scrutinizer test run failure.
-
-## v2.2.0
-
-### Breaking changes
-
-- TabPy fails with 400 when it is not configure for authentication
-  but credentials are provided by client.
-
-### Bug fixes
-
-- When TabPy is running with no console attached it is not failing
-  with 500 when trying to respond with 401 status.
-- tabpy.query() failing when auth is configured.
-
-### Improvements
-
-- Minor code cleanup.
-
-## v1.1.0
-
-### Improvements
-
-- Authorization is now required for the /info API method.
-  This method did not check authentication previously. This change is
-  backwards compatible with Tableau clients.
-- Improved config parsing flexibility. Previously the
-  TABPY_EVALUATE_TIMEOUT setting would be set to a default if
-  tabpy couldn't parse the value. Now it will throw an exception
-  at startup.
-
-## v1.0.0
-
-### Improvements
-
-- Minor: feature name changed to analytics extensions.
-- Startup script files deleted.
-- Index page updated.
-
-### Other
-
-- TabPy is now Tableau Supported (used to be Community Supported).
-
-## v0.9.0
-
-### Improvements
-
-- Models deployment doesn't depend on pip._internal anymore.
-- Package size reduced.
-
-## v0.8.13
-
-### Improvements
-
-- TabPy works with Python 3.8 now.
-- Documentation updates with referencing Tableau Help pages.
-- Added Client.remove() method for deleting deployed models.
-
-### Bug Fixes
-
-- Fixed failing Ctrl+C handler.
-- Fixed query_timeout bug.
-- Fixed None in result collection bug.
-- Fixed script evaluation with missing result/return bug.
-- Fixed startup failure on Windows for Python 3.8.
-
-## v0.8.9
-
-### Improvements
-
-- Added Ctrl+C handler
-- Added configurable buffer size for HTTP requests
-- Added anvoa to supported pre-deployed models in tabpy
-
-## v0.8.7
-
-### Improvements
-
-- Enabled the use of environment variables in the config file.
-
-## v0.8.6
-
-### Fixes
-
-- Fixed file names for package building.
-- Fixed reading version info for /info call.
-
-## v0.8
-
-### Improvements
-
-- TabPy is pip package now
-- Models are deployed with updated script
-
-## v0.7
-
-### Improvements
-
-- Added t-test model
-- Fixed models call with /evaluate for HTTPS
-- Migrated to Tornado 6
-- Timeout is configurable with TABPY_EVALUATE_TIMEOUT config
-  file option
-
-## v0.6.1
-
-### Improvements
-
-- Scripts, documentation, and integration tests for models
-- Small bug fixes 
-- Added request context logging as a feature controlled with
-  TABPY_LOG_DETAILS configuration setting.
-- Updated documentation for /info method and v1 API.
-- Added integration tests.
-
-## v0.4
-
-### Improvements
-
-- Added basic access authentication (all methods except /info)
-- tabpy-tools can deploy models to TabPy with authentication on
-- Increased unit tests coverage
-- Travis CI for merge requests: unit tests executed, code style checking
-
-## v0.3.2
-
-### Breaking changes
-
-- Logger configuration now is in TabPy config file.
-
-### Improvements
-
-- Remove versioneer and just replace it with VERSION file
-- Require Python 3.6.5
-- Require jsonschema to be compatible with 2.3.0
-- Added setup instructions (known issues) for CentOS
-
-## v0.3.1
-
-- Fixed dependency on tabpy-tools in startup scripts
-- Fixed Python version dependency in tabpy-server setup script
-
-## v0.3
-
-### Breaking changes
-
-- The config file is now not just Python code but an actual config
-- Tornado config file has a different setting for CORS
-- Setup scripts are deleted - setup (if needed) happens with the startup script
-- tabpy-client is tabpy-tools now
-
-### Improvements
-
-- Secure connection (HTTPS) is supported with Tableau 2019.2 and newer versions
-- Documentation is improved with more examples added
-- Versioning is done with Versioneer and github release tags
-- Improved logging
-- Unit tests are passing now
-- Configurations for Postman and Swagger are available to use those against running TabPy
-
-## v0.2
-
-- Initial version
+# Changelog
+
+## v2.7.0
+
+### Improvements
+
+- Adds support for data streaming in Arrow columnar format via Apache
+Arrow Flight.
+
+## v2.6.0
+
+### Improvements
+
+- Fixes deprecation of sklearn in favor of current package name
+scikit-learn
+
+## v2.5.1
+
+### Improvements
+
+- Gzip encoded requests are now supported by default. This can be disabled in
+the config file.
+- The INFO method will return the enabled status of features.
+
+## v2.5.0
+
+### Improvements
+
+- A server with Adhoc Disabled Flag on with the wrong credentials will now
+  return wrong credentials error instead of telling the user
+  that Adhoc Scripts are not allowed on this server.
+- Added documentation for how to run TabPy projects with local changes
+
+### Breaking changes
+
+- Discontinued support for Python 3.6
+- Added support for Python 3.9
+
+## v2.4.0
+
+### Improvements
+
+- Add toggle to turn off evaluate API.
+
+### Breaking changes
+
+- Changing error code to 406 when server not configured for authentication
+  but credentials are provided by client.
+
+## v2.3.2
+
+### Improvements
+
+- Test files added to tar.gz and zip releases.
+
+## v2.3.1
+
+### Bug fixes
+
+- Overriding deployed models.
+
+## v2.3.0
+
+### Improvements
+
+- Fixed scrutinizer test run failure.
+
+## v2.2.0
+
+### Breaking changes
+
+- TabPy fails with 400 when it is not configure for authentication
+  but credentials are provided by client.
+
+### Bug fixes
+
+- When TabPy is running with no console attached it is not failing
+  with 500 when trying to respond with 401 status.
+- tabpy.query() failing when auth is configured.
+
+### Improvements
+
+- Minor code cleanup.
+
+## v1.1.0
+
+### Improvements
+
+- Authorization is now required for the /info API method.
+  This method did not check authentication previously. This change is
+  backwards compatible with Tableau clients.
+- Improved config parsing flexibility. Previously the
+  TABPY_EVALUATE_TIMEOUT setting would be set to a default if
+  tabpy couldn't parse the value. Now it will throw an exception
+  at startup.
+
+## v1.0.0
+
+### Improvements
+
+- Minor: feature name changed to analytics extensions.
+- Startup script files deleted.
+- Index page updated.
+
+### Other
+
+- TabPy is now Tableau Supported (used to be Community Supported).
+
+## v0.9.0
+
+### Improvements
+
+- Models deployment doesn't depend on pip._internal anymore.
+- Package size reduced.
+
+## v0.8.13
+
+### Improvements
+
+- TabPy works with Python 3.8 now.
+- Documentation updates with referencing Tableau Help pages.
+- Added Client.remove() method for deleting deployed models.
+
+### Bug Fixes
+
+- Fixed failing Ctrl+C handler.
+- Fixed query_timeout bug.
+- Fixed None in result collection bug.
+- Fixed script evaluation with missing result/return bug.
+- Fixed startup failure on Windows for Python 3.8.
+
+## v0.8.9
+
+### Improvements
+
+- Added Ctrl+C handler
+- Added configurable buffer size for HTTP requests
+- Added anvoa to supported pre-deployed models in tabpy
+
+## v0.8.7
+
+### Improvements
+
+- Enabled the use of environment variables in the config file.
+
+## v0.8.6
+
+### Fixes
+
+- Fixed file names for package building.
+- Fixed reading version info for /info call.
+
+## v0.8
+
+### Improvements
+
+- TabPy is pip package now
+- Models are deployed with updated script
+
+## v0.7
+
+### Improvements
+
+- Added t-test model
+- Fixed models call with /evaluate for HTTPS
+- Migrated to Tornado 6
+- Timeout is configurable with TABPY_EVALUATE_TIMEOUT config
+  file option
+
+## v0.6.1
+
+### Improvements
+
+- Scripts, documentation, and integration tests for models
+- Small bug fixes 
+- Added request context logging as a feature controlled with
+  TABPY_LOG_DETAILS configuration setting.
+- Updated documentation for /info method and v1 API.
+- Added integration tests.
+
+## v0.4
+
+### Improvements
+
+- Added basic access authentication (all methods except /info)
+- tabpy-tools can deploy models to TabPy with authentication on
+- Increased unit tests coverage
+- Travis CI for merge requests: unit tests executed, code style checking
+
+## v0.3.2
+
+### Breaking changes
+
+- Logger configuration now is in TabPy config file.
+
+### Improvements
+
+- Remove versioneer and just replace it with VERSION file
+- Require Python 3.6.5
+- Require jsonschema to be compatible with 2.3.0
+- Added setup instructions (known issues) for CentOS
+
+## v0.3.1
+
+- Fixed dependency on tabpy-tools in startup scripts
+- Fixed Python version dependency in tabpy-server setup script
+
+## v0.3
+
+### Breaking changes
+
+- The config file is now not just Python code but an actual config
+- Tornado config file has a different setting for CORS
+- Setup scripts are deleted - setup (if needed) happens with the startup script
+- tabpy-client is tabpy-tools now
+
+### Improvements
+
+- Secure connection (HTTPS) is supported with Tableau 2019.2 and newer versions
+- Documentation is improved with more examples added
+- Versioning is done with Versioneer and github release tags
+- Improved logging
+- Unit tests are passing now
+- Configurations for Postman and Swagger are available to use those against running TabPy
+
+## v0.2
+
+- Initial version
```

### Comparing `tabpy-2.6.0/MANIFEST.in` & `tabpy-2.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/PKG-INFO` & `tabpy-2.7.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,262 +1,269 @@
-Metadata-Version: 2.1
-Name: tabpy
-Version: 2.6.0
-Summary: Web server Tableau uses to run Python scripts.
-Home-page: https://github.com/tableau/TabPy
-Download-URL: https://pypi.org/project/tabpy
-Author: Tableau
-Author-email: github@tableau.com
-Maintainer: Tableau
-Maintainer-email: github@tableau.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/tableau/TabPy/issues
-Project-URL: Documentation, https://tableau.github.io/TabPy/
-Project-URL: Source Code, https://github.com/tableau/TabPy
-Keywords: tabpy tableau
-Platform: Windows
-Platform: Linux
-Platform: Mac OS-X
-Platform: Unix
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-TabPy (the Tableau Python Server) is an external service implementation
-which expands Tableau's capabilities by allowing users to execute Python
-scripts and saved functions via Tableau's table calculations.
-
-# Changelog
-
-## v2.6.0
-
-### Improvements
-
-- Fixes deprecation of sklearn in favor of current package name
-scikit-learn
-
-## v2.5.1
-
-### Improvements
-
-- Gzip encoded requests are now supported by default. This can be disabled in
-the config file.
-- The INFO method will return the enabled status of features.
-
-## v2.5.0
-
-### Improvements
-
-- A server with Adhoc Disabled Flag on with the wrong credentials will now
-  return wrong credentials error instead of telling the user
-  that Adhoc Scripts are not allowed on this server.
-- Added documentation for how to run TabPy projects with local changes
-
-### Breaking changes
-
-- Discontinued support for Python 3.6
-- Added support for Python 3.9
-
-## v2.4.0
-
-### Improvements
-
-- Add toggle to turn off evaluate API.
-
-### Breaking changes
-
-- Changing error code to 406 when server not configured for authentication
-  but credentials are provided by client.
-
-## v2.3.2
-
-### Improvements
-
-- Test files added to tar.gz and zip releases.
-
-## v2.3.1
-
-### Bug fixes
-
-- Overriding deployed models.
-
-## v2.3.0
-
-### Improvements
-
-- Fixed scrutinizer test run failure.
-
-## v2.2.0
-
-### Breaking changes
-
-- TabPy fails with 400 when it is not configure for authentication
-  but credentials are provided by client.
-
-### Bug fixes
-
-- When TabPy is running with no console attached it is not failing
-  with 500 when trying to respond with 401 status.
-- tabpy.query() failing when auth is configured.
-
-### Improvements
-
-- Minor code cleanup.
-
-## v1.1.0
-
-### Improvements
-
-- Authorization is now required for the /info API method.
-  This method did not check authentication previously. This change is
-  backwards compatible with Tableau clients.
-- Improved config parsing flexibility. Previously the
-  TABPY_EVALUATE_TIMEOUT setting would be set to a default if
-  tabpy couldn't parse the value. Now it will throw an exception
-  at startup.
-
-## v1.0.0
-
-### Improvements
-
-- Minor: feature name changed to analytics extensions.
-- Startup script files deleted.
-- Index page updated.
-
-### Other
-
-- TabPy is now Tableau Supported (used to be Community Supported).
-
-## v0.9.0
-
-### Improvements
-
-- Models deployment doesn't depend on pip._internal anymore.
-- Package size reduced.
-
-## v0.8.13
-
-### Improvements
-
-- TabPy works with Python 3.8 now.
-- Documentation updates with referencing Tableau Help pages.
-- Added Client.remove() method for deleting deployed models.
-
-### Bug Fixes
-
-- Fixed failing Ctrl+C handler.
-- Fixed query_timeout bug.
-- Fixed None in result collection bug.
-- Fixed script evaluation with missing result/return bug.
-- Fixed startup failure on Windows for Python 3.8.
-
-## v0.8.9
-
-### Improvements
-
-- Added Ctrl+C handler
-- Added configurable buffer size for HTTP requests
-- Added anvoa to supported pre-deployed models in tabpy
-
-## v0.8.7
-
-### Improvements
-
-- Enabled the use of environment variables in the config file.
-
-## v0.8.6
-
-### Fixes
-
-- Fixed file names for package building.
-- Fixed reading version info for /info call.
-
-## v0.8
-
-### Improvements
-
-- TabPy is pip package now
-- Models are deployed with updated script
-
-## v0.7
-
-### Improvements
-
-- Added t-test model
-- Fixed models call with /evaluate for HTTPS
-- Migrated to Tornado 6
-- Timeout is configurable with TABPY_EVALUATE_TIMEOUT config
-  file option
-
-## v0.6.1
-
-### Improvements
-
-- Scripts, documentation, and integration tests for models
-- Small bug fixes 
-- Added request context logging as a feature controlled with
-  TABPY_LOG_DETAILS configuration setting.
-- Updated documentation for /info method and v1 API.
-- Added integration tests.
-
-## v0.4
-
-### Improvements
-
-- Added basic access authentication (all methods except /info)
-- tabpy-tools can deploy models to TabPy with authentication on
-- Increased unit tests coverage
-- Travis CI for merge requests: unit tests executed, code style checking
-
-## v0.3.2
-
-### Breaking changes
-
-- Logger configuration now is in TabPy config file.
-
-### Improvements
-
-- Remove versioneer and just replace it with VERSION file
-- Require Python 3.6.5
-- Require jsonschema to be compatible with 2.3.0
-- Added setup instructions (known issues) for CentOS
-
-## v0.3.1
-
-- Fixed dependency on tabpy-tools in startup scripts
-- Fixed Python version dependency in tabpy-server setup script
-
-## v0.3
-
-### Breaking changes
-
-- The config file is now not just Python code but an actual config
-- Tornado config file has a different setting for CORS
-- Setup scripts are deleted - setup (if needed) happens with the startup script
-- tabpy-client is tabpy-tools now
-
-### Improvements
-
-- Secure connection (HTTPS) is supported with Tableau 2019.2 and newer versions
-- Documentation is improved with more examples added
-- Versioning is done with Versioneer and github release tags
-- Improved logging
-- Unit tests are passing now
-- Configurations for Postman and Swagger are available to use those against running TabPy
-
-## v0.2
-
-- Initial version
+Metadata-Version: 2.1
+Name: tabpy
+Version: 2.7.0
+Summary: Web server Tableau uses to run Python scripts.
+Home-page: https://github.com/tableau/TabPy
+Download-URL: https://pypi.org/project/tabpy
+Author: Tableau
+Author-email: github@tableau.com
+Maintainer: Tableau
+Maintainer-email: github@tableau.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/tableau/TabPy/issues
+Project-URL: Documentation, https://tableau.github.io/TabPy/
+Project-URL: Source Code, https://github.com/tableau/TabPy
+Keywords: tabpy tableau
+Platform: Windows
+Platform: Linux
+Platform: Mac OS-X
+Platform: Unix
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+TabPy (the Tableau Python Server) is an external service implementation
+which expands Tableau's capabilities by allowing users to execute Python
+scripts and saved functions via Tableau's table calculations.
+
+# Changelog
+
+## v2.7.0
+
+### Improvements
+
+- Adds support for data streaming in Arrow columnar format via Apache
+Arrow Flight.
+
+## v2.6.0
+
+### Improvements
+
+- Fixes deprecation of sklearn in favor of current package name
+scikit-learn
+
+## v2.5.1
+
+### Improvements
+
+- Gzip encoded requests are now supported by default. This can be disabled in
+the config file.
+- The INFO method will return the enabled status of features.
+
+## v2.5.0
+
+### Improvements
+
+- A server with Adhoc Disabled Flag on with the wrong credentials will now
+  return wrong credentials error instead of telling the user
+  that Adhoc Scripts are not allowed on this server.
+- Added documentation for how to run TabPy projects with local changes
+
+### Breaking changes
+
+- Discontinued support for Python 3.6
+- Added support for Python 3.9
+
+## v2.4.0
+
+### Improvements
+
+- Add toggle to turn off evaluate API.
+
+### Breaking changes
+
+- Changing error code to 406 when server not configured for authentication
+  but credentials are provided by client.
+
+## v2.3.2
+
+### Improvements
+
+- Test files added to tar.gz and zip releases.
+
+## v2.3.1
+
+### Bug fixes
+
+- Overriding deployed models.
+
+## v2.3.0
+
+### Improvements
+
+- Fixed scrutinizer test run failure.
+
+## v2.2.0
+
+### Breaking changes
+
+- TabPy fails with 400 when it is not configure for authentication
+  but credentials are provided by client.
+
+### Bug fixes
+
+- When TabPy is running with no console attached it is not failing
+  with 500 when trying to respond with 401 status.
+- tabpy.query() failing when auth is configured.
+
+### Improvements
+
+- Minor code cleanup.
+
+## v1.1.0
+
+### Improvements
+
+- Authorization is now required for the /info API method.
+  This method did not check authentication previously. This change is
+  backwards compatible with Tableau clients.
+- Improved config parsing flexibility. Previously the
+  TABPY_EVALUATE_TIMEOUT setting would be set to a default if
+  tabpy couldn't parse the value. Now it will throw an exception
+  at startup.
+
+## v1.0.0
+
+### Improvements
+
+- Minor: feature name changed to analytics extensions.
+- Startup script files deleted.
+- Index page updated.
+
+### Other
+
+- TabPy is now Tableau Supported (used to be Community Supported).
+
+## v0.9.0
+
+### Improvements
+
+- Models deployment doesn't depend on pip._internal anymore.
+- Package size reduced.
+
+## v0.8.13
+
+### Improvements
+
+- TabPy works with Python 3.8 now.
+- Documentation updates with referencing Tableau Help pages.
+- Added Client.remove() method for deleting deployed models.
+
+### Bug Fixes
+
+- Fixed failing Ctrl+C handler.
+- Fixed query_timeout bug.
+- Fixed None in result collection bug.
+- Fixed script evaluation with missing result/return bug.
+- Fixed startup failure on Windows for Python 3.8.
+
+## v0.8.9
+
+### Improvements
+
+- Added Ctrl+C handler
+- Added configurable buffer size for HTTP requests
+- Added anvoa to supported pre-deployed models in tabpy
+
+## v0.8.7
+
+### Improvements
+
+- Enabled the use of environment variables in the config file.
+
+## v0.8.6
+
+### Fixes
+
+- Fixed file names for package building.
+- Fixed reading version info for /info call.
+
+## v0.8
+
+### Improvements
+
+- TabPy is pip package now
+- Models are deployed with updated script
+
+## v0.7
+
+### Improvements
+
+- Added t-test model
+- Fixed models call with /evaluate for HTTPS
+- Migrated to Tornado 6
+- Timeout is configurable with TABPY_EVALUATE_TIMEOUT config
+  file option
+
+## v0.6.1
+
+### Improvements
+
+- Scripts, documentation, and integration tests for models
+- Small bug fixes 
+- Added request context logging as a feature controlled with
+  TABPY_LOG_DETAILS configuration setting.
+- Updated documentation for /info method and v1 API.
+- Added integration tests.
+
+## v0.4
+
+### Improvements
+
+- Added basic access authentication (all methods except /info)
+- tabpy-tools can deploy models to TabPy with authentication on
+- Increased unit tests coverage
+- Travis CI for merge requests: unit tests executed, code style checking
+
+## v0.3.2
+
+### Breaking changes
+
+- Logger configuration now is in TabPy config file.
+
+### Improvements
+
+- Remove versioneer and just replace it with VERSION file
+- Require Python 3.6.5
+- Require jsonschema to be compatible with 2.3.0
+- Added setup instructions (known issues) for CentOS
+
+## v0.3.1
+
+- Fixed dependency on tabpy-tools in startup scripts
+- Fixed Python version dependency in tabpy-server setup script
+
+## v0.3
+
+### Breaking changes
+
+- The config file is now not just Python code but an actual config
+- Tornado config file has a different setting for CORS
+- Setup scripts are deleted - setup (if needed) happens with the startup script
+- tabpy-client is tabpy-tools now
+
+### Improvements
+
+- Secure connection (HTTPS) is supported with Tableau 2019.2 and newer versions
+- Documentation is improved with more examples added
+- Versioning is done with Versioneer and github release tags
+- Improved logging
+- Unit tests are passing now
+- Configurations for Postman and Swagger are available to use those against running TabPy
+
+## v0.2
+
+- Initial version
```

### Comparing `tabpy-2.6.0/README.md` & `tabpy-2.7.0/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-# TabPy
-
-[![Tableau Supported](https://img.shields.io/badge/Support%20Level-Tableau%20Supported-53bd92.svg)](https://www.tableau.com/support-levels-it-and-developer-tools)
-[![GitHub](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://raw.githubusercontent.com/Tableau/TabPy/master/LICENSE)
-
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/tableau/tabpy/Test%20Run%20on%20Push)](https://github.com/tableau/TabPy/actions?query=workflow%3A%22Test+Run+on+Push%22)
-[![Coverage Status](https://coveralls.io/repos/github/tableau/TabPy/badge.svg?branch=master)](https://coveralls.io/github/tableau/TabPy?branch=master)
-[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/tableau/TabPy/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/tableau/TabPy/?branch=master)
-[![Requirements Status](https://requires.io/github/tableau/TabPy/requirements.svg?branch=master)](https://requires.io/github/tableau/TabPy/requirements/?branch=master)
-
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tabpy?label=PyPI%20Python%20versions)
-[![PyPI version](https://badge.fury.io/py/tabpy.svg)](https://pypi.python.org/pypi/tabpy/)
-
-[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/tableau/tabpy)
-
-TabPy (the Tableau Python Server) is an Analytics Extension implementation which
-expands Tableau's capabilities by allowing users to execute Python scripts and
-saved functions via Tableau's table calculations.
-
-Consider reading TabPy documentation in the following order:
-
-* [About TabPy](docs/about.md)
-* [TabPy Installation Instructions](docs/server-install.md)
-* [TabPy Server Configuration Instructions](docs/server-config.md)
-* [Running TabPy in Virtual Environment](docs/tabpy-virtualenv.md)
-* [Running TabPy on Heroku](docs/deploy-to-heroku.md)
-* [Authoring Python calculations in Tableau](docs/TableauConfiguration.md).
-* [TabPy Tools](docs/tabpy-tools.md)
-
-Troubleshooting:
-
-* [TabPy Wiki](https://github.com/tableau/TabPy/wiki)
-
-More technical topics:
-
-* [Contributing Guide](CONTRIBUTING.md) for TabPy developers
-* [TabPy REST API](docs/server-rest.md)
-* [TabPy Security Considerations](docs/security.md)
-
-Other useful resources:
-
-* [Tableau Sci-Fi Blog](http://tabscifi.golovatyi.info/) provides tips, tricks, under
-  the hood, useful resources, and technical details for how to extend
-  Tableau with data science.
-* [Known Issues for the Tableau Analytics Extensions API](https://tableau.github.io/analytics-extensions-api/docs/ae_known_issues.html).
-* For all questions not related to the TabPy code (installation, deployment,
-  connections, Python issues, etc.) and requests use the
-  [Analytics Extensions Forum](https://community.tableau.com/community/forums/analyticsextensions)
-  on [Tableau Community](https://community.tableau.com).
-* [Building advanced analytics applications with TabPy](https://www.tableau.com/about/blog/2017/1/building-advanced-analytics-applications-tabpy-64916)
-* [Building Data Science Applications with TabPy Video Tutorial](https://youtu.be/nRtOMTnBz_Y)
-* [TabPy Tutorial on TabWiki](https://community.tableau.com/docs/DOC-10856)
-
-![GitHub commit activity](https://img.shields.io/github/commit-activity/m/tableau/TabPy.svg)
+# TabPy
+
+[![Tableau Supported](https://img.shields.io/badge/Support%20Level-Tableau%20Supported-53bd92.svg)](https://www.tableau.com/support-levels-it-and-developer-tools)
+[![GitHub](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://raw.githubusercontent.com/Tableau/TabPy/master/LICENSE)
+
+[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/tableau/tabpy/Test%20Run%20on%20Push)](https://github.com/tableau/TabPy/actions?query=workflow%3A%22Test+Run+on+Push%22)
+[![Coverage Status](https://coveralls.io/repos/github/tableau/TabPy/badge.svg?branch=master)](https://coveralls.io/github/tableau/TabPy?branch=master)
+[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/tableau/TabPy/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/tableau/TabPy/?branch=master)
+[![Requirements Status](https://requires.io/github/tableau/TabPy/requirements.svg?branch=master)](https://requires.io/github/tableau/TabPy/requirements/?branch=master)
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tabpy?label=PyPI%20Python%20versions)
+[![PyPI version](https://badge.fury.io/py/tabpy.svg)](https://pypi.python.org/pypi/tabpy/)
+
+[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/tableau/tabpy)
+
+TabPy (the Tableau Python Server) is an Analytics Extension implementation which
+expands Tableau's capabilities by allowing users to execute Python scripts and
+saved functions via Tableau's table calculations.
+
+Consider reading TabPy documentation in the following order:
+
+* [About TabPy](docs/about.md)
+* [TabPy Installation Instructions](docs/server-install.md)
+* [TabPy Server Configuration Instructions](docs/server-config.md)
+* [Running TabPy in Virtual Environment](docs/tabpy-virtualenv.md)
+* [Running TabPy on Heroku](docs/deploy-to-heroku.md)
+* [Authoring Python calculations in Tableau](docs/TableauConfiguration.md).
+* [TabPy Tools](docs/tabpy-tools.md)
+
+Troubleshooting:
+
+* [TabPy Wiki](https://github.com/tableau/TabPy/wiki)
+
+More technical topics:
+
+* [Contributing Guide](CONTRIBUTING.md) for TabPy developers
+* [TabPy REST API](docs/server-rest.md)
+* [TabPy Security Considerations](docs/security.md)
+
+Other useful resources:
+
+* [Tableau Sci-Fi Blog](http://tabscifi.golovatyi.info/) provides tips, tricks, under
+  the hood, useful resources, and technical details for how to extend
+  Tableau with data science.
+* [Known Issues for the Tableau Analytics Extensions API](https://tableau.github.io/analytics-extensions-api/docs/ae_known_issues.html).
+* For all questions not related to the TabPy code (installation, deployment,
+  connections, Python issues, etc.) and requests use the
+  [Analytics Extensions Forum](https://community.tableau.com/community/forums/analyticsextensions)
+  on [Tableau Community](https://community.tableau.com).
+* [Building advanced analytics applications with TabPy](https://www.tableau.com/about/blog/2017/1/building-advanced-analytics-applications-tabpy-64916)
+* [Building Data Science Applications with TabPy Video Tutorial](https://youtu.be/nRtOMTnBz_Y)
+* [TabPy Tutorial on TabWiki](https://community.tableau.com/docs/DOC-10856)
+
+![GitHub commit activity](https://img.shields.io/github/commit-activity/m/tableau/TabPy.svg)
```

### Comparing `tabpy-2.6.0/docs/TableauConfiguration.md` & `tabpy-2.7.0/docs/TableauConfiguration.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-# Using Python in Tableau Calculations
-
-<!-- markdownlint-disable MD004 -->
-
-<!-- toc -->
-
-- [Configuration](#configuration)
-  * [Tableau Desktop](#tableau-desktop)
-  * [Tableau Server 2020.2 and Newer Versions](#tableau-server-20202-and-newer-versions)
-  * [Tableau Server 2020.1 and older](#tableau-server-20201-and-older)
-  * [Tableau Server 2018.2 and 2018.3](#tableau-server-20182-and-20183)
-  * [Tableau Server 2018.1 and Older Versions](#tableau-server-20181-and-older-versions)
-- [Anatomy of a Python Calculation](#anatomy-of-a-python-calculation)
-- [Using Deployed Functions](#using-deployed-functions)
-
-<!-- tocstop -->
-
-<!-- markdownlint-enable MD004 -->
-
-## Configuration
-
-Once you have a [TabPy instance](server-install.md) set up you can easily
-configure Tableau to use this service for evaluating Python code.
-
-### Tableau Desktop
-
-To configure Tableau Desktop version 10.1 or later to connect to TabPy server
-follow steps at Tableau
-[Configure an Analytics Extension connection](https://help.tableau.com/current/pro/desktop/en-us/r_connection_manage.htm#configure-an-external-service-connection)
-documentation page.
-
-### Tableau Server 2020.2 and Newer Versions
-
-Starting from Tableau Server 2020.2 analytics extensions connections
-are configured on site level as shown of
-[Configure Connections to Analytics Extensions](https://help.tableau.com/current/server/en-us/config_r_tabpy.htm)
-page.
-
-### Tableau Server 2020.1 and older
-
-For older Tableau Server versions refer to version specific documentation:
-
-- [2020.1](https://help.tableau.com/v2020.1/server/en-us/config_r_tabpy.htm).
-- [2019.4](https://help.tableau.com/v2019.4/server/en-us/config_r_tabpy.htm).
-- [2019.3](https://help.tableau.com/v2019.3/server/en-us/cli_security_tsm.htm#tsm_security_vizql-extsvc-ssl-enable).
-- [2019.2](https://help.tableau.com/v2019.2/server/en-us/cli_security_tsm.htm#tsm_security_vizql-extsvc-ssl-enable).
-- [2019.1](https://help.tableau.com/v2019.1/server/en-us/cli_security_tsm.htm#tsm_security_vizql-extsvc-ssl-enable).
-
-### Tableau Server 2018.2 and 2018.3
-
-To configure Tableau Server 2018.2 and newer versions to connect to TabPy server
-follow instructions on Tableau
-[Configure Connections to Analytics Extensions](https://onlinehelp.tableau.com/current/server/en-us/tsm.htm)
-page.
-
-Specific details about how to configure a secure connection to TabPy, enable or
-disable connections and other setting can be found at Tableau
-[TSM Security documentation](https://onlinehelp.tableau.com/current/server/en-us/cli_security_tsm.htm#tsm_security_vizql-extsvc-ssl-enable)
-page.
-
-For how to configure TabPy instance follow instructions at
-[TabPy Server Config documentation](server-config.md).
-
-### Tableau Server 2018.1 and Older Versions
-
-For Tableau workbooks with embedded Python code to work on Tableau Server 10.1
-or later, you need to go through a similar setup but using the
-[tabadmin](https://onlinehelp.tableau.com/current/server/en-us/tabadmin.htm)
-command line utility. The two server settings that need to be configured are
-`vizqlserver.extsvc.host` and `vizqlserver.extsvc.port`.
-
-```sh
-tabadmin stop
-tabadmin set vizqlserver.extsvc.host <ip address or host name for TabPy>
-tabadmin set vizqlserver.extsvc.port <port for TabPy>
-tabadmin configure
-tabadmin start
-```
-
-Note that you cannot use TabPy secure connection with 2018.1 and older versions
-of Tableau.
-
-Note that it is not necessary to install TabPy on the Tableau Server or Desktop
-computer-all that is required is a pointer to a TabPy server instance.
-
-Once you're done with configuration, you can use Python in calculated fields in
-Tableau.
-
-## Anatomy of a Python Calculation
-
-Tableau can pass code to TabPy through four different functions: SCRIPT_INT,
-SCRIPT_REAL, SCRIPT_STR and SCRIPT_BOOL to accommodate the different return
-types. In the example below you can see a simple function that passes a column
-of book names (highlighted in blue) to Python for proper casing. Since Python
-returns an array of string, SCRIPT_STR function is used.
-
-![A simple example of a Python calculated field in Tableau Desktop](img/Example1-SimpleFunctionCall.png)
-
-For a SCRIPT call to Python to be successful, it needs to return a result
-explicitly specified with the `return` keyword (highlighted in red).
-
-In this simple example, there is only one input but you can pass as many
-arguments to SCRIPT functions as you like. Tableau takes the arguments in the
-order provided and replaces the \_argN placeholders accordingly. In this case
-ATTR([Book Name]) maps to \_arg1 and both are highlighted to indicate the
-association.
-
-Tableau expects the SCRIPT to return a single column that has either a single
-row or the same number of rows as it passed to TabPy. The example above sends
-18 rows of data to TabPy and receives 18 rows back.
-
-In the example below Tableau passes multiple columns to TabPy and gets a single
-value (correlation coefficient) back. SUM(Sales) and SUM(Profit) are used as
-argument 1 and 2 respectively and highlighted in matching colors.
-In this case the function `corrcoef` returns a matrix from which the correlation
-coefficient is extracted such that a single column is returned.
-
-![Using Partitioning settings with calculations](img/Example2-MultipleFunctionCalls.png)
-
-Tableau aggregates the data before sending to TabPy using the level of detail
-of the view. In this particular example each point in the scatter plot is a
-Customer and TabPy is receiving SUM(Sales) and SUM(Profit) for each Customer.
-
-If you would like to run your Python code on disaggregate data, you can achieve
-this simply by unchecking the Aggregate Measures option under the Analysis menu.
-
-The example above showcases another capability that can come in handy if you
-like to run the same Python script multiple times in different contexts. In this
-particular example, unchecking the Category and Segment boxes in the Table
-Calculation dialog results in Tableau making multiple calls to TabPy, once per
-each pane in the visualization.
-Running regression analysis independently for each Segment-Category combination.
-
-In all of these examples the data structure being returned by the function can
-be consumed by Tableau. This may not always be the case. If your Python code
-returns a one dimensional array but TabPy is failing to serialize it to JSON,
-you may want to convert it to a list as shown in the example below.
-
-![Converting to list to make the results JSON serializable](img/python-calculated-field.png)
-
-You can find two detailed working examples with downloadable sample Tableau
-workbooks on [our blog](https://www.tableau.com/about/blog/2017/1/building-advanced-analytics-applications-tabpy-64916).
-
-## Using Deployed Functions
-
-[TabPy Tools documentation](tabpy-tools.md) covers in detail how functions
-could be deployed as endpoints.
-You can invoke such endpoints using `tabpy.query` option by specifying the
-endpoint name and arguments and retrieving the `response` object.
-
-A SCRIPT calculated field in Tableau using the
-[add endpoint](tabpy-tools.md#deploying-a-function) defined in
-[TabPy Tools documentation](tabpy-tools.md) could look like the following:
-
-```sh
-SCRIPT_REAL("
-return tabpy.query('add',_arg1,_arg2)['response']",
--SUM([Discount]),SUM([Price]))
-```
-
-You can find a detailed working example with a downloadable sample Tableau
-workbook showing how to publish models and use the published models in
-calculated fields on
-[our blog](https://www.tableau.com/about/blog/2017/1/building-advanced-analytics-applications-tabpy-64916).
+# Using Python in Tableau Calculations
+
+<!-- markdownlint-disable MD004 -->
+
+<!-- toc -->
+
+- [Configuration](#configuration)
+  * [Tableau Desktop](#tableau-desktop)
+  * [Tableau Server 2020.2 and Newer Versions](#tableau-server-20202-and-newer-versions)
+  * [Tableau Server 2020.1 and older](#tableau-server-20201-and-older)
+  * [Tableau Server 2018.2 and 2018.3](#tableau-server-20182-and-20183)
+  * [Tableau Server 2018.1 and Older Versions](#tableau-server-20181-and-older-versions)
+- [Anatomy of a Python Calculation](#anatomy-of-a-python-calculation)
+- [Using Deployed Functions](#using-deployed-functions)
+
+<!-- tocstop -->
+
+<!-- markdownlint-enable MD004 -->
+
+## Configuration
+
+Once you have a [TabPy instance](server-install.md) set up you can easily
+configure Tableau to use this service for evaluating Python code.
+
+### Tableau Desktop
+
+To configure Tableau Desktop version 10.1 or later to connect to TabPy server
+follow steps at Tableau
+[Configure an Analytics Extension connection](https://help.tableau.com/current/pro/desktop/en-us/r_connection_manage.htm#configure-an-external-service-connection)
+documentation page.
+
+### Tableau Server 2020.2 and Newer Versions
+
+Starting from Tableau Server 2020.2 analytics extensions connections
+are configured on site level as shown of
+[Configure Connections to Analytics Extensions](https://help.tableau.com/current/server/en-us/config_r_tabpy.htm)
+page.
+
+### Tableau Server 2020.1 and older
+
+For older Tableau Server versions refer to version specific documentation:
+
+- [2020.1](https://help.tableau.com/v2020.1/server/en-us/config_r_tabpy.htm).
+- [2019.4](https://help.tableau.com/v2019.4/server/en-us/config_r_tabpy.htm).
+- [2019.3](https://help.tableau.com/v2019.3/server/en-us/cli_security_tsm.htm#tsm_security_vizql-extsvc-ssl-enable).
+- [2019.2](https://help.tableau.com/v2019.2/server/en-us/cli_security_tsm.htm#tsm_security_vizql-extsvc-ssl-enable).
+- [2019.1](https://help.tableau.com/v2019.1/server/en-us/cli_security_tsm.htm#tsm_security_vizql-extsvc-ssl-enable).
+
+### Tableau Server 2018.2 and 2018.3
+
+To configure Tableau Server 2018.2 and newer versions to connect to TabPy server
+follow instructions on Tableau
+[Configure Connections to Analytics Extensions](https://onlinehelp.tableau.com/current/server/en-us/tsm.htm)
+page.
+
+Specific details about how to configure a secure connection to TabPy, enable or
+disable connections and other setting can be found at Tableau
+[TSM Security documentation](https://onlinehelp.tableau.com/current/server/en-us/cli_security_tsm.htm#tsm_security_vizql-extsvc-ssl-enable)
+page.
+
+For how to configure TabPy instance follow instructions at
+[TabPy Server Config documentation](server-config.md).
+
+### Tableau Server 2018.1 and Older Versions
+
+For Tableau workbooks with embedded Python code to work on Tableau Server 10.1
+or later, you need to go through a similar setup but using the
+[tabadmin](https://onlinehelp.tableau.com/current/server/en-us/tabadmin.htm)
+command line utility. The two server settings that need to be configured are
+`vizqlserver.extsvc.host` and `vizqlserver.extsvc.port`.
+
+```sh
+tabadmin stop
+tabadmin set vizqlserver.extsvc.host <ip address or host name for TabPy>
+tabadmin set vizqlserver.extsvc.port <port for TabPy>
+tabadmin configure
+tabadmin start
+```
+
+Note that you cannot use TabPy secure connection with 2018.1 and older versions
+of Tableau.
+
+Note that it is not necessary to install TabPy on the Tableau Server or Desktop
+computer-all that is required is a pointer to a TabPy server instance.
+
+Once you're done with configuration, you can use Python in calculated fields in
+Tableau.
+
+## Anatomy of a Python Calculation
+
+Tableau can pass code to TabPy through four different functions: SCRIPT_INT,
+SCRIPT_REAL, SCRIPT_STR and SCRIPT_BOOL to accommodate the different return
+types. In the example below you can see a simple function that passes a column
+of book names (highlighted in blue) to Python for proper casing. Since Python
+returns an array of string, SCRIPT_STR function is used.
+
+![A simple example of a Python calculated field in Tableau Desktop](img/Example1-SimpleFunctionCall.png)
+
+For a SCRIPT call to Python to be successful, it needs to return a result
+explicitly specified with the `return` keyword (highlighted in red).
+
+In this simple example, there is only one input but you can pass as many
+arguments to SCRIPT functions as you like. Tableau takes the arguments in the
+order provided and replaces the \_argN placeholders accordingly. In this case
+ATTR([Book Name]) maps to \_arg1 and both are highlighted to indicate the
+association.
+
+Tableau expects the SCRIPT to return a single column that has either a single
+row or the same number of rows as it passed to TabPy. The example above sends
+18 rows of data to TabPy and receives 18 rows back.
+
+In the example below Tableau passes multiple columns to TabPy and gets a single
+value (correlation coefficient) back. SUM(Sales) and SUM(Profit) are used as
+argument 1 and 2 respectively and highlighted in matching colors.
+In this case the function `corrcoef` returns a matrix from which the correlation
+coefficient is extracted such that a single column is returned.
+
+![Using Partitioning settings with calculations](img/Example2-MultipleFunctionCalls.png)
+
+Tableau aggregates the data before sending to TabPy using the level of detail
+of the view. In this particular example each point in the scatter plot is a
+Customer and TabPy is receiving SUM(Sales) and SUM(Profit) for each Customer.
+
+If you would like to run your Python code on disaggregate data, you can achieve
+this simply by unchecking the Aggregate Measures option under the Analysis menu.
+
+The example above showcases another capability that can come in handy if you
+like to run the same Python script multiple times in different contexts. In this
+particular example, unchecking the Category and Segment boxes in the Table
+Calculation dialog results in Tableau making multiple calls to TabPy, once per
+each pane in the visualization.
+Running regression analysis independently for each Segment-Category combination.
+
+In all of these examples the data structure being returned by the function can
+be consumed by Tableau. This may not always be the case. If your Python code
+returns a one dimensional array but TabPy is failing to serialize it to JSON,
+you may want to convert it to a list as shown in the example below.
+
+![Converting to list to make the results JSON serializable](img/python-calculated-field.png)
+
+You can find two detailed working examples with downloadable sample Tableau
+workbooks on [our blog](https://www.tableau.com/about/blog/2017/1/building-advanced-analytics-applications-tabpy-64916).
+
+## Using Deployed Functions
+
+[TabPy Tools documentation](tabpy-tools.md) covers in detail how functions
+could be deployed as endpoints.
+You can invoke such endpoints using `tabpy.query` option by specifying the
+endpoint name and arguments and retrieving the `response` object.
+
+A SCRIPT calculated field in Tableau using the
+[add endpoint](tabpy-tools.md#deploying-a-function) defined in
+[TabPy Tools documentation](tabpy-tools.md) could look like the following:
+
+```sh
+SCRIPT_REAL("
+return tabpy.query('add',_arg1,_arg2)['response']",
+-SUM([Discount]),SUM([Price]))
+```
+
+You can find a detailed working example with a downloadable sample Tableau
+workbook showing how to publish models and use the published models in
+calculated fields on
+[our blog](https://www.tableau.com/about/blog/2017/1/building-advanced-analytics-applications-tabpy-64916).
```

### Comparing `tabpy-2.6.0/docs/about.md` & `tabpy-2.7.0/docs/about.md`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# About TabPy
-
-TabPy framework allows Tableau to remotely execute Python code. It has two components:
-
-1. A process built on Tornado, which allows for the remote execution of Python
-   code through a set of [REST APIs](server-rest.md). The code can either be immediately
-   executed or persisted in the server process and exposed as a REST endpoint,
-   to be called later.
-
-2. A [tools library](tabpy-tools.md),
-   based on Python functions which enables the deployment of such endpoints.
-
-Tableau can connect to the TabPy server to execute Python code on the fly and
-display results in Tableau visualizations. Users can control data and parameters
-being sent to TabPy by interacting with their Tableau worksheets, dashboard or stories.
-
-For how to configure Tableau to connect to TabPy server follow steps in
-[Tableau Configuration Document](TableauConfiguration.md).
+# About TabPy
+
+TabPy framework allows Tableau to remotely execute Python code. It has two components:
+
+1. A process built on Tornado, which allows for the remote execution of Python
+   code through a set of [REST APIs](server-rest.md). The code can either be immediately
+   executed or persisted in the server process and exposed as a REST endpoint,
+   to be called later.
+
+2. A [tools library](tabpy-tools.md),
+   based on Python functions which enables the deployment of such endpoints.
+
+Tableau can connect to the TabPy server to execute Python code on the fly and
+display results in Tableau visualizations. Users can control data and parameters
+being sent to TabPy by interacting with their Tableau worksheets, dashboard or stories.
+
+For how to configure Tableau to connect to TabPy server follow steps in
+[Tableau Configuration Document](TableauConfiguration.md).
```

### Comparing `tabpy-2.6.0/docs/img/Example1-SimpleFunctionCall.png` & `tabpy-2.7.0/docs/img/Example1-SimpleFunctionCall.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/docs/img/Example2-MultipleFunctionCalls.png` & `tabpy-2.7.0/docs/img/Example2-MultipleFunctionCalls.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/docs/img/python-calculated-field.png` & `tabpy-2.7.0/docs/img/python-calculated-field.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/docs/security.md` & `tabpy-2.7.0/docs/security.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# TabPy Security Considerations
-
-If security is a significant concern within your organization,
-you may want to consider the following as you use TabPy:
-
-- The REST server and Python execution share the same Python session,
-  meaning that HTTP requests and user scripts are evaluated in the
-  same addressable memory and processor threads.
-- The tabpy.tabpy_tools client does not perform client-side validation of the
-  SSL certificate on TabPy Server.
-- Python scripts can contain code which can harm security on the server
-  where the TabPy is running. For example, Python scripts can:
-  - Access the file system (read/write).
-  - Install new Python packages which can contain binary code.
-  - Execute operating system commands.
-  - Open network connections to other servers and download files.
-- Execution of ad-hoc Python scripts can be disabled by turning off the
-  /evaluate endpoint. To disable /evaluate endpoint, set "TABPY_EVALUATE_ENABLE"
-  to false in config file.
-- Always use the most up-to-date version of Python.
-  TabPy relies on Tornado and if older verions of Python are used with Tornado
-  then malicious users can potentially poison Python server web caches
-  with parameter cloaking.
+# TabPy Security Considerations
+
+If security is a significant concern within your organization,
+you may want to consider the following as you use TabPy:
+
+- The REST server and Python execution share the same Python session,
+  meaning that HTTP requests and user scripts are evaluated in the
+  same addressable memory and processor threads.
+- The tabpy.tabpy_tools client does not perform client-side validation of the
+  SSL certificate on TabPy Server.
+- Python scripts can contain code which can harm security on the server
+  where the TabPy is running. For example, Python scripts can:
+  - Access the file system (read/write).
+  - Install new Python packages which can contain binary code.
+  - Execute operating system commands.
+  - Open network connections to other servers and download files.
+- Execution of ad-hoc Python scripts can be disabled by turning off the
+  /evaluate endpoint. To disable /evaluate endpoint, set "TABPY_EVALUATE_ENABLE"
+  to false in config file.
+- Always use the most up-to-date version of Python.
+  TabPy relies on Tornado and if older verions of Python are used with Tornado
+  then malicious users can potentially poison Python server web caches
+  with parameter cloaking.
```

### Comparing `tabpy-2.6.0/docs/server-config.md` & `tabpy-2.7.0/docs/server-config.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,309 +1,348 @@
-# TabPy Server Configuration Instructions
-
-<!-- markdownlint-disable MD004 -->
-
-<!-- toc -->
-
-- [Custom Settings](#custom-settings)
-  * [Configuration File Content](#configuration-file-content)
-  * [Configuration File Example](#configuration-file-example)
-- [Configuring HTTP vs HTTPS](#configuring-http-vs-https)
-- [Configuring TPS](#configuring-http-vs-https)
-- [Authentication](#authentication)
-  * [Enabling Authentication](#enabling-authentication)
-  * [Password File](#password-file)
-  * [Adding an Account](#adding-an-account)
-  * [Updating an Account](#updating-an-account)
-  * [Deleting an Account](#deleting-an-account)
-- [Logging](#logging)
-  * [Request Context Logging](#request-context-logging)
-
-<!-- tocstop -->
-
-<!-- markdownlint-enable MD004 -->
-
-## Custom Settings
-
-TabPy starts with set of default settings unless settings are provided via
-environment variables or with a config file.
-
-Configuration parameters can be updated with:
-
-1. Adding environment variables - set the environment variable as required by
-   your Operating System. When creating environment variables, use the same
-   name for your environment variable as specified in the config file.
-2. Specifying a parameter in a config file (environment variable value overwrites
-   configuration setting).
-
-Configuration file with custom settings is specified as a command line parameter:
-
-```sh
-tabpy --config=path/to/my/config/file.conf
-```
-
-The default config file is provided to show you the default values but does not
-need to be present to run TabPy.
-
-### Configuration File Content
-
-Configuration file consists of settings for TabPy itself and Python logger
-settings. You should only set parameters if you need different values than
-the defaults.
-
-Environment variables can be used in the config file. Any instances of
-`%(ENV_VAR)s` will be replaced by the value of the environment variable `ENV_VAR`.
-
-TabPy parameters explained below, the logger documentation can be found
-at [`logging.config` documentation page](https://docs.python.org/3.6/library/logging.config.html).
-
-`[TabPy]` parameters:
-
-- `TABPY_PORT` - port for TabPy to listen on. Default value - `9004`.
-- `TABPY_QUERY_OBJECT_PATH` - query objects location. Used with models, see
-  [TabPy Tools documentation](tabpy-tools.md) for details. Default value -
-  `/tmp/query_objects`.
-- `TABPY_STATE_PATH` - state folder location (absolute path) for Tornado web
-   server. Default value - `tabpy/tabpy_server` subfolder in TabPy package
-   folder.
-- `TABPY_STATIC_PATH` - absolute path for location of static files (index.html
-  page) for TabPy instance. Default value - `tabpy/tabpy_server/static`
-  subfolder in TabPy package folder.
-- `TABPY_PWD_FILE` - absolute path to password file. Setting up this parameter
-  makes TabPy require credentials with HTTP(S) requests. More details about
-  authentication can be found in [Authentication](#authentication)
-  section. Default value - not set.
-- `TABPY_TRANSFER_PROTOCOL` - transfer protocol. Default value - `http`. If
-  set to `https` two additional parameters have to be specified:
-  `TABPY_CERTIFICATE_FILE` and `TABPY_KEY_FILE`.
-  Details are in the [Configuring HTTP vs HTTPS](#configuring-http-vs-https)
-  section.
-- `TABPY_CERTIFICATE_FILE` - absolute path to the certificate file to run
-  TabPy with. Only used with `TABPY_TRANSFER_PROTOCOL` set to `https`.
-  Default value - not set.
-- `TABPY_KEY_FILE` - absolute path to private key file to run TabPy with.
-  Only used with `TABPY_TRANSFER_PROTOCOL` set to `https`. Default value -
-  not set.
-- `TABPY_LOG_DETAILS` - when set to `true` additional call information
-  (caller IP, URL, client info, etc.) is logged. Default value - `false`.
-- `TABPY_MAX_REQUEST_SIZE_MB` - maximal request size supported by TabPy server
-  in Megabytes. All requests of exceeding size are rejected. Default value is
-  100 Mb.
-- `TABPY_EVALUATE_ENABLE` - enable evaluate api to execute ad-hoc Python scripts
-  Default value - `true`.
-- `TABPY_EVALUATE_TIMEOUT` - script evaluation timeout in seconds. Default
-  value - `30`. This timeout does not apply when evaluating models either
-  through the `/query` method, or using the `tabpy.query(...)` syntax with
-  the `/evaluate` method.
-- `TABPY_GZIP_ENABLE` - Enable Gzip support for requests. Enabled by default.
-
-### Configuration File Example
-
-**Note:** _Always use absolute paths for the configuration paths
-settings._
-
-```ini
-[TabPy]
-# TABPY_QUERY_OBJECT_PATH = /tmp/query_objects
-# TABPY_PORT = 9004
-# TABPY_STATE_PATH = <package-path>/tabpy/tabpy_server
-
-# Where static pages live
-# TABPY_STATIC_PATH = <package-path>/tabpy/tabpy_server/static
-
-# For how to configure TabPy authentication read
-# docs/server-config.md.
-# TABPY_PWD_FILE = /path/to/password/file.txt
-
-# To set up secure TabPy uncomment and modify the following lines.
-# Note only PEM-encoded x509 certificates are supported.
-# TABPY_TRANSFER_PROTOCOL = https
-# TABPY_CERTIFICATE_FILE = /path/to/certificate/file.crt
-# TABPY_KEY_FILE = /path/to/key/file.key
-
-# Log additional request details including caller IP, full URL, client
-# end user info if provided.
-# TABPY_LOG_DETAILS = true
-
-# Limit request size (in Mb) - any request which size exceeds
-# specified amount will be rejected by TabPy.
-# Default value is 100 Mb.
-# TABPY_MAX_REQUEST_SIZE_MB = 100
-
-# Enable evaluate api to execute ad-hoc Python scripts
-# Enabled by default. Disabling it will result in 404 error.
-# TABPY_EVALUATE_ENABLE = true
-
-# Configure how long a custom script provided to the /evaluate method
-# will run before throwing a TimeoutError.
-# The value should be a float representing the timeout time in seconds.
-# TABPY_EVALUATE_TIMEOUT = 30
-
-[loggers]
-keys=root
-
-[handlers]
-keys=rootHandler,rotatingFileHandler
-
-[formatters]
-keys=rootFormatter
-
-[logger_root]
-level=DEBUG
-handlers=rootHandler,rotatingFileHandler
-qualname=root
-propagete=0
-
-[handler_rootHandler]
-class=StreamHandler
-level=DEBUG
-formatter=rootFormatter
-args=(sys.stdout,)
-
-[handler_rotatingFileHandler]
-class=handlers.RotatingFileHandler
-level=DEBUG
-formatter=rootFormatter
-args=('tabpy_log.log', 'a', 1000000, 5)
-
-[formatter_rootFormatter]
-format=%(asctime)s [%(levelname)s] (%(filename)s:%(module)s:%(lineno)d): %(message)s
-datefmt=%Y-%m-%d,%H:%M:%S
-
-```
-
-## Configuring HTTP vs HTTPS
-
-By default, TabPy serves only HTTP requests. TabPy can be configured to serve
-only HTTPS requests by setting the following parameter in the config file:
-
-```sh
-TABPY_TRANSFER_PROTOCOL = https
-```
-
-If HTTPS is selected, the absolute paths to the cert and key file need to be
-specified in your config file using the following parameters:
-
-```sh
-TABPY_CERTIFICATE_FILE = C:/path/to/cert/file.crt
-TABPY_KEY_FILE = C:/path/to/key/file.key
-```
-
-Note that only PEM-encoded x509 certificates are supported for the secure
-connection scenario.
-
-## Authentication
-
-TabPy supports basic access authentication (see
-[https://en.wikipedia.org/wiki/Basic_access_authentication](https://en.wikipedia.org/wiki/Basic_access_authentication)
-for more details).
-
-### Enabling Authentication
-
-To enable the feature specify the `TABPY_PWD_FILE` parameter in the
-TabPy configuration file with a fully qualified name:
-
-```sh
-TABPY_PWD_FILE = c:\path\to\password\file.txt
-```
-
-### Password File
-
-Password file is a text file containing usernames and hashed passwords
-per line separated by single space. For username only ASCII characters
-are supported. Usernames are case-insensitive.
-
-Passwords in the password file are hashed with PBKDF2.
-
-**It is highly recommended to restrict access to the password file
-with hosting OS mechanisms. Ideally the file should only be accessible
-for reading with the account under which TabPy runs and TabPy admin account.**
-
-There is a `tabpy-user` command provided with `tabpy` package to
-operate with accounts in the password file. Run `tabpy-user -h`
-to see how to use it.
-
-After making any changes to the password file, TabPy needs to be restarted.
-
-### Adding an Account
-
-To add an account run `tabpy-user add`
-command  providing user name, password (optional) and password file:
-
-```sh
-tabpy-user add -u <username> -p <password> -f <pwdfile>
-```
-
-If the (recommended) `-p` argument is not provided a password for the user name
-will be generated and displayed in the command line.
-
-### Updating an Account
-
-To update the password for an account run `tabpy-user update`
-command:
-
-```sh
-tabpy-user update -u <username> -p <password> -f <pwdfile>
-```
-
-If the (recommended) `-p` agrument is not provided a password for the user name
-will be generated and displayed in the command line.
-
-### Deleting an Account
-
-To delete an account open password file in any text editor and delete the
-line with the user name.
-
-### Endpoint Security
-
-All endpoints require authentication if it is enabled for the server.
-
-## Logging
-
-Logging for TabPy is implemented with Python's standard logger and can be configured
-as explained in Python documentation at
-[Logging Configuration page](https://docs.python.org/3.6/library/logging.config.html).
-
-A default config provided with TabPy is at
-[`tabpy-server/tabpy_server/common/default.conf`](tabpy-server/tabpy_server/common/default.conf)
-and has a configuration for console and file loggers. Changing the config file
-allows the user to modify the log level, format of the logged messages and
-add or remove loggers.
-
-### Request Context Logging
-
-For extended logging (e.g. for auditing purposes) additional logging can be turned
-on with setting `TABPY_LOG_DETAILS` configuration file parameter to `true`.
-
-With the feature on additional information is logged for HTTP requests: caller ip,
-URL, client infomation (Tableau Desktop\Server), Tableau user name (for Tableau Server)
-and TabPy user name as shown in the example below:
-
-<!-- markdownlint-disable MD013 -->
-<!-- markdownlint-disable MD040 -->
-
-```
-2019-05-02,13:50:08 [INFO] (base_handler.py:base_handler:90): Call ID: 934073bd-0d29-46d3-b693-b1e4b1efa9e4, Caller: ::1, Method: POST, Resource: http://localhost:9004/evaluate, Client: Postman for manual testing, Tableau user: ogolovatyi
-2019-05-02,13:50:08 [DEBUG] (base_handler.py:base_handler:120): Checking if need to handle authentication, <<
-call ID: 934073bd-0d29-46d3-b693-b1e4b1efa9e4>>
-2019-05-02,13:50:08 [DEBUG] (base_handler.py:base_handler:120): Handling authentication, <<call ID: 934073bd-
-0d29-46d3-b693-b1e4b1efa9e4>>
-2019-05-02,13:50:08 [DEBUG] (base_handler.py:base_handler:120): Checking request headers for authentication d
-ata, <<call ID: 934073bd-0d29-46d3-b693-b1e4b1efa9e4>>
-2019-05-02,13:50:08 [DEBUG] (base_handler.py:base_handler:120): Validating credentials for user name "user1",
- <<call ID: 934073bd-0d29-46d3-b693-b1e4b1efa9e4>>
-2019-05-02,13:50:08 [DEBUG] (state.py:state:484): Collecting Access-Control-Allow-Origin from state file...  
-2019-05-02,13:50:08 [INFO] (base_handler.py:base_handler:120): function to evaluate=def _user_script(tabpy, _
-arg1, _arg2):
- res = []
- for i in range(len(_arg1)):
-   res.append(_arg1[i] * _arg2[i])
- return res
-, <<call ID: 934073bd-0d29-46d3-b693-b1e4b1efa9e4>>
-```
-
-<!-- markdownlint-enable MD040 -->
-<!-- markdownlint-enable MD013 -->
-
-No passwords are logged.
-
-NOTE the request context details are logged with INFO level.
+# TabPy Server Configuration Instructions
+
+<!-- markdownlint-disable MD004 -->
+
+<!-- toc -->
+
+- [Custom Settings](#custom-settings)
+  * [Configuration File Content](#configuration-file-content)
+  * [Configuration File Example](#configuration-file-example)
+- [Configuring HTTP vs HTTPS](#configuring-http-vs-https)
+- [Configuring TPS](#configuring-http-vs-https)
+- [Authentication](#authentication)
+  * [Enabling Authentication](#enabling-authentication)
+  * [Password File](#password-file)
+  * [Adding an Account](#adding-an-account)
+  * [Updating an Account](#updating-an-account)
+  * [Deleting an Account](#deleting-an-account)
+- [Logging](#logging)
+  * [Request Context Logging](#request-context-logging)
+
+<!-- tocstop -->
+
+<!-- markdownlint-enable MD004 -->
+
+## Custom Settings
+
+TabPy starts with set of default settings unless settings are provided via
+environment variables or with a config file.
+
+Configuration parameters can be updated with:
+
+1. Adding environment variables - set the environment variable as required by
+   your Operating System. When creating environment variables, use the same
+   name for your environment variable as specified in the config file.
+2. Specifying a parameter in a config file (environment variable value overwrites
+   configuration setting).
+
+Configuration file with custom settings is specified as a command line parameter:
+
+```sh
+tabpy --config=path/to/my/config/file.conf
+```
+
+The default config file is provided to show you the default values but does not
+need to be present to run TabPy.
+
+### Configuration File Content
+
+Configuration file consists of settings for TabPy itself and Python logger
+settings. You should only set parameters if you need different values than
+the defaults.
+
+Environment variables can be used in the config file. Any instances of
+`%(ENV_VAR)s` will be replaced by the value of the environment variable `ENV_VAR`.
+
+TabPy parameters explained below, the logger documentation can be found
+at [`logging.config` documentation page](https://docs.python.org/3.6/library/logging.config.html).
+
+`[TabPy]` parameters:
+
+- `TABPY_PORT` - port for TabPy to listen on. Default value - `9004`.
+- `TABPY_QUERY_OBJECT_PATH` - query objects location. Used with models, see
+  [TabPy Tools documentation](tabpy-tools.md) for details. Default value -
+  `/tmp/query_objects`.
+- `TABPY_STATE_PATH` - state folder location (absolute path) for Tornado web
+   server. Default value - `tabpy/tabpy_server` subfolder in TabPy package
+   folder.
+- `TABPY_STATIC_PATH` - absolute path for location of static files (index.html
+  page) for TabPy instance. Default value - `tabpy/tabpy_server/static`
+  subfolder in TabPy package folder.
+- `TABPY_PWD_FILE` - absolute path to password file. Setting up this parameter
+  makes TabPy require credentials with HTTP(S) requests. More details about
+  authentication can be found in [Authentication](#authentication)
+  section. Default value - not set.
+- `TABPY_TRANSFER_PROTOCOL` - transfer protocol. Default value - `http`. If
+  set to `https` two additional parameters have to be specified:
+  `TABPY_CERTIFICATE_FILE` and `TABPY_KEY_FILE`.
+  Details are in the [Configuring HTTP vs HTTPS](#configuring-http-vs-https)
+  section.
+- `TABPY_CERTIFICATE_FILE` - absolute path to the certificate file to run
+  TabPy with. Only used with `TABPY_TRANSFER_PROTOCOL` set to `https`.
+  Default value - not set.
+- `TABPY_KEY_FILE` - absolute path to private key file to run TabPy with.
+  Only used with `TABPY_TRANSFER_PROTOCOL` set to `https`. Default value -
+  not set.
+- `TABPY_LOG_DETAILS` - when set to `true` additional call information
+  (caller IP, URL, client info, etc.) is logged. Default value - `false`.
+- `TABPY_MAX_REQUEST_SIZE_MB` - maximal request size supported by TabPy server
+  in Megabytes. All requests of exceeding size are rejected. Default value is
+  100 Mb.
+- `TABPY_EVALUATE_ENABLE` - enable evaluate api to execute ad-hoc Python scripts
+  Default value - `true`.
+- `TABPY_EVALUATE_TIMEOUT` - script evaluation timeout in seconds. Default
+  value - `30`. This timeout does not apply when evaluating models either
+  through the `/query` method, or using the `tabpy.query(...)` syntax with
+  the `/evaluate` method.
+- `TABPY_GZIP_ENABLE` - Enable Gzip support for requests. Enabled by default.
+- `TABPY_ARROW_ENABLE` - Enable Arrow connection for data streaming. Default
+  value is False.
+- `TABPY_ARROWFLIGHT_PORT` - port for
+  [Arrow Flight](https://arrow.apache.org/docs/format/Flight.html)
+  connection used in streaming mode. Default value is 13622.
+
+### Configuration File Example
+
+**Note:** _Always use absolute paths for the configuration paths
+settings._
+
+```ini
+[TabPy]
+# TABPY_QUERY_OBJECT_PATH = /tmp/query_objects
+# TABPY_PORT = 9004
+# TABPY_STATE_PATH = <package-path>/tabpy/tabpy_server
+
+# Where static pages live
+# TABPY_STATIC_PATH = <package-path>/tabpy/tabpy_server/static
+
+# For how to configure TabPy authentication read
+# docs/server-config.md.
+# TABPY_PWD_FILE = /path/to/password/file.txt
+
+# To set up secure TabPy uncomment and modify the following lines.
+# Note only PEM-encoded x509 certificates are supported.
+# TABPY_TRANSFER_PROTOCOL = https
+# TABPY_CERTIFICATE_FILE = /path/to/certificate/file.crt
+# TABPY_KEY_FILE = /path/to/key/file.key
+
+# Log additional request details including caller IP, full URL, client
+# end user info if provided.
+# TABPY_LOG_DETAILS = true
+
+# Limit request size (in Mb) - any request which size exceeds
+# specified amount will be rejected by TabPy.
+# Default value is 100 Mb.
+# TABPY_MAX_REQUEST_SIZE_MB = 100
+
+# Enable evaluate api to execute ad-hoc Python scripts
+# Enabled by default. Disabling it will result in 404 error.
+# TABPY_EVALUATE_ENABLE = true
+
+# Configure how long a custom script provided to the /evaluate method
+# will run before throwing a TimeoutError.
+# The value should be a float representing the timeout time in seconds.
+# TABPY_EVALUATE_TIMEOUT = 30
+
+# Configure TabPy to support streaming data via Arrow Flight.
+# This will cause an Arrow Flight server start up. The Arrow
+# Flight port defaults to 13622 if not set here.
+# TABPY_ARROW_ENABLE = True
+# TABPY_ARROWFLIGHT_PORT = 13622
+
+
+[loggers]
+keys=root
+
+[handlers]
+keys=rootHandler,rotatingFileHandler
+
+[formatters]
+keys=rootFormatter
+
+[logger_root]
+level=DEBUG
+handlers=rootHandler,rotatingFileHandler
+qualname=root
+propagete=0
+
+[handler_rootHandler]
+class=StreamHandler
+level=DEBUG
+formatter=rootFormatter
+args=(sys.stdout,)
+
+[handler_rotatingFileHandler]
+class=handlers.RotatingFileHandler
+level=DEBUG
+formatter=rootFormatter
+args=('tabpy_log.log', 'a', 1000000, 5)
+
+[formatter_rootFormatter]
+format=%(asctime)s [%(levelname)s] (%(filename)s:%(module)s:%(lineno)d): %(message)s
+datefmt=%Y-%m-%d,%H:%M:%S
+
+```
+
+## Configuring HTTP vs HTTPS
+
+By default, TabPy serves only HTTP requests. TabPy can be configured to serve
+only HTTPS requests by setting the following parameter in the config file:
+
+```sh
+TABPY_TRANSFER_PROTOCOL = https
+```
+
+If HTTPS is selected, the absolute paths to the cert and key file need to be
+specified in your config file using the following parameters:
+
+```sh
+TABPY_CERTIFICATE_FILE = C:/path/to/cert/file.crt
+TABPY_KEY_FILE = C:/path/to/key/file.key
+```
+
+Note that only PEM-encoded x509 certificates are supported for the secure
+connection scenario.
+
+## Authentication
+
+TabPy supports basic access authentication (see
+[https://en.wikipedia.org/wiki/Basic_access_authentication](https://en.wikipedia.org/wiki/Basic_access_authentication)
+for more details).
+
+### Enabling Authentication
+
+To enable the feature specify the `TABPY_PWD_FILE` parameter in the
+TabPy configuration file with a fully qualified name:
+
+```sh
+TABPY_PWD_FILE = c:\path\to\password\file.txt
+```
+
+### Password File
+
+Password file is a text file containing usernames and hashed passwords
+per line separated by single space. For username only ASCII characters
+are supported. Usernames are case-insensitive.
+
+Passwords in the password file are hashed with PBKDF2.
+
+**It is highly recommended to restrict access to the password file
+with hosting OS mechanisms. Ideally the file should only be accessible
+for reading with the account under which TabPy runs and TabPy admin account.**
+
+There is a `tabpy-user` command provided with `tabpy` package to
+operate with accounts in the password file. Run `tabpy-user -h`
+to see how to use it.
+
+After making any changes to the password file, TabPy needs to be restarted.
+
+### Adding an Account
+
+To add an account run `tabpy-user add`
+command  providing user name, password (optional) and password file:
+
+```sh
+tabpy-user add -u <username> -p <password> -f <pwdfile>
+```
+
+If the (recommended) `-p` argument is not provided a password for the user name
+will be generated and displayed in the command line.
+
+### Updating an Account
+
+To update the password for an account run `tabpy-user update`
+command:
+
+```sh
+tabpy-user update -u <username> -p <password> -f <pwdfile>
+```
+
+If the (recommended) `-p` agrument is not provided a password for the user name
+will be generated and displayed in the command line.
+
+### Deleting an Account
+
+To delete an account open password file in any text editor and delete the
+line with the user name.
+
+### Endpoint Security
+
+All endpoints require authentication if it is enabled for the server.
+
+## Arrow Flight
+
+TabPy can be configured to enable Arrow Flight. This will cause a Flight
+server to start up alongside the HTTP server and will allow for handling
+incoming streamed data in the Arrow columnar format.
+
+**As of May 2023, the Arrow Flight feature can only be used by compatible
+versions of Tableau Prep. The Arrow Flight feature is not used by Tableau
+Desktop, Tableau Server, or Tableau Cloud, regardless of the
+`TABPY_ARROW_ENABLE` setting. In other words, those products will continue
+to send the data in a single payload when Arrow Flight is both enabled
+and disabled.**
+
+To leverage the Flight server, use an existing Flight Client API. There
+are implementations available in C++, Java, and Python. To begin streaming
+data to the server, a Flight Descriptor (data path) must be generated.
+One can be obtained via the TabPy Flight server by using the client to
+submit a `getUniquePath` Action to the server or it can be randomly generated
+locally. The client's `do_put` interface can then be used to begin sending
+data to the server.
+
+Structure the data payload in Arrow format according to the client's API
+requirements. Continue using the client to append the data path with the
+data stream.
+
+The mechanism for sending the Python script to the server does not change.
+
+## Logging
+
+Logging for TabPy is implemented with Python's standard logger and can be configured
+as explained in Python documentation at
+[Logging Configuration page](https://docs.python.org/3.6/library/logging.config.html).
+
+A default config provided with TabPy is at
+[`tabpy-server/tabpy_server/common/default.conf`](tabpy-server/tabpy_server/common/default.conf)
+and has a configuration for console and file loggers. Changing the config file
+allows the user to modify the log level, format of the logged messages and
+add or remove loggers.
+
+### Request Context Logging
+
+For extended logging (e.g. for auditing purposes) additional logging can be turned
+on with setting `TABPY_LOG_DETAILS` configuration file parameter to `true`.
+
+With the feature on additional information is logged for HTTP requests: caller ip,
+URL, client infomation (Tableau Desktop\Server), Tableau user name (for Tableau Server)
+and TabPy user name as shown in the example below:
+
+<!-- markdownlint-disable MD013 -->
+<!-- markdownlint-disable MD040 -->
+
+```
+2019-05-02,13:50:08 [INFO] (base_handler.py:base_handler:90): Call ID: 934073bd-0d29-46d3-b693-b1e4b1efa9e4, Caller: ::1, Method: POST, Resource: http://localhost:9004/evaluate, Client: Postman for manual testing, Tableau user: ogolovatyi
+2019-05-02,13:50:08 [DEBUG] (base_handler.py:base_handler:120): Checking if need to handle authentication, <<
+call ID: 934073bd-0d29-46d3-b693-b1e4b1efa9e4>>
+2019-05-02,13:50:08 [DEBUG] (base_handler.py:base_handler:120): Handling authentication, <<call ID: 934073bd-
+0d29-46d3-b693-b1e4b1efa9e4>>
+2019-05-02,13:50:08 [DEBUG] (base_handler.py:base_handler:120): Checking request headers for authentication d
+ata, <<call ID: 934073bd-0d29-46d3-b693-b1e4b1efa9e4>>
+2019-05-02,13:50:08 [DEBUG] (base_handler.py:base_handler:120): Validating credentials for user name "user1",
+ <<call ID: 934073bd-0d29-46d3-b693-b1e4b1efa9e4>>
+2019-05-02,13:50:08 [DEBUG] (state.py:state:484): Collecting Access-Control-Allow-Origin from state file...  
+2019-05-02,13:50:08 [INFO] (base_handler.py:base_handler:120): function to evaluate=def _user_script(tabpy, _
+arg1, _arg2):
+ res = []
+ for i in range(len(_arg1)):
+   res.append(_arg1[i] * _arg2[i])
+ return res
+, <<call ID: 934073bd-0d29-46d3-b693-b1e4b1efa9e4>>
+```
+
+<!-- markdownlint-enable MD040 -->
+<!-- markdownlint-enable MD013 -->
+
+No passwords are logged.
+
+NOTE the request context details are logged with INFO level.
```

### Comparing `tabpy-2.6.0/docs/server-rest.md` & `tabpy-2.7.0/docs/server-rest.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-# TabPy REST Interface
-
-The server process exposes several REST APIs to get status and to execute
-Python code and query deployed methods.
-
-<!-- markdownlint-disable MD004 -->
-
-<!-- toc -->
-
-- [Authentication, /info and /evaluate](#authentication-info-and-evaluate)
-- [http:get:: /status](#httpget-status)
-- [http:get:: /endpoints](#httpget-endpoints)
-- [http:get:: /endpoints/:endpoint](#httpget-endpointsendpoint)
-- [http:post:: /query/:endpoint](#httppost-queryendpoint)
-
-<!-- tocstop -->
-
-<!-- markdownlint-enable MD004 -->
-
-## Authentication, /info and /evaluate
-
-Analytics Extensions API v1 is documented at
-[https://tableau.github.io/analytics-extensions-api/docs/ae_api_ref.html](https://tableau.github.io/analytics-extensions-api/docs/ae_api_ref.html).
-
-The following documentation is for methods not currently used by Tableau.
-
-## http:get:: /status
-
-Gets runtime status of deployed endpoints. If no endpoints are deployed in
-the server, the returned data is an empty JSON object.
-
-Example request:
-
-```HTTP
-GET /status HTTP/1.1
-Host: localhost:9004
-Accept: application/json
-```
-
-Example response:
-
-```HTTP
-HTTP/1.1 200 OK
-Content-Type: application/json
-
-{"clustering": {
-  "status": "LoadSuccessful",
-  "last_error": null,
-  "version": 1,
-  "type": "model"},
- "add": {
-  "status": "LoadSuccessful",
-  "last_error": null,
-  "version": 1,
-  "type": "model"}
-}
-```
-
-Using curl:
-
-```bash
-curl -X GET http://localhost:9004/status
-```
-
-## http:get:: /endpoints
-
-Gets a list of deployed endpoints and their static information. If no
-endpoints are deployed in the server, the returned data is an empty JSON object.
-
-Example request:
-
-```HTTP
-GET /endpoints HTTP/1.1
-Host: localhost:9004
-Accept: application/json
-```
-
-Example response:
-
-```HTTP
-HTTP/1.1 200 OK
-Content-Type: application/json
-
-{"clustering":
-  {"description": "",
-   "docstring": "-- no docstring found in query function --",
-   "creation_time": 1469511182,
-   "version": 1,
-   "dependencies": [],
-   "last_modified_time": 1469511182,
-   "type": "model",
-   "target": null},
-"add": {
-  "description": "",
-  "docstring": "-- no docstring found in query function --",
-  "creation_time": 1469505967,
-  "version": 1,
-  "dependencies": [],
-  "last_modified_time": 1469505967,
-  "type": "model",
-  "target": null}
-}
-```
-
-Using curl:
-
-```bash
-curl -X GET http://localhost:9004/endpoints
-```
-
-## http:get:: /endpoints/:endpoint
-
-Gets the description of a specific deployed endpoint. The endpoint must first
-be deployed in the server (see the [TabPy Tools documentation](tabpy-tools.md)).
-
-Example request:
-
-```HTTP
-GET /endpoints/add HTTP/1.1
-Host: localhost:9004
-Accept: application/json
-```
-
-Example response:
-
-```HTTP
-HTTP/1.1 200 OK
-Content-Type: application/json
-
-{"description": "", "docstring": "-- no docstring found in query function --",
- "creation_time": 1469505967, "version": 1, "dependencies": [],
- "last_modified_time": 1469505967, "type": "model", "target": null}
-```
-
-Using curl:
-
-```bash
-curl -X GET http://localhost:9004/endpoints/add
-```
-
-## http:post:: /query/:endpoint
-
-Executes a function at the specified endpoint. The function must first be
-deployed (see the [TabPy Tools documentation](tabpy-tools.md)).
-
-This interface expects a JSON body with a `data` key, specifying the values
-for the function, according to its original definition. In the example below,
-the function `clustering` was defined with a signature of two parameters `x`
-and `y`, expecting arrays of numbers.
-
-Example request:
-
-```HTTP
-POST /query/clustering HTTP/1.1
-Host: localhost:9004
-Accept: application/json
-
-{"data": {
-  "x": [6.35, 6.40, 6.65, 8.60, 8.90, 9.00, 9.10],
-  "y": [1.95, 1.95, 2.05, 3.05, 3.05, 3.10, 3.15]}}
-```
-
-Example response:
-
-```HTTP
-HTTP/1.1 200 OK
-Content-Type: application/json
-
-{"model": "clustering", "version": 1, "response": [0, 0, 0, 1, 1, 1, 1],
- "uuid": "46d3df0e-acca-4560-88f1-67c5aedeb1c4"}
-```
-
-Using curl:
-
-```bash
-curl -X GET http://localhost:9004/query/clustering -d \
-'{"data": {"x": [6.35, 6.40, 6.65, 8.60, 8.90, 9.00, 9.10],
-           "y": [1.95, 1.95, 2.05, 3.05, 3.05, 3.10, 3.15]}}'
-```
+# TabPy REST Interface
+
+The server process exposes several REST APIs to get status and to execute
+Python code and query deployed methods.
+
+<!-- markdownlint-disable MD004 -->
+
+<!-- toc -->
+
+- [Authentication, /info and /evaluate](#authentication-info-and-evaluate)
+- [http:get:: /status](#httpget-status)
+- [http:get:: /endpoints](#httpget-endpoints)
+- [http:get:: /endpoints/:endpoint](#httpget-endpointsendpoint)
+- [http:post:: /query/:endpoint](#httppost-queryendpoint)
+
+<!-- tocstop -->
+
+<!-- markdownlint-enable MD004 -->
+
+## Authentication, /info and /evaluate
+
+Analytics Extensions API v1 is documented at
+[https://tableau.github.io/analytics-extensions-api/docs/ae_api_ref.html](https://tableau.github.io/analytics-extensions-api/docs/ae_api_ref.html).
+
+The following documentation is for methods not currently used by Tableau.
+
+## http:get:: /status
+
+Gets runtime status of deployed endpoints. If no endpoints are deployed in
+the server, the returned data is an empty JSON object.
+
+Example request:
+
+```HTTP
+GET /status HTTP/1.1
+Host: localhost:9004
+Accept: application/json
+```
+
+Example response:
+
+```HTTP
+HTTP/1.1 200 OK
+Content-Type: application/json
+
+{"clustering": {
+  "status": "LoadSuccessful",
+  "last_error": null,
+  "version": 1,
+  "type": "model"},
+ "add": {
+  "status": "LoadSuccessful",
+  "last_error": null,
+  "version": 1,
+  "type": "model"}
+}
+```
+
+Using curl:
+
+```bash
+curl -X GET http://localhost:9004/status
+```
+
+## http:get:: /endpoints
+
+Gets a list of deployed endpoints and their static information. If no
+endpoints are deployed in the server, the returned data is an empty JSON object.
+
+Example request:
+
+```HTTP
+GET /endpoints HTTP/1.1
+Host: localhost:9004
+Accept: application/json
+```
+
+Example response:
+
+```HTTP
+HTTP/1.1 200 OK
+Content-Type: application/json
+
+{"clustering":
+  {"description": "",
+   "docstring": "-- no docstring found in query function --",
+   "creation_time": 1469511182,
+   "version": 1,
+   "dependencies": [],
+   "last_modified_time": 1469511182,
+   "type": "model",
+   "target": null},
+"add": {
+  "description": "",
+  "docstring": "-- no docstring found in query function --",
+  "creation_time": 1469505967,
+  "version": 1,
+  "dependencies": [],
+  "last_modified_time": 1469505967,
+  "type": "model",
+  "target": null}
+}
+```
+
+Using curl:
+
+```bash
+curl -X GET http://localhost:9004/endpoints
+```
+
+## http:get:: /endpoints/:endpoint
+
+Gets the description of a specific deployed endpoint. The endpoint must first
+be deployed in the server (see the [TabPy Tools documentation](tabpy-tools.md)).
+
+Example request:
+
+```HTTP
+GET /endpoints/add HTTP/1.1
+Host: localhost:9004
+Accept: application/json
+```
+
+Example response:
+
+```HTTP
+HTTP/1.1 200 OK
+Content-Type: application/json
+
+{"description": "", "docstring": "-- no docstring found in query function --",
+ "creation_time": 1469505967, "version": 1, "dependencies": [],
+ "last_modified_time": 1469505967, "type": "model", "target": null}
+```
+
+Using curl:
+
+```bash
+curl -X GET http://localhost:9004/endpoints/add
+```
+
+## http:post:: /query/:endpoint
+
+Executes a function at the specified endpoint. The function must first be
+deployed (see the [TabPy Tools documentation](tabpy-tools.md)).
+
+This interface expects a JSON body with a `data` key, specifying the values
+for the function, according to its original definition. In the example below,
+the function `clustering` was defined with a signature of two parameters `x`
+and `y`, expecting arrays of numbers.
+
+Example request:
+
+```HTTP
+POST /query/clustering HTTP/1.1
+Host: localhost:9004
+Accept: application/json
+
+{"data": {
+  "x": [6.35, 6.40, 6.65, 8.60, 8.90, 9.00, 9.10],
+  "y": [1.95, 1.95, 2.05, 3.05, 3.05, 3.10, 3.15]}}
+```
+
+Example response:
+
+```HTTP
+HTTP/1.1 200 OK
+Content-Type: application/json
+
+{"model": "clustering", "version": 1, "response": [0, 0, 0, 1, 1, 1, 1],
+ "uuid": "46d3df0e-acca-4560-88f1-67c5aedeb1c4"}
+```
+
+Using curl:
+
+```bash
+curl -X GET http://localhost:9004/query/clustering -d \
+'{"data": {"x": [6.35, 6.40, 6.65, 8.60, 8.90, 9.00, 9.10],
+           "y": [1.95, 1.95, 2.05, 3.05, 3.05, 3.10, 3.15]}}'
+```
```

### Comparing `tabpy-2.6.0/docs/tabpy-tools.md` & `tabpy-2.7.0/docs/tabpy-tools.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,449 +1,449 @@
-# TabPy Tools
-
-TabPy tools is the Python package of tools for managing the published Python functions
-on TabPy server.
-
-<!-- markdownlint-disable MD004 -->
-
-<!-- toc -->
-
-- [Connecting to TabPy](#connecting-to-tabpy)
-- [Authentication](#authentication)
-- [Deploying a Function](#deploying-a-function)
-- [Predeployed Functions](#predeployed-functions)
-  * [Principal Component Analysis (PCA)](#principal-component-analysis-pca)
-  * [Sentiment Analysis](#sentiment-analysis)
-  * [T-Test](#t-test)
-  * [ANOVA](#anova)
-- [Providing Schema Metadata](#providing-schema-metadata)
-- [Querying an Endpoint](#querying-an-endpoint)
-- [Evaluating Arbitrary Python Scripts](#evaluating-arbitrary-python-scripts)
-- [Deploying Models in TabPy Docker Container](#deploying-models-in-tabpy-docker-container)
-
-<!-- tocstop -->
-
-<!-- markdownlint-enable MD004 -->
-
-## Connecting to TabPy
-
-The tools library uses the notion of connecting to a service to avoid having
-to specify the service location for all subsequent operations:
-
-```python
-
-from tabpy.tabpy_tools.client import Client
-
-client = Client('http://localhost:9004/')
-
-```
-
-The URL and port are where the Tableau-Python-Server process has been started -
-more info can be found in the
-[Starting TabPy](server-install.md#starting-tabpy) section of the documentation.
-
-## Authentication
-
-When TabPy is configured with the authentication feature on, client code
-has to specify the credentials to use during model deployment with the
-`set_credentials` call for a client:
-
-```python
-client.set_credentials('username', 'P@ssw0rd')
-```
-
-Credentials only need to be set once for all further client operations.
-
-In cases where credentials are not provided but are required, the deployment will
-fail with an "Unauthorized" code (401).
-
-For instructions on how to configure and enable the authentication feature for
-TabPy, see [TabPy Server Configuration Instructions](server-config.md).
-
-## Deploying a Function
-
-A persisted endpoint is backed by a Python method. For example:
-
-```python
-def add(x,y):
-    import numpy as np
-    return np.add(x, y).tolist()
-
-client.deploy('add', add, 'Adds two numbers x and y')
-```
-
-The next example is more complex, using scikit-learn's clustering API:
-
-```python
-
-def clustering(x, y):
-    import numpy as np
-    from sklearn.cluster import DBSCAN
-    from sklearn.preprocessing import StandardScaler
-    X = np.column_stack([x, y])
-    X = StandardScaler().fit_transform(X)
-    db = DBSCAN(eps=1, min_samples=3).fit(X)
-    return db.labels_.tolist()
-
-
-client.deploy('clustering',
-              clustering,
-              'Returns cluster Ids for each data point specified by the '
-              'pairs in x and y')
-
-```
-
-In this example the function `clustering` expects a set of two-dimensional
-data points, represented by the list of all x-coordinates and the list of all
-y-coordinates. It will return a set of numerical labels corresponding to the
-clusters to which each datapoint is assigned. We deploy this function as an
-endpoint named `clustering`.
-It is now reachable as a [REST API](server-rest.md#httppost-queryendpoint), as
-well as through the TabPy tools - for details see the next section.
-
-You can re-deploy a function (for example, after you modified its code) by setting
-the `override` parameter to `True`:
-
-```python
-client.deploy('add', add, 'Adds two numbers x and y', override=True)
-```
-
-Each re-deployment of an endpoint will increment its version number, which is also
-returned as part of the query result.
-
-When deploying endpoints which rely on supervised learning models, you may want to
-load a saved model instead of training on-the-fly for performance reasons.
-
-Below is an excerpt from the training stage of a hypothetical model that predicts
-whether or not a loan will default:
-
-```python
-
-from sklearn.ensemble import GradientBoostingClassifier
-
-predictors = [x for x in train.columns if x not in [target, RowID]]
-gbm = GradientBoostingClassifier(learning_rate=0.01, n_estimators=600,max_depth=9,
-min_samples_split=1200, min_samples_leaf=60, subsample=0.85, random_state=10)
-modelfit(gbm, train, test, predictors)
-
-```
-
-When the trained model (named `gbm` in this case) is used in a function being
-deployed (as in `gbm.predict(...)` below), Tableau will automatically save its
-definition using `cloudpickle` along with the definition of the function. The model
-will also be kept in memory on the server in order to achieve faster response times.
-If you persist your model manually to disk and read as part of your scoring function
-code however, you will notice that the response times are noticeably longer - as
-every time a client hits an endpoint, the code (including model loading) will get
-executed. In order to get the best performance, we recommended following the
-methodology outlined in this example.
-
-```python
-def LoanDefaultClassifier(Loan_Amount, Loan_Tenure, Monthly_Income, Age):
-    import pandas as pd
-    data=pd.concat([Loan_Amount,Loan_Tenure,Monthly_Income,Age],axis=1)
-    return gbm.predict(data)
-
-client.deploy('WillItDefault',
-              LoanDefaultClassifier,
-              'Returns whether a loan application is likely to default.')
-```
-
-You can find a detailed working example with a downloadable sample Tableau workbook
-and an accompanying Jupyter workbook that walks through model fitting, evaluation
-and publishing steps on
-[our blog](https://www.tableau.com/about/blog/2017/1/building-advanced-analytics-applications-tabpy-64916).
-
-The endpoints that are no longer needed can be removed the following way:
-
-```python
-
-client.remove('WillItDefault')
-
-```
-
-## Predeployed Functions
-
-### Deploying Models Shipped With TabPy
-
-To deploy models shipped with TabPy follow the
-[TabPy Installation Instructions](server-install.md) and then
-[TabPy Server Configuration Instructions](server-config.md).
-Once your server is running execute the following command:
-
-```sh
-tabpy-deploy-models
-```
-
-If your server is running using a custom config specify the config
-in the command line:
-
-```sh
-tabpy-deploy-models custom.conf
-```
-
-The command will deploy all of the prebuilt models.
-For every successfully deployed model a message will be printed to the console:
-
-```sh
-"Successfully deployed PCA"
-```
-
-Use code in [`tabpy/models/scripts`](../tabpy/models/scripts)
-as an example of how to create a model and
-[`tabpy/models/deploy_models.py`](../tabpy/models/deploy_models.py)
-as an example for how to deploy a model. Before executing delpoyment script
-install all the required dependencies with `pip`.
-
-You can deploy models individually by navigating to
-[`tabpy/models/scripts`](../tabpy/models/scripts) and running
-each file in isolation like so:
-
-```sh
-
-python PCA.py
-
-```
-
-Similarly to the setup script, if your server is running using a custom config,
-you can specify the config's file path through the command line.
-
-### Principal Component Analysis (PCA)
-
-[Principal component analysis](https://en.wikipedia.org/wiki/Principal_component_analysis)
-is a statistical technique which extracts new, linearly uncorrelated,
-variables out of a dataset which capture the maximum variance in the
-data. In this way, `PCA` can be used to reduce the number of variables
-in a high dimensional dataset, a process that is called dimensionality
-reduction. The first principal component captures the largest amount of
-variance, while the second captures the largest portion of the remaining
-variance while remaining orthogonal to the first and so on. This allows the
-reduction of the number of dimensions while maintaining as much of the
-information from the original data as possible. `PCA` is useful in
-exploratory data analysis because complex linear relationships can be
-visualized in a 2D scatter plot of the first few principal components.
-
-TabPy’s implementation of `PCA` uses the scikit-learn
-[decomposition.PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)
-algorithm, which is further documented [here](https://scikit-learn.org/stable/modules/decomposition.html#pca).
-In the Tableau script, after the function name `PCA`, you must specify a
-principal component to return. This integer input should be > 0 and <= the
-number of variables you pass in to the function. When passing categorical
-variables we perform the `scikit-learn` [One Hot Encoding](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.OneHotEncoder.html)
-to transform your non-numeric variables into a one-hot numeric array of 0s and
-1s. In order for `One Hot Encoding` to be performant we have limited the number
-of unique values your categorical column may contain to 25 and do not permit
-any nulls or empty strings in the column. In Tableau's implementation of `PCA`
-is performed, all variables are normalized to have a mean of 0 and unit
-variance using the `scikit-learn` [StandardScaler](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html).
-
-A Tableau calculated field to perform PCA will look like:
-
-```python
-
-tabpy.query(‘PCA’, 1, _arg1, _arg2, _arg3)[‘response’]
-
-```
-
-### Sentiment Analysis
-
-[Sentiment analysis](https://en.wikipedia.org/wiki/Sentiment_analysis) is
-a technique which uses natural language processing to extract the emotional
-positivity or negativity – the sentiment – behind a piece of text and converts
-that into a numeric value. Our implementation of `sentiment analysis` returns a
-polarity score between -1 and 1 which rates the positivity of the string with
-1 being very positive and -1 being very negative. Calling the `Sentiment
-Analysis` function from TabPy in Tableau will look like the following,
-where \_arg1 is a Tableau dimension containing text
-
-```python
-
-tabpy.query('Sentiment Analysis', _arg1)[‘response’]
-
-```
-
-Python provides multiple packages that compute `sentiment analysis` – our implementation
-defaults to use [NLTK’s sentiment package](https://www.nltk.org/api/nltk.sentiment.html).
-If you would like to use [TextBlob’s sentiment analysis](https://textblob.readthedocs.io/en/dev/quickstart.html)
-algorithm you can do so by specifying the optional argument “library=textblob”
-when calling the `Sentiment Analysis` function through a calculated field in
-Tableau
-
-```python
-
-tabpy.query('Sentiment Analysis', _arg1, library='textblob')[‘response’]
-
-```
-
-### T-Test
-
-A [t-test](https://en.wikipedia.org/wiki/Student%27s_t-test) is a statistical
-hypothesis test that is used to compare two sample means or a sample’s mean against
-a known population mean. The ttest should be used when the means of the samples
-follows a normal distribution but the variance may not be known.
-
-TabPy’s pre-deployed t-test implementation can be called using the following syntax,
-
-```python
-
-tabpy.query(‘ttest’, _arg1, _arg2)[‘response’]
-
-```
-
-and is capable of performing two types of t-tests:
-
-1. [A t-test for the means of two independent samples with equal variance](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.ttest_ind.html)
-   This is a two-sided t test with the null hypothesis being that the mean of
-   sample1 is equal to the mean of sample2:
-
-   - `_arg1` (list of numeric values): a list of independent observations.
-   - `_arg2` (list of numeric values): a list of independent observations equal to
-     the length of `_arg1`.
-
-   Alternatively, your data may not be split into separate measures. If that is
-   the case you can pass the following fields to ttest:
-
-   - `_arg1` (list of numeric values): a list of independent observations
-   - `_arg2` (list of categorical variables with cardinality two): a binary factor
-     that maps each observation in `_arg1` to either sample1 or sample2 (this list
-     should be equal to the length of `_arg1`).
-
-2. [A t-test for the mean of one group](https://docs.scipy.org/doc/scipy-0.14.0/reference/generated/scipy.stats.ttest_1samp.html):
-   - `_arg1` (list of numeric values): a list of independent observations.
-   - `_arg2` (a numeric value): the known population mean
-     A two-sided t test with the null hypothesis being that the mean of a sample
-     of independent observations is equal to the given population mean.
-
-   The function returns a two-tailed [p-value](https://en.wikipedia.org/wiki/P-value)
-   (between 0 and 1). Depending on your [significance level](https://en.wikipedia.org/wiki/Statistical_significance)
-   you may reject or fail to reject the null hypothesis.
-
-### ANOVA
-
-[Analysis of variance](https://en.wikipedia.org/wiki/Analysis_of_variance)
-helps inform if two or more group means within a sample differ. By measuring
-the variation between and among groups and computing the resulting F-statistic
-we are able to obtain a p-value. While a statistically significant p-value
-will inform you that at least 2 of your groups’ means are different from each
-other, it will not tell you which of the two groups differ.
-
-You can call ANOVA from tableau in the following way,
-
-```python
-
-tabpy.query(‘anova’, _arg1, _arg2, _arg3)[‘response’]
-```
-
-## Providing Schema Metadata
-
-As soon as you share your deployed functions, you also need to share metadata
-about the function. The consumer of an endpoint needs to know the details of how
-to use the endpoint, such as:
-
-- The general purpose of the endpoint
-- Input parameter names, data types, and their meaning
-- Return data type and description
-
-This data goes beyond the single string that we used above when deploying the
-function `add`. You can use an optional parameter to `deploy` to provide such
-a structured description, which can then be retrieved by other users connected
-to the same server. The schema is interpreted as a [Json Schema](<http://json-schema.org/documentation.html>)
-object, which you can either manually create or generate using a utility
-method provided in this tools package:
-
-```python
-
-from tabpy.tabpy_tools.schema import generate_schema
-
-schema = generate_schema(
-  input={'x': 3, 'y': 2},
-  output=5,
-  input_description={'x': 'first value',
-                     'y': 'second value'},
-  output_description='the sum of x and y')
-
-  client.deploy('add', add, 'Adds two numbers x and y', schema=schema)
-
-```
-
-To describe more complex input, like arrays, you would use the following syntax:
-
-```python
-
-from tabpy.tabpy_tools.schema import generate_schema
-
-schema = generate_schema(
-  input={'x': [6.35, 6.40, 6.65, 8.60],
-         'y': [1.95, 1.95, 2.05, 3.05]},
-  output=[0, 0, 0, 1],
-  input_description={'x': 'list of x values',
-                     'y': 'list of y values'},
-  output_description='cluster Ids for each point x, y')
-
-  client.deploy('clustering',
-      clustering,
-      'Returns cluster Ids for each data point specified by the pairs in x and y',
-      schema=schema)
-
-```
-
-A schema described as such can be retrieved through the [REST Endpoints API](server-rest.md#httpget-endpoints)
-or through the `get_endpoints` client API as follows:
-
-```python
-
-client.get_endpoints()['add']['schema']
-
-```
-
-## Querying an Endpoint
-
-Once a Python function has been deployed to the server process, you can use the
-client's `query` method to query it (assuming that you’re already connected to the
-service):
-
-```python
-
-x = [6.35, 6.40, 6.65, 8.60, 8.90, 9.00, 9.10]
-y = [1.95, 1.95, 2.05, 3.05, 3.05, 3.10, 3.15]
-
-client.query('clustering', x, y)
-
-```
-
-Response:
-
-```json
-{
-  "model": "clustering",
-  "response": [0, 0, 0, 1, 1, 1, 1],
-  "uuid": "1ca01e46-733c-4a77-b3da-3ded84dff4cd",
-  "version": 2
-}
-
-```
-
-## Evaluating Arbitrary Python Scripts
-
-The other core functionality aside from deploying and querying methods as endpoints
-is the ad-hoc execution of Python code, called `evaluate`. Evaluate does not
-have a Python API in `tabpy-tools`, only a raw [REST interface](server-rest.md)
-that other client bindings can easily implement. Tableau connects to TabPy
-using REST `Evaluate`.
-
-`evaluate` allows calling a deployed endpoint from within the Python code block.
-The convention for this is to use a provided function call `tabpy.query` in the
-code, which behaves like the `query` method in `tabpy-tools`. See the
-[REST API documentation](server-rest.md) for an example.
-
-## Deploying Models in TabPy Docker Container
-
-To deploy custom models for TabPy running in docker container, first copy all
-python model files onto host machine.
-
-For example, `myFunction.py` is the model we want to deploy.
-Run following from the folder containing `myFunction.py` on host machine
-
-```console
-docker cp myFunction.py <container_id>:/app/scripts/myFunction.py
-docker exec -it <container_id> python /app/scripts/myFunction.py
-```
+# TabPy Tools
+
+TabPy tools is the Python package of tools for managing the published Python functions
+on TabPy server.
+
+<!-- markdownlint-disable MD004 -->
+
+<!-- toc -->
+
+- [Connecting to TabPy](#connecting-to-tabpy)
+- [Authentication](#authentication)
+- [Deploying a Function](#deploying-a-function)
+- [Predeployed Functions](#predeployed-functions)
+  * [Principal Component Analysis (PCA)](#principal-component-analysis-pca)
+  * [Sentiment Analysis](#sentiment-analysis)
+  * [T-Test](#t-test)
+  * [ANOVA](#anova)
+- [Providing Schema Metadata](#providing-schema-metadata)
+- [Querying an Endpoint](#querying-an-endpoint)
+- [Evaluating Arbitrary Python Scripts](#evaluating-arbitrary-python-scripts)
+- [Deploying Models in TabPy Docker Container](#deploying-models-in-tabpy-docker-container)
+
+<!-- tocstop -->
+
+<!-- markdownlint-enable MD004 -->
+
+## Connecting to TabPy
+
+The tools library uses the notion of connecting to a service to avoid having
+to specify the service location for all subsequent operations:
+
+```python
+
+from tabpy.tabpy_tools.client import Client
+
+client = Client('http://localhost:9004/')
+
+```
+
+The URL and port are where the Tableau-Python-Server process has been started -
+more info can be found in the
+[Starting TabPy](server-install.md#starting-tabpy) section of the documentation.
+
+## Authentication
+
+When TabPy is configured with the authentication feature on, client code
+has to specify the credentials to use during model deployment with the
+`set_credentials` call for a client:
+
+```python
+client.set_credentials('username', 'P@ssw0rd')
+```
+
+Credentials only need to be set once for all further client operations.
+
+In cases where credentials are not provided but are required, the deployment will
+fail with an "Unauthorized" code (401).
+
+For instructions on how to configure and enable the authentication feature for
+TabPy, see [TabPy Server Configuration Instructions](server-config.md).
+
+## Deploying a Function
+
+A persisted endpoint is backed by a Python method. For example:
+
+```python
+def add(x,y):
+    import numpy as np
+    return np.add(x, y).tolist()
+
+client.deploy('add', add, 'Adds two numbers x and y')
+```
+
+The next example is more complex, using scikit-learn's clustering API:
+
+```python
+
+def clustering(x, y):
+    import numpy as np
+    from sklearn.cluster import DBSCAN
+    from sklearn.preprocessing import StandardScaler
+    X = np.column_stack([x, y])
+    X = StandardScaler().fit_transform(X)
+    db = DBSCAN(eps=1, min_samples=3).fit(X)
+    return db.labels_.tolist()
+
+
+client.deploy('clustering',
+              clustering,
+              'Returns cluster Ids for each data point specified by the '
+              'pairs in x and y')
+
+```
+
+In this example the function `clustering` expects a set of two-dimensional
+data points, represented by the list of all x-coordinates and the list of all
+y-coordinates. It will return a set of numerical labels corresponding to the
+clusters to which each datapoint is assigned. We deploy this function as an
+endpoint named `clustering`.
+It is now reachable as a [REST API](server-rest.md#httppost-queryendpoint), as
+well as through the TabPy tools - for details see the next section.
+
+You can re-deploy a function (for example, after you modified its code) by setting
+the `override` parameter to `True`:
+
+```python
+client.deploy('add', add, 'Adds two numbers x and y', override=True)
+```
+
+Each re-deployment of an endpoint will increment its version number, which is also
+returned as part of the query result.
+
+When deploying endpoints which rely on supervised learning models, you may want to
+load a saved model instead of training on-the-fly for performance reasons.
+
+Below is an excerpt from the training stage of a hypothetical model that predicts
+whether or not a loan will default:
+
+```python
+
+from sklearn.ensemble import GradientBoostingClassifier
+
+predictors = [x for x in train.columns if x not in [target, RowID]]
+gbm = GradientBoostingClassifier(learning_rate=0.01, n_estimators=600,max_depth=9,
+min_samples_split=1200, min_samples_leaf=60, subsample=0.85, random_state=10)
+modelfit(gbm, train, test, predictors)
+
+```
+
+When the trained model (named `gbm` in this case) is used in a function being
+deployed (as in `gbm.predict(...)` below), Tableau will automatically save its
+definition using `cloudpickle` along with the definition of the function. The model
+will also be kept in memory on the server in order to achieve faster response times.
+If you persist your model manually to disk and read as part of your scoring function
+code however, you will notice that the response times are noticeably longer - as
+every time a client hits an endpoint, the code (including model loading) will get
+executed. In order to get the best performance, we recommended following the
+methodology outlined in this example.
+
+```python
+def LoanDefaultClassifier(Loan_Amount, Loan_Tenure, Monthly_Income, Age):
+    import pandas as pd
+    data=pd.concat([Loan_Amount,Loan_Tenure,Monthly_Income,Age],axis=1)
+    return gbm.predict(data)
+
+client.deploy('WillItDefault',
+              LoanDefaultClassifier,
+              'Returns whether a loan application is likely to default.')
+```
+
+You can find a detailed working example with a downloadable sample Tableau workbook
+and an accompanying Jupyter workbook that walks through model fitting, evaluation
+and publishing steps on
+[our blog](https://www.tableau.com/about/blog/2017/1/building-advanced-analytics-applications-tabpy-64916).
+
+The endpoints that are no longer needed can be removed the following way:
+
+```python
+
+client.remove('WillItDefault')
+
+```
+
+## Predeployed Functions
+
+### Deploying Models Shipped With TabPy
+
+To deploy models shipped with TabPy follow the
+[TabPy Installation Instructions](server-install.md) and then
+[TabPy Server Configuration Instructions](server-config.md).
+Once your server is running execute the following command:
+
+```sh
+tabpy-deploy-models
+```
+
+If your server is running using a custom config specify the config
+in the command line:
+
+```sh
+tabpy-deploy-models custom.conf
+```
+
+The command will deploy all of the prebuilt models.
+For every successfully deployed model a message will be printed to the console:
+
+```sh
+"Successfully deployed PCA"
+```
+
+Use code in [`tabpy/models/scripts`](../tabpy/models/scripts)
+as an example of how to create a model and
+[`tabpy/models/deploy_models.py`](../tabpy/models/deploy_models.py)
+as an example for how to deploy a model. Before executing delpoyment script
+install all the required dependencies with `pip`.
+
+You can deploy models individually by navigating to
+[`tabpy/models/scripts`](../tabpy/models/scripts) and running
+each file in isolation like so:
+
+```sh
+
+python PCA.py
+
+```
+
+Similarly to the setup script, if your server is running using a custom config,
+you can specify the config's file path through the command line.
+
+### Principal Component Analysis (PCA)
+
+[Principal component analysis](https://en.wikipedia.org/wiki/Principal_component_analysis)
+is a statistical technique which extracts new, linearly uncorrelated,
+variables out of a dataset which capture the maximum variance in the
+data. In this way, `PCA` can be used to reduce the number of variables
+in a high dimensional dataset, a process that is called dimensionality
+reduction. The first principal component captures the largest amount of
+variance, while the second captures the largest portion of the remaining
+variance while remaining orthogonal to the first and so on. This allows the
+reduction of the number of dimensions while maintaining as much of the
+information from the original data as possible. `PCA` is useful in
+exploratory data analysis because complex linear relationships can be
+visualized in a 2D scatter plot of the first few principal components.
+
+TabPy’s implementation of `PCA` uses the scikit-learn
+[decomposition.PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)
+algorithm, which is further documented [here](https://scikit-learn.org/stable/modules/decomposition.html#pca).
+In the Tableau script, after the function name `PCA`, you must specify a
+principal component to return. This integer input should be > 0 and <= the
+number of variables you pass in to the function. When passing categorical
+variables we perform the `scikit-learn` [One Hot Encoding](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.OneHotEncoder.html)
+to transform your non-numeric variables into a one-hot numeric array of 0s and
+1s. In order for `One Hot Encoding` to be performant we have limited the number
+of unique values your categorical column may contain to 25 and do not permit
+any nulls or empty strings in the column. In Tableau's implementation of `PCA`
+is performed, all variables are normalized to have a mean of 0 and unit
+variance using the `scikit-learn` [StandardScaler](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html).
+
+A Tableau calculated field to perform PCA will look like:
+
+```python
+
+tabpy.query(‘PCA’, 1, _arg1, _arg2, _arg3)[‘response’]
+
+```
+
+### Sentiment Analysis
+
+[Sentiment analysis](https://en.wikipedia.org/wiki/Sentiment_analysis) is
+a technique which uses natural language processing to extract the emotional
+positivity or negativity – the sentiment – behind a piece of text and converts
+that into a numeric value. Our implementation of `sentiment analysis` returns a
+polarity score between -1 and 1 which rates the positivity of the string with
+1 being very positive and -1 being very negative. Calling the `Sentiment
+Analysis` function from TabPy in Tableau will look like the following,
+where \_arg1 is a Tableau dimension containing text
+
+```python
+
+tabpy.query('Sentiment Analysis', _arg1)[‘response’]
+
+```
+
+Python provides multiple packages that compute `sentiment analysis` – our implementation
+defaults to use [NLTK’s sentiment package](https://www.nltk.org/api/nltk.sentiment.html).
+If you would like to use [TextBlob’s sentiment analysis](https://textblob.readthedocs.io/en/dev/quickstart.html)
+algorithm you can do so by specifying the optional argument “library=textblob”
+when calling the `Sentiment Analysis` function through a calculated field in
+Tableau
+
+```python
+
+tabpy.query('Sentiment Analysis', _arg1, library='textblob')[‘response’]
+
+```
+
+### T-Test
+
+A [t-test](https://en.wikipedia.org/wiki/Student%27s_t-test) is a statistical
+hypothesis test that is used to compare two sample means or a sample’s mean against
+a known population mean. The ttest should be used when the means of the samples
+follows a normal distribution but the variance may not be known.
+
+TabPy’s pre-deployed t-test implementation can be called using the following syntax,
+
+```python
+
+tabpy.query(‘ttest’, _arg1, _arg2)[‘response’]
+
+```
+
+and is capable of performing two types of t-tests:
+
+1. [A t-test for the means of two independent samples with equal variance](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.ttest_ind.html)
+   This is a two-sided t test with the null hypothesis being that the mean of
+   sample1 is equal to the mean of sample2:
+
+   - `_arg1` (list of numeric values): a list of independent observations.
+   - `_arg2` (list of numeric values): a list of independent observations equal to
+     the length of `_arg1`.
+
+   Alternatively, your data may not be split into separate measures. If that is
+   the case you can pass the following fields to ttest:
+
+   - `_arg1` (list of numeric values): a list of independent observations
+   - `_arg2` (list of categorical variables with cardinality two): a binary factor
+     that maps each observation in `_arg1` to either sample1 or sample2 (this list
+     should be equal to the length of `_arg1`).
+
+2. [A t-test for the mean of one group](https://docs.scipy.org/doc/scipy-0.14.0/reference/generated/scipy.stats.ttest_1samp.html):
+   - `_arg1` (list of numeric values): a list of independent observations.
+   - `_arg2` (a numeric value): the known population mean
+     A two-sided t test with the null hypothesis being that the mean of a sample
+     of independent observations is equal to the given population mean.
+
+   The function returns a two-tailed [p-value](https://en.wikipedia.org/wiki/P-value)
+   (between 0 and 1). Depending on your [significance level](https://en.wikipedia.org/wiki/Statistical_significance)
+   you may reject or fail to reject the null hypothesis.
+
+### ANOVA
+
+[Analysis of variance](https://en.wikipedia.org/wiki/Analysis_of_variance)
+helps inform if two or more group means within a sample differ. By measuring
+the variation between and among groups and computing the resulting F-statistic
+we are able to obtain a p-value. While a statistically significant p-value
+will inform you that at least 2 of your groups’ means are different from each
+other, it will not tell you which of the two groups differ.
+
+You can call ANOVA from tableau in the following way,
+
+```python
+
+tabpy.query(‘anova’, _arg1, _arg2, _arg3)[‘response’]
+```
+
+## Providing Schema Metadata
+
+As soon as you share your deployed functions, you also need to share metadata
+about the function. The consumer of an endpoint needs to know the details of how
+to use the endpoint, such as:
+
+- The general purpose of the endpoint
+- Input parameter names, data types, and their meaning
+- Return data type and description
+
+This data goes beyond the single string that we used above when deploying the
+function `add`. You can use an optional parameter to `deploy` to provide such
+a structured description, which can then be retrieved by other users connected
+to the same server. The schema is interpreted as a [Json Schema](<http://json-schema.org/documentation.html>)
+object, which you can either manually create or generate using a utility
+method provided in this tools package:
+
+```python
+
+from tabpy.tabpy_tools.schema import generate_schema
+
+schema = generate_schema(
+  input={'x': 3, 'y': 2},
+  output=5,
+  input_description={'x': 'first value',
+                     'y': 'second value'},
+  output_description='the sum of x and y')
+
+  client.deploy('add', add, 'Adds two numbers x and y', schema=schema)
+
+```
+
+To describe more complex input, like arrays, you would use the following syntax:
+
+```python
+
+from tabpy.tabpy_tools.schema import generate_schema
+
+schema = generate_schema(
+  input={'x': [6.35, 6.40, 6.65, 8.60],
+         'y': [1.95, 1.95, 2.05, 3.05]},
+  output=[0, 0, 0, 1],
+  input_description={'x': 'list of x values',
+                     'y': 'list of y values'},
+  output_description='cluster Ids for each point x, y')
+
+  client.deploy('clustering',
+      clustering,
+      'Returns cluster Ids for each data point specified by the pairs in x and y',
+      schema=schema)
+
+```
+
+A schema described as such can be retrieved through the [REST Endpoints API](server-rest.md#httpget-endpoints)
+or through the `get_endpoints` client API as follows:
+
+```python
+
+client.get_endpoints()['add']['schema']
+
+```
+
+## Querying an Endpoint
+
+Once a Python function has been deployed to the server process, you can use the
+client's `query` method to query it (assuming that you’re already connected to the
+service):
+
+```python
+
+x = [6.35, 6.40, 6.65, 8.60, 8.90, 9.00, 9.10]
+y = [1.95, 1.95, 2.05, 3.05, 3.05, 3.10, 3.15]
+
+client.query('clustering', x, y)
+
+```
+
+Response:
+
+```json
+{
+  "model": "clustering",
+  "response": [0, 0, 0, 1, 1, 1, 1],
+  "uuid": "1ca01e46-733c-4a77-b3da-3ded84dff4cd",
+  "version": 2
+}
+
+```
+
+## Evaluating Arbitrary Python Scripts
+
+The other core functionality aside from deploying and querying methods as endpoints
+is the ad-hoc execution of Python code, called `evaluate`. Evaluate does not
+have a Python API in `tabpy-tools`, only a raw [REST interface](server-rest.md)
+that other client bindings can easily implement. Tableau connects to TabPy
+using REST `Evaluate`.
+
+`evaluate` allows calling a deployed endpoint from within the Python code block.
+The convention for this is to use a provided function call `tabpy.query` in the
+code, which behaves like the `query` method in `tabpy-tools`. See the
+[REST API documentation](server-rest.md) for an example.
+
+## Deploying Models in TabPy Docker Container
+
+To deploy custom models for TabPy running in docker container, first copy all
+python model files onto host machine.
+
+For example, `myFunction.py` is the model we want to deploy.
+Run following from the folder containing `myFunction.py` on host machine
+
+```console
+docker cp myFunction.py <container_id>:/app/scripts/myFunction.py
+docker exec -it <container_id> python /app/scripts/myFunction.py
+```
```

### Comparing `tabpy-2.6.0/docs/tabpy-virtualenv.md` & `tabpy-2.7.0/docs/tabpy-virtualenv.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/misc/TabPy.postman_collection.json` & `tabpy-2.7.0/misc/TabPy.postman_collection.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 24% similar despite different names*

```diff
@@ -1,223 +1,235 @@
-00000000: 7b0a 0922 696e 666f 223a 207b 0a09 0922  {.."info": {..."
-00000010: 5f70 6f73 746d 616e 5f69 6422 3a20 2261  _postman_id": "a
-00000020: 6464 3062 3833 622d 3363 3131 2d34 6338  dd0b83b-3c11-4c8
-00000030: 302d 3937 3361 2d30 6135 6662 6638 3033  0-973a-0a5fbf803
-00000040: 6535 3822 2c0a 0909 226e 616d 6522 3a20  e58",..."name": 
-00000050: 2254 6162 5079 222c 0a09 0922 7363 6865  "TabPy",..."sche
-00000060: 6d61 223a 2022 6874 7470 733a 2f2f 7363  ma": "https://sc
-00000070: 6865 6d61 2e67 6574 706f 7374 6d61 6e2e  hema.getpostman.
-00000080: 636f 6d2f 6a73 6f6e 2f63 6f6c 6c65 6374  com/json/collect
-00000090: 696f 6e2f 7632 2e31 2e30 2f63 6f6c 6c65  ion/v2.1.0/colle
-000000a0: 6374 696f 6e2e 6a73 6f6e 220a 097d 2c0a  ction.json"..},.
-000000b0: 0922 6974 656d 223a 205b 0a09 097b 0a09  ."item": [...{..
-000000c0: 0909 226e 616d 6522 3a20 227b 7b68 6f73  .."name": "{{hos
-000000d0: 747d 7d3a 7b7b 706f 7274 7d7d 2f69 6e66  t}}:{{port}}/inf
-000000e0: 6f22 2c0a 0909 0922 7265 7175 6573 7422  o",...."request"
-000000f0: 3a20 7b0a 0909 0909 226d 6574 686f 6422  : {....."method"
-00000100: 3a20 2247 4554 222c 0a09 0909 0922 6865  : "GET",....."he
-00000110: 6164 6572 223a 205b 5d2c 0a09 0909 0922  ader": [],....."
-00000120: 7572 6c22 3a20 7b0a 0909 0909 0922 7261  url": {......"ra
-00000130: 7722 3a20 227b 7b68 6f73 747d 7d3a 7b7b  w": "{{host}}:{{
-00000140: 706f 7274 7d7d 2f69 6e66 6f22 2c0a 0909  port}}/info",...
-00000150: 0909 0922 686f 7374 223a 205b 0a09 0909  ..."host": [....
-00000160: 0909 0922 7b7b 686f 7374 7d7d 220a 0909  ..."{{host}}"...
-00000170: 0909 095d 2c0a 0909 0909 0922 706f 7274  ...],......"port
-00000180: 223a 2022 7b7b 706f 7274 7d7d 222c 0a09  ": "{{port}}",..
-00000190: 0909 0909 2270 6174 6822 3a20 5b0a 0909  ...."path": [...
-000001a0: 0909 0909 2269 6e66 6f22 0a09 0909 0909  ...."info"......
-000001b0: 5d0a 0909 0909 7d0a 0909 097d 2c0a 0909  ].....}....},...
-000001c0: 0922 7265 7370 6f6e 7365 223a 205b 5d0a  ."response": [].
-000001d0: 0909 7d2c 0a09 097b 0a09 0909 226e 616d  ..},...{...."nam
-000001e0: 6522 3a20 227b 7b68 6f73 747d 7d3a 7b7b  e": "{{host}}:{{
-000001f0: 706f 7274 7d7d 2f65 7661 6c75 6174 6522  port}}/evaluate"
-00000200: 2c0a 0909 0922 7265 7175 6573 7422 3a20  ,...."request": 
-00000210: 7b0a 0909 0909 2261 7574 6822 3a20 7b0a  {....."auth": {.
-00000220: 0909 0909 0922 7479 7065 223a 2022 6261  ....."type": "ba
-00000230: 7369 6322 2c0a 0909 0909 0922 6261 7369  sic",......"basi
-00000240: 6322 3a20 5b0a 0909 0909 0909 7b0a 0909  c": [.......{...
-00000250: 0909 0909 0922 6b65 7922 3a20 2270 6173  ....."key": "pas
-00000260: 7377 6f72 6422 2c0a 0909 0909 0909 0922  sword",........"
-00000270: 7661 6c75 6522 3a20 2250 4073 7377 3072  value": "P@ssw0r
-00000280: 6422 2c0a 0909 0909 0909 0922 7479 7065  d",........"type
-00000290: 223a 2022 7374 7269 6e67 220a 0909 0909  ": "string".....
-000002a0: 0909 7d2c 0a09 0909 0909 097b 0a09 0909  ..},.......{....
-000002b0: 0909 0909 226b 6579 223a 2022 7573 6572  ...."key": "user
-000002c0: 6e61 6d65 222c 0a09 0909 0909 0909 2276  name",........"v
-000002d0: 616c 7565 223a 2022 7573 6572 3122 2c0a  alue": "user1",.
-000002e0: 0909 0909 0909 0922 7479 7065 223a 2022  ......."type": "
-000002f0: 7374 7269 6e67 220a 0909 0909 0909 7d0a  string".......}.
-00000300: 0909 0909 095d 0a09 0909 097d 2c0a 0909  .....].....},...
-00000310: 0909 226d 6574 686f 6422 3a20 2250 4f53  .."method": "POS
-00000320: 5422 2c0a 0909 0909 2268 6561 6465 7222  T",....."header"
-00000330: 3a20 5b0a 0909 0909 097b 0a09 0909 0909  : [......{......
-00000340: 0922 6b65 7922 3a20 2243 6f6e 7465 6e74  ."key": "Content
-00000350: 2d54 7970 6522 2c0a 0909 0909 0909 226e  -Type",......."n
-00000360: 616d 6522 3a20 2243 6f6e 7465 6e74 2d54  ame": "Content-T
-00000370: 7970 6522 2c0a 0909 0909 0909 2276 616c  ype",......."val
-00000380: 7565 223a 2022 6170 706c 6963 6174 696f  ue": "applicatio
-00000390: 6e2f 6a73 6f6e 222c 0a09 0909 0909 0922  n/json",......."
-000003a0: 7479 7065 223a 2022 7465 7874 220a 0909  type": "text"...
-000003b0: 0909 097d 2c0a 0909 0909 097b 0a09 0909  ...},......{....
-000003c0: 0909 0922 6b65 7922 3a20 2254 6162 5079  ..."key": "TabPy
-000003d0: 2d43 6c69 656e 7422 2c0a 0909 0909 0909  -Client",.......
-000003e0: 2276 616c 7565 223a 2022 506f 7374 6d61  "value": "Postma
-000003f0: 6e20 666f 7220 6d61 6e75 616c 2074 6573  n for manual tes
-00000400: 7469 6e67 222c 0a09 0909 0909 0922 7479  ting",......."ty
-00000410: 7065 223a 2022 7465 7874 220a 0909 0909  pe": "text".....
-00000420: 097d 2c0a 0909 0909 097b 0a09 0909 0909  .},......{......
-00000430: 0922 6b65 7922 3a20 2254 6162 5079 2d55  ."key": "TabPy-U
-00000440: 7365 7222 2c0a 0909 0909 0909 2276 616c  ser",......."val
-00000450: 7565 223a 2022 6f67 6f6c 6f76 6174 7969  ue": "ogolovatyi
-00000460: 222c 0a09 0909 0909 0922 7479 7065 223a  ",......."type":
-00000470: 2022 7465 7874 220a 0909 0909 097d 0a09   "text"......}..
-00000480: 0909 095d 2c0a 0909 0909 2262 6f64 7922  ...],....."body"
-00000490: 3a20 7b0a 0909 0909 0922 6d6f 6465 223a  : {......"mode":
-000004a0: 2022 7261 7722 2c0a 0909 0909 0922 7261   "raw",......"ra
-000004b0: 7722 3a20 227b 5c6e 5c74 5c22 6461 7461  w": "{\n\t\"data
-000004c0: 5c22 3a20 5c6e 5c74 7b20 5c6e 5c74 5c74  \": \n\t{ \n\t\t
-000004d0: 5c22 5f61 7267 315c 2220 3a20 5b31 2c20  \"_arg1\" : [1, 
-000004e0: 322c 2033 5d2c 205c 6e5c 745c 745c 225f  2, 3], \n\t\t\"_
-000004f0: 6172 6732 5c22 203a 205b 332c 202d 312c  arg2\" : [3, -1,
-00000500: 2035 5d5c 6e5c 747d 2c5c 6e5c 745c 2273   5]\n\t},\n\t\"s
-00000510: 6372 6970 745c 223a 205c 6e5c 745c 2272  cript\": \n\t\"r
-00000520: 6574 7572 6e20 5b78 202b 2079 2066 6f72  eturn [x + y for
-00000530: 2078 2c20 7920 696e 207a 6970 285f 6172   x, y in zip(_ar
-00000540: 6731 2c20 5f61 7267 3229 5d5c 225c 6e7d  g1, _arg2)]\"\n}
-00000550: 5c6e 222c 0a09 0909 0909 226f 7074 696f  \n",......"optio
-00000560: 6e73 223a 207b 0a09 0909 0909 0922 7261  ns": {......."ra
-00000570: 7722 3a20 7b7d 0a09 0909 0909 7d0a 0909  w": {}......}...
-00000580: 0909 7d2c 0a09 0909 0922 7572 6c22 3a20  ..},....."url": 
-00000590: 7b0a 0909 0909 0922 7261 7722 3a20 227b  {......"raw": "{
-000005a0: 7b68 6f73 747d 7d3a 7b7b 706f 7274 7d7d  {host}}:{{port}}
-000005b0: 2f65 7661 6c75 6174 6522 2c0a 0909 0909  /evaluate",.....
-000005c0: 0922 686f 7374 223a 205b 0a09 0909 0909  ."host": [......
-000005d0: 0922 7b7b 686f 7374 7d7d 220a 0909 0909  ."{{host}}".....
-000005e0: 095d 2c0a 0909 0909 0922 706f 7274 223a  .],......"port":
-000005f0: 2022 7b7b 706f 7274 7d7d 222c 0a09 0909   "{{port}}",....
-00000600: 0909 2270 6174 6822 3a20 5b0a 0909 0909  .."path": [.....
-00000610: 0909 2265 7661 6c75 6174 6522 0a09 0909  .."evaluate"....
-00000620: 0909 5d2c 0a09 0909 0909 2271 7565 7279  ..],......"query
-00000630: 223a 205b 0a09 0909 0909 097b 0a09 0909  ": [.......{....
-00000640: 0909 0909 226b 6579 223a 2022 5461 6250  ...."key": "TabP
-00000650: 792d 436c 6965 6e74 222c 0a09 0909 0909  y-Client",......
-00000660: 0909 2276 616c 7565 223a 2022 506f 7374  .."value": "Post
-00000670: 6d61 6e20 666f 7220 4d61 6e75 616c 2054  man for Manual T
-00000680: 6573 7469 6e67 222c 0a09 0909 0909 0909  esting",........
-00000690: 2264 6973 6162 6c65 6422 3a20 7472 7565  "disabled": true
-000006a0: 0a09 0909 0909 097d 2c0a 0909 0909 0909  .......},.......
-000006b0: 7b0a 0909 0909 0909 0922 6b65 7922 3a20  {........"key": 
-000006c0: 2254 6162 5079 2d55 7365 7222 2c0a 0909  "TabPy-User",...
-000006d0: 0909 0909 0922 7661 6c75 6522 3a20 226f  ....."value": "o
-000006e0: 676f 6c6f 7661 7479 6922 2c0a 0909 0909  golovatyi",.....
-000006f0: 0909 0922 6469 7361 626c 6564 223a 2074  ..."disabled": t
-00000700: 7275 650a 0909 0909 0909 7d0a 0909 0909  rue.......}.....
-00000710: 095d 0a09 0909 097d 0a09 0909 7d2c 0a09  .].....}....},..
-00000720: 0909 2272 6573 706f 6e73 6522 3a20 5b5d  .."response": []
-00000730: 0a09 097d 2c0a 0909 7b0a 0909 0922 6e61  ...},...{...."na
-00000740: 6d65 223a 2022 7b7b 656e 6470 6f69 6e74  me": "{{endpoint
-00000750: 7d7d 2f73 7461 7475 7322 2c0a 0909 0922  }}/status",...."
-00000760: 7265 7175 6573 7422 3a20 7b0a 0909 0909  request": {.....
-00000770: 226d 6574 686f 6422 3a20 2247 4554 222c  "method": "GET",
-00000780: 0a09 0909 0922 6865 6164 6572 223a 205b  ....."header": [
-00000790: 5d2c 0a09 0909 0922 7572 6c22 3a20 7b0a  ],....."url": {.
-000007a0: 0909 0909 0922 7261 7722 3a20 227b 7b68  ....."raw": "{{h
-000007b0: 6f73 747d 7d3a 7b7b 706f 7274 7d7d 2f73  ost}}:{{port}}/s
-000007c0: 7461 7475 7322 2c0a 0909 0909 0922 686f  tatus",......"ho
-000007d0: 7374 223a 205b 0a09 0909 0909 0922 7b7b  st": [......."{{
-000007e0: 686f 7374 7d7d 220a 0909 0909 095d 2c0a  host}}"......],.
-000007f0: 0909 0909 0922 706f 7274 223a 2022 7b7b  ....."port": "{{
-00000800: 706f 7274 7d7d 222c 0a09 0909 0909 2270  port}}",......"p
-00000810: 6174 6822 3a20 5b0a 0909 0909 0909 2273  ath": [......."s
-00000820: 7461 7475 7322 0a09 0909 0909 5d0a 0909  tatus"......]...
-00000830: 0909 7d0a 0909 097d 2c0a 0909 0922 7265  ..}....},...."re
-00000840: 7370 6f6e 7365 223a 205b 5d0a 0909 7d2c  sponse": []...},
-00000850: 0a09 097b 0a09 0909 226e 616d 6522 3a20  ...{...."name": 
-00000860: 227b 7b68 6f73 747d 7d3a 7b7b 706f 7274  "{{host}}:{{port
-00000870: 7d7d 2f65 6e64 706f 696e 7473 222c 0a09  }}/endpoints",..
-00000880: 0909 2272 6571 7565 7374 223a 207b 0a09  .."request": {..
-00000890: 0909 0922 6d65 7468 6f64 223a 2022 4745  ..."method": "GE
-000008a0: 5422 2c0a 0909 0909 2268 6561 6465 7222  T",....."header"
-000008b0: 3a20 5b5d 2c0a 0909 0909 2275 726c 223a  : [],....."url":
-000008c0: 207b 0a09 0909 0909 2272 6177 223a 2022   {......"raw": "
-000008d0: 7b7b 686f 7374 7d7d 3a7b 7b70 6f72 747d  {{host}}:{{port}
-000008e0: 7d2f 656e 6470 6f69 6e74 7322 2c0a 0909  }/endpoints",...
-000008f0: 0909 0922 686f 7374 223a 205b 0a09 0909  ..."host": [....
-00000900: 0909 0922 7b7b 686f 7374 7d7d 220a 0909  ..."{{host}}"...
-00000910: 0909 095d 2c0a 0909 0909 0922 706f 7274  ...],......"port
-00000920: 223a 2022 7b7b 706f 7274 7d7d 222c 0a09  ": "{{port}}",..
-00000930: 0909 0909 2270 6174 6822 3a20 5b0a 0909  ...."path": [...
-00000940: 0909 0909 2265 6e64 706f 696e 7473 220a  ...."endpoints".
-00000950: 0909 0909 095d 0a09 0909 097d 0a09 0909  .....].....}....
-00000960: 7d2c 0a09 0909 2272 6573 706f 6e73 6522  },...."response"
-00000970: 3a20 5b5d 0a09 097d 2c0a 0909 7b0a 0909  : []...},...{...
-00000980: 0922 6e61 6d65 223a 2022 7b7b 686f 7374  ."name": "{{host
-00000990: 7d7d 3a7b 7b70 6f72 747d 7d2f 7175 6572  }}:{{port}}/quer
-000009a0: 792f 6d6f 6465 6c5f 6e61 6d65 222c 0a09  y/model_name",..
-000009b0: 0909 2272 6571 7565 7374 223a 207b 0a09  .."request": {..
-000009c0: 0909 0922 6d65 7468 6f64 223a 2022 504f  ..."method": "PO
-000009d0: 5354 222c 0a09 0909 0922 6865 6164 6572  ST",....."header
-000009e0: 223a 205b 0a09 0909 0909 7b0a 0909 0909  ": [......{.....
-000009f0: 0909 226b 6579 223a 2022 436f 6e74 656e  .."key": "Conten
-00000a00: 742d 5479 7065 222c 0a09 0909 0909 0922  t-Type",......."
-00000a10: 6e61 6d65 223a 2022 436f 6e74 656e 742d  name": "Content-
-00000a20: 5479 7065 222c 0a09 0909 0909 0922 7661  Type",......."va
-00000a30: 6c75 6522 3a20 2261 7070 6c69 6361 7469  lue": "applicati
-00000a40: 6f6e 2f6a 736f 6e22 2c0a 0909 0909 0909  on/json",.......
-00000a50: 2274 7970 6522 3a20 2274 6578 7422 0a09  "type": "text"..
-00000a60: 0909 0909 7d0a 0909 0909 5d2c 0a09 0909  ....}.....],....
-00000a70: 0922 626f 6479 223a 207b 0a09 0909 0909  ."body": {......
-00000a80: 226d 6f64 6522 3a20 2272 6177 222c 0a09  "mode": "raw",..
-00000a90: 0909 0909 2272 6177 223a 2022 7b5c 725c  ...."raw": "{\r\
-00000aa0: 6e20 205c 2264 6174 615c 223a 207b 5c72  n  \"data\": {\r
-00000ab0: 5c6e 2020 2020 5c22 785c 223a 205b 5c72  \n    \"x\": [\r
-00000ac0: 5c6e 2020 2020 2020 362e 3335 2c5c 725c  \n      6.35,\r\
-00000ad0: 6e20 2020 2020 2036 2e34 2c5c 725c 6e20  n      6.4,\r\n 
-00000ae0: 2020 2020 2036 2e36 352c 5c72 5c6e 2020       6.65,\r\n  
-00000af0: 2020 2020 382e 362c 5c72 5c6e 2020 2020      8.6,\r\n    
-00000b00: 2020 382e 392c 5c72 5c6e 2020 2020 2020    8.9,\r\n      
-00000b10: 392c 5c72 5c6e 2020 2020 2020 392e 315c  9,\r\n      9.1\
-00000b20: 725c 6e20 2020 205d 2c5c 725c 6e20 2020  r\n    ],\r\n   
-00000b30: 205c 2279 5c22 3a20 5b5c 725c 6e20 2020   \"y\": [\r\n   
-00000b40: 2020 2031 2e39 352c 5c72 5c6e 2020 2020     1.95,\r\n    
-00000b50: 2020 312e 3935 2c5c 725c 6e20 2020 2020    1.95,\r\n     
-00000b60: 2032 2e30 352c 5c72 5c6e 2020 2020 2020   2.05,\r\n      
-00000b70: 332e 3035 2c5c 725c 6e20 2020 2020 2033  3.05,\r\n      3
-00000b80: 2e30 352c 5c72 5c6e 2020 2020 2020 332e  .05,\r\n      3.
-00000b90: 312c 5c72 5c6e 2020 2020 2020 332e 3135  1,\r\n      3.15
-00000ba0: 5c72 5c6e 2020 2020 5d5c 725c 6e20 207d  \r\n    ]\r\n  }
-00000bb0: 5c72 5c6e 7d22 0a09 0909 097d 2c0a 0909  \r\n}".....},...
-00000bc0: 0909 2275 726c 223a 207b 0a09 0909 0909  .."url": {......
-00000bd0: 2272 6177 223a 2022 7b7b 686f 7374 7d7d  "raw": "{{host}}
-00000be0: 3a7b 7b70 6f72 747d 7d2f 7175 6572 792f  :{{port}}/query/
-00000bf0: 6d6f 6465 6c5f 6e61 6d65 222c 0a09 0909  model_name",....
-00000c00: 0909 2268 6f73 7422 3a20 5b0a 0909 0909  .."host": [.....
-00000c10: 0909 227b 7b68 6f73 747d 7d22 0a09 0909  .."{{host}}"....
-00000c20: 0909 5d2c 0a09 0909 0909 2270 6f72 7422  ..],......"port"
-00000c30: 3a20 227b 7b70 6f72 747d 7d22 2c0a 0909  : "{{port}}",...
-00000c40: 0909 0922 7061 7468 223a 205b 0a09 0909  ..."path": [....
-00000c50: 0909 0922 7175 6572 7922 2c0a 0909 0909  ..."query",.....
-00000c60: 0909 226d 6f64 656c 5f6e 616d 6522 0a09  .."model_name"..
-00000c70: 0909 0909 5d0a 0909 0909 7d0a 0909 097d  ....].....}....}
-00000c80: 2c0a 0909 0922 7265 7370 6f6e 7365 223a  ,...."response":
-00000c90: 205b 5d0a 0909 7d2c 0a09 097b 0a09 0909   []...},...{....
-00000ca0: 226e 616d 6522 3a20 227b 7b68 6f73 747d  "name": "{{host}
-00000cb0: 7d3a 7b7b 706f 7274 7d7d 2f65 6e64 706f  }:{{port}}/endpo
-00000cc0: 696e 7473 2f6d 6f64 656c 5f6e 616d 6522  ints/model_name"
-00000cd0: 2c0a 0909 0922 7265 7175 6573 7422 3a20  ,...."request": 
-00000ce0: 7b0a 0909 0909 226d 6574 686f 6422 3a20  {....."method": 
-00000cf0: 2247 4554 222c 0a09 0909 0922 6865 6164  "GET",....."head
-00000d00: 6572 223a 205b 5d2c 0a09 0909 0922 7572  er": [],....."ur
-00000d10: 6c22 3a20 7b0a 0909 0909 0922 7261 7722  l": {......"raw"
-00000d20: 3a20 227b 7b68 6f73 747d 7d3a 7b7b 706f  : "{{host}}:{{po
-00000d30: 7274 7d7d 2f65 6e64 706f 696e 7473 2f6d  rt}}/endpoints/m
-00000d40: 6f64 656c 5f6e 616d 6522 2c0a 0909 0909  odel_name",.....
-00000d50: 0922 686f 7374 223a 205b 0a09 0909 0909  ."host": [......
-00000d60: 0922 7b7b 686f 7374 7d7d 220a 0909 0909  ."{{host}}".....
-00000d70: 095d 2c0a 0909 0909 0922 706f 7274 223a  .],......"port":
-00000d80: 2022 7b7b 706f 7274 7d7d 222c 0a09 0909   "{{port}}",....
-00000d90: 0909 2270 6174 6822 3a20 5b0a 0909 0909  .."path": [.....
-00000da0: 0909 2265 6e64 706f 696e 7473 222c 0a09  .."endpoints",..
-00000db0: 0909 0909 0922 6d6f 6465 6c5f 6e61 6d65  ....."model_name
-00000dc0: 220a 0909 0909 095d 0a09 0909 097d 0a09  "......].....}..
-00000dd0: 0909 7d2c 0a09 0909 2272 6573 706f 6e73  ..},...."respons
-00000de0: 6522 3a20 5b5d 0a09 097d 0a09 5d0a 7d    e": []...}..].}
+00000000: 7b0d 0a09 2269 6e66 6f22 3a20 7b0d 0a09  {..."info": {...
+00000010: 0922 5f70 6f73 746d 616e 5f69 6422 3a20  ."_postman_id": 
+00000020: 2261 6464 3062 3833 622d 3363 3131 2d34  "add0b83b-3c11-4
+00000030: 6338 302d 3937 3361 2d30 6135 6662 6638  c80-973a-0a5fbf8
+00000040: 3033 6535 3822 2c0d 0a09 0922 6e61 6d65  03e58",...."name
+00000050: 223a 2022 5461 6250 7922 2c0d 0a09 0922  ": "TabPy",...."
+00000060: 7363 6865 6d61 223a 2022 6874 7470 733a  schema": "https:
+00000070: 2f2f 7363 6865 6d61 2e67 6574 706f 7374  //schema.getpost
+00000080: 6d61 6e2e 636f 6d2f 6a73 6f6e 2f63 6f6c  man.com/json/col
+00000090: 6c65 6374 696f 6e2f 7632 2e31 2e30 2f63  lection/v2.1.0/c
+000000a0: 6f6c 6c65 6374 696f 6e2e 6a73 6f6e 220d  ollection.json".
+000000b0: 0a09 7d2c 0d0a 0922 6974 656d 223a 205b  ..},..."item": [
+000000c0: 0d0a 0909 7b0d 0a09 0909 226e 616d 6522  ....{....."name"
+000000d0: 3a20 227b 7b68 6f73 747d 7d3a 7b7b 706f  : "{{host}}:{{po
+000000e0: 7274 7d7d 2f69 6e66 6f22 2c0d 0a09 0909  rt}}/info",.....
+000000f0: 2272 6571 7565 7374 223a 207b 0d0a 0909  "request": {....
+00000100: 0909 226d 6574 686f 6422 3a20 2247 4554  .."method": "GET
+00000110: 222c 0d0a 0909 0909 2268 6561 6465 7222  ",......"header"
+00000120: 3a20 5b5d 2c0d 0a09 0909 0922 7572 6c22  : [],......"url"
+00000130: 3a20 7b0d 0a09 0909 0909 2272 6177 223a  : {......."raw":
+00000140: 2022 7b7b 686f 7374 7d7d 3a7b 7b70 6f72   "{{host}}:{{por
+00000150: 747d 7d2f 696e 666f 222c 0d0a 0909 0909  t}}/info",......
+00000160: 0922 686f 7374 223a 205b 0d0a 0909 0909  ."host": [......
+00000170: 0909 227b 7b68 6f73 747d 7d22 0d0a 0909  .."{{host}}"....
+00000180: 0909 095d 2c0d 0a09 0909 0909 2270 6f72  ...],......."por
+00000190: 7422 3a20 227b 7b70 6f72 747d 7d22 2c0d  t": "{{port}}",.
+000001a0: 0a09 0909 0909 2270 6174 6822 3a20 5b0d  ......"path": [.
+000001b0: 0a09 0909 0909 0922 696e 666f 220d 0a09  ......."info"...
+000001c0: 0909 0909 5d0d 0a09 0909 097d 0d0a 0909  ....]......}....
+000001d0: 097d 2c0d 0a09 0909 2272 6573 706f 6e73  .},....."respons
+000001e0: 6522 3a20 5b5d 0d0a 0909 7d2c 0d0a 0909  e": []....},....
+000001f0: 7b0d 0a09 0909 226e 616d 6522 3a20 227b  {....."name": "{
+00000200: 7b68 6f73 747d 7d3a 7b7b 706f 7274 7d7d  {host}}:{{port}}
+00000210: 2f65 7661 6c75 6174 6522 2c0d 0a09 0909  /evaluate",.....
+00000220: 2272 6571 7565 7374 223a 207b 0d0a 0909  "request": {....
+00000230: 0909 2261 7574 6822 3a20 7b0d 0a09 0909  .."auth": {.....
+00000240: 0909 2274 7970 6522 3a20 2262 6173 6963  .."type": "basic
+00000250: 222c 0d0a 0909 0909 0922 6261 7369 6322  ",......."basic"
+00000260: 3a20 5b0d 0a09 0909 0909 097b 0d0a 0909  : [........{....
+00000270: 0909 0909 0922 6b65 7922 3a20 2270 6173  ....."key": "pas
+00000280: 7377 6f72 6422 2c0d 0a09 0909 0909 0909  sword",.........
+00000290: 2276 616c 7565 223a 2022 5040 7373 7730  "value": "P@ssw0
+000002a0: 7264 222c 0d0a 0909 0909 0909 0922 7479  rd",........."ty
+000002b0: 7065 223a 2022 7374 7269 6e67 220d 0a09  pe": "string"...
+000002c0: 0909 0909 097d 2c0d 0a09 0909 0909 097b  .....},........{
+000002d0: 0d0a 0909 0909 0909 0922 6b65 7922 3a20  ........."key": 
+000002e0: 2275 7365 726e 616d 6522 2c0d 0a09 0909  "username",.....
+000002f0: 0909 0909 2276 616c 7565 223a 2022 7573  ...."value": "us
+00000300: 6572 3122 2c0d 0a09 0909 0909 0909 2274  er1",........."t
+00000310: 7970 6522 3a20 2273 7472 696e 6722 0d0a  ype": "string"..
+00000320: 0909 0909 0909 7d0d 0a09 0909 0909 5d0d  ......}.......].
+00000330: 0a09 0909 097d 2c0d 0a09 0909 0922 6d65  .....},......"me
+00000340: 7468 6f64 223a 2022 504f 5354 222c 0d0a  thod": "POST",..
+00000350: 0909 0909 2268 6561 6465 7222 3a20 5b0d  ...."header": [.
+00000360: 0a09 0909 0909 7b0d 0a09 0909 0909 0922  ......{........"
+00000370: 6b65 7922 3a20 2243 6f6e 7465 6e74 2d54  key": "Content-T
+00000380: 7970 6522 2c0d 0a09 0909 0909 0922 6e61  ype",........"na
+00000390: 6d65 223a 2022 436f 6e74 656e 742d 5479  me": "Content-Ty
+000003a0: 7065 222c 0d0a 0909 0909 0909 2276 616c  pe",........"val
+000003b0: 7565 223a 2022 6170 706c 6963 6174 696f  ue": "applicatio
+000003c0: 6e2f 6a73 6f6e 222c 0d0a 0909 0909 0909  n/json",........
+000003d0: 2274 7970 6522 3a20 2274 6578 7422 0d0a  "type": "text"..
+000003e0: 0909 0909 097d 2c0d 0a09 0909 0909 7b0d  .....},.......{.
+000003f0: 0a09 0909 0909 0922 6b65 7922 3a20 2254  ......."key": "T
+00000400: 6162 5079 2d43 6c69 656e 7422 2c0d 0a09  abPy-Client",...
+00000410: 0909 0909 0922 7661 6c75 6522 3a20 2250  ....."value": "P
+00000420: 6f73 746d 616e 2066 6f72 206d 616e 7561  ostman for manua
+00000430: 6c20 7465 7374 696e 6722 2c0d 0a09 0909  l testing",.....
+00000440: 0909 0922 7479 7065 223a 2022 7465 7874  ..."type": "text
+00000450: 220d 0a09 0909 0909 7d2c 0d0a 0909 0909  ".......},......
+00000460: 097b 0d0a 0909 0909 0909 226b 6579 223a  .{........"key":
+00000470: 2022 5461 6250 792d 5573 6572 222c 0d0a   "TabPy-User",..
+00000480: 0909 0909 0909 2276 616c 7565 223a 2022  ......"value": "
+00000490: 6f67 6f6c 6f76 6174 7969 222c 0d0a 0909  ogolovatyi",....
+000004a0: 0909 0909 2274 7970 6522 3a20 2274 6578  ...."type": "tex
+000004b0: 7422 0d0a 0909 0909 097d 0d0a 0909 0909  t".......}......
+000004c0: 5d2c 0d0a 0909 0909 2262 6f64 7922 3a20  ],......"body": 
+000004d0: 7b0d 0a09 0909 0909 226d 6f64 6522 3a20  {......."mode": 
+000004e0: 2272 6177 222c 0d0a 0909 0909 0922 7261  "raw",......."ra
+000004f0: 7722 3a20 227b 5c6e 5c74 5c22 6461 7461  w": "{\n\t\"data
+00000500: 5c22 3a20 5c6e 5c74 7b20 5c6e 5c74 5c74  \": \n\t{ \n\t\t
+00000510: 5c22 5f61 7267 315c 2220 3a20 5b31 2c20  \"_arg1\" : [1, 
+00000520: 322c 2033 5d2c 205c 6e5c 745c 745c 225f  2, 3], \n\t\t\"_
+00000530: 6172 6732 5c22 203a 205b 332c 202d 312c  arg2\" : [3, -1,
+00000540: 2035 5d5c 6e5c 747d 2c5c 6e5c 745c 2273   5]\n\t},\n\t\"s
+00000550: 6372 6970 745c 223a 205c 6e5c 745c 2272  cript\": \n\t\"r
+00000560: 6574 7572 6e20 5b78 202b 2079 2066 6f72  eturn [x + y for
+00000570: 2078 2c20 7920 696e 207a 6970 285f 6172   x, y in zip(_ar
+00000580: 6731 2c20 5f61 7267 3229 5d5c 225c 6e7d  g1, _arg2)]\"\n}
+00000590: 5c6e 222c 0d0a 0909 0909 0922 6f70 7469  \n",......."opti
+000005a0: 6f6e 7322 3a20 7b0d 0a09 0909 0909 0922  ons": {........"
+000005b0: 7261 7722 3a20 7b7d 0d0a 0909 0909 097d  raw": {}.......}
+000005c0: 0d0a 0909 0909 7d2c 0d0a 0909 0909 2275  ......},......"u
+000005d0: 726c 223a 207b 0d0a 0909 0909 0922 7261  rl": {......."ra
+000005e0: 7722 3a20 227b 7b68 6f73 747d 7d3a 7b7b  w": "{{host}}:{{
+000005f0: 706f 7274 7d7d 2f65 7661 6c75 6174 6522  port}}/evaluate"
+00000600: 2c0d 0a09 0909 0909 2268 6f73 7422 3a20  ,......."host": 
+00000610: 5b0d 0a09 0909 0909 0922 7b7b 686f 7374  [........"{{host
+00000620: 7d7d 220d 0a09 0909 0909 5d2c 0d0a 0909  }}".......],....
+00000630: 0909 0922 706f 7274 223a 2022 7b7b 706f  ..."port": "{{po
+00000640: 7274 7d7d 222c 0d0a 0909 0909 0922 7061  rt}}",......."pa
+00000650: 7468 223a 205b 0d0a 0909 0909 0909 2265  th": [........"e
+00000660: 7661 6c75 6174 6522 0d0a 0909 0909 095d  valuate".......]
+00000670: 2c0d 0a09 0909 0909 2271 7565 7279 223a  ,......."query":
+00000680: 205b 0d0a 0909 0909 0909 7b0d 0a09 0909   [........{.....
+00000690: 0909 0909 226b 6579 223a 2022 5461 6250  ...."key": "TabP
+000006a0: 792d 436c 6965 6e74 222c 0d0a 0909 0909  y-Client",......
+000006b0: 0909 0922 7661 6c75 6522 3a20 2250 6f73  ..."value": "Pos
+000006c0: 746d 616e 2066 6f72 204d 616e 7561 6c20  tman for Manual 
+000006d0: 5465 7374 696e 6722 2c0d 0a09 0909 0909  Testing",.......
+000006e0: 0909 2264 6973 6162 6c65 6422 3a20 7472  .."disabled": tr
+000006f0: 7565 0d0a 0909 0909 0909 7d2c 0d0a 0909  ue........},....
+00000700: 0909 0909 7b0d 0a09 0909 0909 0909 226b  ....{........."k
+00000710: 6579 223a 2022 5461 6250 792d 5573 6572  ey": "TabPy-User
+00000720: 222c 0d0a 0909 0909 0909 0922 7661 6c75  ",........."valu
+00000730: 6522 3a20 226f 676f 6c6f 7661 7479 6922  e": "ogolovatyi"
+00000740: 2c0d 0a09 0909 0909 0909 2264 6973 6162  ,........."disab
+00000750: 6c65 6422 3a20 7472 7565 0d0a 0909 0909  led": true......
+00000760: 0909 7d0d 0a09 0909 0909 5d0d 0a09 0909  ..}.......].....
+00000770: 097d 0d0a 0909 097d 2c0d 0a09 0909 2272  .}.....},....."r
+00000780: 6573 706f 6e73 6522 3a20 5b5d 0d0a 0909  esponse": []....
+00000790: 7d2c 0d0a 0909 7b0d 0a09 0909 226e 616d  },....{....."nam
+000007a0: 6522 3a20 227b 7b65 6e64 706f 696e 747d  e": "{{endpoint}
+000007b0: 7d2f 7374 6174 7573 222c 0d0a 0909 0922  }/status",....."
+000007c0: 7265 7175 6573 7422 3a20 7b0d 0a09 0909  request": {.....
+000007d0: 0922 6d65 7468 6f64 223a 2022 4745 5422  ."method": "GET"
+000007e0: 2c0d 0a09 0909 0922 6865 6164 6572 223a  ,......"header":
+000007f0: 205b 5d2c 0d0a 0909 0909 2275 726c 223a   [],......"url":
+00000800: 207b 0d0a 0909 0909 0922 7261 7722 3a20   {......."raw": 
+00000810: 227b 7b68 6f73 747d 7d3a 7b7b 706f 7274  "{{host}}:{{port
+00000820: 7d7d 2f73 7461 7475 7322 2c0d 0a09 0909  }}/status",.....
+00000830: 0909 2268 6f73 7422 3a20 5b0d 0a09 0909  .."host": [.....
+00000840: 0909 0922 7b7b 686f 7374 7d7d 220d 0a09  ..."{{host}}"...
+00000850: 0909 0909 5d2c 0d0a 0909 0909 0922 706f  ....],......."po
+00000860: 7274 223a 2022 7b7b 706f 7274 7d7d 222c  rt": "{{port}}",
+00000870: 0d0a 0909 0909 0922 7061 7468 223a 205b  ......."path": [
+00000880: 0d0a 0909 0909 0909 2273 7461 7475 7322  ........"status"
+00000890: 0d0a 0909 0909 095d 0d0a 0909 0909 7d0d  .......]......}.
+000008a0: 0a09 0909 7d2c 0d0a 0909 0922 7265 7370  ....},....."resp
+000008b0: 6f6e 7365 223a 205b 5d0d 0a09 097d 2c0d  onse": []....},.
+000008c0: 0a09 097b 0d0a 0909 0922 6e61 6d65 223a  ...{....."name":
+000008d0: 2022 7b7b 686f 7374 7d7d 3a7b 7b70 6f72   "{{host}}:{{por
+000008e0: 747d 7d2f 656e 6470 6f69 6e74 7322 2c0d  t}}/endpoints",.
+000008f0: 0a09 0909 2272 6571 7565 7374 223a 207b  ...."request": {
+00000900: 0d0a 0909 0909 226d 6574 686f 6422 3a20  ......"method": 
+00000910: 2247 4554 222c 0d0a 0909 0909 2268 6561  "GET",......"hea
+00000920: 6465 7222 3a20 5b5d 2c0d 0a09 0909 0922  der": [],......"
+00000930: 7572 6c22 3a20 7b0d 0a09 0909 0909 2272  url": {......."r
+00000940: 6177 223a 2022 7b7b 686f 7374 7d7d 3a7b  aw": "{{host}}:{
+00000950: 7b70 6f72 747d 7d2f 656e 6470 6f69 6e74  {port}}/endpoint
+00000960: 7322 2c0d 0a09 0909 0909 2268 6f73 7422  s",......."host"
+00000970: 3a20 5b0d 0a09 0909 0909 0922 7b7b 686f  : [........"{{ho
+00000980: 7374 7d7d 220d 0a09 0909 0909 5d2c 0d0a  st}}".......],..
+00000990: 0909 0909 0922 706f 7274 223a 2022 7b7b  ....."port": "{{
+000009a0: 706f 7274 7d7d 222c 0d0a 0909 0909 0922  port}}",......."
+000009b0: 7061 7468 223a 205b 0d0a 0909 0909 0909  path": [........
+000009c0: 2265 6e64 706f 696e 7473 220d 0a09 0909  "endpoints".....
+000009d0: 0909 5d0d 0a09 0909 097d 0d0a 0909 097d  ..]......}.....}
+000009e0: 2c0d 0a09 0909 2272 6573 706f 6e73 6522  ,....."response"
+000009f0: 3a20 5b5d 0d0a 0909 7d2c 0d0a 0909 7b0d  : []....},....{.
+00000a00: 0a09 0909 226e 616d 6522 3a20 227b 7b68  ...."name": "{{h
+00000a10: 6f73 747d 7d3a 7b7b 706f 7274 7d7d 2f71  ost}}:{{port}}/q
+00000a20: 7565 7279 2f6d 6f64 656c 5f6e 616d 6522  uery/model_name"
+00000a30: 2c0d 0a09 0909 2272 6571 7565 7374 223a  ,....."request":
+00000a40: 207b 0d0a 0909 0909 226d 6574 686f 6422   {......"method"
+00000a50: 3a20 2250 4f53 5422 2c0d 0a09 0909 0922  : "POST",......"
+00000a60: 6865 6164 6572 223a 205b 0d0a 0909 0909  header": [......
+00000a70: 097b 0d0a 0909 0909 0909 226b 6579 223a  .{........"key":
+00000a80: 2022 436f 6e74 656e 742d 5479 7065 222c   "Content-Type",
+00000a90: 0d0a 0909 0909 0909 226e 616d 6522 3a20  ........"name": 
+00000aa0: 2243 6f6e 7465 6e74 2d54 7970 6522 2c0d  "Content-Type",.
+00000ab0: 0a09 0909 0909 0922 7661 6c75 6522 3a20  ......."value": 
+00000ac0: 2261 7070 6c69 6361 7469 6f6e 2f6a 736f  "application/jso
+00000ad0: 6e22 2c0d 0a09 0909 0909 0922 7479 7065  n",........"type
+00000ae0: 223a 2022 7465 7874 220d 0a09 0909 0909  ": "text".......
+00000af0: 7d0d 0a09 0909 095d 2c0d 0a09 0909 0922  }......],......"
+00000b00: 626f 6479 223a 207b 0d0a 0909 0909 0922  body": {......."
+00000b10: 6d6f 6465 223a 2022 7261 7722 2c0d 0a09  mode": "raw",...
+00000b20: 0909 0909 2272 6177 223a 2022 7b5c 725c  ...."raw": "{\r\
+00000b30: 6e20 205c 2264 6174 615c 223a 207b 5c72  n  \"data\": {\r
+00000b40: 5c6e 2020 2020 5c22 785c 223a 205b 5c72  \n    \"x\": [\r
+00000b50: 5c6e 2020 2020 2020 362e 3335 2c5c 725c  \n      6.35,\r\
+00000b60: 6e20 2020 2020 2036 2e34 2c5c 725c 6e20  n      6.4,\r\n 
+00000b70: 2020 2020 2036 2e36 352c 5c72 5c6e 2020       6.65,\r\n  
+00000b80: 2020 2020 382e 362c 5c72 5c6e 2020 2020      8.6,\r\n    
+00000b90: 2020 382e 392c 5c72 5c6e 2020 2020 2020    8.9,\r\n      
+00000ba0: 392c 5c72 5c6e 2020 2020 2020 392e 315c  9,\r\n      9.1\
+00000bb0: 725c 6e20 2020 205d 2c5c 725c 6e20 2020  r\n    ],\r\n   
+00000bc0: 205c 2279 5c22 3a20 5b5c 725c 6e20 2020   \"y\": [\r\n   
+00000bd0: 2020 2031 2e39 352c 5c72 5c6e 2020 2020     1.95,\r\n    
+00000be0: 2020 312e 3935 2c5c 725c 6e20 2020 2020    1.95,\r\n     
+00000bf0: 2032 2e30 352c 5c72 5c6e 2020 2020 2020   2.05,\r\n      
+00000c00: 332e 3035 2c5c 725c 6e20 2020 2020 2033  3.05,\r\n      3
+00000c10: 2e30 352c 5c72 5c6e 2020 2020 2020 332e  .05,\r\n      3.
+00000c20: 312c 5c72 5c6e 2020 2020 2020 332e 3135  1,\r\n      3.15
+00000c30: 5c72 5c6e 2020 2020 5d5c 725c 6e20 207d  \r\n    ]\r\n  }
+00000c40: 5c72 5c6e 7d22 0d0a 0909 0909 7d2c 0d0a  \r\n}"......},..
+00000c50: 0909 0909 2275 726c 223a 207b 0d0a 0909  ...."url": {....
+00000c60: 0909 0922 7261 7722 3a20 227b 7b68 6f73  ..."raw": "{{hos
+00000c70: 747d 7d3a 7b7b 706f 7274 7d7d 2f71 7565  t}}:{{port}}/que
+00000c80: 7279 2f6d 6f64 656c 5f6e 616d 6522 2c0d  ry/model_name",.
+00000c90: 0a09 0909 0909 2268 6f73 7422 3a20 5b0d  ......"host": [.
+00000ca0: 0a09 0909 0909 0922 7b7b 686f 7374 7d7d  ......."{{host}}
+00000cb0: 220d 0a09 0909 0909 5d2c 0d0a 0909 0909  ".......],......
+00000cc0: 0922 706f 7274 223a 2022 7b7b 706f 7274  ."port": "{{port
+00000cd0: 7d7d 222c 0d0a 0909 0909 0922 7061 7468  }}",......."path
+00000ce0: 223a 205b 0d0a 0909 0909 0909 2271 7565  ": [........"que
+00000cf0: 7279 222c 0d0a 0909 0909 0909 226d 6f64  ry",........"mod
+00000d00: 656c 5f6e 616d 6522 0d0a 0909 0909 095d  el_name".......]
+00000d10: 0d0a 0909 0909 7d0d 0a09 0909 7d2c 0d0a  ......}.....},..
+00000d20: 0909 0922 7265 7370 6f6e 7365 223a 205b  ..."response": [
+00000d30: 5d0d 0a09 097d 2c0d 0a09 097b 0d0a 0909  ]....},....{....
+00000d40: 0922 6e61 6d65 223a 2022 7b7b 686f 7374  ."name": "{{host
+00000d50: 7d7d 3a7b 7b70 6f72 747d 7d2f 656e 6470  }}:{{port}}/endp
+00000d60: 6f69 6e74 732f 6d6f 6465 6c5f 6e61 6d65  oints/model_name
+00000d70: 222c 0d0a 0909 0922 7265 7175 6573 7422  ",....."request"
+00000d80: 3a20 7b0d 0a09 0909 0922 6d65 7468 6f64  : {......"method
+00000d90: 223a 2022 4745 5422 2c0d 0a09 0909 0922  ": "GET",......"
+00000da0: 6865 6164 6572 223a 205b 5d2c 0d0a 0909  header": [],....
+00000db0: 0909 2275 726c 223a 207b 0d0a 0909 0909  .."url": {......
+00000dc0: 0922 7261 7722 3a20 227b 7b68 6f73 747d  ."raw": "{{host}
+00000dd0: 7d3a 7b7b 706f 7274 7d7d 2f65 6e64 706f  }:{{port}}/endpo
+00000de0: 696e 7473 2f6d 6f64 656c 5f6e 616d 6522  ints/model_name"
+00000df0: 2c0d 0a09 0909 0909 2268 6f73 7422 3a20  ,......."host": 
+00000e00: 5b0d 0a09 0909 0909 0922 7b7b 686f 7374  [........"{{host
+00000e10: 7d7d 220d 0a09 0909 0909 5d2c 0d0a 0909  }}".......],....
+00000e20: 0909 0922 706f 7274 223a 2022 7b7b 706f  ..."port": "{{po
+00000e30: 7274 7d7d 222c 0d0a 0909 0909 0922 7061  rt}}",......."pa
+00000e40: 7468 223a 205b 0d0a 0909 0909 0909 2265  th": [........"e
+00000e50: 6e64 706f 696e 7473 222c 0d0a 0909 0909  ndpoints",......
+00000e60: 0909 226d 6f64 656c 5f6e 616d 6522 0d0a  .."model_name"..
+00000e70: 0909 0909 095d 0d0a 0909 0909 7d0d 0a09  .....]......}...
+00000e80: 0909 7d2c 0d0a 0909 0922 7265 7370 6f6e  ..},....."respon
+00000e90: 7365 223a 205b 5d0d 0a09 097d 0d0a 095d  se": []....}...]
+00000ea0: 0d0a 7d                                  ..}
```

### Comparing `tabpy-2.6.0/misc/TabPy.yml` & `tabpy-2.7.0/misc/TabPy.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/setup.py` & `tabpy-2.7.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,107 +1,108 @@
-"""Web server Tableau uses to run Python scripts.
-
-TabPy (the Tableau Python Server) is an external service implementation
-which expands Tableau's capabilities by allowing users to execute Python
-scripts and saved functions via Tableau's table calculations.
-"""
-
-import os
-from setuptools import setup, find_packages
-import unittest
-
-
-DOCLINES = (__doc__ or "").split("\n")
-
-
-def setup_package():
-    def read(fname):
-        return open(os.path.join(os.path.dirname(__file__), fname)).read()
-
-    setup(
-        name="tabpy",
-        version=read("tabpy/VERSION"),
-        description=DOCLINES[0],
-        long_description="\n".join(DOCLINES[1:]) + "\n" + read("CHANGELOG"),
-        long_description_content_type="text/markdown",
-        url="https://github.com/tableau/TabPy",
-        author="Tableau",
-        author_email="github@tableau.com",
-        maintainer="Tableau",
-        maintainer_email="github@tableau.com",
-        download_url="https://pypi.org/project/tabpy",
-        project_urls={
-            "Bug Tracker": "https://github.com/tableau/TabPy/issues",
-            "Documentation": "https://tableau.github.io/TabPy/",
-            "Source Code": "https://github.com/tableau/TabPy",
-        },
-        classifiers=[
-            "Development Status :: 5 - Production/Stable",
-            "Intended Audience :: Developers",
-            "Intended Audience :: Science/Research",
-            "License :: OSI Approved :: MIT License",
-            "Programming Language :: Python :: 3.7",
-            "Programming Language :: Python :: 3.8",
-            "Programming Language :: Python :: 3.9",
-            "Topic :: Scientific/Engineering",
-            "Topic :: Scientific/Engineering :: Information Analysis",
-            "Operating System :: Microsoft :: Windows",
-            "Operating System :: POSIX",
-            "Operating System :: Unix",
-            "Operating System :: MacOS",
-        ],
-        platforms=["Windows", "Linux", "Mac OS-X", "Unix"],
-        keywords=["tabpy tableau"],
-        packages=find_packages(exclude=["docs", "misc"]),
-        package_data={
-            "tabpy": [
-                "VERSION",
-                "tabpy_server/state.ini.template",
-                "tabpy_server/static/*",
-                "tabpy_server/common/default.conf",
-            ]
-        },
-        python_requires=">=3.7",
-        license="MIT",
-        # Note: many of these required packages are included in base python
-        # but are listed here because different linux distros use custom
-        # python installations.  And users can remove packages at any point
-        install_requires=[
-            "cloudpickle",
-            "configparser",
-            "coverage",
-            "coveralls",
-            "docopt",
-            "future",
-            "genson",
-            "hypothesis",
-            "jsonschema",
-            "mock",
-            "nltk",
-            "numpy",
-            "pandas",
-            "pyopenssl",
-            "pytest",
-            "pytest-cov",
-            "requests",
-            "scipy",
-            "simplejson",
-            "scikit-learn",
-            "textblob",
-            "tornado",
-            "twisted",
-            "urllib3",
-        ],
-        entry_points={
-            "console_scripts": [
-                "tabpy=tabpy.tabpy:main",
-                "tabpy-deploy-models=tabpy.models.deploy_models:main",
-                "tabpy-user=tabpy.utils.tabpy_user:main",
-            ],
-        },
-        setup_requires=["pytest-runner"],
-        test_suite="pytest",
-    )
-
-
-if __name__ == "__main__":
-    setup_package()
+"""Web server Tableau uses to run Python scripts.
+
+TabPy (the Tableau Python Server) is an external service implementation
+which expands Tableau's capabilities by allowing users to execute Python
+scripts and saved functions via Tableau's table calculations.
+"""
+
+import os
+from setuptools import setup, find_packages
+import unittest
+
+
+DOCLINES = (__doc__ or "").split("\n")
+
+
+def setup_package():
+    def read(fname):
+        return open(os.path.join(os.path.dirname(__file__), fname)).read()
+
+    setup(
+        name="tabpy",
+        version=read("tabpy/VERSION"),
+        description=DOCLINES[0],
+        long_description="\n".join(DOCLINES[1:]) + "\n" + read("CHANGELOG"),
+        long_description_content_type="text/markdown",
+        url="https://github.com/tableau/TabPy",
+        author="Tableau",
+        author_email="github@tableau.com",
+        maintainer="Tableau",
+        maintainer_email="github@tableau.com",
+        download_url="https://pypi.org/project/tabpy",
+        project_urls={
+            "Bug Tracker": "https://github.com/tableau/TabPy/issues",
+            "Documentation": "https://tableau.github.io/TabPy/",
+            "Source Code": "https://github.com/tableau/TabPy",
+        },
+        classifiers=[
+            "Development Status :: 5 - Production/Stable",
+            "Intended Audience :: Developers",
+            "Intended Audience :: Science/Research",
+            "License :: OSI Approved :: MIT License",
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Topic :: Scientific/Engineering",
+            "Topic :: Scientific/Engineering :: Information Analysis",
+            "Operating System :: Microsoft :: Windows",
+            "Operating System :: POSIX",
+            "Operating System :: Unix",
+            "Operating System :: MacOS",
+        ],
+        platforms=["Windows", "Linux", "Mac OS-X", "Unix"],
+        keywords=["tabpy tableau"],
+        packages=find_packages(exclude=["docs", "misc"]),
+        package_data={
+            "tabpy": [
+                "VERSION",
+                "tabpy_server/state.ini.template",
+                "tabpy_server/static/*",
+                "tabpy_server/common/default.conf",
+            ]
+        },
+        python_requires=">=3.7",
+        license="MIT",
+        # Note: many of these required packages are included in base python
+        # but are listed here because different linux distros use custom
+        # python installations.  And users can remove packages at any point
+        install_requires=[
+            "cloudpickle",
+            "configparser",
+            "coverage",
+            "coveralls",
+            "docopt",
+            "future",
+            "genson",
+            "hypothesis",
+            "jsonschema",
+            "mock",
+            "nltk",
+            "numpy",
+            "pandas",
+            "pyopenssl",
+            "pytest",
+            "pytest-cov",
+            "requests",
+            "scipy",
+            "simplejson",
+            "scikit-learn",
+            "textblob",
+            "tornado",
+            "twisted",
+            "urllib3",
+            "pyarrow",
+        ],
+        entry_points={
+            "console_scripts": [
+                "tabpy=tabpy.tabpy:main",
+                "tabpy-deploy-models=tabpy.models.deploy_models:main",
+                "tabpy-user=tabpy.utils.tabpy_user:main",
+            ],
+        },
+        setup_requires=["pytest-runner"],
+        test_suite="pytest",
+    )
+
+
+if __name__ == "__main__":
+    setup_package()
```

### Comparing `tabpy-2.6.0/tabpy/models/deploy_models.py` & `tabpy-2.7.0/tabpy/models/deploy_models.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import os
-from pathlib import Path
-import platform
-import subprocess
-import sys
-from tabpy.models.utils import setup_utils
-
-
-def main():
-    # Determine if we run python or python3
-    py = "python" if platform.system() == "Windows" else "python3"
-
-    file_path = sys.argv[1] if len(sys.argv) > 1 else setup_utils.get_default_config_file_path()
-    print(f"Using config file at {file_path}")
-
-    port, auth_on, prefix = setup_utils.parse_config(file_path)
-    auth_args = setup_utils.get_creds() if auth_on else []
-
-    directory = str(Path(__file__).resolve().parent / "scripts")
-    # Deploy each model in the scripts directory
-    for filename in os.listdir(directory):
-        subprocess.run([py, f"{directory}/{filename}", file_path] + auth_args)
-
-
-if __name__ == "__main__":
-    main()
+import os
+from pathlib import Path
+import platform
+import subprocess
+import sys
+from tabpy.models.utils import setup_utils
+
+
+def main():
+    # Determine if we run python or python3
+    py = "python" if platform.system() == "Windows" else "python3"
+
+    file_path = sys.argv[1] if len(sys.argv) > 1 else setup_utils.get_default_config_file_path()
+    print(f"Using config file at {file_path}")
+
+    port, auth_on, prefix = setup_utils.parse_config(file_path)
+    auth_args = setup_utils.get_creds() if auth_on else []
+
+    directory = str(Path(__file__).resolve().parent / "scripts")
+    # Deploy each model in the scripts directory
+    for filename in os.listdir(directory):
+        subprocess.run([py, f"{directory}/{filename}", file_path] + auth_args)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `tabpy-2.6.0/tabpy/models/scripts/PCA.py` & `tabpy-2.7.0/tabpy/models/scripts/PCA.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import pandas as pd
-from numpy import array
-from sklearn.decomposition import PCA as sklearnPCA
-from sklearn.preprocessing import StandardScaler
-from sklearn.preprocessing import LabelEncoder
-from sklearn.preprocessing import OneHotEncoder
-from tabpy.models.utils import setup_utils
-
-
-def PCA(component, _arg1, _arg2, *_argN):
-    """
-    Principal Component Analysis is a technique that extracts the key
-    distinct components from a high dimensional space whie attempting
-    to capture as much of the variance as possible. For more information
-    on the function and how to use it please refer to tabpy-tools.md
-    """
-    cols = [_arg1, _arg2] + list(_argN)
-    encodedCols = []
-    labelEncoder = LabelEncoder()
-    oneHotEncoder = OneHotEncoder(categories="auto", sparse=False)
-
-    for col in cols:
-        if isinstance(col[0], (int, float)):
-            encodedCols.append(col)
-        elif type(col[0]) is bool:
-            intCol = array(col)
-            encodedCols.append(intCol.astype(int))
-        else:
-            if len(set(col)) > 25:
-                print(
-                    "ERROR: Non-numeric arguments cannot have more than "
-                    "25 unique values"
-                )
-                raise ValueError
-            integerEncoded = labelEncoder.fit_transform(array(col))
-            integerEncoded = integerEncoded.reshape(len(col), 1)
-            oneHotEncoded = oneHotEncoder.fit_transform(integerEncoded)
-            transformedMatrix = oneHotEncoded.transpose()
-            encodedCols += list(transformedMatrix)
-
-    dataDict = {}
-    for i in range(len(encodedCols)):
-        dataDict[f"col{1 + i}"] = list(encodedCols[i])
-
-    if component <= 0 or component > len(dataDict):
-        print("ERROR: Component specified must be >= 0 and " "<= number of arguments")
-        raise ValueError
-
-    df = pd.DataFrame(data=dataDict, dtype=float)
-    scale = StandardScaler()
-    scaledData = scale.fit_transform(df)
-
-    pca = sklearnPCA()
-    pcaComponents = pca.fit_transform(scaledData)
-
-    return pcaComponents[:, component - 1].tolist()
-
-
-if __name__ == "__main__":
-    setup_utils.deploy_model("PCA", PCA, "Returns the specified principal component")
+import pandas as pd
+from numpy import array
+from sklearn.decomposition import PCA as sklearnPCA
+from sklearn.preprocessing import StandardScaler
+from sklearn.preprocessing import LabelEncoder
+from sklearn.preprocessing import OneHotEncoder
+from tabpy.models.utils import setup_utils
+
+
+def PCA(component, _arg1, _arg2, *_argN):
+    """
+    Principal Component Analysis is a technique that extracts the key
+    distinct components from a high dimensional space whie attempting
+    to capture as much of the variance as possible. For more information
+    on the function and how to use it please refer to tabpy-tools.md
+    """
+    cols = [_arg1, _arg2] + list(_argN)
+    encodedCols = []
+    labelEncoder = LabelEncoder()
+    oneHotEncoder = OneHotEncoder(categories="auto", sparse=False)
+
+    for col in cols:
+        if isinstance(col[0], (int, float)):
+            encodedCols.append(col)
+        elif type(col[0]) is bool:
+            intCol = array(col)
+            encodedCols.append(intCol.astype(int))
+        else:
+            if len(set(col)) > 25:
+                print(
+                    "ERROR: Non-numeric arguments cannot have more than "
+                    "25 unique values"
+                )
+                raise ValueError
+            integerEncoded = labelEncoder.fit_transform(array(col))
+            integerEncoded = integerEncoded.reshape(len(col), 1)
+            oneHotEncoded = oneHotEncoder.fit_transform(integerEncoded)
+            transformedMatrix = oneHotEncoded.transpose()
+            encodedCols += list(transformedMatrix)
+
+    dataDict = {}
+    for i in range(len(encodedCols)):
+        dataDict[f"col{1 + i}"] = list(encodedCols[i])
+
+    if component <= 0 or component > len(dataDict):
+        print("ERROR: Component specified must be >= 0 and " "<= number of arguments")
+        raise ValueError
+
+    df = pd.DataFrame(data=dataDict, dtype=float)
+    scale = StandardScaler()
+    scaledData = scale.fit_transform(df)
+
+    pca = sklearnPCA()
+    pcaComponents = pca.fit_transform(scaledData)
+
+    return pcaComponents[:, component - 1].tolist()
+
+
+if __name__ == "__main__":
+    setup_utils.deploy_model("PCA", PCA, "Returns the specified principal component")
```

### Comparing `tabpy-2.6.0/tabpy/models/scripts/tTest.py` & `tabpy-2.7.0/tabpy/models/scripts/tTest.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from scipy import stats
-from tabpy.models.utils import setup_utils
-
-
-def ttest(_arg1, _arg2):
-    """
-    T-Test is a statistical hypothesis test that is used to compare
-    two sample means or a sample’s mean against a known population mean.
-    For more information on the function and how to use it please refer
-    to tabpy-tools.md
-    """
-    # one sample test with mean
-    if len(_arg2) == 1:
-        test_stat, p_value = stats.ttest_1samp(_arg1, _arg2)
-        return p_value
-    # two sample t-test where _arg1 is numeric and _arg2 is a binary factor
-    elif len(set(_arg2)) == 2:
-        # each sample in _arg1 needs to have a corresponding classification
-        # in _arg2
-        if not (len(_arg1) == len(_arg2)):
-            raise ValueError
-        class1, class2 = set(_arg2)
-        sample1 = []
-        sample2 = []
-        for i in range(len(_arg1)):
-            if _arg2[i] == class1:
-                sample1.append(_arg1[i])
-            else:
-                sample2.append(_arg1[i])
-        test_stat, p_value = stats.ttest_ind(sample1, sample2, equal_var=False)
-        return p_value
-    # arg1 is a sample and arg2 is a sample
-    else:
-        test_stat, p_value = stats.ttest_ind(_arg1, _arg2, equal_var=False)
-        return p_value
-
-
-if __name__ == "__main__":
-    setup_utils.deploy_model("ttest", ttest, "Returns the p-value form a t-test")
+from scipy import stats
+from tabpy.models.utils import setup_utils
+
+
+def ttest(_arg1, _arg2):
+    """
+    T-Test is a statistical hypothesis test that is used to compare
+    two sample means or a sample’s mean against a known population mean.
+    For more information on the function and how to use it please refer
+    to tabpy-tools.md
+    """
+    # one sample test with mean
+    if len(_arg2) == 1:
+        test_stat, p_value = stats.ttest_1samp(_arg1, _arg2)
+        return p_value
+    # two sample t-test where _arg1 is numeric and _arg2 is a binary factor
+    elif len(set(_arg2)) == 2:
+        # each sample in _arg1 needs to have a corresponding classification
+        # in _arg2
+        if not (len(_arg1) == len(_arg2)):
+            raise ValueError
+        class1, class2 = set(_arg2)
+        sample1 = []
+        sample2 = []
+        for i in range(len(_arg1)):
+            if _arg2[i] == class1:
+                sample1.append(_arg1[i])
+            else:
+                sample2.append(_arg1[i])
+        test_stat, p_value = stats.ttest_ind(sample1, sample2, equal_var=False)
+        return p_value
+    # arg1 is a sample and arg2 is a sample
+    else:
+        test_stat, p_value = stats.ttest_ind(_arg1, _arg2, equal_var=False)
+        return p_value
+
+
+if __name__ == "__main__":
+    setup_utils.deploy_model("ttest", ttest, "Returns the p-value form a t-test")
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/app/app.py` & `tabpy-2.7.0/tabpy/tabpy_server/app/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,445 +1,499 @@
-import concurrent.futures
-import configparser
-import logging
-import multiprocessing
-import os
-import shutil
-import signal
-import sys
-import tabpy
-from tabpy.tabpy import __version__
-from tabpy.tabpy_server.app.app_parameters import ConfigParameters, SettingsParameters
-from tabpy.tabpy_server.app.util import parse_pwd_file
-from tabpy.tabpy_server.management.state import TabPyState
-from tabpy.tabpy_server.management.util import _get_state_from_file
-from tabpy.tabpy_server.psws.callbacks import init_model_evaluator, init_ps_server
-from tabpy.tabpy_server.psws.python_service import PythonService, PythonServiceHandler
-from tabpy.tabpy_server.handlers import (
-    EndpointHandler,
-    EndpointsHandler,
-    EvaluationPlaneHandler,
-    EvaluationPlaneDisabledHandler,
-    QueryPlaneHandler,
-    ServiceInfoHandler,
-    StatusHandler,
-    UploadDestinationHandler,
-)
-import tornado
-
-
-logger = logging.getLogger(__name__)
-
-
-def _init_asyncio_patch():
-    """
-    Select compatible event loop for Tornado 5+.
-    As of Python 3.8, the default event loop on Windows is `proactor`,
-    however Tornado requires the old default "selector" event loop.
-    As Tornado has decided to leave this to users to set, MkDocs needs
-    to set it. See https://github.com/tornadoweb/tornado/issues/2608.
-    """
-    if sys.platform.startswith("win") and sys.version_info >= (3, 8):
-        import asyncio
-        try:
-            from asyncio import WindowsSelectorEventLoopPolicy
-        except ImportError:
-            pass  # Can't assign a policy which doesn't exist.
-        else:
-            if not isinstance(asyncio.get_event_loop_policy(), WindowsSelectorEventLoopPolicy):
-                asyncio.set_event_loop_policy(WindowsSelectorEventLoopPolicy())
-
-
-class TabPyApp:
-    """
-    TabPy application class for keeping context like settings, state, etc.
-    """
-
-    settings = {}
-    subdirectory = ""
-    tabpy_state = None
-    python_service = None
-    credentials = {}
-
-    def __init__(self, config_file):
-        if config_file is None:
-            config_file = os.path.join(
-                os.path.dirname(__file__), os.path.pardir, "common", "default.conf"
-            )
-
-        if os.path.isfile(config_file):
-            try:
-                from logging import config
-                config.fileConfig(config_file, disable_existing_loggers=False)
-            except KeyError:
-                logging.basicConfig(level=logging.DEBUG)
-
-        self._parse_config(config_file)
-
-    def run(self):
-        application = self._create_tornado_web_app()
-        max_request_size = (
-            int(self.settings[SettingsParameters.MaxRequestSizeInMb]) * 1024 * 1024
-        )
-        logger.info(f"Setting max request size to {max_request_size} bytes")
-
-        init_model_evaluator(self.settings, self.tabpy_state, self.python_service)
-
-        protocol = self.settings[SettingsParameters.TransferProtocol]
-        ssl_options = None
-        if protocol == "https":
-            ssl_options = {
-                "certfile": self.settings[SettingsParameters.CertificateFile],
-                "keyfile": self.settings[SettingsParameters.KeyFile],
-            }
-        elif protocol != "http":
-            msg = f"Unsupported transfer protocol {protocol}."
-            logger.critical(msg)
-            raise RuntimeError(msg)
-
-        settings = {}
-        if self.settings[SettingsParameters.GzipEnabled] is True:
-            settings["decompress_request"] = True
-        application.listen(
-            self.settings[SettingsParameters.Port],
-            ssl_options=ssl_options,
-            max_buffer_size=max_request_size,
-            max_body_size=max_request_size,
-            **settings,
-        )
-
-        logger.info(
-            "Web service listening on port "
-            f"{str(self.settings[SettingsParameters.Port])}"
-        )
-        tornado.ioloop.IOLoop.instance().start()
-
-    def _create_tornado_web_app(self):
-        class TabPyTornadoApp(tornado.web.Application):
-            is_closing = False
-
-            def signal_handler(self, signal, _):
-                logger.critical(f"Exiting on signal {signal}...")
-                self.is_closing = True
-
-            def try_exit(self):
-                if self.is_closing:
-                    tornado.ioloop.IOLoop.instance().stop()
-                    logger.info("Shutting down TabPy...")
-
-        logger.info("Initializing TabPy...")
-        tornado.ioloop.IOLoop.instance().run_sync(
-            lambda: init_ps_server(self.settings, self.tabpy_state)
-        )
-        logger.info("Done initializing TabPy.")
-
-        executor = concurrent.futures.ThreadPoolExecutor(
-            max_workers=multiprocessing.cpu_count()
-        )
-
-        # initialize Tornado application
-        _init_asyncio_patch()
-        application = TabPyTornadoApp(
-            [
-                (
-                    self.subdirectory + r"/query/([^/]+)",
-                    QueryPlaneHandler,
-                    dict(app=self),
-                ),
-                (self.subdirectory + r"/status", StatusHandler, dict(app=self)),
-                (self.subdirectory + r"/info", ServiceInfoHandler, dict(app=self)),
-                (self.subdirectory + r"/endpoints", EndpointsHandler, dict(app=self)),
-                (
-                    self.subdirectory + r"/endpoints/([^/]+)?",
-                    EndpointHandler,
-                    dict(app=self),
-                ),
-                (
-                    self.subdirectory + r"/evaluate",
-                    EvaluationPlaneHandler if self.settings[SettingsParameters.EvaluateEnabled]
-                    else EvaluationPlaneDisabledHandler,
-                    dict(executor=executor, app=self),
-                ),
-                (
-                    self.subdirectory + r"/configurations/endpoint_upload_destination",
-                    UploadDestinationHandler,
-                    dict(app=self),
-                ),
-                (
-                    self.subdirectory + r"/(.*)",
-                    tornado.web.StaticFileHandler,
-                    dict(
-                        path=self.settings[SettingsParameters.StaticPath],
-                        default_filename="index.html",
-                    ),
-                ),
-            ],
-            debug=False,
-            **self.settings,
-        )
-
-        signal.signal(signal.SIGINT, application.signal_handler)
-        tornado.ioloop.PeriodicCallback(application.try_exit, 500).start()
-
-        signal.signal(signal.SIGINT, application.signal_handler)
-        tornado.ioloop.PeriodicCallback(application.try_exit, 500).start()
-
-        return application
-
-    def _set_parameter(self, parser, settings_key, config_key, default_val, parse_function):
-        key_is_set = False
-
-        if (
-            config_key is not None
-            and parser.has_section("TabPy")
-            and parser.has_option("TabPy", config_key)
-        ):
-            if parse_function is None:
-                parse_function = parser.get
-            self.settings[settings_key] = parse_function("TabPy", config_key)
-            key_is_set = True
-            logger.debug(
-                f"Parameter {settings_key} set to "
-                f'"{self.settings[settings_key]}" '
-                "from config file or environment variable"
-            )
-
-        if not key_is_set and default_val is not None:
-            self.settings[settings_key] = default_val
-            key_is_set = True
-            logger.debug(
-                f"Parameter {settings_key} set to "
-                f'"{self.settings[settings_key]}" '
-                "from default value"
-            )
-
-        if not key_is_set:
-            logger.debug(f"Parameter {settings_key} is not set")
-
-    def _parse_config(self, config_file):
-        """Provide consistent mechanism for pulling in configuration.
-
-        Attempt to retain backward compatibility for
-        existing implementations by grabbing port
-        setting from CLI first.
-
-        Take settings in the following order:
-
-        1. CLI arguments if present
-        2. config file
-        3. OS environment variables (for ease of
-           setting defaults if not present)
-        4. current defaults if a setting is not present in any location
-
-        Additionally provide similar configuration capabilities in between
-        config file and environment variables.
-        For consistency use the same variable name in the config file as
-        in the os environment.
-        For naming standards use all capitals and start with 'TABPY_'
-        """
-        self.settings = {}
-        self.subdirectory = ""
-        self.tabpy_state = None
-        self.python_service = None
-        self.credentials = {}
-
-        pkg_path = os.path.dirname(tabpy.__file__)
-
-        parser = configparser.ConfigParser(os.environ)
-        logger.info(f"Parsing config file {config_file}")
-
-        file_exists = False
-        if os.path.isfile(config_file):
-            try:
-                with open(config_file, 'r') as f:
-                    parser.read_string(f.read())
-                    file_exists = True
-            except Exception:
-                pass
-
-        if not file_exists:
-            logger.warning(
-                f"Unable to open config file {config_file}, "
-                "using default settings."
-            )
-
-        settings_parameters = [
-            (SettingsParameters.Port, ConfigParameters.TABPY_PORT, 9004, None),
-            (SettingsParameters.ServerVersion, None, __version__, None),
-            (SettingsParameters.EvaluateEnabled, ConfigParameters.TABPY_EVALUATE_ENABLE,
-             True, parser.getboolean),
-            (SettingsParameters.EvaluateTimeout, ConfigParameters.TABPY_EVALUATE_TIMEOUT,
-             30, parser.getfloat),
-            (SettingsParameters.UploadDir, ConfigParameters.TABPY_QUERY_OBJECT_PATH,
-             os.path.join(pkg_path, "tmp", "query_objects"), None),
-            (SettingsParameters.TransferProtocol, ConfigParameters.TABPY_TRANSFER_PROTOCOL,
-             "http", None),
-            (SettingsParameters.CertificateFile, ConfigParameters.TABPY_CERTIFICATE_FILE,
-             None, None),
-            (SettingsParameters.KeyFile, ConfigParameters.TABPY_KEY_FILE, None, None),
-            (SettingsParameters.StateFilePath, ConfigParameters.TABPY_STATE_PATH,
-             os.path.join(pkg_path, "tabpy_server"), None),
-            (SettingsParameters.StaticPath, ConfigParameters.TABPY_STATIC_PATH,
-             os.path.join(pkg_path, "tabpy_server", "static"), None),
-            (ConfigParameters.TABPY_PWD_FILE, ConfigParameters.TABPY_PWD_FILE, None, None),
-            (SettingsParameters.LogRequestContext, ConfigParameters.TABPY_LOG_DETAILS,
-             "false", None),
-            (SettingsParameters.MaxRequestSizeInMb, ConfigParameters.TABPY_MAX_REQUEST_SIZE_MB,
-             100, None),
-            (SettingsParameters.GzipEnabled, ConfigParameters.TABPY_GZIP_ENABLE,
-             True, parser.getboolean),
-        ]
-
-        for setting, parameter, default_val, parse_function in settings_parameters:
-            self._set_parameter(parser, setting, parameter, default_val, parse_function)
-
-        if not os.path.exists(self.settings[SettingsParameters.UploadDir]):
-            os.makedirs(self.settings[SettingsParameters.UploadDir])
-
-        # set and validate transfer protocol
-        self.settings[SettingsParameters.TransferProtocol] = self.settings[
-            SettingsParameters.TransferProtocol
-        ].lower()
-
-        self._validate_transfer_protocol_settings()
-
-        # if state.ini does not exist try and create it - remove
-        # last dependence on batch/shell script
-        self.settings[SettingsParameters.StateFilePath] = os.path.realpath(
-            os.path.normpath(
-                os.path.expanduser(self.settings[SettingsParameters.StateFilePath])
-            )
-        )
-        state_config, self.tabpy_state = self._build_tabpy_state()
-
-        self.python_service = PythonServiceHandler(PythonService())
-        self.settings["compress_response"] = True
-        self.settings[SettingsParameters.StaticPath] = os.path.abspath(
-            self.settings[SettingsParameters.StaticPath]
-        )
-        logger.debug(
-            f"Static pages folder set to "
-            f'"{self.settings[SettingsParameters.StaticPath]}"'
-        )
-
-        # Set subdirectory from config if applicable
-        if state_config.has_option("Service Info", "Subdirectory"):
-            self.subdirectory = "/" + state_config.get("Service Info", "Subdirectory")
-
-        # If passwords file specified load credentials
-        if ConfigParameters.TABPY_PWD_FILE in self.settings:
-            if not self._parse_pwd_file():
-                msg = (
-                    "Failed to read passwords file "
-                    f"{self.settings[ConfigParameters.TABPY_PWD_FILE]}"
-                )
-                logger.critical(msg)
-                raise RuntimeError(msg)
-        else:
-            logger.info(
-                "Password file is not specified: " "Authentication is not enabled"
-            )
-
-        features = self._get_features()
-        self.settings[SettingsParameters.ApiVersions] = {"v1": {"features": features}}
-
-        self.settings[SettingsParameters.LogRequestContext] = (
-            self.settings[SettingsParameters.LogRequestContext].lower() != "false"
-        )
-        call_context_state = (
-            "enabled"
-            if self.settings[SettingsParameters.LogRequestContext]
-            else "disabled"
-        )
-        logger.info(f"Call context logging is {call_context_state}")
-
-    def _validate_transfer_protocol_settings(self):
-        if SettingsParameters.TransferProtocol not in self.settings:
-            msg = "Missing transfer protocol information."
-            logger.critical(msg)
-            raise RuntimeError(msg)
-
-        protocol = self.settings[SettingsParameters.TransferProtocol]
-
-        if protocol == "http":
-            return
-
-        if protocol != "https":
-            msg = f"Unsupported transfer protocol: {protocol}"
-            logger.critical(msg)
-            raise RuntimeError(msg)
-
-        self._validate_cert_key_state(
-            "The parameter(s) {} must be set.",
-            SettingsParameters.CertificateFile in self.settings,
-            SettingsParameters.KeyFile in self.settings,
-        )
-        cert = self.settings[SettingsParameters.CertificateFile]
-
-        self._validate_cert_key_state(
-            "The parameter(s) {} must point to " "an existing file.",
-            os.path.isfile(cert),
-            os.path.isfile(self.settings[SettingsParameters.KeyFile]),
-        )
-        tabpy.tabpy_server.app.util.validate_cert(cert)
-
-    @staticmethod
-    def _validate_cert_key_state(msg, cert_valid, key_valid):
-        cert_and_key_param = (
-            f"{ConfigParameters.TABPY_CERTIFICATE_FILE} and "
-            f"{ConfigParameters.TABPY_KEY_FILE}"
-        )
-        https_error = "Error using HTTPS: "
-        err = None
-        if not cert_valid and not key_valid:
-            err = https_error + msg.format(cert_and_key_param)
-        elif not cert_valid:
-            err = https_error + msg.format(ConfigParameters.TABPY_CERTIFICATE_FILE)
-        elif not key_valid:
-            err = https_error + msg.format(ConfigParameters.TABPY_KEY_FILE)
-
-        if err is not None:
-            logger.critical(err)
-            raise RuntimeError(err)
-
-    def _parse_pwd_file(self):
-        succeeded, self.credentials = parse_pwd_file(
-            self.settings[ConfigParameters.TABPY_PWD_FILE]
-        )
-
-        if succeeded and len(self.credentials) == 0:
-            logger.error("No credentials found")
-            succeeded = False
-
-        return succeeded
-
-    def _get_features(self):
-        features = {}
-
-        # Check for auth
-        if ConfigParameters.TABPY_PWD_FILE in self.settings:
-            features["authentication"] = {
-                "required": True,
-                "methods": {"basic-auth": {}},
-            }
-
-        features["evaluate_enabled"] = self.settings[SettingsParameters.EvaluateEnabled]
-        features["gzip_enabled"] = self.settings[SettingsParameters.GzipEnabled]
-        return features
-
-    def _build_tabpy_state(self):
-        pkg_path = os.path.dirname(tabpy.__file__)
-        state_file_dir = self.settings[SettingsParameters.StateFilePath]
-        state_file_path = os.path.join(state_file_dir, "state.ini")
-        if not os.path.isfile(state_file_path):
-            state_file_template_path = os.path.join(
-                pkg_path, "tabpy_server", "state.ini.template"
-            )
-            logger.debug(
-                f"File {state_file_path} not found, creating from "
-                f"template {state_file_template_path}..."
-            )
-            shutil.copy(state_file_template_path, state_file_path)
-
-        logger.info(f"Loading state from state file {state_file_path}")
-        tabpy_state = _get_state_from_file(state_file_dir)
-        return tabpy_state, TabPyState(config=tabpy_state, settings=self.settings)
+import concurrent.futures
+import configparser
+import logging
+import multiprocessing
+import os
+import shutil
+import signal
+import sys
+import tabpy
+from tabpy.tabpy import __version__
+from tabpy.tabpy_server.app.app_parameters import ConfigParameters, SettingsParameters
+from tabpy.tabpy_server.app.util import parse_pwd_file
+from tabpy.tabpy_server.handlers.basic_auth_server_middleware_factory import BasicAuthServerMiddlewareFactory
+from tabpy.tabpy_server.handlers.no_op_auth_handler import NoOpAuthHandler
+from tabpy.tabpy_server.management.state import TabPyState
+from tabpy.tabpy_server.management.util import _get_state_from_file
+from tabpy.tabpy_server.psws.callbacks import init_model_evaluator, init_ps_server
+from tabpy.tabpy_server.psws.python_service import PythonService, PythonServiceHandler
+from tabpy.tabpy_server.handlers import (
+    EndpointHandler,
+    EndpointsHandler,
+    EvaluationPlaneHandler,
+    EvaluationPlaneDisabledHandler,
+    QueryPlaneHandler,
+    ServiceInfoHandler,
+    StatusHandler,
+    UploadDestinationHandler,
+)
+import tornado
+import tabpy.tabpy_server.app.arrow_server as pa
+import _thread
+
+logger = logging.getLogger(__name__)
+
+def _init_asyncio_patch():
+    """
+    Select compatible event loop for Tornado 5+.
+    As of Python 3.8, the default event loop on Windows is `proactor`,
+    however Tornado requires the old default "selector" event loop.
+    As Tornado has decided to leave this to users to set, MkDocs needs
+    to set it. See https://github.com/tornadoweb/tornado/issues/2608.
+    """
+    if sys.platform.startswith("win") and sys.version_info >= (3, 8):
+        import asyncio
+        try:
+            from asyncio import WindowsSelectorEventLoopPolicy
+        except ImportError:
+            pass  # Can't assign a policy which doesn't exist.
+        else:
+            if not isinstance(asyncio.get_event_loop_policy(), WindowsSelectorEventLoopPolicy):
+                asyncio.set_event_loop_policy(WindowsSelectorEventLoopPolicy())
+
+
+class TabPyApp:
+    """
+    TabPy application class for keeping context like settings, state, etc.
+    """
+
+    settings = {}
+    subdirectory = ""
+    tabpy_state = None
+    python_service = None
+    credentials = {}
+    arrow_server = None
+
+    def __init__(self, config_file):
+        if config_file is None:
+            config_file = os.path.join(
+                os.path.dirname(__file__), os.path.pardir, "common", "default.conf"
+            )
+
+        if os.path.isfile(config_file):
+            try:
+                from logging import config
+                config.fileConfig(config_file, disable_existing_loggers=False)
+            except KeyError:
+                logging.basicConfig(level=logging.DEBUG)
+
+        self._parse_config(config_file)
+
+    def _get_tls_certificates(self, config):
+        tls_certificates = []
+        cert = config[SettingsParameters.CertificateFile]
+        key = config[SettingsParameters.KeyFile]
+        with open(cert, "rb") as cert_file:
+            tls_cert_chain = cert_file.read()
+        with open(key, "rb") as key_file:
+            tls_private_key = key_file.read()
+        tls_certificates.append((tls_cert_chain, tls_private_key))
+        return tls_certificates
+    
+    def _get_arrow_server(self, config):
+        verify_client = None
+        tls_certificates = None
+        scheme = "grpc+tcp"
+        if config[SettingsParameters.TransferProtocol] == "https":
+            scheme = "grpc+tls"
+            tls_certificates = self._get_tls_certificates(config)
+
+        host = "localhost"
+        port = config.get(SettingsParameters.ArrowFlightPort)
+        location = "{}://{}:{}".format(scheme, host, port)
+
+        auth_middleware = None
+        if "authentication" in config[SettingsParameters.ApiVersions]["v1"]["features"]:
+            _, creds = parse_pwd_file(config[ConfigParameters.TABPY_PWD_FILE])
+            auth_middleware = {
+                "basic": BasicAuthServerMiddlewareFactory(creds)
+            }
+
+        server = pa.FlightServer(host, location,
+                            tls_certificates=tls_certificates,
+                            verify_client=verify_client, auth_handler=NoOpAuthHandler(),
+                            middleware=auth_middleware)
+        return server
+
+    def run(self):
+        application = self._create_tornado_web_app()
+        max_request_size = (
+            int(self.settings[SettingsParameters.MaxRequestSizeInMb]) * 1024 * 1024
+        )
+        logger.info(f"Setting max request size to {max_request_size} bytes")
+
+        init_model_evaluator(self.settings, self.tabpy_state, self.python_service)
+
+        protocol = self.settings[SettingsParameters.TransferProtocol]
+        ssl_options = None
+        if protocol == "https":
+            ssl_options = {
+                "certfile": self.settings[SettingsParameters.CertificateFile],
+                "keyfile": self.settings[SettingsParameters.KeyFile],
+            }
+        elif protocol != "http":
+            msg = f"Unsupported transfer protocol {protocol}."
+            logger.critical(msg)
+            raise RuntimeError(msg)
+
+        settings = {}
+        if self.settings[SettingsParameters.GzipEnabled] is True:
+            settings["decompress_request"] = True
+
+        application.listen(
+            self.settings[SettingsParameters.Port],
+            ssl_options=ssl_options,
+            max_buffer_size=max_request_size,
+            max_body_size=max_request_size,
+            **settings,
+        ) 
+
+        logger.info(
+            "Web service listening on port "
+            f"{str(self.settings[SettingsParameters.Port])}"
+        )
+
+        if self.settings[SettingsParameters.ArrowEnabled]:
+            def start_pyarrow():
+                self.arrow_server = self._get_arrow_server(self.settings)
+                pa.start(self.arrow_server)
+
+            try:
+                _thread.start_new_thread(start_pyarrow, ())
+            except Exception as e:
+                logger.critical(f"Failed to start PyArrow server: {e}")
+
+        tornado.ioloop.IOLoop.instance().start()
+
+    def _create_tornado_web_app(self):
+        class TabPyTornadoApp(tornado.web.Application):
+            is_closing = False
+
+            def signal_handler(self, signal, _):
+                logger.critical(f"Exiting on signal {signal}...")
+                self.is_closing = True
+
+            def try_exit(self):
+                if self.is_closing:
+                    tornado.ioloop.IOLoop.instance().stop()
+                    logger.info("Shutting down TabPy...")
+
+        logger.info("Initializing TabPy...")
+        tornado.ioloop.IOLoop.instance().run_sync(
+            lambda: init_ps_server(self.settings, self.tabpy_state)
+        )
+        logger.info("Done initializing TabPy.")
+
+        executor = concurrent.futures.ThreadPoolExecutor(
+            max_workers=multiprocessing.cpu_count()
+        )
+
+        # initialize Tornado application
+        _init_asyncio_patch()
+        application = TabPyTornadoApp(
+            [
+                (
+                    self.subdirectory + r"/query/([^/]+)",
+                    QueryPlaneHandler,
+                    dict(app=self),
+                ),
+                (self.subdirectory + r"/status", StatusHandler, dict(app=self)),
+                (self.subdirectory + r"/info", ServiceInfoHandler, dict(app=self)),
+                (self.subdirectory + r"/endpoints", EndpointsHandler, dict(app=self)),
+                (
+                    self.subdirectory + r"/endpoints/([^/]+)?",
+                    EndpointHandler,
+                    dict(app=self),
+                ),
+                (
+                    self.subdirectory + r"/evaluate",
+                    EvaluationPlaneHandler if self.settings[SettingsParameters.EvaluateEnabled]
+                    else EvaluationPlaneDisabledHandler,
+                    dict(executor=executor, app=self),
+                ),
+                (
+                    self.subdirectory + r"/configurations/endpoint_upload_destination",
+                    UploadDestinationHandler,
+                    dict(app=self),
+                ),
+                (
+                    self.subdirectory + r"/(.*)",
+                    tornado.web.StaticFileHandler,
+                    dict(
+                        path=self.settings[SettingsParameters.StaticPath],
+                        default_filename="index.html",
+                    ),
+                ),
+            ],
+            debug=False,
+            **self.settings,
+        )
+
+        signal.signal(signal.SIGINT, application.signal_handler)
+        tornado.ioloop.PeriodicCallback(application.try_exit, 500).start()
+
+        signal.signal(signal.SIGINT, application.signal_handler)
+        tornado.ioloop.PeriodicCallback(application.try_exit, 500).start()
+
+        return application
+
+    def _set_parameter(self, parser, settings_key, config_key, default_val, parse_function):
+        key_is_set = False
+
+        if (
+            config_key is not None
+            and parser.has_section("TabPy")
+            and parser.has_option("TabPy", config_key)
+        ):
+            if parse_function is None:
+                parse_function = parser.get
+            self.settings[settings_key] = parse_function("TabPy", config_key)
+            key_is_set = True
+            logger.debug(
+                f"Parameter {settings_key} set to "
+                f'"{self.settings[settings_key]}" '
+                "from config file or environment variable"
+            )
+
+        if not key_is_set and default_val is not None:
+            self.settings[settings_key] = default_val
+            key_is_set = True
+            logger.debug(
+                f"Parameter {settings_key} set to "
+                f'"{self.settings[settings_key]}" '
+                "from default value"
+            )
+
+        if not key_is_set:
+            logger.debug(f"Parameter {settings_key} is not set")
+
+    def _parse_config(self, config_file):
+        """Provide consistent mechanism for pulling in configuration.
+
+        Attempt to retain backward compatibility for
+        existing implementations by grabbing port
+        setting from CLI first.
+
+        Take settings in the following order:
+
+        1. CLI arguments if present
+        2. config file
+        3. OS environment variables (for ease of
+           setting defaults if not present)
+        4. current defaults if a setting is not present in any location
+
+        Additionally provide similar configuration capabilities in between
+        config file and environment variables.
+        For consistency use the same variable name in the config file as
+        in the os environment.
+        For naming standards use all capitals and start with 'TABPY_'
+        """
+        self.settings = {}
+        self.subdirectory = ""
+        self.tabpy_state = None
+        self.python_service = None
+        self.credentials = {}
+
+        pkg_path = os.path.dirname(tabpy.__file__)
+
+        parser = configparser.ConfigParser(os.environ)
+        logger.info(f"Parsing config file {config_file}")
+
+        file_exists = False
+        if os.path.isfile(config_file):
+            try:
+                with open(config_file, 'r') as f:
+                    parser.read_string(f.read())
+                    file_exists = True
+            except Exception:
+                pass
+
+        if not file_exists:
+            logger.warning(
+                f"Unable to open config file {config_file}, "
+                "using default settings."
+            )
+
+        settings_parameters = [
+            (SettingsParameters.Port, ConfigParameters.TABPY_PORT, 9004, None),
+            (SettingsParameters.ServerVersion, None, __version__, None),
+            (SettingsParameters.EvaluateEnabled, ConfigParameters.TABPY_EVALUATE_ENABLE,
+             True, parser.getboolean),
+            (SettingsParameters.EvaluateTimeout, ConfigParameters.TABPY_EVALUATE_TIMEOUT,
+             30, parser.getfloat),
+            (SettingsParameters.UploadDir, ConfigParameters.TABPY_QUERY_OBJECT_PATH,
+             os.path.join(pkg_path, "tmp", "query_objects"), None),
+            (SettingsParameters.TransferProtocol, ConfigParameters.TABPY_TRANSFER_PROTOCOL,
+             "http", None),
+            (SettingsParameters.CertificateFile, ConfigParameters.TABPY_CERTIFICATE_FILE,
+             None, None),
+            (SettingsParameters.KeyFile, ConfigParameters.TABPY_KEY_FILE, None, None),
+            (SettingsParameters.StateFilePath, ConfigParameters.TABPY_STATE_PATH,
+             os.path.join(pkg_path, "tabpy_server"), None),
+            (SettingsParameters.StaticPath, ConfigParameters.TABPY_STATIC_PATH,
+             os.path.join(pkg_path, "tabpy_server", "static"), None),
+            (ConfigParameters.TABPY_PWD_FILE, ConfigParameters.TABPY_PWD_FILE, None, None),
+            (SettingsParameters.LogRequestContext, ConfigParameters.TABPY_LOG_DETAILS,
+             "false", None),
+            (SettingsParameters.MaxRequestSizeInMb, ConfigParameters.TABPY_MAX_REQUEST_SIZE_MB,
+             100, None),
+            (SettingsParameters.GzipEnabled, ConfigParameters.TABPY_GZIP_ENABLE,
+             True, parser.getboolean),
+            (SettingsParameters.ArrowEnabled, ConfigParameters.TABPY_ARROW_ENABLE, False, parser.getboolean), 
+            (SettingsParameters.ArrowFlightPort, ConfigParameters.TABPY_ARROWFLIGHT_PORT, 13622, parser.getint),
+        ]
+
+        for setting, parameter, default_val, parse_function in settings_parameters:
+            self._set_parameter(parser, setting, parameter, default_val, parse_function)
+
+        if not os.path.exists(self.settings[SettingsParameters.UploadDir]):
+            os.makedirs(self.settings[SettingsParameters.UploadDir])
+
+        # set and validate transfer protocol
+        self.settings[SettingsParameters.TransferProtocol] = self.settings[
+            SettingsParameters.TransferProtocol
+        ].lower()
+
+        self._validate_transfer_protocol_settings()
+
+        # if state.ini does not exist try and create it - remove
+        # last dependence on batch/shell script
+        self.settings[SettingsParameters.StateFilePath] = os.path.realpath(
+            os.path.normpath(
+                os.path.expanduser(self.settings[SettingsParameters.StateFilePath])
+            )
+        )
+        state_config, self.tabpy_state = self._build_tabpy_state()
+
+        self.python_service = PythonServiceHandler(PythonService())
+        self.settings["compress_response"] = True
+        self.settings[SettingsParameters.StaticPath] = os.path.abspath(
+            self.settings[SettingsParameters.StaticPath]
+        )
+        logger.debug(
+            f"Static pages folder set to "
+            f'"{self.settings[SettingsParameters.StaticPath]}"'
+        )
+
+        # Set subdirectory from config if applicable
+        if state_config.has_option("Service Info", "Subdirectory"):
+            self.subdirectory = "/" + state_config.get("Service Info", "Subdirectory")
+
+        # If passwords file specified load credentials
+        if ConfigParameters.TABPY_PWD_FILE in self.settings:
+            if not self._parse_pwd_file():
+                msg = (
+                    "Failed to read passwords file "
+                    f"{self.settings[ConfigParameters.TABPY_PWD_FILE]}"
+                )
+                logger.critical(msg)
+                raise RuntimeError(msg)
+        else:
+            logger.info(
+                "Password file is not specified: " "Authentication is not enabled"
+            )
+
+        features = self._get_features()
+        self.settings[SettingsParameters.ApiVersions] = {"v1": {"features": features}}
+
+        self.settings[SettingsParameters.LogRequestContext] = (
+            self.settings[SettingsParameters.LogRequestContext].lower() != "false"
+        )
+        call_context_state = (
+            "enabled"
+            if self.settings[SettingsParameters.LogRequestContext]
+            else "disabled"
+        )
+        logger.info(f"Call context logging is {call_context_state}")
+
+    def _validate_transfer_protocol_settings(self):
+        if SettingsParameters.TransferProtocol not in self.settings:
+            msg = "Missing transfer protocol information."
+            logger.critical(msg)
+            raise RuntimeError(msg)
+
+        protocol = self.settings[SettingsParameters.TransferProtocol]
+
+        if protocol == "http":
+            return
+
+        if protocol != "https":
+            msg = f"Unsupported transfer protocol: {protocol}"
+            logger.critical(msg)
+            raise RuntimeError(msg)
+
+        self._validate_cert_key_state(
+            "The parameter(s) {} must be set.",
+            SettingsParameters.CertificateFile in self.settings,
+            SettingsParameters.KeyFile in self.settings,
+        )
+        cert = self.settings[SettingsParameters.CertificateFile]
+
+        self._validate_cert_key_state(
+            "The parameter(s) {} must point to " "an existing file.",
+            os.path.isfile(cert),
+            os.path.isfile(self.settings[SettingsParameters.KeyFile]),
+        )
+        tabpy.tabpy_server.app.util.validate_cert(cert)
+
+    @staticmethod
+    def _validate_cert_key_state(msg, cert_valid, key_valid):
+        cert_and_key_param = (
+            f"{ConfigParameters.TABPY_CERTIFICATE_FILE} and "
+            f"{ConfigParameters.TABPY_KEY_FILE}"
+        )
+        https_error = "Error using HTTPS: "
+        err = None
+        if not cert_valid and not key_valid:
+            err = https_error + msg.format(cert_and_key_param)
+        elif not cert_valid:
+            err = https_error + msg.format(ConfigParameters.TABPY_CERTIFICATE_FILE)
+        elif not key_valid:
+            err = https_error + msg.format(ConfigParameters.TABPY_KEY_FILE)
+
+        if err is not None:
+            logger.critical(err)
+            raise RuntimeError(err)
+
+    def _parse_pwd_file(self):
+        succeeded, self.credentials = parse_pwd_file(
+            self.settings[ConfigParameters.TABPY_PWD_FILE]
+        )
+
+        if succeeded and len(self.credentials) == 0:
+            logger.error("No credentials found")
+            succeeded = False
+
+        return succeeded
+
+    def _get_features(self):
+        features = {}
+
+        # Check for auth
+        if ConfigParameters.TABPY_PWD_FILE in self.settings:
+            features["authentication"] = {
+                "required": True,
+                "methods": {"basic-auth": {}},
+            }
+
+        features["evaluate_enabled"] = self.settings[SettingsParameters.EvaluateEnabled]
+        features["gzip_enabled"] = self.settings[SettingsParameters.GzipEnabled]
+        features["arrow_enabled"] = self.settings[SettingsParameters.ArrowEnabled]
+        return features
+
+    def _build_tabpy_state(self):
+        pkg_path = os.path.dirname(tabpy.__file__)
+        state_file_dir = self.settings[SettingsParameters.StateFilePath]
+        state_file_path = os.path.join(state_file_dir, "state.ini")
+        if not os.path.isfile(state_file_path):
+            state_file_template_path = os.path.join(
+                pkg_path, "tabpy_server", "state.ini.template"
+            )
+            logger.debug(
+                f"File {state_file_path} not found, creating from "
+                f"template {state_file_template_path}..."
+            )
+            shutil.copy(state_file_template_path, state_file_path)
+
+        logger.info(f"Loading state from state file {state_file_path}")
+        tabpy_state = _get_state_from_file(state_file_dir)
+        return tabpy_state, TabPyState(config=tabpy_state, settings=self.settings)
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/app/util.py` & `tabpy-2.7.0/tabpy/tabpy_server/app/util.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import csv
-from datetime import datetime
-import logging
-from OpenSSL import crypto
-import os
-
-
-logger = logging.getLogger(__name__)
-
-
-def validate_cert(cert_file_path):
-    with open(cert_file_path, "r") as f:
-        cert_buf = f.read()
-
-    cert = crypto.load_certificate(crypto.FILETYPE_PEM, cert_buf)
-
-    date_format, encoding = "%Y%m%d%H%M%SZ", "ascii"
-    not_before = datetime.strptime(cert.get_notBefore().decode(encoding), date_format)
-    not_after = datetime.strptime(cert.get_notAfter().decode(encoding), date_format)
-    now = datetime.now()
-
-    https_error = "Error using HTTPS: "
-    if now < not_before:
-        msg = https_error + f"The certificate provided is not valid until {not_before}."
-        logger.critical(msg)
-        raise RuntimeError(msg)
-    if now > not_after:
-        msg = https_error + f"The certificate provided expired on {not_after}."
-        logger.critical(msg)
-        raise RuntimeError(msg)
-
-
-def parse_pwd_file(pwd_file_name):
-    """
-    Parses passwords file and returns set of credentials.
-
-    Parameters
-    ----------
-    pwd_file_name : str
-        Passwords file name.
-
-    Returns
-    -------
-    succeeded : bool
-        True if specified file was parsed successfully.
-        False if there were any issues with parsing specified file.
-
-    credentials : dict
-        Credentials from the file. Empty if succeeded is False.
-    """
-    logger.info(f"Parsing passwords file {pwd_file_name}...")
-
-    if not os.path.isfile(pwd_file_name):
-        logger.critical(f"Passwords file {pwd_file_name} not found")
-        return False, {}
-
-    credentials = {}
-    with open(pwd_file_name) as pwd_file:
-        pwd_file_reader = csv.reader(pwd_file, delimiter=" ")
-        for row in pwd_file_reader:
-            # skip empty lines
-            if len(row) == 0:
-                continue
-
-            # skip commented lines
-            if row[0][0] == "#":
-                continue
-
-            if len(row) != 2:
-                logger.error(f'Incorrect entry "{row}" in password file')
-                return False, {}
-
-            login = row[0].lower()
-            if login in credentials:
-                logger.error(
-                    f"Multiple entries for username {login} in password file"
-                )
-                return False, {}
-
-            if len(row[1]) > 0:
-                credentials[login] = row[1]
-                logger.debug(f"Found username {login}")
-            else:
-                logger.warning(f"Found username {row[0]} but no password")
-                return False, {}
-
-    logger.info("Authentication is enabled")
-    return True, credentials
+import csv
+from datetime import datetime
+import logging
+from OpenSSL import crypto
+import os
+
+
+logger = logging.getLogger(__name__)
+
+
+def validate_cert(cert_file_path):
+    with open(cert_file_path, "r") as f:
+        cert_buf = f.read()
+
+    cert = crypto.load_certificate(crypto.FILETYPE_PEM, cert_buf)
+
+    date_format, encoding = "%Y%m%d%H%M%SZ", "ascii"
+    not_before = datetime.strptime(cert.get_notBefore().decode(encoding), date_format)
+    not_after = datetime.strptime(cert.get_notAfter().decode(encoding), date_format)
+    now = datetime.now()
+
+    https_error = "Error using HTTPS: "
+    if now < not_before:
+        msg = https_error + f"The certificate provided is not valid until {not_before}."
+        logger.critical(msg)
+        raise RuntimeError(msg)
+    if now > not_after:
+        msg = https_error + f"The certificate provided expired on {not_after}."
+        logger.critical(msg)
+        raise RuntimeError(msg)
+
+
+def parse_pwd_file(pwd_file_name):
+    """
+    Parses passwords file and returns set of credentials.
+
+    Parameters
+    ----------
+    pwd_file_name : str
+        Passwords file name.
+
+    Returns
+    -------
+    succeeded : bool
+        True if specified file was parsed successfully.
+        False if there were any issues with parsing specified file.
+
+    credentials : dict
+        Credentials from the file. Empty if succeeded is False.
+    """
+    logger.info(f"Parsing passwords file {pwd_file_name}...")
+
+    if not os.path.isfile(pwd_file_name):
+        logger.critical(f"Passwords file {pwd_file_name} not found")
+        return False, {}
+
+    credentials = {}
+    with open(pwd_file_name) as pwd_file:
+        pwd_file_reader = csv.reader(pwd_file, delimiter=" ")
+        for row in pwd_file_reader:
+            # skip empty lines
+            if len(row) == 0:
+                continue
+
+            # skip commented lines
+            if row[0][0] == "#":
+                continue
+
+            if len(row) != 2:
+                logger.error(f'Incorrect entry "{row}" in password file')
+                return False, {}
+
+            login = row[0].lower()
+            if login in credentials:
+                logger.error(
+                    f"Multiple entries for username {login} in password file"
+                )
+                return False, {}
+
+            if len(row[1]) > 0:
+                credentials[login] = row[1]
+                logger.debug(f"Found username {login}")
+            else:
+                logger.warning(f"Found username {row[0]} but no password")
+                return False, {}
+
+    logger.info("Authentication is enabled")
+    return True, credentials
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/common/default.conf` & `tabpy-2.7.0/tabpy/tabpy_server/common/default.conf`

 * *Files 18% similar despite different names*

```diff
@@ -1,120 +1,125 @@
-00000000: 5b54 6162 5079 5d0a 2320 5441 4250 595f  [TabPy].# TABPY_
-00000010: 5155 4552 595f 4f42 4a45 4354 5f50 4154  QUERY_OBJECT_PAT
-00000020: 4820 3d20 2f74 6d70 2f71 7565 7279 5f6f  H = /tmp/query_o
-00000030: 626a 6563 7473 0a23 2054 4142 5059 5f50  bjects.# TABPY_P
-00000040: 4f52 5420 3d20 3930 3034 0a23 2054 4142  ORT = 9004.# TAB
-00000050: 5059 5f53 5441 5445 5f50 4154 4820 3d20  PY_STATE_PATH = 
-00000060: 2e2f 7461 6270 792f 7461 6270 795f 7365  ./tabpy/tabpy_se
-00000070: 7276 6572 0a0a 2320 5768 6572 6520 7374  rver..# Where st
-00000080: 6174 6963 2070 6167 6573 206c 6976 650a  atic pages live.
-00000090: 2320 5441 4250 595f 5354 4154 4943 5f50  # TABPY_STATIC_P
-000000a0: 4154 4820 3d20 2e2f 7461 6270 792f 7461  ATH = ./tabpy/ta
-000000b0: 6270 795f 7365 7276 6572 2f73 7461 7469  bpy_server/stati
-000000c0: 630a 0a23 2046 6f72 2068 6f77 2074 6f20  c..# For how to 
-000000d0: 636f 6e66 6967 7572 6520 5461 6250 7920  configure TabPy 
-000000e0: 6175 7468 656e 7469 6361 7469 6f6e 2072  authentication r
-000000f0: 6561 640a 2320 4175 7468 656e 7469 6361  ead.# Authentica
-00000100: 7469 6f6e 2073 6563 7469 6f6e 2069 6e20  tion section in 
-00000110: 646f 6373 2f73 6572 7665 722d 636f 6e66  docs/server-conf
-00000120: 6967 2e6d 642e 0a23 2054 4142 5059 5f50  ig.md..# TABPY_P
-00000130: 5744 5f46 494c 4520 3d20 2f70 6174 682f  WD_FILE = /path/
-00000140: 746f 2f70 6173 7377 6f72 642f 6669 6c65  to/password/file
-00000150: 2e74 7874 0a0a 2320 546f 2073 6574 2075  .txt..# To set u
-00000160: 7020 7365 6375 7265 2054 6162 5079 2075  p secure TabPy u
-00000170: 6e63 6f6d 6d65 6e74 2061 6e64 206d 6f64  ncomment and mod
-00000180: 6966 7920 7468 6520 666f 6c6c 6f77 696e  ify the followin
-00000190: 6720 6c69 6e65 732e 0a23 204e 6f74 6520  g lines..# Note 
-000001a0: 6f6e 6c79 2050 454d 2d65 6e63 6f64 6564  only PEM-encoded
-000001b0: 2078 3530 3920 6365 7274 6966 6963 6174   x509 certificat
-000001c0: 6573 2061 7265 2073 7570 706f 7274 6564  es are supported
-000001d0: 2e0a 2320 5441 4250 595f 5452 414e 5346  ..# TABPY_TRANSF
-000001e0: 4552 5f50 524f 544f 434f 4c20 3d20 6874  ER_PROTOCOL = ht
-000001f0: 7470 730a 2320 5441 4250 595f 4345 5254  tps.# TABPY_CERT
-00000200: 4946 4943 4154 455f 4649 4c45 203d 202f  IFICATE_FILE = /
-00000210: 7061 7468 2f74 6f2f 6365 7274 6966 6963  path/to/certific
-00000220: 6174 652f 6669 6c65 2e63 7274 0a23 2054  ate/file.crt.# T
-00000230: 4142 5059 5f4b 4559 5f46 494c 4520 3d20  ABPY_KEY_FILE = 
-00000240: 2f70 6174 682f 746f 2f6b 6579 2f66 696c  /path/to/key/fil
-00000250: 652e 6b65 790a 0a23 204c 6f67 2061 6464  e.key..# Log add
-00000260: 6974 696f 6e61 6c20 7265 7175 6573 7420  itional request 
-00000270: 6465 7461 696c 7320 696e 636c 7564 696e  details includin
-00000280: 6720 6361 6c6c 6572 2049 502c 2066 756c  g caller IP, ful
-00000290: 6c20 5552 4c2c 2063 6c69 656e 740a 2320  l URL, client.# 
-000002a0: 656e 6420 7573 6572 2069 6e66 6f20 6966  end user info if
-000002b0: 2070 726f 7669 6465 642e 0a23 2054 4142   provided..# TAB
-000002c0: 5059 5f4c 4f47 5f44 4554 4149 4c53 203d  PY_LOG_DETAILS =
-000002d0: 2074 7275 650a 0a23 204c 696d 6974 2072   true..# Limit r
-000002e0: 6571 7565 7374 2073 697a 6520 2869 6e20  equest size (in 
-000002f0: 4d62 2920 2d20 616e 7920 7265 7175 6573  Mb) - any reques
-00000300: 7420 7768 6963 6820 7369 7a65 2065 7863  t which size exc
-00000310: 6565 6473 0a23 2073 7065 6369 6669 6564  eeds.# specified
-00000320: 2061 6d6f 756e 7420 7769 6c6c 2062 6520   amount will be 
-00000330: 7265 6a65 6374 6564 2062 7920 5461 6250  rejected by TabP
-00000340: 792e 0a23 2044 6566 6175 6c74 2076 616c  y..# Default val
-00000350: 7565 2069 7320 3130 3020 4d62 2e0a 2320  ue is 100 Mb..# 
-00000360: 5441 4250 595f 4d41 585f 5245 5155 4553  TABPY_MAX_REQUES
-00000370: 545f 5349 5a45 5f4d 4220 3d20 3130 300a  T_SIZE_MB = 100.
-00000380: 0a23 2045 6e61 626c 6520 6576 616c 7561  .# Enable evalua
-00000390: 7465 2061 7069 2074 6f20 6578 6563 7574  te api to execut
-000003a0: 6520 6164 2d68 6f63 2050 7974 686f 6e20  e ad-hoc Python 
-000003b0: 7363 7269 7074 730a 2320 456e 6162 6c65  scripts.# Enable
-000003c0: 6420 6279 2064 6566 6175 6c74 2e20 4469  d by default. Di
-000003d0: 7361 626c 696e 6720 6974 2077 696c 6c20  sabling it will 
-000003e0: 7265 7375 6c74 2069 6e20 3430 3420 6572  result in 404 er
-000003f0: 726f 722e 0a23 2054 4142 5059 5f45 5641  ror..# TABPY_EVA
-00000400: 4c55 4154 455f 454e 4142 4c45 203d 2074  LUATE_ENABLE = t
-00000410: 7275 650a 0a23 2043 6f6e 6669 6775 7265  rue..# Configure
-00000420: 2068 6f77 206c 6f6e 6720 6120 6375 7374   how long a cust
-00000430: 6f6d 2073 6372 6970 7420 7072 6f76 6964  om script provid
-00000440: 6564 2074 6f20 7468 6520 2f65 7661 6c75  ed to the /evalu
-00000450: 6174 6520 6d65 7468 6f64 0a23 2077 696c  ate method.# wil
-00000460: 6c20 7275 6e20 6265 666f 7265 2074 6872  l run before thr
-00000470: 6f77 696e 6720 6120 5469 6d65 6f75 7445  owing a TimeoutE
-00000480: 7272 6f72 2e0a 2320 5468 6520 7661 6c75  rror..# The valu
-00000490: 6520 7368 6f75 6c64 2062 6520 6120 666c  e should be a fl
-000004a0: 6f61 7420 7265 7072 6573 656e 7469 6e67  oat representing
-000004b0: 2074 6865 2074 696d 656f 7574 2074 696d   the timeout tim
-000004c0: 6520 696e 2073 6563 6f6e 6473 2e0a 2320  e in seconds..# 
-000004d0: 5441 4250 595f 4556 414c 5541 5445 5f54  TABPY_EVALUATE_T
-000004e0: 494d 454f 5554 203d 2033 300a 0a23 2045  IMEOUT = 30..# E
-000004f0: 6e61 626c 6520 477a 6970 2063 6f6d 7072  nable Gzip compr
-00000500: 6573 7369 6f6e 2066 6f72 2072 6571 7565  ession for reque
-00000510: 7374 7320 616e 6420 7265 7370 6f6e 7365  sts and response
-00000520: 732e 0a23 2054 4142 5059 5f47 5a49 505f  s..# TABPY_GZIP_
-00000530: 454e 4142 4c45 203d 2074 7275 650a 0a5b  ENABLE = true..[
-00000540: 6c6f 6767 6572 735d 0a6b 6579 733d 726f  loggers].keys=ro
-00000550: 6f74 0a0a 5b68 616e 646c 6572 735d 0a6b  ot..[handlers].k
-00000560: 6579 733d 726f 6f74 4861 6e64 6c65 722c  eys=rootHandler,
-00000570: 726f 7461 7469 6e67 4669 6c65 4861 6e64  rotatingFileHand
-00000580: 6c65 720a 0a5b 666f 726d 6174 7465 7273  ler..[formatters
-00000590: 5d0a 6b65 7973 3d72 6f6f 7446 6f72 6d61  ].keys=rootForma
-000005a0: 7474 6572 0a0a 5b6c 6f67 6765 725f 726f  tter..[logger_ro
-000005b0: 6f74 5d0a 6c65 7665 6c3d 4445 4255 470a  ot].level=DEBUG.
-000005c0: 6861 6e64 6c65 7273 3d72 6f6f 7448 616e  handlers=rootHan
-000005d0: 646c 6572 2c72 6f74 6174 696e 6746 696c  dler,rotatingFil
-000005e0: 6548 616e 646c 6572 0a71 7561 6c6e 616d  eHandler.qualnam
-000005f0: 653d 726f 6f74 0a70 726f 7061 6765 7465  e=root.propagete
-00000600: 3d30 0a0a 5b68 616e 646c 6572 5f72 6f6f  =0..[handler_roo
-00000610: 7448 616e 646c 6572 5d0a 636c 6173 733d  tHandler].class=
-00000620: 5374 7265 616d 4861 6e64 6c65 720a 6c65  StreamHandler.le
-00000630: 7665 6c3d 494e 464f 0a66 6f72 6d61 7474  vel=INFO.formatt
-00000640: 6572 3d72 6f6f 7446 6f72 6d61 7474 6572  er=rootFormatter
-00000650: 0a61 7267 733d 2873 7973 2e73 7464 6f75  .args=(sys.stdou
-00000660: 742c 290a 0a5b 6861 6e64 6c65 725f 726f  t,)..[handler_ro
-00000670: 7461 7469 6e67 4669 6c65 4861 6e64 6c65  tatingFileHandle
-00000680: 725d 0a63 6c61 7373 3d68 616e 646c 6572  r].class=handler
-00000690: 732e 526f 7461 7469 6e67 4669 6c65 4861  s.RotatingFileHa
-000006a0: 6e64 6c65 720a 6c65 7665 6c3d 4445 4255  ndler.level=DEBU
-000006b0: 470a 666f 726d 6174 7465 723d 726f 6f74  G.formatter=root
-000006c0: 466f 726d 6174 7465 720a 6172 6773 3d28  Formatter.args=(
-000006d0: 2774 6162 7079 5f6c 6f67 2e6c 6f67 272c  'tabpy_log.log',
-000006e0: 2027 6127 2c20 3130 3030 3030 302c 2035   'a', 1000000, 5
-000006f0: 290a 0a5b 666f 726d 6174 7465 725f 726f  )..[formatter_ro
-00000700: 6f74 466f 726d 6174 7465 725d 0a66 6f72  otFormatter].for
-00000710: 6d61 743d 2528 6173 6374 696d 6529 7320  mat=%(asctime)s 
-00000720: 5b25 286c 6576 656c 6e61 6d65 2973 5d20  [%(levelname)s] 
-00000730: 2825 2866 696c 656e 616d 6529 733a 2528  (%(filename)s:%(
-00000740: 6d6f 6475 6c65 2973 3a25 286c 696e 656e  module)s:%(linen
-00000750: 6f29 6429 3a20 2528 6d65 7373 6167 6529  o)d): %(message)
-00000760: 730a 6461 7465 666d 743d 2559 2d25 6d2d  s.datefmt=%Y-%m-
-00000770: 2564 2c25 483a 254d 3a25 530a            %d,%H:%M:%S.
+00000000: 5b54 6162 5079 5d0d 0a23 2054 4142 5059  [TabPy]..# TABPY
+00000010: 5f51 5545 5259 5f4f 424a 4543 545f 5041  _QUERY_OBJECT_PA
+00000020: 5448 203d 202f 746d 702f 7175 6572 795f  TH = /tmp/query_
+00000030: 6f62 6a65 6374 730d 0a23 2054 4142 5059  objects..# TABPY
+00000040: 5f50 4f52 5420 3d20 3930 3034 0d0a 2320  _PORT = 9004..# 
+00000050: 5441 4250 595f 5354 4154 455f 5041 5448  TABPY_STATE_PATH
+00000060: 203d 202e 2f74 6162 7079 2f74 6162 7079   = ./tabpy/tabpy
+00000070: 5f73 6572 7665 720d 0a0d 0a23 2057 6865  _server....# Whe
+00000080: 7265 2073 7461 7469 6320 7061 6765 7320  re static pages 
+00000090: 6c69 7665 0d0a 2320 5441 4250 595f 5354  live..# TABPY_ST
+000000a0: 4154 4943 5f50 4154 4820 3d20 2e2f 7461  ATIC_PATH = ./ta
+000000b0: 6270 792f 7461 6270 795f 7365 7276 6572  bpy/tabpy_server
+000000c0: 2f73 7461 7469 630d 0a0d 0a23 2046 6f72  /static....# For
+000000d0: 2068 6f77 2074 6f20 636f 6e66 6967 7572   how to configur
+000000e0: 6520 5461 6250 7920 6175 7468 656e 7469  e TabPy authenti
+000000f0: 6361 7469 6f6e 2072 6561 640d 0a23 2041  cation read..# A
+00000100: 7574 6865 6e74 6963 6174 696f 6e20 7365  uthentication se
+00000110: 6374 696f 6e20 696e 2064 6f63 732f 7365  ction in docs/se
+00000120: 7276 6572 2d63 6f6e 6669 672e 6d64 2e0d  rver-config.md..
+00000130: 0a23 2054 4142 5059 5f50 5744 5f46 494c  .# TABPY_PWD_FIL
+00000140: 4520 3d20 2f70 6174 682f 746f 2f70 6173  E = /path/to/pas
+00000150: 7377 6f72 642f 6669 6c65 2e74 7874 0d0a  sword/file.txt..
+00000160: 0d0a 2320 546f 2073 6574 2075 7020 7365  ..# To set up se
+00000170: 6375 7265 2054 6162 5079 2075 6e63 6f6d  cure TabPy uncom
+00000180: 6d65 6e74 2061 6e64 206d 6f64 6966 7920  ment and modify 
+00000190: 7468 6520 666f 6c6c 6f77 696e 6720 6c69  the following li
+000001a0: 6e65 732e 0d0a 2320 4e6f 7465 206f 6e6c  nes...# Note onl
+000001b0: 7920 5045 4d2d 656e 636f 6465 6420 7835  y PEM-encoded x5
+000001c0: 3039 2063 6572 7469 6669 6361 7465 7320  09 certificates 
+000001d0: 6172 6520 7375 7070 6f72 7465 642e 0d0a  are supported...
+000001e0: 2320 5441 4250 595f 5452 414e 5346 4552  # TABPY_TRANSFER
+000001f0: 5f50 524f 544f 434f 4c20 3d20 6874 7470  _PROTOCOL = http
+00000200: 730d 0a23 2054 4142 5059 5f43 4552 5449  s..# TABPY_CERTI
+00000210: 4649 4341 5445 5f46 494c 4520 3d20 2f70  FICATE_FILE = /p
+00000220: 6174 682f 746f 2f63 6572 7469 6669 6361  ath/to/certifica
+00000230: 7465 2f66 696c 652e 6372 740d 0a23 2054  te/file.crt..# T
+00000240: 4142 5059 5f4b 4559 5f46 494c 4520 3d20  ABPY_KEY_FILE = 
+00000250: 2f70 6174 682f 746f 2f6b 6579 2f66 696c  /path/to/key/fil
+00000260: 652e 6b65 790d 0a0d 0a23 204c 6f67 2061  e.key....# Log a
+00000270: 6464 6974 696f 6e61 6c20 7265 7175 6573  dditional reques
+00000280: 7420 6465 7461 696c 7320 696e 636c 7564  t details includ
+00000290: 696e 6720 6361 6c6c 6572 2049 502c 2066  ing caller IP, f
+000002a0: 756c 6c20 5552 4c2c 2063 6c69 656e 740d  ull URL, client.
+000002b0: 0a23 2065 6e64 2075 7365 7220 696e 666f  .# end user info
+000002c0: 2069 6620 7072 6f76 6964 6564 2e0d 0a23   if provided...#
+000002d0: 2054 4142 5059 5f4c 4f47 5f44 4554 4149   TABPY_LOG_DETAI
+000002e0: 4c53 203d 2074 7275 650d 0a0d 0a23 204c  LS = true....# L
+000002f0: 696d 6974 2072 6571 7565 7374 2073 697a  imit request siz
+00000300: 6520 2869 6e20 4d62 2920 2d20 616e 7920  e (in Mb) - any 
+00000310: 7265 7175 6573 7420 7768 6963 6820 7369  request which si
+00000320: 7a65 2065 7863 6565 6473 0d0a 2320 7370  ze exceeds..# sp
+00000330: 6563 6966 6965 6420 616d 6f75 6e74 2077  ecified amount w
+00000340: 696c 6c20 6265 2072 656a 6563 7465 6420  ill be rejected 
+00000350: 6279 2054 6162 5079 2e0d 0a23 2044 6566  by TabPy...# Def
+00000360: 6175 6c74 2076 616c 7565 2069 7320 3130  ault value is 10
+00000370: 3020 4d62 2e0d 0a23 2054 4142 5059 5f4d  0 Mb...# TABPY_M
+00000380: 4158 5f52 4551 5545 5354 5f53 495a 455f  AX_REQUEST_SIZE_
+00000390: 4d42 203d 2031 3030 0d0a 0d0a 2320 456e  MB = 100....# En
+000003a0: 6162 6c65 2065 7661 6c75 6174 6520 6170  able evaluate ap
+000003b0: 6920 746f 2065 7865 6375 7465 2061 642d  i to execute ad-
+000003c0: 686f 6320 5079 7468 6f6e 2073 6372 6970  hoc Python scrip
+000003d0: 7473 0d0a 2320 456e 6162 6c65 6420 6279  ts..# Enabled by
+000003e0: 2064 6566 6175 6c74 2e20 4469 7361 626c   default. Disabl
+000003f0: 696e 6720 6974 2077 696c 6c20 7265 7375  ing it will resu
+00000400: 6c74 2069 6e20 3430 3420 6572 726f 722e  lt in 404 error.
+00000410: 0d0a 2320 5441 4250 595f 4556 414c 5541  ..# TABPY_EVALUA
+00000420: 5445 5f45 4e41 424c 4520 3d20 7472 7565  TE_ENABLE = true
+00000430: 0d0a 0d0a 2320 436f 6e66 6967 7572 6520  ....# Configure 
+00000440: 686f 7720 6c6f 6e67 2061 2063 7573 746f  how long a custo
+00000450: 6d20 7363 7269 7074 2070 726f 7669 6465  m script provide
+00000460: 6420 746f 2074 6865 202f 6576 616c 7561  d to the /evalua
+00000470: 7465 206d 6574 686f 640d 0a23 2077 696c  te method..# wil
+00000480: 6c20 7275 6e20 6265 666f 7265 2074 6872  l run before thr
+00000490: 6f77 696e 6720 6120 5469 6d65 6f75 7445  owing a TimeoutE
+000004a0: 7272 6f72 2e0d 0a23 2054 6865 2076 616c  rror...# The val
+000004b0: 7565 2073 686f 756c 6420 6265 2061 2066  ue should be a f
+000004c0: 6c6f 6174 2072 6570 7265 7365 6e74 696e  loat representin
+000004d0: 6720 7468 6520 7469 6d65 6f75 7420 7469  g the timeout ti
+000004e0: 6d65 2069 6e20 7365 636f 6e64 732e 0d0a  me in seconds...
+000004f0: 2320 5441 4250 595f 4556 414c 5541 5445  # TABPY_EVALUATE
+00000500: 5f54 494d 454f 5554 203d 2033 300d 0a0d  _TIMEOUT = 30...
+00000510: 0a23 2045 6e61 626c 6520 477a 6970 2063  .# Enable Gzip c
+00000520: 6f6d 7072 6573 7369 6f6e 2066 6f72 2072  ompression for r
+00000530: 6571 7565 7374 7320 616e 6420 7265 7370  equests and resp
+00000540: 6f6e 7365 732e 0d0a 2320 5441 4250 595f  onses...# TABPY_
+00000550: 475a 4950 5f45 4e41 424c 4520 3d20 7472  GZIP_ENABLE = tr
+00000560: 7565 0d0a 0d0a 5b6c 6f67 6765 7273 5d0d  ue....[loggers].
+00000570: 0a6b 6579 733d 726f 6f74 0d0a 0d0a 5b68  .keys=root....[h
+00000580: 616e 646c 6572 735d 0d0a 6b65 7973 3d72  andlers]..keys=r
+00000590: 6f6f 7448 616e 646c 6572 2c72 6f74 6174  ootHandler,rotat
+000005a0: 696e 6746 696c 6548 616e 646c 6572 0d0a  ingFileHandler..
+000005b0: 0d0a 5b66 6f72 6d61 7474 6572 735d 0d0a  ..[formatters]..
+000005c0: 6b65 7973 3d72 6f6f 7446 6f72 6d61 7474  keys=rootFormatt
+000005d0: 6572 0d0a 0d0a 5b6c 6f67 6765 725f 726f  er....[logger_ro
+000005e0: 6f74 5d0d 0a6c 6576 656c 3d44 4542 5547  ot]..level=DEBUG
+000005f0: 0d0a 6861 6e64 6c65 7273 3d72 6f6f 7448  ..handlers=rootH
+00000600: 616e 646c 6572 2c72 6f74 6174 696e 6746  andler,rotatingF
+00000610: 696c 6548 616e 646c 6572 0d0a 7175 616c  ileHandler..qual
+00000620: 6e61 6d65 3d72 6f6f 740d 0a70 726f 7061  name=root..propa
+00000630: 6765 7465 3d30 0d0a 0d0a 5b68 616e 646c  gete=0....[handl
+00000640: 6572 5f72 6f6f 7448 616e 646c 6572 5d0d  er_rootHandler].
+00000650: 0a63 6c61 7373 3d53 7472 6561 6d48 616e  .class=StreamHan
+00000660: 646c 6572 0d0a 6c65 7665 6c3d 494e 464f  dler..level=INFO
+00000670: 0d0a 666f 726d 6174 7465 723d 726f 6f74  ..formatter=root
+00000680: 466f 726d 6174 7465 720d 0a61 7267 733d  Formatter..args=
+00000690: 2873 7973 2e73 7464 6f75 742c 290d 0a0d  (sys.stdout,)...
+000006a0: 0a5b 6861 6e64 6c65 725f 726f 7461 7469  .[handler_rotati
+000006b0: 6e67 4669 6c65 4861 6e64 6c65 725d 0d0a  ngFileHandler]..
+000006c0: 636c 6173 733d 6861 6e64 6c65 7273 2e52  class=handlers.R
+000006d0: 6f74 6174 696e 6746 696c 6548 616e 646c  otatingFileHandl
+000006e0: 6572 0d0a 6c65 7665 6c3d 4445 4255 470d  er..level=DEBUG.
+000006f0: 0a66 6f72 6d61 7474 6572 3d72 6f6f 7446  .formatter=rootF
+00000700: 6f72 6d61 7474 6572 0d0a 6172 6773 3d28  ormatter..args=(
+00000710: 2774 6162 7079 5f6c 6f67 2e6c 6f67 272c  'tabpy_log.log',
+00000720: 2027 6127 2c20 3130 3030 3030 302c 2035   'a', 1000000, 5
+00000730: 290d 0a0d 0a5b 666f 726d 6174 7465 725f  )....[formatter_
+00000740: 726f 6f74 466f 726d 6174 7465 725d 0d0a  rootFormatter]..
+00000750: 666f 726d 6174 3d25 2861 7363 7469 6d65  format=%(asctime
+00000760: 2973 205b 2528 6c65 7665 6c6e 616d 6529  )s [%(levelname)
+00000770: 735d 2028 2528 6669 6c65 6e61 6d65 2973  s] (%(filename)s
+00000780: 3a25 286d 6f64 756c 6529 733a 2528 6c69  :%(module)s:%(li
+00000790: 6e65 6e6f 2964 293a 2025 286d 6573 7361  neno)d): %(messa
+000007a0: 6765 2973 0d0a 6461 7465 666d 743d 2559  ge)s..datefmt=%Y
+000007b0: 2d25 6d2d 2564 2c25 483a 254d 3a25 530d  -%m-%d,%H:%M:%S.
+000007c0: 0a                                       .
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/common/endpoint_file_mgr.py` & `tabpy-2.7.0/tabpy/tabpy_server/common/endpoint_file_mgr.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-"""
-This module provides functionality required for managing endpoint objects in
-TabPy. It provides a way to download endpoint files from remote
-and then properly cleanup local the endpoint files on update/remove of endpoint
-objects.
-
-The local temporary files for TabPy will by default located at
-    /tmp/query_objects
-
-"""
-import logging
-import os
-import shutil
-from re import compile as _compile
-
-
-_name_checker = _compile(r"^[a-zA-Z0-9-_\s]+$")
-
-
-def _check_endpoint_name(name, logger=logging.getLogger(__name__)):
-    """Checks that the endpoint name is valid by comparing it with an RE and
-    checking that it is not reserved."""
-    if not isinstance(name, str):
-        msg = "Endpoint name must be a string"
-        logger.log(logging.CRITICAL, msg)
-        raise TypeError(msg)
-
-    if name == "":
-        msg = "Endpoint name cannot be empty"
-        logger.log(logging.CRITICAL, msg)
-        raise ValueError(msg)
-
-    if not _name_checker.match(name):
-        msg = (
-            "Endpoint name can only contain: a-z, A-Z, 0-9,"
-            " underscore, hyphens and spaces."
-        )
-        logger.log(logging.CRITICAL, msg)
-        raise ValueError(msg)
-
-
-def grab_files(directory):
-    """
-    Generator that returns all files in a directory.
-    """
-    if not os.path.isdir(directory):
-        return
-    else:
-        for name in os.listdir(directory):
-            full_path = os.path.join(directory, name)
-            if os.path.isdir(full_path):
-                for entry in grab_files(full_path):
-                    yield entry
-            elif os.path.isfile(full_path):
-                yield full_path
-
-
-def cleanup_endpoint_files(
-    name, query_path, logger=logging.getLogger(__name__), retain_versions=None
-):
-    """
-    Cleanup the disk space a certain endpiont uses.
-
-    Parameters
-    ----------
-    name : str
-        The endpoint name
-
-    retain_version : int, optional
-        If given, then all files for this endpoint are removed except the
-        folder for the given version, otherwise, all files for that endpoint
-        are removed.
-    """
-    _check_endpoint_name(name, logger=logger)
-    local_dir = os.path.join(query_path, name)
-
-    # nothing to clean, this is true for state file path where we load
-    # Query Object directly from the state path instead of downloading
-    # to temporary location
-    if not os.path.exists(local_dir):
-        return
-
-    if not retain_versions:
-        shutil.rmtree(local_dir)
-    else:
-        retain_folders = [
-            os.path.join(local_dir, str(version)) for version in retain_versions
-        ]
-        logger.log(logging.INFO, f"Retain folders: {retain_folders}")
-
-        for file_or_dir in os.listdir(local_dir):
-            candidate_dir = os.path.join(local_dir, file_or_dir)
-            if os.path.isdir(candidate_dir) and (candidate_dir not in retain_folders):
-                shutil.rmtree(candidate_dir)
+"""
+This module provides functionality required for managing endpoint objects in
+TabPy. It provides a way to download endpoint files from remote
+and then properly cleanup local the endpoint files on update/remove of endpoint
+objects.
+
+The local temporary files for TabPy will by default located at
+    /tmp/query_objects
+
+"""
+import logging
+import os
+import shutil
+from re import compile as _compile
+
+
+_name_checker = _compile(r"^[a-zA-Z0-9-_\s]+$")
+
+
+def _check_endpoint_name(name, logger=logging.getLogger(__name__)):
+    """Checks that the endpoint name is valid by comparing it with an RE and
+    checking that it is not reserved."""
+    if not isinstance(name, str):
+        msg = "Endpoint name must be a string"
+        logger.log(logging.CRITICAL, msg)
+        raise TypeError(msg)
+
+    if name == "":
+        msg = "Endpoint name cannot be empty"
+        logger.log(logging.CRITICAL, msg)
+        raise ValueError(msg)
+
+    if not _name_checker.match(name):
+        msg = (
+            "Endpoint name can only contain: a-z, A-Z, 0-9,"
+            " underscore, hyphens and spaces."
+        )
+        logger.log(logging.CRITICAL, msg)
+        raise ValueError(msg)
+
+
+def grab_files(directory):
+    """
+    Generator that returns all files in a directory.
+    """
+    if not os.path.isdir(directory):
+        return
+    else:
+        for name in os.listdir(directory):
+            full_path = os.path.join(directory, name)
+            if os.path.isdir(full_path):
+                for entry in grab_files(full_path):
+                    yield entry
+            elif os.path.isfile(full_path):
+                yield full_path
+
+
+def cleanup_endpoint_files(
+    name, query_path, logger=logging.getLogger(__name__), retain_versions=None
+):
+    """
+    Cleanup the disk space a certain endpiont uses.
+
+    Parameters
+    ----------
+    name : str
+        The endpoint name
+
+    retain_version : int, optional
+        If given, then all files for this endpoint are removed except the
+        folder for the given version, otherwise, all files for that endpoint
+        are removed.
+    """
+    _check_endpoint_name(name, logger=logger)
+    local_dir = os.path.join(query_path, name)
+
+    # nothing to clean, this is true for state file path where we load
+    # Query Object directly from the state path instead of downloading
+    # to temporary location
+    if not os.path.exists(local_dir):
+        return
+
+    if not retain_versions:
+        shutil.rmtree(local_dir)
+    else:
+        retain_folders = [
+            os.path.join(local_dir, str(version)) for version in retain_versions
+        ]
+        logger.log(logging.INFO, f"Retain folders: {retain_folders}")
+
+        for file_or_dir in os.listdir(local_dir):
+            candidate_dir = os.path.join(local_dir, file_or_dir)
+            if os.path.isdir(candidate_dir) and (candidate_dir not in retain_folders):
+                shutil.rmtree(candidate_dir)
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/handlers/__init__.py` & `tabpy-2.7.0/tabpy/tabpy_server/handlers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from tabpy.tabpy_server.handlers.base_handler import BaseHandler
-from tabpy.tabpy_server.handlers.management_handler import ManagementHandler
-
-from tabpy.tabpy_server.handlers.endpoint_handler import EndpointHandler
-from tabpy.tabpy_server.handlers.endpoints_handler import EndpointsHandler
-from tabpy.tabpy_server.handlers.evaluation_plane_handler import EvaluationPlaneDisabledHandler
-from tabpy.tabpy_server.handlers.evaluation_plane_handler import EvaluationPlaneHandler
-from tabpy.tabpy_server.handlers.query_plane_handler import QueryPlaneHandler
-from tabpy.tabpy_server.handlers.service_info_handler import ServiceInfoHandler
-from tabpy.tabpy_server.handlers.status_handler import StatusHandler
-from tabpy.tabpy_server.handlers.upload_destination_handler import (
-    UploadDestinationHandler,
-)
+from tabpy.tabpy_server.handlers.base_handler import BaseHandler
+from tabpy.tabpy_server.handlers.management_handler import ManagementHandler
+
+from tabpy.tabpy_server.handlers.endpoint_handler import EndpointHandler
+from tabpy.tabpy_server.handlers.endpoints_handler import EndpointsHandler
+from tabpy.tabpy_server.handlers.evaluation_plane_handler import EvaluationPlaneDisabledHandler
+from tabpy.tabpy_server.handlers.evaluation_plane_handler import EvaluationPlaneHandler
+from tabpy.tabpy_server.handlers.query_plane_handler import QueryPlaneHandler
+from tabpy.tabpy_server.handlers.service_info_handler import ServiceInfoHandler
+from tabpy.tabpy_server.handlers.status_handler import StatusHandler
+from tabpy.tabpy_server.handlers.upload_destination_handler import (
+    UploadDestinationHandler,
+)
+from tabpy.tabpy_server.handlers.no_op_auth_handler import NoOpAuthHandler
+from tabpy.tabpy_server.handlers.basic_auth_server_middleware_factory import (
+    BasicAuthServerMiddlewareFactory,
+)
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/handlers/base_handler.py` & `tabpy-2.7.0/tabpy/tabpy_server/handlers/base_handler.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,444 +1,444 @@
-import base64
-import binascii
-import concurrent
-import json
-import logging
-import tornado.web
-from tabpy.tabpy_server.app.app_parameters import SettingsParameters
-from tabpy.tabpy_server.handlers.util import hash_password
-from tabpy.tabpy_server.handlers.util import AuthErrorStates
-import uuid
-
-
-STAGING_THREAD = concurrent.futures.ThreadPoolExecutor(max_workers=3)
-
-
-class ContextLoggerWrapper:
-    """
-    This class appends request context to logged messages.
-    """
-
-    @staticmethod
-    def _generate_call_id():
-        return str(uuid.uuid4())
-
-    def __init__(self, request: tornado.httputil.HTTPServerRequest):
-        self.call_id = self._generate_call_id()
-        self.set_request(request)
-
-        self.tabpy_username = None
-        self.log_request_context = False
-        self.request_context_logged = False
-
-    def set_request(self, request: tornado.httputil.HTTPServerRequest):
-        """
-        Set HTTP(S) request for logger. Headers will be used to
-        append request data as client information, Tableau user name, etc.
-        """
-        self.remote_ip = request.remote_ip
-        self.method = request.method
-        self.url = request.full_url()
-
-        self.client = request.headers.get("TabPy-Client", None)
-        self.tableau_username = request.headers.get("TabPy-User", None)
-
-    def set_tabpy_username(self, tabpy_username: str):
-        self.tabpy_username = tabpy_username
-
-    def enable_context_logging(self, enable: bool):
-        """
-        Enable/disable request context information logging.
-
-        Parameters
-        ----------
-        enable: bool
-            If True request context information will be logged and
-            every log entry for a request handler will have call ID
-            with it.
-        """
-        self.log_request_context = enable
-
-    def _log_context_info(self):
-        if not self.log_request_context:
-            return
-
-        context = f"Call ID: {self.call_id}"
-
-        if self.remote_ip is not None:
-            context += f", Caller: {self.remote_ip}"
-
-        if self.method is not None:
-            context += f", Method: {self.method}"
-
-        if self.url is not None:
-            context += f", URL: {self.url}"
-
-        if self.client is not None:
-            context += f", Client: {self.client}"
-
-        if self.tableau_username is not None:
-            context += f", Tableau user: {self.tableau_username}"
-
-        if self.tabpy_username is not None:
-            context += f", TabPy user: {self.tabpy_username}"
-
-        logging.getLogger(__name__).log(logging.INFO, context)
-        self.request_context_logged = True
-
-    def log(self, level: int, msg: str):
-        """
-        Log message with or without call ID. If call context is logged and
-        call ID added to any log entry is specified by if context logging
-        is enabled (see CallContext.enable_context_logging for more details).
-
-        Parameters
-        ----------
-        level: int
-            Log level: logging.CRITICAL, ERROR, WARNING, INFO, DEBUG, NOTSET.
-
-        msg: str
-            Message format string.
-
-        args
-            Same as args in Logger.debug().
-
-        kwargs
-            Same as kwargs in Logger.debug().
-        """
-        extended_msg = msg
-        if self.log_request_context:
-            if not self.request_context_logged:
-                self._log_context_info()
-
-            extended_msg += f", <<call ID: {self.call_id}>>"
-
-        logging.getLogger(__name__).log(level, extended_msg)
-
-
-class BaseHandler(tornado.web.RequestHandler):
-    def initialize(self, app):
-        self.tabpy_state = app.tabpy_state
-        # set content type to application/json
-        self.set_header("Content-Type", "application/json")
-        self.protocol = self.settings[SettingsParameters.TransferProtocol]
-        self.port = self.settings[SettingsParameters.Port]
-        self.python_service = app.python_service
-        self.credentials = app.credentials
-        self.username = None
-        self.password = None
-        self.eval_timeout = self.settings[SettingsParameters.EvaluateTimeout]
-
-        self.logger = ContextLoggerWrapper(self.request)
-        self.logger.enable_context_logging(
-            app.settings[SettingsParameters.LogRequestContext]
-        )
-        self.logger.log(logging.DEBUG, "Checking if need to handle authentication")
-        self.auth_error = self.handle_authentication("v1")
-
-    def error_out(self, code, log_message, info=None):
-        self.set_status(code)
-        self.write(json.dumps({"message": log_message, "info": info or {}}))
-
-        self.logger.log(
-            logging.ERROR,
-            'Responding with status={}, message="{}", info="{}"'.format(
-                code, log_message, info
-            ),
-        )
-
-    def options(self):
-        # add CORS headers if TabPy has a cors_origin specified
-        self._add_CORS_header()
-        self.write({})
-
-    def _add_CORS_header(self):
-        """
-        Add CORS header if the TabPy has attribute _cors_origin
-        and _cors_origin is not an empty string.
-        """
-        origin = self.tabpy_state.get_access_control_allow_origin()
-        if len(origin) > 0:
-            self.set_header("Access-Control-Allow-Origin", origin)
-            self.logger.log(logging.DEBUG, f"Access-Control-Allow-Origin:{origin}")
-
-        headers = self.tabpy_state.get_access_control_allow_headers()
-        if len(headers) > 0:
-            self.set_header("Access-Control-Allow-Headers", headers)
-            self.logger.log(logging.DEBUG, f"Access-Control-Allow-Headers:{headers}")
-
-        methods = self.tabpy_state.get_access_control_allow_methods()
-        if len(methods) > 0:
-            self.set_header("Access-Control-Allow-Methods", methods)
-            self.logger.log(logging.DEBUG, f"Access-Control-Allow-Methods:{methods}")
-
-    def _get_auth_method(self, api_version) -> (bool, str):
-        """
-        Finds authentication method if provided.
-
-        Parameters
-        ----------
-        api_version : str
-            API version for authentication.
-
-        Returns
-        -------
-        bool
-            True if known authentication method is found.
-            False otherwise.
-
-        str
-            Name of authentication method used by client.
-            If empty no authentication required.
-
-        (True, '') as result of this function means authentication
-        is not needed.
-        """
-        if api_version not in self.settings[SettingsParameters.ApiVersions]:
-            self.logger.log(logging.CRITICAL, f'Unknown API version "{api_version}"')
-            return False, ""
-
-        version_settings = self.settings[SettingsParameters.ApiVersions][api_version]
-        if "features" not in version_settings:
-            self.logger.log(
-                logging.INFO, f'No features configured for API "{api_version}"'
-            )
-            return True, ""
-
-        features = version_settings["features"]
-        if (
-            "authentication" not in features
-            or not features["authentication"]["required"]
-        ):
-            self.logger.log(
-                logging.INFO,
-                "Authentication is not a required feature for API " f'"{api_version}"',
-            )
-            return True, ""
-
-        auth_feature = features["authentication"]
-        if "methods" not in auth_feature:
-            self.logger.log(
-                logging.INFO,
-                "Authentication method is not configured for API " f'"{api_version}"',
-            )
-
-        methods = auth_feature["methods"]
-        if "basic-auth" in auth_feature["methods"]:
-            return True, "basic-auth"
-        # Add new methods here...
-
-        # No known methods were found
-        self.logger.log(
-            logging.CRITICAL,
-            f'Unknown authentication method(s) "{methods}" are configured '
-            f'for API "{api_version}"',
-        )
-        return False, ""
-
-    def _get_basic_auth_credentials(self) -> bool:
-        """
-        Find credentials for basic access authentication method. Credentials if
-        found stored in Credentials.username and Credentials.password.
-
-        Returns
-        -------
-        bool
-            True if valid credentials were found.
-            False otherwise.
-        """
-        self.logger.log(
-            logging.DEBUG, "Checking request headers for authentication data"
-        )
-        if "Authorization" not in self.request.headers:
-            self.logger.log(logging.INFO, "Authorization header not found")
-            return False
-
-        auth_header = self.request.headers["Authorization"]
-        auth_header_list = auth_header.split(" ")
-        if len(auth_header_list) != 2 or auth_header_list[0] != "Basic":
-            self.logger.log(
-                logging.ERROR, f'Unknown authentication method "{auth_header}"'
-            )
-            return False
-
-        try:
-            cred = base64.b64decode(auth_header_list[1]).decode("utf-8")
-        except (binascii.Error, UnicodeDecodeError) as ex:
-            self.logger.log(logging.CRITICAL, f"Cannot decode credentials: {str(ex)}")
-            return False
-
-        login_pwd = cred.split(":")
-        if len(login_pwd) != 2:
-            self.logger.log(logging.ERROR, "Invalid string in encoded credentials")
-            return False
-
-        self.username = login_pwd[0]
-        self.logger.set_tabpy_username(self.username)
-        self.password = login_pwd[1]
-        return True
-
-    def _get_credentials(self, method) -> bool:
-        """
-        Find credentials for specified authentication method. Credentials if
-        found stored in self.username and self.password.
-
-        Parameters
-        ----------
-        method: str
-            Authentication method name.
-
-        Returns
-        -------
-        bool
-            True if valid credentials were found.
-            False otherwise.
-        """
-        if method == "basic-auth":
-            return self._get_basic_auth_credentials()
-        # Add new methods here...
-
-        # No known methods were found
-        self.logger.log(
-            logging.CRITICAL,
-            f'Unknown authentication method(s) "{method}" are configured ',
-        )
-        return False
-
-    def _validate_basic_auth_credentials(self) -> bool:
-        """
-        Validates username:pwd if they are the same as
-        stored credentials.
-
-        Returns
-        -------
-        bool
-            True if credentials has key login and
-            credentials[login] equal SHA3(pwd), False
-            otherwise.
-        """
-        login = self.username.lower()
-        self.logger.log(
-            logging.DEBUG, f'Validating credentials for user name "{login}"'
-        )
-        if login not in self.credentials:
-            self.logger.log(logging.ERROR, f'User name "{self.username}" not found')
-            return False
-
-        hashed_pwd = hash_password(login, self.password)
-        if self.credentials[login].lower() != hashed_pwd.lower():
-            self.logger.log(
-                logging.ERROR, f'Wrong password for user name "{self.username}"'
-            )
-            return False
-
-        return True
-
-    def _validate_credentials(self, method) -> bool:
-        """
-        Validates credentials according to specified methods if they
-        are what expected.
-
-        Parameters
-        ----------
-        method: str
-            Authentication method name.
-
-        Returns
-        -------
-        bool
-            True if credentials are valid.
-            False otherwise.
-        """
-        if method == "basic-auth":
-            return self._validate_basic_auth_credentials()
-        # Add new methods here...
-
-        # No known methods were found
-        self.logger.log(
-            logging.CRITICAL,
-            f'Unknown authentication method(s) "{method}" are configured ',
-        )
-        return False
-
-    def handle_authentication(self, api_version):
-        """
-        If authentication feature is configured checks provided
-        credentials.
-
-        Parameters
-        ----------
-        api_version : str
-            API version for authentication.
-
-        Returns
-        -------
-        String
-            None if authentication is not required and username and password are None.
-            None if authentication is required and valid credentials provided.
-            NotAuthorized if authenication is required and credentials are incorrect.
-            NotRequired if authentication is not required but credentials are provided.
-        """
-        self.logger.log(logging.DEBUG, "Handling authentication")
-        found, method = self._get_auth_method(api_version)
-        if not found:
-            return AuthErrorStates.NotAuthorized
-
-        if method == "":
-            if not self._get_basic_auth_credentials():
-                self.logger.log(logging.DEBUG,
-                                "authentication not required, username and password are none")
-                return AuthErrorStates.NONE
-            else:
-                self.logger.log(logging.DEBUG,
-                                "authentication not required, username and password are not none")
-                return AuthErrorStates.NotRequired
-
-        if not self._get_credentials(method):
-            return AuthErrorStates.NotAuthorized
-
-        if not self._validate_credentials(method):
-            return AuthErrorStates.NotAuthorized
-
-        return AuthErrorStates.NONE
-
-    def should_fail_with_auth_error(self):
-        """
-        Checks if authentication is required:
-        - if it is not returns false, None
-        - if it is required validates provided credentials
-
-        Returns
-        -------
-        bool
-            False if authentication is not required and username
-            and password is None or isrequired and validation
-            for credentials passes.
-            True if validation for credentials failed or
-            if authentication is not required and username and password
-            fields are not empty.
-        """
-        return self.auth_error
-
-    def fail_with_auth_error(self):
-        """
-        Prepares server 401 response and server 406 response depending
-        on the value of the self.auth_error flag
-        """
-        if self.auth_error == AuthErrorStates.NotAuthorized:
-            self.logger.log(logging.ERROR, "Failing with 401 for unauthorized request")
-            self.set_status(401)
-            self.set_header("WWW-Authenticate", f'Basic realm="{self.tabpy_state.name}"')
-            self.error_out(
-                401,
-                info="Unauthorized request.",
-                log_message="Invalid credentials provided.",
-            )
-        else:
-            self.logger.log(logging.ERROR, "Failing with 406 for Not Acceptable")
-            self.set_status(406)
-            self.set_header("WWW-Authenticate", f'Basic realm="{self.tabpy_state.name}"')
-            self.error_out(
-                406,
-                info="Not Acceptable",
-                log_message="Username or password provided when authentication not available.",
-            )
+import base64
+import binascii
+import concurrent
+import json
+import logging
+import tornado.web
+from tabpy.tabpy_server.app.app_parameters import SettingsParameters
+from tabpy.tabpy_server.handlers.util import hash_password
+from tabpy.tabpy_server.handlers.util import AuthErrorStates
+import uuid
+
+
+STAGING_THREAD = concurrent.futures.ThreadPoolExecutor(max_workers=3)
+
+
+class ContextLoggerWrapper:
+    """
+    This class appends request context to logged messages.
+    """
+
+    @staticmethod
+    def _generate_call_id():
+        return str(uuid.uuid4())
+
+    def __init__(self, request: tornado.httputil.HTTPServerRequest):
+        self.call_id = self._generate_call_id()
+        self.set_request(request)
+
+        self.tabpy_username = None
+        self.log_request_context = False
+        self.request_context_logged = False
+
+    def set_request(self, request: tornado.httputil.HTTPServerRequest):
+        """
+        Set HTTP(S) request for logger. Headers will be used to
+        append request data as client information, Tableau user name, etc.
+        """
+        self.remote_ip = request.remote_ip
+        self.method = request.method
+        self.url = request.full_url()
+
+        self.client = request.headers.get("TabPy-Client", None)
+        self.tableau_username = request.headers.get("TabPy-User", None)
+
+    def set_tabpy_username(self, tabpy_username: str):
+        self.tabpy_username = tabpy_username
+
+    def enable_context_logging(self, enable: bool):
+        """
+        Enable/disable request context information logging.
+
+        Parameters
+        ----------
+        enable: bool
+            If True request context information will be logged and
+            every log entry for a request handler will have call ID
+            with it.
+        """
+        self.log_request_context = enable
+
+    def _log_context_info(self):
+        if not self.log_request_context:
+            return
+
+        context = f"Call ID: {self.call_id}"
+
+        if self.remote_ip is not None:
+            context += f", Caller: {self.remote_ip}"
+
+        if self.method is not None:
+            context += f", Method: {self.method}"
+
+        if self.url is not None:
+            context += f", URL: {self.url}"
+
+        if self.client is not None:
+            context += f", Client: {self.client}"
+
+        if self.tableau_username is not None:
+            context += f", Tableau user: {self.tableau_username}"
+
+        if self.tabpy_username is not None:
+            context += f", TabPy user: {self.tabpy_username}"
+
+        logging.getLogger(__name__).log(logging.INFO, context)
+        self.request_context_logged = True
+
+    def log(self, level: int, msg: str):
+        """
+        Log message with or without call ID. If call context is logged and
+        call ID added to any log entry is specified by if context logging
+        is enabled (see CallContext.enable_context_logging for more details).
+
+        Parameters
+        ----------
+        level: int
+            Log level: logging.CRITICAL, ERROR, WARNING, INFO, DEBUG, NOTSET.
+
+        msg: str
+            Message format string.
+
+        args
+            Same as args in Logger.debug().
+
+        kwargs
+            Same as kwargs in Logger.debug().
+        """
+        extended_msg = msg
+        if self.log_request_context:
+            if not self.request_context_logged:
+                self._log_context_info()
+
+            extended_msg += f", <<call ID: {self.call_id}>>"
+
+        logging.getLogger(__name__).log(level, extended_msg)
+
+
+class BaseHandler(tornado.web.RequestHandler):
+    def initialize(self, app):
+        self.tabpy_state = app.tabpy_state
+        # set content type to application/json
+        self.set_header("Content-Type", "application/json")
+        self.protocol = self.settings[SettingsParameters.TransferProtocol]
+        self.port = self.settings[SettingsParameters.Port]
+        self.python_service = app.python_service
+        self.credentials = app.credentials
+        self.username = None
+        self.password = None
+        self.eval_timeout = self.settings[SettingsParameters.EvaluateTimeout]
+
+        self.logger = ContextLoggerWrapper(self.request)
+        self.logger.enable_context_logging(
+            app.settings[SettingsParameters.LogRequestContext]
+        )
+        self.logger.log(logging.DEBUG, "Checking if need to handle authentication")
+        self.auth_error = self.handle_authentication("v1")
+
+    def error_out(self, code, log_message, info=None):
+        self.set_status(code)
+        self.write(json.dumps({"message": log_message, "info": info or {}}))
+
+        self.logger.log(
+            logging.ERROR,
+            'Responding with status={}, message="{}", info="{}"'.format(
+                code, log_message, info
+            ),
+        )
+
+    def options(self):
+        # add CORS headers if TabPy has a cors_origin specified
+        self._add_CORS_header()
+        self.write({})
+
+    def _add_CORS_header(self):
+        """
+        Add CORS header if the TabPy has attribute _cors_origin
+        and _cors_origin is not an empty string.
+        """
+        origin = self.tabpy_state.get_access_control_allow_origin()
+        if len(origin) > 0:
+            self.set_header("Access-Control-Allow-Origin", origin)
+            self.logger.log(logging.DEBUG, f"Access-Control-Allow-Origin:{origin}")
+
+        headers = self.tabpy_state.get_access_control_allow_headers()
+        if len(headers) > 0:
+            self.set_header("Access-Control-Allow-Headers", headers)
+            self.logger.log(logging.DEBUG, f"Access-Control-Allow-Headers:{headers}")
+
+        methods = self.tabpy_state.get_access_control_allow_methods()
+        if len(methods) > 0:
+            self.set_header("Access-Control-Allow-Methods", methods)
+            self.logger.log(logging.DEBUG, f"Access-Control-Allow-Methods:{methods}")
+
+    def _get_auth_method(self, api_version) -> (bool, str):
+        """
+        Finds authentication method if provided.
+
+        Parameters
+        ----------
+        api_version : str
+            API version for authentication.
+
+        Returns
+        -------
+        bool
+            True if known authentication method is found.
+            False otherwise.
+
+        str
+            Name of authentication method used by client.
+            If empty no authentication required.
+
+        (True, '') as result of this function means authentication
+        is not needed.
+        """
+        if api_version not in self.settings[SettingsParameters.ApiVersions]:
+            self.logger.log(logging.CRITICAL, f'Unknown API version "{api_version}"')
+            return False, ""
+
+        version_settings = self.settings[SettingsParameters.ApiVersions][api_version]
+        if "features" not in version_settings:
+            self.logger.log(
+                logging.INFO, f'No features configured for API "{api_version}"'
+            )
+            return True, ""
+
+        features = version_settings["features"]
+        if (
+            "authentication" not in features
+            or not features["authentication"]["required"]
+        ):
+            self.logger.log(
+                logging.INFO,
+                "Authentication is not a required feature for API " f'"{api_version}"',
+            )
+            return True, ""
+
+        auth_feature = features["authentication"]
+        if "methods" not in auth_feature:
+            self.logger.log(
+                logging.INFO,
+                "Authentication method is not configured for API " f'"{api_version}"',
+            )
+
+        methods = auth_feature["methods"]
+        if "basic-auth" in auth_feature["methods"]:
+            return True, "basic-auth"
+        # Add new methods here...
+
+        # No known methods were found
+        self.logger.log(
+            logging.CRITICAL,
+            f'Unknown authentication method(s) "{methods}" are configured '
+            f'for API "{api_version}"',
+        )
+        return False, ""
+
+    def _get_basic_auth_credentials(self) -> bool:
+        """
+        Find credentials for basic access authentication method. Credentials if
+        found stored in Credentials.username and Credentials.password.
+
+        Returns
+        -------
+        bool
+            True if valid credentials were found.
+            False otherwise.
+        """
+        self.logger.log(
+            logging.DEBUG, "Checking request headers for authentication data"
+        )
+        if "Authorization" not in self.request.headers:
+            self.logger.log(logging.INFO, "Authorization header not found")
+            return False
+
+        auth_header = self.request.headers["Authorization"]
+        auth_header_list = auth_header.split(" ")
+        if len(auth_header_list) != 2 or auth_header_list[0] != "Basic":
+            self.logger.log(
+                logging.ERROR, f'Unknown authentication method "{auth_header}"'
+            )
+            return False
+
+        try:
+            cred = base64.b64decode(auth_header_list[1]).decode("utf-8")
+        except (binascii.Error, UnicodeDecodeError) as ex:
+            self.logger.log(logging.CRITICAL, f"Cannot decode credentials: {str(ex)}")
+            return False
+
+        login_pwd = cred.split(":")
+        if len(login_pwd) != 2:
+            self.logger.log(logging.ERROR, "Invalid string in encoded credentials")
+            return False
+
+        self.username = login_pwd[0]
+        self.logger.set_tabpy_username(self.username)
+        self.password = login_pwd[1]
+        return True
+
+    def _get_credentials(self, method) -> bool:
+        """
+        Find credentials for specified authentication method. Credentials if
+        found stored in self.username and self.password.
+
+        Parameters
+        ----------
+        method: str
+            Authentication method name.
+
+        Returns
+        -------
+        bool
+            True if valid credentials were found.
+            False otherwise.
+        """
+        if method == "basic-auth":
+            return self._get_basic_auth_credentials()
+        # Add new methods here...
+
+        # No known methods were found
+        self.logger.log(
+            logging.CRITICAL,
+            f'Unknown authentication method(s) "{method}" are configured ',
+        )
+        return False
+
+    def _validate_basic_auth_credentials(self) -> bool:
+        """
+        Validates username:pwd if they are the same as
+        stored credentials.
+
+        Returns
+        -------
+        bool
+            True if credentials has key login and
+            credentials[login] equal SHA3(pwd), False
+            otherwise.
+        """
+        login = self.username.lower()
+        self.logger.log(
+            logging.DEBUG, f'Validating credentials for user name "{login}"'
+        )
+        if login not in self.credentials:
+            self.logger.log(logging.ERROR, f'User name "{self.username}" not found')
+            return False
+
+        hashed_pwd = hash_password(login, self.password)
+        if self.credentials[login].lower() != hashed_pwd.lower():
+            self.logger.log(
+                logging.ERROR, f'Wrong password for user name "{self.username}"'
+            )
+            return False
+
+        return True
+
+    def _validate_credentials(self, method) -> bool:
+        """
+        Validates credentials according to specified methods if they
+        are what expected.
+
+        Parameters
+        ----------
+        method: str
+            Authentication method name.
+
+        Returns
+        -------
+        bool
+            True if credentials are valid.
+            False otherwise.
+        """
+        if method == "basic-auth":
+            return self._validate_basic_auth_credentials()
+        # Add new methods here...
+
+        # No known methods were found
+        self.logger.log(
+            logging.CRITICAL,
+            f'Unknown authentication method(s) "{method}" are configured ',
+        )
+        return False
+
+    def handle_authentication(self, api_version):
+        """
+        If authentication feature is configured checks provided
+        credentials.
+
+        Parameters
+        ----------
+        api_version : str
+            API version for authentication.
+
+        Returns
+        -------
+        String
+            None if authentication is not required and username and password are None.
+            None if authentication is required and valid credentials provided.
+            NotAuthorized if authenication is required and credentials are incorrect.
+            NotRequired if authentication is not required but credentials are provided.
+        """
+        self.logger.log(logging.DEBUG, "Handling authentication")
+        found, method = self._get_auth_method(api_version)
+        if not found:
+            return AuthErrorStates.NotAuthorized
+
+        if method == "":
+            if not self._get_basic_auth_credentials():
+                self.logger.log(logging.DEBUG,
+                                "authentication not required, username and password are none")
+                return AuthErrorStates.NONE
+            else:
+                self.logger.log(logging.DEBUG,
+                                "authentication not required, username and password are not none")
+                return AuthErrorStates.NotRequired
+
+        if not self._get_credentials(method):
+            return AuthErrorStates.NotAuthorized
+
+        if not self._validate_credentials(method):
+            return AuthErrorStates.NotAuthorized
+
+        return AuthErrorStates.NONE
+
+    def should_fail_with_auth_error(self):
+        """
+        Checks if authentication is required:
+        - if it is not returns false, None
+        - if it is required validates provided credentials
+
+        Returns
+        -------
+        bool
+            False if authentication is not required and username
+            and password is None or isrequired and validation
+            for credentials passes.
+            True if validation for credentials failed or
+            if authentication is not required and username and password
+            fields are not empty.
+        """
+        return self.auth_error
+
+    def fail_with_auth_error(self):
+        """
+        Prepares server 401 response and server 406 response depending
+        on the value of the self.auth_error flag
+        """
+        if self.auth_error == AuthErrorStates.NotAuthorized:
+            self.logger.log(logging.ERROR, "Failing with 401 for unauthorized request")
+            self.set_status(401)
+            self.set_header("WWW-Authenticate", f'Basic realm="{self.tabpy_state.name}"')
+            self.error_out(
+                401,
+                info="Unauthorized request.",
+                log_message="Invalid credentials provided.",
+            )
+        else:
+            self.logger.log(logging.ERROR, "Failing with 406 for Not Acceptable")
+            self.set_status(406)
+            self.set_header("WWW-Authenticate", f'Basic realm="{self.tabpy_state.name}"')
+            self.error_out(
+                406,
+                info="Not Acceptable",
+                log_message="Username or password provided when authentication not available.",
+            )
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/handlers/endpoint_handler.py` & `tabpy-2.7.0/tabpy/tabpy_server/handlers/endpoint_handler.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-"""
-HTTP handeler to serve specific endpoint request like
-http://myserver:9004/endpoints/mymodel
-
-For how generic endpoints requests is served look
-at endpoints_handler.py
-"""
-
-import json
-import logging
-import shutil
-from tabpy.tabpy_server.common.util import format_exception
-from tabpy.tabpy_server.handlers import ManagementHandler
-from tabpy.tabpy_server.handlers.base_handler import STAGING_THREAD
-from tabpy.tabpy_server.management.state import get_query_object_path
-from tabpy.tabpy_server.psws.callbacks import on_state_change
-from tabpy.tabpy_server.handlers.util import AuthErrorStates
-from tornado import gen
-
-
-class EndpointHandler(ManagementHandler):
-    def initialize(self, app):
-        super(EndpointHandler, self).initialize(app)
-
-    def get(self, endpoint_name):
-        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
-            self.fail_with_auth_error()
-            return
-
-        self.logger.log(logging.DEBUG, f"Processing GET for /endpoints/{endpoint_name}")
-
-        self._add_CORS_header()
-        if not endpoint_name:
-            self.write(json.dumps(self.tabpy_state.get_endpoints()))
-        else:
-            if endpoint_name in self.tabpy_state.get_endpoints():
-                self.write(json.dumps(self.tabpy_state.get_endpoints()[endpoint_name]))
-            else:
-                self.error_out(
-                    404,
-                    "Unknown endpoint",
-                    info=f"Endpoint {endpoint_name} is not found",
-                )
-
-    @gen.coroutine
-    def put(self, name):
-        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
-            self.fail_with_auth_error()
-            return
-
-        self.logger.log(logging.DEBUG, f"Processing PUT for /endpoints/{name}")
-
-        try:
-            if not self.request.body:
-                self.error_out(400, "Input body cannot be empty")
-                self.finish()
-                return
-            try:
-                request_data = json.loads(self.request.body.decode("utf-8"))
-            except BaseException as ex:
-                self.error_out(
-                    400, log_message="Failed to decode input body", info=str(ex)
-                )
-                self.finish()
-                return
-
-            # check if endpoint exists
-            endpoints = self.tabpy_state.get_endpoints(name)
-            if len(endpoints) == 0:
-                self.error_out(404, f"endpoint {name} does not exist.")
-                self.finish()
-                return
-
-            new_version = int(endpoints[name]["version"]) + 1
-            self.logger.log(logging.INFO, f"Endpoint info: {request_data}")
-            err_msg = yield self._add_or_update_endpoint(
-                "update", name, new_version, request_data
-            )
-            if err_msg:
-                self.error_out(400, err_msg)
-                self.finish()
-            else:
-                self.write(self.tabpy_state.get_endpoints(name))
-                self.finish()
-
-        except Exception as e:
-            err_msg = format_exception(e, "update_endpoint")
-            self.error_out(500, err_msg)
-            self.finish()
-
-    @gen.coroutine
-    def delete(self, name):
-        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
-            self.fail_with_auth_error()
-            return
-
-        self.logger.log(logging.DEBUG, f"Processing DELETE for /endpoints/{name}")
-
-        try:
-            endpoints = self.tabpy_state.get_endpoints(name)
-            if len(endpoints) == 0:
-                self.error_out(404, f"endpoint {name} does not exist.")
-                self.finish()
-                return
-
-            # update state
-            try:
-                endpoint_info = self.tabpy_state.delete_endpoint(name)
-            except Exception as e:
-                self.error_out(400, f"Error when removing endpoint: {e.message}")
-                self.finish()
-                return
-
-            # delete files
-            if endpoint_info["type"] != "alias":
-                delete_path = get_query_object_path(
-                    self.settings["state_file_path"], name, None
-                )
-                try:
-                    yield self._delete_po_future(delete_path)
-                except Exception as e:
-                    self.error_out(400, f"Error while deleting: {e}")
-                    self.finish()
-                    return
-
-            self.set_status(204)
-            self.finish()
-
-        except Exception as e:
-            err_msg = format_exception(e, "delete endpoint")
-            self.error_out(500, err_msg)
-            self.finish()
-
-        on_state_change(
-            self.settings, self.tabpy_state, self.python_service, self.logger
-        )
-
-    @gen.coroutine
-    def _delete_po_future(self, delete_path):
-        future = STAGING_THREAD.submit(shutil.rmtree, delete_path)
-        ret = yield future
-        raise gen.Return(ret)
+"""
+HTTP handeler to serve specific endpoint request like
+http://myserver:9004/endpoints/mymodel
+
+For how generic endpoints requests is served look
+at endpoints_handler.py
+"""
+
+import json
+import logging
+import shutil
+from tabpy.tabpy_server.common.util import format_exception
+from tabpy.tabpy_server.handlers import ManagementHandler
+from tabpy.tabpy_server.handlers.base_handler import STAGING_THREAD
+from tabpy.tabpy_server.management.state import get_query_object_path
+from tabpy.tabpy_server.psws.callbacks import on_state_change
+from tabpy.tabpy_server.handlers.util import AuthErrorStates
+from tornado import gen
+
+
+class EndpointHandler(ManagementHandler):
+    def initialize(self, app):
+        super(EndpointHandler, self).initialize(app)
+
+    def get(self, endpoint_name):
+        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
+            self.fail_with_auth_error()
+            return
+
+        self.logger.log(logging.DEBUG, f"Processing GET for /endpoints/{endpoint_name}")
+
+        self._add_CORS_header()
+        if not endpoint_name:
+            self.write(json.dumps(self.tabpy_state.get_endpoints()))
+        else:
+            if endpoint_name in self.tabpy_state.get_endpoints():
+                self.write(json.dumps(self.tabpy_state.get_endpoints()[endpoint_name]))
+            else:
+                self.error_out(
+                    404,
+                    "Unknown endpoint",
+                    info=f"Endpoint {endpoint_name} is not found",
+                )
+
+    @gen.coroutine
+    def put(self, name):
+        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
+            self.fail_with_auth_error()
+            return
+
+        self.logger.log(logging.DEBUG, f"Processing PUT for /endpoints/{name}")
+
+        try:
+            if not self.request.body:
+                self.error_out(400, "Input body cannot be empty")
+                self.finish()
+                return
+            try:
+                request_data = json.loads(self.request.body.decode("utf-8"))
+            except BaseException as ex:
+                self.error_out(
+                    400, log_message="Failed to decode input body", info=str(ex)
+                )
+                self.finish()
+                return
+
+            # check if endpoint exists
+            endpoints = self.tabpy_state.get_endpoints(name)
+            if len(endpoints) == 0:
+                self.error_out(404, f"endpoint {name} does not exist.")
+                self.finish()
+                return
+
+            new_version = int(endpoints[name]["version"]) + 1
+            self.logger.log(logging.INFO, f"Endpoint info: {request_data}")
+            err_msg = yield self._add_or_update_endpoint(
+                "update", name, new_version, request_data
+            )
+            if err_msg:
+                self.error_out(400, err_msg)
+                self.finish()
+            else:
+                self.write(self.tabpy_state.get_endpoints(name))
+                self.finish()
+
+        except Exception as e:
+            err_msg = format_exception(e, "update_endpoint")
+            self.error_out(500, err_msg)
+            self.finish()
+
+    @gen.coroutine
+    def delete(self, name):
+        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
+            self.fail_with_auth_error()
+            return
+
+        self.logger.log(logging.DEBUG, f"Processing DELETE for /endpoints/{name}")
+
+        try:
+            endpoints = self.tabpy_state.get_endpoints(name)
+            if len(endpoints) == 0:
+                self.error_out(404, f"endpoint {name} does not exist.")
+                self.finish()
+                return
+
+            # update state
+            try:
+                endpoint_info = self.tabpy_state.delete_endpoint(name)
+            except Exception as e:
+                self.error_out(400, f"Error when removing endpoint: {e.message}")
+                self.finish()
+                return
+
+            # delete files
+            if endpoint_info["type"] != "alias":
+                delete_path = get_query_object_path(
+                    self.settings["state_file_path"], name, None
+                )
+                try:
+                    yield self._delete_po_future(delete_path)
+                except Exception as e:
+                    self.error_out(400, f"Error while deleting: {e}")
+                    self.finish()
+                    return
+
+            self.set_status(204)
+            self.finish()
+
+        except Exception as e:
+            err_msg = format_exception(e, "delete endpoint")
+            self.error_out(500, err_msg)
+            self.finish()
+
+        on_state_change(
+            self.settings, self.tabpy_state, self.python_service, self.logger
+        )
+
+    @gen.coroutine
+    def _delete_po_future(self, delete_path):
+        future = STAGING_THREAD.submit(shutil.rmtree, delete_path)
+        ret = yield future
+        raise gen.Return(ret)
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/handlers/endpoints_handler.py` & `tabpy-2.7.0/tabpy/tabpy_server/handlers/endpoints_handler.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-"""
-HTTP handeler to serve general endpoints request, specifically
-http://myserver:9004/endpoints
-
-For how individual endpoint requests are served look
-at endpoint_handler.py
-"""
-
-import json
-import logging
-from tabpy.tabpy_server.common.util import format_exception
-from tabpy.tabpy_server.handlers import ManagementHandler
-from tabpy.tabpy_server.handlers.util import AuthErrorStates
-from tornado import gen
-
-
-class EndpointsHandler(ManagementHandler):
-    def initialize(self, app):
-        super(EndpointsHandler, self).initialize(app)
-
-    def get(self):
-        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
-            self.fail_with_auth_error()
-            return
-
-        self._add_CORS_header()
-        self.write(json.dumps(self.tabpy_state.get_endpoints()))
-
-    @gen.coroutine
-    def post(self):
-        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
-            self.fail_with_auth_error()
-            return
-
-        try:
-            if not self.request.body:
-                self.error_out(400, "Input body cannot be empty")
-                self.finish()
-                return
-
-            try:
-                request_data = json.loads(self.request.body.decode("utf-8"))
-            except Exception as ex:
-                self.error_out(400, "Failed to decode input body", str(ex))
-                self.finish()
-                return
-
-            if "name" not in request_data:
-                self.error_out(400, "name is required to add an endpoint.")
-                self.finish()
-                return
-
-            name = request_data["name"]
-
-            # check if endpoint already exist
-            if name in self.tabpy_state.get_endpoints():
-                self.error_out(400, f"endpoint {name} already exists.")
-                self.finish()
-                return
-
-            self.logger.log(logging.DEBUG, f'Adding endpoint "{name}"')
-            err_msg = yield self._add_or_update_endpoint("add", name, 1, request_data)
-            if err_msg:
-                self.error_out(400, err_msg)
-            else:
-                self.logger.log(logging.DEBUG, f"Endpoint {name} successfully added")
-                self.set_status(201)
-                self.write(self.tabpy_state.get_endpoints(name))
-                self.finish()
-                return
-
-        except Exception as e:
-            err_msg = format_exception(e, "/add_endpoint")
-            self.error_out(500, "error adding endpoint", err_msg)
-            self.finish()
-            return
+"""
+HTTP handeler to serve general endpoints request, specifically
+http://myserver:9004/endpoints
+
+For how individual endpoint requests are served look
+at endpoint_handler.py
+"""
+
+import json
+import logging
+from tabpy.tabpy_server.common.util import format_exception
+from tabpy.tabpy_server.handlers import ManagementHandler
+from tabpy.tabpy_server.handlers.util import AuthErrorStates
+from tornado import gen
+
+
+class EndpointsHandler(ManagementHandler):
+    def initialize(self, app):
+        super(EndpointsHandler, self).initialize(app)
+
+    def get(self):
+        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
+            self.fail_with_auth_error()
+            return
+
+        self._add_CORS_header()
+        self.write(json.dumps(self.tabpy_state.get_endpoints()))
+
+    @gen.coroutine
+    def post(self):
+        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
+            self.fail_with_auth_error()
+            return
+
+        try:
+            if not self.request.body:
+                self.error_out(400, "Input body cannot be empty")
+                self.finish()
+                return
+
+            try:
+                request_data = json.loads(self.request.body.decode("utf-8"))
+            except Exception as ex:
+                self.error_out(400, "Failed to decode input body", str(ex))
+                self.finish()
+                return
+
+            if "name" not in request_data:
+                self.error_out(400, "name is required to add an endpoint.")
+                self.finish()
+                return
+
+            name = request_data["name"]
+
+            # check if endpoint already exist
+            if name in self.tabpy_state.get_endpoints():
+                self.error_out(400, f"endpoint {name} already exists.")
+                self.finish()
+                return
+
+            self.logger.log(logging.DEBUG, f'Adding endpoint "{name}"')
+            err_msg = yield self._add_or_update_endpoint("add", name, 1, request_data)
+            if err_msg:
+                self.error_out(400, err_msg)
+            else:
+                self.logger.log(logging.DEBUG, f"Endpoint {name} successfully added")
+                self.set_status(201)
+                self.write(self.tabpy_state.get_endpoints(name))
+                self.finish()
+                return
+
+        except Exception as e:
+            err_msg = format_exception(e, "/add_endpoint")
+            self.error_out(500, "error adding endpoint", err_msg)
+            self.finish()
+            return
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/handlers/management_handler.py` & `tabpy-2.7.0/tabpy/tabpy_server/handlers/management_handler.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-import logging
-import os
-import shutil
-from re import compile as _compile
-from uuid import uuid4 as random_uuid
-
-from tornado import gen
-
-from tabpy.tabpy_server.app.app_parameters import SettingsParameters
-from tabpy.tabpy_server.handlers import BaseHandler
-from tabpy.tabpy_server.handlers.base_handler import STAGING_THREAD
-from tabpy.tabpy_server.management.state import get_query_object_path
-from tabpy.tabpy_server.psws.callbacks import on_state_change
-
-
-def copy_from_local(localpath, remotepath, is_dir=False):
-    if is_dir:
-        if not os.path.exists(remotepath):
-            # remote folder does not exist
-            shutil.copytree(localpath, remotepath)
-        else:
-            # remote folder exists, copy each file
-            src_files = os.listdir(localpath)
-            for file_name in src_files:
-                full_file_name = os.path.join(localpath, file_name)
-                if os.path.isdir(full_file_name):
-                    # copy folder recursively
-                    full_remote_path = os.path.join(remotepath, file_name)
-                    shutil.copytree(full_file_name, full_remote_path)
-                else:
-                    # copy each file
-                    shutil.copy(full_file_name, remotepath)
-    else:
-        shutil.copy(localpath, remotepath)
-
-
-class ManagementHandler(BaseHandler):
-    def initialize(self, app):
-        super(ManagementHandler, self).initialize(app)
-        self.port = self.settings[SettingsParameters.Port]
-
-    def _get_protocol(self):
-        return "http://"
-
-    @gen.coroutine
-    def _add_or_update_endpoint(self, action, name, version, request_data):
-        """
-        Add or update an endpoint
-        """
-        self.logger.log(logging.DEBUG, f"Adding/updating model {name}...")
-
-        if not isinstance(name, str):
-            msg = "Endpoint name must be a string"
-            self.logger.log(logging.CRITICAL, msg)
-            raise TypeError(msg)
-
-        name_checker = _compile(r"^[a-zA-Z0-9-_\s]+$")
-        if not name_checker.match(name):
-            raise gen.Return(
-                "endpoint name can only contain: a-z, A-Z, 0-9,"
-                " underscore, hyphens and spaces."
-            )
-
-        if self.settings.get("add_or_updating_endpoint"):
-            msg = (
-                "Another endpoint update is already in progress"
-                ", please wait a while and try again"
-            )
-            self.logger.log(logging.CRITICAL, msg)
-            raise RuntimeError(msg)
-
-        self.settings["add_or_updating_endpoint"] = random_uuid()
-        try:
-            docstring = None
-            if "docstring" in request_data:
-                docstring = str(
-                    bytes(request_data["docstring"], "utf-8").decode("unicode_escape")
-                )
-
-            description = request_data.get("description", None)
-            endpoint_type = request_data.get("type", None)
-            methods = request_data.get("methods", [])
-            dependencies = request_data.get("dependencies", None)
-            target = request_data.get("target", None)
-            schema = request_data.get("schema", None)
-            src_path = request_data.get("src_path", None)
-            target_path = get_query_object_path(
-                self.settings[SettingsParameters.StateFilePath], name, version
-            )
-
-            path_checker = _compile(r"^[\\\:a-zA-Z0-9-_~\s/\.\(\)]+$")
-            # copy from staging
-            if src_path:
-                if not isinstance(src_path, str):
-                    raise gen.Return("src_path must be a string.")
-                if not path_checker.match(src_path):
-                    raise gen.Return(f"Invalid source path for endpoint {name}")
-
-                yield self._copy_po_future(src_path, target_path)
-            elif endpoint_type != "alias":
-                raise gen.Return("src_path is required to add/update an endpoint.")
-            else:
-                # alias special logic:
-                if not target:
-                    raise gen.Return("Target is required for alias endpoint.")
-                dependencies = [target]
-
-            # update local config
-            try:
-                if action == "add":
-                    self.tabpy_state.add_endpoint(
-                        name=name,
-                        description=description,
-                        docstring=docstring,
-                        endpoint_type=endpoint_type,
-                        methods=methods,
-                        dependencies=dependencies,
-                        target=target,
-                        schema=schema,
-                    )
-                else:
-                    self.tabpy_state.update_endpoint(
-                        name=name,
-                        description=description,
-                        docstring=docstring,
-                        endpoint_type=endpoint_type,
-                        methods=methods,
-                        dependencies=dependencies,
-                        target=target,
-                        schema=schema,
-                        version=version,
-                    )
-
-            except Exception as e:
-                raise gen.Return(f"Error when changing TabPy state: {e}")
-
-            on_state_change(
-                self.settings, self.tabpy_state, self.python_service, self.logger
-            )
-
-        finally:
-            self.settings["add_or_updating_endpoint"] = None
-
-    @gen.coroutine
-    def _copy_po_future(self, src_path, target_path):
-        future = STAGING_THREAD.submit(
-            copy_from_local, src_path, target_path, is_dir=True
-        )
-        ret = yield future
-        raise gen.Return(ret)
+import logging
+import os
+import shutil
+from re import compile as _compile
+from uuid import uuid4 as random_uuid
+
+from tornado import gen
+
+from tabpy.tabpy_server.app.app_parameters import SettingsParameters
+from tabpy.tabpy_server.handlers import BaseHandler
+from tabpy.tabpy_server.handlers.base_handler import STAGING_THREAD
+from tabpy.tabpy_server.management.state import get_query_object_path
+from tabpy.tabpy_server.psws.callbacks import on_state_change
+
+
+def copy_from_local(localpath, remotepath, is_dir=False):
+    if is_dir:
+        if not os.path.exists(remotepath):
+            # remote folder does not exist
+            shutil.copytree(localpath, remotepath)
+        else:
+            # remote folder exists, copy each file
+            src_files = os.listdir(localpath)
+            for file_name in src_files:
+                full_file_name = os.path.join(localpath, file_name)
+                if os.path.isdir(full_file_name):
+                    # copy folder recursively
+                    full_remote_path = os.path.join(remotepath, file_name)
+                    shutil.copytree(full_file_name, full_remote_path)
+                else:
+                    # copy each file
+                    shutil.copy(full_file_name, remotepath)
+    else:
+        shutil.copy(localpath, remotepath)
+
+
+class ManagementHandler(BaseHandler):
+    def initialize(self, app):
+        super(ManagementHandler, self).initialize(app)
+        self.port = self.settings[SettingsParameters.Port]
+
+    def _get_protocol(self):
+        return "http://"
+
+    @gen.coroutine
+    def _add_or_update_endpoint(self, action, name, version, request_data):
+        """
+        Add or update an endpoint
+        """
+        self.logger.log(logging.DEBUG, f"Adding/updating model {name}...")
+
+        if not isinstance(name, str):
+            msg = "Endpoint name must be a string"
+            self.logger.log(logging.CRITICAL, msg)
+            raise TypeError(msg)
+
+        name_checker = _compile(r"^[a-zA-Z0-9-_\s]+$")
+        if not name_checker.match(name):
+            raise gen.Return(
+                "endpoint name can only contain: a-z, A-Z, 0-9,"
+                " underscore, hyphens and spaces."
+            )
+
+        if self.settings.get("add_or_updating_endpoint"):
+            msg = (
+                "Another endpoint update is already in progress"
+                ", please wait a while and try again"
+            )
+            self.logger.log(logging.CRITICAL, msg)
+            raise RuntimeError(msg)
+
+        self.settings["add_or_updating_endpoint"] = random_uuid()
+        try:
+            docstring = None
+            if "docstring" in request_data:
+                docstring = str(
+                    bytes(request_data["docstring"], "utf-8").decode("unicode_escape")
+                )
+
+            description = request_data.get("description", None)
+            endpoint_type = request_data.get("type", None)
+            methods = request_data.get("methods", [])
+            dependencies = request_data.get("dependencies", None)
+            target = request_data.get("target", None)
+            schema = request_data.get("schema", None)
+            src_path = request_data.get("src_path", None)
+            target_path = get_query_object_path(
+                self.settings[SettingsParameters.StateFilePath], name, version
+            )
+
+            path_checker = _compile(r"^[\\\:a-zA-Z0-9-_~\s/\.\(\)]+$")
+            # copy from staging
+            if src_path:
+                if not isinstance(src_path, str):
+                    raise gen.Return("src_path must be a string.")
+                if not path_checker.match(src_path):
+                    raise gen.Return(f"Invalid source path for endpoint {name}")
+
+                yield self._copy_po_future(src_path, target_path)
+            elif endpoint_type != "alias":
+                raise gen.Return("src_path is required to add/update an endpoint.")
+            else:
+                # alias special logic:
+                if not target:
+                    raise gen.Return("Target is required for alias endpoint.")
+                dependencies = [target]
+
+            # update local config
+            try:
+                if action == "add":
+                    self.tabpy_state.add_endpoint(
+                        name=name,
+                        description=description,
+                        docstring=docstring,
+                        endpoint_type=endpoint_type,
+                        methods=methods,
+                        dependencies=dependencies,
+                        target=target,
+                        schema=schema,
+                    )
+                else:
+                    self.tabpy_state.update_endpoint(
+                        name=name,
+                        description=description,
+                        docstring=docstring,
+                        endpoint_type=endpoint_type,
+                        methods=methods,
+                        dependencies=dependencies,
+                        target=target,
+                        schema=schema,
+                        version=version,
+                    )
+
+            except Exception as e:
+                raise gen.Return(f"Error when changing TabPy state: {e}")
+
+            on_state_change(
+                self.settings, self.tabpy_state, self.python_service, self.logger
+            )
+
+        finally:
+            self.settings["add_or_updating_endpoint"] = None
+
+    @gen.coroutine
+    def _copy_po_future(self, src_path, target_path):
+        future = STAGING_THREAD.submit(
+            copy_from_local, src_path, target_path, is_dir=True
+        )
+        ret = yield future
+        raise gen.Return(ret)
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/handlers/query_plane_handler.py` & `tabpy-2.7.0/tabpy/tabpy_server/handlers/query_plane_handler.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,234 +1,234 @@
-from tabpy.tabpy_server.handlers import BaseHandler
-import logging
-import time
-from tabpy.tabpy_server.common.messages import (
-    Query,
-    QuerySuccessful,
-    QueryError,
-    UnknownURI,
-)
-from hashlib import md5
-import uuid
-import json
-from tabpy.tabpy_server.common.util import format_exception
-import urllib
-from tornado import gen
-from tabpy.tabpy_server.handlers.util import AuthErrorStates
-
-
-def _get_uuid():
-    """Generate a unique identifier string"""
-    return str(uuid.uuid4())
-
-
-class QueryPlaneHandler(BaseHandler):
-    def initialize(self, app):
-        super(QueryPlaneHandler, self).initialize(app)
-
-    def _query(self, po_name, data, uid, qry):
-        """
-        Parameters
-        ----------
-        po_name : str
-            The name of the query object to query
-
-        data : dict
-            The deserialized request body
-
-        uid: str
-            A unique identifier for the request
-
-        qry: str
-            The incoming query object. This object maintains
-            raw incoming request, which is different from the sanitied data
-
-        Returns
-        -------
-        out : (result type, dict, int)
-            A triple containing a result type, the result message
-            as a dictionary, and the time in seconds that it took to complete
-            the request.
-        """
-        self.logger.log(logging.DEBUG, f"Collecting query info for {po_name}...")
-        start_time = time.time()
-        response = self.python_service.ps.query(po_name, data, uid)
-        gls_time = time.time() - start_time
-        self.logger.log(logging.DEBUG, f"Query info: {response}")
-
-        if isinstance(response, QuerySuccessful):
-            response_json = response.to_json()
-            md5_tag = md5(response_json.encode("utf-8")).hexdigest()
-            self.set_header("Etag", f'"{md5_tag}"')
-            return (QuerySuccessful, response.for_json(), gls_time)
-        else:
-            self.logger.log(logging.ERROR, f"Failed query, response: {response}")
-            return (type(response), response.for_json(), gls_time)
-
-    # handle HTTP Options requests to support CORS
-    # don't check API key (client does not send or receive data for OPTIONS,
-    # it just allows the client to subsequently make a POST request)
-    def options(self, pred_name):
-        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
-            self.fail_with_auth_error()
-            return
-
-        self.logger.log(logging.DEBUG, f"Processing OPTIONS for /query/{pred_name}")
-
-        # add CORS headers if TabPy has a cors_origin specified
-        self._add_CORS_header()
-        self.write({})
-
-    def _handle_result(self, po_name, data, qry, uid):
-        (response_type, response, gls_time) = self._query(po_name, data, uid, qry)
-
-        if response_type == QuerySuccessful:
-            result_dict = {
-                "response": response["response"],
-                "version": response["version"],
-                "model": po_name,
-                "uuid": uid,
-            }
-            self.write(result_dict)
-            self.finish()
-            return (gls_time, response["response"])
-        else:
-            if response_type == UnknownURI:
-                self.error_out(
-                    404,
-                    "UnknownURI",
-                    info=(
-                        "No query object has been registered"
-                        f' with the name "{po_name}"'
-                    ),
-                )
-            elif response_type == QueryError:
-                self.error_out(400, "QueryError", info=response)
-            else:
-                self.error_out(500, f"Error querying function '{po_name}'", info=response)
-
-            return (None, None)
-
-    def _sanitize_request_data(self, data):
-        if not isinstance(data, dict):
-            msg = "Input data must be a dictionary"
-            self.logger.log(logging.CRITICAL, msg)
-            raise RuntimeError(msg)
-
-        if "method" in data:
-            return {"data": data.get("data"), "method": data.get("method")}
-        elif "data" in data:
-            return data.get("data")
-        else:
-            msg = 'Input data must be a dictionary with a key called "data"'
-            self.logger.log(logging.CRITICAL, msg)
-            raise RuntimeError(msg)
-
-    def _process_query(self, endpoint_name, start):
-        self.logger.log(logging.DEBUG, f"Processing query {endpoint_name}...")
-        try:
-            self._add_CORS_header()
-
-            if not self.request.body:
-                self.request.body = {}
-
-            # extract request data explicitly for caching purpose
-            request_json = self.request.body.decode("utf-8")
-
-            # Sanitize input data
-            data = self._sanitize_request_data(json.loads(request_json))
-        except Exception as e:
-            self.logger.log(logging.ERROR, str(e))
-            err_msg = format_exception(e, "Invalid Input Data")
-            self.error_out(400, err_msg)
-            return
-
-        try:
-            (po_name, _) = self._get_actual_model(endpoint_name)
-
-            # po_name is None if self.python_service.ps.query_objects.get(
-            # endpoint_name) is None
-            if not po_name:
-                self.error_out(
-                    404, "UnknownURI", info=f"Endpoint '{endpoint_name}' does not exist"
-                )
-                return
-
-            po_obj = self.python_service.ps.query_objects.get(po_name)
-
-            if not po_obj:
-                self.error_out(
-                    404, "UnknownURI", info=f'Endpoint "{po_name}" does not exist'
-                )
-                return
-
-            if po_name != endpoint_name:
-                self.logger.log(
-                    logging.INFO, f"Querying actual model: po_name={po_name}"
-                )
-
-            uid = _get_uuid()
-
-            # record query w/ request ID in query log
-            qry = Query(po_name, request_json)
-            gls_time = 0
-            # send a query to PythonService and return
-            (gls_time, _) = self._handle_result(po_name, data, qry, uid)
-
-            # if error occurred, GLS time is None.
-            if not gls_time:
-                return
-
-        except Exception as e:
-            self.logger.log(logging.ERROR, str(e))
-            err_msg = format_exception(e, "process query")
-            self.error_out(500, "Error processing query", info=err_msg)
-            return
-
-    def _get_actual_model(self, endpoint_name):
-        # Find the actual query to run from given endpoint
-        all_endpoint_names = []
-
-        while True:
-            endpoint_info = self.python_service.ps.query_objects.get(endpoint_name)
-            if not endpoint_info:
-                return [None, None]
-
-            all_endpoint_names.append(endpoint_name)
-
-            endpoint_type = endpoint_info.get("type", "model")
-
-            if endpoint_type == "alias":
-                endpoint_name = endpoint_info["endpoint_obj"]
-            elif endpoint_type == "model":
-                break
-            else:
-                self.error_out(
-                    500,
-                    "Unknown endpoint type",
-                    info=f'Endpoint type "{endpoint_type}" does not exist',
-                )
-                return
-
-        return (endpoint_name, all_endpoint_names)
-
-    @gen.coroutine
-    def get(self, endpoint_name):
-        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
-            self.fail_with_auth_error()
-            return
-
-        start = time.time()
-        endpoint_name = urllib.parse.unquote(endpoint_name)
-        self._process_query(endpoint_name, start)
-
-    @gen.coroutine
-    def post(self, endpoint_name):
-        self.logger.log(logging.DEBUG, f"Processing POST for /query/{endpoint_name}...")
-
-        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
-            self.fail_with_auth_error()
-            return
-
-        start = time.time()
-        endpoint_name = urllib.parse.unquote(endpoint_name)
-        self._process_query(endpoint_name, start)
+from tabpy.tabpy_server.handlers import BaseHandler
+import logging
+import time
+from tabpy.tabpy_server.common.messages import (
+    Query,
+    QuerySuccessful,
+    QueryError,
+    UnknownURI,
+)
+from hashlib import md5
+import uuid
+import json
+from tabpy.tabpy_server.common.util import format_exception
+import urllib
+from tornado import gen
+from tabpy.tabpy_server.handlers.util import AuthErrorStates
+
+
+def _get_uuid():
+    """Generate a unique identifier string"""
+    return str(uuid.uuid4())
+
+
+class QueryPlaneHandler(BaseHandler):
+    def initialize(self, app):
+        super(QueryPlaneHandler, self).initialize(app)
+
+    def _query(self, po_name, data, uid, qry):
+        """
+        Parameters
+        ----------
+        po_name : str
+            The name of the query object to query
+
+        data : dict
+            The deserialized request body
+
+        uid: str
+            A unique identifier for the request
+
+        qry: str
+            The incoming query object. This object maintains
+            raw incoming request, which is different from the sanitied data
+
+        Returns
+        -------
+        out : (result type, dict, int)
+            A triple containing a result type, the result message
+            as a dictionary, and the time in seconds that it took to complete
+            the request.
+        """
+        self.logger.log(logging.DEBUG, f"Collecting query info for {po_name}...")
+        start_time = time.time()
+        response = self.python_service.ps.query(po_name, data, uid)
+        gls_time = time.time() - start_time
+        self.logger.log(logging.DEBUG, f"Query info: {response}")
+
+        if isinstance(response, QuerySuccessful):
+            response_json = response.to_json()
+            md5_tag = md5(response_json.encode("utf-8")).hexdigest()
+            self.set_header("Etag", f'"{md5_tag}"')
+            return (QuerySuccessful, response.for_json(), gls_time)
+        else:
+            self.logger.log(logging.ERROR, f"Failed query, response: {response}")
+            return (type(response), response.for_json(), gls_time)
+
+    # handle HTTP Options requests to support CORS
+    # don't check API key (client does not send or receive data for OPTIONS,
+    # it just allows the client to subsequently make a POST request)
+    def options(self, pred_name):
+        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
+            self.fail_with_auth_error()
+            return
+
+        self.logger.log(logging.DEBUG, f"Processing OPTIONS for /query/{pred_name}")
+
+        # add CORS headers if TabPy has a cors_origin specified
+        self._add_CORS_header()
+        self.write({})
+
+    def _handle_result(self, po_name, data, qry, uid):
+        (response_type, response, gls_time) = self._query(po_name, data, uid, qry)
+
+        if response_type == QuerySuccessful:
+            result_dict = {
+                "response": response["response"],
+                "version": response["version"],
+                "model": po_name,
+                "uuid": uid,
+            }
+            self.write(result_dict)
+            self.finish()
+            return (gls_time, response["response"])
+        else:
+            if response_type == UnknownURI:
+                self.error_out(
+                    404,
+                    "UnknownURI",
+                    info=(
+                        "No query object has been registered"
+                        f' with the name "{po_name}"'
+                    ),
+                )
+            elif response_type == QueryError:
+                self.error_out(400, "QueryError", info=response)
+            else:
+                self.error_out(500, f"Error querying function '{po_name}'", info=response)
+
+            return (None, None)
+
+    def _sanitize_request_data(self, data):
+        if not isinstance(data, dict):
+            msg = "Input data must be a dictionary"
+            self.logger.log(logging.CRITICAL, msg)
+            raise RuntimeError(msg)
+
+        if "method" in data:
+            return {"data": data.get("data"), "method": data.get("method")}
+        elif "data" in data:
+            return data.get("data")
+        else:
+            msg = 'Input data must be a dictionary with a key called "data"'
+            self.logger.log(logging.CRITICAL, msg)
+            raise RuntimeError(msg)
+
+    def _process_query(self, endpoint_name, start):
+        self.logger.log(logging.DEBUG, f"Processing query {endpoint_name}...")
+        try:
+            self._add_CORS_header()
+
+            if not self.request.body:
+                self.request.body = {}
+
+            # extract request data explicitly for caching purpose
+            request_json = self.request.body.decode("utf-8")
+
+            # Sanitize input data
+            data = self._sanitize_request_data(json.loads(request_json))
+        except Exception as e:
+            self.logger.log(logging.ERROR, str(e))
+            err_msg = format_exception(e, "Invalid Input Data")
+            self.error_out(400, err_msg)
+            return
+
+        try:
+            (po_name, _) = self._get_actual_model(endpoint_name)
+
+            # po_name is None if self.python_service.ps.query_objects.get(
+            # endpoint_name) is None
+            if not po_name:
+                self.error_out(
+                    404, "UnknownURI", info=f"Endpoint '{endpoint_name}' does not exist"
+                )
+                return
+
+            po_obj = self.python_service.ps.query_objects.get(po_name)
+
+            if not po_obj:
+                self.error_out(
+                    404, "UnknownURI", info=f'Endpoint "{po_name}" does not exist'
+                )
+                return
+
+            if po_name != endpoint_name:
+                self.logger.log(
+                    logging.INFO, f"Querying actual model: po_name={po_name}"
+                )
+
+            uid = _get_uuid()
+
+            # record query w/ request ID in query log
+            qry = Query(po_name, request_json)
+            gls_time = 0
+            # send a query to PythonService and return
+            (gls_time, _) = self._handle_result(po_name, data, qry, uid)
+
+            # if error occurred, GLS time is None.
+            if not gls_time:
+                return
+
+        except Exception as e:
+            self.logger.log(logging.ERROR, str(e))
+            err_msg = format_exception(e, "process query")
+            self.error_out(500, "Error processing query", info=err_msg)
+            return
+
+    def _get_actual_model(self, endpoint_name):
+        # Find the actual query to run from given endpoint
+        all_endpoint_names = []
+
+        while True:
+            endpoint_info = self.python_service.ps.query_objects.get(endpoint_name)
+            if not endpoint_info:
+                return [None, None]
+
+            all_endpoint_names.append(endpoint_name)
+
+            endpoint_type = endpoint_info.get("type", "model")
+
+            if endpoint_type == "alias":
+                endpoint_name = endpoint_info["endpoint_obj"]
+            elif endpoint_type == "model":
+                break
+            else:
+                self.error_out(
+                    500,
+                    "Unknown endpoint type",
+                    info=f'Endpoint type "{endpoint_type}" does not exist',
+                )
+                return
+
+        return (endpoint_name, all_endpoint_names)
+
+    @gen.coroutine
+    def get(self, endpoint_name):
+        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
+            self.fail_with_auth_error()
+            return
+
+        start = time.time()
+        endpoint_name = urllib.parse.unquote(endpoint_name)
+        self._process_query(endpoint_name, start)
+
+    @gen.coroutine
+    def post(self, endpoint_name):
+        self.logger.log(logging.DEBUG, f"Processing POST for /query/{endpoint_name}...")
+
+        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
+            self.fail_with_auth_error()
+            return
+
+        start = time.time()
+        endpoint_name = urllib.parse.unquote(endpoint_name)
+        self._process_query(endpoint_name, start)
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/handlers/status_handler.py` & `tabpy-2.7.0/tabpy/tabpy_server/handlers/status_handler.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import json
-import logging
-from tabpy.tabpy_server.handlers import BaseHandler
-from tabpy.tabpy_server.handlers.util import AuthErrorStates
-
-class StatusHandler(BaseHandler):
-    def initialize(self, app):
-        super(StatusHandler, self).initialize(app)
-
-    def get(self):
-        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
-            self.fail_with_auth_error()
-            return
-
-        self._add_CORS_header()
-
-        status_dict = {}
-        for k, v in self.python_service.ps.query_objects.items():
-            status_dict[k] = {
-                "version": v["version"],
-                "type": v["type"],
-                "status": v["status"],
-                "last_error": v["last_error"],
-            }
-
-        self.logger.log(logging.DEBUG, f"Found models: {status_dict}")
-        self.write(json.dumps(status_dict))
-        self.finish()
-        return
+import json
+import logging
+from tabpy.tabpy_server.handlers import BaseHandler
+from tabpy.tabpy_server.handlers.util import AuthErrorStates
+
+class StatusHandler(BaseHandler):
+    def initialize(self, app):
+        super(StatusHandler, self).initialize(app)
+
+    def get(self):
+        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
+            self.fail_with_auth_error()
+            return
+
+        self._add_CORS_header()
+
+        status_dict = {}
+        for k, v in self.python_service.ps.query_objects.items():
+            status_dict[k] = {
+                "version": v["version"],
+                "type": v["type"],
+                "status": v["status"],
+                "last_error": v["last_error"],
+            }
+
+        self.logger.log(logging.DEBUG, f"Found models: {status_dict}")
+        self.write(json.dumps(status_dict))
+        self.finish()
+        return
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/handlers/upload_destination_handler.py` & `tabpy-2.7.0/tabpy/tabpy_server/handlers/upload_destination_handler.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from tabpy.tabpy_server.app.app_parameters import SettingsParameters
-from tabpy.tabpy_server.handlers import ManagementHandler
-import os
-from tabpy.tabpy_server.handlers.util import AuthErrorStates
-
-
-_QUERY_OBJECT_STAGING_FOLDER = "staging"
-
-
-class UploadDestinationHandler(ManagementHandler):
-    def initialize(self, app):
-        super(UploadDestinationHandler, self).initialize(app)
-
-    def get(self):
-        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
-            self.fail_with_auth_error()
-            return
-
-        path = self.settings[SettingsParameters.StateFilePath]
-        path = os.path.join(path, _QUERY_OBJECT_STAGING_FOLDER)
-        self.write({"path": path})
+from tabpy.tabpy_server.app.app_parameters import SettingsParameters
+from tabpy.tabpy_server.handlers import ManagementHandler
+import os
+from tabpy.tabpy_server.handlers.util import AuthErrorStates
+
+
+_QUERY_OBJECT_STAGING_FOLDER = "staging"
+
+
+class UploadDestinationHandler(ManagementHandler):
+    def initialize(self, app):
+        super(UploadDestinationHandler, self).initialize(app)
+
+    def get(self):
+        if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
+            self.fail_with_auth_error()
+            return
+
+        path = self.settings[SettingsParameters.StateFilePath]
+        path = os.path.join(path, _QUERY_OBJECT_STAGING_FOLDER)
+        self.write({"path": path})
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/handlers/util.py` & `tabpy-2.7.0/tabpy/tabpy_server/handlers/util.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import binascii
-from hashlib import pbkdf2_hmac
-from enum import Enum, auto
-
-
-class AuthErrorStates(Enum):
-    NONE = auto()
-    NotAuthorized = auto()
-    NotRequired = auto()
-
-def hash_password(username, pwd):
-    """
-    Hashes password using PKDBF2 method:
-    hash = PKDBF2('sha512', pwd, salt=username, 10000)
-
-    Parameters
-    ----------
-    username : str
-        User name (login). Used as salt for hashing.
-        User name is lowercased befor being used in hashing.
-        Salt is formatted as '_$salt@tabpy:<username>$_' to
-        guarantee there's at least 16 characters.
-
-    pwd : str
-        Password to hash.
-
-    Returns
-    -------
-    str
-        Sting representation (hexidecimal) for PBKDF2 hash
-        for the password.
-    """
-    salt = f"_$salt@tabpy:{username.lower()}$_"
-
-    hash = pbkdf2_hmac(
-        hash_name="sha512", password=pwd.encode(), salt=salt.encode(), iterations=10000
-    )
-    return binascii.hexlify(hash).decode()
+import binascii
+from hashlib import pbkdf2_hmac
+from enum import Enum, auto
+
+
+class AuthErrorStates(Enum):
+    NONE = auto()
+    NotAuthorized = auto()
+    NotRequired = auto()
+
+def hash_password(username, pwd):
+    """
+    Hashes password using PKDBF2 method:
+    hash = PKDBF2('sha512', pwd, salt=username, 10000)
+
+    Parameters
+    ----------
+    username : str
+        User name (login). Used as salt for hashing.
+        User name is lowercased befor being used in hashing.
+        Salt is formatted as '_$salt@tabpy:<username>$_' to
+        guarantee there's at least 16 characters.
+
+    pwd : str
+        Password to hash.
+
+    Returns
+    -------
+    str
+        Sting representation (hexidecimal) for PBKDF2 hash
+        for the password.
+    """
+    salt = f"_$salt@tabpy:{username.lower()}$_"
+
+    hash = pbkdf2_hmac(
+        hash_name="sha512", password=pwd.encode(), salt=salt.encode(), iterations=10000
+    )
+    return binascii.hexlify(hash).decode()
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/psws/callbacks.py` & `tabpy-2.7.0/tabpy/tabpy_server/psws/callbacks.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-import logging
-from tabpy.tabpy_server.app.app_parameters import SettingsParameters
-from tabpy.tabpy_server.common.messages import (
-    LoadObject,
-    DeleteObjects,
-    ListObjects,
-    ObjectList,
-)
-from tabpy.tabpy_server.common.endpoint_file_mgr import cleanup_endpoint_files
-from tabpy.tabpy_server.common.util import format_exception
-from tabpy.tabpy_server.management.state import TabPyState, get_query_object_path
-from tabpy.tabpy_server.management import util
-from time import sleep
-from tornado import gen
-
-
-logger = logging.getLogger(__name__)
-
-
-def wait_for_endpoint_loaded(python_service, object_uri):
-    """
-    This method waits for the object to be loaded.
-    """
-    logger.info("Waiting for object to be loaded...")
-    while True:
-        msg = ListObjects()
-        list_object_msg = python_service.manage_request(msg)
-        if not isinstance(list_object_msg, ObjectList):
-            logger.error(f"Error loading endpoint {object_uri}: {list_object_msg}")
-            return
-
-        for (uri, info) in list_object_msg.objects.items():
-            if uri == object_uri:
-                if info["status"] != "LoadInProgress":
-                    logger.info(f'Object load status: {info["status"]}')
-                    return
-
-        sleep(0.1)
-
-
-@gen.coroutine
-def init_ps_server(settings, tabpy_state):
-    logger.info("Initializing TabPy Server...")
-    existing_pos = tabpy_state.get_endpoints()
-    for (object_name, obj_info) in existing_pos.items():
-        try:
-            object_version = obj_info["version"]
-            get_query_object_path(
-                settings[SettingsParameters.StateFilePath], object_name, object_version
-            )
-        except Exception as e:
-            logger.error(
-                f"Exception encounted when downloading object: {object_name}"
-                f", error: {e}"
-            )
-
-
-@gen.coroutine
-def init_model_evaluator(settings, tabpy_state, python_service):
-    """
-    This will go through all models that the service currently have and
-    initialize them.
-    """
-    logger.info("Initializing models...")
-
-    existing_pos = tabpy_state.get_endpoints()
-
-    for (object_name, obj_info) in existing_pos.items():
-        object_version = obj_info["version"]
-        object_type = obj_info["type"]
-        object_path = get_query_object_path(
-            settings[SettingsParameters.StateFilePath], object_name, object_version
-        )
-
-        logger.info(
-            f"Load endpoint: {object_name}, "
-            f"version: {object_version}, "
-            f"type: {object_type}"
-        )
-        if object_type == "alias":
-            msg = LoadObject(
-                object_name, obj_info["target"], object_version, False, "alias"
-            )
-        else:
-            local_path = object_path
-            msg = LoadObject(
-                object_name, local_path, object_version, False, object_type
-            )
-        python_service.manage_request(msg)
-
-
-def _get_latest_service_state(settings, tabpy_state, new_ps_state, python_service):
-    """
-    Update the endpoints from the latest remote state file.
-
-    Returns
-    --------
-    (has_changes, endpoint_diff):
-        has_changes: True or False
-        endpoint_diff: Summary of what has changed, one entry for each changes
-    """
-    # Shortcut when nothing is changed
-    changes = {"endpoints": {}}
-
-    # update endpoints
-    new_endpoints = new_ps_state.get_endpoints()
-    diff = {}
-    current_endpoints = python_service.ps.query_objects
-    for (endpoint_name, endpoint_info) in new_endpoints.items():
-        existing_endpoint = current_endpoints.get(endpoint_name)
-        if (existing_endpoint is None) or endpoint_info["version"] != existing_endpoint[
-            "version"
-        ]:
-            # Either a new endpoint or new endpoint version
-            path_to_new_version = get_query_object_path(
-                settings[SettingsParameters.StateFilePath],
-                endpoint_name,
-                endpoint_info["version"],
-            )
-            endpoint_type = endpoint_info.get("type", "model")
-            diff[endpoint_name] = (
-                endpoint_type,
-                endpoint_info["version"],
-                path_to_new_version,
-            )
-
-    # add removed models too
-    for (endpoint_name, endpoint_info) in current_endpoints.items():
-        if endpoint_name not in new_endpoints.keys():
-            endpoint_type = current_endpoints[endpoint_name].get("type", "model")
-            diff[endpoint_name] = (endpoint_type, None, None)
-
-    if diff:
-        changes["endpoints"] = diff
-
-    return (True, changes)
-
-
-@gen.coroutine
-def on_state_change(
-    settings, tabpy_state, python_service, logger=logging.getLogger(__name__)
-):
-    try:
-        logger.log(logging.INFO, "Loading state from state file")
-        config = util._get_state_from_file(
-            settings[SettingsParameters.StateFilePath], logger=logger
-        )
-        new_ps_state = TabPyState(config=config, settings=settings)
-
-        (has_changes, changes) = _get_latest_service_state(
-            settings, tabpy_state, new_ps_state, python_service
-        )
-        if not has_changes:
-            logger.info("Nothing changed, return.")
-            return
-
-        new_endpoints = new_ps_state.get_endpoints()
-        for object_name in changes["endpoints"]:
-            (object_type, object_version, object_path) = changes["endpoints"][
-                object_name
-            ]
-
-            if not object_path and not object_version:  # removal
-                logger.info(f"Removing object: URI={object_name}")
-
-                python_service.manage_request(DeleteObjects([object_name]))
-
-                cleanup_endpoint_files(
-                    object_name, settings[SettingsParameters.UploadDir], logger=logger
-                )
-
-            else:
-                endpoint_info = new_endpoints[object_name]
-                is_update = object_version > 1
-                if object_type == "alias":
-                    msg = LoadObject(
-                        object_name,
-                        endpoint_info["target"],
-                        object_version,
-                        is_update,
-                        "alias",
-                    )
-                else:
-                    local_path = object_path
-                    msg = LoadObject(
-                        object_name, local_path, object_version, is_update, object_type
-                    )
-
-                python_service.manage_request(msg)
-                wait_for_endpoint_loaded(python_service, object_name)
-
-                # cleanup old version of endpoint files
-                if object_version > 2:
-                    cleanup_endpoint_files(
-                        object_name,
-                        settings[SettingsParameters.UploadDir],
-                        logger=logger,
-                        retain_versions=[object_version, object_version - 1],
-                    )
-
-    except Exception as e:
-        err_msg = format_exception(e, "on_state_change")
-        logger.log(
-            logging.ERROR, f"Error submitting update model request: error={err_msg}"
-        )
+import logging
+from tabpy.tabpy_server.app.app_parameters import SettingsParameters
+from tabpy.tabpy_server.common.messages import (
+    LoadObject,
+    DeleteObjects,
+    ListObjects,
+    ObjectList,
+)
+from tabpy.tabpy_server.common.endpoint_file_mgr import cleanup_endpoint_files
+from tabpy.tabpy_server.common.util import format_exception
+from tabpy.tabpy_server.management.state import TabPyState, get_query_object_path
+from tabpy.tabpy_server.management import util
+from time import sleep
+from tornado import gen
+
+
+logger = logging.getLogger(__name__)
+
+
+def wait_for_endpoint_loaded(python_service, object_uri):
+    """
+    This method waits for the object to be loaded.
+    """
+    logger.info("Waiting for object to be loaded...")
+    while True:
+        msg = ListObjects()
+        list_object_msg = python_service.manage_request(msg)
+        if not isinstance(list_object_msg, ObjectList):
+            logger.error(f"Error loading endpoint {object_uri}: {list_object_msg}")
+            return
+
+        for (uri, info) in list_object_msg.objects.items():
+            if uri == object_uri:
+                if info["status"] != "LoadInProgress":
+                    logger.info(f'Object load status: {info["status"]}')
+                    return
+
+        sleep(0.1)
+
+
+@gen.coroutine
+def init_ps_server(settings, tabpy_state):
+    logger.info("Initializing TabPy Server...")
+    existing_pos = tabpy_state.get_endpoints()
+    for (object_name, obj_info) in existing_pos.items():
+        try:
+            object_version = obj_info["version"]
+            get_query_object_path(
+                settings[SettingsParameters.StateFilePath], object_name, object_version
+            )
+        except Exception as e:
+            logger.error(
+                f"Exception encounted when downloading object: {object_name}"
+                f", error: {e}"
+            )
+
+
+@gen.coroutine
+def init_model_evaluator(settings, tabpy_state, python_service):
+    """
+    This will go through all models that the service currently have and
+    initialize them.
+    """
+    logger.info("Initializing models...")
+
+    existing_pos = tabpy_state.get_endpoints()
+
+    for (object_name, obj_info) in existing_pos.items():
+        object_version = obj_info["version"]
+        object_type = obj_info["type"]
+        object_path = get_query_object_path(
+            settings[SettingsParameters.StateFilePath], object_name, object_version
+        )
+
+        logger.info(
+            f"Load endpoint: {object_name}, "
+            f"version: {object_version}, "
+            f"type: {object_type}"
+        )
+        if object_type == "alias":
+            msg = LoadObject(
+                object_name, obj_info["target"], object_version, False, "alias"
+            )
+        else:
+            local_path = object_path
+            msg = LoadObject(
+                object_name, local_path, object_version, False, object_type
+            )
+        python_service.manage_request(msg)
+
+
+def _get_latest_service_state(settings, tabpy_state, new_ps_state, python_service):
+    """
+    Update the endpoints from the latest remote state file.
+
+    Returns
+    --------
+    (has_changes, endpoint_diff):
+        has_changes: True or False
+        endpoint_diff: Summary of what has changed, one entry for each changes
+    """
+    # Shortcut when nothing is changed
+    changes = {"endpoints": {}}
+
+    # update endpoints
+    new_endpoints = new_ps_state.get_endpoints()
+    diff = {}
+    current_endpoints = python_service.ps.query_objects
+    for (endpoint_name, endpoint_info) in new_endpoints.items():
+        existing_endpoint = current_endpoints.get(endpoint_name)
+        if (existing_endpoint is None) or endpoint_info["version"] != existing_endpoint[
+            "version"
+        ]:
+            # Either a new endpoint or new endpoint version
+            path_to_new_version = get_query_object_path(
+                settings[SettingsParameters.StateFilePath],
+                endpoint_name,
+                endpoint_info["version"],
+            )
+            endpoint_type = endpoint_info.get("type", "model")
+            diff[endpoint_name] = (
+                endpoint_type,
+                endpoint_info["version"],
+                path_to_new_version,
+            )
+
+    # add removed models too
+    for (endpoint_name, endpoint_info) in current_endpoints.items():
+        if endpoint_name not in new_endpoints.keys():
+            endpoint_type = current_endpoints[endpoint_name].get("type", "model")
+            diff[endpoint_name] = (endpoint_type, None, None)
+
+    if diff:
+        changes["endpoints"] = diff
+
+    return (True, changes)
+
+
+@gen.coroutine
+def on_state_change(
+    settings, tabpy_state, python_service, logger=logging.getLogger(__name__)
+):
+    try:
+        logger.log(logging.INFO, "Loading state from state file")
+        config = util._get_state_from_file(
+            settings[SettingsParameters.StateFilePath], logger=logger
+        )
+        new_ps_state = TabPyState(config=config, settings=settings)
+
+        (has_changes, changes) = _get_latest_service_state(
+            settings, tabpy_state, new_ps_state, python_service
+        )
+        if not has_changes:
+            logger.info("Nothing changed, return.")
+            return
+
+        new_endpoints = new_ps_state.get_endpoints()
+        for object_name in changes["endpoints"]:
+            (object_type, object_version, object_path) = changes["endpoints"][
+                object_name
+            ]
+
+            if not object_path and not object_version:  # removal
+                logger.info(f"Removing object: URI={object_name}")
+
+                python_service.manage_request(DeleteObjects([object_name]))
+
+                cleanup_endpoint_files(
+                    object_name, settings[SettingsParameters.UploadDir], logger=logger
+                )
+
+            else:
+                endpoint_info = new_endpoints[object_name]
+                is_update = object_version > 1
+                if object_type == "alias":
+                    msg = LoadObject(
+                        object_name,
+                        endpoint_info["target"],
+                        object_version,
+                        is_update,
+                        "alias",
+                    )
+                else:
+                    local_path = object_path
+                    msg = LoadObject(
+                        object_name, local_path, object_version, is_update, object_type
+                    )
+
+                python_service.manage_request(msg)
+                wait_for_endpoint_loaded(python_service, object_name)
+
+                # cleanup old version of endpoint files
+                if object_version > 2:
+                    cleanup_endpoint_files(
+                        object_name,
+                        settings[SettingsParameters.UploadDir],
+                        logger=logger,
+                        retain_versions=[object_version, object_version - 1],
+                    )
+
+    except Exception as e:
+        err_msg = format_exception(e, "on_state_change")
+        logger.log(
+            logging.ERROR, f"Error submitting update model request: error={err_msg}"
+        )
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/static/TabPy_logo.png` & `tabpy-2.7.0/tabpy/tabpy_server/static/TabPy_logo.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/tabpy/tabpy_server/static/tableau.png` & `tabpy-2.7.0/tabpy/tabpy_server/static/tableau.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/tabpy/tabpy_tools/client.py` & `tabpy-2.7.0/tabpy/tabpy_tools/client.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,389 +1,389 @@
-import copy
-from re import compile
-import time
-import requests
-
-from .rest import RequestsNetworkWrapper, ServiceClient
-
-from .rest_client import RESTServiceClient, Endpoint
-
-from .custom_query_object import CustomQueryObject
-import os
-import logging
-
-logger = logging.getLogger(__name__)
-
-_name_checker = compile(r"^[\w -]+$")
-
-
-def _check_endpoint_type(name):
-    if not isinstance(name, str):
-        raise TypeError("Endpoint name must be a string")
-
-    if name == "":
-        raise ValueError("Endpoint name cannot be empty")
-
-
-def _check_hostname(name):
-    _check_endpoint_type(name)
-    hostname_checker = compile(r"^^http(s)?://[\w.-]+(/)?(:\d+)?(/)?$")
-
-    if not hostname_checker.match(name):
-        raise ValueError(
-            f"endpoint name {name} should be in http(s)://<hostname>"
-            "[:<port>] and hostname may consist only of: "
-            "a-z, A-Z, 0-9, underscore and hyphens."
-        )
-
-
-def _check_endpoint_name(name):
-    """Checks that the endpoint name is valid by comparing it with an RE and
-    checking that it is not reserved."""
-    _check_endpoint_type(name)
-
-    if not _name_checker.match(name):
-        raise ValueError(
-            f"endpoint name {name} can only contain: a-z, A-Z, 0-9,"
-            " underscore, hyphens and spaces."
-        )
-
-
-class Client:
-    def __init__(self, endpoint, query_timeout=1000):
-        """
-        Connects to a running server.
-
-        The class constructor takes a server address which is then used to
-        connect for all subsequent member APIs.
-
-        Parameters
-        ----------
-        endpoint : str, optional
-            The server URL.
-
-        query_timeout : float, optional
-            The timeout for query operations.
-        """
-        _check_hostname(endpoint)
-
-        self._endpoint = endpoint
-
-        session = requests.session()
-        session.verify = False
-        requests.packages.urllib3.disable_warnings()
-
-        # Setup the communications layer.
-        network_wrapper = RequestsNetworkWrapper(session)
-        service_client = ServiceClient(self._endpoint, network_wrapper)
-
-        self._service = RESTServiceClient(service_client)
-        if not type(query_timeout) in (int, float) or query_timeout <= 0:
-            query_timeout = 0.0
-        self._service.query_timeout = query_timeout
-
-    def __repr__(self):
-        return (
-            "<"
-            + self.__class__.__name__
-            + " object at "
-            + hex(id(self))
-            + " connected to "
-            + repr(self._endpoint)
-            + ">"
-        )
-
-    def get_status(self):
-        """
-        Gets the status of the deployed endpoints.
-
-        Returns
-        -------
-        dict
-            Keys are endpoints and values are dicts describing the state of
-            the endpoint.
-
-        Examples
-        --------
-        .. sourcecode:: python
-            {
-                u'foo': {
-                    u'status': u'LoadFailed',
-                    u'last_error': u'error mesasge',
-                    u'version': 1,
-                    u'type': u'model',
-                },
-            }
-        """
-        return self._service.get_status()
-
-    #
-    # Query
-    #
-
-    @property
-    def query_timeout(self):
-        """The timeout for queries in milliseconds."""
-        return self._service.query_timeout
-
-    @query_timeout.setter
-    def query_timeout(self, value):
-        if type(value) in (int, float) and value > 0:
-            self._service.query_timeout = value
-
-    def query(self, name, *args, **kwargs):
-        """Query an endpoint.
-
-        Parameters
-        ----------
-        name : str
-            The name of the endpoint.
-
-        *args : list of anything
-            Ordered parameters to the endpoint.
-
-        **kwargs : dict of anything
-            Named parameters to the endpoint.
-
-        Returns
-        -------
-        dict
-            Keys are:
-                model: the name of the endpoint
-                version: the version used.
-                response: the response to the query.
-                uuid : a unique id for the request.
-        """
-        return self._service.query(name, *args, **kwargs)
-
-    #
-    # Endpoints
-    #
-
-    def get_endpoints(self, type=None):
-        """Returns all deployed endpoints.
-
-        Examples
-        --------
-        .. sourcecode:: python
-            {"clustering":
-              {"description": "",
-               "docstring": "-- no docstring found in query function --",
-               "creation_time": 1469511182,
-               "version": 1,
-               "dependencies": [],
-               "last_modified_time": 1469511182,
-               "type": "model",
-               "target": null},
-            "add": {
-              "description": "",
-              "docstring": "-- no docstring found in query function --",
-              "creation_time": 1469505967,
-              "version": 1,
-              "dependencies": [],
-              "last_modified_time": 1469505967,
-              "type": "model",
-              "target": null}
-            }
-        """
-        return self._service.get_endpoints(type)
-
-    def _get_endpoint_upload_destination(self):
-        """Returns the endpoint upload destination."""
-        return self._service.get_endpoint_upload_destination()["path"]
-
-    def deploy(self, name, obj, description="", schema=None, override=False):
-        """Deploys a Python function as an endpoint in the server.
-
-        Parameters
-        ----------
-        name : str
-            A unique identifier for the endpoint.
-
-        obj :  function
-            Refers to a user-defined function with any signature. However both
-            input and output of the function need to be JSON serializable.
-
-        description : str, optional
-            The description for the endpoint. This string will be returned by
-            the ``endpoints`` API.
-
-        schema : dict, optional
-            The schema of the function, containing information about input and
-            output parameters, and respective examples. Providing a schema for
-            a deployed function lets other users of the service discover how to
-            use it. Refer to schema.generate_schema for more information on
-            how to generate the schema.
-
-        override : bool
-            Whether to override (update) an existing endpoint. If False and
-            there is already an endpoint with that name, it will raise a
-            RuntimeError. If True and there is already an endpoint with that
-            name, it will deploy a new version on top of it.
-
-        See Also
-        --------
-        remove, get_endpoints
-        """
-        endpoint = self.get_endpoints().get(name)
-        version = 1
-        if endpoint:
-            if not override:
-                raise RuntimeError(
-                    f"An endpoint with that name ({name}) already"
-                    ' exists. Use "override = True" to force update '
-                    "an existing endpoint."
-                )
-
-            version = endpoint.version + 1
-
-        obj = self._gen_endpoint(name, obj, description, version, schema)
-
-        self._upload_endpoint(obj)
-
-        if version == 1:
-            self._service.add_endpoint(Endpoint(**obj))
-        else:
-            self._service.set_endpoint(Endpoint(**obj))
-
-        self._wait_for_endpoint_deployment(obj["name"], obj["version"])
-
-    def remove(self, name):
-        '''Removes an endpoint dict.
-
-        Parameters
-        ----------
-        name : str
-            Endpoint name to remove'''
-        self._service.remove_endpoint(name)
-
-    def _gen_endpoint(self, name, obj, description, version=1, schema=None):
-        """Generates an endpoint dict.
-
-        Parameters
-        ----------
-        name : str
-            Endpoint name to add or update
-
-        obj :  func
-            Object that backs the endpoint. See add() for a complete
-            description.
-
-        description : str
-            Description of the endpoint
-
-        version : int
-            The version. Defaults to 1.
-
-        Returns
-        -------
-        dict
-            Keys:
-                name : str
-                    The name provided.
-
-                version : int
-                    The version provided.
-
-                description : str
-                    The provided description.
-
-                type : str
-                    The type of the endpoint.
-
-                endpoint_obj : object
-                    The wrapper around the obj provided that can be used to
-                    generate the code and dependencies for the endpoint.
-
-        Raises
-        ------
-        TypeError
-            When obj is not one of the expected types.
-        """
-        # check for invalid PO names
-        _check_endpoint_name(name)
-
-        if description is None:
-            description = obj.__doc__.strip() or "" if isinstance(obj.__doc__, str) else ""
-
-        endpoint_object = CustomQueryObject(query=obj, description=description,)
-
-        return {
-            "name": name,
-            "version": version,
-            "description": description,
-            "type": "model",
-            "endpoint_obj": endpoint_object,
-            "dependencies": endpoint_object.get_dependencies(),
-            "methods": endpoint_object.get_methods(),
-            "required_files": [],
-            "required_packages": [],
-            "schema": copy.copy(schema),
-        }
-
-    def _upload_endpoint(self, obj):
-        """Sends the endpoint across the wire."""
-        endpoint_obj = obj["endpoint_obj"]
-
-        dest_path = self._get_endpoint_upload_destination()
-
-        # Upload the endpoint
-        obj["src_path"] = os.path.join(
-            dest_path, "endpoints", obj["name"], str(obj["version"])
-        )
-
-        endpoint_obj.save(obj["src_path"])
-
-    def _wait_for_endpoint_deployment(
-        self, endpoint_name, version=1, interval=1.0,
-    ):
-        """
-        Waits for the endpoint to be deployed by calling get_status() and
-        checking the versions deployed of the endpoint against the expected
-        version. If all the versions are equal to or greater than the version
-        expected, then it will return. Uses time.sleep().
-        """
-        logger.info(
-            f"Waiting for endpoint {endpoint_name} to deploy to " f"version {version}"
-        )
-        start = time.time()
-        while True:
-            ep_status = self.get_status()
-            try:
-                ep = ep_status[endpoint_name]
-            except KeyError:
-                logger.info(
-                    f"Endpoint {endpoint_name} doesn't " "exist in endpoints yet"
-                )
-            else:
-                logger.info(f"ep={ep}")
-
-                if ep["status"] == "LoadFailed":
-                    raise RuntimeError(f'LoadFailed: {ep["last_error"]}')
-
-                elif ep["status"] == "LoadSuccessful":
-                    if ep["version"] >= version:
-                        logger.info("LoadSuccessful")
-                        break
-                    else:
-                        logger.info("LoadSuccessful but wrong version")
-
-            if time.time() - start > 10:
-                raise RuntimeError("Waited more then 10s for deployment")
-
-            logger.info(f"Sleeping {interval}...")
-            time.sleep(interval)
-
-    def set_credentials(self, username, password):
-        """
-        Set credentials for all the TabPy client-server communication
-        where client is tabpy-tools and server is tabpy-server.
-
-        Parameters
-        ----------
-        username : str
-            User name (login). Username is case insensitive.
-
-        password : str
-            Password in plain text.
-        """
-        self._service.set_credentials(username, password)
+import copy
+from re import compile
+import time
+import requests
+
+from .rest import RequestsNetworkWrapper, ServiceClient
+
+from .rest_client import RESTServiceClient, Endpoint
+
+from .custom_query_object import CustomQueryObject
+import os
+import logging
+
+logger = logging.getLogger(__name__)
+
+_name_checker = compile(r"^[\w -]+$")
+
+
+def _check_endpoint_type(name):
+    if not isinstance(name, str):
+        raise TypeError("Endpoint name must be a string")
+
+    if name == "":
+        raise ValueError("Endpoint name cannot be empty")
+
+
+def _check_hostname(name):
+    _check_endpoint_type(name)
+    hostname_checker = compile(r"^^http(s)?://[\w.-]+(/)?(:\d+)?(/)?$")
+
+    if not hostname_checker.match(name):
+        raise ValueError(
+            f"endpoint name {name} should be in http(s)://<hostname>"
+            "[:<port>] and hostname may consist only of: "
+            "a-z, A-Z, 0-9, underscore and hyphens."
+        )
+
+
+def _check_endpoint_name(name):
+    """Checks that the endpoint name is valid by comparing it with an RE and
+    checking that it is not reserved."""
+    _check_endpoint_type(name)
+
+    if not _name_checker.match(name):
+        raise ValueError(
+            f"endpoint name {name} can only contain: a-z, A-Z, 0-9,"
+            " underscore, hyphens and spaces."
+        )
+
+
+class Client:
+    def __init__(self, endpoint, query_timeout=1000):
+        """
+        Connects to a running server.
+
+        The class constructor takes a server address which is then used to
+        connect for all subsequent member APIs.
+
+        Parameters
+        ----------
+        endpoint : str, optional
+            The server URL.
+
+        query_timeout : float, optional
+            The timeout for query operations.
+        """
+        _check_hostname(endpoint)
+
+        self._endpoint = endpoint
+
+        session = requests.session()
+        session.verify = False
+        requests.packages.urllib3.disable_warnings()
+
+        # Setup the communications layer.
+        network_wrapper = RequestsNetworkWrapper(session)
+        service_client = ServiceClient(self._endpoint, network_wrapper)
+
+        self._service = RESTServiceClient(service_client)
+        if not type(query_timeout) in (int, float) or query_timeout <= 0:
+            query_timeout = 0.0
+        self._service.query_timeout = query_timeout
+
+    def __repr__(self):
+        return (
+            "<"
+            + self.__class__.__name__
+            + " object at "
+            + hex(id(self))
+            + " connected to "
+            + repr(self._endpoint)
+            + ">"
+        )
+
+    def get_status(self):
+        """
+        Gets the status of the deployed endpoints.
+
+        Returns
+        -------
+        dict
+            Keys are endpoints and values are dicts describing the state of
+            the endpoint.
+
+        Examples
+        --------
+        .. sourcecode:: python
+            {
+                u'foo': {
+                    u'status': u'LoadFailed',
+                    u'last_error': u'error mesasge',
+                    u'version': 1,
+                    u'type': u'model',
+                },
+            }
+        """
+        return self._service.get_status()
+
+    #
+    # Query
+    #
+
+    @property
+    def query_timeout(self):
+        """The timeout for queries in milliseconds."""
+        return self._service.query_timeout
+
+    @query_timeout.setter
+    def query_timeout(self, value):
+        if type(value) in (int, float) and value > 0:
+            self._service.query_timeout = value
+
+    def query(self, name, *args, **kwargs):
+        """Query an endpoint.
+
+        Parameters
+        ----------
+        name : str
+            The name of the endpoint.
+
+        *args : list of anything
+            Ordered parameters to the endpoint.
+
+        **kwargs : dict of anything
+            Named parameters to the endpoint.
+
+        Returns
+        -------
+        dict
+            Keys are:
+                model: the name of the endpoint
+                version: the version used.
+                response: the response to the query.
+                uuid : a unique id for the request.
+        """
+        return self._service.query(name, *args, **kwargs)
+
+    #
+    # Endpoints
+    #
+
+    def get_endpoints(self, type=None):
+        """Returns all deployed endpoints.
+
+        Examples
+        --------
+        .. sourcecode:: python
+            {"clustering":
+              {"description": "",
+               "docstring": "-- no docstring found in query function --",
+               "creation_time": 1469511182,
+               "version": 1,
+               "dependencies": [],
+               "last_modified_time": 1469511182,
+               "type": "model",
+               "target": null},
+            "add": {
+              "description": "",
+              "docstring": "-- no docstring found in query function --",
+              "creation_time": 1469505967,
+              "version": 1,
+              "dependencies": [],
+              "last_modified_time": 1469505967,
+              "type": "model",
+              "target": null}
+            }
+        """
+        return self._service.get_endpoints(type)
+
+    def _get_endpoint_upload_destination(self):
+        """Returns the endpoint upload destination."""
+        return self._service.get_endpoint_upload_destination()["path"]
+
+    def deploy(self, name, obj, description="", schema=None, override=False):
+        """Deploys a Python function as an endpoint in the server.
+
+        Parameters
+        ----------
+        name : str
+            A unique identifier for the endpoint.
+
+        obj :  function
+            Refers to a user-defined function with any signature. However both
+            input and output of the function need to be JSON serializable.
+
+        description : str, optional
+            The description for the endpoint. This string will be returned by
+            the ``endpoints`` API.
+
+        schema : dict, optional
+            The schema of the function, containing information about input and
+            output parameters, and respective examples. Providing a schema for
+            a deployed function lets other users of the service discover how to
+            use it. Refer to schema.generate_schema for more information on
+            how to generate the schema.
+
+        override : bool
+            Whether to override (update) an existing endpoint. If False and
+            there is already an endpoint with that name, it will raise a
+            RuntimeError. If True and there is already an endpoint with that
+            name, it will deploy a new version on top of it.
+
+        See Also
+        --------
+        remove, get_endpoints
+        """
+        endpoint = self.get_endpoints().get(name)
+        version = 1
+        if endpoint:
+            if not override:
+                raise RuntimeError(
+                    f"An endpoint with that name ({name}) already"
+                    ' exists. Use "override = True" to force update '
+                    "an existing endpoint."
+                )
+
+            version = endpoint.version + 1
+
+        obj = self._gen_endpoint(name, obj, description, version, schema)
+
+        self._upload_endpoint(obj)
+
+        if version == 1:
+            self._service.add_endpoint(Endpoint(**obj))
+        else:
+            self._service.set_endpoint(Endpoint(**obj))
+
+        self._wait_for_endpoint_deployment(obj["name"], obj["version"])
+
+    def remove(self, name):
+        '''Removes an endpoint dict.
+
+        Parameters
+        ----------
+        name : str
+            Endpoint name to remove'''
+        self._service.remove_endpoint(name)
+
+    def _gen_endpoint(self, name, obj, description, version=1, schema=None):
+        """Generates an endpoint dict.
+
+        Parameters
+        ----------
+        name : str
+            Endpoint name to add or update
+
+        obj :  func
+            Object that backs the endpoint. See add() for a complete
+            description.
+
+        description : str
+            Description of the endpoint
+
+        version : int
+            The version. Defaults to 1.
+
+        Returns
+        -------
+        dict
+            Keys:
+                name : str
+                    The name provided.
+
+                version : int
+                    The version provided.
+
+                description : str
+                    The provided description.
+
+                type : str
+                    The type of the endpoint.
+
+                endpoint_obj : object
+                    The wrapper around the obj provided that can be used to
+                    generate the code and dependencies for the endpoint.
+
+        Raises
+        ------
+        TypeError
+            When obj is not one of the expected types.
+        """
+        # check for invalid PO names
+        _check_endpoint_name(name)
+
+        if description is None:
+            description = obj.__doc__.strip() or "" if isinstance(obj.__doc__, str) else ""
+
+        endpoint_object = CustomQueryObject(query=obj, description=description,)
+
+        return {
+            "name": name,
+            "version": version,
+            "description": description,
+            "type": "model",
+            "endpoint_obj": endpoint_object,
+            "dependencies": endpoint_object.get_dependencies(),
+            "methods": endpoint_object.get_methods(),
+            "required_files": [],
+            "required_packages": [],
+            "schema": copy.copy(schema),
+        }
+
+    def _upload_endpoint(self, obj):
+        """Sends the endpoint across the wire."""
+        endpoint_obj = obj["endpoint_obj"]
+
+        dest_path = self._get_endpoint_upload_destination()
+
+        # Upload the endpoint
+        obj["src_path"] = os.path.join(
+            dest_path, "endpoints", obj["name"], str(obj["version"])
+        )
+
+        endpoint_obj.save(obj["src_path"])
+
+    def _wait_for_endpoint_deployment(
+        self, endpoint_name, version=1, interval=1.0,
+    ):
+        """
+        Waits for the endpoint to be deployed by calling get_status() and
+        checking the versions deployed of the endpoint against the expected
+        version. If all the versions are equal to or greater than the version
+        expected, then it will return. Uses time.sleep().
+        """
+        logger.info(
+            f"Waiting for endpoint {endpoint_name} to deploy to " f"version {version}"
+        )
+        start = time.time()
+        while True:
+            ep_status = self.get_status()
+            try:
+                ep = ep_status[endpoint_name]
+            except KeyError:
+                logger.info(
+                    f"Endpoint {endpoint_name} doesn't " "exist in endpoints yet"
+                )
+            else:
+                logger.info(f"ep={ep}")
+
+                if ep["status"] == "LoadFailed":
+                    raise RuntimeError(f'LoadFailed: {ep["last_error"]}')
+
+                elif ep["status"] == "LoadSuccessful":
+                    if ep["version"] >= version:
+                        logger.info("LoadSuccessful")
+                        break
+                    else:
+                        logger.info("LoadSuccessful but wrong version")
+
+            if time.time() - start > 10:
+                raise RuntimeError("Waited more then 10s for deployment")
+
+            logger.info(f"Sleeping {interval}...")
+            time.sleep(interval)
+
+    def set_credentials(self, username, password):
+        """
+        Set credentials for all the TabPy client-server communication
+        where client is tabpy-tools and server is tabpy-server.
+
+        Parameters
+        ----------
+        username : str
+            User name (login). Username is case insensitive.
+
+        password : str
+            Password in plain text.
+        """
+        self._service.set_credentials(username, password)
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_tools/custom_query_object.py` & `tabpy-2.7.0/tabpy/tabpy_tools/custom_query_object.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import logging
-from .query_object import QueryObject as _QueryObject
-
-
-logger = logging.getLogger(__name__)
-
-
-class CustomQueryObject(_QueryObject):
-    def __init__(self, query, description=""):
-        """Create a new CustomQueryObject.
-
-        Parameters
-        -----------
-
-        query : function
-            Function that defines a custom query method. The query can have any
-            signature, but input and output of the query needs to be JSON
-            serializable.
-
-        description : str
-            The description of the custom query object
-
-        """
-        super().__init__(description)
-
-        self.custom_query = query
-
-    def query(self, *args, **kwargs):
-        """Query the custom defined query method using the given input.
-
-        Parameters
-        ----------
-        args : list
-            positional arguments to the query
-
-        kwargs : dict
-            keyword arguments to the query
-
-        Returns
-        -------
-        out: object.
-            The results depends on the implementation of the query method.
-            Typically the return value will be whatever that function returns.
-
-        See Also
-        --------
-        QueryObject
-        """
-        # include the dependent files in sys path so that the query can run
-        # correctly
-
-        try:
-            logger.debug(
-                "Running custom query with arguments " f"({args}, {kwargs})..."
-            )
-            ret = self.custom_query(*args, **kwargs)
-        except Exception as e:
-            logger.exception(
-                "Exception hit when running custom query, error: " f"{str(e)}"
-            )
-            raise
-
-        logger.debug(f"Received response {ret}")
-        try:
-            return self._make_serializable(ret)
-        except Exception as e:
-            logger.exception(
-                "Cannot properly serialize custom query result, " f"error: {str(e)}"
-            )
-            raise
-
-    def get_doc_string(self):
-        """Get doc string from customized query"""
-        if self.custom_query.__doc__ is not None:
-            return self.custom_query.__doc__
-        else:
-            return "-- no docstring found in query function --"
-
-    def get_methods(self):
-        return [self.get_query_method()]
-
-    def get_query_method(self):
-        return {"method": "query"}
+import logging
+from .query_object import QueryObject as _QueryObject
+
+
+logger = logging.getLogger(__name__)
+
+
+class CustomQueryObject(_QueryObject):
+    def __init__(self, query, description=""):
+        """Create a new CustomQueryObject.
+
+        Parameters
+        -----------
+
+        query : function
+            Function that defines a custom query method. The query can have any
+            signature, but input and output of the query needs to be JSON
+            serializable.
+
+        description : str
+            The description of the custom query object
+
+        """
+        super().__init__(description)
+
+        self.custom_query = query
+
+    def query(self, *args, **kwargs):
+        """Query the custom defined query method using the given input.
+
+        Parameters
+        ----------
+        args : list
+            positional arguments to the query
+
+        kwargs : dict
+            keyword arguments to the query
+
+        Returns
+        -------
+        out: object.
+            The results depends on the implementation of the query method.
+            Typically the return value will be whatever that function returns.
+
+        See Also
+        --------
+        QueryObject
+        """
+        # include the dependent files in sys path so that the query can run
+        # correctly
+
+        try:
+            logger.debug(
+                "Running custom query with arguments " f"({args}, {kwargs})..."
+            )
+            ret = self.custom_query(*args, **kwargs)
+        except Exception as e:
+            logger.exception(
+                "Exception hit when running custom query, error: " f"{str(e)}"
+            )
+            raise
+
+        logger.debug(f"Received response {ret}")
+        try:
+            return self._make_serializable(ret)
+        except Exception as e:
+            logger.exception(
+                "Cannot properly serialize custom query result, " f"error: {str(e)}"
+            )
+            raise
+
+    def get_doc_string(self):
+        """Get doc string from customized query"""
+        if self.custom_query.__doc__ is not None:
+            return self.custom_query.__doc__
+        else:
+            return "-- no docstring found in query function --"
+
+    def get_methods(self):
+        return [self.get_query_method()]
+
+    def get_query_method(self):
+        return {"method": "query"}
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_tools/query_object.py` & `tabpy-2.7.0/tabpy/tabpy_tools/query_object.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-import abc
-import logging
-import os
-import json
-import shutil
-
-import cloudpickle as _cloudpickle
-
-
-logger = logging.getLogger(__name__)
-
-
-class QueryObject(abc.ABC):
-    """
-    Derived class needs to implement the following interface:
-      * query() -- given input, return query result
-      * get_doc_string() -- returns documentation for the Query Object
-    """
-
-    def __init__(self, description=""):
-        self.description = description
-
-    def get_dependencies(self):
-        """All endpoints this endpoint depends on"""
-        return []
-
-    @abc.abstractmethod
-    def query(self, input):
-        """execute query on the provided input"""
-        pass
-
-    @abc.abstractmethod
-    def get_doc_string(self):
-        """Returns documentation for the query object
-
-        By default, this method returns the docstring for 'query' method
-        Derived class may overwrite this method to dynamically create docstring
-        """
-        pass
-
-    def save(self, path):
-        """ Save query object to the given local path
-
-        Parameters
-        ----------
-        path : str
-          The location to save the query object to
-        """
-        if os.path.exists(path):
-            logger.warning(
-                f'Overwriting existing file "{path}" when saving query object'
-            )
-            rm_fn = os.remove if os.path.isfile(path) else shutil.rmtree
-            rm_fn(path)
-        self._save_local(path)
-
-    def _save_local(self, path):
-        """Save current query object to local path
-        """
-        try:
-            os.makedirs(path)
-        except OSError as e:
-            import errno
-
-            if e.errno == errno.EEXIST and os.path.isdir(path):
-                pass
-            else:
-                raise
-
-        with open(os.path.join(path, "pickle_archive"), "wb") as f:
-            _cloudpickle.dump(self, f)
-
-    @classmethod
-    def load(cls, path):
-        """ Load query object from given path
-        """
-        new_po = None
-        new_po = cls._load_local(path)
-
-        logger.info(f'Loaded query object "{type(new_po).__name__}" successfully')
-
-        return new_po
-
-    @classmethod
-    def _load_local(cls, path):
-        path = os.path.abspath(os.path.expanduser(path))
-        with open(os.path.join(path, "pickle_archive"), "rb") as f:
-            return _cloudpickle.load(f)
-
-    @classmethod
-    def _make_serializable(cls, result):
-        """Convert a result from object query to python data structure that can
-        easily serialize over network
-        """
-        try:
-            json.dumps(result)
-        except TypeError:
-            raise TypeError(
-                "Result from object query is not json serializable: " f"{result}"
-            )
-
-        return result
-
-    # Returns an array of dictionary that contains the methods and their
-    # corresponding schema information.
-    @abc.abstractmethod
-    def get_methods(self):
-        return None
+import abc
+import logging
+import os
+import json
+import shutil
+
+import cloudpickle as _cloudpickle
+
+
+logger = logging.getLogger(__name__)
+
+
+class QueryObject(abc.ABC):
+    """
+    Derived class needs to implement the following interface:
+      * query() -- given input, return query result
+      * get_doc_string() -- returns documentation for the Query Object
+    """
+
+    def __init__(self, description=""):
+        self.description = description
+
+    def get_dependencies(self):
+        """All endpoints this endpoint depends on"""
+        return []
+
+    @abc.abstractmethod
+    def query(self, input):
+        """execute query on the provided input"""
+        pass
+
+    @abc.abstractmethod
+    def get_doc_string(self):
+        """Returns documentation for the query object
+
+        By default, this method returns the docstring for 'query' method
+        Derived class may overwrite this method to dynamically create docstring
+        """
+        pass
+
+    def save(self, path):
+        """ Save query object to the given local path
+
+        Parameters
+        ----------
+        path : str
+          The location to save the query object to
+        """
+        if os.path.exists(path):
+            logger.warning(
+                f'Overwriting existing file "{path}" when saving query object'
+            )
+            rm_fn = os.remove if os.path.isfile(path) else shutil.rmtree
+            rm_fn(path)
+        self._save_local(path)
+
+    def _save_local(self, path):
+        """Save current query object to local path
+        """
+        try:
+            os.makedirs(path)
+        except OSError as e:
+            import errno
+
+            if e.errno == errno.EEXIST and os.path.isdir(path):
+                pass
+            else:
+                raise
+
+        with open(os.path.join(path, "pickle_archive"), "wb") as f:
+            _cloudpickle.dump(self, f)
+
+    @classmethod
+    def load(cls, path):
+        """ Load query object from given path
+        """
+        new_po = None
+        new_po = cls._load_local(path)
+
+        logger.info(f'Loaded query object "{type(new_po).__name__}" successfully')
+
+        return new_po
+
+    @classmethod
+    def _load_local(cls, path):
+        path = os.path.abspath(os.path.expanduser(path))
+        with open(os.path.join(path, "pickle_archive"), "rb") as f:
+            return _cloudpickle.load(f)
+
+    @classmethod
+    def _make_serializable(cls, result):
+        """Convert a result from object query to python data structure that can
+        easily serialize over network
+        """
+        try:
+            json.dumps(result)
+        except TypeError:
+            raise TypeError(
+                "Result from object query is not json serializable: " f"{result}"
+            )
+
+        return result
+
+    # Returns an array of dictionary that contains the methods and their
+    # corresponding schema information.
+    @abc.abstractmethod
+    def get_methods(self):
+        return None
```

### Comparing `tabpy-2.6.0/tabpy/tabpy_tools/rest.py` & `tabpy-2.7.0/tabpy/tabpy_tools/rest.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,423 +1,423 @@
-import abc
-from collections.abc import MutableMapping
-import logging
-import requests
-from requests.auth import HTTPBasicAuth
-from re import compile
-import json as json
-
-
-logger = logging.getLogger(__name__)
-
-
-class ResponseError(Exception):
-    """Raised when we get an unexpected response."""
-
-    def __init__(self, response):
-        super().__init__("Unexpected server response")
-        self.response = response
-        self.status_code = response.status_code
-
-        try:
-            r = response.json()
-            self.info = r["info"]
-            self.message = response.json()["message"]
-        except (json.JSONDecodeError, KeyError):
-            self.info = None
-            self.message = response.text
-
-    def __str__(self):
-        return f"({self.status_code}) " f"{self.message} " f"{self.info}"
-
-
-class RequestsNetworkWrapper:
-    """The NetworkWrapper wraps the underlying network connection to simplify
-    the interface a bit. This can be replaced with something that can be built
-    on some other type of network connection, such as PyCURL.
-
-    This version requires you to instantiate a requests session object to your
-    liking. It will create a generic session for you if you don't specify it,
-    which you can modify later.
-
-    For authentication, use::
-
-        session.auth = (username, password)
-    """
-
-    def __init__(self, session=None):
-        # Set .auth as appropriate.
-        if session is None:
-            session = requests.session()
-
-        self.session = session
-        self.auth = None
-
-    @staticmethod
-    def raise_error(response):
-        logger.error(
-            f"Error with server response. code={response.status_code}; "
-            f"text={response.text}"
-        )
-
-        raise ResponseError(response)
-
-    @staticmethod
-    def _remove_nones(data):
-        if isinstance(data, dict):
-            for k in [k for k, v in data.items() if v is None]:
-                del data[k]
-
-    def _encode_request(self, data):
-        self._remove_nones(data)
-
-        if data is not None:
-            return json.dumps(data)
-        else:
-            return None
-
-    def GET(self, url, data, timeout=None):
-        """Issues a GET request to the URL with the data specified. Returns an
-        object that is parsed from the response JSON."""
-        self._remove_nones(data)
-
-        logger.info(f"GET {url} with {data}")
-
-        response = self.session.get(url, params=data, timeout=timeout, auth=self.auth)
-        if response.status_code != 200:
-            self.raise_error(response)
-        logger.info(f"response={response.text}")
-
-        if response.text == "":
-            return dict()
-        else:
-            return response.json()
-
-    def POST(self, url, data, timeout=None):
-        """Issues a POST request to the URL with the data specified. Returns an
-        object that is parsed from the response JSON."""
-        data = self._encode_request(data)
-
-        logger.info(f"POST {url} with {data}")
-        response = self.session.post(
-            url,
-            data=data,
-            headers={"content-type": "application/json"},
-            timeout=timeout,
-            auth=self.auth,
-        )
-
-        if response.status_code not in (200, 201):
-            self.raise_error(response)
-
-        return response.json()
-
-    def PUT(self, url, data, timeout=None):
-        """Issues a PUT request to the URL with the data specified. Returns an
-        object that is parsed from the response JSON."""
-        data = self._encode_request(data)
-
-        logger.info(f"PUT {url} with {data}")
-
-        response = self.session.put(
-            url,
-            data=data,
-            headers={"content-type": "application/json"},
-            timeout=timeout,
-            auth=self.auth,
-        )
-        if response.status_code != 200:
-            self.raise_error(response)
-
-        return response.json()
-
-    def DELETE(self, url, data, timeout=None):
-        """
-        Issues a DELETE request to the URL with the data specified. Returns an
-        object that is parsed from the response JSON.
-        """
-        if data is not None:
-            data = json.dumps(data)
-
-        logger.info(f"DELETE {url} with {data}")
-
-        response = self.session.delete(url, data=data, timeout=timeout, auth=self.auth)
-
-        if response.status_code <= 499 and response.status_code >= 400:
-            raise RuntimeError(response.text)
-
-        if response.status_code not in (200, 201, 204):
-            raise RuntimeError(
-                f"Error with server response code: {response.status_code}"
-            )
-
-    def set_credentials(self, username, password):
-        """
-        Set credentials for all the TabPy client-server communication
-        where client is tabpy-tools and server is tabpy-server.
-
-        Parameters
-        ----------
-        username : str
-            User name (login). Username is case insensitive.
-
-        password : str
-            Password in plain text.
-        """
-        logger.info(f"Setting credentials (username: {username})")
-        self.auth = HTTPBasicAuth(username, password)
-
-
-class ServiceClient:
-    """
-    A generic service client.
-
-    This will take an endpoint URL and a network_wrapper. You can use the
-    RequestsNetworkWrapper if you want to use the requests module. The
-    endpoint URL is prepended to all the requests and forwarded to the network
-    wrapper.
-    """
-
-    def __init__(self, endpoint, network_wrapper=None):
-        if network_wrapper is None:
-            network_wrapper = RequestsNetworkWrapper(session=requests.session())
-
-        self.network_wrapper = network_wrapper
-
-        pattern = compile(".*(:[0-9]+)$")
-        if not endpoint.endswith("/") and not pattern.match(endpoint):
-            logger.warning(f"endpoint {endpoint} does not end with '/': appending.")
-            endpoint = endpoint + "/"
-
-        self.endpoint = endpoint
-
-    def GET(self, url, data=None, timeout=None):
-        """Prepends self.endpoint to the url and issues a GET request."""
-        return self.network_wrapper.GET(self.endpoint + url, data, timeout)
-
-    def POST(self, url, data=None, timeout=None):
-        """Prepends self.endpoint to the url and issues a POST request."""
-        return self.network_wrapper.POST(self.endpoint + url, data, timeout)
-
-    def PUT(self, url, data=None, timeout=None):
-        """Prepends self.endpoint to the url and issues a PUT request."""
-        return self.network_wrapper.PUT(self.endpoint + url, data, timeout)
-
-    def DELETE(self, url, data=None, timeout=None):
-        """Prepends self.endpoint to the url and issues a DELETE request."""
-        self.network_wrapper.DELETE(self.endpoint + url, data, timeout)
-
-    def set_credentials(self, username, password):
-        """
-        Set credentials for all the TabPy client-server communication
-        where client is tabpy-tools and server is tabpy-server.
-
-        Parameters
-        ----------
-        username : str
-            User name (login). Username is case insensitive.
-
-        password : str
-            Password in plain text.
-        """
-        self.network_wrapper.set_credentials(username, password)
-
-
-class RESTProperty:
-    """A descriptor that will control the type of value stored."""
-
-    def __init__(self, type, from_json=lambda x: x, to_json=lambda x: x, doc=None):
-        self.__doc__ = doc
-        self.type = type
-        self.from_json = from_json
-        self.to_json = to_json
-
-    def __get__(self, instance, _):
-        if instance:
-            try:
-                return getattr(instance, self.name)
-            except AttributeError:
-                raise AttributeError(f"{self.name} has not been set yet.")
-        else:
-            return self
-
-    def __set__(self, instance, value):
-        if value is not None and not isinstance(value, self.type):
-            value = self.type(value)
-
-        setattr(instance, self.name, value)
-
-    def __delete__(self, instance):
-        delattr(instance, self.name)
-
-
-class _RESTMetaclass(abc.ABCMeta):
-    """The metaclass for RESTObjects.
-
-    This will look into the attributes for the class. If they are a
-    RESTProperty, then it will add it to the __rest__ set and give it its
-    name.
-
-    If the bases have __rest__, then it will add them to the __rest__ set as
-    well.
-    """
-
-    def __init__(self, name, bases, dict):
-        super().__init__(name, bases, dict)
-
-        self.__rest__ = set()
-        for base in bases:
-            self.__rest__.update(getattr(base, "__rest__", set()))
-
-        for k, v in dict.items():
-            if isinstance(v, RESTProperty):
-                v.__dict__["name"] = "_" + k
-                self.__rest__.add(k)
-
-
-class RESTObject(MutableMapping, metaclass=_RESTMetaclass):
-    """A base class that has methods generally useful for interacting with
-    REST objects. The attributes are accessible either as dict keys or as
-    attributes. The object also behaves like a dict, even replicating the
-    repr() functionality.
-
-    Attributes
-    ----------
-
-    __rest__ : set of str
-        A set of all the rest attribute names. This is generated automatically
-        and should include all of the base classes' __rest__ as well as any
-        addition RESTProperty.
-
-    """
-
-    """ __metaclass__ = _RESTMetaclass"""
-
-    def __init__(self, **kwargs):
-        """Creates a new instance of the RESTObject.
-
-        Parameters
-        ----------
-
-        The parameters depend on __rest__. Each item in __rest__ is searched
-        for. If found, it is assigned to the instance. Additional parameters
-        are ignored.
-
-        """
-        logger.info(f"Initializing {self.__class__.__name__} from {kwargs}")
-        for attr in self.__rest__:
-            if attr in kwargs:
-                setattr(self, attr, kwargs.pop(attr))
-
-    def __repr__(self):
-        return (
-            "{" + ", ".join([repr(k) + ": " + repr(v) for k, v in self.items()]) + "}"
-        )
-
-    @classmethod
-    def from_json(cls, data):
-        """Returns a new class object with data populated from json.loads()."""
-        attrs = {}
-        for attr in cls.__rest__:
-            try:
-                value = data[attr]
-            except KeyError:
-                pass
-            else:
-                prop = cls.__dict__[attr]
-                attrs[attr] = prop.from_json(value)
-        return cls(**attrs)
-
-    def to_json(self):
-        """Returns a dict representing this object. This dict will be sent to
-        json.dumps().
-
-        The keys are the items in __rest__ and the values are the current
-        values. If missing, it is not included.
-        """
-        result = {}
-        for attr in self.__rest__:
-            prop = getattr(self.__class__, attr)
-            try:
-                result[attr] = prop.to_json(getattr(self, attr))
-            except AttributeError:
-                pass
-
-        return result
-
-    def __eq__(self, other):
-        return isinstance(self, type(other)) and all(
-            (getattr(self, a) == getattr(other, a) for a in self.__rest__)
-        )
-
-    def __len__(self):
-        return len([a for a in self.__rest__ if hasattr(self, "_" + a)])
-
-    def __iter__(self):
-        return iter([a for a in self.__rest__ if hasattr(self, "_" + a)])
-
-    def __getitem__(self, item):
-        if item not in self.__rest__:
-            raise KeyError(item)
-        try:
-            return getattr(self, item)
-        except AttributeError:
-            raise KeyError(item)
-
-    def __setitem__(self, item, value):
-        if item not in self.__rest__:
-            raise KeyError(item)
-        setattr(self, item, value)
-
-    def __delitem__(self, item):
-        if item not in self.__rest__:
-            raise KeyError(item)
-        try:
-            delattr(self, "_" + item)
-        except AttributeError:
-            raise KeyError(item)
-
-    def __contains__(self, item):
-        return item in self.__rest__
-
-
-def enum(*values, **kwargs):
-    """Generates an enum function that only accepts particular values. Other
-    values will raise a ValueError.
-
-    Parameters
-    ----------
-
-    values : list
-        These are the acceptable values.
-
-    type : type
-        The acceptable types of values. Values will be converted before being
-        checked against the allowed values. If not specified, no conversion
-        will be performed.
-
-    Example
-    -------
-
-    >>> my_enum = enum(1, 2, 3, 4, 5, type=int)
-    >>> a = my_enum(1)
-    >>> b = my_enum(2)
-    >>> c = mu_enum(6) # Raises ValueError
-
-    """
-    if len(values) < 1:
-        raise ValueError("At least one value is required.")
-    enum_type = kwargs.pop("type", str)
-    if kwargs:
-        raise TypeError(f'Unexpected parameters: {", ".join(kwargs.keys())}')
-
-    def __new__(cls, value):
-        if value not in cls.values:
-            raise ValueError(
-                f"{value} is an unexpected value. " f"Expected one of {cls.values}"
-            )
-
-        return super(enum, cls).__new__(cls, value)
-
-    enum = type("Enum", (enum_type,), {"values": values, "__new__": __new__})
-
-    return enum
+import abc
+from collections.abc import MutableMapping
+import logging
+import requests
+from requests.auth import HTTPBasicAuth
+from re import compile
+import json as json
+
+
+logger = logging.getLogger(__name__)
+
+
+class ResponseError(Exception):
+    """Raised when we get an unexpected response."""
+
+    def __init__(self, response):
+        super().__init__("Unexpected server response")
+        self.response = response
+        self.status_code = response.status_code
+
+        try:
+            r = response.json()
+            self.info = r["info"]
+            self.message = response.json()["message"]
+        except (json.JSONDecodeError, KeyError):
+            self.info = None
+            self.message = response.text
+
+    def __str__(self):
+        return f"({self.status_code}) " f"{self.message} " f"{self.info}"
+
+
+class RequestsNetworkWrapper:
+    """The NetworkWrapper wraps the underlying network connection to simplify
+    the interface a bit. This can be replaced with something that can be built
+    on some other type of network connection, such as PyCURL.
+
+    This version requires you to instantiate a requests session object to your
+    liking. It will create a generic session for you if you don't specify it,
+    which you can modify later.
+
+    For authentication, use::
+
+        session.auth = (username, password)
+    """
+
+    def __init__(self, session=None):
+        # Set .auth as appropriate.
+        if session is None:
+            session = requests.session()
+
+        self.session = session
+        self.auth = None
+
+    @staticmethod
+    def raise_error(response):
+        logger.error(
+            f"Error with server response. code={response.status_code}; "
+            f"text={response.text}"
+        )
+
+        raise ResponseError(response)
+
+    @staticmethod
+    def _remove_nones(data):
+        if isinstance(data, dict):
+            for k in [k for k, v in data.items() if v is None]:
+                del data[k]
+
+    def _encode_request(self, data):
+        self._remove_nones(data)
+
+        if data is not None:
+            return json.dumps(data)
+        else:
+            return None
+
+    def GET(self, url, data, timeout=None):
+        """Issues a GET request to the URL with the data specified. Returns an
+        object that is parsed from the response JSON."""
+        self._remove_nones(data)
+
+        logger.info(f"GET {url} with {data}")
+
+        response = self.session.get(url, params=data, timeout=timeout, auth=self.auth)
+        if response.status_code != 200:
+            self.raise_error(response)
+        logger.info(f"response={response.text}")
+
+        if response.text == "":
+            return dict()
+        else:
+            return response.json()
+
+    def POST(self, url, data, timeout=None):
+        """Issues a POST request to the URL with the data specified. Returns an
+        object that is parsed from the response JSON."""
+        data = self._encode_request(data)
+
+        logger.info(f"POST {url} with {data}")
+        response = self.session.post(
+            url,
+            data=data,
+            headers={"content-type": "application/json"},
+            timeout=timeout,
+            auth=self.auth,
+        )
+
+        if response.status_code not in (200, 201):
+            self.raise_error(response)
+
+        return response.json()
+
+    def PUT(self, url, data, timeout=None):
+        """Issues a PUT request to the URL with the data specified. Returns an
+        object that is parsed from the response JSON."""
+        data = self._encode_request(data)
+
+        logger.info(f"PUT {url} with {data}")
+
+        response = self.session.put(
+            url,
+            data=data,
+            headers={"content-type": "application/json"},
+            timeout=timeout,
+            auth=self.auth,
+        )
+        if response.status_code != 200:
+            self.raise_error(response)
+
+        return response.json()
+
+    def DELETE(self, url, data, timeout=None):
+        """
+        Issues a DELETE request to the URL with the data specified. Returns an
+        object that is parsed from the response JSON.
+        """
+        if data is not None:
+            data = json.dumps(data)
+
+        logger.info(f"DELETE {url} with {data}")
+
+        response = self.session.delete(url, data=data, timeout=timeout, auth=self.auth)
+
+        if response.status_code <= 499 and response.status_code >= 400:
+            raise RuntimeError(response.text)
+
+        if response.status_code not in (200, 201, 204):
+            raise RuntimeError(
+                f"Error with server response code: {response.status_code}"
+            )
+
+    def set_credentials(self, username, password):
+        """
+        Set credentials for all the TabPy client-server communication
+        where client is tabpy-tools and server is tabpy-server.
+
+        Parameters
+        ----------
+        username : str
+            User name (login). Username is case insensitive.
+
+        password : str
+            Password in plain text.
+        """
+        logger.info(f"Setting credentials (username: {username})")
+        self.auth = HTTPBasicAuth(username, password)
+
+
+class ServiceClient:
+    """
+    A generic service client.
+
+    This will take an endpoint URL and a network_wrapper. You can use the
+    RequestsNetworkWrapper if you want to use the requests module. The
+    endpoint URL is prepended to all the requests and forwarded to the network
+    wrapper.
+    """
+
+    def __init__(self, endpoint, network_wrapper=None):
+        if network_wrapper is None:
+            network_wrapper = RequestsNetworkWrapper(session=requests.session())
+
+        self.network_wrapper = network_wrapper
+
+        pattern = compile(".*(:[0-9]+)$")
+        if not endpoint.endswith("/") and not pattern.match(endpoint):
+            logger.warning(f"endpoint {endpoint} does not end with '/': appending.")
+            endpoint = endpoint + "/"
+
+        self.endpoint = endpoint
+
+    def GET(self, url, data=None, timeout=None):
+        """Prepends self.endpoint to the url and issues a GET request."""
+        return self.network_wrapper.GET(self.endpoint + url, data, timeout)
+
+    def POST(self, url, data=None, timeout=None):
+        """Prepends self.endpoint to the url and issues a POST request."""
+        return self.network_wrapper.POST(self.endpoint + url, data, timeout)
+
+    def PUT(self, url, data=None, timeout=None):
+        """Prepends self.endpoint to the url and issues a PUT request."""
+        return self.network_wrapper.PUT(self.endpoint + url, data, timeout)
+
+    def DELETE(self, url, data=None, timeout=None):
+        """Prepends self.endpoint to the url and issues a DELETE request."""
+        self.network_wrapper.DELETE(self.endpoint + url, data, timeout)
+
+    def set_credentials(self, username, password):
+        """
+        Set credentials for all the TabPy client-server communication
+        where client is tabpy-tools and server is tabpy-server.
+
+        Parameters
+        ----------
+        username : str
+            User name (login). Username is case insensitive.
+
+        password : str
+            Password in plain text.
+        """
+        self.network_wrapper.set_credentials(username, password)
+
+
+class RESTProperty:
+    """A descriptor that will control the type of value stored."""
+
+    def __init__(self, type, from_json=lambda x: x, to_json=lambda x: x, doc=None):
+        self.__doc__ = doc
+        self.type = type
+        self.from_json = from_json
+        self.to_json = to_json
+
+    def __get__(self, instance, _):
+        if instance:
+            try:
+                return getattr(instance, self.name)
+            except AttributeError:
+                raise AttributeError(f"{self.name} has not been set yet.")
+        else:
+            return self
+
+    def __set__(self, instance, value):
+        if value is not None and not isinstance(value, self.type):
+            value = self.type(value)
+
+        setattr(instance, self.name, value)
+
+    def __delete__(self, instance):
+        delattr(instance, self.name)
+
+
+class _RESTMetaclass(abc.ABCMeta):
+    """The metaclass for RESTObjects.
+
+    This will look into the attributes for the class. If they are a
+    RESTProperty, then it will add it to the __rest__ set and give it its
+    name.
+
+    If the bases have __rest__, then it will add them to the __rest__ set as
+    well.
+    """
+
+    def __init__(self, name, bases, dict):
+        super().__init__(name, bases, dict)
+
+        self.__rest__ = set()
+        for base in bases:
+            self.__rest__.update(getattr(base, "__rest__", set()))
+
+        for k, v in dict.items():
+            if isinstance(v, RESTProperty):
+                v.__dict__["name"] = "_" + k
+                self.__rest__.add(k)
+
+
+class RESTObject(MutableMapping, metaclass=_RESTMetaclass):
+    """A base class that has methods generally useful for interacting with
+    REST objects. The attributes are accessible either as dict keys or as
+    attributes. The object also behaves like a dict, even replicating the
+    repr() functionality.
+
+    Attributes
+    ----------
+
+    __rest__ : set of str
+        A set of all the rest attribute names. This is generated automatically
+        and should include all of the base classes' __rest__ as well as any
+        addition RESTProperty.
+
+    """
+
+    """ __metaclass__ = _RESTMetaclass"""
+
+    def __init__(self, **kwargs):
+        """Creates a new instance of the RESTObject.
+
+        Parameters
+        ----------
+
+        The parameters depend on __rest__. Each item in __rest__ is searched
+        for. If found, it is assigned to the instance. Additional parameters
+        are ignored.
+
+        """
+        logger.info(f"Initializing {self.__class__.__name__} from {kwargs}")
+        for attr in self.__rest__:
+            if attr in kwargs:
+                setattr(self, attr, kwargs.pop(attr))
+
+    def __repr__(self):
+        return (
+            "{" + ", ".join([repr(k) + ": " + repr(v) for k, v in self.items()]) + "}"
+        )
+
+    @classmethod
+    def from_json(cls, data):
+        """Returns a new class object with data populated from json.loads()."""
+        attrs = {}
+        for attr in cls.__rest__:
+            try:
+                value = data[attr]
+            except KeyError:
+                pass
+            else:
+                prop = cls.__dict__[attr]
+                attrs[attr] = prop.from_json(value)
+        return cls(**attrs)
+
+    def to_json(self):
+        """Returns a dict representing this object. This dict will be sent to
+        json.dumps().
+
+        The keys are the items in __rest__ and the values are the current
+        values. If missing, it is not included.
+        """
+        result = {}
+        for attr in self.__rest__:
+            prop = getattr(self.__class__, attr)
+            try:
+                result[attr] = prop.to_json(getattr(self, attr))
+            except AttributeError:
+                pass
+
+        return result
+
+    def __eq__(self, other):
+        return isinstance(self, type(other)) and all(
+            (getattr(self, a) == getattr(other, a) for a in self.__rest__)
+        )
+
+    def __len__(self):
+        return len([a for a in self.__rest__ if hasattr(self, "_" + a)])
+
+    def __iter__(self):
+        return iter([a for a in self.__rest__ if hasattr(self, "_" + a)])
+
+    def __getitem__(self, item):
+        if item not in self.__rest__:
+            raise KeyError(item)
+        try:
+            return getattr(self, item)
+        except AttributeError:
+            raise KeyError(item)
+
+    def __setitem__(self, item, value):
+        if item not in self.__rest__:
+            raise KeyError(item)
+        setattr(self, item, value)
+
+    def __delitem__(self, item):
+        if item not in self.__rest__:
+            raise KeyError(item)
+        try:
+            delattr(self, "_" + item)
+        except AttributeError:
+            raise KeyError(item)
+
+    def __contains__(self, item):
+        return item in self.__rest__
+
+
+def enum(*values, **kwargs):
+    """Generates an enum function that only accepts particular values. Other
+    values will raise a ValueError.
+
+    Parameters
+    ----------
+
+    values : list
+        These are the acceptable values.
+
+    type : type
+        The acceptable types of values. Values will be converted before being
+        checked against the allowed values. If not specified, no conversion
+        will be performed.
+
+    Example
+    -------
+
+    >>> my_enum = enum(1, 2, 3, 4, 5, type=int)
+    >>> a = my_enum(1)
+    >>> b = my_enum(2)
+    >>> c = mu_enum(6) # Raises ValueError
+
+    """
+    if len(values) < 1:
+        raise ValueError("At least one value is required.")
+    enum_type = kwargs.pop("type", str)
+    if kwargs:
+        raise TypeError(f'Unexpected parameters: {", ".join(kwargs.keys())}')
+
+    def __new__(cls, value):
+        if value not in cls.values:
+            raise ValueError(
+                f"{value} is an unexpected value. " f"Expected one of {cls.values}"
+            )
+
+        return super(enum, cls).__new__(cls, value)
+
+    enum = type("Enum", (enum_type,), {"values": values, "__new__": __new__})
+
+    return enum
```

### Comparing `tabpy-2.6.0/tabpy/utils/tabpy_user.py` & `tabpy-2.7.0/tabpy/utils/tabpy_user.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/tabpy.egg-info/PKG-INFO` & `tabpy-2.7.0/tabpy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,262 +1,269 @@
-Metadata-Version: 2.1
-Name: tabpy
-Version: 2.6.0
-Summary: Web server Tableau uses to run Python scripts.
-Home-page: https://github.com/tableau/TabPy
-Download-URL: https://pypi.org/project/tabpy
-Author: Tableau
-Author-email: github@tableau.com
-Maintainer: Tableau
-Maintainer-email: github@tableau.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/tableau/TabPy/issues
-Project-URL: Documentation, https://tableau.github.io/TabPy/
-Project-URL: Source Code, https://github.com/tableau/TabPy
-Keywords: tabpy tableau
-Platform: Windows
-Platform: Linux
-Platform: Mac OS-X
-Platform: Unix
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-TabPy (the Tableau Python Server) is an external service implementation
-which expands Tableau's capabilities by allowing users to execute Python
-scripts and saved functions via Tableau's table calculations.
-
-# Changelog
-
-## v2.6.0
-
-### Improvements
-
-- Fixes deprecation of sklearn in favor of current package name
-scikit-learn
-
-## v2.5.1
-
-### Improvements
-
-- Gzip encoded requests are now supported by default. This can be disabled in
-the config file.
-- The INFO method will return the enabled status of features.
-
-## v2.5.0
-
-### Improvements
-
-- A server with Adhoc Disabled Flag on with the wrong credentials will now
-  return wrong credentials error instead of telling the user
-  that Adhoc Scripts are not allowed on this server.
-- Added documentation for how to run TabPy projects with local changes
-
-### Breaking changes
-
-- Discontinued support for Python 3.6
-- Added support for Python 3.9
-
-## v2.4.0
-
-### Improvements
-
-- Add toggle to turn off evaluate API.
-
-### Breaking changes
-
-- Changing error code to 406 when server not configured for authentication
-  but credentials are provided by client.
-
-## v2.3.2
-
-### Improvements
-
-- Test files added to tar.gz and zip releases.
-
-## v2.3.1
-
-### Bug fixes
-
-- Overriding deployed models.
-
-## v2.3.0
-
-### Improvements
-
-- Fixed scrutinizer test run failure.
-
-## v2.2.0
-
-### Breaking changes
-
-- TabPy fails with 400 when it is not configure for authentication
-  but credentials are provided by client.
-
-### Bug fixes
-
-- When TabPy is running with no console attached it is not failing
-  with 500 when trying to respond with 401 status.
-- tabpy.query() failing when auth is configured.
-
-### Improvements
-
-- Minor code cleanup.
-
-## v1.1.0
-
-### Improvements
-
-- Authorization is now required for the /info API method.
-  This method did not check authentication previously. This change is
-  backwards compatible with Tableau clients.
-- Improved config parsing flexibility. Previously the
-  TABPY_EVALUATE_TIMEOUT setting would be set to a default if
-  tabpy couldn't parse the value. Now it will throw an exception
-  at startup.
-
-## v1.0.0
-
-### Improvements
-
-- Minor: feature name changed to analytics extensions.
-- Startup script files deleted.
-- Index page updated.
-
-### Other
-
-- TabPy is now Tableau Supported (used to be Community Supported).
-
-## v0.9.0
-
-### Improvements
-
-- Models deployment doesn't depend on pip._internal anymore.
-- Package size reduced.
-
-## v0.8.13
-
-### Improvements
-
-- TabPy works with Python 3.8 now.
-- Documentation updates with referencing Tableau Help pages.
-- Added Client.remove() method for deleting deployed models.
-
-### Bug Fixes
-
-- Fixed failing Ctrl+C handler.
-- Fixed query_timeout bug.
-- Fixed None in result collection bug.
-- Fixed script evaluation with missing result/return bug.
-- Fixed startup failure on Windows for Python 3.8.
-
-## v0.8.9
-
-### Improvements
-
-- Added Ctrl+C handler
-- Added configurable buffer size for HTTP requests
-- Added anvoa to supported pre-deployed models in tabpy
-
-## v0.8.7
-
-### Improvements
-
-- Enabled the use of environment variables in the config file.
-
-## v0.8.6
-
-### Fixes
-
-- Fixed file names for package building.
-- Fixed reading version info for /info call.
-
-## v0.8
-
-### Improvements
-
-- TabPy is pip package now
-- Models are deployed with updated script
-
-## v0.7
-
-### Improvements
-
-- Added t-test model
-- Fixed models call with /evaluate for HTTPS
-- Migrated to Tornado 6
-- Timeout is configurable with TABPY_EVALUATE_TIMEOUT config
-  file option
-
-## v0.6.1
-
-### Improvements
-
-- Scripts, documentation, and integration tests for models
-- Small bug fixes 
-- Added request context logging as a feature controlled with
-  TABPY_LOG_DETAILS configuration setting.
-- Updated documentation for /info method and v1 API.
-- Added integration tests.
-
-## v0.4
-
-### Improvements
-
-- Added basic access authentication (all methods except /info)
-- tabpy-tools can deploy models to TabPy with authentication on
-- Increased unit tests coverage
-- Travis CI for merge requests: unit tests executed, code style checking
-
-## v0.3.2
-
-### Breaking changes
-
-- Logger configuration now is in TabPy config file.
-
-### Improvements
-
-- Remove versioneer and just replace it with VERSION file
-- Require Python 3.6.5
-- Require jsonschema to be compatible with 2.3.0
-- Added setup instructions (known issues) for CentOS
-
-## v0.3.1
-
-- Fixed dependency on tabpy-tools in startup scripts
-- Fixed Python version dependency in tabpy-server setup script
-
-## v0.3
-
-### Breaking changes
-
-- The config file is now not just Python code but an actual config
-- Tornado config file has a different setting for CORS
-- Setup scripts are deleted - setup (if needed) happens with the startup script
-- tabpy-client is tabpy-tools now
-
-### Improvements
-
-- Secure connection (HTTPS) is supported with Tableau 2019.2 and newer versions
-- Documentation is improved with more examples added
-- Versioning is done with Versioneer and github release tags
-- Improved logging
-- Unit tests are passing now
-- Configurations for Postman and Swagger are available to use those against running TabPy
-
-## v0.2
-
-- Initial version
+Metadata-Version: 2.1
+Name: tabpy
+Version: 2.7.0
+Summary: Web server Tableau uses to run Python scripts.
+Home-page: https://github.com/tableau/TabPy
+Download-URL: https://pypi.org/project/tabpy
+Author: Tableau
+Author-email: github@tableau.com
+Maintainer: Tableau
+Maintainer-email: github@tableau.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/tableau/TabPy/issues
+Project-URL: Documentation, https://tableau.github.io/TabPy/
+Project-URL: Source Code, https://github.com/tableau/TabPy
+Keywords: tabpy tableau
+Platform: Windows
+Platform: Linux
+Platform: Mac OS-X
+Platform: Unix
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+TabPy (the Tableau Python Server) is an external service implementation
+which expands Tableau's capabilities by allowing users to execute Python
+scripts and saved functions via Tableau's table calculations.
+
+# Changelog
+
+## v2.7.0
+
+### Improvements
+
+- Adds support for data streaming in Arrow columnar format via Apache
+Arrow Flight.
+
+## v2.6.0
+
+### Improvements
+
+- Fixes deprecation of sklearn in favor of current package name
+scikit-learn
+
+## v2.5.1
+
+### Improvements
+
+- Gzip encoded requests are now supported by default. This can be disabled in
+the config file.
+- The INFO method will return the enabled status of features.
+
+## v2.5.0
+
+### Improvements
+
+- A server with Adhoc Disabled Flag on with the wrong credentials will now
+  return wrong credentials error instead of telling the user
+  that Adhoc Scripts are not allowed on this server.
+- Added documentation for how to run TabPy projects with local changes
+
+### Breaking changes
+
+- Discontinued support for Python 3.6
+- Added support for Python 3.9
+
+## v2.4.0
+
+### Improvements
+
+- Add toggle to turn off evaluate API.
+
+### Breaking changes
+
+- Changing error code to 406 when server not configured for authentication
+  but credentials are provided by client.
+
+## v2.3.2
+
+### Improvements
+
+- Test files added to tar.gz and zip releases.
+
+## v2.3.1
+
+### Bug fixes
+
+- Overriding deployed models.
+
+## v2.3.0
+
+### Improvements
+
+- Fixed scrutinizer test run failure.
+
+## v2.2.0
+
+### Breaking changes
+
+- TabPy fails with 400 when it is not configure for authentication
+  but credentials are provided by client.
+
+### Bug fixes
+
+- When TabPy is running with no console attached it is not failing
+  with 500 when trying to respond with 401 status.
+- tabpy.query() failing when auth is configured.
+
+### Improvements
+
+- Minor code cleanup.
+
+## v1.1.0
+
+### Improvements
+
+- Authorization is now required for the /info API method.
+  This method did not check authentication previously. This change is
+  backwards compatible with Tableau clients.
+- Improved config parsing flexibility. Previously the
+  TABPY_EVALUATE_TIMEOUT setting would be set to a default if
+  tabpy couldn't parse the value. Now it will throw an exception
+  at startup.
+
+## v1.0.0
+
+### Improvements
+
+- Minor: feature name changed to analytics extensions.
+- Startup script files deleted.
+- Index page updated.
+
+### Other
+
+- TabPy is now Tableau Supported (used to be Community Supported).
+
+## v0.9.0
+
+### Improvements
+
+- Models deployment doesn't depend on pip._internal anymore.
+- Package size reduced.
+
+## v0.8.13
+
+### Improvements
+
+- TabPy works with Python 3.8 now.
+- Documentation updates with referencing Tableau Help pages.
+- Added Client.remove() method for deleting deployed models.
+
+### Bug Fixes
+
+- Fixed failing Ctrl+C handler.
+- Fixed query_timeout bug.
+- Fixed None in result collection bug.
+- Fixed script evaluation with missing result/return bug.
+- Fixed startup failure on Windows for Python 3.8.
+
+## v0.8.9
+
+### Improvements
+
+- Added Ctrl+C handler
+- Added configurable buffer size for HTTP requests
+- Added anvoa to supported pre-deployed models in tabpy
+
+## v0.8.7
+
+### Improvements
+
+- Enabled the use of environment variables in the config file.
+
+## v0.8.6
+
+### Fixes
+
+- Fixed file names for package building.
+- Fixed reading version info for /info call.
+
+## v0.8
+
+### Improvements
+
+- TabPy is pip package now
+- Models are deployed with updated script
+
+## v0.7
+
+### Improvements
+
+- Added t-test model
+- Fixed models call with /evaluate for HTTPS
+- Migrated to Tornado 6
+- Timeout is configurable with TABPY_EVALUATE_TIMEOUT config
+  file option
+
+## v0.6.1
+
+### Improvements
+
+- Scripts, documentation, and integration tests for models
+- Small bug fixes 
+- Added request context logging as a feature controlled with
+  TABPY_LOG_DETAILS configuration setting.
+- Updated documentation for /info method and v1 API.
+- Added integration tests.
+
+## v0.4
+
+### Improvements
+
+- Added basic access authentication (all methods except /info)
+- tabpy-tools can deploy models to TabPy with authentication on
+- Increased unit tests coverage
+- Travis CI for merge requests: unit tests executed, code style checking
+
+## v0.3.2
+
+### Breaking changes
+
+- Logger configuration now is in TabPy config file.
+
+### Improvements
+
+- Remove versioneer and just replace it with VERSION file
+- Require Python 3.6.5
+- Require jsonschema to be compatible with 2.3.0
+- Added setup instructions (known issues) for CentOS
+
+## v0.3.1
+
+- Fixed dependency on tabpy-tools in startup scripts
+- Fixed Python version dependency in tabpy-server setup script
+
+## v0.3
+
+### Breaking changes
+
+- The config file is now not just Python code but an actual config
+- Tornado config file has a different setting for CORS
+- Setup scripts are deleted - setup (if needed) happens with the startup script
+- tabpy-client is tabpy-tools now
+
+### Improvements
+
+- Secure connection (HTTPS) is supported with Tableau 2019.2 and newer versions
+- Documentation is improved with more examples added
+- Versioning is done with Versioneer and github release tags
+- Improved logging
+- Unit tests are passing now
+- Configurations for Postman and Swagger are available to use those against running TabPy
+
+## v0.2
+
+- Initial version
```

### Comparing `tabpy-2.6.0/tabpy.egg-info/SOURCES.txt` & `tabpy-2.7.0/tabpy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -40,26 +40,29 @@
 tabpy/models/utils/__init__.py
 tabpy/models/utils/setup_utils.py
 tabpy/tabpy_server/__init__.py
 tabpy/tabpy_server/state.ini.template
 tabpy/tabpy_server/app/__init__.py
 tabpy/tabpy_server/app/app.py
 tabpy/tabpy_server/app/app_parameters.py
+tabpy/tabpy_server/app/arrow_server.py
 tabpy/tabpy_server/app/util.py
 tabpy/tabpy_server/common/__init__.py
 tabpy/tabpy_server/common/default.conf
 tabpy/tabpy_server/common/endpoint_file_mgr.py
 tabpy/tabpy_server/common/messages.py
 tabpy/tabpy_server/common/util.py
 tabpy/tabpy_server/handlers/__init__.py
 tabpy/tabpy_server/handlers/base_handler.py
+tabpy/tabpy_server/handlers/basic_auth_server_middleware_factory.py
 tabpy/tabpy_server/handlers/endpoint_handler.py
 tabpy/tabpy_server/handlers/endpoints_handler.py
 tabpy/tabpy_server/handlers/evaluation_plane_handler.py
 tabpy/tabpy_server/handlers/management_handler.py
+tabpy/tabpy_server/handlers/no_op_auth_handler.py
 tabpy/tabpy_server/handlers/query_plane_handler.py
 tabpy/tabpy_server/handlers/service_info_handler.py
 tabpy/tabpy_server/handlers/status_handler.py
 tabpy/tabpy_server/handlers/upload_destination_handler.py
 tabpy/tabpy_server/handlers/util.py
 tabpy/tabpy_server/management/__init__.py
 tabpy/tabpy_server/management/state.py
@@ -78,14 +81,15 @@
 tabpy/tabpy_tools/rest_client.py
 tabpy/tabpy_tools/schema.py
 tabpy/utils/__init__.py
 tabpy/utils/tabpy_user.py
 tests/__init__.py
 tests/integration/__init__.py
 tests/integration/integ_test_base.py
+tests/integration/test_arrow_server.py
 tests/integration/test_auth.py
 tests/integration/test_custom_evaluate_timeout.py
 tests/integration/test_deploy_and_evaluate_model.py
 tests/integration/test_deploy_and_evaluate_model_auth_on.py
 tests/integration/test_deploy_and_evaluate_model_ssl.py
 tests/integration/test_deploy_model_ssl_off_auth_off.py
 tests/integration/test_deploy_model_ssl_off_auth_on.py
```

### Comparing `tabpy-2.6.0/tests/integration/integ_test_base.py` & `tabpy-2.7.0/tests/integration/integ_test_base.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/tests/integration/resources/2019_04_24_to_3018_08_25.crt` & `tabpy-2.7.0/tests/integration/resources/2019_04_24_to_3018_08_25.crt`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,88 @@
 00000000: 2d2d 2d2d 2d42 4547 494e 2043 4552 5449  -----BEGIN CERTI
-00000010: 4649 4341 5445 2d2d 2d2d 2d0a 4d49 4944  FICATE-----.MIID
-00000020: 796a 4343 4172 4943 4351 4433 2b54 6b35  yjCCArICCQD3+Tk5
-00000030: 3352 6275 7a54 414e 4267 6b71 686b 6947  3RbuzTANBgkqhkiG
-00000040: 3977 3042 4151 7346 4144 4342 7054 454c  9w0BAQsFADCBpTEL
-00000050: 4d41 6b47 4131 5545 4268 4d43 0a56 564d  MAkGA1UEBhMC.VVM
-00000060: 7843 7a41 4a42 674e 5642 4167 4d41 6c64  xCzAJBgNVBAgMAld
-00000070: 424d 5245 7744 7759 4456 5151 4844 4168  BMREwDwYDVQQHDAh
-00000080: 4c61 584a 7262 4746 755a 4445 5a4d 4263  LaXJrbGFuZDEZMBc
-00000090: 4741 3155 4543 6777 5156 4746 690a 6247  GA1UECgwQVGFi.bG
-000000a0: 5668 6453 4254 6232 5a30 6432 4679 5a54  VhdSBTb2Z0d2FyZT
-000000b0: 4562 4d42 6b47 4131 5545 4377 7753 5157  EbMBkGA1UECwwSQW
-000000c0: 5232 5957 356a 5a57 5167 5157 3568 6248  R2YW5jZWQgQW5hbH
-000000d0: 6c30 6157 4e7a 4d52 6377 4651 5944 0a56  l0aWNzMRcwFQYD.V
-000000e0: 5151 4444 4135 5062 4756 7249 4564 7662  QQDDA5PbGVrIEdvb
-000000f0: 4739 3259 5852 3561 5445 6c4d 434d 4743  G92YXR5aTElMCMGC
-00000100: 5371 4753 4962 3344 5145 4a41 5259 5762  SqGSIb3DQEJARYWb
-00000110: 3264 7662 4739 3259 5852 3561 5542 300a  2dvbG92YXR5aUB0.
-00000120: 5957 4a73 5a57 4631 4c6d 4e76 6254 4167  YWJsZWF1LmNvbTAg
-00000130: 4677 3078 4f54 4130 4d6a 5179 4d54 5531  Fw0xOTA0MjQyMTU1
-00000140: 4e44 5661 4741 387a 4d44 4534 4d44 6779  NDVaGA8zMDE4MDgy
-00000150: 4e54 4978 4e54 5530 4e56 6f77 6761 5578  NTIxNTU0NVowgaUx
-00000160: 0a43 7a41 4a42 674e 5642 4159 5441 6c56  .CzAJBgNVBAYTAlV
-00000170: 544d 5173 7743 5159 4456 5151 4944 414a  TMQswCQYDVQQIDAJ
-00000180: 5851 5445 524d 4138 4741 3155 4542 7777  XQTERMA8GA1UEBww
-00000190: 4953 326c 7961 3278 6862 6d51 7847 5441  IS2lya2xhbmQxGTA
-000001a0: 580a 4267 4e56 4241 6f4d 4546 5268 596d  X.BgNVBAoMEFRhYm
-000001b0: 786c 5958 5567 5532 396d 6448 6468 636d  xlYXUgU29mdHdhcm
-000001c0: 5578 477a 415a 4267 4e56 4241 734d 456b  UxGzAZBgNVBAsMEk
-000001d0: 466b 646d 4675 5932 566b 4945 4675 5957  FkdmFuY2VkIEFuYW
-000001e0: 7835 0a64 476c 6a63 7a45 584d 4255 4741  x5.dGljczEXMBUGA
-000001f0: 3155 4541 7777 4f54 3278 6c61 7942 4862  1UEAwwOT2xlayBHb
-00000200: 3278 7664 6d46 3065 576b 784a 5441 6a42  2xvdmF0eWkxJTAjB
-00000210: 676b 7168 6b69 4739 7730 4243 5145 5746  gkqhkiG9w0BCQEWF
-00000220: 6d39 6e0a 6232 7876 646d 4630 6557 6c41  m9n.b2xvdmF0eWlA
-00000230: 6447 4669 6247 5668 6453 356a 6232 3077  dGFibGVhdS5jb20w
-00000240: 6767 4569 4d41 3047 4353 7147 5349 6233  ggEiMA0GCSqGSIb3
-00000250: 4451 4542 4151 5541 4134 4942 4477 4177  DQEBAQUAA4IBDwAw
-00000260: 6767 454b 0a41 6f49 4241 5143 6e6f 4f67  ggEK.AoIBAQCnoOg
-00000270: 4330 7733 6d53 5332 756f 5251 4f63 4b74  C0w3mSS2uoRQOcKt
-00000280: 6b43 3375 6548 786f 3868 4458 7364 6e42  kC3ueHxo8hDXsdnB
-00000290: 6143 6463 766f 3869 7871 7659 694b 502f  aCdcvo8ixqvYiKP/
-000002a0: 7477 5a43 620a 737a 2b35 5947 4647 6b43  twZCb.sz+5YGFGkC
-000002b0: 7747 5772 6458 3955 3949 792f 3730 7231  wGWrdX9U9Iy/70r1
-000002c0: 664c 796f 5a38 396f 7377 6a66 3465 6933  fLyoZ89oswjf4ei3
-000002d0: 4663 7a46 666a 5442 316c 3470 676e 4442  FczFfjTB1l4pgnDB
-000002e0: 594b 5767 516d 0a49 646b 5a33 6e32 3659  YKWgQm.IdkZ3n26Y
-000002f0: 6d4e 576d 2f34 6533 636d 3631 4b59 5938  mNWm/4e3cm61KYY8
-00000300: 664a 4e30 7639 516c 354e 4278 482b 7852  fJN0v9Ql5NBxH+xR
-00000310: 7276 7771 676b 4652 5a4a 6349 7541 4561  rvwqgkFRZJcIuAEa
-00000320: 376b 3238 4644 2f0a 4b61 4d4c 4f67 444d  7k28FD/.KaMLOgDM
-00000330: 7874 7546 5863 6f51 5377 5437 3567 676d  xtuFXcoQSwT75ggm
-00000340: 684d 3839 6165 4534 6b4b 662b 4d62 4737  hM89aeE4kKf+MbG7
-00000350: 646b 776f 5633 7931 685a 472f 6757 3642  dkwoV3y1hZG/gW6B
-00000360: 7279 4c66 6f32 7841 0a59 6c61 5177 747a  ryLfo2xA.YlaQwtz
-00000370: 5042 5068 6745 3867 7371 7874 4f37 6c2b  PBPhgE8gsqxtO7l+
-00000380: 7778 7630 334a 4f6e 6b50 514e 4257 4841  wxv03JOnkPQNBWHA
-00000390: 6637 4d74 6c6b 7164 4d36 6730 3355 7257  f7MtlkqdM6g03UrW
-000003a0: 6d66 5446 6871 7a50 450a 727a 7369 574f  mfTFhqzPE.rzsiWO
-000003b0: 5844 7844 3263 3548 5369 7373 3234 4848  XDxD2c5HSiss24HH
-000003c0: 7267 4633 3772 4167 4d42 4141 4577 4451  rgF37rAgMBAAEwDQ
-000003d0: 594a 4b6f 5a49 6876 634e 4151 454c 4251  YJKoZIhvcNAQELBQ
-000003e0: 4144 6767 4542 4149 5162 0a54 7750 6372  ADggEBAIQb.TwPcr
-000003f0: 4465 5955 7749 7a38 5457 4545 6349 5833  DeYUwIz8TWEEcIX3
-00000400: 6a4a 6f44 4d79 5236 512b 4145 6d4d 3843  jJoDMyR6Q+AEmM8C
-00000410: 3865 6430 4a6c 6176 4532 7150 695a 632b  8ed0JlavE2qPiZc+
-00000420: 6c4c 7238 4463 3142 2b66 450a 3755 6b78  lLr8Dc1B+fE.7Ukx
-00000430: 4850 5a4f 7730 6643 7472 5133 4933 2b30  HPZOw0fCtrQ3I3+0
-00000440: 5a2f 3659 6671 5a73 336d 3166 3149 3859  Z/6YfqZs3m1f1I8Y
-00000450: 7236 5353 5736 4e6a 416a 372b 6d6d 4d51  r6SSW6NjAj7+mmMQ
-00000460: 3844 754a 4762 3579 7565 6650 0a5a 304c  8DuJGb5yuefP.Z0L
-00000470: 5638 462b 4f77 5558 4e49 3762 736c 3051  V8F+OwUXNI7bsl0Q
-00000480: 3455 4b74 3851 5130 6f76 4933 4936 7738  4UKt8QQ0ovI3I6w8
-00000490: 4856 7375 7937 7a79 4555 4e32 3638 7469  HVsuy7zyEUN268ti
-000004a0: 4b35 3862 4d6b 5366 627a 5661 6c0a 5576  K58bMkSfbzVal.Uv
-000004b0: 4963 5871 5a79 4246 4b51 2f5a 5a33 426b  IcXqZyBFKQ/ZZ3Bk
-000004c0: 6e49 3862 3369 6279 6137 6837 522f 3932  nI8b3ibya7h7R/92
-000004d0: 4373 4d44 6650 4151 4153 5a63 4277 4b4a  CsMDfPAQASZcBwKJ
-000004e0: 3634 5257 3957 6935 477a 7a71 6d70 0a44  64RW9Wi5Gzzqmp.D
-000004f0: 3256 6b36 4d64 794f 6770 3462 4439 7744  2Vk6MdyOgp4bD9wD
-00000500: 716d 3466 3670 3230 4665 7761 6753 4c35  qm4f6p20FewagSL5
-00000510: 2f63 336c 6b31 456a 6f43 7965 3655 4148  /c3lk1EjoCye6UAH
-00000520: 3263 6e71 5052 546f 7749 3265 6c4a 670a  2cnqPRTowI2elJg.
-00000530: 5739 6d72 5948 326b 394c 3263 6e6e 5549  W9mrYH2k9L2cnnUI
-00000540: 7978 343d 0a2d 2d2d 2d2d 454e 4420 4345  yx4=.-----END CE
-00000550: 5254 4946 4943 4154 452d 2d2d 2d2d 0a    RTIFICATE-----.
+00000010: 4649 4341 5445 2d2d 2d2d 2d0d 0a4d 4949  FICATE-----..MII
+00000020: 4479 6a43 4341 7249 4343 5144 332b 546b  DyjCCArICCQD3+Tk
+00000030: 3533 5262 757a 5441 4e42 676b 7168 6b69  53RbuzTANBgkqhki
+00000040: 4739 7730 4241 5173 4641 4443 4270 5445  G9w0BAQsFADCBpTE
+00000050: 4c4d 416b 4741 3155 4542 684d 430d 0a56  LMAkGA1UEBhMC..V
+00000060: 564d 7843 7a41 4a42 674e 5642 4167 4d41  VMxCzAJBgNVBAgMA
+00000070: 6c64 424d 5245 7744 7759 4456 5151 4844  ldBMREwDwYDVQQHD
+00000080: 4168 4c61 584a 7262 4746 755a 4445 5a4d  AhLaXJrbGFuZDEZM
+00000090: 4263 4741 3155 4543 6777 5156 4746 690d  BcGA1UECgwQVGFi.
+000000a0: 0a62 4756 6864 5342 5462 325a 3064 3246  .bGVhdSBTb2Z0d2F
+000000b0: 795a 5445 624d 426b 4741 3155 4543 7777  yZTEbMBkGA1UECww
+000000c0: 5351 5752 3259 5735 6a5a 5751 6751 5735  SQWR2YW5jZWQgQW5
+000000d0: 6862 486c 3061 574e 7a4d 5263 7746 5159  hbHl0aWNzMRcwFQY
+000000e0: 440d 0a56 5151 4444 4135 5062 4756 7249  D..VQQDDA5PbGVrI
+000000f0: 4564 7662 4739 3259 5852 3561 5445 6c4d  EdvbG92YXR5aTElM
+00000100: 434d 4743 5371 4753 4962 3344 5145 4a41  CMGCSqGSIb3DQEJA
+00000110: 5259 5762 3264 7662 4739 3259 5852 3561  RYWb2dvbG92YXR5a
+00000120: 5542 300d 0a59 574a 735a 5746 314c 6d4e  UB0..YWJsZWF1LmN
+00000130: 7662 5441 6746 7730 784f 5441 304d 6a51  vbTAgFw0xOTA0MjQ
+00000140: 794d 5455 314e 4456 6147 4138 7a4d 4445  yMTU1NDVaGA8zMDE
+00000150: 344d 4467 794e 5449 784e 5455 304e 566f  4MDgyNTIxNTU0NVo
+00000160: 7767 6155 780d 0a43 7a41 4a42 674e 5642  wgaUx..CzAJBgNVB
+00000170: 4159 5441 6c56 544d 5173 7743 5159 4456  AYTAlVTMQswCQYDV
+00000180: 5151 4944 414a 5851 5445 524d 4138 4741  QQIDAJXQTERMA8GA
+00000190: 3155 4542 7777 4953 326c 7961 3278 6862  1UEBwwIS2lya2xhb
+000001a0: 6d51 7847 5441 580d 0a42 674e 5642 416f  mQxGTAX..BgNVBAo
+000001b0: 4d45 4652 6859 6d78 6c59 5855 6755 3239  MEFRhYmxlYXUgU29
+000001c0: 6d64 4864 6863 6d55 7847 7a41 5a42 674e  mdHdhcmUxGzAZBgN
+000001d0: 5642 4173 4d45 6b46 6b64 6d46 7559 3256  VBAsMEkFkdmFuY2V
+000001e0: 6b49 4546 7559 5778 350d 0a64 476c 6a63  kIEFuYWx5..dGljc
+000001f0: 7a45 584d 4255 4741 3155 4541 7777 4f54  zEXMBUGA1UEAwwOT
+00000200: 3278 6c61 7942 4862 3278 7664 6d46 3065  2xlayBHb2xvdmF0e
+00000210: 576b 784a 5441 6a42 676b 7168 6b69 4739  WkxJTAjBgkqhkiG9
+00000220: 7730 4243 5145 5746 6d39 6e0d 0a62 3278  w0BCQEWFm9n..b2x
+00000230: 7664 6d46 3065 576c 4164 4746 6962 4756  vdmF0eWlAdGFibGV
+00000240: 6864 5335 6a62 3230 7767 6745 694d 4130  hdS5jb20wggEiMA0
+00000250: 4743 5371 4753 4962 3344 5145 4241 5155  GCSqGSIb3DQEBAQU
+00000260: 4141 3449 4244 7741 7767 6745 4b0d 0a41  AA4IBDwAwggEK..A
+00000270: 6f49 4241 5143 6e6f 4f67 4330 7733 6d53  oIBAQCnoOgC0w3mS
+00000280: 5332 756f 5251 4f63 4b74 6b43 3375 6548  S2uoRQOcKtkC3ueH
+00000290: 786f 3868 4458 7364 6e42 6143 6463 766f  xo8hDXsdnBaCdcvo
+000002a0: 3869 7871 7659 694b 502f 7477 5a43 620d  8ixqvYiKP/twZCb.
+000002b0: 0a73 7a2b 3559 4746 476b 4377 4757 7264  .sz+5YGFGkCwGWrd
+000002c0: 5839 5539 4979 2f37 3072 3166 4c79 6f5a  X9U9Iy/70r1fLyoZ
+000002d0: 3839 6f73 776a 6634 6569 3346 637a 4666  89oswjf4ei3FczFf
+000002e0: 6a54 4231 6c34 7067 6e44 4259 4b57 6751  jTB1l4pgnDBYKWgQ
+000002f0: 6d0d 0a49 646b 5a33 6e32 3659 6d4e 576d  m..IdkZ3n26YmNWm
+00000300: 2f34 6533 636d 3631 4b59 5938 664a 4e30  /4e3cm61KYY8fJN0
+00000310: 7639 516c 354e 4278 482b 7852 7276 7771  v9Ql5NBxH+xRrvwq
+00000320: 676b 4652 5a4a 6349 7541 4561 376b 3238  gkFRZJcIuAEa7k28
+00000330: 4644 2f0d 0a4b 614d 4c4f 6744 4d78 7475  FD/..KaMLOgDMxtu
+00000340: 4658 636f 5153 7754 3735 6767 6d68 4d38  FXcoQSwT75ggmhM8
+00000350: 3961 6545 346b 4b66 2b4d 6247 3764 6b77  9aeE4kKf+MbG7dkw
+00000360: 6f56 3379 3168 5a47 2f67 5736 4272 794c  oV3y1hZG/gW6BryL
+00000370: 666f 3278 410d 0a59 6c61 5177 747a 5042  fo2xA..YlaQwtzPB
+00000380: 5068 6745 3867 7371 7874 4f37 6c2b 7778  PhgE8gsqxtO7l+wx
+00000390: 7630 334a 4f6e 6b50 514e 4257 4841 6637  v03JOnkPQNBWHAf7
+000003a0: 4d74 6c6b 7164 4d36 6730 3355 7257 6d66  MtlkqdM6g03UrWmf
+000003b0: 5446 6871 7a50 450d 0a72 7a73 6957 4f58  TFhqzPE..rzsiWOX
+000003c0: 4478 4432 6335 4853 6973 7332 3448 4872  DxD2c5HSiss24HHr
+000003d0: 6746 3337 7241 674d 4241 4145 7744 5159  gF37rAgMBAAEwDQY
+000003e0: 4a4b 6f5a 4968 7663 4e41 5145 4c42 5141  JKoZIhvcNAQELBQA
+000003f0: 4467 6745 4241 4951 620d 0a54 7750 6372  DggEBAIQb..TwPcr
+00000400: 4465 5955 7749 7a38 5457 4545 6349 5833  DeYUwIz8TWEEcIX3
+00000410: 6a4a 6f44 4d79 5236 512b 4145 6d4d 3843  jJoDMyR6Q+AEmM8C
+00000420: 3865 6430 4a6c 6176 4532 7150 695a 632b  8ed0JlavE2qPiZc+
+00000430: 6c4c 7238 4463 3142 2b66 450d 0a37 556b  lLr8Dc1B+fE..7Uk
+00000440: 7848 505a 4f77 3066 4374 7251 3349 332b  xHPZOw0fCtrQ3I3+
+00000450: 305a 2f36 5966 715a 7333 6d31 6631 4938  0Z/6YfqZs3m1f1I8
+00000460: 5972 3653 5357 364e 6a41 6a37 2b6d 6d4d  Yr6SSW6NjAj7+mmM
+00000470: 5138 4475 4a47 6235 7975 6566 500d 0a5a  Q8DuJGb5yuefP..Z
+00000480: 304c 5638 462b 4f77 5558 4e49 3762 736c  0LV8F+OwUXNI7bsl
+00000490: 3051 3455 4b74 3851 5130 6f76 4933 4936  0Q4UKt8QQ0ovI3I6
+000004a0: 7738 4856 7375 7937 7a79 4555 4e32 3638  w8HVsuy7zyEUN268
+000004b0: 7469 4b35 3862 4d6b 5366 627a 5661 6c0d  tiK58bMkSfbzVal.
+000004c0: 0a55 7649 6358 715a 7942 464b 512f 5a5a  .UvIcXqZyBFKQ/ZZ
+000004d0: 3342 6b6e 4938 6233 6962 7961 3768 3752  3BknI8b3ibya7h7R
+000004e0: 2f39 3243 734d 4466 5041 5141 535a 6342  /92CsMDfPAQASZcB
+000004f0: 774b 4a36 3452 5739 5769 3547 7a7a 716d  wKJ64RW9Wi5Gzzqm
+00000500: 700d 0a44 3256 6b36 4d64 794f 6770 3462  p..D2Vk6MdyOgp4b
+00000510: 4439 7744 716d 3466 3670 3230 4665 7761  D9wDqm4f6p20Fewa
+00000520: 6753 4c35 2f63 336c 6b31 456a 6f43 7965  gSL5/c3lk1EjoCye
+00000530: 3655 4148 3263 6e71 5052 546f 7749 3265  6UAH2cnqPRTowI2e
+00000540: 6c4a 670d 0a57 396d 7259 4832 6b39 4c32  lJg..W9mrYH2k9L2
+00000550: 636e 6e55 4979 7834 3d0d 0a2d 2d2d 2d2d  cnnUIyx4=..-----
+00000560: 454e 4420 4345 5254 4946 4943 4154 452d  END CERTIFICATE-
+00000570: 2d2d 2d2d 0d0a                           ----..
```

### Comparing `tabpy-2.6.0/tests/integration/resources/2019_04_24_to_3018_08_25.key` & `tabpy-2.7.0/tests/integration/resources/2019_04_24_to_3018_08_25.key`

 * *Files 13% similar despite different names*

```diff
@@ -1,105 +1,107 @@
 00000000: 2d2d 2d2d 2d42 4547 494e 2052 5341 2050  -----BEGIN RSA P
-00000010: 5249 5641 5445 204b 4559 2d2d 2d2d 2d0a  RIVATE KEY-----.
-00000020: 4d49 4945 7041 4942 4141 4b43 4151 4541  MIIEpAIBAAKCAQEA
-00000030: 7036 446f 4174 4d4e 356b 6b74 7271 4555  p6DoAtMN5kktrqEU
-00000040: 446e 4372 5a41 7437 6e68 3861 5049 5131  DnCrZAt7nh8aPIQ1
-00000050: 3748 5a77 5767 6e58 4c36 5049 7361 7232  7HZwWgnXL6PIsar2
-00000060: 0a49 696a 2f37 6347 516d 374d 2f75 5742  .Iij/7cGQm7M/uWB
-00000070: 6852 7041 7342 6c71 3356 2f56 5053 4d76  hRpAsBlq3V/VPSMv
-00000080: 2b39 4b39 5879 3871 4766 5061 4c4d 4933  +9K9Xy8qGfPaLMI3
-00000090: 2b48 6f74 7858 4d78 5834 3077 645a 654b  +HotxXMxX40wdZeK
-000000a0: 590a 4a77 7757 436c 6f45 4a69 485a 4764  Y.JwwWCloEJiHZGd
-000000b0: 3539 756d 4a6a 5670 762b 4874 334a 7574  59umJjVpv+Ht3Jut
-000000c0: 536d 4750 4879 5464 4c2f 554a 6554 5163  SmGPHyTdL/UJeTQc
-000000d0: 522f 7355 6137 384b 6f4a 4255 5753 5843  R/sUa78KoJBUWSXC
-000000e0: 4c67 0a42 4775 354e 7642 512f 796d 6a43  Lg.BGu5NvBQ/ymjC
-000000f0: 7a6f 417a 4d62 6268 5633 4b45 4573 452b  zoAzMbbhV3KEEsE+
-00000100: 2b59 494a 6f54 5050 576e 684f 4a43 6e2f  +YIJoTPPWnhOJCn/
-00000110: 6a47 7875 335a 4d4b 4664 3874 5957 5276  jGxu3ZMKFd8tYWRv
-00000120: 3446 750a 6761 3869 3336 4e73 5147 4a57  4Fu.ga8i36NsQGJW
-00000130: 6b4d 4c63 7a77 5434 5942 5049 4c4b 7362  kMLczwT4YBPILKsb
-00000140: 5475 3566 734d 6239 4e79 5470 3544 3044  Tu5fsMb9NyTp5D0D
-00000150: 5156 6877 482b 7a4c 5a5a 4b6e 544f 6f4e  QVhwH+zLZZKnTOoN
-00000160: 4e31 4b31 0a70 6e30 7859 6173 7a78 4b38  N1K1.pn0xYaszxK8
-00000170: 3749 6c6a 6c77 3851 396e 4f52 306f 724c  7Iljlw8Q9nOR0orL
-00000180: 4e75 4278 3634 4264 2b36 7749 4441 5141  NuBx64Bd+6wIDAQA
-00000190: 4241 6f49 4241 4373 5652 4178 5679 6d44  BAoIBACsVRAxVymD
-000001a0: 4274 6967 480a 356d 752f 7359 314a 466b  BtigH.5mu/sY1JFk
-000001b0: 4352 7065 4366 366d 7759 464e 4250 6279  CRpeCf6mwYFNBPby
-000001c0: 736a 5956 576f 7078 496f 6a33 3741 4854  sjYVWopxIoj37AHT
-000001d0: 616e 5831 3135 3141 6161 7a33 5869 6f76  anX1151Aaaz3Xiov
-000001e0: 544d 6139 4139 0a2f 6731 4e63 3764 4247  TMa9A9./g1Nc7dBG
-000001f0: 6b66 4c35 674a 5976 464f 4661 3246 3663  kfL5gJYvFOFa2F6c
-00000200: 3678 4c78 394b 4435 7139 4366 2f65 7849  6xLx9KD5q9Cf/exI
-00000210: 7866 5a34 7a36 7533 496d 6d39 2f6b 7570  xfZ4z6u3Imm9/kup
-00000220: 7157 7751 3054 740a 6d72 4d57 6e44 7738  qWwQ0Tt.mrMWnDw8
-00000230: 5772 7150 2b70 3051 722f 4555 5351 4756  WrqP+p0Qr/EUSQGV
-00000240: 386a 4f55 5033 5379 4133 7a51 6245 6273  8jOUP3SyA3zQbEbs
-00000250: 426b 6574 747a 344e 696c 394e 4954 7762  Bkettz4Nil9NITwb
-00000260: 5172 626e 4736 6f37 0a52 6e4e 7578 4377  QrbnG6o7.RnNuxCw
-00000270: 5277 4f33 5142 3170 3059 4f58 6e4b 7974  RwO3QB1p0YOXnKyt
-00000280: 5538 7849 7537 3858 6733 7177 5678 3831  U8xIu78Xg3qwVx81
-00000290: 5150 332f 6f6d 4239 6a4e 4359 3532 7031  QP3/omB9jNCY52p1
-000002a0: 4652 4c7a 474f 3231 710a 4a46 5a4c 4963  FRLzGO21q.JFZLIc
-000002b0: 5037 6845 4365 736e 3576 3964 5a61 3939  P7hECesn5v9dZa99
-000002c0: 6f43 6855 2b52 647a 6939 3356 4579 6d77  oChU+Rdzi93VEymw
-000002d0: 6d5a 4256 6c38 6769 764e 6457 4165 3159  mZBVl8givNdWAe1Y
-000002e0: 3763 2f5a 3866 4957 532f 0a46 5156 7652  7c/Z8fIWS/.FQVvR
-000002f0: 6745 4367 5945 4131 3275 5a52 6c4c 446e  gECgYEA12uZRlLDn
-00000300: 446f 7159 546a 354f 7473 3837 4b70 7931  DoqYTj5Ots87Kpy1
-00000310: 3577 5535 6c41 3241 5347 4e67 6151 4c58  5wU5lA2ASGNgaQLX
-00000320: 5a42 6768 3849 442f 386f 350a 5152 6b31  ZBgh8ID/8o5.QRk1
-00000330: 2f43 4e57 3269 2f63 572f 6649 3758 5261  /CNW2i/cW/fI7XRa
-00000340: 6946 6f48 6a72 7644 3658 6754 306d 2f62  iFoHjrvD6XgT0m/b
-00000350: 574f 657a 4657 586f 656d 6b4d 522f 6a52  WOezFWXoemkMR/jR
-00000360: 326b 595a 6a53 3076 7063 3034 0a77 642f  2kYZjS0vpc04.wd/
-00000370: 7276 7248 7234 6e62 5351 4531 6356 4277  rvrHr4nbSQE1cVBw
-00000380: 4c72 597a 7259 4a36 7172 4779 6278 3950  LrYzrYJ6qrGybx9P
-00000390: 366b 3066 6875 3266 5549 4a49 4a47 454f  6k0fhu2fUIJIJGEO
-000003a0: 5451 3045 4367 5945 4178 7a53 610a 6634  TQ0ECgYEAxzSa.f4
-000003b0: 4b4c 4753 725a 6a66 5a6c 3639 357a 2b38  KLGSrZjfZl695z+8
-000003c0: 3356 5547 3561 6567 3856 3430 376e 4136  3VUG5aeg8V407nA6
-000003d0: 5242 7733 5865 4b39 426a 4868 7166 7352  RBw3XeK9BjHhqfsR
-000003e0: 6e46 4166 7668 7479 546f 6c6d 334d 0a51  nFAfvhtyTolm3M.Q
-000003f0: 4f61 5a4c 6853 6e68 6e57 3548 5364 5957  OaZLhSnhnW5HSdYW
-00000400: 3051 4574 5734 4c62 3547 6b69 4764 5a53  0QEtW4Lb5GkiGdZS
-00000410: 4172 6a4d 357a 442f 4d67 4869 746c 4f6d  ArjM5zD/MgHitlOm
-00000420: 3972 3049 4c2b 6e42 6274 4e51 5972 640a  9r0IL+nBbtNQYrd.
-00000430: 6938 3570 5465 6549 6c47 3743 5446 4774  i85pTeeIlG7CTFGt
-00000440: 7833 6239 4569 5159 4859 6c32 7865 5333  x3b9EiQYHYl2xeS3
-00000450: 5162 626c 6379 7343 6759 4276 5156 506b  QbblcysCgYBvQVPk
-00000460: 334f 5048 734d 616f 645a 744b 5357 5936  3OPHsMaodZtKSWY6
-00000470: 0a75 4945 6456 362f 336a 742b 4655 4158  .uIEdV6/3jt+FUAX
-00000480: 634f 5a50 6847 3671 7645 6f57 734f 6f32  cOZPhG6qvEoWsOo2
-00000490: 3955 4437 7758 4851 4474 596f 794f 564f  9UD7wXHQDtYoyOVO
-000004a0: 6452 3256 6d58 4644 6735 3570 7a33 7038  dR2VmXFDg55pz3p8
-000004b0: 6d0a 4a4c 7a39 4f70 546a 3755 4457 7a36  m.JLz9OpTj7UDWz6
-000004c0: 4158 4836 754a 396f 4246 7946 742b 5876  AXH6uJ9oBFyFt+Xv
-000004d0: 4838 4e79 4279 3255 4d42 4c2b 7241 6150  H8NyBy2UMBL+rAaP
-000004e0: 5052 514c 624c 5343 6463 5044 5862 5854  PRQLbLSCdcPDXbXT
-000004f0: 424c 0a55 5042 7431 6b62 2f32 637a 566b  BL.UPBt1kb/2czVk
-00000500: 585a 2f41 4939 7977 514b 4267 5143 4767  XZ/AI9ywQKBgQCGg
-00000510: 736d 3051 6854 6b36 4a39 416b 646d 656e  sm0QhTk6J9Akdmen
-00000520: 485a 6132 4645 7133 326b 7574 464d 4753  HZa2FEq32kutFMGS
-00000530: 7a67 490a 7148 6854 6f4a 706c 6f57 2f63  zgI.qHhToJploW/c
-00000540: 5777 5072 3155 6648 4943 7234 764f 356b  WwPr1UfHICr4vO5k
-00000550: 3754 3058 7364 354c 5646 304f 6d52 316e  7T0Xsd5LVF0OmR1n
-00000560: 527a 4d4e 5a57 3938 6878 4d6e 7767 4f45  RzMNZW98hxMnwgOE
-00000570: 7136 7949 0a7a 666b 2b31 364d 725a 484a  q6yI.zfk+16MrZHJ
-00000580: 6257 6f4d 5045 4a6a 364b 412b 432b 6b65  bWoMPEJj6KA+C+ke
-00000590: 6663 304a 4837 6867 444a 3831 3831 5246  fc0JH7hgDJ8181RF
-000005a0: 5438 5739 546d 6441 6d32 4d4b 4435 3165  T8W9TmdAm2MKD51e
-000005b0: 524a 7642 720a 616a 476a 5177 4b42 6751  RJvBr.ajGjQwKBgQ
-000005c0: 4376 4e66 3844 7334 536d 792f 3541 4e79  CvNf8Ds4Smy/5ANy
-000005d0: 4f6a 4b33 2f69 505a 6947 6956 6779 614b  OjK3/iPZiGiVgyaK
-000005e0: 434a 4f4b 4e48 512b 7041 4430 4a53 3858  CJOKNHQ+pAD0JS8X
-000005f0: 664f 682f 4b6d 0a4b 6958 7638 6a42 4551  fOh/Km.KiXv8jBEQ
-00000600: 6343 6842 3759 6f59 4b42 5566 5877 7053  cChB7YoYKBUfXwpS
-00000610: 4c46 7275 4a55 336b 434c 764e 344d 4851  LFruJU3kCLvN4MHQ
-00000620: 4167 5630 4266 5678 384d 6b63 4c4a 6836  AgV0BfVx8MkcLJh6
-00000630: 4b2b 774d 4750 580a 4573 3568 6a36 7234  K+wMGPX.Es5hj6r4
-00000640: 5251 5162 6c4a 616a 3971 3871 6233 2b39  RQQblJaj9q8qb3+9
-00000650: 7547 336b 3753 6e34 5458 6330 5459 6737  uG3k7Sn4TXc0TYg7
-00000660: 6d6c 3332 7567 5853 584d 7866 4b67 3d3d  ml32ugXSXMxfKg==
-00000670: 0a2d 2d2d 2d2d 454e 4420 5253 4120 5052  .-----END RSA PR
-00000680: 4956 4154 4520 4b45 592d 2d2d 2d2d 0a    IVATE KEY-----.
+00000010: 5249 5641 5445 204b 4559 2d2d 2d2d 2d0d  RIVATE KEY-----.
+00000020: 0a4d 4949 4570 4149 4241 414b 4341 5145  .MIIEpAIBAAKCAQE
+00000030: 4170 3644 6f41 744d 4e35 6b6b 7472 7145  Ap6DoAtMN5kktrqE
+00000040: 5544 6e43 725a 4174 376e 6838 6150 4951  UDnCrZAt7nh8aPIQ
+00000050: 3137 485a 7757 676e 584c 3650 4973 6172  17HZwWgnXL6PIsar
+00000060: 320d 0a49 696a 2f37 6347 516d 374d 2f75  2..Iij/7cGQm7M/u
+00000070: 5742 6852 7041 7342 6c71 3356 2f56 5053  WBhRpAsBlq3V/VPS
+00000080: 4d76 2b39 4b39 5879 3871 4766 5061 4c4d  Mv+9K9Xy8qGfPaLM
+00000090: 4933 2b48 6f74 7858 4d78 5834 3077 645a  I3+HotxXMxX40wdZ
+000000a0: 654b 590d 0a4a 7777 5743 6c6f 454a 6948  eKY..JwwWCloEJiH
+000000b0: 5a47 6435 3975 6d4a 6a56 7076 2b48 7433  ZGd59umJjVpv+Ht3
+000000c0: 4a75 7453 6d47 5048 7954 644c 2f55 4a65  JutSmGPHyTdL/UJe
+000000d0: 5451 6352 2f73 5561 3738 4b6f 4a42 5557  TQcR/sUa78KoJBUW
+000000e0: 5358 434c 670d 0a42 4775 354e 7642 512f  SXCLg..BGu5NvBQ/
+000000f0: 796d 6a43 7a6f 417a 4d62 6268 5633 4b45  ymjCzoAzMbbhV3KE
+00000100: 4573 452b 2b59 494a 6f54 5050 576e 684f  EsE++YIJoTPPWnhO
+00000110: 4a43 6e2f 6a47 7875 335a 4d4b 4664 3874  JCn/jGxu3ZMKFd8t
+00000120: 5957 5276 3446 750d 0a67 6138 6933 364e  YWRv4Fu..ga8i36N
+00000130: 7351 474a 576b 4d4c 637a 7754 3459 4250  sQGJWkMLczwT4YBP
+00000140: 494c 4b73 6254 7535 6673 4d62 394e 7954  ILKsbTu5fsMb9NyT
+00000150: 7035 4430 4451 5668 7748 2b7a 4c5a 5a4b  p5D0DQVhwH+zLZZK
+00000160: 6e54 4f6f 4e4e 314b 310d 0a70 6e30 7859  nTOoNN1K1..pn0xY
+00000170: 6173 7a78 4b38 3749 6c6a 6c77 3851 396e  aszxK87Iljlw8Q9n
+00000180: 4f52 306f 724c 4e75 4278 3634 4264 2b36  OR0orLNuBx64Bd+6
+00000190: 7749 4441 5141 4241 6f49 4241 4373 5652  wIDAQABAoIBACsVR
+000001a0: 4178 5679 6d44 4274 6967 480d 0a35 6d75  AxVymDBtigH..5mu
+000001b0: 2f73 5931 4a46 6b43 5270 6543 6636 6d77  /sY1JFkCRpeCf6mw
+000001c0: 5946 4e42 5062 7973 6a59 5657 6f70 7849  YFNBPbysjYVWopxI
+000001d0: 6f6a 3337 4148 5461 6e58 3131 3531 4161  oj37AHTanX1151Aa
+000001e0: 617a 3358 696f 7654 4d61 3941 390d 0a2f  az3XiovTMa9A9../
+000001f0: 6731 4e63 3764 4247 6b66 4c35 674a 5976  g1Nc7dBGkfL5gJYv
+00000200: 464f 4661 3246 3663 3678 4c78 394b 4435  FOFa2F6c6xLx9KD5
+00000210: 7139 4366 2f65 7849 7866 5a34 7a36 7533  q9Cf/exIxfZ4z6u3
+00000220: 496d 6d39 2f6b 7570 7157 7751 3054 740d  Imm9/kupqWwQ0Tt.
+00000230: 0a6d 724d 576e 4477 3857 7271 502b 7030  .mrMWnDw8WrqP+p0
+00000240: 5172 2f45 5553 5147 5638 6a4f 5550 3353  Qr/EUSQGV8jOUP3S
+00000250: 7941 337a 5162 4562 7342 6b65 7474 7a34  yA3zQbEbsBkettz4
+00000260: 4e69 6c39 4e49 5477 6251 7262 6e47 366f  Nil9NITwbQrbnG6o
+00000270: 370d 0a52 6e4e 7578 4377 5277 4f33 5142  7..RnNuxCwRwO3QB
+00000280: 3170 3059 4f58 6e4b 7974 5538 7849 7537  1p0YOXnKytU8xIu7
+00000290: 3858 6733 7177 5678 3831 5150 332f 6f6d  8Xg3qwVx81QP3/om
+000002a0: 4239 6a4e 4359 3532 7031 4652 4c7a 474f  B9jNCY52p1FRLzGO
+000002b0: 3231 710d 0a4a 465a 4c49 6350 3768 4543  21q..JFZLIcP7hEC
+000002c0: 6573 6e35 7639 645a 6139 396f 4368 552b  esn5v9dZa99oChU+
+000002d0: 5264 7a69 3933 5645 796d 776d 5a42 566c  Rdzi93VEymwmZBVl
+000002e0: 3867 6976 4e64 5741 6531 5937 632f 5a38  8givNdWAe1Y7c/Z8
+000002f0: 6649 5753 2f0d 0a46 5156 7652 6745 4367  fIWS/..FQVvRgECg
+00000300: 5945 4131 3275 5a52 6c4c 446e 446f 7159  YEA12uZRlLDnDoqY
+00000310: 546a 354f 7473 3837 4b70 7931 3577 5535  Tj5Ots87Kpy15wU5
+00000320: 6c41 3241 5347 4e67 6151 4c58 5a42 6768  lA2ASGNgaQLXZBgh
+00000330: 3849 442f 386f 350d 0a51 526b 312f 434e  8ID/8o5..QRk1/CN
+00000340: 5732 692f 6357 2f66 4937 5852 6169 466f  W2i/cW/fI7XRaiFo
+00000350: 486a 7276 4436 5867 5430 6d2f 6257 4f65  HjrvD6XgT0m/bWOe
+00000360: 7a46 5758 6f65 6d6b 4d52 2f6a 5232 6b59  zFWXoemkMR/jR2kY
+00000370: 5a6a 5330 7670 6330 340d 0a77 642f 7276  ZjS0vpc04..wd/rv
+00000380: 7248 7234 6e62 5351 4531 6356 4277 4c72  rHr4nbSQE1cVBwLr
+00000390: 597a 7259 4a36 7172 4779 6278 3950 366b  YzrYJ6qrGybx9P6k
+000003a0: 3066 6875 3266 5549 4a49 4a47 454f 5451  0fhu2fUIJIJGEOTQ
+000003b0: 3045 4367 5945 4178 7a53 610d 0a66 344b  0ECgYEAxzSa..f4K
+000003c0: 4c47 5372 5a6a 665a 6c36 3935 7a2b 3833  LGSrZjfZl695z+83
+000003d0: 5655 4735 6165 6738 5634 3037 6e41 3652  VUG5aeg8V407nA6R
+000003e0: 4277 3358 654b 3942 6a48 6871 6673 526e  Bw3XeK9BjHhqfsRn
+000003f0: 4641 6676 6874 7954 6f6c 6d33 4d0d 0a51  FAfvhtyTolm3M..Q
+00000400: 4f61 5a4c 6853 6e68 6e57 3548 5364 5957  OaZLhSnhnW5HSdYW
+00000410: 3051 4574 5734 4c62 3547 6b69 4764 5a53  0QEtW4Lb5GkiGdZS
+00000420: 4172 6a4d 357a 442f 4d67 4869 746c 4f6d  ArjM5zD/MgHitlOm
+00000430: 3972 3049 4c2b 6e42 6274 4e51 5972 640d  9r0IL+nBbtNQYrd.
+00000440: 0a69 3835 7054 6565 496c 4737 4354 4647  .i85pTeeIlG7CTFG
+00000450: 7478 3362 3945 6951 5948 596c 3278 6553  tx3b9EiQYHYl2xeS
+00000460: 3351 6262 6c63 7973 4367 5942 7651 5650  3QbblcysCgYBvQVP
+00000470: 6b33 4f50 4873 4d61 6f64 5a74 4b53 5759  k3OPHsMaodZtKSWY
+00000480: 360d 0a75 4945 6456 362f 336a 742b 4655  6..uIEdV6/3jt+FU
+00000490: 4158 634f 5a50 6847 3671 7645 6f57 734f  AXcOZPhG6qvEoWsO
+000004a0: 6f32 3955 4437 7758 4851 4474 596f 794f  o29UD7wXHQDtYoyO
+000004b0: 564f 6452 3256 6d58 4644 6735 3570 7a33  VOdR2VmXFDg55pz3
+000004c0: 7038 6d0d 0a4a 4c7a 394f 7054 6a37 5544  p8m..JLz9OpTj7UD
+000004d0: 577a 3641 5848 3675 4a39 6f42 4679 4674  Wz6AXH6uJ9oBFyFt
+000004e0: 2b58 7648 384e 7942 7932 554d 424c 2b72  +XvH8NyBy2UMBL+r
+000004f0: 4161 5050 5251 4c62 4c53 4364 6350 4458  AaPPRQLbLSCdcPDX
+00000500: 6258 5442 4c0d 0a55 5042 7431 6b62 2f32  bXTBL..UPBt1kb/2
+00000510: 637a 566b 585a 2f41 4939 7977 514b 4267  czVkXZ/AI9ywQKBg
+00000520: 5143 4767 736d 3051 6854 6b36 4a39 416b  QCGgsm0QhTk6J9Ak
+00000530: 646d 656e 485a 6132 4645 7133 326b 7574  dmenHZa2FEq32kut
+00000540: 464d 4753 7a67 490d 0a71 4868 546f 4a70  FMGSzgI..qHhToJp
+00000550: 6c6f 572f 6357 7750 7231 5566 4849 4372  loW/cWwPr1UfHICr
+00000560: 3476 4f35 6b37 5430 5873 6435 4c56 4630  4vO5k7T0Xsd5LVF0
+00000570: 4f6d 5231 6e52 7a4d 4e5a 5739 3868 784d  OmR1nRzMNZW98hxM
+00000580: 6e77 674f 4571 3679 490d 0a7a 666b 2b31  nwgOEq6yI..zfk+1
+00000590: 364d 725a 484a 6257 6f4d 5045 4a6a 364b  6MrZHJbWoMPEJj6K
+000005a0: 412b 432b 6b65 6663 304a 4837 6867 444a  A+C+kefc0JH7hgDJ
+000005b0: 3831 3831 5246 5438 5739 546d 6441 6d32  8181RFT8W9TmdAm2
+000005c0: 4d4b 4435 3165 524a 7642 720d 0a61 6a47  MKD51eRJvBr..ajG
+000005d0: 6a51 774b 4267 5143 764e 6638 4473 3453  jQwKBgQCvNf8Ds4S
+000005e0: 6d79 2f35 414e 794f 6a4b 332f 6950 5a69  my/5ANyOjK3/iPZi
+000005f0: 4769 5667 7961 4b43 4a4f 4b4e 4851 2b70  GiVgyaKCJOKNHQ+p
+00000600: 4144 304a 5338 5866 4f68 2f4b 6d0d 0a4b  AD0JS8XfOh/Km..K
+00000610: 6958 7638 6a42 4551 6343 6842 3759 6f59  iXv8jBEQcChB7YoY
+00000620: 4b42 5566 5877 7053 4c46 7275 4a55 336b  KBUfXwpSLFruJU3k
+00000630: 434c 764e 344d 4851 4167 5630 4266 5678  CLvN4MHQAgV0BfVx
+00000640: 384d 6b63 4c4a 6836 4b2b 774d 4750 580d  8MkcLJh6K+wMGPX.
+00000650: 0a45 7335 686a 3672 3452 5151 626c 4a61  .Es5hj6r4RQQblJa
+00000660: 6a39 7138 7162 332b 3975 4733 6b37 536e  j9q8qb3+9uG3k7Sn
+00000670: 3454 5863 3054 5967 376d 6c33 3275 6758  4TXc0TYg7ml32ugX
+00000680: 5358 4d78 664b 673d 3d0d 0a2d 2d2d 2d2d  SXMxfKg==..-----
+00000690: 454e 4420 5253 4120 5052 4956 4154 4520  END RSA PRIVATE 
+000006a0: 4b45 592d 2d2d 2d2d 0d0a                 KEY-----..
```

### Comparing `tabpy-2.6.0/tests/integration/resources/deploy_and_evaluate_model.conf` & `tabpy-2.7.0/tests/integration/resources/deploy_and_evaluate_model_auth.conf`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,99 @@
-00000000: 5b54 6162 5079 5d0a 2320 5441 4250 595f  [TabPy].# TABPY_
-00000010: 5155 4552 595f 4f42 4a45 4354 5f50 4154  QUERY_OBJECT_PAT
-00000020: 4820 3d20 2f74 6d70 2f71 7565 7279 5f6f  H = /tmp/query_o
-00000030: 626a 6563 7473 0a54 4142 5059 5f50 4f52  bjects.TABPY_POR
-00000040: 5420 3d20 3930 3038 0a23 2054 4142 5059  T = 9008.# TABPY
-00000050: 5f53 5441 5445 5f50 4154 4820 3d20 2e2f  _STATE_PATH = ./
-00000060: 7461 6270 792f 7461 6270 795f 7365 7276  tabpy/tabpy_serv
-00000070: 6572 0a0a 2320 5768 6572 6520 7374 6174  er..# Where stat
-00000080: 6963 2070 6167 6573 206c 6976 650a 2320  ic pages live.# 
-00000090: 5441 4250 595f 5354 4154 4943 5f50 4154  TABPY_STATIC_PAT
-000000a0: 4820 3d20 2e2f 7461 6270 792f 7461 6270  H = ./tabpy/tabp
-000000b0: 795f 7365 7276 6572 2f73 7461 7469 630a  y_server/static.
-000000c0: 0a23 2046 6f72 2068 6f77 2074 6f20 636f  .# For how to co
-000000d0: 6e66 6967 7572 6520 5461 6250 7920 6175  nfigure TabPy au
-000000e0: 7468 656e 7469 6361 7469 6f6e 2072 6561  thentication rea
-000000f0: 640a 2320 4175 7468 656e 7469 6361 7469  d.# Authenticati
-00000100: 6f6e 2073 6563 7469 6f6e 2069 6e20 646f  on section in do
-00000110: 6373 2f73 6572 7665 722d 636f 6e66 6967  cs/server-config
-00000120: 2e6d 642e 0a23 2054 4142 5059 5f50 5744  .md..# TABPY_PWD
-00000130: 5f46 494c 4520 3d20 2f70 6174 682f 746f  _FILE = /path/to
-00000140: 2f70 6173 7377 6f72 642f 6669 6c65 2e74  /password/file.t
-00000150: 7874 0a0a 2320 546f 2073 6574 2075 7020  xt..# To set up 
-00000160: 7365 6375 7265 2054 6162 5079 2075 6e63  secure TabPy unc
-00000170: 6f6d 6d65 6e74 2061 6e64 206d 6f64 6966  omment and modif
-00000180: 7920 7468 6520 666f 6c6c 6f77 696e 6720  y the following 
-00000190: 6c69 6e65 732e 0a23 204e 6f74 6520 6f6e  lines..# Note on
-000001a0: 6c79 2050 454d 2d65 6e63 6f64 6564 2078  ly PEM-encoded x
-000001b0: 3530 3920 6365 7274 6966 6963 6174 6573  509 certificates
-000001c0: 2061 7265 2073 7570 706f 7274 6564 2e0a   are supported..
-000001d0: 2320 5441 4250 595f 5452 414e 5346 4552  # TABPY_TRANSFER
-000001e0: 5f50 524f 544f 434f 4c20 3d20 6874 7470  _PROTOCOL = http
-000001f0: 730a 2320 5441 4250 595f 4345 5254 4946  s.# TABPY_CERTIF
-00000200: 4943 4154 455f 4649 4c45 203d 2070 6174  ICATE_FILE = pat
-00000210: 682f 746f 2f63 6572 7469 6669 6361 7465  h/to/certificate
-00000220: 2f66 696c 652e 6372 740a 2320 5441 4250  /file.crt.# TABP
-00000230: 595f 4b45 595f 4649 4c45 203d 2070 6174  Y_KEY_FILE = pat
-00000240: 682f 746f 2f6b 6579 2f66 696c 652e 6b65  h/to/key/file.ke
-00000250: 790a 0a23 204c 6f67 2061 6464 6974 696f  y..# Log additio
-00000260: 6e61 6c20 7265 7175 6573 7420 6465 7461  nal request deta
-00000270: 696c 7320 696e 636c 7564 696e 6720 6361  ils including ca
-00000280: 6c6c 6572 2049 502c 2066 756c 6c20 5552  ller IP, full UR
-00000290: 4c2c 2063 6c69 656e 740a 2320 656e 6420  L, client.# end 
-000002a0: 7573 6572 2069 6e66 6f20 6966 2070 726f  user info if pro
-000002b0: 7669 6465 642e 0a23 2054 4142 5059 5f4c  vided..# TABPY_L
-000002c0: 4f47 5f44 4554 4149 4c53 203d 2074 7275  OG_DETAILS = tru
-000002d0: 650a 0a23 2043 6f6e 6669 6775 7265 2068  e..# Configure h
-000002e0: 6f77 206c 6f6e 6720 6120 6375 7374 6f6d  ow long a custom
-000002f0: 2073 6372 6970 7420 7072 6f76 6964 6564   script provided
-00000300: 2074 6f20 7468 6520 2f65 7661 6c75 6174   to the /evaluat
-00000310: 6520 6d65 7468 6f64 0a23 2077 696c 6c20  e method.# will 
-00000320: 7275 6e20 6265 666f 7265 2074 6872 6f77  run before throw
-00000330: 696e 6720 6120 5469 6d65 6f75 7445 7272  ing a TimeoutErr
-00000340: 6f72 2e0a 2320 5468 6520 7661 6c75 6520  or..# The value 
-00000350: 7368 6f75 6c64 2062 6520 6120 666c 6f61  should be a floa
-00000360: 7420 7265 7072 6573 656e 7469 6e67 2074  t representing t
-00000370: 6865 2074 696d 656f 7574 2074 696d 6520  he timeout time 
-00000380: 696e 2073 6563 6f6e 6473 2e0a 2354 4142  in seconds..#TAB
-00000390: 5059 5f45 5641 4c55 4154 455f 5449 4d45  PY_EVALUATE_TIME
-000003a0: 4f55 5420 3d20 3330 0a0a 5b6c 6f67 6765  OUT = 30..[logge
-000003b0: 7273 5d0a 6b65 7973 3d72 6f6f 740a 0a5b  rs].keys=root..[
-000003c0: 6861 6e64 6c65 7273 5d0a 6b65 7973 3d72  handlers].keys=r
-000003d0: 6f6f 7448 616e 646c 6572 2c72 6f74 6174  ootHandler,rotat
-000003e0: 696e 6746 696c 6548 616e 646c 6572 0a0a  ingFileHandler..
-000003f0: 5b66 6f72 6d61 7474 6572 735d 0a6b 6579  [formatters].key
-00000400: 733d 726f 6f74 466f 726d 6174 7465 720a  s=rootFormatter.
-00000410: 0a5b 6c6f 6767 6572 5f72 6f6f 745d 0a6c  .[logger_root].l
-00000420: 6576 656c 3d44 4542 5547 0a68 616e 646c  evel=DEBUG.handl
-00000430: 6572 733d 726f 6f74 4861 6e64 6c65 722c  ers=rootHandler,
-00000440: 726f 7461 7469 6e67 4669 6c65 4861 6e64  rotatingFileHand
-00000450: 6c65 720a 7175 616c 6e61 6d65 3d72 6f6f  ler.qualname=roo
-00000460: 740a 7072 6f70 6167 6574 653d 300a 0a5b  t.propagete=0..[
-00000470: 6861 6e64 6c65 725f 726f 6f74 4861 6e64  handler_rootHand
-00000480: 6c65 725d 0a63 6c61 7373 3d53 7472 6561  ler].class=Strea
-00000490: 6d48 616e 646c 6572 0a6c 6576 656c 3d44  mHandler.level=D
-000004a0: 4542 5547 0a66 6f72 6d61 7474 6572 3d72  EBUG.formatter=r
-000004b0: 6f6f 7446 6f72 6d61 7474 6572 0a61 7267  ootFormatter.arg
-000004c0: 733d 2873 7973 2e73 7464 6f75 742c 290a  s=(sys.stdout,).
-000004d0: 0a5b 6861 6e64 6c65 725f 726f 7461 7469  .[handler_rotati
-000004e0: 6e67 4669 6c65 4861 6e64 6c65 725d 0a63  ngFileHandler].c
-000004f0: 6c61 7373 3d68 616e 646c 6572 732e 526f  lass=handlers.Ro
-00000500: 7461 7469 6e67 4669 6c65 4861 6e64 6c65  tatingFileHandle
-00000510: 720a 6c65 7665 6c3d 4445 4255 470a 666f  r.level=DEBUG.fo
-00000520: 726d 6174 7465 723d 726f 6f74 466f 726d  rmatter=rootForm
-00000530: 6174 7465 720a 6172 6773 3d28 2774 6162  atter.args=('tab
-00000540: 7079 5f6c 6f67 2e6c 6f67 272c 2027 6127  py_log.log', 'a'
-00000550: 2c20 3130 3030 3030 302c 2035 290a 0a5b  , 1000000, 5)..[
-00000560: 666f 726d 6174 7465 725f 726f 6f74 466f  formatter_rootFo
-00000570: 726d 6174 7465 725d 0a66 6f72 6d61 743d  rmatter].format=
-00000580: 2528 6173 6374 696d 6529 7320 5b25 286c  %(asctime)s [%(l
-00000590: 6576 656c 6e61 6d65 2973 5d20 2825 2866  evelname)s] (%(f
-000005a0: 696c 656e 616d 6529 733a 2528 6d6f 6475  ilename)s:%(modu
-000005b0: 6c65 2973 3a25 286c 696e 656e 6f29 6429  le)s:%(lineno)d)
-000005c0: 3a20 2528 6d65 7373 6167 6529 730a 6461  : %(message)s.da
-000005d0: 7465 666d 743d 2559 2d25 6d2d 2564 2c25  tefmt=%Y-%m-%d,%
-000005e0: 483a 254d 3a25 530a                      H:%M:%S.
+00000000: 5b54 6162 5079 5d0d 0a23 2054 4142 5059  [TabPy]..# TABPY
+00000010: 5f51 5545 5259 5f4f 424a 4543 545f 5041  _QUERY_OBJECT_PA
+00000020: 5448 203d 202f 746d 702f 7175 6572 795f  TH = /tmp/query_
+00000030: 6f62 6a65 6374 730d 0a54 4142 5059 5f50  objects..TABPY_P
+00000040: 4f52 5420 3d20 3930 3039 0d0a 2320 5441  ORT = 9009..# TA
+00000050: 4250 595f 5354 4154 455f 5041 5448 203d  BPY_STATE_PATH =
+00000060: 202e 2f74 6162 7079 2f74 6162 7079 5f73   ./tabpy/tabpy_s
+00000070: 6572 7665 720d 0a0d 0a23 2057 6865 7265  erver....# Where
+00000080: 2073 7461 7469 6320 7061 6765 7320 6c69   static pages li
+00000090: 7665 0d0a 2320 5441 4250 595f 5354 4154  ve..# TABPY_STAT
+000000a0: 4943 5f50 4154 4820 3d20 2e2f 7461 6270  IC_PATH = ./tabp
+000000b0: 792f 7461 6270 795f 7365 7276 6572 2f73  y/tabpy_server/s
+000000c0: 7461 7469 630d 0a0d 0a23 2046 6f72 2068  tatic....# For h
+000000d0: 6f77 2074 6f20 636f 6e66 6967 7572 6520  ow to configure 
+000000e0: 5461 6250 7920 6175 7468 656e 7469 6361  TabPy authentica
+000000f0: 7469 6f6e 2072 6561 640d 0a23 2041 7574  tion read..# Aut
+00000100: 6865 6e74 6963 6174 696f 6e20 7365 6374  hentication sect
+00000110: 696f 6e20 696e 2064 6f63 732f 7365 7276  ion in docs/serv
+00000120: 6572 2d63 6f6e 6669 672e 6d64 2e0d 0a54  er-config.md...T
+00000130: 4142 5059 5f50 5744 5f46 494c 4520 3d20  ABPY_PWD_FILE = 
+00000140: 2e2f 7465 7374 732f 696e 7465 6772 6174  ./tests/integrat
+00000150: 696f 6e2f 7265 736f 7572 6365 732f 7077  ion/resources/pw
+00000160: 6466 696c 652e 7478 740d 0a0d 0a23 2054  dfile.txt....# T
+00000170: 6f20 7365 7420 7570 2073 6563 7572 6520  o set up secure 
+00000180: 5461 6250 7920 756e 636f 6d6d 656e 7420  TabPy uncomment 
+00000190: 616e 6420 6d6f 6469 6679 2074 6865 2066  and modify the f
+000001a0: 6f6c 6c6f 7769 6e67 206c 696e 6573 2e0d  ollowing lines..
+000001b0: 0a23 204e 6f74 6520 6f6e 6c79 2050 454d  .# Note only PEM
+000001c0: 2d65 6e63 6f64 6564 2078 3530 3920 6365  -encoded x509 ce
+000001d0: 7274 6966 6963 6174 6573 2061 7265 2073  rtificates are s
+000001e0: 7570 706f 7274 6564 2e0d 0a23 2054 4142  upported...# TAB
+000001f0: 5059 5f54 5241 4e53 4645 525f 5052 4f54  PY_TRANSFER_PROT
+00000200: 4f43 4f4c 203d 2068 7474 7073 0d0a 2320  OCOL = https..# 
+00000210: 5441 4250 595f 4345 5254 4946 4943 4154  TABPY_CERTIFICAT
+00000220: 455f 4649 4c45 203d 2070 6174 682f 746f  E_FILE = path/to
+00000230: 2f63 6572 7469 6669 6361 7465 2f66 696c  /certificate/fil
+00000240: 652e 6372 740d 0a23 2054 4142 5059 5f4b  e.crt..# TABPY_K
+00000250: 4559 5f46 494c 4520 3d20 7061 7468 2f74  EY_FILE = path/t
+00000260: 6f2f 6b65 792f 6669 6c65 2e6b 6579 0d0a  o/key/file.key..
+00000270: 0d0a 2320 4c6f 6720 6164 6469 7469 6f6e  ..# Log addition
+00000280: 616c 2072 6571 7565 7374 2064 6574 6169  al request detai
+00000290: 6c73 2069 6e63 6c75 6469 6e67 2063 616c  ls including cal
+000002a0: 6c65 7220 4950 2c20 6675 6c6c 2055 524c  ler IP, full URL
+000002b0: 2c20 636c 6965 6e74 0d0a 2320 656e 6420  , client..# end 
+000002c0: 7573 6572 2069 6e66 6f20 6966 2070 726f  user info if pro
+000002d0: 7669 6465 642e 0d0a 2320 5441 4250 595f  vided...# TABPY_
+000002e0: 4c4f 475f 4445 5441 494c 5320 3d20 7472  LOG_DETAILS = tr
+000002f0: 7565 0d0a 0d0a 2320 436f 6e66 6967 7572  ue....# Configur
+00000300: 6520 686f 7720 6c6f 6e67 2061 2063 7573  e how long a cus
+00000310: 746f 6d20 7363 7269 7074 2070 726f 7669  tom script provi
+00000320: 6465 6420 746f 2074 6865 202f 6576 616c  ded to the /eval
+00000330: 7561 7465 206d 6574 686f 640d 0a23 2077  uate method..# w
+00000340: 696c 6c20 7275 6e20 6265 666f 7265 2074  ill run before t
+00000350: 6872 6f77 696e 6720 6120 5469 6d65 6f75  hrowing a Timeou
+00000360: 7445 7272 6f72 2e0d 0a23 2054 6865 2076  tError...# The v
+00000370: 616c 7565 2073 686f 756c 6420 6265 2061  alue should be a
+00000380: 2066 6c6f 6174 2072 6570 7265 7365 6e74   float represent
+00000390: 696e 6720 7468 6520 7469 6d65 6f75 7420  ing the timeout 
+000003a0: 7469 6d65 2069 6e20 7365 636f 6e64 732e  time in seconds.
+000003b0: 0d0a 2354 4142 5059 5f45 5641 4c55 4154  ..#TABPY_EVALUAT
+000003c0: 455f 5449 4d45 4f55 5420 3d20 3330 0d0a  E_TIMEOUT = 30..
+000003d0: 0d0a 5b6c 6f67 6765 7273 5d0d 0a6b 6579  ..[loggers]..key
+000003e0: 733d 726f 6f74 0d0a 0d0a 5b68 616e 646c  s=root....[handl
+000003f0: 6572 735d 0d0a 6b65 7973 3d72 6f6f 7448  ers]..keys=rootH
+00000400: 616e 646c 6572 2c72 6f74 6174 696e 6746  andler,rotatingF
+00000410: 696c 6548 616e 646c 6572 0d0a 0d0a 5b66  ileHandler....[f
+00000420: 6f72 6d61 7474 6572 735d 0d0a 6b65 7973  ormatters]..keys
+00000430: 3d72 6f6f 7446 6f72 6d61 7474 6572 0d0a  =rootFormatter..
+00000440: 0d0a 5b6c 6f67 6765 725f 726f 6f74 5d0d  ..[logger_root].
+00000450: 0a6c 6576 656c 3d44 4542 5547 0d0a 6861  .level=DEBUG..ha
+00000460: 6e64 6c65 7273 3d72 6f6f 7448 616e 646c  ndlers=rootHandl
+00000470: 6572 2c72 6f74 6174 696e 6746 696c 6548  er,rotatingFileH
+00000480: 616e 646c 6572 0d0a 7175 616c 6e61 6d65  andler..qualname
+00000490: 3d72 6f6f 740d 0a70 726f 7061 6765 7465  =root..propagete
+000004a0: 3d30 0d0a 0d0a 5b68 616e 646c 6572 5f72  =0....[handler_r
+000004b0: 6f6f 7448 616e 646c 6572 5d0d 0a63 6c61  ootHandler]..cla
+000004c0: 7373 3d53 7472 6561 6d48 616e 646c 6572  ss=StreamHandler
+000004d0: 0d0a 6c65 7665 6c3d 4445 4255 470d 0a66  ..level=DEBUG..f
+000004e0: 6f72 6d61 7474 6572 3d72 6f6f 7446 6f72  ormatter=rootFor
+000004f0: 6d61 7474 6572 0d0a 6172 6773 3d28 7379  matter..args=(sy
+00000500: 732e 7374 646f 7574 2c29 0d0a 0d0a 5b68  s.stdout,)....[h
+00000510: 616e 646c 6572 5f72 6f74 6174 696e 6746  andler_rotatingF
+00000520: 696c 6548 616e 646c 6572 5d0d 0a63 6c61  ileHandler]..cla
+00000530: 7373 3d68 616e 646c 6572 732e 526f 7461  ss=handlers.Rota
+00000540: 7469 6e67 4669 6c65 4861 6e64 6c65 720d  tingFileHandler.
+00000550: 0a6c 6576 656c 3d44 4542 5547 0d0a 666f  .level=DEBUG..fo
+00000560: 726d 6174 7465 723d 726f 6f74 466f 726d  rmatter=rootForm
+00000570: 6174 7465 720d 0a61 7267 733d 2827 7461  atter..args=('ta
+00000580: 6270 795f 6c6f 672e 6c6f 6727 2c20 2761  bpy_log.log', 'a
+00000590: 272c 2031 3030 3030 3030 2c20 3529 0d0a  ', 1000000, 5)..
+000005a0: 0d0a 5b66 6f72 6d61 7474 6572 5f72 6f6f  ..[formatter_roo
+000005b0: 7446 6f72 6d61 7474 6572 5d0d 0a66 6f72  tFormatter]..for
+000005c0: 6d61 743d 2528 6173 6374 696d 6529 7320  mat=%(asctime)s 
+000005d0: 5b25 286c 6576 656c 6e61 6d65 2973 5d20  [%(levelname)s] 
+000005e0: 2825 2866 696c 656e 616d 6529 733a 2528  (%(filename)s:%(
+000005f0: 6d6f 6475 6c65 2973 3a25 286c 696e 656e  module)s:%(linen
+00000600: 6f29 6429 3a20 2528 6d65 7373 6167 6529  o)d): %(message)
+00000610: 730d 0a64 6174 6566 6d74 3d25 592d 256d  s..datefmt=%Y-%m
+00000620: 2d25 642c 2548 3a25 4d3a 2553 0d0a       -%d,%H:%M:%S..
```

### Comparing `tabpy-2.6.0/tests/integration/resources/deploy_and_evaluate_model_auth.conf` & `tabpy-2.7.0/tests/integration/resources/deploy_and_evaluate_model.conf`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,99 @@
-00000000: 5b54 6162 5079 5d0a 2320 5441 4250 595f  [TabPy].# TABPY_
-00000010: 5155 4552 595f 4f42 4a45 4354 5f50 4154  QUERY_OBJECT_PAT
-00000020: 4820 3d20 2f74 6d70 2f71 7565 7279 5f6f  H = /tmp/query_o
-00000030: 626a 6563 7473 0a54 4142 5059 5f50 4f52  bjects.TABPY_POR
-00000040: 5420 3d20 3930 3039 0a23 2054 4142 5059  T = 9009.# TABPY
-00000050: 5f53 5441 5445 5f50 4154 4820 3d20 2e2f  _STATE_PATH = ./
-00000060: 7461 6270 792f 7461 6270 795f 7365 7276  tabpy/tabpy_serv
-00000070: 6572 0a0a 2320 5768 6572 6520 7374 6174  er..# Where stat
-00000080: 6963 2070 6167 6573 206c 6976 650a 2320  ic pages live.# 
-00000090: 5441 4250 595f 5354 4154 4943 5f50 4154  TABPY_STATIC_PAT
-000000a0: 4820 3d20 2e2f 7461 6270 792f 7461 6270  H = ./tabpy/tabp
-000000b0: 795f 7365 7276 6572 2f73 7461 7469 630a  y_server/static.
-000000c0: 0a23 2046 6f72 2068 6f77 2074 6f20 636f  .# For how to co
-000000d0: 6e66 6967 7572 6520 5461 6250 7920 6175  nfigure TabPy au
-000000e0: 7468 656e 7469 6361 7469 6f6e 2072 6561  thentication rea
-000000f0: 640a 2320 4175 7468 656e 7469 6361 7469  d.# Authenticati
-00000100: 6f6e 2073 6563 7469 6f6e 2069 6e20 646f  on section in do
-00000110: 6373 2f73 6572 7665 722d 636f 6e66 6967  cs/server-config
-00000120: 2e6d 642e 0a54 4142 5059 5f50 5744 5f46  .md..TABPY_PWD_F
-00000130: 494c 4520 3d20 2e2f 7465 7374 732f 696e  ILE = ./tests/in
-00000140: 7465 6772 6174 696f 6e2f 7265 736f 7572  tegration/resour
-00000150: 6365 732f 7077 6466 696c 652e 7478 740a  ces/pwdfile.txt.
-00000160: 0a23 2054 6f20 7365 7420 7570 2073 6563  .# To set up sec
-00000170: 7572 6520 5461 6250 7920 756e 636f 6d6d  ure TabPy uncomm
-00000180: 656e 7420 616e 6420 6d6f 6469 6679 2074  ent and modify t
-00000190: 6865 2066 6f6c 6c6f 7769 6e67 206c 696e  he following lin
-000001a0: 6573 2e0a 2320 4e6f 7465 206f 6e6c 7920  es..# Note only 
+00000000: 5b54 6162 5079 5d0d 0a23 2054 4142 5059  [TabPy]..# TABPY
+00000010: 5f51 5545 5259 5f4f 424a 4543 545f 5041  _QUERY_OBJECT_PA
+00000020: 5448 203d 202f 746d 702f 7175 6572 795f  TH = /tmp/query_
+00000030: 6f62 6a65 6374 730d 0a54 4142 5059 5f50  objects..TABPY_P
+00000040: 4f52 5420 3d20 3930 3038 0d0a 2320 5441  ORT = 9008..# TA
+00000050: 4250 595f 5354 4154 455f 5041 5448 203d  BPY_STATE_PATH =
+00000060: 202e 2f74 6162 7079 2f74 6162 7079 5f73   ./tabpy/tabpy_s
+00000070: 6572 7665 720d 0a0d 0a23 2057 6865 7265  erver....# Where
+00000080: 2073 7461 7469 6320 7061 6765 7320 6c69   static pages li
+00000090: 7665 0d0a 2320 5441 4250 595f 5354 4154  ve..# TABPY_STAT
+000000a0: 4943 5f50 4154 4820 3d20 2e2f 7461 6270  IC_PATH = ./tabp
+000000b0: 792f 7461 6270 795f 7365 7276 6572 2f73  y/tabpy_server/s
+000000c0: 7461 7469 630d 0a0d 0a23 2046 6f72 2068  tatic....# For h
+000000d0: 6f77 2074 6f20 636f 6e66 6967 7572 6520  ow to configure 
+000000e0: 5461 6250 7920 6175 7468 656e 7469 6361  TabPy authentica
+000000f0: 7469 6f6e 2072 6561 640d 0a23 2041 7574  tion read..# Aut
+00000100: 6865 6e74 6963 6174 696f 6e20 7365 6374  hentication sect
+00000110: 696f 6e20 696e 2064 6f63 732f 7365 7276  ion in docs/serv
+00000120: 6572 2d63 6f6e 6669 672e 6d64 2e0d 0a23  er-config.md...#
+00000130: 2054 4142 5059 5f50 5744 5f46 494c 4520   TABPY_PWD_FILE 
+00000140: 3d20 2f70 6174 682f 746f 2f70 6173 7377  = /path/to/passw
+00000150: 6f72 642f 6669 6c65 2e74 7874 0d0a 0d0a  ord/file.txt....
+00000160: 2320 546f 2073 6574 2075 7020 7365 6375  # To set up secu
+00000170: 7265 2054 6162 5079 2075 6e63 6f6d 6d65  re TabPy uncomme
+00000180: 6e74 2061 6e64 206d 6f64 6966 7920 7468  nt and modify th
+00000190: 6520 666f 6c6c 6f77 696e 6720 6c69 6e65  e following line
+000001a0: 732e 0d0a 2320 4e6f 7465 206f 6e6c 7920  s...# Note only 
 000001b0: 5045 4d2d 656e 636f 6465 6420 7835 3039  PEM-encoded x509
 000001c0: 2063 6572 7469 6669 6361 7465 7320 6172   certificates ar
-000001d0: 6520 7375 7070 6f72 7465 642e 0a23 2054  e supported..# T
-000001e0: 4142 5059 5f54 5241 4e53 4645 525f 5052  ABPY_TRANSFER_PR
-000001f0: 4f54 4f43 4f4c 203d 2068 7474 7073 0a23  OTOCOL = https.#
-00000200: 2054 4142 5059 5f43 4552 5449 4649 4341   TABPY_CERTIFICA
-00000210: 5445 5f46 494c 4520 3d20 7061 7468 2f74  TE_FILE = path/t
-00000220: 6f2f 6365 7274 6966 6963 6174 652f 6669  o/certificate/fi
-00000230: 6c65 2e63 7274 0a23 2054 4142 5059 5f4b  le.crt.# TABPY_K
-00000240: 4559 5f46 494c 4520 3d20 7061 7468 2f74  EY_FILE = path/t
-00000250: 6f2f 6b65 792f 6669 6c65 2e6b 6579 0a0a  o/key/file.key..
-00000260: 2320 4c6f 6720 6164 6469 7469 6f6e 616c  # Log additional
-00000270: 2072 6571 7565 7374 2064 6574 6169 6c73   request details
-00000280: 2069 6e63 6c75 6469 6e67 2063 616c 6c65   including calle
-00000290: 7220 4950 2c20 6675 6c6c 2055 524c 2c20  r IP, full URL, 
-000002a0: 636c 6965 6e74 0a23 2065 6e64 2075 7365  client.# end use
-000002b0: 7220 696e 666f 2069 6620 7072 6f76 6964  r info if provid
-000002c0: 6564 2e0a 2320 5441 4250 595f 4c4f 475f  ed..# TABPY_LOG_
-000002d0: 4445 5441 494c 5320 3d20 7472 7565 0a0a  DETAILS = true..
-000002e0: 2320 436f 6e66 6967 7572 6520 686f 7720  # Configure how 
-000002f0: 6c6f 6e67 2061 2063 7573 746f 6d20 7363  long a custom sc
-00000300: 7269 7074 2070 726f 7669 6465 6420 746f  ript provided to
-00000310: 2074 6865 202f 6576 616c 7561 7465 206d   the /evaluate m
-00000320: 6574 686f 640a 2320 7769 6c6c 2072 756e  ethod.# will run
-00000330: 2062 6566 6f72 6520 7468 726f 7769 6e67   before throwing
-00000340: 2061 2054 696d 656f 7574 4572 726f 722e   a TimeoutError.
-00000350: 0a23 2054 6865 2076 616c 7565 2073 686f  .# The value sho
-00000360: 756c 6420 6265 2061 2066 6c6f 6174 2072  uld be a float r
-00000370: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
-00000380: 7469 6d65 6f75 7420 7469 6d65 2069 6e20  timeout time in 
-00000390: 7365 636f 6e64 732e 0a23 5441 4250 595f  seconds..#TABPY_
-000003a0: 4556 414c 5541 5445 5f54 494d 454f 5554  EVALUATE_TIMEOUT
-000003b0: 203d 2033 300a 0a5b 6c6f 6767 6572 735d   = 30..[loggers]
-000003c0: 0a6b 6579 733d 726f 6f74 0a0a 5b68 616e  .keys=root..[han
-000003d0: 646c 6572 735d 0a6b 6579 733d 726f 6f74  dlers].keys=root
-000003e0: 4861 6e64 6c65 722c 726f 7461 7469 6e67  Handler,rotating
-000003f0: 4669 6c65 4861 6e64 6c65 720a 0a5b 666f  FileHandler..[fo
-00000400: 726d 6174 7465 7273 5d0a 6b65 7973 3d72  rmatters].keys=r
-00000410: 6f6f 7446 6f72 6d61 7474 6572 0a0a 5b6c  ootFormatter..[l
-00000420: 6f67 6765 725f 726f 6f74 5d0a 6c65 7665  ogger_root].leve
-00000430: 6c3d 4445 4255 470a 6861 6e64 6c65 7273  l=DEBUG.handlers
-00000440: 3d72 6f6f 7448 616e 646c 6572 2c72 6f74  =rootHandler,rot
-00000450: 6174 696e 6746 696c 6548 616e 646c 6572  atingFileHandler
-00000460: 0a71 7561 6c6e 616d 653d 726f 6f74 0a70  .qualname=root.p
-00000470: 726f 7061 6765 7465 3d30 0a0a 5b68 616e  ropagete=0..[han
-00000480: 646c 6572 5f72 6f6f 7448 616e 646c 6572  dler_rootHandler
-00000490: 5d0a 636c 6173 733d 5374 7265 616d 4861  ].class=StreamHa
-000004a0: 6e64 6c65 720a 6c65 7665 6c3d 4445 4255  ndler.level=DEBU
-000004b0: 470a 666f 726d 6174 7465 723d 726f 6f74  G.formatter=root
-000004c0: 466f 726d 6174 7465 720a 6172 6773 3d28  Formatter.args=(
-000004d0: 7379 732e 7374 646f 7574 2c29 0a0a 5b68  sys.stdout,)..[h
-000004e0: 616e 646c 6572 5f72 6f74 6174 696e 6746  andler_rotatingF
-000004f0: 696c 6548 616e 646c 6572 5d0a 636c 6173  ileHandler].clas
-00000500: 733d 6861 6e64 6c65 7273 2e52 6f74 6174  s=handlers.Rotat
-00000510: 696e 6746 696c 6548 616e 646c 6572 0a6c  ingFileHandler.l
-00000520: 6576 656c 3d44 4542 5547 0a66 6f72 6d61  evel=DEBUG.forma
-00000530: 7474 6572 3d72 6f6f 7446 6f72 6d61 7474  tter=rootFormatt
-00000540: 6572 0a61 7267 733d 2827 7461 6270 795f  er.args=('tabpy_
-00000550: 6c6f 672e 6c6f 6727 2c20 2761 272c 2031  log.log', 'a', 1
-00000560: 3030 3030 3030 2c20 3529 0a0a 5b66 6f72  000000, 5)..[for
-00000570: 6d61 7474 6572 5f72 6f6f 7446 6f72 6d61  matter_rootForma
-00000580: 7474 6572 5d0a 666f 726d 6174 3d25 2861  tter].format=%(a
-00000590: 7363 7469 6d65 2973 205b 2528 6c65 7665  sctime)s [%(leve
-000005a0: 6c6e 616d 6529 735d 2028 2528 6669 6c65  lname)s] (%(file
-000005b0: 6e61 6d65 2973 3a25 286d 6f64 756c 6529  name)s:%(module)
-000005c0: 733a 2528 6c69 6e65 6e6f 2964 293a 2025  s:%(lineno)d): %
-000005d0: 286d 6573 7361 6765 2973 0a64 6174 6566  (message)s.datef
-000005e0: 6d74 3d25 592d 256d 2d25 642c 2548 3a25  mt=%Y-%m-%d,%H:%
-000005f0: 4d3a 2553 0a                             M:%S.
+000001d0: 6520 7375 7070 6f72 7465 642e 0d0a 2320  e supported...# 
+000001e0: 5441 4250 595f 5452 414e 5346 4552 5f50  TABPY_TRANSFER_P
+000001f0: 524f 544f 434f 4c20 3d20 6874 7470 730d  ROTOCOL = https.
+00000200: 0a23 2054 4142 5059 5f43 4552 5449 4649  .# TABPY_CERTIFI
+00000210: 4341 5445 5f46 494c 4520 3d20 7061 7468  CATE_FILE = path
+00000220: 2f74 6f2f 6365 7274 6966 6963 6174 652f  /to/certificate/
+00000230: 6669 6c65 2e63 7274 0d0a 2320 5441 4250  file.crt..# TABP
+00000240: 595f 4b45 595f 4649 4c45 203d 2070 6174  Y_KEY_FILE = pat
+00000250: 682f 746f 2f6b 6579 2f66 696c 652e 6b65  h/to/key/file.ke
+00000260: 790d 0a0d 0a23 204c 6f67 2061 6464 6974  y....# Log addit
+00000270: 696f 6e61 6c20 7265 7175 6573 7420 6465  ional request de
+00000280: 7461 696c 7320 696e 636c 7564 696e 6720  tails including 
+00000290: 6361 6c6c 6572 2049 502c 2066 756c 6c20  caller IP, full 
+000002a0: 5552 4c2c 2063 6c69 656e 740d 0a23 2065  URL, client..# e
+000002b0: 6e64 2075 7365 7220 696e 666f 2069 6620  nd user info if 
+000002c0: 7072 6f76 6964 6564 2e0d 0a23 2054 4142  provided...# TAB
+000002d0: 5059 5f4c 4f47 5f44 4554 4149 4c53 203d  PY_LOG_DETAILS =
+000002e0: 2074 7275 650d 0a0d 0a23 2043 6f6e 6669   true....# Confi
+000002f0: 6775 7265 2068 6f77 206c 6f6e 6720 6120  gure how long a 
+00000300: 6375 7374 6f6d 2073 6372 6970 7420 7072  custom script pr
+00000310: 6f76 6964 6564 2074 6f20 7468 6520 2f65  ovided to the /e
+00000320: 7661 6c75 6174 6520 6d65 7468 6f64 0d0a  valuate method..
+00000330: 2320 7769 6c6c 2072 756e 2062 6566 6f72  # will run befor
+00000340: 6520 7468 726f 7769 6e67 2061 2054 696d  e throwing a Tim
+00000350: 656f 7574 4572 726f 722e 0d0a 2320 5468  eoutError...# Th
+00000360: 6520 7661 6c75 6520 7368 6f75 6c64 2062  e value should b
+00000370: 6520 6120 666c 6f61 7420 7265 7072 6573  e a float repres
+00000380: 656e 7469 6e67 2074 6865 2074 696d 656f  enting the timeo
+00000390: 7574 2074 696d 6520 696e 2073 6563 6f6e  ut time in secon
+000003a0: 6473 2e0d 0a23 5441 4250 595f 4556 414c  ds...#TABPY_EVAL
+000003b0: 5541 5445 5f54 494d 454f 5554 203d 2033  UATE_TIMEOUT = 3
+000003c0: 300d 0a0d 0a5b 6c6f 6767 6572 735d 0d0a  0....[loggers]..
+000003d0: 6b65 7973 3d72 6f6f 740d 0a0d 0a5b 6861  keys=root....[ha
+000003e0: 6e64 6c65 7273 5d0d 0a6b 6579 733d 726f  ndlers]..keys=ro
+000003f0: 6f74 4861 6e64 6c65 722c 726f 7461 7469  otHandler,rotati
+00000400: 6e67 4669 6c65 4861 6e64 6c65 720d 0a0d  ngFileHandler...
+00000410: 0a5b 666f 726d 6174 7465 7273 5d0d 0a6b  .[formatters]..k
+00000420: 6579 733d 726f 6f74 466f 726d 6174 7465  eys=rootFormatte
+00000430: 720d 0a0d 0a5b 6c6f 6767 6572 5f72 6f6f  r....[logger_roo
+00000440: 745d 0d0a 6c65 7665 6c3d 4445 4255 470d  t]..level=DEBUG.
+00000450: 0a68 616e 646c 6572 733d 726f 6f74 4861  .handlers=rootHa
+00000460: 6e64 6c65 722c 726f 7461 7469 6e67 4669  ndler,rotatingFi
+00000470: 6c65 4861 6e64 6c65 720d 0a71 7561 6c6e  leHandler..qualn
+00000480: 616d 653d 726f 6f74 0d0a 7072 6f70 6167  ame=root..propag
+00000490: 6574 653d 300d 0a0d 0a5b 6861 6e64 6c65  ete=0....[handle
+000004a0: 725f 726f 6f74 4861 6e64 6c65 725d 0d0a  r_rootHandler]..
+000004b0: 636c 6173 733d 5374 7265 616d 4861 6e64  class=StreamHand
+000004c0: 6c65 720d 0a6c 6576 656c 3d44 4542 5547  ler..level=DEBUG
+000004d0: 0d0a 666f 726d 6174 7465 723d 726f 6f74  ..formatter=root
+000004e0: 466f 726d 6174 7465 720d 0a61 7267 733d  Formatter..args=
+000004f0: 2873 7973 2e73 7464 6f75 742c 290d 0a0d  (sys.stdout,)...
+00000500: 0a5b 6861 6e64 6c65 725f 726f 7461 7469  .[handler_rotati
+00000510: 6e67 4669 6c65 4861 6e64 6c65 725d 0d0a  ngFileHandler]..
+00000520: 636c 6173 733d 6861 6e64 6c65 7273 2e52  class=handlers.R
+00000530: 6f74 6174 696e 6746 696c 6548 616e 646c  otatingFileHandl
+00000540: 6572 0d0a 6c65 7665 6c3d 4445 4255 470d  er..level=DEBUG.
+00000550: 0a66 6f72 6d61 7474 6572 3d72 6f6f 7446  .formatter=rootF
+00000560: 6f72 6d61 7474 6572 0d0a 6172 6773 3d28  ormatter..args=(
+00000570: 2774 6162 7079 5f6c 6f67 2e6c 6f67 272c  'tabpy_log.log',
+00000580: 2027 6127 2c20 3130 3030 3030 302c 2035   'a', 1000000, 5
+00000590: 290d 0a0d 0a5b 666f 726d 6174 7465 725f  )....[formatter_
+000005a0: 726f 6f74 466f 726d 6174 7465 725d 0d0a  rootFormatter]..
+000005b0: 666f 726d 6174 3d25 2861 7363 7469 6d65  format=%(asctime
+000005c0: 2973 205b 2528 6c65 7665 6c6e 616d 6529  )s [%(levelname)
+000005d0: 735d 2028 2528 6669 6c65 6e61 6d65 2973  s] (%(filename)s
+000005e0: 3a25 286d 6f64 756c 6529 733a 2528 6c69  :%(module)s:%(li
+000005f0: 6e65 6e6f 2964 293a 2025 286d 6573 7361  neno)d): %(messa
+00000600: 6765 2973 0d0a 6461 7465 666d 743d 2559  ge)s..datefmt=%Y
+00000610: 2d25 6d2d 2564 2c25 483a 254d 3a25 530d  -%m-%d,%H:%M:%S.
+00000620: 0a                                       .
```

### Comparing `tabpy-2.6.0/tests/integration/test_auth.py` & `tabpy-2.7.0/tests/integration/test_auth.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/tests/integration/test_custom_evaluate_timeout.py` & `tabpy-2.7.0/tests/integration/test_custom_evaluate_timeout.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from . import integ_test_base
-
-
-class TestCustomEvaluateTimeout(integ_test_base.IntegTestBase):
-    def _get_evaluate_timeout(self) -> str:
-        return "3"
-
-    def test_custom_evaluate_timeout_with_script(self):
-        # Uncomment the following line to preserve
-        # test case output and other files (config, state, ect.)
-        # in system temp folder.
-        self.set_delete_temp_folder(False)
-
-        payload = """
-            {
-                "data": { "_arg1": 1 },
-                "script":
-                "import time\\ntime.sleep(100)\\nreturn 1"
-            }
-            """
-        headers = {
-            "Content-Type": "application/json",
-            "TabPy-Client": "Integration test for testing custom evaluate timeouts "
-            "with scripts.",
-        }
-
-        conn = self._get_connection()
-        conn.request("POST", "/evaluate", payload, headers)
-        res = conn.getresponse()
-        actual_error_message = res.read().decode("utf-8")
-
-        self.assertEqual(408, res.status)
-        self.assertEqual(
-            '{"message": '
-            '"User defined script timed out. Timeout is set to 3.0 s.", '
-            '"info": {}}',
-            actual_error_message,
-        )
+from . import integ_test_base
+
+
+class TestCustomEvaluateTimeout(integ_test_base.IntegTestBase):
+    def _get_evaluate_timeout(self) -> str:
+        return "3"
+
+    def test_custom_evaluate_timeout_with_script(self):
+        # Uncomment the following line to preserve
+        # test case output and other files (config, state, ect.)
+        # in system temp folder.
+        self.set_delete_temp_folder(False)
+
+        payload = """
+            {
+                "data": { "_arg1": 1 },
+                "script":
+                "import time\\ntime.sleep(100)\\nreturn 1"
+            }
+            """
+        headers = {
+            "Content-Type": "application/json",
+            "TabPy-Client": "Integration test for testing custom evaluate timeouts "
+            "with scripts.",
+        }
+
+        conn = self._get_connection()
+        conn.request("POST", "/evaluate", payload, headers)
+        res = conn.getresponse()
+        actual_error_message = res.read().decode("utf-8")
+
+        self.assertEqual(408, res.status)
+        self.assertEqual(
+            '{"message": '
+            '"User defined script timed out. Timeout is set to 3.0 s.", '
+            '"info": {}}',
+            actual_error_message,
+        )
```

### Comparing `tabpy-2.6.0/tests/integration/test_deploy_and_evaluate_model.py` & `tabpy-2.7.0/tests/integration/test_deploy_and_evaluate_model.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from . import integ_test_base
-
-
-class TestDeployAndEvaluateModel(integ_test_base.IntegTestBase):
-    def _get_config_file_name(self) -> str:
-        return "./tests/integration/resources/deploy_and_evaluate_model.conf"
-
-    def _get_port(self) -> str:
-        return "9008"
-
-    def test_deploy_and_evaluate_model(self):
-        # Uncomment the following line to preserve
-        # test case output and other files (config, state, ect.)
-        # in system temp folder.
-        # self.set_delete_temp_folder(False)
-
-        self.deploy_models(self._get_username(), self._get_password())
-
-        payload = """{
-                "data": { "_arg1": ["happy", "sad", "neutral"] },
-                "script":
-                "return tabpy.query('Sentiment Analysis',_arg1)['response']"
-            }"""
-
-        conn = self._get_connection()
-        conn.request("POST", "/evaluate", payload)
-        SentimentAnalysis_eval = conn.getresponse()
-        self.assertEqual(200, SentimentAnalysis_eval.status)
-        SentimentAnalysis_eval.read()
+from . import integ_test_base
+
+
+class TestDeployAndEvaluateModel(integ_test_base.IntegTestBase):
+    def _get_config_file_name(self) -> str:
+        return "./tests/integration/resources/deploy_and_evaluate_model.conf"
+
+    def _get_port(self) -> str:
+        return "9008"
+
+    def test_deploy_and_evaluate_model(self):
+        # Uncomment the following line to preserve
+        # test case output and other files (config, state, ect.)
+        # in system temp folder.
+        # self.set_delete_temp_folder(False)
+
+        self.deploy_models(self._get_username(), self._get_password())
+
+        payload = """{
+                "data": { "_arg1": ["happy", "sad", "neutral"] },
+                "script":
+                "return tabpy.query('Sentiment Analysis',_arg1)['response']"
+            }"""
+
+        conn = self._get_connection()
+        conn.request("POST", "/evaluate", payload)
+        SentimentAnalysis_eval = conn.getresponse()
+        self.assertEqual(200, SentimentAnalysis_eval.status)
+        SentimentAnalysis_eval.read()
```

### Comparing `tabpy-2.6.0/tests/integration/test_deploy_and_evaluate_model_auth_on.py` & `tabpy-2.7.0/tests/integration/test_deploy_and_evaluate_model_auth_on.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from . import integ_test_base
-
-
-class TestDeployAndEvaluateModelAuthOn(integ_test_base.IntegTestBase):
-    def _get_config_file_name(self) -> str:
-        return "./tests/integration/resources/deploy_and_evaluate_model_auth.conf"
-
-    def _get_port(self) -> str:
-        return "9009"
-
-    def test_deploy_and_evaluate_model(self):
-        # Uncomment the following line to preserve
-        # test case output and other files (config, state, ect.)
-        # in system temp folder.
-        # self.set_delete_temp_folder(False)
-
-        self.deploy_models(self._get_username(), self._get_password())
-
-        headers = {
-            "Content-Type": "application/json",
-            "Authorization": "Basic dXNlcjE6UEBzc3cwcmQ=",
-            "Host": "localhost:9009",
-        }
-        payload = """{
-                "data": { "_arg1": ["happy", "sad", "neutral"] },
-                "script":
-                "return tabpy.query('Sentiment Analysis',_arg1)['response']"
-            }"""
-
-        conn = self._get_connection()
-        conn.request("POST", "/evaluate", payload, headers)
-        SentimentAnalysis_eval = conn.getresponse()
-        self.assertEqual(200, SentimentAnalysis_eval.status)
-        SentimentAnalysis_eval.read()
+from . import integ_test_base
+
+
+class TestDeployAndEvaluateModelAuthOn(integ_test_base.IntegTestBase):
+    def _get_config_file_name(self) -> str:
+        return "./tests/integration/resources/deploy_and_evaluate_model_auth.conf"
+
+    def _get_port(self) -> str:
+        return "9009"
+
+    def test_deploy_and_evaluate_model(self):
+        # Uncomment the following line to preserve
+        # test case output and other files (config, state, ect.)
+        # in system temp folder.
+        # self.set_delete_temp_folder(False)
+
+        self.deploy_models(self._get_username(), self._get_password())
+
+        headers = {
+            "Content-Type": "application/json",
+            "Authorization": "Basic dXNlcjE6UEBzc3cwcmQ=",
+            "Host": "localhost:9009",
+        }
+        payload = """{
+                "data": { "_arg1": ["happy", "sad", "neutral"] },
+                "script":
+                "return tabpy.query('Sentiment Analysis',_arg1)['response']"
+            }"""
+
+        conn = self._get_connection()
+        conn.request("POST", "/evaluate", payload, headers)
+        SentimentAnalysis_eval = conn.getresponse()
+        self.assertEqual(200, SentimentAnalysis_eval.status)
+        SentimentAnalysis_eval.read()
```

### Comparing `tabpy-2.6.0/tests/integration/test_deploy_model_ssl_off_auth_off.py` & `tabpy-2.7.0/tests/integration/test_deploy_model_ssl_off_auth_off.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from . import integ_test_base
-
-
-class TestDeployModelSSLOffAuthOff(integ_test_base.IntegTestBase):
-    def test_deploy_ssl_off_auth_off(self):
-        # Uncomment the following line to preserve
-        # test case output and other files (config, state, ect.)
-        # in system temp folder.
-        # self.set_delete_temp_folder(False)
-
-        self.deploy_models(self._get_username(), self._get_password())
-
-        conn = self._get_connection()
-
-        models = ["PCA", "Sentiment%20Analysis", "ttest", "anova"]
-        for m in models:
-            conn.request("GET", f"/endpoints/{m}")
-            m_request = conn.getresponse()
-            self.assertEqual(200, m_request.status)
-            m_request.read()
+from . import integ_test_base
+
+
+class TestDeployModelSSLOffAuthOff(integ_test_base.IntegTestBase):
+    def test_deploy_ssl_off_auth_off(self):
+        # Uncomment the following line to preserve
+        # test case output and other files (config, state, ect.)
+        # in system temp folder.
+        # self.set_delete_temp_folder(False)
+
+        self.deploy_models(self._get_username(), self._get_password())
+
+        conn = self._get_connection()
+
+        models = ["PCA", "Sentiment%20Analysis", "ttest", "anova"]
+        for m in models:
+            conn.request("GET", f"/endpoints/{m}")
+            m_request = conn.getresponse()
+            self.assertEqual(200, m_request.status)
+            m_request.read()
```

### Comparing `tabpy-2.6.0/tests/integration/test_deploy_model_ssl_off_auth_on.py` & `tabpy-2.7.0/tests/integration/test_deploy_model_ssl_off_auth_on.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from . import integ_test_base
-import base64
-
-
-class TestDeployModelSSLOffAuthOn(integ_test_base.IntegTestBase):
-    def _get_pwd_file(self) -> str:
-        return "./tests/integration/resources/pwdfile.txt"
-
-    def test_deploy_ssl_off_auth_on(self):
-        self.deploy_models(self._get_username(), self._get_password())
-
-        headers = {
-            "Content-Type": "application/json",
-            "TabPy-Client": "Integration test for deploying models with auth",
-            "Authorization": "Basic "
-            + base64.b64encode("user1:P@ssw0rd".encode("utf-8")).decode("utf-8"),
-        }
-
-        conn = self._get_connection()
-
-        models = ["PCA", "Sentiment%20Analysis", "ttest", "anova"]
-        for m in models:
-            conn.request("GET", f"/endpoints/{m}", headers=headers)
-            m_request = conn.getresponse()
-            self.assertEqual(200, m_request.status)
-            m_request.read()
+from . import integ_test_base
+import base64
+
+
+class TestDeployModelSSLOffAuthOn(integ_test_base.IntegTestBase):
+    def _get_pwd_file(self) -> str:
+        return "./tests/integration/resources/pwdfile.txt"
+
+    def test_deploy_ssl_off_auth_on(self):
+        self.deploy_models(self._get_username(), self._get_password())
+
+        headers = {
+            "Content-Type": "application/json",
+            "TabPy-Client": "Integration test for deploying models with auth",
+            "Authorization": "Basic "
+            + base64.b64encode("user1:P@ssw0rd".encode("utf-8")).decode("utf-8"),
+        }
+
+        conn = self._get_connection()
+
+        models = ["PCA", "Sentiment%20Analysis", "ttest", "anova"]
+        for m in models:
+            conn.request("GET", f"/endpoints/{m}", headers=headers)
+            m_request = conn.getresponse()
+            self.assertEqual(200, m_request.status)
+            m_request.read()
```

### Comparing `tabpy-2.6.0/tests/integration/test_deploy_model_ssl_on_auth_on.py` & `tabpy-2.7.0/tests/integration/test_deploy_model_ssl_on_auth_on.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-from . import integ_test_base
-import base64
-import requests
-
-
-class TestDeployModelSSLOnAuthOn(integ_test_base.IntegTestBase):
-    def _get_transfer_protocol(self) -> str:
-        return "https"
-
-    def _get_certificate_file_name(self) -> str:
-        return "./tests/integration/resources/2019_04_24_to_3018_08_25.crt"
-
-    def _get_key_file_name(self) -> str:
-        return "./tests/integration/resources/2019_04_24_to_3018_08_25.key"
-
-    def _get_pwd_file(self) -> str:
-        return "./tests/integration/resources/pwdfile.txt"
-
-    def test_deploy_ssl_on_auth_on(self):
-        # Uncomment the following line to preserve
-        # test case output and other files (config, state, ect.)
-        # in system temp folder.
-        # self.set_delete_temp_folder(False)
-
-        self.deploy_models(self._get_username(), self._get_password())
-
-        headers = {
-            "Content-Type": "application/json",
-            "TabPy-Client": "Integration test for deploying models with auth",
-            "Authorization": "Basic "
-            + base64.b64encode("user1:P@ssw0rd".encode("utf-8")).decode("utf-8"),
-        }
-
-        session = requests.Session()
-        # Do not verify servers' cert to be signed by trusted CA
-        session.verify = False
-        # Do not warn about insecure request
-        requests.packages.urllib3.disable_warnings()
-
-        models = ["PCA", "Sentiment%20Analysis", "ttest", "anova"]
-        for m in models:
-            m_response = session.get(
-                url=f"{self._get_transfer_protocol()}://"
-                f"localhost:9004/endpoints/{m}",
-                headers=headers,
-            )
-            self.assertEqual(200, m_response.status_code)
-
-    def test_override_model_ssl_on_auth_on(self):
-        # Uncomment the following line to preserve
-        # test case output and other files (config, state, ect.)
-        # in system temp folder.
-        # self.set_delete_temp_folder(False)
-
-        self.deploy_models(self._get_username(), self._get_password())
-
-        # Override models
-        self.deploy_models(self._get_username(), self._get_password())
-
-        headers = {
-            "Content-Type": "application/json",
-            "TabPy-Client": "Integration test for deploying models with auth",
-            "Authorization": "Basic "
-            + base64.b64encode("user1:P@ssw0rd".encode("utf-8")).decode("utf-8"),
-        }
-
-        session = requests.Session()
-        # Do not verify servers' cert to be signed by trusted CA
-        session.verify = False
-        # Do not warn about insecure request
-        requests.packages.urllib3.disable_warnings()
-
-        models = ["PCA", "Sentiment%20Analysis", "ttest", "anova"]
-        for m in models:
-            m_response = session.get(
-                url=f"{self._get_transfer_protocol()}://"
-                f"localhost:9004/endpoints/{m}",
-                headers=headers,
-            )
-            self.assertEqual(200, m_response.status_code)
+from . import integ_test_base
+import base64
+import requests
+
+
+class TestDeployModelSSLOnAuthOn(integ_test_base.IntegTestBase):
+    def _get_transfer_protocol(self) -> str:
+        return "https"
+
+    def _get_certificate_file_name(self) -> str:
+        return "./tests/integration/resources/2019_04_24_to_3018_08_25.crt"
+
+    def _get_key_file_name(self) -> str:
+        return "./tests/integration/resources/2019_04_24_to_3018_08_25.key"
+
+    def _get_pwd_file(self) -> str:
+        return "./tests/integration/resources/pwdfile.txt"
+
+    def test_deploy_ssl_on_auth_on(self):
+        # Uncomment the following line to preserve
+        # test case output and other files (config, state, ect.)
+        # in system temp folder.
+        # self.set_delete_temp_folder(False)
+
+        self.deploy_models(self._get_username(), self._get_password())
+
+        headers = {
+            "Content-Type": "application/json",
+            "TabPy-Client": "Integration test for deploying models with auth",
+            "Authorization": "Basic "
+            + base64.b64encode("user1:P@ssw0rd".encode("utf-8")).decode("utf-8"),
+        }
+
+        session = requests.Session()
+        # Do not verify servers' cert to be signed by trusted CA
+        session.verify = False
+        # Do not warn about insecure request
+        requests.packages.urllib3.disable_warnings()
+
+        models = ["PCA", "Sentiment%20Analysis", "ttest", "anova"]
+        for m in models:
+            m_response = session.get(
+                url=f"{self._get_transfer_protocol()}://"
+                f"localhost:9004/endpoints/{m}",
+                headers=headers,
+            )
+            self.assertEqual(200, m_response.status_code)
+
+    def test_override_model_ssl_on_auth_on(self):
+        # Uncomment the following line to preserve
+        # test case output and other files (config, state, ect.)
+        # in system temp folder.
+        # self.set_delete_temp_folder(False)
+
+        self.deploy_models(self._get_username(), self._get_password())
+
+        # Override models
+        self.deploy_models(self._get_username(), self._get_password())
+
+        headers = {
+            "Content-Type": "application/json",
+            "TabPy-Client": "Integration test for deploying models with auth",
+            "Authorization": "Basic "
+            + base64.b64encode("user1:P@ssw0rd".encode("utf-8")).decode("utf-8"),
+        }
+
+        session = requests.Session()
+        # Do not verify servers' cert to be signed by trusted CA
+        session.verify = False
+        # Do not warn about insecure request
+        requests.packages.urllib3.disable_warnings()
+
+        models = ["PCA", "Sentiment%20Analysis", "ttest", "anova"]
+        for m in models:
+            m_response = session.get(
+                url=f"{self._get_transfer_protocol()}://"
+                f"localhost:9004/endpoints/{m}",
+                headers=headers,
+            )
+            self.assertEqual(200, m_response.status_code)
```

### Comparing `tabpy-2.6.0/tests/integration/test_evaluate.py` & `tabpy-2.7.0/tests/integration/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/tests/integration/test_gzip.py` & `tabpy-2.7.0/tests/integration/test_gzip.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-"""
-Script evaluation tests.
-"""
-
-from . import integ_test_base
-import json
-import gzip
-import os
-import requests
-
-
-class TestEvaluate(integ_test_base.IntegTestBase):
-    def _get_config_file_name(self) -> str:
-        """
-        Generates config file. Overwrite this function for tests to
-        run against not default state file.
-
-        Returns
-        -------
-        str
-            Absolute path to config file.
-        """
-        config_file = open(os.path.join(self.tmp_dir, "test.conf"), "w+")
-        config_file.write(
-            "[TabPy]\n"
-            f"TABPY_QUERY_OBJECT_PATH = {self.tmp_dir}/query_objects\n"
-            f"TABPY_PORT = {self._get_port()}\n"
-            f"TABPY_GZIP_ENABLE = TRUE\n"
-            f"TABPY_STATE_PATH = {self.tmp_dir}\n"
-        )
-
-        pwd_file = self._get_pwd_file()
-        if pwd_file is not None:
-            pwd_file = os.path.abspath(pwd_file)
-            config_file.write(f"TABPY_PWD_FILE = {pwd_file}\n")
-
-        transfer_protocol = self._get_transfer_protocol()
-        if transfer_protocol is not None:
-            config_file.write(f"TABPY_TRANSFER_PROTOCOL = {transfer_protocol}\n")
-
-        cert_file_name = self._get_certificate_file_name()
-        if cert_file_name is not None:
-            cert_file_name = os.path.abspath(cert_file_name)
-            config_file.write(f"TABPY_CERTIFICATE_FILE = {cert_file_name}\n")
-
-        key_file_name = self._get_key_file_name()
-        if key_file_name is not None:
-            key_file_name = os.path.abspath(key_file_name)
-            config_file.write(f"TABPY_KEY_FILE = {key_file_name}\n")
-
-        evaluate_timeout = self._get_evaluate_timeout()
-        if evaluate_timeout is not None:
-            config_file.write(f"TABPY_EVALUATE_TIMEOUT = {evaluate_timeout}\n")
-
-        config_file.close()
-
-        self.delete_config_file = True
-        return config_file.name
-
-    def test_single_value_returned(self):
-        payload = """
-            {
-                "data": { "_arg1": 2, "_arg2": 40 },
-                "script":
-                "return _arg1 + _arg2"
-            }
-            """
-        headers = {
-            "Content-Type": "application/json",
-            "Content-Encoding": "gzip",
-        }
-
-        url = self._get_url() + "/evaluate"
-        response = requests.request("POST", url, data=gzip.compress(payload.encode('utf-8')),
-            headers=headers)
-        result = json.loads(response.text)
-
-        self.assertEqual(200, response.status_code)
-        self.assertEqual(42, result)
-
-    def test_syntax_error(self):
-        payload = """
-            {
-                "data": { "_arg1": [2], "_arg2": [40] },
-                "script":
-                "% ^ !! return Nothing"
-            }
-            """
-        headers = {
-            "Content-Type": "application/json",
-            "Content-Encoding": "gzip",
-        }
-
-        url = self._get_url() + "/evaluate"
-        response = requests.request("POST", url, data=gzip.compress(payload.encode('utf-8')),
-            headers=headers)
-        result = json.loads(response.text)
-
-        self.assertEqual(500, response.status_code)
-        self.assertEqual("Error processing script", result["message"])
-        self.assertTrue(result["info"].startswith("SyntaxError"))
+"""
+Script evaluation tests.
+"""
+
+from . import integ_test_base
+import json
+import gzip
+import os
+import requests
+
+
+class TestEvaluate(integ_test_base.IntegTestBase):
+    def _get_config_file_name(self) -> str:
+        """
+        Generates config file. Overwrite this function for tests to
+        run against not default state file.
+
+        Returns
+        -------
+        str
+            Absolute path to config file.
+        """
+        config_file = open(os.path.join(self.tmp_dir, "test.conf"), "w+")
+        config_file.write(
+            "[TabPy]\n"
+            f"TABPY_QUERY_OBJECT_PATH = {self.tmp_dir}/query_objects\n"
+            f"TABPY_PORT = {self._get_port()}\n"
+            f"TABPY_GZIP_ENABLE = TRUE\n"
+            f"TABPY_STATE_PATH = {self.tmp_dir}\n"
+        )
+
+        pwd_file = self._get_pwd_file()
+        if pwd_file is not None:
+            pwd_file = os.path.abspath(pwd_file)
+            config_file.write(f"TABPY_PWD_FILE = {pwd_file}\n")
+
+        transfer_protocol = self._get_transfer_protocol()
+        if transfer_protocol is not None:
+            config_file.write(f"TABPY_TRANSFER_PROTOCOL = {transfer_protocol}\n")
+
+        cert_file_name = self._get_certificate_file_name()
+        if cert_file_name is not None:
+            cert_file_name = os.path.abspath(cert_file_name)
+            config_file.write(f"TABPY_CERTIFICATE_FILE = {cert_file_name}\n")
+
+        key_file_name = self._get_key_file_name()
+        if key_file_name is not None:
+            key_file_name = os.path.abspath(key_file_name)
+            config_file.write(f"TABPY_KEY_FILE = {key_file_name}\n")
+
+        evaluate_timeout = self._get_evaluate_timeout()
+        if evaluate_timeout is not None:
+            config_file.write(f"TABPY_EVALUATE_TIMEOUT = {evaluate_timeout}\n")
+
+        config_file.close()
+
+        self.delete_config_file = True
+        return config_file.name
+
+    def test_single_value_returned(self):
+        payload = """
+            {
+                "data": { "_arg1": 2, "_arg2": 40 },
+                "script":
+                "return _arg1 + _arg2"
+            }
+            """
+        headers = {
+            "Content-Type": "application/json",
+            "Content-Encoding": "gzip",
+        }
+
+        url = self._get_url() + "/evaluate"
+        response = requests.request("POST", url, data=gzip.compress(payload.encode('utf-8')),
+            headers=headers)
+        result = json.loads(response.text)
+
+        self.assertEqual(200, response.status_code)
+        self.assertEqual(42, result)
+
+    def test_syntax_error(self):
+        payload = """
+            {
+                "data": { "_arg1": [2], "_arg2": [40] },
+                "script":
+                "% ^ !! return Nothing"
+            }
+            """
+        headers = {
+            "Content-Type": "application/json",
+            "Content-Encoding": "gzip",
+        }
+
+        url = self._get_url() + "/evaluate"
+        response = requests.request("POST", url, data=gzip.compress(payload.encode('utf-8')),
+            headers=headers)
+        result = json.loads(response.text)
+
+        self.assertEqual(500, response.status_code)
+        self.assertEqual("Error processing script", result["message"])
+        self.assertTrue(result["info"].startswith("SyntaxError"))
```

### Comparing `tabpy-2.6.0/tests/integration/test_url.py` & `tabpy-2.7.0/tests/integration/test_url.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/tests/integration/test_url_ssl.py` & `tabpy-2.7.0/tests/integration/test_url_ssl.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/tests/unit/server_tests/resources/expired.crt` & `tabpy-2.7.0/tests/unit/server_tests/resources/expired.crt`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 00000000: 2d2d 2d2d 2d42 4547 494e 2043 4552 5449  -----BEGIN CERTI
-00000010: 4649 4341 5445 2d2d 2d2d 2d0a 4d49 4942  FICATE-----.MIIB
-00000020: 2b54 4343 4157 4943 4351 4379 7736 7050  +TCCAWICCQCyw6pP
-00000030: 5366 7978 4d54 414e 4267 6b71 686b 6947  SfyxMTANBgkqhkiG
-00000040: 3977 3042 4151 7346 4144 4242 4d51 7377  9w0BAQsFADBBMQsw
-00000050: 4351 5944 5651 5147 4577 4a56 0a55 7a45  CQYDVQQGEwJV.UzE
-00000060: 4c4d 416b 4741 3155 4543 4177 4356 4667  LMAkGA1UECAwCVFg
-00000070: 7843 7a41 4a42 674e 5642 4163 4d41 6b46  xCzAJBgNVBAcMAkF
-00000080: 424d 5173 7743 5159 4456 5151 4b44 414a  BMQswCQYDVQQKDAJ
-00000090: 4251 5445 4c4d 416b 4741 3155 450a 4377  BQTELMAkGA1UE.Cw
-000000a0: 7743 5155 4577 4868 634e 4d54 6777 4f44  wCQUEwHhcNMTgwOD
-000000b0: 4533 4d54 6b30 4e7a 4534 5768 634e 4d54  E3MTk0NzE4WhcNMT
-000000c0: 6777 4f44 4534 4d54 6b30 4e7a 4534 576a  gwODE4MTk0NzE4Wj
-000000d0: 4242 4d51 7377 4351 5944 5651 5147 0a45  BBMQswCQYDVQQG.E
-000000e0: 774a 5655 7a45 4c4d 416b 4741 3155 4543  wJVUzELMAkGA1UEC
-000000f0: 4177 4356 4667 7843 7a41 4a42 674e 5642  AwCVFgxCzAJBgNVB
-00000100: 4163 4d41 6b46 424d 5173 7743 5159 4456  AcMAkFBMQswCQYDV
-00000110: 5151 4b44 414a 4251 5445 4c4d 416b 470a  QQKDAJBQTELMAkG.
-00000120: 4131 5545 4377 7743 5155 4577 675a 3877  A1UECwwCQUEwgZ8w
-00000130: 4451 594a 4b6f 5a49 6876 634e 4151 4542  DQYJKoZIhvcNAQEB
-00000140: 4251 4144 6759 3041 4d49 474a 416f 4742  BQADgY0AMIGJAoGB
-00000150: 414e 3248 5a73 357a 5168 6e38 576b 6d75  AN2HZs5zQhn8Wkmu
-00000160: 0a57 5270 6648 2b7a 6b4e 3753 2f6e 4446  .WRpfH+zkN7S/nDF
-00000170: 5130 6a33 6370 7479 6749 7263 6243 4c32  Q0j3cptygIrcbCL2
-00000180: 6c2f 6363 3343 5a35 5a42 744f 4673 395a  l/cc3CZ5ZBtOFs9Z
-00000190: 4d6f 385a 726c 6954 356c 5539 3453 6c49  Mo8ZrliT5lU94SlI
-000001a0: 480a 6738 5456 5177 3666 5250 614c 3867  H.g8TVQw6fRPaL8g
-000001b0: 4177 4575 7379 7859 7949 532f 6f36 386a  AwEusyxYyIS/o68j
-000001c0: 5858 464b 3143 4370 454a 4466 7034 492f  XXFK1CCpEJDfp4I/
-000001d0: 5a6d 4c58 4269 496d 7148 5632 457a 4e37  ZmLXBiImqHV2EzN7
-000001e0: 7146 0a6b 766d 4f43 6746 4d62 3937 2f33  qF.kvmOCgFMb97/3
-000001f0: 4979 734f 7a44 3451 5567 755a 5431 6441  IysOzD4QUguZT1dA
-00000200: 674d 4241 4145 7744 5159 4a4b 6f5a 4968  gMBAAEwDQYJKoZIh
-00000210: 7663 4e41 5145 4c42 5141 4467 5945 4177  vcNAQELBQADgYEAw
-00000220: 3579 4b0a 4243 6947 6176 6c68 536d 316d  5yK.BCiGavlhSm1m
-00000230: 4845 5456 6f31 584f 6846 3947 7933 3461  HETVo1XOhF9Gy34a
-00000240: 6a33 5054 4f2f 6c57 5873 5750 774c 5759  j3PTO/lWXsWPwLWY
-00000250: 6e4b 4c4f 4531 2f34 6250 3141 6750 732b  nKLOE1/4bP1AgPs+
-00000260: 524e 7178 0a50 4961 7331 796c 5761 4c7a  RNqx.PIas1ylWaLz
-00000270: 7735 4845 3072 2b4a 4b6d 7454 3654 7445  w5HE0r+JKmtT6TtE
-00000280: 7665 4d2b 4742 4f4b 756d 6643 2f77 4668  veM+GBOKumfC/wFh
-00000290: 4c36 4946 7951 424a 6950 4c5a 4b62 5071  L6IFyQBJiPLZKbPq
-000002a0: 5345 6c58 5a0a 6b78 5a64 6e41 704d 636f  SElXZ.kxZdnApMco
-000002b0: 5942 366b 596b 5572 6a63 735a 5a53 6651  YB6kYkUrjcsZZSfQ
-000002c0: 3177 3342 6741 6d73 4d6a 7a51 6b3d 0a2d  1w3BgAmsMjzQk=.-
-000002d0: 2d2d 2d2d 454e 4420 4345 5254 4946 4943  ----END CERTIFIC
-000002e0: 4154 452d 2d2d 2d2d 0a                   ATE-----.
+00000010: 4649 4341 5445 2d2d 2d2d 2d0d 0a4d 4949  FICATE-----..MII
+00000020: 422b 5443 4341 5749 4343 5143 7977 3670  B+TCCAWICCQCyw6p
+00000030: 5053 6679 784d 5441 4e42 676b 7168 6b69  PSfyxMTANBgkqhki
+00000040: 4739 7730 4241 5173 4641 4442 424d 5173  G9w0BAQsFADBBMQs
+00000050: 7743 5159 4456 5151 4745 774a 560d 0a55  wCQYDVQQGEwJV..U
+00000060: 7a45 4c4d 416b 4741 3155 4543 4177 4356  zELMAkGA1UECAwCV
+00000070: 4667 7843 7a41 4a42 674e 5642 4163 4d41  FgxCzAJBgNVBAcMA
+00000080: 6b46 424d 5173 7743 5159 4456 5151 4b44  kFBMQswCQYDVQQKD
+00000090: 414a 4251 5445 4c4d 416b 4741 3155 450d  AJBQTELMAkGA1UE.
+000000a0: 0a43 7777 4351 5545 7748 6863 4e4d 5467  .CwwCQUEwHhcNMTg
+000000b0: 774f 4445 334d 546b 304e 7a45 3457 6863  wODE3MTk0NzE4Whc
+000000c0: 4e4d 5467 774f 4445 344d 546b 304e 7a45  NMTgwODE4MTk0NzE
+000000d0: 3457 6a42 424d 5173 7743 5159 4456 5151  4WjBBMQswCQYDVQQ
+000000e0: 470d 0a45 774a 5655 7a45 4c4d 416b 4741  G..EwJVUzELMAkGA
+000000f0: 3155 4543 4177 4356 4667 7843 7a41 4a42  1UECAwCVFgxCzAJB
+00000100: 674e 5642 4163 4d41 6b46 424d 5173 7743  gNVBAcMAkFBMQswC
+00000110: 5159 4456 5151 4b44 414a 4251 5445 4c4d  QYDVQQKDAJBQTELM
+00000120: 416b 470d 0a41 3155 4543 7777 4351 5545  AkG..A1UECwwCQUE
+00000130: 7767 5a38 7744 5159 4a4b 6f5a 4968 7663  wgZ8wDQYJKoZIhvc
+00000140: 4e41 5145 4242 5141 4467 5930 414d 4947  NAQEBBQADgY0AMIG
+00000150: 4a41 6f47 4241 4e32 485a 7335 7a51 686e  JAoGBAN2HZs5zQhn
+00000160: 3857 6b6d 750d 0a57 5270 6648 2b7a 6b4e  8Wkmu..WRpfH+zkN
+00000170: 3753 2f6e 4446 5130 6a33 6370 7479 6749  7S/nDFQ0j3cptygI
+00000180: 7263 6243 4c32 6c2f 6363 3343 5a35 5a42  rcbCL2l/cc3CZ5ZB
+00000190: 744f 4673 395a 4d6f 385a 726c 6954 356c  tOFs9ZMo8ZrliT5l
+000001a0: 5539 3453 6c49 480d 0a67 3854 5651 7736  U94SlIH..g8TVQw6
+000001b0: 6652 5061 4c38 6741 7745 7573 7978 5979  fRPaL8gAwEusyxYy
+000001c0: 4953 2f6f 3638 6a58 5846 4b31 4343 7045  IS/o68jXXFK1CCpE
+000001d0: 4a44 6670 3449 2f5a 6d4c 5842 6949 6d71  JDfp4I/ZmLXBiImq
+000001e0: 4856 3245 7a4e 3771 460d 0a6b 766d 4f43  HV2EzN7qF..kvmOC
+000001f0: 6746 4d62 3937 2f33 4979 734f 7a44 3451  gFMb97/3IysOzD4Q
+00000200: 5567 755a 5431 6441 674d 4241 4145 7744  UguZT1dAgMBAAEwD
+00000210: 5159 4a4b 6f5a 4968 7663 4e41 5145 4c42  QYJKoZIhvcNAQELB
+00000220: 5141 4467 5945 4177 3579 4b0d 0a42 4369  QADgYEAw5yK..BCi
+00000230: 4761 766c 6853 6d31 6d48 4554 566f 3158  GavlhSm1mHETVo1X
+00000240: 4f68 4639 4779 3334 616a 3350 544f 2f6c  OhF9Gy34aj3PTO/l
+00000250: 5758 7357 5077 4c57 596e 4b4c 4f45 312f  WXsWPwLWYnKLOE1/
+00000260: 3462 5031 4167 5073 2b52 4e71 780d 0a50  4bP1AgPs+RNqx..P
+00000270: 4961 7331 796c 5761 4c7a 7735 4845 3072  Ias1ylWaLzw5HE0r
+00000280: 2b4a 4b6d 7454 3654 7445 7665 4d2b 4742  +JKmtT6TtEveM+GB
+00000290: 4f4b 756d 6643 2f77 4668 4c36 4946 7951  OKumfC/wFhL6IFyQ
+000002a0: 424a 6950 4c5a 4b62 5071 5345 6c58 5a0d  BJiPLZKbPqSElXZ.
+000002b0: 0a6b 785a 646e 4170 4d63 6f59 4236 6b59  .kxZdnApMcoYB6kY
+000002c0: 6b55 726a 6373 5a5a 5366 5131 7733 4267  kUrjcsZZSfQ1w3Bg
+000002d0: 416d 734d 6a7a 516b 3d0d 0a2d 2d2d 2d2d  AmsMjzQk=..-----
+000002e0: 454e 4420 4345 5254 4946 4943 4154 452d  END CERTIFICATE-
+000002f0: 2d2d 2d2d 0d0a                           ----..
```

### Comparing `tabpy-2.6.0/tests/unit/server_tests/resources/future.crt` & `tabpy-2.7.0/tests/unit/server_tests/resources/future.crt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-Certificate:
-    Data:
-        Version: 1 (0x0)
-        Serial Number: 1 (0x1)
-    Signature Algorithm: sha1WithRSAEncryption
-        Issuer: C=UA, ST=Dnipropetrovs'k reg., O=Planet Express, OU=Delivery Crew, CN=Fry\x1B[D\x1B[D\x1B[DH=\x1B[Phillip J. Fry/emailAddress=pfry@planetexpress.com
-        Validity
-            Not Before: Jan  1 00:00:00 3001 GMT
-            Not After : Jan  2 00:00:00 3001 GMT
-        Subject: C=UA, ST=Dnipropetrovs'k reg., O=Planet Express, OU=Delivery Crew, CN=Fry\x1B[D\x1B[D\x1B[DH=\x1B[Phillip J. Fry/emailAddress=pfry@planetexpress.com
-        Subject Public Key Info:
-            Public Key Algorithm: rsaEncryption
-                Public-Key: (2048 bit)
-                Modulus:
-                    00:9b:da:01:8d:b3:c6:71:ed:2a:17:e9:33:f9:f7:
-                    0a:4c:35:1b:25:48:c1:8d:d2:ed:18:e2:51:b1:50:
-                    20:e7:85:24:ca:13:dc:08:41:3d:ab:93:dd:1b:98:
-                    1b:c9:a3:31:46:2c:59:0c:04:15:97:ed:2d:ea:e7:
-                    00:de:bf:31:2f:52:4d:1b:d5:b1:50:32:7c:8e:a7:
-                    a4:1d:c1:e4:fe:35:32:c0:72:4c:38:f4:0b:99:76:
-                    89:2f:f9:32:1d:99:05:ec:b8:b0:46:8f:3e:7a:24:
-                    63:18:a6:01:d3:af:a6:02:3c:1a:67:f6:c2:c5:82:
-                    de:e6:8f:49:4f:02:74:aa:d7:77:2c:63:f1:31:66:
-                    54:a1:d4:79:59:05:5b:01:b8:c5:48:b8:79:d8:38:
-                    cd:30:11:bc:f7:a7:39:d8:14:85:6c:a5:10:8f:80:
-                    08:97:3f:12:bc:85:18:dc:a1:e2:b7:4f:0c:4a:90:
-                    71:32:c5:8b:b4:cf:ae:a3:6c:c6:c6:00:49:49:fb:
-                    34:14:1d:72:4f:2f:0c:3b:53:1a:33:72:ed:69:8b:
-                    51:45:2f:1c:c5:76:71:ca:94:f0:86:a8:d8:fd:dd:
-                    6d:5a:c2:d5:74:69:6e:af:9a:94:66:aa:68:9f:ef:
-                    87:7e:e3:3d:11:40:5c:e8:5f:33:9f:8d:8b:a1:1d:
-                    96:45
-                Exponent: 65537 (0x10001)
-    Signature Algorithm: sha1WithRSAEncryption
-         13:78:d5:41:2b:07:bd:ec:35:90:f4:37:26:6d:e1:2c:e1:2a:
-         61:0b:c8:40:27:31:76:0d:a8:8e:fe:e2:a9:e5:74:fa:14:96:
-         71:fc:b4:3d:ac:dd:44:93:6e:cf:50:35:67:84:db:90:53:3a:
-         2e:47:df:98:5e:cc:c3:c7:7c:24:bf:06:2d:d0:4a:70:30:33:
-         1f:2e:59:5e:40:74:ba:f3:05:c4:25:1d:6e:e2:b2:1c:71:6d:
-         b2:24:e0:8c:ab:c2:00:40:6c:ab:d8:57:84:90:f1:02:24:18:
-         29:9f:4c:b3:30:64:fa:25:5c:12:56:8a:a5:28:20:b2:b5:68:
-         86:4f:60:83:3c:d1:37:32:de:49:89:25:7a:cb:15:e6:54:a2:
-         47:b6:15:36:80:84:fa:61:8a:9c:63:e7:00:76:83:90:fc:90:
-         31:b8:fa:2f:32:45:1d:35:dc:ee:f4:c9:0b:de:9d:33:89:9a:
-         1a:fd:19:e0:63:23:7c:60:70:d6:a9:87:d1:24:24:c4:5f:57:
-         34:69:32:d8:18:fd:9a:25:8c:c6:88:c1:65:1c:3a:9c:6c:e5:
-         86:fb:e7:7f:dd:6e:a5:ac:d1:0e:65:fe:0c:19:12:63:4b:50:
-         d7:ff:5d:cc:9d:0c:10:4a:b5:ad:bc:33:78:d0:84:91:11:04:
-         c1:75:59:98
------BEGIN CERTIFICATE-----
-MIID1DCCArwCAQEwDQYJKoZIhvcNAQEFBQAwga0xCzAJBgNVBAYTAlVBMR0wGwYD
-VQQIDBREbmlwcm9wZXRyb3ZzJ2sgcmVnLjEXMBUGA1UECgwOUGxhbmV0IEV4cHJl
-c3MxFjAUBgNVBAsMDURlbGl2ZXJ5IENyZXcxJzAlBgNVBAMMHkZyeRtbRBtbRBtb
-REg9G1tQaGlsbGlwIEouIEZyeTElMCMGCSqGSIb3DQEJARYWcGZyeUBwbGFuZXRl
-eHByZXNzLmNvbTAiGA8zMDAxMDEwMTAwMDAwMFoYDzMwMDEwMTAyMDAwMDAwWjCB
-rTELMAkGA1UEBhMCVUExHTAbBgNVBAgMFERuaXByb3BldHJvdnMnayByZWcuMRcw
-FQYDVQQKDA5QbGFuZXQgRXhwcmVzczEWMBQGA1UECwwNRGVsaXZlcnkgQ3JldzEn
-MCUGA1UEAwweRnJ5G1tEG1tEG1tESD0bW1BoaWxsaXAgSi4gRnJ5MSUwIwYJKoZI
-hvcNAQkBFhZwZnJ5QHBsYW5ldGV4cHJlc3MuY29tMIIBIjANBgkqhkiG9w0BAQEF
-AAOCAQ8AMIIBCgKCAQEAm9oBjbPGce0qF+kz+fcKTDUbJUjBjdLtGOJRsVAg54Uk
-yhPcCEE9q5PdG5gbyaMxRixZDAQVl+0t6ucA3r8xL1JNG9WxUDJ8jqekHcHk/jUy
-wHJMOPQLmXaJL/kyHZkF7LiwRo8+eiRjGKYB06+mAjwaZ/bCxYLe5o9JTwJ0qtd3
-LGPxMWZUodR5WQVbAbjFSLh52DjNMBG896c52BSFbKUQj4AIlz8SvIUY3KHit08M
-SpBxMsWLtM+uo2zGxgBJSfs0FB1yTy8MO1MaM3LtaYtRRS8cxXZxypTwhqjY/d1t
-WsLVdGlur5qUZqpon++HfuM9EUBc6F8zn42LoR2WRQIDAQABMA0GCSqGSIb3DQEB
-BQUAA4IBAQATeNVBKwe97DWQ9DcmbeEs4SphC8hAJzF2DaiO/uKp5XT6FJZx/LQ9
-rN1Ek27PUDVnhNuQUzouR9+YXszDx3wkvwYt0EpwMDMfLlleQHS68wXEJR1u4rIc
-cW2yJOCMq8IAQGyr2FeEkPECJBgpn0yzMGT6JVwSVoqlKCCytWiGT2CDPNE3Mt5J
-iSV6yxXmVKJHthU2gIT6YYqcY+cAdoOQ/JAxuPovMkUdNdzu9MkL3p0ziZoa/Rng
-YyN8YHDWqYfRJCTEX1c0aTLYGP2aJYzGiMFlHDqcbOWG++d/3W6lrNEOZf4MGRJj
-S1DX/13MnQwQSrWtvDN40ISREQTBdVmY
------END CERTIFICATE-----
+Certificate:
+    Data:
+        Version: 1 (0x0)
+        Serial Number: 1 (0x1)
+    Signature Algorithm: sha1WithRSAEncryption
+        Issuer: C=UA, ST=Dnipropetrovs'k reg., O=Planet Express, OU=Delivery Crew, CN=Fry\x1B[D\x1B[D\x1B[DH=\x1B[Phillip J. Fry/emailAddress=pfry@planetexpress.com
+        Validity
+            Not Before: Jan  1 00:00:00 3001 GMT
+            Not After : Jan  2 00:00:00 3001 GMT
+        Subject: C=UA, ST=Dnipropetrovs'k reg., O=Planet Express, OU=Delivery Crew, CN=Fry\x1B[D\x1B[D\x1B[DH=\x1B[Phillip J. Fry/emailAddress=pfry@planetexpress.com
+        Subject Public Key Info:
+            Public Key Algorithm: rsaEncryption
+                Public-Key: (2048 bit)
+                Modulus:
+                    00:9b:da:01:8d:b3:c6:71:ed:2a:17:e9:33:f9:f7:
+                    0a:4c:35:1b:25:48:c1:8d:d2:ed:18:e2:51:b1:50:
+                    20:e7:85:24:ca:13:dc:08:41:3d:ab:93:dd:1b:98:
+                    1b:c9:a3:31:46:2c:59:0c:04:15:97:ed:2d:ea:e7:
+                    00:de:bf:31:2f:52:4d:1b:d5:b1:50:32:7c:8e:a7:
+                    a4:1d:c1:e4:fe:35:32:c0:72:4c:38:f4:0b:99:76:
+                    89:2f:f9:32:1d:99:05:ec:b8:b0:46:8f:3e:7a:24:
+                    63:18:a6:01:d3:af:a6:02:3c:1a:67:f6:c2:c5:82:
+                    de:e6:8f:49:4f:02:74:aa:d7:77:2c:63:f1:31:66:
+                    54:a1:d4:79:59:05:5b:01:b8:c5:48:b8:79:d8:38:
+                    cd:30:11:bc:f7:a7:39:d8:14:85:6c:a5:10:8f:80:
+                    08:97:3f:12:bc:85:18:dc:a1:e2:b7:4f:0c:4a:90:
+                    71:32:c5:8b:b4:cf:ae:a3:6c:c6:c6:00:49:49:fb:
+                    34:14:1d:72:4f:2f:0c:3b:53:1a:33:72:ed:69:8b:
+                    51:45:2f:1c:c5:76:71:ca:94:f0:86:a8:d8:fd:dd:
+                    6d:5a:c2:d5:74:69:6e:af:9a:94:66:aa:68:9f:ef:
+                    87:7e:e3:3d:11:40:5c:e8:5f:33:9f:8d:8b:a1:1d:
+                    96:45
+                Exponent: 65537 (0x10001)
+    Signature Algorithm: sha1WithRSAEncryption
+         13:78:d5:41:2b:07:bd:ec:35:90:f4:37:26:6d:e1:2c:e1:2a:
+         61:0b:c8:40:27:31:76:0d:a8:8e:fe:e2:a9:e5:74:fa:14:96:
+         71:fc:b4:3d:ac:dd:44:93:6e:cf:50:35:67:84:db:90:53:3a:
+         2e:47:df:98:5e:cc:c3:c7:7c:24:bf:06:2d:d0:4a:70:30:33:
+         1f:2e:59:5e:40:74:ba:f3:05:c4:25:1d:6e:e2:b2:1c:71:6d:
+         b2:24:e0:8c:ab:c2:00:40:6c:ab:d8:57:84:90:f1:02:24:18:
+         29:9f:4c:b3:30:64:fa:25:5c:12:56:8a:a5:28:20:b2:b5:68:
+         86:4f:60:83:3c:d1:37:32:de:49:89:25:7a:cb:15:e6:54:a2:
+         47:b6:15:36:80:84:fa:61:8a:9c:63:e7:00:76:83:90:fc:90:
+         31:b8:fa:2f:32:45:1d:35:dc:ee:f4:c9:0b:de:9d:33:89:9a:
+         1a:fd:19:e0:63:23:7c:60:70:d6:a9:87:d1:24:24:c4:5f:57:
+         34:69:32:d8:18:fd:9a:25:8c:c6:88:c1:65:1c:3a:9c:6c:e5:
+         86:fb:e7:7f:dd:6e:a5:ac:d1:0e:65:fe:0c:19:12:63:4b:50:
+         d7:ff:5d:cc:9d:0c:10:4a:b5:ad:bc:33:78:d0:84:91:11:04:
+         c1:75:59:98
+-----BEGIN CERTIFICATE-----
+MIID1DCCArwCAQEwDQYJKoZIhvcNAQEFBQAwga0xCzAJBgNVBAYTAlVBMR0wGwYD
+VQQIDBREbmlwcm9wZXRyb3ZzJ2sgcmVnLjEXMBUGA1UECgwOUGxhbmV0IEV4cHJl
+c3MxFjAUBgNVBAsMDURlbGl2ZXJ5IENyZXcxJzAlBgNVBAMMHkZyeRtbRBtbRBtb
+REg9G1tQaGlsbGlwIEouIEZyeTElMCMGCSqGSIb3DQEJARYWcGZyeUBwbGFuZXRl
+eHByZXNzLmNvbTAiGA8zMDAxMDEwMTAwMDAwMFoYDzMwMDEwMTAyMDAwMDAwWjCB
+rTELMAkGA1UEBhMCVUExHTAbBgNVBAgMFERuaXByb3BldHJvdnMnayByZWcuMRcw
+FQYDVQQKDA5QbGFuZXQgRXhwcmVzczEWMBQGA1UECwwNRGVsaXZlcnkgQ3JldzEn
+MCUGA1UEAwweRnJ5G1tEG1tEG1tESD0bW1BoaWxsaXAgSi4gRnJ5MSUwIwYJKoZI
+hvcNAQkBFhZwZnJ5QHBsYW5ldGV4cHJlc3MuY29tMIIBIjANBgkqhkiG9w0BAQEF
+AAOCAQ8AMIIBCgKCAQEAm9oBjbPGce0qF+kz+fcKTDUbJUjBjdLtGOJRsVAg54Uk
+yhPcCEE9q5PdG5gbyaMxRixZDAQVl+0t6ucA3r8xL1JNG9WxUDJ8jqekHcHk/jUy
+wHJMOPQLmXaJL/kyHZkF7LiwRo8+eiRjGKYB06+mAjwaZ/bCxYLe5o9JTwJ0qtd3
+LGPxMWZUodR5WQVbAbjFSLh52DjNMBG896c52BSFbKUQj4AIlz8SvIUY3KHit08M
+SpBxMsWLtM+uo2zGxgBJSfs0FB1yTy8MO1MaM3LtaYtRRS8cxXZxypTwhqjY/d1t
+WsLVdGlur5qUZqpon++HfuM9EUBc6F8zn42LoR2WRQIDAQABMA0GCSqGSIb3DQEB
+BQUAA4IBAQATeNVBKwe97DWQ9DcmbeEs4SphC8hAJzF2DaiO/uKp5XT6FJZx/LQ9
+rN1Ek27PUDVnhNuQUzouR9+YXszDx3wkvwYt0EpwMDMfLlleQHS68wXEJR1u4rIc
+cW2yJOCMq8IAQGyr2FeEkPECJBgpn0yzMGT6JVwSVoqlKCCytWiGT2CDPNE3Mt5J
+iSV6yxXmVKJHthU2gIT6YYqcY+cAdoOQ/JAxuPovMkUdNdzu9MkL3p0ziZoa/Rng
+YyN8YHDWqYfRJCTEX1c0aTLYGP2aJYzGiMFlHDqcbOWG++d/3W6lrNEOZf4MGRJj
+S1DX/13MnQwQSrWtvDN40ISREQTBdVmY
+-----END CERTIFICATE-----
```

### Comparing `tabpy-2.6.0/tests/unit/server_tests/resources/valid.crt` & `tabpy-2.7.0/tests/unit/server_tests/resources/valid.crt`

 * *Files 7% similar despite different names*

```diff
@@ -1,87 +1,89 @@
 00000000: 2d2d 2d2d 2d42 4547 494e 2043 4552 5449  -----BEGIN CERTI
-00000010: 4649 4341 5445 2d2d 2d2d 2d0a 4d49 4944  FICATE-----.MIID
-00000020: 3144 4343 4172 7743 4151 4577 4451 594a  1DCCArwCAQEwDQYJ
-00000030: 4b6f 5a49 6876 634e 4151 4546 4251 4177  KoZIhvcNAQEFBQAw
-00000040: 6761 3078 437a 414a 4267 4e56 4241 5954  ga0xCzAJBgNVBAYT
-00000050: 416c 5642 4d52 3077 4777 5944 0a56 5151  AlVBMR0wGwYD.VQQ
-00000060: 4944 4252 4562 6d6c 7763 6d39 775a 5852  IDBREbmlwcm9wZXR
-00000070: 7962 335a 7a4a 3273 6763 6d56 6e4c 6a45  yb3ZzJ2sgcmVnLjE
-00000080: 584d 4255 4741 3155 4543 6777 4f55 4778  XMBUGA1UECgwOUGx
-00000090: 6862 6d56 3049 4556 3463 484a 6c0a 6333  hbmV0IEV4cHJl.c3
-000000a0: 4d78 466a 4155 4267 4e56 4241 734d 4455  MxFjAUBgNVBAsMDU
-000000b0: 526c 6247 6c32 5a58 4a35 4945 4e79 5a58  RlbGl2ZXJ5IENyZX
-000000c0: 6378 4a7a 416c 4267 4e56 4241 4d4d 486b  cxJzAlBgNVBAMMHk
-000000d0: 5a79 6552 7462 5242 7462 5242 7462 0a52  ZyeRtbRBtbRBtb.R
-000000e0: 4567 3947 3174 5161 476c 7362 476c 7749  Eg9G1tQaGlsbGlwI
-000000f0: 456f 7549 455a 7965 5445 6c4d 434d 4743  EouIEZyeTElMCMGC
-00000100: 5371 4753 4962 3344 5145 4a41 5259 5763  SqGSIb3DQEJARYWc
-00000110: 475a 7965 5542 7762 4746 755a 5852 6c0a  GZyeUBwbGFuZXRl.
-00000120: 6548 4279 5a58 4e7a 4c6d 4e76 6254 4169  eHByZXNzLmNvbTAi
-00000130: 4741 3879 4d44 4178 4d44 4577 4d54 4177  GA8yMDAxMDEwMTAw
-00000140: 4d44 4177 4d46 6f59 447a 4d35 4f54 6b77  MDAwMFoYDzM5OTkw
-00000150: 4d54 4179 4d44 4177 4d44 4177 576a 4342  MTAyMDAwMDAwWjCB
-00000160: 0a72 5445 4c4d 416b 4741 3155 4542 684d  .rTELMAkGA1UEBhM
-00000170: 4356 5545 7848 5441 6242 674e 5642 4167  CVUExHTAbBgNVBAg
-00000180: 4d46 4552 7561 5842 7962 3342 6c64 484a  MFERuaXByb3BldHJ
-00000190: 7664 6e4d 6e61 7942 795a 5763 754d 5263  vdnMnayByZWcuMRc
-000001a0: 770a 4651 5944 5651 514b 4441 3551 6247  w.FQYDVQQKDA5QbG
-000001b0: 4675 5a58 5167 5258 6877 636d 567a 637a  FuZXQgRXhwcmVzcz
-000001c0: 4557 4d42 5147 4131 5545 4377 774e 5247  EWMBQGA1UECwwNRG
-000001d0: 5673 6158 5a6c 636e 6b67 5133 4a6c 647a  VsaXZlcnkgQ3Jldz
-000001e0: 456e 0a4d 4355 4741 3155 4541 7777 6552  En.MCUGA1UEAwweR
-000001f0: 6e4a 3547 3174 4547 3174 4547 3174 4553  nJ5G1tEG1tEG1tES
-00000200: 4430 6257 3142 6f61 5778 7361 5841 6753  D0bW1BoaWxsaXAgS
-00000210: 6934 6752 6e4a 354d 5355 7749 7759 4a4b  i4gRnJ5MSUwIwYJK
-00000220: 6f5a 490a 6876 634e 4151 6b42 4668 5a77  oZI.hvcNAQkBFhZw
-00000230: 5a6e 4a35 5148 4273 5957 356c 6447 5634  ZnJ5QHBsYW5ldGV4
-00000240: 6348 4a6c 6333 4d75 5932 3974 4d49 4942  cHJlc3MuY29tMIIB
-00000250: 496a 414e 4267 6b71 686b 6947 3977 3042  IjANBgkqhkiG9w0B
-00000260: 4151 4546 0a41 414f 4341 5138 414d 4949  AQEF.AAOCAQ8AMII
-00000270: 4243 674b 4341 5145 416d 396f 426a 6250  BCgKCAQEAm9oBjbP
-00000280: 4763 6530 7146 2b6b 7a2b 6663 4b54 4455  Gce0qF+kz+fcKTDU
-00000290: 624a 556a 426a 644c 7447 4f4a 5273 5641  bJUjBjdLtGOJRsVA
-000002a0: 6735 3455 6b0a 7968 5063 4345 4539 7135  g54Uk.yhPcCEE9q5
-000002b0: 5064 4735 6762 7961 4d78 5269 785a 4441  PdG5gbyaMxRixZDA
-000002c0: 5156 6c2b 3074 3675 6341 3372 3878 4c31  QVl+0t6ucA3r8xL1
-000002d0: 4a4e 4739 5778 5544 4a38 6a71 656b 4863  JNG9WxUDJ8jqekHc
-000002e0: 486b 2f6a 5579 0a77 484a 4d4f 5051 4c6d  Hk/jUy.wHJMOPQLm
-000002f0: 5861 4a4c 2f6b 7948 5a6b 4637 4c69 7752  XaJL/kyHZkF7LiwR
-00000300: 6f38 2b65 6952 6a47 4b59 4230 362b 6d41  o8+eiRjGKYB06+mA
-00000310: 6a77 615a 2f62 4378 594c 6535 6f39 4a54  jwaZ/bCxYLe5o9JT
-00000320: 774a 3071 7464 330a 4c47 5078 4d57 5a55  wJ0qtd3.LGPxMWZU
-00000330: 6f64 5235 5751 5662 4162 6a46 534c 6835  odR5WQVbAbjFSLh5
-00000340: 3244 6a4e 4d42 4738 3936 6335 3242 5346  2DjNMBG896c52BSF
-00000350: 624b 5551 6a34 4149 6c7a 3853 7649 5559  bKUQj4AIlz8SvIUY
-00000360: 334b 4869 7430 384d 0a53 7042 784d 7357  3KHit08M.SpBxMsW
-00000370: 4c74 4d2b 756f 327a 4778 6742 4a53 6673  LtM+uo2zGxgBJSfs
-00000380: 3046 4231 7954 7938 4d4f 314d 614d 334c  0FB1yTy8MO1MaM3L
-00000390: 7461 5974 5252 5338 6378 585a 7879 7054  taYtRRS8cxXZxypT
-000003a0: 7768 716a 592f 6431 740a 5773 4c56 6447  whqjY/d1t.WsLVdG
-000003b0: 6c75 7235 7155 5a71 706f 6e2b 2b48 6675  lur5qUZqpon++Hfu
-000003c0: 4d39 4555 4263 3646 387a 6e34 324c 6f52  M9EUBc6F8zn42LoR
-000003d0: 3257 5251 4944 4151 4142 4d41 3047 4353  2WRQIDAQABMA0GCS
-000003e0: 7147 5349 6233 4451 4542 0a42 5155 4141  qGSIb3DQEB.BQUAA
-000003f0: 3449 4241 5142 6d4d 6265 7679 4d4e 5a2f  4IBAQBmMbevyMNZ/
-00000400: 5173 5168 2f6b 5162 5968 744d 7347 7675  QsQh/kQbYhtMsGvu
-00000410: 6778 5256 6638 7139 2f42 4346 6b4f 7733  gxRVf8q9/BCFkOw3
-00000420: 4f54 704e 5542 4b6b 2b46 570a 7479 2f50  OTpNUBKk+FW.ty/P
-00000430: 5662 494e 6936 4d50 6b7a 3461 3332 4673  VbINi6MPkz4a32Fs
-00000440: 516a 4257 2f34 2b4b 6530 416a 6345 5055  QjBW/4+Ke0AjcEPU
-00000450: 7a52 3435 4135 7961 4e4f 612b 7154 554f  zR45A5yaNOa+qTUO
-00000460: 4f62 7943 6a36 4376 4b69 7074 0a44 796c  ObyCj6CvKipt.Dyl
-00000470: 704c 7265 5130 562f 5342 4a66 454f 2f66  pLreQ0V/SBJfEO/f
-00000480: 304c 4876 6844 3849 4775 6979 6263 3839  0LHvhD8IGuiybc89
-00000490: 5041 7151 577a 5a57 6b36 5753 5771 4962  PAqQWzZWk6WSWqIb
-000004a0: 314a 5231 3278 5454 4f66 3242 440a 5232  1JR12xTTOf2BD.R2
-000004b0: 5552 2f31 5843 726c 6976 6f76 5436 5371  UR/1XCrlivovT6Sq
-000004c0: 6a4d 476d 5761 7635 5451 5558 6e50 3053  jMGmWav5TQUXnP0S
-000004d0: 4544 377a 6966 312b 5268 536b 796a 6647  ED7zif1+RhSkyjfG
-000004e0: 4c6d 6870 3155 6836 5437 5a45 4475 0a59  Lmhp1Uh6T7ZEDu.Y
-000004f0: 526e 4677 3072 4970 504d 4a34 5539 614d  RnFw0rIpPMJ4U9aM
-00000500: 5477 7758 6f36 4d44 5158 6f62 787a 5243  TwwXo6MDQXobxzRC
-00000510: 754c 6866 6337 4167 5171 494f 5061 4b50  uLhfc7AgQqIOPaKP
-00000520: 5870 4f4b 6e34 416f 3764 4335 5768 590a  XpOKn4Ao7dC5WhY.
-00000530: 6562 4e2f 5461 5451 526e 7a56 5675 414b  ebN/TaTQRnzVVuAK
-00000540: 6f63 6e6c 6961 4d70 4176 5538 3841 5849  ocnliaMpAvU88AXI
-00000550: 0a2d 2d2d 2d2d 454e 4420 4345 5254 4946  .-----END CERTIF
-00000560: 4943 4154 452d 2d2d 2d2d 0a              ICATE-----.
+00000010: 4649 4341 5445 2d2d 2d2d 2d0d 0a4d 4949  FICATE-----..MII
+00000020: 4431 4443 4341 7277 4341 5145 7744 5159  D1DCCArwCAQEwDQY
+00000030: 4a4b 6f5a 4968 7663 4e41 5145 4642 5141  JKoZIhvcNAQEFBQA
+00000040: 7767 6130 7843 7a41 4a42 674e 5642 4159  wga0xCzAJBgNVBAY
+00000050: 5441 6c56 424d 5230 7747 7759 440d 0a56  TAlVBMR0wGwYD..V
+00000060: 5151 4944 4252 4562 6d6c 7763 6d39 775a  QQIDBREbmlwcm9wZ
+00000070: 5852 7962 335a 7a4a 3273 6763 6d56 6e4c  XRyb3ZzJ2sgcmVnL
+00000080: 6a45 584d 4255 4741 3155 4543 6777 4f55  jEXMBUGA1UECgwOU
+00000090: 4778 6862 6d56 3049 4556 3463 484a 6c0d  GxhbmV0IEV4cHJl.
+000000a0: 0a63 334d 7846 6a41 5542 674e 5642 4173  .c3MxFjAUBgNVBAs
+000000b0: 4d44 5552 6c62 476c 325a 584a 3549 454e  MDURlbGl2ZXJ5IEN
+000000c0: 795a 5863 784a 7a41 6c42 674e 5642 414d  yZXcxJzAlBgNVBAM
+000000d0: 4d48 6b5a 7965 5274 6252 4274 6252 4274  MHkZyeRtbRBtbRBt
+000000e0: 620d 0a52 4567 3947 3174 5161 476c 7362  b..REg9G1tQaGlsb
+000000f0: 476c 7749 456f 7549 455a 7965 5445 6c4d  GlwIEouIEZyeTElM
+00000100: 434d 4743 5371 4753 4962 3344 5145 4a41  CMGCSqGSIb3DQEJA
+00000110: 5259 5763 475a 7965 5542 7762 4746 755a  RYWcGZyeUBwbGFuZ
+00000120: 5852 6c0d 0a65 4842 795a 584e 7a4c 6d4e  XRl..eHByZXNzLmN
+00000130: 7662 5441 6947 4138 794d 4441 784d 4445  vbTAiGA8yMDAxMDE
+00000140: 774d 5441 774d 4441 774d 466f 5944 7a4d  wMTAwMDAwMFoYDzM
+00000150: 354f 546b 774d 5441 794d 4441 774d 4441  5OTkwMTAyMDAwMDA
+00000160: 7757 6a43 420d 0a72 5445 4c4d 416b 4741  wWjCB..rTELMAkGA
+00000170: 3155 4542 684d 4356 5545 7848 5441 6242  1UEBhMCVUExHTAbB
+00000180: 674e 5642 4167 4d46 4552 7561 5842 7962  gNVBAgMFERuaXByb
+00000190: 3342 6c64 484a 7664 6e4d 6e61 7942 795a  3BldHJvdnMnayByZ
+000001a0: 5763 754d 5263 770d 0a46 5159 4456 5151  WcuMRcw..FQYDVQQ
+000001b0: 4b44 4135 5162 4746 755a 5851 6752 5868  KDA5QbGFuZXQgRXh
+000001c0: 7763 6d56 7a63 7a45 574d 4251 4741 3155  wcmVzczEWMBQGA1U
+000001d0: 4543 7777 4e52 4756 7361 585a 6c63 6e6b  ECwwNRGVsaXZlcnk
+000001e0: 6751 334a 6c64 7a45 6e0d 0a4d 4355 4741  gQ3JldzEn..MCUGA
+000001f0: 3155 4541 7777 6552 6e4a 3547 3174 4547  1UEAwweRnJ5G1tEG
+00000200: 3174 4547 3174 4553 4430 6257 3142 6f61  1tEG1tESD0bW1Boa
+00000210: 5778 7361 5841 6753 6934 6752 6e4a 354d  WxsaXAgSi4gRnJ5M
+00000220: 5355 7749 7759 4a4b 6f5a 490d 0a68 7663  SUwIwYJKoZI..hvc
+00000230: 4e41 516b 4246 685a 775a 6e4a 3551 4842  NAQkBFhZwZnJ5QHB
+00000240: 7359 5735 6c64 4756 3463 484a 6c63 334d  sYW5ldGV4cHJlc3M
+00000250: 7559 3239 744d 4949 4249 6a41 4e42 676b  uY29tMIIBIjANBgk
+00000260: 7168 6b69 4739 7730 4241 5145 460d 0a41  qhkiG9w0BAQEF..A
+00000270: 414f 4341 5138 414d 4949 4243 674b 4341  AOCAQ8AMIIBCgKCA
+00000280: 5145 416d 396f 426a 6250 4763 6530 7146  QEAm9oBjbPGce0qF
+00000290: 2b6b 7a2b 6663 4b54 4455 624a 556a 426a  +kz+fcKTDUbJUjBj
+000002a0: 644c 7447 4f4a 5273 5641 6735 3455 6b0d  dLtGOJRsVAg54Uk.
+000002b0: 0a79 6850 6343 4545 3971 3550 6447 3567  .yhPcCEE9q5PdG5g
+000002c0: 6279 614d 7852 6978 5a44 4151 566c 2b30  byaMxRixZDAQVl+0
+000002d0: 7436 7563 4133 7238 784c 314a 4e47 3957  t6ucA3r8xL1JNG9W
+000002e0: 7855 444a 386a 7165 6b48 6348 6b2f 6a55  xUDJ8jqekHcHk/jU
+000002f0: 790d 0a77 484a 4d4f 5051 4c6d 5861 4a4c  y..wHJMOPQLmXaJL
+00000300: 2f6b 7948 5a6b 4637 4c69 7752 6f38 2b65  /kyHZkF7LiwRo8+e
+00000310: 6952 6a47 4b59 4230 362b 6d41 6a77 615a  iRjGKYB06+mAjwaZ
+00000320: 2f62 4378 594c 6535 6f39 4a54 774a 3071  /bCxYLe5o9JTwJ0q
+00000330: 7464 330d 0a4c 4750 784d 575a 556f 6452  td3..LGPxMWZUodR
+00000340: 3557 5156 6241 626a 4653 4c68 3532 446a  5WQVbAbjFSLh52Dj
+00000350: 4e4d 4247 3839 3663 3532 4253 4662 4b55  NMBG896c52BSFbKU
+00000360: 516a 3441 496c 7a38 5376 4955 5933 4b48  Qj4AIlz8SvIUY3KH
+00000370: 6974 3038 4d0d 0a53 7042 784d 7357 4c74  it08M..SpBxMsWLt
+00000380: 4d2b 756f 327a 4778 6742 4a53 6673 3046  M+uo2zGxgBJSfs0F
+00000390: 4231 7954 7938 4d4f 314d 614d 334c 7461  B1yTy8MO1MaM3Lta
+000003a0: 5974 5252 5338 6378 585a 7879 7054 7768  YtRRS8cxXZxypTwh
+000003b0: 716a 592f 6431 740d 0a57 734c 5664 476c  qjY/d1t..WsLVdGl
+000003c0: 7572 3571 555a 7170 6f6e 2b2b 4866 754d  ur5qUZqpon++HfuM
+000003d0: 3945 5542 6336 4638 7a6e 3432 4c6f 5232  9EUBc6F8zn42LoR2
+000003e0: 5752 5149 4441 5141 424d 4130 4743 5371  WRQIDAQABMA0GCSq
+000003f0: 4753 4962 3344 5145 420d 0a42 5155 4141  GSIb3DQEB..BQUAA
+00000400: 3449 4241 5142 6d4d 6265 7679 4d4e 5a2f  4IBAQBmMbevyMNZ/
+00000410: 5173 5168 2f6b 5162 5968 744d 7347 7675  QsQh/kQbYhtMsGvu
+00000420: 6778 5256 6638 7139 2f42 4346 6b4f 7733  gxRVf8q9/BCFkOw3
+00000430: 4f54 704e 5542 4b6b 2b46 570d 0a74 792f  OTpNUBKk+FW..ty/
+00000440: 5056 6249 4e69 364d 506b 7a34 6133 3246  PVbINi6MPkz4a32F
+00000450: 7351 6a42 572f 342b 4b65 3041 6a63 4550  sQjBW/4+Ke0AjcEP
+00000460: 557a 5234 3541 3579 614e 4f61 2b71 5455  UzR45A5yaNOa+qTU
+00000470: 4f4f 6279 436a 3643 764b 6970 740d 0a44  OObyCj6CvKipt..D
+00000480: 796c 704c 7265 5130 562f 5342 4a66 454f  ylpLreQ0V/SBJfEO
+00000490: 2f66 304c 4876 6844 3849 4775 6979 6263  /f0LHvhD8IGuiybc
+000004a0: 3839 5041 7151 577a 5a57 6b36 5753 5771  89PAqQWzZWk6WSWq
+000004b0: 4962 314a 5231 3278 5454 4f66 3242 440d  Ib1JR12xTTOf2BD.
+000004c0: 0a52 3255 522f 3158 4372 6c69 766f 7654  .R2UR/1XCrlivovT
+000004d0: 3653 716a 4d47 6d57 6176 3554 5155 586e  6SqjMGmWav5TQUXn
+000004e0: 5030 5345 4437 7a69 6631 2b52 6853 6b79  P0SED7zif1+RhSky
+000004f0: 6a66 474c 6d68 7031 5568 3654 375a 4544  jfGLmhp1Uh6T7ZED
+00000500: 750d 0a59 526e 4677 3072 4970 504d 4a34  u..YRnFw0rIpPMJ4
+00000510: 5539 614d 5477 7758 6f36 4d44 5158 6f62  U9aMTwwXo6MDQXob
+00000520: 787a 5243 754c 6866 6337 4167 5171 494f  xzRCuLhfc7AgQqIO
+00000530: 5061 4b50 5870 4f4b 6e34 416f 3764 4335  PaKPXpOKn4Ao7dC5
+00000540: 5768 590d 0a65 624e 2f54 6154 5152 6e7a  WhY..ebN/TaTQRnz
+00000550: 5656 7541 4b6f 636e 6c69 614d 7041 7655  VVuAKocnliaMpAvU
+00000560: 3838 4158 490d 0a2d 2d2d 2d2d 454e 4420  88AXI..-----END 
+00000570: 4345 5254 4946 4943 4154 452d 2d2d 2d2d  CERTIFICATE-----
+00000580: 0d0a                                     ..
```

### Comparing `tabpy-2.6.0/tests/unit/server_tests/test_config.py` & `tabpy-2.7.0/tests/unit/server_tests/test_config.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,365 +1,365 @@
-import os
-import unittest
-from tempfile import NamedTemporaryFile
-import tabpy
-from tabpy.tabpy_server.app.util import validate_cert
-from tabpy.tabpy_server.app.app import TabPyApp
-
-from unittest.mock import patch
-
-
-class TestConfigEnvironmentCalls(unittest.TestCase):
-    def test_config_file_does_not_exist(self):
-        app = TabPyApp("/folder_does_not_exit/file_does_not_exist.conf")
-
-        self.assertEqual(app.settings["port"], 9004)
-        self.assertEqual(
-            app.settings["server_version"], open("tabpy/VERSION").read().strip()
-        )
-        self.assertEqual(app.settings["transfer_protocol"], "http")
-        self.assertTrue("certificate_file" not in app.settings)
-        self.assertTrue("key_file" not in app.settings)
-        self.assertEqual(app.settings["log_request_context"], False)
-        self.assertEqual(app.settings["evaluate_timeout"], 30)
-
-    @patch("tabpy.tabpy_server.app.app.TabPyState")
-    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
-    @patch("tabpy.tabpy_server.app.app.PythonServiceHandler")
-    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=True)
-    @patch("tabpy.tabpy_server.app.app.os")
-    def test_no_config_file(
-        self,
-        mock_os,
-        mock_path_exists,
-        mock_psws,
-        mock_management_util,
-        mock_tabpy_state,
-    ):
-        pkg_path = os.path.dirname(tabpy.__file__)
-        obj_path = os.path.join(pkg_path, "tmp", "query_objects")
-        state_path = os.path.join(pkg_path, "tabpy_server")
-        mock_os.environ = {
-            "TABPY_PORT": "9004",
-            "TABPY_QUERY_OBJECT_PATH": obj_path,
-            "TABPY_STATE_PATH": state_path,
-        }
-
-        TabPyApp(None)
-
-        self.assertEqual(len(mock_psws.mock_calls), 1)
-        self.assertEqual(len(mock_tabpy_state.mock_calls), 1)
-        self.assertEqual(len(mock_path_exists.mock_calls), 1)
-        self.assertTrue(len(mock_management_util.mock_calls) > 0)
-        mock_os.makedirs.assert_not_called()
-
-    @patch("tabpy.tabpy_server.app.app.TabPyState")
-    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
-    @patch("tabpy.tabpy_server.app.app.PythonServiceHandler")
-    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=False)
-    @patch("tabpy.tabpy_server.app.app.os")
-    def test_no_state_ini_file_or_state_dir(
-        self,
-        mock_os,
-        mock_path_exists,
-        mock_psws,
-        mock_management_util,
-        mock_tabpy_state,
-    ):
-        TabPyApp(None)
-        self.assertEqual(len(mock_os.makedirs.mock_calls), 1)
-
-
-class TestPartialConfigFile(unittest.TestCase):
-    def setUp(self):
-        self.config_file = NamedTemporaryFile(delete=False)
-
-    def tearDown(self):
-        os.remove(self.config_file.name)
-        self.config_file = None
-
-    @patch("tabpy.tabpy_server.app.app.TabPyState")
-    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
-    @patch("tabpy.tabpy_server.app.app.PythonServiceHandler")
-    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=True)
-    @patch("tabpy.tabpy_server.app.app.os")
-    def test_config_file_present(
-        self,
-        mock_os,
-        mock_path_exists,
-        mock_psws,
-        mock_management_util,
-        mock_tabpy_state,
-    ):
-        self.assertTrue(self.config_file is not None)
-        config_file = self.config_file
-        config_file.write(
-            "[TabPy]\n"
-            "TABPY_QUERY_OBJECT_PATH = foo\n"
-            "TABPY_STATE_PATH = bar\n".encode()
-        )
-        config_file.close()
-
-        mock_os.path.realpath.return_value = "bar"
-        mock_os.environ = {"TABPY_PORT": "1234"}
-
-        app = TabPyApp(config_file.name)
-
-        self.assertEqual(app.settings["port"], "1234")
-        self.assertEqual(
-            app.settings["server_version"], open("tabpy/VERSION").read().strip()
-        )
-        self.assertEqual(app.settings["upload_dir"], "foo")
-        self.assertEqual(app.settings["state_file_path"], "bar")
-        self.assertEqual(app.settings["transfer_protocol"], "http")
-        self.assertTrue("certificate_file" not in app.settings)
-        self.assertTrue("key_file" not in app.settings)
-        self.assertEqual(app.settings["log_request_context"], False)
-        self.assertEqual(app.settings["evaluate_timeout"], 30)
-
-    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=True)
-    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
-    @patch("tabpy.tabpy_server.app.app.TabPyState")
-    def test_custom_evaluate_timeout_valid(
-        self, mock_state, mock_get_state_from_file, mock_path_exists
-    ):
-        self.assertTrue(self.config_file is not None)
-        config_file = self.config_file
-        config_file.write("[TabPy]\n" "TABPY_EVALUATE_TIMEOUT = 1996".encode())
-        config_file.close()
-
-        app = TabPyApp(self.config_file.name)
-        self.assertEqual(app.settings["evaluate_timeout"], 1996.0)
-
-    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=True)
-    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
-    @patch("tabpy.tabpy_server.app.app.TabPyState")
-    def test_custom_evaluate_timeout_invalid(
-        self, mock_state, mock_get_state_from_file, mock_path_exists
-    ):
-        self.assertTrue(self.config_file is not None)
-        config_file = self.config_file
-        config_file.write(
-            "[TabPy]\n" 'TABPY_EVALUATE_TIMEOUT = "im not a float"'.encode()
-        )
-        config_file.close()
-
-        with self.assertRaises(ValueError):
-            TabPyApp(self.config_file.name)
-
-    @patch("tabpy.tabpy_server.app.app.os")
-    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=True)
-    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
-    @patch("tabpy.tabpy_server.app.app.TabPyState")
-    def test_env_variables_in_config(
-        self, mock_state, mock_get_state, mock_path_exists, mock_os
-    ):
-        mock_os.environ = {"foo": "baz"}
-        config_file = self.config_file
-        config_file.write("[TabPy]\n" "TABPY_PORT = %(foo)sbar".encode())
-        config_file.close()
-
-        app = TabPyApp(self.config_file.name)
-        self.assertEqual(app.settings["port"], "bazbar")
-
-    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=True)
-    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
-    @patch("tabpy.tabpy_server.app.app.TabPyState")
-    def test_gzip_setting_on_valid(
-        self, mock_state, mock_get_state_from_file, mock_path_exists
-    ):
-        self.assertTrue(self.config_file is not None)
-        config_file = self.config_file
-        config_file.write("[TabPy]\n" "TABPY_GZIP_ENABLE = true".encode())
-        config_file.close()
-
-        app = TabPyApp(self.config_file.name)
-        self.assertEqual(app.settings["gzip_enabled"], True)
-
-    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=True)
-    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
-    @patch("tabpy.tabpy_server.app.app.TabPyState")
-    def test_gzip_setting_off_valid(
-        self, mock_state, mock_get_state_from_file, mock_path_exists
-    ):
-        self.assertTrue(self.config_file is not None)
-        config_file = self.config_file
-        config_file.write("[TabPy]\n" "TABPY_GZIP_ENABLE = false".encode())
-        config_file.close()
-
-        app = TabPyApp(self.config_file.name)
-        self.assertEqual(app.settings["gzip_enabled"], False)
-
-class TestTransferProtocolValidation(unittest.TestCase):
-    def assertTabPyAppRaisesRuntimeError(self, expected_message):
-        with self.assertRaises(RuntimeError) as err:
-            TabPyApp(self.fp.name)
-        self.assertEqual(err.exception.args[0], expected_message)
-
-    @staticmethod
-    def mock_isfile(target_file, existing_files):
-        if target_file in existing_files:
-            return True
-        return False
-
-    @staticmethod
-    def raise_attribute_error():
-        raise AttributeError()
-
-    def __init__(self, *args, **kwargs):
-        super(TestTransferProtocolValidation, self).__init__(*args, **kwargs)
-        self.fp = None
-
-    def setUp(self):
-        self.fp = NamedTemporaryFile(mode="w+t", delete=False)
-
-    def tearDown(self):
-        os.remove(self.fp.name)
-        self.fp = None
-
-    def test_invalid_protocol(self):
-        self.fp.write("[TabPy]\n" "TABPY_TRANSFER_PROTOCOL = gopher")
-        self.fp.close()
-
-        self.assertTabPyAppRaisesRuntimeError("Unsupported transfer protocol: gopher")
-
-    def test_http(self):
-        self.fp.write("[TabPy]\n" "TABPY_TRANSFER_PROTOCOL = http")
-        self.fp.close()
-
-        app = TabPyApp(self.fp.name)
-        self.assertEqual(app.settings["transfer_protocol"], "http")
-
-    def test_https_without_cert_and_key(self):
-        self.fp.write("[TabPy]\n" "TABPY_TRANSFER_PROTOCOL = https")
-        self.fp.close()
-
-        self.assertTabPyAppRaisesRuntimeError(
-            "Error using HTTPS: The paramete"
-            "r(s) TABPY_CERTIFICATE_FILE and"
-            " TABPY_KEY_FILE must be set."
-        )
-
-    def test_https_without_cert(self):
-        self.fp.write(
-            "[TabPy]\n" "TABPY_TRANSFER_PROTOCOL = https\n" "TABPY_KEY_FILE = foo"
-        )
-        self.fp.close()
-
-        self.assertTabPyAppRaisesRuntimeError(
-            "Error using HTTPS: The parameter(s) TABPY_CERTIFICATE_FILE must " "be set."
-        )
-
-    def test_https_without_key(self):
-        self.fp.write(
-            "[TabPy]\n"
-            "TABPY_TRANSFER_PROTOCOL = https\n"
-            "TABPY_CERTIFICATE_FILE = foo"
-        )
-        self.fp.close()
-
-        self.assertTabPyAppRaisesRuntimeError(
-            "Error using HTTPS: The parameter(s) TABPY_KEY_FILE must be set."
-        )
-
-    @patch("tabpy.tabpy_server.app.app.os.path")
-    def test_https_cert_and_key_file_not_found(self, mock_path):
-        self.fp.write(
-            "[TabPy]\n"
-            "TABPY_TRANSFER_PROTOCOL = https\n"
-            "TABPY_CERTIFICATE_FILE = foo\n"
-            "TABPY_KEY_FILE = bar"
-        )
-        self.fp.close()
-
-        mock_path.isfile.side_effect = lambda x: self.mock_isfile(x, {self.fp.name})
-
-        self.assertTabPyAppRaisesRuntimeError(
-            "Error using HTTPS: The parameter(s) TABPY_CERTIFICATE_FILE and "
-            "TABPY_KEY_FILE must point to an existing file."
-        )
-
-    @patch("tabpy.tabpy_server.app.app.os.path")
-    def test_https_cert_file_not_found(self, mock_path):
-        self.fp.write(
-            "[TabPy]\n"
-            "TABPY_TRANSFER_PROTOCOL = https\n"
-            "TABPY_CERTIFICATE_FILE = foo\n"
-            "TABPY_KEY_FILE = bar"
-        )
-        self.fp.close()
-
-        mock_path.isfile.side_effect = lambda x: self.mock_isfile(
-            x, {self.fp.name, "bar"}
-        )
-
-        self.assertTabPyAppRaisesRuntimeError(
-            "Error using HTTPS: The parameter(s) TABPY_CERTIFICATE_FILE "
-            "must point to an existing file."
-        )
-
-    @patch("tabpy.tabpy_server.app.app.os.path")
-    def test_https_key_file_not_found(self, mock_path):
-        self.fp.write(
-            "[TabPy]\n"
-            "TABPY_TRANSFER_PROTOCOL = https\n"
-            "TABPY_CERTIFICATE_FILE = foo\n"
-            "TABPY_KEY_FILE = bar"
-        )
-        self.fp.close()
-
-        mock_path.isfile.side_effect = lambda x: self.mock_isfile(
-            x, {self.fp.name, "foo"}
-        )
-
-        self.assertTabPyAppRaisesRuntimeError(
-            "Error using HTTPS: The parameter(s) TABPY_KEY_FILE "
-            "must point to an existing file."
-        )
-
-    @patch("tabpy.tabpy_server.app.app.os.path.isfile", return_value=True)
-    @patch("tabpy.tabpy_server.app.util.validate_cert")
-    def test_https_success(self, mock_isfile, mock_validate_cert):
-        self.fp.write(
-            "[TabPy]\n"
-            "TABPY_TRANSFER_PROTOCOL = HtTpS\n"
-            "TABPY_CERTIFICATE_FILE = foo\n"
-            "TABPY_KEY_FILE = bar"
-        )
-        self.fp.close()
-
-        app = TabPyApp(self.fp.name)
-
-        self.assertEqual(app.settings["transfer_protocol"], "https")
-        self.assertEqual(app.settings["certificate_file"], "foo")
-        self.assertEqual(app.settings["key_file"], "bar")
-
-
-class TestCertificateValidation(unittest.TestCase):
-    def assertValidateCertRaisesRuntimeError(self, expected_message, path):
-        with self.assertRaises(RuntimeError) as err:
-            validate_cert(path)
-        self.assertEqual(err.exception.args[0], expected_message)
-
-    def __init__(self, *args, **kwargs):
-        super(TestCertificateValidation, self).__init__(*args, **kwargs)
-        self.resources_path = os.path.join(os.path.dirname(__file__), "resources")
-
-    def test_expired_cert(self):
-        path = os.path.join(self.resources_path, "expired.crt")
-        message = (
-            "Error using HTTPS: The certificate provided expired "
-            "on 2018-08-18 19:47:18."
-        )
-        self.assertValidateCertRaisesRuntimeError(message, path)
-
-    def test_future_cert(self):
-        path = os.path.join(self.resources_path, "future.crt")
-        message = (
-            "Error using HTTPS: The certificate provided is not valid "
-            "until 3001-01-01 00:00:00."
-        )
-        self.assertValidateCertRaisesRuntimeError(message, path)
-
-    def test_valid_cert(self):
-        path = os.path.join(self.resources_path, "valid.crt")
-        validate_cert(path)
+import os
+import unittest
+from tempfile import NamedTemporaryFile
+import tabpy
+from tabpy.tabpy_server.app.util import validate_cert
+from tabpy.tabpy_server.app.app import TabPyApp
+
+from unittest.mock import patch
+
+
+class TestConfigEnvironmentCalls(unittest.TestCase):
+    def test_config_file_does_not_exist(self):
+        app = TabPyApp("/folder_does_not_exit/file_does_not_exist.conf")
+
+        self.assertEqual(app.settings["port"], 9004)
+        self.assertEqual(
+            app.settings["server_version"], open("tabpy/VERSION").read().strip()
+        )
+        self.assertEqual(app.settings["transfer_protocol"], "http")
+        self.assertTrue("certificate_file" not in app.settings)
+        self.assertTrue("key_file" not in app.settings)
+        self.assertEqual(app.settings["log_request_context"], False)
+        self.assertEqual(app.settings["evaluate_timeout"], 30)
+
+    @patch("tabpy.tabpy_server.app.app.TabPyState")
+    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
+    @patch("tabpy.tabpy_server.app.app.PythonServiceHandler")
+    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=True)
+    @patch("tabpy.tabpy_server.app.app.os")
+    def test_no_config_file(
+        self,
+        mock_os,
+        mock_path_exists,
+        mock_psws,
+        mock_management_util,
+        mock_tabpy_state,
+    ):
+        pkg_path = os.path.dirname(tabpy.__file__)
+        obj_path = os.path.join(pkg_path, "tmp", "query_objects")
+        state_path = os.path.join(pkg_path, "tabpy_server")
+        mock_os.environ = {
+            "TABPY_PORT": "9004",
+            "TABPY_QUERY_OBJECT_PATH": obj_path,
+            "TABPY_STATE_PATH": state_path,
+        }
+
+        TabPyApp(None)
+
+        self.assertEqual(len(mock_psws.mock_calls), 1)
+        self.assertEqual(len(mock_tabpy_state.mock_calls), 1)
+        self.assertEqual(len(mock_path_exists.mock_calls), 1)
+        self.assertTrue(len(mock_management_util.mock_calls) > 0)
+        mock_os.makedirs.assert_not_called()
+
+    @patch("tabpy.tabpy_server.app.app.TabPyState")
+    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
+    @patch("tabpy.tabpy_server.app.app.PythonServiceHandler")
+    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=False)
+    @patch("tabpy.tabpy_server.app.app.os")
+    def test_no_state_ini_file_or_state_dir(
+        self,
+        mock_os,
+        mock_path_exists,
+        mock_psws,
+        mock_management_util,
+        mock_tabpy_state,
+    ):
+        TabPyApp(None)
+        self.assertEqual(len(mock_os.makedirs.mock_calls), 1)
+
+
+class TestPartialConfigFile(unittest.TestCase):
+    def setUp(self):
+        self.config_file = NamedTemporaryFile(delete=False)
+
+    def tearDown(self):
+        os.remove(self.config_file.name)
+        self.config_file = None
+
+    @patch("tabpy.tabpy_server.app.app.TabPyState")
+    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
+    @patch("tabpy.tabpy_server.app.app.PythonServiceHandler")
+    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=True)
+    @patch("tabpy.tabpy_server.app.app.os")
+    def test_config_file_present(
+        self,
+        mock_os,
+        mock_path_exists,
+        mock_psws,
+        mock_management_util,
+        mock_tabpy_state,
+    ):
+        self.assertTrue(self.config_file is not None)
+        config_file = self.config_file
+        config_file.write(
+            "[TabPy]\n"
+            "TABPY_QUERY_OBJECT_PATH = foo\n"
+            "TABPY_STATE_PATH = bar\n".encode()
+        )
+        config_file.close()
+
+        mock_os.path.realpath.return_value = "bar"
+        mock_os.environ = {"TABPY_PORT": "1234"}
+
+        app = TabPyApp(config_file.name)
+
+        self.assertEqual(app.settings["port"], "1234")
+        self.assertEqual(
+            app.settings["server_version"], open("tabpy/VERSION").read().strip()
+        )
+        self.assertEqual(app.settings["upload_dir"], "foo")
+        self.assertEqual(app.settings["state_file_path"], "bar")
+        self.assertEqual(app.settings["transfer_protocol"], "http")
+        self.assertTrue("certificate_file" not in app.settings)
+        self.assertTrue("key_file" not in app.settings)
+        self.assertEqual(app.settings["log_request_context"], False)
+        self.assertEqual(app.settings["evaluate_timeout"], 30)
+
+    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=True)
+    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
+    @patch("tabpy.tabpy_server.app.app.TabPyState")
+    def test_custom_evaluate_timeout_valid(
+        self, mock_state, mock_get_state_from_file, mock_path_exists
+    ):
+        self.assertTrue(self.config_file is not None)
+        config_file = self.config_file
+        config_file.write("[TabPy]\n" "TABPY_EVALUATE_TIMEOUT = 1996".encode())
+        config_file.close()
+
+        app = TabPyApp(self.config_file.name)
+        self.assertEqual(app.settings["evaluate_timeout"], 1996.0)
+
+    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=True)
+    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
+    @patch("tabpy.tabpy_server.app.app.TabPyState")
+    def test_custom_evaluate_timeout_invalid(
+        self, mock_state, mock_get_state_from_file, mock_path_exists
+    ):
+        self.assertTrue(self.config_file is not None)
+        config_file = self.config_file
+        config_file.write(
+            "[TabPy]\n" 'TABPY_EVALUATE_TIMEOUT = "im not a float"'.encode()
+        )
+        config_file.close()
+
+        with self.assertRaises(ValueError):
+            TabPyApp(self.config_file.name)
+
+    @patch("tabpy.tabpy_server.app.app.os")
+    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=True)
+    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
+    @patch("tabpy.tabpy_server.app.app.TabPyState")
+    def test_env_variables_in_config(
+        self, mock_state, mock_get_state, mock_path_exists, mock_os
+    ):
+        mock_os.environ = {"foo": "baz"}
+        config_file = self.config_file
+        config_file.write("[TabPy]\n" "TABPY_PORT = %(foo)sbar".encode())
+        config_file.close()
+
+        app = TabPyApp(self.config_file.name)
+        self.assertEqual(app.settings["port"], "bazbar")
+
+    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=True)
+    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
+    @patch("tabpy.tabpy_server.app.app.TabPyState")
+    def test_gzip_setting_on_valid(
+        self, mock_state, mock_get_state_from_file, mock_path_exists
+    ):
+        self.assertTrue(self.config_file is not None)
+        config_file = self.config_file
+        config_file.write("[TabPy]\n" "TABPY_GZIP_ENABLE = true".encode())
+        config_file.close()
+
+        app = TabPyApp(self.config_file.name)
+        self.assertEqual(app.settings["gzip_enabled"], True)
+
+    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=True)
+    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
+    @patch("tabpy.tabpy_server.app.app.TabPyState")
+    def test_gzip_setting_off_valid(
+        self, mock_state, mock_get_state_from_file, mock_path_exists
+    ):
+        self.assertTrue(self.config_file is not None)
+        config_file = self.config_file
+        config_file.write("[TabPy]\n" "TABPY_GZIP_ENABLE = false".encode())
+        config_file.close()
+
+        app = TabPyApp(self.config_file.name)
+        self.assertEqual(app.settings["gzip_enabled"], False)
+
+class TestTransferProtocolValidation(unittest.TestCase):
+    def assertTabPyAppRaisesRuntimeError(self, expected_message):
+        with self.assertRaises(RuntimeError) as err:
+            TabPyApp(self.fp.name)
+        self.assertEqual(err.exception.args[0], expected_message)
+
+    @staticmethod
+    def mock_isfile(target_file, existing_files):
+        if target_file in existing_files:
+            return True
+        return False
+
+    @staticmethod
+    def raise_attribute_error():
+        raise AttributeError()
+
+    def __init__(self, *args, **kwargs):
+        super(TestTransferProtocolValidation, self).__init__(*args, **kwargs)
+        self.fp = None
+
+    def setUp(self):
+        self.fp = NamedTemporaryFile(mode="w+t", delete=False)
+
+    def tearDown(self):
+        os.remove(self.fp.name)
+        self.fp = None
+
+    def test_invalid_protocol(self):
+        self.fp.write("[TabPy]\n" "TABPY_TRANSFER_PROTOCOL = gopher")
+        self.fp.close()
+
+        self.assertTabPyAppRaisesRuntimeError("Unsupported transfer protocol: gopher")
+
+    def test_http(self):
+        self.fp.write("[TabPy]\n" "TABPY_TRANSFER_PROTOCOL = http")
+        self.fp.close()
+
+        app = TabPyApp(self.fp.name)
+        self.assertEqual(app.settings["transfer_protocol"], "http")
+
+    def test_https_without_cert_and_key(self):
+        self.fp.write("[TabPy]\n" "TABPY_TRANSFER_PROTOCOL = https")
+        self.fp.close()
+
+        self.assertTabPyAppRaisesRuntimeError(
+            "Error using HTTPS: The paramete"
+            "r(s) TABPY_CERTIFICATE_FILE and"
+            " TABPY_KEY_FILE must be set."
+        )
+
+    def test_https_without_cert(self):
+        self.fp.write(
+            "[TabPy]\n" "TABPY_TRANSFER_PROTOCOL = https\n" "TABPY_KEY_FILE = foo"
+        )
+        self.fp.close()
+
+        self.assertTabPyAppRaisesRuntimeError(
+            "Error using HTTPS: The parameter(s) TABPY_CERTIFICATE_FILE must " "be set."
+        )
+
+    def test_https_without_key(self):
+        self.fp.write(
+            "[TabPy]\n"
+            "TABPY_TRANSFER_PROTOCOL = https\n"
+            "TABPY_CERTIFICATE_FILE = foo"
+        )
+        self.fp.close()
+
+        self.assertTabPyAppRaisesRuntimeError(
+            "Error using HTTPS: The parameter(s) TABPY_KEY_FILE must be set."
+        )
+
+    @patch("tabpy.tabpy_server.app.app.os.path")
+    def test_https_cert_and_key_file_not_found(self, mock_path):
+        self.fp.write(
+            "[TabPy]\n"
+            "TABPY_TRANSFER_PROTOCOL = https\n"
+            "TABPY_CERTIFICATE_FILE = foo\n"
+            "TABPY_KEY_FILE = bar"
+        )
+        self.fp.close()
+
+        mock_path.isfile.side_effect = lambda x: self.mock_isfile(x, {self.fp.name})
+
+        self.assertTabPyAppRaisesRuntimeError(
+            "Error using HTTPS: The parameter(s) TABPY_CERTIFICATE_FILE and "
+            "TABPY_KEY_FILE must point to an existing file."
+        )
+
+    @patch("tabpy.tabpy_server.app.app.os.path")
+    def test_https_cert_file_not_found(self, mock_path):
+        self.fp.write(
+            "[TabPy]\n"
+            "TABPY_TRANSFER_PROTOCOL = https\n"
+            "TABPY_CERTIFICATE_FILE = foo\n"
+            "TABPY_KEY_FILE = bar"
+        )
+        self.fp.close()
+
+        mock_path.isfile.side_effect = lambda x: self.mock_isfile(
+            x, {self.fp.name, "bar"}
+        )
+
+        self.assertTabPyAppRaisesRuntimeError(
+            "Error using HTTPS: The parameter(s) TABPY_CERTIFICATE_FILE "
+            "must point to an existing file."
+        )
+
+    @patch("tabpy.tabpy_server.app.app.os.path")
+    def test_https_key_file_not_found(self, mock_path):
+        self.fp.write(
+            "[TabPy]\n"
+            "TABPY_TRANSFER_PROTOCOL = https\n"
+            "TABPY_CERTIFICATE_FILE = foo\n"
+            "TABPY_KEY_FILE = bar"
+        )
+        self.fp.close()
+
+        mock_path.isfile.side_effect = lambda x: self.mock_isfile(
+            x, {self.fp.name, "foo"}
+        )
+
+        self.assertTabPyAppRaisesRuntimeError(
+            "Error using HTTPS: The parameter(s) TABPY_KEY_FILE "
+            "must point to an existing file."
+        )
+
+    @patch("tabpy.tabpy_server.app.app.os.path.isfile", return_value=True)
+    @patch("tabpy.tabpy_server.app.util.validate_cert")
+    def test_https_success(self, mock_isfile, mock_validate_cert):
+        self.fp.write(
+            "[TabPy]\n"
+            "TABPY_TRANSFER_PROTOCOL = HtTpS\n"
+            "TABPY_CERTIFICATE_FILE = foo\n"
+            "TABPY_KEY_FILE = bar"
+        )
+        self.fp.close()
+
+        app = TabPyApp(self.fp.name)
+
+        self.assertEqual(app.settings["transfer_protocol"], "https")
+        self.assertEqual(app.settings["certificate_file"], "foo")
+        self.assertEqual(app.settings["key_file"], "bar")
+
+
+class TestCertificateValidation(unittest.TestCase):
+    def assertValidateCertRaisesRuntimeError(self, expected_message, path):
+        with self.assertRaises(RuntimeError) as err:
+            validate_cert(path)
+        self.assertEqual(err.exception.args[0], expected_message)
+
+    def __init__(self, *args, **kwargs):
+        super(TestCertificateValidation, self).__init__(*args, **kwargs)
+        self.resources_path = os.path.join(os.path.dirname(__file__), "resources")
+
+    def test_expired_cert(self):
+        path = os.path.join(self.resources_path, "expired.crt")
+        message = (
+            "Error using HTTPS: The certificate provided expired "
+            "on 2018-08-18 19:47:18."
+        )
+        self.assertValidateCertRaisesRuntimeError(message, path)
+
+    def test_future_cert(self):
+        path = os.path.join(self.resources_path, "future.crt")
+        message = (
+            "Error using HTTPS: The certificate provided is not valid "
+            "until 3001-01-01 00:00:00."
+        )
+        self.assertValidateCertRaisesRuntimeError(message, path)
+
+    def test_valid_cert(self):
+        path = os.path.join(self.resources_path, "valid.crt")
+        validate_cert(path)
```

### Comparing `tabpy-2.6.0/tests/unit/server_tests/test_endpoint_handler.py` & `tabpy-2.7.0/tests/unit/server_tests/test_endpoint_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/tests/unit/server_tests/test_endpoints_handler.py` & `tabpy-2.7.0/tests/unit/server_tests/test_endpoints_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/tests/unit/server_tests/test_evaluation_plane_handler.py` & `tabpy-2.7.0/tests/unit/server_tests/test_evaluation_plane_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/tests/unit/server_tests/test_pwd_file.py` & `tabpy-2.7.0/tests/unit/server_tests/test_pwd_file.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.6.0/tests/unit/server_tests/test_service_info_handler.py` & `tabpy-2.7.0/tests/unit/server_tests/test_service_info_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-import base64
-import json
-import os
-from tabpy.tabpy_server.app.app import TabPyApp
-from tabpy.tabpy_server.app.app_parameters import SettingsParameters
-import tempfile
-from tornado.testing import AsyncHTTPTestCase
-
-
-def _create_expected_info_response(settings, tabpy_state):
-    return {
-        "description": tabpy_state.get_description(),
-        "creation_time": tabpy_state.creation_time,
-        "state_path": settings["state_file_path"],
-        "server_version": settings[SettingsParameters.ServerVersion],
-        "name": tabpy_state.name,
-        "versions": settings["versions"]
-    }
-
-
-class BaseTestServiceInfoHandler(AsyncHTTPTestCase):
-    def get_app(self):
-        if hasattr(self, 'config_file') and hasattr(self.config_file, 'name'):
-            self.app = TabPyApp(self.config_file.name)
-        else:
-            self.app = TabPyApp()
-        return self.app._create_tornado_web_app()
-
-    @classmethod
-    def tearDownClass(cls):
-        os.remove(cls.state_file.name)
-        os.remove(cls.config_file.name)
-        os.rmdir(cls.state_dir)
-
-    @classmethod
-    def setUpClass(cls):
-        # create state.ini dir and file
-        cls.state_dir = tempfile.mkdtemp(prefix=cls.prefix)
-        with open(os.path.join(cls.state_dir, "state.ini"), "w+") as cls.state_file:
-            cls.state_file.write(
-                "[Service Info]\n"
-                "Name = TabPy Serve\n"
-                "Description = \n"
-                "Creation Time = 0\n"
-                "Access-Control-Allow-Origin = \n"
-                "Access-Control-Allow-Headers = \n"
-                "Access-Control-Allow-Methods = \n"
-                "\n"
-                "[Query Objects Service Versions]\n"
-                "\n"
-                "[Query Objects Docstrings]\n"
-                "\n"
-                "[Meta]\n"
-                "Revision Number = 1\n"
-            )
-        cls.state_file.close()
-
-        # create config file
-        cls.config_file = tempfile.NamedTemporaryFile(
-            prefix=cls.prefix, suffix=".conf", delete=False, mode='w'
-        )
-        cls.config_file.write("[TabPy]\n")
-        if hasattr(cls, 'tabpy_config'):
-            for k in cls.tabpy_config:
-                cls.config_file.write(k)
-        cls.config_file.close()
-
-
-class TestServiceInfoHandlerWithAuth(BaseTestServiceInfoHandler):
-    @classmethod
-    def setUpClass(cls):
-        cls.prefix = "__TestServiceInfoHandlerWithAuth_"
-        cls.tabpy_config = ["TABPY_PWD_FILE = ./tests/integration/resources/pwdfile.txt\n"]
-        super(TestServiceInfoHandlerWithAuth, cls).setUpClass()
-
-    def test_given_server_with_auth_expect_error_info_response(self):
-        response = self.fetch("/info")
-        self.assertEqual(response.code, 401)
-
-    def test_given_server_with_auth_expect_correct_info_response(self):
-        header = {
-            "Content-Type": "application/json",
-            "TabPy-Client": "Integration test for deploying models with auth",
-            "Authorization": "Basic " +
-            base64.b64encode("user1:P@ssw0rd".encode("utf-8")).decode("utf-8"),
-        }
-
-        response = self.fetch("/info", headers=header)
-        self.assertEqual(response.code, 200)
-        actual_response = json.loads(response.body)
-        expected_response = _create_expected_info_response(
-            self.app.settings, self.app.tabpy_state
-        )
-
-        self.assertDictEqual(actual_response, expected_response)
-        self.assertTrue("versions" in actual_response)
-        versions = actual_response["versions"]
-        self.assertTrue("v1" in versions)
-        v1 = versions["v1"]
-        self.assertTrue("features" in v1)
-        features = v1["features"]
-        self.assertDictEqual(
-            {"authentication": {"methods": {"basic-auth": {}}, "required": True},
-                'evaluate_enabled': True, 'gzip_enabled': True},
-                features,
-        )
-
-
-class TestServiceInfoHandlerWithoutAuth(BaseTestServiceInfoHandler):
-    @classmethod
-    def setUpClass(cls):
-        cls.prefix = "__TestServiceInfoHandlerWithoutAuth_"
-        super(TestServiceInfoHandlerWithoutAuth, cls).setUpClass()
-
-    def test_server_with_no_auth_expect_correct_info_response(self):
-        response = self.fetch("/info")
-        self.assertEqual(response.code, 200)
-        actual_response = json.loads(response.body)
-        expected_response = _create_expected_info_response(
-            self.app.settings, self.app.tabpy_state
-        )
-
-        self.assertDictEqual(actual_response, expected_response)
-        self.assertTrue("versions" in actual_response)
-        versions = actual_response["versions"]
-        self.assertTrue("v1" in versions)
-        v1 = versions["v1"]
-        self.assertTrue("features" in v1)
-        features = v1["features"]
-        self.assertDictEqual({'evaluate_enabled': True, 'gzip_enabled': True}, features)
-
-    def test_given_server_with_no_auth_and_password_expect_correct_info_response(self):
-        header = {
-            "Content-Type": "application/json",
-            "TabPy-Client": "Integration test for deploying models with auth",
-            "Authorization": "Basic " +
-            base64.b64encode("user1:P@ssw0rd".encode("utf-8")).decode("utf-8"),
-        }
-
-        response = self.fetch("/info", headers=header)
-        self.assertEqual(response.code, 406)
+import base64
+import json
+import os
+from tabpy.tabpy_server.app.app import TabPyApp
+from tabpy.tabpy_server.app.app_parameters import SettingsParameters
+import tempfile
+from tornado.testing import AsyncHTTPTestCase
+
+
+def _create_expected_info_response(settings, tabpy_state):
+    return {
+        "description": tabpy_state.get_description(),
+        "creation_time": tabpy_state.creation_time,
+        "state_path": settings["state_file_path"],
+        "server_version": settings[SettingsParameters.ServerVersion],
+        "name": tabpy_state.name,
+        "versions": settings["versions"]
+    }
+
+
+class BaseTestServiceInfoHandler(AsyncHTTPTestCase):
+    def get_app(self):
+        if hasattr(self, 'config_file') and hasattr(self.config_file, 'name'):
+            self.app = TabPyApp(self.config_file.name)
+        else:
+            self.app = TabPyApp()
+        return self.app._create_tornado_web_app()
+
+    @classmethod
+    def tearDownClass(cls):
+        os.remove(cls.state_file.name)
+        os.remove(cls.config_file.name)
+        os.rmdir(cls.state_dir)
+
+    @classmethod
+    def setUpClass(cls):
+        # create state.ini dir and file
+        cls.state_dir = tempfile.mkdtemp(prefix=cls.prefix)
+        with open(os.path.join(cls.state_dir, "state.ini"), "w+") as cls.state_file:
+            cls.state_file.write(
+                "[Service Info]\n"
+                "Name = TabPy Serve\n"
+                "Description = \n"
+                "Creation Time = 0\n"
+                "Access-Control-Allow-Origin = \n"
+                "Access-Control-Allow-Headers = \n"
+                "Access-Control-Allow-Methods = \n"
+                "\n"
+                "[Query Objects Service Versions]\n"
+                "\n"
+                "[Query Objects Docstrings]\n"
+                "\n"
+                "[Meta]\n"
+                "Revision Number = 1\n"
+            )
+        cls.state_file.close()
+
+        # create config file
+        cls.config_file = tempfile.NamedTemporaryFile(
+            prefix=cls.prefix, suffix=".conf", delete=False, mode='w'
+        )
+        cls.config_file.write("[TabPy]\n")
+        if hasattr(cls, 'tabpy_config'):
+            for k in cls.tabpy_config:
+                cls.config_file.write(k)
+        cls.config_file.close()
+
+
+class TestServiceInfoHandlerWithAuth(BaseTestServiceInfoHandler):
+    @classmethod
+    def setUpClass(cls):
+        cls.prefix = "__TestServiceInfoHandlerWithAuth_"
+        cls.tabpy_config = ["TABPY_PWD_FILE = ./tests/integration/resources/pwdfile.txt\n"]
+        super(TestServiceInfoHandlerWithAuth, cls).setUpClass()
+
+    def test_given_server_with_auth_expect_error_info_response(self):
+        response = self.fetch("/info")
+        self.assertEqual(response.code, 401)
+
+    def test_given_server_with_auth_expect_correct_info_response(self):
+        header = {
+            "Content-Type": "application/json",
+            "TabPy-Client": "Integration test for deploying models with auth",
+            "Authorization": "Basic " +
+            base64.b64encode("user1:P@ssw0rd".encode("utf-8")).decode("utf-8"),
+        }
+
+        response = self.fetch("/info", headers=header)
+        self.assertEqual(response.code, 200)
+        actual_response = json.loads(response.body)
+        expected_response = _create_expected_info_response(
+            self.app.settings, self.app.tabpy_state
+        )
+
+        self.assertDictEqual(actual_response, expected_response)
+        self.assertTrue("versions" in actual_response)
+        versions = actual_response["versions"]
+        self.assertTrue("v1" in versions)
+        v1 = versions["v1"]
+        self.assertTrue("features" in v1)
+        features = v1["features"]
+        self.assertDictEqual(
+            {"authentication": {"methods": {"basic-auth": {}}, "required": True},
+                'arrow_enabled': False, 'evaluate_enabled': True, 'gzip_enabled': True},
+                features,
+        )
+
+
+class TestServiceInfoHandlerWithoutAuth(BaseTestServiceInfoHandler):
+    @classmethod
+    def setUpClass(cls):
+        cls.prefix = "__TestServiceInfoHandlerWithoutAuth_"
+        super(TestServiceInfoHandlerWithoutAuth, cls).setUpClass()
+
+    def test_server_with_no_auth_expect_correct_info_response(self):
+        response = self.fetch("/info")
+        self.assertEqual(response.code, 200)
+        actual_response = json.loads(response.body)
+        expected_response = _create_expected_info_response(
+            self.app.settings, self.app.tabpy_state
+        )
+
+        self.assertDictEqual(actual_response, expected_response)
+        self.assertTrue("versions" in actual_response)
+        versions = actual_response["versions"]
+        self.assertTrue("v1" in versions)
+        v1 = versions["v1"]
+        self.assertTrue("features" in v1)
+        features = v1["features"]
+        self.assertDictEqual({'arrow_enabled': False, 'evaluate_enabled': True, 'gzip_enabled': True}, features)
+
+    def test_given_server_with_no_auth_and_password_expect_correct_info_response(self):
+        header = {
+            "Content-Type": "application/json",
+            "TabPy-Client": "Integration test for deploying models with auth",
+            "Authorization": "Basic " +
+            base64.b64encode("user1:P@ssw0rd".encode("utf-8")).decode("utf-8"),
+        }
+
+        response = self.fetch("/info", headers=header)
+        self.assertEqual(response.code, 406)
```

### Comparing `tabpy-2.6.0/tests/unit/tools_tests/test_client.py` & `tabpy-2.7.0/tests/unit/tools_tests/test_client.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import unittest
-from unittest.mock import Mock
-
-from tabpy.tabpy_tools.client import Client
-from tabpy.tabpy_tools.client import _check_endpoint_name
-
-
-class TestClient(unittest.TestCase):
-    def setUp(self):
-        self.client = Client("http://example.com/")
-        self.client._service = Mock()  # TODO: should spec this
-
-    def test_init(self):
-        client = Client("http://example.com:9004")
-
-        self.assertEqual(client._endpoint, "http://example.com:9004")
-
-        client = Client("http://example.com/", 10.0)
-
-        self.assertEqual(client._endpoint, "http://example.com/")
-
-        client = Client(endpoint="https://example.com/", query_timeout=-10.0)
-
-        self.assertEqual(client._endpoint, "https://example.com/")
-        self.assertEqual(client.query_timeout, 0.0)
-
-        # valid name tests
-        with self.assertRaises(ValueError):
-            Client("")
-        with self.assertRaises(TypeError):
-            Client(1.0)
-        with self.assertRaises(ValueError):
-            Client("*#")
-        with self.assertRaises(TypeError):
-            Client()
-        with self.assertRaises(ValueError):
-            Client("http:/www.example.com/")
-        with self.assertRaises(ValueError):
-            Client("httpx://www.example.com:9004")
-
-    def test_get_status(self):
-        self.client._service.get_status.return_value = "asdf"
-        self.assertEqual(self.client.get_status(), "asdf")
-
-    def test_query_timeout(self):
-        self.client.query_timeout = 5.0
-        self.assertEqual(self.client.query_timeout, 5.0)
-        self.assertEqual(self.client._service.query_timeout, 5.0)
-
-    def test_query(self):
-        self.client._service.query.return_value = "ok"
-
-        self.assertEqual(self.client.query("foo", 1, 2, 3), "ok")
-
-        self.client._service.query.assert_called_once_with("foo", 1, 2, 3)
-
-        self.client._service.query.reset_mock()
-
-        self.assertEqual(self.client.query("foo", a=1, b=2, c=3), "ok")
-
-        self.client._service.query.assert_called_once_with("foo", a=1, b=2, c=3)
-
-    def test_get_endpoints(self):
-        self.client._service.get_endpoints.return_value = "foo"
-
-        self.assertEqual(self.client.get_endpoints("foo"), "foo")
-
-        self.client._service.get_endpoints.assert_called_once_with("foo")
-
-    def test_get_endpoint_upload_destination(self):
-        self.client._service.get_endpoint_upload_destination.return_value = {
-            "path": "foo"
-        }
-
-        self.assertEqual(self.client._get_endpoint_upload_destination(), "foo")
-
-    def test_set_credentials(self):
-        username, password = "username", "password"
-        self.client.set_credentials(username, password)
-
-        self.client._service.set_credentials.assert_called_once_with(username, password)
-
-    def test_check_invalid_endpoint_name(self):
-        endpoint_name = "Invalid:model:@name"
-        with self.assertRaises(ValueError) as err:
-            _check_endpoint_name(endpoint_name)
-
-        self.assertEqual(
-            err.exception.args[0],
-            f"endpoint name {endpoint_name } can only contain: "
-            "a-z, A-Z, 0-9, underscore, hyphens and spaces.",
-        )
+import unittest
+from unittest.mock import Mock
+
+from tabpy.tabpy_tools.client import Client
+from tabpy.tabpy_tools.client import _check_endpoint_name
+
+
+class TestClient(unittest.TestCase):
+    def setUp(self):
+        self.client = Client("http://example.com/")
+        self.client._service = Mock()  # TODO: should spec this
+
+    def test_init(self):
+        client = Client("http://example.com:9004")
+
+        self.assertEqual(client._endpoint, "http://example.com:9004")
+
+        client = Client("http://example.com/", 10.0)
+
+        self.assertEqual(client._endpoint, "http://example.com/")
+
+        client = Client(endpoint="https://example.com/", query_timeout=-10.0)
+
+        self.assertEqual(client._endpoint, "https://example.com/")
+        self.assertEqual(client.query_timeout, 0.0)
+
+        # valid name tests
+        with self.assertRaises(ValueError):
+            Client("")
+        with self.assertRaises(TypeError):
+            Client(1.0)
+        with self.assertRaises(ValueError):
+            Client("*#")
+        with self.assertRaises(TypeError):
+            Client()
+        with self.assertRaises(ValueError):
+            Client("http:/www.example.com/")
+        with self.assertRaises(ValueError):
+            Client("httpx://www.example.com:9004")
+
+    def test_get_status(self):
+        self.client._service.get_status.return_value = "asdf"
+        self.assertEqual(self.client.get_status(), "asdf")
+
+    def test_query_timeout(self):
+        self.client.query_timeout = 5.0
+        self.assertEqual(self.client.query_timeout, 5.0)
+        self.assertEqual(self.client._service.query_timeout, 5.0)
+
+    def test_query(self):
+        self.client._service.query.return_value = "ok"
+
+        self.assertEqual(self.client.query("foo", 1, 2, 3), "ok")
+
+        self.client._service.query.assert_called_once_with("foo", 1, 2, 3)
+
+        self.client._service.query.reset_mock()
+
+        self.assertEqual(self.client.query("foo", a=1, b=2, c=3), "ok")
+
+        self.client._service.query.assert_called_once_with("foo", a=1, b=2, c=3)
+
+    def test_get_endpoints(self):
+        self.client._service.get_endpoints.return_value = "foo"
+
+        self.assertEqual(self.client.get_endpoints("foo"), "foo")
+
+        self.client._service.get_endpoints.assert_called_once_with("foo")
+
+    def test_get_endpoint_upload_destination(self):
+        self.client._service.get_endpoint_upload_destination.return_value = {
+            "path": "foo"
+        }
+
+        self.assertEqual(self.client._get_endpoint_upload_destination(), "foo")
+
+    def test_set_credentials(self):
+        username, password = "username", "password"
+        self.client.set_credentials(username, password)
+
+        self.client._service.set_credentials.assert_called_once_with(username, password)
+
+    def test_check_invalid_endpoint_name(self):
+        endpoint_name = "Invalid:model:@name"
+        with self.assertRaises(ValueError) as err:
+            _check_endpoint_name(endpoint_name)
+
+        self.assertEqual(
+            err.exception.args[0],
+            f"endpoint name {endpoint_name } can only contain: "
+            "a-z, A-Z, 0-9, underscore, hyphens and spaces.",
+        )
```

### Comparing `tabpy-2.6.0/tests/unit/tools_tests/test_rest_object.py` & `tabpy-2.7.0/tests/unit/tools_tests/test_rest_object.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import unittest
-import sys
-
-from tabpy.tabpy_tools.rest import RESTObject, RESTProperty, enum
-
-
-class TestRESTObject(unittest.TestCase):
-    def test_new_class(self):
-        class FooObject(RESTObject):
-            f = RESTProperty(float)
-            i = RESTProperty(int)
-            s = RESTProperty(str)
-            e = RESTProperty(enum("a", "b"))
-
-        f = FooObject(f="6.0", i="3", s="hello!")
-        self.assertEqual(f.f, 6.0)
-        self.assertEqual(f.i, 3)
-        self.assertEqual(f.s, "hello!")
-
-        with self.assertRaises(AttributeError):
-            f.e
-
-        self.assertEqual(f["f"], 6.0)
-        self.assertEqual(f["i"], 3)
-        self.assertEqual(f["s"], "hello!")
-
-        with self.assertRaises(KeyError):
-            f["e"]
-        with self.assertRaises(KeyError):
-            f["cat"]
-        with self.assertRaises(KeyError):
-            f["cat"] = 5
-
-        self.assertEqual(len(f), 3)
-        self.assertEqual(set(f), set(["f", "i", "s"]))
-        self.assertEqual(set(f.keys()), set(["f", "i", "s"]))
-        self.assertEqual(set(f.values()), set([6.0, 3, "hello!"]))
-        self.assertEqual(set(f.items()), set([("f", 6.0), ("i", 3), ("s", "hello!")]))
-
-        f.e = "a"
-        self.assertEqual(f.e, "a")
-        self.assertEqual(f["e"], "a")
-        f["e"] = "b"
-        self.assertEqual(f.e, "b")
-
-        with self.assertRaises(ValueError):
-            f.e = "fubar"
-
-        f.f = sys.float_info.max
-        self.assertEqual(f.f, sys.float_info.max)
-        f.f = float("inf")
-        self.assertEqual(f.f, float("inf"))
-        f.f = None
-        self.assertEqual(f.f, None)
-
-        class BarObject(FooObject):
-            x = RESTProperty(str)
-
-        f = BarObject(f="6.0", i="3", s="hello!", x="5")
-        self.assertEqual(f.f, 6.0)
-        self.assertEqual(f.i, 3)
-        self.assertEqual(f.s, "hello!")
-        self.assertEqual(f.x, "5")
+import unittest
+import sys
+
+from tabpy.tabpy_tools.rest import RESTObject, RESTProperty, enum
+
+
+class TestRESTObject(unittest.TestCase):
+    def test_new_class(self):
+        class FooObject(RESTObject):
+            f = RESTProperty(float)
+            i = RESTProperty(int)
+            s = RESTProperty(str)
+            e = RESTProperty(enum("a", "b"))
+
+        f = FooObject(f="6.0", i="3", s="hello!")
+        self.assertEqual(f.f, 6.0)
+        self.assertEqual(f.i, 3)
+        self.assertEqual(f.s, "hello!")
+
+        with self.assertRaises(AttributeError):
+            f.e
+
+        self.assertEqual(f["f"], 6.0)
+        self.assertEqual(f["i"], 3)
+        self.assertEqual(f["s"], "hello!")
+
+        with self.assertRaises(KeyError):
+            f["e"]
+        with self.assertRaises(KeyError):
+            f["cat"]
+        with self.assertRaises(KeyError):
+            f["cat"] = 5
+
+        self.assertEqual(len(f), 3)
+        self.assertEqual(set(f), set(["f", "i", "s"]))
+        self.assertEqual(set(f.keys()), set(["f", "i", "s"]))
+        self.assertEqual(set(f.values()), set([6.0, 3, "hello!"]))
+        self.assertEqual(set(f.items()), set([("f", 6.0), ("i", 3), ("s", "hello!")]))
+
+        f.e = "a"
+        self.assertEqual(f.e, "a")
+        self.assertEqual(f["e"], "a")
+        f["e"] = "b"
+        self.assertEqual(f.e, "b")
+
+        with self.assertRaises(ValueError):
+            f.e = "fubar"
+
+        f.f = sys.float_info.max
+        self.assertEqual(f.f, sys.float_info.max)
+        f.f = float("inf")
+        self.assertEqual(f.f, float("inf"))
+        f.f = None
+        self.assertEqual(f.f, None)
+
+        class BarObject(FooObject):
+            x = RESTProperty(str)
+
+        f = BarObject(f="6.0", i="3", s="hello!", x="5")
+        self.assertEqual(f.f, 6.0)
+        self.assertEqual(f.i, 3)
+        self.assertEqual(f.s, "hello!")
+        self.assertEqual(f.x, "5")
```

