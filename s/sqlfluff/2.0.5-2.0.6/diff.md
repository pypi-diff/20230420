# Comparing `tmp/sqlfluff-2.0.5.tar.gz` & `tmp/sqlfluff-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-60oswayg/sqlfluff-2.0.5.tar", last modified: Fri Apr 14 21:23:13 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-qhi7531s/sqlfluff-2.0.6.tar", last modified: Thu Apr 20 09:29:28 2023, max compression
```

## Comparing `sqlfluff-2.0.5.tar` & `sqlfluff-2.0.6.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)   376831 2023-04-14 21:22:59.000000 sqlfluff-2.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 21:22:59.000000 sqlfluff-2.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 21:22:59.000000 sqlfluff-2.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-04-14 21:22:59.000000 sqlfluff-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/api/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/api/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/cli/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/cli/click_deprecated_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    43973 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    24252 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/cli/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/cli/outputstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/default_config.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/dialects/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/file_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/linted_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)    24458 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/linted_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    50049 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/linter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/linting_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/anyof.py
--rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/delimited.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/noncode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    34648 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/match_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/match_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/match_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/matchable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72950 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/plugin/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/plugin/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/plugin/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/config_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/crawlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/doc_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/slice_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/string_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20636 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24963 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/slicers/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/slicers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28534 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/slicers/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   130209 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_ansi_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_athena_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    68391 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_bigquery_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_databricks.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_databricks_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_db2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_db2_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    99588 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_exasol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_exasol_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_greenplum.py
--rw-r--r--   0 runner    (1001) docker     (123)    33201 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_hive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_hive_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_materialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_materialize_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    80857 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_mysql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)   166481 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    36696 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_postgres_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    69070 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_redshift_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)   200667 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_snowflake_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_soql.py
--rw-r--r--   0 runner    (1001) docker     (123)   103493 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sparksql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sparksql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sqlite_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    28206 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_teradata.py
--rw-r--r--   0 runner    (1001) docker     (123)   172382 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_tsql.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_tsql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/diff_quality_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL04.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL05.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL06.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL07.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM02.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM03.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM05.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM06.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM07.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP02.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP03.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP05.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV04.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV05.py
--rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV07.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV08.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV09.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV10.py
--rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV11.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/jinja/JJ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT02.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT03.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT04.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT05.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT07.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT08.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT09.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT11.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT12.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT13.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/RF01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/RF02.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/RF03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/RF04.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/RF05.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/RF06.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST01.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST02.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST04.py
--rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST05.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST06.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST07.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST08.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/tsql/
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/tsql/TQ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/tsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/utils/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/analysis/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/analysis/select_crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/raw_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/segment_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/templated_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/identifers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    31913 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/rebreak.py
--rw-r--r--   0 runner    (1001) docker     (123)    89766 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/reindent.py
--rw-r--r--   0 runner    (1001) docker     (123)    22930 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/respace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/testing/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/testing/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/test/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)   380758 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/api/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/cli/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/cli/click_deprecated_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44986 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24440 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/cli/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/cli/outputstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/default_config.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/dialects/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/file_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/linted_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/linted_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50768 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/linter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/linting_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/anyof.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/delimited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/noncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34592 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/match_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/match_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/matchable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72950 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/plugin/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/plugin/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/plugin/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/crawlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/doc_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/slice_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/string_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24963 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/slicers/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/slicers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28808 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/slicers/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129858 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_ansi_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_athena_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68071 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_bigquery_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17642 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_databricks_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_db2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_db2_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95470 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_exasol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_exasol_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32876 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_hive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_hive_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_materialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_materialize_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80702 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_mysql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165688 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36696 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_postgres_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69018 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_redshift_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)   200280 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_snowflake_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_soql.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102212 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sparksql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sparksql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sqlite_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_teradata.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172023 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_tsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_tsql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/diff_quality_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL06.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP05.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV05.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV08.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV09.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/jinja/JJ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT08.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT09.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/RF01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/RF02.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/RF03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/RF04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/RF05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/RF06.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST04.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST08.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/tsql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/tsql/TQ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/tsql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/utils/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/analysis/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/analysis/select_crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/raw_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/segment_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/templated_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/identifers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/rebreak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91962 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/reindent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/respace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/testing/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/testing/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/test/test_testing.py
```

### Comparing `sqlfluff-2.0.5/CHANGELOG.md` & `sqlfluff-2.0.6/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,56 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!--
 Note: Changes are now automatically tracked in [GitHub](https://github.com/sqlfluff/sqlfluff/releases) and will be copied in here on each release (please remember to update the issues and contributors to links!). There is no need to manually edit this file going forward.
 -->
 <!--Start Of Releases (DO NOT DELETE THIS LINE)-->
 
+## [2.0.6] - 2023-04-19
+
+## Highlights
+
+* Introduction of a `--quiet` option for the CLI for situations
+  where less output is useful.
+* When using the `--force` option is used for `sqlfluff fix` each
+  file is fixed during the linting process rather than at the end.
+* Bugfixes to comment and templated section indentation.
+* Performance improvements to parsing.
+* Bugfix to macros triggering LT01.
+* Renaming `layout.end-of-file` to `layout.end_of_file` in line
+  with other rules.
+* Dialect improvements to SparkSQL, BigQuery, Hive & Snowflake.
+
+
+## What’s Changed
+
+* Snowflake: Support Temporary View [#4789](https://github.com/sqlfluff/sqlfluff/pull/4789) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Inroduce `SAFE` prefix segment [#4773](https://github.com/sqlfluff/sqlfluff/pull/4773) [@dmohns](https://github.com/dmohns)
+* Fix #4660: Better handling of empty files. [#4780](https://github.com/sqlfluff/sqlfluff/pull/4780) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Fix #3538: (Fix files as we go) [#4777](https://github.com/sqlfluff/sqlfluff/pull/4777) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Fix #2855: (Tech debt: check consistency in TemplatedFile init) [#4776](https://github.com/sqlfluff/sqlfluff/pull/4776) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Add a --quiet option for fix [#4764](https://github.com/sqlfluff/sqlfluff/pull/4764) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Fix #4603 indent after Jinja 'do' directive [#4778](https://github.com/sqlfluff/sqlfluff/pull/4778) [@fredriv](https://github.com/fredriv)
+* Snowflake Execute Task with Schema [#4771](https://github.com/sqlfluff/sqlfluff/pull/4771) [@Thashin](https://github.com/Thashin)
+* SQLite: Support CreateTrigger [#4767](https://github.com/sqlfluff/sqlfluff/pull/4767) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Fix #2865 (AL05 exception for Redshift Semi-structured) [#4775](https://github.com/sqlfluff/sqlfluff/pull/4775) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Fix #4540: Untaken indents evaluation order. [#4768](https://github.com/sqlfluff/sqlfluff/pull/4768) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Use the new CollationReferenceSegment everywhere [#4770](https://github.com/sqlfluff/sqlfluff/pull/4770) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* SQLite: Fix multiple parse issues in Expression_A_Grammar [#4769](https://github.com/sqlfluff/sqlfluff/pull/4769) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* SQLite: Remove refs to RESPECT and QUALIFY [#4765](https://github.com/sqlfluff/sqlfluff/pull/4765) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* SQLite: Support STRICT [#4766](https://github.com/sqlfluff/sqlfluff/pull/4766) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Support hive set syntax [#4763](https://github.com/sqlfluff/sqlfluff/pull/4763) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Fix #4582: Comments after end of line [#4760](https://github.com/sqlfluff/sqlfluff/pull/4760) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Allow comment match with preceding line [#4758](https://github.com/sqlfluff/sqlfluff/pull/4758) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Remove the majority of greedy matchers [#4761](https://github.com/sqlfluff/sqlfluff/pull/4761) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Fix #4745: (max() error in reindent) [#4752](https://github.com/sqlfluff/sqlfluff/pull/4752) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Fix issue with macros triggering LT01 [#4757](https://github.com/sqlfluff/sqlfluff/pull/4757) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* end-of-file > end_of_file [#4753](https://github.com/sqlfluff/sqlfluff/pull/4753) [@alanmcruickshank](https://github.com/alanmcruickshank)
+
+
 ## [2.0.5] - 2023-04-14
 
 ## Highlights
 
 This is a relatively swift bugfix to refine some of the changes made to
 widow function indentation in `2.0.4`. In addition there are two dialect
 refinements also made since that release.
```

### Comparing `sqlfluff-2.0.5/LICENSE.md` & `sqlfluff-2.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/PKG-INFO` & `sqlfluff-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.0.5
+Version: 2.0.6
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
@@ -136,15 +136,15 @@
 L:   1 | P:  11 | LT01 | Expected only single space before binary operator '+'.
                        | Found '  '. [layout.spacing]
 L:   1 | P:  14 | LT01 | Expected only single space before naked identifier.
                        | Found '  '. [layout.spacing]
 L:   1 | P:  27 | LT01 | Unnecessary trailing whitespace at end of file.
                        | [layout.spacing]
 L:   1 | P:  27 | LT12 | Files must end with a single trailing newline.
-                       | [layout.end-of-file]
+                       | [layout.end_of_file]
 All Finished 📜 🎉!
 ```
 
 Alternatively, you can use the [**Official SQLFluff Docker Image**](https://hub.docker.com/r/sqlfluff/sqlfluff)
 or have a play using [**SQLFluff online**](https://online.sqlfluff.com/).
 
 For full [CLI usage](https://docs.sqlfluff.com/en/stable/cli.html) and
```

### Comparing `sqlfluff-2.0.5/README.md` & `sqlfluff-2.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 L:   1 | P:  11 | LT01 | Expected only single space before binary operator '+'.
                        | Found '  '. [layout.spacing]
 L:   1 | P:  14 | LT01 | Expected only single space before naked identifier.
                        | Found '  '. [layout.spacing]
 L:   1 | P:  27 | LT01 | Unnecessary trailing whitespace at end of file.
                        | [layout.spacing]
 L:   1 | P:  27 | LT12 | Files must end with a single trailing newline.
-                       | [layout.end-of-file]
+                       | [layout.end_of_file]
 All Finished 📜 🎉!
 ```
 
 Alternatively, you can use the [**Official SQLFluff Docker Image**](https://hub.docker.com/r/sqlfluff/sqlfluff)
 or have a play using [**SQLFluff online**](https://online.sqlfluff.com/).
 
 For full [CLI usage](https://docs.sqlfluff.com/en/stable/cli.html) and
```

### Comparing `sqlfluff-2.0.5/setup.cfg` & `sqlfluff-2.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff
-version = 2.0.5
+version = 2.0.6
 description = The SQL Linter for Humans
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -110,13 +110,13 @@
 [options.package_data]
 sqlfluff = 
 	config.ini
 	core/default_config.cfg
 	py.typed
 
 [sqlfluff_docs]
-stable_version = 2.0.5
+stable_version = 2.0.6
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/api/simple.py` & `sqlfluff-2.0.6/src/sqlfluff/api/simple.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/cli/autocomplete.py` & `sqlfluff-2.0.6/src/sqlfluff/cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/cli/click_deprecated_option.py` & `sqlfluff-2.0.6/src/sqlfluff/cli/click_deprecated_option.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/cli/commands.py` & `sqlfluff-2.0.6/src/sqlfluff/cli/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     FluffConfig,
     SQLLintError,
     SQLTemplaterError,
     SQLFluffUserError,
     dialect_selector,
     dialect_readout,
 )
+from sqlfluff.core.linter import LintingResult
 from sqlfluff.core.config import progress_bar_configuration
 
 from sqlfluff.core.enums import FormatType, Color
 from sqlfluff.core.plugin.host import get_plugin_manager
 
 
 class StreamHandlerTqdm(logging.StreamHandler):
@@ -687,32 +688,40 @@
         if not non_human_output:
             formatter.completion_message()
         sys.exit(result.stats()["exit code"])
     else:
         sys.exit(EXIT_SUCCESS)
 
 
-def do_fixes(lnt, result, formatter=None, **kwargs):
+def do_fixes(
+    result: LintingResult,
+    formatter: Optional[OutputStreamFormatter] = None,
+    fixed_file_suffix: str = "",
+):
     """Actually do the fixes."""
-    click.echo("Persisting Changes...")
-    res = result.persist_changes(formatter=formatter, **kwargs)
+    if formatter and formatter.verbosity >= 0:
+        click.echo("Persisting Changes...")
+    res = result.persist_changes(
+        formatter=formatter, fixed_file_suffix=fixed_file_suffix
+    )
     if all(res.values()):
-        click.echo("Done. Please check your files to confirm.")
+        if formatter and formatter.verbosity >= 0:
+            click.echo("Done. Please check your files to confirm.")
         return True
     # If some failed then return false
     click.echo(
         "Done. Some operations failed. Please check your files to confirm."
     )  # pragma: no cover
     click.echo(
         "Some errors cannot be fixed or there is another error blocking it."
     )  # pragma: no cover
     return False  # pragma: no cover
 
 
-def _stdin_fix(linter, formatter, fix_even_unparsable):
+def _stdin_fix(linter: Linter, formatter, fix_even_unparsable):
     """Handle fixing from stdin."""
     exit_code = EXIT_SUCCESS
     stdin = sys.stdin.read()
 
     result = linter.lint_string_wrapped(stdin, fname="stdin", fix=True)
     templater_error = result.num_violations(types=SQLTemplaterError) > 0
     unfixable_error = result.num_violations(types=SQLLintError, fixable=False) > 0
@@ -747,105 +756,103 @@
         )
 
     click.echo(stdout, nl=False)
     sys.exit(EXIT_FAIL if templater_error or unfixable_error else exit_code)
 
 
 def _paths_fix(
-    linter,
+    linter: Linter,
     formatter,
     paths,
     processes,
     fix_even_unparsable,
     force,
     fixed_suffix,
     bench,
     show_lint_violations,
     warn_force: bool = True,
     persist_timing: Optional[str] = None,
 ):
     """Handle fixing from paths."""
     # Lint the paths (not with the fix argument at this stage), outputting as we go.
-    click.echo("==== finding fixable violations ====")
+    if formatter.verbosity >= 0:
+        click.echo("==== finding fixable violations ====")
     exit_code = EXIT_SUCCESS
 
+    if force and warn_force and formatter.verbosity >= 0:
+        click.echo(
+            f"{formatter.colorize('FORCE MODE', Color.red)}: " "Attempting fixes..."
+        )
+
     with PathAndUserErrorHandler(formatter):
-        result = linter.lint_paths(
+        result: LintingResult = linter.lint_paths(
             paths,
             fix=True,
             ignore_non_existent_files=False,
             processes=processes,
+            # If --force is set, then apply the changes as we go rather
+            # than waiting until the end.
+            apply_fixes=force,
+            fixed_file_suffix=fixed_suffix,
+            fix_even_unparsable=fix_even_unparsable,
         )
 
     if not fix_even_unparsable:
         exit_code = formatter.handle_files_with_tmp_or_prs_errors(result)
 
     # NB: We filter to linting violations here, because they're
     # the only ones which can be potentially fixed.
-    if result.num_violations(types=SQLLintError, fixable=True) > 0:
-        click.echo("==== fixing violations ====")
-        click.echo(
-            f"{result.num_violations(types=SQLLintError, fixable=True)} fixable "
-            "linting violations found"
-        )
-        if force:
-            if warn_force:
-                click.echo(
-                    f"{formatter.colorize('FORCE MODE', Color.red)}: "
-                    "Attempting fixes..."
-                )
-            success = do_fixes(
-                linter,
-                result,
-                formatter,
-                types=SQLLintError,
-                fixed_file_suffix=fixed_suffix,
-            )
-            if not success:
-                sys.exit(EXIT_FAIL)  # pragma: no cover
-        else:
+    num_fixable = result.num_violations(types=SQLLintError, fixable=True)
+
+    if num_fixable > 0:
+        if not force and formatter.verbosity >= 0:
+            click.echo("==== fixing violations ====")
+
+        click.echo(f"{num_fixable} " "fixable linting violations found")
+
+        if not force:
             click.echo(
                 "Are you sure you wish to attempt to fix these? [Y/n] ", nl=False
             )
             c = click.getchar().lower()
             click.echo("...")
             if c in ("y", "\r", "\n"):
-                click.echo("Attempting fixes...")
+                if formatter.verbosity >= 0:
+                    click.echo("Attempting fixes...")
                 success = do_fixes(
-                    linter,
                     result,
                     formatter,
-                    types=SQLLintError,
                     fixed_file_suffix=fixed_suffix,
                 )
                 if not success:
                     sys.exit(EXIT_FAIL)  # pragma: no cover
                 else:
                     formatter.completion_message()
             elif c == "n":
                 click.echo("Aborting...")
                 exit_code = EXIT_FAIL
             else:  # pragma: no cover
                 click.echo("Invalid input, please enter 'Y' or 'N'")
                 click.echo("Aborting...")
                 exit_code = EXIT_FAIL
     else:
-        click.echo("==== no fixable linting violations found ====")
-        formatter.completion_message()
+        if formatter.verbosity >= 0:
+            click.echo("==== no fixable linting violations found ====")
+            formatter.completion_message()
 
     error_types = [
         (
             dict(types=SQLLintError, fixable=False),
             "  [{} unfixable linting violations found]",
             EXIT_FAIL,
         ),
     ]
     for num_violations_kwargs, message_format, error_level in error_types:
         num_violations = result.num_violations(**num_violations_kwargs)
-        if num_violations > 0:
+        if num_violations > 0 and formatter.verbosity >= 0:
             click.echo(message_format.format(num_violations))
             exit_code = max(exit_code, error_level)
 
     if bench:
         click.echo("==== overall timings ====")
         click.echo(formatter.cli_table([("Clock time", result.total_time)]))
         timing_summary = result.timing_summary()
@@ -876,16 +883,28 @@
 @core_options
 @lint_options
 @click.option(
     "-f",
     "--force",
     is_flag=True,
     help=(
-        "skip the confirmation prompt and go straight to applying "
-        "fixes. **Use this with caution.**"
+        "Skip the confirmation prompt and go straight to applying "
+        "fixes. Fixes will also be applied file by file, during the "
+        "linting process, rather than waiting until all files are "
+        "linted before fixing. **Use this with caution.**"
+    ),
+)
+@click.option(
+    "-q",
+    "--quiet",
+    is_flag=True,
+    help=(
+        "Reduces the amount of output to stdout to a minimal level. "
+        "This is effectively the opposite of -v. NOTE: It will only "
+        "take effect if -f/--force is also set."
     ),
 )
 @click.option(
     "-x",
     "--fixed-suffix",
     default=None,
     help="An optional suffix to add to fixed files.",
@@ -909,14 +928,15 @@
     help="Show lint violations",
 )
 @click.argument("paths", nargs=-1, type=click.Path(allow_dash=True))
 def fix(
     force: bool,
     paths: Tuple[str],
     bench: bool = False,
+    quiet: bool = False,
     fixed_suffix: str = "",
     logger: Optional[logging.Logger] = None,
     processes: Optional[int] = None,
     disable_progress_bar: Optional[bool] = False,
     persist_timing: Optional[str] = None,
     extra_config_path: Optional[str] = None,
     ignore_local_config: bool = False,
@@ -928,14 +948,21 @@
     PATH is the path to a sql file or directory to lint. This can be either a
     file ('path/to/file.sql'), a path ('directory/of/sql/files'), a single ('-')
     character to indicate reading from *stdin* or a dot/blank ('.'/' ') which will
     be interpreted like passing the current working directory as a path argument.
     """
     # some quick checks
     fixing_stdin = ("-",) == paths
+    if quiet:
+        if kwargs["verbose"]:
+            click.echo(
+                "ERROR: The --quiet flag can only be used if --verbose is not set.",
+            )
+            sys.exit(EXIT_ERROR)
+        kwargs["verbose"] = -1
 
     config = get_config(
         extra_config_path, ignore_local_config, require_dialect=False, **kwargs
     )
     fix_even_unparsable = config.get("fix_even_unparsable")
     output_stream = make_output_stream(
         config, None, os.devnull if fixing_stdin else None
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/cli/formatters.py` & `sqlfluff-2.0.6/src/sqlfluff/cli/formatters.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         nocolor: bool,
         verbosity: int = 0,
         filter_empty: bool = True,
         output_line_length: int = 80,
     ):
         self._output_stream = output_stream
         self.plain_output = self.should_produce_plain_output(nocolor)
-        self._verbosity = verbosity
+        self.verbosity = verbosity
         self._filter_empty = filter_empty
         self.output_line_length = output_line_length
 
     @staticmethod
     def should_produce_plain_output(nocolor: bool) -> bool:
         """Returns True if text output should be plain (not colored)."""
         return nocolor or not sys.stdout.isatty()
@@ -112,21 +112,21 @@
         if (not self._filter_empty) or s.strip(" \n\t"):
             self._output_stream.write(s)
 
     def _format_config(self, linter: Linter) -> str:
         """Format the config of a `Linter`."""
         text_buffer = StringIO()
         # Only show version information if verbosity is high enough
-        if self._verbosity > 0:
+        if self.verbosity > 0:
             text_buffer.write("==== sqlfluff ====\n")
             config_content = [
                 ("sqlfluff", get_package_version()),
                 ("python", get_python_version()),
                 ("implementation", get_python_implementation()),
-                ("verbosity", self._verbosity),
+                ("verbosity", self.verbosity),
             ]
             if linter.dialect:
                 config_content.append(("dialect", linter.dialect.name))
             config_content += linter.templater.config_pairs()
             text_buffer.write(
                 self.cli_table(config_content, col_width=30, max_label_width=15)
             )
@@ -134,43 +134,43 @@
             if linter.config.get("rule_allowlist"):
                 text_buffer.write(
                     self.cli_table(
                         [("rules", ", ".join(linter.config.get("rule_allowlist")))],
                         col_width=41,
                     )
                 )
-            if self._verbosity > 1:
+            if self.verbosity > 1:
                 text_buffer.write("\n== Raw Config:\n")
                 text_buffer.write(self.format_config_vals(linter.config.iter_vals()))
         return text_buffer.getvalue()
 
     def dispatch_config(self, linter: Linter) -> None:
         """Dispatch configuration output appropriately."""
         self._dispatch(self._format_config(linter))
 
     def dispatch_persist_filename(self, filename, result):
         """Dispatch filenames during a persist operation."""
         # Only show the skip records at higher levels of verbosity
-        if self._verbosity >= 2 or result != "SKIP":
+        if self.verbosity >= 2 or result != "SKIP":
             self._dispatch(self.format_filename(filename=filename, success=result))
 
     def _format_path(self, path: str) -> str:
         """Format paths."""
         return f"=== [ path: {self.colorize(path, Color.lightgrey)} ] ===\n"
 
     def dispatch_path(self, path: str) -> None:
         """Dispatch paths for display."""
-        if self._verbosity > 0:
+        if self.verbosity > 0:
             self._dispatch(self._format_path(path))
 
     def dispatch_template_header(
         self, fname: str, linter_config: FluffConfig, file_config: FluffConfig
     ) -> None:
         """Dispatch the header displayed before templating."""
-        if self._verbosity > 1:
+        if self.verbosity > 1:
             self._dispatch(self.format_filename(filename=fname, success="TEMPLATING"))
             # This is where we output config diffs if they exist.
             if file_config:
                 # Only output config diffs if there is a config to diff to.
                 config_diff = file_config.diff_to(linter_config)
                 if config_diff:  # pragma: no cover
                     self._dispatch("   Config Diff:")
@@ -178,35 +178,35 @@
                         self.format_config_vals(
                             linter_config.iter_vals(cfg=config_diff)
                         )
                     )
 
     def dispatch_parse_header(self, fname: str) -> None:
         """Dispatch the header displayed before parsing."""
-        if self._verbosity > 1:
+        if self.verbosity > 1:
             self._dispatch(self.format_filename(filename=fname, success="PARSING"))
 
     def dispatch_lint_header(self, fname: str, rules: List[str]) -> None:
         """Dispatch the header displayed before linting."""
-        if self._verbosity > 1:
+        if self.verbosity > 1:
             self._dispatch(
                 self.format_filename(
                     filename=fname, success=f"LINTING ({', '.join(rules)})"
                 )
             )
 
     def dispatch_compilation_header(self, templater, message):
         """Dispatch the header displayed before linting."""
         self._dispatch(
             f"=== [{self.colorize(templater, Color.lightgrey)}] {message}"
         )  # pragma: no cover
 
     def dispatch_processing_header(self, processes: int) -> None:
         """Dispatch the header displayed before linting."""
-        if self._verbosity > 0:
+        if self.verbosity > 0:
             self._dispatch(  # pragma: no cover
                 f"{self.colorize('effective configured processes: ', Color.lightgrey)} "
                 f"{processes}"
             )
 
     def dispatch_dialect_warning(self, dialect) -> None:
         """Dispatch a warning for dialects."""
@@ -224,15 +224,15 @@
             int(not violation.ignore and not violation.warning)
             for violation in violations
         )
         warns = sum(int(violation.warning) for violation in violations)
         show = fails + warns > 0
 
         # Only print the filename if it's either a failure or verbosity > 1
-        if self._verbosity > 0 or show:
+        if self.verbosity > 0 or show:
             text_buffer.write(self.format_filename(fname, success=fails == 0))
             text_buffer.write("\n")
 
         # If we have violations, print them
         if show:
             # sort by position in file (using line number and position)
             s = sorted(violations, key=lambda v: (v.line_no, v.line_pos))
@@ -249,14 +249,16 @@
             str_buffer = str_buffer[:-1]
         return str_buffer
 
     def dispatch_file_violations(
         self, fname: str, linted_file: LintedFile, only_fixable: bool
     ) -> None:
         """Dispatch any violations found in a file."""
+        if self.verbosity < 0:
+            return
         s = self._format_file_violations(
             fname,
             linted_file.get_violations(
                 fixable=True if only_fixable else None, filter_warning=False
             ),
         )
         self._dispatch(s)
@@ -388,18 +390,21 @@
         success: Union[str, bool] = False,
         success_text: str = "PASS",
     ) -> str:
         """Format filenames."""
         if isinstance(success, str):
             status_string = success
         else:
-            status_string = self.colorize(
-                success_text if success else "FAIL",
-                Color.green if success else Color.red,
-            )
+            status_string = success_text if success else "FAIL"
+
+        if status_string in ("PASS", "FIXED", success_text):
+            status_string = self.colorize(status_string, Color.green)
+        elif status_string in ("FAIL", "ERROR"):
+            status_string = self.colorize(status_string, Color.red)
+
         return f"== [{self.colorize(filename, Color.lightgrey)}] {status_string}"
 
     def format_violation(
         self, violation: SQLBaseError, max_line_length: int = 90
     ) -> str:
         """Format a violation."""
         if not isinstance(violation, SQLBaseError):  # pragma: no cover
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/cli/helpers.py` & `sqlfluff-2.0.6/src/sqlfluff/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/cli/outputstream.py` & `sqlfluff-2.0.6/src/sqlfluff/cli/outputstream.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/config.py` & `sqlfluff-2.0.6/src/sqlfluff/core/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/default_config.cfg` & `sqlfluff-2.0.6/src/sqlfluff/core/default_config.cfg`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/dialects/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/core/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/dialects/base.py` & `sqlfluff-2.0.6/src/sqlfluff/core/dialects/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/dialects/common.py` & `sqlfluff-2.0.6/src/sqlfluff/core/dialects/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/enums.py` & `sqlfluff-2.0.6/src/sqlfluff/core/enums.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/errors.py` & `sqlfluff-2.0.6/src/sqlfluff/core/errors.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/linter/common.py` & `sqlfluff-2.0.6/src/sqlfluff/core/linter/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/linter/linted_dir.py` & `sqlfluff-2.0.6/src/sqlfluff/core/linter/linted_dir.py`

 * *Files 10% similar despite different names*

```diff
@@ -102,32 +102,26 @@
             files=len(self.files),
             clean=sum(file.is_clean() for file in self.files),
             unclean=sum(not file.is_clean() for file in self.files),
             violations=sum(file.num_violations() for file in self.files),
         )
 
     def persist_changes(
-        self, formatter: Any = None, fixed_file_suffix: str = "", **kwargs
+        self, formatter: Any = None, fixed_file_suffix: str = ""
     ) -> Dict[str, Union[bool, str]]:
         """Persist changes to files in the given path.
 
         This also logs the output as we go using the formatter if present.
         """
         # Run all the fixes for all the files and return a dict
         buffer: Dict[str, Union[bool, str]] = {}
         for file in self.files:
-            if file.num_violations(fixable=True, **kwargs) > 0:
-                buffer[file.path] = file.persist_tree(suffix=fixed_file_suffix)
-                result = buffer[file.path]
-            else:  # pragma: no cover TODO?
-                buffer[file.path] = True
-                result = "SKIP"
-
-            if formatter:
-                formatter.dispatch_persist_filename(filename=file.path, result=result)
+            buffer[file.path] = file.persist_tree(
+                suffix=fixed_file_suffix, formatter=formatter
+            )
         return buffer
 
     @property
     def tree(self) -> Optional[BaseSegment]:
         """A convenience method for when there is only one file and we want the tree."""
         if len(self.files) > 1:  # pragma: no cover
             raise ValueError(
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/linter/linted_file.py` & `sqlfluff-2.0.6/src/sqlfluff/core/linter/linted_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,26 +24,30 @@
     Type,
     Dict,
 )
 
 from sqlfluff.core.errors import (
     SQLBaseError,
     SQLLintError,
+    SQLParseError,
+    SQLTemplaterError,
     CheckTuple,
 )
 from sqlfluff.core.templaters import TemplatedFile, RawFileSlice
 
 # Classes needed only for type checking
 from sqlfluff.core.parser.segments import BaseSegment, FixPatch
 
 from sqlfluff.core.linter.common import NoQaDirective
 
 # Instantiate the linter logger
 linter_logger: logging.Logger = logging.getLogger("sqlfluff.linter")
 
+TMP_PRS_ERROR_TYPES = (SQLTemplaterError, SQLParseError)
+
 
 @dataclass
 class FileTimings:
     """A dataclass for holding the timings information for a file."""
 
     step_timings: Dict[str, float]
     # NOTE: Because rules may run more than once for any
@@ -552,27 +556,54 @@
                     "Appending Raw:                    %s     %r",
                     source_slice,
                     raw_source_string[source_slice],
                 )
                 str_buff += raw_source_string[source_slice]
         return str_buff
 
-    def persist_tree(self, suffix: str = "") -> bool:
+    def persist_tree(self, suffix: str = "", formatter: Any = None) -> bool:
         """Persist changes to the given path."""
-        write_buff, success = self.fix_string()
+        if self.num_violations(fixable=True) > 0:
+            write_buff, success = self.fix_string()
+
+            if success:
+                fname = self.path
+                # If there is a suffix specified, then use it.s
+                if suffix:
+                    root, ext = os.path.splitext(fname)
+                    fname = root + suffix + ext
+                self._safe_create_replace_file(
+                    self.path, fname, write_buff, self.encoding
+                )
+                result_label = "FIXED"
+            else:  # pragma: no cover
+                result_label = "FAIL"
+        else:
+            result_label = "SKIP"
+            success = True
+
+        if formatter:
+            formatter.dispatch_persist_filename(filename=self.path, result=result_label)
 
-        if success:
-            fname = self.path
-            # If there is a suffix specified, then use it.s
-            if suffix:
-                root, ext = os.path.splitext(fname)
-                fname = root + suffix + ext
-            self._safe_create_replace_file(self.path, fname, write_buff, self.encoding)
         return success
 
+    def discard_fixes_if_tmp_or_prs_errors(self) -> None:
+        """Discard lint fixes for files with templating or parse errors."""
+        num_errors = self.num_violations(
+            types=TMP_PRS_ERROR_TYPES,
+            filter_ignore=False,
+            filter_warning=False,
+        )
+        if num_errors:
+            # File has errors. Discard all the SQLLintError fixes:
+            # they are potentially unsafe.
+            for violation in self.violations:
+                if isinstance(violation, SQLLintError):
+                    violation.fixes = []
+
     @staticmethod
     def _safe_create_replace_file(
         input_path: str, output_path: str, write_buff: str, encoding: str
     ):
         # Write to a temporary file first, so in case of encoding or other
         # issues, we don't delete or corrupt the user's existing file.
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/linter/linter.py` & `sqlfluff-2.0.6/src/sqlfluff/core/linter/linter.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,19 @@
 
 from sqlfluff.core.linter.common import (
     RuleTuple,
     ParsedString,
     NoQaDirective,
     RenderedFile,
 )
-from sqlfluff.core.linter.linted_file import LintedFile, FileTimings
+from sqlfluff.core.linter.linted_file import (
+    LintedFile,
+    FileTimings,
+    TMP_PRS_ERROR_TYPES,
+)
 from sqlfluff.core.linter.linted_dir import LintedDir
 from sqlfluff.core.linter.linting_result import LintingResult
 
 
 WalkableType = Iterable[Tuple[str, Optional[List[str]], List[str]]]
 RuleTimingsType = List[Tuple[str, str, float]]
 
@@ -185,15 +189,15 @@
         templating_blocks_indent = bool(templating_blocks_indent)
         # If we're forcing it through we don't check.
         if templating_blocks_indent and not force_block_indent:
             indent_balance = sum(
                 getattr(elem, "indent_val", 0)
                 for elem in cast(Tuple[BaseSegment, ...], tokens)
             )
-            if indent_balance != 0:
+            if indent_balance != 0:  # pragma: no cover
                 linter_logger.debug(
                     "Indent balance test failed for %r. Template indents will not be "
                     "linted for this file.",
                     templated_file.fname,
                 )
                 # Don't enable the templating blocks.
                 templating_blocks_indent = False
@@ -203,15 +207,15 @@
         new_tokens = []
         for token in cast(Tuple[BaseSegment, ...], tokens):
             if token.is_meta:
                 token = cast(MetaSegment, token)
                 if token.indent_val != 0:
                     # Don't allow it if we're not linting templating block indents.
                     if not templating_blocks_indent:
-                        continue
+                        continue  # pragma: no cover
             new_tokens.append(token)
 
         # Return new buffer
         return new_tokens, violations, config
 
     @staticmethod
     def _parse_tokens(
@@ -378,15 +382,15 @@
         rendered: RenderedFile,
         recurse: bool = True,
     ) -> ParsedString:
         """Parse a rendered file."""
         t0 = time.monotonic()
         violations = cast(List[SQLBaseError], rendered.templater_violations)
         tokens: Optional[Sequence[BaseSegment]]
-        if rendered.templated_file:
+        if rendered.templated_file is not None:
             tokens, lvs, config = cls._lex_templated_file(
                 rendered.templated_file, rendered.config
             )
             violations += lvs
         else:
             tokens = None
 
@@ -847,15 +851,15 @@
                 in_str=in_str, fname=fname, config=config, formatter=self.formatter
             )
         except SQLFluffSkipFile as s:  # pragma: no cover
             linter_logger.warning(str(s))
             templated_file = None
             templater_violations = []
 
-        if not templated_file:
+        if templated_file is None:
             linter_logger.info("TEMPLATING FAILED: %s", templater_violations)
 
         # Record time
         time_dict = {"templating": time.monotonic() - t0}
 
         return RenderedFile(
             templated_file,
@@ -1145,14 +1149,17 @@
     def lint_paths(
         self,
         paths: Tuple[str, ...],
         fix: bool = False,
         ignore_non_existent_files: bool = False,
         ignore_files: bool = True,
         processes: Optional[int] = None,
+        apply_fixes: bool = False,
+        fixed_file_suffix: str = "",
+        fix_even_unparsable: bool = False,
     ) -> LintingResult:
         """Lint an iterable of paths."""
         # If no paths specified - assume local
         if not paths:  # pragma: no cover
             paths = (os.getcwd(),)
         # Set up the result to hold what we get back
         result = LintingResult()
@@ -1200,14 +1207,26 @@
             linted_dir = expanded_path_to_linted_dir[linted_file.path]
             linted_dir.add(linted_file)
             # If any fatal errors, then stop iteration.
             if any(v.fatal for v in linted_file.violations):  # pragma: no cover
                 linter_logger.error("Fatal linting error. Halting further linting.")
                 break
 
+            # If we're applying fixes, then do that here.
+            if apply_fixes:
+                num_tmp_prs_errors = linted_file.num_violations(
+                    types=TMP_PRS_ERROR_TYPES,
+                    filter_ignore=False,
+                    filter_warning=False,
+                )
+                if fix_even_unparsable or num_tmp_prs_errors == 0:
+                    linted_file.persist_tree(
+                        suffix=fixed_file_suffix, formatter=self.formatter
+                    )
+
             # Progress bar for files is rendered only when there is more than one file.
             # Additionally, as it's updated after each loop, we need to get file name
             # from the next loop. This is why `enumerate` starts with `1` and there
             # is `i < len` to not exceed files list length.
             progress_bar_files.update(n=1)
             if i < len(expanded_paths):
                 progress_bar_files.set_description(f"file {expanded_paths[i]}")
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/linter/linting_result.py` & `sqlfluff-2.0.6/src/sqlfluff/core/linter/linting_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,24 +14,22 @@
 )
 from typing_extensions import Literal
 
 from sqlfluff.cli import EXIT_FAIL, EXIT_SUCCESS
 
 from sqlfluff.core.errors import (
     CheckTuple,
-    SQLLintError,
-    SQLParseError,
-    SQLTemplaterError,
 )
 
 from sqlfluff.core.timing import TimingSummary, RuleTimingSummary
 
 # Classes needed only for type checking
 from sqlfluff.core.parser.segments.base import BaseSegment
 from sqlfluff.core.linter.linted_dir import LintedDir
+from sqlfluff.core.linter.linted_file import TMP_PRS_ERROR_TYPES
 
 
 class LintingResult:
     """A class to represent the result of a linting operation.
 
     Notably this might be a collection of paths, all with multiple
     potential files within them.
@@ -233,60 +231,54 @@
                 ),
             }
             for LintedDir in self.paths
             for path, violations in LintedDir.violation_dict().items()
             if violations
         ]
 
-    def persist_changes(self, formatter, **kwargs) -> dict:
+    def persist_changes(self, formatter, fixed_file_suffix: str = "") -> dict:
         """Run all the fixes for all the files and return a dict."""
         return self.combine_dicts(
             *(
-                path.persist_changes(formatter=formatter, **kwargs)
+                path.persist_changes(
+                    formatter=formatter, fixed_file_suffix=fixed_file_suffix
+                )
                 for path in self.paths
             )
         )
 
     @property
     def tree(self) -> Optional[BaseSegment]:  # pragma: no cover
         """A convenience method for when there is only one file and we want the tree."""
         if len(self.paths) > 1:
             raise ValueError(
                 ".tree() cannot be called when a LintingResult contains more than one "
                 "path."
             )
         return self.paths[0].tree
 
-    TMP_PRS_ERROR_TYPES = (SQLTemplaterError, SQLParseError)
-
     def count_tmp_prs_errors(self) -> Tuple[int, int]:
         """Count templating or parse errors before and after filtering."""
         total_errors = self.num_violations(
-            types=self.TMP_PRS_ERROR_TYPES, filter_ignore=False, filter_warning=False
+            types=TMP_PRS_ERROR_TYPES,
+            filter_ignore=False,
+            filter_warning=False,
         )
         num_filtered_errors = 0
         for linted_dir in self.paths:
             for linted_file in linted_dir.files:
                 num_filtered_errors += linted_file.num_violations(
-                    types=self.TMP_PRS_ERROR_TYPES
+                    types=TMP_PRS_ERROR_TYPES
                 )
         return total_errors, num_filtered_errors
 
     def discard_fixes_for_lint_errors_in_files_with_tmp_or_prs_errors(self) -> None:
         """Discard lint fixes for files with templating or parse errors."""
         total_errors = self.num_violations(
-            types=self.TMP_PRS_ERROR_TYPES, filter_ignore=False, filter_warning=False
+            types=TMP_PRS_ERROR_TYPES,
+            filter_ignore=False,
+            filter_warning=False,
         )
         if total_errors:
             for linted_dir in self.paths:
                 for linted_file in linted_dir.files:
-                    num_errors = linted_file.num_violations(
-                        types=self.TMP_PRS_ERROR_TYPES,
-                        filter_ignore=False,
-                        filter_warning=False,
-                    )
-                    if num_errors:
-                        # File has errors. Discard all the SQLLintError fixes:
-                        # they are potentially unsafe.
-                        for violation in linted_file.violations:
-                            if isinstance(violation, SQLLintError):
-                                violation.fixes = []
+                    linted_file.discard_fixes_if_tmp_or_prs_errors()
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/linter/runner.py` & `sqlfluff-2.0.6/src/sqlfluff/core/linter/runner.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/context.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/anyof.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/anyof.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/base.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/conditional.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/conditional.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/delimited.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/delimited.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/greedy.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/greedy.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/noncode.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/noncode.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/sequence.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/helpers.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/lexer.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,22 +443,22 @@
         tfs.slice_type,
         templated_file,
     )
 
 
 def _iter_segments(
     lexed_elements: List[TemplateElement],
-    templated_file_slices: List[TemplatedFileSlice],
     templated_file: TemplatedFile,
     add_indents: bool = True,
 ) -> Iterator[RawSegment]:
     # An index to track where we've got to in the templated file.
     tfs_idx = 0
     # We keep a map of previous block locations in case they re-occur.
     block_stack = BlockTracker()
