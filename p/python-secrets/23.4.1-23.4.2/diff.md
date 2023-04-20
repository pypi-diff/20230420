# Comparing `tmp/python_secrets-23.4.1.tar.gz` & `tmp/python_secrets-23.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_secrets-23.4.1.tar", last modified: Wed Apr 19 21:52:37 2023, max compression
+gzip compressed data, was "python_secrets-23.4.2.tar", last modified: Thu Apr 20 19:06:30 2023, max compression
```

## Comparing `python_secrets-23.4.1.tar` & `python_secrets-23.4.2.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.380944 python_secrets-23.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.360944 python_secrets-23.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.364944 python_secrets-23.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     4224 2023-04-19 21:46:29.000000 python_secrets-23.4.1/.github/workflows/test-build-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-04-19 21:46:29.000000 python_secrets-23.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-19 21:46:29.000000 python_secrets-23.4.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-04-19 21:46:29.000000 python_secrets-23.4.1/.travis.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.364944 python_secrets-23.4.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (122)    31952 2023-04-19 21:46:29.000000 python_secrets-23.4.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (122)      528 2023-04-19 21:46:29.000000 python_secrets-23.4.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4108 2023-04-19 21:46:29.000000 python_secrets-23.4.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)    13073 2023-04-19 21:46:29.000000 python_secrets-23.4.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (122)      611 2023-04-19 21:46:29.000000 python_secrets-23.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-04-19 21:46:29.000000 python_secrets-23.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7052 2023-04-19 21:46:29.000000 python_secrets-23.4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)    78965 2023-04-19 21:52:37.380944 python_secrets-23.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    65524 2023-04-19 21:46:29.000000 python_secrets-23.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-19 21:46:29.000000 python_secrets-23.4.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-19 21:46:29.000000 python_secrets-23.4.1/bandit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.368944 python_secrets-23.4.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (122)      502 2023-04-19 21:46:29.000000 python_secrets-23.4.1/bin/psec
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.368944 python_secrets-23.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     6794 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.368944 python_secrets-23.4.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1997 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/advanced.rst
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (122)     8728 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (122)      647 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6475 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9602 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.368944 python_secrets-23.4.1/psec/
--rwxr-xr-x   0 runner    (1001) docker     (122)      718 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12422 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/about.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.368944 python_secrets-23.4.1/psec/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.372944 python_secrets-23.4.1/psec/cli/environments/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5301 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     5363 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/default.py
--rw-r--r--   0 runner    (1001) docker     (122)     5112 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     3760 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     4533 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/path.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/rename.py
--rw-r--r--   0 runner    (1001) docker     (122)     3412 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.372944 python_secrets-23.4.1/psec/cli/groups/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/groups/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     3518 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/groups/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/groups/list.py
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/groups/path.py
--rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/groups/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     2579 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.372944 python_secrets-23.4.1/psec/cli/secrets/
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2075 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/backup.py
--rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     5067 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     4081 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/describe.py
--rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/find.py
--rw-r--r--   0 runner    (1001) docker     (122)     3889 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/generate.py
--rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/get.py
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/path.py
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/restore.py
--rw-r--r--   0 runner    (1001) docker     (122)     5292 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/send.py
--rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/set.py
--rw-r--r--   0 runner    (1001) docker     (122)     5473 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    48131 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     2635 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/template.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.372944 python_secrets-23.4.1/psec/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6301 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/utils/myip.py
--rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/utils/netblock.py
--rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/utils/set_aws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (122)     2172 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/utils/tfbackend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4391 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/utils/tfoutput.py
--rw-r--r--   0 runner    (1001) docker     (122)     7459 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/utils/yaml_to_json.py
--rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    17834 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/google_oauth2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.376944 python_secrets-23.4.1/psec/secrets_environment/
--rw-r--r--   0 runner    (1001) docker     (122)    30739 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.376944 python_secrets-23.4.1/psec/secrets_environment/factory/
--rw-r--r--   0 runner    (1001) docker     (122)     2401 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/factory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.376944 python_secrets-23.4.1/psec/secrets_environment/handlers/
--rw-r--r--   0 runner    (1001) docker     (122)      392 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/boolean.py
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/crypt_6.py
--rw-r--r--   0 runner    (1001) docker     (122)     4945 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/password.py
--rw-r--r--   0 runner    (1001) docker     (122)      846 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/sha256_digest.py
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/string.py
--rw-r--r--   0 runner    (1001) docker     (122)      730 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/token_base64.py
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/token_hex.py
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/token_urlsafe.py
--rw-r--r--   0 runner    (1001) docker     (122)      458 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/uuid4.py
--rw-r--r--   0 runner    (1001) docker     (122)    32045 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.376944 python_secrets-23.4.1/python_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    78965 2023-04-19 21:52:37.000000 python_secrets-23.4.1/python_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3350 2023-04-19 21:52:37.000000 python_secrets-23.4.1/python_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 21:52:37.000000 python_secrets-23.4.1/python_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2166 2023-04-19 21:52:37.000000 python_secrets-23.4.1/python_secrets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 21:52:37.000000 python_secrets-23.4.1/python_secrets.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 21:48:55.000000 python_secrets-23.4.1/python_secrets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-19 21:52:37.000000 python_secrets-23.4.1/python_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-04-19 21:52:37.000000 python_secrets-23.4.1/python_secrets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-19 21:46:29.000000 python_secrets-23.4.1/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-19 21:46:29.000000 python_secrets-23.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-19 21:46:29.000000 python_secrets-23.4.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.376944 python_secrets-23.4.1/secrets.d/
--rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-04-19 21:46:29.000000 python_secrets-23.4.1/secrets.d/hypriot.json
--rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-04-19 21:52:37.380944 python_secrets-23.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2148 2023-04-19 21:46:29.000000 python_secrets-23.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)      375 2023-04-19 21:46:29.000000 python_secrets-23.4.1/test-environment.bash
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.380944 python_secrets-23.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/00_usage.bats
--rwxr-xr-x   0 runner    (1001) docker     (122)       24 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/gosecure.json
--rw-r--r--   0 runner    (1001) docker     (122)     1047 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/runtime_00_initialization.bats
--rw-r--r--   0 runner    (1001) docker     (122)     9024 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/runtime_05_environments.bats
--rw-r--r--   0 runner    (1001) docker     (122)     3371 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/runtime_10_groups.bats
--rw-r--r--   0 runner    (1001) docker     (122)     6909 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/runtime_20_secrets.bats
--rw-r--r--   0 runner    (1001) docker     (122)     3145 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/runtime_30_utils.bats
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/runtime_40_run.bats
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.380944 python_secrets-23.4.1/tests/secrets.d/
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/secrets.d/consul.json
--rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/secrets.d/hypriot.json
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/secrets.d/jenkins.json
--rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/secrets.d/myapp.json
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/secrets.d/oauth.json
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/secrets.d/trident.json
--rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1285 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (122)     1167 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/test_helper.bash
--rw-r--r--   0 runner    (1001) docker     (122)     9069 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/test_secrets.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1076 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.364944 python_secrets-23.4.1/tests/yamlsecrets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.380944 python_secrets-23.4.1/tests/yamlsecrets/secrets.d/
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/yamlsecrets/secrets.d/jenkins.yml
--rw-r--r--   0 runner    (1001) docker     (122)      637 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/yamlsecrets/secrets.d/myapp.yml
--rw-r--r--   0 runner    (1001) docker     (122)      384 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/yamlsecrets/secrets.d/oauth.yml
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/yamlsecrets/secrets.d/trident.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.646124 python_secrets-23.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.626124 python_secrets-23.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.630124 python_secrets-23.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     4224 2023-04-20 19:00:23.000000 python_secrets-23.4.2/.github/workflows/test-build-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-04-20 19:00:23.000000 python_secrets-23.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-20 19:00:23.000000 python_secrets-23.4.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-04-20 19:00:23.000000 python_secrets-23.4.2/.travis.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.634124 python_secrets-23.4.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (122)    31952 2023-04-20 19:00:23.000000 python_secrets-23.4.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-04-20 19:00:23.000000 python_secrets-23.4.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4108 2023-04-20 19:00:23.000000 python_secrets-23.4.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    13300 2023-04-20 19:00:23.000000 python_secrets-23.4.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-04-20 19:00:23.000000 python_secrets-23.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-04-20 19:00:23.000000 python_secrets-23.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7052 2023-04-20 19:00:23.000000 python_secrets-23.4.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)    79192 2023-04-20 19:06:30.646124 python_secrets-23.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    65524 2023-04-20 19:00:23.000000 python_secrets-23.4.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-20 19:00:23.000000 python_secrets-23.4.2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-20 19:00:23.000000 python_secrets-23.4.2/bandit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.634124 python_secrets-23.4.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      502 2023-04-20 19:00:23.000000 python_secrets-23.4.2/bin/psec
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.634124 python_secrets-23.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     6794 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.634124 python_secrets-23.4.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1997 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8728 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      647 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6475 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9602 2023-04-20 19:00:23.000000 python_secrets-23.4.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.634124 python_secrets-23.4.2/psec/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      718 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12466 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/about.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.634124 python_secrets-23.4.2/psec/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.638124 python_secrets-23.4.2/psec/cli/environments/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5301 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/environments/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5363 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/environments/default.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5112 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/environments/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3760 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/environments/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4533 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/environments/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/environments/rename.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3412 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/environments/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.638124 python_secrets-23.4.2/psec/cli/groups/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/groups/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3518 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/groups/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/groups/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/groups/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/groups/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2579 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.638124 python_secrets-23.4.2/psec/cli/secrets/
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2075 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/secrets/backup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/secrets/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5067 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/secrets/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4081 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/secrets/describe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/secrets/find.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3889 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/secrets/generate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/secrets/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/secrets/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/secrets/restore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5292 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/secrets/send.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/secrets/set.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5473 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/secrets/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/secrets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47945 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2635 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/template.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.638124 python_secrets-23.4.2/psec/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6301 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/utils/myip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/utils/netblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/utils/set_aws_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/utils/tfbackend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4365 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/utils/tfoutput.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7459 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/cli/utils/yaml_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17814 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/google_oauth2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.638124 python_secrets-23.4.2/psec/secrets_environment/
+-rw-r--r--   0 runner    (1001) docker     (122)    30713 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/secrets_environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.638124 python_secrets-23.4.2/psec/secrets_environment/factory/
+-rw-r--r--   0 runner    (1001) docker     (122)     2401 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/secrets_environment/factory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.642124 python_secrets-23.4.2/psec/secrets_environment/handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/secrets_environment/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/secrets_environment/handlers/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/secrets_environment/handlers/crypt_6.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4945 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/secrets_environment/handlers/password.py
+-rw-r--r--   0 runner    (1001) docker     (122)      846 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/secrets_environment/handlers/sha256_digest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/secrets_environment/handlers/string.py
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/secrets_environment/handlers/token_base64.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/secrets_environment/handlers/token_hex.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/secrets_environment/handlers/token_urlsafe.py
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/secrets_environment/handlers/uuid4.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31979 2023-04-20 19:00:23.000000 python_secrets-23.4.2/psec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.642124 python_secrets-23.4.2/python_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    79192 2023-04-20 19:06:30.000000 python_secrets-23.4.2/python_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3350 2023-04-20 19:06:30.000000 python_secrets-23.4.2/python_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 19:06:30.000000 python_secrets-23.4.2/python_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2166 2023-04-20 19:06:30.000000 python_secrets-23.4.2/python_secrets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 19:06:30.000000 python_secrets-23.4.2/python_secrets.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 19:02:57.000000 python_secrets-23.4.2/python_secrets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-20 19:06:30.000000 python_secrets-23.4.2/python_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-04-20 19:06:30.000000 python_secrets-23.4.2/python_secrets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-20 19:00:23.000000 python_secrets-23.4.2/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-20 19:00:23.000000 python_secrets-23.4.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-20 19:00:23.000000 python_secrets-23.4.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.642124 python_secrets-23.4.2/secrets.d/
+-rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-04-20 19:00:23.000000 python_secrets-23.4.2/secrets.d/hypriot.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-04-20 19:06:30.646124 python_secrets-23.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2148 2023-04-20 19:00:23.000000 python_secrets-23.4.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-04-20 19:00:23.000000 python_secrets-23.4.2/test-environment.bash
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.642124 python_secrets-23.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/00_usage.bats
+-rwxr-xr-x   0 runner    (1001) docker     (122)       24 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/gosecure.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1047 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/runtime_00_initialization.bats
+-rw-r--r--   0 runner    (1001) docker     (122)     9016 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/runtime_05_environments.bats
+-rw-r--r--   0 runner    (1001) docker     (122)     3371 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/runtime_10_groups.bats
+-rw-r--r--   0 runner    (1001) docker     (122)     7141 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/runtime_20_secrets.bats
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/runtime_30_utils.bats
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/runtime_40_run.bats
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.646124 python_secrets-23.4.2/tests/secrets.d/
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/secrets.d/consul.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/secrets.d/hypriot.json
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/secrets.d/jenkins.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/secrets.d/myapp.json
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/secrets.d/oauth.json
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/secrets.d/trident.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1285 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1167 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/test_helper.bash
+-rw-r--r--   0 runner    (1001) docker     (122)     9069 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/test_secrets.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1076 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.630124 python_secrets-23.4.2/tests/yamlsecrets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:06:30.646124 python_secrets-23.4.2/tests/yamlsecrets/secrets.d/
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/yamlsecrets/secrets.d/jenkins.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      637 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/yamlsecrets/secrets.d/myapp.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      384 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/yamlsecrets/secrets.d/oauth.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tests/yamlsecrets/secrets.d/trident.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-04-20 19:00:23.000000 python_secrets-23.4.2/tox.ini
```

### Comparing `python_secrets-23.4.1/.github/workflows/test-build-publish.yml` & `python_secrets-23.4.2/.github/workflows/test-build-publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     - name: Dump select GitHub event context
       run: |
         echo "github.ref=${{ github.ref }}"
         echo "github.event.head_commit=$HEAD_COMMIT"
       env:
         HEAD_COMMIT: ${{ toJson(github.event.head_commit) }}
     - name: Check out src from GitHub
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
         python-version: 3.9.16
     - uses: conda-incubator/setup-miniconda@v2
