# Comparing `tmp/liiatools-0.1.5.0.tar.gz` & `tmp/liiatools-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liiatools-0.1.5.0.tar", max compression
+gzip compressed data, was "liiatools-0.1.5.1.tar", max compression
```

## Comparing `liiatools-0.1.5.0.tar` & `liiatools-0.1.5.1.tar`

### file list

```diff
@@ -1,103 +1,129 @@
--rw-r--r--   0        0        0     1084 2023-04-14 07:55:59.245828 liiatools-0.1.5.0/LICENSE
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.245828 liiatools-0.1.5.0/liiatools/__init__.py
--rw-r--r--   0        0        0      434 2023-04-14 07:55:59.245828 liiatools-0.1.5.0/liiatools/__main__.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.245828 liiatools-0.1.5.0/liiatools/csdatatools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.245828 liiatools-0.1.5.0/liiatools/csdatatools/datasets/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.245828 liiatools-0.1.5.0/liiatools/csdatatools/datasets/cincensus/__init__.py
--rw-r--r--   0        0        0     4364 2023-04-14 07:55:59.245828 liiatools-0.1.5.0/liiatools/csdatatools/datasets/cincensus/filters.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/csdatatools/util/__init__.py
--rw-r--r--   0        0        0      280 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/csdatatools/util/stream.py
--rw-r--r--   0        0        0     1640 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/csdatatools/util/xml.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/__init__.py
--rw-r--r--   0        0        0      131 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/README.md
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/__init__.py
--rw-r--r--   0        0        0     7047 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/annex_a_cli.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/__init__.py
--rw-r--r--   0        0        0     4908 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/cleaner.py
--rw-r--r--   0        0        0    11751 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/configuration.py
--rw-r--r--   0        0        0      451 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/converters.py
--rw-r--r--   0        0        0     1381 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/degrade.py
--rw-r--r--   0        0        0     5122 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/file_creator.py
--rw-r--r--   0        0        0    12608 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/logger.py
--rw-r--r--   0        0        0      772 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/populate.py
--rw-r--r--   0        0        0      885 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/regex.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_la_agg/__init__.py
--rw-r--r--   0        0        0     2495 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_la_agg/configuration.py
--rw-r--r--   0        0        0     3052 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_la_agg/process.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_pan_agg/__init__.py
--rw-r--r--   0        0        0     2894 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_pan_agg/configuration.py
--rw-r--r--   0        0        0     2066 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_pan_agg/process.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/__init__.py
--rw-r--r--   0        0        0    11514 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/cin_cli.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_clean/__init__.py
--rw-r--r--   0        0        0     6065 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_clean/cin_record.py
--rw-r--r--   0        0        0     2644 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_clean/configuration.py
--rw-r--r--   0        0        0      811 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_clean/converter.py
--rw-r--r--   0        0        0     2906 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_clean/file_creator.py
--rw-r--r--   0        0        0     6012 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_clean/logger.py
--rw-r--r--   0        0        0      410 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_clean/schema.py
--rw-r--r--   0        0        0     3860 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_clean/validator.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_la_agg/__init__.py
--rw-r--r--   0        0        0     2487 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_la_agg/configuration.py
--rw-r--r--   0        0        0    10532 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_la_agg/process.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_pan_agg/__init__.py
--rw-r--r--   0        0        0     2885 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_pan_agg/configuration.py
--rw-r--r--   0        0        0    10132 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_pan_agg/process.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/__init__.py
--rw-r--r--   0        0        0     1547 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/columns.py
--rw-r--r--   0        0        0     5105 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/configuration.py
--rw-r--r--   0        0        0     1612 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/converters.py
--rw-r--r--   0        0        0     1248 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/degrade.py
--rw-r--r--   0        0        0     2993 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/file_creator.py
--rw-r--r--   0        0        0     3184 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/filters.py
--rw-r--r--   0        0        0     8547 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/logger.py
--rw-r--r--   0        0        0     1189 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/parse.py
--rw-r--r--   0        0        0     2000 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/populate.py
--rw-r--r--   0        0        0     5080 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/prep.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_la_agg/__init__.py
--rw-r--r--   0        0        0     2486 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_la_agg/configuration.py
--rw-r--r--   0        0        0     2425 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_la_agg/process.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_pan_agg/__init__.py
--rw-r--r--   0        0        0     2885 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_pan_agg/configuration.py
--rw-r--r--   0        0        0     1482 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_pan_agg/process.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_sufficiency/__init__.py
--rw-r--r--   0        0        0     2491 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_sufficiency/configuration.py
--rw-r--r--   0        0        0     1078 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_sufficiency/process.py
--rw-r--r--   0        0        0     4704 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/s903_cli.py
--rw-r--r--   0        0        0     6921 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/s903/s903_main_functions.py
--rw-r--r--   0        0        0        1 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/school_census/__init__.py
--rw-r--r--   0        0        0        1 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/school_census/lds_school_clean/__init__.py
--rw-r--r--   0        0        0        1 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/school_census/lds_school_la_agg/__init__.py
--rw-r--r--   0        0        0     6324 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/shared_functions/common.py
--rw-r--r--   0        0        0     1827 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/shared_functions/converters.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/social_work_workforce/__init__.py
--rw-r--r--   0        0        0      829 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/social_work_workforce/csww_cli.py
--rw-r--r--   0        0        0      839 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/social_work_workforce/csww_main_functions.py
--rw-r--r--   0        0        0     9774 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/social_work_workforce/sample_data.py
--rw-r--r--   0        0        0      470 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/datasets/social_work_workforce/schema.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/spec/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/spec/annex_a/__init__.py
--rw-r--r--   0        0        0    11870 2023-04-14 07:55:59.249829 liiatools-0.1.5.0/liiatools/spec/annex_a/annex-a-merge.yml
--rw-r--r--   0        0        0    45318 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/annex_a/data-map.yml
--rw-r--r--   0        0        0    10542 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/annex_a/la-agg.yml
--rw-r--r--   0        0        0     1757 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/annex_a/pan-agg.yml
--rw-r--r--   0        0        0    27319 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/annex_a/samples/Annex_A.xlsx
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/cin_census/__init__.py
--rw-r--r--   0        0        0      711 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/cin_census/agg.yml
--rw-r--r--   0        0        0    31534 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/cin_census/cin-2022.xsd
--rw-r--r--   0        0        0     3423 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/cin_census/samples/cin-2022.xml
--rw-r--r--   0        0        0      739 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/common/LA-codes.yml
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/common/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/s903/__init__.py
--rw-r--r--   0        0        0    10833 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/s903/config.yml
--rw-r--r--   0        0        0     3339 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/s903/la-agg.yml
--rw-r--r--   0        0        0     1792 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/s903/pan-agg.yml
--rw-r--r--   0        0        0      459 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/s903/samples/SSDA903_2020_episodes.csv
--rw-r--r--   0        0        0     1585 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/s903/sufficiency.yml
--rw-r--r--   0        0        0        1 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/school_census/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/social_work_workforce/__init__.py
--rw-r--r--   0        0        0     3716 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/social_work_workforce/samples/social_work_workforce_2022.xml
--rw-r--r--   0        0        0    17431 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/liiatools/spec/social_work_workforce/social_work_workforce_2022.xsd
--rw-r--r--   0        0        0     1049 2023-04-14 07:55:59.253829 liiatools-0.1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 liiatools-0.1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/__init__.py
+-rw-r--r--   0        0        0      434 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/csdatatools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/csdatatools/datasets/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/csdatatools/datasets/cincensus/__init__.py
+-rw-r--r--   0        0        0     4364 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/csdatatools/datasets/cincensus/filters.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/csdatatools/util/__init__.py
+-rw-r--r--   0        0        0      280 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/csdatatools/util/stream.py
+-rw-r--r--   0        0        0     1640 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/csdatatools/util/xml.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/__init__.py
+-rw-r--r--   0        0        0      131 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/__init__.py
+-rw-r--r--   0        0        0     7047 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/annex_a_cli.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/__init__.py
+-rw-r--r--   0        0        0     4908 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/cleaner.py
+-rw-r--r--   0        0        0    11751 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/configuration.py
+-rw-r--r--   0        0        0      451 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/converters.py
+-rw-r--r--   0        0        0     1381 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/degrade.py
+-rw-r--r--   0        0        0     5122 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/file_creator.py
+-rw-r--r--   0        0        0    12608 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/logger.py
+-rw-r--r--   0        0        0      772 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/populate.py
+-rw-r--r--   0        0        0      885 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/regex.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_la_agg/__init__.py
+-rw-r--r--   0        0        0     2495 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_la_agg/configuration.py
+-rw-r--r--   0        0        0     3052 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_la_agg/process.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_pan_agg/__init__.py
+-rw-r--r--   0        0        0     2894 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_pan_agg/configuration.py
+-rw-r--r--   0        0        0     2066 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_pan_agg/process.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/__init__.py
+-rw-r--r--   0        0        0    11514 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/cin_cli.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/__init__.py
+-rw-r--r--   0        0        0     6065 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/cin_record.py
+-rw-r--r--   0        0        0     2644 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/configuration.py
+-rw-r--r--   0        0        0      811 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/converter.py
+-rw-r--r--   0        0        0     2906 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/file_creator.py
+-rw-r--r--   0        0        0     6012 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/logger.py
+-rw-r--r--   0        0        0      410 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/schema.py
+-rw-r--r--   0        0        0     3860 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/validator.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_la_agg/__init__.py
+-rw-r--r--   0        0        0     2487 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_la_agg/configuration.py
+-rw-r--r--   0        0        0    10532 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_la_agg/process.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_pan_agg/__init__.py
+-rw-r--r--   0        0        0     2885 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_pan_agg/configuration.py
+-rw-r--r--   0        0        0    10132 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_pan_agg/process.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/__init__.py
+-rw-r--r--   0        0        0     1547 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/columns.py
+-rw-r--r--   0        0        0     5105 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/configuration.py
+-rw-r--r--   0        0        0     1612 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/converters.py
+-rw-r--r--   0        0        0     1248 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/degrade.py
+-rw-r--r--   0        0        0     2993 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/file_creator.py
+-rw-r--r--   0        0        0     3184 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/filters.py
+-rw-r--r--   0        0        0     8547 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/logger.py
+-rw-r--r--   0        0        0     1189 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/parse.py
+-rw-r--r--   0        0        0     2000 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/populate.py
+-rw-r--r--   0        0        0     5080 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/prep.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_la_agg/__init__.py
+-rw-r--r--   0        0        0     2486 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_la_agg/configuration.py
+-rw-r--r--   0        0        0     2425 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_la_agg/process.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_pan_agg/__init__.py
+-rw-r--r--   0        0        0     2885 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_pan_agg/configuration.py
+-rw-r--r--   0        0        0     1482 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_pan_agg/process.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_sufficiency/__init__.py
+-rw-r--r--   0        0        0     2491 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_sufficiency/configuration.py
+-rw-r--r--   0        0        0     1078 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_sufficiency/process.py
+-rw-r--r--   0        0        0     4704 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/s903_cli.py
+-rw-r--r--   0        0        0     6921 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/s903_main_functions.py
+-rw-r--r--   0        0        0        1 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/school_census/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/school_census/lds_school_clean/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/school_census/lds_school_la_agg/__init__.py
+-rw-r--r--   0        0        0     6324 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/shared_functions/common.py
+-rw-r--r--   0        0        0     1827 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/shared_functions/converters.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/__init__.py
+-rw-r--r--   0        0        0      778 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/FTESum.py
+-rw-r--r--   0        0        0      778 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/FTESum_2020.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/__init__.py
+-rw-r--r--   0        0        0     2452 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/growth_tables.py
+-rw-r--r--   0        0        0      851 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/pivotGen.py
+-rw-r--r--   0        0        0      745 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/progressed.py
+-rw-r--r--   0        0        0     2508 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority.py
+-rw-r--r--   0        0        0     2842 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority_forecast_04.py
+-rw-r--r--   0        0        0     3204 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority_forecast_5c.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/__init__.py
+-rw-r--r--   0        0        0     5395 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/converter.py
+-rw-r--r--   0        0        0     7134 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/file_operations.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/__init__.py
+-rw-r--r--   0        0        0      980 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validation_error.py
+-rw-r--r--   0        0        0     7796 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validator.py
+-rw-r--r--   0        0        0       24 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/env
+-rw-r--r--   0        0        0     1628 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/spec/__init__.py
+-rw-r--r--   0        0        0    23265 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/spec/wf_xmlschema.xsd
+-rw-r--r--   0        0        0     4771 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/util/AppLogs.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/util/__init__.py
+-rw-r--r--   0        0        0     2268 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/util/work_path.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/__init__.py
+-rw-r--r--   0        0        0      829 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/csww_cli.py
+-rw-r--r--   0        0        0      839 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/csww_main_functions.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/lds_csww_clean/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/lds_csww_la_agg/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/lds_csww_pan_agg/__init__.py
+-rw-r--r--   0        0        0     9774 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/sample_data.py
+-rw-r--r--   0        0        0      470 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/schema.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/annex_a/__init__.py
+-rw-r--r--   0        0        0    11870 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/annex_a/annex-a-merge.yml
+-rw-r--r--   0        0        0    45318 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/annex_a/data-map.yml
+-rw-r--r--   0        0        0    10542 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/annex_a/la-agg.yml
+-rw-r--r--   0        0        0     1757 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/annex_a/pan-agg.yml
+-rw-r--r--   0        0        0    27319 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/annex_a/samples/Annex_A.xlsx
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/cin_census/__init__.py
+-rw-r--r--   0        0        0      711 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/cin_census/agg.yml
+-rw-r--r--   0        0        0    31534 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/cin_census/cin-2022.xsd
+-rw-r--r--   0        0        0     3423 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/cin_census/samples/cin-2022.xml
+-rw-r--r--   0        0        0      739 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/common/LA-codes.yml
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/s903/__init__.py
+-rw-r--r--   0        0        0    10875 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/s903/config.yml
+-rw-r--r--   0        0        0     3339 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/s903/la-agg.yml
+-rw-r--r--   0        0        0     1792 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/s903/pan-agg.yml
+-rw-r--r--   0        0        0      459 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/s903/samples/SSDA903_2020_episodes.csv
+-rw-r--r--   0        0        0     1585 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/s903/sufficiency.yml
+-rw-r--r--   0        0        0        1 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/school_census/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/social_work_workforce/__init__.py
+-rw-r--r--   0        0        0     3716 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/social_work_workforce/samples/social_work_workforce_2022.xml
+-rw-r--r--   0        0        0    17431 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/social_work_workforce/social_work_workforce_2022.xsd
+-rw-r--r--   0        0        0     1049 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 liiatools-0.1.5.1/PKG-INFO
```

### Comparing `liiatools-0.1.5.0/LICENSE` & `liiatools-0.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/csdatatools/datasets/cincensus/filters.py` & `liiatools-0.1.5.1/liiatools/csdatatools/datasets/cincensus/filters.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/csdatatools/util/xml.py` & `liiatools-0.1.5.1/liiatools/csdatatools/util/xml.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/annex_a/annex_a_cli.py` & `liiatools-0.1.5.1/liiatools/datasets/annex_a/annex_a_cli.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/cleaner.py` & `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/cleaner.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/configuration.py` & `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/degrade.py` & `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/degrade.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/file_creator.py` & `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/file_creator.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/logger.py` & `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/logger.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/populate.py` & `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/populate.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_clean/regex.py` & `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/regex.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_la_agg/configuration.py` & `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_la_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_la_agg/process.py` & `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_la_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_pan_agg/configuration.py` & `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_pan_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/annex_a/lds_annexa_pan_agg/process.py` & `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_pan_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/cin_census/cin_cli.py` & `liiatools-0.1.5.1/liiatools/datasets/cin_census/cin_cli.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_clean/cin_record.py` & `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/cin_record.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_clean/configuration.py` & `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_clean/converter.py` & `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/converter.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_clean/file_creator.py` & `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/file_creator.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_clean/logger.py` & `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/logger.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_clean/validator.py` & `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/validator.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_la_agg/configuration.py` & `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_la_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_la_agg/process.py` & `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_la_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_pan_agg/configuration.py` & `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_pan_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/cin_census/lds_cin_pan_agg/process.py` & `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_pan_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/columns.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/columns.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/configuration.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/converters.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/converters.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/degrade.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/degrade.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/file_creator.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/file_creator.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/filters.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/filters.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/logger.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/logger.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/parse.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/parse.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/populate.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/populate.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_clean/prep.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/prep.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_la_agg/configuration.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_la_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_la_agg/process.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_la_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_pan_agg/configuration.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_pan_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_pan_agg/process.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_pan_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_sufficiency/configuration.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_sufficiency/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/lds_ssda903_sufficiency/process.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_sufficiency/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/s903_cli.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/s903_cli.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/s903/s903_main_functions.py` & `liiatools-0.1.5.1/liiatools/datasets/s903/s903_main_functions.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/shared_functions/common.py` & `liiatools-0.1.5.1/liiatools/datasets/shared_functions/common.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/shared_functions/converters.py` & `liiatools-0.1.5.1/liiatools/datasets/shared_functions/converters.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/social_work_workforce/csww_cli.py` & `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/csww_cli.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/social_work_workforce/csww_main_functions.py` & `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/csww_main_functions.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/datasets/social_work_workforce/sample_data.py` & `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/sample_data.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/spec/annex_a/annex-a-merge.yml` & `liiatools-0.1.5.1/liiatools/spec/annex_a/annex-a-merge.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/spec/annex_a/data-map.yml` & `liiatools-0.1.5.1/liiatools/spec/annex_a/data-map.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/spec/annex_a/la-agg.yml` & `liiatools-0.1.5.1/liiatools/spec/annex_a/la-agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/spec/annex_a/pan-agg.yml` & `liiatools-0.1.5.1/liiatools/spec/annex_a/pan-agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/spec/annex_a/samples/Annex_A.xlsx` & `liiatools-0.1.5.1/liiatools/spec/annex_a/samples/Annex_A.xlsx`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/spec/cin_census/agg.yml` & `liiatools-0.1.5.1/liiatools/spec/cin_census/agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/spec/cin_census/cin-2022.xsd` & `liiatools-0.1.5.1/liiatools/spec/cin_census/cin-2022.xsd`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/spec/cin_census/samples/cin-2022.xml` & `liiatools-0.1.5.1/liiatools/spec/cin_census/samples/cin-2022.xml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/spec/common/LA-codes.yml` & `liiatools-0.1.5.1/liiatools/spec/common/LA-codes.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/spec/s903/config.yml` & `liiatools-0.1.5.1/liiatools/spec/s903/config.yml`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,16 @@
        - code: "E12"
        - code: "E2"
        - code: "E3"
        - code: "E4A"
        - code: "E4B"
        - code: "E13"
        - code: "E41"
+       - code: "E43"
+       - code: "E44"
        - code: "E45"
        - code: "E46"
        - code: "E47"
        - code: "E48"
        - code: "E5"
        - code: "E6"
        - code: "E7"
```