+    templated_file_slices = templated_file.sliced_file
 
     # Now work out source slices, and add in template placeholders.
     for idx, element in enumerate(lexed_elements):
         # We're working through elements in the rendered file.
         # When they enter this code they don't have a position in the source.
         # We already have a map of how templated elements map to the source file
         # so we work through them to work out what's going on. In theory we can
@@ -767,17 +767,15 @@
         self, elements: List[TemplateElement], templated_file: TemplatedFile
     ) -> Tuple[RawSegment, ...]:
         """Convert a tuple of lexed elements into a tuple of segments."""
         lexer_logger.info("Elements to Segments.")
         add_indents = self.config.get("template_blocks_indent", "indentation")
         # Delegate to _iter_segments
         segment_buffer: List[RawSegment] = list(
-            _iter_segments(
-                elements, templated_file.sliced_file, templated_file, add_indents
-            )
+            _iter_segments(elements, templated_file, add_indents)
         )
 
         # Add an end of file marker
         segment_buffer.append(
             EndOfFile(
                 pos_marker=segment_buffer[-1].pos_marker.end_point_marker()
                 if segment_buffer
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/markers.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/markers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/match_logging.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/match_logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/match_result.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/match_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/match_wrapper.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/match_wrapper.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/matchable.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/matchable.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/parser.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/parser.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/parsers.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/parsers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/base.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/ephemeral.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/ephemeral.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/generator.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/generator.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/meta.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/meta.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/raw.py` & `sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/raw.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/plugin/hookspecs.py` & `sqlfluff-2.0.6/src/sqlfluff/core/plugin/hookspecs.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/plugin/lib.py` & `sqlfluff-2.0.6/src/sqlfluff/core/plugin/lib.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/rules/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/core/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/rules/base.py` & `sqlfluff-2.0.6/src/sqlfluff/core/rules/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/rules/config_info.py` & `sqlfluff-2.0.6/src/sqlfluff/core/rules/config_info.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/rules/context.py` & `sqlfluff-2.0.6/src/sqlfluff/core/rules/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/rules/crawlers.py` & `sqlfluff-2.0.6/src/sqlfluff/core/rules/crawlers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/rules/doc_decorators.py` & `sqlfluff-2.0.6/src/sqlfluff/core/rules/doc_decorators.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/rules/loader.py` & `sqlfluff-2.0.6/src/sqlfluff/core/rules/loader.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/rules/reference.py` & `sqlfluff-2.0.6/src/sqlfluff/core/rules/reference.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/slice_helpers.py` & `sqlfluff-2.0.6/src/sqlfluff/core/slice_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/string_helpers.py` & `sqlfluff-2.0.6/src/sqlfluff/core/string_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/templaters/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/core/templaters/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/templaters/base.py` & `sqlfluff-2.0.6/src/sqlfluff/core/templaters/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,100 +116,101 @@
     def __init__(
         self,
         source_str: str,
         fname: str,
         templated_str: Optional[str] = None,
         sliced_file: Optional[List[TemplatedFileSlice]] = None,
         raw_sliced: Optional[List[RawFileSlice]] = None,
-        check_consistency=True,
     ):
         """Initialise the TemplatedFile.
 
         If no templated_str is provided then we assume that
         the file is NOT templated and that the templated view
         is the same as the source view.
         """
         self.source_str = source_str
         # An empty string is still allowed as the templated string.
         self.templated_str = source_str if templated_str is None else templated_str
         # If no fname, we assume this is from a string or stdin.
         self.fname = fname
         # Assume that no sliced_file, means the file is not templated
-        # TODO: Enable error handling.
-        if (
-            not sliced_file
-        ) and self.templated_str != self.source_str:  # pragma: no cover
-            raise ValueError("Cannot instantiate a templated file unsliced!")
-        # If we get here and we don't have sliced files, then it's raw, so create them.
-        self.sliced_file: List[TemplatedFileSlice] = sliced_file or [
-            TemplatedFileSlice(
-                "literal", slice(0, len(source_str)), slice(0, len(source_str))
-            )
-        ]
-        self.raw_sliced: List[RawFileSlice] = raw_sliced or [
-            RawFileSlice(source_str, "literal", 0)
-        ]
+        self.sliced_file: List[TemplatedFileSlice]
+        if sliced_file is None:
+            if self.templated_str != self.source_str:  # pragma: no cover
+                raise ValueError("Cannot instantiate a templated file unsliced!")
+            # If we get here and we don't have sliced files,
+            # then it's raw, so create them.
+            self.sliced_file = [
+                TemplatedFileSlice(
+                    "literal", slice(0, len(source_str)), slice(0, len(source_str))
+                )
+            ]
+            assert (
+                raw_sliced is None
+            ), "Templated file was not sliced, but not has raw slices."
+            self.raw_sliced: List[RawFileSlice] = [
+                RawFileSlice(source_str, "literal", 0)
+            ]
+        else:
+            self.sliced_file = sliced_file
+            assert raw_sliced is not None, "Templated file was sliced, but not raw."
+            self.raw_sliced = raw_sliced
+
         # Precalculate newlines, character positions.
         self._source_newlines = list(iter_indices_of_newlines(self.source_str))
         self._templated_newlines = list(iter_indices_of_newlines(self.templated_str))
 
-        # NOTE: The "check_consistency" flag should always be True when using
-        # SQLFluff in real life. This flag was only added because some legacy
-        # templater tests in test/core/templaters/jinja_test.py use hardcoded
-        # test data with issues that will trigger errors here. It would be cool
-        # to fix that data someday. I (Barry H.) started looking into it, but
-        # it was much trickier than I expected, because bits of the same data
-        # are shared across multiple tests.
-        if check_consistency:
-            # Sanity check raw string and slices.
-            pos = 0
-            rfs: RawFileSlice
-            for idx, rfs in enumerate(self.raw_sliced):
-                assert rfs.source_idx == pos
-                pos += len(rfs.raw)
-            assert pos == len(self.source_str)
-
-            # Sanity check templated string and slices.
-            previous_slice = None
-            tfs: Optional[TemplatedFileSlice] = None
-            for idx, tfs in enumerate(self.sliced_file):
-                if previous_slice:
-                    if tfs.templated_slice.start != previous_slice.templated_slice.stop:
-                        raise SQLFluffSkipFile(  # pragma: no cover
-                            "Templated slices found to be non-contiguous. "
-                            f"{tfs.templated_slice} (starting"
-                            f" {self.templated_str[tfs.templated_slice]!r})"
-                            f" does not follow {previous_slice.templated_slice} "
-                            "(starting "
-                            f"{self.templated_str[previous_slice.templated_slice]!r}"
-                            ")"
-                        )
-                else:
-                    if tfs.templated_slice.start != 0:
-                        raise SQLFluffSkipFile(  # pragma: no cover
-                            "First Templated slice not started at index 0 "
-                            f"(found slice {tfs.templated_slice})"
-                        )
-                previous_slice = tfs
-            if self.sliced_file and templated_str is not None:
-                if tfs.templated_slice.stop != len(templated_str):
+        # Consistency check raw string and slices.
+        pos = 0
+        rfs: RawFileSlice
+        for rfs in self.raw_sliced:
+            assert rfs.source_idx == pos, (
+                "TemplatedFile. Consistency fail on running source length"
+                f": {pos} != {rfs.source_idx}"
+            )
+            pos += len(rfs.raw)
+        assert pos == len(self.source_str), (
+            "TemplatedFile. Consistency fail on total source length"
+            f": {pos} != {len(self.source_str)}"
+        )
+
+        # Consistency check templated string and slices.
+        previous_slice = None
+        tfs: Optional[TemplatedFileSlice] = None
+        for tfs in self.sliced_file:
+            if previous_slice:
+                if tfs.templated_slice.start != previous_slice.templated_slice.stop:
                     raise SQLFluffSkipFile(  # pragma: no cover
-                        "Length of templated file mismatch with final slice: "
-                        f"{len(templated_str)} != {tfs.templated_slice.stop}."
+                        "Templated slices found to be non-contiguous. "
+                        f"{tfs.templated_slice} (starting"
+                        f" {self.templated_str[tfs.templated_slice]!r})"
+                        f" does not follow {previous_slice.templated_slice} "
+                        "(starting "
+                        f"{self.templated_str[previous_slice.templated_slice]!r}"
+                        ")"
                     )
+            else:
+                if tfs.templated_slice.start != 0:
+                    raise SQLFluffSkipFile(  # pragma: no cover
+                        "First Templated slice not started at index 0 "
+                        f"(found slice {tfs.templated_slice})"
+                    )
+            previous_slice = tfs
+        if self.sliced_file and templated_str is not None:
+            if tfs.templated_slice.stop != len(templated_str):
+                raise SQLFluffSkipFile(  # pragma: no cover
+                    "Length of templated file mismatch with final slice: "
+                    f"{len(templated_str)} != {tfs.templated_slice.stop}."
+                )
 
     @classmethod
     def from_string(cls, raw):
         """Create TemplatedFile from a string."""
         return cls(source_str=raw, fname="<string>")
 
-    def __bool__(self):
-        """Return true if there's a templated file."""
-        return bool(self.templated_str)
-
     def __repr__(self):  # pragma: no cover TODO?
         return "<TemplatedFile>"
 
     def __str__(self):
         """Return the templated file if coerced to string."""
         return self.templated_str
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/templaters/jinja.py` & `sqlfluff-2.0.6/src/sqlfluff/core/templaters/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/templaters/placeholder.py` & `sqlfluff-2.0.6/src/sqlfluff/core/templaters/placeholder.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/templaters/python.py` & `sqlfluff-2.0.6/src/sqlfluff/core/templaters/python.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/templaters/slicers/tracer.py` & `sqlfluff-2.0.6/src/sqlfluff/core/templaters/slicers/tracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,20 @@
         )
         trace_template = self.make_template(trace_template_str)
         trace_template_output = trace_template.render()
         # Split output by section. Each section has two possible formats.
         trace_entries: List[regex.Match] = list(
             regex.finditer(r"\0", trace_template_output)
         )
+        # If the file has no templated entries, we should just iterate
+        # through the raw slices to add all the placeholders.
+        if not trace_entries:
+            for raw_idx, _ in enumerate(self.raw_sliced):
+                self.record_trace(0, raw_idx)
+
         for match_idx, match in enumerate(trace_entries):
             pos1 = match.span()[0]
             try:
                 pos2 = trace_entries[match_idx + 1].span()[0]
             except IndexError:
                 pos2 = len(trace_template_output)
             p = trace_template_output[pos1 + 1 : pos2]
@@ -520,15 +526,15 @@
     @staticmethod
     def extract_block_type(tag_name, block_subtype):
         """Determine block type."""
         # :TRICKY: Syntactically, the Jinja {% include %} directive looks like
         # a block, but its behavior is basically syntactic sugar for
         # {{ open("somefile).read() }}. Thus, treat it as templated code.
         # It's a similar situation with {% import %} and {% from ... import %}.
-        if tag_name in ["include", "import", "from"]:
+        if tag_name in ["include", "import", "from", "do"]:
             block_type = "templated"
         elif tag_name.startswith("end"):
             block_type = "block_end"
         elif tag_name.startswith("el"):
             # else, elif
             block_type = "block_mid"
         else:
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/core/timing.py` & `sqlfluff-2.0.6/src/sqlfluff/core/timing.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_ansi.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_ansi.py`

 * *Files 0% similar despite different names*

```diff
@@ -601,14 +601,15 @@
             # now, the most reliable (and impactful) is the comma.
             # Others could include some variant on AliasExpressionSegment.
         ],
     ),
     FilterClauseGrammar=Sequence(
         "FILTER", Bracketed(Sequence("WHERE", Ref("ExpressionSegment")))
     ),
