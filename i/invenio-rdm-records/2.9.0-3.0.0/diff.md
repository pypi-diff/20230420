# Comparing `tmp/invenio-rdm-records-2.9.0.tar.gz` & `tmp/invenio-rdm-records-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-rdm-records-2.9.0.tar", last modified: Fri Mar 24 17:42:06 2023, max compression
+gzip compressed data, was "dist/invenio-rdm-records-3.0.0.tar", last modified: Thu Apr 20 11:19:16 2023, max compression
```

## Comparing `invenio-rdm-records-2.9.0.tar` & `invenio-rdm-records-3.0.0.tar`

### file list

```diff
@@ -1,701 +1,768 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/.github/workflows/stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/.github/workflows/tests-feature.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/babel.ini
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/constraints-pypi.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/administration/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/administration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/administration/views/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/administration/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/administration/views/oai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/0cf260eb8e97_create_table_for_secret_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/4a15e8671f4d_create_rdm_records_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/88d1463de5c0_create_parent_record_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/8ed1a438601c_migrate_secret_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/9e0ac518b9df_create_records_communities_m2m_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/a3957490361d_remove_pidrelations_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/b822ba22c688_create_rdm_records_branch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/details/
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/details/CopyButton.js
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/details/LinksTable.js
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/details/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/search/
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/search/DeleteModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/search/SearchResultItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/i18next-scanner.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/de/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/de/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/el/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/el/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/en/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/en/translations.json
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    60991 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/scripts/compileCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/scripts/initCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/translations.pot
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/codemeta/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/codemeta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/codemeta/custom_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/imprint/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/imprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/imprint/custom_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/journal/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/journal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/journal/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/journal/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/meeting/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/meeting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/meeting/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/meeting/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/thesis/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/thesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/thesis/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/communities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/communities.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/records.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/subjects.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/users.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/affiliations_ror.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/awards.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/community_types.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/contrib/codemeta/
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/contrib/codemeta/development_status.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/date_types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/description_types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/funders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)   757044 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/languages.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    51778 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/licenses.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/names.yaml
--rw-r--r--   0 runner    (1001) docker     (123)  1272433 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/names_orcid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/relation_types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/resource_types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/roles.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/title_types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/users.py
--rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/vocabularies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/links.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/uow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/dumpers/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/dumpers/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/dumpers/edtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/dumpers/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/dumpers/pids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/definitions-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/definitions-v1.1.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/definitions-v1.2.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/definitions-v2.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/parent-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/parent-v2.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    14481 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/record-v2.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/record-v3.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/record-v4.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/record-v5.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v2.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v3.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v4.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    20690 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v5.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v2.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v3.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v4.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v5.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v2.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v3.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v4.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    20690 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v5.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v2.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v3.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v4.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v5.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v2.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v3.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v4.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    20690 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v5.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v2.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v3.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v4.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v5.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/embargo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/field/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/field/parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/field/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/owners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/draft_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/has_draftcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/requests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/requests/community_inclusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/requests/community_submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/requests/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/requests/entity_resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/deserializers/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/deserializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/deserializers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/deserializers/rocrate/
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/deserializers/rocrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/deserializers/rocrate/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/bibtex/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/bibtex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/bibtex/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/bibtex/schema_formats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/csl/
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/csl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/csl/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/datacite/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/datacite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20124 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/datacite/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/dcat/
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/dcat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   154012 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/dcat/datacite-to-dcat-ap.xsl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/dublincore/
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/dublincore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/dublincore/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/geojson/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/geojson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/geojson/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/iiif/
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/iiif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/iiif/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/marcxml/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/marcxml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/marcxml/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/ui/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/ui/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/secret_links/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/secret_links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/secret_links/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/secret_links/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/secret_links/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/secret_links/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/secret_links/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/communities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/communities/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/communities/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/community_inclusion/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/community_inclusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/community_inclusion/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/community_records/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/community_records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/community_records/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/components/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/components/access.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/components/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/components/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/components/parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/components/pids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/components/review.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/customizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/iiif/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/iiif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/iiif/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/providers/datacite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/providers/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/providers/oai.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/result_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/review/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/review/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/review/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/review/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/access.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/community_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/parent/
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/parent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/parent/access.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/parent/communities.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/pids.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/record_communities.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/secret_links/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/secret_links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/secret_links/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/services/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/templates/semantic-ui/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/templates/semantic-ui/imprint.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/templates/semantic-ui/invenio_rdm_records/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/templates/semantic-ui/invenio_rdm_records/oai-details.html
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/templates/semantic-ui/invenio_rdm_records/oai-search.html
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/templates/semantic-ui/journal.html
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/templates/semantic-ui/meeting.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13515 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13726 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13716 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13646 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    17019 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-24 17:42:05.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13737 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/invenio_rdm_records/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26330 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/invenio_rdm_records.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/requirements-feature.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/run-i18n-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1884 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53591 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/contrib/codemeta/
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/contrib/codemeta/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/contrib/codemeta/test_codemeta_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fake_datacite_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/app_data/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/app_data/communities.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/app_data/img/
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/app_data/img/community1.png
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/app_data/records.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/app_data/users.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/app_data/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/app_data/vocabularies/affiliations_ror.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/app_data/vocabularies/resource_types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/app_data/vocabularies/subjects_anzsrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/app_data/vocabularies/subjects_mesh.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/app_data/vocabularies/title_types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/app_data/vocabularies.alt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/app_data/vocabularies.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/data/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/data/vocabularies/awards.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/data/vocabularies/community_types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/data/vocabularies/description_types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/data/vocabularies/funders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/data/vocabularies/languages.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/data/vocabularies/relation_types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/data/vocabularies/resource_types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/data/vocabularies/roles.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/data/vocabularies/title_types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/data/vocabularies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/conflicting_module_A/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/conflicting_module_A/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/conflicting_module_A/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/conflicting_module_A/fixtures/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/conflicting_module_A/fixtures/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/conflicting_module_A/fixtures/vocabularies/subjects.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/conflicting_module_A/fixtures/vocabularies/vocabularies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/conflicting_module_B/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/conflicting_module_B/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/conflicting_module_B/fixtures/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/conflicting_module_B/fixtures/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/conflicting_module_B/fixtures/vocabularies/subjects.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/conflicting_module_B/fixtures/vocabularies/vocabularies.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/load_error/test_vocabularies_load_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_A/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_A/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_A/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_A/fixtures/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_A/fixtures/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_A/fixtures/vocabularies/subjects_anzsrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_A/fixtures/vocabularies/subjects_mesh.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_A/fixtures/vocabularies/vocabularies.alt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_A/fixtures/vocabularies/vocabularies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_B/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_B/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_B/fixtures/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_B/fixtures/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_B/fixtures/vocabularies/subjects.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/mock_module_B/fixtures/vocabularies/vocabularies.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/fixtures/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/records/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/records/dumpers/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/dumpers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/dumpers/test_access_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/dumpers/test_edtf_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/dumpers/test_location_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/dumpers/test_pids_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/full-record.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/systemfields/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/systemfields/test_access_systemfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/test_jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/test_records_communities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/test_relations_affiliations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/test_relations_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/test_relations_resource_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/test_relations_subjects.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/records/tombstone.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/resources/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/serializers/test_bibtex_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/serializers/test_csl_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/serializers/test_datacite_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/serializers/test_dcat_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/serializers/test_dublincore_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/serializers/test_geojson_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/serializers/test_marcxml_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/serializers/test_ui_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/test_draft_file_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/test_iiif_image_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/test_iiif_presentation_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/test_publish_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/test_record_file_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30779 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/test_resources_communities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/test_resources_community_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/test_resources_oai.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/test_resources_pids.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/test_resources_review.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/test_rocrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/test_serialized_links.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/resources/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/vocabularies/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/vocabularies/test_affiliations_vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/vocabularies/test_awards_vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/vocabularies/test_funders_vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/vocabularies/test_names_vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/resources/vocabularies/test_subjects_vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/secret_links/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/secret_links/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/secret_links/test_secret_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/secret_links/test_sharing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/secret_links/test_token_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/services/components/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/components/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/components/test_access_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/components/test_metadata_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/components/test_pids_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/components/test_relations_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/services/data/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/data/contributor_role.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/services/pids/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/services/pids/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/pids/providers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/pids/providers/test_datacite_pid_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/pids/providers/test_external_pid_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/pids/providers/test_oai_invenio_pid_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    32110 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/pids/test_pids_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/pids/test_pids_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:42:06.000000 invenio-rdm-records-2.9.0/tests/services/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_additional_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_additional_title.py
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_creator_contributor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_funding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_pids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_publication_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_rdm_record_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_related_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_rights.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/schemas/test_vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/test_oai_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/test_permissions_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/test_rdm_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/test_service_communities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/test_service_community_records.py
--rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/test_service_review.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/test_service_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/services/test_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/test_alembic.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/test_invenio_rdm_records.py
--rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-03-24 17:41:59.000000 invenio-rdm-records-2.9.0/tests/test_oai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/.github/workflows/tests-feature.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/administration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/administration/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/administration/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/administration/views/oai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/0cf260eb8e97_create_table_for_secret_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/4a15e8671f4d_create_rdm_records_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/88d1463de5c0_create_parent_record_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/8ed1a438601c_migrate_secret_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/9e0ac518b9df_create_records_communities_m2m_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/a3957490361d_remove_pidrelations_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/b822ba22c688_create_rdm_records_branch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/details/
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/details/CopyButton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/details/LinksTable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/details/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/search/DeleteModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/search/SearchResultItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/i18next-scanner.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/de/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/de/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/el/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/el/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/en/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    60991 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/scripts/compileCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/scripts/initCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/translations.pot
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/codemeta/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/codemeta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/codemeta/custom_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/imprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/imprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/imprint/custom_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/journal/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/journal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/journal/custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/journal/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/journal/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/meeting/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/meeting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/meeting/custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/meeting/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/meeting/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/thesis/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/thesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/thesis/custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/communities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/communities.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/records.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/subjects.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/users.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/affiliations_ror.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/awards.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/community_types.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/contrib/codemeta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/contrib/codemeta/development_status.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/date_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/description_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/funders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)   757044 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/languages.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    51778 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/licenses.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/names.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)  1272433 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/names_orcid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/relation_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/resource_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/roles.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/title_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/vocabularies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/uow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/dumpers/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/dumpers/edtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/dumpers/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/dumpers/pids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/dumpers/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/definitions-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/definitions-v1.1.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/definitions-v1.2.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/definitions-v2.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/parent-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/parent-v2.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14481 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/record-v2.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/record-v3.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/record-v4.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/record-v5.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v2.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v3.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v4.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21727 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v5.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v2.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v3.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v4.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20506 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v5.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v2.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v3.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v4.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21727 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v5.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v2.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v3.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v4.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20506 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v5.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v2.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v3.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v4.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21727 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v5.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v2.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v3.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v4.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20506 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v5.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/os-v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/os-v1/aggr-file-download-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/os-v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/os-v2/aggr-file-download-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/v7/aggr-file-download-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/os-v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/os-v1/aggr-record-view-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/os-v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/os-v2/aggr-record-view-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/v7/aggr-record-view-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/file_download/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/file_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/file_download/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/file_download/os-v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/file_download/os-v1/file-download-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/file_download/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/file_download/os-v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/file_download/os-v2/file-download-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/file_download/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/file_download/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/file_download/v7/file-download-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/record_view/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/record_view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/record_view/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/record_view/os-v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/record_view/os-v1/record-view-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/record_view/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/record_view/os-v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/record_view/os-v2/record-view-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/record_view/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/record_view/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/stats/templates/events/record_view/v7/record-view-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/embargo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/field/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/field/parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/field/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/owners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/draft_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/has_draftcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/requests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/requests/community_inclusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/requests/community_submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/requests/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/requests/entity_resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/deserializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/deserializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/deserializers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/deserializers/rocrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/deserializers/rocrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/deserializers/rocrate/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19158 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/bibtex/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/bibtex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/bibtex/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/bibtex/schema_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/csl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/csl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/csl/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/datacite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/datacite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20169 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/datacite/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/dcat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/dcat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154012 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/dcat/datacite-to-dcat-ap.xsl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/dublincore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/dublincore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/dublincore/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/geojson/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/geojson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/geojson/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/iiif/
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/iiif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/iiif/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/marcxml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/marcxml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/marcxml/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/ui/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/ui/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/resources/stats/event_builders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/secret_links/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/secret_links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/secret_links/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/secret_links/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/secret_links/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/secret_links/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/secret_links/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/communities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/communities/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/communities/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/community_inclusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/community_inclusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/community_inclusion/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/community_records/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/community_records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/community_records/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/components/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/components/custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/components/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/components/parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/components/pids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/components/review.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/customizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/iiif/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/iiif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/iiif/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/providers/datacite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/providers/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/providers/oai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/requests/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/result_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/review/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/review/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/review/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/review/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/community_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/parent/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/parent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/parent/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/parent/communities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/pids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/record_communities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/secret_links/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/secret_links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/secret_links/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/stats/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/services/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/templates/semantic-ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/templates/semantic-ui/imprint.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/templates/semantic-ui/invenio_rdm_records/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/templates/semantic-ui/invenio_rdm_records/oai-details.html
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/templates/semantic-ui/invenio_rdm_records/oai-search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/templates/semantic-ui/journal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/templates/semantic-ui/meeting.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13515 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-04-20 11:19:14.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-20 11:19:14.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-20 11:19:14.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-20 11:19:14.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-20 11:19:14.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13726 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13716 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-04-20 11:19:14.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-20 11:19:14.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-20 11:19:14.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13646 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-20 11:19:14.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-20 11:19:14.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    17019 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13737 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-04-20 11:19:14.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/invenio_rdm_records/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    29749 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/invenio_rdm_records.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/requirements-feature.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/run-i18n-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1884 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53205 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/tests/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/contrib/codemeta/
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/contrib/codemeta/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/contrib/codemeta/test_codemeta_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fake_datacite_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/fixtures/app_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/app_data/communities.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/fixtures/app_data/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/app_data/img/community1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/app_data/records.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/app_data/users.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/fixtures/app_data/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/app_data/vocabularies/affiliations_ror.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/app_data/vocabularies/resource_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/app_data/vocabularies/subjects_anzsrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/app_data/vocabularies/subjects_mesh.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/app_data/vocabularies/title_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/app_data/vocabularies.alt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/app_data/vocabularies.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/fixtures/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/fixtures/data/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/data/vocabularies/awards.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/data/vocabularies/community_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/data/vocabularies/description_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/data/vocabularies/funders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/data/vocabularies/languages.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/data/vocabularies/relation_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/data/vocabularies/resource_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/data/vocabularies/roles.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/data/vocabularies/title_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/data/vocabularies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/conflicting_module_A/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/conflicting_module_A/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/conflicting_module_A/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/conflicting_module_A/fixtures/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/conflicting_module_A/fixtures/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/conflicting_module_A/fixtures/vocabularies/subjects.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/conflicting_module_A/fixtures/vocabularies/vocabularies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/conflicting_module_B/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/conflicting_module_B/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/conflicting_module_B/fixtures/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/conflicting_module_B/fixtures/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/conflicting_module_B/fixtures/vocabularies/subjects.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/conflicting_module_B/fixtures/vocabularies/vocabularies.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/load_error/test_vocabularies_load_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_A/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_A/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_A/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_A/fixtures/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_A/fixtures/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_A/fixtures/vocabularies/subjects_anzsrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_A/fixtures/vocabularies/subjects_mesh.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_A/fixtures/vocabularies/vocabularies.alt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_A/fixtures/vocabularies/vocabularies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_B/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:15.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_B/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_B/fixtures/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_B/fixtures/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_B/fixtures/vocabularies/subjects.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/mock_module_B/fixtures/vocabularies/vocabularies.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/fixtures/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/records/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/dumpers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/dumpers/test_access_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/dumpers/test_edtf_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/dumpers/test_location_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/dumpers/test_pids_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/full-record.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/systemfields/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/systemfields/test_access_systemfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/test_jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/test_records_communities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/test_relations_affiliations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/test_relations_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/test_relations_resource_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/test_relations_subjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/records/tombstone.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/resources/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/serializers/test_bibtex_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/serializers/test_csl_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/serializers/test_datacite_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/serializers/test_dcat_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/serializers/test_dublincore_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/serializers/test_geojson_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/serializers/test_marcxml_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/serializers/test_ui_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/test_draft_file_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/test_iiif_image_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/test_iiif_presentation_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/test_publish_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/test_record_file_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30779 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/test_resources_communities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/test_resources_community_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/test_resources_oai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/test_resources_pids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/test_resources_record_communities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/test_resources_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/test_rocrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/test_serialized_links.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/resources/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/vocabularies/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/vocabularies/test_affiliations_vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/vocabularies/test_awards_vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/vocabularies/test_funders_vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/vocabularies/test_names_vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/resources/vocabularies/test_subjects_vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/secret_links/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/secret_links/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/secret_links/test_secret_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/secret_links/test_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/secret_links/test_token_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/services/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/components/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/components/test_access_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/components/test_metadata_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/components/test_pids_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/components/test_relations_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/services/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/data/contributor_role.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/services/pids/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/services/pids/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/pids/providers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/pids/providers/test_datacite_pid_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/pids/providers/test_external_pid_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/pids/providers/test_oai_invenio_pid_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32110 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/pids/test_pids_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/pids/test_pids_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:19:16.000000 invenio-rdm-records-3.0.0/tests/services/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_additional_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_additional_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_creator_contributor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_pids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_publication_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_rdm_record_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_related_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_rights.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/schemas/test_vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/test_oai_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/test_permissions_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/test_rdm_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/test_service_communities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/test_service_community_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/test_service_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/test_service_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/services/test_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/test_alembic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/test_invenio_rdm_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-04-20 11:19:02.000000 invenio-rdm-records-3.0.0/tests/test_oai.py
```

### Comparing `invenio-rdm-records-2.9.0/.editorconfig` & `invenio-rdm-records-3.0.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/.github/workflows/i18n-pull.yml` & `invenio-rdm-records-3.0.0/.github/workflows/i18n-pull.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/.github/workflows/i18n-push.yml` & `invenio-rdm-records-3.0.0/.github/workflows/i18n-push.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/.github/workflows/pypi-publish.yml` & `invenio-rdm-records-3.0.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/.github/workflows/stale.yml` & `invenio-rdm-records-3.0.0/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/.github/workflows/tests-feature.yml` & `invenio-rdm-records-3.0.0/.github/workflows/tests-feature.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/.github/workflows/tests.yml` & `invenio-rdm-records-3.0.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/.tx/config` & `invenio-rdm-records-3.0.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/CHANGES.rst` & `invenio-rdm-records-3.0.0/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,39 @@
     Invenio-RDM-Records is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 3.0.0 (released 2023-04-20)
+
+- usage statistics: refactor files structure
+
+Version 2.13.0 (released 2023-04-17)
+
+- serializers: added schema processors (custom fields)
+- serializers: created dump and load mixins for custom fields
+
+Version 2.12.0 (released 2023-04-06)
+
+- api: add record community suggestion endpoint
+
+Version 2.11.0 (released 2023-03-30)
+
+- add usage statistics indexing (by system field)
+- add sorting by most viewed to the config
+- move statistics events from invenio-app-rdm
+
+Version 2.10.0 (released 2023-03-28)
+
+- add requests endpoint to the record
+- dublincore: transform identifiers tu urls
+- record service: update community records
+
 Version 2.9.0 (released 2023-03-24)
 
 - communities: return ghost parent community when cannot be resolved
 - contrib: add journal and meeting sort options
 - contrib: updated custom fields UI widgets
 - custom_fields: rename CodeMeta to Software