@@ -113,22 +113,22 @@
         startsWith(github.ref, 'refs/tags') &&
         contains(github.ref, 'rc') == true
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         repository_url: https://test.pypi.org/legacy/
         user: __token__
         password: ${{ secrets.PSEC_TEST_PYPI_PASSWORD }}
-        packages_dir: ${{ steps.get_vars.outputs.ARTIFACT }}
-        verify_metadata: false
+        packages-dir: ${{ steps.get_vars.outputs.ARTIFACT }}
+        verify-metadata: false
     - name: Publish tagged artifacts to PyPI
       if: >-
         github.event_name == 'push' &&
         startsWith(github.ref, 'refs/tags') &&
         contains(github.ref, 'rc') == false
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PSEC_PYPI_PASSWORD }}
-        packages_dir: ${{ steps.get_vars.outputs.ARTIFACT }}
-        verify_metadata: false
+        packages-dir: ${{ steps.get_vars.outputs.ARTIFACT }}
+        verify-metadata: false
     # ![2-test-build-publish]
```

### Comparing `python_secrets-23.4.1/.gitignore` & `python_secrets-23.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/.travis.yml` & `python_secrets-23.4.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/.vscode/launch.json` & `python_secrets-23.4.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/AUTHORS.rst` & `python_secrets-23.4.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/CONTRIBUTING.rst` & `python_secrets-23.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/HISTORY.rst` & `python_secrets-23.4.2/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,29 @@
 .. Added for new features.
 .. Changed for changes in existing functionality.
 .. Deprecated for soon-to-be removed features.
 .. Removed for now removed features.
 .. Fixed for any bug fixes.
 .. Security in case of vulnerabilities.
 