+    IgnoreRespectNullsGrammar=Sequence(OneOf("IGNORE", "RESPECT"), "NULLS"),
     FrameClauseUnitGrammar=OneOf("ROWS", "RANGE"),
     JoinTypeKeywordsGrammar=OneOf(
         "CROSS",
         "INNER",
         Sequence(
             OneOf(
                 "FULL",
@@ -1069,14 +1070,28 @@
     type = "index_reference"
 
 
 class CollationReferenceSegment(ObjectReferenceSegment):
     """A reference to a collation."""
 
     type = "collation_reference"
+    # Some dialects like PostgreSQL want an identifier only, and quoted
+    # literals aren't allowed.  Other dialects like Snowflake only accept
+    # a quoted string literal.  We'll be a little overly-permissive and
+    # accept either... it shouldn't be too greedy since this segment generally
+    # occurs only in a Sequence after the "COLLATE" keyword.
+    match_grammar: Matchable = OneOf(
+        Ref("QuotedLiteralSegment"),
+        Delimited(
+            Ref("SingleIdentifierGrammar"),
+            delimiter=Ref("ObjectReferenceDelimiterGrammar"),
+            terminator=Ref("ObjectReferenceTerminatorGrammar"),
+            allow_gaps=False,
+        ),
+    )
 
 
 class RoleReferenceSegment(ObjectReferenceSegment):
     """A reference to a role, user, or account."""
 
     type = "role_reference"
     match_grammar: Matchable = Ref("SingleIdentifierGrammar")
@@ -1260,15 +1275,15 @@
             "IN",
             OneOf(
                 Ref("QuotedLiteralSegment"),
                 Ref("SingleIdentifierGrammar"),
                 Ref("ColumnReferenceSegment"),
             ),
         ),
-        Sequence(OneOf("IGNORE", "RESPECT"), "NULLS"),
+        Ref("IgnoreRespectNullsGrammar"),
         Ref("IndexColumnDefinitionSegment"),
     ),
     PostFunctionGrammar=OneOf(
         # Optional OVER suffix for window functions.
         # This is supported in bigquery & postgres (and its derivatives)
         # and so is included here for now.
         Ref("OverClauseSegment"),
@@ -1280,15 +1295,15 @@
 
 class OverClauseSegment(BaseSegment):
     """An OVER clause for window functions."""
 
     type = "over_clause"
     match_grammar: Matchable = Sequence(
         Indent,
-        Sequence(OneOf("IGNORE", "RESPECT"), "NULLS", optional=True),
+        Ref("IgnoreRespectNullsGrammar", optional=True),
         "OVER",
         OneOf(
             Ref("SingleIdentifierGrammar"),  # Window name
             Bracketed(
                 Ref("WindowSpecificationSegment", optional=True),
             ),
         ),
@@ -1386,20 +1401,15 @@
     )
 
 
 class PartitionClauseSegment(BaseSegment):
     """A `PARTITION BY` for window functions."""
 
     type = "partitionby_clause"
-    match_grammar: Matchable = StartsWith(
-        "PARTITION",
-        terminator=OneOf(Sequence("ORDER", "BY"), Ref("FrameClauseUnitGrammar")),
-        enforce_whitespace_preceding_terminator=True,
-    )
-    parse_grammar: Optional[Matchable] = Sequence(
+    match_grammar: Matchable = Sequence(
         "PARTITION",
         "BY",
         Indent,
         # Brackets are optional in a partition by statement
         OptionallyBracketed(Delimited(Ref("ExpressionSegment"))),
         Dedent,
     )
@@ -1439,14 +1449,15 @@
     type = "from_expression_element"
     match_grammar: Matchable = Sequence(
         Ref("PreTableFunctionKeywordsGrammar", optional=True),
         OptionallyBracketed(Ref("TableExpressionSegment")),
         Ref(
             "AliasExpressionSegment",
             exclude=OneOf(
+                Ref("FromClauseTerminatorGrammar"),
                 Ref("SamplingExpressionSegment"),
                 Ref("JoinLikeClauseGrammar"),
             ),
             optional=True,
         ),
         # https://cloud.google.com/bigquery/docs/reference/standard-sql/arrays#flattening_arrays
         Sequence("WITH", "OFFSET", Ref("AliasExpressionSegment"), optional=True),
@@ -1801,20 +1812,15 @@
     ```
     SELECT *
     FROM a JOIN b, c JOIN d
     ```
     """
 
     type = "from_clause"
-    match_grammar: Matchable = StartsWith(
-        "FROM",
-        terminator=Ref("FromClauseTerminatorGrammar"),
-        enforce_whitespace_preceding_terminator=True,
-    )
-    parse_grammar: Optional[Matchable] = Sequence(
+    match_grammar: Matchable = Sequence(
         "FROM",
         Delimited(
             Ref("FromExpressionSegment"),
         ),
     )
 
     def get_eventual_aliases(self) -> List[Tuple[BaseSegment, AliasInfo]]:
@@ -2224,20 +2230,15 @@
     match_grammar: Matchable = Ref("Expression_A_Grammar")
 
 
 class WhereClauseSegment(BaseSegment):
     """A `WHERE` clause like in `SELECT` or `INSERT`."""
 
     type = "where_clause"
-    match_grammar: Matchable = StartsWith(
-        "WHERE",
-        terminator=Ref("WhereClauseTerminatorGrammar"),
-        enforce_whitespace_preceding_terminator=True,
-    )
-    parse_grammar: Optional[Matchable] = Sequence(
+    match_grammar: Matchable = Sequence(
         "WHERE",
         # NOTE: The indent here is implicit to allow
         # constructions like:
         #
         #    WHERE a
         #        AND b
         #
@@ -2249,19 +2250,15 @@
     )
 
 
 class OrderByClauseSegment(BaseSegment):
     """A `ORDER BY` clause like in `SELECT`."""
 
     type = "orderby_clause"
-    match_grammar: Matchable = StartsWith(
-        Sequence("ORDER", "BY"),
-        terminator=Ref("OrderByClauseTerminators"),
-    )
-    parse_grammar: Optional[Matchable] = Sequence(
+    match_grammar: Matchable = Sequence(
         "ORDER",
         "BY",
         Indent,
         Delimited(
             Sequence(
                 OneOf(
                     Ref("ColumnReferenceSegment"),
@@ -2283,21 +2280,15 @@
 
 
 class GroupByClauseSegment(BaseSegment):
     """A `GROUP BY` clause like in `SELECT`."""
 
     type = "groupby_clause"
 
-    match_grammar: Matchable = StartsWith(
-        Sequence("GROUP", "BY"),
-        terminator=Ref("GroupByClauseTerminatorGrammar"),
-        enforce_whitespace_preceding_terminator=True,
-    )
-
-    parse_grammar: Optional[Matchable] = Sequence(
+    match_grammar: Matchable = Sequence(
         "GROUP",
         "BY",
         Indent,
         Delimited(
             OneOf(
                 Ref("ColumnReferenceSegment"),
                 # Can `GROUP BY 1`
@@ -2311,20 +2302,15 @@
     )
 
 
 class HavingClauseSegment(BaseSegment):
     """A `HAVING` clause like in `SELECT`."""
 
     type = "having_clause"
-    match_grammar: Matchable = StartsWith(
-        "HAVING",
-        terminator=Ref("HavingClauseTerminatorGrammar"),
-        enforce_whitespace_preceding_terminator=True,
-    )
-    parse_grammar: Optional[Matchable] = Sequence(
+    match_grammar: Matchable = Sequence(
         "HAVING",
         ImplicitIndent,
         OptionallyBracketed(Ref("ExpressionSegment")),
         Dedent,
     )
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_ansi_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_ansi_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_athena.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_athena.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_athena_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_athena_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_bigquery.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     OneOf,
     OptionallyBracketed,
     Ref,
     RegexLexer,
     RegexParser,
     SegmentGenerator,
     Sequence,
-    StartsWith,
     StringLexer,
     StringParser,
     SymbolSegment,
     MultiStringParser,
 )
 from sqlfluff.core.parser.segments.base import BracketedSegment
 from sqlfluff.dialects.dialect_bigquery_keywords import (
@@ -328,21 +327,15 @@
     )
 
 
 class QualifyClauseSegment(BaseSegment):
     """A `QUALIFY` clause like in `SELECT`."""
 
     type = "qualify_clause"
-    match_grammar = StartsWith(
-        "QUALIFY",
-        terminator=OneOf("WINDOW", "ORDER", "LIMIT"),
-        enforce_whitespace_preceding_terminator=True,
-    )
-
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "QUALIFY",
         Indent,
         OptionallyBracketed(Ref("ExpressionSegment")),
         Dedent,
     )
 
 
@@ -514,18 +507,15 @@
 class ForInStatementSegment(BaseSegment):
     """FOR..IN...DO...END FOR statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/procedural-language#for-in
     """
 
     type = "for_in_statement"
-    match_grammar = StartsWith(
-        "FOR", terminator=Sequence("END", "FOR"), include_terminator=True
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "FOR",
         Ref("SingleIdentifierGrammar"),
         "IN",
         Indent,
         Ref("SelectableGrammar"),
         Dedent,
         "DO",
@@ -559,18 +549,15 @@
 class RepeatStatementSegment(BaseSegment):
     """REPEAT...END REPEAT statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/procedural-language#repeat
     """
 
     type = "repeat_statement"
-    match_grammar = StartsWith(
-        "REPEAT", terminator=Sequence("END", "REPEAT"), include_terminator=True
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "REPEAT",
         Indent,
         Ref("RepeatStatementsSegment"),
         "UNTIL",
         Ref("ExpressionSegment"),
         Dedent,
         "END",
@@ -600,18 +587,15 @@
 class IfStatementSegment(BaseSegment):
     """IF...END IF statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/procedural-language#if
     """
 
     type = "if_statement"
-    match_grammar = StartsWith(
-        "IF", terminator=Sequence("END", "IF"), include_terminator=True
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "IF",
         Ref("ExpressionSegment"),
         "THEN",
         Indent,
         Ref("IfStatementsSegment"),
         Dedent,
         AnyNumberOf(
@@ -658,18 +642,15 @@
 class LoopStatementSegment(BaseSegment):
     """LOOP...END LOOP statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/procedural-language#loop
     """
 
     type = "loop_statement"
-    match_grammar = StartsWith(
-        "LOOP", terminator=Sequence("END", "LOOP"), include_terminator=True
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "LOOP",
         Indent,
         Ref("LoopStatementsSegment"),
         Dedent,
         "END",
         "LOOP",
     )
@@ -694,18 +675,15 @@
 class WhileStatementSegment(BaseSegment):
     """WHILE...END WHILE statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/procedural-language#while
     """
 
     type = "while_statement"
-    match_grammar = StartsWith(
-        "WHILE", terminator=Sequence("END", "WHILE"), include_terminator=True
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "WHILE",
         Ref("ExpressionSegment"),
         "DO",
         Indent,
         Ref("WhileStatementsSegment"),
         Dedent,
         "END",
@@ -841,28 +819,53 @@
             "NORMALIZE_AND_CASEFOLD",
             CodeSegment,
             type="function_name_identifier",
         ),
     )
 
 
+class FunctionNameSegment(ansi.FunctionNameSegment):
+    """Describes the name of a function.
+
+    This includes any prefix bits, e.g. project, schema or the SAFE keyword.
+    """
+
+    match_grammar: Matchable = Sequence(
+        # Project name, schema identifier, etc.
+        AnyNumberOf(
+            Sequence(
+                # BigQuery Function names can be prefixed by the keyword SAFE to
+                # return NULL instead of error.
+                # https://cloud.google.com/bigquery/docs/reference/standard-sql/functions-reference#safe_prefix
+                OneOf("SAFE", Ref("SingleIdentifierGrammar")),
+                Ref("DotSegment"),
+            ),
+        ),
+        # Base function name
+        OneOf(
+            Ref("FunctionNameIdentifierSegment"),
+            Ref("QuotedIdentifierSegment"),
+        ),
+        # BigQuery allows whitespaces between the `.` of a function refrence or
+        # SAFE prefix. Keeping the explicit `allow_gaps=True` here to
+        # make the distinction from `ansi.FunctionNameSegment` clear.
+        allow_gaps=True,
+    )
+
+
 class FunctionSegment(ansi.FunctionSegment):
     """A scalar or aggregate function.
 
     Maybe in the future we should distinguish between
     aggregate functions and other functions. For now
     we treat them the same because they look the same
     for our purposes.
     """
 
     match_grammar = Sequence(
-        # BigQuery Function names can be prefixed by the keyword SAFE to
-        # return NULL instead of error.
-        # https://cloud.google.com/bigquery/docs/reference/standard-sql/functions-reference#safe_prefix
-        Sequence("SAFE", Ref("DotSegment"), optional=True),
         OneOf(
             Sequence(
                 # BigQuery EXTRACT allows optional TimeZone
                 Ref("ExtractFunctionNameSegment"),
                 Bracketed(
                     OneOf(
                         Ref("DatetimeUnitSegment"),
@@ -1371,36 +1374,26 @@
     )
 
 
 class PartitionBySegment(BaseSegment):
     """PARTITION BY partition_expression."""
 
     type = "partition_by_segment"
-    match_grammar = StartsWith(
-        "PARTITION",
-        terminator=OneOf("CLUSTER", "OPTIONS", "AS", Ref("DelimiterGrammar")),
-        enforce_whitespace_preceding_terminator=True,
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "PARTITION",
         "BY",
         Ref("ExpressionSegment"),
     )
 
 
 class ClusterBySegment(BaseSegment):
     """CLUSTER BY clustering_column_list."""
 
     type = "cluster_by_segment"
-    match_grammar = StartsWith(
-        "CLUSTER",
-        terminator=OneOf("OPTIONS", "AS", Ref("DelimiterGrammar")),
-        enforce_whitespace_preceding_terminator=True,
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "CLUSTER",
         "BY",
         Delimited(Ref("ExpressionSegment")),
     )
 
 
 class OptionsSegment(BaseSegment):
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_bigquery_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_bigquery_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_clickhouse.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_clickhouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,14 +269,15 @@
     type = "from_expression_element"
     match_grammar: Matchable = Sequence(
         Ref("PreTableFunctionKeywordsGrammar", optional=True),
         OptionallyBracketed(Ref("TableExpressionSegment")),
         Ref(
             "AliasExpressionSegment",
             exclude=OneOf(
+                Ref("FromClauseTerminatorGrammar"),
                 Ref("SamplingExpressionSegment"),
                 Ref("JoinLikeClauseGrammar"),
                 "FINAL",
                 Ref("JoinClauseSegment"),
             ),
             optional=True,
         ),
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_clickhouse_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_clickhouse_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_databricks.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_db2.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_db2.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_db2_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_db2_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_duckdb.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_duckdb.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 """The DuckDB dialect.
 
 https://duckdb.org/docs/
 """
 
-from typing import Optional
-
 from sqlfluff.core.dialects import load_raw_dialect
 from sqlfluff.dialects import dialect_ansi as ansi
 from sqlfluff.core.parser import (
     Bracketed,
     Dedent,
     Delimited,
     Indent,
     Matchable,
     OneOf,
     Ref,
     Sequence,
-    StartsWith,
 )
 
 postgres_dialect = load_raw_dialect("postgres")
 
 duckdb_dialect = postgres_dialect.copy_as("duckdb")
 
 duckdb_dialect.replace(
@@ -68,20 +65,15 @@
         ),
     )
 
 
 class OrderByClauseSegment(ansi.OrderByClauseSegment):
     """A `ORDER BY` clause like in `SELECT`."""
 
-    match_grammar: Matchable = StartsWith(
-        Sequence("ORDER", "BY"),
-        terminator=Ref("OrderByClauseTerminators"),
-    )
-
-    parse_grammar: Optional[Matchable] = Sequence(
+    match_grammar: Matchable = Sequence(
         "ORDER",
         "BY",
         Indent,
         Delimited(
             Sequence(
                 OneOf(
                     "ALL",
@@ -89,30 +81,24 @@
                     Ref("NumericLiteralSegment"),
                     Ref("ExpressionSegment"),
                 ),
                 OneOf("ASC", "DESC", optional=True),
                 Sequence("NULLS", OneOf("FIRST", "LAST"), optional=True),
             ),
             allow_trailing=True,
-            terminator=OneOf(Ref.keyword("LIMIT"), Ref("FrameClauseUnitGrammar")),
+            terminator=Ref("OrderByClauseTerminators"),
         ),
         Dedent,
     )
 
 
 class GroupByClauseSegment(ansi.GroupByClauseSegment):
     """A `GROUP BY` clause like in `SELECT`."""
 
-    match_grammar: Matchable = StartsWith(
-        Sequence("GROUP", "BY"),
-        terminator=Ref("GroupByClauseTerminatorGrammar"),
-        enforce_whitespace_preceding_terminator=True,
-    )
-
-    parse_grammar: Optional[Matchable] = Sequence(
+    match_grammar: Matchable = Sequence(
         "GROUP",
         "BY",
         Indent,
         Delimited(
             OneOf(
                 "ALL",
                 Ref("ColumnReferenceSegment"),
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_exasol.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_exasol.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,41 +153,35 @@
         Ref("TableReferenceSegment"),
         Ref("BracketedColumnReferenceListGrammar", optional=True),
     ),
     ColumnReferenceListGrammar=Delimited(
         Ref("ColumnReferenceSegment"),
         ephemeral_name="ColumnReferenceList",
     ),
-    TableDistributeByGrammar=StartsWith(
-        Sequence(
-            "DISTRIBUTE",
-            "BY",
-            Delimited(
-                Ref("ColumnReferenceSegment"),
+    TableDistributeByGrammar=Sequence(
+        "DISTRIBUTE",
+        "BY",
+        Delimited(
+            Ref("ColumnReferenceSegment"),
+            terminator=OneOf(
+                Ref("TablePartitionByGrammar"),
+                Ref("DelimiterGrammar"),
             ),
         ),
-        terminator=OneOf(
-            Ref("TablePartitionByGrammar"),
-            Ref("DelimiterGrammar"),
-        ),
-        enforce_whitespace_preceding_terminator=True,
     ),
-    TablePartitionByGrammar=StartsWith(
-        Sequence(
-            "PARTITION",
-            "BY",
-            Delimited(
-                Ref("ColumnReferenceSegment"),
+    TablePartitionByGrammar=Sequence(
+        "PARTITION",
+        "BY",
+        Delimited(
+            Ref("ColumnReferenceSegment"),
+            terminator=OneOf(
+                Ref("TableDistributeByGrammar"),
+                Ref("DelimiterGrammar"),
             ),
         ),
-        terminator=OneOf(
-            Ref("TableDistributeByGrammar"),
-            Ref("DelimiterGrammar"),
-        ),
-        enforce_whitespace_preceding_terminator=True,
     ),
     TableConstraintEnableDisableGrammar=OneOf("ENABLE", "DISABLE"),
     EscapedIdentifierSegment=TypedParser(
         "escaped_identifier", SymbolSegment, type="identifier"
     ),
     SessionParameterSegment=SegmentGenerator(
         lambda dialect: MultiStringParser(
@@ -400,41 +394,27 @@
     )
 
 
 class WithInvalidUniquePKSegment(BaseSegment):
     """`WITH INVALID UNIQUE` or `WITH INVALID PRIMARY KEY` clause within `SELECT`."""
 
     type = "with_invalid_unique_pk_clause"
-    match_grammar = StartsWith(
-        Sequence(
-            Ref.keyword("WITH", optional=True),
-            "INVALID",
-            OneOf("UNIQUE", Ref("PrimaryKeyGrammar")),
-        ),
-        terminator="FROM",
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         Ref.keyword("WITH", optional=True),
         "INVALID",
         OneOf("UNIQUE", Ref("PrimaryKeyGrammar")),
         Ref("BracketedColumnReferenceListGrammar"),
     )
 
 
 class WithInvalidForeignKeySegment(BaseSegment):
     """`WITH INVALID FOREIGN KEY` clause within `SELECT`."""
 
     type = "with_invalid_foreign_key_clause"
-    match_grammar = StartsWith(
-        Sequence(
-            Ref.keyword("WITH", optional=True), "INVALID", Ref("ForeignKeyGrammar")
-        ),
-        terminator=Ref("FromClauseTerminatorGrammar"),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         Ref.keyword("WITH", optional=True),
         "INVALID",
         Ref("ForeignKeyGrammar"),
         Ref("BracketedColumnReferenceListGrammar"),
         Dedent,  # dedent for the indent in the select clause
         "FROM",
         Ref("TableReferenceSegment"),
@@ -444,16 +424,15 @@
     )
 
 
 class IntoTableSegment(BaseSegment):
     """`INTO TABLE` clause within `SELECT`."""
 
     type = "into_table_clause"
-    match_grammar = StartsWith(Sequence("INTO", "TABLE"), terminator="FROM")
-    parse_grammar = Sequence("INTO", "TABLE", Ref("TableReferenceSegment"))
+    match_grammar = Sequence("INTO", "TABLE", Ref("TableReferenceSegment"))
 
 
 class TableExpressionSegment(BaseSegment):
     """The main table expression e.g. within a FROM clause."""
 
     type = "table_expression"
     match_grammar = OneOf(
@@ -521,30 +500,15 @@
     )
 
 
 class ConnectByClauseSegment(BaseSegment):
     """`CONNECT BY` clause within a select statement."""
 
     type = "connect_by_clause"
-    match_grammar = StartsWith(
-        OneOf(
-            Sequence("CONNECT", "BY"),
-            Sequence("START", "WITH"),
-        ),
-        terminator=OneOf(
-            "PREFERRING",
-            Sequence("GROUP", "BY"),
-            "QUALIFY",
-            Sequence("ORDER", "BY"),
-            "LIMIT",
-            Ref("SetOperatorSegment"),
-        ),
-        enforce_whitespace_preceding_terminator=True,
-    )
-    parse_grammar = OneOf(
+    match_grammar = OneOf(
         Sequence(
             "CONNECT",
             "BY",
             Ref.keyword("NOCYCLE", optional=True),
             Delimited(
                 Ref("ExpressionSegment"),
                 delimiter="AND",
@@ -564,26 +528,15 @@
     )
 
 
 class GroupByClauseSegment(BaseSegment):
     """A `GROUP BY` clause like in `SELECT`."""
 
     type = "groupby_clause"
-    match_grammar = StartsWith(
-        Sequence("GROUP", "BY"),
-        terminator=OneOf(
-            Sequence("ORDER", "BY"),
-            "LIMIT",
-            "HAVING",
-            "QUALIFY",
-            Ref("SetOperatorSegment"),
-        ),
-        enforce_whitespace_preceding_terminator=True,
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "GROUP",
         "BY",
         Indent,
         Delimited(
             OneOf(
                 Ref("ColumnReferenceSegment"),
                 # Can `GROUP BY 1`
@@ -606,47 +559,27 @@
     )
 
 
 class CubeRollupClauseSegment(BaseSegment):
     """`CUBE` / `ROLLUP` clause within the `GROUP BY` clause."""
 
     type = "cube_rollup_clause"
-    match_grammar = StartsWith(
-        OneOf("CUBE", "ROLLUP"),
-        terminator=OneOf(
-            "HAVING",
-            "QUALIFY",
-            Sequence("ORDER", "BY"),
-            "LIMIT",
-            Ref("SetOperatorSegment"),
-        ),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         OneOf("CUBE", "ROLLUP"),
         Bracketed(
             Ref("GroupingExpressionList"),
         ),
     )
 
 
 class GroupingSetsClauseSegment(BaseSegment):
     """`GROUPING SETS` clause within the `GROUP BY` clause."""
 
     type = "grouping_sets_clause"
-    match_grammar = StartsWith(
-        Sequence("GROUPING", "SETS"),
-        terminator=OneOf(
-            "HAVING",
-            "QUALIFY",
-            Sequence("ORDER", "BY"),
-            "LIMIT",
-            Ref("SetOperatorSegment"),
-        ),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "GROUPING",
         "SETS",
         Bracketed(
             Delimited(
                 Ref("CubeRollupClauseSegment"),
                 Ref("GroupingExpressionList"),
             )
@@ -667,23 +600,15 @@
     )
 
 
 class QualifyClauseSegment(BaseSegment):
     """`QUALIFY` clause within `SELECT`."""
 
     type = "qualify_clause"
-    match_grammar = StartsWith(
-        "QUALIFY",
-        terminator=OneOf(
-            Sequence("ORDER", "BY"),
-            "LIMIT",
-            Ref("SetOperatorSegment"),
-        ),
-    )
-    parse_grammar = Sequence("QUALIFY", Ref("ExpressionSegment"))
+    match_grammar = Sequence("QUALIFY", Ref("ExpressionSegment"))
 
 
 class LimitClauseSegment(BaseSegment):
     """A `LIMIT` clause like in `SELECT`."""
 
     type = "limit_clause"
     match_grammar = Sequence(
@@ -1188,19 +1113,15 @@
     )
 
 
 class TableInlineConstraintSegment(BaseSegment):
     """Inline table constraint for CREATE / ALTER TABLE."""
 
     type = "table_constraint_definition"
-    match_grammar = StartsWith(
-        OneOf("CONSTRAINT", "NOT", "NULL", "PRIMARY", "FOREIGN"),
-        terminator=OneOf("COMMENT", Ref("CommaSegment"), Ref("EndBracketSegment")),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         Sequence(
             "CONSTRAINT",
             Ref(
                 "SingleIdentifierGrammar",
                 # exclude UNRESERVED_KEYWORDS which could used as NakedIdentifier
                 # to make e.g. `id NUMBER CONSTRAINT PRIMARY KEY` work (which is equal
                 # to just `id NUMBER PRIMARY KEY`)
@@ -1221,19 +1142,15 @@
     )
 
 
 class TableOutOfLineConstraintSegment(BaseSegment):
     """Out of line table constraint for CREATE / ALTER TABLE."""
 
     type = "table_constraint_definition"
-    match_grammar = StartsWith(
-        OneOf("CONSTRAINT", "PRIMARY", "FOREIGN"),
-        terminator=OneOf(Ref("CommaSegment"), "DISTRIBUTE", "PARTITION"),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         Sequence(
             "CONSTRAINT",
             Ref(
                 "SingleIdentifierGrammar",
                 # exclude UNRESERVED_KEYWORDS which could used as NakedIdentifier
                 # to make e.g. `id NUMBER, CONSTRAINT PRIMARY KEY(id)` work (which is
                 # equal to just `id NUMBER, PRIMARY KEY(id)`)
@@ -1769,43 +1686,30 @@
     )
 
 
 class MergeMatchedClauseSegment(BaseSegment):
     """The `WHEN MATCHED` clause within a `MERGE` statement."""
 
     type = "merge_when_matched_clause"
-    match_grammar = StartsWith(
-        Sequence("WHEN", "MATCHED", "THEN", OneOf("UPDATE", "DELETE")),
-        terminator=Ref("MergeNotMatchedClauseSegment"),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "WHEN",
         "MATCHED",
         "THEN",
         OneOf(
             Ref("MergeUpdateClauseSegment"),
             Ref("MergeDeleteClauseSegment"),
         ),
     )
 
 
 class MergeNotMatchedClauseSegment(BaseSegment):
     """The `WHEN NOT MATCHED` clause within a `MERGE` statement."""
 
     type = "merge_when_not_matched_clause"
-    match_grammar = StartsWith(
-        Sequence(
-            "WHEN",
-            "NOT",
-            "MATCHED",
-            "THEN",
-        ),
-        terminator=Ref("MergeMatchedClauseSegment"),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "WHEN",
         "NOT",
         "MATCHED",
         "THEN",
         Ref("MergeInsertClauseSegment"),
     )
 
@@ -2011,19 +1915,15 @@
     )
 
 
 class ImportFromExportIntoDbSrcSegment(BaseSegment):
     """`IMPORT` from or `EXPORT` to a external database source (EXA,ORA,JDBC)."""
 
     type = "import_export_dbsrc"
-    match_grammar = StartsWith(
-        OneOf("EXA", "ORA", "JDBC"),
-        terminator=OneOf(Ref("ImportErrorsClauseSegment"), Ref("RejectClauseSegment")),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         OneOf(
             "EXA",
             "ORA",
             Sequence(
                 "JDBC",
                 Sequence(
                     "DRIVER",
@@ -2066,19 +1966,15 @@
     )
 
 
 class ImportFromExportIntoFileSegment(BaseSegment):
     """`IMPORT` from or `EXPORT` to a file source (FBV,CSV)."""
 
     type = "import_file"
-    match_grammar = StartsWith(
-        OneOf("CSV", "FBV", "LOCAL"),
-        terminator=Ref("ImportErrorsClauseSegment"),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         OneOf(
             Sequence(
                 OneOf(
                     "CSV",
                     "FBV",
                 ),
                 AnyNumberOf(
@@ -2904,26 +2800,15 @@
 class PreferringClauseSegment(BaseSegment):
     """`PREFERRING` clause of the Exasol Skyline extension.
 
     https://docs.exasol.com/advanced_analytics/skyline.htm#preferring_clause
     """
 
     type = "preferring_clause"
-    match_grammar = StartsWith(
-        "PREFERRING",
-        terminator=OneOf(
-            "LIMIT",
-            Sequence("GROUP", "BY"),
-            Sequence("ORDER", "BY"),
-            "HAVING",
-            "QUALIFY",
-            Ref("SetOperatorSegment"),
-        ),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "PREFERRING",
         OptionallyBracketed(Ref("PreferringPreferenceTermSegment")),
         Ref("PartitionClauseSegment", optional=True),
     )
 
 
 class PreferringPreferenceTermSegment(BaseSegment):
@@ -3391,24 +3276,15 @@
     type = "create_scripting_lua_script"
 
     is_ddl = True
     is_dml = False
     is_dql = False
     is_dcl = False
 
-    match_grammar = StartsWith(
-        Sequence(
-            "CREATE",
-            Ref("OrReplaceGrammar", optional=True),
-            Ref.keyword("LUA", optional=True),
-            "SCRIPT",
-        ),
-        terminator=Ref("FunctionScriptTerminatorSegment"),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "CREATE",
         Ref("OrReplaceGrammar", optional=True),
         Ref.keyword("LUA", optional=True),
         "SCRIPT",
         Ref("ScriptReferenceSegment"),
         Bracketed(
             Delimited(
@@ -3436,32 +3312,15 @@
     type = "create_udf_script"
 
     is_ddl = True
     is_dml = False
     is_dql = False
     is_dcl = False
 
-    match_grammar = StartsWith(
-        Sequence(
-            "CREATE",
-            Ref("OrReplaceGrammar", optional=True),
-            OneOf(
-                "JAVA",
-                "PYTHON",
-                "LUA",
-                "R",
-                Ref("SingleIdentifierGrammar"),
-                optional=True,
-            ),
-            OneOf("SCALAR", "SET"),
-            "SCRIPT",
-        ),
-        terminator=Ref("FunctionScriptTerminatorSegment"),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "CREATE",
         Ref("OrReplaceGrammar", optional=True),
         OneOf(
             "JAVA", "PYTHON", "LUA", "R", Ref("SingleIdentifierGrammar"), optional=True
         ),
         OneOf("SCALAR", "SET"),
         "SCRIPT",
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_exasol_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_exasol_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_greenplum.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_greenplum.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                                 AnyNumberOf(
                                     # A single COLLATE segment can come before or after
                                     # constraint segments
                                     OneOf(
                                         Ref("ColumnConstraintSegment"),
                                         Sequence(
                                             "COLLATE",
-                                            Ref("ObjectReferenceSegment"),
+                                            Ref("CollationReferenceSegment"),
                                         ),
                                     ),
                                 ),
                             ),
                             Ref("TableConstraintSegment"),
                             Sequence(
                                 "LIKE",
@@ -131,15 +131,15 @@
                                 OneOf(
                                     Ref("ColumnReferenceSegment"),
                                     Ref("FunctionSegment"),
                                 ),
                                 AnyNumberOf(
                                     Sequence(
                                         "COLLATE",
-                                        Ref("QuotedLiteralSegment"),
+                                        Ref("CollationReferenceSegment"),
                                         optional=True,
                                     ),
                                     Ref("ParameterNameSegment", optional=True),
                                 ),
                             ),
                         )
                     )
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_hive.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_hive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """The Hive dialect."""
-from typing import Optional
 
 from sqlfluff.core.parser import (
     AnyNumberOf,
     BaseSegment,
     Sequence,
     Ref,
     OneOf,
@@ -12,15 +11,14 @@
     TypedParser,
     Nothing,
     SymbolSegment,
     StringParser,
     OptionallyBracketed,
     RegexParser,
     Matchable,
-    StartsWith,
     Indent,
     Dedent,
 )
 
 from sqlfluff.core.dialects import load_raw_dialect
 from sqlfluff.core.parser.segments.raw import CodeSegment, KeywordSegment
 from sqlfluff.dialects.dialect_hive_keywords import (
@@ -615,22 +613,54 @@
         "TRUNCATE",
         Ref.keyword("TABLE", optional=True),
         Ref("TableReferenceSegment"),
         Ref("PartitionSpecGrammar", optional=True),
     )
 
 
+class SetStatementSegment(BaseSegment):
+    """A `SET` statement.
+
+    https://cwiki.apache.org/confluence/display/Hive/LanguageManual+Commands
+    """
+
+    type = "set_statement"
+
+    match_grammar = Sequence(
+        "SET",
+        OneOf(
+            # set -v
+            Sequence(
+                StringParser("-", SymbolSegment, type="option_indicator"),
+                StringParser("v", CodeSegment, type="option"),
+            ),
+            # set key = value
+            Sequence(
+                Delimited(
+                    Ref("ParameterNameSegment"),
+                    delimiter=OneOf(Ref("DotSegment"), Ref("ColonSegment")),
+                    allow_gaps=False,
+                ),
+                Ref("RawEqualsSegment"),
+                Ref("LiteralGrammar"),
+            ),
+            optional=True,
+        ),
+    )
+
+
 class StatementSegment(ansi.StatementSegment):
     """Overriding StatementSegment to allow for additional segment parsing."""
 
     parse_grammar = ansi.StatementSegment.parse_grammar.copy(
         insert=[
             Ref("AlterDatabaseStatementSegment"),
             Ref("MsckRepairTableStatementSegment"),
             Ref("MsckTableStatementSegment"),
+            Ref("SetStatementSegment"),
         ],
         remove=[
             Ref("TransactionStatementSegment"),
             Ref("CreateSchemaStatementSegment"),
             Ref("SetSchemaStatementSegment"),
             Ref("CreateModelStatementSegment"),
             Ref("DropModelStatementSegment"),
@@ -943,29 +973,14 @@
             Ref("DistributeByClauseSegment", optional=True),
             Ref("SortByClauseSegment", optional=True),
         ],
         before=Ref("LimitClauseSegment", optional=True),
     )
 
 
-class PartitionClauseSegment(ansi.PartitionClauseSegment):
-    """Overriding SetExpressionSegment to allow for additional segment parsing."""
-
-    match_grammar = ansi.PartitionClauseSegment.match_grammar.copy()
-    match_grammar.terminator = match_grammar.terminator.copy(  # type: ignore
-        insert=[
-            Sequence("CLUSTER", "BY"),
-            Sequence("DISTRIBUTE", "BY"),
-            Sequence("SORT", "BY"),
-        ],
-        before=Ref("FrameClauseUnitGrammar"),
-    )
-    parse_grammar = ansi.PartitionClauseSegment.parse_grammar
-
-
 class OrderByClauseSegment(ansi.OrderByClauseSegment):
     """A `ORDER BY` clause like in `SELECT`."""
 
     match_grammar = ansi.OrderByClauseSegment.match_grammar.copy()
     match_grammar.terminator = OneOf(  # type: ignore
         "CLUSTER",
         "DISTRIBUTE",
@@ -974,26 +989,21 @@
         "HAVING",
         "QUALIFY",
         # For window functions
         "WINDOW",
         Ref("FrameClauseUnitGrammar"),
         "SEPARATOR",
     )
-    parse_grammar = ansi.OrderByClauseSegment.parse_grammar
 
 
 class ClusterByClauseSegment(ansi.OrderByClauseSegment):
     """A `CLUSTER BY` clause like in `SELECT`."""
 
     type = "clusterby_clause"
-    match_grammar: Matchable = StartsWith(
-        Sequence("CLUSTER", "BY"),
-        terminator=ansi.OrderByClauseSegment.match_grammar.terminator,  # type: ignore
-    )
-    parse_grammar: Optional[Matchable] = Sequence(
+    match_grammar: Matchable = Sequence(
         "CLUSTER",
         "BY",
         Indent,
         Delimited(
             Sequence(
                 OneOf(
                     Ref("ColumnReferenceSegment"),
@@ -1007,56 +1017,46 @@
     )
 
 
 class DistributeByClauseSegment(ansi.OrderByClauseSegment):
     """A `DISTRIBUTE BY` clause like in `SELECT`."""
 
     type = "distributeby_clause"
-    match_grammar: Matchable = StartsWith(
-        Sequence("DISTRIBUTE", "BY"),
-        terminator=OneOf(
-            "SORT",
-            "LIMIT",
-            "HAVING",
-            "QUALIFY",
-            # For window functions
-            "WINDOW",
-            Ref("FrameClauseUnitGrammar"),
-            "SEPARATOR",
-        ),
-    )
-    parse_grammar: Optional[Matchable] = Sequence(
+    match_grammar: Matchable = Sequence(
         "DISTRIBUTE",
         "BY",
         Indent,
         Delimited(
             Sequence(
                 OneOf(
                     Ref("ColumnReferenceSegment"),
                     Ref("NumericLiteralSegment"),
                     Ref("ExpressionSegment"),
                 ),
             ),
             terminator=OneOf(
-                Ref.keyword("LIMIT"), Ref("FrameClauseUnitGrammar"), Ref.keyword("SORT")
+                "SORT",
+                "LIMIT",
+                "HAVING",
+                "QUALIFY",
+                # For window functions
+                "WINDOW",
+                Ref("FrameClauseUnitGrammar"),
+                "SEPARATOR",
             ),
         ),
         Dedent,
     )
 
 
 class SortByClauseSegment(ansi.OrderByClauseSegment):
     """A `SORT BY` clause like in `SELECT`."""
 
     type = "sortby_clause"
-    match_grammar: Matchable = StartsWith(
-        Sequence("SORT", "BY"),
-        terminator=ansi.OrderByClauseSegment.match_grammar.terminator,  # type: ignore
-    )
-    parse_grammar: Optional[Matchable] = Sequence(
+    match_grammar: Matchable = Sequence(
         "SORT",
         "BY",
         Indent,
         Delimited(
             Sequence(
                 OneOf(
                     Ref("ColumnReferenceSegment"),
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_hive_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_hive_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_materialize.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_materialize.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_materialize_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_materialize_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_mysql.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -604,20 +604,15 @@
     )
 
 
 class DeleteUsingClauseSegment(BaseSegment):
     """A `USING` clause froma `DELETE` Statement`."""
 
     type = "using_clause"
-    match_grammar = StartsWith(
-        "USING",
-        terminator=Ref("FromClauseTerminatorGrammar"),
-        enforce_whitespace_preceding_terminator=True,
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "USING",
         Delimited(
             Ref("FromExpressionSegment"),
         ),
     )
 
 
@@ -660,15 +655,15 @@
 
 class ColumnConstraintSegment(ansi.ColumnConstraintSegment):
     """A column option; each CREATE TABLE column can have 0 or more."""
 
     match_grammar: Matchable = OneOf(
         ansi.ColumnConstraintSegment.match_grammar,
         Sequence("CHARACTER", "SET", Ref("NakedIdentifierSegment")),
-        Sequence("COLLATE", Ref("NakedIdentifierSegment")),
+        Sequence("COLLATE", Ref("CollationReferenceSegment")),
     )
 
 
 class IndexTypeGrammar(BaseSegment):
     """index_type in table_constraint."""
 
     type = "index_type"
@@ -2606,15 +2601,15 @@
                 "SET",
                 Ref("EqualsSegment", optional=True),
                 Ref("NakedIdentifierSegment"),
             ),
             Sequence(
                 "COLLATE",
                 Ref("EqualsSegment", optional=True),
-                Ref("NakedIdentifierSegment"),
+                Ref("CollationReferenceSegment"),
             ),
             Sequence(
                 "ENCRYPTION",
                 Ref("EqualsSegment", optional=True),
                 Ref("QuotedLiteralSegment"),
             ),
         ),
@@ -2652,15 +2647,15 @@
                 Ref("EqualsSegment", optional=True),
                 Ref("NakedIdentifierSegment"),
             ),
             Sequence(
                 Ref.keyword("DEFAULT", optional=True),
                 "COLLATE",
                 Ref("EqualsSegment", optional=True),
-                Ref("NakedIdentifierSegment"),
+                Ref("CollationReferenceSegment"),
             ),
             Sequence(
                 Ref.keyword("DEFAULT", optional=True),
                 "ENCRYPTION",
                 Ref("EqualsSegment", optional=True),
                 Ref("QuotedLiteralSegment"),
             ),
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_mysql_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_oracle.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_oracle.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_postgres.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_postgres.py`

 * *Files 0% similar despite different names*

```diff
@@ -1458,52 +1458,30 @@
 class CubeRollupClauseSegment(BaseSegment):
     """`CUBE` / `ROLLUP` clause within the `GROUP BY` clause.
 
     https://www.postgresql.org/docs/current/queries-table-expressions.html#QUERIES-GROUPING-SETS
     """
 
     type = "cube_rollup_clause"
-    match_grammar = StartsWith(
-        OneOf("CUBE", "ROLLUP"),
-        terminator=OneOf(
-            "HAVING",
-            "QUALIFY",
-            Sequence("ORDER", "BY"),
-            "LIMIT",
-            "WINDOW",
-            Ref("SetOperatorSegment"),
-        ),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         OneOf("CUBE", "ROLLUP"),
         Bracketed(
             Ref("GroupingExpressionList"),
         ),
     )
 
 
 class GroupingSetsClauseSegment(BaseSegment):
     """`GROUPING SETS` clause within the `GROUP BY` clause.
 
     https://www.postgresql.org/docs/current/queries-table-expressions.html#QUERIES-GROUPING-SETS
     """
 
     type = "grouping_sets_clause"
-    match_grammar = StartsWith(
-        Sequence("GROUPING", "SETS"),
-        terminator=OneOf(
-            "HAVING",
-            "QUALIFY",
-            Sequence("ORDER", "BY"),
-            "LIMIT",
-            "WINDOW",
-            Ref("SetOperatorSegment"),
-        ),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "GROUPING",
         "SETS",
         Bracketed(
             Delimited(
                 Ref("CubeRollupClauseSegment"),
                 Ref("GroupingExpressionList"),
             )
@@ -1524,27 +1502,15 @@
     )
 
 
 class GroupByClauseSegment(BaseSegment):
     """A `GROUP BY` clause like in `SELECT`."""
 
     type = "groupby_clause"
-    match_grammar = StartsWith(
-        Sequence("GROUP", "BY"),
-        terminator=OneOf(
-            Sequence("ORDER", "BY"),
-            "LIMIT",
-            "HAVING",
-            "QUALIFY",
-            "WINDOW",
-            Ref("SetOperatorSegment"),
-        ),
-        enforce_whitespace_preceding_terminator=True,
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "GROUP",
         "BY",
         Indent,
         Delimited(
             OneOf(
                 Ref("ColumnReferenceSegment"),
                 # Can `GROUP BY 1`
@@ -1796,15 +1762,15 @@
                                 AnyNumberOf(
                                     # A single COLLATE segment can come before or after
                                     # constraint segments
                                     OneOf(
                                         Ref("ColumnConstraintSegment"),
                                         Sequence(
                                             "COLLATE",
-                                            Ref("ObjectReferenceSegment"),
+                                            Ref("CollationReferenceSegment"),
                                         ),
                                     ),
                                 ),
                             ),
                             Ref("TableConstraintSegment"),
                             Sequence(
                                 "LIKE",
@@ -1870,15 +1836,15 @@
                                 OneOf(
                                     Ref("ColumnReferenceSegment"),
                                     Ref("FunctionSegment"),
                                 ),
                                 AnyNumberOf(
                                     Sequence(
                                         "COLLATE",
-                                        Ref("QuotedLiteralSegment"),
+                                        Ref("CollationReferenceSegment"),
                                         optional=True,
                                     ),
                                     Ref("ParameterNameSegment", optional=True),
                                 ),
                             ),
                         )
                     )
@@ -2057,15 +2023,15 @@
     match_grammar = OneOf(
         Sequence(
             "ADD",
             Ref.keyword("COLUMN", optional=True),
             Ref("IfNotExistsGrammar", optional=True),
             Ref("ColumnReferenceSegment"),
             Ref("DatatypeSegment"),
-            Sequence("COLLATE", Ref("QuotedLiteralSegment"), optional=True),
+            Sequence("COLLATE", Ref("CollationReferenceSegment"), optional=True),
             AnyNumberOf(Ref("ColumnConstraintSegment")),
         ),
         Sequence(
             "DROP",
             Ref.keyword("COLUMN", optional=True),
             Ref("IfExistsGrammar", optional=True),
             Ref("ColumnReferenceSegment"),
@@ -2076,15 +2042,17 @@
             Ref.keyword("COLUMN", optional=True),
             Ref("ColumnReferenceSegment"),
             OneOf(
                 Sequence(
                     Sequence("SET", "DATA", optional=True),
                     "TYPE",
                     Ref("DatatypeSegment"),
-                    Sequence("COLLATE", Ref("QuotedLiteralSegment"), optional=True),
+                    Sequence(
+                        "COLLATE", Ref("CollationReferenceSegment"), optional=True
+                    ),
                     Sequence("USING", OneOf(Ref("ExpressionSegment")), optional=True),
                 ),
                 Sequence(
                     "SET",
                     "DEFAULT",
                     OneOf(
                         OneOf(
@@ -4178,15 +4146,15 @@
                     Sequence(
                         OneOf(
                             Ref("ColumnReferenceSegment"),
                             Bracketed(Ref("ExpressionSegment")),
                         ),
                         Sequence(
                             "COLLATE",
-                            Ref("QuotedLiteralSegment"),
+                            Ref("CollationReferenceSegment"),
                             optional=True,
                         ),
                         Ref("OperationClassReferenceSegment", optional=True),
                     )
                 )
             ),
             Sequence("WHERE", Ref("ExpressionSegment"), optional=True),
@@ -4344,15 +4312,15 @@
     type = "create_domain_statement"
     match_grammar = Sequence(
         "CREATE",
         "DOMAIN",
         Ref("ObjectReferenceSegment"),
         Sequence("AS", optional=True),
         Ref("DatatypeSegment"),
-        Sequence("COLLATE", Ref("ObjectReferenceSegment"), optional=True),
+        Sequence("COLLATE", Ref("CollationReferenceSegment"), optional=True),
         Sequence("DEFAULT", Ref("ExpressionSegment"), optional=True),
         AnyNumberOf(
             Sequence(
                 Sequence(
                     "CONSTRAINT",
                     Ref("ObjectReferenceSegment"),
                     optional=True,
@@ -4979,29 +4947,29 @@
                 Sequence(
                     "ADD",
                     "ATTRIBUTE",
                     Ref("ColumnReferenceSegment"),
                     Ref("DatatypeSegment"),
                     Sequence(
                         "COLLATE",
-                        Ref("QuotedLiteralSegment"),
+                        Ref("CollationReferenceSegment"),
                         optional=True,
                     ),
                     Ref("CascadeRestrictGrammar", optional=True),
                 ),
                 Sequence(
                     "ALTER",
                     "ATTRIBUTE",
                     Ref("ColumnReferenceSegment"),
                     Sequence("SET", "DATA", optional=True),
                     "TYPE",
                     Ref("DatatypeSegment"),
                     Sequence(
                         "COLLATE",
-                        Ref("QuotedLiteralSegment"),
+                        Ref("CollationReferenceSegment"),
                         optional=True,
                     ),
                     Ref("CascadeRestrictGrammar", optional=True),
                 ),
                 Sequence(
                     "DROP",
                     "ATTRIBUTE",
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_postgres_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_postgres_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_redshift.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_redshift.py`

 * *Files 0% similar despite different names*

```diff
@@ -678,15 +678,15 @@
         ),
         Sequence(
             "ADD",
             Ref.keyword("COLUMN", optional=True),
             Ref("ColumnReferenceSegment"),
             Ref("DatatypeSegment"),
             Sequence("DEFAULT", Ref("ExpressionSegment"), optional=True),
-            Sequence("COLLATE", Ref("QuotedLiteralSegment"), optional=True),
+            Sequence("COLLATE", Ref("CollationReferenceSegment"), optional=True),
             AnyNumberOf(Ref("ColumnConstraintSegment")),
         ),
         Sequence(
             "DROP",
             Ref.keyword("COLUMN", optional=True),
             Ref("ColumnReferenceSegment"),
             Ref("DropBehaviorGrammar", optional=True),
@@ -2504,16 +2504,15 @@
         ),
     )
 
 
 class FromClauseSegment(ansi.FromClauseSegment):
     """Slightly modified version which allows for using brackets for content of FROM."""
 
-    match_grammar = ansi.FromClauseSegment.match_grammar
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "FROM",
         Delimited(
             OptionallyBracketed(Ref("FromExpressionSegment")),
         ),
     )
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_redshift_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_redshift_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_snowflake.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """The Snowflake dialect.
 
 Inherits from ANSI.
 
 Based on https://docs.snowflake.com/en/sql-reference-commands.html
 """
-from typing import Optional
 
 from sqlfluff.core.dialects import load_raw_dialect
 from sqlfluff.core.parser import (
     AnyNumberOf,
     AnySetOf,
     Anything,
     BaseSegment,
@@ -824,20 +823,15 @@
     """A `GROUP BY` clause like in `SELECT`.
 
     Snowflake supports Cube, Rollup, and Grouping Sets
 
     https://docs.snowflake.com/en/sql-reference/constructs/group-by.html
     """
 
-    match_grammar: Matchable = StartsWith(
-        Sequence("GROUP", "BY"),
-        terminator=Ref("GroupByClauseTerminatorGrammar"),
-        enforce_whitespace_preceding_terminator=True,
-    )
-    parse_grammar: Optional[Matchable] = Sequence(
+    match_grammar: Matchable = Sequence(
         "GROUP",
         "BY",
         Indent,
         OneOf(
             Sequence(
                 OneOf("CUBE", "ROLLUP", Sequence("GROUPING", "SETS")),
                 Bracketed(
@@ -1089,14 +1083,15 @@
     type = "from_expression_element"
     match_grammar = Sequence(
         Ref("PreTableFunctionKeywordsGrammar", optional=True),
         OptionallyBracketed(Ref("TableExpressionSegment")),
         Ref(
             "AliasExpressionSegment",
             exclude=OneOf(
+                Ref("FromClauseTerminatorGrammar"),
                 Ref("SamplingExpressionSegment"),
                 Ref("ChangesClauseSegment"),
                 Ref("JoinLikeClauseGrammar"),
             ),
             optional=True,
         ),
         # https://cloud.google.com/bigquery/docs/reference/standard-sql/arrays#flattening_arrays
@@ -1394,24 +1389,15 @@
 class QualifyClauseSegment(BaseSegment):
     """A `QUALIFY` clause like in `SELECT`.
 
     https://docs.snowflake.com/en/sql-reference/constructs/qualify.html
     """
 
     type = "qualify_clause"
-    match_grammar = StartsWith(
-        "QUALIFY",
-        terminator=OneOf(
-            Sequence("ORDER", "BY"),
-            "LIMIT",
-            "FETCH",
-            "OFFSET",
-        ),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "QUALIFY",
         Indent,
         OneOf(
             Bracketed(
                 Ref("ExpressionSegment"),
             ),
             Ref("ExpressionSegment"),
@@ -2922,15 +2908,15 @@
 class ColumnConstraintSegment(ansi.ColumnConstraintSegment):
     """A column option; each CREATE TABLE column can have 0 or more.
 
     https://docs.snowflake.com/en/sql-reference/sql/create-table.html
     """
 
     match_grammar = AnySetOf(
-        Sequence("COLLATE", Ref("QuotedLiteralSegment")),
+        Sequence("COLLATE", Ref("CollationReferenceSegment")),
         Sequence(
             "DEFAULT",
             OneOf(
                 Ref("QuotedLiteralSegment"),
                 # https://docs.snowflake.com/en/sql-reference/functions/current_timestamp.html
                 Sequence(
                     "CURRENT_TIMESTAMP",
@@ -3774,14 +3760,15 @@
     match_grammar = Sequence(
         "CREATE",
         Ref("OrReplaceGrammar", optional=True),
         AnySetOf(
             "SECURE",
             "RECURSIVE",
         ),
+        Ref("TemporaryGrammar", optional=True),
         "VIEW",
         Ref("IfNotExistsGrammar", optional=True),
         Ref("TableReferenceSegment"),
         AnySetOf(
             Bracketed(
                 Delimited(
                     Sequence(
@@ -5746,15 +5733,15 @@
     https://docs.snowflake.com/en/sql-reference/sql/execute-task
     """
 
     type = "execute_task_clause"
     match_grammar = Sequence(
         "EXECUTE",
         "TASK",
-        Ref("ParameterNameSegment"),
+        Ref("ObjectReferenceSegment"),
     )
 
 
 ############################
 # MERGE
 ############################
 class MergeUpdateClauseSegment(ansi.MergeUpdateClauseSegment):
@@ -6273,16 +6260,15 @@
 
 class OrderByClauseSegment(ansi.OrderByClauseSegment):
     """An `ORDER BY` clause.
 
     https://docs.snowflake.com/en/sql-reference/constructs/order-by.html
     """
 
-    match_grammar = ansi.OrderByClauseSegment.match_grammar.copy()
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "ORDER",
         "BY",
         Indent,
         Delimited(
             Sequence(
                 OneOf(
                     Ref("ColumnReferenceSegment"),
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_snowflake_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_snowflake_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_soql.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_soql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sparksql.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sparksql.py`

 * *Files 0% similar despite different names*

```diff
@@ -790,21 +790,15 @@
     match_grammar = Ref.keyword("DIV")
 
 
 class QualifyClauseSegment(BaseSegment):
     """A `QUALIFY` clause like in `SELECT`."""
 
     type = "qualify_clause"
-    match_grammar = StartsWith(
-        "QUALIFY",
-        terminator=OneOf("WINDOW", Sequence("ORDER", "BY"), "LIMIT"),
-        enforce_whitespace_preceding_terminator=True,
-    )
-
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "QUALIFY",
         Indent,
         OptionallyBracketed(Ref("ExpressionSegment")),
         Dedent,
     )
 
 
@@ -1562,44 +1556,35 @@
     Equivalent to `DISTRIBUTE BY` and `SORT BY` in tandem.
     This clause is mutually exclusive with SORT BY, ORDER BY and DISTRIBUTE BY.
     https://spark.apache.org/docs/latest/sql-ref-syntax-qry-select-clusterby.html
     """
 
     type = "cluster_by_clause"
 
-    match_grammar = StartsWith(
-        Sequence("CLUSTER", "BY"),
-        terminator=OneOf(
-            "LIMIT",
-            "HAVING",
-            # For window functions
-            "WINDOW",
-            Ref("FrameClauseUnitGrammar"),
-            "SEPARATOR",
-        ),
-    )
-
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "CLUSTER",
         "BY",
         Indent,
         Delimited(
             Sequence(
                 OneOf(
                     Ref("ColumnReferenceSegment"),
                     # Can `CLUSTER BY 1`
                     Ref("NumericLiteralSegment"),
                     # Can cluster by an expression
                     Ref("ExpressionSegment"),
                 ),
             ),
             terminator=OneOf(
-                "WINDOW",
                 "LIMIT",
+                "HAVING",
+                # For window functions
+                "WINDOW",
                 Ref("FrameClauseUnitGrammar"),
+                "SEPARATOR",
             ),
         ),
         Dedent,
     )
 
 
 class DistributeByClauseSegment(BaseSegment):
@@ -1607,46 +1592,36 @@
 
     This clause is mutually exclusive with SORT BY, ORDER BY and DISTRIBUTE BY.
     https://spark.apache.org/docs/latest/sql-ref-syntax-qry-select-distribute-by.html
     """
 
     type = "distribute_by_clause"
 
-    match_grammar = StartsWith(
-        Sequence("DISTRIBUTE", "BY"),
-        terminator=OneOf(
-            "SORT",
-            "LIMIT",
-            "HAVING",
-            # For window functions
-            "WINDOW",
-            Ref("FrameClauseUnitGrammar"),
-            "SEPARATOR",
-        ),
-    )
-
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "DISTRIBUTE",
         "BY",
         Indent,
         Delimited(
             Sequence(
                 OneOf(
                     Ref("ColumnReferenceSegment"),
                     # Can `DISTRIBUTE BY 1`
                     Ref("NumericLiteralSegment"),
                     # Can distribute by an expression
                     Ref("ExpressionSegment"),
                 ),
             ),
             terminator=OneOf(
-                "WINDOW",
+                "SORT",
                 "LIMIT",
+                "HAVING",
+                # For window functions
+                "WINDOW",
                 Ref("FrameClauseUnitGrammar"),
-                "SORT",
+                "SEPARATOR",
             ),
         ),
         Dedent,
     )
 
 
 class HintFunctionSegment(BaseSegment):
@@ -1810,21 +1785,15 @@
 
 class GroupByClauseSegment(ansi.GroupByClauseSegment):
     """Enhance `GROUP BY` clause like in `SELECT` for 'CUBE' and 'ROLLUP`.
 
     https://spark.apache.org/docs/latest/sql-ref-syntax-qry-select-groupby.html
     """
 
-    match_grammar = StartsWith(
-        Sequence("GROUP", "BY"),
-        terminator=Ref("GroupByClauseTerminatorGrammar"),
-        enforce_whitespace_preceding_terminator=True,
-    )
-
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "GROUP",
         "BY",
         Indent,
         OneOf(
             Delimited(
                 Ref("ColumnReferenceSegment"),
                 # Can `GROUP BY 1`
@@ -1888,48 +1857,28 @@
     """`[CUBE | ROLLUP]` clause within the `GROUP BY` clause.
 
     https://spark.apache.org/docs/latest/sql-ref-syntax-qry-select-groupby.html
     """
 
     type = "cube_rollup_clause"
 
-    match_grammar = StartsWith(
-        OneOf("CUBE", "ROLLUP"),
-        terminator=OneOf(
-            "HAVING",
-            Sequence("ORDER", "BY"),
-            "LIMIT",
-            Ref("SetOperatorSegment"),
-        ),
-    )
-
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         OneOf("CUBE", "ROLLUP"),
         Bracketed(
             Ref("GroupingExpressionList"),
         ),
     )
 
 
 class GroupingSetsClauseSegment(BaseSegment):
     """`GROUPING SETS` clause within the `GROUP BY` clause."""
 
     type = "grouping_sets_clause"
 
-    match_grammar = StartsWith(
-        Sequence("GROUPING", "SETS"),
-        terminator=OneOf(
-            "HAVING",
-            Sequence("ORDER", "BY"),
-            "LIMIT",
-            Ref("SetOperatorSegment"),
-        ),
-    )
-
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "GROUPING",
         "SETS",
         Bracketed(
             Delimited(
                 Ref("CubeRollupClauseSegment"),
                 Ref("GroupingExpressionList"),
             )
@@ -1956,27 +1905,15 @@
 
     This clause is mutually exclusive with SORT BY, ORDER BY and DISTRIBUTE BY.
     https://spark.apache.org/docs/latest/sql-ref-syntax-qry-select-sortby.html
     """
 
     type = "sort_by_clause"
 
-    match_grammar = StartsWith(
-        Sequence("SORT", "BY"),
-        terminator=OneOf(
-            "LIMIT",
-            "HAVING",
-            "QUALIFY",
-            # For window functions
-            "WINDOW",
-            Ref("FrameClauseUnitGrammar"),
-            "SEPARATOR",
-        ),
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "SORT",
         "BY",
         Indent,
         Delimited(
             Sequence(
                 OneOf(
                     Ref("ColumnReferenceSegment"),
@@ -1989,15 +1926,20 @@
                 # NB: This isn't really ANSI, and isn't supported in Mysql,
                 # but is supported in enough other dialects for it to make
                 # sense here for now.
                 Sequence("NULLS", OneOf("FIRST", "LAST"), optional=True),
             ),
             terminator=OneOf(
                 "LIMIT",
+                "HAVING",
+                "QUALIFY",
+                # For window functions
+                "WINDOW",
                 Ref("FrameClauseUnitGrammar"),
+                "SEPARATOR",
             ),
         ),
         Dedent,
     )
 
 
 class SamplingExpressionSegment(ansi.SamplingExpressionSegment):
@@ -2878,15 +2820,18 @@
     """
 
     match_grammar = Sequence(
         Ref("PreTableFunctionKeywordsGrammar", optional=True),
         OptionallyBracketed(Ref("TableExpressionSegment")),
         Ref(
             "AliasExpressionSegment",
-            exclude=Ref("SamplingExpressionSegment"),
+            exclude=OneOf(
+                Ref("FromClauseTerminatorGrammar"),
+                Ref("SamplingExpressionSegment"),
+            ),
             optional=True,
         ),
         Ref("SamplingExpressionSegment", optional=True),
         # NB: `LateralViewClauseSegment`, `NamedWindowSegment`,
         # and `PivotClauseSegment should come after Alias/Sampling
         # expressions so those are matched before
         AnyNumberOf(Ref("LateralViewClauseSegment")),
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sparksql_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sparksql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sqlite.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sqlite.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Ref,
     Sequence,
     Delimited,
     TypedParser,
     Nothing,
     AnyNumberOf,
     Anything,
-    StartsWith,
+    Dedent,
 )
 from sqlfluff.dialects import dialect_ansi as ansi
 from sqlfluff.dialects.dialect_sqlite_keywords import (
     RESERVED_KEYWORDS,
     UNRESERVED_KEYWORDS,
 )
 
@@ -88,14 +88,22 @@
         Sequence("GROUP", "BY"),
         Sequence("ORDER", "BY"),
         "WINDOW",
         Ref("SetOperatorSegment"),
         Ref("WithNoSchemaBindingClauseSegment"),
         Ref("WithDataClauseSegment"),
     ),
+    GroupByClauseTerminatorGrammar=OneOf(
+        Sequence("ORDER", "BY"),
+        "LIMIT",
+        "HAVING",
+        "WINDOW",
+    ),
+    PostFunctionGrammar=Ref("FilterClauseGrammar"),
+    IgnoreRespectNullsGrammar=Nothing(),
     SelectClauseElementTerminatorGrammar=OneOf(
         "FROM",
         "WHERE",
         Sequence("ORDER", "BY"),
         "LIMIT",
         Ref("SetOperatorSegment"),
     ),
@@ -142,89 +150,23 @@
                 Ref("QuotedLiteralSegment"),
                 Ref("SingleIdentifierGrammar"),
                 Ref("ColumnReferenceSegment"),
             ),
         ),
         Ref("IndexColumnDefinitionSegment"),
     ),
-    Expression_A_Grammar=Sequence(
-        OneOf(
-            Ref("Expression_C_Grammar"),
-            Sequence(
-                OneOf(
-                    Ref("SignedSegmentGrammar"),
-                    # Ref('TildeSegment'),
-                    Ref("NotOperatorGrammar"),
-                    # used in CONNECT BY clauses (EXASOL, Snowflake, Postgres...)
-                ),
-                Ref("Expression_C_Grammar"),
-            ),
-        ),
-        AnyNumberOf(
-            OneOf(
-                Sequence(
-                    OneOf(
-                        Sequence(
-                            Ref.keyword("NOT", optional=True),
-                            Ref("LikeGrammar"),
-                        ),
-                        Sequence(
-                            Ref("BinaryOperatorGrammar"),
-                            Ref.keyword("NOT", optional=True),
-                        ),
-                        # We need to add a lot more here...
-                    ),
-                    Ref("Expression_C_Grammar"),
-                    Sequence(
-                        Ref.keyword("ESCAPE"),
-                        Ref("Expression_C_Grammar"),
-                        optional=True,
-                    ),
-                ),
-                Sequence(
-                    Ref.keyword("NOT", optional=True),
-                    "IN",
-                    Bracketed(
-                        OneOf(
-                            Delimited(
-                                Ref("Expression_A_Grammar"),
-                            ),
-                            Ref("SelectableGrammar"),
-                            ephemeral_name="InExpression",
-                        )
-                    ),
-                ),
-                Sequence(
-                    Ref.keyword("NOT", optional=True),
-                    "IN",
-                    Ref("FunctionSegment"),  # E.g. UNNEST()
-                ),
-                Sequence(
-                    "IS",
-                    Ref.keyword("NOT", optional=True),
-                    Ref("IsClauseGrammar"),
-                ),
-                Ref("IsNullGrammar"),
-                Ref("NotNullGrammar"),
-                Ref("CollateGrammar"),
-                Sequence(
-                    # e.g. NOT EXISTS, but other expressions could be met as
-                    # well by inverting the condition with the NOT operator
-                    "NOT",
-                    Ref("Expression_C_Grammar"),
-                ),
-                Sequence(
-                    Ref.keyword("NOT", optional=True),
-                    "BETWEEN",
-                    Ref("Expression_B_Grammar"),
-                    "AND",
-                    Ref("Expression_A_Grammar"),
-                ),
-            )
+    # NOTE: This block was copy/pasted from dialect_ansi.py with these changes made:
+    #  - "PRIOR" keyword removed from Expression_A_Unary_Operator_Grammar
+    Expression_A_Unary_Operator_Grammar=OneOf(
+        Ref(
+            "SignedSegmentGrammar",
+            exclude=Sequence(Ref("QualifiedNumericLiteralSegment")),
         ),
+        Ref("TildeSegment"),
+        Ref("NotOperatorGrammar"),
     ),
 )
 
 
 class SetOperatorSegment(BaseSegment):
     """A set operator such as Union, Minus, Except or Intersect."""
 
@@ -265,21 +207,21 @@
             ),
             Ref("BracketedArguments", optional=True),
         ),
     )
 
 
 class TableEndClauseSegment(BaseSegment):
-    """Support WITHOUT ROWID at end of tables.
+    """Support Table Options at end of tables.
 
-    https://www.sqlite.org/withoutrowid.html
+    https://www.sqlite.org/syntax/table-options.html
     """
 
     type = "table_end_clause_segment"
-    match_grammar: Matchable = Sequence("WITHOUT", "ROWID")
+    match_grammar: Matchable = Delimited(Sequence("WITHOUT", "ROWID"), "STRICT")
 
 
 class ValuesClauseSegment(ansi.ValuesClauseSegment):
     """A `VALUES` clause like in `INSERT`."""
 
     type = "values_clause"
     match_grammar: Matchable = Sequence(
@@ -363,33 +305,14 @@
                 Sequence("INITIALLY", "IMMEDIATE"),
                 optional=True,
             ),
         ],
     )
 
 
-class SelectClauseSegment(ansi.SelectClauseSegment):
-    """A group of elements in a select target statement."""
-
-    type = "select_clause"
-    match_grammar: Matchable = StartsWith(
-        "SELECT",
-        terminator=OneOf(
-            "FROM",
-            "WHERE",
-            Sequence("ORDER", "BY"),
-            "LIMIT",
-            Ref("SetOperatorSegment"),
-        ),
-        enforce_whitespace_preceding_terminator=True,
-    )
-
-    parse_grammar: Matchable = Ref("SelectClauseSegmentGrammar")
-
-
 class TableConstraintSegment(ansi.TableConstraintSegment):
     """Overriding TableConstraintSegment to allow for additional segment parsing."""
 
     match_grammar: Matchable = Sequence(
         Sequence(  # [ CONSTRAINT <Constraint name> ]
             "CONSTRAINT", Ref("ObjectReferenceSegment"), optional=True
         ),
@@ -486,20 +409,116 @@
         Bracketed(_pragma_value, optional=True),
         Sequence(
             Ref("EqualsSegment"), OptionallyBracketed(_pragma_value), optional=True
         ),
     )
 
 
+class CreateTriggerStatementSegment(ansi.CreateTriggerStatementSegment):
+    """Create Trigger Statement.
+
+    https://www.sqlite.org/lang_createtrigger.html
+    """
+
+    type = "create_trigger"
+
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        Ref("TemporaryGrammar", optional=True),
+        "TRIGGER",
+        Ref("IfNotExistsGrammar", optional=True),
+        Ref("TriggerReferenceSegment"),
+        OneOf("BEFORE", "AFTER", Sequence("INSTEAD", "OF"), optional=True),
+        OneOf(
+            "DELETE",
+            "INSERT",
+            Sequence(
+                "UPDATE",
+                Sequence(
+                    "OF",
+                    Delimited(
+                        Ref("ColumnReferenceSegment"),
+                    ),
+                    optional=True,
+                ),
+            ),
+        ),
+        "ON",
+        Ref("TableReferenceSegment"),
+        Sequence("FOR", "EACH", "ROW", optional=True),
+        Sequence("WHEN", Bracketed(Ref("ExpressionSegment")), optional=True),
+        "BEGIN",
+        Delimited(
+            Ref("UpdateStatementSegment"),
+            Ref("InsertStatementSegment"),
+            Ref("DeleteStatementSegment"),
+            Ref("SelectableGrammar"),
+            delimiter=AnyNumberOf(Ref("DelimiterGrammar"), min_times=1),
+            allow_gaps=True,
+            allow_trailing=True,
+        ),
+        "END",
+    )
+
+
+class SelectClauseSegment(BaseSegment):
+    """A group of elements in a select target statement.
+
+    Overriding ANSI to remove StartsWith logic which assumes statements have been
+    delimited
+    """
+
+    type = "select_clause"
+    match_grammar = Ref("SelectClauseSegmentGrammar")
+
+
+class UnorderedSelectStatementSegment(BaseSegment):
+    """A `SELECT` statement without any ORDER clauses or later.
+
+    Replaces (without overriding) ANSI to remove Greedy Matcher
+    """
+
+    type = "select_statement"
+
+    match_grammar = Sequence(
+        Ref("SelectClauseSegment"),
+        # Dedent for the indent in the select clause.
+        # It's here so that it can come AFTER any whitespace.
+        Dedent,
+        Ref("FromClauseSegment", optional=True),
+        Ref("WhereClauseSegment", optional=True),
+        Ref("GroupByClauseSegment", optional=True),
+        Ref("HavingClauseSegment", optional=True),
+        Ref("OverlapsClauseSegment", optional=True),
+        Ref("NamedWindowSegment", optional=True),
+    )
+
+
+class SelectStatementSegment(BaseSegment):
+    """A `SELECT` statement.
+
+    Replaces (without overriding) ANSI to remove Greedy Matcher
+    """
+
+    type = "select_statement"
+    # Remove the Limit and Window statements from ANSI
+    match_grammar = UnorderedSelectStatementSegment.match_grammar.copy(
+        insert=[
+            Ref("OrderByClauseSegment", optional=True),
+            Ref("FetchClauseSegment", optional=True),
+            Ref("LimitClauseSegment", optional=True),
+            Ref("NamedWindowSegment", optional=True),
+        ]
+    )
+
+
 class StatementSegment(ansi.StatementSegment):
     """Overriding StatementSegment to allow for additional segment parsing."""
 
-    match_grammar = ansi.StatementSegment.match_grammar
-
-    parse_grammar: Matchable = OneOf(
+    match_grammar = OneOf(
         Ref("AlterTableStatementSegment"),
         Ref("CreateIndexStatementSegment"),
         Ref("CreateTableStatementSegment"),
         Ref("CreateTriggerStatementSegment"),
         Ref("CreateViewStatementSegment"),
         Ref("DeleteStatementSegment"),
         Ref("DropIndexStatementSegment"),
@@ -510,7 +529,9 @@
         Ref("InsertStatementSegment"),
         Ref("PragmaStatementSegment"),
         Ref("SelectableGrammar"),
         Ref("TransactionStatementSegment"),
         Ref("UpdateStatementSegment"),
         Bracketed(Ref("StatementSegment")),
     )
+
+    parse_grammar = match_grammar
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sqlite_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sqlite_keywords.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,8 +196,9 @@
     "NORMAL",
     "FAST",
     "EXTRA",
     "FILE",
     "PASSIVE",
     "RESTART",
     "RESET",
+    "STRICT",
 ]
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_teradata.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_teradata.py`

 * *Files 2% similar despite different names*

```diff
@@ -692,16 +692,15 @@
     )
 
 
 class FromUpdateClauseSegment(BaseSegment):
     """A `FROM` clause like in `SELECT` but terminated by SET."""
 
     type = "from_in_update_clause"
-    match_grammar = StartsWith("FROM", terminator=Ref.keyword("SET"))
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "FROM",
         Delimited(
             # Optional old school delimited joins
             Ref("FromExpressionElementSegment"),
         ),
     )
 
