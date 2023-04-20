# Comparing `tmp/vetiver-0.2.0.tar.gz` & `tmp/vetiver-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vetiver-0.2.0.tar", last modified: Wed Jan 25 17:22:47 2023, max compression
+gzip compressed data, was "vetiver-0.2.1.tar", last modified: Thu Apr 20 16:36:50 2023, max compression
```

## Comparing `vetiver-0.2.0.tar` & `vetiver-0.2.1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.454563 vetiver-0.2.0/
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.437631 vetiver-0.2.0/.github/
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.441420 vetiver-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      834 2022-11-14 21:49:09.000000 vetiver-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      595 2022-11-14 21:49:09.000000 vetiver-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      255 2022-11-14 21:49:09.000000 vetiver-0.2.0/.github/ISSUE_TEMPLATE/release-checklist.md
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.441970 vetiver-0.2.0/.github/workflows/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1544 2023-01-20 15:55:32.000000 vetiver-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      322 2022-11-14 21:49:09.000000 vetiver-0.2.0/.github/workflows/precommit.yml
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3263 2023-01-25 17:05:36.000000 vetiver-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4895 2023-01-23 19:10:01.000000 vetiver-0.2.0/.github/workflows/weekly.yml
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1953 2022-11-14 21:49:09.000000 vetiver-0.2.0/.gitignore
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      571 2022-11-14 21:49:09.000000 vetiver-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     5216 2022-11-14 21:49:09.000000 vetiver-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1083 2022-11-14 21:49:09.000000 vetiver-0.2.0/LICENSE
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)        0 2022-11-14 21:49:09.000000 vetiver-0.2.0/MANIFEST.in
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2711 2023-01-25 17:22:24.000000 vetiver-0.2.0/Makefile
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4028 2023-01-25 17:22:47.454695 vetiver-0.2.0/PKG-INFO
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3374 2023-01-23 19:10:01.000000 vetiver-0.2.0/README.md
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      494 2022-11-28 21:56:39.000000 vetiver-0.2.0/docker-compose.yml
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.442243 vetiver-0.2.0/docs/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      639 2022-11-14 21:49:09.000000 vetiver-0.2.0/docs/Makefile
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.442801 vetiver-0.2.0/docs/figures/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)   482544 2022-11-14 21:49:09.000000 vetiver-0.2.0/docs/figures/logo.png
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)    19004 2022-11-14 21:49:09.000000 vetiver-0.2.0/docs/figures/logo.svg
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      800 2022-11-14 21:49:09.000000 vetiver-0.2.0/docs/make.bat
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.443115 vetiver-0.2.0/docs/source/
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.443259 vetiver-0.2.0/docs/source/advancedusage/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1953 2023-01-23 19:10:01.000000 vetiver-0.2.0/docs/source/advancedusage/custom_handler.md
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2256 2022-11-28 21:56:34.000000 vetiver-0.2.0/docs/source/conf.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1958 2022-12-19 16:34:48.000000 vetiver-0.2.0/docs/source/index.rst
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.444803 vetiver-0.2.0/docs/source/reference/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      328 2023-01-20 15:55:32.000000 vetiver-0.2.0/docs/source/reference/vetiver.VetiverAPI.rst
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      109 2023-01-20 15:55:32.000000 vetiver-0.2.0/docs/source/reference/vetiver.VetiverAPI.run.rst
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      138 2023-01-20 15:55:32.000000 vetiver-0.2.0/docs/source/reference/vetiver.VetiverAPI.vetiver_post.rst
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      208 2023-01-20 15:55:32.000000 vetiver-0.2.0/docs/source/reference/vetiver.VetiverModel.rst
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)       98 2023-01-20 15:55:32.000000 vetiver-0.2.0/docs/source/reference/vetiver.load_pkgs.rst
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      170 2022-11-28 21:56:34.000000 vetiver-0.2.0/docs/source/reference/vetiver.pin_read_write.vetiver_pin_read.rst
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      173 2022-11-28 21:56:34.000000 vetiver-0.2.0/docs/source/reference/vetiver.pin_read_write.vetiver_pin_write.rst
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)       90 2023-01-20 15:55:32.000000 vetiver-0.2.0/docs/source/reference/vetiver.predict.rst
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      119 2023-01-20 15:55:32.000000 vetiver-0.2.0/docs/source/reference/vetiver.vetiver_endpoint.rst
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      124 2022-11-28 21:56:34.000000 vetiver-0.2.0/docs/source/reference/vetiver.vetiver_write_app.rst
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      133 2022-11-28 21:56:34.000000 vetiver-0.2.0/docs/source/reference/vetiver.vetiver_write_docker.rst
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.444948 vetiver-0.2.0/examples/
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.445376 vetiver-0.2.0/examples/coffeeratings/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      352 2022-11-14 21:49:09.000000 vetiver-0.2.0/examples/coffeeratings/Dockerfile
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      287 2022-11-14 21:49:09.000000 vetiver-0.2.0/examples/coffeeratings/app.py
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.438403 vetiver-0.2.0/examples/coffeeratings/v/
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.445649 vetiver-0.2.0/examples/coffeeratings/v/20220415T174503Z-06d9b/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      455 2022-11-14 21:49:09.000000 vetiver-0.2.0/examples/coffeeratings/v/20220415T174503Z-06d9b/data.txt
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1035 2022-11-14 21:49:09.000000 vetiver-0.2.0/examples/coffeeratings/v/20220415T174503Z-06d9b/v.joblib
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1566 2022-11-14 21:49:09.000000 vetiver-0.2.0/examples/coffeeratings/vetiver_requirements.txt
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1649 2022-11-14 21:49:09.000000 vetiver-0.2.0/examples/coffeeratings.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      443 2022-12-13 18:42:30.000000 vetiver-0.2.0/pyproject.toml
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.445785 vetiver-0.2.0/requirements/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3290 2022-11-14 21:49:09.000000 vetiver-0.2.0/requirements/dev.txt
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.438728 vetiver-0.2.0/script/
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.446080 vetiver-0.2.0/script/setup-docker/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)       53 2022-12-05 15:40:50.000000 vetiver-0.2.0/script/setup-docker/.gitignore
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      343 2022-12-19 21:08:29.000000 vetiver-0.2.0/script/setup-docker/docker.py
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.446649 vetiver-0.2.0/script/setup-rsconnect/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      122 2022-11-14 21:49:09.000000 vetiver-0.2.0/script/setup-rsconnect/add-users.sh
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      505 2022-11-14 21:49:09.000000 vetiver-0.2.0/script/setup-rsconnect/dump_api_keys.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      466 2022-11-28 21:56:39.000000 vetiver-0.2.0/script/setup-rsconnect/rstudio-connect.gcfg
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)       48 2022-11-14 21:49:09.000000 vetiver-0.2.0/script/setup-rsconnect/users.txt
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1138 2023-01-25 17:22:47.455103 vetiver-0.2.0/setup.cfg
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)       39 2022-11-14 21:49:09.000000 vetiver-0.2.0/setup.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)       93 2022-11-14 21:49:09.000000 vetiver-0.2.0/tox.ini
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.448904 vetiver-0.2.0/vetiver/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1321 2023-01-25 17:05:36.000000 vetiver-0.2.0/vetiver/__init__.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1079 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/attach_pkgs.py
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.450468 vetiver-0.2.0/vetiver/data/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      521 2022-11-14 21:49:09.000000 vetiver-0.2.0/vetiver/data/__init__.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)   181099 2022-11-14 21:49:09.000000 vetiver-0.2.0/vetiver/data/chicago.csv
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1281 2022-11-14 21:49:09.000000 vetiver-0.2.0/vetiver/data/mtcars.csv
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     5103 2022-11-14 21:49:09.000000 vetiver-0.2.0/vetiver/data/sacramento.csv
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.451490 vetiver-0.2.0/vetiver/handlers/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)        0 2022-11-14 21:49:09.000000 vetiver-0.2.0/vetiver/handlers/__init__.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4115 2023-01-25 17:05:36.000000 vetiver-0.2.0/vetiver/handlers/base.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1090 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/handlers/sklearn.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1278 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/handlers/statsmodels.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1355 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/handlers/torch.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1371 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/handlers/xgboost.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1107 2023-01-25 17:05:41.000000 vetiver-0.2.0/vetiver/meta.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      680 2023-01-13 15:40:59.000000 vetiver-0.2.0/vetiver/mock.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      461 2022-11-14 21:49:09.000000 vetiver-0.2.0/vetiver/model_card.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     7852 2023-01-25 17:05:36.000000 vetiver-0.2.0/vetiver/monitor.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3211 2023-01-25 17:05:41.000000 vetiver-0.2.0/vetiver/pin_read_write.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4782 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/prototype.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3268 2023-01-25 17:05:36.000000 vetiver-0.2.0/vetiver/rsconnect.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)    10258 2023-01-25 17:05:36.000000 vetiver-0.2.0/vetiver/server.py
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.451621 vetiver-0.2.0/vetiver/templates/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3821 2022-11-14 21:49:09.000000 vetiver-0.2.0/vetiver/templates/model_card.qmd
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.454256 vetiver-0.2.0/vetiver/tests/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      136 2022-11-14 21:49:09.000000 vetiver-0.2.0/vetiver/tests/rsconnect_api_keys.json
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.454437 vetiver-0.2.0/vetiver/tests/snapshots/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      616 2022-11-14 21:49:09.000000 vetiver-0.2.0/vetiver/tests/snapshots/test_monitor.json
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1838 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/tests/test_add_endpoint.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      605 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/tests/test_build_api.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4657 2023-01-25 17:05:41.000000 vetiver-0.2.0/vetiver/tests/test_build_vetiver_model.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1894 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/tests/test_custom_handler.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      311 2022-11-14 21:49:09.000000 vetiver-0.2.0/vetiver/tests/test_mock_data.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4086 2022-11-14 21:49:09.000000 vetiver-0.2.0/vetiver/tests/test_monitor.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      416 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/tests/test_no_handler.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      883 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/tests/test_pin_write.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      802 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/tests/test_ping_server.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2772 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/tests/test_predict.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      452 2022-12-13 18:42:30.000000 vetiver-0.2.0/vetiver/tests/test_prepare_docker.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3441 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/tests/test_pytorch.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2711 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/tests/test_rsconnect.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2792 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/tests/test_sklearn.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1949 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/tests/test_statsmodels.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1012 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/tests/test_write_app.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1842 2022-12-05 15:40:50.000000 vetiver-0.2.0/vetiver/tests/test_write_docker.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2339 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/tests/test_xgboost.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      232 2023-01-23 19:10:01.000000 vetiver-0.2.0/vetiver/types.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      642 2022-11-14 21:49:09.000000 vetiver-0.2.0/vetiver/utils.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4227 2023-01-25 17:05:41.000000 vetiver-0.2.0/vetiver/vetiver_model.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3627 2023-01-25 17:05:36.000000 vetiver-0.2.0/vetiver/write_docker.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2919 2023-01-25 17:05:36.000000 vetiver-0.2.0/vetiver/write_fastapi.py
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-01-25 17:22:47.449740 vetiver-0.2.0/vetiver.egg-info/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4028 2023-01-25 17:22:47.000000 vetiver-0.2.0/vetiver.egg-info/PKG-INFO
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3057 2023-01-25 17:22:47.000000 vetiver-0.2.0/vetiver.egg-info/SOURCES.txt
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)        1 2023-01-25 17:22:47.000000 vetiver-0.2.0/vetiver.egg-info/dependency_links.txt
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      400 2023-01-25 17:22:47.000000 vetiver-0.2.0/vetiver.egg-info/requires.txt
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)        8 2023-01-25 17:22:47.000000 vetiver-0.2.0/vetiver.egg-info/top_level.txt
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.917091 vetiver-0.2.1/
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.888528 vetiver-0.2.1/.github/
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.895044 vetiver-0.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      834 2023-03-30 20:56:23.000000 vetiver-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      595 2023-03-30 20:56:23.000000 vetiver-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      255 2023-03-30 20:56:23.000000 vetiver-0.2.1/.github/ISSUE_TEMPLATE/release-checklist.md
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.896403 vetiver-0.2.1/.github/workflows/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3726 2023-04-12 18:18:16.000000 vetiver-0.2.1/.github/workflows/docs.yml
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      322 2023-03-30 20:56:23.000000 vetiver-0.2.1/.github/workflows/precommit.yml
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3962 2023-04-12 18:18:16.000000 vetiver-0.2.1/.github/workflows/tests.yml
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4901 2023-03-30 20:56:23.000000 vetiver-0.2.1/.github/workflows/weekly.yml
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1964 2023-03-30 20:56:23.000000 vetiver-0.2.1/.gitignore
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      592 2023-03-30 20:56:23.000000 vetiver-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     5243 2023-03-30 20:56:23.000000 vetiver-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1082 2023-03-30 20:56:23.000000 vetiver-0.2.1/LICENSE
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      419 2023-03-30 20:56:23.000000 vetiver-0.2.1/MAINTAINERS.md
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)        0 2023-03-30 20:56:23.000000 vetiver-0.2.1/MANIFEST.in
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2333 2023-04-12 18:18:16.000000 vetiver-0.2.1/Makefile
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4197 2023-04-20 16:36:50.917206 vetiver-0.2.1/PKG-INFO
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3444 2023-04-20 16:33:43.000000 vetiver-0.2.1/README.md
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      494 2023-03-30 20:56:23.000000 vetiver-0.2.1/docker-compose.yml
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.897817 vetiver-0.2.1/docs/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)       87 2023-03-30 20:56:23.000000 vetiver-0.2.1/docs/.gitignore
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      213 2023-04-12 18:18:16.000000 vetiver-0.2.1/docs/Makefile
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.888783 vetiver-0.2.1/docs/_extensions/
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.888860 vetiver-0.2.1/docs/_extensions/machow/
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.899755 vetiver-0.2.1/docs/_extensions/machow/interlinks/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)       22 2023-03-30 20:56:23.000000 vetiver-0.2.1/docs/_extensions/machow/interlinks/.gitignore
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      654 2023-03-30 20:56:23.000000 vetiver-0.2.1/docs/_extensions/machow/interlinks/README.md
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      125 2023-03-30 20:56:23.000000 vetiver-0.2.1/docs/_extensions/machow/interlinks/_extension.yml
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      997 2023-03-30 20:56:23.000000 vetiver-0.2.1/docs/_extensions/machow/interlinks/example.qmd
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     7534 2023-03-30 20:56:23.000000 vetiver-0.2.1/docs/_extensions/machow/interlinks/interlinks.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      447 2023-03-30 20:56:23.000000 vetiver-0.2.1/docs/_extensions/machow/interlinks/objects_siuba.json
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      970 2023-03-30 20:56:23.000000 vetiver-0.2.1/docs/_extensions/machow/interlinks/objects_vetiver.inv
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)    11583 2023-03-30 20:56:23.000000 vetiver-0.2.1/docs/_extensions/machow/interlinks/objects_vetiver.json
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2326 2023-04-20 16:33:43.000000 vetiver-0.2.1/docs/_quarto.yml
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4588 2023-03-30 20:56:23.000000 vetiver-0.2.1/docs/changelog.md
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1953 2023-03-30 20:56:23.000000 vetiver-0.2.1/docs/custom_handler.md
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.900900 vetiver-0.2.1/docs/figures/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)   173095 2023-03-30 20:56:23.000000 vetiver-0.2.1/docs/figures/logo.png
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)    19004 2023-03-30 20:56:23.000000 vetiver-0.2.1/docs/figures/logo.svg
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3400 2023-04-20 16:33:43.000000 vetiver-0.2.1/docs/index.qmd
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      135 2023-03-30 20:56:23.000000 vetiver-0.2.1/docs/version_config.py
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.901269 vetiver-0.2.1/examples/
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.901980 vetiver-0.2.1/examples/coffeeratings/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      352 2023-03-30 20:56:23.000000 vetiver-0.2.1/examples/coffeeratings/Dockerfile
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      287 2023-03-30 20:56:23.000000 vetiver-0.2.1/examples/coffeeratings/app.py
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.889282 vetiver-0.2.1/examples/coffeeratings/v/
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.902404 vetiver-0.2.1/examples/coffeeratings/v/20220415T174503Z-06d9b/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      455 2023-03-30 20:56:23.000000 vetiver-0.2.1/examples/coffeeratings/v/20220415T174503Z-06d9b/data.txt
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1035 2023-03-30 20:56:23.000000 vetiver-0.2.1/examples/coffeeratings/v/20220415T174503Z-06d9b/v.joblib
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1566 2023-03-30 20:56:23.000000 vetiver-0.2.1/examples/coffeeratings/vetiver_requirements.txt
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1649 2023-03-30 20:56:23.000000 vetiver-0.2.1/examples/coffeeratings.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2723 2023-04-12 18:18:16.000000 vetiver-0.2.1/pyproject.toml
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.889529 vetiver-0.2.1/script/
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.902748 vetiver-0.2.1/script/setup-docker/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)       53 2023-03-30 20:56:23.000000 vetiver-0.2.1/script/setup-docker/.gitignore
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      343 2023-03-30 20:56:23.000000 vetiver-0.2.1/script/setup-docker/docker.py
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.903580 vetiver-0.2.1/script/setup-rsconnect/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      122 2023-03-30 20:56:23.000000 vetiver-0.2.1/script/setup-rsconnect/add-users.sh
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      505 2023-03-30 20:56:23.000000 vetiver-0.2.1/script/setup-rsconnect/dump_api_keys.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      466 2023-03-30 20:56:23.000000 vetiver-0.2.1/script/setup-rsconnect/rstudio-connect.gcfg
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)       48 2023-03-30 20:56:23.000000 vetiver-0.2.1/script/setup-rsconnect/users.txt
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1225 2023-04-20 16:36:50.917650 vetiver-0.2.1/setup.cfg
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)       39 2023-03-30 20:56:23.000000 vetiver-0.2.1/setup.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)       93 2023-03-30 20:55:52.000000 vetiver-0.2.1/tox.ini
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.907754 vetiver-0.2.1/vetiver/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1430 2023-04-20 16:33:43.000000 vetiver-0.2.1/vetiver/__init__.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1972 2023-04-12 18:18:16.000000 vetiver-0.2.1/vetiver/attach_pkgs.py
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.910354 vetiver-0.2.1/vetiver/data/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      521 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/data/__init__.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)   181099 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/data/chicago.csv
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1281 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/data/mtcars.csv
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     5103 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/data/sacramento.csv
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.911921 vetiver-0.2.1/vetiver/handlers/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)        0 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/handlers/__init__.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4076 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/handlers/base.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1099 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/handlers/sklearn.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2420 2023-04-20 16:33:43.000000 vetiver-0.2.1/vetiver/handlers/spacy.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1287 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/handlers/statsmodels.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1335 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/handlers/torch.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1397 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/handlers/xgboost.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1186 2023-04-20 16:33:43.000000 vetiver-0.2.1/vetiver/helpers.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1351 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/meta.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      680 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/mock.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      467 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/model_card.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     7858 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/monitor.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3384 2023-04-12 18:18:16.000000 vetiver-0.2.1/vetiver/pin_read_write.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4782 2023-04-12 18:12:42.000000 vetiver-0.2.1/vetiver/prototype.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3342 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/rsconnect.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)    10327 2023-04-20 16:33:43.000000 vetiver-0.2.1/vetiver/server.py
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.912142 vetiver-0.2.1/vetiver/templates/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3821 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/templates/model_card.qmd
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.916727 vetiver-0.2.1/vetiver/tests/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      136 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/rsconnect_api_keys.json
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.916924 vetiver-0.2.1/vetiver/tests/snapshots/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      616 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/snapshots/test_monitor.json
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1929 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/test_add_endpoint.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      605 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/test_build_api.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     5308 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/test_build_vetiver_model.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1894 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/test_custom_handler.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      311 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/test_mock_data.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4086 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/test_monitor.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      416 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/test_no_handler.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      874 2023-04-12 18:18:16.000000 vetiver-0.2.1/vetiver/tests/test_pin_write.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1679 2023-04-12 18:18:16.000000 vetiver-0.2.1/vetiver/tests/test_prepare_docker.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3285 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/test_pytorch.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2711 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/test_rsconnect.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1189 2023-04-20 16:33:43.000000 vetiver-0.2.1/vetiver/tests/test_server.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2570 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/test_sklearn.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     5161 2023-04-20 16:33:43.000000 vetiver-0.2.1/vetiver/tests/test_spacy.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1949 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/test_statsmodels.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1136 2023-04-12 18:18:16.000000 vetiver-0.2.1/vetiver/tests/test_write_app.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1842 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/test_write_docker.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2339 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/tests/test_xgboost.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      232 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/types.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      642 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/utils.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4028 2023-04-12 18:18:16.000000 vetiver-0.2.1/vetiver/vetiver_model.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4274 2023-04-12 18:18:16.000000 vetiver-0.2.1/vetiver/write_docker.py
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2919 2023-03-30 20:56:23.000000 vetiver-0.2.1/vetiver/write_fastapi.py
+drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2023-04-20 16:36:50.908805 vetiver-0.2.1/vetiver.egg-info/
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4197 2023-04-20 16:36:50.000000 vetiver-0.2.1/vetiver.egg-info/PKG-INFO
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2927 2023-04-20 16:36:50.000000 vetiver-0.2.1/vetiver.egg-info/SOURCES.txt
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)        1 2023-04-20 16:36:50.000000 vetiver-0.2.1/vetiver.egg-info/dependency_links.txt
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)      480 2023-04-20 16:36:50.000000 vetiver-0.2.1/vetiver.egg-info/requires.txt
+-rw-r--r--   0 isabelzimmerman   (501) staff       (20)        8 2023-04-20 16:36:50.000000 vetiver-0.2.1/vetiver.egg-info/top_level.txt
```

### Comparing `vetiver-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `vetiver-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `vetiver-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/.github/workflows/weekly.yml` & `vetiver-0.2.1/.github/workflows/weekly.yml`

 * *Files 4% similar despite different names*

```diff
@@ -5,41 +5,43 @@
 #   2. main branch version
 
 name: Weekly Tests
 
 on:
   schedule:
     - cron: "03 14 * * MON"
