# Comparing `tmp/invenio-users-resources-1.2.0.tar.gz` & `tmp/invenio-users-resources-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-users-resources-1.2.0.tar", last modified: Fri Mar 24 16:28:34 2023, max compression
+gzip compressed data, was "dist/invenio-users-resources-1.3.0.tar", last modified: Thu Apr 20 15:41:19 2023, max compression
```

## Comparing `invenio-users-resources-1.2.0.tar` & `invenio-users-resources-1.3.0.tar`

### file list

```diff
@@ -1,254 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/entity_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/dumpers/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/dumpers/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v1/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v1/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v2/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v2/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/v7/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/v7/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/resources/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/resources/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/resources/groups/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/resources/groups/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/resources/users/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/resources/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/resources/users/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/resources/users/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/groups/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/groups/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/groups/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/groups/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/users/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/users/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/users/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/users/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/services/users/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/templates/avatar.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/invenio_users_resources/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/invenio_users_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/tests/resources/test_resources_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/tests/resources/test_resources_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:28:34.000000 invenio-users-resources-1.2.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/tests/services/test_service_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/tests/services/test_service_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-24 16:28:29.000000 invenio-users-resources-1.2.0/tests/test_invenio_users_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/entity_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/dumpers/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v1/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v1/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v2/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v2/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/v7/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/v7/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/resources/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/resources/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/resources/groups/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/resources/groups/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/resources/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/resources/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/resources/users/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/resources/users/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/groups/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/groups/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/groups/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/groups/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/users/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/users/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/users/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/services/users/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/templates/avatar.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/invenio_users_resources/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/invenio_users_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/tests/resources/test_resources_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/tests/resources/test_resources_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:41:19.000000 invenio-users-resources-1.3.0/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/tests/services/test_service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/tests/services/test_service_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-20 15:41:09.000000 invenio-users-resources-1.3.0/tests/test_invenio_users_resources.py
```

### Comparing `invenio-users-resources-1.2.0/.editorconfig` & `invenio-users-resources-1.3.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/.github/workflows/i18n-pull.yml` & `invenio-users-resources-1.3.0/.github/workflows/i18n-pull.yml`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/.github/workflows/i18n-push.yml` & `invenio-users-resources-1.3.0/.github/workflows/i18n-push.yml`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/.github/workflows/pypi-publish.yml` & `invenio-users-resources-1.3.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/.github/workflows/tests.yml` & `invenio-users-resources-1.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/.tx/config` & `invenio-users-resources-1.3.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/CHANGES.rst` & `invenio-users-resources-1.3.0/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,19 @@
     Invenio-Users-Resources is free software; you can redistribute it
     and/or modify it under the terms of the MIT License; see LICENSE file for
     more details.
 
 Changes
 =======
 
+Version 1.3.0 (2023-04-20)
+
+- upgrade invenio-records-resources
+- fix query parser method call with allowlist
+
 Version 1.2.0 (2023-03-24)
 
 - bump invenio-records-resources to v2.0.0
 - expand: add ghost user representation
 
 Version 1.1.0 (released 2023-03-02)
```

### Comparing `invenio-users-resources-1.2.0/CONTRIBUTING.rst` & `invenio-users-resources-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/LICENSE` & `invenio-users-resources-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/MANIFEST.in` & `invenio-users-resources-1.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/PKG-INFO` & `invenio-users-resources-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-users-resources
-Version: 1.2.0
+Version: 1.3.0
 Summary: Invenio module providing management APIs for users and roles/groups.
 Home-page: https://github.com/inveniosoftware/invenio-users-resources
 Author: CERN/TU Wien/JRC
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -42,14 +42,19 @@
             Invenio-Users-Resources is free software; you can redistribute it
             and/or modify it under the terms of the MIT License; see LICENSE file for
             more details.
         
         Changes
         =======
         
+        Version 1.3.0 (2023-04-20)
+        
+        - upgrade invenio-records-resources
+        - fix query parser method call with allowlist
+        
         Version 1.2.0 (2023-03-24)
         
         - bump invenio-records-resources to v2.0.0
         - expand: add ghost user representation
         
         Version 1.1.0 (released 2023-03-02)
