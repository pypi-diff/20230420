# Comparing `tmp/prunerr-1.1.1b0.tar.gz` & `tmp/prunerr-1.1.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prunerr-1.1.1b0.tar", last modified: Sun Apr 16 17:06:51 2023, max compression
+gzip compressed data, was "prunerr-1.1.2b1.tar", last modified: Thu Apr 20 00:48:22 2023, max compression
```

## Comparing `prunerr-1.1.1b0.tar` & `prunerr-1.1.2b1.tar`

### file list

```diff
@@ -1,1374 +1,1377 @@
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      543 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/.dir-locals.el.in
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1485 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/.dockerignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1226 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/.env.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/.github/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/.github/workflows/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3938 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/.github/workflows/build-test.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1485 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4466 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/.gitlab-ci.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      779 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/.pre-commit-config.yaml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2448 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/.prospector.yaml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4109 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/CONTRIBUTING.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2430 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/Dockerfile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2753 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/Dockerfile.devel
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1081 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/LICENSE
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    59200 2023-04-16 16:54:04.000000 prunerr-1.1.1b0/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      168 2023-04-16 16:55:55.000000 prunerr-1.1.1b0/NEWS-VERSION.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3997 2023-04-16 16:55:58.000000 prunerr-1.1.1b0/NEWS.rst
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    14101 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/PKG-INFO
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13114 2023-04-16 16:54:04.000000 prunerr-1.1.1b0/README.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3726 2023-04-16 16:54:04.000000 prunerr-1.1.1b0/TODO.rst
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/bin/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2792 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/bin/cz-check-bump
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      918 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/bin/entrypoint
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     1101 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/bin/get-base-version
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      321 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/bin/hadolint
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/build-host/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1994 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/build-host/Dockerfile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1464 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/build-host/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      746 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/build-host/README.rst
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/build-host/bin/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2041 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/build-host/bin/entrypoint
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      731 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/build-host/requirements-py310.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      674 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/build-host/requirements-py311.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      948 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/build-host/requirements-py37.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      729 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/build-host/requirements-py38.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      729 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/build-host/requirements-py39.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        4 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/build-host/requirements.txt.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/dist/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/dist/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1397 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/docker-compose-servarr.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5046 2023-04-16 16:54:04.000000 prunerr-1.1.1b0/docker-compose.override.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4029 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/docker-compose.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/gitlab-runner/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       46 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/gitlab-runner/.gitignore
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/gitlab-runner/config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1323 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/gitlab-runner/config/config.toml.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/home/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       64 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/home/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      327 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/home/.pypirc.in
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)     3007 2023-04-16 16:56:01.000000 prunerr-1.1.1b0/pyproject.toml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/requirements/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      578 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/requirements/build.txt.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/requirements/py310/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2414 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/requirements/py310/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5273 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/requirements/py310/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/requirements/py310/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/requirements/py311/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2414 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/requirements/py311/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5024 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/requirements/py311/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/requirements/py311/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/requirements/py37/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2645 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/requirements/py37/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     6115 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/requirements/py37/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1398 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/requirements/py37/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/requirements/py38/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2515 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/requirements/py38/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5591 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/requirements/py38/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/requirements/py38/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/requirements/py39/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2412 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/requirements/py39/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5578 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/requirements/py39/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-16 16:56:26.000000 prunerr-1.1.1b0/requirements/py39/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/s6/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/s6/etc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/s6/etc/s6-overlay/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/s6/etc/s6-overlay/s6-rc.d/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/s6/etc/s6-overlay/s6-rc.d/svc-transmission/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      243 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/s6/etc/s6-overlay/s6-rc.d/svc-transmission/finish
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1764 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/setup.cfg
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8429 2023-04-16 16:54:04.000000 prunerr-1.1.1b0/src/prunerr/__init__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      201 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/__main__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    15438 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/downloadclient.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11377 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/downloaditem.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/home/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/home/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9913 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/home/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/newsfragments/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       91 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/newsfragments/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     7937 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/operations.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    19064 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/runner.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11415 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/servarr.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      911 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    22019 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/__init__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    67861 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/example-5s.mkv
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/home/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/home/daemon/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/home/daemon/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3204 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/home/daemon/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/home/download-client-only/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/home/download-client-only/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/home/download-client-only/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/home/download-clients/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/home/download-clients/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2957 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/home/download-clients/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/home/download-items/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/home/download-items/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/home/download-items/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/home/empty/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/home/empty/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/home/empty/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/home/move-exec/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/home/move-exec/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       88 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/home/move-exec/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/home/review-edge-cases/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/home/review-edge-cases/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      820 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:05:45.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1077 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.878453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9537 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:05:45.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13662 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5081 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.882453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      126 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.910453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1484 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.886453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1495 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1498 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.914453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.890453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.894453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.918453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2102 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:05:45.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16163 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5383 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5495 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:05:45.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:05:45.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.898453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    27061 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       61 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.922453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10807 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.902453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      123 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.926453 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4730 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/test_cli.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2906 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/test_daemon.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8822 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/test_downloadclient.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3745 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/test_downloaditem.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11350 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/test_free_space.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    17208 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/test_move.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8074 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/test_operations.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13110 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/test_review.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1468 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/test_runner.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/test_servarr.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1204 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/tests/test_verify.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1374 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/src/prunerr/utils.py
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      162 2023-04-16 17:06:51.000000 prunerr-1.1.1b0/src/prunerr/version.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-16 17:06:51.906453 prunerr-1.1.1b0/src/prunerr.egg-info/
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    14101 2023-04-16 17:06:51.000000 prunerr-1.1.1b0/src/prunerr.egg-info/PKG-INFO
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    64648 2023-04-16 17:06:51.000000 prunerr-1.1.1b0/src/prunerr.egg-info/SOURCES.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)        1 2023-04-16 17:06:51.000000 prunerr-1.1.1b0/src/prunerr.egg-info/dependency_links.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)       41 2023-04-16 17:06:51.000000 prunerr-1.1.1b0/src/prunerr.egg-info/entry_points.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      327 2023-04-16 17:06:51.000000 prunerr-1.1.1b0/src/prunerr.egg-info/requires.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)        8 2023-04-16 17:06:51.000000 prunerr-1.1.1b0/src/prunerr.egg-info/top_level.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3321 2023-04-15 18:40:58.000000 prunerr-1.1.1b0/tox.ini
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.506140 prunerr-1.1.2b1/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      543 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/.dir-locals.el.in
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1485 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/.dockerignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1226 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/.env.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.434139 prunerr-1.1.2b1/.github/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/.github/workflows/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3938 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/.github/workflows/build-test.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1485 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4466 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/.gitlab-ci.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      779 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/.pre-commit-config.yaml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2448 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/.prospector.yaml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4109 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/CONTRIBUTING.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2430 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/Dockerfile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2753 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/Dockerfile.devel
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1081 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/LICENSE
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    58363 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       84 2023-04-20 00:04:51.000000 prunerr-1.1.2b1/NEWS-VERSION.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4248 2023-04-20 00:04:53.000000 prunerr-1.1.2b1/NEWS.rst
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    16130 2023-04-20 00:48:22.506140 prunerr-1.1.2b1/PKG-INFO
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    15143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/README.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4953 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/TODO.rst
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/bin/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2792 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/bin/cz-check-bump
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      918 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/bin/entrypoint
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     1101 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/bin/get-base-version
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      321 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/bin/hadolint
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/build-host/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1994 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/build-host/Dockerfile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1464 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/build-host/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      746 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/build-host/README.rst
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/build-host/bin/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2041 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/build-host/bin/entrypoint
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      731 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/build-host/requirements-py310.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      674 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/build-host/requirements-py311.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      948 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/build-host/requirements-py37.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      729 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/build-host/requirements-py38.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      729 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/build-host/requirements-py39.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        4 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/build-host/requirements.txt.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/dist/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/dist/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1397 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/docker-compose-servarr.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5132 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/docker-compose.override.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4047 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/docker-compose.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/gitlab-runner/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       46 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/gitlab-runner/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/gitlab-runner/config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1323 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/gitlab-runner/config/config.toml.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/home/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       64 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/home/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      327 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/home/.pypirc.in
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3007 2023-04-20 00:04:54.000000 prunerr-1.1.2b1/pyproject.toml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/requirements/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      578 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/requirements/build.txt.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/requirements/py310/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2414 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/requirements/py310/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5274 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/requirements/py310/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/requirements/py310/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/requirements/py311/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2414 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/requirements/py311/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5025 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/requirements/py311/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/requirements/py311/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/requirements/py37/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2645 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/requirements/py37/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     6116 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/requirements/py37/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1398 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/requirements/py37/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/requirements/py38/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2515 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/requirements/py38/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5592 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/requirements/py38/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/requirements/py38/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/requirements/py39/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2412 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/requirements/py39/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5579 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/requirements/py39/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-20 00:05:09.000000 prunerr-1.1.2b1/requirements/py39/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.434139 prunerr-1.1.2b1/s6/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.434139 prunerr-1.1.2b1/s6/etc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.434139 prunerr-1.1.2b1/s6/etc/s6-overlay/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.434139 prunerr-1.1.2b1/s6/etc/s6-overlay/s6-rc.d/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/s6/etc/s6-overlay/s6-rc.d/svc-transmission/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      243 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/s6/etc/s6-overlay/s6-rc.d/svc-transmission/finish
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1764 2023-04-20 00:48:22.506140 prunerr-1.1.2b1/setup.cfg
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/src/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8429 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/__init__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      201 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/__main__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    15438 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/downloadclient.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11377 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/downloaditem.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/home/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/home/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9913 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/home/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/newsfragments/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       91 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/newsfragments/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     7937 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/operations.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    19064 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/runner.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11415 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/servarr.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/tests/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      911 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    22019 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/__init__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    67861 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/example-5s.mkv
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/home/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/home/daemon/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/tests/home/daemon/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3204 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/home/daemon/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/home/download-client-only/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/tests/home/download-client-only/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/home/download-client-only/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/home/download-clients/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/tests/home/download-clients/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2957 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/home/download-clients/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/home/download-items/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/tests/home/download-items/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/home/download-items/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/home/empty/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/tests/home/empty/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/home/empty/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/home/move-exec/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/tests/home/move-exec/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       88 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/home/move-exec/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/home/review-edge-cases/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/tests/home/review-edge-cases/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      820 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:47:12.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1077 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9537 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:47:12.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.438139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.478140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13662 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5081 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.442139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      126 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.482140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1484 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.446139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1495 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.486140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1498 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.450139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.490140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.454139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.458140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.494140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2102 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:47:12.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.462139 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16163 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5383 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.498140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5495 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:47:12.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:47:12.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    27061 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       61 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10807 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.466140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.502140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.506140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.506140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      123 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.506140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.506140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.506140 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4730 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/test_cli.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2906 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/test_daemon.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8822 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/test_downloadclient.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3745 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/test_downloaditem.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11350 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/test_free_space.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    17208 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/test_move.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8074 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/test_operations.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13110 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/test_review.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1468 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/test_runner.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/test_servarr.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1204 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/tests/test_verify.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1374 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/prunerr/utils.py
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)      162 2023-04-20 00:48:22.000000 prunerr-1.1.2b1/src/prunerr/version.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.474140 prunerr-1.1.2b1/src/prunerr.egg-info/
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    16130 2023-04-20 00:48:22.000000 prunerr-1.1.2b1/src/prunerr.egg-info/PKG-INFO
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    64722 2023-04-20 00:48:22.000000 prunerr-1.1.2b1/src/prunerr.egg-info/SOURCES.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)        1 2023-04-20 00:48:22.000000 prunerr-1.1.2b1/src/prunerr.egg-info/dependency_links.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)       41 2023-04-20 00:48:22.000000 prunerr-1.1.2b1/src/prunerr.egg-info/entry_points.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)      327 2023-04-20 00:48:22.000000 prunerr-1.1.2b1/src/prunerr.egg-info/requires.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)        8 2023-04-20 00:48:22.000000 prunerr-1.1.2b1/src/prunerr.egg-info/top_level.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.470140 prunerr-1.1.2b1/src/pythonprojectstructure/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-20 00:48:22.506140 prunerr-1.1.2b1/src/pythonprojectstructure/newsfragments/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       87 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/src/pythonprojectstructure/newsfragments/+upgrade-requirements.bugfix.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3321 2023-04-20 00:02:46.000000 prunerr-1.1.2b1/tox.ini
```

### Comparing `prunerr-1.1.1b0/.dir-locals.el.in` & `prunerr-1.1.2b1/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/.dockerignore` & `prunerr-1.1.2b1/.dockerignore`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/.env.in` & `prunerr-1.1.2b1/.env.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/.github/workflows/build-test.yml` & `prunerr-1.1.2b1/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/.gitignore` & `prunerr-1.1.2b1/.gitignore`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/.gitlab-ci.yml` & `prunerr-1.1.2b1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/.pre-commit-config.yaml` & `prunerr-1.1.2b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/.prospector.yaml` & `prunerr-1.1.2b1/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/CONTRIBUTING.rst` & `prunerr-1.1.2b1/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ########################################################################################
-CONTRIBUTING
+Contributing
 ########################################################################################
 
 Development requires fairly standard development tools, but ``git`` and ``make`` to
 bootstrap the local development environment.  Once installed, clone the repository::
 
   $ git clone "https://gitlab.com/rpatterson/prunerr"