+  push:
+    branches: ['update-weekly']
 
 jobs:
   vetiver_main_pins_main:
     name: 'vetiver main, pins main'
     if: github.repository == 'rstudio/vetiver-python'
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
         # Minimum and Maximum supported versions
         python-version: ['3.10']
 
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install '.[all]'
           python -m pip install --upgrade git+https://github.com/rstudio/pins-python
 
-      - name: run RStudio Connect
+      - name: run Connect
         run: |
           docker-compose up --build -d
           make dev
         env:
           RSC_LICENSE: ${{ secrets.RSC_LICENSE }}
           GITHUB_TOKEN: ${{secrets.GITHUB_TOKEN}}
 
@@ -68,25 +70,25 @@
           echo ${{ steps.latestrelease.outputs.releasetag }}
 
       - name: Checkout Code
         uses: actions/checkout@v3
         with:
           ref: ${{ steps.latestrelease.outputs.releasetag }}
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install .[dev]
           python -m pip install --upgrade git+https://github.com/rstudio/pins-python
 
-      - name: run RStudio Connect
+      - name: run Connect
         run: |
           docker-compose up --build -d
           make dev
         env:
           RSC_LICENSE: ${{ secrets.RSC_LICENSE }}
           GITHUB_TOKEN: ${{secrets.GITHUB_TOKEN}}
 