```

### Comparing `invenio-rdm-records-2.9.0/CONTRIBUTING.rst` & `invenio-rdm-records-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/LICENSE` & `invenio-rdm-records-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/MANIFEST.in` & `invenio-rdm-records-3.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/PKG-INFO` & `invenio-rdm-records-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-records
-Version: 2.9.0
+Version: 3.0.0
 Summary: InvenioRDM module for the communities feature.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-records
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2019 CERN.
@@ -66,14 +66,39 @@
             Invenio-RDM-Records is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 3.0.0 (released 2023-04-20)
+        
+        - usage statistics: refactor files structure
+        
+        Version 2.13.0 (released 2023-04-17)
+        
+        - serializers: added schema processors (custom fields)
+        - serializers: created dump and load mixins for custom fields
+        
+        Version 2.12.0 (released 2023-04-06)
+        
+        - api: add record community suggestion endpoint
+        
+        Version 2.11.0 (released 2023-03-30)
+        
+        - add usage statistics indexing (by system field)
+        - add sorting by most viewed to the config
+        - move statistics events from invenio-app-rdm
+        
+        Version 2.10.0 (released 2023-03-28)
+        
+        - add requests endpoint to the record
+        - dublincore: transform identifiers tu urls
+        - record service: update community records
+        
         Version 2.9.0 (released 2023-03-24)
         
         - communities: return ghost parent community when cannot be resolved
         - contrib: add journal and meeting sort options
         - contrib: updated custom fields UI widgets
         - custom_fields: rename CodeMeta to Software
```

### Comparing `invenio-rdm-records-2.9.0/README.rst` & `invenio-rdm-records-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/babel.ini` & `invenio-rdm-records-3.0.0/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/docs/Makefile` & `invenio-rdm-records-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/docs/conf.py` & `invenio-rdm-records-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/docs/index.rst` & `invenio-rdm-records-3.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/docs/make.bat` & `invenio-rdm-records-3.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/administration/views/oai.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/administration/views/oai.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/0cf260eb8e97_create_table_for_secret_links.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/0cf260eb8e97_create_table_for_secret_links.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/4a15e8671f4d_create_rdm_records_tables.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/4a15e8671f4d_create_rdm_records_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/88d1463de5c0_create_parent_record_table.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/88d1463de5c0_create_parent_record_table.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/8ed1a438601c_migrate_secret_links.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/8ed1a438601c_migrate_secret_links.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/9e0ac518b9df_create_records_communities_m2m_table.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/9e0ac518b9df_create_records_communities_m2m_table.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/a3957490361d_remove_pidrelations_tables.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/a3957490361d_remove_pidrelations_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/alembic/b822ba22c688_create_rdm_records_branch.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/alembic/b822ba22c688_create_rdm_records_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/details/CopyButton.js` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/details/CopyButton.js`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/details/LinksTable.js` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/details/LinksTable.js`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/details/index.js` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/details/index.js`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/search/DeleteModal.js` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/search/DeleteModal.js`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/search/SearchResultItem.js` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/search/SearchResultItem.js`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/search/index.js` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/js/invenio_rdm_records/oaipmh/search/index.js`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/i18next-scanner.config.js` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/i18next-scanner.config.js`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/i18next.js` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/i18next.js`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/de/translations.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/de/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/el/translations.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/el/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/en/translations.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/messages/en/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/package-lock.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/package-lock.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/package.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/package.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/scripts/compileCatalog.js` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/scripts/compileCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/scripts/initCatalog.js` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/scripts/initCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/translations.pot` & `invenio-rdm-records-3.0.0/invenio_rdm_records/assets/semantic-ui/translations/invenio_rdm_records/translations.pot`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/cli.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/config.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2019 CERN.
 # Copyright (C) 2019 Northwestern University.
 # Copyright (C) 2021-2023 Graz University of Technology.
+# Copyright (C) 2023 TU Wien.
 #
 # Invenio-RDM-Records is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """DataCite-based data model for Invenio."""
 
 import idutils
@@ -193,29 +194,42 @@
         title=_("Recently updated"),
         fields=["-updated"],
     ),
     "updated-asc": dict(
         title=_("Least recently updated"),
         fields=["updated"],
     ),
+    "mostviewed": dict(
+        title=_("Most viewed"), fields=["-stats.all_versions.unique_views"]
+    ),
+    "mostdownloaded": dict(
+        title=_("Most downloaded"), fields=["-stats.all_versions.unique_downloads"]
+    ),
 }
 """Definitions of available record sort options.
 
 .. code-block:
 
     "<option name>": dict(
         title=_('<title>'),
         fields=['-updated'],
     ),
 
 """
 
 RDM_SEARCH = {
     "facets": ["access_status", "resource_type"],
-    "sort": ["bestmatch", "newest", "oldest", "version"],
+    "sort": [
+        "bestmatch",
+        "newest",
+        "oldest",
+        "version",
+        "mostviewed",
+        "mostdownloaded",
+    ],
 }
 """Record search configuration.
 
 The configuration has four possible keys:
 
 - ``facets`` - A list of facet names which must have been defined in
   ``RDM_FACETS``.
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/codemeta/custom_fields.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/codemeta/custom_fields.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/imprint/custom_fields.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/imprint/custom_fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,14 @@
                 "isbn": SanitizedUnicode(
                     validate=is_isbn,
                     error_messages={
                         "validator_failed": _("Please provide a valid ISBN.")
                     },
                 ),
                 "pages": SanitizedUnicode(),
-                "year": SanitizedUnicode(),
                 "place": SanitizedUnicode(),
             }
         )
 
     @property
     def mapping(self):
         """Imprint search mappings."""
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/journal/custom_fields.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/journal/custom_fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 - journal.title
 - journal.volume
 """
 
 from idutils import is_issn
 from invenio_i18n import lazy_gettext as _
 from invenio_records_resources.services.custom_fields import BaseCF
-from invenio_records_resources.services.records.facets import CFTermsFacet
 from marshmallow import fields
 from marshmallow_utils.fields import SanitizedUnicode
 
 
 class JournalCF(BaseCF):
     """Nested custom field."""
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/journal/sort.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/journal/sort.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/meeting/custom_fields.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/meeting/custom_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #
 # Copyright (C) 2023 CERN.
 #
 # Invenio-RDM-Records is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
+
 """Meeting custom fields.
 
 Implements the following fields:
 
 - meeting.acronym
 - meeting.dates
 - meeting.place
@@ -14,18 +15,18 @@
 - meeting.session
 - meeting.title
 - meeting.url
 """
 
 from invenio_i18n import lazy_gettext as _
 from invenio_records_resources.services.custom_fields import BaseCF
-from marshmallow import fields, validate
+from marshmallow import fields
 from marshmallow_utils.fields import SanitizedUnicode
 
-from invenio_rdm_records.services.schemas.metadata import _valid_url
+from ...services.schemas.metadata import _valid_url
 
 
 class MeetingCF(BaseCF):
     """Nested custom field."""
 
     @property
     def field(self):
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/meeting/sort.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/meeting/sort.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/contrib/thesis/custom_fields.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/contrib/thesis/custom_fields.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/ext.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,28 +34,31 @@
     RDMCommunityRecordsResource,
     RDMCommunityRecordsResourceConfig,
     RDMDraftFilesResourceConfig,
     RDMParentRecordLinksResource,
     RDMParentRecordLinksResourceConfig,
     RDMRecordCommunitiesResourceConfig,
     RDMRecordFilesResourceConfig,
+    RDMRecordRequestsResourceConfig,
     RDMRecordResource,
     RDMRecordResourceConfig,
 )
-from .resources.resources import RDMRecordCommunitiesResource
+from .resources.resources import RDMRecordCommunitiesResource, RDMRecordRequestsResource
 from .secret_links import LinkNeed, SecretLink
 from .services import (
     CommunityRecordsService,
     IIIFService,
     RDMCommunityRecordsConfig,
     RDMFileDraftServiceConfig,
     RDMFileRecordServiceConfig,
     RDMRecordCommunitiesConfig,
+    RDMRecordRequestsConfig,
     RDMRecordService,
     RDMRecordServiceConfig,
+    RecordRequestsService,
     SecretLinkService,
 )
 from .services.pids import PIDManager, PIDsService
 from .services.review.service import ReviewService
 
 
 def verify_token():
@@ -145,14 +148,15 @@
         class ServiceConfigs:
             record = RDMRecordServiceConfig.build(app)
             file = RDMFileRecordServiceConfig.build(app)
             file_draft = RDMFileDraftServiceConfig.build(app)
             oaipmh_server = OAIPMHServerServiceConfig
             record_communities = RDMRecordCommunitiesConfig.build(app)
             community_records = RDMCommunityRecordsConfig.build(app)
+            record_requests = RDMRecordRequestsConfig.build(app)
 
         return ServiceConfigs
 
     def init_services(self, app):
         """Initialize services."""
         service_configs = self.service_configs(app)
 
@@ -175,14 +179,17 @@
         )
 
         self.community_records_service = CommunityRecordsService(
             config=service_configs.community_records,
         )
 
         self.community_inclusion_service = CommunityInclusionService()
+        self.record_requests_service = RecordRequestsService(
+            config=service_configs.record_requests
+        )
 
         self.oaipmh_server_service = OAIPMHServerService(
             config=service_configs.oaipmh_server,
         )
 
     def init_resource(self, app):
         """Initialize resources."""
@@ -211,14 +218,19 @@
 
         # Record's communities
         self.record_communities_resource = RDMRecordCommunitiesResource(
             service=self.record_communities_service,
             config=RDMRecordCommunitiesResourceConfig.build(app),
         )
 
+        self.record_requests_resource = RDMRecordRequestsResource(
+            service=self.record_requests_service,
+            config=RDMRecordRequestsResourceConfig.build(app),
+        )
+
         # Community's records
         self.community_records_resource = RDMCommunityRecordsResource(
             service=self.community_records_service,
             config=RDMCommunityRecordsResourceConfig.build(app),
         )
 
         # OAI-PMH
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/communities.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/communities.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/affiliations_ror.yaml` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/affiliations_ror.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/contrib/codemeta/development_status.yaml` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/contrib/codemeta/development_status.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/date_types.yaml` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/date_types.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/description_types.yaml` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/description_types.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/funders.yaml` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/funders.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/languages.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/languages.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/languages.yaml` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/languages.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/licenses.csv` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/licenses.csv`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/names_orcid.yaml` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/names_orcid.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/relation_types.yaml` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/relation_types.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/resource_types.yaml` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/resource_types.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies/roles.yaml` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies/roles.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/data/vocabularies.yaml` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/data/vocabularies.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/demo.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/fixture.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/fixture.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/records.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/records.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/tasks.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/users.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/users.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/fixtures/vocabularies.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/fixtures/vocabularies.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/oai.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/oai.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 from .resources.serializers.datacite import DataCite43XMLSerializer
 from .resources.serializers.dcat import DCATSerializer
 from .resources.serializers.dublincore import DublinCoreXMLSerializer
 from .resources.serializers.marcxml import MARCXMLSerializer
 from .services.pids.providers.oai import OAIPIDProvider
 
 
-def dublincore_etree(pid, record):
+def dublincore_etree(pid, record, **serializer_kwargs):
     """Get DublinCore XML etree for OAI-PMH."""
