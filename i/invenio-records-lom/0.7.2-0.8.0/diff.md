# Comparing `tmp/invenio-records-lom-0.7.2.tar.gz` & `tmp/invenio-records-lom-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-records-lom-0.7.2.tar", last modified: Wed Mar 15 11:36:44 2023, max compression
+gzip compressed data, was "invenio-records-lom-0.8.0.tar", last modified: Thu Apr 20 11:41:19 2023, max compression
```

## Comparing `invenio-records-lom-0.7.2.tar` & `invenio-records-lom-0.8.0.tar`

### file list

```diff
@@ -1,160 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.853136 invenio-records-lom-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-03-15 11:36:44.853136 invenio-records-lom-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.845136 invenio-records-lom-0.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.845136 invenio-records-lom-0.7.2/invenio_records_lom/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.845136 invenio-records-lom-0.7.2/invenio_records_lom/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/fixtures/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.845136 invenio-records-lom-0.7.2/invenio_records_lom/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.845136 invenio-records-lom-0.7.2/invenio_records_lom/jsonschemas/lomrecords/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/jsonschemas/lomrecords/lom-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/oai.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.845136 invenio-records-lom-0.7.2/invenio_records_lom/records/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.845136 invenio-records-lom-0.7.2/invenio_records_lom/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.845136 invenio-records-lom-0.7.2/invenio_records_lom/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.841136 invenio-records-lom-0.7.2/invenio_records_lom/records/mappings/os-v2/lomrecords/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.845136 invenio-records-lom-0.7.2/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.845136 invenio-records-lom-0.7.2/invenio_records_lom/records/mappings/os-v2/lomrecords/records/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/records/mappings/os-v2/lomrecords/records/record-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.845136 invenio-records-lom-0.7.2/invenio_records_lom/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/records/systemfields/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/records/systemfields/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/records/systemfields/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/records/systemfields/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/records/systemfields/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.845136 invenio-records-lom-0.7.2/invenio_records_lom/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.845136 invenio-records-lom-0.7.2/invenio_records_lom/resources/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/resources/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/resources/serializers/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.849136 invenio-records-lom-0.7.2/invenio_records_lom/services/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/services/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/services/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.849136 invenio-records-lom-0.7.2/invenio_records_lom/services/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/services/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/services/schemas/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/services/schemas/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/services/schemas/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/services/services.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/services/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.841136 invenio-records-lom-0.7.2/invenio_records_lom/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.841136 invenio-records-lom-0.7.2/invenio_records_lom/static/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.849136 invenio-records-lom-0.7.2/invenio_records_lom/static/templates/invenio_records_lom/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/static/templates/invenio_records_lom/results.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.841136 invenio-records-lom-0.7.2/invenio_records_lom/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.849136 invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/record.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.849136 invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/records/deposit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/records/export.html
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/records/files.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.849136 invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/records/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/records/macros/files.html
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/records/macros/tree.html
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/uploads.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.849136 invenio-records-lom-0.7.2/invenio_records_lom/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.841136 invenio-records-lom-0.7.2/invenio_records_lom/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.849136 invenio-records-lom-0.7.2/invenio_records_lom/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.841136 invenio-records-lom-0.7.2/invenio_records_lom/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.849136 invenio-records-lom-0.7.2/invenio_records_lom/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.849136 invenio-records-lom-0.7.2/invenio_records_lom/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.849136 invenio-records-lom-0.7.2/invenio_records_lom/ui/records/
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/records/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/records/deposits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/records/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/records/records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.853136 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.841136 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.841136 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.841136 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.841136 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.853136 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/LOMDepositForm.js
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/components.js
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/debug.js
--rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/fields.js
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/serializers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.853136 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/components.js
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.841136 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.853136 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/less/invenio_records_lom/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/less/invenio_records_lom/theme.less
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.853136 invenio-records-lom-0.7.2/invenio_records_lom/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    64221 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/utils/OEFOS2012_DE_CTI_20211111_154218_utf8.csv
--rw-r--r--   0 runner    (1001) docker     (123)    64211 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/utils/OEFOS2012_EN_CTI_20211111_154228_utf8.csv
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/utils/learning_resource_types.json
--rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/invenio_records_lom/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.845136 invenio-records-lom-0.7.2/invenio_records_lom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-03-15 11:36:44.000000 invenio-records-lom-0.7.2/invenio_records_lom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-03-15 11:36:44.000000 invenio-records-lom-0.7.2/invenio_records_lom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 11:36:44.000000 invenio-records-lom-0.7.2/invenio_records_lom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-15 11:36:44.000000 invenio-records-lom-0.7.2/invenio_records_lom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 11:36:44.000000 invenio-records-lom-0.7.2/invenio_records_lom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-15 11:36:44.000000 invenio-records-lom-0.7.2/invenio_records_lom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-15 11:36:44.000000 invenio-records-lom-0.7.2/invenio_records_lom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      737 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-03-15 11:36:44.853136 invenio-records-lom-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:36:44.853136 invenio-records-lom-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/tests/test_invenio_records_lom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/tests/test_pids_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-03-15 11:36:38.000000 invenio-records-lom-0.7.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.133244 invenio-records-lom-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-20 11:41:19.133244 invenio-records-lom-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.117244 invenio-records-lom-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/fixtures/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/jsonschemas/lomrecords/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/jsonschemas/lomrecords/lom-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/oai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/lomrecords/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/lomrecords/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/lomrecords/records/record-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/resources/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/resources/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15953 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/resources/serializers/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.125244 invenio-records-lom-0.8.0/invenio_records_lom/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/pids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.125244 invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/static/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.125244 invenio-records-lom-0.8.0/invenio_records_lom/static/templates/invenio_records_lom/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/static/templates/invenio_records_lom/results.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.125244 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/record.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.125244 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/deposit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/export.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/files.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.125244 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/macros/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/macros/tree.html
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/uploads.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.125244 invenio-records-lom-0.8.0/invenio_records_lom/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/ui/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/records/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/records/deposits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/records/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/records/records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/LOMDepositForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/components.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/debug.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/fields.js
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/serializers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/components.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/less/invenio_records_lom/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/less/invenio_records_lom/theme.less
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.133244 invenio-records-lom-0.8.0/invenio_records_lom/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    64221 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/utils/OEFOS2012_DE_CTI_20211111_154218_utf8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    64211 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/utils/OEFOS2012_EN_CTI_20211111_154228_utf8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/utils/learning_resource_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-20 11:41:19.000000 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-20 11:41:19.000000 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:41:19.000000 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-20 11:41:19.000000 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:41:19.000000 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 11:41:19.000000 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 11:41:19.000000 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      737 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-04-20 11:41:19.133244 invenio-records-lom-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.133244 invenio-records-lom-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/tests/test_invenio_records_lom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/tests/test_pids_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/tests/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/tests/test_utils.py
```

### Comparing `invenio-records-lom-0.7.2/.editorconfig` & `invenio-records-lom-0.8.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/CHANGES.rst` & `invenio-records-lom-0.8.0/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
     invenio-records-lom is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.0 (release 2023-04-20)
+
+- make compatible with invenio v11
+- support DOI, publishing, deleting
+
+
 Version v0.7.2 (release 2023-03-15)
 
 - fix file-upload
 
 
 Version v0.7.1 (release 2023-03-13)
```

### Comparing `invenio-records-lom-0.7.2/CONTRIBUTING.rst` & `invenio-records-lom-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/INSTALL.rst` & `invenio-records-lom-0.8.0/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/LICENSE` & `invenio-records-lom-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/MANIFEST.in` & `invenio-records-lom-0.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/PKG-INFO` & `invenio-records-lom-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-lom
-Version: 0.7.2
+Version: 0.8.0
 Summary: "Invenio data model for Learning Object Metadata."
 Home-page: https://github.com/tu-graz-library/invenio-records-lom
 Author: "Graz University of Technology"
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio record LOM learning object metadata
 Platform: any
@@ -59,14 +59,20 @@
 
     invenio-records-lom is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.0 (release 2023-04-20)
+
+- make compatible with invenio v11
+- support DOI, publishing, deleting
+
+
 Version v0.7.2 (release 2023-03-15)
 
 - fix file-upload
 
 
 Version v0.7.1 (release 2023-03-13)
```

### Comparing `invenio-records-lom-0.7.2/README.rst` & `invenio-records-lom-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/babel.ini` & `invenio-records-lom-0.8.0/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/docs/Makefile` & `invenio-records-lom-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/docs/conf.py` & `invenio-records-lom-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/docs/index.rst` & `invenio-records-lom-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/docs/make.bat` & `invenio-records-lom-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/cli.py` & `invenio-records-lom-0.8.0/invenio_records_lom/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/config.py` & `invenio-records-lom-0.8.0/invenio_records_lom/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """Default configuration."""
 
 import idutils
 from flask_babelex import gettext as _
 from invenio_rdm_records.services.pids import providers
 
 from .resources.serializers import LOMToDataCite44Serializer