@@ -741,20 +740,15 @@
 )
 
 
 class QualifyClauseSegment(BaseSegment):
     """A `QUALIFY` clause like in `SELECT`."""
 
     type = "qualify_clause"
-    match_grammar = StartsWith(
-        "QUALIFY",
-        terminator=OneOf(Sequence("ORDER", "BY"), "LIMIT", "QUALIFY", "WINDOW"),
-        enforce_whitespace_preceding_terminator=True,
-    )
-    parse_grammar = Sequence(
+    match_grammar = Sequence(
         "QUALIFY",
         Indent,
         OptionallyBracketed(Ref("ExpressionSegment")),
         Dedent,
     )
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_tsql.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_tsql.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,23 +271,14 @@
         OptionallyBracketed(Ref("ExpressionSegment")),
         Ref.keyword("PERCENT", optional=True),
     ),
     CursorNameGrammar=OneOf(
         Sequence(Ref.keyword("GLOBAL", optional=True), Ref("NakedIdentifierSegment")),
         Ref("ParameterNameSegment"),
     ),
-    CollationSegment=SegmentGenerator(
-        # Generate the anti template from the set of reserved keywords
-        lambda dialect: RegexParser(
-            r"[A-Z][A-Za-z0-9_]*[A-Za-z0-9_]",
-            CodeSegment,
-            type="collation",
-            anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
-        )
-    ),
     SqlcmdOperatorSegment=SegmentGenerator(
         lambda dialect: MultiStringParser(
             dialect.sets("sqlcmd_operators"),
             CodeSegment,
             type="sqlcmd_operator",
         )
     ),