-    json = DublinCoreXMLSerializer().dump_obj(record["_source"])
+    json = DublinCoreXMLSerializer(**serializer_kwargs).dump_obj(record["_source"])
     return simpledc.dump_etree(json)
 
 
 def oai_marcxml_etree(pid, record):
     """OAI MARCXML format for OAI-PMH.
 
     It assumes that record is a search result.
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/resources/config.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/resources/resources.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/resources/resources.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/config.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/errors.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/links.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/links.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/permissions.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/results.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/results.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/schema.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/services.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/services.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/oaiserver/services/uow.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/oaiserver/services/uow.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/proxies.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/api.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2020 CERN.
-# Copyright (C) 2021 TU Wien.
+# Copyright (C) 2021-2023 TU Wien.
 #
 # Invenio-RDM-Records is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """RDM Record and Draft API."""
 
 from invenio_communities.records.records.systemfields import CommunitiesField
@@ -32,16 +32,26 @@
 from invenio_vocabularies.contrib.awards.api import Award
 from invenio_vocabularies.contrib.funders.api import Funder
 from invenio_vocabularies.contrib.subjects.api import Subject
 from invenio_vocabularies.records.api import Vocabulary
 from invenio_vocabularies.records.systemfields.relations import CustomFieldsRelation
 
 from . import models
-from .dumpers import EDTFDumperExt, EDTFListDumperExt, GrantTokensDumperExt
-from .systemfields import HasDraftCheckField, ParentRecordAccessField, RecordAccessField
+from .dumpers import (
+    EDTFDumperExt,
+    EDTFListDumperExt,
+    GrantTokensDumperExt,
+    StatisticsDumperExt,
+)
+from .systemfields import (
+    HasDraftCheckField,
+    ParentRecordAccessField,
+    RecordAccessField,
+    RecordStatisticsField,
+)
 from .systemfields.draft_status import DraftStatus
 
 
 #
 # Parent record API
 #
 class RDMParent(ParentRecordBase):
@@ -82,14 +92,15 @@
 
     dumper = SearchDumper(
         extensions=[
             EDTFDumperExt("metadata.publication_date"),
             EDTFListDumperExt("metadata.dates", "date"),
             RelationDumperExt("relations"),
             CustomFieldsDumperExt(fields_var="RDM_CUSTOM_FIELDS"),
+            StatisticsDumperExt("stats"),
         ]
     )
 
     relations = MultiRelationsField(
         creator_affiliations=PIDNestedListRelation(
             "metadata.creators",
             relation_field="affiliations",
@@ -284,9 +295,11 @@
         delete=False,
     )
 
     has_draft = HasDraftCheckField(RDMDraft)
 
     status = DraftStatus()
 
+    stats = RecordStatisticsField()
+
 
 RDMFileRecord.record_cls = RDMRecord
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/dumpers/access.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/dumpers/access.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/dumpers/edtf.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/dumpers/edtf.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/dumpers/locations.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/dumpers/locations.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/dumpers/pids.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/dumpers/pids.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/definitions-v1.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/definitions-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/definitions-v1.1.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/definitions-v1.1.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/definitions-v1.2.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/definitions-v1.2.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/definitions-v2.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/definitions-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/parent-v1.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/parent-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/parent-v2.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/parent-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/record-v2.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/record-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/record-v3.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/record-v3.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/record-v4.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/record-v4.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/jsonschemas/records/record-v5.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/jsonschemas/records/record-v5.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v2.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v3.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v3.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v4.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v4.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v5.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v5.0.0.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9920394736842105%*

 * *Differences: {"'mappings'": "{'properties': {'parent': {'properties': {delete: ['review']}}, 'stats': "*

 * *               "OrderedDict([('properties', OrderedDict([('this_version', "*

 * *               "OrderedDict([('properties', OrderedDict([('views', OrderedDict([('type', "*

 * *               "'integer')])), ('unique_views', OrderedDict([('type', 'integer')])), ('downloads', "*

 * *               "OrderedDict([('type', 'integer')])), ('unique_downloads', OrderedDict([('type', "*

 * *               "'integer')])), ('data_volume', OrderedD […]*

```diff
@@ -81,31 +81,25 @@
             "created": {
                 "type": "date"
             },
             "custom_fields": {
                 "dynamic": true,
                 "type": "object"
             },
-            "expires_at": {
-                "type": "date"
-            },
             "files": {
                 "properties": {
                     "default_preview": {
                         "type": "keyword"
                     },
                     "enabled": {
                         "type": "boolean"
                     }
                 },
                 "type": "object"
             },
-            "fork_version_id": {
-                "type": "long"
-            },
             "has_draft": {
                 "type": "boolean"
             },
             "id": {
                 "type": "keyword"
             },
             "is_published": {
@@ -704,57 +698,14 @@
                             },
                             "status": {
                                 "index": false,
                                 "type": "keyword"
                             }
                         }
                     },
-                    "review": {
-                        "properties": {
-                            "$schema": {
-                                "index": false,
-                                "type": "keyword"
-                            },
-                            "@v": {
-                                "type": "keyword"
-                            },
-                            "created_by": {
-                                "dynamic": true,
-                                "type": "object"
-                            },
-                            "description": {
-                                "type": "text"
-                            },
-                            "id": {
-                                "type": "keyword"
-                            },
-                            "payload": {
-                                "dynamic": true,
-                                "type": "object"
-                            },
-                            "receiver": {
-                                "dynamic": true,
-                                "type": "object"
-                            },
-                            "status": {
-                                "type": "keyword"
-                            },
-                            "title": {
-                                "type": "text"
-                            },
-                            "topic": {
-                                "dynamic": true,
-                                "type": "object"
-                            },
-                            "type": {
-                                "type": "keyword"
-                            }
-                        },
-                        "type": "object"
-                    },
                     "updated": {
                         "type": "date"
                     },
                     "uuid": {
                         "index": false,
                         "type": "keyword"
                     },
@@ -783,14 +734,56 @@
                     }
                 }
             },
             "pids": {
                 "dynamic": true,
                 "type": "object"
             },
+            "stats": {
+                "properties": {
+                    "all_versions": {
+                        "properties": {
+                            "data_volume": {
+                                "type": "double"
+                            },
+                            "downloads": {
+                                "type": "integer"
+                            },
+                            "unique_downloads": {
+                                "type": "integer"
+                            },
+                            "unique_views": {
+                                "type": "integer"
+                            },
+                            "views": {
+                                "type": "integer"
+                            }
+                        }
+                    },
+                    "this_version": {
+                        "properties": {
+                            "data_volume": {
+                                "type": "double"
+                            },
+                            "downloads": {
+                                "type": "integer"
+                            },
+                            "unique_downloads": {
+                                "type": "integer"
+                            },
+                            "unique_views": {
+                                "type": "integer"
+                            },
+                            "views": {
+                                "type": "integer"
+                            }
+                        }
+                    }
+                }
+            },
             "updated": {
                 "type": "date"
             },
             "uuid": {
                 "index": false,
                 "type": "keyword"
             },
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v2.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v3.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v3.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v4.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v4.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/records/record-v5.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v5.0.0.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970588235294118%*

 * *Differences: {"'mappings'": "{'properties': {'stats': OrderedDict([('properties', OrderedDict([('this_version', "*

 * *               "OrderedDict([('properties', OrderedDict([('views', OrderedDict([('type', "*

 * *               "'integer')])), ('unique_views', OrderedDict([('type', 'integer')])), ('downloads', "*

 * *               "OrderedDict([('type', 'integer')])), ('unique_downloads', OrderedDict([('type', "*

 * *               "'integer')])), ('data_volume', OrderedDict([('type', 'double')]))]))])), "*

 * *               "('all_versions […]*

```diff
@@ -734,14 +734,56 @@
                     }
                 }
             },
             "pids": {
                 "dynamic": true,
                 "type": "object"
             },
+            "stats": {
+                "properties": {
+                    "all_versions": {
+                        "properties": {
+                            "data_volume": {
+                                "type": "double"
+                            },
+                            "downloads": {
+                                "type": "integer"
+                            },
+                            "unique_downloads": {
+                                "type": "integer"
+                            },
+                            "unique_views": {
+                                "type": "integer"
+                            },
+                            "views": {
+                                "type": "integer"
+                            }
+                        }
+                    },
+                    "this_version": {
+                        "properties": {
+                            "data_volume": {
+                                "type": "double"
+                            },
+                            "downloads": {
+                                "type": "integer"
+                            },
+                            "unique_downloads": {
+                                "type": "integer"
+                            },
+                            "unique_views": {
+                                "type": "integer"
+                            },
+                            "views": {
+                                "type": "integer"
+                            }
+                        }
+                    }
+                }
+            },
             "updated": {
                 "type": "date"
             },
             "uuid": {
                 "index": false,
                 "type": "keyword"
             },
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v2.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v3.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v3.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v4.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v4.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v5.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v5.0.0.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9920394736842105%*

 * *Differences: {"'mappings'": "{'properties': {'parent': {'properties': {delete: ['review']}}, 'stats': "*

 * *               "OrderedDict([('properties', OrderedDict([('this_version', "*

 * *               "OrderedDict([('properties', OrderedDict([('views', OrderedDict([('type', "*

 * *               "'integer')])), ('unique_views', OrderedDict([('type', 'integer')])), ('downloads', "*

 * *               "OrderedDict([('type', 'integer')])), ('unique_downloads', OrderedDict([('type', "*

 * *               "'integer')])), ('data_volume', OrderedD […]*

```diff
@@ -81,31 +81,25 @@
             "created": {
                 "type": "date"
             },
             "custom_fields": {
                 "dynamic": true,
                 "type": "object"
             },
-            "expires_at": {
-                "type": "date"
-            },
             "files": {
                 "properties": {
                     "default_preview": {
                         "type": "keyword"
                     },
                     "enabled": {
                         "type": "boolean"
                     }
                 },
                 "type": "object"
             },
-            "fork_version_id": {
-                "type": "long"
-            },
             "has_draft": {
                 "type": "boolean"
             },
             "id": {
                 "type": "keyword"
             },
             "is_published": {
@@ -704,57 +698,14 @@
                             },
                             "status": {
                                 "index": false,
                                 "type": "keyword"
                             }
                         }
                     },
-                    "review": {
-                        "properties": {
-                            "$schema": {
-                                "index": false,
-                                "type": "keyword"
-                            },
-                            "@v": {
-                                "type": "keyword"
-                            },
-                            "created_by": {
-                                "dynamic": true,
-                                "type": "object"
-                            },
-                            "description": {
-                                "type": "text"
-                            },
-                            "id": {
-                                "type": "keyword"
-                            },
-                            "payload": {
-                                "dynamic": true,
-                                "type": "object"
-                            },
-                            "receiver": {
-                                "dynamic": true,
-                                "type": "object"
-                            },
-                            "status": {
-                                "type": "keyword"
-                            },
-                            "title": {
-                                "type": "text"
-                            },
-                            "topic": {
-                                "dynamic": true,
-                                "type": "object"
-                            },
-                            "type": {
-                                "type": "keyword"
-                            }
-                        },
-                        "type": "object"
-                    },
                     "updated": {
                         "type": "date"
                     },
                     "uuid": {
                         "index": false,
                         "type": "keyword"
                     },
@@ -783,14 +734,56 @@
                     }
                 }
             },
             "pids": {
                 "dynamic": true,
                 "type": "object"
             },
+            "stats": {
+                "properties": {
+                    "all_versions": {
+                        "properties": {
+                            "data_volume": {
+                                "type": "double"
+                            },
+                            "downloads": {
+                                "type": "integer"
+                            },
+                            "unique_downloads": {
+                                "type": "integer"
+                            },
+                            "unique_views": {
+                                "type": "integer"
+                            },
+                            "views": {
+                                "type": "integer"
+                            }
+                        }
+                    },
+                    "this_version": {
+                        "properties": {
+                            "data_volume": {
+                                "type": "double"
+                            },
+                            "downloads": {
+                                "type": "integer"
+                            },
+                            "unique_downloads": {
+                                "type": "integer"
+                            },
+                            "unique_views": {
+                                "type": "integer"
+                            },
+                            "views": {
+                                "type": "integer"
+                            }
+                        }
+                    }
+                }
+            },
             "updated": {
                 "type": "date"
             },
             "uuid": {
                 "index": false,
                 "type": "keyword"
             },
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v2.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v3.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v3.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v4.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v4.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/records/record-v5.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v1/rdmrecords/drafts/draft-v5.0.0.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9920394736842105%*

 * *Differences: {"'mappings'": "{'properties': {'parent': {'properties': {'review': OrderedDict([('type', "*

 * *               "'object'), ('properties', OrderedDict([('$schema', OrderedDict([('type', "*

 * *               "'keyword'), ('index', False)])), ('id', OrderedDict([('type', 'keyword')])), "*

 * *               "('type', OrderedDict([('type', 'keyword')])), ('title', OrderedDict([('type', "*

 * *               "'text')])), ('description', OrderedDict([('type', 'text')])), ('status', "*

 * *               "OrderedDict([('type', 'keyword' […]*

```diff
@@ -81,25 +81,31 @@
             "created": {
                 "type": "date"
             },
             "custom_fields": {
                 "dynamic": true,
                 "type": "object"
             },
+            "expires_at": {
+                "type": "date"
+            },
             "files": {
                 "properties": {
                     "default_preview": {
                         "type": "keyword"
                     },
                     "enabled": {
                         "type": "boolean"
                     }
                 },
                 "type": "object"
             },
+            "fork_version_id": {
+                "type": "long"
+            },
             "has_draft": {
                 "type": "boolean"
             },
             "id": {
                 "type": "keyword"
             },
             "is_published": {
@@ -698,14 +704,57 @@
                             },
                             "status": {
                                 "index": false,
                                 "type": "keyword"
                             }
                         }
                     },
+                    "review": {
+                        "properties": {
+                            "$schema": {
+                                "index": false,
+                                "type": "keyword"
+                            },
+                            "@v": {
+                                "type": "keyword"
+                            },
+                            "created_by": {
+                                "dynamic": true,
+                                "type": "object"
+                            },
+                            "description": {
+                                "type": "text"
+                            },
+                            "id": {
+                                "type": "keyword"
+                            },
+                            "payload": {
+                                "dynamic": true,
+                                "type": "object"
+                            },
+                            "receiver": {
+                                "dynamic": true,
+                                "type": "object"
+                            },
+                            "status": {
+                                "type": "keyword"
+                            },
+                            "title": {
+                                "type": "text"
+                            },
+                            "topic": {
+                                "dynamic": true,
+                                "type": "object"
+                            },
+                            "type": {
+                                "type": "keyword"
+                            }
+                        },
+                        "type": "object"
+                    },
                     "updated": {
                         "type": "date"
                     },
                     "uuid": {
                         "index": false,
                         "type": "keyword"
                     },
@@ -734,14 +783,56 @@
                     }
                 }
             },
             "pids": {
                 "dynamic": true,
                 "type": "object"
             },
+            "stats": {
+                "properties": {
+                    "all_versions": {
+                        "properties": {
+                            "data_volume": {
+                                "type": "double"
+                            },
+                            "downloads": {
+                                "type": "integer"
+                            },
+                            "unique_downloads": {
+                                "type": "integer"
+                            },
+                            "unique_views": {
+                                "type": "integer"
+                            },
+                            "views": {
+                                "type": "integer"
+                            }
+                        }
+                    },
+                    "this_version": {
+                        "properties": {
+                            "data_volume": {
+                                "type": "double"
+                            },
+                            "downloads": {
+                                "type": "integer"
+                            },
+                            "unique_downloads": {
+                                "type": "integer"
+                            },
+                            "unique_views": {
+                                "type": "integer"
+                            },
+                            "views": {
+                                "type": "integer"
+                            }
+                        }
+                    }
+                }
+            },
             "updated": {
                 "type": "date"
             },
             "uuid": {
                 "index": false,
                 "type": "keyword"
             },
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v2.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v3.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v3.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v4.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v4.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v5.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/os-v2/rdmrecords/drafts/draft-v5.0.0.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973684210526316%*

 * *Differences: {"'mappings'": "{'properties': {'stats': OrderedDict([('properties', OrderedDict([('this_version', "*

 * *               "OrderedDict([('properties', OrderedDict([('views', OrderedDict([('type', "*

 * *               "'integer')])), ('unique_views', OrderedDict([('type', 'integer')])), ('downloads', "*

 * *               "OrderedDict([('type', 'integer')])), ('unique_downloads', OrderedDict([('type', "*

 * *               "'integer')])), ('data_volume', OrderedDict([('type', 'double')]))]))])), "*

 * *               "('all_versions […]*

```diff
@@ -783,14 +783,56 @@
                     }
                 }
             },
             "pids": {
                 "dynamic": true,
                 "type": "object"
             },
+            "stats": {
+                "properties": {
+                    "all_versions": {
+                        "properties": {
+                            "data_volume": {
+                                "type": "double"
+                            },
+                            "downloads": {
+                                "type": "integer"
+                            },
+                            "unique_downloads": {
+                                "type": "integer"
+                            },
+                            "unique_views": {
+                                "type": "integer"
+                            },
+                            "views": {
+                                "type": "integer"
+                            }
+                        }
+                    },
+                    "this_version": {
+                        "properties": {
+                            "data_volume": {
+                                "type": "double"
+                            },
+                            "downloads": {
+                                "type": "integer"
+                            },
+                            "unique_downloads": {
+                                "type": "integer"
+                            },
+                            "unique_views": {
+                                "type": "integer"
+                            },
+                            "views": {
+                                "type": "integer"
+                            }
+                        }
+                    }
+                }
+            },
             "updated": {
                 "type": "date"
             },
             "uuid": {
                 "index": false,
                 "type": "keyword"
             },
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v2.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v3.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v3.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v4.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v4.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v5.0.0.json` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v5.0.0.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9920394736842105%*

 * *Differences: {"'mappings'": "{'properties': {'parent': {'properties': {'review': OrderedDict([('type', "*

 * *               "'object'), ('properties', OrderedDict([('$schema', OrderedDict([('type', "*

 * *               "'keyword'), ('index', False)])), ('id', OrderedDict([('type', 'keyword')])), "*

 * *               "('type', OrderedDict([('type', 'keyword')])), ('title', OrderedDict([('type', "*

 * *               "'text')])), ('description', OrderedDict([('type', 'text')])), ('status', "*

 * *               "OrderedDict([('type', 'keyword' […]*

```diff
@@ -81,25 +81,31 @@
             "created": {
                 "type": "date"
             },
             "custom_fields": {
                 "dynamic": true,
                 "type": "object"
             },
+            "expires_at": {
+                "type": "date"
+            },
             "files": {
                 "properties": {
                     "default_preview": {
                         "type": "keyword"
                     },
                     "enabled": {
                         "type": "boolean"
                     }
                 },
                 "type": "object"
             },
+            "fork_version_id": {
+                "type": "long"
+            },
             "has_draft": {
                 "type": "boolean"
             },
             "id": {
                 "type": "keyword"
             },
             "is_published": {
@@ -698,14 +704,57 @@
                             },
                             "status": {
                                 "index": false,
                                 "type": "keyword"
                             }
                         }
                     },
+                    "review": {
+                        "properties": {
+                            "$schema": {
+                                "index": false,
+                                "type": "keyword"
+                            },
+                            "@v": {
+                                "type": "keyword"
+                            },
+                            "created_by": {
+                                "dynamic": true,
+                                "type": "object"
+                            },
+                            "description": {
+                                "type": "text"
+                            },
+                            "id": {
+                                "type": "keyword"
+                            },
+                            "payload": {
+                                "dynamic": true,
+                                "type": "object"
+                            },
+                            "receiver": {
+                                "dynamic": true,
+                                "type": "object"
+                            },
+                            "status": {
+                                "type": "keyword"
+                            },
+                            "title": {
+                                "type": "text"
+                            },
+                            "topic": {
+                                "dynamic": true,
+                                "type": "object"
+                            },
+                            "type": {
+                                "type": "keyword"
+                            }
+                        },
+                        "type": "object"
+                    },
                     "updated": {
                         "type": "date"
                     },
                     "uuid": {
                         "index": false,
                         "type": "keyword"
                     },
@@ -734,14 +783,56 @@
                     }
                 }
             },
             "pids": {
                 "dynamic": true,
                 "type": "object"
             },
+            "stats": {
+                "properties": {
+                    "all_versions": {
+                        "properties": {
+                            "data_volume": {
+                                "type": "double"
+                            },
+                            "downloads": {
+                                "type": "integer"
+                            },
+                            "unique_downloads": {
+                                "type": "integer"
+                            },
+                            "unique_views": {
+                                "type": "integer"
+                            },
+                            "views": {
+                                "type": "integer"
+                            }
+                        }
+                    },
+                    "this_version": {
+                        "properties": {
+                            "data_volume": {
+                                "type": "double"
+                            },
+                            "downloads": {
+                                "type": "integer"
+                            },
+                            "unique_downloads": {
+                                "type": "integer"
+                            },
+                            "unique_views": {
+                                "type": "integer"
+                            },
+                            "views": {
+                                "type": "integer"
+                            }
+                        }
+                    }
+                }
+            },
             "updated": {
                 "type": "date"
             },
             "uuid": {
                 "index": false,
                 "type": "keyword"
             },
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/models.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """System Fields for RDM Records."""
 
 from .access import ParentRecordAccessField, RecordAccessField
 from .draft_status import DraftStatus
 from .has_draftcheck import HasDraftCheckField
+from .statistics import RecordStatisticsField
 
 __all__ = (
     "DraftStatus",
     "HasDraftCheckField",
     "ParentRecordAccessField",
     "RecordAccessField",
+    "RecordStatisticsField",
 )
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/embargo.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/embargo.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/field/parent.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/field/parent.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/field/record.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/field/record.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/grants.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/grants.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/links.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/links.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/owners.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/owners.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/access/protection.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/access/protection.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/draft_status.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/draft_status.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/records/systemfields/has_draftcheck.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/records/systemfields/has_draftcheck.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/requests/community_inclusion.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/requests/community_inclusion.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,29 @@
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Community addition request."""
 
 from invenio_i18n import lazy_gettext as _
 from invenio_records_resources.services.uow import RecordCommitOp, RecordIndexOp
 from invenio_requests.customizations import RequestType, actions
+from invenio_requests.errors import CannotExecuteActionError
+
+from invenio_rdm_records.services.errors import InvalidAccessRestrictions
 
 from ..proxies import current_rdm_records_service as service
 
 
+def is_access_restriction_valid(record, community):
+    """Validate that public record cannot be added to restricted community."""
+    is_record_public = record.access.protection.record == "public"
+    is_community_restricted = community.access.visibility_is_restricted
+    invalid = is_record_public and is_community_restricted
+    return not invalid
+
+
 #
 # Actions
 #
 class SubmitAction(actions.SubmitAction):
     """Submit action."""
 
     def execute(self, identity, uow):
@@ -37,14 +48,18 @@
         # community receivers and record topics.
         record = self.request.topic.resolve()
         community = self.request.receiver.resolve()
 
         # integrity check, it should never happen on a published record
         assert not record.parent.review
 
+        if not is_access_restriction_valid(record, community):
+            description = InvalidAccessRestrictions.description
+            raise CannotExecuteActionError(description)
+
         # set the community to `default` if it is the first
         default = not record.parent.communities
         record.parent.communities.add(community, request=self.request, default=default)
         uow.register(RecordCommitOp(record.parent))
         uow.register(RecordIndexOp(record, indexer=service.indexer))
 
         super().execute(identity, uow)
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/requests/community_submission.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/requests/community_submission.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/requests/decorators.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/requests/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/requests/entity_resolvers.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/requests/entity_resolvers.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 from .config import (
     IIIFResourceConfig,
     RDMCommunityRecordsResourceConfig,
     RDMDraftFilesResourceConfig,
     RDMParentRecordLinksResourceConfig,
     RDMRecordCommunitiesResourceConfig,
     RDMRecordFilesResourceConfig,
+    RDMRecordRequestsResourceConfig,
     RDMRecordResourceConfig,
 )
 from .resources import (
     IIIFResource,
     RDMCommunityRecordsResource,
     RDMParentRecordLinksResource,
+    RDMRecordRequestsResource,
     RDMRecordResource,
 )
 
 __all__ = (
     "IIIFResource",
     "IIIFResourceConfig",
     "RDMCommunityRecordsResourceConfig",
@@ -32,8 +34,10 @@
     "RDMDraftFilesResourceConfig",
     "RDMParentRecordLinksResource",
     "RDMParentRecordLinksResourceConfig",
     "RDMRecordFilesResourceConfig",
     "RDMRecordResource",
     "RDMRecordResourceConfig",
     "RDMRecordCommunitiesResourceConfig",
+    "RDMRecordRequestsResourceConfig",
+    "RDMRecordRequestsResource",
 )
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/args.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/args.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/config.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,19 +25,18 @@
 from invenio_communities.communities.resources import CommunityResourceConfig
 from invenio_communities.communities.resources.config import community_error_handlers
 from invenio_drafts_resources.resources import RecordResourceConfig
 from invenio_i18n import lazy_gettext as _
 from invenio_records.systemfields.relations import InvalidRelationValue
 from invenio_records_resources.resources.files import FileResourceConfig
 from invenio_records_resources.services.base.config import ConfiguratorMixin, FromConfig
+from invenio_requests.resources.requests.config import RequestSearchRequestArgsSchema
 
 from ..services.errors import (
-    CommunityInclusionInconsistentAccessRestrictions,
-    MaxNumberCommunitiesExceeded,
-    MaxNumberOfRecordsExceed,
+    InvalidAccessRestrictions,
     ReviewExistsError,
     ReviewNotFoundError,
     ReviewStateError,
     ValidationErrorWithMessageAsList,
 )
 from .args import RDMSearchRequestArgsSchema
 from .deserializers import ROCrateJSONDeserializer
@@ -156,15 +155,15 @@
         ),
         InvalidRelationValue: create_error_handler(
             lambda exc: HTTPJSONException(
                 code=400,
                 description=exc.args[0],
             )
         ),