+23.4.2 (2023-04-20)
+~~~~~~~~~~~~~~~~~~~
+
+Added
+^^^^^
+
+- Added bats test for `secrets find` command.
+
+Changed
+^^^^^^^
+
+- Switched to using f-strings for formatting.
+- Fixed broken bats tests.
+- Update GitHub Actions workflows.
+
 23.4.1 (2023-04-19)
 ~~~~~~~~~~~~~~~~~~~
 
 Added
 ^^^^^
 
 - Added `secrets find` command.
```

### Comparing `python_secrets-23.4.1/LICENSE.txt` & `python_secrets-23.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/Makefile` & `python_secrets-23.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/PKG-INFO` & `python_secrets-23.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_secrets
-Version: 23.4.1
+Version: 23.4.2
 Home-page: https://github.com/davedittrich/python_secrets
 Download-URL: https://github.com/davedittrich/python_secrets/tarball/master
 Author: Dave Dittrich
 Author-email: dave.dittrich@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -25,15 +25,15 @@
         :alt: Documentation Status
 
 
 Python command line app for managing groups of secrets (passwords, API keys, etc) and
 other project variables. Reduces security risks from things like weak default passwords,
 secrets stored in files in the source code repository directory.
 
-Version: 23.4.1
+Version: 23.4.2
 
 * Free software: `Apache 2.0 License <https://www.apache.org/licenses/LICENSE-2.0>`_
 * Documentation: https://python_secrets.readthedocs.org.
 
 Features
 --------
 
@@ -1226,15 +1226,15 @@
     To: dittrich@u.washington.edu
 
     The following secret is being shared with you:
 
     myapp_app_password=brunt.outclass.alike.turbine
 
     --
-    Sent using psec version 23.4.1
+    Sent using psec version 23.4.2
     https://pypi.org/project/python-secrets/
     https://github.com/davedittrich/python_secrets
 
 ..
 
 A group of secrets required for Google's `OAuth 2.0 Mechanism`_  is provided
 and must be set according to Google's instructions. See also:
@@ -1712,14 +1712,29 @@
 .. Added for new features.
 .. Changed for changes in existing functionality.
 .. Deprecated for soon-to-be removed features.
 .. Removed for now removed features.
 .. Fixed for any bug fixes.
 .. Security in case of vulnerabilities.
 
+23.4.2 (2023-04-20)
+~~~~~~~~~~~~~~~~~~~
+
+Added
+^^^^^
+
+- Added bats test for `secrets find` command.
+
+Changed
+^^^^^^^
+
+- Switched to using f-strings for formatting.
+- Fixed broken bats tests.
+- Update GitHub Actions workflows.
+
 23.4.1 (2023-04-19)
 ~~~~~~~~~~~~~~~~~~~
 
 Added
 ^^^^^
 
 - Added `secrets find` command.
```

### Comparing `python_secrets-23.4.1/README.rst` & `python_secrets-23.4.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         :alt: Documentation Status
 
 
 Python command line app for managing groups of secrets (passwords, API keys, etc) and
 other project variables. Reduces security risks from things like weak default passwords,
 secrets stored in files in the source code repository directory.
 
-Version: 23.4.1
+Version: 23.4.2
 
 * Free software: `Apache 2.0 License <https://www.apache.org/licenses/LICENSE-2.0>`_
 * Documentation: https://python_secrets.readthedocs.org.
 
 Features
 --------
 
@@ -1214,15 +1214,15 @@
     To: dittrich@u.washington.edu
 
     The following secret is being shared with you:
 
     myapp_app_password=brunt.outclass.alike.turbine
 
     --
-    Sent using psec version 23.4.1
+    Sent using psec version 23.4.2
     https://pypi.org/project/python-secrets/
     https://github.com/davedittrich/python_secrets
 
 ..
 
 A group of secrets required for Google's `OAuth 2.0 Mechanism`_  is provided
 and must be set according to Google's instructions. See also:
```

### Comparing `python_secrets-23.4.1/docs/Makefile` & `python_secrets-23.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/docs/advanced.rst` & `python_secrets-23.4.2/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/docs/conf.py` & `python_secrets-23.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/docs/index.rst` & `python_secrets-23.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/docs/installation.rst` & `python_secrets-23.4.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/docs/make.bat` & `python_secrets-23.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/docs/reference.rst` & `python_secrets-23.4.2/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/docs/usage.rst` & `python_secrets-23.4.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/__init__.py` & `python_secrets-23.4.2/psec/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 __version__ = None
-__release__ = '23.4.1'
+__release__ = '23.4.2'
 
 # Get development version from repository tags.
 try:
     from setuptools_scm import get_version
     __version__ = get_version(root='..', relative_to=__file__)
 except (ImportError, LookupError):
     pass
```

### Comparing `python_secrets-23.4.1/psec/__main__.py` & `python_secrets-23.4.2/psec/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,18 +68,19 @@
         self.secrets_file = None
         self.timer = Timer()
         # Alias the following variable for consistency using code
         # using "logger" instead of "LOG".
         self.logger = self.LOG
         self.secret_factory = SecretFactory()
 