@@ -426,15 +417,14 @@
         ),
         # NB: The Dedent for the indent above lives in the
         # SelectStatementSegment so that it sits in the right
         # place corresponding to the whitespace.
     ),
     FromClauseTerminatorGrammar=OneOf(
         "WHERE",
-        "LIMIT",
         Sequence("GROUP", "BY"),
         Sequence("ORDER", "BY"),
         "HAVING",
         Ref("SetOperatorSegment"),
         Ref("WithNoSchemaBindingClauseSegment"),
         Ref("DelimiterGrammar"),
     ),
@@ -551,15 +541,15 @@
     ),
     TrimParametersGrammar=Nothing(),
     TemporaryGrammar=Nothing(),
     JoinLikeClauseGrammar=AnySetOf(
         Ref("PivotUnpivotStatementSegment"),
         min_times=1,
     ),
-    CollateGrammar=Sequence("COLLATE", Ref("CollationSegment")),
+    CollateGrammar=Sequence("COLLATE", Ref("CollationReferenceSegment")),
 )
 
 
 class StatementSegment(ansi.StatementSegment):
     """Overriding StatementSegment to allow for additional segment parsing."""
 
     match_grammar = ansi.StatementSegment.parse_grammar.copy(
@@ -2147,15 +2137,15 @@
             "CONSTRAINT",
             Ref("ObjectReferenceSegment"),  # Constraint name
             optional=True,
         ),
         OneOf(
             "FILESTREAM",
             Sequence(
-                "COLLATE", Ref("ObjectReferenceSegment")
+                "COLLATE", Ref("CollationReferenceSegment")
             ),  # [COLLATE collation_name]
             "SPARSE",
             Sequence(
                 "MASKED",
                 "WITH",
                 Bracketed("FUNCTION", Ref("EqualsSegment"), Ref("LiteralGrammar")),
             ),
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_tsql_keywords.py` & `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_tsql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/diff_quality_plugin.py` & `sqlfluff-2.0.6/src/sqlfluff/diff_quality_plugin.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL01.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL02.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL03.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL04.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL05.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL05.py`

 * *Files 12% similar despite different names*

```diff
@@ -75,19 +75,43 @@
         assert context.segment.is_type("select_statement")
         # Exit early if the SELECT does not define any aliases.
         select_info = get_select_statement_info(context.segment, context.dialect)
         if not select_info or not select_info.table_aliases:
             return None
 
         # Analyze the SELECT.
+        alias: AliasInfo
         crawler = SelectCrawler(context.segment, context.dialect, query_class=AL05Query)
         query: AL05Query = cast(AL05Query, crawler.query_tree)
         self._analyze_table_aliases(query, context.dialect)
 
-        alias: AliasInfo
+        if context.dialect.name == "redshift":
+            # Redshift supports un-nesting using aliases.
+            # Detect that situation and ignore.
+            # https://docs.aws.amazon.com/redshift/latest/dg/query-super.html#unnest
+
+            # Do any references refer to aliases in the same list?
+            references = set()
+            aliases = set()
+
+            for alias in query.aliases:
+                aliases.add(alias.ref_str)
+                if not alias.object_reference:
+                    continue  # pragma: no cover
+                for seg in alias.object_reference.segments:
+                    if seg.is_type("identifier"):
+                        references.add(seg.raw)
+
+            # If there's any overlap between aliases and reference
+            if aliases.intersection(references):
+                self.logger.debug(
+                    "Overlapping references found. Assuming redshift semi-structured."
+                )
+                return None
+
         for alias in query.aliases:
             # Skip alias if it's required (some dialects require aliases for
             # VALUES clauses).
             if alias.from_expression_element and self._is_alias_required(
                 alias.from_expression_element, context.dialect.name
             ):
                 continue
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL06.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL07.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM01.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM02.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM03.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM04.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM05.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM06.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM07.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP01.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP02.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP03.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP04.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP05.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV01.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV02.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV03.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV04.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV05.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV06.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV07.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV08.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV09.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV10.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV11.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/convention/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/convention/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/jinja/JJ01.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/jinja/JJ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT01.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT02.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT03.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT04.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT05.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT06.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT07.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT08.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT09.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT10.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT11.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT12.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT12.py`

 * *Files 9% similar despite different names*

```diff
@@ -98,16 +98,18 @@
             a
         FROM foo
         ;
         $
 
     """
 
-    name = "layout.end-of-file"
-    aliases = ("L009",)
+    name = "layout.end_of_file"
+    # Between 2.0.0 and 2.0.4 we supported had a kebab-case name for this rule
+    # so the old name remains here as an alias to enable backward compatibility.
+    aliases = ("L009", "layout.end-of-file")
     groups = ("all", "core", "layout")
 
     targets_templated = True
     # Use the RootOnlyCrawler to only call _eval() ONCE, with the root segment.
     crawl_behaviour = RootOnlyCrawler()
     lint_phase = "post"
     is_fix_compatible = True
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT13.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT13.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/layout/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/references/RF01.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/references/RF01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/references/RF02.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/references/RF02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/references/RF03.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/references/RF03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/references/RF04.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/references/RF04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/references/RF05.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/references/RF05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/references/RF06.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/references/RF06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/references/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/references/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST01.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST02.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST03.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST04.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST05.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST06.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST07.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST08.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/structure/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/rules/tsql/TQ01.py` & `sqlfluff-2.0.6/src/sqlfluff/rules/tsql/TQ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/analysis/select.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/analysis/select.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/analysis/select_crawler.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/analysis/select_crawler.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/functional/__init__.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/functional/context.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/functional/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/functional/raw_file_slice_predicates.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/functional/raw_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/functional/raw_file_slices.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/functional/raw_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/functional/segment_predicates.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/functional/segment_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/functional/segments.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/functional/segments.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/functional/templated_file_slice_predicates.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/functional/templated_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/functional/templated_file_slices.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/functional/templated_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/identifers.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/identifers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/config.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/depthmap.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/depthmap.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/elements.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/elements.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Dataclasses for reflow work."""
 
 from itertools import chain
 import logging
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Dict, List, Optional, Sequence, Set, Tuple, Type, Union, cast
 
 from sqlfluff.core.parser import PositionMarker
 from sqlfluff.core.parser.segments import (
     BaseSegment,
     RawSegment,
     NewlineSegment,
@@ -243,15 +243,15 @@
         return cls(
             first.impulse + second.impulse,
             min(first.trough, first.impulse + second.trough),
             second.implicit_indents,
         )
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, init=False)
 class ReflowPoint(ReflowElement):
     """Class for keeping track of editable elements in reflow.
 
     This class, and its sibling :obj:`ReflowBlock`, should not
     normally be manipulated directly by rules, but instead should
     be manipulated using :obj:`ReflowSequence`.
 
@@ -260,14 +260,21 @@
     and :obj:`Dedent` elements.
 
     It holds no configuration and is influenced by the blocks on either
     side, so that any operations on it usually have that configuration
     passed in as required.
     """
 
+    _stats: IndentStats = field(init=False)
+
+    def __init__(self, segments: Tuple[RawSegment, ...]):
+        """Override the init method to calculate indent stats."""
+        object.__setattr__(self, "segments", segments)
+        object.__setattr__(self, "_stats", self._generate_indent_stats(segments))
+
     def _get_indent_segment(self) -> Optional[RawSegment]:
         """Get the current indent segment (if there).
 
         NOTE: This only returns _untemplated_ indents. If templated
         newline or whitespace segments are found they are skipped.
         """
         indent = None
@@ -304,54 +311,44 @@
         if consumed_whitespace:  # pragma: no cover
             # Return last bit after newline.
             # NOTE: Not tested, because usually this would happen
             # directly via _get_indent_segment.
             return consumed_whitespace.split("\n")[-1]
         return seg.raw if seg else ""
 
-    def get_indent_impulse(
-        self,
-        allow_implicit_indents: bool = False,
-        following_class_types: Set[str] = set(),
+    @staticmethod
+    def _generate_indent_stats(
+        segments: Sequence[RawSegment],
     ) -> IndentStats:
-        """Get the change in intended indent balance from this point.
+        """Generate the change in intended indent balance.
 
-        NOTE: The reason we check `following_class_types` is because
-        bracketed expressions behave a little differently and are an
-        exception to the normal implicit indent rules. For implicit
-        indents which precede bracketed expressions, the implicit indent
-        is treated as a normal indent.
-
-        Returns:
-            :obj:`tuple` of :obj:`int`: The first value is the raw
-                impulse. The second is the deepest trough in the indent
-                through the values to allow wiping of buffers.
+        This is the main logic which powers .get_indent_impulse()
         """
         trough = 0
         running_sum = 0
         implicit_indents = []
-        for seg in self.segments:
+        for seg in segments:
             if seg.is_type("indent"):
                 indent_seg = cast(Indent, seg)
                 running_sum += indent_seg.indent_val
                 # Do we need to add a new implicit indent?
-                if (
-                    allow_implicit_indents
-                    and indent_seg.is_implicit
-                    and "start_bracket" not in following_class_types
-                ):
+                if indent_seg.is_implicit:
                     implicit_indents.append(running_sum)
                 # NOTE: We don't check for removal of implicit indents
                 # because it's unlikely that one would be opened, and then
                 # closed within the same point. That would probably be the
                 # sign of a bug in the dialect.
             if running_sum < trough:
                 trough = running_sum
         return IndentStats(running_sum, trough, tuple(implicit_indents))
 
+    def get_indent_impulse(self) -> IndentStats:
+        """Get the change in intended indent balance from this point."""
+        return self._stats
+
     def indent_to(
         self,
         desired_indent: str,
         after: Optional[BaseSegment] = None,
         before: Optional[BaseSegment] = None,
         description: Optional[str] = None,
         source: Optional[str] = None,
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/helpers.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/rebreak.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/rebreak.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/reindent.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/reindent.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,32 +268,33 @@
     # Because we want to modify the original lines, we're going
     # to use their list index to keep track of them.
     depths = defaultdict(list)
     grouped = defaultdict(list)
     for idx, line in enumerate(lines):
         if line.is_all_templates(elements):
             # We can't assume they're all a single block.
-            # But if they _start_ with a block, we should
-            # respect the indent of that block.
-            segment = cast(
-                MetaSegment, elements[line.indent_points[-1].idx - 1].segments[0]
-            )
-            assert segment.is_type("placeholder", "template_loop")
-            # If it's not got a block uuid, it's not a block, so it
-            # should just be indented as usual. No need to revise.
-            # e.g. comments or variables
-            if segment.block_uuid:
-                grouped[segment.block_uuid].append(idx)
-                depths[segment.block_uuid].append(line.initial_indent_balance)
-                reflow_logger.debug(
-                    "  UUID: %s @ %s = %r",
-                    segment.block_uuid,
-                    idx,
-                    segment.pos_marker.source_str(),
-                )
+            # So handle all blocks on the line.
+            for i in range(line.indent_points[0].idx, line.indent_points[-1].idx):
+                if isinstance(elements[i], ReflowPoint):
+                    continue
+                # We already checked that it's all templates.
+                segment = cast(MetaSegment, elements[i].segments[0])
+                assert segment.is_type("placeholder", "template_loop")
+                # If it's not got a block uuid, it's not a block, so it
+                # should just be indented as usual. No need to revise.
+                # e.g. comments or variables
+                if segment.block_uuid:
+                    grouped[segment.block_uuid].append(idx)
+                    depths[segment.block_uuid].append(line.initial_indent_balance)
+                    reflow_logger.debug(
+                        "  UUID: %s @ %s = %r",
+                        segment.block_uuid,
+                        idx,
+                        segment.pos_marker.source_str(),
+                    )
 
     # Sort through the lines, so we do to *most* indented first.
     sorted_group_indices = sorted(
         grouped.keys(), key=lambda x: max(depths[x]), reverse=True
     )
     reflow_logger.debug("  Sorted Group UUIDs: %s", sorted_group_indices)
 
@@ -488,37 +489,37 @@
                         )
                     # NOTE: We update net_balance _after_ the clause above.
                     net_balance += ip.indent_impulse
 
         # Evaluate options.
         # NOTE: We don't use the _last_ option, because it tends to be trailing
         # and have strange effects.
+        reflow_logger.debug("    Options: %s", options)
         overlap = set.intersection(*options[:-1])
         reflow_logger.debug("    Simple Overlap: %s", overlap)
         # Remove any options above the limit option.
         # We minus one from the limit, because if it comes into effect
         # we'll effectively remove the effects of the indents between the elements.
 
-        best_indent = max(overlap)
-
         # Is there a mutually agreeable option?
         reflow_logger.debug("    Balance Trough: %s", balance_trough)
-        if balance_trough is not None and balance_trough <= 0:
+        if not overlap or (balance_trough is not None and balance_trough <= 0):
             # Set the indent to the minimum of the existing ones.
             best_indent = min(lines[idx].initial_indent_balance for idx in group_lines)
             reflow_logger.debug(
                 "    Case 3: Best: %s. Inner Lines: %s", best_indent, inner_lines
             )
             # Remove one indent from all intermediate lines.
             # This is because we're effectively saying that these
             # placeholders shouldn't impact the indentation within them.
             for idx in inner_lines:
                 # MUTATION
                 lines[idx].initial_indent_balance -= 1
         else:
+            best_indent = max(overlap)
             reflow_logger.debug(
                 "    Case 2: Best: %s, Overlap: %s", best_indent, overlap
             )
 
         # Set all the lines to this indent
         for idx in group_lines:
             # MUTATION
@@ -675,17 +676,30 @@
             # NOTE: The following line should never lead to an index error
             # because files should always have a trailing IndentBlock containing
             # an "end_of_file" marker, and so the final IndentPoint should always
             # have _something_ after it.
             following_class_types = elements[idx + 1].class_types
             indent_stats = IndentStats.from_combination(
                 cached_indent_stats,
-                elem.get_indent_impulse(allow_implicit_indents, following_class_types),
+                elem.get_indent_impulse(),
             )
 
+            # If don't allow implicit indents we should remove them here.
+            # Also, if we do - we should check for brackets.
+            # NOTE: The reason we check `following_class_types` is because
+            # bracketed expressions behave a little differently and are an
+            # exception to the normal implicit indent rules. For implicit
+            # indents which precede bracketed expressions, the implicit indent
+            # is treated as a normal indent.
+            if not allow_implicit_indents or "start_bracket" in following_class_types:
+                # Blank indent stats if not using them
+                indent_stats = IndentStats(
+                    indent_stats.impulse, indent_stats.trough, ()
+                )
+
             # Was there a cache?
             if cached_indent_stats:
                 # If there was we can safely assume there is a cached point.
                 assert cached_point
                 # If there was, this is a signal that we need to yield two points.
                 # The content of those points depends on the newlines that surround the
                 # last segments (which will be comment block).
@@ -798,14 +812,15 @@
             is untaken, but its corresponding negative indent *is*
             taken.
 
     """
     # First build up the buffer of lines.
     lines = []
     point_buffer = []
+    _previous_points = {}
     # Buffers to keep track of indents which are untaken on the way
     # up but taken on the way down. We track them explicitly so we
     # can force them later.
 
     #: dict of ints: maps indentation balance values to the last
     #: index location where they were seen. This is a working buffer
     #: and not directly returned by the function.
@@ -818,14 +833,15 @@
 
     for indent_point in _crawl_indent_points(
         elements, allow_implicit_indents=allow_implicit_indents
     ):
         # We evaluate all the points in a line at the same time, so
         # we first build up a buffer.
         point_buffer.append(indent_point)
+        _previous_points[indent_point.idx] = indent_point
 
         if not indent_point.is_line_break:
             # If it's not a line break, we should still check whether it's
             # a positive untaken to keep track of them.
             if indent_point.indent_impulse > indent_point.indent_trough:
                 untaken_indent_locs[
                     indent_point.initial_indent_balance + indent_point.indent_impulse
@@ -864,40 +880,62 @@
                     indent_point.initial_indent_balance,
                     indent_point.initial_indent_balance + indent_point.indent_trough,
                     -1,
                 )
             )
             # There might be many indents at this point, but if any match, then
             # we should still force an indent
-            if any(i in indent_point.untaken_indents for i in passing_indents):
-                for i in passing_indents:
-                    # If we don't have the location of the untaken indent, then
-                    # skip it for now. TODO: Check this isn't a bug when this happens.
-                    # It seems very rare for now.
-                    if i not in untaken_indent_locs:
-                        continue
 
-                    loc = untaken_indent_locs[i]
+            # NOTE: We work _inward_ to check which have been taken.
+            for i in reversed(passing_indents):
+                # Was this outer one untaken?
+                if i not in untaken_indent_locs:
+                    # No? Stop the loop. If we've a corresponding indent for
+                    # this dedent, we shouldn't use the same location to force
+                    # untaken indents at inner levels.
+                    break
+
+                loc = untaken_indent_locs[i]
 
-                    # First check for bracket special case. It's less about whether
-                    # the section _ends_ with a lone bracket, and more about whether
-                    # the _starting point_ is a bracket which closes a line. If it
-                    # is, then skip this location. (Special case 2).
-                    # NOTE: We can safely "look ahead" here because we know all files
-                    # end with an IndentBlock, and we know here that `loc` refers to
-                    # an IndentPoint.
-                    if "start_bracket" in elements[loc + 1].class_types:
+                # First check for bracket special case. It's less about whether
+                # the section _ends_ with a lone bracket, and more about whether
+                # the _starting point_ is a bracket which closes a line. If it
+                # is, then skip this location. (Special case 2).
+                # NOTE: We can safely "look ahead" here because we know all files
+                # end with an IndentBlock, and we know here that `loc` refers to
+                # an IndentPoint.
+                if "start_bracket" in elements[loc + 1].class_types:
+                    continue
+
+                # If the location was in the line we're just closing. That's
+                # not a problem because it's an untaken indent which is closed
+                # on the same line.
+                if any(ip.idx == loc for ip in point_buffer):
+                    continue
+
+                # If the only elements between current point and the end of the
+                # reference line are comments, then don't trigger, it's a misplaced
+                # indent.
+                # First find the end of the reference line.
+                for j in range(loc, indent_point.idx):
+                    _pt = _previous_points.get(j, None)
+                    if not _pt:
                         continue
+                    if _pt.is_line_break:
+                        break
+                assert _pt
+                # Then check if all comments.
+                if all(
+                    "comment" in elements[k].class_types
+                    for k in range(_pt.idx + 1, indent_point.idx, 2)
+                ):
+                    # It is all comments. Ignore it.
+                    continue
 
-                    # If the location was in the line we're just closing. That's
-                    # not a problem because it's an untaken indent which is closed
-                    # on the same line. Otherwise it is - append it to the buffer
-                    # to sort later.
-                    if not any(ip.idx == loc for ip in point_buffer):
-                        imbalanced_locs.append(loc)
+                imbalanced_locs.append(loc)
 
         # Remove any which are now no longer relevant from the working buffer.
         for k in list(untaken_indent_locs.keys()):
             if k > indent_point.initial_indent_balance + indent_point.indent_trough:
                 del untaken_indent_locs[k]
 
         # Reset the buffer
@@ -915,15 +953,17 @@
 ) -> str:
     """Deduce the current indent string.
 
     This method accounts for both literal indents and indents
     consumed from the source as by potential templating tags.
     """
     indent_seg = None