```

### Comparing `invenio-users-resources-1.2.0/README.rst` & `invenio-users-resources-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/docs/Makefile` & `invenio-users-resources-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/docs/conf.py` & `invenio-users-resources-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/docs/index.rst` & `invenio-users-resources-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/docs/make.bat` & `invenio-users-resources-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/config.py` & `invenio-users-resources-1.3.0/invenio_users_resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/entity_resolvers.py` & `invenio-users-resources-1.3.0/invenio_users_resources/entity_resolvers.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/ext.py` & `invenio-users-resources-1.3.0/invenio_users_resources/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/proxies.py` & `invenio-users-resources-1.3.0/invenio_users_resources/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/records/api.py` & `invenio-users-resources-1.3.0/invenio_users_resources/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/records/dumpers/email.py` & `invenio-users-resources-1.3.0/invenio_users_resources/records/dumpers/email.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/records/hooks.py` & `invenio-users-resources-1.3.0/invenio_users_resources/records/hooks.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json` & `invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json` & `invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json` & `invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json` & `invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json` & `invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json` & `invenio-users-resources-1.3.0/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/records/models.py` & `invenio-users-resources-1.3.0/invenio_users_resources/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/resources/groups/config.py` & `invenio-users-resources-1.3.0/invenio_users_resources/resources/groups/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/resources/groups/resource.py` & `invenio-users-resources-1.3.0/invenio_users_resources/resources/groups/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/resources/users/config.py` & `invenio-users-resources-1.3.0/invenio_users_resources/resources/users/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/resources/users/resource.py` & `invenio-users-resources-1.3.0/invenio_users_resources/resources/users/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/services/common.py` & `invenio-users-resources-1.3.0/invenio_users_resources/services/common.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/services/generators.py` & `invenio-users-resources-1.3.0/invenio_users_resources/services/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/services/groups/config.py` & `invenio-users-resources-1.3.0/invenio_users_resources/services/groups/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/services/groups/results.py` & `invenio-users-resources-1.3.0/invenio_users_resources/services/groups/results.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/services/groups/service.py` & `invenio-users-resources-1.3.0/invenio_users_resources/services/groups/service.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/services/groups/tasks.py` & `invenio-users-resources-1.3.0/invenio_users_resources/services/groups/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/services/params.py` & `invenio-users-resources-1.3.0/invenio_users_resources/services/params.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/services/permissions.py` & `invenio-users-resources-1.3.0/invenio_users_resources/services/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/services/results.py` & `invenio-users-resources-1.3.0/invenio_users_resources/services/results.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/services/schemas.py` & `invenio-users-resources-1.3.0/invenio_users_resources/services/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/services/users/config.py` & `invenio-users-resources-1.3.0/invenio_users_resources/services/users/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,26 +33,24 @@
 
     pagination_options = {
         "default_results_per_page": 10,
         "default_max_results": 10,
     }
 
     query_parser_cls = QueryParser.factory(
+        tree_transformer_cls=SearchFieldTransformer,
         fields=["username^2", "email^2", "profile.full_name^3", "profile.affiliations"],
-        tree_transformer_factory=SearchFieldTransformer.factory(
-            mapping={
-                "affiliation": "profile.affiliations",
-                "affiliations": "profile.affiliations",
-                "email": "email",
-                "full_name": "profile.full_name",
-                "fullname": "profile.full_name",
-                "name": "profile.full_name",
-                "username": "username",
-            }
-        ),
+        allow_list=["username", "email"],  # mapped fields are added on the query parser
+        mapping={
+            "affiliation": "profile.affiliations",
+            "affiliations": "profile.affiliations",
+            "full_name": "profile.full_name",
+            "fullname": "profile.full_name",
+            "name": "profile.full_name",
+        },
     )
 
     params_interpreters_cls = [
         QueryStrParam,
         SortParam,
         FixedPagination,
     ]
```

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/services/users/results.py` & `invenio-users-resources-1.3.0/invenio_users_resources/services/users/results.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/services/users/service.py` & `invenio-users-resources-1.3.0/invenio_users_resources/services/users/service.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/services/users/tasks.py` & `invenio-users-resources-1.3.0/invenio_users_resources/services/users/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/messages.pot` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-users-resources-1.3.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources/views.py` & `invenio-users-resources-1.3.0/invenio_users_resources/views.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources.egg-info/PKG-INFO` & `invenio-users-resources-1.3.0/invenio_users_resources.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-users-resources
-Version: 1.2.0
+Version: 1.3.0
 Summary: Invenio module providing management APIs for users and roles/groups.
 Home-page: https://github.com/inveniosoftware/invenio-users-resources
 Author: CERN/TU Wien/JRC
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -42,14 +42,19 @@
             Invenio-Users-Resources is free software; you can redistribute it
             and/or modify it under the terms of the MIT License; see LICENSE file for
             more details.
         
         Changes
         =======
         
+        Version 1.3.0 (2023-04-20)
+        
+        - upgrade invenio-records-resources
+        - fix query parser method call with allowlist
+        
         Version 1.2.0 (2023-03-24)
         
         - bump invenio-records-resources to v2.0.0
         - expand: add ghost user representation
         
         Version 1.1.0 (released 2023-03-02)
```

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources.egg-info/SOURCES.txt` & `invenio-users-resources-1.3.0/invenio_users_resources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/invenio_users_resources.egg-info/entry_points.txt` & `invenio-users-resources-1.3.0/invenio_users_resources.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/run-tests.sh` & `invenio-users-resources-1.3.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/setup.cfg` & `invenio-users-resources-1.3.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 install_requires = 
 	invenio-oauthclient>=2.2.0,<3.0.0
-	invenio-records-resources>=2.0.0,<3.0.0
+	invenio-records-resources>=3.0.0,<4.0.0
 
 [options.extras_require]
 tests = 
 	pytest-black>=0.3.0
 	invenio-app>=1.3.3,<2.0.0
 	invenio-db[postgresql,mysql]>=1.0.14,<2.0.0
 	pytest-invenio>=2.1.0,<3.0.0
```

### Comparing `invenio-users-resources-1.2.0/tests/conftest.py` & `invenio-users-resources-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/tests/resources/test_resources_groups.py` & `invenio-users-resources-1.3.0/tests/resources/test_resources_groups.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/tests/resources/test_resources_users.py` & `invenio-users-resources-1.3.0/tests/resources/test_resources_users.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/tests/services/test_service_groups.py` & `invenio-users-resources-1.3.0/tests/services/test_service_groups.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/tests/services/test_service_users.py` & `invenio-users-resources-1.3.0/tests/services/test_service_users.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-1.2.0/tests/test_invenio_users_resources.py` & `invenio-users-resources-1.3.0/tests/test_invenio_users_resources.py`

 * *Files identical despite different names*