-    def build_option_parser(self, description, version):
+    def build_option_parser(self, description, version, argparse_kwargs=None):
         parser = super().build_option_parser(
             description,
-            version
+            version,
+            argparse_kwargs,
         )
         # OCD hack: Make ``help`` output report main program name,
         # even if run as ``python -m psec.main`` or such.
         if parser.prog.endswith('.py'):
             parser.prog = self.command_manager.namespace
         # Replace the cliff SmartHelpFormatter class before first use
         # by subcommand `--help`.
@@ -292,15 +293,15 @@
             or (
                 self.options.verbose_level > 1
                 and cmd.cmd_name != "complete"
             )
         ):
             self.timer.stop()
             elapsed = self.timer.elapsed()
-            self.stderr.write('[+] elapsed time {}\n'.format(elapsed))
+            self.stderr.write(f'[+] elapsed time {elapsed}\n')
             bell()
 
 
 def main(argv=sys.argv[1:]):
     """
     Command line interface for the ``psec`` program.
     """
```

### Comparing `python_secrets-23.4.1/psec/about.py` & `python_secrets-23.4.2/psec/about.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/environments/create.py` & `python_secrets-23.4.2/psec/cli/environments/create.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/environments/default.py` & `python_secrets-23.4.2/psec/cli/environments/default.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/environments/delete.py` & `python_secrets-23.4.2/psec/cli/environments/delete.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/environments/list.py` & `python_secrets-23.4.2/psec/cli/environments/list.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/environments/path.py` & `python_secrets-23.4.2/psec/cli/environments/path.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/environments/rename.py` & `python_secrets-23.4.2/psec/cli/environments/rename.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/environments/tree.py` & `python_secrets-23.4.2/psec/cli/environments/tree.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/groups/create.py` & `python_secrets-23.4.2/psec/cli/groups/create.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/groups/delete.py` & `python_secrets-23.4.2/psec/cli/groups/delete.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/groups/list.py` & `python_secrets-23.4.2/psec/cli/groups/list.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/groups/path.py` & `python_secrets-23.4.2/psec/cli/groups/path.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/groups/show.py` & `python_secrets-23.4.2/psec/cli/groups/show.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/init.py` & `python_secrets-23.4.2/psec/cli/init.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/run.py` & `python_secrets-23.4.2/psec/cli/run.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/secrets/backup.py` & `python_secrets-23.4.2/psec/cli/secrets/backup.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/secrets/create.py` & `python_secrets-23.4.2/psec/cli/secrets/create.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/secrets/delete.py` & `python_secrets-23.4.2/psec/cli/secrets/delete.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/secrets/describe.py` & `python_secrets-23.4.2/psec/cli/secrets/describe.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/secrets/find.py` & `python_secrets-23.4.2/psec/cli/secrets/find.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/secrets/generate.py` & `python_secrets-23.4.2/psec/cli/secrets/generate.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/secrets/get.py` & `python_secrets-23.4.2/psec/cli/secrets/get.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/secrets/path.py` & `python_secrets-23.4.2/psec/cli/secrets/path.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/secrets/restore.py` & `python_secrets-23.4.2/psec/cli/secrets/restore.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/secrets/send.py` & `python_secrets-23.4.2/psec/cli/secrets/send.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/secrets/set.py` & `python_secrets-23.4.2/psec/cli/secrets/set.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/secrets/show.py` & `python_secrets-23.4.2/psec/cli/secrets/show.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/secrets/tree.py` & `python_secrets-23.4.2/psec/cli/secrets/tree.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/ssh.py` & `python_secrets-23.4.2/psec/cli/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import argparse
 import glob
 import json
 import logging
 import os
 import pexpect
 import re
+import shlex
 import socket
 import sys
 import tempfile
 import textwrap
 import time
 
 from cliff.command import Command
@@ -170,38 +171,38 @@
                 raise RuntimeError(
                     f"[-] '{dir}' exists and is not a directory")
     for host, v in hostdict.items():
         for fingerprint in v['fingerprint']:
             dir = os.path.join(known_hosts_root, 'fingerprints', host)
             os.makedirs(dir, exist_ok=True)
             ktype = _get_type(fingerprint)
-            fp_file = os.path.join(dir, '{}.fingerprint'.format(ktype))
+            fp_file = os.path.join(dir, f'{ktype}.fingerprint')
             with open(fp_file, 'w') as f:
-                f.write('{}\n'.format(fingerprint))
+                f.write(f'{fingerprint}\n')
                 logger.debug("[+] wrote fingerprint to '%s'", fp_file)
 
         for hostkey in v['hostkey']:
             dir = os.path.join(known_hosts_root, 'known_hosts', host)
             os.makedirs(dir, exist_ok=True)
             ktype = _get_type(hostkey)
-            hk_file = os.path.join(dir, '{}.known_hosts'.format(ktype))
+            hk_file = os.path.join(dir, f'{ktype}.known_hosts')
             with open(hk_file, 'w') as f:
-                f.write('{}\n'.format(hostkey))
+                f.write(f'{hostkey}\n')
                 logger.debug("[+] wrote hostkey to '%s'", hk_file)
     pass
 
 
 def _ansible_verbose(verbose_level=1):
     """
     Return an ansible verbose flag for a given Cliff app verbose
     level to pass along desired verbosity intent.
     """
     flag = ''
     if verbose_level > 1:
-        flag = '-{}'.format("v" * (verbose_level - 1))
+        flag = f'-{"v" * (verbose_level - 1)}'
     return flag
 
 
 def _ansible_set_hostkeys(hostkeys,  # nosec
                           debug=False,
                           ask_become_pass='--ask-become-pass',
                           verbose_level=1):
@@ -212,15 +213,15 @@
         playbook.flush()
         if verbose_level > 2:
             print(REKEY_PLAYBOOK, file=sys.stderr, flush=True)
         # TODO(dittrich): Look for local ansible.cfg file
         cmd = ['ansible-playbook',
                ask_become_pass,
                _ansible_verbose(verbose_level),
-               '-e', "'{}'".format(hostkeys),
+               '-e', f"'{hostkeys}'",
                playbook.name
                ]
         ansible = pexpect.spawnu(
             " ".join([arg for arg in cmd]))
         ansible.interact()
         if ansible.isalive():
             raise RuntimeError('[-] Ansible did not exit gracefully.')
@@ -240,15 +241,15 @@
         hosts = [i.split()[0]
                  for i in json.loads(hostkeys)['ssh_host_public_keys']]
         ssh_hosts = json.dumps({'ssh_hosts': list(set(hosts))})
         # TODO(dittrich): Look for local ansible.cfg file
         cmd = ['ansible-playbook',
                ask_become_pass,
                _ansible_verbose(verbose_level),
-               '-e', "'{}'".format(ssh_hosts),
+               '-e', f"'{ssh_hosts}'",
                '-e', 'remove_keys=true',
                playbook.name,
                ]
         ansible = pexpect.spawnu(
             " ".join([arg for arg in cmd]))
         ansible.interact()
         # Short delay because randomly this causes an exception