-    if last_line_break_idx:
+    if not elements[0].segments:
+        return ""
+    elif last_line_break_idx:
         indent_seg = cast(
             ReflowPoint, elements[last_line_break_idx]
         )._get_indent_segment()
     elif isinstance(elements[0], ReflowPoint) and elements[0].segments[
         0
     ].pos_marker.working_loc == (1, 1):
         # No last_line_break_idx, but this is a point. It's the first line.
@@ -998,27 +1038,38 @@
     desired_indent_units = indent_line.desired_indent_units(forced_indents)
     desired_starting_indent = desired_indent_units * single_indent
     initial_point = cast(ReflowPoint, elements[initial_point_idx])
 
     if current_indent == desired_starting_indent:
         return []
 
-    # Edge case: Multiline comments. If the previous line was a multiline
-    # comment and this line starts with a multiline comment, then we should
-    # only lint the indent if it's _too small_. Otherwise we risk destroying
-    # indentation which the logic here is not smart enough to handle.
-    if (
-        initial_point_idx > 0
-        and initial_point_idx < len(elements) - 1
-        and "block_comment" in elements[initial_point_idx - 1].class_types
-        and "block_comment" in elements[initial_point_idx + 1].class_types
-    ):
-        if len(current_indent) > len(desired_starting_indent):
-            reflow_logger.debug("    Indent is bigger than required. OK.")
-            return []
+    if initial_point_idx > 0 and initial_point_idx < len(elements) - 1:
+        # Edge case: Lone comments. Normally comments are anchored to the line
+        # _after_ where they come. However, if the existing location _matches_
+        # the _preceding line_, then we will allow it. It's not the "expected"
+        # location but it is allowable.
+        if "comment" in elements[initial_point_idx + 1].class_types:
+            last_indent = _deduce_line_current_indent(
+                elements, indent_points[0].last_line_break_idx
+            )
+            if len(current_indent) == len(last_indent):
+                reflow_logger.debug("    Indent matches previous line. OK.")
+                return []
+
+        # Edge case: Multiline comments. If the previous line was a multiline
+        # comment and this line starts with a multiline comment, then we should
+        # only lint the indent if it's _too small_. Otherwise we risk destroying
+        # indentation which the logic here is not smart enough to handle.
+        if (
+            "block_comment" in elements[initial_point_idx - 1].class_types
+            and "block_comment" in elements[initial_point_idx + 1].class_types
+        ):
+            if len(current_indent) > len(desired_starting_indent):
+                reflow_logger.debug("    Indent is bigger than required. OK.")
+                return []
 
     reflow_logger.debug(
         "    Correcting indent @ line %s. Existing indent: %r -> %r",
         elements[initial_point_idx + 1].segments[0].pos_marker.working_line_no,
         current_indent,
         desired_starting_indent,
     )