@@ -97,15 +99,15 @@
   vetiver_pypi_rsconnect_latest:
     name: 'vetiver pypi, rsconnect latest'
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
         # Minimum and Maximum supported versions
-        python-version: ['3.10']
+        python-version: ['3.9']
 
     steps:
       - name: Get latest release with tag from GitHub API
         id: latestrelease
         run: |
           echo "::set-output name=releasetag::$(curl -s https://api.github.com/repos/rstudio/vetiver-python/releases/latest | jq '.tag_name' | sed 's/\"//g')"
 
@@ -114,26 +116,26 @@
           echo ${{ steps.latestrelease.outputs.releasetag }}
 
       - name: Checkout Code
         uses: actions/checkout@v3
         with:
           ref: ${{ steps.latestrelease.outputs.releasetag }}
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install .[dev]
           python -m pip install --upgrade git+https://github.com/rstudio/rsconnect-python
           pip freeze > requirements.txt
 
-      - name: run RStudio Connect
+      - name: run Connect
         run: |
           docker-compose up --build -d
           make dev
         env:
           RSC_LICENSE: ${{ secrets.RSC_LICENSE }}
           GITHUB_TOKEN: ${{secrets.GITHUB_TOKEN}}
 
@@ -144,31 +146,31 @@
   vetiver_latest_rsconnect_latest:
     name: 'vetiver latest, rsconnect latest'
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
         # Minimum and Maximum supported versions
-        python-version: ['3.10']
+        python-version: ['3.9']
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install '.[all]'
           python -m pip install --upgrade git+https://github.com/rstudio/rsconnect-python
           pip freeze > requirements.txt
 
-      - name: run RStudio Connect
+      - name: run Connect
         run: |
           docker-compose up --build -d
           make dev
         env:
           RSC_LICENSE: ${{ secrets.RSC_LICENSE }}
           GITHUB_TOKEN: ${{secrets.GITHUB_TOKEN}}
```

### Comparing `vetiver-0.2.0/.gitignore` & `vetiver-0.2.1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -138,7 +138,9 @@
 .pyre/
 
 NOTES.md
 
 ## RStudio
 *.Rproj
 .Rproj.user
+
+/.quarto/
```

### Comparing `vetiver-0.2.0/.pre-commit-config.yaml` & `vetiver-0.2.1/.pre-commit-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 
-exclude: "(.*\\.csv)|(^examples/)|(^vetiver/tests/snapshots/)"
+exclude: "(.*\\.csv)|(^examples/)|(^vetiver/tests/snapshots/)|(^docs/_extensions/)"
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v2.4.0
     hooks:
       - id: flake8
         # line too long and line before binary operator (black is ok with these)
         types:
```

### Comparing `vetiver-0.2.0/CODE_OF_CONDUCT.md` & `vetiver-0.2.1/CODE_OF_CONDUCT.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,69 +2,69 @@
 
 ## Our Pledge
 
 We as members, contributors, and leaders pledge to make participation in our
 community a harassment-free experience for everyone, regardless of age, body
 size, visible or invisible disability, ethnicity, sex characteristics, gender
 identity and expression, level of experience, education, socio-economic status,
-nationality, personal appearance, race, religion, or sexual identity and
-orientation.
+nationality, personal appearance, race, caste, color, religion, or sexual
+identity and orientation.
 
 We pledge to act and interact in ways that contribute to an open, welcoming,
 diverse, inclusive, and healthy community.
 
 ## Our Standards
 
 Examples of behavior that contributes to a positive environment for our
 community include:
 
 * Demonstrating empathy and kindness toward other people
 * Being respectful of differing opinions, viewpoints, and experiences
 * Giving and gracefully accepting constructive feedback
 * Accepting responsibility and apologizing to those affected by our mistakes,
-and learning from the experience
+  and learning from the experience
 * Focusing on what is best not just for us as individuals, but for the overall
-community
+  community
 
 Examples of unacceptable behavior include:
 
-* The use of sexualized language or imagery, and sexual attention or
-advances of any kind
+* The use of sexualized language or imagery, and sexual attention or advances of
+  any kind
 * Trolling, insulting or derogatory comments, and personal or political attacks
 * Public or private harassment
-* Publishing others' private information, such as a physical or email
-address, without their explicit permission
+* Publishing others' private information, such as a physical or email address,
+  without their explicit permission
 * Other conduct which could reasonably be considered inappropriate in a
-professional setting
+  professional setting
 
 ## Enforcement Responsibilities
 
-Community leaders are responsible for clarifying and enforcing our standards
-of acceptable behavior and will take appropriate and fair corrective action in
+Community leaders are responsible for clarifying and enforcing our standards of
+acceptable behavior and will take appropriate and fair corrective action in
 response to any behavior that they deem inappropriate, threatening, offensive,
 or harmful.
 
 Community leaders have the right and responsibility to remove, edit, or reject
 comments, commits, code, wiki edits, issues, and other contributions that are
 not aligned to this Code of Conduct, and will communicate reasons for moderation
 decisions when appropriate.
 
 ## Scope
 
-This Code of Conduct applies within all community spaces, and also applies
-when an individual is officially representing the community in public spaces.
-Examples of representing our community include using an official e-mail
-address, posting via an official social media account, or acting as an appointed
+This Code of Conduct applies within all community spaces, and also applies when
+an individual is officially representing the community in public spaces.
+Examples of representing our community include using an official e-mail address,
+posting via an official social media account, or acting as an appointed
 representative at an online or offline event.
 
 ## Enforcement
 
 Instances of abusive, harassing, or otherwise unacceptable behavior may be
-reported to the community leaders responsible for enforcement at [INSERT CONTACT
-METHOD]. All complaints will be reviewed and investigated promptly and fairly.
+reported to the community leaders responsible for enforcement at codeofconduct@posit.co.
+All complaints will be reviewed and investigated promptly and fairly.
 
 All community leaders are obligated to respect the privacy and security of the
 reporter of any incident.
 
 ## Enforcement Guidelines
 
 Community leaders will follow these Community Impact Guidelines in determining
@@ -110,19 +110,17 @@
 
 **Consequence**: A permanent ban from any sort of public interaction within the
 community.
 
 ## Attribution
 
 This Code of Conduct is adapted from the [Contributor Covenant][homepage],
-version 2.0,
-available at https://www.contributor-covenant.org/version/2/0/
-code_of_conduct.html.
+version 2.1, available at
+<https://www.contributor-covenant.org/version/2/1/code_of_conduct.html>.
 