@@ -257,15 +258,15 @@
         if ansible.isalive():
             raise RuntimeError('[-] Ansible did not exit gracefully.')
 
 
 def _ansible_debug(hostkeys):
     """Debug Ansible"""
     cmd = ['ansible',
-           '-e', "'{}'".format(hostkeys),
+           '-e', f"'{hostkeys}'",
            '-m', 'debug',
            '-a', 'var=vars',
            'all'
            ]
     output, exitstatus = pexpect.runu(
         " ".join([arg for arg in cmd]),
         withexitstatus=1)
@@ -430,15 +431,15 @@
             r'digitalocean_droplet\.([a-zA-Z]+):{0,1} ')
         self.host_info = None
         if known_hosts_root is not None:
             self.host_info = _parse_known_hosts(root=known_hosts_root)
             for host, info in self.host_info.items():
                 for item in ['public_dns', 'public_ip']:
                     for key in info['full_hostkey']:
-                        pubkey = "{} {}".format(info[item], key)
+                        pubkey = f"{info[item]} {key}"
                         if host not in self.hostdict:
                             self.hostdict[host] = dict()
                         try:
                             self.hostdict[host]['hostkey'].extend([pubkey])
                         except KeyError:
                             self.hostdict[host]['hostkey'] = [pubkey]
 
@@ -606,16 +607,15 @@
             else:
                 line = line.strip()
             if line.find('(remote-exec):   Host: ') >= 0:
                 # DigitalOcean style from Terraform
                 _host = line.split(' Host: ')[1]
                 if _host != "":
                     public_ip = _host
-                    public_dns = '{}.{}'.format(short_name,
-                                                self.domain)
+                    public_dns = f'{short_name}.{self.domain}'
                     if short_name not in self.hostdict:
                         self.hostdict[short_name] = dict()
                     self.hostdict[short_name]['public_ip'] = public_ip  # noqa
                     self.hostdict[short_name]['public_dns'] = public_dns  # noqa
             elif line.find('[+] Host: ') >= 0:
                 # AWS style from Pulumi
                 _host = line.split(' Host: ')[1]
@@ -650,19 +650,19 @@
                     self.hostdict[short_name]['fingerprint'] = [fingerprint]
                 if self.debug:
                     self.logger.info('fingerprint: %s', fingerprint)
             elif in_pubkeys:
                 # TODO(dittrich): Should use regex instead.
                 fields = line.split(' ')
                 # 'digitalocean_droplet.red (remote-exec): ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIA69uuX+ItFoAAe+xE9c+XggGw7Z2Z7t3YVRJxSHMupv root@debian.example.com'  # noqa
-                hostid = "{},{}".format(public_dns, public_ip)
+                hostid = f"{public_dns},{public_ip}"
                 if fields[1] == '(remote-exec):':
-                    pubkey = "{} {} {}".format(hostid, fields[2], fields[3])
+                    pubkey = f"{hostid} {fields[2]} {fields[3]}"
                 else:
-                    pubkey = "{} {} {}".format(hostid, fields[0], fields[1])
+                    pubkey = f"{hostid} {fields[0]} {fields[1]}"
                 try:
                     self.hostdict[short_name]['hostkey'].extend([pubkey])
                 except KeyError:
                     self.hostdict[short_name]['hostkey'] = [pubkey]
                 if self.debug:
                     self.logger.info('pubkey: %s', pubkey)
 
@@ -682,17 +682,17 @@
             for k, v in self.hostdict.items():
                 keylist.extend(v['hostkey'])
         else:
             if self.public_ip is None or self.public_dns is None:
                 raise RuntimeError('[-] no host IP or name found or specified')
             for key in self.hostkey:
                 if self.public_ip is not None:
-                    keylist.append("{} {}".format(self.public_ip, key))
+                    keylist.append(f"{self.public_ip} {key}")
                 if self.public_dns is not None:
-                    keylist.append("{} {}".format(self.public_dns, key))
+                    keylist.append(f"{self.public_dns} {key}")
         return json.dumps({'ssh_host_public_keys': keylist})
 
     def get_hostkey_list(self):
         """Return the hostkey list"""
         return self.hostkey
 
 
@@ -774,43 +774,43 @@
         #     raise RuntimeError(
         #         '[-] must specify --public-ip and --public-dns')
         # TODO(dittrich): Need to pass key name explicitly...
         # _aws_privatekey_path = \
         #     se.get_secret('aws_privatekey_path')
         home = os.path.expanduser('~')
         ssh_config = os.path.join(home, '.ssh', 'config')
-        snippet_prefix = 'psec.{}'.format(se._environment)
+        snippet_prefix = f'psec.{se._environment}'
         if parsed_args.clean:
             files = glob.glob(os.path.join(ssh_config + '.d',
                                            snippet_prefix + ".*"))
             for f in files:
                 if self.app_args.verbose_level > 1:
                     self.logger.info("[+] deleting '%s'", f)
                 os.remove(f)
         host_info = _parse_known_hosts(root=parsed_args.known_hosts_root)
         private_key_file = self._get_private_key_file()
         if private_key_file is None:
             raise RuntimeError('[-] no SSH private key specified')
         for host, info in host_info.items():