```

### Comparing `prunerr-1.1.1b0/Dockerfile` & `prunerr-1.1.2b1/Dockerfile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/Dockerfile.devel` & `prunerr-1.1.2b1/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/LICENSE` & `prunerr-1.1.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/Makefile` & `prunerr-1.1.2b1/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -215,57 +215,61 @@
 export TOX_RUN_ARGS
 # The options that allow for rapid execution of arbitrary commands in the venvs managed
 # by tox
 TOX_EXEC_OPTS=--no-recreate-pkg --skip-pkg-install
 TOX_EXEC_ARGS=tox exec $(TOX_EXEC_OPTS) -e "$(PYTHON_ENV)" --
 TOX_EXEC_BUILD_ARGS=tox exec $(TOX_EXEC_OPTS) -e "build" --
 
-# Values used to build Docker images and run containers:
+# Values used to build Docker images:
+DOCKER_FILE=./Dockerfile
+DOCKER_PLATFORMS=
+DOCKER_BUILD_ARGS=--output "type=docker"
+export DOCKER_BUILD_PULL=false
+# Values used to tag built images:
+export DOCKER_VARIANT=
+DOCKER_VARIANT_PREFIX=
+ifneq ($(DOCKER_VARIANT),)
+DOCKER_VARIANT_PREFIX=$(DOCKER_VARIANT)-
+endif
+export DOCKER_BRANCH_TAG=$(subst /,-,$(VCS_BRANCH))
 GITLAB_CI=false
 GITHUB_ACTIONS=false
 CI_PROJECT_NAMESPACE=$(CI_UPSTREAM_NAMESPACE)
 CI_TEMPLATE_REGISTRY_HOST=registry.gitlab.com
 CI_REGISTRY=$(CI_TEMPLATE_REGISTRY_HOST)/$(CI_PROJECT_NAMESPACE)
 CI_REGISTRY_IMAGE=$(CI_REGISTRY)/$(CI_PROJECT_NAME)
-DOCKER_COMPOSE_RUN_ARGS=
-DOCKER_COMPOSE_RUN_ARGS+= --rm
-ifneq ($(CI),true)
-DOCKER_COMPOSE_RUN_ARGS+= --quiet-pull
-endif
-ifeq ($(shell tty),not a tty)
-DOCKER_COMPOSE_RUN_ARGS+= -T
-endif
-DOCKER_BUILD_ARGS=
 DOCKER_REGISTRIES=DOCKER GITLAB GITHUB
 export DOCKER_REGISTRY=$(firstword $(DOCKER_REGISTRIES))
 DOCKER_IMAGE_DOCKER=$(DOCKER_USER)/$(CI_PROJECT_NAME)
 DOCKER_IMAGE_GITLAB=$(CI_REGISTRY_IMAGE)
 DOCKER_IMAGE_GITHUB=ghcr.io/$(CI_PROJECT_NAMESPACE)/$(CI_PROJECT_NAME)
 DOCKER_IMAGE=$(DOCKER_IMAGE_$(DOCKER_REGISTRY))
 DOCKER_IMAGES=
 ifeq ($(GITLAB_CI),true)
 DOCKER_IMAGES+=$(DOCKER_IMAGE_GITLAB)
 else ifeq ($(GITHUB_ACTIONS),true)
 DOCKER_IMAGES+=$(DOCKER_IMAGE_GITHUB)
 else
 DOCKER_IMAGES+=$(DOCKER_IMAGE_DOCKER)
 endif
-export DOCKER_VARIANT=
-DOCKER_VARIANT_PREFIX=
-ifneq ($(DOCKER_VARIANT),)
-DOCKER_VARIANT_PREFIX=$(DOCKER_VARIANT)-
-endif
-export DOCKER_BRANCH_TAG=$(subst /,-,$(VCS_BRANCH))
+# Values used to run built images in containers:
 DOCKER_VOLUMES=\
 ./var/docker/$(PYTHON_ENV)/ \
 ./src/prunerr.egg-info/ \
 ./var/docker/$(PYTHON_ENV)/prunerr.egg-info/ \
 ./.tox/ ./var/docker/$(PYTHON_ENV)/.tox/ \
 ./var/media/Library/
-export DOCKER_BUILD_PULL=false
+DOCKER_COMPOSE_RUN_ARGS=
+DOCKER_COMPOSE_RUN_ARGS+= --rm
+ifneq ($(CI),true)
+DOCKER_COMPOSE_RUN_ARGS+= --quiet-pull
+endif
+ifeq ($(shell tty),not a tty)
+DOCKER_COMPOSE_RUN_ARGS+= -T
+endif
 
 # Values derived from or overridden by CI environments:
 GITHUB_REPOSITORY_OWNER=$(CI_UPSTREAM_NAMESPACE)
 # Determine if this checkout is a fork of the upstream project:
 CI_IS_FORK=false
 ifeq ($(GITLAB_CI),true)
 USER_EMAIL=$(USER_NAME)@runners-manager.gitlab.com
@@ -325,18 +329,20 @@
 # canonical CI/CD platform:
 ifeq ($(GITLAB_CI),true)
 ifeq ($(VCS_BRANCH),main)
 RELEASE_PUBLISH=true
 PYPI_REPO=pypi
 PYPI_HOSTNAME=pypi.org
 GITHUB_RELEASE_ARGS=
+DOCKER_PLATFORMS=linux/amd64,linux/arm64,linux/arm/v7
 else ifeq ($(VCS_BRANCH),develop)
 # Publish pre-releases from the `develop` branch:
 RELEASE_PUBLISH=true
 PYPI_REPO=pypi
+DOCKER_PLATFORMS=linux/amd64,linux/arm64,linux/arm/v7
 endif
 endif
 CI_REGISTRY_USER=$(CI_PROJECT_NAMESPACE)
 CI_REGISTRY_IMAGE=$(CI_REGISTRY)/$(CI_PROJECT_NAME)
 # Address undefined variables warnings when running under local development
 PYPI_PASSWORD=
 export PYPI_PASSWORD
@@ -491,14 +497,73 @@
 	echo $${docker_image}:latest
 else
 	echo $${docker_image}:$(DOCKER_VARIANT)
 endif
 endif
 endif
 