### Comparing `liiatools-0.1.5.0/liiatools/spec/s903/la-agg.yml` & `liiatools-0.1.5.1/liiatools/spec/s903/la-agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/spec/s903/pan-agg.yml` & `liiatools-0.1.5.1/liiatools/spec/s903/pan-agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/spec/s903/sufficiency.yml` & `liiatools-0.1.5.1/liiatools/spec/s903/sufficiency.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/spec/social_work_workforce/samples/social_work_workforce_2022.xml` & `liiatools-0.1.5.1/liiatools/spec/social_work_workforce/samples/social_work_workforce_2022.xml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/liiatools/spec/social_work_workforce/social_work_workforce_2022.xsd` & `liiatools-0.1.5.1/liiatools/spec/social_work_workforce/social_work_workforce_2022.xsd`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.0/pyproject.toml` & `liiatools-0.1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liiatools"
-version = "0.1.5.0"
+version = "0.1.5.1"
 description = "Children's Services Data Tools - Utilities for cleaning and normalising CS data by Social Finance"
 authors = [
     "Michael Hanks <michael.hanks@socialfinance.org.uk>",
     "Patrick Troy <patrick.troy@socialfinance.org.uk>",
     "Céline Gross <celine.m.gross@gmail.com>",
     "Kaj Siebert <kaj@k-si.com>",
     "Matthew Pugh <matthew.pugh@socialfinance.org.uk>"
```

### Comparing `liiatools-0.1.5.0/PKG-INFO` & `liiatools-0.1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liiatools
-Version: 0.1.5.0
+Version: 0.1.5.1
 Summary: Children's Services Data Tools - Utilities for cleaning and normalising CS data by Social Finance
 License: MIT
 Author: Michael Hanks
 Author-email: michael.hanks@socialfinance.org.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