@@ -1109,14 +1160,30 @@
     indent_points = indent_line.indent_points
 
     # Account for the closing trough.
     closing_trough = last_ip.initial_indent_balance + (
         last_ip.indent_trough or last_ip.indent_impulse
     )
 
+    # Edge case: Adjust closing trough for trailing indents
+    # after comments disrupting closing trough.
+    _bal = 0
+    for elem in elements[last_ip.idx + 1 :]:
+        if not isinstance(elem, ReflowPoint):
+            if "comment" not in elem.class_types:
+                break
+            continue
+        # Otherwise it's a point
+        stats = elem.get_indent_impulse()
+        # If it's positive, stop. We likely won't find enough negative to come.
+        if stats.impulse > 0:  # pragma: no cover
+            break
+        closing_trough = _bal + stats.trough
+        _bal += stats.impulse
+
     # On the way up we're looking for whether the ending balance
     # was an untaken indent or not. If it *was* untaken, there's
     # a good chance that we *should* take it.
     # NOTE: an implicit indent would not force a newline
     # because it wouldn't be in the untaken_indents. It's
     # considered _taken_ even if not.
     if closing_trough not in indent_points[-1].untaken_indents:
@@ -1610,15 +1677,15 @@
             continue
 
         # As usual, indents are referred to by their "uphill" side
         # so what number we store the point against depends on whether
         # it's positive or negative.
         # NOTE: Here we don't actually pass in the forward types because
         # we don't need them for the output. It doesn't make a difference.