+.PHONY: build-docker-build
+### Run the actual commands used to build the Docker container image.
+build-docker-build: $(HOME)/.local/var/log/docker-multi-platform-host-install.log \
+		./var/log/tox/build/build.log \
+		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
+		./var/log/docker-login-DOCKER.log
+# https://github.com/moby/moby/issues/39003#issuecomment-879441675
+ifeq ($(CI),true)
+# Workaround broken interactive session detection
+	docker pull "python:$(PYTHON_MINOR)"
+endif
+	docker_build_caches=""
+ifeq ($(GITLAB_CI),true)
+# Don't cache when building final releases on `main`
+	$(MAKE) -e "./var/log/docker-login-GITLAB.log" || true
+ifneq ($(VCS_BRANCH),main)
+	if $(MAKE) -e pull-docker
+	then
+	    docker_build_caches+=" --cache-from $(DOCKER_IMAGE_GITLAB):\
+	$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
+	fi
+endif
+endif
+ifeq ($(GITHUB_ACTIONS),true)
+	$(MAKE) -e "./var/log/docker-login-GITHUB.log" || true
+ifneq ($(VCS_BRANCH),main)
+	if $(MAKE) -e pull-docker
+	then
+	    docker_build_caches+=" --cache-from $(DOCKER_IMAGE_GITHUB):\
+	$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
+	fi
+endif
+endif
+	docker_image_tags=""
+	for image_tag in $$(
+	    $(MAKE) -e --no-print-directory build-docker-tags
+	)
+	do
+	    docker_image_tags+="--tag $${image_tag} "
+	done
+# https://github.com/moby/moby/issues/39003#issuecomment-879441675
+	docker buildx build $(DOCKER_BUILD_ARGS) \
+	    --build-arg BUILDKIT_INLINE_CACHE="1" \
+	    --build-arg PYTHON_MINOR="$(PYTHON_MINOR)" \
+	    --build-arg PYTHON_ENV="$(PYTHON_ENV)" \
+	    --build-arg VERSION="$$(./.tox/build/bin/cz version --project)" \
+	    $${docker_image_tags} $${docker_build_caches} --file "$(DOCKER_FILE)" "./"
+# Ensure any subsequent builds have optimal caches
+ifeq ($(GITLAB_CI),true)
+	docker push "$(DOCKER_IMAGE_GITLAB):\
+	$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
+endif
+ifeq ($(GITHUB_ACTIONS),true)
+ifneq ($(CI_IS_FORK),true)
+	docker push "$(DOCKER_IMAGE_GITHUB):\
+	$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
+endif
+endif
+
 .PHONY: $(PYTHON_MINORS:%=build-docker-requirements-%)
 ### Pull container images and compile fixed/pinned dependency versions if necessary.
 $(PYTHON_MINORS:%=build-docker-requirements-%): ./.env
 	export PYTHON_MINOR="$(@:build-docker-requirements-%=%)"
 	export PYTHON_ENV="py$(subst .,,$(@:build-docker-requirements-%=%))"
 	$(MAKE) -e build-docker-volumes-$${PYTHON_ENV} \
 	    "./var/docker/$${PYTHON_ENV}/log/build-devel.log"
@@ -712,47 +777,43 @@
 ### Publish all container images to all container registries.
 release-docker: build-docker-volumes-$(PYTHON_ENV) build-docker \
 		$(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log)
 	$(MAKE) -e -j DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
 	    $(PYTHON_MINORS:%=release-docker-%)
 
 .PHONY: $(PYTHON_MINORS:%=release-docker-%)
-### Publish the container images for one Python version to all container registry.
-$(PYTHON_MINORS:%=release-docker-%): $(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log)
+### Publish the container images for one Python version to all container registries.
+$(PYTHON_MINORS:%=release-docker-%): \
+		$(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log) \
+		$(HOME)/.local/var/log/docker-multi-platform-host-install.log
 	export PYTHON_ENV="py$(subst .,,$(@:release-docker-%=%))"
-	$(MAKE) -e -j DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
-	    $(DOCKER_REGISTRIES:%=release-docker-registry-%)
+# Build other platforms in emulation and rely on the layer cache for bundling the
+# previously built native images into the manifests.
+	DOCKER_BUILD_ARGS="--push"
+ifneq ($(DOCKER_PLATFORMS),)
+	DOCKER_BUILD_ARGS+=" --platform $(DOCKER_PLATFORMS)"
+endif
+	export DOCKER_BUILD_ARGS
+# Push the development manifest and images:
+	$(MAKE) -e DOCKER_FILE="./Dockerfile.devel" DOCKER_VARIANT="devel" \
+	    build-docker-build
+# Push the end-user manifest and images:
+	PYTHON_WHEEL="$$(ls -t ./dist/*.whl | head -n 1)"
+	$(MAKE) -e DOCKER_BUILD_ARGS="$${DOCKER_BUILD_ARGS}\
+	    --build-arg PYTHON_WHEEL=$${PYTHON_WHEEL}" build-docker-build
+# Update Docker Hub `README.md` from the official/canonical Python version:
 ifeq ($(VCS_BRANCH),main)
-ifeq ($${PYTHON_ENV},$(PYTHON_HOST_ENV))
-	$(MAKE) -e "./var/log/docker-login-DOCKER.log"
-	docker compose pull pandoc docker-pushrm
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) docker-pushrm
-endif
+	if [ "$${PYTHON_ENV}" == "$(PYTHON_HOST_ENV)" ]
+	then
+	    $(MAKE) -e "./var/log/docker-login-DOCKER.log"
+	    docker compose pull pandoc docker-pushrm
+	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) docker-pushrm
+	fi
 endif
 
-.PHONY: $(DOCKER_REGISTRIES:%=release-docker-registry-%)
-### Publish all container images to one container registry.
-$(DOCKER_REGISTRIES:%=release-docker-registry-%):
-# https://docs.docker.com/docker-hub/#step-5-build-and-push-a-container-image-to-docker-hub-from-your-computer
-	$(MAKE) -e "./var/log/docker-login-$(@:release-docker-registry-%=%).log"
-	for user_tag in $$(
-	    $(MAKE) -e --no-print-directory \
-	        build-docker-tags-$(@:release-docker-registry-%=%)
-	)
-	do
-	    docker push "$${user_tag}"
-	done
-	for devel_tag in $$(
-	    $(MAKE) -e DOCKER_VARIANT="devel" --no-print-directory \
-	        build-docker-tags-$(@:release-docker-registry-%=%)
-	)
-	do
-	    docker push "$${devel_tag}"
-	done
-
 .PHONY: release-bump
 ### Bump the package version if on a branch that should trigger a release.
 release-bump: ~/.gitconfig $(VCS_RELEASE_FETCH_TARGETS) \
 		./var/log/git-remotes.log ./var/log/tox/build/build.log \
 		./var/docker/$(PYTHON_ENV)/log/build-devel.log \
 		./.env build-docker-volumes-$(PYTHON_ENV)
 	if ! git diff --cached --exit-code
@@ -1022,87 +1083,30 @@
 ./var/docker/$(PYTHON_ENV)/log/build-devel.log: \
 		./Dockerfile.devel ./.dockerignore ./bin/entrypoint \
 		./pyproject.toml ./setup.cfg ./tox.ini \
 		./build-host/requirements.txt.in ./docker-compose.yml \
 		./docker-compose.override.yml ./.env \
 		./var/docker/$(PYTHON_ENV)/log/rebuild.log
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e "./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH)" \
-	    build-docker-volumes-$(PYTHON_ENV) "./var/log/tox/build/build.log" \
-	    "./var/log/docker-login-DOCKER.log"
+	$(MAKE) -e build-docker-volumes-$(PYTHON_ENV)
 	mkdir -pv "$(dir $(@))"
-# Workaround issues with local images and the development image depending on the end
-# user image.  It seems that `depends_on` isn't sufficient.
-	$(MAKE) -e $(HOME)/.local/var/log/prunerr-host-install.log
-	export VERSION=$$(./.tox/build/bin/cz version --project)
 ifeq ($(DOCKER_BUILD_PULL),true)
 # Pull the development image and simulate as if it had been built here.
 	if $(MAKE) -e DOCKER_VARIANT="devel" pull-docker
 	then
 	    touch "$(@)" "./var/docker/$(PYTHON_ENV)/log/rebuild.log"
 # Ensure the virtualenv in the volume is also current:
 	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) \
 	        prunerr-devel make -e PYTHON_MINORS="$(PYTHON_MINOR)" \
 	        "./var/log/tox/$(PYTHON_ENV)/build.log"
 	    exit
 	fi
 endif