-        CommunityInclusionInconsistentAccessRestrictions: create_error_handler(
+        InvalidAccessRestrictions: create_error_handler(
             lambda exc: HTTPJSONException(
                 code=400,
                 description=exc.args[0],
             )
         ),
         ValidationErrorWithMessageAsList: create_error_handler(
             lambda e: HTTPJSONValidationWithMessageAsListException(e)
@@ -243,47 +242,53 @@
 #
 # Community's records
 #
 class RDMCommunityRecordsResourceConfig(RecordResourceConfig, ConfiguratorMixin):
     """Community's records resource config."""
 
     blueprint_name = "community-records"
-
     url_prefix = "/communities"
-
-    # Community's records
     routes = {"list": "/<pid_value>/records"}
 
     response_handlers = record_serializers
 
-    error_handlers = {
-        MaxNumberOfRecordsExceed: create_error_handler(
-            lambda e: HTTPJSONException(
-                code=400,
-                description=str(e),
-            )
-        ),
-    }
-
 
 class RDMRecordCommunitiesResourceConfig(CommunityResourceConfig, ConfiguratorMixin):
     """Record communities resource config."""
 
     blueprint_name = "records-community"
     url_prefix = "/records"
-    routes = {"list": "/<pid_value>/communities"}
+    routes = {
+        "list": "/<pid_value>/communities",
+        "suggestions": "/<pid_value>/communities-suggestions",
+    }
 
-    error_handlers = {
-        **community_error_handlers,
-        MaxNumberCommunitiesExceeded: create_error_handler(
-            lambda e: HTTPJSONException(
-                code=400,
-                description=str(e),
-            )
-        ),
+    request_extra_args = {
+        "expand": ma.fields.Boolean(),
+        "membership": ma.fields.Boolean(),
+    }
+
+    error_handlers = community_error_handlers
+
+
+class RDMRecordRequestsResourceConfig(ResourceConfig, ConfiguratorMixin):
+    """Record communities resource config."""
+
+    blueprint_name = "records-requests"
+    url_prefix = "/records"
+    routes = {"list": "/<record_pid>/requests"}
+
+    request_search_args = RequestSearchRequestArgsSchema
+
+    request_view_args = {
+        "record_pid": ma.fields.Str(),
+    }
+
+    request_extra_args = {
+        "expand": ma.fields.Boolean(),
     }
 
 
 #
 # IIIF
 #
 class IIIFResourceConfig(ResourceConfig, ConfiguratorMixin):
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/deserializers/rocrate/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/deserializers/rocrate/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/deserializers/rocrate/schema.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/deserializers/rocrate/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/errors.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/resources.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,14 +170,15 @@
     def create_url_rules(self):
         """Create the URL rules for the record resource."""
         routes = self.config.routes
         url_rules = [
             route("GET", routes["list"], self.search),
             route("POST", routes["list"], self.add),
             route("DELETE", routes["list"], self.remove),
+            route("GET", routes["suggestions"], self.get_suggestions),
         ]
         return url_rules
 
     @request_search_args
     @request_view_args
     @response_handler(many=True)
     def search(self):
@@ -192,38 +193,99 @@
         return items.to_dict(), 200
 
     @request_view_args
     @response_handler()
     @request_data
     def add(self):
         """Include record in communities."""
-        response = self.service.add(
+        processed, errors = self.service.add(
             identity=g.identity,
             id_=resource_requestctx.view_args["pid_value"],
             data=resource_requestctx.data,
         )
 
-        return response, 200
+        response = {}
+        if processed:
+            response["processed"] = processed
+        if errors:
+            response["errors"] = errors
+
+        # TODO why not checking errors
+        return response, 200 if len(processed) > 0 else 400
 
     @request_view_args
     @request_data
     @response_handler()
     def remove(self):
         """Remove communities from the record."""
-        errors = self.service.remove(
+        processed, errors = self.service.remove(
             identity=g.identity,
             id_=resource_requestctx.view_args["pid_value"],
             data=resource_requestctx.data,
         )
 
         response = {}
         if errors:
             response["errors"] = errors
 
-        return response, 200
+        return response, 200 if len(processed) > 0 else 400
+
+    @request_extra_args
+    @request_search_args
+    @request_view_args
+    @response_handler(many=True)
+    def get_suggestions(self):
+        """Search for record's communities."""
+        by_membership = resource_requestctx.args.get("membership", False)
+
+        items = self.service.search_suggested_communities(
+            identity=g.identity,
+            id_=resource_requestctx.view_args["pid_value"],
+            params=resource_requestctx.args,
+            search_preference=search_preference(),
+            by_membership=by_membership,
+            expand=resource_requestctx.args.get("expand", False),
+        )
+        return items.to_dict(), 200
+
+
+class RDMRecordRequestsResource(ErrorHandlersMixin, Resource):
+    """Record requests resource."""
+
+    def __init__(self, config, service):
+        """Constructor."""
+        super().__init__(config)
+        self.service = service
+
+    def create_url_rules(self):
+        """Create the URL rules for the record resource."""
+        routes = self.config.routes
+        url_rules = [
+            route("GET", routes["list"], self.search),
+        ]
+        return url_rules
+
+    @request_extra_args
+    @request_search_args
+    @request_view_args
+    @response_handler(many=True)
+    def search(self):
+        """Search for record's requests.
+
+        GET /records/<pid>/requests
+        """
+        items = self.service.search(
+            identity=g.identity,
+            params=resource_requestctx.args,
+            record_pid=resource_requestctx.view_args["record_pid"],
+            search_preference=search_preference(),
+            expand=resource_requestctx.args.get("expand", False),
+        )
+
+        return items.to_dict(), 200
 
 
 #
 # Parent Record Links
 #
 class RDMParentRecordLinksResource(RecordResource):
     """Secret links resource."""
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/bibtex/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/bibtex/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/bibtex/schema.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/bibtex/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 # Invenio-RDM-Records is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """BibTex based Schema for Invenio RDM Records."""
 
 import datetime
 
-from marshmallow import fields, missing, post_dump
+from flask_resources.serializers import BaseSerializerSchema
+from marshmallow import fields, post_dump
 from slugify import slugify
 
-from ..schemas import BaseSchema
+from ..schemas import CommonFieldsMixin
 from .schema_formats import BibTexFormatter
 
 
-class BibTexSchema(BaseSchema):
+class BibTexSchema(BaseSerializerSchema, CommonFieldsMixin):
     """Schema for records in BibTex."""
 
     id = fields.Str()
     resource_id = fields.Str(attribute="metadata.resource_type.id")
     version = fields.Str(attribute="metadata.version")
     date_created = fields.Method("get_date_created")
     locations = fields.Method("get_locations")
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/bibtex/schema_formats.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/bibtex/schema_formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     #     return BibTexFormatter.other()
 
     def publication_book():
         """Format book entry type. A book with an explicit publisher."""
         name = "book"
         req_fields = ["author", "title", "publisher", "year"]
         opt_fields = ["volume", "address", "month", "note"]
-        return format(name, req_fields, opt_fields)
+        return BibTexFormatter.format(name, req_fields, opt_fields)
 
     # def publication_section():
     #     return BibTexFormatter.other()
 
     # def publication_conferencepaper():
     #     return BibTexFormatter.other()
 
@@ -77,15 +77,15 @@
     #     return BibTexFormatter.other()
 
     def publication_article():
         """Format article entry type. An article from a journal or magazine."""
         name = "article"
         req_fields = ["author", "title", "journal", "year"]
         opt_fields = ["volume", "number", "pages", "month", "note"]
-        return format(name, req_fields, opt_fields)
+        return BibTexFormatter.format(name, req_fields, opt_fields)
 
     # def publication_patent():
     #     return BibTexFormatter.other()
 
     # def publication_preprint():
     #     return BibTexFormatter().other()
 
@@ -111,15 +111,15 @@
     #     return BibTexFormatter().other()
 
     def publication_thesis():
         """Format article entry type. An article from a journal or magazine."""
         name = "phdthesis"
         req_fields = ["author", "title", "school", "year"]
         opt_fields = ["address", "month", "note"]
-        return format(name, req_fields, opt_fields)
+        return BibTexFormatter.format(name, req_fields, opt_fields)
 
     # def publication_other():
     #     return BibTexFormatter().other()
 
     # def poster():
     #     return BibTexFormatter().other()
 
@@ -135,15 +135,15 @@
             "title",
             "month",
             "year",
             "note",
             "publisher",
             "version",
         ]
-        return format(name, req_fields, opt_fields)
+        return BibTexFormatter.format(name, req_fields, opt_fields)
 
     # def image_figure():
     #     return BibTexFormatter().other()
 
     # def image_plot():
     #     return BibTexFormatter().other()
 
@@ -171,15 +171,15 @@
             "title",
             "month",
             "year",
             "note",
             "publisher",
             "version",
         ]
-        return format(name, req_fields, opt_fields)
+        return BibTexFormatter.format(name, req_fields, opt_fields)
 
     # def lesson():
     #     return BibTexFormatter().other()
 
     def other():
         """Format misc entry type. For use when nothing else fits."""
         name = "misc"
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/csl/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/csl/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,26 +20,28 @@
 from citeproc_styles import get_style_filepath
 from citeproc_styles.errors import StyleNotFoundError
 from flask import current_app
 from flask_resources import BaseListSchema, MarshmallowSerializer
 from flask_resources.serializers import JSONSerializer
 from webargs import fields
 
+from ....contrib.journal.processors import JournalCSLDumper
 from .schema import CSLJSONSchema
 
 
 class CSLJSONSerializer(MarshmallowSerializer):
     """Marshmallow based CSL JSON serializer for records."""
 
     def __init__(self, **options):
         """Constructor."""
         super().__init__(
             format_serializer_cls=JSONSerializer,
             object_schema_cls=CSLJSONSchema,
             list_schema_cls=BaseListSchema,
+            schema_kwargs={"dumpers": [JournalCSLDumper()]},  # Order matters
             **options,
         )
 
 
 def get_citation_string(json, id, style, locale):
     """Get the citation string from CiteProc library."""
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/csl/schema.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/csl/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """CSL based Schema for Invenio RDM Records."""
 
 from edtf import parse_edtf
 from edtf.parser.edtf_exceptions import EDTFParseException
 from edtf.parser.parser_classes import Date, Interval
+from flask_resources.serializers import BaseSerializerSchema
 from invenio_access.permissions import system_identity
 from invenio_records_resources.proxies import current_service_registry
 from invenio_vocabularies.proxies import current_service as vocabulary_service
 from marshmallow import Schema, fields, missing, pre_dump
 from marshmallow_utils.fields import SanitizedUnicode, StrippedHTML
 
 from ..utils import get_preferred_identifier
@@ -41,15 +42,15 @@
     _list = []
     _list.append(year) if year else None
     _list.append(month) if month else None
     _list.append(day) if day else None
     return _list
 
 
-class CSLJSONSchema(Schema):
+class CSLJSONSchema(BaseSerializerSchema):
     """CSL Marshmallow Schema."""
 
     id_ = SanitizedUnicode(data_key="id", attribute="id")
     type_ = fields.Method("get_type", data_key="type")
     title = SanitizedUnicode(attribute="metadata.title")
     abstract = StrippedHTML(attribute="metadata.description")
     author = fields.List(fields.Nested(CSLCreatorSchema), attribute="metadata.creators")
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/datacite/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/datacite/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,35 +6,38 @@
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """DataCite Serializers for Invenio RDM Records."""
 from datacite import schema43
 from flask_resources import BaseListSchema, MarshmallowSerializer
 from flask_resources.serializers import JSONSerializer, SimpleSerializer
 
+from ....contrib.journal.processors import JournalDataciteDumper
 from .schema import DataCite43Schema
 
 
 class DataCite43JSONSerializer(MarshmallowSerializer):
     """Marshmallow based DataCite serializer for records."""
 
     def __init__(self, **options):
         """Constructor."""
         super().__init__(
             format_serializer_cls=JSONSerializer,
             object_schema_cls=DataCite43Schema,
             list_schema_cls=BaseListSchema,
+            schema_kwargs={"dumpers": [JournalDataciteDumper()]},  # Order matters
             **options
         )
 
 
 class DataCite43XMLSerializer(MarshmallowSerializer):
     """JSON based DataCite XML serializer for records."""
 
     def __init__(self, **options):
         """Constructor."""
         encoder = options.get("encoder", schema43.tostring)
         super().__init__(
             format_serializer_cls=SimpleSerializer,
             object_schema_cls=DataCite43Schema,
             list_schema_cls=BaseListSchema,
+            schema_kwargs={"dumpers": [JournalDataciteDumper()]},  # Order matters
             encoder=encoder,
         )
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/datacite/schema.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/datacite/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """DataCite based Schema for Invenio RDM Records."""
 
 from edtf import parse_edtf
 from edtf.parser.grammar import ParseException
 from flask import current_app
+from flask_resources.serializers import BaseSerializerSchema
 from invenio_access.permissions import system_identity
 from invenio_i18n import lazy_gettext as _
 from invenio_records_resources.proxies import current_service_registry
 from invenio_vocabularies.proxies import current_service as vocabulary_service
 from marshmallow import Schema, ValidationError, fields, missing, post_dump, validate
 from marshmallow_utils.fields import SanitizedUnicode
 from marshmallow_utils.html import strip_html
 
-from invenio_rdm_records.resources.serializers.ui.schema import current_default_locale
-
+from ...serializers.ui.schema import current_default_locale
 from ..utils import get_preferred_identifier, get_vocabulary_props
 
 
 def get_scheme_datacite(scheme, config_name, default=None):
     """Returns the datacite equivalent of a scheme."""
     config_item = current_app.config[config_name]
     return config_item.get(scheme, {}).get("datacite", default)
@@ -164,15 +164,15 @@
     """Subjects schema for v43."""
 
     subject = fields.Str(attribute="subject")
     valueURI = fields.Str(attribute="identifier")
     subjectScheme = fields.Str(attribute="scheme")
 
 
-class DataCite43Schema(Schema):
+class DataCite43Schema(BaseSerializerSchema):
     """DataCite JSON 4.3 Marshmallow Schema."""
 
     # PIDS-FIXME: What about versioning links and related ids
     types = fields.Method("get_type")
     titles = fields.Method("get_titles")
     creators = fields.List(
         fields.Nested(CreatorSchema43), attribute="metadata.creators"
@@ -256,15 +256,15 @@
         try:
             publication_date = obj["metadata"]["publication_date"]
             parsed_date = parse_edtf(publication_date)
             return str(parsed_date.lower_strict().tm_year)
         except ParseException:
             # Should not fail since it was validated at service schema
             current_app.logger.error(
-                "Error parsing publication_date field for" f"record {obj['metadata']}"
+                f"Error parsing publication_date field for record {obj['metadata']}"
             )
             raise ValidationError(_("Invalid publication date value."))
 
     def get_dates(self, obj):
         """Get dates."""
         dates = [{"date": obj["metadata"]["publication_date"], "dateType": "Issued"}]
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/dcat/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/dcat/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/dcat/datacite-to-dcat-ap.xsl` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/dcat/datacite-to-dcat-ap.xsl`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/dublincore/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/dublincore/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,27 +7,34 @@
 
 """Dublin Core Serializers for Invenio RDM Records."""
 
 from dcxml import simpledc
 from flask_resources import BaseListSchema, MarshmallowSerializer
 from flask_resources.serializers import JSONSerializer, SimpleSerializer
 
+from invenio_rdm_records.contrib.journal.processors import JournalDublinCoreDumper
+from invenio_rdm_records.contrib.meeting.processors import MeetingDublinCoreDumper
+
 from .schema import DublinCoreSchema
 
 
 class DublinCoreJSONSerializer(MarshmallowSerializer):
     """Marshmallow based Dublin Core serializer for records."""
 
     def __init__(self, **options):
         """Constructor."""
         super().__init__(
             format_serializer_cls=JSONSerializer,
             object_schema_cls=DublinCoreSchema,
             list_schema_cls=BaseListSchema,
-            **options
+            schema_kwargs={
+                # processors order matters
+                "dumpers": [JournalDublinCoreDumper(), MeetingDublinCoreDumper()]
+            },
+            **options,
         )
 
 
 class DublinCoreXMLSerializer(MarshmallowSerializer):
     """Marshmallow based Dublin Core serializer for records.
 
     Note: This serializer is not suitable for serializing large number of
@@ -36,9 +43,13 @@
 
     def __init__(self, **options):
         """Constructor."""
         super().__init__(
             format_serializer_cls=SimpleSerializer,
             object_schema_cls=DublinCoreSchema,
             list_schema_cls=BaseListSchema,
+            schema_kwargs={
+                "dumpers": [JournalDublinCoreDumper(), MeetingDublinCoreDumper()]
+            },
             encoder=simpledc.tostring,
+            **options,
         )
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/geojson/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/geojson/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/geojson/schema.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/geojson/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/iiif/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/iiif/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/iiif/schema.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/iiif/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/marcxml/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/marcxml/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """MARCXML Serializer for Invenio RDM Records."""
 
 from dojson.contrib.to_marc21.utils import dumps_etree
 from flask_resources import BaseListSchema, MarshmallowSerializer
 from flask_resources.serializers import SimpleSerializer
 from lxml import etree
 
+from ....contrib.journal.processors import JournalMarcXMLDumper
 from .schema import MARCXMLSchema
 
 
 class MARCXMLSerializer(MarshmallowSerializer):
     """Marshmallow based MARCXML serializer for records.
 
     Note: This serializer is not suitable for serializing large number of
@@ -24,14 +25,15 @@
 
     def __init__(self, **options):
         """Constructor."""
         super().__init__(
             format_serializer_cls=SimpleSerializer,
             object_schema_cls=MARCXMLSchema,
             list_schema_cls=BaseListSchema,
+            schema_kwargs={"dumpers": [JournalMarcXMLDumper()]},
             encoder=self.marcxml_tostring,
         )
 
     @classmethod
     def marcxml_tostring(cls, record):
         """Stringify a MarcXML record."""
         return etree.tostring(
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/marcxml/schema.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/marcxml/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """MARCXML based Schema for Invenio RDM Records."""
 
 from copy import deepcopy
 
 import bleach
+from flask_resources.serializers import BaseSerializerSchema
 from invenio_access.permissions import system_identity
 from invenio_vocabularies.proxies import current_service as vocabulary_service
 from marshmallow import fields, missing, post_dump
 
-from ..schemas import BaseSchema
+from ..schemas import CommonFieldsMixin
 from ..ui.schema import current_default_locale
 from ..utils import get_vocabulary_props
 
 
-class MARCXMLSchema(BaseSchema):
+class MARCXMLSchema(BaseSerializerSchema, CommonFieldsMixin):
     """Schema for records in MARC."""
 
     doi = fields.Method("get_doi")
     oai = fields.Str(attribute="pids.oai.identifier")
     contributors = fields.Method("get_contributors")
     titles = fields.Method("get_titles")
     creators = fields.Method("get_creators")
@@ -198,14 +199,16 @@
                 "props.eurepo",
             ],
             obj["metadata"]["resource_type"]["id"],
         )
         t = props.get("eurepo")
         return [t] if t else missing
 
+    # FIXME should this be a processor? that's somehow the post_dump place
+    # otherwise we cannot guarantee order
     @post_dump()
     def keys_to_tags(self, data, many, **kwargs):
         """Changes the key name to the corresponding MARCXML tag (number)."""
         # [!] The string in the first array corresponds to the tag[0:4] + ind1[4] + ind2[5]
         # [!] The first string needs to be length *5* (this is to do with the dojson parser)
         # [!] The second string corresponds to the subfield code
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/schemas.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/schemas.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 #
 # Copyright (C) 2023 CERN
 #
 # Invenio-RDM-Records is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Base parsing functions for the various serializers."""
-from marshmallow import Schema, fields, missing
 
+from marshmallow import missing
 
-class BaseSchema(Schema):
-    """BaseSchema for serializers in JSON."""
+
+class CommonFieldsMixin:
+    """Common fields serialization."""
 
     def get_doi(self, obj):
         """Get DOI."""
         if "doi" in obj["pids"]:
             return obj["pids"]["doi"]["identifier"]
 
         for identifier in obj["metadata"].get("identifiers", []):
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/ui/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/ui/fields.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/ui/fields.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/ui/schema.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/ui/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/resources/serializers/utils.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/resources/serializers/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/secret_links/errors.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/secret_links/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/secret_links/models.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/secret_links/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/secret_links/serializers.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/secret_links/serializers.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,26 +9,30 @@
 """High-level API for wokring with RDM records, files, pids and search."""
 from .community_records import CommunityRecordsService
 from .config import (
     RDMCommunityRecordsConfig,
     RDMFileDraftServiceConfig,
     RDMFileRecordServiceConfig,
     RDMRecordCommunitiesConfig,
+    RDMRecordRequestsConfig,
     RDMRecordServiceConfig,
 )
 from .iiif import IIIFService
 from .permissions import RDMRecordPermissionPolicy
+from .requests import RecordRequestsService
 from .secret_links import SecretLinkService
 from .services import RDMRecordService
 
 __all__ = (
     "IIIFService",
     "RDMFileDraftServiceConfig",
     "RDMFileRecordServiceConfig",
     "RDMRecordPermissionPolicy",
     "RDMRecordService",
     "RDMRecordServiceConfig",
     "SecretLinkService",
     "RDMRecordCommunitiesConfig",
     "RDMCommunityRecordsConfig",
     "CommunityRecordsService",
+    "RDMRecordRequestsConfig",
+    "RecordRequestsService",
 )
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/communities/components.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/communities/components.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,28 +3,26 @@
 # Copyright (C) 2023 CERN.
 #
 # Invenio-RDM-Records is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Record communities service components."""
 
-from invenio_communities.communities.records.systemfields.access import (
-    CommunityAccess,
-    VisibilityEnum,
-)
+from invenio_communities.communities.records.systemfields.access import VisibilityEnum
 from invenio_communities.communities.services.components import (
     CommunityAccessComponent as BaseAccessComponent,
 )
 from invenio_communities.communities.services.components import (
     CustomFieldsComponent,
     FeaturedCommunityComponent,
     OAISetComponent,
     OwnershipComponent,
     PIDComponent,
 )
+from invenio_i18n import lazy_gettext as _
 from invenio_records_resources.services.records.components import (
     MetadataComponent,
     RelationsComponent,
 )
 from invenio_search.engine import dsl
 
 from ...proxies import current_community_records_service
@@ -33,26 +31,22 @@
 
 class CommunityAccessComponent(BaseAccessComponent):
     """Community access component."""
 
     def _check_visibility(self, identity, record):
         """Checks if the visibility change is allowed."""
         if VisibilityEnum(record.access.visibility) == VisibilityEnum.RESTRICTED:
-            assert CommunityAccess.validate_visibility_level(VisibilityEnum.PUBLIC)
-
-            total = current_community_records_service.search(
+            count_public_records = current_community_records_service.search(
                 identity,
                 community_id=record.id,
-                extra_filter=dsl.Q(
-                    "term", **{"access.record": str(VisibilityEnum.PUBLIC)}
-                ),
+                extra_filter=dsl.Q("term", **{"access.record": "public"}),
             ).total
-            if total > 0:
+            if count_public_records > 0:
                 raise InvalidCommunityVisibility(
-                    reason="Cannot restrict a community with public records."
+                    reason=_("Cannot restrict a community with public records.")
                 )
 
     def update(self, identity, data=None, record=None, **kwargs):
         """Update handler."""
         old_visibility = record.get("access", {}).get("visibility")
         new_visibility = data.get("access", {}).get("visibility")
         check_visibility = old_visibility != new_visibility
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/communities/service.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/communities/service.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) 2023 CERN.
 #
 # Invenio-RDM-Records is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """RDM Record Communities Service."""
 
-from invenio_communities.communities.records.api import Community
 from invenio_communities.proxies import current_communities
 from invenio_i18n import lazy_gettext as _
 from invenio_pidstore.errors import PIDDoesNotExistError
 from invenio_records_resources.services import (
     RecordIndexerMixin,
     Service,
     ServiceSchemaWrapper,
@@ -28,15 +27,15 @@
 from invenio_search.engine import dsl
 from sqlalchemy.orm.exc import NoResultFound
 
 from invenio_rdm_records.proxies import current_rdm_records
 from invenio_rdm_records.requests import CommunityInclusion
 from invenio_rdm_records.services.errors import (
     CommunityAlreadyExists,
-    CommunityInclusionInconsistentAccessRestrictions,
+    InvalidAccessRestrictions,
     OpenRequestAlreadyExists,
     RecordCommunityMissing,
 )
 
 
 class RecordCommunitiesService(Service, RecordIndexerMixin):
     """Record communities service.
@@ -66,50 +65,53 @@
                     dsl.Q("term", **{"type": CommunityInclusion.type_id}),
                     dsl.Q("term", **{"is_open": True}),
                 ],
             ),
         )
         return next(results.hits)["id"] if results.total > 0 else None
 
-    def _include(self, identity, community_id, record, uow):
+    def _include(self, identity, community_id, comment, require_review, record, uow):
         """Create request to add the community to the record."""
-        already_included = community_id in record.parent.communities
-        if already_included:
-            raise CommunityAlreadyExists()
-
         # check if the community exists
         community = current_communities.service.record_cls.pid.resolve(community_id)
+        com_id = str(community.id)
+
+        already_included = com_id in record.parent.communities
+        if already_included:
+            raise CommunityAlreadyExists()
 
         # check if there is already an open request, to avoid duplications
-        existing_request_id = self._exists(identity, str(community.id), record)
+        existing_request_id = self._exists(identity, com_id, record)
         if existing_request_id:
             raise OpenRequestAlreadyExists(existing_request_id)
 
         type_ = current_request_type_registry.lookup(CommunityInclusion.type_id)
         receiver = ResolverRegistry.resolve_entity_proxy(
-            {"community": community_id}
+            {"community": com_id}
         ).resolve()
 
-        no_comments = {}  # empty `data` to avoid adding comments in the request
         request_item = current_requests_service.create(
             identity,
-            no_comments,
+            {},
             type_,
             receiver,
             topic=record,
             uow=uow,
         )
+
         # create review request
         request_item = current_rdm_records.community_inclusion_service.submit(
-            identity, record, community, request_item._request, no_comments, uow
+            identity, record, community, request_item._request, comment, uow
         )
         # include directly when allowed
-        return current_rdm_records.community_inclusion_service.include(
-            identity, community, request_item._request, uow
-        )
+        if not require_review:
+            request_item = current_rdm_records.community_inclusion_service.include(
+                identity, community, request_item._request, uow
+            )
+        return request_item
 
     @unit_of_work()
     def add(self, identity, id_, data, uow):
         """Include the record in the given communities."""
         valid_data, errors = self.schema.load(
             data,
             context={
@@ -119,48 +121,45 @@
             raise_errors=True,
         )
         communities = valid_data["communities"]
 
         record = self.record_cls.pid.resolve(id_)
         self.require_permission(identity, "add_community", record=record)
 
-        success = []
+        processed = []
         for community in communities:
             community_id = community["id"]
+            comment = community.get("comment", None)
+            require_review = community.get("require_review", False)
 
             result = {
-                "community": community_id,
+                "community_id": community_id,
             }
             try:
-                request_item = self._include(identity, community_id, record, uow)
-                result["request"] = str(request_item.data["id"])
-                success.append(result)
+                request_item = self._include(
+                    identity, community_id, comment, require_review, record, uow
+                )
+                result["request_id"] = str(request_item.data["id"])
+                result["request"] = request_item.to_dict()
+                processed.append(result)
             except (NoResultFound, PIDDoesNotExistError):
                 result["message"] = _("Community not found.")
                 errors.append(result)
-            except CommunityAlreadyExists:
-                result["message"] = _(
-                    "The record is already included in this community."
-                )
-                errors.append(result)
-            except OpenRequestAlreadyExists:
-                result["message"] = _(
-                    "There is already an open inclusion request for this community."
-                )
-                errors.append(result)
-            except CommunityInclusionInconsistentAccessRestrictions as ex:
-                result["message"] = ex.args[0]
-                errors.append(result)
-            except PermissionDeniedError:
-                result["message"] = _("Permission denied.")
+            except (
+                CommunityAlreadyExists,
+                OpenRequestAlreadyExists,
+                InvalidAccessRestrictions,
+                PermissionDeniedError,
+            ) as ex:
+                result["message"] = ex.description
                 errors.append(result)
 
         uow.register(IndexRefreshOp(indexer=self.indexer))
 
-        return dict(success=success, errors=errors)
+        return processed, errors
 
     def _remove(self, identity, community_id, record):
         """Remove a community from the record."""
         if community_id not in record.parent.communities.ids:
             raise RecordCommunityMissing(record.id, community_id)
 
         # check permission here, per community: curator cannot remove another community
@@ -181,38 +180,34 @@
             context={
                 "identity": identity,
                 "max_number": self.config.max_number_of_removals,
             },
             raise_errors=True,
         )
         communities = valid_data["communities"]
-
+        processed = []
         for community in communities:
             community_id = community["id"]
             try:
                 self._remove(identity, community_id, record)
-            except RecordCommunityMissing:
-                errors.append(
-                    {
-                        "community": community_id,
-                        "message": _("The record does not belong to the community."),
-                    }
-                )
-            except PermissionDeniedError:
+                processed.append({"community": community_id})
+            except (RecordCommunityMissing, PermissionDeniedError) as ex:
                 errors.append(
                     {
                         "community": community_id,
-                        "message": _("Permission denied."),
+                        "message": ex.description,
                     }
                 )
+        if processed:
+            uow.register(RecordCommitOp(record.parent))
+            uow.register(
+                RecordIndexOp(record, indexer=self.indexer, index_refresh=True)
+            )
 
-        uow.register(RecordCommitOp(record.parent))
-        uow.register(RecordIndexOp(record, indexer=self.indexer, index_refresh=True))
-
-        return errors
+        return processed, errors
 
     def search(
         self,
         identity,
         id_,
         params=None,
         search_preference=None,
@@ -231,9 +226,82 @@
 
         return current_communities.service.search(
             identity,
             params=params,
             search_preference=search_preference,
             expand=expand,
             extra_filter=communities_filter,
+            **kwargs
+        )
+
+    @staticmethod
+    def _get_excluded_communities_filter(record, identity, id_):
+        """Return filter to exclude communities that should not be suggested."""
+        communities_to_exclude = []
+        communities_ids = record.parent.communities.ids
+
+        for community_id in communities_ids:
+            communities_to_exclude.append(dsl.Q("term", **{"id": community_id}))
+
+        open_requests = current_requests_service.search(
+            identity,
+            extra_filter=dsl.query.Bool(
+                "must",
+                must=[
+                    dsl.Q("term", **{"topic.record": id_}),
+                    dsl.Q("term", **{"type": CommunityInclusion.type_id}),
+                    dsl.Q("term", **{"is_open": True}),
+                ],
+            ),
+        )
+
+        # the assumption here is that there should be only a few open requests,
+        # so requests.hits (first page one) should be enough
+        for request in open_requests.hits:
+            communities_to_exclude.append(
+                dsl.Q("term", **{"id": request["receiver"]["community"]})
+            )
+
+        exclusion_filter = dsl.query.Bool("must_not", must_not=communities_to_exclude)
+
+        return exclusion_filter
+
+    def search_suggested_communities(
+        self,
+        identity,
+        id_,
+        params=None,
+        search_preference=None,
+        expand=False,
+        by_membership=False,
+        extra_filter=None,
+        **kwargs
+    ):
+        """Search for communities that can be added to a record."""
+        record = self.record_cls.pid.resolve(id_)
+
+        self.require_permission(identity, "add_community", record=record)
+
+        communities_filter = self._get_excluded_communities_filter(
+            record, identity, id_
+        )
+
+        if extra_filter is not None:
+            communities_filter = communities_filter & extra_filter
+
+        if by_membership:
+            return current_communities.service.search_user_communities(
+                identity,
+                params=params,
+                search_preference=search_preference,
+                extra_filter=communities_filter,
+                **kwargs
+            )
+
+        return current_communities.service.search(
+            identity,
+            params=params,
+            search_preference=search_preference,
+            expand=expand,
+            extra_filter=communities_filter,
             **kwargs
         )
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/community_inclusion/service.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/community_inclusion/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,25 +6,22 @@
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Community Inclusion Service."""
 
 from flask import current_app
 from invenio_communities import current_communities
 from invenio_i18n import lazy_gettext as _
-from invenio_records_resources.services.errors import PermissionDeniedError
 from invenio_requests import current_requests_service
 
-from invenio_rdm_records.records.systemfields.access.field.record import (
-    AccessStatusEnum,
+from invenio_rdm_records.requests.community_inclusion import (
+    CommunityInclusion,
+    is_access_restriction_valid,
 )
-from invenio_rdm_records.requests.community_inclusion import CommunityInclusion
 from invenio_rdm_records.requests.community_submission import CommunitySubmission
-from invenio_rdm_records.services.errors import (
-    CommunityInclusionInconsistentAccessRestrictions,
-)
+from invenio_rdm_records.services.errors import InvalidAccessRestrictions
 
 
 class CommunityInclusionService:
     """Service for including a record in a community.
 
     The RDM Requests service wraps some operations of the generic requests service,
     implementing RDM business logic.
@@ -44,18 +41,17 @@
         """Submit a request to include a record in a community.
 
         It ensures that public records cannot be included in restricted communities.
         """
         if request.type.type_id not in self.supported_types:
             raise ValueError("Invalid request type.")
 
-        record_is_restricted = record.access.status == AccessStatusEnum.RESTRICTED
-
-        if community.access.visibility_is_restricted and not record_is_restricted:
-            raise CommunityInclusionInconsistentAccessRestrictions()
+        # validate record and community access
+        if not is_access_restriction_valid(record, community):
+            raise InvalidAccessRestrictions()
 
         # All other preconditions can be checked by the action itself which can
         # raise appropriate exceptions.
         return current_requests_service.execute_action(
             identity, request.id, "submit", data=data, uow=uow
         )
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/community_records/service.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/community_records/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             ),
             links_item_tpl=self.links_item_tpl,
         )
 
     def _remove(self, community, record, identity):
         """Remove a community from the record."""
         data = dict(communities=[dict(id=str(community.id))])
-        errors = current_record_communities_service.remove(
+        _, errors = current_record_communities_service.remove(
             identity, id_=record.pid.pid_value, data=data
         )
 
         return errors
 
     @unit_of_work()
     def delete(self, identity, community_id, data, revision_id=None, uow=None):
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/components/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/components/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/components/access.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/components/access.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/components/metadata.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/components/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/components/parent.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/components/parent.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/components/pids.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/components/pids.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/components/review.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/components/review.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/config.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,31 +42,34 @@
 from invenio_records_resources.services.records.config import (
     RecordServiceConfig as BaseRecordServiceConfig,
 )
 from invenio_records_resources.services.records.links import (
     RecordLink,
     pagination_links,
 )
+from invenio_requests.services.requests import RequestItem, RequestList
+from invenio_requests.services.requests.config import RequestSearchOptions
+from requests import Request
 
 from ..records import RDMDraft, RDMRecord
 from . import facets
 from .components import (
     AccessComponent,
     CustomFieldsComponent,
     MetadataComponent,
     PIDsComponent,
     ReviewComponent,
 )
 from .customizations import FromConfigPIDsProviders, FromConfigRequiredPIDs
 from .permissions import RDMRecordPermissionPolicy
 from .result_items import SecretLinkItem, SecretLinkList
 from .schemas import RDMParentSchema, RDMRecordSchema
-from .schemas.community_records import RecordCommunitiesSchema
+from .schemas.community_records import CommunityRecordsSchema
 from .schemas.parent.access import SecretLink
-from .schemas.record_communities import CommunityRecordsSchema
+from .schemas.record_communities import RecordCommunitiesSchema
 
 
 def is_draft_and_has_review(record, ctx):
     """Determine if submit review link should be included."""
     return is_draft(record, ctx) and record.parent.review is not None
 
 
@@ -137,24 +140,57 @@
 
     # Max n. communities that can be added at once
     max_number_of_additions = 10
     # Max n. communities that can be removed at once
     max_number_of_removals = 10
 
 
+class RDMRecordRequestsConfig(ServiceConfig, ConfiguratorMixin):
+    """Record community inclusion config."""
+
+    request_record_cls = RDMRecord
+    service_id = "record-requests"
+    permission_policy_cls = FromConfig(
+        "RDM_PERMISSION_POLICY", default=RDMRecordPermissionPolicy, import_string=True
+    )
+    result_item_cls = RequestItem
+    result_list_cls = RequestList
+    search = RequestSearchOptions
+
+    # request-specific configuration
+    record_cls = Request  # needed for model queries
+    schema = None  # stored in the API classes, for customization
+    indexer_queue_name = "requests"
+    index_dumper = None
+
+
 class RDMCommunityRecordsConfig(BaseRecordServiceConfig, ConfiguratorMixin):
     """Community records service config."""
 
     service_id = "community-records"
     record_cls = RDMRecord
     community_cls = Community
     permission_policy_cls = FromConfig(
         "RDM_PERMISSION_POLICY", default=RDMRecordPermissionPolicy, import_string=True
     )
 
+    # Search configuration
+    search = FromConfigSearchOptions(
+        "RDM_SEARCH",
+        "RDM_SORT_OPTIONS",
+        "RDM_FACETS",
+        search_option_cls=RDMSearchOptions,
+    )
+    search_versions = FromConfigSearchOptions(
+        "RDM_SEARCH_VERSIONING",
+        "RDM_SORT_OPTIONS",
+        "RDM_FACETS",
+        search_option_cls=RDMSearchVersionsOptions,
+    )
+
     # Service schemas
     community_record_schema = CommunityRecordsSchema
     schema = RDMRecordSchema
 
     # Max n. records that can be removed at once
     max_number_of_removals = 10
 
@@ -299,14 +335,18 @@
             when=is_draft_and_has_review,
         ),
         "versions": RecordLink("{+api}/records/{id}/versions"),
         "access_links": RecordLink("{+api}/records/{id}/access/links"),
         # TODO: only include link when DOI support is enabled.
         "reserve_doi": RecordLink("{+api}/records/{id}/draft/pids/doi"),
         "communities": RecordLink("{+api}/records/{id}/communities"),
+        "communities-suggestions": RecordLink(
+            "{+api}/records/{id}/communities-suggestions"
+        ),
+        "requests": RecordLink("{+api}/records/{id}/requests"),
     }
 
 
 class RDMFileRecordServiceConfig(FileServiceConfig, ConfiguratorMixin):
     """Configuration for record files."""
 
     record_cls = RDMRecord
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/customizations.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/customizations.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/errors.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/errors.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,27 +16,34 @@
 
 
 class EmbargoNotLiftedError(RDMRecordsException):
     """Embargo could not be lifted ."""
 
     def __init__(self, record_id):
         """Initialise error."""
-        super().__init__(f"Embargo could not be lifted for record: {record_id}")
+        self.record_id = record_id
+
+    @property
+    def description(self):
+        """Exception's description."""
+        return _(
+            "Embargo could not be lifted for record: {record_id}".format(
+                record_id=self.record_id
+            )
+        )
 
 
 class ReviewException(RDMRecordsException):
     """Base class for review errors."""
 
 
 class ReviewNotFoundError(ReviewException):
     """Review was not found for record/draft."""
 
-    def __init__(self, *args, **kwargs):
-        """Initialize exception."""
-        super().__init__(_("Review not found."), *args, **kwargs)
+    description = _("Review not found.")
 
 
 class ReviewStateError(ReviewException):
     """Review was not found for record/draft."""
 
 
 class ReviewExistsError(ReviewException):
@@ -46,38 +53,38 @@
 class CommunitySubmissionException(Exception):
     """Base exception for community submission requests."""
 
 
 class CommunityAlreadyExists(CommunitySubmissionException):
     """The record is already in the community."""
 
+    description = _("The record is already included in this community.")
+
 
 class CommunityInclusionException(Exception):
     """Base exception for community inclusion requests."""
 
 
-class CommunityInclusionInconsistentAccessRestrictions(CommunityInclusionException):
-    """Inclusion has inconsistent record vs community access restrictions."""
+class InvalidAccessRestrictions(CommunityInclusionException):
+    """Invalid access restrictions for record and community."""
 
-    def __init__(self, *args, **kwargs):
-        """Initialize exception."""
-        super().__init__(
-            _("A public record cannot be included in a restricted community."),
-            *args,
-            **kwargs,
-        )
+    description = _("A public record cannot be included in a restricted community.")
 
 
 class OpenRequestAlreadyExists(CommunitySubmissionException):
     """An open request already exists."""
 
     def __init__(self, request_id):
         """Initialize exception."""
         self.request_id = request_id
-        super().__init__()
+
+    @property
+    def description(self):
+        """Exception's description."""
+        return _("There is already an open inclusion request for this community.")
 
 
 class ValidationErrorWithMessageAsList(Exception):
     """Record Validation error where the messages are already a list.
 
     There is a large context around this to understand. Field errors are
     sent to the frontend by either:
@@ -116,40 +123,33 @@
         assert isinstance(message, list)
         self.messages = message
 
 
 class RecordCommunityMissing(Exception):
     """Record does not belong to the community."""
 
-    def __init__(self, record_id, communities_id):
+    def __init__(self, record_id, community_id):
         """Initialise error."""
-        super().__init__(
-            f"The record {record_id} does not belong to any of the listed communities {communities_id}."
-        )
-
+        self.record_id = record_id
+        self.community_id = community_id
 
-class MaxNumberCommunitiesExceeded(Exception):
-    """Maximum number of communities exceed."""
-
-    def __init__(self, allowed_number):
-        """Initialise error."""
-        super().__init__(
-            f"Exceeded maximum amount of communities that can be updated at once: {allowed_number}."
-        )
-
-
-class MaxNumberOfRecordsExceed(Exception):
-    """Maximum number of records exceed."""
-
-    def __init__(self, allowed_number):
-        """Initialise error."""
-        super().__init__(
-            f"Exceeded maximum amount of records that can be updated at once: {allowed_number}."
+    @property
+    def description(self):
+        """Exception description."""
+        return _(
+            "The record {record_id} in not included in the community {community_id}.".format(
+                record_id=self.record_id, community_id=self.community_id
+            )
         )
 
 
 class InvalidCommunityVisibility(Exception):
     """Community visibility does not match the content."""
 
     def __init__(self, reason):
         """Constructor."""
-        super().__init__(f"Cannot modify community visibility. {reason}")
+        self.reason = reason
+
+    @property
+    def description(self):
+        """Exception description."""
+        return _("Cannot modify community visibility: {reason}".format(self.reason))
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/facets.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/generators.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/iiif/service.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/iiif/service.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/permissions.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/permissions.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,22 @@
         RecordCommunitiesAction("view"),
     ]
 
     can_authenticated = [AuthenticatedUser(), SystemProcess()]
     can_all = [AnyUser(), SystemProcess()]
 
     #
+    # Miscellaneous
+    #
+    # Allow for querying of statistics
+    # - This is currently disabled because it's not needed and could potentially
+    #   open up surface for denial of service attacks
+    can_query_stats = [Disable()]
+
+    #
     #  Records
     #
     # Allow searching of records
     can_search = can_all
 
     # Allow reading metadata of a record
     can_read = [
@@ -144,15 +152,15 @@
     # Allow lifting a record or draft.
     can_lift_embargo = can_manage
 
     #
     # Record communities
     #
     # Who can add record to a community
-    can_add_community = [RecordOwners()]
+    can_add_community = [RecordOwners(), SystemProcess()]
     # Who can remove a community from a record
     can_remove_community = [
         RecordOwners(),
         CommunityCurators(),
         SystemProcess(),
     ]
     # Who can remove records from a community
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/manager.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/manager.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/providers/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/providers/base.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/providers/base.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/providers/datacite.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/providers/datacite.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/providers/external.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/providers/external.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/providers/oai.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/providers/oai.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/service.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/service.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/pids/tasks.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/pids/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/result_items.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/result_items.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/results.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/results.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/review/links.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/review/links.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/review/service.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/review/service.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2020-2021 CERN.
 # Copyright (C) 2020-2021 Northwestern University.
-# Copyright (C) 2021 TU Wien.
+# Copyright (C) 2021-2023 TU Wien.
 # Copyright (C) 2021-2023 Graz University of Technology.
 #
 # Invenio-RDM-Records is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """RDM record schemas."""
 
@@ -21,14 +21,15 @@
 from marshmallow_utils.permissions import FieldPermissionsMixin
 
 from .access import AccessSchema
 from .files import FilesSchema
 from .metadata import MetadataSchema
 from .parent import RDMParentSchema
 from .pids import PIDSchema
+from .stats import StatsSchema
 from .versions import VersionsSchema
 
 
 def validate_scheme(scheme):
     """Validate a PID scheme."""
     if scheme not in current_app.config["RDM_PERSISTENT_IDENTIFIERS"]:
         raise ValidationError(_("Invalid persistent identifier scheme."))
@@ -66,15 +67,15 @@
     # notes = fields.List(fields.Nested(InternalNoteSchema))
     revision = fields.Integer(dump_only=True)
     versions = NestedAttribute(VersionsSchema, dump_only=True)
     parent = NestedAttribute(RDMParentSchema)
     is_published = fields.Boolean(dump_only=True)
     status = fields.String(dump_only=True)
 
-    # stats = NestedAttribute(StatsSchema, dump_only=True)
+    stats = NestedAttribute(StatsSchema, dump_only=True)
     # schema_version = fields.Interger(dump_only=True)
 
     @post_dump
     def default_nested(self, data, many, **kwargs):
         """Serialize fields as empty dict for partial drafts.
 
         Cannot use marshmallow for Nested fields due to issue:
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/access.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/access.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/files.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/files.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/metadata.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/parent/__init__.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/parent/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/parent/access.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/parent/access.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/pids.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/pids.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/utils.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/schemas/versions.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/schemas/versions.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/secret_links/service.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/secret_links/service.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/services.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/services.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/services/tasks.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/services/tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,12 +20,10 @@
     """Lift expired embargos."""
     service = current_rdm_records.records_service
 
     records = service.scan_expired_embargos(system_identity)
     for record in records.hits:
         try:
             service.lift_embargo(_id=record["id"], identity=system_identity)
-        except EmbargoNotLiftedError:
-            current_app.logger.warning(
-                f"Embargo from record with id {record['id']} was not lifted"
-            )
+        except EmbargoNotLiftedError as ex:
+            current_app.logger.warning(ex.description)
             continue
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/templates/semantic-ui/imprint.html` & `invenio-rdm-records-3.0.0/invenio_rdm_records/templates/semantic-ui/imprint.html`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/templates/semantic-ui/journal.html` & `invenio-rdm-records-3.0.0/invenio_rdm_records/templates/semantic-ui/journal.html`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/templates/semantic-ui/meeting.html` & `invenio-rdm-records-3.0.0/invenio_rdm_records/templates/semantic-ui/meeting.html`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/af/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/af/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ar/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ar/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/bg/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/bg/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ca/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ca/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/cs/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/cs/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/da/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/da/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/de/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/de/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/el/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/el/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/es/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/es/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/et/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/et/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/fa/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/fa/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/fr/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/fr/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/gl/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/gl/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/hr/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/hr/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/hu/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/hu/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/it/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/it/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ja/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ja/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ka/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ka/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/lt/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/lt/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/messages.pot` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/no/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/no/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/pl/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/pl/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/pt/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/pt/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ro/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ro/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ru/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/ru/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/rw/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/rw/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/sk/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/sk/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/sv/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/sv/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/tr/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/tr/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/uk/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/uk/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-rdm-records-3.0.0/invenio_rdm_records/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/utils.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/views.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,19 @@
 def create_record_communities_bp(app):
     """Create record communities blueprint."""
     return app.extensions[
         "invenio-rdm-records"
     ].record_communities_resource.as_blueprint()
 
 
+def create_record_requests_bp(app):
+    """Create record communities blueprint."""
+    return app.extensions["invenio-rdm-records"].record_requests_resource.as_blueprint()
+
+
 def create_oaipmh_server_blueprint_from_app(app):
     """Create app blueprint."""
     return app.extensions["invenio-rdm-records"].oaipmh_server_resource.as_blueprint()
 
 
 def create_iiif_bp(app):
     """Create IIIF blueprint."""
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records/webpack.py` & `invenio-rdm-records-3.0.0/invenio_rdm_records/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records.egg-info/PKG-INFO` & `invenio-rdm-records-3.0.0/invenio_rdm_records.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-records
-Version: 2.9.0
+Version: 3.0.0
 Summary: InvenioRDM module for the communities feature.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-records
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2019 CERN.
@@ -66,14 +66,39 @@
             Invenio-RDM-Records is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 3.0.0 (released 2023-04-20)
+        
+        - usage statistics: refactor files structure
+        
+        Version 2.13.0 (released 2023-04-17)
+        
+        - serializers: added schema processors (custom fields)
+        - serializers: created dump and load mixins for custom fields
+        
+        Version 2.12.0 (released 2023-04-06)
+        
+        - api: add record community suggestion endpoint
+        
+        Version 2.11.0 (released 2023-03-30)
+        
+        - add usage statistics indexing (by system field)
+        - add sorting by most viewed to the config
+        - move statistics events from invenio-app-rdm
+        
+        Version 2.10.0 (released 2023-03-28)
+        
+        - add requests endpoint to the record
+        - dublincore: transform identifiers tu urls
+        - record service: update community records
+        
         Version 2.9.0 (released 2023-03-24)
         
         - communities: return ghost parent community when cannot be resolved
         - contrib: add journal and meeting sort options
         - contrib: updated custom fields UI widgets
         - custom_fields: rename CodeMeta to Software
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records.egg-info/SOURCES.txt` & `invenio-rdm-records-3.0.0/invenio_rdm_records.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -83,17 +83,19 @@
 invenio_rdm_records/contrib/__init__.py
 invenio_rdm_records/contrib/codemeta/__init__.py
 invenio_rdm_records/contrib/codemeta/custom_fields.py
 invenio_rdm_records/contrib/imprint/__init__.py
 invenio_rdm_records/contrib/imprint/custom_fields.py
 invenio_rdm_records/contrib/journal/__init__.py
 invenio_rdm_records/contrib/journal/custom_fields.py
+invenio_rdm_records/contrib/journal/processors.py
 invenio_rdm_records/contrib/journal/sort.py
 invenio_rdm_records/contrib/meeting/__init__.py
 invenio_rdm_records/contrib/meeting/custom_fields.py
+invenio_rdm_records/contrib/meeting/processors.py
 invenio_rdm_records/contrib/meeting/sort.py
 invenio_rdm_records/contrib/thesis/__init__.py
 invenio_rdm_records/contrib/thesis/custom_fields.py
 invenio_rdm_records/fixtures/__init__.py
 invenio_rdm_records/fixtures/communities.py
 invenio_rdm_records/fixtures/demo.py
 invenio_rdm_records/fixtures/fixture.py
@@ -139,14 +141,15 @@
 invenio_rdm_records/records/api.py
 invenio_rdm_records/records/models.py
 invenio_rdm_records/records/dumpers/__init__.py
 invenio_rdm_records/records/dumpers/access.py
 invenio_rdm_records/records/dumpers/edtf.py
 invenio_rdm_records/records/dumpers/locations.py
 invenio_rdm_records/records/dumpers/pids.py
+invenio_rdm_records/records/dumpers/statistics.py
 invenio_rdm_records/records/jsonschemas/__init__.py
 invenio_rdm_records/records/jsonschemas/records/definitions-v1.0.0.json
 invenio_rdm_records/records/jsonschemas/records/definitions-v1.1.0.json
 invenio_rdm_records/records/jsonschemas/records/definitions-v1.2.0.json
 invenio_rdm_records/records/jsonschemas/records/definitions-v2.0.0.json
 invenio_rdm_records/records/jsonschemas/records/parent-v1.0.0.json
 invenio_rdm_records/records/jsonschemas/records/parent-v2.0.0.json
@@ -178,17 +181,51 @@
 invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v3.0.0.json
 invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v4.0.0.json
 invenio_rdm_records/records/mappings/v7/rdmrecords/drafts/draft-v5.0.0.json
 invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v2.0.0.json
 invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v3.0.0.json
 invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v4.0.0.json
 invenio_rdm_records/records/mappings/v7/rdmrecords/records/record-v5.0.0.json
+invenio_rdm_records/records/stats/__init__.py
+invenio_rdm_records/records/stats/api.py
+invenio_rdm_records/records/stats/templates/__init__.py
+invenio_rdm_records/records/stats/templates/aggregations/__init__.py
+invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/__init__.py
+invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/os-v1/__init__.py
+invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/os-v1/aggr-file-download-v1.0.0.json
+invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/os-v2/__init__.py
+invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/os-v2/aggr-file-download-v1.0.0.json
+invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/v7/__init__.py
+invenio_rdm_records/records/stats/templates/aggregations/aggr_file_download/v7/aggr-file-download-v1.0.0.json
+invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/__init__.py
+invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/os-v1/__init__.py
+invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/os-v1/aggr-record-view-v1.0.0.json
+invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/os-v2/__init__.py
+invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/os-v2/aggr-record-view-v1.0.0.json
+invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/v7/__init__.py
+invenio_rdm_records/records/stats/templates/aggregations/aggr_record_view/v7/aggr-record-view-v1.0.0.json
+invenio_rdm_records/records/stats/templates/events/__init__.py
+invenio_rdm_records/records/stats/templates/events/file_download/__init__.py
+invenio_rdm_records/records/stats/templates/events/file_download/os-v1/__init__.py
+invenio_rdm_records/records/stats/templates/events/file_download/os-v1/file-download-v1.0.0.json
+invenio_rdm_records/records/stats/templates/events/file_download/os-v2/__init__.py
+invenio_rdm_records/records/stats/templates/events/file_download/os-v2/file-download-v1.0.0.json
+invenio_rdm_records/records/stats/templates/events/file_download/v7/__init__.py
+invenio_rdm_records/records/stats/templates/events/file_download/v7/file-download-v1.0.0.json
+invenio_rdm_records/records/stats/templates/events/record_view/__init__.py
+invenio_rdm_records/records/stats/templates/events/record_view/os-v1/__init__.py
+invenio_rdm_records/records/stats/templates/events/record_view/os-v1/record-view-v1.0.0.json
+invenio_rdm_records/records/stats/templates/events/record_view/os-v2/__init__.py
+invenio_rdm_records/records/stats/templates/events/record_view/os-v2/record-view-v1.0.0.json
+invenio_rdm_records/records/stats/templates/events/record_view/v7/__init__.py
+invenio_rdm_records/records/stats/templates/events/record_view/v7/record-view-v1.0.0.json
 invenio_rdm_records/records/systemfields/__init__.py
 invenio_rdm_records/records/systemfields/draft_status.py
 invenio_rdm_records/records/systemfields/has_draftcheck.py
+invenio_rdm_records/records/systemfields/statistics.py
 invenio_rdm_records/records/systemfields/access/__init__.py
 invenio_rdm_records/records/systemfields/access/embargo.py
 invenio_rdm_records/records/systemfields/access/grants.py
 invenio_rdm_records/records/systemfields/access/links.py
 invenio_rdm_records/records/systemfields/access/owners.py
 invenio_rdm_records/records/systemfields/access/protection.py
 invenio_rdm_records/records/systemfields/access/field/__init__.py
@@ -229,14 +266,16 @@
 invenio_rdm_records/resources/serializers/iiif/__init__.py
 invenio_rdm_records/resources/serializers/iiif/schema.py
 invenio_rdm_records/resources/serializers/marcxml/__init__.py
 invenio_rdm_records/resources/serializers/marcxml/schema.py
 invenio_rdm_records/resources/serializers/ui/__init__.py
 invenio_rdm_records/resources/serializers/ui/fields.py
 invenio_rdm_records/resources/serializers/ui/schema.py
+invenio_rdm_records/resources/stats/__init__.py
+invenio_rdm_records/resources/stats/event_builders.py
 invenio_rdm_records/secret_links/__init__.py
 invenio_rdm_records/secret_links/errors.py
 invenio_rdm_records/secret_links/models.py
 invenio_rdm_records/secret_links/permissions.py
 invenio_rdm_records/secret_links/serializers.py
 invenio_rdm_records/secret_links/signals.py
 invenio_rdm_records/services/__init__.py
@@ -272,14 +311,16 @@
 invenio_rdm_records/services/pids/service.py
 invenio_rdm_records/services/pids/tasks.py
 invenio_rdm_records/services/pids/providers/__init__.py
 invenio_rdm_records/services/pids/providers/base.py
 invenio_rdm_records/services/pids/providers/datacite.py
 invenio_rdm_records/services/pids/providers/external.py
 invenio_rdm_records/services/pids/providers/oai.py
+invenio_rdm_records/services/requests/__init__.py
+invenio_rdm_records/services/requests/service.py
 invenio_rdm_records/services/review/__init__.py
 invenio_rdm_records/services/review/links.py
 invenio_rdm_records/services/review/service.py
 invenio_rdm_records/services/schemas/__init__.py
 invenio_rdm_records/services/schemas/access.py
 invenio_rdm_records/services/schemas/community_records.py
 invenio_rdm_records/services/schemas/files.py
@@ -290,14 +331,16 @@
 invenio_rdm_records/services/schemas/utils.py
 invenio_rdm_records/services/schemas/versions.py
 invenio_rdm_records/services/schemas/parent/__init__.py
 invenio_rdm_records/services/schemas/parent/access.py
 invenio_rdm_records/services/schemas/parent/communities.py
 invenio_rdm_records/services/secret_links/__init__.py
 invenio_rdm_records/services/secret_links/service.py
+invenio_rdm_records/services/stats/__init__.py
+invenio_rdm_records/services/stats/permissions.py
 invenio_rdm_records/templates/semantic-ui/imprint.html
 invenio_rdm_records/templates/semantic-ui/journal.html
 invenio_rdm_records/templates/semantic-ui/meeting.html
 invenio_rdm_records/templates/semantic-ui/invenio_rdm_records/oai-details.html
 invenio_rdm_records/templates/semantic-ui/invenio_rdm_records/oai-search.html
 invenio_rdm_records/translations/messages.pot
 invenio_rdm_records/translations/af/LC_MESSAGES/messages.mo
@@ -439,14 +482,15 @@
 tests/resources/test_publish_errors.py
 tests/resources/test_record_file_permissions.py
 tests/resources/test_resources.py
 tests/resources/test_resources_communities.py
 tests/resources/test_resources_community_records.py
 tests/resources/test_resources_oai.py
 tests/resources/test_resources_pids.py
+tests/resources/test_resources_record_communities.py
 tests/resources/test_resources_review.py
 tests/resources/test_rocrate.py
 tests/resources/test_serialized_links.py
 tests/resources/serializers/test_bibtex_serializer.py
 tests/resources/serializers/test_csl_serializer.py
 tests/resources/serializers/test_datacite_serializer.py
 tests/resources/serializers/test_dcat_serializer.py
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records.egg-info/entry_points.txt` & `invenio-rdm-records-3.0.0/invenio_rdm_records.egg-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 invenio_rdm_records = invenio_rdm_records:InvenioRDMRecords
 
 [invenio_base.api_blueprints]
 invenio_iiif = invenio_rdm_records.views:create_iiif_bp
 invenio_oaipmh_server = invenio_rdm_records.views:create_oaipmh_server_blueprint_from_app
 invenio_rdm_community_records = invenio_rdm_records.views:create_community_records_bp
 invenio_rdm_record_communities = invenio_rdm_records.views:create_record_communities_bp
+invenio_rdm_record_requests = invenio_rdm_records.views:create_record_requests_bp
 invenio_rdm_records = invenio_rdm_records.views:create_records_bp
 invenio_rdm_records_draft_files = invenio_rdm_records.views:create_draft_files_bp
 invenio_rdm_records_ext = invenio_rdm_records.views:blueprint
 invenio_rdm_records_parent_links = invenio_rdm_records.views:create_parent_record_links_bp
 invenio_rdm_records_record_files = invenio_rdm_records.views:create_record_files_bp
 
 [invenio_base.apps]
```

### Comparing `invenio-rdm-records-2.9.0/invenio_rdm_records.egg-info/requires.txt` & `invenio-rdm-records-3.0.0/invenio_rdm_records.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/run-tests.sh` & `invenio-rdm-records-3.0.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/setup.cfg` & `invenio-rdm-records-3.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 	invenio_rdm_records_draft_files = invenio_rdm_records.views:create_draft_files_bp
 	invenio_rdm_records_ext = invenio_rdm_records.views:blueprint
 	invenio_rdm_records_parent_links = invenio_rdm_records.views:create_parent_record_links_bp
 	invenio_rdm_records_record_files = invenio_rdm_records.views:create_record_files_bp
 	invenio_rdm_community_records = invenio_rdm_records.views:create_community_records_bp
 	invenio_oaipmh_server = invenio_rdm_records.views:create_oaipmh_server_blueprint_from_app
 	invenio_rdm_record_communities = invenio_rdm_records.views:create_record_communities_bp
+	invenio_rdm_record_requests = invenio_rdm_records.views:create_record_requests_bp
 	invenio_iiif = invenio_rdm_records.views:create_iiif_bp
 invenio_base.blueprints = 
 	invenio_rdm_records_ext = invenio_rdm_records.views:blueprint
 invenio_celery.tasks = 
 	invenio_rdm_records_fixtures = invenio_rdm_records.fixtures.tasks
 	invenio_rdm_records_services = invenio_rdm_records.services.tasks
 invenio_db.models =
```

### Comparing `invenio-rdm-records-2.9.0/tests/conftest.py` & `invenio-rdm-records-3.0.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 from invenio_vocabularies.contrib.awards.api import Award
 from invenio_vocabularies.contrib.funders.api import Funder
 from invenio_vocabularies.contrib.subjects.api import Subject
 from invenio_vocabularies.proxies import current_service as vocabulary_service
 from invenio_vocabularies.records.api import Vocabulary
 
 from invenio_rdm_records import config
-from invenio_rdm_records.proxies import current_rdm_records
+from invenio_rdm_records.proxies import current_rdm_records_service
 from invenio_rdm_records.records.api import RDMDraft, RDMParent, RDMRecord
 from invenio_rdm_records.services.communities.components import (
     CommunityServiceComponents,
 )
 from invenio_rdm_records.services.pids import providers
 
 from .fake_datacite_client import FakeDataCiteClient
@@ -496,22 +496,14 @@
                 {
                     "reference": "Nielsen et al,..",
                     "identifier": "0000 0001 1456 7559",
                     "scheme": "isni",
                 }
             ],
         },
-        "ext": {
-            "dwc": {
-                "collectionCode": "abc",
-                "collectionCode2": 1.1,
-                "collectionCode3": True,
-                "test": ["abc", 1, True],
-            }
-        },
         "provenance": {
             "created_by": {"user": users[0].id},
             "on_behalf_of": {"user": users[1].id},
         },
         "access": {
             "record": "public",
             "files": "restricted",
@@ -768,22 +760,14 @@
                 {
                     "reference": "Nielsen et al,..",
                     "identifier": "0000 0001 1456 7559",
                     "scheme": "isni",
                 }
             ],
         },
-        "ext": {
-            "dwc": {
-                "collectionCode": "abc",
-                "collectionCode2": 1.1,
-                "collectionCode3": True,
-                "test": ["abc", 1, True],
-            }
-        },
         "provenance": {
             "created_by": {"user": users[0].id},
             "on_behalf_of": {"user": users[1].id},
         },
         "access": {
             "record": "public",
             "files": "restricted",
@@ -1528,15 +1512,15 @@
 
     return action_role.need
 
 
 @pytest.fixture()
 def embargoed_record(running_app, minimal_record, superuser_identity):
     """Embargoed record."""
-    service = current_rdm_records.records_service
+    service = current_rdm_records_service
     today = arrow.utcnow().date().isoformat()
 
     # Add embargo to record
     with mock.patch("arrow.utcnow") as mock_arrow:
         minimal_record["access"]["files"] = "restricted"
         minimal_record["access"]["status"] = "embargoed"
         minimal_record["access"]["embargo"] = dict(
@@ -1694,42 +1678,46 @@
     )
 
 
 @pytest.fixture()
 def closed_review_community(
     running_app, community_type_record, community_owner, closed_review_minimal_community
 ):
-    """Create community with open review policy i.e allow direct publishes."""
+    """Create community with close review policy i.e allow direct publishes."""
     return _community_get_or_create(
         closed_review_minimal_community, community_owner.identity
     )
 
 
 @pytest.fixture()
-def record_community(db, uploader, minimal_record, community, rdm_record_service):
+def record_community(db, uploader, minimal_record, community):
     """Creates a record that belongs to a community."""
 
     class Record:
         """Test record class."""
 
         def create_record(
             self, record_dict=minimal_record, uploader=uploader, community=community
         ):
             """Creates new record that belongs to the same community."""
             # create draft
             community_record = community._record
-            draft = rdm_record_service.create(uploader.identity, record_dict)
+            draft = current_rdm_records_service.create(uploader.identity, record_dict)
             # publish and get record
-            result_item = rdm_record_service.publish(uploader.identity, draft.id)
+            result_item = current_rdm_records_service.publish(
+                uploader.identity, draft.id
+            )
             record = result_item._record
             # add the record to the community
             record.parent.communities.add(community_record, default=False)
             record.parent.commit()
             db.session.commit()
-            rdm_record_service.indexer.index(record, arguments={"refresh": True})
+            current_rdm_records_service.indexer.index(
+                record, arguments={"refresh": True}
+            )
             return record
 
     return Record()
 
 
 @pytest.fixture(scope="session")
 def headers():
```

### Comparing `invenio-rdm-records-2.9.0/tests/contrib/codemeta/conftest.py` & `invenio-rdm-records-3.0.0/tests/contrib/codemeta/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/contrib/codemeta/test_codemeta_custom_fields.py` & `invenio-rdm-records-3.0.0/tests/contrib/codemeta/test_codemeta_custom_fields.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/fake_datacite_client.py` & `invenio-rdm-records-3.0.0/tests/fake_datacite_client.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/fixtures/app_data/img/community1.png` & `invenio-rdm-records-3.0.0/tests/fixtures/app_data/img/community1.png`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/fixtures/app_data/records.yaml` & `invenio-rdm-records-3.0.0/tests/fixtures/app_data/records.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/fixtures/app_data/vocabularies/resource_types.yaml` & `invenio-rdm-records-3.0.0/tests/fixtures/app_data/vocabularies/resource_types.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/fixtures/app_data/vocabularies.alt.yaml` & `invenio-rdm-records-3.0.0/tests/fixtures/app_data/vocabularies.alt.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/fixtures/app_data/vocabularies.yaml` & `invenio-rdm-records-3.0.0/tests/fixtures/app_data/vocabularies.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/fixtures/conftest.py` & `invenio-rdm-records-3.0.0/tests/fixtures/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/fixtures/data/vocabularies/resource_types.yaml` & `invenio-rdm-records-3.0.0/tests/fixtures/data/vocabularies/resource_types.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/fixtures/data/vocabularies.yaml` & `invenio-rdm-records-3.0.0/tests/fixtures/data/vocabularies.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/fixtures/load_error/conflicting_module_B/fixtures/vocabularies/vocabularies.yaml` & `invenio-rdm-records-3.0.0/tests/fixtures/load_error/conflicting_module_B/fixtures/vocabularies/vocabularies.yaml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/fixtures/load_error/conftest.py` & `invenio-rdm-records-3.0.0/tests/fixtures/load_error/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/fixtures/load_error/test_vocabularies_load_error.py` & `invenio-rdm-records-3.0.0/tests/fixtures/load_error/test_vocabularies_load_error.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/fixtures/test_cli.py` & `invenio-rdm-records-3.0.0/tests/fixtures/test_cli.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/fixtures/test_fixtures.py` & `invenio-rdm-records-3.0.0/tests/fixtures/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/helpers.py` & `invenio-rdm-records-3.0.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/conftest.py` & `invenio-rdm-records-3.0.0/tests/records/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/dumpers/test_access_dumpers.py` & `invenio-rdm-records-3.0.0/tests/records/dumpers/test_access_dumpers.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/dumpers/test_edtf_dumpers.py` & `invenio-rdm-records-3.0.0/tests/records/dumpers/test_edtf_dumpers.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/dumpers/test_location_dumpers.py` & `invenio-rdm-records-3.0.0/tests/records/dumpers/test_location_dumpers.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/dumpers/test_pids_dumper.py` & `invenio-rdm-records-3.0.0/tests/records/dumpers/test_pids_dumper.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/full-record.json` & `invenio-rdm-records-3.0.0/tests/records/full-record.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/systemfields/test_access_systemfield.py` & `invenio-rdm-records-3.0.0/tests/records/systemfields/test_access_systemfield.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/test_api.py` & `invenio-rdm-records-3.0.0/tests/records/test_api.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/test_jsonschema.py` & `invenio-rdm-records-3.0.0/tests/records/test_jsonschema.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/test_records_communities.py` & `invenio-rdm-records-3.0.0/tests/records/test_records_communities.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/test_relations_affiliations.py` & `invenio-rdm-records-3.0.0/tests/records/test_relations_affiliations.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/test_relations_languages.py` & `invenio-rdm-records-3.0.0/tests/records/test_relations_languages.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/test_relations_resource_types.py` & `invenio-rdm-records-3.0.0/tests/records/test_relations_resource_types.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/test_relations_subjects.py` & `invenio-rdm-records-3.0.0/tests/records/test_relations_subjects.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/records/tombstone.json` & `invenio-rdm-records-3.0.0/tests/records/tombstone.json`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/conftest.py` & `invenio-rdm-records-3.0.0/tests/secret_links/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,21 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020 CERN.
-# Copyright (C) 2020 Northwestern University.
 # Copyright (C) 2021 TU Wien.
 #
 # Invenio-RDM-Records is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Pytest configuration.
 
 See https://pytest-invenio.readthedocs.io/ for documentation on which test
 fixtures are available.
 """
 
 import pytest
 from invenio_app.factory import create_api
 
-from invenio_rdm_records.proxies import current_rdm_records_service
-
 
 @pytest.fixture(scope="module")
 def create_app(instance_path):
     """Application factory fixture."""
     return create_api
-
-
-@pytest.fixture()
-def rdm_record_service():
-    """Get the current RDM records service."""
-    return current_rdm_records_service
-
-
-def link(url):
-    """Strip the host part of a link."""
-    api_prefix = "https://127.0.0.1:5000/api"
-    if url.startswith(api_prefix):
-        return url[len(api_prefix) :]
```

### Comparing `invenio-rdm-records-2.9.0/tests/resources/serializers/test_bibtex_serializer.py` & `invenio-rdm-records-3.0.0/tests/resources/serializers/test_bibtex_serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/serializers/test_csl_serializer.py` & `invenio-rdm-records-3.0.0/tests/resources/serializers/test_csl_serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/serializers/test_datacite_serializer.py` & `invenio-rdm-records-3.0.0/tests/resources/serializers/test_datacite_serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/serializers/test_dcat_serializer.py` & `invenio-rdm-records-3.0.0/tests/resources/serializers/test_dcat_serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/serializers/test_dublincore_serializer.py` & `invenio-rdm-records-3.0.0/tests/resources/serializers/test_dublincore_serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,25 +37,25 @@
 
 
 def test_dublincorejson_serializer(running_app, updated_full_record):
     """Test serializer to Dublin Core JSON"""
     expected_data = {
         "contributors": ["Nielsen, Lars Holm"],
         "types": ["info:eu-repo/semantic/other"],
-        "relations": ["doi:10.1234/foo.bar"],
+        "relations": ["https://doi.org/10.1234/foo.bar"],
         "descriptions": ["A description \nwith HTML tags", "Bla bla bla"],
         "publishers": ["InvenioRDM"],
         "languages": ["dan", "eng"],
         "locations": [
             "name=test location place; description=test location description; lat=-32.94682; lon=-60.63932"
         ],
         "identifiers": [
-            "1924MNRAS..84..308E",
-            "10.5281/inveniordm.1234",
+            "https://doi.org/10.5281/inveniordm.1234",
             "oai:vvv.com:abcde-fghij",
+            "bibcode:1924MNRAS..84..308E",
         ],
         "formats": ["application/pdf"],
         "titles": ["InvenioRDM"],
         "creators": ["Nielsen, Lars Holm"],
         "subjects": ["custom"],
         "dates": ["2018/2020-09", "info:eu-repo/date/embargoEnd/2131-01-01"],
         "rights": [
@@ -104,27 +104,26 @@
         "<dc:contributor>Nielsen, Lars Holm</dc:contributor>",
         "<dc:creator>Nielsen, Lars Holm</dc:creator>",
         "<dc:date>2018/2020-09</dc:date>",
         "<dc:date>info:eu-repo/date/embargoEnd/2131-01-01</dc:date>",
         "<dc:description>A description \nwith HTML tags</dc:description>",
         "<dc:description>Bla bla bla</dc:description>",
         "<dc:format>application/pdf</dc:format>",
-        "<dc:identifier>1924MNRAS..84..308E</dc:identifier>",
-        "<dc:identifier>10.5281/inveniordm.1234</dc:identifier>",
+        "<dc:identifier>https://doi.org/10.5281/inveniordm.1234</dc:identifier>",
         "<dc:identifier>oai:vvv.com:abcde-fghij</dc:identifier>",
+        "<dc:identifier>bibcode:1924MNRAS..84..308E</dc:identifier>",
         "<dc:language>dan</dc:language>",
         "<dc:language>eng</dc:language>",
         "<dc:publisher>InvenioRDM</dc:publisher>",
-        "<dc:relation>doi:10.1234/foo.bar</dc:relation>",
+        "<dc:relation>https://doi.org/10.1234/foo.bar</dc:relation>",
         "<dc:rights>info:eu-repo/semantics/embargoedAccess</dc:rights>",
         "<dc:rights>A custom license</dc:rights>",
         "<dc:rights>https://customlicense.org/licenses/by/4.0/</dc:rights>",
         "<dc:rights>Creative Commons Attribution 4.0 " + "International</dc:rights>",
-        "<dc:rights>https://creativecommons.org/licenses/by/4.0/legalcode"
-        + "</dc:rights>",
+        "<dc:rights>https://creativecommons.org/licenses/by/4.0/legalcode</dc:rights>",
         "<dc:title>InvenioRDM</dc:title>",
         "<dc:type>info:eu-repo/semantic/other</dc:type>",
     ]
 
     serializer = DublinCoreXMLSerializer()
     serialized_record = serializer.serialize_object(updated_full_record)
 
@@ -157,26 +156,25 @@
         "<dc:contributor>Nielsen, Lars Holm</dc:contributor>",
         "<dc:creator>Nielsen, Lars Holm</dc:creator>",
         "<dc:date>2018/2020-09</dc:date>",
         "<dc:date>info:eu-repo/date/embargoEnd/2131-01-01</dc:date>",
         "<dc:description>A description \nwith HTML tags</dc:description>",
         "<dc:description>Bla bla bla</dc:description>",
         "<dc:format>application/pdf</dc:format>",
-        "<dc:identifier>1924MNRAS..84..308E</dc:identifier>",
-        "<dc:identifier>10.5281/inveniordm.1234</dc:identifier>",
+        "<dc:identifier>https://doi.org/10.5281/inveniordm.1234</dc:identifier>",
+        "<dc:identifier>bibcode:1924MNRAS..84..308E</dc:identifier>",
         "<dc:language>dan</dc:language>",
         "<dc:language>eng</dc:language>",
         "<dc:publisher>InvenioRDM</dc:publisher>",
-        "<dc:relation>doi:10.1234/foo.bar</dc:relation>",
+        "<dc:relation>https://doi.org/10.1234/foo.bar</dc:relation>",
         "<dc:rights>info:eu-repo/semantics/embargoedAccess</dc:rights>",
         "<dc:rights>A custom license</dc:rights>",
         "<dc:rights>https://customlicense.org/licenses/by/4.0/</dc:rights>",
         "<dc:rights>Creative Commons Attribution 4.0 " + "International</dc:rights>",
-        "<dc:rights>https://creativecommons.org/licenses/by/4.0/legalcode"
-        + "</dc:rights>",
+        "<dc:rights>https://creativecommons.org/licenses/by/4.0/legalcode</dc:rights>",
         "<dc:title>InvenioRDM</dc:title>",
         "<dc:type>info:eu-repo/semantic/other</dc:type>",
     ]
 
     expected_data_minimal = [
         "<dc:creator>Name</dc:creator>",
         "<dc:creator>Troy Inc.</dc:creator>",
```

### Comparing `invenio-rdm-records-2.9.0/tests/resources/serializers/test_geojson_serializer.py` & `invenio-rdm-records-3.0.0/tests/resources/serializers/test_geojson_serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/serializers/test_marcxml_serializer.py` & `invenio-rdm-records-3.0.0/tests/resources/serializers/test_marcxml_serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/serializers/test_ui_serializer.py` & `invenio-rdm-records-3.0.0/tests/resources/serializers/test_ui_serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/test_draft_file_permissions.py` & `invenio-rdm-records-3.0.0/tests/resources/test_draft_file_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/test_iiif_image_api.py` & `invenio-rdm-records-3.0.0/tests/resources/test_iiif_image_api.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/test_iiif_presentation_api.py` & `invenio-rdm-records-3.0.0/tests/resources/test_iiif_presentation_api.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/test_publish_errors.py` & `invenio-rdm-records-3.0.0/tests/resources/test_publish_errors.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/test_record_file_permissions.py` & `invenio-rdm-records-3.0.0/tests/resources/test_record_file_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/test_resources.py` & `invenio-rdm-records-3.0.0/tests/resources/test_resources.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/test_resources_communities.py` & `invenio-rdm-records-3.0.0/tests/resources/test_resources_community_records.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,108 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2023 CERN.
 #
 # Invenio-RDM-Records is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
-"""Tests record's communities resources."""
+"""Tests community records resources."""
+import pytest
 
-from invenio_rdm_records.proxies import current_record_communities_service
+from invenio_rdm_records.proxies import current_community_records_service
 
 
-def test_remove_community(client, uploader, record_community, headers, community):
-    """Test removal of a community from the record."""
-    client = uploader.login(client)
+@pytest.fixture()
+def service():
+    """Get the current community records service."""
+    return current_community_records_service
 
-    data = {"communities": [{"id": community.id}]}
+
+def test_remove_community(client, curator, record_community, headers, community):
+    """Remove a record from the community."""
+    client = curator.login(client)
     record = record_community.create_record()
+    data = {"records": [{"id": record.pid.pid_value}]}
+
     response = client.delete(
-        f"/records/{record.pid.pid_value}/communities",
+        f"/communities/{community.id}/records",
         headers=headers,
         json=data,
     )
     assert response.status_code == 200
     assert not response.json.get("errors")
-    record_saved = client.get(f"/records/{record.pid.pid_value}", headers=headers)
-    assert not record_saved.json["parent"]["communities"]
 
 
 def test_permission_denied(
     client, uploader, test_user, record_community, headers, community
 ):
-    """Test remove of a community from the record by an unauthorized user."""
-    data = {"communities": [{"id": community.id}]}
+    """Missing permissions when removing a record from the community."""
+    record = record_community.create_record()
+    data = {"records": [{"id": record.pid.pid_value}]}
 
     test_user_client = test_user.login(client)
-    record = record_community.create_record()
 
-    response = test_user_client.delete(
-        f"/records/{record.pid.pid_value}/communities",
+    response_403 = test_user_client.delete(
+        f"/communities/{community.id}/records",
         headers=headers,
         json=data,
     )
-    assert response.status_code == 200
-    assert len(response.json["errors"]) == 1
-    record_saved = client.get(f"/records/{record.pid.pid_value}", headers=headers)
-    assert record_saved.json["parent"]["communities"] == {"ids": [str(community.id)]}
+    assert response_403.status_code == 403
 
 
-def test_error_data(client, uploader, record_community, headers, community):
-    """Test remove of a non-existing community from the record."""
-    data = {"communities": [{"id": "wrong-id"}]}
+def test_error_data(client, curator, headers, community):
+    """Remove a wrong record from the community."""
+    data = {"records": [{"id": "wrong-id"}]}
 
-    uploader_client = uploader.login(client)
-    record = record_community.create_record()
+    uploader_client = curator.login(client)
 
     response = uploader_client.delete(
-        f"/records/{record.pid.pid_value}/communities",
+        f"/communities/{community.id}/records",
         headers=headers,
         json=data,
     )
     assert response.status_code == 200
-    assert len(response.json["errors"]) == 1
-    record_saved = client.get(f"/records/{record.pid.pid_value}", headers=headers)
-    assert record_saved.json["parent"]["communities"] == {"ids": [str(community.id)]}
+    assert response.json["errors"]
 
 
-def test_exceeded_max_number_of_communities(
-    client, uploader, record_community, headers, community
+def test_removal_of_multiple_communities_success(
+    client, curator, record_community, headers, community
 ):
-    """Test raise exceeded max number of communities."""
-    client = uploader.login(client)
-    record = record_community.create_record()
+    """Remove multiple records from a community."""
+    client = curator.login(client)
+    record1 = record_community.create_record()
+    record2 = record_community.create_record()
+    record3 = record_community.create_record()
+    data = {
+        "records": [
+            {"id": record1.pid.pid_value},
+            {"id": record2.pid.pid_value},
+            {"id": record3.pid.pid_value},
+        ]
+    }
 
-    random_community = {"id": "random-id"}
-    lots_of_communities = []
-    while (
-        len(lots_of_communities)
-        <= current_record_communities_service.config.max_number_of_removals
-    ):
-        lots_of_communities.append(random_community)
-    data = {"communities": lots_of_communities}
     response = client.delete(
-        f"/records/{record.pid.pid_value}/communities",
+        f"/communities/{community.id}/records",
         headers=headers,
         json=data,
     )
-    assert response.status_code == 400
+    assert response.status_code == 200
+    assert not response.json.get("errors")
+
 
+def test_exceeded_max_number_of_records(
+    client, curator, record_community, headers, community, service
+):
+    """Test raise exceeded max number of records."""
+    client = curator.login(client)
+    random_record = {"id": "random-id"}
+    lots_of_records = []
+    while len(lots_of_records) <= service.config.max_number_of_removals:
+        lots_of_records.append(random_record)
 
-# TODO once upload to multiple communities is implemented
-def test_removal_of_multiple_communities():
-    """Remove multiple communities from a record."""
-    pass
+    data = {"records": lots_of_records}
+    response = client.delete(
+        f"/communities/{community.id}/records",
+        headers=headers,
+        json=data,
+    )
+    assert response.status_code == 400
```

### Comparing `invenio-rdm-records-2.9.0/tests/resources/test_resources_oai.py` & `invenio-rdm-records-3.0.0/tests/resources/test_resources_oai.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/test_resources_pids.py` & `invenio-rdm-records-3.0.0/tests/resources/test_resources_pids.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/test_resources_review.py` & `invenio-rdm-records-3.0.0/tests/resources/test_resources_review.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/test_rocrate.py` & `invenio-rdm-records-3.0.0/tests/resources/test_rocrate.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/test_serialized_links.py` & `invenio-rdm-records-3.0.0/tests/resources/test_serialized_links.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         "access_links": f"https://127.0.0.1:5000/api/records/{pid_value}/access/links",  # noqa
         "files": f"https://127.0.0.1:5000/api/records/{pid_value}/draft/files",
         "archive": f"https://127.0.0.1:5000/api/records/{pid_value}/draft/files-archive",  # noqa
         "reserve_doi": f"https://127.0.0.1:5000/api/records/{pid_value}/draft/pids/doi",  # noqa
         "self_iiif_manifest": f"https://127.0.0.1:5000/api/iiif/draft:{pid_value}/manifest",  # noqa
         "self_iiif_sequence": f"https://127.0.0.1:5000/api/iiif/draft:{pid_value}/sequence/default",  # noqa
         "communities": f"https://127.0.0.1:5000/api/records/{pid_value}/communities",  # noqa
+        "communities-suggestions": f"https://127.0.0.1:5000/api/records/{pid_value}/communities-suggestions",  # noqa
+        "requests": f"https://127.0.0.1:5000/api/records/{pid_value}/requests",  # noqa
     }
     assert expected_links == created_draft_links == read_draft_links
 
 
 def test_record_links(client, published_json, headers):
     """Tests the links for a published RDM record."""
     pid_value = published_json["id"]
@@ -92,14 +94,16 @@
         "latest": f"https://127.0.0.1:5000/api/records/{pid_value}/versions/latest",  # noqa
         "latest_html": f"https://127.0.0.1:5000/records/{pid_value}/latest",  # noqa
         "access_links": f"https://127.0.0.1:5000/api/records/{pid_value}/access/links",  # noqa
         "reserve_doi": f"https://127.0.0.1:5000/api/records/{pid_value}/draft/pids/doi",  # noqa
         "self_iiif_manifest": f"https://127.0.0.1:5000/api/iiif/record:{pid_value}/manifest",  # noqa
         "self_iiif_sequence": f"https://127.0.0.1:5000/api/iiif/record:{pid_value}/sequence/default",  # noqa
         "communities": f"https://127.0.0.1:5000/api/records/{pid_value}/communities",  # noqa
+        "communities-suggestions": f"https://127.0.0.1:5000/api/records/{pid_value}/communities-suggestions",  # noqa
+        "requests": f"https://127.0.0.1:5000/api/records/{pid_value}/requests",  # noqa
     }
     assert expected_links == published_record_links == read_record_links
 
 
 def test_record_search_links(client, published_json, headers):
     """Tests the links for a search of published RDM records."""
     response = client.get("/records", headers=headers)
```

### Comparing `invenio-rdm-records-2.9.0/tests/resources/vocabularies/conftest.py` & `invenio-rdm-records-3.0.0/tests/resources/vocabularies/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/vocabularies/test_affiliations_vocabulary.py` & `invenio-rdm-records-3.0.0/tests/resources/vocabularies/test_affiliations_vocabulary.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/vocabularies/test_awards_vocabulary.py` & `invenio-rdm-records-3.0.0/tests/resources/vocabularies/test_awards_vocabulary.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/vocabularies/test_funders_vocabulary.py` & `invenio-rdm-records-3.0.0/tests/resources/vocabularies/test_funders_vocabulary.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/vocabularies/test_names_vocabulary.py` & `invenio-rdm-records-3.0.0/tests/resources/vocabularies/test_names_vocabulary.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/resources/vocabularies/test_subjects_vocabulary.py` & `invenio-rdm-records-3.0.0/tests/resources/vocabularies/test_subjects_vocabulary.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/secret_links/test_secret_links.py` & `invenio-rdm-records-3.0.0/tests/secret_links/test_secret_links.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/secret_links/test_sharing.py` & `invenio-rdm-records-3.0.0/tests/secret_links/test_sharing.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/secret_links/test_token_serializers.py` & `invenio-rdm-records-3.0.0/tests/secret_links/test_token_serializers.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/components/test_access_component.py` & `invenio-rdm-records-3.0.0/tests/services/components/test_access_component.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/components/test_metadata_component.py` & `invenio-rdm-records-3.0.0/tests/services/components/test_metadata_component.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/components/test_pids_component.py` & `invenio-rdm-records-3.0.0/tests/services/components/test_pids_component.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/components/test_relations_component.py` & `invenio-rdm-records-3.0.0/tests/services/components/test_relations_component.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/conftest.py` & `invenio-rdm-records-3.0.0/tests/services/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 """
 
 import pytest
 from flask_principal import Identity, UserNeed
 from invenio_access.permissions import any_user, authenticated_user
 from invenio_app.factory import create_api
 
-from invenio_rdm_records.proxies import current_rdm_records_service
-
 
 @pytest.fixture(scope="module")
 def create_app(instance_path):
     """Application factory fixture."""
     return create_api
 
 
@@ -38,13 +36,7 @@
 @pytest.fixture(scope="function")
 def authenticated_identity():
     """Authenticated identity fixture."""
     identity = Identity(1)
     identity.provides.add(UserNeed(1))
     identity.provides.add(authenticated_user)
     return identity
-
-
-@pytest.fixture()
-def rdm_record_service():
-    """Get the current RDM records service."""
-    return current_rdm_records_service
```

### Comparing `invenio-rdm-records-2.9.0/tests/services/pids/providers/conftest.py` & `invenio-rdm-records-3.0.0/tests/services/pids/providers/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/pids/providers/test_datacite_pid_provider.py` & `invenio-rdm-records-3.0.0/tests/services/pids/providers/test_datacite_pid_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 @pytest.fixture(scope="function")
 def record_w_links(running_app, minimal_record):
     """Creates an empty record."""
     service = current_rdm_records.records_service
     draft = service.create(system_identity, minimal_record)
     record = service.publish(system_identity, draft.id)
 
-    return record
+    return record.to_dict()
 
 
 def test_datacite_provider_create(record, datacite_provider):
     created_pid = datacite_provider.create(record)
     db_pid = PersistentIdentifier.get(pid_value=created_pid.pid_value, pid_type="doi")
 
     assert created_pid == db_pid
@@ -83,21 +83,19 @@
 
 
 def test_datacite_provider_register(record_w_links, datacite_provider, mocker):
     mocker.patch(
         "invenio_rdm_records.services.pids.providers.datacite."
         + "DataCite43JSONSerializer"
     )
-    created_pid = datacite_provider.get(
-        record_w_links._record.pids["doi"]["identifier"]
-    )
+    created_pid = datacite_provider.get(record_w_links["pids"]["doi"]["identifier"])
     assert datacite_provider.register(
         pid=created_pid,
-        record=record_w_links._record,
-        url=record_w_links.links["self_html"],
+        record=record_w_links,
+        url=record_w_links["links"]["self_html"],
     )
 
     db_pid = PersistentIdentifier.get(pid_value=created_pid.pid_value, pid_type="doi")
 
     assert created_pid == db_pid
     assert db_pid.pid_value
     assert db_pid.pid_type == "doi"
@@ -105,23 +103,19 @@
 
 
 def test_datacite_provider_update(record_w_links, datacite_provider, mocker):
     mocker.patch(
         "invenio_rdm_records.services.pids.providers.datacite."
         + "DataCite43JSONSerializer"
     )
-    created_pid = datacite_provider.get(
-        record_w_links._record.pids["doi"]["identifier"]
-    )
+    created_pid = datacite_provider.get(record_w_links["pids"]["doi"]["identifier"])
     assert datacite_provider.register(
-        pid=created_pid, record=record_w_links, url=record_w_links.links["self_html"]
-    )
-    assert datacite_provider.update(
-        pid=created_pid, record=record_w_links._record, url=None
+        pid=created_pid, record=record_w_links, url=record_w_links["links"]["self_html"]
     )
+    assert datacite_provider.update(pid=created_pid, record=record_w_links, url=None)
 
     db_pid = PersistentIdentifier.get(pid_value=created_pid.pid_value, pid_type="doi")
 
     assert created_pid == db_pid
     assert db_pid.pid_value
     assert db_pid.pid_type == "doi"
     assert db_pid.status == PIDStatus.REGISTERED
@@ -153,19 +147,17 @@
     record_w_links, datacite_provider, mocker
 ):
     mocker.patch(
         "invenio_rdm_records.services.pids.providers.datacite."
         + "DataCite43JSONSerializer"
     )
     # Unregister NEW is a soft delete
-    created_pid = datacite_provider.get(
-        record_w_links._record.pids["doi"]["identifier"]
-    )
+    created_pid = datacite_provider.get(record_w_links["pids"]["doi"]["identifier"])
     assert datacite_provider.register(
-        pid=created_pid, record=record_w_links, url=record_w_links.links["self_html"]
+        pid=created_pid, record=record_w_links, url=record_w_links["links"]["self_html"]
     )
     assert created_pid.status == PIDStatus.REGISTERED
     assert datacite_provider.delete(created_pid)
 
     deleted_pid = PersistentIdentifier.get(
         pid_value=created_pid.pid_value, pid_type="doi"
     )
```

### Comparing `invenio-rdm-records-2.9.0/tests/services/pids/providers/test_external_pid_provider.py` & `invenio-rdm-records-3.0.0/tests/services/pids/providers/test_external_pid_provider.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/pids/providers/test_oai_invenio_pid_provider.py` & `invenio-rdm-records-3.0.0/tests/services/pids/providers/test_oai_invenio_pid_provider.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/pids/test_pids_service.py` & `invenio-rdm-records-3.0.0/tests/services/pids/test_pids_service.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/pids/test_pids_tasks.py` & `invenio-rdm-records-3.0.0/tests/services/pids/test_pids_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/conftest.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_access.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_access.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_additional_description.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_additional_description.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_additional_title.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_additional_title.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_creator_contributor.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_creator_contributor.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_dates.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_dates.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_formats.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_formats.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_funding.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_funding.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_identifier.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_identifier.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_languages.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_languages.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_location.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_location.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_metadata.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_pids.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_pids.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_publication_date.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_publication_date.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_rdm_record_schema.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_rdm_record_schema.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_reference.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_reference.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_related_identifier.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_related_identifier.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_resource_type.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_resource_type.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_rights.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_rights.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_sizes.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_sizes.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_utils.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_version.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_version.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/schemas/test_vocabulary.py` & `invenio-rdm-records-3.0.0/tests/services/schemas/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/test_generators.py` & `invenio-rdm-records-3.0.0/tests/services/test_generators.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/test_oai_service.py` & `invenio-rdm-records-3.0.0/tests/services/test_oai_service.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/test_permissions_policy.py` & `invenio-rdm-records-3.0.0/tests/services/test_permissions_policy.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/test_rdm_service.py` & `invenio-rdm-records-3.0.0/tests/services/test_rdm_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 # and/or modify it under the terms of the MIT License; see LICENSE file for
 # more details.
 
 """Service level tests for Invenio RDM Records."""
 
 import pytest
 
-from invenio_rdm_records.proxies import current_rdm_records, current_rdm_records_service
-from invenio_rdm_records.records import RDMDraft, RDMRecord
+from invenio_rdm_records.proxies import current_rdm_records
 from invenio_rdm_records.services.errors import EmbargoNotLiftedError
 
 
 def test_minimal_draft_creation(running_app, search_clear, minimal_record):
     superuser_identity = running_app.superuser_identity
     service = current_rdm_records.records_service
```

### Comparing `invenio-rdm-records-2.9.0/tests/services/test_service_community_records.py` & `invenio-rdm-records-3.0.0/tests/services/test_service_community_records.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 
 """Test community records service."""
 
 import pytest
 from invenio_records_resources.services.errors import PermissionDeniedError
 from marshmallow import ValidationError
 
-from invenio_rdm_records.proxies import current_community_records_service
+from invenio_rdm_records.proxies import (
+    current_community_records_service,
+    current_rdm_records_service,
+)
 from invenio_rdm_records.records import RDMRecord
-from invenio_rdm_records.services.errors import MaxNumberOfRecordsExceed
 
 
 @pytest.fixture()
 def service():
     """Get the current community records service."""
     return current_community_records_service
 
@@ -75,37 +77,36 @@
     errors = service.delete(curator.identity, str(community.id), data)
 
     assert len(errors) == 1
     assert errors[0]["message"] == "The record does not exist."
 
 
 def test_remove_record_of_other_community(
-    db, curator, community, community2, record_community, service, rdm_record_service
+    db, curator, community, community2, record_community, service
 ):
     """Test error on removing a record that belongs to another community."""
 
-    # TODO: remove this extra func when the `add` to a community is implemented
     def add_to_community2(record):
         record.parent.communities.remove(community._record)
         record.parent.communities.add(community2._record, default=False)
         record.parent.commit()
         record.commit()
         db.session.commit()
-        rdm_record_service.indexer.index(record)
+        current_rdm_records_service.indexer.index(record)
         RDMRecord.index.refresh()
         return record
 
     record_comm2 = record_community.create_record()
     record_comm2 = add_to_community2(record_comm2)
 
     data = {"records": [{"id": record_comm2.pid.pid_value}]}
     errors = service.delete(curator.identity, str(community.id), data)
 
     assert len(errors) == 1
-    assert errors[0]["message"] == "The record does not belong to the community."
+    assert "not included in the community" in errors[0]["message"]
 
 
 def test_remove_records_from_communities_success_w_errors(
     curator, community, record_community, service
 ):
     """Test removal of records from communities with errors."""
     record = record_community.create_record()
@@ -120,15 +121,15 @@
 def test_remove_too_many_records(curator, community, record_community, service):
     """Test removal of too many records from a community."""
     random_record = {"id": "random-id"}
     lots_of_records = []
     while len(lots_of_records) <= service.config.max_number_of_removals:
         lots_of_records.append(random_record)
     data = {"records": lots_of_records}
-    with pytest.raises(MaxNumberOfRecordsExceed):
+    with pytest.raises(ValidationError):
         service.delete(curator.identity, str(community.id), data)
 
 
 def test_remove_w_empty_payload(curator, community, service):
     """Test removal of records from communities with empty payload."""
     data = {"records": []}
     with pytest.raises(ValidationError):
```

### Comparing `invenio-rdm-records-2.9.0/tests/services/test_service_review.py` & `invenio-rdm-records-3.0.0/tests/services/test_service_review.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from sqlalchemy.orm.exc import NoResultFound
 
 from invenio_rdm_records.proxies import current_rdm_records
 from invenio_rdm_records.records.api import RDMDraft
 from invenio_rdm_records.records.systemfields.draft_status import DraftStatus
 from invenio_rdm_records.requests.community_submission import CommunitySubmission
 from invenio_rdm_records.services.errors import (
-    CommunityInclusionInconsistentAccessRestrictions,
+    InvalidAccessRestrictions,
     ReviewExistsError,
     ReviewNotFoundError,
     ReviewStateError,
 )
 
 
 def get_community_owner_identity(community):
@@ -372,15 +372,15 @@
 
 
 def test_submit_public_record_review_to_restricted_community(
     running_app, public_draft_review_restricted, service
 ):
     """Test creation of review after draft was created."""
     # Create draft
-    with pytest.raises(CommunityInclusionInconsistentAccessRestrictions):
+    with pytest.raises(InvalidAccessRestrictions):
         service.review.submit(
             running_app.superuser_identity, public_draft_review_restricted.id
         )
 
 
 def test_submit_restricted_record_review_to_restricted_community(
     running_app, restricted_draft_review_restricted, service
```

### Comparing `invenio-rdm-records-2.9.0/tests/services/test_service_tasks.py` & `invenio-rdm-records-3.0.0/tests/services/test_service_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/services/test_sort.py` & `invenio-rdm-records-3.0.0/tests/services/test_sort.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/test_alembic.py` & `invenio-rdm-records-3.0.0/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-records-2.9.0/tests/test_oai.py` & `invenio-rdm-records-3.0.0/tests/test_oai.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,21 +116,21 @@
         "  <dc:contributor>Nielsen, Lars Holm</dc:contributor>\n"
         "  <dc:creator>Nielsen, Lars Holm</dc:creator>\n"
         "  <dc:date>2018/2020-09</dc:date>\n"
         "  <dc:date>info:eu-repo/date/embargoEnd/2131-01-01</dc:date>\n"
         "  <dc:description>A description \nwith HTML tags</dc:description>\n"
         "  <dc:description>Bla bla bla</dc:description>\n"
         "  <dc:format>application/pdf</dc:format>\n"
-        "  <dc:identifier>1924MNRAS..84..308E</dc:identifier>\n"
-        "  <dc:identifier>10.5281/inveniordm.1234</dc:identifier>\n"
+        "  <dc:identifier>https://doi.org/10.5281/inveniordm.1234</dc:identifier>\n"
         "  <dc:identifier>oai:vvv.com:abcde-fghij</dc:identifier>\n"
+        "  <dc:identifier>bibcode:1924MNRAS..84..308E</dc:identifier>\n"
         "  <dc:language>dan</dc:language>\n"
         "  <dc:language>eng</dc:language>\n"
         "  <dc:publisher>InvenioRDM</dc:publisher>\n"
-        "  <dc:relation>doi:10.1234/foo.bar</dc:relation>\n"
+        "  <dc:relation>https://doi.org/10.1234/foo.bar</dc:relation>\n"
         "  <dc:rights>info:eu-repo/semantics/embargoedAccess</dc:rights>\n"
         "  <dc:rights>A custom license</dc:rights>\n"
         "  <dc:rights>https://customlicense.org/licenses/by/4.0/</dc:rights>\n"
         "  <dc:rights>Creative Commons Attribution 4.0 International</dc:rights>\n"  # noqa
         "  <dc:rights>https://creativecommons.org/licenses/by/4.0/legalcode</dc:rights>\n"  # noqa
         "  <dc:subject>custom</dc:subject>\n"
         "  <dc:title>InvenioRDM</dc:title>\n"
```