-        indent_stats = e.get_indent_impulse(allow_implicit_indents, set())
+        indent_stats = e.get_indent_impulse()
         e_idx = newline_idx - len(line_elements) + idx + 1
         # Save any implicit indents.
         if indent_stats.implicit_indents:
             implicit_indents[e_idx] = indent_stats.implicit_indents
         balance, nmi = _increment_balance(balance, indent_stats, e_idx)
         # Incorporate nmi into matched_indents
         for b, indices in nmi.items():
@@ -1799,38 +1866,22 @@
 
 def _fix_long_line_with_integer_targets(
     elements: ReflowSequenceType,
     target_breaks: List[int],
     line_length_limit: int,
     inner_indent: str,
     outer_indent: str,
-    allow_implicit_indents: bool,
 ) -> List[LintResult]:
     """Work out fixes for splitting a long line at locations like indents.
 
     NOTE: This mutates `elements` to avoid copying.
 
     This is a helper function within .lint_line_length().
     """
     line_results = []
-    # Create a stash of indent_stats. We're going to need them
-    # twice, so we generate them one for later use.
-    _indent_stats_cache: Dict[int, IndentStats] = {}
-    for e_idx in target_breaks:
-        # Generate indent stats for it.
-        e = cast(ReflowPoint, elements[e_idx])
-        # We need to check for negative sections so they get the right
-        # indent (otherwise they'll be over indented).
-        # The `desired_indent` above is for the "uphill" side.
-        following_class_types = elements[e_idx + 1].class_types
-        indent_stats = e.get_indent_impulse(
-            allow_implicit_indents, following_class_types
-        )
-        # Cache them for later
-        _indent_stats_cache[e_idx] = indent_stats
 
     # If we can get to the uphill indent of later break, and still be within
     # the line limit, then we can skip everything before it.
     purge_before = 0
     for e_idx in target_breaks:
         # Is the following block already past the limit?
         # NOTE: We use the block because we know it will have segments.
@@ -1841,31 +1892,30 @@
         if (
             elements[e_idx + 1].segments[0].pos_marker.working_line_pos
             > line_length_limit
         ):
             # If we're past the line length limit, stop looking.
             break
 
-        # Fetch cached indent stats
-        indent_stats = _indent_stats_cache[e_idx]
-        if indent_stats.trough < 0:
+        e = cast(ReflowPoint, elements[e_idx])
+        if e.get_indent_impulse().trough < 0:
             # It's negative. Skip onward.
             continue
 
         # If we get this far, then it's positive, but still within
         # the line limit. We can purge any pairs before this.
         purge_before = e_idx
         reflow_logger.debug("    ...breaks before %s unnecessary.", purge_before)
     # Only keep indices which are after the critical point.
     target_breaks = [e_idx for e_idx in target_breaks if e_idx >= purge_before]
     reflow_logger.debug("    Remaining breaks: %s.", target_breaks)
 
     for e_idx in target_breaks:
         e = cast(ReflowPoint, elements[e_idx])
-        indent_stats = _indent_stats_cache[e_idx]
+        indent_stats = e.get_indent_impulse()
         # NOTE: We check against the _impulse_ here rather than the
         # _trough_ because if we're about to step back up again then
         # it should still be indented.
         if indent_stats.impulse < 0:
             new_indent = outer_indent
             # NOTE: If we're about to insert a dedent before a
             # comma or semicolon ... don't. They are a bit special
@@ -2101,15 +2151,14 @@
                 if target_balance % 1 == 0:
                     line_results = _fix_long_line_with_integer_targets(
                         elem_buffer,
                         target_breaks,
                         line_length_limit,
                         desired_indent,
                         current_indent,
-                        allow_implicit_indents=allow_implicit_indents,
                     )
                 else:
                     line_results = _fix_long_line_with_fractional_targets(
                         elem_buffer, target_breaks, desired_indent
                     )
 
                 # Consolidate all the results for the line into one.
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/respace.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/respace.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,19 @@
         # If it's whitespace, store it.
         if seg.is_type("whitespace"):
             last_whitespace.append(seg)
 
         # If it's a newline, react accordingly.
         # NOTE: This should only trigger on literal newlines.
         elif seg.is_type("newline", "end_of_file"):
+            if seg.pos_marker and not seg.pos_marker.is_literal():
+                last_whitespace = []
+                reflow_logger.debug("    Skipping templated newline: %s", seg)
+                continue
+
             # Are we stripping newlines?
             if strip_newlines and seg.is_type("newline"):
                 reflow_logger.debug("    Stripping newline: %s", seg)
                 removal_buffer.append(seg)
                 result_buffer.append(
                     LintResult(
                         seg, [LintFix.delete(seg)], description="Unexpected line break."
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/sequence.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/testing/cli.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/testing/cli.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/testing/logging.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/testing/logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff/utils/testing/rules.py` & `sqlfluff-2.0.6/src/sqlfluff/utils/testing/rules.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff.egg-info/PKG-INFO` & `sqlfluff-2.0.6/src/sqlfluff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.0.5
+Version: 2.0.6
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
@@ -136,15 +136,15 @@
 L:   1 | P:  11 | LT01 | Expected only single space before binary operator '+'.
                        | Found '  '. [layout.spacing]
 L:   1 | P:  14 | LT01 | Expected only single space before naked identifier.
                        | Found '  '. [layout.spacing]
 L:   1 | P:  27 | LT01 | Unnecessary trailing whitespace at end of file.
                        | [layout.spacing]
 L:   1 | P:  27 | LT12 | Files must end with a single trailing newline.
-                       | [layout.end-of-file]
+                       | [layout.end_of_file]
 All Finished 📜 🎉!
 ```
 
 Alternatively, you can use the [**Official SQLFluff Docker Image**](https://hub.docker.com/r/sqlfluff/sqlfluff)
 or have a play using [**SQLFluff online**](https://online.sqlfluff.com/).
 
 For full [CLI usage](https://docs.sqlfluff.com/en/stable/cli.html) and
```

### Comparing `sqlfluff-2.0.5/src/sqlfluff.egg-info/SOURCES.txt` & `sqlfluff-2.0.6/src/sqlfluff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/src/sqlfluff.egg-info/entry_points.txt` & `sqlfluff-2.0.6/src/sqlfluff.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.5/test/test_testing.py` & `sqlfluff-2.0.6/test/test_testing.py`

 * *Files identical despite different names*