-# https://github.com/moby/moby/issues/39003#issuecomment-879441675
-	docker_build_args="$(DOCKER_BUILD_ARGS) \
-	    --build-arg BUILDKIT_INLINE_CACHE=1 \
-	    --build-arg PYTHON_MINOR=$(PYTHON_MINOR) \
-	    --build-arg PYTHON_ENV=$(PYTHON_ENV) \
-	    --build-arg VERSION=$${VERSION}"
-	docker_build_devel_tags=""
-	for devel_tag in $$(
-	    $(MAKE) -e DOCKER_VARIANT="devel" --no-print-directory build-docker-tags
-	)
-	do
-	    docker_build_devel_tags+="--tag $${devel_tag} "
-	done
-	docker_build_caches=""
-ifeq ($(GITLAB_CI),true)
-# Don't cache when building final releases on `main`
-	$(MAKE) -e "./var/log/docker-login-GITLAB.log" || true
-ifneq ($(VCS_BRANCH),main)
-	if $(MAKE) -e DOCKER_VARIANT="devel" pull-docker
-	then
-	    docker_build_caches+=" --cache-from \
-	$(DOCKER_IMAGE_GITLAB):devel-$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-	fi
-endif
-endif
-ifeq ($(GITHUB_ACTIONS),true)
-	$(MAKE) -e "./var/log/docker-login-GITHUB.log" || true
-ifneq ($(VCS_BRANCH),main)
-	if $(MAKE) -e DOCKER_VARIANT="devel" pull-docker
-	then
-	    docker_build_caches+=" --cache-from \
-	$(DOCKER_IMAGE_GITHUB):devel-$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-	fi
-endif
-endif
-ifeq ($(CI),true)
-# Workaround broken interactive session detection
-	docker pull "python:${PYTHON_MINOR}"
-endif
-	docker buildx build $${docker_build_args} $${docker_build_devel_tags} \
-	    $${docker_build_caches} --file "./Dockerfile.devel" "./"
-# Ensure any subsequent builds have optimal caches
-ifeq ($(GITLAB_CI),true)
-	docker push \
-	    "$(DOCKER_IMAGE_GITLAB):devel-$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-endif
-ifeq ($(GITHUB_ACTIONS),true)
-ifneq ($(CI_IS_FORK),true)
-	docker push \
-	    "$(DOCKER_IMAGE_GITHUB):devel-$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-endif
-endif
-	date >>"$(@)"
+	$(MAKE) -e DOCKER_FILE="./Dockerfile.devel" DOCKER_VARIANT="devel" \
+	    build-docker-build >>"$(@)"
 # Update the pinned/frozen versions, if needed, using the container.  If changed, then
 # we may need to re-build the container image again to ensure it's current and correct.
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) prunerr-devel \
 	    make -e PYTHON_MINORS="$(PYTHON_MINOR)" build-requirements-$(PYTHON_ENV)
 ifeq ($(CI),true)
 # On CI, any changes from compiling requirements is a failure so no need to waste time
 # rebuilding images:
@@ -1112,67 +1116,24 @@
 endif
 
 # Build the end-user image:
 ./var/docker/$(PYTHON_ENV)/log/build-user.log: \
 		./var/docker/$(PYTHON_ENV)/log/build-devel.log ./Dockerfile \
 		./var/docker/$(PYTHON_ENV)/log/rebuild.log
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e "./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH)" \
-	    "./var/log/tox/build/build.log"
-	mkdir -pv "$(dir $(@))"
-	export VERSION=$$(./.tox/build/bin/cz version --project)
-# https://github.com/moby/moby/issues/39003#issuecomment-879441675
-	docker_build_args="$(DOCKER_BUILD_ARGS) \
-	    --build-arg BUILDKIT_INLINE_CACHE=1 \
-	    --build-arg PYTHON_MINOR=$(PYTHON_MINOR) \
-	    --build-arg PYTHON_ENV=$(PYTHON_ENV) \
-	    --build-arg VERSION=$${VERSION}"
-# Build the end-user image now that all required artifacts are built"
 ifeq ($(PYTHON_WHEEL),)
 	$(MAKE) -e "build-pkgs"
 	PYTHON_WHEEL="$$(ls -t ./dist/*.whl | head -n 1)"
 endif
-	docker_build_user_tags=""
-	for user_tag in $$($(MAKE) -e --no-print-directory build-docker-tags)
-	do
-	    docker_build_user_tags+="--tag $${user_tag} "
-	done
-	docker_build_caches=""
-ifeq ($(GITLAB_CI),true)
-ifneq ($(VCS_BRANCH),main)
-	if $(MAKE) -e pull-docker
-	then
-	    docker_build_caches+=" \
-	--cache-from $(DOCKER_IMAGE_GITLAB):$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-	fi
-endif
-endif
-ifeq ($(GITHUB_ACTIONS),true)
-ifneq ($(VCS_BRANCH),main)
-	if $(MAKE) -e pull-docker
-	then
-	    docker_build_caches+=" \
-	--cache-from $(DOCKER_IMAGE_GITHUB):$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-	fi
-endif
-endif
-	docker buildx build $${docker_build_args} $${docker_build_user_tags} \
-	    --build-arg PYTHON_WHEEL="$${PYTHON_WHEEL}" $${docker_build_caches} "./"
-# Ensure any subsequent builds have optimal caches
-ifeq ($(GITLAB_CI),true)
-	docker push "$(DOCKER_IMAGE_GITLAB):$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-endif
-ifeq ($(GITHUB_ACTIONS),true)
-ifneq ($(CI_IS_FORK),true)
-	docker push "$(DOCKER_IMAGE_GITHUB):$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-endif
-endif
-	date >>"$(@)"
-# The images install the host requirements, reflect that in the bind mount volumes
-	date >>"$(@:%/build.log=%/host-install.log)"
+# Build the end-user image now that all required artifacts are built"
+	mkdir -pv "$(dir $(@))"
+	$(MAKE) -e DOCKER_BUILD_ARGS="$(DOCKER_BUILD_ARGS)\
+	    --build-arg PYTHON_WHEEL=$${PYTHON_WHEEL}" build-docker-build >>"$(@)"
+# The image installs the host requirements, reflect that in the bind mount volumes
+	date >>"$(@:%/build-user.log=%/host-install.log)"
 
 ./var/ $(PYTHON_ENVS:%=./var/docker/%/) \
 ./src/prunerr.egg-info/ \
 $(PYTHON_ENVS:%=./var/docker/%/prunerr.egg-info/) \
 ./.tox/ $(PYTHON_ENVS:%=./var/docker/%/.tox/) \
 ./var/media/Library/:
 	mkdir -pv "$(@)"
@@ -1217,14 +1178,20 @@
 	    then
 	        pip install -r "./build-host/requirements-$(PYTHON_HOST_ENV).txt"
 	    else
 	        pip install -r "./build-host/requirements.txt.in"
 	    fi
 	) | tee -a "$(@)"
 