+from .services.pids import LOMDataCitePIDProvider
 
 LOM_BASE_TEMPLATE = "invenio_records_lom/base.html"
 
 LOM_FACETS = {}
 
 LOM_SORT_OPTIONS = {
     "bestmatch": {
@@ -67,15 +68,15 @@
 LOM_PUBLISHER = "Graz University of Technology"
 
 #
 # Persistent identifiers configuration
 #
 LOM_PERSISTENT_IDENTIFIER_PROVIDERS = [
     # DataCite DOI provider
-    providers.DataCitePIDProvider(
+    LOMDataCitePIDProvider(
         "datacite",
         client=providers.DataCiteClient(
             "datacite",
             config_prefix="DATACITE",
         ),
         serializer=LOMToDataCite44Serializer(),
         label=_("DOI"),
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ext.py` & `invenio-records-lom-0.8.0/invenio_records_lom/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/fixtures/demo.py` & `invenio-records-lom-0.8.0/invenio_records_lom/fixtures/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from ..proxies import current_records_lom
 
 
 #
 # functions for LOM datatypes
 #
 def langstringify(fake: Faker, text: str, lang: str = "") -> dict:
-    """Wraps `text` in a dict, emulating LOMv1.0 LangString-objects.
+    """Wraps `text` in a dict, emulating LOMv1.0 langstring-objects.
 
     If `lang` is given and None, no "lang"-key is added to the returned dict.
     If `lang` is given and truthy, its value is used for the "lang"-key.
     If `lang` is not given or is falsy but not None, a fake-value is used for "lang".
     """
     langstring = {}
     if lang is not None:
@@ -52,28 +52,28 @@
         datetime = fake.date()
     elif pattern == "YMDhms":
         datetime = fake.date_time().isoformat()
     elif pattern == "YMDhmsTZD":
         time_zone_designator = fake.pytimezone()
         datetime = fake.date_time(tzinfo=time_zone_designator).isoformat()
 
-    return {"dateTime": datetime, "description": langstringify(fake, fake.sentence())}
+    return {"datetime": datetime, "description": langstringify(fake, fake.sentence())}
 
 
 def create_fake_duration(fake: Faker) -> dict:
     """Create a fake duration dict, as per LOM-UIBK specification."""
     randint = fake.random.randint
     return {
         "datetime": f"{randint(0,23):02}:{randint(0,59):02}:{randint(0,59):02}",
         "description": langstringify(fake, fake.sentence()),
     }
 
 
 def create_fake_vcard(fake: Faker) -> str:
-    """Returns a placeholder-string for a vCard-object."""
+    """Returns a placeholder-string for a vcard-object."""
     return f"{fake.last_name()}, {fake.first_name()}"
 
 
 #
 # functions for elements that are part of more than one category
 #
 def create_fake_language(fake: Faker) -> str:
@@ -103,41 +103,41 @@
     }
 
 
 def create_fake_contribute(fake: Faker, roles: list) -> dict:
     """Create a fake "contribute"-element, compatible with LOMv1.0."""
     return {
         "role": vocabularify(fake, roles),
-        "entity": create_fake_vcard(fake),
+        "entity": [create_fake_vcard(fake) for __ in range(2)],
         "date": create_fake_datetime(fake),
     }
 
 
 #
 # functions for categories or used by only one category
 #
 def create_fake_general(fake: Faker) -> dict:
     """Create a fake "general"-element, compatible with LOMv1.0."""
     structures = ["atomic", "collection", "networked", "hierarchical", "linear"]
-    aggregationLevels = ["1", "2", "3", "4"]
+    aggregationlevels = ["1", "2", "3", "4"]
 
     return {
         "identifier": [create_fake_identifier(fake) for __ in range(2)],
         "title": langstringify(fake, " ".join(fake.words()).title()),
         "language": [fake.random.choice([create_fake_language(fake), "none"])],
         "description": [langstringify(fake, fake.paragraph()) for __ in range(2)],
         "keyword": [langstringify(fake, fake.word()) for __ in range(2)],
         "coverage": [langstringify(fake, fake.paragraph()) for __ in range(2)],
         "structure": vocabularify(fake, structures),
-        "aggregationLevel": vocabularify(fake, aggregationLevels),
+        "aggregationlevel": vocabularify(fake, aggregationlevels),
     }
 
 
 def create_fake_lifecycle(fake: Faker) -> dict:
-    """Create a fake "lifeCycle"-element, compatible with LOMv1.0."""
+    """Create a fake "lifecycle"-element, compatible with LOMv1.0."""
     roles = [
         "author",
         "publisher",
         "unknown",
         "initiator",
         "terminator",
         "validator",
@@ -155,52 +155,55 @@
     statuses = ["draft", "final", "revised", "unavailable"]
 
     randint = fake.random.randint
 
     return {
         "version": langstringify(fake, f"{randint(0,9)}.{randint(0,9)}"),
         "status": vocabularify(fake, statuses),
-        "contribute": [create_fake_contribute(fake, roles) for __ in range(2)],
+        "contribute": [
+            create_fake_contribute(fake, ["author"]),  # guarantee one author exists
+            create_fake_contribute(fake, roles[1:]),  # create one random other role
+        ],
     }
 
 
 def create_fake_metametadata(fake: Faker) -> dict:
-    """Create a fake "metaMetadata"-element, compatible with LOMv1.0."""
+    """Create a fake "metametadata"-element, compatible with LOMv1.0."""
     roles = ["creator", "validator"]
     return {
         "identifier": [create_fake_identifier(fake) for __ in range(2)],
         "contribute": [create_fake_contribute(fake, roles) for __ in range(2)],
-        "metadataSchemas": ["LOMv1.0"],
+        "metadataschemas": ["LOMv1.0"],
         "language": create_fake_language(fake),
     }
 
 
 def create_fake_technical(fake: Faker) -> dict:
     """Create a fake "technical"-element, with fields from LOMv1.0 and LOM-UIBK."""
     return {
         "format": [fake.random.choice([fake.mime_type(), "non-digital"])],
         "size": str(fake.random.randint(1, 2**32)),
         "location": {"type": "URI", "#text": fake.uri()},
         "thumbnail": {"url": fake.uri()},
         "requirement": [create_fake_requirement(fake) for __ in range(2)],
-        "installationRemarks": langstringify(fake, fake.paragraph()),
-        "otherPlatformRequirements": langstringify(fake, fake.paragraph()),
+        "installationremarks": langstringify(fake, fake.paragraph()),
+        "otherplatformrequirements": langstringify(fake, fake.paragraph()),
         "duration": create_fake_duration(fake),
     }
 
 
 def create_fake_requirement(fake: Faker) -> dict:
     """Create a fake "requirement"-element, compatible with LOMv1.0."""
     return {
-        "orComposite": [create_fake_orcomposite(fake) for __ in range(2)],
+        "orcomposite": [create_fake_orcomposite(fake) for __ in range(2)],
     }
 
 
 def create_fake_orcomposite(fake: Faker) -> dict:
-    """Create a fake "orComposite"-element, compatible with LOMv1.0."""
+    """Create a fake "orcomposite"-element, compatible with LOMv1.0."""
     type_ = fake.random.choice(["operating system", "browser"])
     if type_ == "operating system":
         requirement_names = [
             "pc-dos",
             "ms-windows",
             "macos",
             "unix",
@@ -215,46 +218,46 @@
             "opera",
             "amaya",
         ]
 
     return {
         "type": vocabularify(fake, [type_]),
         "name": vocabularify(fake, requirement_names),
-        "minimumVersion": str(fake.random.randint(1, 4)),
-        "maximumVersion": str(fake.random.randint(5, 8)),
+        "minimumversion": str(fake.random.randint(1, 4)),
+        "maximumversion": str(fake.random.randint(5, 8)),
     }
 
 
 def create_fake_educational(fake: Faker) -> dict:
     """Create a fake "educational"-element, compatible with LOMv1.0."""
     interactivity_types = ["active", "expositive", "mixed"]
     levels = ["very low", "low", "medium", "high", "very high"]
     difficulties = ["very easy", "easy", "medium", "difficult", "very difficult"]
     end_user_roles = ["teacher", "author", "learner", "manager"]
     contexts = ["school", "higher education", "training", "other"]
 
     random_int = fake.random.randint
 
     return {
-        "interactivityType": vocabularify(fake, interactivity_types),
-        "learningResourceType": create_fake_learningresourcetype(fake),
-        "interactivityLevel": vocabularify(fake, levels),
-        "semanticDensity": vocabularify(fake, levels),
-        "intendedEndUserRole": vocabularify(fake, end_user_roles),
+        "interactivitytype": vocabularify(fake, interactivity_types),
+        "learningresourcetype": create_fake_learningresourcetype(fake),
+        "interactivitylevel": vocabularify(fake, levels),
+        "semanticdensity": vocabularify(fake, levels),
+        "intendedenduserrole": vocabularify(fake, end_user_roles),
         "context": [vocabularify(fake, contexts) for __ in range(2)],
-        "typicalAgeRange": langstringify(fake, f"{random_int(1,4)}-{random_int(5,9)}"),
+        "typicalagerange": langstringify(fake, f"{random_int(1,4)}-{random_int(5,9)}"),
         "difficulty": vocabularify(fake, difficulties),
-        "typicalLearningTime": create_fake_duration(fake),
+        "typicallearningtime": create_fake_duration(fake),
         "description": langstringify(fake, fake.paragraph()),
         "language": [create_fake_language(fake) for __ in range(2)],
     }
 
 
 def create_fake_learningresourcetype(fake: Faker) -> dict:
-    """Create a fake "learningResourceType"-element, compatible with LOM-UIBK."""
+    """Create a fake "learningresourcetype"-element, compatible with LOM-UIBK."""
     url_endings = [
         "application",
         "assessment",
         "audio",
         "case_study",
         "course",
         "data",
@@ -299,15 +302,15 @@
         "https://creativecommons.org/licenses/by-nc-nd/4.0",
         "https://mit-license.org/",
     ]
     url = fake.random.choice(urls)
     lang = "x-t-cc-url" if url.startswith("https://creativecommons.org/") else None
     return {
         "cost": vocabularify(fake, ["yes", "no"]),
-        "copyrightAndOtherRestrictions": vocabularify(fake, ["yes", "no"]),
+        "copyrightandotherrestrictions": vocabularify(fake, ["yes", "no"]),
         "description": langstringify(fake, fake.paragraph(), lang=lang),
         "url": fake.random.choice(urls),
     }
 
 
 def create_fake_relation(fake: Faker) -> dict:
     """Create a fake "relation"-element, compatible with LOMv1.0."""
@@ -356,22 +359,22 @@
         "skill level",
         "security level",
         "competency",
     ]
 
     return {
         "purpose": vocabularify(fake, purposes),
-        "taxonPath": [create_fake_taxonpath(fake) for __ in range(2)],
+        "taxonpath": [create_fake_taxonpath(fake) for __ in range(2)],
         "description": langstringify(fake, fake.paragraph()),
         "keyword": langstringify(fake, fake.word()),
     }
 
 
 def create_fake_taxonpath(fake: Faker) -> dict:
-    """Create a fake "taxonPath"-element, compatible with LOMv1.0."""
+    """Create a fake "taxonpath"-element, compatible with LOMv1.0."""
     return {
         "source": langstringify(fake, fake.word(), lang="x-none"),
         "taxon": [create_fake_taxon(fake) for __ in range(2)],
     }
 
 
 def create_fake_taxon(fake: Faker) -> dict:
@@ -389,16 +392,16 @@
 #
 # functions for creating LOMv1.0-fakes
 #
 def create_fake_metadata(fake: Faker) -> dict:
     """Create a fake json-representation of a "lom"-element, compatible with LOMv1.0."""
     data_to_use = {
         "general": create_fake_general(fake),
-        "lifeCycle": create_fake_lifecycle(fake),
-        "metaMetadata": create_fake_metametadata(fake),
+        "lifecycle": create_fake_lifecycle(fake),
+        "metametadata": create_fake_metametadata(fake),
         "technical": create_fake_technical(fake),
         "educational": create_fake_educational(fake),
         "rights": create_fake_rights(fake),
         "relation": [create_fake_relation(fake) for __ in range(2)],
         "annotation": [create_fake_annotation(fake) for __ in range(2)],
         "classification": [create_fake_classification(fake) for __ in range(2)],
     }
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/jsonschemas/lomrecords/lom-v1.0.0.json` & `invenio-records-lom-0.8.0/invenio_records_lom/jsonschemas/lomrecords/lom-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/oai.py` & `invenio-records-lom-0.8.0/invenio_records_lom/oai.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/records/__init__.py` & `invenio-records-lom-0.8.0/invenio_records_lom/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/records/api.py` & `invenio-records-lom-0.8.0/invenio_records_lom/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/draft-v1.0.0.json` & `invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/records/mappings/os-v2/lomrecords/records/record-v1.0.0.json` & `invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/lomrecords/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/records/models.py` & `invenio-records-lom-0.8.0/invenio_records_lom/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/records/systemfields/__init__.py` & `invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/records/systemfields/context.py` & `invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/context.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/records/systemfields/providers.py` & `invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/providers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/records/systemfields/relations.py` & `invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/relations.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/records/systemfields/resolver.py` & `invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/resolver.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/records/systemfields/results.py` & `invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/resources/__init__.py` & `invenio-records-lom-0.8.0/invenio_records_lom/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/resources/config.py` & `invenio-records-lom-0.8.0/invenio_records_lom/resources/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 # Copyright (C) 2021 Graz University of Technology.
 #
 # invenio-records-lom is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """REST API configuration."""
 
-from flask_resources import ResponseHandler
+import marshmallow
+from flask_resources import JSONSerializer, ResponseHandler
 from invenio_records_resources.resources import RecordResourceConfig
 from invenio_records_resources.resources.files import FileResourceConfig
 
 from .serializers import LOMUIJSONSerializer
 
 record_serializer = {
+    "application/json": ResponseHandler(JSONSerializer()),
     "application/vnd.inveniolom.v1+json": ResponseHandler(LOMUIJSONSerializer()),
 }
 
 
 class LOMDraftFilesResourceConfig(FileResourceConfig):
     """LOM Draft Files Resource configuration."""
 
@@ -41,10 +43,17 @@
 
     default_accept_mimetype = "application/json"
 
     routes = {
         "list": "",
         "item": "/<pid_value>",
         "item-draft": "/<pid_value>/draft",
+        "item-publish": "/<pid_value>/draft/actions/publish",
+        "item-pids-reserve": "/<pid_value>/draft/pids/<scheme>",
+    }
+
+    request_view_args = {
+        "pid_value": marshmallow.fields.Str(),
+        "scheme": marshmallow.fields.Str(),
     }
 
     response_handlers = record_serializer
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/resources/resources.py` & `invenio-records-lom-0.8.0/invenio_records_lom/resources/resources.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 #
 # invenio-records-lom is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """LOM resources."""
 
 from flask_resources import route
-from invenio_drafts_resources.resources import RecordResource
+from invenio_rdm_records.resources import RDMRecordResource
 
 
-class LOMRecordResource(RecordResource):
+class LOMRecordResource(RDMRecordResource):
     """LOM Record resource."""
 
     def create_url_rules(self):
         """Create the URL rules for the record resource."""
 
         def prefix(route_str):
             """Prefix a route with `self.config.prefix`."""
             return f"{self.config.url_prefix}{route_str}"
 
         routes = self.config.routes
         return [
+            route("DELETE", prefix(routes["item-pids-reserve"]), self.pids_discard),
+            route("DELETE", prefix(routes["item-draft"]), self.delete_draft),
             route("GET", prefix(routes["list"]), self.search),
             route("GET", prefix(routes["item"]), self.read),
             route("POST", prefix(routes["list"]), self.create),
+            route("POST", prefix(routes["item-publish"]), self.publish),
+            route("POST", prefix(routes["item-pids-reserve"]), self.pids_reserve),
             route("PUT", prefix(routes["item-draft"]), self.update_draft),
         ]
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/resources/serializers/__init__.py` & `invenio-records-lom-0.8.0/invenio_records_lom/resources/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/resources/serializers/schemas.py` & `invenio-records-lom-0.8.0/invenio_records_lom/resources/serializers/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 #
 # Copyright (C) 2021-2022 Graz University of Technology.
 #
 # invenio-records-lom is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Schemas which get wrapped by serializers."""
+# TODO: remove the following lines after moving to python3.9
+# allow `list[dict]` annotation, works without future-import for python>=3.9
+from __future__ import annotations
+
 import re
 
 import arrow
 from flask import current_app
 from flask_resources import BaseObjectSchema
 from invenio_rdm_records.resources.serializers.datacite.schema import (
     get_scheme_datacite,
@@ -164,15 +168,15 @@
 
     def get_contributors(self, obj: dict):
         """Get contributors."""
         ui_contributors = []
         for lom_contribute in (
             obj["metadata"].get("lifecycle", {}).get("contribute", [])
         ):
-            for entity in lom_contribute["entity"]:
+            for entity in lom_contribute.get("entity", []):
                 ui_contributors.append(
                     {
                         "fullname": entity,
                         "role": get_text(lom_contribute["role"]["value"]),
                     }
                 )
         return ui_contributors
@@ -276,18 +280,18 @@
     schemaVersion = fields.Constant("http://datacite.org/schema/kernel-4")
 
     def get_identifiers(self, obj: LOMRecord):
         """Get list of (main and alternate) identifiers."""
         serialized_identifiers = []
 
         # identifiers from 'pids'-key, goes first so DOI gets included
-        for scheme, id_ in obj["pids"].items():
+        for scheme, pid_info in obj["pids"].items():
             serialized_identifiers.append(
                 {
-                    "identifier": id_["identifier"],  # e.g. 10.1234/foo
+                    "identifier": pid_info["identifier"],  # e.g. 10.1234/foo
                     "identifierType": scheme.upper(),  # e.g. 'DOI', 'ISBN'
                 }
             )
 
         # identifiers from LOM-metadata
         for lom_identifier in obj["metadata"].get("general", {}).get("identifier", []):
             identifier = lom_identifier.get("entry")
@@ -299,59 +303,66 @@
             if serialized_identifier not in serialized_identifiers:
                 serialized_identifiers.append(serialized_identifier)
 
         return serialized_identifiers
 
     def get_creators(self, obj: LOMRecord):
         """Get list of creator-dicts."""
-        contributes = obj["metadata"].get("lifeCycle", {}).get("contribute", [])
+        contributes = obj["metadata"].get("lifecycle", {}).get("contribute", [])
         entities = []
         for contribute in contributes:
-            entities.append(contribute.get("entity"))
+            entities.extend(contribute.get("entity", []))
         return [{"name": entity} for entity in entities]
 
     def get_titles(self, obj: LOMRecord):
         """Get list of title-dicts."""
-        title = obj["metadata"].get("general", {}).get("title", "")
-        if not title:
+        title = obj["metadata"].get("general", {}).get("title", None)
+        if title is None:
             return []
         return [{"title": get_text(title), "lang": get_lang(title)}]
 
     def get_publisher(self, obj: LOMRecord):  # pylint: disable=unused-argument
         """Get publisher."""
         return current_app.config["LOM_PUBLISHER"]
 
     def get_publicationYear(self, obj: LOMRecord):
         """Get publication year."""
-        contributes = obj["metadata"].get("lifeCycle", {}).get("contribute", [])
+        contributes = obj["metadata"].get("lifecycle", {}).get("contribute", [])
         publish_dates = []
         for contribute in contributes:
-            role = contribute.get("role", {}).get("value")
-            if role == "publisher":
-                publish_dates.append(contribute.get("date", {}).get("dateTime"))
+            role = (
+                contribute.get("role", {})
+                .get("value", {})
+                .get("langstring", {})
+                .get("#text", "")
+            )
+            if role.lower() == "publisher":
+                if publish_date := contribute.get("date", {}).get("dateTime"):
+                    publish_dates.append(publish_date)
 
         if publish_dates:
             year = min(arrow.get(publish_date).year for publish_date in publish_dates)
         else:
             # from datacite specification: "For resources that do not have a standard publication year value, DataCite recommends that PublicationYear should include the date that is preferred for use in a citation."
             year = arrow.now().year
 
         return str(year)
 
     def get_contributors(self, obj: LOMRecord):
         """Get list of contributor-dicts."""
         contributes = obj["metadata"].get("lifeCycle", {}).get("contribute", [])
-        contributordicts = []
+        contributors: list[dict[str, str]] = []
         for contribute in contributes:
-            contributordict = {
-                "contributorType": "Other",
-                "name": contribute.get("entity"),
-            }
-            contributordicts.append(contributordict)
-        return contributordicts or missing
+            for entity in contribute.get("entity", []):
+                contributor = {
+                    "contributorType": "Other",
+                    "name": entity,
+                }
+                contributors.append(contributor)
+        return contributors or missing
 
     def get_dates(self, obj: LOMRecord):
         """Get list of date-dicts."""
         contributes = obj["metadata"].get("lifeCycle", {}).get("contribute", [])
         creator_dates = []
 
         for contribute in contributes:
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/services/__init__.py` & `invenio-records-lom-0.8.0/invenio_records_lom/services/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/services/components.py` & `invenio-records-lom-0.8.0/invenio_records_lom/services/components.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/services/config.py` & `invenio-records-lom-0.8.0/invenio_records_lom/services/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,15 +109,17 @@
         ),
         "files": ConditionalLink(
             cond=is_record,
             if_=RecordLink("{+api}/lom/{id}/files"),
             else_=RecordLink("{+api}/lom/{id}/draft/files"),
         ),
         "latest_html": RecordLink("{+ui}/lom/id/latest", when=is_record),
+        "publish": RecordLink("{+api}/lom/{id}/draft/actions/publish", when=is_draft),
         "record_html": RecordLink("{+ui}/lom/{id}", when=is_draft),
+        "reserve_doi": RecordLink("{+api}/lom/{id}/draft/pids/doi"),
         "self": ConditionalLink(
             cond=is_record,
             if_=RecordLink("{+api}/lom/{id}"),
             else_=RecordLink("{+api}/lom/{id}/draft"),
         ),
         "self_doi": Link(
             "{+ui}/lom/doi/{+pid_doi}",
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/services/schemas/fields.py` & `invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/services/schemas/metadata.py` & `invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,69 +3,84 @@
 # Copyright (C) 202 Graz University of Technology.
 #
 # invenio-records-lom is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Marshmallow schema for validating and serializing LOM JSONs."""
 
+import copy
+
 from marshmallow import INCLUDE, Schema, fields, validate
 
 
 class NoValidationSchema(Schema):
     """Let data through unchanged, without validation."""
 
     class Meta:
         """Configure this schema to include unknown fields no questions asked."""
 
         unknown = INCLUDE
 
+    def dump(self, obj, **_):
+        """Overwrite dump to return `obj`, bypassing validation as class name indicates."""
+        return copy.copy(obj)
+
 
-class LangstringField(fields.Dict):
-    """A dict-field of form {"langstring": {"#text": str, "lang": str}}."""
+class LangstringField(fields.Field):
+    """Verifies against form {"langstring": {"#text": str, "lang": str}}."""
 
     default_error_messages = {
-        "missing_langstring_key": "No {keys!r}-key in this langstring.",
         "extraneous_keys": "Extraneous keys in this langstring: {keys!r}.",
+        "extraneous_lang": "This Langstring must not have a `lang`-field.",
+        "missing_langstring_key": "No {keys!r}-key in this langstring.",
     }
 
+    def __init__(self, lang_exists=True, **kwargs):
+        """Init."""
+        super().__init__(**kwargs)
+        self.lang_exists = lang_exists
+
     def _deserialize(self, value, attr, data, **kwargs):
-        langstring_outer = super()._deserialize(value, attr, data, **kwargs)
+        if not isinstance(value, dict):
+            raise self.make_error("invalid")
 
         # validate outer keys
-        outer_keys = set(langstring_outer)
+        outer_keys = set(value)
         if "langstring" not in outer_keys:
             raise self.make_error("missing_langstring_key", keys="langstring")
         if not outer_keys <= {"langstring"}:
             raise self.make_error(
                 "extraneous_keys", keys=sorted(outer_keys - {"langstring"})
             )
 
-        langstring_inner = langstring_outer["langstring"]
+        langstring_inner = value["langstring"]
 
         # validate inner keys
         if not isinstance(langstring_inner, dict):
             raise self.make_error("invalid")
         inner_keys = set(langstring_inner)
         if "#text" not in inner_keys:
             raise self.make_error("missing_langstring_key", keys="#text")
-        if "lang" not in inner_keys:
+        if "lang" not in inner_keys and self.lang_exists:
             raise self.make_error("missing_langstring_key", keys="lang")
+        if "lang" in inner_keys and not self.lang_exists:
+            raise self.make_error("extraneous_lang")
         if not inner_keys <= {"#text", "lang"}:
             raise self.make_error(
                 "extraneous_keys", keys=sorted(inner_keys - {"#text", "lang"})
             )
 
         text = langstring_inner["#text"]
-        lang = langstring_inner["lang"]
+        lang = langstring_inner.get("lang", True)
 
         # validate non-emptiness of "#text"-, "lang"-key
         if not text or not lang:
             raise self.make_error("required")
 
-        return langstring_outer
+        return value
 
 
 class GeneralSchema(Schema):
     """Schema for LOM's `general` category."""
 
     class Meta:
         """Configure this schema to include unknown fields no questions asked."""
@@ -76,15 +91,17 @@
     keyword = fields.List(LangstringField)
 
 
 class ContributeSchema(Schema):
     """Schema for LOM's contribute-fields."""
 
     role = fields.Dict()
-    entity = fields.List(fields.String())
+    entity = fields.List(
+        fields.String(validate=validate.Length(min=1, error="Name cannot be empty."))
+    )
 
 
 class LifecycleSchema(Schema):
     """Schema for Lom's `lifecycle category."""
 
     contribute = fields.List(
         fields.Nested(ContributeSchema()),
@@ -99,28 +116,91 @@
     description = fields.Dict()
     url = fields.String(
         required=True,
         validate=validate.Length(min=1, error="Missing data for required field."),
     )
 
 
+class TaxonSchema(Schema):
+    """Schema for Lom's `classification.taxonpath.taxon`-category."""
+
+    id = fields.String(
+        required=True,
+        validate=validate.Regexp(
+            r"https://w3id.org/oerbase/vocabs/oefos2012/\d+",
+            error="Not a valid OEFOS-url.",
+        ),
+    )
+    entry = LangstringField(lang_exists=False)
+
+
+class TaxonpathSchema(Schema):
+    """Schema for LOM's `classification.taxonpath`-category."""
+
+    source = fields.Field(
+        required=True,
+        validate=validate.Equal(
+            {
+                "langstring": {
+                    "#text": "https://w3id.org/oerbase/vocabs/oefos2012",
+                    "lang": "x-none",
+                }
+            }
+        ),
+    )
+    taxon = fields.Nested(
+        TaxonSchema,
+        many=True,
+        required=True,
+        validate=validate.Length(
+            min=1, error="Must add at least one taxonomy to OEFOS taxonomy-path."
+        ),
+    )
+
+
+class ClassificationSchema(Schema):
+    """Schema for LOM's `classification`-category."""
+
+    purpose = fields.Field(
+        required=True,
+        validate=validate.Equal(
+            {
+                "source": {"langstring": {"#text": "LOMv1.0", "lang": "x-none"}},
+                "value": {"langstring": {"#text": "discipline", "lang": "x-none"}},
+            }
+        ),
+    )
+    taxonpath = fields.Nested(
+        TaxonpathSchema,
+        many=True,
+        required=True,
+        validate=validate.Length(min=1, error="Must add at least one OEFOS."),
+    )
+
+
 class MetadataSchema(Schema):
     """Schema for LOM-Metadata uploaded by deposit-page."""
 
     class Meta:
         """Configure this schema to include unknown fields no questions asked."""
 
         unknown = INCLUDE
 
     # passed by parent as to multiplex, removed by parent affter load/dump
-    type = fields.Constant("upload")
+    type = fields.Field(validate=validate.Equal("upload"))
 
-    general = fields.Nested(GeneralSchema)
-    lifecycle = fields.Nested(LifecycleSchema)
-    rights = fields.Nested(RightsSchema)
+    general = fields.Nested(GeneralSchema, required=True)
+    lifecycle = fields.Nested(LifecycleSchema, required=True)
+    rights = fields.Nested(RightsSchema, required=True)
+    classification = fields.Nested(
+        ClassificationSchema,
+        many=True,
+        required=True,
+        validate=validate.Length(min=1, error="Must add OEFOS-classification."),
+    )
 
     def load(self, data, **kwargs):
         """Overwrite parent as to use `NoValidationSchema` for resource-type!="upload"."""
         if data["type"] != "upload":
             return NoValidationSchema().load(data, **kwargs)
         data = super().load(data, **kwargs)
         return data
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/services/schemas/records.py` & `invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/records.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/services/services.py` & `invenio-records-lom-0.8.0/invenio_records_lom/services/services.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     @unit_of_work()
     def create(self, identity, data, uow=None, expand=False):
         """Create."""
         draft_item = super().create(identity, data, uow=uow, expand=expand)
 
         # add repo-pid to the record's identifiers
-        metadata = LOMMetadata(draft_item.to_dict())
+        metadata = LOMMetadata(data)
         metadata.append_identifier(draft_item.id, catalog="repo-pid")
         return super().update_draft(
             identity=identity,
             id_=draft_item.id,
             data=metadata.json,
             uow=uow,
             expand=expand,
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/services/tasks.py` & `invenio-records-lom-0.8.0/invenio_records_lom/services/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/static/templates/invenio_records_lom/results.html` & `invenio-records-lom-0.8.0/invenio_records_lom/static/templates/invenio_records_lom/results.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/record.html` & `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/record.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/records/deposit.html` & `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/deposit.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/records/export.html` & `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/export.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/records/files.html` & `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/files.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/records/macros/files.html` & `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/macros/files.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/records/macros/tree.html` & `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/macros/tree.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/search.html` & `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/search.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/templates/invenio_records_lom/uploads.html` & `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/uploads.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/translations/de/LC_MESSAGES/messages.po` & `invenio-records-lom-0.8.0/invenio_records_lom/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/translations/en/LC_MESSAGES/messages.po` & `invenio-records-lom-0.8.0/invenio_records_lom/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/translations/messages.pot` & `invenio-records-lom-0.8.0/invenio_records_lom/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/__init__.py` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/records/__init__.py` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/records/decorators.py` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/records/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/records/deposits.py` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/records/deposits.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2022-2023 Graz University of Technology.
 #
 # invenio-records-lom is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """View-functions for deposit-related pages."""
 
-from flask import current_app, render_template
+from flask import current_app, g, render_template
 from flask_login import current_user, login_required
 from invenio_i18n.ext import current_i18n
 from invenio_records_resources.services.files.results import FileList
 from invenio_records_resources.services.records.results import RecordItem
 from invenio_users_resources.proxies import current_user_resources
 
 from ...proxies import current_records_lom
@@ -134,16 +134,18 @@
         searchbar_config=template_context["searchbar_config"],
     )
 
 
 @login_required
 def uploads():
     """Show overview of lom-records uploaded by user, upload further records."""
-    # TODO: newer versions of expand also take flask.g.identity
     avatar_url = current_user_resources.users_service.links_item_tpl.expand(
-        current_user
+        g.identity, current_user
     )["avatar"]
     return render_template(
         "invenio_records_lom/uploads.html",
-        # TODO: newer versions also take `searchbar_config` here
+        # TODO: newer versions of the original template now also take `searchbar_config` here
+        # see `invenio_app_rdm/users_ui/views/dashboard.py:uploads`
+        # also see `invenio_app_rdm/users_ui/templates/uploads.html`
+        # searchbar_config={"searchUrl": ...},
         user_avatar=avatar_url,
     )
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/records/errors.py` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/records/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/records/records.py` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/records/records.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/LOMDepositForm.js` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/LOMDepositForm.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -21,16 +21,19 @@
 import {
     AccordionField
 } from "react-invenio-forms";
 import {
     Card,
     Container,
     Grid,
+    Icon,
+    Message,
+    Popup,
     Ref,
-    Sticky
+    Sticky,
 } from "semantic-ui-react";
 import {
     i18next
 } from "@translations/invenio_app_rdm/i18next";
 
 import {
     OptionalAccordion,
@@ -94,16 +97,22 @@
             // draftsService={new LOMDepositDraftsService()}  // defaults to RDMDepositDraftsService, which defers to apiClient
             // filesService={new LOMDepositFilesService()}  // defaults to RDMDeposiFilesService, which defers to fileApiClient
             >
             <
             FormFeedback fieldPath = "message"
             labels = {
                 {
-                    "metadata.general": "General",
-                    "metadata.general.title.langstring.lang": "Title-lang",
+                    // TODO:
+                    // uses paths of length two for now
+                    // this works for now, as every category has only one sub-field that can have errors
+                    // use longer paths once implemented in invenio...
+                    "metadata.general": i18next.t("Title"),
+                    "metadata.lifecycle": i18next.t("Contributors"),
+                    "metadata.rights": i18next.t("License"),
+                    "metadata.classification": i18next.t("OEFOS"),
                 }
             }
             /> {
                 /* TODO: Community-Header */ } <
             Container id = "deposit-form"
             className = "rel-mt-1" >
             <
@@ -119,15 +128,30 @@
                 11
             } >
             <
             AccordionField active includesPaths = {
                 ["files.enabled"]
             }
             label = {
-                i18next.t("Files")
+                <
+                >
+                <
+                Icon
+                color = "red"
+                name = "asterisk"
+                style = {
+                    {
+                        float: "left",
+                        marginRight: 14
+                    }
+                }
+                /> {
+                    i18next.t("Files")
+                } <
+                />
             } >
             {
                 this.noFiles && this.props.record.is_published && ( <
                     div className = "text-align-center pb-10" >
                     <
                     em > {
                         i18next.t("The record has no files.")
@@ -217,21 +241,59 @@
             <
             PublishButton fluid / >
             <
             /Grid.Column> <
             /Grid> <
             /Card.Content> <
             /Card> <
-            AccessRightField label = {
+            Card className = "access-right" >
+            <
+            Card.Content >
+            <
+            Card.Header >
+            <
+            label className = "field-label-class invenio-field-label"
+            htmlFor = "access" >
+            <
+            Icon name = "shield" / > {
                 i18next.t("Visibility")
+            } <
+            Popup trigger = {
+                <
+                Icon className = "ml-10"
+                name = "info circle" / >
+            }
+            content = {
+                i18next.t(
+                    "OER-uploads are always public."
+                )
             }
-            labelIcon = "shield"
-            fieldPath = "access" /
-            >
+            /> <
+            /label> <
+            /Card.Header> <
+            /Card.Content> <
+            Card.Content >
+            <
+            Message icon positive visible data - test - id = "access-message" >
+            <
+            Icon name = "lock open" / >
+            <
+            Message.Content >
             <
+            Message.Header > {
+                i18next.t("Public")
+            } < /Message.Header> {
+                i18next.t(
+                    "The record and files are publicly accessible."
+                )
+            } <
+            /Message.Content> <
+            /Message> <
+            /Card.Content> <
+            /Card> <
             Card >
             <
             Card.Content >
             <
             DeleteButton fluid isPublished = {
                 this.props.record.is_published
             }
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/components.js` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/components.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -13,14 +13,20 @@
     ArrayField,
     FieldLabel,
     GroupField,
     RichInputField,
     TextField,
 } from "react-invenio-forms";
 import {
+    PIDField
+} from "react-invenio-deposit";
+import {
+    useSelector
+} from "react-redux";
+import {
     Button,
     Divider,
     Form,
     Icon,
     Input
 } from "semantic-ui-react";
 import {
@@ -36,50 +42,133 @@
     TitledTextField,
     VocabularyGroupField,
 } from "./fields";
 
 // TODO: translations via i18next.t
 
 export function RequiredAccordion(props) {
+    // record.is_published should be one of `true`, `false`, `null` (counts as false)
+    const recordIsPublished =
+        useSelector((state) => state?.deposit?.record?.is_published) === true;
+
     return ( <
         AccordionField active includesPaths = {
             [
                 "metadata.general",
                 "metadata.general.title.langstring.lang",
                 "metadata.general.title.langstring.#text",
             ]
         }
-        label = "Required Fields" >
+        label = {
+            <
+            >
+            <
+            Icon
+            color = "red"
+            name = "asterisk"
+            style = {
+                {
+                    float: "left",
+                    marginRight: 14
+                }
+            }
+            /> {
+                i18next.t("Required Fields")
+            } <
+            />
+        } >
         <
+        PIDField btnLabelDiscardPID = {
+            i18next.t("Cancel DOI reservation.")
+        }
+        btnLabelGetPID = {
+            i18next.t("Reserve a DOI.")
+        }
+        canBeManaged = {
+            true
+        }
+        canBeUnmanaged = {
+            true
+        }
+        fieldPath = "pids.doi"
+        fieldLabel = {
+            <
+            >
+            <
+            Icon color = "red"
+            name = "asterisk" / >
+            <
+            Icon name = "book" / > {
+                i18next.t("Digital Object Identifier")
+            } <
+            />
+        }
+        isEditingPublishedRecord = {
+            recordIsPublished
+        }
+        managedHelpText = {
+            i18next.t(
+                "Reserved DOIs are registered when publishing your upload."
+            )
+        }
+        pidIcon = {
+            null
+        }
+        pidLabel = {
+            i18next.t("DOI")
+        }
+        pidPlaceholder = {
+            i18next.t("Enter your existing DOI here.")
+        }
+        pidType = "doi"
+        required = {
+            false
+        } // this field is required, but the red asterisk is added via the fieldLabel prop...
+        unmanagedHelpText = {
+            i18next.t(
+                "A DOI allows your upload to be unambiguously cited. It is of form `10.1234/foo.bar`."
+            )
+        }
+        /> <
         TitledTextField fieldPath = "metadata.form.title"
-        label = "Title"
-        placeholder = "Enter your title here."
-        required /
-        >
-        <
+        iconName = "book"
+        placeholder = {
+            i18next.t("Enter your title here.")
+        }
+        required title = {
+            i18next.t("Title")
+        }
+        /> <
         DropdownField fieldPath = "metadata.form.license"
         iconName = "drivers license"
-        placeholder = "Select License"
-        required title = "License"
+        placeholder = {
+            i18next.t("Select License")
+        }
+        required title = {
+            i18next.t("License")
+        }
         vocabularyName = "license" /
         >
         <
-        ArrayField addButtonLabel = "Add Contributor"
+        ArrayField addButtonLabel = {
+            i18next.t("Add Contributor")
+        }
         defaultNewValue = {
             {}
         }
         fieldPath = "metadata.form.contributor"
         label = {
             <
             label >
             <
-            Icon name = "red asterisk" / >
+            Icon color = "red"
+            name = "asterisk" / >
             <
             Icon name = "user plus" / > {
-                "Contributors"
+                i18next.t("Contributors")
             } <
             /label>
         } >
         {
             ({
                 arrayHelpers,
                 indexPath
@@ -91,377 +180,402 @@
                     `metadata.form.contributor.${indexPath}`
                 }
                 vocabularyName = "contributor" /
                 >
             )
         } <
         /ArrayField> <
-        ArrayField addButtonLabel = "Add OEFOS"
+        ArrayField addButtonLabel = {
+            i18next.t("Add OEFOS")
+        }
         defaultNewValue = {
             {}
         }
         fieldPath = "metadata.form.oefos"
         label = {
             //<FieldLabel icon="barcode" label="OEFOS" />
             <
             label >
             <
-            Icon name = "red asterisk" / >
+            Icon color = "red"
+            name = "asterisk" / >
             <
             Icon name = "barcode" / > {
-                "OEFOS"
+                i18next.t("OEFOS")
             } <
             /label>
         } >
         {
             ({
                 arrayHelpers,
                 indexPath
             }) => ( <
                 DropdownField closeAction = {
                     () => arrayHelpers.remove(indexPath)
                 }
                 fieldPath = {
                     `metadata.form.oefos.${indexPath}`
                 }
-                placeholder = "Select OEFOS"
+                placeholder = {
+                    i18next.t("Select OEFOS")
+                }
                 vocabularyName = "oefos" /
                 >
             )
         } <
         /ArrayField> <
         /AccordionField>
     );
 }
 
 export function OptionalAccordion(props) {
     return ( <
         AccordionField includesPaths = {
             []
         }
-        label = "Optional" >
+        label = {
+            i18next.t("Optional Fields")
+        } >
         <
         TitledTextField fieldPath = "metadata.form.description"
-        label = "Description"
-        placeholder = "Enter your description here."
+        iconName = "pencil"
+        placeholder = {
+            i18next.t("Enter your description here.")
+        }
         rows = {
             5
         }
+        title = {
+            i18next.t("Description")
+        }
         /> <
-        ArrayField addButtonLabel = "Add Tag"
+        ArrayField addButtonLabel = {
+            i18next.t("Add Tag")
+        }
         defaultNewValue = {
             {
                 value: ""
             }
         }
         fieldPath = "metadata.form.tag"
         label = {
             < FieldLabel icon = "tag"
-            label = "Tags" / >
-        } >
-        {
-            ({
-                arrayHelpers,
-                indexPath
-            }) => ( <
-                TitledTextField closeAction = {
-                    () => arrayHelpers.remove(indexPath)
-                }
-                fieldPath = {
-                    `metadata.form.tag.${indexPath}.value`
-                }
-                label = "Tag"
-                placeholder = "Enter your tag here" /
-                >
-            )
-        } <
-        /ArrayField> <
-        DropdownField fieldPath = "metadata.form.language"
-        iconName = "globe"
-        placeholder = "Select Language"
-        title = "Language"
-        vocabularyName = "language" /
-        > {
-            // TODO: resource_type
-        } <
-        /AccordionField>
-    );
-}
-
-export function TestAccordion(props) {
-    return ( <
-        AccordionField active includesPaths = {
-            [
-                "metadata.general",
-                "metadata.general.title.langstring.lang",
-                "metadata.general.title.langstring.#text",
-            ]
-        }
-        label = {
-            "Tests"
-        } >
-        <
-        DebugInfo fieldPath = "metadata" / >
-        <
-        p > 1 < /p> <
-        LeftLabeledTextField className = "twelve wide"
-        label = "test"
-        fieldPath = "metadata.general.title.langstring.#text"
-        required /
-        >
-        <
-        p > 2 < /p> <
-        LangstringGroupField debug fieldPath = "metadata.general.title"
-        label = "Test"
-        placeholder = "Hitchhiker's Guide to the Galaxy" /
-        >
-        <
-        p > 3 < /p> <
-        LangstringGroupField fieldPath = "metadata.general.title"
-        iconName = "book"
-        label = "label"
-        placeholder = "Hitchhiker's Guide to the Galaxy"
-        required title = "Title" /
-        >
-        <
-        p > 4 < /p> <
-        ArrayField addButtonLabel = "Add Description"
-        defaultNewValue = {
+            label = {
+                i18next.t("Tags")
+            }
+            />} >
             {
-                langstring: {
-                    "#text": "",
-                    lang: ""
-                }
+                ({
+                    arrayHelpers,
+                    indexPath
+                }) => ( <
+                    TitledTextField closeAction = {
+                        () => arrayHelpers.remove(indexPath)
+                    }
+                    fieldPath = {
+                        `metadata.form.tag.${indexPath}.value`
+                    }
+                    label = {
+                        i18next.t("Tag")
+                    }
+                    placeholder = {
+                        i18next.t("Enter your tag here")
+                    }
+                    />
+                )
+            } <
+            /ArrayField> <
+            DropdownField
+            fieldPath = "metadata.form.language"
+            iconName = "globe"
+            placeholder = {
+                i18next.t("Select Language")
             }
-        }
-        fieldPath = "metadata.general.description"
-        label = {
+            title = {
+                i18next.t("Language")
+            }
+            vocabularyName = "language" /
+            > {
+                // TODO: resource_type
+            } <
+            /AccordionField>
+        );
+    }
+
+    export function TestAccordion(props) {
+        return ( <
+            AccordionField active includesPaths = {
+                [
+                    "metadata.general",
+                    "metadata.general.title.langstring.lang",
+                    "metadata.general.title.langstring.#text",
+                ]
+            }
+            label = {
+                "Tests"
+            } >
             <
-            FieldLabel
-            htmlfor = "metadata.general.description"
-            icon = "pencil"
-            label = "Descriptions" /
+            DebugInfo fieldPath = "metadata" / >
+            <
+            p > 1 < /p> <
+            LeftLabeledTextField className = "twelve wide"
+            label = "test"
+            fieldPath = "metadata.general.title.langstring.#text"
+            required /
             >
-        } >
-        {
-            ({
-                arrayHelpers,
-                indexPath
-            }) => ( <
-                LangstringGroupField debug closeAction = {
-                    () => arrayHelpers.remove(indexPath)
-                }
-                fieldPath = {
-                    `metadata.general.description.${indexPath}`
-                }
-                label = "Description"
-                rows = "5" /
-                >
-            )
-        } <
-        /ArrayField> <
-        p > 5 < /p> <
-        LangstringGroupField / >
-        <
-        p > 6 < /p> <
-        DebugInfo fieldPath = "metadata.general.identifier" / >
-        <
-        ArrayField addButtonLabel = "Add Identifier"
-        defaultNewValue = {
-            {
-                catalog: "",
-                entry: {
+            <
+            p > 2 < /p> <
+            LangstringGroupField debug fieldPath = "metadata.general.title"
+            label = "Test"
+            placeholder = "Hitchhiker's Guide to the Galaxy" /
+            >
+            <
+            p > 3 < /p> <
+            LangstringGroupField fieldPath = "metadata.general.title"
+            iconName = "book"
+            label = "label"
+            placeholder = "Hitchhiker's Guide to the Galaxy"
+            required title = "Title" /
+            >
+            <
+            p > 4 < /p> <
+            ArrayField addButtonLabel = "Add Description"
+            defaultNewValue = {
+                {
                     langstring: {
                         "#text": "",
-                        lang: "x-none"
+                        lang: ""
                     }
-                },
-            }
-        }
-        fieldPath = "metadata.general.identifier"
-        label = {
-            <
-            FieldLabel
-            htmlFor = "metadata.general.identifier"
-            icon = "barcode"
-            label = "Identifiers" /
-            >
-        } >
-        {
-            ({
-                arrayHelpers,
-                indexPath
-            }) => ( <
-                VocabularyGroupField closeAction = {
-                    () => arrayHelpers.remove(indexPath)
-                }
-                debug fieldPath = {
-                    `metadata.general.identifier.${indexPath}`
                 }
-                label = "Identifier"
-                placeholder = "e.g. 123456-789" /
+            }
+            fieldPath = "metadata.general.description"
+            label = {
+                <
+                FieldLabel
+                htmlfor = "metadata.general.description"
+                icon = "pencil"
+                label = "Descriptions" /
                 >
-            )
-        } <
-        /ArrayField> <
-        p > 7 < /p> <
-        ArrayField addButtonLabel = "Add OEFOS"
-        defaultNewValue = {
-            {}
-        }
-        fieldPath = "metadata.oefos"
-        label = {
-            < FieldLabel icon = "barcode"
-            label = "OEFOS" / >
-        } >
-        {
-            ({
-                arrayHelpers,
-                indexPath
-            }) => ( <
-                DropdownField closeAction = {
-                    () => arrayHelpers.remove(indexPath)
-                }
-                debug fieldPath = {
-                    `metadata.oefos.${indexPath}`
-                }
-                />
-            )
-        } <
-        /ArrayField> <
-        DebugInfo fieldPath = "metadata.oefos" / >
-        <
-        p > 8 < /p> <
-        /AccordionField>
-    );
-}
-
-const Language = () => {
-    return ( <
-        ArrayField addButtonLabel = "Add Language"
-        defaultNewValue = {
+            } >
             {
-                value: ""
-            }
-        }
-        fieldPath = "metadata.general.language"
-        label = {
+                ({
+                    arrayHelpers,
+                    indexPath
+                }) => ( <
+                    LangstringGroupField debug closeAction = {
+                        () => arrayHelpers.remove(indexPath)
+                    }
+                    fieldPath = {
+                        `metadata.general.description.${indexPath}`
+                    }
+                    label = "Description"
+                    rows = "5" /
+                    >
+                )
+            } <
+            /ArrayField> <
+            p > 5 < /p> <
+            LangstringGroupField / >
             <
-            FieldLabel
-            htmlFor = "metadata.general.language"
-            icon = "globe"
-            label = "Languages" /
-            >
-        } >
-        {
-            ({
-                arrayHelpers,
-                indexPath
-            }) => ( <
-                GroupField >
-                <
-                TextField fieldPath = {
-                    `metadata.general.language.${indexPath}.value`
-                }
-                helpText = {
-                    null
-                }
-                label = {
-                    null
-                }
-                placeholder = ""
-                width = {
-                    16
+            p > 6 < /p> <
+            DebugInfo fieldPath = "metadata.general.identifier" / >
+            <
+            ArrayField addButtonLabel = "Add Identifier"
+            defaultNewValue = {
+                {
+                    catalog: "",
+                    entry: {
+                        langstring: {
+                            "#text": "",
+                            lang: "x-none"
+                        }
+                    },
                 }
-                /> <
-                Form.Field >
+            }
+            fieldPath = "metadata.general.identifier"
+            label = {
                 <
-                Button aria - label = "Remove Field"
-                className = "close-btn"
-                icon = "close"
-                onClick = {
-                    () => arrayHelpers.remove(indexPath)
-                }
-                /> <
-                /Form.Field> <
-                /GroupField>
-            )
-        } <
-        /ArrayField>
-    );
-};
-
-const RichInput = ({
-    indexPath
-}) => {
-    return ( <
-        RichInputField className = "fourteen wide"
-        fieldPath = {
-            `metadata.general.description.${indexPath}.langstring.#text`
-        }
-        editorConfig = {
+                FieldLabel
+                htmlFor = "metadata.general.identifier"
+                icon = "barcode"
+                label = "Identifiers" /
+                >
+            } >
             {
-                removePlugins: [
-                    "Image",
-                    "ImageCaption",
-                    "ImageStyle",
-                    "ImageToolbar",
-                    "ImageUpload",
-                    "MediaEmbed",
-                    "Table",
-                    "TableToolbar",
-                    "TableProperties",
-                    "TableCellProperties",
-                ],
+                ({
+                    arrayHelpers,
+                    indexPath
+                }) => ( <
+                    VocabularyGroupField closeAction = {
+                        () => arrayHelpers.remove(indexPath)
+                    }
+                    debug fieldPath = {
+                        `metadata.general.identifier.${indexPath}`
+                    }
+                    label = "Identifier"
+                    placeholder = "e.g. 123456-789" /
+                    >
+                )
+            } <
+            /ArrayField> <
+            p > 7 < /p> <
+            ArrayField addButtonLabel = "Add OEFOS"
+            defaultNewValue = {
+                {}
             }
-        }
-        label = {
+            fieldPath = "metadata.oefos"
+            label = {
+                < FieldLabel icon = "barcode"
+                label = "OEFOS" / >
+            } >
+            {
+                ({
+                    arrayHelpers,
+                    indexPath
+                }) => ( <
+                    DropdownField closeAction = {
+                        () => arrayHelpers.remove(indexPath)
+                    }
+                    debug fieldPath = {
+                        `metadata.oefos.${indexPath}`
+                    }
+                    />
+                )
+            } <
+            /ArrayField> <
+            DebugInfo fieldPath = "metadata.oefos" / >
             <
-            FieldLabel
-            htmlFor = {
-                `metadata.general.description.${indexPath}.langstring.#text`
-            }
-            icon = "pencil"
-            label = "Description" /
-            >
-        }
-        optimized /
-        >
-    );
-};
-const FormikChildren = ({
-    indexPath
-}) => {
-    <
-    FormikField
-    className = "invenio-text-input-field"
-    id = {
-        `metadata.lifecycle.identifier.${indexPath}.catalog`
+            p > 8 < /p> <
+            /AccordionField>
+        );
     }
-    name = {
-            `metadata.lifecycle.identifier.${indexPath}.catalog`
-        } >
-        {
-            ({
-                field,
-                meta
-            }) => {
-                return ( <
-                    div className = "four wide field" >
+
+    const Language = () => {
+        return ( <
+            ArrayField addButtonLabel = "Add Language"
+            defaultNewValue = {
+                {
+                    value: ""
+                }
+            }
+            fieldPath = "metadata.general.language"
+            label = {
+                <
+                FieldLabel
+                htmlFor = "metadata.general.language"
+                icon = "globe"
+                label = "Languages" /
+                >
+            } >
+            {
+                ({
+                    arrayHelpers,
+                    indexPath
+                }) => ( <
+                    GroupField >
                     <
-                    Input {
-                        ...field
+                    TextField fieldPath = {
+                        `metadata.general.language.${indexPath}.value`
                     }
-                    error = {
-                        meta.error
+                    helpText = {
+                        null
                     }
-                    fluid label = "Catalog"
-                    placeholder = "e.g. ISBN, DOI"
-                    type = "text" /
-                    >
+                    label = {
+                        null
+                    }
+                    placeholder = ""
+                    width = {
+                        16
+                    }
+                    /> <
+                    Form.Field >
                     <
-                    /div>
-                );
+                    Button aria - label = "Remove Field"
+                    className = "close-btn"
+                    icon = "close"
+                    onClick = {
+                        () => arrayHelpers.remove(indexPath)
+                    }
+                    /> <
+                    /Form.Field> <
+                    /GroupField>
+                )
+            } <
+            /ArrayField>
+        );
+    };
+
+    const RichInput = ({
+        indexPath
+    }) => {
+        return ( <
+            RichInputField className = "fourteen wide"
+            fieldPath = {
+                `metadata.general.description.${indexPath}.langstring.#text`
             }
-        } <
-        /FormikField>;
-};
+            editorConfig = {
+                {
+                    removePlugins: [
+                        "Image",
+                        "ImageCaption",
+                        "ImageStyle",
+                        "ImageToolbar",
+                        "ImageUpload",
+                        "MediaEmbed",
+                        "Table",
+                        "TableToolbar",
+                        "TableProperties",
+                        "TableCellProperties",
+                    ],
+                }
+            }
+            label = {
+                <
+                FieldLabel
+                htmlFor = {
+                    `metadata.general.description.${indexPath}.langstring.#text`
+                }
+                icon = "pencil"
+                label = "Description" /
+                >
+            }
+            optimized /
+            >
+        );
+    };
+    const FormikChildren = ({
+        indexPath
+    }) => {
+        <
+        FormikField
+        className = "invenio-text-input-field"
+        id = {
+            `metadata.lifecycle.identifier.${indexPath}.catalog`
+        }
+        name = {
+                `metadata.lifecycle.identifier.${indexPath}.catalog`
+            } >
+            {
+                ({
+                    field,
+                    meta
+                }) => {
+                    return ( <
+                        div className = "four wide field" >
+                        <
+                        Input {
+                            ...field
+                        }
+                        error = {
+                            meta.error
+                        }
+                        fluid label = "Catalog"
+                        placeholder = "e.g. ISBN, DOI"
+                        type = "text" /
+                        >
+                        <
+                        /div>
+                    );
+                }
+            } <
+            /FormikField>;
+    };
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/debug.js` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/debug.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -72,27 +72,51 @@
                 },
             })
         );
         console.log(resp);
         return resp;
     }
     async publishDraft(draftLinks) {
-        throw new Error("Not implemented.");
+        return this._createResponse(() =>
+            debugAxiosWithConfig.post(
+                draftLinks.publish, {}, {
+                    params: {
+                        expand: 1
+                    }
+                }
+            )
+        );
     }
 
     async deleteDraft(draftLinks) {
-        throw new Error("Not implemented.");
+        return this._createResponse(() =>
+            debugAxiosWithConfig.delete(draftLinks.self, {})
+        );
     }
 
     async reservePID(draftLinks, pidType) {
-        throw new Error("Not implemented.");
+        return this._createResponse(() => {
+            const link = draftLinks[`reserve_${pidType}`];
+            return debugAxiosWithConfig.post(link, {}, {
+                params: {
+                    expand: 1
+                }
+            });
+        });
     }
 
     async discardPID(draftLinks, pidType) {
-        throw new Error("Not implemented.");
+        return this._createResponse(() => {
+            const link = draftLinks[`reserve_${pidType}`];
+            return debugAxiosWithConfig.delete(link, {
+                params: {
+                    expand: 1
+                }
+            });
+        });
     }
 
     async createOrUpdateReview(draftLinks, communityId) {
         throw new Error("Not implemented.");
     }
 
     async deleteReview(draftLinks) {
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/fields.js` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/fields.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -57,15 +57,17 @@
 
 const CloseButton = ({
     closeAction
 }) => {
     return closeAction ? ( <
         Form.Field >
         <
-        Button aria - label = "Remove Field"
+        Button aria - label = {
+            i18next.t("Remove Field")
+        }
         className = "close-btn"
         icon = "close"
         onClick = {
             closeAction
         }
         /> <
         /Form.Field>
@@ -78,15 +80,16 @@
     label,
     required
 }) => {
     const icon = iconName ? < Icon name = {
         iconName
     }
     /> : null;
-    const requiredIcon = required ? < Icon name = "red asterisk" / > : null;
+    const requiredIcon = required ? < Icon color = "red"
+    name = "asterisk" / >: null;
     return label || icon ? ( <
         label htmlFor = {
             fieldPath || null
         } > {
             requiredIcon
         } {
             icon
@@ -145,23 +148,21 @@
                             label
                         } < /div>
                     )
                 } <
                 InputTag disabled = {
                     isSubmitting
                 }
-                fluid id = {
+                fluid = "true"
+                id = {
                     fieldPath
                 }
                 label = {
                     label
                 }
-                minHeight = {
-                    InputTag === "textarea" ? "100" : undefined
-                }
                 name = {
                     fieldPath
                 }
                 onBlur = {
                     handleBlur
                 }
                 onChange = {
@@ -228,15 +229,16 @@
                     rows,
                     title,
                 } = props;
                 const icon = iconName ? < Icon name = {
                     iconName
                 }
                 /> : null;
-                const requiredIcon = required ? < Icon name = "red asterisk" / > : null;
+                const requiredIcon = required ? < Icon color = "red"
+                name = "asterisk" / >: null;
                 const labelElement =
                     title || icon ? ( <
                         label htmlFor = {
                             fieldPath
                         } > {
                             requiredIcon
                         } {
@@ -264,17 +266,14 @@
                     }
                     label = {
                         label
                     }
                     placeholder = {
                         placeholder
                     }
-                    required = {
-                        required
-                    }
                     rows = {
                         rows
                     }
                     /> <
                     CloseButton closeAction = {
                         closeAction
                     }
@@ -460,26 +459,31 @@
                                             value
                                         }) =>
                                         setFieldValue(`${name}.value`, value)
                                     }
                                     options = {
                                         options
                                     }
-                                    placeholder = "Select Role"
+                                    placeholder = {
+                                        i18next.t("Select Role")
+                                    }
                                     search selection /
                                     >
                                     <
                                     LeftLabeledTextField className = "twelve wide"
                                     fieldPath = {
                                         `${fieldPath}.name`
                                     }
-                                    label = "Name"
-                                    placeholder = "Enter name here" /
-                                    >
-                                    <
+                                    label = {
+                                        i18next.t("Name")
+                                    }
+                                    placeholder = {
+                                        i18next.t("Enter name here")
+                                    }
+                                    /> <
                                     CloseButton closeAction = {
                                         closeAction
                                     }
                                     /> <
                                     /GroupField> <
                                     /Form.Field>
                                 );
@@ -510,15 +514,16 @@
                                     rows,
                                     title,
                                 } = props;
                                 const icon = iconName ? < Icon name = {
                                     iconName
                                 }
                                 /> : null;
-                                const requiredIcon = required ? < Icon name = "red asterisk" / > : null;
+                                const requiredIcon = required ? < Icon color = "red"
+                                name = "asterisk" / >: null;
                                 const labelElement =
                                     title || icon ? ( <
                                         label htmlFor = {
                                             `${fieldPath}.langstring.#text`
                                         } > {
                                             requiredIcon
                                         } {
@@ -595,15 +600,16 @@
                                             rows,
                                             title,
                                         } = props;
                                         const icon = iconName ? < Icon name = {
                                             iconName
                                         }
                                         /> : null;
-                                        const requiredIcon = required ? < Icon name = "red asterisk" / > : null;
+                                        const requiredIcon = required ? < Icon color = "red"
+                                        name = "asterisk" / >: null;
                                         const labelElement =
                                             title || icon ? ( <
                                                 label htmlFor = {
                                                     `${fieldPath}.langstring.#text`
                                                 } > {
                                                     requiredIcon
                                                 } {
@@ -664,15 +670,16 @@
                                                         icon,
                                                         label,
                                                         placeholder,
                                                         required,
                                                         title,
                                                     } = this.props;
 
-                                                    const requiredIcon = required ? < Icon name = "red asterisk" / > : null;
+                                                    const requiredIcon = required ? < Icon color = "red"
+                                                    name = "asterisk" / >: null;
                                                     const labelElement =
                                                         title || icon ? ( <
                                                             label > {
                                                                 requiredIcon
                                                             } {
                                                                 icon
                                                             } {
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/index.js` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/index.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/serializers.js` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/serializers.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -145,15 +145,15 @@
         );
         // create oefos-classification
         let oefosClassification = {
             purpose: {
                 source: {
                     langstring: {
                         lang: "x-none",
-                        "#text": "LOMv1.0."
+                        "#text": "LOMv1.0"
                     }
                 },
                 value: {
                     langstring: {
                         lang: "x-none",
                         "#text": "discipline"
                     }
@@ -212,19 +212,19 @@
             record.metadata = {};
         }
         const metadata = record.metadata;
         metadata.form = {};
         const form = metadata.form;
 
         // deserialize title
-        form.title = _get(metadata, "general.title.langstring.#text");
+        form.title = _get(metadata, "general.title.langstring.#text", "");
 
         // deserialize license
         form.license = {
-            value: _get(metadata, "rights.url")
+            value: _get(metadata, "rights.url", "")
         };
 
         // deserialize contributors
         const validRoles = Object.keys(_get(this, "vocabularies.contributor", {}));
         form.contributor = [];
         for (const contribute of _get(metadata, "lifecycle.contribute", [])) {
             let role = _get(contribute, "role.value.langstring.#text", "");
@@ -248,20 +248,20 @@
             "general.description.0.langstring.#text",
             ""
         );
 
         // deserialize tags
         const tagLangstringObjects = _get(metadata, "general.keyword", []);
         form.tag = tagLangstringObjects.map((langstringObject) => ({
-            value: _get(langstringObject, "langstring.#text"),
+            value: _get(langstringObject, "langstring.#text", ""),
         }));
 
         // deserialize language
         form.language = {
-            value: _get(metadata, "general.language.0")
+            value: _get(metadata, "general.language.0", "")
         };
 
         return record;
     }
 
     // frontend->backend
     serialize(record) {
@@ -365,42 +365,62 @@
 
         for (const e of errors) {
             _set(deserializedErrors, e.field, e.messages.join(" "));
         }
 
         // deserialize error for title
         const titleError = _get(deserializedErrors, "metadata.general.title", null);
-        _set(deserializedErrors, "metadata.form.title", titleError);
+        if (titleError) {
+            _set(deserializedErrors, "metadata.form.title", titleError);
+        }
 
         // deserialize error for license
         const licenseErrorMessages = [];
         for (const {
                 field,
                 messages
             }
             of errors) {
             if (String(field).startsWith("metadata.rights")) {
                 licenseErrorMessages.push(...messages);
             }
         }
-        _set(
-            deserializedErrors,
-            "metadata.form.license",
-            licenseErrorMessages.join(" ")
-        );
+        const licenseErrorMessage = licenseErrorMessages.join(" ");
+        if (licenseErrorMessage) {
+            _set(
+                deserializedErrors,
+                "metadata.form.license",
+                licenseErrorMessages.join(" ")
+            );
+        }
 
         // deserialize error for contribute
         const contributeError = _get(
             deserializedErrors,
             "metadata.lifecycle.contribute",
             null
         );
-        _set(deserializedErrors, "metadata.form.contribute", contributeError);
+        if (contributeError) {
+            _set(deserializedErrors, "metadata.form.contribute", contributeError);
+        }
 
-        // debug({ deserializedErrors });
+        // deserialize error for oefos
+        const classificationErrorMessages = errors
+            .filter((error) =>
+                String(error.field || "").startsWith("metadata.classification")
+            )
+            .map((error) => error.messages || [])
+            .flat();
+        if (classificationErrorMessages.length > 0) {
+            _set(
+                deserializedErrors,
+                "metadata.form.oefos",
+                classificationErrorMessages.join(" ")
+            );
+        }
 
         // add error for debug-purposes
         /*deserializedErrors["metadata"] = {
           // "general.title.langstring.lang": "deserialization-error",
           general: {
             title: { langstring: { lang: "title-lang error" } },
             description: {
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/components.js` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/components.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/index.js` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/index.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/config.py` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/views.py` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/views.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/ui/theme/webpack.py` & `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/utils/OEFOS2012_DE_CTI_20211111_154218_utf8.csv` & `invenio-records-lom-0.8.0/invenio_records_lom/utils/OEFOS2012_DE_CTI_20211111_154218_utf8.csv`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/utils/OEFOS2012_EN_CTI_20211111_154228_utf8.csv` & `invenio-records-lom-0.8.0/invenio_records_lom/utils/OEFOS2012_EN_CTI_20211111_154228_utf8.csv`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/utils/__init__.py` & `invenio-records-lom-0.8.0/invenio_records_lom/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/utils/learning_resource_types.json` & `invenio-records-lom-0.8.0/invenio_records_lom/utils/learning_resource_types.json`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/utils/util.py` & `invenio-records-lom-0.8.0/invenio_records_lom/utils/util.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom/views.py` & `invenio-records-lom-0.8.0/invenio_records_lom/views.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom.egg-info/PKG-INFO` & `invenio-records-lom-0.8.0/invenio_records_lom.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-lom
-Version: 0.7.2
+Version: 0.8.0
 Summary: "Invenio data model for Learning Object Metadata."
 Home-page: https://github.com/tu-graz-library/invenio-records-lom
 Author: "Graz University of Technology"
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio record LOM learning object metadata
 Platform: any
@@ -59,14 +59,20 @@
 
     invenio-records-lom is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.0 (release 2023-04-20)
+
+- make compatible with invenio v11
+- support DOI, publishing, deleting
+
+
 Version v0.7.2 (release 2023-03-15)
 
 - fix file-upload
 
 
 Version v0.7.1 (release 2023-03-13)
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom.egg-info/SOURCES.txt` & `invenio-records-lom-0.8.0/invenio_records_lom.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 invenio_records_lom/resources/resources.py
 invenio_records_lom/resources/serializers/__init__.py
 invenio_records_lom/resources/serializers/schemas.py
 invenio_records_lom/services/__init__.py
 invenio_records_lom/services/components.py
 invenio_records_lom/services/config.py
 invenio_records_lom/services/permissions.py
+invenio_records_lom/services/pids.py
 invenio_records_lom/services/services.py
 invenio_records_lom/services/tasks.py
 invenio_records_lom/services/schemas/__init__.py
 invenio_records_lom/services/schemas/fields.py
 invenio_records_lom/services/schemas/metadata.py
 invenio_records_lom/services/schemas/records.py
 invenio_records_lom/static/templates/invenio_records_lom/results.html
```

### Comparing `invenio-records-lom-0.7.2/invenio_records_lom.egg-info/entry_points.txt` & `invenio-records-lom-0.8.0/invenio_records_lom.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/run-tests.sh` & `invenio-records-lom-0.8.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/setup.cfg` & `invenio-records-lom-0.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.8
 zip_safe = False
 install_requires = 
-	invenio-previewer>=1.3.4
-	invenio-rdm-records>=0.35.16,<0.99
+	invenio-previewer>=1.3.6
+	invenio-rdm-records>=1.1.0,<2.0.0
 
 [options.extras_require]
 tests = 
 	flake8<5.0.0 # necessary to prevent error AttributeError ConfigFileFinder not found
 	invenio-app>=1.3.3,<2.0.0
 	invenio-cache>=1.0.6
 	invenio-search[opensearch2]>=2.0.0
```

### Comparing `invenio-records-lom-0.7.2/tests/conftest.py` & `invenio-records-lom-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/tests/test_invenio_records_lom.py` & `invenio-records-lom-0.8.0/tests/test_invenio_records_lom.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/tests/test_pids_service.py` & `invenio-records-lom-0.8.0/tests/test_pids_service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/tests/test_service.py` & `invenio-records-lom-0.8.0/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.7.2/tests/test_utils.py` & `invenio-records-lom-0.8.0/tests/test_utils.py`

 * *Files identical despite different names*

