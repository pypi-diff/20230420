# Comparing `tmp/d_geolib-0.5.1.tar.gz` & `tmp/d_geolib-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d_geolib-0.5.1.tar", max compression
+gzip compressed data, was "d_geolib-0.6.0.tar", max compression
```

## Comparing `d_geolib-0.5.1.tar` & `d_geolib-0.6.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0       97 2023-04-04 08:31:43.174813 d_geolib-0.5.1/geolib/__init__.py
--rw-r--r--   0        0        0      629 2023-04-03 17:11:48.352689 d_geolib-0.5.1/geolib/errors.py
--rw-r--r--   0        0        0       86 2023-04-03 17:11:48.352689 d_geolib-0.5.1/geolib/geometry/__init__.py
--rw-r--r--   0        0        0     1018 2023-04-03 17:11:48.352689 d_geolib-0.5.1/geolib/geometry/one.py
--rw-r--r--   0        0        0      510 2023-04-03 17:11:48.352689 d_geolib-0.5.1/geolib/models/__init__.py
--rw-r--r--   0        0        0    11494 2023-04-03 17:11:48.352689 d_geolib-0.5.1/geolib/models/base_model.py
--rw-r--r--   0        0        0      749 2023-04-03 17:11:48.352689 d_geolib-0.5.1/geolib/models/base_model_structure.py
--rw-r--r--   0        0        0      109 2023-04-03 17:11:48.352689 d_geolib-0.5.1/geolib/models/dfoundations/__init__.py
--rw-r--r--   0        0        0    12353 2023-04-03 17:11:48.352689 d_geolib-0.5.1/geolib/models/dfoundations/dfoundations_model.py
--rw-r--r--   0        0        0     1621 2023-04-03 17:11:48.352689 d_geolib-0.5.1/geolib/models/dfoundations/dfoundations_parserprovider.py
--rw-r--r--   0        0        0     3195 2023-04-03 17:11:48.352689 d_geolib-0.5.1/geolib/models/dfoundations/dfoundations_structures.py
--rw-r--r--   0        0        0    29122 2023-04-03 17:11:48.352689 d_geolib-0.5.1/geolib/models/dfoundations/internal.py
--rw-r--r--   0        0        0     3141 2023-04-03 17:11:48.352689 d_geolib-0.5.1/geolib/models/dfoundations/internal_soil.py
--rw-r--r--   0        0        0    19272 2023-04-03 17:11:48.352689 d_geolib-0.5.1/geolib/models/dfoundations/piles.py
--rw-r--r--   0        0        0     3954 2023-04-03 17:11:48.352689 d_geolib-0.5.1/geolib/models/dfoundations/profiles.py
--rw-r--r--   0        0        0      603 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dfoundations/serializer.py
--rw-r--r--   0        0        0     4350 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv
--rw-r--r--   0        0        0     4337 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv
--rw-r--r--   0        0        0    27893 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dfoundations/templates/input.foi.j2
--rw-r--r--   0        0        0      114 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dgeoflow/__init__.py
--rw-r--r--   0        0        0    16856 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dgeoflow/dgeoflow_model.py
--rw-r--r--   0        0        0     4281 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dgeoflow/dgeoflow_parserprovider.py
--rw-r--r--   0        0        0      333 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dgeoflow/dgeoflow_validator.py
--rw-r--r--   0        0        0    31789 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dgeoflow/internal.py
--rw-r--r--   0        0        0     3517 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dgeoflow/serializer.py
--rw-r--r--   0        0        0      581 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dgeoflow/utils.py
--rw-r--r--   0        0        0    53125 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dseries_parser.py
--rw-r--r--   0        0        0      106 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dsettlement/__init__.py
--rw-r--r--   0        0        0      301 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dsettlement/drain_types.py
--rw-r--r--   0        0        0     5529 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dsettlement/drains.py
--rw-r--r--   0        0        0    21412 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dsettlement/dsettlement_model.py
--rw-r--r--   0        0        0     1520 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dsettlement/dsettlement_parserprovider.py
--rw-r--r--   0        0        0     7149 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dsettlement/dsettlement_structures.py
--rw-r--r--   0        0        0    34039 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dsettlement/internal.py
--rw-r--r--   0        0        0     5500 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dsettlement/internal_soil.py
--rw-r--r--   0        0        0     5962 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dsettlement/loads.py
--rw-r--r--   0        0        0      233 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dsettlement/probabilistic_calculation_types.py
--rw-r--r--   0        0        0      559 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dsettlement/serializer.py
--rw-r--r--   0        0        0    18393 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dsettlement/templates/input.sli.j2
--rw-r--r--   0        0        0     4965 2023-04-03 17:11:48.368309 d_geolib-0.5.1/geolib/models/dsettlement/templates/soil_template.j2
--rw-r--r--   0        0        0      110 2023-04-03 17:11:48.383935 d_geolib-0.5.1/geolib/models/dsheetpiling/__init__.py
--rw-r--r--   0        0        0    11029 2023-04-03 17:11:48.383935 d_geolib-0.5.1/geolib/models/dsheetpiling/calculation_options.py
--rw-r--r--   0        0        0    21824 2023-04-03 17:11:48.383935 d_geolib-0.5.1/geolib/models/dsheetpiling/constructions.py
--rw-r--r--   0        0        0    19429 2023-04-03 17:11:48.383935 d_geolib-0.5.1/geolib/models/dsheetpiling/dsheetpiling_model.py
--rw-r--r--   0        0        0     1530 2023-04-03 17:11:48.383935 d_geolib-0.5.1/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py
--rw-r--r--   0        0        0     4775 2023-04-03 17:11:48.383935 d_geolib-0.5.1/geolib/models/dsheetpiling/dsheetpiling_structures.py
--rw-r--r--   0        0        0     3841 2023-04-03 17:11:48.383935 d_geolib-0.5.1/geolib/models/dsheetpiling/dsheetpiling_validator.py
--rw-r--r--   0        0        0    54530 2023-04-03 17:11:48.383935 d_geolib-0.5.1/geolib/models/dsheetpiling/internal.py
--rw-r--r--   0        0        0    25934 2023-04-03 17:11:48.383935 d_geolib-0.5.1/geolib/models/dsheetpiling/internal_partial_factors.py
--rw-r--r--   0        0        0     9894 2023-04-03 17:11:48.383935 d_geolib-0.5.1/geolib/models/dsheetpiling/loads.py
--rw-r--r--   0        0        0     1726 2023-04-03 17:11:48.383935 d_geolib-0.5.1/geolib/models/dsheetpiling/profiles.py
--rw-r--r--   0        0        0      561 2023-04-03 17:11:48.383935 d_geolib-0.5.1/geolib/models/dsheetpiling/serializer.py
--rw-r--r--   0        0        0     5035 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dsheetpiling/settings.py
--rw-r--r--   0        0        0     3467 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dsheetpiling/supports.py
--rw-r--r--   0        0        0     1702 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dsheetpiling/surface.py
--rw-r--r--   0        0        0    43328 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dsheetpiling/templates/input.shi.j2
--rw-r--r--   0        0        0      462 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dsheetpiling/water_level.py
--rw-r--r--   0        0        0      118 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dstability/__init__.py
--rw-r--r--   0        0        0    12238 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dstability/analysis.py
--rw-r--r--   0        0        0    27144 2023-04-04 08:31:43.174813 d_geolib-0.5.1/geolib/models/dstability/dstability_model.py
--rw-r--r--   0        0        0     4195 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dstability/dstability_parserprovider.py
--rw-r--r--   0        0        0     2199 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dstability/dstability_validator.py
--rw-r--r--   0        0        0    79894 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dstability/internal.py
--rw-r--r--   0        0        0     2528 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dstability/loads.py
--rw-r--r--   0        0        0     3435 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dstability/reinforcements.py
--rw-r--r--   0        0        0     3529 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dstability/serializer.py
--rw-r--r--   0        0        0     3331 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dstability/states.py
--rw-r--r--   0        0        0      581 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/dstability/utils.py
--rw-r--r--   0        0        0      142 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/internal.py
--rw-r--r--   0        0        0     1781 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/meta.py
--rw-r--r--   0        0        0       89 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/model_enums.py
--rw-r--r--   0        0        0     1821 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/parsers.py
--rw-r--r--   0        0        0      840 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/serializers.py
--rw-r--r--   0        0        0     2433 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/utils.py
--rw-r--r--   0        0        0      314 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/models/validators.py
--rw-r--r--   0        0        0       55 2023-04-03 17:11:48.415187 d_geolib-0.5.1/geolib/service/__init__.py
--rw-r--r--   0        0        0     5659 2023-04-03 17:11:48.415187 d_geolib-0.5.1/geolib/service/main.py
--rw-r--r--   0        0        0      546 2023-04-03 17:11:48.399562 d_geolib-0.5.1/geolib/service/README.md
--rw-r--r--   0        0        0      797 2023-04-03 17:11:48.415187 d_geolib-0.5.1/geolib/soils/__init__.py
--rw-r--r--   0        0        0     1720 2023-04-03 17:11:48.415187 d_geolib-0.5.1/geolib/soils/layers.py
--rw-r--r--   0        0        0      592 2023-04-03 17:11:48.415187 d_geolib-0.5.1/geolib/soils/library.py
--rw-r--r--   0        0        0    37105 2023-04-03 17:11:48.415187 d_geolib-0.5.1/geolib/soils/soil.py
--rw-r--r--   0        0        0      775 2023-04-03 17:11:48.415187 d_geolib-0.5.1/geolib/soils/soil_utils.py
--rw-r--r--   0        0        0     1574 2023-04-03 17:11:48.415187 d_geolib-0.5.1/geolib/utils.py
--rw-r--r--   0        0        0     1086 2023-04-03 17:11:48.321437 d_geolib-0.5.1/LICENSE
--rw-r--r--   0        0        0     1982 2023-04-04 08:31:43.174813 d_geolib-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2955 2023-04-03 17:11:48.321437 d_geolib-0.5.1/README.rst
--rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 d_geolib-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/__init__.py
+-rw-r--r--   0        0        0      629 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/errors.py
+-rw-r--r--   0        0        0       86 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/geometry/__init__.py
+-rw-r--r--   0        0        0     1018 2023-04-17 12:25:37.521419 d_geolib-0.6.0/geolib/geometry/one.py
+-rw-r--r--   0        0        0      510 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/models/__init__.py
+-rw-r--r--   0        0        0    11538 2023-04-17 12:25:37.521419 d_geolib-0.6.0/geolib/models/base_model.py
+-rw-r--r--   0        0        0      749 2023-04-17 12:25:37.521419 d_geolib-0.6.0/geolib/models/base_model_structure.py
+-rw-r--r--   0        0        0      109 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/models/dfoundations/__init__.py
+-rw-r--r--   0        0        0    12327 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/models/dfoundations/dfoundations_model.py
+-rw-r--r--   0        0        0     1621 2023-04-17 12:25:37.521419 d_geolib-0.6.0/geolib/models/dfoundations/dfoundations_parserprovider.py
+-rw-r--r--   0        0        0     3532 2023-04-17 12:25:37.521419 d_geolib-0.6.0/geolib/models/dfoundations/dfoundations_structures.py
+-rw-r--r--   0        0        0    27774 2023-04-17 12:25:37.521419 d_geolib-0.6.0/geolib/models/dfoundations/internal.py
+-rw-r--r--   0        0        0     3020 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/models/dfoundations/internal_soil.py
+-rw-r--r--   0        0        0    19272 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dfoundations/piles.py
+-rw-r--r--   0        0        0     3958 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dfoundations/profiles.py
+-rw-r--r--   0        0        0      603 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dfoundations/serializer.py
+-rw-r--r--   0        0        0     4350 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv
+-rw-r--r--   0        0        0     4337 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv
+-rw-r--r--   0        0        0    27924 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dfoundations/templates/input.foi.j2
+-rw-r--r--   0        0        0      114 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/models/dgeoflow/__init__.py
+-rw-r--r--   0        0        0    16856 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/models/dgeoflow/dgeoflow_model.py
+-rw-r--r--   0        0        0     4281 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dgeoflow/dgeoflow_parserprovider.py
+-rw-r--r--   0        0        0      333 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dgeoflow/dgeoflow_validator.py
+-rw-r--r--   0        0        0    31789 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dgeoflow/internal.py
+-rw-r--r--   0        0        0     3517 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dgeoflow/serializer.py
+-rw-r--r--   0        0        0      581 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dgeoflow/utils.py
+-rw-r--r--   0        0        0    54613 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dseries_parser.py
+-rw-r--r--   0        0        0      106 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsettlement/__init__.py
+-rw-r--r--   0        0        0      301 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/drain_types.py
+-rw-r--r--   0        0        0     5529 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/drains.py
+-rw-r--r--   0        0        0    21412 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsettlement/dsettlement_model.py
+-rw-r--r--   0        0        0     1520 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/dsettlement_parserprovider.py
+-rw-r--r--   0        0        0     7149 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/dsettlement_structures.py
+-rw-r--r--   0        0        0    34039 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/internal.py
+-rw-r--r--   0        0        0     5500 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/internal_soil.py
+-rw-r--r--   0        0        0     5962 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/loads.py
+-rw-r--r--   0        0        0      233 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/probabilistic_calculation_types.py
+-rw-r--r--   0        0        0      559 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/serializer.py
+-rw-r--r--   0        0        0    18393 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/templates/input.sli.j2
+-rw-r--r--   0        0        0     4965 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/templates/soil_template.j2
+-rw-r--r--   0        0        0      110 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsheetpiling/__init__.py
+-rw-r--r--   0        0        0    11248 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsheetpiling/calculation_options.py
+-rw-r--r--   0        0        0    21608 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsheetpiling/constructions.py
+-rw-r--r--   0        0        0    19439 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_model.py
+-rw-r--r--   0        0        0     1530 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py
+-rw-r--r--   0        0        0     4647 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_structures.py
+-rw-r--r--   0        0        0     3841 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_validator.py
+-rw-r--r--   0        0        0    53551 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/internal.py
+-rw-r--r--   0        0        0    15561 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/internal_partial_factors.py
+-rw-r--r--   0        0        0     9894 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsheetpiling/loads.py
+-rw-r--r--   0        0        0     1726 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/profiles.py
+-rw-r--r--   0        0        0      561 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/serializer.py
+-rw-r--r--   0        0        0     5060 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsheetpiling/settings.py
+-rw-r--r--   0        0        0     3467 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/supports.py
+-rw-r--r--   0        0        0     1702 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/surface.py
+-rw-r--r--   0        0        0    35235 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsheetpiling/templates/input.shi.j2
+-rw-r--r--   0        0        0      462 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/water_level.py
+-rw-r--r--   0        0        0      118 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dstability/__init__.py
+-rw-r--r--   0        0        0    12238 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dstability/analysis.py
+-rw-r--r--   0        0        0    27144 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dstability/dstability_model.py
+-rw-r--r--   0        0        0     4195 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dstability/dstability_parserprovider.py
+-rw-r--r--   0        0        0     2199 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dstability/dstability_validator.py
+-rw-r--r--   0        0        0    79894 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dstability/internal.py
+-rw-r--r--   0        0        0     2528 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dstability/loads.py
+-rw-r--r--   0        0        0     3435 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dstability/reinforcements.py
+-rw-r--r--   0        0        0     3529 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dstability/serializer.py
+-rw-r--r--   0        0        0     3331 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dstability/states.py
+-rw-r--r--   0        0        0      581 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dstability/utils.py
+-rw-r--r--   0        0        0      142 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/internal.py
+-rw-r--r--   0        0        0     1781 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/meta.py
+-rw-r--r--   0        0        0       89 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/model_enums.py
+-rw-r--r--   0        0        0     1821 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/parsers.py
+-rw-r--r--   0        0        0      840 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/serializers.py
+-rw-r--r--   0        0        0     2433 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/utils.py
+-rw-r--r--   0        0        0      314 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/validators.py
+-rw-r--r--   0        0        0       55 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/service/__init__.py
+-rw-r--r--   0        0        0     5659 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/service/main.py
+-rw-r--r--   0        0        0      546 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/service/README.md
+-rw-r--r--   0        0        0      797 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/soils/__init__.py
+-rw-r--r--   0        0        0     1720 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/soils/layers.py
+-rw-r--r--   0        0        0      592 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/soils/library.py
+-rw-r--r--   0        0        0    37210 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/soils/soil.py
+-rw-r--r--   0        0        0      775 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/soils/soil_utils.py
+-rw-r--r--   0        0        0     1574 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/utils.py
+-rw-r--r--   0        0        0     1086 2023-04-17 12:25:37.505796 d_geolib-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1982 2023-04-20 08:35:02.126648 d_geolib-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2955 2023-04-20 08:35:02.111023 d_geolib-0.6.0/README.rst
+-rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 d_geolib-0.6.0/PKG-INFO
```

### Comparing `d_geolib-0.5.1/geolib/errors.py` & `d_geolib-0.6.0/geolib/errors.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/geometry/one.py` & `d_geolib-0.6.0/geolib/geometry/one.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/base_model.py` & `d_geolib-0.6.0/geolib/models/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,34 +58,34 @@
             + [str(self.filename.resolve())]
             + self.console_flags_post,
             timeout=timeout_in_seconds,
             cwd=str(self.filename.resolve().parent),
         )
         logger.debug(f"Executed with {process.args}")
 
-        # Successfull run
+        # Successful run
         output_filename = output_filename_from_input(self)
         logger.info(
             f"Checking for {output_filename}, while process exited with {process.returncode}"
         )
         if output_filename.exists():
             try:
                 self.parse(output_filename)
                 return self  # TODO Figure out whether we should instantiate a new model (parse is a classmethod)
             except ValidationError:
                 logger.warning(
-                    f"Ouput file generated but parsing of {output_filename} failed."
+                    f"Output file generated but parsing of {output_filename} failed."
                 )
                 error = self.get_error_context()
                 raise CalculationError(process.returncode, error)
 
         # Unsuccessful run
         else:
             error = self.get_error_context()