+# https://docs.docker.com/build/building/multi-platform/#building-multi-platform-images
+$(HOME)/.local/var/log/docker-multi-platform-host-install.log:
+	mkdir -pv "$(dir $(@))"
+	docker context create "multi-platform" |& tee -a "$(@)"
+	docker buildx create --use "multi-platform" |& tee -a "$(@)"
+
 ./var/log/codecov-install.log:
 	mkdir -pv "$(dir $(@))"
 # Install the code test coverage publishing tool
 	(
 	    if ! which codecov
 	    then
 	        mkdir -pv ~/.local/bin/
```

### Comparing `prunerr-1.1.1b0/NEWS.rst` & `prunerr-1.1.2b1/NEWS.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+prunerr 1.1.2b1 (2023-04-20)
+============================
+
+No significant changes.
+
+
+prunerr 1.1.2b0 (2023-04-18)
+============================
+
+No significant changes.
+
+
+prunerr 1.1.1 (2023-04-16)
+==========================
+
+No significant changes.
+
+
 prunerr 1.1.1b0 (2023-04-16)
 ============================
 
 Bugfixes
 --------
 
 - Upgrade all requirements to the latest versions as of Sun Apr 16 03:54:21 PM UTC 2023.
```

### Comparing `prunerr-1.1.1b0/PKG-INFO` & `prunerr-1.1.2b1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: prunerr
-Version: 1.1.1b0
-Summary: Perma-seed Servarr media libraries
-Home-page: https://gitlab.com/rpatterson/prunerr
-Author: Ross Patterson
-Author-email: me@rpatterson.net
-License: MIT
-Keywords: servarr,sonarr,radarr,transmission,bittorent,torrent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: BSD
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Communications :: File Sharing
-Classifier: Topic :: Internet
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: devel
-License-File: LICENSE
-
 ########################################################################################
 Prunerr
 ########################################################################################
 Perma-seed Servarr media libraries
 ****************************************************************************************
 
 .. list-table::
@@ -82,23 +55,39 @@
        .. figure:: https://img.shields.io/docker/stars/merpatterson/prunerr?logo=docker
 	  :alt: Docker Hub stars
           :target: https://hub.docker.com/r/merpatterson/prunerr
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/prunerr?logo=docker
 	  :alt: Docker Hub image size (latest semver)
           :target: https://hub.docker.com/r/merpatterson/prunerr
 
+     - .. figure:: https://img.shields.io/keybase/pgp/rpatterson?logo=keybase
+          :alt: KeyBase PGP key ID
+          :target: https://keybase.io/rpatterson
+       .. figure:: https://img.shields.io/github/followers/rpatterson?style=social
+          :alt: GitHub followers count
+          :target: https://github.com/rpatterson
+       .. figure:: https://img.shields.io/liberapay/receives/rpatterson.svg?logo=liberapay
+          :alt: LiberaPay donated per week
+          :target: https://liberapay.com/rpatterson/donate
+       .. figure:: https://img.shields.io/liberapay/patrons/rpatterson.svg?logo=liberapay
+          :alt: LiberaPay patrons count
+          :target: https://liberapay.com/rpatterson/donate
+
+
 TL;DR: Perma-seeding of whole Servarr libraries optimized for per-tracker ratio.
 
 - Delete torrents/items only as disk space gets low.
 - Don't delete currently imported items.  IOW, only delete upgraded items.
 - Don't delete private items that haven't met seeding requirements.
 - Delete public items first
 - Delete private items in an order to maximize tracker ratio and/or bonuses.
 - And more...
 
+.. contents:: Table of Contents
+
 *******
 Summary
 *******
 
 Seed Servarr download client torrents/items as long as possible only deleting them as
 necessary as disk space gets low, hence the name based on "to prune".  Which download
 items are considered eligible for deletion is configured by the user.  The common case
@@ -132,22 +121,50 @@
 See the `Usage`_ section below for full details.
 
 
 ****************************************************************************************
 Installation
 ****************************************************************************************
 
+Install and use either via a local, native installation or a Docker container image:
+
+Local/Native Installation
+========================================================================================
+
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
-  $ sudo pip3 install prunerr
+  $ pip3 install --user prunerr
 
 Optional shell tab completion is available via `argcomplete`_.
 
-Or use `the Docker image`_.  See `the example ./docker-compose.yml file`_ for usage
-details.
+Docker Container Image Installation
+========================================================================================
+
+The recommended way to use the Docker container image is via `Docker Compose`_.  See
+`the example ./docker-compose.yml file`_ for an example configuration.  Once you have
+your configuration, you can create and run the container::
+
+  $ docker compose up
+
+Alternatively, you make use the image directly.  Pull `the Docker image`_::
+
+  $ docker pull "docker.io/merpatterson/prunerr"
+
+And then use the image to create and run a container::
+
+  $ docker run --rm -it "docker.io/merpatterson/prunerr" ...
+
+The Docker images support the following platforms or architectures:
+
+- ``linux/amd64``
+- ``linux/arm64``
+- ``linux/arm/v7``
+
+Images are tagged with the branch name so images tagged with ``main`` are final releases
+and images tagged with ``develop`` are pre-releases.
 
 
 ****************************************************************************************
 Usage
 ****************************************************************************************
 
 Start by writing your ``~/.config/prunerr.yml`` configuration file.  See the comments in
@@ -158,18 +175,18 @@
 loop using the ``$ prunerr daemon`` sub-command.  See the `Order of Operations`_ section
 for a detailed description of the operations.  Use the CLI help to list the other
 sub-commands and to get help on the individual sub-commands::
 
   $ prunerr --help
   $ prunerr exec --help
 
-Set the ``DEBUG`` environment variable to ``true`` to get verbose details and help
-understand what Prunerr is doing::
+If using the Docker container image, the container can be run from the command-line as
+well::
 
-  $ DEBUG=true prunerr exec
+  $ docker compose run "prunerr" prunerr --help
 
 
 *******************
 Order of Operations
 *******************
 
 Note that polling is required because there is no event we can subscribe to that
@@ -238,15 +255,15 @@
 
    For the other groups delete items in the order determined by the configured
    ``indexers/priorities`` indexer order then by the configured operations for that
    item's indexer.
 
 
 ****************************************************************************************
-CONTRIBUTING
+Contributing
 ****************************************************************************************
 
 NOTE: `This project is hosted on GitLab`_.  There's `a mirror on GitHub`_ but please use
 GitLab for reporting issues, submitting PRs/MRs and any other development or maintenance
 activity.
 
 See `the ./CONTRIBUTING.rst file`_ for more details on how to get started with
@@ -259,18 +276,22 @@
 
 I didn't like the available options I could find at the time for maximizing seeding from
 a lovingly managed media library.  Deleting by a ratio threshold doesn't make sense to
 me because that can delete items when there's plenty of disk space.  Also the ratio
 threshold is a reverse indicator for items from private indexers vs items from public
 indexers.  Items from private indexers with high ratios should be kept around as long as
 possible to build user total ratio whereas items from public indexers with low ratios
-should be kept around as long as possibility to preserve access in the
-community/ecosystem.  Finally, deleting any item still imported in the Servarr just
-because it hit the ratio threshold is the biggest waste since it doesn't free any space.
-So I wrote Prunerr to prune download items in the correct order.
+should be kept around as long as possible to preserve access in the community/ecosystem.
+Finally, deleting any item still imported in the Servarr just because it hit the ratio
+threshold is the biggest waste since it doesn't free any space.  So I wrote Prunerr to
+prune download items in the correct order.
+
+The use case for Prunerr is not tracker ratio racing.  It's goal it to seed as long as
+possible and to seed as much of your library as possible.  This should have some
+secondary benefits to ratio, but that's not the main goal.
 
 Finally, there is a laundry list of other download client management tasks that can be
 automated but aren't by anything I could find.  So I added them to Prunerr as well.
 
 
 .. _`Transmission BitTorrent client`: https://transmissionbt.com/
 
@@ -280,14 +301,15 @@
 .. _`download clients`: https://wiki.servarr.com/radarr/settings#download-clients
 .. _`FlexGet`: https://flexget.com/
 
 .. _pip: https://pip.pypa.io/en/stable/installation/
 .. _argcomplete: https://kislyuk.github.io/argcomplete/#installation
 
 .. _the Docker image: https://hub.docker.com/r/merpatterson/prunerr
+.. _`Docker Compose`: https://docs.docker.com/compose/
 .. _`the example ./docker-compose.yml file`: https://gitlab.com/rpatterson/prunerr/blob/main/docker-compose.yml
 
 .. _`the example configuration`:
    https://gitlab.com/rpatterson/prunerr/blob/main/src/prunerr/home/.config/prunerr.yml
 
 .. _`This project is hosted on GitLab`:
    https://gitlab.com/rpatterson/prunerr
```

### Comparing `prunerr-1.1.1b0/README.rst` & `prunerr-1.1.2b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: prunerr
+Version: 1.1.2b1
+Summary: Perma-seed Servarr media libraries
+Home-page: https://gitlab.com/rpatterson/prunerr
+Author: Ross Patterson
+Author-email: me@rpatterson.net
+License: MIT
+Keywords: servarr,sonarr,radarr,transmission,bittorent,torrent
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: BSD
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Communications :: File Sharing
+Classifier: Topic :: Internet
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: devel
+License-File: LICENSE
+
 ########################################################################################
 Prunerr
 ########################################################################################
 Perma-seed Servarr media libraries
 ****************************************************************************************
 
 .. list-table::
@@ -55,23 +82,39 @@
        .. figure:: https://img.shields.io/docker/stars/merpatterson/prunerr?logo=docker
 	  :alt: Docker Hub stars
           :target: https://hub.docker.com/r/merpatterson/prunerr
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/prunerr?logo=docker
 	  :alt: Docker Hub image size (latest semver)
           :target: https://hub.docker.com/r/merpatterson/prunerr
 
+     - .. figure:: https://img.shields.io/keybase/pgp/rpatterson?logo=keybase
+          :alt: KeyBase PGP key ID
+          :target: https://keybase.io/rpatterson
+       .. figure:: https://img.shields.io/github/followers/rpatterson?style=social
+          :alt: GitHub followers count
+          :target: https://github.com/rpatterson
+       .. figure:: https://img.shields.io/liberapay/receives/rpatterson.svg?logo=liberapay
+          :alt: LiberaPay donated per week
+          :target: https://liberapay.com/rpatterson/donate
+       .. figure:: https://img.shields.io/liberapay/patrons/rpatterson.svg?logo=liberapay
+          :alt: LiberaPay patrons count
+          :target: https://liberapay.com/rpatterson/donate
+
+
 TL;DR: Perma-seeding of whole Servarr libraries optimized for per-tracker ratio.
 
 - Delete torrents/items only as disk space gets low.
 - Don't delete currently imported items.  IOW, only delete upgraded items.
 - Don't delete private items that haven't met seeding requirements.
 - Delete public items first
 - Delete private items in an order to maximize tracker ratio and/or bonuses.
 - And more...
 
+.. contents:: Table of Contents
+
 *******
 Summary
 *******
 
 Seed Servarr download client torrents/items as long as possible only deleting them as
 necessary as disk space gets low, hence the name based on "to prune".  Which download
 items are considered eligible for deletion is configured by the user.  The common case
@@ -105,22 +148,50 @@
 See the `Usage`_ section below for full details.
 
 
 ****************************************************************************************
 Installation
 ****************************************************************************************
 
+Install and use either via a local, native installation or a Docker container image:
+
+Local/Native Installation
+========================================================================================
+
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
-  $ sudo pip3 install prunerr
+  $ pip3 install --user prunerr
 
 Optional shell tab completion is available via `argcomplete`_.
 
-Or use `the Docker image`_.  See `the example ./docker-compose.yml file`_ for usage
-details.
+Docker Container Image Installation
+========================================================================================
+
+The recommended way to use the Docker container image is via `Docker Compose`_.  See
+`the example ./docker-compose.yml file`_ for an example configuration.  Once you have
+your configuration, you can create and run the container::
+
+  $ docker compose up
+
+Alternatively, you make use the image directly.  Pull `the Docker image`_::
+
+  $ docker pull "docker.io/merpatterson/prunerr"
+
+And then use the image to create and run a container::
+
+  $ docker run --rm -it "docker.io/merpatterson/prunerr" ...
+
+The Docker images support the following platforms or architectures:
+
+- ``linux/amd64``
+- ``linux/arm64``
+- ``linux/arm/v7``
+
+Images are tagged with the branch name so images tagged with ``main`` are final releases
+and images tagged with ``develop`` are pre-releases.
 
 
 ****************************************************************************************
 Usage
 ****************************************************************************************
 
 Start by writing your ``~/.config/prunerr.yml`` configuration file.  See the comments in
@@ -131,18 +202,18 @@
 loop using the ``$ prunerr daemon`` sub-command.  See the `Order of Operations`_ section
 for a detailed description of the operations.  Use the CLI help to list the other
 sub-commands and to get help on the individual sub-commands::
 
   $ prunerr --help
   $ prunerr exec --help
 
-Set the ``DEBUG`` environment variable to ``true`` to get verbose details and help
-understand what Prunerr is doing::
+If using the Docker container image, the container can be run from the command-line as
+well::
 
-  $ DEBUG=true prunerr exec
+  $ docker compose run "prunerr" prunerr --help
 
 
 *******************
 Order of Operations
 *******************
 
 Note that polling is required because there is no event we can subscribe to that
@@ -211,15 +282,15 @@
 
    For the other groups delete items in the order determined by the configured
    ``indexers/priorities`` indexer order then by the configured operations for that
    item's indexer.
 
 
 ****************************************************************************************
-CONTRIBUTING
+Contributing
 ****************************************************************************************
 
 NOTE: `This project is hosted on GitLab`_.  There's `a mirror on GitHub`_ but please use
 GitLab for reporting issues, submitting PRs/MRs and any other development or maintenance
 activity.
 
 See `the ./CONTRIBUTING.rst file`_ for more details on how to get started with
@@ -232,18 +303,22 @@
 
 I didn't like the available options I could find at the time for maximizing seeding from
 a lovingly managed media library.  Deleting by a ratio threshold doesn't make sense to
 me because that can delete items when there's plenty of disk space.  Also the ratio
 threshold is a reverse indicator for items from private indexers vs items from public
 indexers.  Items from private indexers with high ratios should be kept around as long as
 possible to build user total ratio whereas items from public indexers with low ratios
-should be kept around as long as possibility to preserve access in the
-community/ecosystem.  Finally, deleting any item still imported in the Servarr just
-because it hit the ratio threshold is the biggest waste since it doesn't free any space.
-So I wrote Prunerr to prune download items in the correct order.
+should be kept around as long as possible to preserve access in the community/ecosystem.
+Finally, deleting any item still imported in the Servarr just because it hit the ratio
+threshold is the biggest waste since it doesn't free any space.  So I wrote Prunerr to
+prune download items in the correct order.
+
+The use case for Prunerr is not tracker ratio racing.  It's goal it to seed as long as
+possible and to seed as much of your library as possible.  This should have some
+secondary benefits to ratio, but that's not the main goal.
 
 Finally, there is a laundry list of other download client management tasks that can be
 automated but aren't by anything I could find.  So I added them to Prunerr as well.
 
 
 .. _`Transmission BitTorrent client`: https://transmissionbt.com/
 
@@ -253,14 +328,15 @@
 .. _`download clients`: https://wiki.servarr.com/radarr/settings#download-clients
 .. _`FlexGet`: https://flexget.com/
 
 .. _pip: https://pip.pypa.io/en/stable/installation/
 .. _argcomplete: https://kislyuk.github.io/argcomplete/#installation
 
 .. _the Docker image: https://hub.docker.com/r/merpatterson/prunerr
+.. _`Docker Compose`: https://docs.docker.com/compose/
 .. _`the example ./docker-compose.yml file`: https://gitlab.com/rpatterson/prunerr/blob/main/docker-compose.yml
 
 .. _`the example configuration`:
    https://gitlab.com/rpatterson/prunerr/blob/main/src/prunerr/home/.config/prunerr.yml
 
 .. _`This project is hosted on GitLab`:
    https://gitlab.com/rpatterson/prunerr
```

### Comparing `prunerr-1.1.1b0/bin/cz-check-bump` & `prunerr-1.1.2b1/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/bin/entrypoint` & `prunerr-1.1.2b1/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/bin/get-base-version` & `prunerr-1.1.2b1/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/build-host/Dockerfile` & `prunerr-1.1.2b1/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/build-host/Makefile` & `prunerr-1.1.2b1/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/build-host/README.rst` & `prunerr-1.1.2b1/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/build-host/bin/entrypoint` & `prunerr-1.1.2b1/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/build-host/requirements-py310.txt` & `prunerr-1.1.2b1/build-host/requirements-py38.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=build-host/requirements-py310.txt --resolver=backtracking build-host/requirements.txt.in
+#    pip-compile --output-file=build-host/requirements-py38.txt --resolver=backtracking build-host/requirements.txt.in
 #
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.11.0
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
@@ -30,9 +30,9 @@
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
 tox==4.4.12
     # via -r build-host/requirements.txt.in
-virtualenv==20.21.0
+virtualenv==20.21.1
     # via tox
```

### Comparing `prunerr-1.1.1b0/build-host/requirements-py311.txt` & `prunerr-1.1.2b1/build-host/requirements-py37.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,50 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
-#    pip-compile --output-file=build-host/requirements-py311.txt --resolver=backtracking build-host/requirements.txt.in
+#    pip-compile --output-file=build-host/requirements-py37.txt --resolver=backtracking build-host/requirements.txt.in
 #
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.11.0
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
+importlib-metadata==6.5.0
+    # via
+    #   pluggy
+    #   tox
+    #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
 platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
+tomli==2.0.1
+    # via
+    #   pyproject-api
+    #   tox
 tox==4.4.12
     # via -r build-host/requirements.txt.in
-virtualenv==20.21.0
+typing-extensions==4.5.0
+    # via
+    #   importlib-metadata
+    #   platformdirs
+    #   tox
+virtualenv==20.21.1
     # via tox
+zipp==3.15.0
+    # via importlib-metadata
```

### Comparing `prunerr-1.1.1b0/build-host/requirements-py37.txt` & `prunerr-1.1.2b1/build-host/requirements-py311.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,34 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=build-host/requirements-py37.txt --resolver=backtracking build-host/requirements.txt.in
+#    pip-compile --output-file=build-host/requirements-py311.txt --resolver=backtracking build-host/requirements.txt.in
 #
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.11.0
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
-importlib-metadata==6.4.1
-    # via
-    #   pluggy
-    #   tox
-    #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
 platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
-tomli==2.0.1
-    # via
-    #   pyproject-api
-    #   tox
 tox==4.4.12
     # via -r build-host/requirements.txt.in
-typing-extensions==4.5.0
-    # via
-    #   importlib-metadata
-    #   platformdirs
-    #   tox
-virtualenv==20.21.0
+virtualenv==20.21.1
     # via tox
-zipp==3.15.0
-    # via importlib-metadata
```

### Comparing `prunerr-1.1.1b0/build-host/requirements-py39.txt` & `prunerr-1.1.2b1/build-host/requirements-py39.txt`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.11.0
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
@@ -30,9 +30,9 @@
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
 tox==4.4.12
     # via -r build-host/requirements.txt.in
-virtualenv==20.21.0
+virtualenv==20.21.1
     # via tox
```

### Comparing `prunerr-1.1.1b0/docker-compose-servarr.yml` & `prunerr-1.1.2b1/docker-compose-servarr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/docker-compose.override.yml` & `prunerr-1.1.2b1/docker-compose.override.yml`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,17 @@
   sonarr:
     container_name: "prunerr-devel-sonarr"
   radarr:
     container_name: "prunerr-devel-radarr"
 
   # Configuration specific to development:
   prunerr-daemon:
-    image: "merpatterson/prunerr:${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
+    image: "\
+      registry.gitlab.com/rpatterson/prunerr\
+      :${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
     container_name: "prunerr-daemon-checkout"
     build:
       context: "${CHECKOUT_DIR}/"
       args:
         PYTHON_MINOR: "${PYTHON_MINOR:-3.10}"
         PYTHON_ENV: "${PYTHON_ENV:-py310}"
         VERSION: "${VERSION:-}"
@@ -30,15 +32,17 @@
       # Preserve caches caches between container runs
       - "${CHECKOUT_DIR}/home/:/home/prunerr/"
 
   ## Contianers used for development and release:
 
   # Container for use by developers:
   prunerr-devel:
-    image: "merpatterson/prunerr:devel-${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
+    image: "\
+      registry.gitlab.com/rpatterson/prunerr\
+      :devel-${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
     container_name: "prunerr-devel"
     profiles:
       - "test"
     build:
       context: "${CHECKOUT_DIR}/"
       dockerfile: "${CHECKOUT_DIR}/Dockerfile.devel"
       args:
@@ -117,15 +121,15 @@
       - "./:/usr/local/src/prunerr/"
     working_dir: "/usr/local/src/prunerr/"
 
   ## Containers related to CI/CD:
 
   # The container in which CI/CD is run:
   build-host:
-    image: "merpatterson/prunerr:build-host"
+    image: "registry.gitlab.com/rpatterson/prunerr:build-host"
     profiles:
       - "ci"
     build: "${CHECKOUT_DIR}/build-host/"
     privileged: true
     volumes:
       - "/var/run/docker.sock:/var/run/docker.sock"
       - "${CHECKOUT_DIR}/:${CHECKOUT_DIR}"
```

### Comparing `prunerr-1.1.1b0/docker-compose.yml` & `prunerr-1.1.2b1/docker-compose.yml`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
       traefik.http.routers.transmission.entrypoints: "websecure"
       traefik.http.routers.transmission.tls.certresolver: "letsencrypt"
 
   # See `./docker-compose-servarr.yml` for example Servarr configurations
 
   ## Container for use by end users:
   prunerr-daemon:
-    image: "merpatterson/prunerr"
+    image: "registry.gitlab.com/rpatterson/prunerr"
     container_name: "prunerr-daemon"
     depends_on:
       - "transmission"
     environment:
       TZ: "${TZ:-Etc/UTC}"
       # Make the run-time user configurable in `./.env` to match permissions inside and
       # outside the container.  Default to the common/standard main/first user and group
```

### Comparing `prunerr-1.1.1b0/gitlab-runner/config/config.toml.in` & `prunerr-1.1.2b1/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/pyproject.toml` & `prunerr-1.1.2b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [tool.commitizen]
 # Parse commit messages according to conventional commits to decide wether the next
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 changelog_start_rev = "v0.0.0"
-version = "1.1.1b0"
+version = "1.1.2b1"
 tag_format = "v$version"
 annotated_tag = true
 gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
```

### Comparing `prunerr-1.1.1b0/requirements/build.txt.in` & `prunerr-1.1.2b1/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/requirements/py310/build.txt` & `prunerr-1.1.2b1/requirements/py39/build.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py310/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py39/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==2.0.6
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
@@ -26,21 +26,21 @@
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.4.1
+importlib-metadata==6.5.0
     # via
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
@@ -68,15 +68,15 @@
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
@@ -106,15 +106,15 @@
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
     # via commitizen
 urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.21.0
+virtualenv==20.21.1
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `prunerr-1.1.1b0/requirements/py310/devel.txt` & `prunerr-1.1.2b1/requirements/py311/devel.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=requirements/py310/devel.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py311/devel.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.5
     # via prunerr (pyproject.toml)
 arrapi==1.4.2
     # via prunerr (pyproject.toml)
-astroid==2.15.2
+astroid==2.15.3
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 autoflake==1.7.8
     # via prunerr (pyproject.toml)
@@ -52,16 +52,14 @@
     # via pylint
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
-exceptiongroup==1.1.1
-    # via pytest
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
 future==0.18.3
@@ -139,15 +137,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
@@ -221,43 +219,30 @@
 tenacity==8.2.2
     # via prunerr (pyproject.toml)
 toml==0.10.2
     # via
     #   prospector
     #   requirements-detector
     #   vulture
-tomli==2.0.1
-    # via
-    #   autoflake
-    #   autopep8
-    #   black
-    #   build
-    #   mypy
-    #   pylint
-    #   pyproject-hooks
-    #   pytest
-    #   setuptools-scm
-    #   towncrier
 tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
-trove-classifiers==2023.3.9
+trove-classifiers==2023.4.18
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
 types-docutils==0.19.1.7
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via prunerr (pyproject.toml)
 typing-extensions==4.5.0
     # via
-    #   astroid
     #   mypy
     #   pydantic
     #   setuptools-scm
     #   transmission-rpc
 urllib3==1.26.15
     # via requests
 vulture==2.7
```

### Comparing `prunerr-1.1.1b0/requirements/py310/user.txt` & `prunerr-1.1.2b1/requirements/py310/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/requirements/py311/build.txt` & `prunerr-1.1.2b1/requirements/py311/build.txt`

 * *Files 0% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.4.1
+importlib-metadata==6.5.0
     # via
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
@@ -68,15 +68,15 @@
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
@@ -106,15 +106,15 @@
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
     # via commitizen
 urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.21.0
+virtualenv==20.21.1
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `prunerr-1.1.1b0/requirements/py311/devel.txt` & `prunerr-1.1.2b1/requirements/py39/devel.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=requirements/py311/devel.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py39/devel.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.5
     # via prunerr (pyproject.toml)
 arrapi==1.4.2
     # via prunerr (pyproject.toml)
-astroid==2.15.2
+astroid==2.15.3
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 autoflake==1.7.8
     # via prunerr (pyproject.toml)
@@ -27,18 +27,25 @@
     #   pip-tools
     #   prunerr (pyproject.toml)
     #   pyroma
 certifi==2022.12.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
+cli-exit-tools==1.2.3.2
+    # via
+    #   lib-detect-testenv
+    #   pathlib3x
 click==8.1.3
     # via
     #   black
+    #   cli-exit-tools
     #   click-default-group
+    #   lib-detect-testenv
+    #   pathlib3x
     #   pip-tools
     #   towncrier
     #   typer
 click-default-group==1.2.2
     # via towncrier
 colorama==0.4.6
     # via
@@ -52,14 +59,16 @@
     # via pylint
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
+exceptiongroup==1.1.1
+    # via pytest
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
 future==0.18.3
@@ -78,14 +87,16 @@
     # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
     # via towncrier
 lazy-object-proxy==1.9.0
     # via astroid
+lib-detect-testenv==2.0.3
+    # via cli-exit-tools
 main-wrapper==0.1.1
     # via service-logging
 mando==0.6.4
     # via radon
 markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
@@ -104,14 +115,16 @@
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
     #   setuptools-scm
+pathlib3x==2.0.2.1 ; python_version < "3.10"
+    # via prunerr (pyproject.toml)
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
@@ -137,15 +150,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
@@ -219,32 +232,47 @@
 tenacity==8.2.2
     # via prunerr (pyproject.toml)
 toml==0.10.2
     # via
     #   prospector
     #   requirements-detector
     #   vulture
+tomli==2.0.1
+    # via
+    #   autoflake
+    #   autopep8
+    #   black
+    #   build
+    #   mypy
+    #   pylint
+    #   pyproject-hooks
+    #   pytest
+    #   setuptools-scm
+    #   towncrier
 tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
-trove-classifiers==2023.3.9
+trove-classifiers==2023.4.18
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
 types-docutils==0.19.1.7
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via prunerr (pyproject.toml)
 typing-extensions==4.5.0
     # via
+    #   astroid
+    #   black
     #   mypy
     #   pydantic
+    #   pylint
     #   setuptools-scm
     #   transmission-rpc
 urllib3==1.26.15
     # via requests
 vulture==2.7
     # via prospector
 wheel==0.40.0
```

### Comparing `prunerr-1.1.1b0/requirements/py311/user.txt` & `prunerr-1.1.2b1/requirements/py311/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/requirements/py37/build.txt` & `prunerr-1.1.2b1/requirements/py37/build.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
 importlib-metadata==5.2.0
     # via
@@ -73,15 +73,15 @@
     # via virtualenv
 pre-commit==2.21.0
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
@@ -116,15 +116,15 @@
     #   markdown-it-py
     #   platformdirs
     #   rich
 urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.21.0
+virtualenv==20.21.1
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
     # via
```

### Comparing `prunerr-1.1.1b0/requirements/py37/devel.txt` & `prunerr-1.1.2b1/requirements/py37/devel.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --extra=devel --output-file=requirements/py37/devel.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.5
     # via prunerr (pyproject.toml)
 arrapi==1.4.2
     # via prunerr (pyproject.toml)
-astroid==2.15.2
+astroid==2.15.3
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 autoflake==1.7.8
     # via prunerr (pyproject.toml)
@@ -164,15 +164,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
@@ -264,15 +264,15 @@
     #   towncrier
 tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
-trove-classifiers==2023.3.9
+trove-classifiers==2023.4.18
     # via pyroma
 typed-ast==1.5.4
     # via
     #   astroid
     #   black
     #   mypy
 typer[all]==0.7.0
```

### Comparing `prunerr-1.1.1b0/requirements/py37/user.txt` & `prunerr-1.1.2b1/requirements/py37/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/requirements/py38/build.txt` & `prunerr-1.1.2b1/requirements/py38/build.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.4.1
+importlib-metadata==6.5.0
     # via
     #   keyring
     #   twine
 importlib-resources==5.12.0
     # via keyring
 jaraco-classes==3.2.3
     # via keyring
@@ -70,15 +70,15 @@
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
@@ -110,15 +110,15 @@
     # via
     #   commitizen
     #   rich
 urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.21.0
+virtualenv==20.21.1
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
     # via
```

### Comparing `prunerr-1.1.1b0/requirements/py38/devel.txt` & `prunerr-1.1.2b1/requirements/py38/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --extra=devel --output-file=requirements/py38/devel.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.5
     # via prunerr (pyproject.toml)
 arrapi==1.4.2
     # via prunerr (pyproject.toml)
-astroid==2.15.2
+astroid==2.15.3
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 autoflake==1.7.8
     # via prunerr (pyproject.toml)
@@ -150,15 +150,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
@@ -250,15 +250,15 @@
     #   towncrier
 tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
-trove-classifiers==2023.3.9
+trove-classifiers==2023.4.18
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
 types-docutils==0.19.1.7
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via prunerr (pyproject.toml)
```

### Comparing `prunerr-1.1.1b0/requirements/py38/user.txt` & `prunerr-1.1.2b1/requirements/py38/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/requirements/py39/build.txt` & `prunerr-1.1.2b1/requirements/py310/build.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py39/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py310/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==2.0.6
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
@@ -26,21 +26,21 @@
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.4.1
+importlib-metadata==6.5.0
     # via
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
@@ -68,15 +68,15 @@
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
@@ -106,15 +106,15 @@
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
     # via commitizen
 urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.21.0
+virtualenv==20.21.1
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `prunerr-1.1.1b0/requirements/py39/devel.txt` & `prunerr-1.1.2b1/requirements/py310/devel.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=requirements/py39/devel.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py310/devel.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.5
     # via prunerr (pyproject.toml)
 arrapi==1.4.2
     # via prunerr (pyproject.toml)
-astroid==2.15.2
+astroid==2.15.3
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 autoflake==1.7.8
     # via prunerr (pyproject.toml)
@@ -27,25 +27,18 @@
     #   pip-tools
     #   prunerr (pyproject.toml)
     #   pyroma
 certifi==2022.12.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-cli-exit-tools==1.2.3.2
-    # via
-    #   lib-detect-testenv
-    #   pathlib3x
 click==8.1.3
     # via
     #   black
-    #   cli-exit-tools
     #   click-default-group
-    #   lib-detect-testenv
-    #   pathlib3x
     #   pip-tools
     #   towncrier
     #   typer
 click-default-group==1.2.2
     # via towncrier
 colorama==0.4.6
     # via
@@ -87,16 +80,14 @@
     # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
     # via towncrier
 lazy-object-proxy==1.9.0
     # via astroid
-lib-detect-testenv==2.0.3
-    # via cli-exit-tools
 main-wrapper==0.1.1
     # via service-logging
 mando==0.6.4
     # via radon
 markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
@@ -115,16 +106,14 @@
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
     #   setuptools-scm
-pathlib3x==2.0.2.1 ; python_version < "3.10"
-    # via prunerr (pyproject.toml)
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
@@ -150,15 +139,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
@@ -250,29 +239,27 @@
     #   towncrier
 tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
-trove-classifiers==2023.3.9
+trove-classifiers==2023.4.18
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
 types-docutils==0.19.1.7
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via prunerr (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   astroid
-    #   black
     #   mypy
     #   pydantic
-    #   pylint
     #   setuptools-scm
     #   transmission-rpc
 urllib3==1.26.15
     # via requests
 vulture==2.7
     # via prospector
 wheel==0.40.0
```

### Comparing `prunerr-1.1.1b0/requirements/py39/user.txt` & `prunerr-1.1.2b1/requirements/py39/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/setup.cfg` & `prunerr-1.1.2b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/__init__.py` & `prunerr-1.1.2b1/src/prunerr/__init__.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/downloadclient.py` & `prunerr-1.1.2b1/src/prunerr/downloadclient.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/downloaditem.py` & `prunerr-1.1.2b1/src/prunerr/downloaditem.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/home/.config/prunerr.yml` & `prunerr-1.1.2b1/src/prunerr/home/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/operations.py` & `prunerr-1.1.2b1/src/prunerr/operations.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/runner.py` & `prunerr-1.1.2b1/src/prunerr/runner.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/servarr.py` & `prunerr-1.1.2b1/src/prunerr/servarr.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/Makefile` & `prunerr-1.1.2b1/src/prunerr/tests/Makefile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/__init__.py` & `prunerr-1.1.2b1/src/prunerr/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/example-5s.mkv` & `prunerr-1.1.2b1/src/prunerr/tests/example-5s.mkv`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/home/daemon/.config/prunerr.yml` & `prunerr-1.1.2b1/src/prunerr/tests/home/daemon/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/home/download-clients/.config/prunerr.yml` & `prunerr-1.1.2b1/src/prunerr/tests/home/download-clients/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml` & `prunerr-1.1.2b1/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json` & `prunerr-1.1.2b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/test_cli.py` & `prunerr-1.1.2b1/src/prunerr/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/test_daemon.py` & `prunerr-1.1.2b1/src/prunerr/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/test_downloadclient.py` & `prunerr-1.1.2b1/src/prunerr/tests/test_downloadclient.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/test_downloaditem.py` & `prunerr-1.1.2b1/src/prunerr/tests/test_downloaditem.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/test_free_space.py` & `prunerr-1.1.2b1/src/prunerr/tests/test_free_space.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/test_move.py` & `prunerr-1.1.2b1/src/prunerr/tests/test_move.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/test_operations.py` & `prunerr-1.1.2b1/src/prunerr/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/test_review.py` & `prunerr-1.1.2b1/src/prunerr/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/test_runner.py` & `prunerr-1.1.2b1/src/prunerr/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/test_servarr.py` & `prunerr-1.1.2b1/src/prunerr/tests/test_servarr.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/tests/test_verify.py` & `prunerr-1.1.2b1/src/prunerr/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr/utils.py` & `prunerr-1.1.2b1/src/prunerr/utils.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.1b0/src/prunerr.egg-info/PKG-INFO` & `prunerr-1.1.2b1/src/prunerr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prunerr
-Version: 1.1.1b0
+Version: 1.1.2b1
 Summary: Perma-seed Servarr media libraries
 Home-page: https://gitlab.com/rpatterson/prunerr
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: servarr,sonarr,radarr,transmission,bittorent,torrent
 Classifier: Development Status :: 4 - Beta
@@ -82,23 +82,39 @@
        .. figure:: https://img.shields.io/docker/stars/merpatterson/prunerr?logo=docker
 	  :alt: Docker Hub stars
           :target: https://hub.docker.com/r/merpatterson/prunerr
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/prunerr?logo=docker
 	  :alt: Docker Hub image size (latest semver)
           :target: https://hub.docker.com/r/merpatterson/prunerr
 
+     - .. figure:: https://img.shields.io/keybase/pgp/rpatterson?logo=keybase
+          :alt: KeyBase PGP key ID
+          :target: https://keybase.io/rpatterson
+       .. figure:: https://img.shields.io/github/followers/rpatterson?style=social
+          :alt: GitHub followers count
+          :target: https://github.com/rpatterson
+       .. figure:: https://img.shields.io/liberapay/receives/rpatterson.svg?logo=liberapay
+          :alt: LiberaPay donated per week
+          :target: https://liberapay.com/rpatterson/donate
+       .. figure:: https://img.shields.io/liberapay/patrons/rpatterson.svg?logo=liberapay
+          :alt: LiberaPay patrons count
+          :target: https://liberapay.com/rpatterson/donate
+
+
 TL;DR: Perma-seeding of whole Servarr libraries optimized for per-tracker ratio.
 
 - Delete torrents/items only as disk space gets low.
 - Don't delete currently imported items.  IOW, only delete upgraded items.
 - Don't delete private items that haven't met seeding requirements.
 - Delete public items first
 - Delete private items in an order to maximize tracker ratio and/or bonuses.
 - And more...
 
+.. contents:: Table of Contents
+
 *******
 Summary
 *******
 
 Seed Servarr download client torrents/items as long as possible only deleting them as
 necessary as disk space gets low, hence the name based on "to prune".  Which download
 items are considered eligible for deletion is configured by the user.  The common case
@@ -132,22 +148,50 @@
 See the `Usage`_ section below for full details.
 
 
 ****************************************************************************************
 Installation
 ****************************************************************************************
 
+Install and use either via a local, native installation or a Docker container image:
+
+Local/Native Installation
+========================================================================================
+
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
-  $ sudo pip3 install prunerr
+  $ pip3 install --user prunerr
 
 Optional shell tab completion is available via `argcomplete`_.
 
-Or use `the Docker image`_.  See `the example ./docker-compose.yml file`_ for usage
-details.
+Docker Container Image Installation
+========================================================================================
+
+The recommended way to use the Docker container image is via `Docker Compose`_.  See
+`the example ./docker-compose.yml file`_ for an example configuration.  Once you have
+your configuration, you can create and run the container::
+
+  $ docker compose up
+
+Alternatively, you make use the image directly.  Pull `the Docker image`_::
+
+  $ docker pull "docker.io/merpatterson/prunerr"
+
+And then use the image to create and run a container::
+
+  $ docker run --rm -it "docker.io/merpatterson/prunerr" ...
+
+The Docker images support the following platforms or architectures:
+
+- ``linux/amd64``
+- ``linux/arm64``
+- ``linux/arm/v7``
+
+Images are tagged with the branch name so images tagged with ``main`` are final releases
+and images tagged with ``develop`` are pre-releases.
 
 
 ****************************************************************************************
 Usage
 ****************************************************************************************
 
 Start by writing your ``~/.config/prunerr.yml`` configuration file.  See the comments in
@@ -158,18 +202,18 @@
 loop using the ``$ prunerr daemon`` sub-command.  See the `Order of Operations`_ section
 for a detailed description of the operations.  Use the CLI help to list the other
 sub-commands and to get help on the individual sub-commands::
 
   $ prunerr --help
   $ prunerr exec --help
 
-Set the ``DEBUG`` environment variable to ``true`` to get verbose details and help
-understand what Prunerr is doing::
+If using the Docker container image, the container can be run from the command-line as
+well::
 
-  $ DEBUG=true prunerr exec
+  $ docker compose run "prunerr" prunerr --help
 
 
 *******************
 Order of Operations
 *******************
 
 Note that polling is required because there is no event we can subscribe to that
@@ -238,15 +282,15 @@
 
    For the other groups delete items in the order determined by the configured
    ``indexers/priorities`` indexer order then by the configured operations for that
    item's indexer.
 
 
 ****************************************************************************************
-CONTRIBUTING
+Contributing
 ****************************************************************************************
 
 NOTE: `This project is hosted on GitLab`_.  There's `a mirror on GitHub`_ but please use
 GitLab for reporting issues, submitting PRs/MRs and any other development or maintenance
 activity.
 
 See `the ./CONTRIBUTING.rst file`_ for more details on how to get started with
@@ -259,18 +303,22 @@
 
 I didn't like the available options I could find at the time for maximizing seeding from
 a lovingly managed media library.  Deleting by a ratio threshold doesn't make sense to
 me because that can delete items when there's plenty of disk space.  Also the ratio
 threshold is a reverse indicator for items from private indexers vs items from public
 indexers.  Items from private indexers with high ratios should be kept around as long as
 possible to build user total ratio whereas items from public indexers with low ratios
-should be kept around as long as possibility to preserve access in the
-community/ecosystem.  Finally, deleting any item still imported in the Servarr just
-because it hit the ratio threshold is the biggest waste since it doesn't free any space.
-So I wrote Prunerr to prune download items in the correct order.
+should be kept around as long as possible to preserve access in the community/ecosystem.
+Finally, deleting any item still imported in the Servarr just because it hit the ratio
+threshold is the biggest waste since it doesn't free any space.  So I wrote Prunerr to
+prune download items in the correct order.
+
+The use case for Prunerr is not tracker ratio racing.  It's goal it to seed as long as
+possible and to seed as much of your library as possible.  This should have some
+secondary benefits to ratio, but that's not the main goal.
 
 Finally, there is a laundry list of other download client management tasks that can be
 automated but aren't by anything I could find.  So I added them to Prunerr as well.
 
 
 .. _`Transmission BitTorrent client`: https://transmissionbt.com/
 
@@ -280,14 +328,15 @@
 .. _`download clients`: https://wiki.servarr.com/radarr/settings#download-clients
 .. _`FlexGet`: https://flexget.com/
 
 .. _pip: https://pip.pypa.io/en/stable/installation/
 .. _argcomplete: https://kislyuk.github.io/argcomplete/#installation
 
 .. _the Docker image: https://hub.docker.com/r/merpatterson/prunerr
+.. _`Docker Compose`: https://docs.docker.com/compose/
 .. _`the example ./docker-compose.yml file`: https://gitlab.com/rpatterson/prunerr/blob/main/docker-compose.yml
 
 .. _`the example configuration`:
    https://gitlab.com/rpatterson/prunerr/blob/main/src/prunerr/home/.config/prunerr.yml
 
 .. _`This project is hosted on GitLab`:
    https://gitlab.com/rpatterson/prunerr
```

### Comparing `prunerr-1.1.1b0/src/prunerr.egg-info/SOURCES.txt` & `prunerr-1.1.2b1/src/prunerr.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -541,8 +541,9 @@
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
-src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
+src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
+src/pythonprojectstructure/newsfragments/+upgrade-requirements.bugfix.rst
```

### Comparing `prunerr-1.1.1b0/tox.ini` & `prunerr-1.1.2b1/tox.ini`

 * *Files identical despite different names*