-Community Impact Guidelines were inspired by [Mozilla's code of conduct
-enforcement ladder](https://github.com/mozilla/diversity).
-
-[homepage]: https://www.contributor-covenant.org
+Community Impact Guidelines were inspired by
+[Mozilla's code of conduct enforcement ladder][https://github.com/mozilla/inclusion].
 
 For answers to common questions about this code of conduct, see the FAQ at
-https://www.contributor-covenant.org/faq. Translations are available at https://
-www.contributor-covenant.org/translations.
+<https://www.contributor-covenant.org/faq>. Translations are available at <https://www.contributor-covenant.org/translations>.
+
+[homepage]: https://www.contributor-covenant.org
```

### Comparing `vetiver-0.2.0/LICENSE` & `vetiver-0.2.1/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021 Isabel Zimmerman
+Copyright (c) 2021 vetiver authors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `vetiver-0.2.0/Makefile` & `vetiver-0.2.1/Makefile`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 .PHONY: clean-pyc clean-build clean docs
 UNAME := $(shell uname)
 
-SPHINX_BUILDARGS=
-# Note that these are keys generated by the docker rsconnect service, so are
-# not really secrets. They are saved to json to make it easy to use rsconnect
-# as multiple users from the tests
 RSC_API_KEYS=vetiver/tests/rsconnect_api_keys.json
 
 ifeq ($(UNAME), Darwin)
     BROWSER := open
 else
     BROWSER := python -mwebbrowser
 endif
@@ -18,24 +14,23 @@
 	@echo "clean-build - remove build artifacts"
 	@echo "clean-pyc - remove Python file artifacts"
 	@echo "clean-test - remove test and coverage artifacts"
 	@echo "lint - check style with flake8"
 	@echo "test - run tests quickly with the default Python"
 	@echo "test-rsc - run tests for rsconnect"
 	@echo "coverage - check code coverage quickly with the default Python"
-	@echo "docs - generate Sphinx HTML documentation, including API docs"
-	@echo "cdocs - cleanout previous build & generate Sphinx HTML documentation, including API docs"
+	@echo "docs - generate HTML documentation, including API docs"
 	@echo "release - package and upload a release"
 	@echo "dist - package"
 	@echo "install - install the package to the active Python's site-packages"
-	@echo "dev - generate RStudio Connect API keys"
-	@echo "dev-start - start up development RStudio Connect in Docker"
-	@echo "dev-stop - stop RStudio Connect dev container"
+	@echo "dev - generate Connect API keys"
+	@echo "dev-start - start up development Connect in Docker"
+	@echo "dev-stop - stop Connect dev container"
 
-clean: clean-build clean-pyc clean-test docs-clean
+clean: clean-build clean-pyc clean-test
 
 clean-build:
 	rm -fr build/
 	rm -fr dist/
 	rm -fr .eggs/
 	find . -name '*.egg-info' -exec rm -fr {} +
 	find . -name '*.egg' -exec rm -f {} +
@@ -53,30 +48,27 @@
 
 lint:
 	flake8 vetiver
 
 test: clean-test
 	pytest -m 'not rsc_test and not docker'
 
+test-pdb: clean-test
+	pytest -m 'not rsc_test and not docker' --pdb
+
 test-rsc: clean-test
 	pytest
 
 coverage:
 	coverage report -m
 	coverage html
 	$(BROWSER) htmlcov/index.html
 
-cdocs cdoc cdocumentation: docs-clean docs
-
-docs-clean:
-	$(MAKE) -C docs clean
-
 docs doc documentation:
-	$(MAKE) -C docs html
-	$(BROWSER) docs/_build/html/index.html
+	$(MAKE) -C docs docs
 
 release: dist
 	twine upload dist/*
 
 dist: clean
 	python setup.py sdist
 
@@ -95,9 +87,12 @@
 	sleep 5
 	curl -s --retry 10 --retry-connrefused http://localhost:3939
 
 dev-stop:
 	docker-compose down
 	rm -f $(RSC_API_KEYS)
 
+typecheck:
+	pyright
+
 $(RSC_API_KEYS): dev-start
 	python script/setup-rsconnect/dump_api_keys.py $@
```

### Comparing `vetiver-0.2.0/PKG-INFO` & `vetiver-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: vetiver
-Version: 0.2.0
-Summary: Deploy models into REST endpoints
-Home-page: https://github.com/isabelizimm/vetiver-python
+Version: 0.2.1
+Summary: Version, share, deploy, and monitor models.
+Home-page: https://github.com/rstudio/vetiver-python
 Author: Isabel Zimmerman
-Author-email: isabel.zimmerman@rstudio.com
+Author-email: isabel.zimmerman@posit.co
 License: MIT
 Keywords: data,mlops
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
+Provides-Extra: all_models
 Provides-Extra: dev
-Provides-Extra: torch
+Provides-Extra: docs
 Provides-Extra: statsmodels
+Provides-Extra: torch
 Provides-Extra: xgboost
+Provides-Extra: spacy
+Provides-Extra: typecheck
 License-File: LICENSE
 
-# vetiver <a href='https://rstudio.github.io/vetiver-python/'><img src='docs/figures/logo.png' align="right" height="139" /></a>
+# vetiver <a href='https://rstudio.github.io/vetiver-python/'><img src='docs/figures/logo.png' align="right" height="138" /></a>
 
 <!-- badges: start -->
 
 [![Lifecycle:
 experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental) [![codecov](https://codecov.io/gh/isabelizimm/vetiver-python/branch/main/graph/badge.svg?token=CW6JHVS6ZX)](https://codecov.io/gh/isabelizimm/vetiver-python)
 
 <!-- badges: end -->
@@ -38,14 +42,15 @@
 
 You can use vetiver with:
 
 -   [scikit-learn](https://scikit-learn.org/)
 -   [torch](https://pytorch.org/)
 -   [statsmodels](https://www.statsmodels.org/stable/index.html)
 -   [xgboost](https://xgboost.readthedocs.io/en/stable/)
+-   [spacy](https://spacy.io/)
 -   or utilize [custom handlers](https://rstudio.github.io/vetiver-python/stable/advancedusage/custom_handler.html) to support your own models!
 
 ## Installation
 
 You can install the released version of vetiver from [PyPI](https://pypi.org/project/vetiver/):
 
 ```python
@@ -67,15 +72,15 @@
 
 X, y = mock.get_mock_data()
 model = mock.get_mock_model().fit(X, y)
 
 v = VetiverModel(model, model_name='mock_model', prototype_data=X)
 ```
 
-You can **version** and **share** your `VetiverModel()` by choosing a [pins](https://rstudio.github.io/pins-python/) "board" for it, including a local folder, RStudio Connect, Amazon S3, and more.
+You can **version** and **share** your `VetiverModel()` by choosing a [pins](https://rstudio.github.io/pins-python/) "board" for it, including a local folder, [Connect](https://posit.co/products/enterprise/connect/), Amazon S3, and more.
 
 ```python
 from pins import board_temp
 from vetiver import vetiver_pin_write
 
 model_board = board_temp(versioned = True, allow_pickle_read = True)
 vetiver_pin_write(model_board, v)
@@ -90,10 +95,10 @@
 
 To start a server using this object, use `app.run(port = 8080)` or your port of choice.
 
 ## Contributing
 
 This project is released with a [Contributor Code of Conduct](https://www.contributor-covenant.org/version/2/1/CODE_OF_CONDUCT.html). By contributing to this project, you agree to abide by its terms.
 
-- For questions and discussions about deploying models, statistical modeling, and machine learning, please [post on RStudio Community](https://community.rstudio.com/new-topic?category_id=15&tags=vetiver,question).
+- For questions and discussions about deploying models, statistical modeling, and machine learning, please [post on Posit Community](https://community.rstudio.com/new-topic?category_id=15&tags=vetiver,question).
 
 - If you think you have encountered a bug, please [submit an issue](https://github.com/rstudio/vetiver-python/issues).
```

#### html2text {}

```diff
@@ -1,53 +1,55 @@
-Metadata-Version: 2.1 Name: vetiver Version: 0.2.0 Summary: Deploy models into
-REST endpoints Home-page: https://github.com/isabelizimm/vetiver-python Author:
-Isabel Zimmerman Author-email: isabel.zimmerman@rstudio.com License: MIT
-Keywords: data,mlops Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Metadata-Version: 2.1 Name: vetiver Version: 0.2.1 Summary: Version, share,
+deploy, and monitor models. Home-page: https://github.com/rstudio/vetiver-
+python Author: Isabel Zimmerman Author-email: isabel.zimmerman@posit.co
+License: MIT Keywords: data,mlops Classifier: Programming Language :: Python ::
+3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-all Provides-Extra: dev Provides-Extra: torch Provides-Extra: statsmodels
-Provides-Extra: xgboost License-File: LICENSE # vetiver [docs/figures/logo.png]
-[![Lifecycle: experimental](https://img.shields.io/badge/lifecycle-
-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/
+all Provides-Extra: all_models Provides-Extra: dev Provides-Extra: docs
+Provides-Extra: statsmodels Provides-Extra: torch Provides-Extra: xgboost
+Provides-Extra: spacy Provides-Extra: typecheck License-File: LICENSE # vetiver
+[docs/figures/logo.png]  [![Lifecycle: experimental](https://img.shields.io/
+badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/
 stages.html#experimental) [![codecov](https://codecov.io/gh/isabelizimm/
 vetiver-python/branch/main/graph/badge.svg?token=CW6JHVS6ZX)](https://
 codecov.io/gh/isabelizimm/vetiver-python)  _Vetiver, the oil of tranquility, is
 used as a stabilizing ingredient in perfumery to preserve more volatile
 fragrances._ The goal of vetiver is to provide fluent tooling to version,
 share, deploy, and monitor a trained model. Functions handle both recording and
 checking the model's input data prototype, and predicting from a remote API
 endpoint. The vetiver package is extensible, with generics that can support
 many kinds of models, and available for both Python and R. To learn more about
 vetiver, see: - the documentation at
 vetiver.rstudio.com/> - the R package at
 rstudio.github.io/vetiver-r/> You can use vetiver with: - [scikit-learn](https:
 //scikit-learn.org/) - [torch](https://pytorch.org/) - [statsmodels](https://
 www.statsmodels.org/stable/index.html) - [xgboost](https://
-xgboost.readthedocs.io/en/stable/) - or utilize [custom handlers](https://
-rstudio.github.io/vetiver-python/stable/advancedusage/custom_handler.html) to
-support your own models! ## Installation You can install the released version
-of vetiver from [PyPI](https://pypi.org/project/vetiver/): ```python python -
-m pip install vetiver ``` And the development version from [GitHub](https://
-github.com/rstudio/vetiver-python) with: ```python python -m pip install
-git+https://github.com/rstudio/vetiver-python ``` ## Example A `VetiverModel()`
-object collects the information needed to store, version, and deploy a trained
-model. ```python from vetiver import mock, VetiverModel X, y =
-mock.get_mock_data() model = mock.get_mock_model().fit(X, y) v = VetiverModel
-(model, model_name='mock_model', prototype_data=X) ``` You can **version** and
-**share** your `VetiverModel()` by choosing a [pins](https://rstudio.github.io/
-pins-python/) "board" for it, including a local folder, RStudio Connect, Amazon
+xgboost.readthedocs.io/en/stable/) - [spacy](https://spacy.io/) - or utilize
+[custom handlers](https://rstudio.github.io/vetiver-python/stable/
+advancedusage/custom_handler.html) to support your own models! ## Installation
+You can install the released version of vetiver from [PyPI](https://pypi.org/
+project/vetiver/): ```python python -m pip install vetiver ``` And the
+development version from [GitHub](https://github.com/rstudio/vetiver-python)
+with: ```python python -m pip install git+https://github.com/rstudio/vetiver-
+python ``` ## Example A `VetiverModel()` object collects the information needed
+to store, version, and deploy a trained model. ```python from vetiver import
+mock, VetiverModel X, y = mock.get_mock_data() model = mock.get_mock_model
+().fit(X, y) v = VetiverModel(model, model_name='mock_model', prototype_data=X)
+``` You can **version** and **share** your `VetiverModel()` by choosing a
+[pins](https://rstudio.github.io/pins-python/) "board" for it, including a
+local folder, [Connect](https://posit.co/products/enterprise/connect/), Amazon
 S3, and more. ```python from pins import board_temp from vetiver import
 vetiver_pin_write model_board = board_temp(versioned = True, allow_pickle_read
 = True) vetiver_pin_write(model_board, v) ``` You can **deploy** your pinned
 `VetiverModel()` using `VetiverAPI()`, an extension of [FastAPI](https://
 fastapi.tiangolo.com/). ```python from vetiver import VetiverAPI app =
 VetiverAPI(v, check_prototype = True) ``` To start a server using this object,
 use `app.run(port = 8080)` or your port of choice. ## Contributing This project
 is released with a [Contributor Code of Conduct](https://www.contributor-
 covenant.org/version/2/1/CODE_OF_CONDUCT.html). By contributing to this
 project, you agree to abide by its terms. - For questions and discussions about
 deploying models, statistical modeling, and machine learning, please [post on
-RStudio Community](https://community.rstudio.com/new-
+Posit Community](https://community.rstudio.com/new-
 topic?category_id=15&tags=vetiver,question). - If you think you have
 encountered a bug, please [submit an issue](https://github.com/rstudio/vetiver-
 python/issues).
```

### Comparing `vetiver-0.2.0/README.md` & `vetiver-0.2.1/docs/index.qmd`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# vetiver <a href='https://rstudio.github.io/vetiver-python/'><img src='docs/figures/logo.png' align="right" height="139" /></a>
+# vetiver <a href='https://rstudio.github.io/vetiver-python/'><img src='figures/logo.png' align="right" height="139" /></a>
 
 <!-- badges: start -->
 
 [![Lifecycle:
 experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental) [![codecov](https://codecov.io/gh/isabelizimm/vetiver-python/branch/main/graph/badge.svg?token=CW6JHVS6ZX)](https://codecov.io/gh/isabelizimm/vetiver-python)
 
 <!-- badges: end -->
@@ -16,14 +16,15 @@
 
 You can use vetiver with:
 
 -   [scikit-learn](https://scikit-learn.org/)
 -   [torch](https://pytorch.org/)
 -   [statsmodels](https://www.statsmodels.org/stable/index.html)
 -   [xgboost](https://xgboost.readthedocs.io/en/stable/)
+-   [spacy](https://spacy.io/)
 -   or utilize [custom handlers](https://rstudio.github.io/vetiver-python/stable/advancedusage/custom_handler.html) to support your own models!
 
 ## Installation
 
 You can install the released version of vetiver from [PyPI](https://pypi.org/project/vetiver/):
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-# vetiver [docs/figures/logo.png]  [![Lifecycle: experimental](https://
+# vetiver [figures/logo.png]  [![Lifecycle: experimental](https://
 img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-
 lib.org/articles/stages.html#experimental) [![codecov](https://codecov.io/gh/
 isabelizimm/vetiver-python/branch/main/graph/badge.svg?token=CW6JHVS6ZX)]
 (https://codecov.io/gh/isabelizimm/vetiver-python)  _Vetiver, the oil of
 tranquility, is used as a stabilizing ingredient in perfumery to preserve more
 volatile fragrances._ The goal of vetiver is to provide fluent tooling to
 version, share, deploy, and monitor a trained model. Functions handle both
@@ -10,35 +10,35 @@
 remote API endpoint. The vetiver package is extensible, with generics that can
 support many kinds of models, and available for both Python and R. To learn
 more about vetiver, see: - the documentation at
 vetiver.rstudio.com/> - the R package at
 rstudio.github.io/vetiver-r/> You can use vetiver with: - [scikit-learn](https:
 //scikit-learn.org/) - [torch](https://pytorch.org/) - [statsmodels](https://
 www.statsmodels.org/stable/index.html) - [xgboost](https://
-xgboost.readthedocs.io/en/stable/) - or utilize [custom handlers](https://
-rstudio.github.io/vetiver-python/stable/advancedusage/custom_handler.html) to
-support your own models! ## Installation You can install the released version
-of vetiver from [PyPI](https://pypi.org/project/vetiver/): ```python python -
-m pip install vetiver ``` And the development version from [GitHub](https://
-github.com/rstudio/vetiver-python) with: ```python python -m pip install
-git+https://github.com/rstudio/vetiver-python ``` ## Example A `VetiverModel()`
-object collects the information needed to store, version, and deploy a trained
-model. ```python from vetiver import mock, VetiverModel X, y =
-mock.get_mock_data() model = mock.get_mock_model().fit(X, y) v = VetiverModel
-(model, model_name='mock_model', prototype_data=X) ``` You can **version** and
-**share** your `VetiverModel()` by choosing a [pins](https://rstudio.github.io/
-pins-python/) "board" for it, including a local folder, RStudio Connect, Amazon
-S3, and more. ```python from pins import board_temp from vetiver import
-vetiver_pin_write model_board = board_temp(versioned = True, allow_pickle_read
-= True) vetiver_pin_write(model_board, v) ``` You can **deploy** your pinned
-`VetiverModel()` using `VetiverAPI()`, an extension of [FastAPI](https://
-fastapi.tiangolo.com/). ```python from vetiver import VetiverAPI app =
-VetiverAPI(v, check_prototype = True) ``` To start a server using this object,
-use `app.run(port = 8080)` or your port of choice. ## Contributing This project
-is released with a [Contributor Code of Conduct](https://www.contributor-
-covenant.org/version/2/1/CODE_OF_CONDUCT.html). By contributing to this
-project, you agree to abide by its terms. - For questions and discussions about
-deploying models, statistical modeling, and machine learning, please [post on
-RStudio Community](https://community.rstudio.com/new-
+xgboost.readthedocs.io/en/stable/) - [spacy](https://spacy.io/) - or utilize
+[custom handlers](https://rstudio.github.io/vetiver-python/stable/
+advancedusage/custom_handler.html) to support your own models! ## Installation
+You can install the released version of vetiver from [PyPI](https://pypi.org/
+project/vetiver/): ```python python -m pip install vetiver ``` And the
+development version from [GitHub](https://github.com/rstudio/vetiver-python)
+with: ```python python -m pip install git+https://github.com/rstudio/vetiver-
+python ``` ## Example A `VetiverModel()` object collects the information needed
+to store, version, and deploy a trained model. ```python from vetiver import
+mock, VetiverModel X, y = mock.get_mock_data() model = mock.get_mock_model
+().fit(X, y) v = VetiverModel(model, model_name='mock_model', prototype_data=X)
+``` You can **version** and **share** your `VetiverModel()` by choosing a
+[pins](https://rstudio.github.io/pins-python/) "board" for it, including a
+local folder, RStudio Connect, Amazon S3, and more. ```python from pins import
+board_temp from vetiver import vetiver_pin_write model_board = board_temp
+(versioned = True, allow_pickle_read = True) vetiver_pin_write(model_board, v)
+``` You can **deploy** your pinned `VetiverModel()` using `VetiverAPI()`, an
+extension of [FastAPI](https://fastapi.tiangolo.com/). ```python from vetiver
+import VetiverAPI app = VetiverAPI(v, check_prototype = True) ``` To start a
+server using this object, use `app.run(port = 8080)` or your port of choice. ##
+Contributing This project is released with a [Contributor Code of Conduct]
+(https://www.contributor-covenant.org/version/2/1/CODE_OF_CONDUCT.html). By
+contributing to this project, you agree to abide by its terms. - For questions
+and discussions about deploying models, statistical modeling, and machine
+learning, please [post on RStudio Community](https://community.rstudio.com/new-
 topic?category_id=15&tags=vetiver,question). - If you think you have
 encountered a bug, please [submit an issue](https://github.com/rstudio/vetiver-
 python/issues).
```

### Comparing `vetiver-0.2.0/docs/figures/logo.svg` & `vetiver-0.2.1/docs/figures/logo.svg`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/docs/source/advancedusage/custom_handler.md` & `vetiver-0.2.1/docs/custom_handler.md`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/examples/coffeeratings/v/20220415T174503Z-06d9b/v.joblib` & `vetiver-0.2.1/examples/coffeeratings/v/20220415T174503Z-06d9b/v.joblib`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/examples/coffeeratings/vetiver_requirements.txt` & `vetiver-0.2.1/examples/coffeeratings/vetiver_requirements.txt`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/examples/coffeeratings.py` & `vetiver-0.2.1/examples/coffeeratings.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/setup.cfg` & `vetiver-0.2.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = vetiver
-description = Deploy models into REST endpoints
+description = Version, share, deploy, and monitor models.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/isabelizimm/vetiver-python
+url = https://github.com/rstudio/vetiver-python
 author = Isabel Zimmerman
-author_email = isabel.zimmerman@rstudio.com
+author_email = isabel.zimmerman@posit.co
 license = MIT
 keywords = data, mlops
 classifiers = 
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
@@ -35,29 +35,37 @@
 	pip-tools
 	httpx
 	importlib-metadata>=4.4  # NOTE: Remove when python_requires>=3.8
 
 [options.extras_require]
 all = 
 	vetiver[dev]
+	vetiver[all_models]
+	vetiver[docs]
+all_models = 
 	vetiver[torch]
 	vetiver[statsmodels]
 	vetiver[xgboost]
+	vetiver[spacy]
 dev = 
 	pytest
 	pytest-cov
 	pytest-snapshot
-	sphinx
-	sphinx-autodoc-typehints
-	sphinx-book-theme==0.3.3
-	myst-parser
-torch = 
-	torch
+	vetiver[typecheck]
+docs = 
+	quartodoc
 statsmodels = 
 	statsmodels
+torch = 
+	torch
 xgboost = 
 	xgboost
+spacy = 
+	spacy
+typecheck = 
+	pyright
+	pandas-stubs
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vetiver-0.2.0/vetiver/__init__.py` & `vetiver-0.2.1/vetiver/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 from importlib_metadata import version as _version
 
 from .prototype import vetiver_create_prototype, vetiver_create_ptype  # noqa
 from .vetiver_model import VetiverModel  # noqa
 from .server import VetiverAPI, vetiver_endpoint, predict  # noqa
 from .mock import get_mock_data, get_mock_model  # noqa
 from .pin_read_write import vetiver_pin_write  # noqa
-from .attach_pkgs import load_pkgs  # noqa
+from .attach_pkgs import load_pkgs, get_board_pkgs  # noqa
 from .meta import VetiverMeta  # noqa
 from .write_docker import write_docker, prepare_docker  # noqa
 from .write_fastapi import write_app, vetiver_write_app  # noqa
 from .handlers.base import BaseHandler, create_handler, InvalidModelError  # noqa
 from .handlers.sklearn import SKLearnHandler  # noqa
 from .handlers.torch import TorchHandler  # noqa
 from .handlers.statsmodels import StatsmodelsHandler  # noqa
 from .handlers.xgboost import XGBoostHandler  # noqa
+from .handlers.spacy import SpacyHandler  # noqa
+from .helpers import api_data_to_frame  # noqa
 from .rsconnect import deploy_rsconnect  # noqa
 from .monitor import compute_metrics, pin_metrics, plot_metrics, _rolling_df  # noqa
 from .model_card import model_card  # noqa
 from .types import create_prototype, Prototype  # noqa
 
-__author__ = "Isabel Zimmerman <isabel.zimmerman@rstudio.com>"
+__author__ = "Isabel Zimmerman <isabel.zimmerman@posit.co>"
 __all__ = []
 __version__ = _version("vetiver")
 del _version
```

### Comparing `vetiver-0.2.0/vetiver/data/__init__.py` & `vetiver-0.2.1/vetiver/data/__init__.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/data/chicago.csv` & `vetiver-0.2.1/vetiver/data/chicago.csv`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/data/mtcars.csv` & `vetiver-0.2.1/vetiver/data/mtcars.csv`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/data/sacramento.csv` & `vetiver-0.2.1/vetiver/data/sacramento.csv`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/handlers/base.py` & `vetiver-0.2.1/vetiver/handlers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from vetiver.handlers import base
 from functools import singledispatch
 from contextlib import suppress
 
 from ..prototype import vetiver_create_prototype
 from ..meta import VetiverMeta
 
 
@@ -141,12 +140,12 @@
 
 
 # BaseHandler for subclassing, Handler for new model types
 Handler = BaseHandler
 
 
 @create_handler.register
-def _(model: base.BaseHandler, prototype_data):
+def _(model: BaseHandler, prototype_data):
     if model.prototype_data is None and prototype_data is not None:
         model.prototype_data = prototype_data
 
     return model
```

### Comparing `vetiver-0.2.0/vetiver/handlers/sklearn.py` & `vetiver-0.2.1/vetiver/handlers/sklearn.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,8 +35,8 @@
         """
 
         if not check_prototype or isinstance(input_data, pd.DataFrame):
             prediction = self.model.predict(input_data)
         else:
             prediction = self.model.predict([input_data])
 
-        return prediction
+        return prediction.tolist()
```

### Comparing `vetiver-0.2.0/vetiver/handlers/statsmodels.py` & `vetiver-0.2.1/vetiver/handlers/statsmodels.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,8 +43,8 @@
             raise ImportError("Cannot import `statsmodels`")
 
         if isinstance(input_data, (list, pd.DataFrame)):
             prediction = self.model.predict(input_data)
         else:
             prediction = self.model.predict([input_data])
 
-        return prediction
+        return prediction.tolist()
```

### Comparing `vetiver-0.2.0/vetiver/handlers/torch.py` & `vetiver-0.2.1/vetiver/handlers/torch.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,17 +37,16 @@
         Returns
         -------
         prediction
             Prediction from model
         """
         if not torch_exists:
             raise ImportError("Cannot import `torch`.")
+
         if check_prototype:
             input_data = np.array(input_data, dtype=np.array(self.prototype_data).dtype)
             prediction = self.model(torch.from_numpy(input_data))
-
-        # do not check ptype
         else:
             input_data = torch.tensor(input_data)
             prediction = self.model(input_data)
 
-        return prediction
+        return prediction.tolist()
```

### Comparing `vetiver-0.2.0/vetiver/handlers/xgboost.py` & `vetiver-0.2.1/vetiver/handlers/xgboost.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class XGBoostHandler(BaseHandler):
     """Handler class for creating VetiverModels with xgboost.
 
     Parameters
     ----------
-    model :
+    model : xgboost.Booster
         a trained and fit xgboost model
     """
 
     model_class = staticmethod(lambda: xgboost.Booster)
     if xgb_exists:
         pip_name = "xgboost"
 
@@ -44,12 +44,13 @@
             raise ImportError("Cannot import `xgboost`")
 
         if not isinstance(input_data, pd.DataFrame):
             try:
                 input_data = pd.DataFrame(input_data)
             except ValueError:
                 raise (f"Expected a dict or DataFrame, got {type(input_data)}")
+
         input_data = xgboost.DMatrix(input_data)
 
         prediction = self.model.predict(input_data)
 
-        return prediction
+        return prediction.tolist()
```

### Comparing `vetiver-0.2.0/vetiver/meta.py` & `vetiver-0.2.1/vetiver/meta.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,21 @@
     def from_dict(cls, metadata, pip_name=None) -> "VetiverMeta":
 
         metadata = {} if metadata is None else metadata
 
         user = metadata.get("user", metadata)
         version = metadata.get("version", None)
         url = metadata.get("url", None)
-        required_pkgs = metadata.get("required_pkgs", [])
-        python_version = tuple(metadata.get("python_version", sys.version_info))
+        # give correct value if key doesnt exist or if value is None
+        required_pkgs = (
+            []
+            if not metadata.get("required_pkgs")
+            else metadata.get("required_pkgs", [])
+        )
+        python_version = metadata.get("python_version", sys.version_info)
+        python_version = python_version if not python_version else tuple(python_version)
 
         if pip_name:
             if not list(filter(lambda x: pip_name in x, required_pkgs)):
                 required_pkgs = required_pkgs + [f"{pip_name}"]
 
         return cls(user, version, url, required_pkgs, python_version)
```

### Comparing `vetiver-0.2.0/vetiver/mock.py` & `vetiver-0.2.1/vetiver/mock.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/monitor.py` & `vetiver-0.2.1/vetiver/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,23 +201,23 @@
 ) -> px.line:
     """
     Plot metrics over a given time period
 
     Parameters
     ----------
     df_metrics : DataFrame
-        Pandas dataframe of metrics over time, such as created by `compute_metircs()`
+         Pandas dataframe of metrics over time, such as created by `compute_metrics()`
     date: str
-        Column in `df_metrics` containing dates
+         Column in `df_metrics` containing dates
     estimate: str
-        Column in `df_metrics` containing metric output
+         Column in `df_metrics` containing metric output
     metric: str
-       Column in `df_metrics` containing metric name
+         Column in `df_metrics` containing metric name
     n: str
-        Column in `df_metrics` containing number of observations
+         Column in `df_metrics` containing number of observations
 
     Examples
     -------
     >>> import vetiver
     >>> import pandas as pd
     >>> df = pd.DataFrame(
     ... {'index': {0: pd.Timestamp('2021-01-01 00:00:00'),
```

### Comparing `vetiver-0.2.0/vetiver/pin_read_write.py` & `vetiver-0.2.1/vetiver/pin_read_write.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,18 @@
     >>> model_board = board_temp(versioned = True, allow_pickle_read = True)
     >>> X, y = vetiver.get_mock_data()
     >>> model = vetiver.get_mock_model().fit(X, y)
     >>> v = vetiver.VetiverModel(model, "my_model", prototype_data = X)
     >>> vetiver.vetiver_pin_write(model_board, v)
     """
     if not board.allow_pickle_read:
-        raise NotImplementedError  # must be pickle-able
+        raise ValueError(
+            "board does not allow pickled models. Set "
+            "allow_pickle_read to True on board creation."
+        )
 
     inform(
         _log,
         "Model Cards provide a framework for transparent, responsible "
         "reporting. \n Use the vetiver `.qmd` Quarto template as a place to start, \n "
         "with vetiver.model_card()",
     )
@@ -66,15 +69,17 @@
         type="joblib",
         description=model.description,
         metadata={
             "user": model.metadata.user,
             "vetiver_meta": {
                 "required_pkgs": model.metadata.required_pkgs,
                 "prototype": None if not model.prototype else model.prototype().json(),
-                "python_version": list(model.metadata.python_version),
+                "python_version": None
+                if not model.metadata.python_version
+                else list(model.metadata.python_version),
             },
         },
         versioned=versioned,
     )
 
 
 def vetiver_pin_read(board, name: str, version: str = None) -> VetiverModel:
```

### Comparing `vetiver-0.2.0/vetiver/prototype.py` & `vetiver-0.2.1/vetiver/prototype.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/rsconnect.py` & `vetiver-0.2.1/vetiver/rsconnect.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 import shutil
 import tempfile
 import typing
 
 from rsconnect.actions import deploy_python_fastapi
+from rsconnect.api import RSConnectServer as ConnectServer
 
 from .write_fastapi import write_app
 
 
 def deploy_rsconnect(
-    connect_server,
+    connect_server: ConnectServer,
     board,
     pin_name: str,
     version: str = None,
     extra_files: typing.List[str] = None,
     new: bool = False,
     app_id: int = None,
     title: str = None,
```

### Comparing `vetiver-0.2.0/vetiver/server.py` & `vetiver-0.2.1/vetiver/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-from typing import Any, Callable, Dict, List, Union
+from typing import Callable, List, Union
 from urllib.parse import urljoin
 
+import re
 import httpx
 import pandas as pd
 import requests
 import uvicorn
 from fastapi import FastAPI, Request, testclient
+from fastapi.exceptions import RequestValidationError
 from fastapi.openapi.utils import get_openapi
 from fastapi.responses import HTMLResponse, RedirectResponse
+from fastapi.responses import PlainTextResponse
 from warnings import warn
 
 from .utils import _jupyter_nb
 from .vetiver_model import VetiverModel
 from .meta import VetiverMeta
+from .helpers import api_data_to_frame, response_to_frame
 
 
 class VetiverAPI:
     """Create model aware API
 
     Parameters
     ----------
@@ -92,14 +96,18 @@
             def pin_url():
                 return repr(self.model.metadata.url)
 
         @app.get("/ping", include_in_schema=True)
         async def ping():
             return {"ping": "pong"}
 
+        @app.get("/metadata")
+        async def get_metadata():
+            return self.model.metadata.to_dict()
+
         self.vetiver_post(
             self.model.handler_predict, "predict", check_prototype=self.check_prototype
         )
 
         @app.get("/__docs__", response_class=HTMLResponse, include_in_schema=False)
         async def rapidoc():
             # save as html html.tpl, .format {spec_url}
@@ -134,14 +142,18 @@
                             width="55"
                             src="https://raw.githubusercontent.com/rstudio/hex-stickers/master/SVG/vetiver.svg"
                             </rapi-doc>
                         </body>
                     </html>
             """
 
+        @app.exception_handler(RequestValidationError)
+        async def validation_exception_handler(request, exc):
+            return PlainTextResponse(str(exc), status_code=422)
+
         return app
 
     def vetiver_post(self, endpoint_fx: Callable, endpoint_name: str = None, **kw):
         """Create new POST endpoint that is aware of model input data
 
         Parameters
         ----------
@@ -163,34 +175,34 @@
         """
         if not endpoint_name:
             endpoint_name = endpoint_fx.__name__
 
         if self.check_prototype is True:
 
             @self.app.post(urljoin("/", endpoint_name), name=endpoint_name)
-            async def custom_endpoint(
-                input_data: Union[self.model.prototype, List[self.model.prototype]]
-            ):
+            async def custom_endpoint(input_data: List[self.model.prototype]):
+                _to_frame = api_data_to_frame(input_data)
+                predictions = endpoint_fx(_to_frame, **kw)
 
-                if isinstance(input_data, List):
-                    served_data = _batch_data(input_data)
+                if isinstance(predictions, List):
+                    return {endpoint_name: predictions}
                 else:
-                    served_data = _prepare_data(input_data)
-
-                new = endpoint_fx(served_data, **kw)
-                return {endpoint_name: new.tolist()}
+                    return predictions
 
         else:
 
             @self.app.post(urljoin("/", endpoint_name))
             async def custom_endpoint(input_data: Request):
                 served_data = await input_data.json()
-                new = endpoint_fx(served_data, **kw)
+                predictions = endpoint_fx(served_data, **kw)
 
-                return {endpoint_name: new.tolist()}
+                if isinstance(predictions, List):
+                    return {endpoint_name: predictions}
+                else:
+                    return predictions
 
     def run(self, port: int = 8000, host: str = "127.0.0.1", **kw):
         """
         Start API
 
         Parameters
         ----------
@@ -257,54 +269,36 @@
     else:
         requester = requests
 
     # TO DO: arrow format
     # TO DO: dispatch
 
     if isinstance(data, pd.DataFrame):
-        data_json = data.to_json(orient="records")
-        response = requester.post(endpoint, data=data_json, **kw)
+        response = requester.post(
+            endpoint, data=data.to_json(orient="records"), **kw
+        )  # TO DO: httpx deprecating data in favor of content for TestClient
     elif isinstance(data, pd.Series):
-        data_dict = data.to_json()
-        response = requester.post(endpoint, data=data_dict, **kw)
+        response = requester.post(endpoint, json=[data.to_dict()], **kw)
     elif isinstance(data, dict):
-        response = requester.post(endpoint, json=data, **kw)
+        response = requester.post(endpoint, json=[data], **kw)
     else:
         response = requester.post(endpoint, json=data, **kw)
 
     try:
         response.raise_for_status()
     except (requests.exceptions.HTTPError, httpx.HTTPStatusError) as e:
         if response.status_code == 422:
-            raise TypeError(
-                f"Predict expects DataFrame, Series, or dict. Given type is {type(data)}"
-            )
+            raise TypeError(re.sub(r"\n", ": ", response.text))
         raise requests.exceptions.HTTPError(
             f"Could not obtain data from endpoint with error: {e}"
         )
 
-    response_df = pd.DataFrame.from_dict(response.json())
-
-    return response_df
-
-
-def _prepare_data(pred_data: Dict[str, Any]) -> List[Any]:
-    served_data = []
-    for key, value in pred_data:
-        served_data.append(value)
-    return served_data
-
-
-def _batch_data(pred_data: List[Any]) -> pd.DataFrame:
-    columns = pred_data[0].dict().keys()
-
-    data = [line.dict() for line in pred_data]
+    response_frame = response_to_frame(response)
 
-    served_data = pd.DataFrame(data, columns=columns)
-    return served_data
+    return response_frame
 
 
 def vetiver_endpoint(url: str = "http://127.0.0.1:8000/predict") -> str:
     """Wrap url where VetiverModel will be deployed
 
     Parameters
     ----------
```

### Comparing `vetiver-0.2.0/vetiver/templates/model_card.qmd` & `vetiver-0.2.1/vetiver/templates/model_card.qmd`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/tests/snapshots/test_monitor.json` & `vetiver-0.2.1/vetiver/tests/snapshots/test_monitor.json`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/tests/test_add_endpoint.py` & `vetiver-0.2.1/vetiver/tests/test_add_endpoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pytest
 
 import numpy as np
 import pandas as pd
 from fastapi.testclient import TestClient
 
 from vetiver import mock, VetiverModel, VetiverAPI
+from vetiver.helpers import api_data_to_frame
 import vetiver
 
 
 @pytest.fixture
 def vetiver_model():
     np.random.seed(500)
     X, y = mock.get_mock_data()
@@ -21,20 +22,19 @@
         description="A regression model for testing purposes",
     )
 
     return v
 
 
 def sum_values(x):
-    return x.sum()
+    return x.sum().to_list()
 
 
-def sum_dict(x):
-    x = pd.DataFrame(x)
-    return x.sum()
+def sum_values_no_prototype(x):
+    return api_data_to_frame(x).sum().to_list()
 
 
 @pytest.fixture
 def vetiver_client(vetiver_model):  # With check_prototype=True
 
     app = VetiverAPI(vetiver_model, check_prototype=True)
     app.vetiver_post(sum_values, "sum")
@@ -45,15 +45,15 @@
     return client
 
 
 @pytest.fixture
 def vetiver_client_check_ptype_false(vetiver_model):  # With check_prototype=False
 
     app = VetiverAPI(vetiver_model, check_prototype=False)
-    app.vetiver_post(sum_dict, "sum")
+    app.vetiver_post(sum_values_no_prototype, "sum")
 
     app.app.root_path = "/sum"
     client = TestClient(app.app)
 
     return client
```

### Comparing `vetiver-0.2.0/vetiver/tests/test_build_api.py` & `vetiver-0.2.1/vetiver/tests/test_build_api.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/tests/test_build_vetiver_model.py` & `vetiver-0.2.1/vetiver/tests/test_build_vetiver_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -173,7 +173,33 @@
     assert isinstance(v2.prototype.construct(), pydantic.BaseModel)
     assert v2.metadata.user == custom_meta
     assert v2.metadata.version is not None
     assert v2.metadata.required_pkgs == loaded_pkgs
     assert v2.metadata.python_version == tuple(custom_meta["python_version"])
 
     board.pin_delete("model")
+
+
+def test_vetiver_model_from_pin_no_version():
+    """
+    Test if standard keys as part of :dataclass:`VetiverMeta` are picked
+    """
+    custom_meta = {
+        "required_pkgs": None,
+        "python_version": None,
+    }
+
+    v = vt.VetiverModel(
+        model=model,
+        prototype_data=X_df,
+        model_name="model",
+        metadata=custom_meta,
+    )
+
+    board = pins.board_temp(allow_pickle_read=True)
+    vt.vetiver_pin_write(board=board, model=v)
+    v2 = vt.VetiverModel.from_pin(board, "model")
+
+    assert v2.metadata.required_pkgs == ["scikit-learn"]
+    assert v2.metadata.python_version is None
+
+    board.pin_delete("model")
```

### Comparing `vetiver-0.2.0/vetiver/tests/test_custom_handler.py` & `vetiver-0.2.1/vetiver/tests/test_custom_handler.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/tests/test_monitor.py` & `vetiver-0.2.1/vetiver/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/tests/test_pin_write.py` & `vetiver-0.2.1/vetiver/tests/test_pin_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def test_board_pin_write_error():
     v = VetiverModel(
         model=model, prototype_data=X_df, model_name="model", versioned=None
     )
     board = pins.board_temp()
-    with pytest.raises(NotImplementedError):
+    with pytest.raises(ValueError):
         vetiver_pin_write(board=board, model=v)
 
 
 def test_board_pin_write():
     v = VetiverModel(
         model=model, prototype_data=X_df, model_name="model", versioned=None
     )
```

### Comparing `vetiver-0.2.0/vetiver/tests/test_predict.py` & `vetiver-0.2.1/vetiver/tests/test_sklearn.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 import pandas as pd
 from requests.exceptions import HTTPError
 from fastapi.testclient import TestClient
 
 from vetiver import mock, VetiverModel, VetiverAPI
 from vetiver.server import predict
 
+np.random.seed(500)
+X, y = mock.get_mock_data()
+
 
 @pytest.fixture
 def vetiver_model():
     np.random.seed(500)
-    X, y = mock.get_mock_data()
     model = mock.get_mock_model().fit(X, y)
     v = VetiverModel(
         model=model,
         prototype_data=X,
         model_name="my_model",
         versioned=None,
         description="A regression model for testing purposes",
@@ -39,54 +41,49 @@
     app = VetiverAPI(vetiver_model, check_prototype=False)
     app.app.root_path = "/predict"
     client = TestClient(app.app)
 
     return client
 
 
-def test_predict_sklearn_dict_ptype(vetiver_client):
-    data = {"B": 0, "C": 0, "D": 0}
+@pytest.mark.parametrize(
+    "data,length",
+    [({"B": 0, "C": 0, "D": 0}, 1), (pd.Series(data=[0, 0, 0]), 1), (X, 100)],
+)
+def test_predict_sklearn_ptype(data, length, vetiver_client):
 
     response = predict(endpoint=vetiver_client, data=data)
 
     assert isinstance(response, pd.DataFrame), response
     assert response.iloc[0, 0] == 44.47
-    assert len(response) == 1
-
-
-def test_predict_sklearn_no_ptype(vetiver_client_check_ptype_false):
-    X, y = mock.get_mock_data()
-    response = predict(endpoint=vetiver_client_check_ptype_false, data=X)
-
-    assert isinstance(response, pd.DataFrame), response
-    assert response.iloc[0, 0] == 44.47
-    assert len(response) == 100
+    assert len(response) == length
 
 
-def test_predict_sklearn_df_check_ptype(vetiver_client):
+@pytest.mark.parametrize(
+    "data,length",
+    [({"B": 0, "C": 0, "D": 0}, 1), (pd.Series(data=[0, 0, 0]), 1), (X, 100)],
+)
+def test_predict_sklearn_no_ptype(data, length, vetiver_client_check_ptype_false):
     X, y = mock.get_mock_data()
-    response = predict(endpoint=vetiver_client, data=X)
+    response = predict(endpoint=vetiver_client_check_ptype_false, data=data)
 
     assert isinstance(response, pd.DataFrame), response
     assert response.iloc[0, 0] == 44.47
-    assert len(response) == 100
+    assert len(response) == length
 
 
-def test_predict_sklearn_series_check_ptype(vetiver_client):
-    ser = pd.Series(data=[0, 0, 0])
-    response = predict(endpoint=vetiver_client, data=ser)
-
-    assert isinstance(response, pd.DataFrame), response
-    assert response.iloc[0, 0] == 44.47
-    assert len(response) == 1
-
-
-@pytest.mark.parametrize("data", [(0, 0), 0, 0.0, "0"])
+@pytest.mark.parametrize("data", [(0), 0, 0.0, "0"])
 def test_predict_sklearn_type_error(data, vetiver_client):
-    msg = f"Predict expects DataFrame, Series, or dict. Given type is {type(data)}"
+    import re
+
+    msg = re.sub(
+        r"\n",
+        ": ",
+        "1 validation error for Request\nbody\n  value is not a valid list \(type=type_error.list\)",  # noqa
+    )
 
     with pytest.raises(TypeError, match=msg):
         predict(endpoint=vetiver_client, data=data)
 
 
 def test_predict_server_error(vetiver_model):
     X, y = mock.get_mock_data()
```

### Comparing `vetiver-0.2.0/vetiver/tests/test_rsconnect.py` & `vetiver-0.2.1/vetiver/tests/test_rsconnect.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/tests/test_statsmodels.py` & `vetiver-0.2.1/vetiver/tests/test_statsmodels.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/tests/test_write_docker.py` & `vetiver-0.2.1/vetiver/tests/test_write_docker.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/tests/test_xgboost.py` & `vetiver-0.2.1/vetiver/tests/test_xgboost.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/utils.py` & `vetiver-0.2.1/vetiver/utils.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver/vetiver_model.py` & `vetiver-0.2.1/vetiver/vetiver_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,16 +48,14 @@
     Notes
     -----
     VetiverModel can also take an initialized custom VetiverHandler
     as a model, for advanced use cases or non-supported model types.
     Parameter `ptype_data` was changed to `prototype_data`. Handling of `ptype_data`
     will be removed in a future version.
 
-
-
     Examples
     -------
     >>> from vetiver import mock, VetiverModel
     >>> X, y = mock.get_mock_data()
     >>> model = mock.get_mock_model().fit(X, y)
     >>> v = VetiverModel(model = model, model_name = "my_model", prototype_data = X)
     >>> v.description
@@ -100,23 +98,17 @@
         meta = board.pin_meta(name, version)
 
         if "vetiver_meta" in meta.user:
             get_prototype = meta.user.get("vetiver_meta").get("prototype", None)
             required_pkgs = meta.user.get("vetiver_meta").get("required_pkgs", None)
             python_version = meta.user.get("vetiver_meta").get("python_version", None)
             meta.user.pop("vetiver_meta")
+        # old pin type
         else:
-            # ptype = meta.user.get("ptype", None)
-
             get_prototype = meta.user.get("ptype")
-            # elif meta.user.get("prototype"):
-            #     get_prototype = meta.user.get("prototype")
-            # else:
-            #     get_prototype = None
-
             required_pkgs = meta.user.get("required_pkgs")
             python_version = meta.user.get("python_version")
 
         return cls(
             model=model,
             model_name=name,
             description=meta.description,
```

### Comparing `vetiver-0.2.0/vetiver/write_docker.py` & `vetiver-0.2.1/vetiver/write_docker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import warnings
 from pathlib import Path
 
 from .write_fastapi import write_app
-from .attach_pkgs import load_pkgs
+from .attach_pkgs import load_pkgs, get_board_pkgs
 from .vetiver_model import VetiverModel
 
 
 def vetiver_write_docker(
     app_file: str = "app.py",
     path: str = "./",
     rspm_env: bool = False,
@@ -32,24 +32,24 @@
     host: str = "0.0.0.0",
     port: str = "8080",
 ):
     """Writes a Dockerfile to run VetiverAPI in a container
 
     Parameters
     ----------
-        app_file: str
-            File containing VetiverAPI to be deployed into container
-        path: str
-            Path to save Dockerfile
-        rspm_env: bool
-            Whether or not RStudio Package Manager should be used
-        host: str
-            Host address to run VetiverAPI from Dockerfile
-        port: str
-            Port to run VetiverAPI from Dockerfile
+    app_file: str
+        File containing VetiverAPI to be deployed into container
+    path: str
+        Path to save Dockerfile
+    rspm_env: bool
+        Whether or not Posit Package Manager should be used
+    host: str
+        Host address to run VetiverAPI from Dockerfile
+    port: str
+        Port to run VetiverAPI from Dockerfile
 
     Examples
     -------
     >>> import vetiver
     >>> import tempfile
     >>> import pins
     >>> tmp = tempfile.TemporaryDirectory()
@@ -106,30 +106,51 @@
     host: str = "0.0.0.0",
     port: str = "8080",
 ):
     """Create all files needed for Docker
 
     Parameters
     ----------
-        board :
-            Pin board for model
-        pin_name : str
-            Name of pin
-        path :
-            Path to output
-        version :
-            Pin version to be used
-        rspm_env: bool
-            Whether or not RStudio Package Manager should be used
-        host: str
-            Host address to run VetiverAPI from Dockerfile
-        port: str
-            Port to run VetiverAPI from Dockerfile
+    board :
+        Pin board for model
+    pin_name : str
+        Name of pin
+    path :
+        Path to output
+    version :
+        Pin version to be used
+    rspm_env: bool
+        Whether or not Posit Package Manager should be used
+    host: str
+        Host address to run VetiverAPI from Dockerfile
+    port: str
+        Port to run VetiverAPI from Dockerfile
 
+    Examples
+    -------
+    >>> import vetiver
+    >>> import tempfile
+    >>> import pins
+    >>> tmp = tempfile.TemporaryDirectory()
+    >>> board = pins.board_temp(allow_pickle_read=True)
+    >>> X, y = vetiver.get_mock_data()
+    >>> model = vetiver.get_mock_model().fit(X, y)
+    >>> v = vetiver.VetiverModel(model, "my_model", prototype_data = X)
+    >>> vetiver.vetiver_pin_write(board, v)
+    >>> vetiver.prepare_docker(board = board, pin_name = "my_model", path = tmp.name)
+
+    Notes
+    ------
+    This function uses `vetiver.get_board_pkgs(board)` for generating requirements.
+    For more complex use cases, call `write_docker()`, `load_pkgs()`, and
+    `write_app()` individually.
     """
 
     v = VetiverModel.from_pin(board=board, name=pin_name, version=version)
+
     write_app(
         board=board, pin_name=pin_name, version=version, file=Path(path, "app.py")
     )
-    load_pkgs(v, path=Path(path, "vetiver_"))
+
+    load_pkgs(v, path=Path(path, "vetiver_"), packages=get_board_pkgs(board))
+
     write_docker(path=path, rspm_env=rspm_env, host=host, port=port)
```

### Comparing `vetiver-0.2.0/vetiver/write_fastapi.py` & `vetiver-0.2.1/vetiver/write_fastapi.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.0/vetiver.egg-info/PKG-INFO` & `vetiver-0.2.1/vetiver.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: vetiver
-Version: 0.2.0
-Summary: Deploy models into REST endpoints
-Home-page: https://github.com/isabelizimm/vetiver-python
+Version: 0.2.1
+Summary: Version, share, deploy, and monitor models.
+Home-page: https://github.com/rstudio/vetiver-python
 Author: Isabel Zimmerman
-Author-email: isabel.zimmerman@rstudio.com
+Author-email: isabel.zimmerman@posit.co
 License: MIT
 Keywords: data,mlops
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
+Provides-Extra: all_models
 Provides-Extra: dev
-Provides-Extra: torch
+Provides-Extra: docs
 Provides-Extra: statsmodels
+Provides-Extra: torch
 Provides-Extra: xgboost
+Provides-Extra: spacy
+Provides-Extra: typecheck
 License-File: LICENSE
 
-# vetiver <a href='https://rstudio.github.io/vetiver-python/'><img src='docs/figures/logo.png' align="right" height="139" /></a>
+# vetiver <a href='https://rstudio.github.io/vetiver-python/'><img src='docs/figures/logo.png' align="right" height="138" /></a>
 
 <!-- badges: start -->
 
 [![Lifecycle:
 experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental) [![codecov](https://codecov.io/gh/isabelizimm/vetiver-python/branch/main/graph/badge.svg?token=CW6JHVS6ZX)](https://codecov.io/gh/isabelizimm/vetiver-python)
 
 <!-- badges: end -->
@@ -38,14 +42,15 @@
 
 You can use vetiver with:
 
 -   [scikit-learn](https://scikit-learn.org/)
 -   [torch](https://pytorch.org/)
 -   [statsmodels](https://www.statsmodels.org/stable/index.html)
 -   [xgboost](https://xgboost.readthedocs.io/en/stable/)
+-   [spacy](https://spacy.io/)
 -   or utilize [custom handlers](https://rstudio.github.io/vetiver-python/stable/advancedusage/custom_handler.html) to support your own models!
 
 ## Installation
 
 You can install the released version of vetiver from [PyPI](https://pypi.org/project/vetiver/):
 
 ```python
@@ -67,15 +72,15 @@
 
 X, y = mock.get_mock_data()
 model = mock.get_mock_model().fit(X, y)
 
 v = VetiverModel(model, model_name='mock_model', prototype_data=X)
 ```
 
-You can **version** and **share** your `VetiverModel()` by choosing a [pins](https://rstudio.github.io/pins-python/) "board" for it, including a local folder, RStudio Connect, Amazon S3, and more.
+You can **version** and **share** your `VetiverModel()` by choosing a [pins](https://rstudio.github.io/pins-python/) "board" for it, including a local folder, [Connect](https://posit.co/products/enterprise/connect/), Amazon S3, and more.
 
 ```python
 from pins import board_temp
 from vetiver import vetiver_pin_write
 
 model_board = board_temp(versioned = True, allow_pickle_read = True)
 vetiver_pin_write(model_board, v)
@@ -90,10 +95,10 @@
 
 To start a server using this object, use `app.run(port = 8080)` or your port of choice.
 
 ## Contributing
 
 This project is released with a [Contributor Code of Conduct](https://www.contributor-covenant.org/version/2/1/CODE_OF_CONDUCT.html). By contributing to this project, you agree to abide by its terms.
 
-- For questions and discussions about deploying models, statistical modeling, and machine learning, please [post on RStudio Community](https://community.rstudio.com/new-topic?category_id=15&tags=vetiver,question).
+- For questions and discussions about deploying models, statistical modeling, and machine learning, please [post on Posit Community](https://community.rstudio.com/new-topic?category_id=15&tags=vetiver,question).
 
 - If you think you have encountered a bug, please [submit an issue](https://github.com/rstudio/vetiver-python/issues).
```

#### html2text {}

```diff
@@ -1,53 +1,55 @@
-Metadata-Version: 2.1 Name: vetiver Version: 0.2.0 Summary: Deploy models into
-REST endpoints Home-page: https://github.com/isabelizimm/vetiver-python Author:
-Isabel Zimmerman Author-email: isabel.zimmerman@rstudio.com License: MIT
-Keywords: data,mlops Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Metadata-Version: 2.1 Name: vetiver Version: 0.2.1 Summary: Version, share,
+deploy, and monitor models. Home-page: https://github.com/rstudio/vetiver-
+python Author: Isabel Zimmerman Author-email: isabel.zimmerman@posit.co
+License: MIT Keywords: data,mlops Classifier: Programming Language :: Python ::
+3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-all Provides-Extra: dev Provides-Extra: torch Provides-Extra: statsmodels
-Provides-Extra: xgboost License-File: LICENSE # vetiver [docs/figures/logo.png]
-[![Lifecycle: experimental](https://img.shields.io/badge/lifecycle-
-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/
+all Provides-Extra: all_models Provides-Extra: dev Provides-Extra: docs
+Provides-Extra: statsmodels Provides-Extra: torch Provides-Extra: xgboost
+Provides-Extra: spacy Provides-Extra: typecheck License-File: LICENSE # vetiver
+[docs/figures/logo.png]  [![Lifecycle: experimental](https://img.shields.io/
+badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/
 stages.html#experimental) [![codecov](https://codecov.io/gh/isabelizimm/
 vetiver-python/branch/main/graph/badge.svg?token=CW6JHVS6ZX)](https://
 codecov.io/gh/isabelizimm/vetiver-python)  _Vetiver, the oil of tranquility, is
 used as a stabilizing ingredient in perfumery to preserve more volatile
 fragrances._ The goal of vetiver is to provide fluent tooling to version,
 share, deploy, and monitor a trained model. Functions handle both recording and
 checking the model's input data prototype, and predicting from a remote API
 endpoint. The vetiver package is extensible, with generics that can support
 many kinds of models, and available for both Python and R. To learn more about
 vetiver, see: - the documentation at
 vetiver.rstudio.com/> - the R package at
 rstudio.github.io/vetiver-r/> You can use vetiver with: - [scikit-learn](https:
 //scikit-learn.org/) - [torch](https://pytorch.org/) - [statsmodels](https://
 www.statsmodels.org/stable/index.html) - [xgboost](https://
-xgboost.readthedocs.io/en/stable/) - or utilize [custom handlers](https://
-rstudio.github.io/vetiver-python/stable/advancedusage/custom_handler.html) to
-support your own models! ## Installation You can install the released version
-of vetiver from [PyPI](https://pypi.org/project/vetiver/): ```python python -
-m pip install vetiver ``` And the development version from [GitHub](https://
-github.com/rstudio/vetiver-python) with: ```python python -m pip install
-git+https://github.com/rstudio/vetiver-python ``` ## Example A `VetiverModel()`
-object collects the information needed to store, version, and deploy a trained
-model. ```python from vetiver import mock, VetiverModel X, y =
-mock.get_mock_data() model = mock.get_mock_model().fit(X, y) v = VetiverModel
-(model, model_name='mock_model', prototype_data=X) ``` You can **version** and
-**share** your `VetiverModel()` by choosing a [pins](https://rstudio.github.io/
-pins-python/) "board" for it, including a local folder, RStudio Connect, Amazon
+xgboost.readthedocs.io/en/stable/) - [spacy](https://spacy.io/) - or utilize
+[custom handlers](https://rstudio.github.io/vetiver-python/stable/
+advancedusage/custom_handler.html) to support your own models! ## Installation
+You can install the released version of vetiver from [PyPI](https://pypi.org/
+project/vetiver/): ```python python -m pip install vetiver ``` And the
+development version from [GitHub](https://github.com/rstudio/vetiver-python)
+with: ```python python -m pip install git+https://github.com/rstudio/vetiver-
+python ``` ## Example A `VetiverModel()` object collects the information needed
+to store, version, and deploy a trained model. ```python from vetiver import
+mock, VetiverModel X, y = mock.get_mock_data() model = mock.get_mock_model
+().fit(X, y) v = VetiverModel(model, model_name='mock_model', prototype_data=X)
+``` You can **version** and **share** your `VetiverModel()` by choosing a
+[pins](https://rstudio.github.io/pins-python/) "board" for it, including a
+local folder, [Connect](https://posit.co/products/enterprise/connect/), Amazon
 S3, and more. ```python from pins import board_temp from vetiver import
 vetiver_pin_write model_board = board_temp(versioned = True, allow_pickle_read
 = True) vetiver_pin_write(model_board, v) ``` You can **deploy** your pinned
 `VetiverModel()` using `VetiverAPI()`, an extension of [FastAPI](https://
 fastapi.tiangolo.com/). ```python from vetiver import VetiverAPI app =
 VetiverAPI(v, check_prototype = True) ``` To start a server using this object,
 use `app.run(port = 8080)` or your port of choice. ## Contributing This project
 is released with a [Contributor Code of Conduct](https://www.contributor-
 covenant.org/version/2/1/CODE_OF_CONDUCT.html). By contributing to this
 project, you agree to abide by its terms. - For questions and discussions about
 deploying models, statistical modeling, and machine learning, please [post on
-RStudio Community](https://community.rstudio.com/new-
+Posit Community](https://community.rstudio.com/new-
 topic?category_id=15&tags=vetiver,question). - If you think you have
 encountered a bug, please [submit an issue](https://github.com/rstudio/vetiver-
 python/issues).
```

### Comparing `vetiver-0.2.0/vetiver.egg-info/SOURCES.txt` & `vetiver-0.2.1/vetiver.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 .pre-commit-config.yaml
 CODE_OF_CONDUCT.md
 LICENSE
+MAINTAINERS.md
 MANIFEST.in
 Makefile
 README.md
 docker-compose.yml
 pyproject.toml
 setup.cfg
 setup.py
@@ -13,47 +14,46 @@
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/release-checklist.md
 .github/workflows/docs.yml
 .github/workflows/precommit.yml
 .github/workflows/tests.yml
 .github/workflows/weekly.yml
+docs/.gitignore
 docs/Makefile
-docs/make.bat
+docs/_quarto.yml
+docs/changelog.md
+docs/custom_handler.md
+docs/index.qmd
+docs/version_config.py
+docs/_extensions/machow/interlinks/.gitignore
+docs/_extensions/machow/interlinks/README.md
+docs/_extensions/machow/interlinks/_extension.yml
+docs/_extensions/machow/interlinks/example.qmd
+docs/_extensions/machow/interlinks/interlinks.py
+docs/_extensions/machow/interlinks/objects_siuba.json
+docs/_extensions/machow/interlinks/objects_vetiver.inv
+docs/_extensions/machow/interlinks/objects_vetiver.json
 docs/figures/logo.png
 docs/figures/logo.svg
-docs/source/conf.py
-docs/source/index.rst
-docs/source/advancedusage/custom_handler.md
-docs/source/reference/vetiver.VetiverAPI.rst
-docs/source/reference/vetiver.VetiverAPI.run.rst
-docs/source/reference/vetiver.VetiverAPI.vetiver_post.rst
-docs/source/reference/vetiver.VetiverModel.rst
-docs/source/reference/vetiver.load_pkgs.rst
-docs/source/reference/vetiver.pin_read_write.vetiver_pin_read.rst
-docs/source/reference/vetiver.pin_read_write.vetiver_pin_write.rst
-docs/source/reference/vetiver.predict.rst
-docs/source/reference/vetiver.vetiver_endpoint.rst
-docs/source/reference/vetiver.vetiver_write_app.rst
-docs/source/reference/vetiver.vetiver_write_docker.rst
 examples/coffeeratings.py
 examples/coffeeratings/Dockerfile
 examples/coffeeratings/app.py
 examples/coffeeratings/vetiver_requirements.txt
 examples/coffeeratings/v/20220415T174503Z-06d9b/data.txt
 examples/coffeeratings/v/20220415T174503Z-06d9b/v.joblib
-requirements/dev.txt
 script/setup-docker/.gitignore
 script/setup-docker/docker.py
 script/setup-rsconnect/add-users.sh
 script/setup-rsconnect/dump_api_keys.py
 script/setup-rsconnect/rstudio-connect.gcfg
 script/setup-rsconnect/users.txt
 vetiver/__init__.py
 vetiver/attach_pkgs.py
+vetiver/helpers.py
 vetiver/meta.py
 vetiver/mock.py
 vetiver/model_card.py
 vetiver/monitor.py
 vetiver/pin_read_write.py
 vetiver/prototype.py
 vetiver/rsconnect.py
@@ -71,31 +71,32 @@
 vetiver/data/__init__.py
 vetiver/data/chicago.csv
 vetiver/data/mtcars.csv
 vetiver/data/sacramento.csv
 vetiver/handlers/__init__.py
 vetiver/handlers/base.py
 vetiver/handlers/sklearn.py
+vetiver/handlers/spacy.py
 vetiver/handlers/statsmodels.py
 vetiver/handlers/torch.py
 vetiver/handlers/xgboost.py
 vetiver/templates/model_card.qmd
 vetiver/tests/rsconnect_api_keys.json
 vetiver/tests/test_add_endpoint.py
 vetiver/tests/test_build_api.py
 vetiver/tests/test_build_vetiver_model.py
 vetiver/tests/test_custom_handler.py
 vetiver/tests/test_mock_data.py
 vetiver/tests/test_monitor.py
 vetiver/tests/test_no_handler.py
 vetiver/tests/test_pin_write.py
-vetiver/tests/test_ping_server.py
-vetiver/tests/test_predict.py
 vetiver/tests/test_prepare_docker.py
 vetiver/tests/test_pytorch.py
 vetiver/tests/test_rsconnect.py
+vetiver/tests/test_server.py
 vetiver/tests/test_sklearn.py
+vetiver/tests/test_spacy.py
 vetiver/tests/test_statsmodels.py
 vetiver/tests/test_write_app.py
 vetiver/tests/test_write_docker.py
 vetiver/tests/test_xgboost.py
 vetiver/tests/snapshots/test_monitor.json
```