-            raise CalculationError(process.returncode, error)
+            raise CalculationError(process.returncode, error + " Path: " + str(output_filename.absolute))
 
     def execute_remote(self, endpoint: HttpUrl) -> "BaseModel":
         """Execute a Model on a remote endpoint.
 
         A new model instance is returned.
         """
         response = requests.post(
```

### Comparing `d_geolib-0.5.1/geolib/models/base_model_structure.py` & `d_geolib-0.6.0/geolib/models/base_model_structure.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dfoundations/dfoundations_model.py` & `d_geolib-0.6.0/geolib/models/dfoundations/dfoundations_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from enum import Enum
 from pathlib import Path
 from subprocess import CompletedProcess, run
 from typing import BinaryIO, List, Optional, Type, Union
 
-from pydantic import FilePath, confloat
+from pydantic import FilePath, confloat, conint
 
 from geolib.geometry import Point
 from geolib.models import BaseDataClass, BaseModel, BaseModelStructure
 from geolib.models.internal import Bool
 from geolib.models.meta import CONSOLE_RUN_BATCH_FLAG
 from geolib.soils import Soil
 
@@ -44,17 +44,17 @@
 
 class ModelOptions(BaseDataClass):
     # Rigidity of superstructure
     is_rigid: Bool = True
 
     # Transformation
     max_allowed_settlement_lim_state_str: confloat(ge=0, le=100000) = 0
-    max_allowed_rel_rotation_lim_state_str: confloat(ge=0.0001, le=10000) = 0.0001
+    max_allowed_rel_rotation_lim_state_str: conint(ge=1, le=10000) = 100
     max_allowed_settlement_lim_state_serv: confloat(ge=0, le=100000) = 0
-    max_allowed_rel_rotation_lim_state_serv: confloat(ge=0.0001, le=10000) = 0.0001
+    max_allowed_rel_rotation_lim_state_serv: conint(ge=1, le=10000) = 300
 
     # Factors
     factor_xi3: Optional[confloat(ge=0.01, le=10)] = None
     factor_xi4: Optional[confloat(ge=0.01, le=10)] = None
     ea_gem: Optional[confloat(ge=1)] = None
 
     # Combined Model Options
@@ -147,15 +147,15 @@
 
     @property
     def parser_provider_type(self) -> Type[DFoundationsParserProvider]:
         return DFoundationsParserProvider
 
     @property
     def console_path(self) -> Path:
-        return Path("DFoundationsConsole/DFoundationsConsole.exe")
+        return Path("DFoundations/DFoundations.exe")
 
     @property
     def console_flags(self) -> List[str]:
         return [CONSOLE_RUN_BATCH_FLAG]
 
     @property
     def output(self) -> DFoundationsDumpfileOutputStructure:
```

### Comparing `d_geolib-0.5.1/geolib/models/dfoundations/dfoundations_parserprovider.py` & `d_geolib-0.6.0/geolib/models/dfoundations/dfoundations_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dfoundations/dfoundations_structures.py` & `d_geolib-0.6.0/geolib/models/dfoundations/dfoundations_structures.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,45 +52,53 @@
         return expected_property, text
 
 
 class DFoundationsTableWrapper(DSeriesStructure):
     @classmethod
     def parse_text(cls, text):
         """Parses a Table wrapped in another group such as:
-        [TABLE GROUP]
+        [TABLE]
+        DataCount = x followed by
+        [END OF TABLE]  directly when x = 0 or, when x > 0, by
         [COLUMN INDICATION]
         A
         B
         [END OF COLUMN INDICATION]
-        [GROUP DATA]
+        [DATA]
         1 1
         2 2
-        [END OF GROUP DATA]
-        [END OF TABLE GROUP]
+        [END OF DATA]
+        [END OF TABLE]
 
         Args:
             text (str): Wrapped table group to parse.
 
         Returns:
             DSerieStructure: Parsed structure.
         """
 
         def split_line(text: str) -> List[str]:
             parts = re.split(" |\t", text.strip())
             return list(filter(lambda part: part != "", parts))
 
         table_text = list(DSerieParser.parse_list_group(text).values())[0]
         table_data = list(DSerieParser.parse_list_group(table_text).values())
-        # Expected two groups (column_indication and data)
-        keys = table_data[0].split("\n")
-        values_dict_list = [
+        if len(table_data) == 0:
+            values_dict_list = table_data;
+            collection_property_name = list(cls.__fields__.items())[0][0]
+            return cls(**{collection_property_name: values_dict_list})
+        else:
+            # Expected two groups (column_indication and data)
+            keys = table_data[0].split("\n")
+            values_dict_list = [
             dict(zip(keys, values))
             for values in map(split_line, table_data[1].split("\n"))
-        ]
-        collection_property_name = list(cls.__fields__.items())[0][0]
+            ]
+            collection_property_name = list(cls.__fields__.items())[0][0]
+
         return cls(**{collection_property_name: values_dict_list})
 
 
 class DFoundationsCPTCollectionWrapper(DSerieListGroupNextStructure):
     @classmethod
     def group_delimiter(cls) -> str:
         return "[NEXT OF NUMBER OF CPTS]"
```

### Comparing `d_geolib-0.5.1/geolib/models/dfoundations/internal.py` & `d_geolib-0.6.0/geolib/models/dfoundations/internal.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,16 @@
 class Layer(DSeriesTreeStructure):
     name: str = ""  # will be generated by template
     material: int
     top_level: float  # [m]
     excess_pore_pressure_top: float = 0.0  # [kN/m3]
     excess_pore_pressure_bottom: float = 0.0  # [kN/m3]
     ocr_value: float = 1.0  # [-]
-    reduction_core_resistance: int = 0  # [%]
+    reduction_core_resistance: float = 0.0  # [%]
+
 
 
 class ReductionCoreResistanceEnum(IntEnum):
     SAFE = 0
     BEGEMANN = 1
     MANUAL = 2
 
@@ -429,31 +430,37 @@
 class CalculationOptions(DSeriesNoParseSubStructure):
 
     # Rigidity of superstructure
     is_rigid: Bool = Bool.TRUE
 
     # Transformation
     max_allowed_settlement_lim_state_str: confloat(ge=0, le=100000) = 0
-    max_allowed_rel_rotation_lim_state_str: confloat(ge=0.0001, le=10000) = 0.0001
+    max_allowed_rel_rotation_lim_state_str: conint(ge=1, le=10000) = 100
     max_allowed_settlement_lim_state_serv: confloat(ge=0, le=100000) = 0
-    max_allowed_rel_rotation_lim_state_serv: confloat(ge=0.0001, le=10000) = 0.0001
+    max_allowed_rel_rotation_lim_state_serv: conint(ge=1, le=10000) = 300
 
     # Overrule parameters Bearing Piles
     is_xi3_overruled: Bool = Bool.FALSE
     factor_xi3: Optional[confloat(ge=0.01, le=10)] = 2
     is_xi4_overruled: Bool = Bool.FALSE
     factor_xi4: Optional[confloat(ge=0.01, le=10)] = 2
     is_gamma_b_overruled: Bool = Bool.FALSE
     factor_gamma_b: Optional[confloat(ge=1, le=100)] = 2
     is_gamma_s_overruled: Bool = Bool.FALSE
     factor_gamma_s: Optional[confloat(ge=1, le=100)] = 2
     is_gamma_fnk_overruled: Bool = Bool.FALSE
     factor_gamma_fnk: Optional[confloat(ge=-100, le=100)] = 2
     is_area_overruled: Bool = Bool.FALSE
     area: Optional[confloat(ge=0, le=100000)] = 1000
+    is_qbmax_overruled: Bool = Bool.FALSE
+    qbmax: Optional[confloat(ge=0, le=100)] = 15
+    is_qcza_low_overruled: Bool = Bool.FALSE
+    qcza_low: Optional[confloat(ge=0, le=100)] = 12
+    is_qcza_high_overruled: Bool = Bool.FALSE
+    qcza_high: Optional[confloat(ge=0, le=100)] = 15
     is_ea_gem_overruled: Bool = Bool.FALSE
     ea_gem: Optional[confloat(ge=1)] = 100000
 
     # Model options combined
     is_suppress_qc_reduction: Bool = Bool.FALSE
     is_overrule_excavation: Bool = Bool.FALSE
     use_pile_group: Bool = Bool.TRUE
@@ -489,31 +496,14 @@
     is_gamma_st_overruled: Bool = Bool.FALSE
     factor_gamma_st: Optional[confloat(ge=0.01, le=100)] = 1.0
     is_gamma_gamma_overruled: Bool = Bool.FALSE
     factor_gamma_gamma: Optional[confloat(ge=0.01, le=100)] = 1.0
     surcharge: confloat(ge=0, le=1e7) = 0
     use_piezometric_levels: Bool = Bool.TRUE
 
-    # Model options Bearing Piles BE
-    is_xi3_bpb_overruled: Bool = Bool.FALSE
-    factor_xi3_bpb: confloat(ge=0.01, le=10) = 1.0
-    is_xi4_bpb_overruled: Bool = Bool.FALSE
-    factor_xi4_bpb: confloat(ge=0.01, le=10) = 1.0
-    is_gamma_rd_overruled: Bool = Bool.FALSE
-    factor_gamma_rd: confloat(ge=1, le=100) = 1.0
-    is_gamma_b_bpb_overruled: Bool = Bool.FALSE
-    factor_gamma_b_bpb: confloat(ge=1, le=100) = 1.0
-    is_gamma_s_bpb_overruled: Bool = Bool.FALSE
-    factor_gamma_s_bpb: confloat(ge=1, le=100) = 1.0
-    suppress_all_qc_reduction_bp: Bool = Bool.FALSE
-    use_quality_assurance: Bool = Bool.FALSE
-    area_covered_per_cpt: confloat(ge=0) = 1000
-    is_beta_bpb_overruled: Bool = Bool.FALSE
-    factor_beat_bpb: confloat(ge=0.0, le=10) = 0
-
     def __init__(self, *args, **kwargs):
         """If defaults are overriden, update
         the related toggle fields as well.
         """
         toggles = {}
         for field, value in kwargs.items():
             if value is None:
@@ -532,15 +522,14 @@
         return "is_" + field.replace("factor_", "") + "_overruled"
 
 
 class ModelTypeEnum(IntEnum):
     BEARING_PILES = 0
     TENSION_PILES = 1
     SHALLOW_FOUNDATIONS = 2
-    BEARING_PILES_BELGIAN = 3
 
 
 class ModelType(DFoundationsInlineProperties):
     model: ModelTypeEnum = ModelTypeEnum.BEARING_PILES
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -591,44 +580,45 @@
     cpt_test_level: Optional[float] = 0.0  # [m]
 
     # Only valid for Prelimary Design
     net_bearing_capacity: Optional[int] = 0  # [kN]
 
 
 class Version(DSerieVersion):
-    soil: int = 1005
-    d__foundations: int = 1015
+    soil: int = 1010
+    d__foundations: int = 1024
 
 
 class VersionExternal(DSeriesInlineMappedProperties):
-    dgsfoundationcalc____dll: str = "19.1.2.26122"
+    dgsfoundationcalc____dll: str = "23.1.0.40358"
 
 
 class DFoundationsInputStructure(DSeriesStructure):
     """Representation of complete .foi file."""
 
     version: Version = Version()
     version_externals: VersionExternal = VersionExternal()
     model: ModelType = ModelType()
     soil_collection: SoilCollection = SoilCollection()
     run_identification: str = 6 * "\n"
     cpt_list: CPTList = CPTList()
     profiles: Profiles = Profiles()
-    slopes: str = cleandoc(
-        """
-            0 = number of items
+    user_classification_method: str = cleandoc(
+        """          
+        [USER CLASSIFICATION METHOD]
+        0
+        [END OF USER CLASSIFICATION METHOD]
         """
     )
-    types___bearing_piles: Union[List[TypesBearingPiles], str] = cleandoc(
+    slopes: str = cleandoc(
         """
-        -1 : pile type shown in main graph
             0 = number of items
         """
     )
-    types___bearing_piles_belgian: str = cleandoc(
+    types___bearing_piles: Union[List[TypesBearingPiles], str] = cleandoc(
         """
         -1 : pile type shown in main graph
             0 = number of items
         """
     )
     types___tension_piles_cur: Union[List[TypesTensionPiles], str] = cleandoc(
         """
@@ -643,70 +633,28 @@
     )
     loads: str = cleandoc(
         """
             0 = number of items
         """
     )
     positions___bearing_piles: Union[PositionsBearingPiles, str] = PositionsBearingPiles()
-    positions___bearing_piles_belgian: str = cleandoc(
-        """
-        [TABLE]
-        [COLUMN INDICATION]
-        index
-        X
-        Y
-        PileHeadLevel
-        Surcharge
-        LimitStateStrGeo
-        LimitStateService
-        PileName
-        [END OF COLUMN INDICATION]
-        [DATA]
-        [END OF DATA]
-        [END OF TABLE]
-        """
-    )
+
     positions___tension_piles_cur: Union[
         PositionsTensionPiles, str
     ] = PositionsTensionPiles()
     positions___shallow_foundations: str = cleandoc(
         """
         [TABLE]
-        [COLUMN INDICATION]
-        index
-        X
-        Y
-        Angle
-        FoundationType
-        Load
-        Profile
-        Slope
-        PileName
-        [END OF COLUMN INDICATION]
-        [DATA]
-        [END OF DATA]
+        DataCount=0
         [END OF TABLE]
         """
     )
     calculation_options: Union[CalculationOptions, str] = CalculationOptions()
     calculationtype: CalculationType = CalculationType()
     preliminary_design: Union[PreliminaryDesign, str] = PreliminaryDesign()
-    de_beer: str = cleandoc(
-        """
-          0.0357 : Cone diameter [m]
-            1.00 : Installation factor [-]
-           1.000 : Scale factor [-]
-           -4.00 : Trajectory begin [m]
-          -20.00 : Trajectory end [m]
-            1.00 : Trajectory interval [m]
-        0 : Number of Profiles selected for calculation
-            -1 : No pile type selected
-        0 : Lambda overruled = FALSE
-        """
-    )
     location_map: str = cleandoc(
         """
          0.0000
                 0.0000
                 0.0000
                 0.0000
         """
@@ -780,17 +728,17 @@
             int: Header line size.
         """
         return 3
 
 
 class DFoundationsGlobalNenResults(DFoundationsInlineProperties):
     wd1b: float
-    betad1b: float
     w2d: float
-    betad2: float
+    reciprocal_max_relative_rotation_calc_1B: float
+    reciprocal_max_relative_rotation_calc_2: float
 
 
 class DFoundationsVerificationResults(DSeriesStructure):
     global_nen_results: Optional[DFoundationsGlobalNenResults]
     demands_nen__en: Optional[str]
     nen_pile_results: Optional[DFoundationsNenPileResults]
 
@@ -814,34 +762,37 @@
     is_warning_sf_fund_length_given: Bool
     is_warning_sf_cud_given: Bool
     is_warning_sf_delta_phi_given: Bool
     is_warning_nen_spacing_given: int = int()
     is_warning_sf_slope_not_relevant_given: Bool
     is_warning_nen_sf_placement_depth_too_deep: Bool
     is_warning_nen_sf_placement_depth_too_shallow: Bool
+    is_warning_nen_bp_positive_skin_friction_zone_given: Bool
+    is_warning_sf_foundation_level_for_punch_to_deep_for_slope_given: Bool
 
 
 class DFoundationsDumpfileOutputStructure(DSeriesStructure):
     results_at_cpt_test_level: Optional[str]
     verification_results: Optional[DFoundationsVerificationResults]
 
     calculation_parameters_tension_piles: Optional[str]
     verification_results_tp: Optional[DFoundationsVerificationResults]
 
     footnote_warnings: Optional[str]
     preliminary_design_results: Optional[str]
     verification_results_sf: Optional[str]
     verification_results_tp_1b2: Optional[str]
     verification_design_results: Optional[str]
+    calculation_warnings: Optional[DFoundationsCalculationWarnings]
 
 
 class DFoundationsStructure(DSeriesStructure):
     input_data: DFoundationsInputStructure = DFoundationsInputStructure()
     dumpfile_output: Optional[DFoundationsDumpfileOutputStructure]
-    calculation_warnings: Optional[DFoundationsCalculationWarnings]
+
 
 
 class DFoundationsDumpStructure(DSeriesStructure):
     dumpfile: DFoundationsStructure = DFoundationsStructure()
 
 
 # endregion
```

### Comparing `d_geolib-0.5.1/geolib/models/dfoundations/internal_soil.py` & `d_geolib-0.6.0/geolib/models/dfoundations/internal_soil.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,34 +15,27 @@
 class SoilTypeNl(IntEnum):
     GRAVEL = 0
     SAND = 1
     LOAM = 2
     CLAY = 3
     PEAT = 4
     SANDYLOAM = 5
-
-
-class SoilTypeBe(IntEnum):
-    GRAVEL = 0
-    SAND = 1
-    LOAM = 2
-    CLAY = 3
-    PEAT = 4
+    TERTCLAY = 6
+    CLAYEYSAND = 7
 
 
 class MaxConeResistType(IntEnum):
     STANDARD = 0
     MANUAL = 1
 
 
 class Soil(DSeriesUnmappedNameProperties):
     name: constr(min_length=1, max_length=25)
     soilcolor: int = 10871211  # could be color
     soilsoiltype: SoilTypeNl = SoilTypeNl.SAND
-    soilbelgiansoiltype: SoilTypeBe = SoilTypeBe.SAND
     soilgamdry: confloat(ge=0.0, le=100) = 20.00
     soilgamwet: confloat(ge=0.0, le=100) = 20.00
     soilinitialvoidratio: confloat(ge=0.0, le=20.0) = 0.001001
     soildiameterd50: confloat(ge=0.0, le=1000.0) = 0.20000
     soilminvoidratio: confloat(ge=0.0, le=1.0) = 0.400
     soilmaxvoidratio: confloat(ge=0.0, le=1.0) = 0.800
     soilcohesion: confloat(ge=0.0, le=1000.0) = 30.00
```

### Comparing `d_geolib-0.5.1/geolib/models/dfoundations/piles.py` & `d_geolib-0.6.0/geolib/models/dfoundations/piles.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dfoundations/profiles.py` & `d_geolib-0.6.0/geolib/models/dfoundations/profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         [{
             "name": str,
             "material": str,
             "top_level": float  # [m]
             "excess_pore_pressure_top": float = 0.0  # [kN/m3]
             "excess_pore_pressure_bottom": float = 0.0  # [kN/m3]
             "ocr_value": float = 1.0  # [-]
-            "reduction_core_resistance": int = 0  # [%]
+            "reduction_core_resistance": float = 0.0  # [%]
         },]
 
     """
 
     name: str
     location: Point
     phreatic_level: float
```

### Comparing `d_geolib-0.5.1/geolib/models/dfoundations/serializer.py` & `d_geolib-0.6.0/geolib/models/dfoundations/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv` & `d_geolib-0.6.0/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv` & `d_geolib-0.6.0/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dfoundations/templates/input.foi.j2` & `d_geolib-0.6.0/geolib/models/dfoundations/templates/input.foi.j2`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 [SOIL COLLECTION]
     {{ soil_collection.soil|length }} = number of items
 {% for soil in soil_collection.soil %}
 [SOIL]
 {{ soil.name }}
 SoilColor={{ soil.soilcolor }}
 SoilSoilType={{ soil.soilsoiltype.value }}
-SoilBelgianSoilType={{ soil.soilbelgiansoiltype.value }}
 SoilGamDry={{ soil.soilgamdry }}
 SoilGamWet={{ soil.soilgamwet }}
 SoilInitialVoidRatio={{ soil.soilinitialvoidratio }}
 SoilDiameterD50={{ soil.soildiameterd50 }}
 SoilMinVoidRatio={{ soil.soilminvoidratio }}
 SoilMaxVoidRatio={{ soil.soilmaxvoidratio }}
 SoilCohesion={{ soil.soilcohesion }}
@@ -216,14 +215,16 @@
 {{ cpt.void_value_friction_number }}
 [END OF VOID VALUE FRICTION NUMBER]
 [VOID VALUE EQUIVALENT ELECTRONIC QC]
 {{ cpt.void_value_equivalent_electronic_qc }}
 [END OF VOID VALUE EQUIVALENT ELECTRONIC QC]
 [MEASURED DATA]
 [TABLE]
+DataCount={{ '{:>4}'.format(cpt.measured_data.data|length) }}
+{% if cpt.measured_data.data|length > 0 %}
 [COLUMN INDICATION]
 {% for key in cpt.measured_data.data[0].keys() %}
 {{ key }}
 {% endfor %}
 [END OF COLUMN INDICATION]
 [DATA]
 {% for row in cpt.measured_data.data %}
@@ -232,14 +233,15 @@
 {{ "{} ".format(value).rjust(5) }}
 {% else %}
 {{ "{} ".format(value).rjust(5) -}}
 {% endif %}
 {% endfor %}
 {% endfor %}
 [END OF DATA]
+{% endif %}
 [END OF TABLE]
 [END OF MEASURED DATA]
 {% if not loop.last %}
 [NEXT OF NUMBER OF CPTS]
 {% endif %}
 {% endfor %} 
 [END OF NUMBER OF CPTS]
@@ -273,14 +275,15 @@
 {{ '{:>12.2f}'.format(layer.excess_pore_pressure_top) }} : Excess pore pressure at top [kN/m3]
 {{ '{:>12.2f}'.format(layer.excess_pore_pressure_bottom) }} : Excess pore pressure at bottom [kN/m3]
 {{ '{:>12.2f}'.format(layer.ocr_value) }} : OCR value [-]
 {{ '{:>12}'.format(layer.reduction_core_resistance) }} : Reduction of cone resistance [%]
 {% endfor %}
 {% endfor %}
 [END OF PROFILES]
+{{user_clasification_method}}
 [SLOPES]
 {{ slopes }}
 [END OF SLOPES]
 [TYPES - BEARING PILES]
 {% if types___bearing_piles is not string %}
 0 : pile type shown in main graph
 {{ types___bearing_piles|length }} = number of items
@@ -357,17 +360,14 @@
 {{ '{:>6.2f}'.format(pile.reduction_percentage_qc) }} : Reduction percentage qc;III
 {{ '{:>2}'.format(pile.is_user_defined.value) }} : User defined name
 {% endfor %}
 {% else %}
 {{ types___bearing_piles }}
 {% endif %}
 [END OF TYPES - BEARING PILES]
-[TYPES - BEARING PILES BELGIAN]
-{{ types___bearing_piles_belgian }}
-[END OF TYPES - BEARING PILES BELGIAN]
 [TYPES - TENSION PILES (CUR)]
 {% if types___tension_piles_cur is not string %}
 0 : pile type shown in main graph
 {{ types___tension_piles_cur|length }} = number of items
 {% for pile in types___tension_piles_cur %}
 {{ pile.pile_name }}
 {{ '{:>2}'.format(pile.pile_type_for_execution_factor_sand_gravel.value) }} : Pile type for execution factor sand/gravel = {{ pile.pile_type_for_execution_factor_sand_gravel.name }}
@@ -433,14 +433,16 @@
 [END OF TYPES - SHALLOW FOUNDATIONS]
 [LOADS]
 {{ loads }}
 [END OF LOADS]
 [POSITIONS - BEARING PILES]
 {% if positions___bearing_piles is mapping %}
 [TABLE]
+DataCount={{ '{:>4}'.format(positions___bearing_piles.positions|length) }}
+{% if positions___bearing_piles.positions|length > 0 %}
 [COLUMN INDICATION]
 index
 X
 Y
 PileHeadLevel
 Surcharge
 LimitStateStrGeo
@@ -448,25 +450,25 @@
 PileName
 [END OF COLUMN INDICATION]
 [DATA]
 {% for position in positions___bearing_piles.positions %}
 {{ '{:>6}'.format(position.index) }}  {{ '{:>9.2f}'.format(position.x_coordinate) }} {{ '{:>9.2f}'.format(position.y_coordinate) }} {{ '{:>9.2f}'.format(position.pile_head_level) }} {{ '{:>9.2f}'.format(position.surcharge) }} {{ '{:>9.2f}'.format(position.limit_state_str) }} {{ '{:>9.2f}'.format(position.limit_state_service) }} {{ '{:>12}'.format(position.pile_name)}}
 {% endfor %}
 [END OF DATA]
+{% endif %}
 [END OF TABLE]
 {% else %}
 {{ positions___bearing_piles }}
 {% endif %}
 [END OF POSITIONS - BEARING PILES]
-[POSITIONS - BEARING PILES BELGIAN]
-{{ positions___bearing_piles_belgian }}
-[END OF POSITIONS - BEARING PILES BELGIAN]
 [POSITIONS - TENSION PILES (CUR)]
 {% if positions___tension_piles_cur is not string %}
 [TABLE]
+DataCount={{ '{:>4}'.format(positions___tension_piles_cur.positions|length) }}
+{% if positions___tension_piles_cur.positions|length > 0 %}
 [COLUMN INDICATION]
 index
 X
 Y
 PileHeadLevel
 UseAlternatingLoads
 MaxForce
@@ -476,30 +478,31 @@
 PileName
 [END OF COLUMN INDICATION]
 [DATA]
 {% for position in positions___tension_piles_cur.positions %}
 {{ '{:>6}'.format(position.index) }}  {{ '{:>9.2f}'.format(position.x_coordinate) }} {{ '{:>9.2f}'.format(position.y_coordinate) }} {{ '{:>9.2f}'.format(position.pile_head_level) }} {{ '{:>2}'.format(position.use_alternating_loads) }} {{ '{:>9.2f}'.format(position.max_force) }} {{ '{:>9.2f}'.format(position.min_force) }} {{ '{:>9.2f}'.format(position.limit_state_str) }} {{ '{:>9.2f}'.format(position.limit_state_service) }} {{ '{:>12}'.format(position.pile_name)}}
 {% endfor %}
 [END OF DATA]
+{% endif %}
 [END OF TABLE]
 {% else %}
 {{ positions___tension_piles_cur }}
 {% endif %}
 [END OF POSITIONS - TENSION PILES (CUR)]
 [POSITIONS - SHALLOW FOUNDATIONS]
 {{ positions___shallow_foundations }}
 [END OF POSITIONS - SHALLOW FOUNDATIONS]
 [CALCULATION OPTIONS]
 {% if calculation_options is mapping %}
 {% set co = calculation_options %}
 {{ '1 : Superstructure rigidity = Rigid' if co.is_rigid else '0 : Superstructure rigidity = Non-rigid' }}
 {{ '{:>12.3f}'.format(co.max_allowed_settlement_lim_state_str) }} : Max. allowed settlement [m]; lim. state STR/GEO
-{{ '{:>12.6f}'.format(co.max_allowed_rel_rotation_lim_state_str) }} : Max. allowed rel. rotation [m/m]; lim. state STR/GEO
+{{ '{:>12}'.format(co.max_allowed_rel_rotation_lim_state_str) }} : Reciprocal max. allowed rel. rotation [m/m]; lim. state STR/GEO
 {{ '{:>12.3f}'.format(co.max_allowed_settlement_lim_state_serv) }} : Max. allowed settlement [m]; serv. lim. state
-{{ '{:>12.6f}'.format(co.max_allowed_rel_rotation_lim_state_serv) }} : Max. allowed rel. rotation [m/m]; serv. lim. state
+{{ '{:>12}'.format(co.max_allowed_rel_rotation_lim_state_serv) }} : Reciprocal max. allowed rel. rotation [m/m]; serv. lim. state
 {{ co.is_xi3_overruled.value }} : Factor xi3 NEN overruled = {{ co.is_xi3_overruled.name }}
 {% if co.is_xi3_overruled %}
 {{ '{:>12.2f}'.format(co.factor_xi3) }} : Factor xi3 user defined
 {% endif %}
 {{ co.is_xi4_overruled.value }} : Factor xi4 NEN overruled = {{ co.is_xi4_overruled.name }}
 {% if co.is_xi4_overruled %}
 {{ '{:>12.2f}'.format(co.factor_xi4) }} : Factor xi4 user defined
@@ -512,14 +515,20 @@
 {% if co.is_gamma_fnk_overruled %}
 {{ '{:>12.2f}'.format(co.factor_gamma_fnk) }} : Factor gamma fnk user defined
 {% endif %}
 {{ co.is_area_overruled.value }} : Area overruled = {{ co.is_area_overruled.name }}
 {% if co.is_area_overruled %}
 {{ '{:>12.2f}'.format(co.area) }} : Area [m2] user defined
 {% endif %}
+{{ co.is_qbmax_overruled.value }} : Qb;max overruled = {{ co.is_qbmax_overruled.name }}
+{{ '{:>12.2f}'.format(co.qbmax) }} : Qb;max user defined
+{{ co.is_qcza_low_overruled.value }} : Qc;z;a low overruled = {{ co.is_qcza_low_overruled.name }}
+{{ '{:>12.2f}'.format(co.qcza_low) }} : Qc;z;a low user defined
+{{ co.is_qcza_high_overruled.value }} : Qc;z;a high overruled = {{ co.is_qcza_high_overruled.name }}
+{{ '{:>12.2f}'.format(co.qcza_high) }} : Qc;z;a high user defined
 {{ co.is_suppress_qc_reduction.value }} : Suppress qcIII reduction = {{ co.is_suppress_qc_reduction.name }}
 {{ co.is_overrule_excavation.value }} : Overrule excavation = {{ co.is_overrule_excavation.name }}
 {{ co.use_pile_group.value }} : Use pile group = {{ co.use_pile_group.name }}
 {{ co.is_write_intermediate_results.value }} : Write intermediate results = {{ co.is_write_intermediate_results.name }}
 {{ co.use_interaction_model.value }} : Use interaction model = {{ co.use_interaction_model.name }}
 0 : Is gamma;gamma overruled (LS STR/GEO) = FALSE
         1.00 : Factor gamma;gamma (LS STR/GEO) user defined
@@ -546,33 +555,18 @@
 {{ '{:>12.2f}'.format(co.factor_gamma_st) }} : Factor gamma st user defined
 {{ co.is_gamma_gamma_overruled.value }} : Gamma gamma overruled = {{ co.is_gamma_gamma_overruled.name }}
 {{ '{:>12.2f}'.format(co.factor_gamma_gamma) }} : Factor gamma_gamma user defined
 {{ '{:>12.2f}'.format(co.surcharge) }} : Surcharge [kN/m2]
 {{ co.use_piezometric_levels.value }} : Use Piezometric levels = {{ co.use_piezometric_levels.name }}
 {{ co.use_almere_rules.value }} : Use Almere rules = {{ co.use_almere_rules.name }}
 {{ co.use_extra_almere_rules.value }} : Use Extra Almere rules = {{ co.use_extra_almere_rules.name }}
-0 : Xi3 BPB overruled = FALSE
-0 : Xi4 BPB overruled = FALSE
-0 : Gamma rd overruled = FALSE
-        1.00 : Factor xi3 user defined
-        1.00 : Factor xi4 user defined
-        1.00 : Factor Gamma rd user defined
-0 : Gamma b BPB overruled = FALSE
-        1.00 : Factor Gamma b user defined
-0 : Gamma s BPB overruled = FALSE
-        1.00 : Factor Gamma s user defined
- 0 : Suppress all qc reduction (BP) = FALSE
 {{ co.is_ea_gem_overruled.value }} : Eea;gem overruled = {{ co.is_ea_gem_overruled.name }}
 {{ '{:.2f}'.format(co.ea_gem) }} : Eea;gem user defined
-0 : Use Quality Assurance = FALSE
-     1000.00 : Area covered per CPT
 {{ co.is_gamma_s_overruled.value }} : Gamma s for NEN overruled = {{ co.is_gamma_s_overruled.name }}
 {{ '{:>12.2f}'.format(co.factor_gamma_s) }} : Factor Gamma s for NEN user defined
-0 : Factor Beta (BPB) overruled = FALSE
-        1.00 : Factor Beta (BPB) user defined
 {% else %}
 {{ calculation_options }}
 {% endif %}
 [END OF CALCULATION OPTIONS]
 [CALCULATIONTYPE]
 {% if calculationtype is mapping %}
  {{ calculationtype.main_calculationtype.value }} : Main calculationtype
@@ -610,16 +604,13 @@
 {% endif %}
 {% endfor %}
 {% endif %}
 {% else %}
 {{ preliminary_design }}
 {% endif %}
 [END OF PRELIMINARY DESIGN]
-[DE BEER]
-{{ de_beer }}
-[END OF DE BEER]
 [LOCATION MAP]
 
        {{ location_map }}
 [END OF LOCATION MAP]
 
 [END OF INPUT DATA]
```

### Comparing `d_geolib-0.5.1/geolib/models/dgeoflow/dgeoflow_model.py` & `d_geolib-0.6.0/geolib/models/dgeoflow/dgeoflow_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dgeoflow/dgeoflow_parserprovider.py` & `d_geolib-0.6.0/geolib/models/dgeoflow/dgeoflow_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dgeoflow/internal.py` & `d_geolib-0.6.0/geolib/models/dgeoflow/internal.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dgeoflow/serializer.py` & `d_geolib-0.6.0/geolib/models/dgeoflow/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dgeoflow/utils.py` & `d_geolib-0.6.0/geolib/models/dgeoflow/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dseries_parser.py` & `d_geolib-0.6.0/geolib/models/dseries_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,18 +99,18 @@
                 else:
                     if DataClass in fieldtype.__mro__:
                         logger.debug(f"Can't parse {fieldtype} for {field} yet")
 
             # If the body is a List[string], we should check
             # whether we can parse it further.
             elif (
-                field in kwargs
-                and isinstance(kwargs[field], list)
-                and len(kwargs[field]) > 0
-                and isinstance(kwargs[field][0], str)
+                    field in kwargs
+                    and isinstance(kwargs[field], list)
+                    and len(kwargs[field]) > 0
+                    and isinstance(kwargs[field][0], str)
             ):
                 body = kwargs[field]
 
                 # We need to decompose a possible Union
                 if is_union(fieldtype):
                     fieldtype, *_ = get_args(fieldtype)
 
@@ -304,17 +304,57 @@
         Args:
             lines (List[str]): Parsed rows.
         """
         pass
 
     @classmethod
     def parse_text(cls, text):
-        unwrapped_text = DSerieParser.parse_group_as_dict(text)
-        return super().parse_text(list(unwrapped_text.values())[0])
+        """Parses a Table wrapped in another group such as:
+        [TABLE]
+        DataCount = x followed by
+        [END OF TABLE]  directly when x = 0 or, when x > 0, by
+        [COLUMN INDICATION]
+        A
+        B
+        [END OF COLUMN INDICATION]
+        [DATA]
+        1 1
+        2 2
+        [END OF DATA]
+        [END OF TABLE]
+
+        Args:
+            text (str): Wrapped table group to parse.
+
+        Returns:
+            DSerieStructure: Parsed structure.
+        """
+
+        def split_line(text: str) -> List[str]:
+            parts = re.split("[ \t]", text.strip())
+            return list(filter(lambda part: part != "", parts))
+
+        table_text = list(DSerieParser.parse_list_group(text).values())[0]
+        table_data = list(DSerieParser.parse_list_group(table_text).values())
+        if len(table_data) == 0:
+            values_dict_list = table_data;
+            collection_property_name = list(cls.__fields__.items())[0][0]
+            return cls(**{collection_property_name: values_dict_list})
+        else:
+            # Expected two groups (column_indication and data)
+            keys = table_data[0].split("\n")
+            keys = [make_key(j) for j in keys]
+
+            values_dict_list = [
+                dict(zip(keys, values))
+                for values in map(split_line, table_data[1].split("\n"))
+            ]
+            collection_property_name = list(cls.__fields__.items())[0][0]
 
+        return cls(**{collection_property_name: values_dict_list})
 
 class DSerieOldTableStructure(DSeriesStructure):
     @classmethod
     def parse_text(cls, text: str):
         """Creates a DSeriesStructure that can parse fields like
 
         [GROUP]
@@ -496,15 +536,15 @@
     @classmethod
     def get_properties_in_text(cls, text: str):
         required_properties_names = [
             structure_name for structure_name, _ in cls.get_structure_required_fields()
         ]
         header_lines = cls.header_lines()
         for idx, (key, value) in enumerate(
-            DSerieParser.parse_group(text, loose_properties=True)
+                DSerieParser.parse_group(text, loose_properties=True)
         ):
             if idx < header_lines:
                 continue
             if not key:
                 # Only loose properties would get through here.
                 # So a grouped property enclosed like [PROPERTY][END OF PROPERTY].
                 key, value = cls.get_property_key_value(
@@ -724,16 +764,16 @@
 
         Returns:
             DSeriesStructure: Parsed structrure.
         """
         generated_dict = {}
         no_key_group_values = []
         for group_key, group_values in groupby(
-            list(DSerieParser.parse_group(text, loose_properties=True)),
-            lambda key_value: key_value[0],
+                list(DSerieParser.parse_group(text, loose_properties=True)),
+                lambda key_value: key_value[0],
         ):
             filtered_values = [value for key, value in group_values]
             if not group_key:
                 no_key_group_values.extend(filtered_values)
                 continue
             if cls.group_value_is_list(group_key):
                 if group_key in generated_dict:
@@ -859,15 +899,15 @@
         parsed_structure, _ = cls.parse_text_lines(
             [split_line_elements(line) for line in text.split("\n") if line != ""]
         )
         return parsed_structure
 
     @classmethod
     def parse_text_lines(
-        cls, text_lines: List[List[str]]
+            cls, text_lines: List[List[str]]
     ) -> Tuple[DSeriesStructure, int]:
         """Parses a list of strings into the properties of a structure.
         Example:
             [   ["1", "Property value"],
                 ["2", "Values in Property"],
                 ["4", "2"]]
         Args:
@@ -879,15 +919,15 @@
 
         Returns:
             DSeriesStructure: Structure with parsed properties.
             int: Index of last line being read as part of current structure.
         """
 
         def get_list_values(
-            struct_idx: int, field_name: str, text_lines: list
+                struct_idx: int, field_name: str, text_lines: list
         ) -> Tuple[DSeriesStructure, int]:
             """Auxiliar method to either parse as a DSeriesStructure or as a list of
             any different object.
 
             Args:
                 struct_idx (int): Type index in the class definition.
                 field_name (str): Name of the field.
@@ -914,17 +954,17 @@
         for struct_idx, (field_name, field) in enumerate(required_fields):
             if lines_read >= len(text_lines):
                 raise ValueError(f"Expected text line property for {field_name}.")
             iteration_lines = 1
             field = unpack_if_union(field)
             # if the current property is a list, then extract the next line values.
             if (
-                is_list(field)
-                or issubclass(field, list)
-                or is_structure_collection(field)
+                    is_list(field)
+                    or issubclass(field, list)
+                    or is_structure_collection(field)
             ):
                 lines_to_parse = cls.get_next_property_text_lines(text_lines[lines_read:])
                 parsed_tuple = get_list_values(struct_idx, field_name, lines_to_parse)
                 (
                     properties[field_name],
                     iteration_lines,
                 ) = cls.get_tree_structure_read_lines(parsed_tuple)
@@ -950,15 +990,15 @@
         Returns:
             list: Filtered list of text to be parsed into a property.
         """
         return text_lines
 
     @classmethod
     def get_tree_structure_read_lines(
-        cls, parsed_tuple: Tuple[DSeriesStructure, int]
+            cls, parsed_tuple: Tuple[DSeriesStructure, int]
     ) -> Tuple[DSeriesStructure, int]:
         """Allows inherited classes to override how many lines have been actually been read
         for a given parsed structure based on the cls being instantiated.
 
         Args:
             parsed_tuple (Tuple[DSeriesStructure, int]): Tuple of parsed structure and read lines for it.
 
@@ -1012,15 +1052,15 @@
             for line in text_lines[0][0].split("\n")
             if line != ""
         ]
         return filtered_property_lines
 
     @classmethod
     def get_tree_structure_read_lines(
-        cls, parsed_tuple: Tuple[DSeriesStructure, int]
+            cls, parsed_tuple: Tuple[DSeriesStructure, int]
     ) -> Tuple[DSeriesStructure, int]:
         # Only one line is meant to be read as parsed_text_lines is mapped 1:1 lines-properties.
         return parsed_tuple[0], 1
 
 
 class DSeriesTreeStructureCollection(DSeriesStructure):
     # TODO Deprecate.
@@ -1063,15 +1103,15 @@
         Returns:
             int: Number of structures expected.
         """
         return int(get_line_property_value(lines[0][0], reversed_key=True))
 
     @classmethod
     def parse_collection_type(
-        cls, collecion_type: Type, lines: list
+            cls, collecion_type: Type, lines: list
     ) -> Tuple[DSeriesStructure, int]:
         return collecion_type.parse_text_lines(lines)
 
     @classmethod
     def parse_text_lines(cls, lines: List[str]) -> Tuple[DSeriesStructure, int]:
         # Get class types
         collection_property_name = list(cls.__fields__.items())[0][0]
@@ -1099,15 +1139,15 @@
 class DSeriesMatrixTreeStructureCollection(DSeriesTreeStructureCollection):
     # TODO Deprecate.
     # This class is overdoing logic that is later on being handled by its parent (DSeriesStructure).
     # It should therefore only be responsible for generating a dictionary of field name - string values,
     # but not object creation.
     @classmethod
     def parse_collection_type(
-        cls, collecion_type: Type, lines: list
+            cls, collecion_type: Type, lines: list
     ) -> Tuple[DSeriesStructure, int]:
         parsed_structure, _ = collecion_type.parse_text_lines(
             [[line] for line in lines[0]]
         )
         return parsed_structure, 1
 
 
@@ -1173,15 +1213,15 @@
         }
 
         """
         return dict(DSerieParser.parse_group(text_lines=text_lines, unique_keys=True))
 
     @staticmethod
     def parse_group(
-        text_lines: str, loose_properties: bool = False, unique_keys: bool = False
+            text_lines: str, loose_properties: bool = False, unique_keys: bool = False
     ) -> Iterable[Tuple[str, str]]:
         """Parses a text with headers such as [GROUP] and [END OF GROUP] and
         yields each property of the group as a Tuple[property name, value].
         Because it is an iterable it may contain repeated elements.
         Delegating responsibility on what to do with such elements to the caller.
 
         Example:
@@ -1246,17 +1286,17 @@
                 if currentkey:
                     data += line + "\n"
                 elif not currentkey and loose_properties:
                     yield (currentkey, line)
 
     @staticmethod
     def parse_list_group(
-        text: str,
-        exceptions=["vertical", "soil", "residual_settlements"],
-        skipped_keys=[],
+            text: str,
+            exceptions=["vertical", "soil", "residual_settlements"],
+            skipped_keys=[],
     ) -> Dict[str, Union[List[str], str]]:
         """Method to parse several groups in a sli/sld file that can include repeated groups.
 
         Includes an exception to always parse a group as a list.
         Can parse the following:
 
         [GROUP A]
@@ -1454,15 +1494,15 @@
 
 
 def is_structure_collection(field: Type) -> bool:
     return inspect.isclass(field) and issubclass(field, DSeriesStructure)
 
 
 def read_property_as_list(
-    field_name: str, field: Type, text_lines: list
+        field_name: str, field: Type, text_lines: list
 ) -> Tuple[List[DSeriesStructure], int]:
     """Reads a property containing a collection of values represented as
     a list of strings.
 
     Args:
         field_name (str): Name of the field to parse.
         field (Type): Type to parse the values to.
@@ -1483,15 +1523,15 @@
     while len(list_values) < list_size:
         if lines_read >= len(text_lines):
             raise ValueError(f"Expected {list_size} values for property {field_name}.")
         iteration_lines = 1
         lines_to_parse = text_lines[lines_read:]
         if issubclass(field, DSeriesTreeStructureCollection):
             # If its an encapsuled collection, number of lines needs to be given.
-            lines_to_parse = text_lines[lines_read - 1 :]
+            lines_to_parse = text_lines[lines_read - 1:]
 
         if is_structure_collection(field):
             parsed_values, iteration_lines = field.parse_text_lines(lines_to_parse)
             list_values.append(parsed_values)
         else:
             parsed_values = text_lines[lines_read]
             list_values.extend(parsed_values)
```

### Comparing `d_geolib-0.5.1/geolib/models/dsettlement/drains.py` & `d_geolib-0.6.0/geolib/models/dsettlement/drains.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsettlement/dsettlement_model.py` & `d_geolib-0.6.0/geolib/models/dsettlement/dsettlement_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsettlement/dsettlement_parserprovider.py` & `d_geolib-0.6.0/geolib/models/dsettlement/dsettlement_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsettlement/dsettlement_structures.py` & `d_geolib-0.6.0/geolib/models/dsettlement/dsettlement_structures.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsettlement/internal.py` & `d_geolib-0.6.0/geolib/models/dsettlement/internal.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsettlement/internal_soil.py` & `d_geolib-0.6.0/geolib/models/dsettlement/internal_soil.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsettlement/loads.py` & `d_geolib-0.6.0/geolib/models/dsettlement/loads.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsettlement/serializer.py` & `d_geolib-0.6.0/geolib/models/dsettlement/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsettlement/templates/input.sli.j2` & `d_geolib-0.6.0/geolib/models/dsettlement/templates/input.sli.j2`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsettlement/templates/soil_template.j2` & `d_geolib-0.6.0/geolib/models/dsettlement/templates/soil_template.j2`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsheetpiling/calculation_options.py` & `d_geolib-0.6.0/geolib/models/dsheetpiling/calculation_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from abc import ABCMeta, abstractmethod
 from typing import Optional, Union
 
-from pydantic.types import confloat, conint
-
 from geolib.models import BaseDataClass
+from pydantic.types import confloat, conint
 
 from .settings import (
     CalculationType,
     DesignType,
     PartialFactorCalculationType,
     PartialFactorSetCUR,
     PartialFactorSetEC,
-    PartialFactorSetEC7NADB,
+    PartialFactorSetEC7NADBE,
     PartialFactorSetEC7NADNL,
     PartialFactorSetVerifyEC,
     VerifyType,
 )
 
 
 class CalculationOptionsPerStage(BaseDataClass):
@@ -25,15 +24,19 @@
     Arguments:
      anchor_factor: multiplication factor for the anchor stiffness.
      partial_factor_set: partial factor sets corresponding to different code annexes.
     """
 
     anchor_factor: float = 1
     partial_factor_set: Optional[
-        Union[PartialFactorSetEC7NADB, PartialFactorSetCUR, PartialFactorSetEC7NADNL]
+        Union[
+            PartialFactorSetEC7NADBE,
+            PartialFactorSetCUR,
+            PartialFactorSetEC7NADNL,
+        ]
     ] = None
 
 
 class CalculationOptions(BaseDataClass, metaclass=ABCMeta):
     """Base class for all calculation options.
 
     Arguments:
@@ -83,29 +86,31 @@
     """Overall stability calculation selected in Start Calculation window.
 
     Arguments:
      cur_stability_stage: Id of the stage to be checked. This id refers to D-SheetPiling so the first stage in D-SheetPiling has an input of 0.
      overall_stability_type: which type of calculation is going to be performed
      stability_eurocode_partial_factor_set: partial factor set selected for the EC7 General calculation
      stability_ec7_nl_partial_factor_set: partial factor set selected for the EC7 NL calculation
-     stability_ec7_b_partial_factor_set: partial factor set selected for the EC7 B calculation
+     stability_ec7_be_partial_factor_set: partial factor set selected for the EC7 BE calculation
      stability_cur_partial_factor_set: partial factor set selected for the CUR calculation
+     stability_export: Set on True to generate an input file with STI format which can be opened with D-Geo Stability
     """
 
     input_calculation_type: CalculationType = CalculationType.OVERALL_STABILITY
     cur_stability_stage: conint(ge=0) = 0
     overall_stability_type: DesignType = DesignType.REPRESENTATIVE
     stability_eurocode_partial_factor_set: PartialFactorSetEC = PartialFactorSetEC.DA1SET1
     stability_ec7_nl_partial_factor_set: PartialFactorSetEC7NADNL = (
         PartialFactorSetEC7NADNL.RC0
     )
-    stability_ec7_b_partial_factor_set: PartialFactorSetEC7NADB = (
-        PartialFactorSetEC7NADB.SET1
+    stability_ec7_be_partial_factor_set: PartialFactorSetEC7NADBE = (
+        PartialFactorSetEC7NADBE.SET1
     )
     stability_cur_partial_factor_set: PartialFactorSetCUR = PartialFactorSetCUR.CLASSI
+    stability_export: bool = False
 
 
 class KranzAnchorStrengthCalculationOptions(CalculationOptions):
     """Kranz anchor strength calculation selected in Start Calculation
     window.
 
     Arguments:
@@ -136,15 +141,15 @@
      verify_type: Select partial factor set
      eurocode_partial_factor_set: Select partial factor set
      eurocode_overall_stability: Set to True to perform an overall stability calculation using modified values for soil properties (cohesion, friction angle and unit weight) depending on the Design approach chosen for all stages.
      ec7_nl_method: Select method of calculation according to CUR 166 design procedure
      ec7_nl_overall_partial_factor_set: Select partial factor set
      ec7_nl_overall_anchor_factor: multiplication factor for the anchor stiffness
      ec7_nad_nl_overall_stability: Set to True to perform an overall stability calculation using modified values for soil properties (cohesion, friction angle and unit weight) depending on the Design approach chosen for all stages.
-     ec7_b_overall_stability: Set to True to perform an overall stability calculation using modified values for soil properties (cohesion, friction angle and unit weight) depending on the Design approach chosen for all stages.
+     ec7_be_overall_stability: Set to True to perform an overall stability calculation using modified values for soil properties (cohesion, friction angle and unit weight) depending on the Design approach chosen for all stages.
      nb_method: Select method of calculation according to CUR 166 design procedure
      cur_method: Select method of calculation according to CUR 166 design procedure
      cur_overall_partial_factor_set: Select partial factor set
      cur_overall_anchor_factor: multiplication factor for the anchor stiffness
      cur_overall_stability: Set to True to perform an overall stability calculation using modified values for soil properties (cohesion, friction angle and unit weight) depending on the Design approach chosen for all stages.
     """
 
@@ -154,15 +159,15 @@
     eurocode_overall_stability: bool = False
     ec7_nl_method: PartialFactorCalculationType = PartialFactorCalculationType.METHODA
     ec7_nl_overall_partial_factor_set: PartialFactorSetEC7NADNL = (
         PartialFactorSetEC7NADNL.RC0
     )
     ec7_nl_overall_anchor_factor: confloat(ge=0.001, le=1000) = 1
     ec7_nad_nl_overall_stability: bool = False
-    ec7_b_overall_stability: bool = False
+    ec7_be_overall_stability: bool = False
     nb_method: PartialFactorCalculationType = PartialFactorCalculationType.METHODA
     cur_method: PartialFactorCalculationType = PartialFactorCalculationType.METHODA
     cur_overall_partial_factor_set: PartialFactorSetCUR = PartialFactorSetCUR.CLASSI
     cur_overall_anchor_factor: confloat(ge=0.001, le=1000) = 1
     cur_overall_stability: bool = False
 
     @property
@@ -183,16 +188,16 @@
      design_pile_length_from: The starting point of the pile over which the analysis should be performed.
      design_pile_length_to: The end point of the pile over which the analysis should be performed
      design_pile_length_decrement: the Decrement in length for each analysis step.
      design_type: types of design.
      design_eurocode_partial_factor_set: Select partial factor set
      design_partial_factor_set_ec7_nad_nl: Select partial factor set
      design_ec7_nl_method: Select method of calculation according to CUR 166 design procedure
-     design_partial_factor_set_ec7_nad_b: Select partial factor set
-     design_ec7_b_method: Select method of calculation according to CUR 166 design procedure
+     design_partial_factor_set_ec7_nad_be: Select partial factor set
+     design_ec7_be_method: Select method of calculation according to CUR 166 design procedure
      design_partial_factor_set: Select partial factor set
      design_cur_method: Select method of calculation according to CUR 166 design procedure
     """
 
     input_calculation_type: CalculationType = CalculationType.DESIGN_SHEETPILING_LENGTH
     design_stage: conint(ge=0) = 0
     design_pile_length_from: confloat(ge=1, le=100) = 1
@@ -202,15 +207,15 @@
     design_eurocode_partial_factor_set: PartialFactorSetEC = PartialFactorSetEC.DA1SET1
     design_partial_factor_set_ec7_nad_nl: PartialFactorSetEC7NADNL = (
         PartialFactorSetEC7NADNL.RC0
     )
     design_ec7_nl_method: PartialFactorCalculationType = (
         PartialFactorCalculationType.METHODA
     )
-    design_partial_factor_set_ec7_nad_b: PartialFactorSetEC7NADB = (
-        PartialFactorSetEC7NADB.SET1
+    design_partial_factor_set_ec7_nad_be: PartialFactorSetEC7NADBE = (
+        PartialFactorSetEC7NADBE.SET1
     )
-    design_ec7_b_method: PartialFactorCalculationType = (
+    design_ec7_be_method: PartialFactorCalculationType = (
         PartialFactorCalculationType.METHODA
     )
     design_partial_factor_set: PartialFactorSetCUR = PartialFactorSetCUR.CLASSI
     design_cur_method: PartialFactorCalculationType = PartialFactorCalculationType.METHODA
```

### Comparing `d_geolib-0.5.1/geolib/models/dsheetpiling/constructions.py` & `d_geolib-0.6.0/geolib/models/dsheetpiling/constructions.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """
     Pile selected from the model window in D-Sheet Piling
 
     Arguments:
      material_type : Select the material of the sheet piling element : User defined, Steel, Concrete, Wood, Synthetic.
      elastic_stiffness_ei  : Stiffness of the section per running meter.
      section_bottom_level  : the vertical co-ordinate of the bottom of the sheet piling, in relation to the reference level.
-     mr_char_el : Characterictic elastic moment without safety factors.
+     mr_char_el : Characteristic elastic moment without safety factors.
      material_factor_gamma_m  : The partial safety factor \u03B3 m should be defined, only if the User defined material type
      is selected. Otherwise, the program will automatically apply the following factors
      (acc. to the corresponding Eurocode) to calculate the design allowable moment
      * Steel : \u03B3m = 1 , acc. to Eurocode 3 – Part 5, art. 5.1.1(4)
      * Concrete : \u03B3m = 1.1, acc. to Eurocode 2 – Part 1.1, art. 3.1.6
      * Wood : \u03B3m = 1 , acc. to Eurocode 5 – Part 1-2, art. 2.3(1)
      * Synthetic : \u03B3m = 1.2
@@ -80,15 +80,15 @@
 
 
     Arguments:
      material_type : Select the material of the sheet piling element : User defined, Steel, Concrete, Wood, Synthetic.
      acting_width : The acting width can be used when the effective width changes along the sheet piling. D-SHEET PILING uses the acting width as a multiplication factor for the sheet piling stiffness and all loads, supports and reactions, except the normal force.
      elastic_stiffness_ei : Stiffness of the section per running meter.
      section_bottom_level : the vertical co-ordinate of the bottom of the sheet piling, in relation to the reference level.
-     mr_char_el: Characterictic elastic moment without safety factors.
+     mr_char_el: Characteristic elastic moment without safety factors.
      material_factor_gamma_m : The partial safety factor \u03B3m should be defined, only if the User defined material type is selected. Otherwise, the program will automatically apply the following factors (acc. to the corresponding Eurocode) to calculate the design allowable moment:
 
         * Steel: \u03B3m = 1 , acc. to Eurocode 3 – Part 5, art. 5.1.1(4)
         * Concrete: \u03B3m = 1.1, acc. to Eurocode 2 – Part 1.1, art. 3.1.6
         * Wood: \u03B3m = 1 , acc. to Eurocode 5 – Part 1-2, art. 2.3(1)
         * Synthetic: \u03B3m = 1.2
 
@@ -96,15 +96,14 @@
 
         * Steel: kmod = 1
         * Concrete: kmod = 1
         * Wood: kmod= 1
 
      reduction_factor_on_maximum_moment : The reduction factor applied to the maximum allowable moment
      reduction_factor_on_ei : Reduction factor applied on the stiffness EI of the pile.
-     coating_area : The area of coating of the sheet piling (> 1). This is defined as the
      length of the perimeter of the sheet piling section per running meter of wall [m2/m2 wall].
 
      height : The thickness of the sheet piling profile [mm].
      elastic_section_modulus_w_el: The section modulus (also called resisting moment in the Netherlands) of the sheet piling,
      [cm3/m], used for a Feasibility control
      section_area : The cross-sectional area of the sheet piling, [cm3/m].
 
@@ -113,17 +112,16 @@
     material_type: Optional[
         SheetPilingElementMaterialType
     ] = SheetPilingElementMaterialType.Steel
     elastic_stiffness_ei: Optional[float] = None
     acting_width: Optional[float] = None
     section_bottom_level: Optional[
         float
-    ] = None  # TODO important paramter, shouldn't be default
+    ] = None  # TODO important parameter, shouldn't be default
     height: Optional[int] = 400  # value is defined in mm
-    coating_area: Optional[float] = None
     width_of_sheet_piles: Optional[float] = None
     section_area: Optional[int] = None
     elastic_section_modulus_w_el: Optional[int] = None
     reduction_factor_on_ei: Optional[float] = None
     note_on_reduction_factor: Optional[str] = None
     mr_char_el: Optional[float] = None
     mr_char_pl: Optional[float] = None
@@ -309,15 +307,14 @@
         return SheetPileElement(
             name=self.name,
             sheetpilingelementmaterialtype=self.sheet_pile_properties.material_type,
             sheetpilingelementei=self.sheet_pile_properties.elastic_stiffness_ei,
             sheetpilingelementwidth=self.sheet_pile_properties.acting_width,
             sheetpilingelementlevel=self.sheet_pile_properties.section_bottom_level,
             sheetpilingelementheight=self.sheet_pile_properties.height,
-            sheetpilingelementcoatingarea=self.sheet_pile_properties.coating_area,
             sheetpilingpilewidth=self.sheet_pile_properties.width_of_sheet_piles,
             sheetpilingelementsectionarea=self.sheet_pile_properties.section_area,
             sheetpilingelementresistingmoment=self.sheet_pile_properties.elastic_section_modulus_w_el,
             sheetpilingelementreductionfactorei=self.sheet_pile_properties.reduction_factor_on_ei,
             sheetpilingelementnote=self.sheet_pile_properties.note_on_reduction_factor,
             sheetpilingelementmaxcharacteristicmoment=self.sheet_pile_properties.mr_char_el,
             sheetpilingelementmaxplasticcharacteristicmoment=self.sheet_pile_properties.mr_char_pl,
```

### Comparing `d_geolib-0.5.1/geolib/models/dsheetpiling/dsheetpiling_model.py` & `d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
 from subprocess import CompletedProcess, run
 from typing import Any, BinaryIO, List, Optional, Type, Union
 
-from pydantic import FilePath, PositiveFloat
-from pydantic.types import confloat, conint
-
 from geolib.geometry import Point
 from geolib.models import BaseDataClass, BaseModel, BaseModelStructure
 from geolib.models.dsheetpiling.constructions import DiaphragmWall, Pile, Sheet
 from geolib.models.meta import CONSOLE_RUN_BATCH_FLAG
 from geolib.soils import Soil
+from pydantic import FilePath, PositiveFloat
+from pydantic.types import confloat, conint
 
 from .calculation_options import CalculationOptions, CalculationOptionsPerStage
 from .dsheetpiling_parserprovider import DSheetPilingParserProvider
 from .internal import CalculationOptions as CalculationOptionsInternal
 from .internal import (
     DSheetPilingDumpStructure,
     DSheetPilingOutputStructure,
@@ -37,15 +36,15 @@
     DesignType,
     LateralEarthPressureMethod,
     LateralEarthPressureMethodStage,
     ModelType,
     PartialFactorCalculationType,
     PartialFactorSetCUR,
     PartialFactorSetEC,
-    PartialFactorSetEC7NADB,
+    PartialFactorSetEC7NADBE,
     PartialFactorSetEC7NADNL,
     PartialFactorSetVerifyEC,
     PassiveSide,
     Side,
     SinglePileLoadOptions,
     VerifyType,
 )
@@ -138,15 +137,15 @@
 
     @property
     def parser_provider_type(self) -> Type[DSheetPilingParserProvider]:
         return DSheetPilingParserProvider
 
     @property
     def console_path(self) -> Path:
-        return Path("DSheetPilingConsole/DSheetPilingConsole.exe")
+        return Path("DSheetPiling/DSheetPiling.exe")
 
     @property
     def console_flags(self) -> List[str]:
         return [CONSOLE_RUN_BATCH_FLAG]
 
     @property
     def output(self) -> DSheetPilingOutputStructure:
@@ -156,29 +155,29 @@
     def model_type(self) -> Union[str, ModelType]:
         return self.datastructure.input_data.model.model
 
     def serialize(self, filename: Union[FilePath, BinaryIO]):
         ds = self.datastructure.input_data.dict()
         ds.update(
             {
-                "version": self.datastructure.version.dict(),
-                "version_externals": self.datastructure.version_externals.dict(),
+                "version": self.datastructure.input_data.version.dict(),
+                "version_externals": self.datastructure.input_data.version_externals.dict(),
             }
         )
         serializer = DSheetPilingInputSerializer(ds=ds)
         serializer.write(filename)
         if isinstance(filename, Path):
             self.filename = filename
 
     def _is_calculation_per_stage_required(self) -> bool:
         """Function that checks if [CALCULATION PER STAGE] can be modified. This is true for a verify sheet-piling calculation and method B."""
         _map_method_b_available = {
             VerifyType.CUR: self.datastructure.input_data.calculation_options.curmethod,
             VerifyType.EC7NL: self.datastructure.input_data.calculation_options.ec7nlmethod,
-            VerifyType.EC7BE: self.datastructure.input_data.calculation_options.nbmethod,
+            VerifyType.EC7BE: self.datastructure.input_data.calculation_options.ec7bemethod,
         }
         if (
             self.datastructure.input_data.calculation_options.inputcalculationtype
             == CalculationType.VERIFY_SHEETPILING
         ):
             if (
                 _map_method_b_available[
```

### Comparing `d_geolib-0.5.1/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py` & `d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsheetpiling/dsheetpiling_structures.py` & `d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_structures.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,18 +73,15 @@
 
         Args:
             text (str): Full contains containing table structure and values.
 
         Returns:
             DSeriesStructure: Fully parsed structure.
         """
-        splitted_text = text.split("\n")
-        # Skip validating for now.
-        splitted_text.pop(0)
-        return super().parse_text("\n".join(splitted_text))
+        return super().parse_text(text)
 
 
 class DSheetpilingUnwrappedTable(DSeriesStructure):
     @classmethod
     def parse_text(cls, text):
         lines = text.split("\n")
         nrow = int(lines.pop(0).split()[0])
```

### Comparing `d_geolib-0.5.1/geolib/models/dsheetpiling/dsheetpiling_validator.py` & `d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_validator.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsheetpiling/internal.py` & `d_geolib-0.6.0/geolib/models/dsheetpiling/internal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import logging
 import warnings
 from abc import ABCMeta
 from enum import Enum, IntEnum
 from inspect import cleandoc
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
-from pydantic import confloat, conint, conlist, constr
-
 import geolib.models.dsheetpiling.constructions as constructions
 from geolib.geometry import Point
 from geolib.models import BaseDataClass
 from geolib.models.dseries_parser import (
     DSerieListStructure,
     DSeriesInlineMappedProperties,
     DSeriesInlineReversedProperties,
@@ -20,14 +18,15 @@
     DSeriesStructureCollection,
     DSeriesTableStructure,
     DSeriesUnmappedNameProperties,
     DSeriesWrappedTableStructure,
     DSerieVersion,
 )
 from geolib.utils import make_newline_validator
+from pydantic import confloat, conint, conlist, constr
 
 from .calculation_options import (
     CalculationOptionsPerStage as CalculationOptionsPerStageExternal,
 )
 from .dsheetpiling_structures import (
     DSeriesPilingDumpParserStructure,
     DSeriesPilingParserStructure,
@@ -37,23 +36,20 @@
     DSheetpilingWithNumberOfRowsTable,
 )
 from .dsheetpiling_validator import DSheetPilingValidator
 from .internal_partial_factors import (
     PartialFactorsCurI,
     PartialFactorsCurIi,
     PartialFactorsCurIii,
-    PartialFactorsEc7BSet1,
-    PartialFactorsEc7BSet2,
+    PartialFactorsEc7BESet1,
+    PartialFactorsEc7BESet2,
     PartialFactorsEc7Nl0,
     PartialFactorsEc7Nl1,
     PartialFactorsEc7Nl2,
     PartialFactorsEc7Nl3,
-    PartialFactorsEc7SeVk1,
-    PartialFactorsEc7SeVk2,
-    PartialFactorsEc7SeVk3,
     PartialFactorsEurocodeDa1Set1,
     PartialFactorsEurocodeDa1Set2,
     PartialFactorsEurocodeDa2,
     PartialFactorsEurocodeDa3,
 )
 from .settings import (
     CalculationType,
@@ -71,15 +67,15 @@
     LoadTypePermanentVariable,
     ModelType,
     ModulusReactionType,
     ModulusSubgradeReaction,
     PartialFactorCalculationType,
     PartialFactorSetCUR,
     PartialFactorSetEC,
-    PartialFactorSetEC7NADB,
+    PartialFactorSetEC7NADBE,
     PartialFactorSetEC7NADNL,
     PartialFactorSetVerifyEC,
     PassiveSide,
     SheetPilingElementMaterialType,
     Side,
     SinglePileLoadOptions,
     SoilTypeModulusSubgradeReaction,
@@ -92,25 +88,24 @@
 _DEFAULT_WATER_LEVEL_NAME: str = "New Water Level"
 _DEFAULT_SOIL_PROFILE_NAME: str = "New Profile"
 _DEFAULT_SURFACE_NAME: str = "New Surface"
 _DEFAULT_SHEET_PILING_ELEMENT_NAME: str = "New element"
 _DEFAULT_UNIT_WEIGHT_WATER: float = 9.81
 _DEFAULT_PRE_STRESS: float = 0.0
 
-_DEFAULT_SOIL_VERSION: int = 1007
-_DEFAULT_SHEETPILING_VERSION: int = 1026
+_DEFAULT_SOIL_VERSION: int = 1010
+_DEFAULT_SHEETPILING_VERSION: int = 1033
 
 REQ_RUN_LINES = 2
 
 
 class Model(DSeriesInlineReversedProperties):
     model: ModelType = ModelType.SHEET_PILING
     method: LateralEarthPressureMethod = LateralEarthPressureMethod.MIXED
     verification: bool = False
-    ec7se_visible: bool = False
     pile_load_option: bool = False
     pile_load_by_user: bool = False
     probabilistic: bool = False
     check_vertical_balance: bool = True
     trildens_calculation: bool = True
     diepwand_calculation: bool = False
     elastic_calculation: bool = True
@@ -119,35 +114,32 @@
 
 class Version(DSerieVersion):
     soil: int = _DEFAULT_SOIL_VERSION
     d__sheet_piling: int = _DEFAULT_SHEETPILING_VERSION
 
 
 class VersionExternals(DSeriesInlineMappedProperties):
-    dgscptipcalc____dll: str = "19.1.1.23469"
-    dgscptipui____dll: str = "19.1.1.23469"
+    dgscptipcalc____dll: str = "21.3.1.35380"
+    dgscptipui____dll: str = "21.3.1.35380"
 
 
 class Soil(DSeriesUnmappedNameProperties):
     name: constr(min_length=1, max_length=25) = "default soil"
     soilcolor: int = 9764853
     soilsoiltype: SoilTypeModulusSubgradeReaction = SoilTypeModulusSubgradeReaction.SAND
     soilgraintype: GrainType = GrainType.FINE
     soilgamdry: confloat(ge=0, le=100) = 0.01
     soilgamwet: confloat(ge=0, le=100) = 0.01
     soilrelativedensity: confloat(ge=0, le=100) = 0
     soilemodmenard: confloat(ge=0.01, le=1000000) = 0.01
     soilcohesion: confloat(ge=0, le=1000000000) = 0
     soilphi: confloat(ge=-89, le=89) = 0
     soildelta: confloat(ge=-80, le=89) = 0.00
-    soilcutop: float = 0  # fixed value
-    soilcubottom: float = 0  # fixed value
-    soilcubearingcapacityfactor: float = 4.10  # fixed value
+    soilisdeltaangleautomaticallycalculated: bool = False
     soilocr: confloat(ge=0, le=1000) = 1.00
-    soildrained: int = 0  # fixed value
     soilpermeabkx: confloat(ge=0.00000000001, le=1000000) = 0.0001
     soilstdcohesion: confloat(ge=0, le=100000000) = 0.00
     soilstdphi: confloat(ge=0, le=100000000) = 0.00
     soildistcohesion: DistributionType = DistributionType.NONE
     soildistphi: DistributionType = DistributionType.NONE
     soilla: confloat(ge=0, le=1000) = 0
     soilln: confloat(ge=0, le=1000) = 0.01
@@ -239,15 +231,14 @@
 
 
 class CalculationOptions(DSeriesStructure):
     # TODO these first values are not used for single pile
     calcfirststageinitial: bool = False
     calcminornodeson: bool = False
     calcreducedeltas: bool = False
-    calcempiricalfactorstresstype: int = 0  # fixed value
     inputcalculationtype: CalculationType = CalculationType.STANDARD
     isvibrationcalculation: bool = False
     allowableanchorforcecalculationtype: bool = False
     # available when c, phi , delta is selected for as a model
     calcautolambdason: bool = True
     # design sheet pile length calculation
     designstage: conint(ge=0) = 0
@@ -257,84 +248,80 @@
     designpilelengthnew: int = 1  # fixed value
     designtype: DesignType = DesignType.REPRESENTATIVE
     designeurocodepartialfactorset: PartialFactorSetEC = PartialFactorSetEC.DA1SET1
     designpartialfactorsetec7nadnl: PartialFactorSetEC7NADNL = (
         PartialFactorSetEC7NADNL.RC0
     )
     designec7nlmethod: PartialFactorCalculationType = PartialFactorCalculationType.METHODA
-    designpartialfactorsetec7nadb: PartialFactorSetEC7NADB = PartialFactorSetEC7NADB.SET1
     designec7bmethod: PartialFactorCalculationType = PartialFactorCalculationType.METHODA
+    designpartialfactorsetec7nadbe: PartialFactorSetEC7NADBE = (
+        PartialFactorSetEC7NADBE.SET1
+    )
+    designec7bemethod: PartialFactorCalculationType = PartialFactorCalculationType.METHODA
     designpartialfactorset: PartialFactorSetCUR = PartialFactorSetCUR.CLASSI
     designcurmethod: PartialFactorCalculationType = PartialFactorCalculationType.METHODA
-    designpartialfactorsetec7nadse: int = 0  # fixed value
-    designec7semethod: int = 0  # fixed value
     # verify sheet piling calculation
     verifytype: VerifyType = VerifyType.CUR
     eurocodepartialfactorset: PartialFactorSetVerifyEC = PartialFactorSetVerifyEC.DA1
     eurocodeoverallstability: bool = False
     ec7nlmethod: PartialFactorCalculationType = PartialFactorCalculationType.METHODA
     ec7nloverallpartialfactorset: PartialFactorSetEC7NADNL = PartialFactorSetEC7NADNL.RC0
     ec7nloverallanchorfactor: confloat(ge=0.001, le=1000) = 1
     ec7nadnloverallstability: bool = False
-    ec7boverallstability: bool = False
+    ec7beoverallstability: bool = False
+    ec7bemethod: PartialFactorCalculationType = PartialFactorCalculationType.METHODA
     nbmethod: PartialFactorCalculationType = PartialFactorCalculationType.METHODA
     curmethod: PartialFactorCalculationType = PartialFactorCalculationType.METHODA
     curoverallpartialfactorset: PartialFactorSetCUR = PartialFactorSetCUR.CLASSI
     curoverallanchorfactor: confloat(ge=0.001, le=1000) = 1
     curoverallstability: bool = False
-    ec7semethod: int = 0  # fixed value
-    ec7seoverallpartialfactorset: int = 0  # fixed value
-    ec7nadseoverallstability: int = 0  # fixed value
     # Characteristic Kranz Anchor Strength calculation
     curanchorforcestage: conint(ge=0) = 0
     # Overall stability calculation
     curstabilitystage: conint(ge=0) = 0
     overallstabilitytype: DesignType = DesignType.REPRESENTATIVE
+    stabilityexport: bool = False
     stabilityeurocodepartialfactorset: PartialFactorSetEC = PartialFactorSetEC.DA1SET1
     stabilityec7nlpartialfactorset: PartialFactorSetEC7NADNL = (
         PartialFactorSetEC7NADNL.RC0
     )
-    stabilityec7bpartialfactorset: PartialFactorSetEC7NADB = PartialFactorSetEC7NADB.SET1
+    stabilityec7bepartialfactorset: PartialFactorSetEC7NADBE = (
+        PartialFactorSetEC7NADBE.SET1
+    )
     stabilitycurpartialfactorset: PartialFactorSetCUR = PartialFactorSetCUR.CLASSI
-    stabilityec7separtialfactorset: int = 0  # fixed value
-    overallstabilitydrained: int = 1  # fixed value
 
     # These are all subgroups (key=value)
     partial_factors_eurocode_da1_set1: PartialFactorsEurocodeDa1Set1 = (
         PartialFactorsEurocodeDa1Set1()
     )
     partial_factors_eurocode_da1_set2: PartialFactorsEurocodeDa1Set2 = (
         PartialFactorsEurocodeDa1Set2()
     )
     partial_factors_eurocode_da2: PartialFactorsEurocodeDa2 = PartialFactorsEurocodeDa2()
     partial_factors_eurocode_da3: PartialFactorsEurocodeDa3 = PartialFactorsEurocodeDa3()
     partial_factors_ec7_nl_0: PartialFactorsEc7Nl0 = PartialFactorsEc7Nl0()
     partial_factors_ec7_nl_1: PartialFactorsEc7Nl1 = PartialFactorsEc7Nl1()
     partial_factors_ec7_nl_2: PartialFactorsEc7Nl2 = PartialFactorsEc7Nl2()
     partial_factors_ec7_nl_3: PartialFactorsEc7Nl3 = PartialFactorsEc7Nl3()
-    partial_factors_ec7_b_set1: PartialFactorsEc7BSet1 = PartialFactorsEc7BSet1()
-    partial_factors_ec7_b_set2: PartialFactorsEc7BSet2 = PartialFactorsEc7BSet2()
+    partial_factors_ec7_be_set1: PartialFactorsEc7BESet1 = PartialFactorsEc7BESet1()
+    partial_factors_ec7_be_set2: PartialFactorsEc7BESet2 = PartialFactorsEc7BESet2()
     partial_factors_cur_i: PartialFactorsCurI = PartialFactorsCurI()
     partial_factors_cur_ii: PartialFactorsCurIi = PartialFactorsCurIi()
     partial_factors_cur_iii: PartialFactorsCurIii = PartialFactorsCurIii()
-    partial_factors_ec7_se_vk1: PartialFactorsEc7SeVk1 = PartialFactorsEc7SeVk1()
-    partial_factors_ec7_se_vk2: PartialFactorsEc7SeVk2 = PartialFactorsEc7SeVk2()
-    partial_factors_ec7_se_vk3: PartialFactorsEc7SeVk3 = PartialFactorsEc7SeVk3()
 
 
 class SheetPileElement(DSeriesUnmappedNameProperties):
     name: constr(min_length=1, max_length=50) = _DEFAULT_SHEET_PILING_ELEMENT_NAME
     sheetpilingelementmaterialtype: SheetPilingElementMaterialType = (
         SheetPilingElementMaterialType.Steel
     )
     sheetpilingelementei: confloat(ge=0.001, le=1e12) = 100000
     sheetpilingelementwidth: confloat(ge=0, le=1000) = 1
     sheetpilingelementlevel: confloat(ge=-10000, le=10000) = -10
     sheetpilingelementheight: conint(ge=10, le=100000) = 400
-    sheetpilingelementcoatingarea: confloat(ge=0.01, le=10) = 1.35
     sheetpilingpilewidth: confloat(ge=0, le=100000) = 0
     sheetpilingelementsectionarea: conint(ge=10, le=100000) = 170
     sheetpilingelementresistingmoment: conint(ge=0, le=100000) = 0
     sheetpilingelementreductionfactorei: confloat(ge=0.01, le=10) = 1
     sheetpilingelementnote: constr(min_length=0, max_length=20) = ""
     sheetpilingelementmaxcharacteristicmoment: confloat(ge=0, le=100000) = 0
     sheetpilingelementmaxplasticcharacteristicmoment: confloat(ge=0, le=100000) = 0
@@ -534,17 +521,15 @@
 
     stagepartialfactorsetcur: PartialFactorSetCUR = PartialFactorSetCUR.UNKNOWN
     stageverify: int = 0
     stageanchorfactor: confloat(ge=0.001, le=1000) = 1
     stagepartialfactorsetec7nadnl: PartialFactorSetEC7NADNL = PartialFactorSetEC7NADNL.RC0
     stageverifyec7nadnl: int = 0
     stageanchorfactorec7nadnl: confloat(ge=0.001, le=1000) = 1
-    stageverifyec7nadb: int = 0
-    stagepartialfactorsetec7nadse: int = 0  # fixed value
-    stageverifyec7nadse: int = 0  # fixed value
+    stageverifyec7nadbe: int = 0
 
 
 class CalculationOptionsPerStage(DSeriesStructureCollection):
     """Representation of [CALCULATION OPTIONS PER STAGE] block."""
 
     stageoptions: List[StageOptions] = []
 
@@ -670,21 +655,32 @@
     supports: List[Support] = []
 
     @property
     def support_names(self) -> Set[str]:
         return {support.name for support in self.supports}
 
 
+class VibrationPosition(DSeriesNoParseSubStructure):
+    x: float
+    z: float
+
+
+class VibrationPositions(DSeriesNoParseSubStructure):
+    positions: List[VibrationPosition] = []
+
+
 class Water(DSeriesUnmappedNameProperties):
     unit_weight_of_water: float = 9.81
 
 
 class DSheetPilingInputStructure(DSeriesStructure):
     """Representation of complete .shi file."""
 
+    version: Version = Version()
+    version_externals: VersionExternals = VersionExternals()
     soil_collection: SoilCollection = SoilCollection()
     run_identification: str = 2 * "\n"
     model: Model = Model()
     cpt_list: str = cleandoc(
         """
         Count=0
         """
@@ -771,24 +767,25 @@
         CriteriaLimit1=0.010000
         CriteriaLimit2=0.010000
         ReliabilityStage=0
         """
     )
 
     """
-    When there are no anchors, struts, supports, or soil displacements in the model,
-    their respective blocks is not present in the .shi file.
+    When there are no anchors, struts, supports, vibration positions or soil displacements in the model,
+    their respective block is not present in the .shi file.
     """
     soil_displacements: Optional[str] = None
     rigid_supports: Union[str, SupportContainer, None] = None
     spring_supports: Union[str, SupportContainer, None] = None
     moments: Union[str, Moments, None] = None
     normal_forces: Union[str, NormalForces, None] = None
     anchors: Union[str, Anchors, None] = None
     struts: Union[str, Struts, None] = None
+    vibration_positions: Union[str, VibrationPositions, None] = None
 
     # Custom validator
     _validate_run_identification = make_newline_validator(
         "run_identification", req_newlines=REQ_RUN_LINES
     )
 
     @property
@@ -842,15 +839,17 @@
                 "stageanchorfactor": input_calc_options.anchor_factor,
             },
             VerifyType.EC7NL: {
                 "stagepartialfactorsetec7nadnl": input_calc_options.partial_factor_set,
                 "stageverifyec7nadnl": stage_id + 1,
                 "stageanchorfactorec7nadnl": input_calc_options.anchor_factor,
             },
-            VerifyType.EC7BE: {"stageverifyec7nadb": stage_id + 1},
+            VerifyType.EC7BE: {
+                "stageverifyec7nadbe": stage_id + 1,
+            },
         }
         stageoptions = StageOptions(
             **_map_external_to_internal_values[self.calculation_options.verifytype]
         )
         self.calculation_options_per_stage.stageoptions[stage_id] = stageoptions
 
     def set_curve_settings(self, curve_settings: CurveSettings) -> None:
@@ -1219,14 +1218,16 @@
     vertical_balance_per_layer: Optional[str]
 
 
 class OutputConstructionStage(DSeriesRepeatedGroupedProperties):
     anchor_data: Optional[AnchorData]
     hload_data: Optional[str]
     breuk_data: Optional[BreukData]
+    passive_side_data: Optional[str]
+    soil_collapse_data: Optional[str]
     moments_forces_displacements: Optional[MomentsForcesDisplacements]
     side: Optional[List[SideOutput]]
     uniform_load_data: Optional[str]
     horizontal_line_load_data: Optional[str]
     surcharge_data: Optional[str]
     normal_force_data: Optional[str]
     moment_data: Optional[str]
@@ -1258,114 +1259,91 @@
 class CurAnchorForceResults(DSheetpilingWithNumberOfRowsTable):
     curanchorforceresults: List[Dict[str, float]]
 
 
 class BaseVerificationStructureProperties(DSeriesRepeatedGroupedProperties):
     points_on_sheetpile: Optional[List[PointsOnSheetpile]]
     construction_stage: Optional[List[OutputConstructionStage]]
-    resume: Optional[Resume]
-    warning: Optional[str]
-    error: Optional[str]
-
-    # TODO Check how many optional variations exist
-    basis_step_of_step_9____1_per_anchor: Optional[str]
-    verify_anchor_force_step_9____1_based_on_step_6____5: Optional[str]
-    verify_anchor_force_step_9____1_based_on_step_6____3: Optional[str]
 
     @classmethod
     def get_list_field_names(cls) -> List[str]:
         return ["points_on_sheetpile", "construction_stage"]
 
 
-class VerifyAnchorForce(BaseVerificationStructureProperties):
-    anchor_number: Optional[int]
-    points_on_sheetpile: Optional[List[PointsOnSheetpile]]
-    construction_stage: Optional[List[OutputConstructionStage]]
-    resume: Optional[Resume]
-
-
-class VerifySheetpileData(DSeriesStructure):
-    verify_deformation: Optional[BaseVerificationStructureProperties]
-    verify_moment_low_angle_of_subgr_reac: Optional[BaseVerificationStructureProperties]
-    verify_moment_high_angle_of_subgr_reac: Optional[BaseVerificationStructureProperties]
-    verify_low_mod_with_alt_passive_waterlevel: Optional[
-        BaseVerificationStructureProperties
-    ]
-    verify_high_mod_with_alt_passive_waterlevel: Optional[
-        BaseVerificationStructureProperties
-    ]
-    verify_anchor_force: Optional[VerifyAnchorForce]
-    resume: Optional[Resume]
-    factors_for_verification: Optional[str]
-
-
 class DSheetPilingOutputStructure(DSeriesRepeatedGroupedProperties):
     @classmethod
     def get_list_field_names(cls) -> List[str]:
-        return ["verify_sheetpile_data", "points_on_sheetpile", "construction_stage"]
+        return ["points_on_sheetpile", "construction_stage"]
 
     @classmethod
     def parse_text(cls, text):
         return super().parse_text(text)
 
     calculation_type: str
 
-    # Sheetpile calculation
+    # General data
     sheet_pile_elements: Optional[str]
-    design_sheetpile_length: Optional[DesignSheetpileLength]
-    verify_sheetpile_data: Optional[List[VerifySheetpileData]]
+    calculated_displacements: Optional[str]
+
+    # Standard, Kranz and Reliability calculation
     points_on_sheetpile: Optional[List[PointsOnSheetpile]]
     construction_stage: Optional[List[OutputConstructionStage]]
 
-    # Vibration calculation
+    # Design Sheet Pile Length calculation
+    design_sheetpile_length: Optional[DesignSheetpileLength]
+
+    # Settlement by Vibration calculation
     settlement_by_vibration: Optional[str]
 
-    # Verification calculation
-    # TODO Split further based on A/B grouping
+    # Verify calculation including Overall Stability calculation
     overall_partial_factor_set: Optional[str]
     factors_for_overall_stability: Optional[str]
     overall_stability_results: Optional[str]
 
-    calculation_overview: Optional[str]
-    number_of_verifications: Optional[str]
-    maximum_moment_effect_included: Optional[str]
-
-    eurocode2: Optional[str]
-    eurocode3: Optional[str]
-    eurocode1_set1: Optional[str]
-    eurocode1_set2: Optional[str]
-    eurocode_belgie_set2: Optional[str]
-    eurocode_belgie_set1: Optional[str]
+    # Verify calculation according to CUR or EC7-NL with method B
+    factors_for_verification: Optional[str]
+
+    # Verify calculation according to CUR or EC7-NL
+    verify_step_6____5_serviceability_limit_state: Optional[BaseVerificationStructureProperties]
+    verify_step_6____5_multiplied_by_factor: Optional[BaseVerificationStructureProperties]
+    verify_step_6____1_low_modulus_of_subgrade_reaction_and_high_passive_water_level: Optional[
+        BaseVerificationStructureProperties]
+    verify_step_6____2_high_modulus_of_subgrade_reaction_and_high_passive_water_level: Optional[
+        BaseVerificationStructureProperties]
+    verify_step_6____3_low_modulus_of_subgrade_reaction_and_low_passive_water_level: Optional[
+        BaseVerificationStructureProperties]
+    verify_step_6____4_high_modulus_of_subgrade_reaction_and_low_passive_water_level: Optional[
+        BaseVerificationStructureProperties]
     cur_anchor_force_results: Optional[CurAnchorForceResults]
-    warning_list: Optional[str]
-    warning: Optional[str]
-    error: Optional[str]
 
-    calculated_displacements: Optional[str]
+    # Verify calculation according to EC7-BE or EC7-General
+    verify_deformation_serviceability_limit_state: Optional[BaseVerificationStructureProperties]
+    eurocode_1_set_1: Optional[BaseVerificationStructureProperties]
+    eurocode_1_set_2: Optional[BaseVerificationStructureProperties]
+    eurocode_2: Optional[BaseVerificationStructureProperties]
+    eurocode_3: Optional[BaseVerificationStructureProperties]
+    eurocode_belgium_set_1: Optional[BaseVerificationStructureProperties]
+    eurocode_belgium_set_2: Optional[BaseVerificationStructureProperties]
+
+    # Kranz calculation
     angles_kranz_calculation: Optional[str]
     kranz_calculation: Optional[str]
+    kranz_diagram_results: Optional[str]
 
-    # Verifications, duplicated for all verifications.
-    verify_deformation: Optional[BaseVerificationStructureProperties]
-    verify_moment_low_angle_of_subgr_reac: Optional[BaseVerificationStructureProperties]
-    verify_moment_high_angle_of_subgr_reac: Optional[BaseVerificationStructureProperties]
-    verify_low_mod_with_alt_passive_waterlevel: Optional[
-        BaseVerificationStructureProperties
-    ]
-    verify_high_mod_with_alt_passive_waterlevel: Optional[
-        BaseVerificationStructureProperties
-    ]
-    verify_anchor_force: Optional[BaseVerificationStructureProperties]
+    # Resumes
     resume: Optional[Resume]
-    factors_for_verification: Optional[str]
+    anchors_and_struts_resume: Optional[str]
+    supports_resume: Optional[str]
+    maximum_anchor_force: Optional[str]
+    maximum_summary_results: Optional[str]
+    warnings: Optional[str]
+    errors: Optional[str]
 
 
 class DSheetPilingStructure(DSeriesPilingParserStructure):
-    version: Version = Version()
-    version_externals: VersionExternals = VersionExternals()
     input_data: DSheetPilingInputStructure = DSheetPilingInputStructure()
     output_data: Optional[DSheetPilingOutputStructure] = None
 
     @property
     def is_valid(self) -> bool:
         return self.input_data.is_valid
```

### Comparing `d_geolib-0.5.1/geolib/models/dsheetpiling/loads.py` & `d_geolib-0.6.0/geolib/models/dsheetpiling/loads.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsheetpiling/profiles.py` & `d_geolib-0.6.0/geolib/models/dsheetpiling/profiles.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsheetpiling/serializer.py` & `d_geolib-0.6.0/geolib/models/dsheetpiling/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsheetpiling/settings.py` & `d_geolib-0.6.0/geolib/models/dsheetpiling/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from enum import Enum, IntEnum
 
-from pydantic import conint
-
 from geolib.models import BaseDataClass
+from pydantic import conint
 
 
 class LateralEarthPressureMethod(IntEnum):
     """The method for input of the lateral earth pressure ratio"""
 
     MIXED = 2
     KA_KO_KP = 0
@@ -115,26 +114,28 @@
 
 
 class PartialFactorSetEC7NADNL(IntEnum):
     RC0 = 0
     RC1 = 1
     RC2 = 2
     RC3 = 3
+    SLS = 4
 
 
-class PartialFactorSetEC7NADB(IntEnum):
+class PartialFactorSetEC7NADBE(IntEnum):
     SET1 = 0
     SET2 = 1
 
 
 class PartialFactorSetCUR(IntEnum):
     UNKNOWN = -1
     CLASSI = 0
     CLASSII = 1
     CLASSIII = 2
+    SLS = 3
 
 
 class PartialFactorCalculationType(IntEnum):
     METHODA = 0
     METHODB = 1
```

### Comparing `d_geolib-0.5.1/geolib/models/dsheetpiling/supports.py` & `d_geolib-0.6.0/geolib/models/dsheetpiling/supports.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsheetpiling/surface.py` & `d_geolib-0.6.0/geolib/models/dsheetpiling/surface.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dsheetpiling/templates/input.shi.j2` & `d_geolib-0.6.0/geolib/models/dsheetpiling/templates/input.shi.j2`

 * *Files 17% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 DATE       : {{ timestamp.strftime('%d-%m-%Y') }}
 TIME       : {{ timestamp.strftime('%H:%M:%S') }}
 FILENAME   : {{ output_fn }}
 CREATED BY : GEOLib version {{ glversion }}
 
 ==========================    BEGINNING OF DATA     ==========================
+[INPUT DATA]
 [VERSION]
 Soil={{ version.soil }}
 D-Sheet Piling={{ version.d__sheet_piling }}
 [END OF VERSION]
 
 [VERSION EXTERNALS]
 DGSCPTipCalc.dll={{ version_externals.dgscptipcalc____dll }}
 DGSCPTipUI.dll={{ version_externals.dgscptipui____dll }}
 [END OF VERSION EXTERNALS]
 
-[INPUT DATA]
 [SOIL COLLECTION]
     {{ soil_collection.soil|length }} = number of items
 {% for soil in soil_collection.soil %}
 [SOIL]
 {{ soil.name }}
 SoilColor={{ soil.soilcolor }}
 SoilSoilType={{ soil.soilsoiltype.value }}
@@ -30,19 +30,16 @@
 SoilGamDry={{ soil.soilgamdry }}
 SoilGamWet={{ soil.soilgamwet }}
 SoilRelativeDensity={{ soil.soilrelativedensity }}
 SoilEModMenard={{ soil.soilemodmenard }}
 SoilCohesion={{ soil.soilcohesion }}
 SoilPhi={{ soil.soilphi }}
 SoilDelta={{ soil.soildelta }}
-SoilCuTop={{ soil.soilcutop }}
-SoilCuBottom={{ soil.soilcubottom }}
-SoilCuBearingCapacityFactor={{ soil.soilcubearingcapacityfactor }}
+SoilIsDeltaAngleAutomaticallyCalculated={{ soil.soilisdeltaangleautomaticallycalculated | int}}
 SoilOCR={{ soil.soilocr }}
-SoilDrained={{ soil.soildrained }}
 SoilPermeabKx={{ soil.soilpermeabkx }}
 SoilStdCohesion={{ soil.soilstdcohesion}}
 SoilStdPhi={{ soil.soilstdphi }}
 SoilDistCohesion={{ soil.soildistcohesion.value  }}
 SoilDistPhi={{ soil.soildistphi.value  }}
 SoilLa={{ soil.soilla }}
 SoilLn={{ soil.soilln }}
@@ -82,15 +79,14 @@
 [END OF RUN IDENTIFICATION]
 
 [MODEL]
 {% if model is mapping -%}
 {{ model.model.value }} : {{ {0: 'Sheet piling', 1: 'Single pile'}[model.model.value]}}
 {{ model.method.value }} : {{ {0: 'Ka, Ko, Kp soil parameters', 1: 'C, phi, delta soil parameters', 2: 'Mixed'}[model.method.value]}}
 {{ model.verification | int }} : Verification = {{ model.verification | string | upper }}
-{{ model.ec7se_visible | int }} : EC7-SE visible = {{ model.ec7se_visible | string | upper }}
 {% if not model.pile_load_option %}
 {{ model.pile_load_option | int }} : Pile loaded by forces
 {{ model.pile_load_by_user | int }} : Pile loaded by user defined soil displacements
 {% elif model.pile_load_option and not model.pile_load_by_user %}
 {{ model.pile_load_option | int }} : Pile loaded by user defined soil displacements
 {{ model.pile_load_by_user | int }} : Pile loaded by user defined soil displacements
 {% elif model.pile_load_option and model.pile_load_by_user %}
@@ -122,15 +118,14 @@
 [SHEET PILING ELEMENT]
 {{ element.name }}
 SheetPilingElementMaterialType={{ element.sheetpilingelementmaterialtype.value }}
 SheetPilingElementEI={{ "%E"|format(element.sheetpilingelementei) }}
 SheetPilingElementWidth={{ "%0.2f"|format(element.sheetpilingelementwidth) }}
 SheetPilingElementLevel={{ "%0.2f"|format(element.sheetpilingelementlevel) }}
 SheetPilingElementHeight={{ element.sheetpilingelementheight|int }}
-SheetPilingElementCoatingArea={{ element.sheetpilingelementcoatingarea }}
 SheetPilingPileWidth={{ element.sheetpilingpilewidth }}
 SheetPilingElementSectionArea={{ element.sheetpilingelementsectionarea }}
 SheetPilingElementResistingMoment={{ element.sheetpilingelementresistingmoment }}
 SheetPilingElementReductionFactorEI={{ "%0.2f"|format(element.sheetpilingelementreductionfactorei) }}
 SheetPilingElementNote={{ element.sheetpilingelementnote }}
 SheetPilingElementMaxCharacteristicMoment={{ "%0.2f"|format(element.sheetpilingelementmaxcharacteristicmoment) }}
 SheetPilingElementMaxPlasticCharacteristicMoment={{ "%0.2f"|format(element.sheetpilingelementmaxplasticcharacteristicmoment) }}
@@ -325,14 +320,27 @@
   {{ loop.index }} {{"%11.2f"|format(load.force_at_sheet_pile_top)}} {{"%11.2f"|format(load.force_at_surface_level_left_side)}} {{"%11.2f"|format(load.force_at_surface_level_right_side)}} {{"%11.2f"|format(load.force_at_sheet_pile_toe)}} {{load.duration_type.value}} {{load.load_type.value}} {{load.name}}
 {% endfor %}
 {% else %}
 {{ normal_forces }}
 {% endif %}
 [END OF NORMAL FORCES]
 {% endif %}
+{% if vibration_positions %}
+
+[VIBRATION POSITIONS]
+{% if vibration_positions is mapping %}
+  {{ vibration_positions.items | length }} : Number of items
+{% for position in vibration_positions.positions %}
+  {{"%5.3f"|format(position.x)}} {{"%5.3f"|format(position.z)}}
+{% endfor %}
+{% else %}
+{{ vibration_positions }}
+{% endif %}
+[END OF VIBRATION POSITIONS]
+{% endif %}
 
 [WATER]
  {{ water.unit_weight_of_water }} Unit weight of water
 [END OF WATER]
 
 [EARTH QUAKE]
 {{ earth_quake }}
@@ -465,242 +473,188 @@
 [STAGE]
 StagePartialFactorSetCUR={{ stage.stagepartialfactorsetcur.value }}
 StageVerify={{ stage.stageverify }}
 StageAnchorFactor={{ stage.stageanchorfactor }}
 StagePartialFactorSetEC7NADNL={{ stage.stagepartialfactorsetec7nadnl.value }}
 StageVerifyEC7NADNL={{ stage.stageverifyec7nadnl }}
 StageAnchorFactorEC7NADNL={{ stage.stageanchorfactorec7nadnl }}
-StageVerifyEC7NADB={{ stage.stageverifyec7nadb }}
-StagePartialFactorSetEC7NADSE={{ stage.stagepartialfactorsetec7nadse }}
-StageVerifyEC7NADSE={{ stage.stageverifyec7nadse }}
+StageVerifyEC7NADBE={{ stage.stageverifyec7nadbe }}
 [END OF STAGE]
 {% endfor %}
 {% else %}
 {{ calculation_options_per_stage }}
 {% endif %}
 [END OF CALCULATION OPTIONS PER STAGE]
 
 [CALCULATION OPTIONS]
 {% if calculation_options is mapping %}
 CalcFirstStageInitial={{ calculation_options.calcfirststageinitial|int }}
 CalcMinorNodesOn={{ calculation_options.calcminornodeson|int }}
 CalcReduceDeltas={{ calculation_options.calcreducedeltas|int }}
-CalcEmpiricalFactorStressType={{ calculation_options.calcempiricalfactorstresstype }}
 InputCalculationType={{ calculation_options.inputcalculationtype.value }}
-IsVibrationCalculation={{ calculation_options.isvibrationcalculation|int}}
+IsVibrationCalculation={{ calculation_options.isvibrationcalculation|int }}
 AllowableAnchorForceCalculationType={{ calculation_options.allowableanchorforcecalculationtype|int }}
-CalcAutoLambdasOn={{ calculation_options.calcautolambdason|int}}
+CalcAutoLambdasOn={{ calculation_options.calcautolambdason|int }}
 DesignStage={{ calculation_options.designstage }}
 DesignPileLengthFrom={{ calculation_options.designpilelengthfrom }}
 DesignPileLengthTo={{ calculation_options.designpilelengthto }}
 DesignPileLengthDecrement={{ calculation_options.designpilelengthdecrement }}
 DesignPileLengthNew={{ calculation_options.designpilelengthnew }}
 DesignType={{ calculation_options.designtype.value }}
 DesignEuroCodePartialFactorSet={{ calculation_options.designeurocodepartialfactorset.value }}
 DesignPartialFactorSetEC7NADNL={{ calculation_options.designpartialfactorsetec7nadnl.value }}
 DesignEC7NLMethod={{ calculation_options.designec7nlmethod.value }}
-DesignPartialFactorSetEC7NADB={{ calculation_options.designpartialfactorsetec7nadb.value }}
-DesignEC7BMethod={{ calculation_options.designec7bmethod.value }}
+DesignPartialFactorSetEC7NADBE={{ calculation_options.designpartialfactorsetec7nadbe.value }}
+DesignEC7BEMethod={{ calculation_options.designec7bemethod.value }}
 DesignPartialFactorSet={{ calculation_options.designpartialfactorset.value }}
 DesignCURMethod={{ calculation_options.designcurmethod.value }}
-DesignPartialFactorSetEC7NADSE={{ calculation_options.designpartialfactorsetec7nadse }}
-DesignEC7SEMethod={{ calculation_options.designec7semethod }}
 VerifyType={{ calculation_options.verifytype.value }}
 EuroCodePartialFactorSet={{ calculation_options.eurocodepartialfactorset.value }}
 EuroCodeOverallStability={{ calculation_options.eurocodeoverallstability|int }}
 EC7NLMethod={{ calculation_options.ec7nlmethod.value }}
 EC7NLOverallPartialFactorSet={{ calculation_options.ec7nloverallpartialfactorset.value }}
 EC7NLOverallAnchorFactor={{ calculation_options.ec7nloverallanchorfactor }}
 EC7NADNLOverallStability={{ calculation_options.ec7nadnloverallstability|int }}
-EC7BOverallStability={{ calculation_options.ec7boverallstability|int }}
-NBMethod={{ calculation_options.nbmethod.value}}
+EC7BEOverallStability={{ calculation_options.ec7beoverallstability|int }}
+EC7BEMethod={{ calculation_options.ec7bemethod.value}}
 CURMethod={{ calculation_options.curmethod.value }}
 CUROverallPartialFactorSet={{ calculation_options.curoverallpartialfactorset.value }}
 CUROverallAnchorFactor={{ calculation_options.curoverallanchorfactor }}
 CUROverallStability={{ calculation_options.curoverallstability|int }}
-EC7SEMethod={{ calculation_options.ec7semethod }}
-EC7SEOverallPartialFactorSet={{ calculation_options.ec7seoverallpartialfactorset }}
-EC7NADSEOverallStability={{ calculation_options.ec7nadseoverallstability }}
 CURAnchorForceStage={{ calculation_options.curanchorforcestage }}
 CURStabilityStage={{ calculation_options.curstabilitystage }}
 OverallStabilityType={{ calculation_options.overallstabilitytype.value }}
+StabilityExport={{ calculation_options.stabilityexport|int }}
 StabilityEuroCodePartialFactorSet={{ calculation_options.stabilityeurocodepartialfactorset.value }}
 StabilityEC7NLPartialFactorSet={{ calculation_options.stabilityec7nlpartialfactorset.value }}
-StabilityEC7BPartialFactorSet={{ calculation_options.stabilityec7bpartialfactorset.value }}
+StabilityEC7BEPartialFactorSet={{ calculation_options.stabilityec7bepartialfactorset.value }}
 StabilityCURPartialFactorSet={{ calculation_options.stabilitycurpartialfactorset.value }}
-StabilityEC7SEPartialFactorSet={{ calculation_options.stabilityec7separtialfactorset }}
-OverallStabilityDrained={{ calculation_options.overallstabilitydrained }}
 {% else %}
 {{ calculation_options }}
 {% endif %}
 [PARTIAL FACTORS EUROCODE DA1 SET1]
-SafetyFactorGammaD=1.00
-SafetyFactorEta=1.00
 LoadFactorPermUnfav=1.000
 LoadFactorPermFav=1.000
 LoadFactorVarUnfav=1.000
 LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.000
-LoadFactorVarUnfavMultiply=1.000
-LoadFactorPermUnfavCalc=0.000
-LoadFactorVarUnfavCalc=0.000
 ConstructLoadFactorPermFav=1.000
-ConstructLoadFactorVarFav=1.000
-ConstructLoadFactorPermUnfavMultiply=1.000
-ConstructLoadFactorVarUnfavMultiply=1.000
+ConstructLoadFactorVarFav=0.000
 ConstructLoadFactorPermUnfavCalc=1.000
 ConstructLoadFactorVarUnfavCalc=1.000
 EffectFactor=1.350
-EffectFactorVarUnfav=1.111
+EffectFactorVarUnfav=1.100
 MaterialFactorCohesion=1.000
-MaterialFactorUndrainedShearStrength=1.000
 MaterialFactorTgPhi=1.000
 MaterialFactorSubgradeReaction=1.000
 ResistanceFactor=1.000
 GeometryIncRetainingHeight=10.00
 GeometryMaxIncRetainingHeight=0.50
 GeometryDeltaPassiveSurfaceLevel=0.00
 GeometryDeltaPassivePhreaticLine=0.00
 GeometryDeltaActivePhreaticLine=0.00
 OverallStabilityFactorDrivingMoment=1.000
 OverallStabilityFactorCohesion=1.000
 OverallStabilityFactorTgPhi=1.000
 OverallStabilityFactorUnitWeight=1.000
 FactorRepValuesMDPmax=0.000
-VerticalBalanceGammaMb=1.000
+VerticalBalanceGammaMb=1.250
 [END OF PARTIAL FACTORS EUROCODE DA1 SET1]
 [PARTIAL FACTORS EUROCODE DA1 SET2]
-SafetyFactorGammaD=1.00
-SafetyFactorEta=1.00
 LoadFactorPermUnfav=1.000
 LoadFactorPermFav=1.000
 LoadFactorVarUnfav=1.300
 LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.000
-LoadFactorVarUnfavMultiply=1.000
-LoadFactorPermUnfavCalc=0.000
-LoadFactorVarUnfavCalc=0.000
 ConstructLoadFactorPermFav=1.000
-ConstructLoadFactorVarFav=1.000
-ConstructLoadFactorPermUnfavMultiply=1.000
-ConstructLoadFactorVarUnfavMultiply=1.000
+ConstructLoadFactorVarFav=0.000
 ConstructLoadFactorPermUnfavCalc=1.000
 ConstructLoadFactorVarUnfavCalc=1.000
 EffectFactor=1.000
 EffectFactorVarUnfav=1.000
 MaterialFactorCohesion=1.250
-MaterialFactorUndrainedShearStrength=1.000
 MaterialFactorTgPhi=1.250
 MaterialFactorSubgradeReaction=1.000
 ResistanceFactor=1.000
 GeometryIncRetainingHeight=10.00
 GeometryMaxIncRetainingHeight=0.50
 GeometryDeltaPassiveSurfaceLevel=0.00
 GeometryDeltaPassivePhreaticLine=0.00
 GeometryDeltaActivePhreaticLine=0.00
 OverallStabilityFactorDrivingMoment=1.000
-OverallStabilityFactorCohesion=1.250
-OverallStabilityFactorTgPhi=1.250
+OverallStabilityFactorCohesion=1.000
+OverallStabilityFactorTgPhi=1.000
 OverallStabilityFactorUnitWeight=1.000
 FactorRepValuesMDPmax=0.000
-VerticalBalanceGammaMb=1.300
+VerticalBalanceGammaMb=1.250
 [END OF PARTIAL FACTORS EUROCODE DA1 SET2]
 [PARTIAL FACTORS EUROCODE DA2]
-SafetyFactorGammaD=1.00
-SafetyFactorEta=1.00
 LoadFactorPermUnfav=1.000
 LoadFactorPermFav=1.000
 LoadFactorVarUnfav=1.000
 LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.000
-LoadFactorVarUnfavMultiply=1.000
-LoadFactorPermUnfavCalc=0.000
-LoadFactorVarUnfavCalc=0.000
 ConstructLoadFactorPermFav=1.000
-ConstructLoadFactorVarFav=1.000
-ConstructLoadFactorPermUnfavMultiply=1.000
-ConstructLoadFactorVarUnfavMultiply=1.000
+ConstructLoadFactorVarFav=0.000
 ConstructLoadFactorPermUnfavCalc=1.000
 ConstructLoadFactorVarUnfavCalc=1.000
 EffectFactor=1.350
-EffectFactorVarUnfav=1.111
+EffectFactorVarUnfav=1.100
 MaterialFactorCohesion=1.000
-MaterialFactorUndrainedShearStrength=1.000
 MaterialFactorTgPhi=1.000
 MaterialFactorSubgradeReaction=1.000
 ResistanceFactor=1.400
 GeometryIncRetainingHeight=10.00
 GeometryMaxIncRetainingHeight=0.50
 GeometryDeltaPassiveSurfaceLevel=0.00
 GeometryDeltaPassivePhreaticLine=0.00
 GeometryDeltaActivePhreaticLine=0.00
 OverallStabilityFactorDrivingMoment=1.000
 OverallStabilityFactorCohesion=1.000
 OverallStabilityFactorTgPhi=1.000
 OverallStabilityFactorUnitWeight=1.000
 FactorRepValuesMDPmax=0.000
-VerticalBalanceGammaMb=1.100
+VerticalBalanceGammaMb=1.250
 [END OF PARTIAL FACTORS EUROCODE DA2]
 [PARTIAL FACTORS EUROCODE DA3]
-SafetyFactorGammaD=1.00
-SafetyFactorEta=1.00
 LoadFactorPermUnfav=1.000
 LoadFactorPermFav=1.000
 LoadFactorVarUnfav=1.300
 LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.000
-LoadFactorVarUnfavMultiply=1.000
-LoadFactorPermUnfavCalc=0.000
-LoadFactorVarUnfavCalc=0.000
 ConstructLoadFactorPermFav=1.000
-ConstructLoadFactorVarFav=1.000
-ConstructLoadFactorPermUnfavMultiply=1.000
-ConstructLoadFactorVarUnfavMultiply=1.000
-ConstructLoadFactorPermUnfavCalc=1.350
-ConstructLoadFactorVarUnfavCalc=1.500
+ConstructLoadFactorVarFav=0.000
+ConstructLoadFactorPermUnfavCalc=1.000
+ConstructLoadFactorVarUnfavCalc=1.000
 EffectFactor=1.000
 EffectFactorVarUnfav=1.000
 MaterialFactorCohesion=1.250
-MaterialFactorUndrainedShearStrength=1.000
 MaterialFactorTgPhi=1.250
 MaterialFactorSubgradeReaction=1.000
 ResistanceFactor=1.000
 GeometryIncRetainingHeight=10.00
 GeometryMaxIncRetainingHeight=0.50
 GeometryDeltaPassiveSurfaceLevel=0.00
 GeometryDeltaPassivePhreaticLine=0.00
 GeometryDeltaActivePhreaticLine=0.00
 OverallStabilityFactorDrivingMoment=1.000
-OverallStabilityFactorCohesion=1.250
-OverallStabilityFactorTgPhi=1.250
+OverallStabilityFactorCohesion=1.000
+OverallStabilityFactorTgPhi=1.000
 OverallStabilityFactorUnitWeight=1.000
 FactorRepValuesMDPmax=0.000
-VerticalBalanceGammaMb=1.000
+VerticalBalanceGammaMb=1.250
 [END OF PARTIAL FACTORS EUROCODE DA3]
 [PARTIAL FACTORS EC7 NL 0]
-SafetyFactorGammaD=1.00
-SafetyFactorEta=1.00
 LoadFactorPermUnfav=1.000
 LoadFactorPermFav=1.000
 LoadFactorVarUnfav=1.000
 LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.000
-LoadFactorVarUnfavMultiply=1.000
-LoadFactorPermUnfavCalc=0.000
-LoadFactorVarUnfavCalc=0.000
 ConstructLoadFactorPermFav=1.000
-ConstructLoadFactorVarFav=1.000
-ConstructLoadFactorPermUnfavMultiply=1.000
-ConstructLoadFactorVarUnfavMultiply=1.000
+ConstructLoadFactorVarFav=0.000
 ConstructLoadFactorPermUnfavCalc=1.000
 ConstructLoadFactorVarUnfavCalc=1.000
 EffectFactor=1.000
 EffectFactorVarUnfav=1.000
 MaterialFactorCohesion=1.000
-MaterialFactorUndrainedShearStrength=1.000
 MaterialFactorTgPhi=1.050
 MaterialFactorSubgradeReaction=1.300
 ResistanceFactor=1.000
 GeometryIncRetainingHeight=10.00
 GeometryMaxIncRetainingHeight=0.50
 GeometryDeltaPassiveSurfaceLevel=0.00
 GeometryDeltaPassivePhreaticLine=0.15
@@ -709,409 +663,229 @@
 OverallStabilityFactorCohesion=1.300
 OverallStabilityFactorTgPhi=1.200
 OverallStabilityFactorUnitWeight=1.000
 FactorRepValuesMDPmax=1.200
 VerticalBalanceGammaMb=1.200
 [END OF PARTIAL FACTORS EC7 NL 0]
 [PARTIAL FACTORS EC7 NL 1]
-SafetyFactorGammaD=1.00
-SafetyFactorEta=1.00
 LoadFactorPermUnfav=1.000
 LoadFactorPermFav=1.000
 LoadFactorVarUnfav=1.000
 LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.000
-LoadFactorVarUnfavMultiply=1.000
-LoadFactorPermUnfavCalc=0.000
-LoadFactorVarUnfavCalc=0.000
-ConstructLoadFactorPermFav=0.900
-ConstructLoadFactorVarFav=1.000
-ConstructLoadFactorPermUnfavMultiply=1.000
-ConstructLoadFactorVarUnfavMultiply=1.000
-ConstructLoadFactorPermUnfavCalc=1.215
-ConstructLoadFactorVarUnfavCalc=1.350
+ConstructLoadFactorPermFav=1.000
+ConstructLoadFactorVarFav=0.000
+ConstructLoadFactorPermUnfavCalc=1.000
+ConstructLoadFactorVarUnfavCalc=1.000
 EffectFactor=1.000
 EffectFactorVarUnfav=1.000
 MaterialFactorCohesion=1.150
-MaterialFactorUndrainedShearStrength=1.000
 MaterialFactorTgPhi=1.150
 MaterialFactorSubgradeReaction=1.300
 ResistanceFactor=1.000
 GeometryIncRetainingHeight=10.00
 GeometryMaxIncRetainingHeight=0.50
 GeometryDeltaPassiveSurfaceLevel=0.00
 GeometryDeltaPassivePhreaticLine=0.20
 GeometryDeltaActivePhreaticLine=0.05
 OverallStabilityFactorDrivingMoment=1.000
 OverallStabilityFactorCohesion=1.300
 OverallStabilityFactorTgPhi=1.200
 OverallStabilityFactorUnitWeight=1.000
 FactorRepValuesMDPmax=1.200
-VerticalBalanceGammaMb=1.200
+VerticalBalanceGammaMb=1.250
 [END OF PARTIAL FACTORS EC7 NL 1]
 [PARTIAL FACTORS EC7 NL 2]
-SafetyFactorGammaD=1.00
-SafetyFactorEta=1.00
 LoadFactorPermUnfav=1.000
 LoadFactorPermFav=1.000
-LoadFactorVarUnfav=1.100
+LoadFactorVarUnfav=1.000
 LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.000
-LoadFactorVarUnfavMultiply=1.000
-LoadFactorPermUnfavCalc=0.000
-LoadFactorVarUnfavCalc=0.000
-ConstructLoadFactorPermFav=0.900
-ConstructLoadFactorVarFav=1.000
-ConstructLoadFactorPermUnfavMultiply=1.000
-ConstructLoadFactorVarUnfavMultiply=1.000
-ConstructLoadFactorPermUnfavCalc=1.350
-ConstructLoadFactorVarUnfavCalc=1.500
+ConstructLoadFactorPermFav=1.000
+ConstructLoadFactorVarFav=0.000
+ConstructLoadFactorPermUnfavCalc=1.000
+ConstructLoadFactorVarUnfavCalc=1.000
 EffectFactor=1.000
 EffectFactorVarUnfav=1.000
 MaterialFactorCohesion=1.250
-MaterialFactorUndrainedShearStrength=1.000
 MaterialFactorTgPhi=1.175
 MaterialFactorSubgradeReaction=1.300
 ResistanceFactor=1.000
 GeometryIncRetainingHeight=10.00
 GeometryMaxIncRetainingHeight=0.50
 GeometryDeltaPassiveSurfaceLevel=0.00
 GeometryDeltaPassivePhreaticLine=0.25
 GeometryDeltaActivePhreaticLine=0.05
 OverallStabilityFactorDrivingMoment=1.000
 OverallStabilityFactorCohesion=1.450
 OverallStabilityFactorTgPhi=1.250
 OverallStabilityFactorUnitWeight=1.000
 FactorRepValuesMDPmax=1.200
-VerticalBalanceGammaMb=1.200
+VerticalBalanceGammaMb=1.250
 [END OF PARTIAL FACTORS EC7 NL 2]
 [PARTIAL FACTORS EC7 NL 3]
-SafetyFactorGammaD=1.00
-SafetyFactorEta=1.00
 LoadFactorPermUnfav=1.000
 LoadFactorPermFav=1.000
 LoadFactorVarUnfav=1.250
 LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.000
-LoadFactorVarUnfavMultiply=1.000
-LoadFactorPermUnfavCalc=0.000
-LoadFactorVarUnfavCalc=0.000
-ConstructLoadFactorPermFav=0.900
-ConstructLoadFactorVarFav=1.000
-ConstructLoadFactorPermUnfavMultiply=1.000
-ConstructLoadFactorVarUnfavMultiply=1.000
-ConstructLoadFactorPermUnfavCalc=1.485
-ConstructLoadFactorVarUnfavCalc=1.650
+ConstructLoadFactorPermFav=1.000
+ConstructLoadFactorVarFav=0.000
+ConstructLoadFactorPermUnfavCalc=1.000
+ConstructLoadFactorVarUnfavCalc=1.000
 EffectFactor=1.000
 EffectFactorVarUnfav=1.000
 MaterialFactorCohesion=1.400
-MaterialFactorUndrainedShearStrength=1.000
 MaterialFactorTgPhi=1.200
 MaterialFactorSubgradeReaction=1.300
 ResistanceFactor=1.000
 GeometryIncRetainingHeight=10.00
 GeometryMaxIncRetainingHeight=0.50
 GeometryDeltaPassiveSurfaceLevel=0.00
 GeometryDeltaPassivePhreaticLine=0.25
 GeometryDeltaActivePhreaticLine=0.05
 OverallStabilityFactorDrivingMoment=1.000
 OverallStabilityFactorCohesion=1.600
 OverallStabilityFactorTgPhi=1.300
 OverallStabilityFactorUnitWeight=1.000
 FactorRepValuesMDPmax=1.350
-VerticalBalanceGammaMb=1.200
+VerticalBalanceGammaMb=1.250
 [END OF PARTIAL FACTORS EC7 NL 3]
-[PARTIAL FACTORS EC7 B SET1]
-SafetyFactorGammaD=1.00
-SafetyFactorEta=1.00
+[PARTIAL FACTORS EC7 BE SET1]
 LoadFactorPermUnfav=1.000
 LoadFactorPermFav=1.000
 LoadFactorVarUnfav=1.000
 LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.000
-LoadFactorVarUnfavMultiply=1.000
-LoadFactorPermUnfavCalc=0.000
-LoadFactorVarUnfavCalc=0.000
 ConstructLoadFactorPermFav=1.000
-ConstructLoadFactorVarFav=1.000
-ConstructLoadFactorPermUnfavMultiply=1.000
-ConstructLoadFactorVarUnfavMultiply=1.000
+ConstructLoadFactorVarFav=0.000
 ConstructLoadFactorPermUnfavCalc=1.000
 ConstructLoadFactorVarUnfavCalc=1.000
 EffectFactor=1.350
-EffectFactorVarUnfav=1.111
+EffectFactorVarUnfav=1.100
 MaterialFactorCohesion=1.000
-MaterialFactorUndrainedShearStrength=1.000
 MaterialFactorTgPhi=1.000
 MaterialFactorSubgradeReaction=1.000
 ResistanceFactor=1.000
 GeometryIncRetainingHeight=10.00
 GeometryMaxIncRetainingHeight=0.50
 GeometryDeltaPassiveSurfaceLevel=0.00
 GeometryDeltaPassivePhreaticLine=0.00
 GeometryDeltaActivePhreaticLine=0.00
 OverallStabilityFactorDrivingMoment=1.000
 OverallStabilityFactorCohesion=1.000
 OverallStabilityFactorTgPhi=1.000
 OverallStabilityFactorUnitWeight=1.000
 FactorRepValuesMDPmax=0.000
-VerticalBalanceGammaMb=1.000
-[END OF PARTIAL FACTORS EC7 B SET1]
-[PARTIAL FACTORS EC7 B SET2]
-SafetyFactorGammaD=1.00
-SafetyFactorEta=1.00
+VerticalBalanceGammaMb=1.200
+[END OF PARTIAL FACTORS EC7 BE SET1]
+[PARTIAL FACTORS EC7 BE SET2]
 LoadFactorPermUnfav=1.000
 LoadFactorPermFav=1.000
 LoadFactorVarUnfav=1.100
 LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.000
-LoadFactorVarUnfavMultiply=1.000
-LoadFactorPermUnfavCalc=0.000
-LoadFactorVarUnfavCalc=0.000
 ConstructLoadFactorPermFav=1.000
-ConstructLoadFactorVarFav=1.000
-ConstructLoadFactorPermUnfavMultiply=1.000
-ConstructLoadFactorVarUnfavMultiply=1.000
+ConstructLoadFactorVarFav=0.000
 ConstructLoadFactorPermUnfavCalc=1.000
 ConstructLoadFactorVarUnfavCalc=1.000
 EffectFactor=1.000
 EffectFactorVarUnfav=1.000
 MaterialFactorCohesion=1.250
-MaterialFactorUndrainedShearStrength=1.000
 MaterialFactorTgPhi=1.250
 MaterialFactorSubgradeReaction=1.000
 ResistanceFactor=1.000
 GeometryIncRetainingHeight=10.00
 GeometryMaxIncRetainingHeight=0.50
 GeometryDeltaPassiveSurfaceLevel=0.00
 GeometryDeltaPassivePhreaticLine=0.00
 GeometryDeltaActivePhreaticLine=0.00
 OverallStabilityFactorDrivingMoment=1.000
 OverallStabilityFactorCohesion=1.250
 OverallStabilityFactorTgPhi=1.250
 OverallStabilityFactorUnitWeight=1.000
 FactorRepValuesMDPmax=0.000
-VerticalBalanceGammaMb=1.300
-[END OF PARTIAL FACTORS EC7 B SET2]
+VerticalBalanceGammaMb=1.200
+[END OF PARTIAL FACTORS EC7 BE SET2]
 [PARTIAL FACTORS CUR I]
-SafetyFactorGammaD=1.00
-SafetyFactorEta=1.00
 LoadFactorPermUnfav=1.000
 LoadFactorPermFav=1.000
 LoadFactorVarUnfav=1.000
 LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.000
-LoadFactorVarUnfavMultiply=1.000
-LoadFactorPermUnfavCalc=0.000
-LoadFactorVarUnfavCalc=0.000
 ConstructLoadFactorPermFav=1.000
-ConstructLoadFactorVarFav=1.000
-ConstructLoadFactorPermUnfavMultiply=1.000
-ConstructLoadFactorVarUnfavMultiply=1.000
+ConstructLoadFactorVarFav=0.000
 ConstructLoadFactorPermUnfavCalc=1.000
 ConstructLoadFactorVarUnfavCalc=1.000
 EffectFactor=1.000
 EffectFactorVarUnfav=1.000
 MaterialFactorCohesion=1.000
-MaterialFactorUndrainedShearStrength=1.000
 MaterialFactorTgPhi=1.050
 MaterialFactorSubgradeReaction=1.300
 ResistanceFactor=1.000
 GeometryIncRetainingHeight=0.00
 GeometryMaxIncRetainingHeight=0.00
 GeometryDeltaPassiveSurfaceLevel=0.20
 GeometryDeltaPassivePhreaticLine=0.15
 GeometryDeltaActivePhreaticLine=0.05
 OverallStabilityFactorDrivingMoment=0.900
 OverallStabilityFactorCohesion=1.500
 OverallStabilityFactorTgPhi=1.200
 OverallStabilityFactorUnitWeight=1.000
 FactorRepValuesMDPmax=0.000
-VerticalBalanceGammaMb=1.200
+VerticalBalanceGammaMb=1.250
 [END OF PARTIAL FACTORS CUR I]
 [PARTIAL FACTORS CUR II]
-SafetyFactorGammaD=1.00
-SafetyFactorEta=1.00
 LoadFactorPermUnfav=1.000
 LoadFactorPermFav=1.000
 LoadFactorVarUnfav=1.000
 LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.000
-LoadFactorVarUnfavMultiply=1.000
-LoadFactorPermUnfavCalc=0.000
-LoadFactorVarUnfavCalc=0.000
 ConstructLoadFactorPermFav=1.000
-ConstructLoadFactorVarFav=1.000
-ConstructLoadFactorPermUnfavMultiply=1.000
-ConstructLoadFactorVarUnfavMultiply=1.000
+ConstructLoadFactorVarFav=0.000
 ConstructLoadFactorPermUnfavCalc=1.000
 ConstructLoadFactorVarUnfavCalc=1.000
 EffectFactor=1.000
 EffectFactorVarUnfav=1.000
 MaterialFactorCohesion=1.000
-MaterialFactorUndrainedShearStrength=1.000
 MaterialFactorTgPhi=1.150
 MaterialFactorSubgradeReaction=1.300
 ResistanceFactor=1.000
 GeometryIncRetainingHeight=0.00
 GeometryMaxIncRetainingHeight=0.00
 GeometryDeltaPassiveSurfaceLevel=0.30
 GeometryDeltaPassivePhreaticLine=0.20
 GeometryDeltaActivePhreaticLine=0.05
 OverallStabilityFactorDrivingMoment=1.000
 OverallStabilityFactorCohesion=1.500
 OverallStabilityFactorTgPhi=1.200
 OverallStabilityFactorUnitWeight=1.000
 FactorRepValuesMDPmax=0.000
-VerticalBalanceGammaMb=1.200
+VerticalBalanceGammaMb=1.250
 [END OF PARTIAL FACTORS CUR II]
 [PARTIAL FACTORS CUR III]
-SafetyFactorGammaD=1.00
-SafetyFactorEta=1.00
 LoadFactorPermUnfav=1.000
 LoadFactorPermFav=1.000
 LoadFactorVarUnfav=1.250
 LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.000
-LoadFactorVarUnfavMultiply=1.000
-LoadFactorPermUnfavCalc=0.000
-LoadFactorVarUnfavCalc=0.000
 ConstructLoadFactorPermFav=1.000
-ConstructLoadFactorVarFav=1.000
-ConstructLoadFactorPermUnfavMultiply=1.000
-ConstructLoadFactorVarUnfavMultiply=1.000
+ConstructLoadFactorVarFav=0.000
 ConstructLoadFactorPermUnfavCalc=1.000
 ConstructLoadFactorVarUnfavCalc=1.000
 EffectFactor=1.000
 EffectFactorVarUnfav=1.000
 MaterialFactorCohesion=1.100
-MaterialFactorUndrainedShearStrength=1.000
 MaterialFactorTgPhi=1.200
 MaterialFactorSubgradeReaction=1.300
 ResistanceFactor=1.000
 GeometryIncRetainingHeight=0.00
 GeometryMaxIncRetainingHeight=0.00
 GeometryDeltaPassiveSurfaceLevel=0.35
 GeometryDeltaPassivePhreaticLine=0.25
 GeometryDeltaActivePhreaticLine=0.05
 OverallStabilityFactorDrivingMoment=1.100
 OverallStabilityFactorCohesion=1.500
 OverallStabilityFactorTgPhi=1.200
 OverallStabilityFactorUnitWeight=1.000
 FactorRepValuesMDPmax=0.000
-VerticalBalanceGammaMb=1.200
+VerticalBalanceGammaMb=1.250
 [END OF PARTIAL FACTORS CUR III]
-[PARTIAL FACTORS EC7 SE VK1]
-SafetyFactorGammaD=0.83
-SafetyFactorEta=1.00
-LoadFactorPermUnfav=1.000
-LoadFactorPermFav=1.000
-LoadFactorVarUnfav=1.000
-LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.100
-LoadFactorVarUnfavMultiply=1.400
-LoadFactorPermUnfavCalc=0.913
-LoadFactorVarUnfavCalc=1.162
-ConstructLoadFactorPermFav=1.000
-ConstructLoadFactorVarFav=0.000
-ConstructLoadFactorPermUnfavMultiply=1.350
-ConstructLoadFactorVarUnfavMultiply=1.500
-ConstructLoadFactorPermUnfavCalc=1.121
-ConstructLoadFactorVarUnfavCalc=1.245
-EffectFactor=1.000
-EffectFactorVarUnfav=1.000
-MaterialFactorCohesion=1.300
-MaterialFactorUndrainedShearStrength=1.500
-MaterialFactorTgPhi=1.300
-MaterialFactorSubgradeReaction=1.000
-ResistanceFactor=1.000
-GeometryIncRetainingHeight=0.00
-GeometryMaxIncRetainingHeight=0.00
-GeometryDeltaPassiveSurfaceLevel=0.00
-GeometryDeltaPassivePhreaticLine=0.00
-GeometryDeltaActivePhreaticLine=0.00
-OverallStabilityFactorDrivingMoment=1.000
-OverallStabilityFactorCohesion=1.300
-OverallStabilityFactorTgPhi=1.300
-OverallStabilityFactorUnitWeight=1.000
-FactorRepValuesMDPmax=1.000
-VerticalBalanceGammaMb=1.300
-[END OF PARTIAL FACTORS EC7 SE VK1]
-[PARTIAL FACTORS EC7 SE VK2]
-SafetyFactorGammaD=0.91
-SafetyFactorEta=1.00
-LoadFactorPermUnfav=1.000
-LoadFactorPermFav=1.000
-LoadFactorVarUnfav=1.000
-LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.100
-LoadFactorVarUnfavMultiply=1.400
-LoadFactorPermUnfavCalc=1.001
-LoadFactorVarUnfavCalc=1.274
-ConstructLoadFactorPermFav=1.000
-ConstructLoadFactorVarFav=0.000
-ConstructLoadFactorPermUnfavMultiply=1.350
-ConstructLoadFactorVarUnfavMultiply=1.500
-ConstructLoadFactorPermUnfavCalc=1.228
-ConstructLoadFactorVarUnfavCalc=1.365
-EffectFactor=1.000
-EffectFactorVarUnfav=1.000
-MaterialFactorCohesion=1.300
-MaterialFactorUndrainedShearStrength=1.500
-MaterialFactorTgPhi=1.300
-MaterialFactorSubgradeReaction=1.000
-ResistanceFactor=1.000
-GeometryIncRetainingHeight=0.00
-GeometryMaxIncRetainingHeight=0.00
-GeometryDeltaPassiveSurfaceLevel=0.00
-GeometryDeltaPassivePhreaticLine=0.00
-GeometryDeltaActivePhreaticLine=0.00
-OverallStabilityFactorDrivingMoment=1.000
-OverallStabilityFactorCohesion=1.300
-OverallStabilityFactorTgPhi=1.300
-OverallStabilityFactorUnitWeight=1.000
-FactorRepValuesMDPmax=1.000
-VerticalBalanceGammaMb=1.300
-[END OF PARTIAL FACTORS EC7 SE VK2]
-[PARTIAL FACTORS EC7 SE VK3]
-SafetyFactorGammaD=1.00
-SafetyFactorEta=1.00
-LoadFactorPermUnfav=1.000
-LoadFactorPermFav=1.000
-LoadFactorVarUnfav=1.000
-LoadFactorVarFav=0.000
-LoadFactorPermUnfavMultiply=1.100
-LoadFactorVarUnfavMultiply=1.400
-LoadFactorPermUnfavCalc=1.100
-LoadFactorVarUnfavCalc=1.400
-ConstructLoadFactorPermFav=1.000
-ConstructLoadFactorVarFav=0.000
-ConstructLoadFactorPermUnfavMultiply=1.350
-ConstructLoadFactorVarUnfavMultiply=1.500
-ConstructLoadFactorPermUnfavCalc=1.350
-ConstructLoadFactorVarUnfavCalc=1.500
-EffectFactor=1.000
-EffectFactorVarUnfav=1.000
-MaterialFactorCohesion=1.300
-MaterialFactorUndrainedShearStrength=1.500
-MaterialFactorTgPhi=1.300
-MaterialFactorSubgradeReaction=1.000
-ResistanceFactor=1.000
-GeometryIncRetainingHeight=0.00
-GeometryMaxIncRetainingHeight=0.00
-GeometryDeltaPassiveSurfaceLevel=0.00
-GeometryDeltaPassivePhreaticLine=0.00
-GeometryDeltaActivePhreaticLine=0.00
-OverallStabilityFactorDrivingMoment=1.000
-OverallStabilityFactorCohesion=1.300
-OverallStabilityFactorTgPhi=1.300
-OverallStabilityFactorUnitWeight=1.000
-FactorRepValuesMDPmax=1.000
-VerticalBalanceGammaMb=1.300
-[END OF PARTIAL FACTORS EC7 SE VK3]
 [END OF CALCULATION OPTIONS]
 
 [PROBABILISTIC CALCULATION OPTIONS]
 {{ probabilistic_calculation_options }}
 [END OF PROBABILISTIC CALCULATION OPTIONS]
 
 [PROBABILISTIC CONTROL PARAMETERS]
```

### Comparing `d_geolib-0.5.1/geolib/models/dstability/analysis.py` & `d_geolib-0.6.0/geolib/models/dstability/analysis.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dstability/dstability_model.py` & `d_geolib-0.6.0/geolib/models/dstability/dstability_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dstability/dstability_parserprovider.py` & `d_geolib-0.6.0/geolib/models/dstability/dstability_parserprovider.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dstability/dstability_validator.py` & `d_geolib-0.6.0/geolib/models/dstability/dstability_validator.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dstability/internal.py` & `d_geolib-0.6.0/geolib/models/dstability/internal.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dstability/loads.py` & `d_geolib-0.6.0/geolib/models/dstability/loads.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dstability/reinforcements.py` & `d_geolib-0.6.0/geolib/models/dstability/reinforcements.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dstability/serializer.py` & `d_geolib-0.6.0/geolib/models/dstability/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dstability/states.py` & `d_geolib-0.6.0/geolib/models/dstability/states.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/dstability/utils.py` & `d_geolib-0.6.0/geolib/models/dstability/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/meta.py` & `d_geolib-0.6.0/geolib/models/meta.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/parsers.py` & `d_geolib-0.6.0/geolib/models/parsers.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/serializers.py` & `d_geolib-0.6.0/geolib/models/serializers.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/models/utils.py` & `d_geolib-0.6.0/geolib/models/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/service/main.py` & `d_geolib-0.6.0/geolib/service/main.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/service/README.md` & `d_geolib-0.6.0/geolib/service/README.md`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/soils/__init__.py` & `d_geolib-0.6.0/geolib/soils/__init__.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/soils/layers.py` & `d_geolib-0.6.0/geolib/soils/layers.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/soils/library.py` & `d_geolib-0.6.0/geolib/soils/library.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/soils/soil.py` & `d_geolib-0.6.0/geolib/soils/soil.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,16 @@
     """
     Mohr Coulomb parameters class
     """
 
     cohesion: Optional[Union[float, StochasticParameter]] = StochasticParameter()
     dilatancy_angle: Optional[Union[float, StochasticParameter]] = StochasticParameter()
     friction_angle: Optional[Union[float, StochasticParameter]] = StochasticParameter()
-    friction_angle_interface: Optional[
-        Union[float, StochasticParameter]
-    ] = StochasticParameter()
+    friction_angle_interface: Optional[Union[float, StochasticParameter]] = StochasticParameter()
+    is_delta_angle_automatically_calculated: Optional[bool] = None
     cohesion_and_friction_angle_correlated: Optional[bool] = None
 
 
 class SuTablePoint(SoilBaseModel):
     su: float = None
     stress: float = None
 
@@ -371,15 +370,16 @@
 class SoilType(IntEnum):
     GRAVEL = 0
     SAND = 1
     LOAM = 2
     CLAY = 3
     PEAT = 4
     SANDY_LOAM = 5
-
+    TERTCLAY = 6
+    CLAYEYSAND = 7
 
 class Soil(SoilBaseModel):
     """Soil Material."""
 
     id: Optional[str] = None
     name: Optional[str] = None
     code: Optional[str] = None
@@ -401,15 +401,14 @@
 
     horizontal_behaviour: Optional[HorizontalBehaviour] = HorizontalBehaviour()
     cone_resistance: Optional[ConeResistance] = ConeResistance()
     use_tension: Optional[bool] = None
     use_probabilistic_defaults: Optional[bool] = False
     soil_type_settlement_by_vibrations: Optional[SoilType] = SoilType.SAND
     soil_type_nl: Optional[SoilType] = SoilType.SAND
-    soil_type_be: Optional[SoilType] = SoilType.SAND
     soil_state: Optional[SoilState] = SoilState()
     shear_strength_model_above_phreatic_level: Optional[
         ShearStrengthModelTypePhreaticLevel
     ] = None
     shear_strength_model_below_phreatic_level: Optional[
         ShearStrengthModelTypePhreaticLevel
     ] = None
@@ -570,15 +569,14 @@
 
         from geolib.models.dfoundations.internal_soil import Soil as DFoundationSoil
 
         return DFoundationSoil(
             name=self.name,
             soilcolor=self.color.to_internal(),
             soilsoiltype=self.soil_type_nl,
-            soilbelgiansoiltype=self.soil_type_be,
             soilgamdry=self.soil_weight_parameters.unsaturated_weight.mean,
             soilgamwet=self.soil_weight_parameters.saturated_weight.mean,
             soilinitialvoidratio=self.soil_classification_parameters.initial_void_ratio.mean,
             soildiameterd50=self.soil_classification_parameters.d_50,
             soilminvoidratio=self.soil_classification_parameters.min_void_ratio,
             soilmaxvoidratio=self.soil_classification_parameters.max_void_ratio,
             soilcohesion=self.mohr_coulomb_parameters.cohesion.mean,
@@ -758,14 +756,15 @@
             soilgamdry=self.soil_weight_parameters.unsaturated_weight.mean,
             soilgamwet=self.soil_weight_parameters.saturated_weight.mean,
             soilrelativedensity=self.soil_classification_parameters.relative_density,
             soilemodmenard=self.soil_stiffness_parameters.emod_menard,
             soilcohesion=self.mohr_coulomb_parameters.cohesion.mean,
             soilphi=self.mohr_coulomb_parameters.friction_angle.mean,
             soildelta=self.mohr_coulomb_parameters.friction_angle_interface.mean,
+            soilisdeltaangleautomaticallycalculated=self.mohr_coulomb_parameters.is_delta_angle_automatically_calculated,
             soilocr=self.soil_state.ocr_layer.mean,
             soilpermeabkx=self.storage_parameters.horizontal_permeability.mean,
             soilstdcohesion=self.mohr_coulomb_parameters.cohesion.standard_deviation,
             soilstdphi=self.mohr_coulomb_parameters.friction_angle.standard_deviation,
             soildistcohesion=self.mohr_coulomb_parameters.cohesion.distribution_type,
             soildistphi=self.mohr_coulomb_parameters.friction_angle.distribution_type,
             soilla=self.earth_pressure_coefficients.active,
```

### Comparing `d_geolib-0.5.1/geolib/soils/soil_utils.py` & `d_geolib-0.6.0/geolib/soils/soil_utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/geolib/utils.py` & `d_geolib-0.6.0/geolib/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/LICENSE` & `d_geolib-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/pyproject.toml` & `d_geolib-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "d-geolib"
-version = "0.5.1"
+version = "0.6.0"
 description = "Python wrappers around the input and output files of the Deltares D-Serie and D-GEO Suite models"
 authors = ["Maarten Pronk <maarten.pronk@deltares.nl>", "Deltares"]
 license = "MIT"
 homepage = "https://deltares.github.io/GEOLib/"
 documentation = "https://deltares.github.io/GEOLib/"
 repository = "https://github.com/Deltares/GEOLib"
 readme = "README.rst"
@@ -66,15 +66,15 @@
 force_grid_wrap=0
 use_parentheses=true
 line_length=90
 profile = "black"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.1"
+version = "0.6.0"
 tag_format = "v$major.$minor.$patch$prerelease"
 version_files = [
     "pyproject.toml:^version",
     "tests/test_geolib.py",
     "geolib/__init__.py:__version__",
 ]
 annotated_tag = true
```

### Comparing `d_geolib-0.5.1/README.rst` & `d_geolib-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `d_geolib-0.5.1/PKG-INFO` & `d_geolib-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d-geolib
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python wrappers around the input and output files of the Deltares D-Serie and D-GEO Suite models
 Home-page: https://deltares.github.io/GEOLib/
 License: MIT
 Author: Maarten Pronk
 Author-email: maarten.pronk@deltares.nl
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