-            snippet = 'psec.{}.{}'.format(se._environment, host)
+            snippet = f'psec.{se._environment}.{host}'
             if parsed_args.show_config:
                 # TODO(dittrich): finish this...
                 print()
             _write_ssh_configd(
                 ssh_config=ssh_config,
                 shortname=host,
                 name=snippet,
                 user=parsed_args.ssh_user,
                 identity_file=private_key_file,
                 public_ip=info['public_ip'],
                 public_dns=info['public_dns']
             )
 
         output, exitstatus = pexpect.runu(
-            'update-dotdee {}'.format(ssh_config),
+            f"update-dotdee {shlex.quote(ssh_config)}",
             withexitstatus=1)
         if exitstatus == 0:
             if self.app_args.verbose_level >= 1:
                 print(output, file=sys.stdout, flush=True)
         else:
             print(output, file=sys.stdout, flush=True)
             raise RuntimeError(
```

### Comparing `python_secrets-23.4.1/psec/cli/template.py` & `python_secrets-23.4.2/psec/cli/template.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/utils/myip.py` & `python_secrets-23.4.2/psec/cli/utils/myip.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/utils/netblock.py` & `python_secrets-23.4.2/psec/cli/utils/netblock.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/utils/set_aws_credentials.py` & `python_secrets-23.4.2/psec/cli/utils/set_aws_credentials.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/cli/utils/tfbackend.py` & `python_secrets-23.4.2/psec/cli/utils/tfbackend.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,21 +43,22 @@
         return parser
 
     def take_action(self, parsed_args):
         e = SecretsEnvironment(environment=self.app.options.environment)
         tmpdir = e.get_tmpdir_path()
         backend_file = os.path.join(os.getcwd(), 'tfbackend.tf')
         tfstate_file = os.path.join(tmpdir, 'terraform.tfstate')
-        backend_text = textwrap.dedent("""\
-            terraform {{
+        backend_text = textwrap.dedent(
+            f"""terraform {{
               backend "local" {{
               path = "{tfstate_file}"
               }}
             }}
-            """.format(tfstate_file=tfstate_file))
+            """
+        )
 
         if parsed_args.path:
             self.logger.debug('[+] showing terraform state file path')
             print(tfstate_file)
         else:
             self.logger.debug('[+] setting up terraform backend')
             if os.path.exists(backend_file):
```

### Comparing `python_secrets-23.4.1/psec/cli/utils/tfoutput.py` & `python_secrets-23.4.2/psec/cli/utils/tfoutput.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,31 +108,31 @@
         if not os.path.exists(tfstate):
             raise RuntimeError(f"[-] file does not exist: '{tfstate}'")
         if self.app_args.verbose_level > 1:
             # NOTE(dittrich): Not DRY, but spend time fixing later.
             self.logger.info(
                 ' '.join(['/usr/local/bin/terraform',
                           'output',
-                          '-state={}'.format(tfstate),
+                          f'-state={tfstate}',
                           '-json'])
             )
         p = subprocess.Popen(
             [
                 '/usr/local/bin/terraform',
                 'output',
-                '-state={}'.format(shlex.quote(tfstate)),
+                f'-state={shlex.quote(tfstate)}',
                 '-json'
             ],
             env=dict(os.environ),
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             shell=False  # nosec
         )
         jout, err = p.communicate()
         dout = json.loads(jout.decode('UTF-8'))
         for prefix in dout.keys():
             for k, v in dout[prefix]['value'].items():
-                data.append(["{}_{}".format(prefix, k), v])
+                data.append([f"{prefix}_{k}", v])
         return columns, data
 
 
 # vim: set fileencoding=utf-8 ts=4 sw=4 tw=0 et :
```

### Comparing `python_secrets-23.4.1/psec/cli/utils/yaml_to_json.py` & `python_secrets-23.4.2/psec/cli/utils/yaml_to_json.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/exceptions.py` & `python_secrets-23.4.2/psec/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/google_oauth2.py` & `python_secrets-23.4.2/psec/google_oauth2.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         """
         self.client_secret = client_secret
 
     def command_to_url(self, command):
         """
         Produce an URL for a given command.
         """
-        return '{}/{}'.format(self.GOOGLE_ACCOUNTS_BASE_URL, command)
+        return f'{self.GOOGLE_ACCOUNTS_BASE_URL}/{command}'
 
     def url_escape(self, text):
         """
         Escape characters in the URL to reduce risk.
         """
         return urllib.parse.quote(text, safe='~-._')
 
@@ -161,17 +161,17 @@
 
     def url_format_params(self, params):
         """
         Format a parameterized URL.
         """
         param_fragments = []
         for param in sorted(params.items(), key=lambda x: x[0]):
-            param_fragments.append('{}={}'.format(
-                param[0], self.url_escape(param[1])
-            ))
+            param_fragments.append(
+                f'{param[0]}={self.url_escape(param[1])}'
+            )
         return '&'.join(param_fragments)
 
     def generate_permission_url(
         self,
         scope='https://mail.google.com/',
     ):
         """
```

### Comparing `python_secrets-23.4.1/psec/secrets_environment/__init__.py` & `python_secrets-23.4.2/psec/secrets_environment/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,17 +263,17 @@
         """Returns the absolute path to secrets environment directory
         or subdirectories within it"""
         if env is None:
             env = self._environment
         _path = self.get_secrets_basedir() / str(env)
         if not (subdir is None and host is None):
             valid_subdir = r'a-zA-Z0-9_/'
-            invalid_subdir = re.compile('[^{}]'.format(valid_subdir))
+            invalid_subdir = re.compile(f'[^{valid_subdir}]')
             valid_host = r'a-zA-Z0-9_\./'  # noqa
-            invalid_host = re.compile('[^{}]'.format(valid_host))
+            invalid_host = re.compile(f'[^{valid_host}]')
             if subdir is None and host is not None:
                 raise RuntimeError(
                     '[-] Must specify subdir when specifying host')
             if subdir is not None:
                 if subdir.startswith('/'):
                     raise RuntimeError('[-] subdir may not start with "/"')
                 elif subdir.endswith('/'):
@@ -458,15 +458,15 @@
             os.environ[secret] = str(value)
             # See if an alternate environment variable name is
             # defined and also export as that.
             # TODO(dittrich): Support more than one, someday, maybe?
             _env_var = self.get_secret_export(secret)
             if _env_var is None:
                 if self.env_var_prefix is not None:
-                    _env_var = '{}{}'.format(self.env_var_prefix, secret)
+                    _env_var = f'{self.env_var_prefix}{secret}'
                 else:
                     _env_var = secret
             if self.preserve_existing and bool(os.getenv(_env_var)):
                 raise RuntimeError(
                     "[-] refusing to overwrite environment "
                     f"variable '{_env_var}'")
             os.environ[_env_var] = str(value)
```

### Comparing `python_secrets-23.4.1/psec/secrets_environment/factory/__init__.py` & `python_secrets-23.4.2/psec/secrets_environment/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/secrets_environment/handlers/crypt_6.py` & `python_secrets-23.4.2/psec/secrets_environment/handlers/crypt_6.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/secrets_environment/handlers/password.py` & `python_secrets-23.4.2/psec/secrets_environment/handlers/password.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/secrets_environment/handlers/sha256_digest.py` & `python_secrets-23.4.2/psec/secrets_environment/handlers/sha256_digest.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/secrets_environment/handlers/token_base64.py` & `python_secrets-23.4.2/psec/secrets_environment/handlers/token_base64.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/secrets_environment/handlers/token_hex.py` & `python_secrets-23.4.2/psec/secrets_environment/handlers/token_hex.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/secrets_environment/handlers/token_urlsafe.py` & `python_secrets-23.4.2/psec/secrets_environment/handlers/token_urlsafe.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/psec/utils.py` & `python_secrets-23.4.2/psec/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 def save_default_environment(
     environment=None,
     cwd=None
 ):
     """Save environment identifier to local file for defaulting."""
     env_file = get_local_default_file(cwd=cwd)
     with open(env_file, 'w') as f_out:
-        f_out.write('{0}\n'.format(str(environment)))
+        f_out.write(f'{str(environment)}\n')
     return True
 
 
 def clear_saved_default_environment(cwd=None):
     """Remove saved default environment file."""
     env_file = get_local_default_file(cwd=cwd)
     if os.path.exists(env_file):
@@ -601,17 +601,18 @@
     ``FAT32``. A log message will be produced when this is encountered.
     """
     # File permissions on Cygwin/Windows filesystems don't work the
     # same way as Linux. Don't try to change them.
     # TODO(dittrich): Is there a Better way to handle perms on Windows?
     fs_type = get_fs_type(dst)
     if fs_type in ['NTFS', 'FAT', 'FAT32']:
-        msg = ('[-] {0} has file system type "{1}": '
-               'skipping setting permissions').format(
-                   dst, fs_type)
+        msg = (
+            f"[-] {dst} has file system type '{fs_type}': "
+            'skipping setting permissions'
+        )
         logger.info(msg)
     else:
         get_output(['chmod', '-R', 'o-rwx', dst])
 
 
 def get_output(cmd=['echo', 'NO COMMAND SPECIFIED'],
                cwd=os.getcwd(),
@@ -696,15 +697,15 @@
     if default is None:
         default = cancel
     else:
         # Remove the default from the list because it will
         # be added back as the first item.
         options = [i for i in options if i != default]
     choices = [default] + options
-    cli = Bullet(prompt='\n{0}'.format(prompt),
+    cli = Bullet(prompt=f'\n{prompt}',
                  choices=choices,
                  indent=0,
                  align=2,
                  margin=1,
                  shift=0,
                  bullet="→",
                  pad_right=5)
@@ -735,15 +736,15 @@
         raise RuntimeError('[-] options is not a list of dictionaries')
     choices = ['<CANCEL>'] + [
                                 opt['descr']
                                 if by_descr
                                 else opt['ident']
                                 for opt in options
                              ]
-    cli = Bullet(prompt='\n{0}'.format(prompt),
+    cli = Bullet(prompt=f'\n{prompt}',
                  choices=choices,
                  indent=0,
                  align=2,
                  margin=1,
                  shift=0,
                  bullet="→",
                  pad_right=5)
@@ -917,30 +918,32 @@
         self.task_description = task_description
         self.laps = OrderedDict()
 
     def __enter__(self):
         """Record initial time."""
         self.start(lap="__enter__")
         if self.verbose:
-            sys.stdout.write('{}...'.format(self.task_description))
+            sys.stdout.write(f'{self.task_description}...')
             sys.stdout.flush()
         return self
 
     def __exit__(self, *args):
         """Record final time."""
         self.stop()
         backspace = '\b\b\b'
         if self.verbose:
             sys.stdout.flush()
             if self.elapsed_raw() < 1.0:
-                sys.stdout.write(backspace + ':' + '{:.2f}ms\n'.format(
-                    self.elapsed_raw() * 1000))
+                sys.stdout.write(
+                    f"{backspace}: {self.elapsed_raw() * 1000:.2f}ms\n"
+                )
             else:
-                sys.stdout.write(backspace + ': ' + '{}\n'.format(
-                    self.elapsed()))
+                sys.stdout.write(
+                    f"{backspace}: {self.elapsed()}\n"
+                )
             sys.stdout.flush()
 
     def start(self, lap=None):
         """Record starting time."""
         t = time.time()
         first = None if len(self.laps) == 0 \
             else self.laps.iteritems().next()[0]
@@ -975,16 +978,15 @@
     def elapsed(self, start="__enter__", end="__exit__"):
         """
         Return a formatted string with elapsed time between 'start'
         and 'end' kwargs (if specified) in HH:MM:SS.SS format.
         """
         hours, rem = divmod(self.elapsed_raw(start, end), 3600)
         minutes, seconds = divmod(rem, 60)
-        return "{:0>2}:{:0>2}:{:05.2f}".format(
-            int(hours), int(minutes), seconds)
+        return f"{int(hours):0>2}:{int(minutes):0>2}:{seconds:05.2f}"
 
 
 def myip_http(arg=None):
     """Use an HTTP service that only returns IP address."""
     # Return type if no argument for use in Lister.
     if arg is None:
         return 'https'
```

### Comparing `python_secrets-23.4.1/python_secrets.egg-info/PKG-INFO` & `python_secrets-23.4.2/python_secrets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-secrets
-Version: 23.4.1
+Version: 23.4.2
 Home-page: https://github.com/davedittrich/python_secrets
 Download-URL: https://github.com/davedittrich/python_secrets/tarball/master
 Author: Dave Dittrich
 Author-email: dave.dittrich@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -25,15 +25,15 @@
         :alt: Documentation Status
 
 
 Python command line app for managing groups of secrets (passwords, API keys, etc) and
 other project variables. Reduces security risks from things like weak default passwords,
 secrets stored in files in the source code repository directory.
 
-Version: 23.4.1
+Version: 23.4.2
 
 * Free software: `Apache 2.0 License <https://www.apache.org/licenses/LICENSE-2.0>`_
 * Documentation: https://python_secrets.readthedocs.org.
 
 Features
 --------
 
@@ -1226,15 +1226,15 @@
     To: dittrich@u.washington.edu
 
     The following secret is being shared with you:
 
     myapp_app_password=brunt.outclass.alike.turbine
 
     --
-    Sent using psec version 23.4.1
+    Sent using psec version 23.4.2
     https://pypi.org/project/python-secrets/
     https://github.com/davedittrich/python_secrets
 
 ..
 
 A group of secrets required for Google's `OAuth 2.0 Mechanism`_  is provided
 and must be set according to Google's instructions. See also:
@@ -1712,14 +1712,29 @@
 .. Added for new features.
 .. Changed for changes in existing functionality.
 .. Deprecated for soon-to-be removed features.
 .. Removed for now removed features.
 .. Fixed for any bug fixes.
 .. Security in case of vulnerabilities.
 
+23.4.2 (2023-04-20)
+~~~~~~~~~~~~~~~~~~~
+
+Added
+^^^^^
+
+- Added bats test for `secrets find` command.
+
+Changed
+^^^^^^^
+
+- Switched to using f-strings for formatting.
+- Fixed broken bats tests.
+- Update GitHub Actions workflows.
+
 23.4.1 (2023-04-19)
 ~~~~~~~~~~~~~~~~~~~
 
 Added
 ^^^^^
 
 - Added `secrets find` command.
```

### Comparing `python_secrets-23.4.1/python_secrets.egg-info/SOURCES.txt` & `python_secrets-23.4.2/python_secrets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/python_secrets.egg-info/entry_points.txt` & `python_secrets-23.4.2/python_secrets.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/secrets.d/hypriot.json` & `python_secrets-23.4.2/secrets.d/hypriot.json`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/setup.cfg` & `python_secrets-23.4.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 23.4.1
+current_version = 23.4.2
 commit = False
 tag = False
 
 [bumpversion:file:VERSION]
 
 [bumpversion:file:README.rst]
```

### Comparing `python_secrets-23.4.1/setup.py` & `python_secrets-23.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/tests/00_usage.bats` & `python_secrets-23.4.2/tests/00_usage.bats`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/tests/gosecure.json` & `python_secrets-23.4.2/tests/gosecure.json`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/tests/runtime_00_initialization.bats` & `python_secrets-23.4.2/tests/runtime_00_initialization.bats`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/tests/runtime_05_environments.bats` & `python_secrets-23.4.2/tests/runtime_05_environments.bats`

 * *Files 1% similar despite different names*

```diff
@@ -61,45 +61,45 @@
 ├── consul.json
 ├── hypriot.json
 ├── jenkins.json
 ├── myapp.json
 ├── oauth.json
 └── trident.json
 
-0 directories, 6 files"
+1 directory, 6 files"
 }
 
 @test "'psec environments create testenv --clone-from tests/secrets.d' works" {
     run $PSEC -vvv environments create testenv --clone-from tests/secrets.d 1>&2
     [ -d $D2_SECRETS_BASEDIR/testenv/secrets.d ]
     run bash -c "cd $D2_SECRETS_BASEDIR/testenv && tree secrets.d" </dev/null
     assert_output "secrets.d
 ├── consul.json
 ├── hypriot.json
 ├── jenkins.json
 ├── myapp.json
 ├── oauth.json
 └── trident.json
 
-0 directories, 6 files"
+1 directory, 6 files"
 }
 
 @test "'psec -e testenv environments create --clone-from tests/secrets.d' works" {
     run $PSEC -vvv -e testenv environments create --clone-from tests/secrets.d 1>&2
     [ -d $D2_SECRETS_BASEDIR/testenv/secrets.d ]
     run bash -c "cd $D2_SECRETS_BASEDIR/testenv && tree secrets.d" </dev/null
     assert_output "secrets.d
 ├── consul.json
 ├── hypriot.json
 ├── jenkins.json
 ├── myapp.json
 ├── oauth.json
 └── trident.json
 
-0 directories, 6 files"
+1 directory, 6 files"
 }
 
 @test "'psec environments create testenv2 --clone-from testenv' works" {
     run $PSEC -q environments create testenv --clone-from tests/secrets.d 1>&2
     run $PSEC -vvv environments create testenv2 --clone-from testenv 1>&2
     assert_success
     [ -d $D2_SECRETS_BASEDIR/testenv2/secrets.d ]
@@ -109,15 +109,15 @@
     run $PSEC environments delete ${D2_ENVIRONMENT} --force 1>&2
     run $PSEC -vvv environments create --clone-from tests/secrets.d/jenkins.json 1>&2
     [ -d $D2_SECRETS_BASEDIR/$D2_ENVIRONMENT/secrets.d ]
     run bash -c "cd $D2_SECRETS_BASEDIR/$D2_ENVIRONMENT && tree secrets.d" </dev/null
     assert_output "secrets.d
 └── jenkins.json
 
-0 directories, 1 file"
+1 directory, 1 file"
 }
 
 @test "'psec environments create --clone-from /tmp' fails" {
     run $PSEC environments delete ${D2_ENVIRONMENT} --force 1>&2
     run $PSEC -vvv environments create --clone-from /tmp 1>&2
     assert_failure
     assert_output --partial "does not exist"
```

### Comparing `python_secrets-23.4.1/tests/runtime_10_groups.bats` & `python_secrets-23.4.2/tests/runtime_10_groups.bats`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/tests/runtime_20_secrets.bats` & `python_secrets-23.4.2/tests/runtime_20_secrets.bats`

 * *Files 2% similar despite different names*

```diff
@@ -61,18 +61,18 @@
     refute_output 'None'
     run $PSEC secrets get myapp_client_psk
     assert_output ''
 }
 
 @test "'psec secrets generate --unique' works properly" {
     run $PSEC secrets generate
-    run bash -c "$PSEC secrets show --no-redact -t password -c Value -f value | sort | uniq | wc -l"
+    run bash -c "$PSEC secrets show --no-redact -t password -c Value -f value | sort | uniq | wc -l | sed 's/ *//g'"
     assert_output '1'
     run $PSEC secrets generate --unique
-    run bash -c "$PSEC secrets show --no-redact -t password -c Value -f value | sort | uniq | wc -l"
+    run bash -c "$PSEC secrets show --no-redact -t password -c Value -f value | sort | uniq | wc -l | sed 's/ *//g'"
     refute_output '1'
 }
 
 @test "'psec secrets generate --from-options' sets variables properly" {
     run $PSEC secrets generate --from-options
     run $PSEC secrets get hypriot_hostname
     assert_output "hypriot"
@@ -115,14 +115,19 @@
 
 @test "'psec secrets path' from directory works properly" {
     [ ! -f .python_secrets_environment ]
     run $PSEC secrets path
     assert_output "${D2_SECRETS_BASEDIR}/${D2_ENVIRONMENT}/secrets.json"
 }
 
+@test "'psec secrets find jenkins_admin_password' works" {
+    run $PSEC secrets find jenkins_admin_password -c Group -c Variable
+    assert_output --partial "| jenkins | jenkins_admin_password |"
+}
+
 @test "'psec secrets describe --group jenkins' works properly" {
     run $PSEC secrets describe --group jenkins
     assert_output "+------------------------+---------+----------+--------------------------------------+---------+------+
 | Variable               | Group   | Type     | Prompt                               | Options | Help |
 +------------------------+---------+----------+--------------------------------------+---------+------+
 | jenkins_admin_password | jenkins | password | Password for Jenkins 'admin' account | *       | *    |
 +------------------------+---------+----------+--------------------------------------+---------+------+"
```

### Comparing `python_secrets-23.4.1/tests/runtime_30_utils.bats` & `python_secrets-23.4.2/tests/runtime_30_utils.bats`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 load test_helper
 
 # Use: files_count /path/to/dir "*.type"
 files_count() {
-    find "$1" -depth 1 -type f -name "${2:-*}" 2>/dev/null | wc -l
+    find "$1" -depth 1 -type f -name "${2:-*}" 2>/dev/null | wc -l | sed 's/ *//g'
 }
 
 export TEST_FILES_COUNT="$(files_count tests/yamlsecrets/secrets.d '*.yml')"
 export KEEP_DIR="${BATS_TMPDIR}/bats_keep"
 export DONOTKEEP_DIR="${BATS_TMPDIR}/bats_donotkeep"
 
 # TODO(dittrich): Some odd bug in bats-core v1.2.1 causes failures
```

### Comparing `python_secrets-23.4.1/tests/runtime_40_run.bats` & `python_secrets-23.4.2/tests/runtime_40_run.bats`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/tests/secrets.d/hypriot.json` & `python_secrets-23.4.2/tests/secrets.d/hypriot.json`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/tests/secrets.d/myapp.json` & `python_secrets-23.4.2/tests/secrets.d/myapp.json`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/tests/test_exceptions.py` & `python_secrets-23.4.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/tests/test_groups.py` & `python_secrets-23.4.2/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/tests/test_helper.bash` & `python_secrets-23.4.2/tests/test_helper.bash`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/tests/test_secrets.py` & `python_secrets-23.4.2/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/tests/test_utils.py` & `python_secrets-23.4.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/tests/yamlsecrets/secrets.d/myapp.yml` & `python_secrets-23.4.2/tests/yamlsecrets/secrets.d/myapp.yml`

 * *Files identical despite different names*

### Comparing `python_secrets-23.4.1/tox.ini` & `python_secrets-23.4.2/tox.ini`

 * *Files identical despite different names*

