# Comparing `tmp/steam_sdk-2023.4.1.tar.gz` & `tmp/steam_sdk-2023.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam_sdk-2023.4.1.tar", last modified: Thu Apr 13 17:30:09 2023, max compression
+gzip compressed data, was "dist\steam_sdk-2023.4.2.tar", last modified: Thu Apr 20 16:50:27 2023, max compression
```

## Comparing `steam_sdk-2023.4.1.tar` & `steam_sdk-2023.4.2.tar`

### file list

```diff
@@ -1,202 +1,206 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.675887 steam_sdk-2023.4.1/
--rw-rw-rw-   0        0        0     3743 2023-01-10 08:52:04.000000 steam_sdk-2023.4.1/.gitignore
--rw-rw-rw-   0        0        0     1963 2023-02-01 10:40:32.000000 steam_sdk-2023.4.1/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      122 2023-02-02 14:39:18.000000 steam_sdk-2023.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1550 2023-04-13 17:30:09.675887 steam_sdk-2023.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2023-04-11 10:02:40.000000 steam_sdk-2023.4.1/Readme.md
--rw-rw-rw-   0        0        0     5370 2023-01-20 13:20:13.000000 steam_sdk-2023.4.1/mkdocs.yaml
--rw-rw-rw-   0        0        0     1684 2023-04-13 15:56:12.000000 steam_sdk-2023.4.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 17:30:09.676884 steam_sdk-2023.4.1/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-04-13 17:24:12.000000 steam_sdk-2023.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.519305 steam_sdk-2023.4.1/steam_sdk/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.526289 steam_sdk-2023.4.1/steam_sdk/analyses/
--rw-rw-rw-   0        0        0    99466 2023-04-13 13:06:52.000000 steam_sdk-2023.4.1/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.527285 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.529280 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23368 2022-10-17 13:51:31.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.538255 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16757 2022-10-07 10:25:49.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2800 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6828 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95412 2022-11-16 07:50:44.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2652 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2341 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.539253 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22374 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.543242 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4527 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2921 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.545236 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29433 2022-09-29 08:14:52.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.549226 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4704 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4852 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.550223 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.563188 steam_sdk-2023.4.1/steam_sdk/builders/
--rw-rw-rw-   0        0        0    10098 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   160973 2023-01-17 16:22:36.000000 steam_sdk-2023.4.1/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    32791 2023-04-13 17:03:42.000000 steam_sdk-2023.4.1/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    38418 2023-04-13 17:10:32.000000 steam_sdk-2023.4.1/steam_sdk/builders/BuilderSIGMA.py
--rw-rw-rw-   0        0        0      246 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/builders/Readme.md
--rw-rw-rw-   0        0        0    11689 2023-01-20 13:20:13.000000 steam_sdk-2023.4.1/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2022-12-02 14:32:36.000000 steam_sdk-2023.4.1/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.564186 steam_sdk-2023.4.1/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.566181 steam_sdk-2023.4.1/steam_sdk/configs/plotters/
--rw-rw-rw-   0        0        0      294 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/plotters/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.569172 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.572164 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0     9137 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml
--rw-rw-rw-   0        0        0    32890 2022-10-04 13:23:53.000000 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
--rw-rw-rw-   0        0        0      174 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/Readme.md
--rw-rw-rw-   0        0        0     1426 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.573162 steam_sdk-2023.4.1/steam_sdk/configs/users/
--rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/users/Readme.md
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.575156 steam_sdk-2023.4.1/steam_sdk/cosims/
--rw-rw-rw-   0        0        0       69 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/cosims/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.598095 steam_sdk-2023.4.1/steam_sdk/data/
--rw-rw-rw-   0        0        0    10029 2023-04-03 16:34:32.000000 steam_sdk-2023.4.1/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0     8004 2023-03-14 14:37:52.000000 steam_sdk-2023.4.1/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0     3281 2022-09-28 15:13:02.000000 steam_sdk-2023.4.1/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2862 2023-03-30 16:17:31.000000 steam_sdk-2023.4.1/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     3169 2023-01-20 13:20:13.000000 steam_sdk-2023.4.1/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0     8492 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0    10767 2022-10-04 13:23:53.000000 steam_sdk-2023.4.1/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     4314 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5869 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    35518 2023-04-13 13:06:52.000000 steam_sdk-2023.4.1/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     2609 2023-04-13 13:06:52.000000 steam_sdk-2023.4.1/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/data/DataParsims.py
--rw-rw-rw-   0        0        0     1995 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2105 2022-09-28 15:19:24.000000 steam_sdk-2023.4.1/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     7899 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     1650 2023-03-14 14:45:17.000000 steam_sdk-2023.4.1/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3204 2023-01-10 08:52:04.000000 steam_sdk-2023.4.1/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0    22928 2022-10-04 13:23:53.000000 steam_sdk-2023.4.1/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0      153 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/data/Readme.md
--rw-rw-rw-   0        0        0    27540 2022-10-04 13:23:53.000000 steam_sdk-2023.4.1/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.609066 steam_sdk-2023.4.1/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3151 2022-11-24 16:16:38.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     2711 2022-11-24 16:16:38.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     1299 2023-02-01 20:32:34.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     3482 2023-01-10 08:52:04.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1924 2022-11-16 07:50:44.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2062 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0     5329 2023-04-13 15:48:42.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverSIGMA.py
--rw-rw-rw-   0        0        0     1932 2022-11-16 07:50:44.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0      193 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/drivers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.611060 steam_sdk-2023.4.1/steam_sdk/drivers/temp/
--rw-rw-rw-   0        0        0    27295 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/drivers/temp/postLEDET.py
--rw-rw-rw-   0        0        0     1820 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/drivers/temp/runLEDET.py
--rw-rw-rw-   0        0        0     5459 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/drivers/temp/simLEDET.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.634000 steam_sdk-2023.4.1/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      317 2023-04-13 13:06:52.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0     2290 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1077 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6220 2022-10-17 13:51:31.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     1650 2023-01-17 13:00:56.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     1030 2023-03-14 14:37:52.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserDatToCsv.py
--rw-rw-rw-   0        0        0     8536 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2287 2022-09-28 15:13:08.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0    48056 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    12436 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    10602 2023-03-14 14:37:52.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    61567 2023-04-03 16:34:32.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4780 2023-03-14 14:37:52.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6838 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     2942 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserProtePyBBQ.py
--rw-rw-rw-   0        0        0    92213 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0    11707 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    55281 2023-02-02 14:52:07.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     4088 2023-03-14 14:37:52.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0      113 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0        2 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/dict_to_in.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.634997 steam_sdk-2023.4.1/steam_sdk/parsers/templates/
--rw-rw-rw-   0        0        0      709 2022-11-16 07:50:44.000000 steam_sdk-2023.4.1/steam_sdk/parsers/templates/template_Dakota.in
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.640980 steam_sdk-2023.4.1/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    41232 2023-04-13 13:06:52.000000 steam_sdk-2023.4.1/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0      916 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    49099 2023-04-13 13:06:52.000000 steam_sdk-2023.4.1/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    59958 2023-04-03 16:34:32.000000 steam_sdk-2023.4.1/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0     1972 2023-01-23 16:45:50.000000 steam_sdk-2023.4.1/steam_sdk/parsims/ParsimSweep.py
--rw-rw-rw-   0        0        0       72 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsims/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.645968 steam_sdk-2023.4.1/steam_sdk/plotters/
--rw-rw-rw-   0        0        0    39596 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2022-12-02 17:12:04.000000 steam_sdk-2023.4.1/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0     8871 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0    18478 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/plotters/PlotterSIGMA.py
--rw-rw-rw-   0        0        0      130 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/plotters/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.647962 steam_sdk-2023.4.1/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0     5564 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.665914 steam_sdk-2023.4.1/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2023-03-14 14:37:52.000000 steam_sdk-2023.4.1/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0    14942 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     4587 2023-01-17 13:00:56.000000 steam_sdk-2023.4.1/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2745 2022-10-04 13:23:53.000000 steam_sdk-2023.4.1/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0      686 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0     3837 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      299 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0     4512 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0      388 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2023-01-10 08:52:04.000000 steam_sdk-2023.4.1/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     6745 2023-04-13 13:06:52.000000 steam_sdk-2023.4.1/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.668905 steam_sdk-2023.4.1/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    35919 2023-03-30 13:07:50.000000 steam_sdk-2023.4.1/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0     6127 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/viewers/ViewerMeas.py
--rw-rw-rw-   0        0        0     1667 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/viewers/ViewerSim.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.671898 steam_sdk-2023.4.1/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0      154 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/wrappers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.671898 steam_sdk-2023.4.1/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.672895 steam_sdk-2023.4.1/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.674889 steam_sdk-2023.4.1/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0    72381 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/wrappers/java/SING/jars/steam-sing.jar
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1834 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.524292 steam_sdk-2023.4.1/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     1550 2023-04-13 17:29:43.000000 steam_sdk-2023.4.1/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7134 2023-04-13 17:30:08.000000 steam_sdk-2023.4.1/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 17:29:43.000000 steam_sdk-2023.4.1/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1595 2023-04-13 17:29:43.000000 steam_sdk-2023.4.1/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 17:29:43.000000 steam_sdk-2023.4.1/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.412520 steam_sdk-2023.4.2/
+-rw-rw-rw-   0        0        0     3743 2023-01-10 08:52:04.000000 steam_sdk-2023.4.2/.gitignore
+-rw-rw-rw-   0        0        0     1963 2023-02-01 10:40:32.000000 steam_sdk-2023.4.2/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      122 2023-02-02 14:39:18.000000 steam_sdk-2023.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1550 2023-04-20 16:50:27.412520 steam_sdk-2023.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2023-04-11 10:02:40.000000 steam_sdk-2023.4.2/Readme.md
+-rw-rw-rw-   0        0        0     5370 2023-01-20 13:20:13.000000 steam_sdk-2023.4.2/mkdocs.yaml
+-rw-rw-rw-   0        0        0     1685 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 16:50:27.413519 steam_sdk-2023.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-04-20 15:51:06.000000 steam_sdk-2023.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.157204 steam_sdk-2023.4.2/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.169171 steam_sdk-2023.4.2/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0   103197 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.174159 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.178148 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23368 2022-10-17 13:51:31.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.188122 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16757 2022-10-07 10:25:49.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2800 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6828 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95412 2022-11-16 07:50:44.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2652 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2341 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.190116 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22374 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.195102 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4527 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2921 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.197097 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29433 2022-09-29 08:14:52.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.203081 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4704 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4852 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.205075 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.245966 steam_sdk-2023.4.2/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    10098 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   160973 2023-01-17 16:22:36.000000 steam_sdk-2023.4.2/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    32791 2023-04-13 17:03:42.000000 steam_sdk-2023.4.2/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    38418 2023-04-13 17:10:32.000000 steam_sdk-2023.4.2/steam_sdk/builders/BuilderSIGMA.py
+-rw-rw-rw-   0        0        0      246 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/builders/Readme.md
+-rw-rw-rw-   0        0        0    11689 2023-01-20 13:20:13.000000 steam_sdk-2023.4.2/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2022-12-02 14:32:36.000000 steam_sdk-2023.4.2/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.247960 steam_sdk-2023.4.2/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.255939 steam_sdk-2023.4.2/steam_sdk/configs/plotters/
+-rw-rw-rw-   0        0        0      294 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/plotters/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.262921 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.265913 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0     9137 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml
+-rw-rw-rw-   0        0        0    32890 2022-10-04 13:23:53.000000 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
+-rw-rw-rw-   0        0        0      174 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/Readme.md
+-rw-rw-rw-   0        0        0     1426 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.266910 steam_sdk-2023.4.2/steam_sdk/configs/users/
+-rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/users/Readme.md
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.268905 steam_sdk-2023.4.2/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0       69 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/cosims/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.297828 steam_sdk-2023.4.2/steam_sdk/data/
+-rw-rw-rw-   0        0        0    10087 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0     8004 2023-03-14 14:37:52.000000 steam_sdk-2023.4.2/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0     3281 2022-09-28 15:13:02.000000 steam_sdk-2023.4.2/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2865 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     3169 2023-01-20 13:20:13.000000 steam_sdk-2023.4.2/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0     8492 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0    10767 2022-10-04 13:23:53.000000 steam_sdk-2023.4.2/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     4314 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5869 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    35518 2023-04-13 13:06:52.000000 steam_sdk-2023.4.2/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     3076 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/data/DataParsims.py
+-rw-rw-rw-   0        0        0     1995 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2105 2022-09-28 15:19:24.000000 steam_sdk-2023.4.2/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     7899 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     1650 2023-03-14 14:45:17.000000 steam_sdk-2023.4.2/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3204 2023-01-10 08:52:04.000000 steam_sdk-2023.4.2/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0    22928 2022-10-04 13:23:53.000000 steam_sdk-2023.4.2/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0      153 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/data/Readme.md
+-rw-rw-rw-   0        0        0    27540 2022-10-04 13:23:53.000000 steam_sdk-2023.4.2/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.313786 steam_sdk-2023.4.2/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3151 2022-11-24 16:16:38.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     2711 2022-11-24 16:16:38.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     1299 2023-02-01 20:32:34.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3482 2023-01-10 08:52:04.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1924 2022-11-16 07:50:44.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2062 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0     5329 2023-04-13 15:48:42.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverSIGMA.py
+-rw-rw-rw-   0        0        0     1932 2022-11-16 07:50:44.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0      193 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/drivers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.320766 steam_sdk-2023.4.2/steam_sdk/drivers/temp/
+-rw-rw-rw-   0        0        0    27295 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/drivers/temp/postLEDET.py
+-rw-rw-rw-   0        0        0     1820 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/drivers/temp/runLEDET.py
+-rw-rw-rw-   0        0        0     5459 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/drivers/temp/simLEDET.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.348691 steam_sdk-2023.4.2/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      317 2023-04-13 13:06:52.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0     2290 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1077 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6220 2022-10-17 13:51:31.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     1650 2023-01-17 13:00:56.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     1030 2023-03-14 14:37:52.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserDatToCsv.py
+-rw-rw-rw-   0        0        0     8536 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2287 2022-09-28 15:13:08.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0    48056 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    12436 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    10602 2023-03-14 14:37:52.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    61567 2023-04-03 16:34:32.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4780 2023-03-14 14:37:52.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6838 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     2942 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserProtePyBBQ.py
+-rw-rw-rw-   0        0        0    92213 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0    11707 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    55281 2023-02-02 14:52:07.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     4088 2023-03-14 14:37:52.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0      113 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0        2 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/dict_to_in.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.349689 steam_sdk-2023.4.2/steam_sdk/parsers/templates/
+-rw-rw-rw-   0        0        0      709 2022-11-16 07:50:44.000000 steam_sdk-2023.4.2/steam_sdk/parsers/templates/template_Dakota.in
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.361657 steam_sdk-2023.4.2/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    44535 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0      916 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    59090 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    59958 2023-04-03 16:34:32.000000 steam_sdk-2023.4.2/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0     1972 2023-01-23 16:45:50.000000 steam_sdk-2023.4.2/steam_sdk/parsims/ParsimSweep.py
+-rw-rw-rw-   0        0        0       72 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsims/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.362654 steam_sdk-2023.4.2/steam_sdk/parsims/translation_dicts/
+-rw-rw-rw-   0        0        0     1735 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.370632 steam_sdk-2023.4.2/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0    39596 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2022-12-02 17:12:04.000000 steam_sdk-2023.4.2/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0     8871 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0    18478 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/plotters/PlotterSIGMA.py
+-rw-rw-rw-   0        0        0      130 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/plotters/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.372627 steam_sdk-2023.4.2/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0     5564 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.395566 steam_sdk-2023.4.2/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2023-03-14 14:37:52.000000 steam_sdk-2023.4.2/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0    14942 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     4587 2023-01-17 13:00:56.000000 steam_sdk-2023.4.2/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2745 2022-10-04 13:23:53.000000 steam_sdk-2023.4.2/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0      686 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0     3837 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0     1279 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/utils/get_attribute_type.py
+-rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      299 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0     1592 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/utils/parse_str_to_list.py
+-rw-rw-rw-   0        0        0      388 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2023-01-10 08:52:04.000000 steam_sdk-2023.4.2/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     6908 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.401550 steam_sdk-2023.4.2/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    35919 2023-03-30 13:07:50.000000 steam_sdk-2023.4.2/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0     6127 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/viewers/ViewerMeas.py
+-rw-rw-rw-   0        0        0     1667 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/viewers/ViewerSim.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.405540 steam_sdk-2023.4.2/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0      154 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/wrappers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.406537 steam_sdk-2023.4.2/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.407534 steam_sdk-2023.4.2/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.410526 steam_sdk-2023.4.2/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0    72381 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/wrappers/java/SING/jars/steam-sing.jar
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1834 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.163187 steam_sdk-2023.4.2/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1550 2023-04-20 16:50:00.000000 steam_sdk-2023.4.2/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7273 2023-04-20 16:50:25.000000 steam_sdk-2023.4.2/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 16:50:00.000000 steam_sdk-2023.4.2/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1596 2023-04-20 16:50:00.000000 steam_sdk-2023.4.2/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-20 16:50:00.000000 steam_sdk-2023.4.2/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam_sdk-2023.4.1/.gitignore` & `steam_sdk-2023.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/.gitlab-ci.yml` & `steam_sdk-2023.4.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/PKG-INFO` & `steam_sdk-2023.4.2/steam_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: steam_sdk
-Version: 2023.4.1
+Name: steam-sdk
+Version: 2023.4.2
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: STEAM,CERN,SDK,API
+Keywords: CERN,API,STEAM,SDK
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam_sdk-2023.4.1/Readme.md` & `steam_sdk-2023.4.2/Readme.md`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/mkdocs.yaml` & `steam_sdk-2023.4.2/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/requirements.txt` & `steam_sdk-2023.4.2/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 ruamel.yaml==0.17.21
 ruamel.yaml.clib==0.2.6
 scipy==1.9.1
 seaborn==0.12.0
 six==1.16.0
 smmap==5.0.0
 stack-data==0.5.0
-STEAM-materials==0.0.2
+STEAM-materials==0.0.33
 svglib == 1.5.1
 tomli==2.0.1
 tqdm==4.64.1
 traitlets==5.4.0
 typing_extensions==4.3.0
 urllib3==1.26.12
 watchdog==2.1.9
```

### Comparing `steam_sdk-2023.4.1/setup.py` & `steam_sdk-2023.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam_sdk',
-    version="2023.4.1",
+    version="2023.4.2",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={'STEAM', 'API', 'SDK', 'CERN'},
```

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/AnalysisSTEAM.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-import csv
 import sys
 import ntpath
 import os
 import pathlib
 import shutil
 import importlib
 import importlib.util
 import pandas as pd
 import pickle
 from copy import deepcopy
 from pathlib import Path
 from typing import Union
-from ast import literal_eval
 
 from steam_sdk.data.DataSettings import DataSettings
 from steam_sdk.builders.BuilderModel import BuilderModel
 from steam_sdk.data.DataAnalysis import DataAnalysis, ModifyModel, ModifyModelMultipleVariables, ParametricSweep, LoadCircuitParameters, WriteStimulusFile
 from steam_sdk.drivers.DriverFiQuS import DriverFiQuS
 from steam_sdk.drivers.DriverLEDET import DriverLEDET
 from steam_sdk.drivers.DriverPSPICE import DriverPSPICE
 from steam_sdk.drivers.DriverPyBBQ import DriverPyBBQ
 from steam_sdk.drivers.DriverSIGMA import DriverSIGMA
 from steam_sdk.drivers.DriverXYCE import DriverXYCE
 from steam_sdk.parsers.ParserYAML import dict_to_yaml, yaml_to_data
 from steam_sdk.parsims.ParsimConductor import ParsimConductor
 from steam_sdk.parsims.ParsimEventCircuit import ParsimEventCircuit
 from steam_sdk.parsims.ParsimEventMagnet import ParsimEventMagnet
-from steam_sdk.parsims.ParsimSweep import ParsimSweep
+from steam_sdk.utils import parse_str_to_list
 from steam_sdk.postprocs.PostprocsMetrics import PostprocsMetrics
 from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
+from steam_sdk.utils.parse_str_to_list import parse_str_to_list
 from steam_sdk.utils.rgetattr import rgetattr
 from steam_sdk.utils.sgetattr import rsetattr
 from steam_sdk.utils.rhasattr import rhasattr
 from steam_sdk.viewers.Viewer import Viewer
 from steam_sdk.parsers.ParserPSPICE import writeStimuliFromInterpolation
 
 
@@ -106,14 +105,16 @@
         # Raise exceptions if folders are not defined.
         if self.data_analysis.WorkingFolders.library_path == 'gitlab':
             import steam_models
             steam_models_path = steam_models.__path__[0]
             self.data_analysis.WorkingFolders.library_path = steam_models_path
         elif self.data_analysis.WorkingFolders.library_path in ['same_as_analysis_yaml']:
             self.data_analysis.WorkingFolders.library_path = '.' + os.sep + self.data_analysis.GeneralParameters.model.name + os.sep + 'input'
+        elif self.data_analysis.WorkingFolders.library_path in ['steam_models_in_same_folder']:
+            self.data_analysis.WorkingFolders.library_path = '..' + os.sep + 'steam_models' + os.sep + 'input'
         if not self.data_analysis.WorkingFolders.library_path:
             raise Exception('Model library path must be defined. Key to provide: WorkingFolders.library_path')
         if not self.data_analysis.WorkingFolders.output_path:
             raise Exception('Output folder path must be defined. Key to provide: WorkingFolders.output_path')
         if not self.data_analysis.WorkingFolders.temp_path:
             raise Exception('Temporary folder path must be defined. Key to provide: WorkingFolders.temp_path')
 
@@ -176,15 +177,16 @@
             settings_dict = yaml_to_data(full_path_file_settings)
 
         # Assign the keys read either from permanent-settings or local-settings
         for name, _ in self.settings.__dict__.items():
             if name in settings_dict:
                 value = settings_dict[name]
                 self.setAttribute(self.settings, name, value)
-                if verbose: print('{} : {}. Added.'.format(name, value))
+                if value:
+                    if verbose: print('{} : {}. Added.'.format(name, value))
             else:
                 if verbose: print('{}: not found in the settings. Skipped.'.format(name))
 
         # Dump read keys to temporary settings file locally
         path_temp_file_settings = Path(os.path.join('', settings_file)).resolve()
         dict_to_yaml(settings_dict, path_temp_file_settings)
         if verbose: print('File {} was saved locally.'.format(path_temp_file_settings))
@@ -1384,20 +1386,31 @@
                 circuit_type = self.__get_circuit_type(circuit_name)
                 number_of_magnets = self.__get_number_of_magnets(circuit_name)
                 number_of_apertures = self.__get_number_of_apertures(circuit_name)
                 current_level = pec.list_events[event_number].PoweredCircuits[circuit_name].current_at_discharge
                 magnets_list = self.__get_magnets_list(number_of_magnets)
                 t_PC_off = pec.list_events[event_number].PoweredCircuits[circuit_name].delta_t_FGC_PIC
                 magnet_types = self.__get_magnet_types_list(number_of_magnets)
-                load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.abspath(f"../../../steam_models/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name)
+                if circuit_family_name == "RQ":
+                    circuit_name_1 = circuit_name.replace(".", "D_")
+                    circuit_name_2 = circuit_name.replace(".", "F_")
+                    load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.abspath(f"../../../steam_models/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_1)
+                else:
+                    load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.abspath(f"../../../steam_models/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name)
                 if circuit_family_name == "IPD":
                     stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_family_name}', f'{event_number + 1}', 'coil_resistances.stl')
                 else:
                     stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_type}', f'{event_number + 1}', 'coil_resistances.stl')
-                write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.abspath(f'../../../steam_models/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                if circuit_family_name == "RQ":
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.abspath(f'../../../steam_models/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                elif circuit_family_name == "RQX":
+                    current_level = [current_level[0]+current_level[1], current_level[0]+current_level[2], current_level[0]+current_level[2], current_level[0]]
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.abspath(f'../../../steam_models/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.abspath(f'../../../steam_models/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=current_level, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                else:
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.abspath(f'../../../steam_models/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 # start parsim sweep step with newly created event file
                 parsim_sweep_step = ParametricSweep(type='ParametricSweep', input_sweep_file=path_output_event_csv,
                                                     model_name=model_name, case_model=case_model, software=software, verbose=verbose)
                 self.load_circuit_parameters(load_circuit_parameters_step, verbose=verbose)
                 self.write_stimuli_from_interpolation(write_stimuli_file_step, verbose=verbose)
                 self.run_parsim_sweep(parsim_sweep_step, verbose=verbose)
 
@@ -1411,33 +1424,44 @@
         if verbose:
             print(f'ParsimEvent called using input file {input_file}.')
 
     def run_parsim_conductor(self, step, verbose):
         '''
         Function to generate steps to change the conductor data of a magnet using a csv database
 
-        :param step:
+        :param step: instance of ParsimConductor step
         :param verbose: if true displays more information
         '''
         # Unpack inputs
         model_name = step.model_name
         case_model = step.case_model
         software = step.software
         groups_to_coils = step.groups_to_coils
+        groups_to_coil_length = step.groups_to_coil_length
         simulation_number = step.simulation_number
         input_file = step.input_file
         path_output_sweeper_csv = step.path_output_sweeper_csv
         strand_critical_current_measurements = step.strand_critical_current_measurements
 
-        # check inputs
+        # check if crucial variables are not None
         if not path_output_sweeper_csv:
             raise Exception('File path path_output_event_csv must be defined for an analysis step of type ParsimEvent.')
         if not input_file:
             raise Exception('File path path_output_event_csv must be defined for an analysis step of type ParsimEvent.')
 
+        # check if all groups are defined in the group dictionaries
+        highest_group_index = max([max(values) for values in groups_to_coils.values()])
+        expected_group_numbers = list(range(1, highest_group_index + 1))
+        all_group_numbers_in_dict = [num for sublist in groups_to_coils.values() for num in sublist]
+        if sorted(all_group_numbers_in_dict) != expected_group_numbers:
+            raise Exception(f'Invalid groups_to_coils entry in step definition. \nSorted groups given by the user: {sorted(all_group_numbers_in_dict)}')
+        all_group_numbers_in_dict = [num for sublist in groups_to_coil_length.values() for num in sublist]
+        if sorted(all_group_numbers_in_dict) != expected_group_numbers:
+            raise Exception(f'Invalid groups_to_coil_length entry in step definition. \nSorted groups given by the user: {sorted(all_group_numbers_in_dict)}')
+
 
         # make a copy of the respective conductor for every coil and store it in the magnet model
         # NOTE: if a coil consists of 2 different conductors the user has to treat them as 2 different coils (so a coil is not always a coil but rather a subcoil with the same conductor)
         new_conductors = [None] * len(groups_to_coils)
         dict_coilname_to_conductorindex = {}
         new_conductor_to_group = [None] * len(self.list_models[model_name].model_data.CoilWindings.conductor_to_group)
         for idx, (coil_name, group_numbers) in enumerate(groups_to_coils.items()):
@@ -1470,21 +1494,23 @@
         self.list_models[model_name].model_data.CoilWindings.conductor_to_group = new_conductor_to_group
         # NOTE: so far no parameters of the model_data were altered, just copies of the conductor have been made and connected to the specified groups
         del new_conductors, new_conductor_to_group
 
 
         if case_model == 'magnet':
             # create instance of ParsimConductor
-            pc = ParsimConductor(verbose=verbose, model_data_conductors=self.list_models[model_name].model_data.Conductors)
+            pc = ParsimConductor(verbose=verbose, model_data=self.list_models[model_name].model_data,
+                                 dict_coilName_to_conductorIndex=dict_coilname_to_conductorindex,
+                                 groups_to_coils=groups_to_coils, groups_to_coil_length=groups_to_coil_length)
             # read the conductor database
             pc.read_from_input(path_input_file=input_file, magnet_name=self.list_models[model_name].model_data.GeneralParameters.magnet_name,
                                strand_critical_current_measurements=strand_critical_current_measurements)
             # write a sweeper csv file
             pc.write_conductor_parameter_file(path_output_file=path_output_sweeper_csv, simulation_name=model_name,
-                                              simulation_number=simulation_number, dict_coilname_to_conductorindex=dict_coilname_to_conductorindex)
+                                              simulation_number=simulation_number)
 
             # create parsim sweep step with newly created sweeper csv file and run it
             parsim_sweep_step = ParametricSweep(type='ParametricSweep', input_sweep_file=path_output_sweeper_csv, # TODO rename teh class to ParametricSweepStep? ParsimConductor is no step class and ParametricSweep is
                                                 model_name=model_name, case_model=case_model, software=software, verbose=verbose)
             self.run_parsim_sweep(parsim_sweep_step, verbose=verbose)
         else:
             raise Exception(f'Case_model "{case_model}" not supported by ParsimConductor.')
@@ -1529,15 +1555,22 @@
             if case_model == 'magnet':
                 new_start_time = self.__get_earliest_QH_starting_time(row)
 
             # set simulation start time 50 ms before the start time of the first Quench Heater
             dict_variables_to_change = dict()
             if case_model == 'magnet' and 'LEDET' in software:
                 time_vec = rgetattr(self.list_models[model_name].model_data,'Options_LEDET.time_vector.time_vector_params')
-                if new_start_time: time_vec[0] = new_start_time
+                if new_start_time:
+                    # shift all times in time_vector by the difference by which the simulation has to start earlier
+                    diff = new_start_time - time_vec[0]
+                    # time_vec structure is: [start_val1, step_size1, end_val1, start_val2, step_size2, end_val2, ...]
+                    # all values of time should be shifted in space by the difference (all start and end values)
+                    for i in range(int(len(time_vec)/3)):
+                        time_vec[0+3*i] = time_vec[0+3*i] + diff
+                        time_vec[2+3*i] = time_vec[2+3*i] + diff
                 dict_variables_to_change['Options_LEDET.time_vector.time_vector_params'] = time_vec
 
             # unpack model_data
             if case_model == 'magnet':
                 model_data = self.list_models[model_name].model_data
                 next_simulation_name = model_data.GeneralParameters.magnet_name
             elif case_model == 'circuit':
@@ -1577,15 +1610,15 @@
 
                 # Check if the current variable is present in the model data structure & value in csv is not empty
                 elif rhasattr(model_data, var_name):
                     # save valid new variable names and values to change them later
                     if type(var_value) == int or type(var_value) == float:
                         dict_variables_to_change[var_name] = var_value
                     elif type(var_value) == str:
-                        dict_variables_to_change[var_name] = self.__parse_string(var_value)
+                        dict_variables_to_change[var_name] = parse_str_to_list(var_value)
                     else:
                         raise Exception(f'ERROR: Datatype of Element in Column "{var_value}" Row "{j + 2}" of csv file {input_sweep_file} is invalid.')
 
                 # print when columns have been skipped
                 elif not rhasattr(model_data, var_name) and var_name != 'simulation_number':
                     print(f'WARNING: Column name "{var_name}" with value "{var_value}" in csv file {input_sweep_file} is skipped.')
             
@@ -1624,67 +1657,57 @@
             # reset changes to the model in self
             self.list_models[model_name] = deepcopy(local_model_copy)
         del local_model_copy
 
         if verbose:
             print(f'Parsim Event called using input file {input_sweep_file}.')
 
-    def __get_earliest_QH_starting_time(self, row: pd.Series, t_before_QH_start: float = 0.05, t_earliest_starting_time: float = -10):
+    def __get_earliest_QH_starting_time(self, row: pd.Series, t_before_QH_start: float = 0.05,
+                                        t_earliest_starting_time: float = -10, t_latest_starting_time: float = 10):
         if 'Quench_Protection.Quench_Heaters.t_trigger' in row:
-            min_value = (min(self.__parse_string(row['Quench_Protection.Quench_Heaters.t_trigger'])))
+            min_value = (min(parse_str_to_list(row['Quench_Protection.Quench_Heaters.t_trigger'])))
+            # if all QH fire after a specified time (default 1sec), it is likely that they are switched off - so dont change default simulation starting time
+            if min_value > t_latest_starting_time: return None
             # start simulation t_before_QH_start seconds before the first Quench Heater starts
             return max(min_value - t_before_QH_start, t_earliest_starting_time)  # no values smaller then t_earliest_starting_time make sense
         else:
             if self.verbose:
                 print('No start time for Quench Heaters found in csv file. Using default simulation time.')
             return None
 
-    def __parse_string(self, s: str):
-        '''
-            this function turns:
-                - strings in the format '[1.3, 23.5, 12.4]' to a list of floats [1.3, 23.5, 12.4]
-                - strings in the format '[hallo, hallo2, hallo3]' to a list of strings [hallo, hallo2, hallo3]
-                - strings in an other format stay the same string
-            :param s: input string from csv
-            :return: parsed python datatype needed in model_data
-        '''
-        if s.startswith('[') and s.endswith(']'):
-            try:
-                # Try to split the string and convert each element to a float
-                return [float(x) for x in s[1:-1].split(',')]
-            except ValueError:
-                try:
-                    # If that fails, try to split the string and convert each element to a string
-                    return [str(x).strip() for x in s[1:-1].split(',')]
-                except ValueError:
-                    # If that also fails, return the original string
-                    raise Exception(
-                        f'The entry ({s}) in the csv file cant be read. Vector with different datatypes used.')
-        else:
-            # if no list: use normal string
-            return s
-
     def __get_circuit_family_name(self, circuit_name: str):
         if circuit_name.startswith("RCBH") or circuit_name.startswith("RCBV"):
             return "60A"
         elif circuit_name.startswith("RD"):
             return "IPD"
+        elif circuit_name.startswith("RQX"):
+            return "RQX"
+        elif circuit_name.startswith("RQ"):
+            return "RQ"
 
     def __get_magnet_name(self, circuit_name: str):
         if circuit_name.startswith("RCBH") or circuit_name.startswith("RCBV"):
             return "MCBH"
         elif circuit_name.startswith("RD"):
             circuit_type = self.__get_circuit_type(circuit_name)
             magnet_dict = {"RD1": "MBX", "RD2": "MBRC", "RD3": "MBRS", "RD4": "MBRB"}
             return magnet_dict.get(circuit_type, "")
+        elif circuit_name.startswith("RQX"):
+            return ["MQXA", "MQXB"]
+        elif circuit_name.startswith("RQ"):
+            return "MQ"
 
     def __get_number_of_magnets(self, circuit_name: str):
         circuit_family_name = self.__get_circuit_family_name(circuit_name)
         if circuit_family_name in ["60A", "IPD"]:
             return 1
+        elif circuit_family_name == "RQ":
+            return 47  # deal with 51 later
+        elif circuit_family_name == "RQX":
+            return 4
 
     def __get_number_of_apertures(self, circuit_name: str):
         circuit_family_name = self.__get_circuit_family_name(circuit_name)
         if circuit_family_name == "IPQ":
             return 2
         else:
             return 1
@@ -1693,18 +1716,25 @@
         list = []
         for i in range(1, number_of_magnets+1):
             list.append(i)
         return list
 
     def __get_magnet_types_list(self, number_of_magnets: int):
         list = []
-        for i in range(1, number_of_magnets+1):
-            list.append(1)
+        if number_of_magnets == 4: #to be improved
+            list = [1, 2, 2, 1]
+        else:
+            for i in range(1, number_of_magnets+1):
+                list.append(1)
         return list
 
     def __get_circuit_type(self, circuit_name: str):
         if circuit_name.startswith("RCBH") or circuit_name.startswith("RCBV"):
             return "RCB"
         elif circuit_name.startswith(("RD1", "RD2", "RD3", "RD4")):
             return {"RD1": "RD1", "RD2": "RD2", "RD3": "RD3", "RD4": "RD4"}.get(circuit_name[:3], "No match found")
+        elif circuit_name.startswith("RQX"):
+            return "RQX"
+        elif circuit_name.startswith("RQ"):
+            return "RQ"
```

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/builders/BuilderFiQuS.py` & `steam_sdk-2023.4.2/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/builders/BuilderLEDET.py` & `steam_sdk-2023.4.2/steam_sdk/builders/BuilderLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/builders/BuilderModel.py` & `steam_sdk-2023.4.2/steam_sdk/builders/BuilderModel.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/builders/BuilderProteCCT.py` & `steam_sdk-2023.4.2/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/builders/BuilderPyBBQ.py` & `steam_sdk-2023.4.2/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/builders/BuilderSIGMA.py` & `steam_sdk-2023.4.2/steam_sdk/builders/BuilderSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam_sdk-2023.4.2/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/builders/Solenoids.py` & `steam_sdk-2023.4.2/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/builders/geometricFunctions.py` & `steam_sdk-2023.4.2/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml` & `steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx` & `steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataAnalysis.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataAnalysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         Level 2: Analysis step to write stimulus file from coil resistance csv file
     """
     type: Literal['WriteStimulusFile']
     output_file: str = None
     path_interpolation_file: Union[str, List[str]] = None
     n_total_magnets: int = None
     n_apertures: int = None
-    current_level: List[int] = []
+    current_level: List[float] = []
     magnets: List[int] = []
     t_offset: List[float] = []
     interpolation_type: str = None  # 'Linear' or 'Spline'
     type_file_writing: str = None  # 'w' or 'a'
     n_sampling: int = None
     magnet_types: List[int] = []
 
@@ -261,14 +261,15 @@
     model_name: str = None
     case_model: str = None
     input_file: str = None
     software: List[str] = []
     simulation_number: int = None
     strand_critical_current_measurements: List[StrandCriticalCurrentMeasurement] = []
     groups_to_coils: Dict[str, List[int]] = {}
+    groups_to_coil_length: Dict[float, List[int]] = {}
     path_output_sweeper_csv: str = None
 
 # class AnalysisStep(BaseModel):
 #     """
 #         Level 1: Class for information on the analysis step
 #         Objects of this class will be defined in AnalysisStepDefinition
 #     """
```

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataConductor.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataConductor.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataDakota.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataEventCircuit.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataEventCircuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # Powering
 class Powering(BaseModel):
     """
         Level 1: Class for information on the circuit powering
     """
     circuit_name: str = None
     circuit_type: str = None
-    delta_t_FGC_PIC: float = None  # time delay between PIC signal and power supply switching-off signal (FGC)
+    delta_t_FGC_PIC: List[float] = [] # time delay between PIC signal and power supply switching-off signal (FGC)
     current_at_discharge: List[float] = []
     dI_dt_at_discharge: List[float] = []
     plateau_duration: List[float] = []
     cause_FPA: str = None
 
 
 ############################
```

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataEventMagnet.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataFiQuS.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataLEDET.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataModelCircuit.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataModelCircuit.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataModelConductor.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataModelMagnet.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataModelMagnet.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataParsimConductor.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataParsimConductor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,90 +1,97 @@
 from typing import (List, Dict, Union, Literal)
 from pydantic import BaseModel
 
 ############################
 # General parameters
-class GeneralParameters(BaseModel):  # TODO do we need this?
+class GeneralParameters(BaseModel):
     magnet_name: str = None
     circuit_name: str = None
     state: str = None  # measured, deduced from short-samples, deduced from design
 
 ############################
 # Magnet
 class Magnet(BaseModel):
     coils: List[str] = []
-    measured_inductance_versus_current: List[List[float]] = []
+    measured_inductance_versus_current: List[List[float]] = []   # TODO why is this needed?
 
-############################
-# Coils
-class Coil(BaseModel):
-    ID: str = None
-    cable_ID: str = None
-    coil_length: float = None
-    coil_RRR: float = None
-    T_ref_RRR_low: float = None
-    T_ref_RRR_high: float = None
-    coil_resistance_room_T: float = None
-    T_ref_coil_resistance: float = None
-    conductors: List[str] = []  # TODO: make sure that names correspond to conductor instances - maybe call it sample?
-    weight_conductors: List[float] = []
+# ############################
+# # Coils
+# class Coil(BaseModel):
+#     ID: str = None
+#     cable_ID: str = None
+#     coil_length: float = None
+#     coil_RRR: float = None
+#     T_ref_RRR_low: float = None
+#     T_ref_RRR_high: float = None
+#     coil_resistance_room_T: float = None
+#     T_ref_coil_resistance: float = None
+#     conductors: List[str] = []
+#     weight_conductors: List[float] = []
 
 ############################
 # Conductors
 class IcMeasurement(BaseModel):
     """
         Level 1: Class for parameters of a critical current measurement to adjust Jc fit parameters
     """
     Ic: float = None
     T_ref_Ic: float = None
     B_ref_Ic: float = None
     Cu_noCu_sample: float = None
 
 
-class Round(BaseModel):
+class StrandGeometry(BaseModel):
     """
-        Level 2: Class for strand parameters
+        Level 2: Class for strand geometry
     """
-    type: Literal['Round']
     diameter: float = None
-
-class Rectangular(BaseModel):
-    """
-        Level 2: Class for strand parameters
-    """
-    type: Literal['Rectangular']
     bare_width: float = None
     bare_height: float = None
 
 
 class ConductorSample(BaseModel):
-    # TODO think of using other conductor class
-    ID: str = None
+    # ID: str = None
+    # Ra: float = None
+    # Rc: float = None
+    index_of_conductor_in_modelData: int = None
+    group_indices_in_modelData: List[int] = []  # TODO new
     number_of_strands: int = None
     width: float = None
     height: float = None
-    Cu_noCu: float = None
-    RRR: float = None
     strand_twist_pitch: float = None
     filament_twist_pitch: float = None
-    Ic_measurements: List[IcMeasurement] = []
+    # Resistance measurement attributes
+    coil_resistance_room_T: float = None  # TODO new
+    Cu_noCu_resistance_meas: float = None   # TODO new
+    total_conductor_length: float = None  # TODO new
+    # critical current measurement attributes
     Tc0: float = None
     Bc20: float = None
     f_rho_eff: float = None
-    Ra: float = None
-    Rc: float = None
-    strand_geometry: Union[Round, Rectangular] = None
+    Ic_measurements: List[IcMeasurement] = []
+    strand_geometry: StrandGeometry = StrandGeometry()
+    # weighted entries with weight factors
+    weight_factors: List[float] = []
+    RRR: List[float] = []
+    Cu_noCu: List[float] = []
+    # names of entries that can be weighted as a read-only attribute
+    _names_of_attributes_to_weight: List[str] = ['RRR', 'Cu_noCu']
+    @property
+    def names_of_attributes_to_weight(self) -> List[str]:
+        return self._names_of_attributes_to_weight
+
 
 
 class DataParsimConductor(BaseModel):
     '''
         **Class for the STEAM conductor**
 
         This class contains the data structure of a Conductor parsim  analyzed with STEAM_SDK.
 
         :return: DataParsimConductor object
     '''
 
     GeneralParameters: GeneralParameters = GeneralParameters()
     Magnet: Magnet = Magnet()
-    Coils: Dict[str, Coil] = {}
+    # Coils: Dict[str, Coil] = {}
     ConductorSamples: Dict[str, ConductorSample] = {}
```

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataProteCCT.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataPyBBQ.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataRoxieParser.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataSettings.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataSettings.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DataSignal.py` & `steam_sdk-2023.4.2/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DictionaryLEDET.py` & `steam_sdk-2023.4.2/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DictionaryProteCCT.py` & `steam_sdk-2023.4.2/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/DictionaryPyBBQ.py` & `steam_sdk-2023.4.2/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/TemplateLEDET.py` & `steam_sdk-2023.4.2/steam_sdk/data/TemplateLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/data/TemplateProteCCT.py` & `steam_sdk-2023.4.2/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/drivers/DriverAnalysis.py` & `steam_sdk-2023.4.2/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/drivers/DriverDakota.py` & `steam_sdk-2023.4.2/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/drivers/DriverFiQuS.py` & `steam_sdk-2023.4.2/steam_sdk/drivers/DriverFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/drivers/DriverLEDET.py` & `steam_sdk-2023.4.2/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/drivers/DriverPSPICE.py` & `steam_sdk-2023.4.2/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/drivers/DriverProteCCT.py` & `steam_sdk-2023.4.2/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/drivers/DriverPyBBQ.py` & `steam_sdk-2023.4.2/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/drivers/DriverSIGMA.py` & `steam_sdk-2023.4.2/steam_sdk/drivers/DriverSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/drivers/DriverXYCE.py` & `steam_sdk-2023.4.2/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/drivers/temp/postLEDET.py` & `steam_sdk-2023.4.2/steam_sdk/drivers/temp/postLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/drivers/temp/runLEDET.py` & `steam_sdk-2023.4.2/steam_sdk/drivers/temp/runLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/drivers/temp/simLEDET.py` & `steam_sdk-2023.4.2/steam_sdk/drivers/temp/simLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/CSD_Reader.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserCond2d.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserCsd.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserCsv.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserDakota.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserDatToCsv.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserDatToCsv.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserExcel.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserFiQuS.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserLEDET.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserMap2d.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserMat.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserMat.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserPSPICE.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserPdf.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserProteCCT.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserProtePyBBQ.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserProtePyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserRoxie.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserTdms.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserXYCE.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserXYCE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/ParserYAML.py` & `steam_sdk-2023.4.2/steam_sdk/parsers/ParserYAML.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsers/templates/template_Dakota.in` & `steam_sdk-2023.4.2/steam_sdk/parsers/templates/template_Dakota.in`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsims/ParsimConductor.py` & `steam_sdk-2023.4.2/steam_sdk/parsims/ParsimConductor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 import csv
-import math
 import warnings
-import time
+import math
 
+from scipy.optimize import fsolve
 import numpy as np
 import pandas as pd
+import steammaterials
+from steammaterials.STEAM_materials import STEAM_materials
 import os
+import yaml
 from typing import List, Dict
 
-from steam_sdk.data.DataParsimConductor import DataParsimConductor, Coil, Round, Rectangular, IcMeasurement
+from steam_sdk.data.DataParsimConductor import DataParsimConductor, IcMeasurement
+from steam_sdk.parsers.ParserMap2d import getParametersFromMap2d
+from steam_sdk.utils.get_attribute_type import get_attribute_type
 from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 from steam_sdk.utils.sgetattr import rsetattr, rgetattr
 from steam_sdk.data.DataParsimConductor import ConductorSample
-# TODO why dont we just use Conductor from DataConductor and read all the data into that class and then write the csv from that class?
-
+from steam_sdk.utils.parse_str_to_list import parse_str_to_list
 
 
 class ParsimConductor:
     """
 
     """
 
-    def __init__(self, model_data_conductors, verbose: bool = True):
+    def __init__(self, model_data, groups_to_coils, groups_to_coil_length, dict_coilName_to_conductorIndex, verbose: bool = True):
         """
         If verbose is read to True, additional information will be displayed
         """
         # Unpack arguments
-        self.model_data_conductors = model_data_conductors
         self.verbose: bool = verbose
+        self.model_data = model_data
+        self.dict_coilName_to_conductorIndex = dict_coilName_to_conductorIndex
+        self.groups_to_coils = groups_to_coils
+
+        # groups_to_coil_length is either None (coil_length will be optimized) or dict
+        self.number_of_groups = max([max(values) for values in self.groups_to_coils.values()])
+        if groups_to_coil_length and type(groups_to_coil_length) == float:
+            expected_group_numbers = list(range(1, self.number_of_groups + 1))
+            self.groups_to_coil_length = {groups_to_coil_length: expected_group_numbers}
+        else:
+            self.groups_to_coil_length = groups_to_coil_length
 
         # DataParsimConductor object that will hold all the information from the input csv file
         self.data_parsim_conductor = DataParsimConductor()
 
     def read_from_input(self, path_input_file: str, magnet_name: str, strand_critical_current_measurements: Dict[str, Dict]):
         '''
         Read a .csv file and assign its content to a instance of DataParsimConductor().
@@ -61,41 +75,39 @@
         # delete all rows of dataframe that don't belong to the magnet
         mask = df_conductors[column_name_magnets] != magnet_name  # create a boolean mask for the rows that do not have the value in the column
         df_conductors = df_conductors.drop(df_conductors[mask].index)  # drop the rows that do not have the value in the column
 
         # Assign the content to a dataclass structure - loop over all the coils of the magnet in the database
         for _, row in df_conductors.iterrows():
             self.__read_magnet(row, column_name_coils, parsed_columns)
-            self.__read_coils(row, column_name_coils, parsed_columns)
-            self.__read_conductors(row, column_name_coils, parsed_columns, strand_critical_current_measurements)
+            # self.__read_coils(row, column_name_coils, parsed_columns)
+            self.read_conductors(row, column_name_coils, parsed_columns, strand_critical_current_measurements)
 
         # show the user all the columns that where ignored by the code
         ignored_column_names = list(set(df_conductors.columns) - set(parsed_columns))
         if self.verbose: print(f'Names of ignored columns: {ignored_column_names}')
 
-    def write_conductor_parameter_file(self, path_output_file: str, simulation_name: str, simulation_number: int,
-                                       dict_coilname_to_conductorindex: Dict[str, int]):
+    def write_conductor_parameter_file(self, path_output_file: str, simulation_name: str, simulation_number: int):
         """
         Write the Parsim Conductor information to a CSV file, that can be used to run a ParsimSweep Step.
 
         Parameters:
             path_output_file (str): path to the output file
+            groups_to_coil_length: None, float or dict
         """
 
         # Make target folder if it is missing
         make_folder_if_not_existing(os.path.dirname(path_output_file))
 
         # save all conductor parameters in a dict
         dict_sweeper = dict()
         dict_sweeper['simulation_name'] = simulation_name
         dict_sweeper['simulation_number'] = int(simulation_number)
-        # self.__write_parsweep_general_parameters(dict_sweeper) # no function needed, just one line of code
-        self.__write_parsweep_magnet(dict_sweeper)
-        self.__write_parsweep_coils(dict_sweeper)
-        self.__write_parsweep_conductors(dict_sweeper, dict_coilname_to_conductorindex)
+        self.__write_parsweep_conductors(dict_sweeper)
+        if not self.groups_to_coil_length: self.__write_parsweep_half_turn_length(dict_sweeper)
 
         # open file in writing mode and write the dict of the parameters as a row in the sweeper csv file
         with open(path_output_file, 'w', newline='') as csv_file:
             writer = csv.DictWriter(csv_file, fieldnames=dict_sweeper.keys())
             writer.writeheader()
             writer.writerow(dict_sweeper)
 
@@ -140,304 +152,309 @@
         rsetattr(self.data_parsim_conductor, 'GeneralParameters.magnet_name', magnet_name)
 
 
     def __read_magnet(self, row, column_name_coils, parsed_columns):
         # add coil name to Coils list
         self.data_parsim_conductor.Magnet.coils.append(row[column_name_coils])
 
-
-    def __read_coils(self, row, column_name_coils, parsed_columns):
-        '''
-            Parses a row of the conductor input csv and creates a Coil instance for the current magnet.
-
-            Args:
-                row (pandas.Series): a row of the coils input file
-                parsed_columns (list): a list of parsed column names
-
-            Raises:
-                Exception: if the coil name is not valid or has been used before
-        '''
-
-        # create Coil instance
-        coil_name = row[column_name_coils]
-        new_Coil = Coil()
-
-        # check if coil name is valid
-        if coil_name not in self.data_parsim_conductor.Magnet.coils:
-            raise Exception(
-                'Unexpected error in steam_sdk.parsims.ParsimConductor.__read_coils(). Coil name previously not found.')
-        if coil_name in self.data_parsim_conductor.Coils.keys():
-            raise Exception(
-                f'Coil names of the magnet {self.data_parsim_conductor.GeneralParameters.magnet_name} in column {column_name_coils} have to be unique. Name {coil_name} has been used before.')
-
-        # change parameters of conductors instance
-        dict_params = {
-            'Estimated coil RRR': 'coil_RRR',
-            # 'Coil ID': 'ID', 'ID': 'ID',
-            # 'Cable ID': 'cable_ID', 'cable_ID': 'cable_ID',
-            # 'Coil length': 'coil_length', 'Coil length [m]': 'coil_length', 'Coil length [mm]': 'coil_length',
-            # 'coil_length': 'coil_length', 'coil length / half/turns [m]': 'coil_length',
-            # 'coil length / half/turns [mm]': 'coil_length',
-            # 'tot coil length [m]': 'coil_length', 'tot coil length [mm]': 'coil_length',
-            # 'tot coil length': 'coil_length',  # TODO check if this is correct
-            # 'Coil RRR': 'coil_RRR', 'coil_RRR': 'coil_RRR',
-            # 'Tref RRR low': 'T_ref_RRR_low', 'T_ref_RRR_low': 'T_ref_RRR_low',
-            # 'Tref RRR high': 'T_ref_RRR_high', 'T_ref_RRR_high': 'T_ref_RRR_high',
-            # 'Coil resistance room T': 'coil_resistance_room_T', 'coil_resistance_room_T': 'coil_resistance_room_T',
-            # 'RT coil resistance [Ohm]': 'coil_resistance_room_T', 'RT coil resistance': 'coil_resistance_room_T',
-            # 'Tref coil resistance': 'T_ref_coil_resistance', 'T_ref_coil_resistance': 'T_ref_coil_resistance',
-        }
-        for csv_col_name, coil_param_name in dict_params.items():
-            if csv_col_name in row:
-                # check dimension of input column to convert number into SI unit
-                dim = csv_col_name[csv_col_name.find('[') + 1:csv_col_name.find(']')] if '[' in csv_col_name else ''
-                # change parameter is not null and convert number into SI unit
-                if not pd.isna(row[csv_col_name]):
-                    # if the RRR value is a list, use the mean value of the list
-                    if coil_param_name is 'coil_RRR' and type(row[csv_col_name]) == str: # TODO function: get_mean_from_stringlist() and use it everywhere - maybe also with weight factor
-                        if '[' not in row[csv_col_name] or ']' not in row[csv_col_name]:
-                            raise Exception(f'Invalid input format in column "{csv_col_name}". Please specify RRR eighter with just a number (e.g. "190") or with a list (e.g. "[190, 200]"). The code will then use the mean value of the list.')
-                        val_list = [float(x) for x in row[csv_col_name].strip("[]").split(",")]
-                        mean_val = sum(val_list) / len(val_list)
-                        rsetattr(new_Coil, coil_param_name, make_value_SI(mean_val, dim))
-                    else:
-                        rsetattr(new_Coil, coil_param_name, make_value_SI(row[csv_col_name], dim))
-                # mark column as parsed
-                if csv_col_name not in parsed_columns: parsed_columns.append(csv_col_name)
-
-        # set Conductor of the Coil and set weightfactor to 1.0
-        new_Coil.conductors.append(f'conductor_{coil_name}')
-        new_Coil.weight_conductors = [1.0]  # TODO: by default avg - when weight factor specified: use that
-
-        # append new coil instance to Coil Dict of ParsimConductor
-        self.data_parsim_conductor.Coils.update({coil_name: new_Coil})
-
-    def __read_conductors(self, row, column_name_coils, parsed_columns, strand_critical_current_measurements):
+    def read_conductors(self, row, column_name_coils, parsed_columns, strand_critical_current_measurements):
         '''
         Function to read Conductors of ParsimConductors
 
         :param row: Series of parameters (read from csv file)
         :param parsed_columns: list of parsed table columns names
         '''
 
-        # create Conductor instance
-        coil_name = row[column_name_coils]
-        cond_name = f'conductor_{coil_name}'
+        # create ConductorSample instance
+        cond_name = row[column_name_coils]
         new_Conductor = ConductorSample()
+        new_Conductor.index_of_conductor_in_modelData = self.dict_coilName_to_conductorIndex[cond_name]
+        new_Conductor.group_indices_in_modelData = self.groups_to_coils[cond_name]
+
+        # read dict for reading columns into local dataclass
+        yaml_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "translation_dicts", "conductor_column_names.yaml")
+        with open(yaml_path, 'r') as file:
+            dict_attribute_to_column = yaml.safe_load(file) # TODO i think this is the better way...we should also use that for ParsimEventMagnet
 
         # read the critical current measurements into the local conductor dataclass
         for meas in strand_critical_current_measurements:
-            if coil_name in meas.coil_names:
+            # raise error when col name of IcMeasurement is in translation dictionary
+            for attr_name, col_names in dict_attribute_to_column.items():
+                if meas.column_name_I_critical in col_names:
+                    raise Exception(f'Invalid column name for I_critical. "{meas.column_name_I_critical}" already used for the attribute "{attr_name}". Please change.')
+                if meas.column_name_CuNoCu_short_sample in col_names:
+                    raise Exception(f'Invalid column name for I_critical. "{meas.column_name_CuNoCu_short_sample}" already used for the attribute "{attr_name}". Please change.')
+
+            if cond_name in meas.coil_names:
                 # create new IcMeasurement instance, add all values and append it to the measurement list of the conductor
                 new_Ic_meas = IcMeasurement()
                 # add temperature and magnetic flux of the measurements (directly given in step definition)
                 rsetattr(new_Ic_meas, 'B_ref_Ic', meas.reference_mag_field)
                 rsetattr(new_Ic_meas, 'T_ref_Ic', meas.reference_temperature)
                 # read critical current form csv file
                 if meas.column_name_I_critical in row and not pd.isna(row[meas.column_name_I_critical]):
                     dim = meas.column_name_I_critical[meas.column_name_I_critical.find('[') + 1:meas.column_name_I_critical.find(']')] if '[' in meas.column_name_I_critical else ''
                     rsetattr(new_Ic_meas, 'Ic', make_value_SI(row[meas.column_name_I_critical], dim))
                 else:
-                    raise Exception(f'Provided coulumn name for Ic measurement "{meas.column_name_I_critical}" was not found in the conductor database or is empty.')
+                    raise Exception(f'Provided coulumn name for Ic measurement "{meas.column_name_I_critical}" was not found in the conductor database or is empty for coil {cond_name}.')
                 # read CuNoCu ratio of the short sample measurement
                 if meas.column_name_CuNoCu_short_sample in row and not pd.isna(row[meas.column_name_CuNoCu_short_sample]):
                     dim = meas.column_name_CuNoCu_short_sample[meas.column_name_CuNoCu_short_sample.find('[') + 1:meas.column_name_CuNoCu_short_sample.find(']')] if '[' in meas.column_name_CuNoCu_short_sample else ''
                     rsetattr(new_Ic_meas, 'Cu_noCu_sample', make_value_SI(row[meas.column_name_CuNoCu_short_sample], dim))
                 else:
                     raise Exception(f'Provided coulumn name for Ic measurement "{meas.column_name_CuNoCu_short_sample}" was not found in the conductor database or is empty.')
                 new_Conductor.Ic_measurements.append(new_Ic_meas)
 
-
-            # check if Conductor name is is valid (new conductor name corresponds to a conductor name already specified in a Coil)
-            if cond_name not in sum([coil.conductors for coil in self.data_parsim_conductor.Coils.values()], []):
-                raise Exception('Unexpected error in steam_sdk.parsims.ParsimConductor.__read_conductors(). Conductor name previously not found.')
-
-            # dict for parsing csv entries into local Conductor class
-            dict_params = {
-                'Ds [m]': 'strand_geometry.diameter', 'Ds [mm]': 'strand_geometry.diameter', 'strand_diameter': 'strand_geometry.diameter',
-                'Tc0 [K]': 'Tc0', 'Tc0': 'Tc0',
-                'Bc20 [T]': 'Bc20', 'Bc20': 'Bc20',
-                'bare strand width': 'strand_geometry.bare_width', 'strand width': 'strand_geometry.bare_width',
-                'bare strand height': 'strand_geometry.bare_height', 'strand height': 'strand_geometry.bare_height',
-                # 'Shape': 'shape', 'shape': 'shape',
-                # 'Number of strands': 'number_of_strands', 'number_of_strands': 'number_of_strands',
-                'width [m]': 'width', 'width [mm]': 'width', 'width': 'width',
-                # 'Height [m]': 'height', 'Height [mm]': 'height', 'height': 'height',
-                # 'Cu noCu': 'Cu_noCu', 'Cu_noCu': 'Cu_noCu', 'Ave Cu/noCu': 'Cu_noCu',
-                # 'RRR [-]': 'RRR',
-                'Strand twist pitch': 'strand_twist_pitch', 'strand_twist_pitch': 'strand_twist_pitch',
-                'Strand twist-pitch [m]': 'strand_twist_pitch', 'Strand twist-pitch [mm]': 'strand_twist_pitch',
-                'Filament twist pitch': 'filament_twist_pitch', 'filament_twist_pitch': 'filament_twist_pitch',
-                'Fil twist-pitch [mm]': 'filament_twist_pitch', 'Fil twist-pitch [m]': 'filament_twist_pitch',
-                # 'F rho eff': 'f_rho_eff', 'f_rho_eff': 'f_rho_eff',
-                # 'Ra [Ohm]': 'Ra',
-                # 'Rc [Ohm]': 'Rc'
-            }
-
-
-            # change parameters of conductors instance
-            for csv_col_name, conductor_name in dict_params.items():
-                if csv_col_name in row:
-                    # check dimension of input column to convert number into SI unit
-                    dim = csv_col_name[csv_col_name.find('[') + 1:csv_col_name.find(']')] if '[' in csv_col_name else ''
-                    # check if value is set in csv file
-                    if not pd.isna(row[csv_col_name]):
-                        # set geometry object (Round, Rectangular) of conductor
-                        if 'strand_geometry' in conductor_name: self.__set_conductor_geometry(new_Conductor, conductor_name)
-                        # change parameter and convert number into SI unit
-                        rsetattr(new_Conductor, conductor_name, make_value_SI(row[csv_col_name], dim))
-                    # mark column as parsed
-                    if csv_col_name not in parsed_columns: parsed_columns.append(csv_col_name)
-
-            # read coil RRR and insert it into the conductor
-            new_Conductor.RRR = self.data_parsim_conductor.Coils[row[column_name_coils]].coil_RRR
-
-            # append new conductor instance to Conductors dictionary of ParsimConductor
-            self.data_parsim_conductor.ConductorSamples.update({cond_name: new_Conductor})
-
-    def __set_conductor_geometry(self, new_Conductor, conductor_name: str):
-        # NOTE: the user can either specify the strand diameter or the strand bare width/height
-        #   - based on what he specifies either a Round or a Rectangular object is created
-        #   - when he tries to provide both an error will be raised
-
-        geometry_property = conductor_name.split('strand_geometry.')[1]
-
-        # if geometry object is not set, add the object that corresponds to entries in the csv that the user wants to change
-        if not new_Conductor.strand_geometry:
-            if geometry_property == 'diameter':
-                new_Conductor.strand_geometry = Round(type='Round')
-            elif geometry_property in ['bare_width', 'bare_height']:
-                new_Conductor.strand_geometry = Rectangular(type='Rectangular')
+        # change parameters of conductors instance according to yaml translation file
+        for attribute_name, column_names in dict_attribute_to_column.items():
+            # check if only one column for the attribute can be found
+            used_column_names = [entry for entry in column_names if entry in row]
+            if len(used_column_names) == 1:
+                used_column_name = used_column_names[0]
+            elif len(used_column_names) == 0:
+                warnings.warn(f'No column for ConductorSample attribute "{attribute_name}" found.')
+                continue
             else:
-                raise Exception(f'Tried to set an unknown geometry property. "{conductor_name}" not defined in DataParsimConductor.')
+                raise ValueError(f"More then one column for the ConductorSample attribute '{attribute_name}' found.")
 
-        # if a geometry object is set, check if the parameter that the user wants to change is in line with the shape of the conductor
-        if new_Conductor.strand_geometry:
-            if geometry_property == 'diameter':
-                if not isinstance(new_Conductor.strand_geometry, Round):
-                    raise Exception('Tried to set diameter after previously setting strand width/height. Only define either diameter or width/height depending on the shape of the conductor.')
-            elif geometry_property in ['bare_width', 'bare_height']:
-                if not isinstance(new_Conductor.strand_geometry, Rectangular):
-                    raise Exception('Tried to set strand width/height after previously setting strand diameter. Only define either diameter or width/height depending on the shape of the conductor.')
-            else:
-                raise Exception(f'Tried to set an unknown geometry property. "{conductor_name}" not defined in DataParsimConductor.')
+            # check dimension of input column to convert number into SI unit - if
+            dim = used_column_name[used_column_name.find('[') + 1:used_column_name.find(']')] if '[' in used_column_name else ''
+            # check if value is set in csv file
+            if not pd.isna(row[used_column_name]):
+                # if input is a float list in string format, parse it into a string
+                if get_attribute_type(new_Conductor, attribute_name)[0] == List[float]:
+                    if isinstance(row[used_column_name], str):
+                        float_list = parse_str_to_list(row[used_column_name], only_float_list=True)
+                    else: float_list = [row[used_column_name]]
+                    rsetattr(new_Conductor, attribute_name, [make_value_SI(val, dim) for val in float_list])
+                else:
+                    # change parameter and convert number into SI unit
+                    rsetattr(new_Conductor, attribute_name, make_value_SI(row[used_column_name], dim))
+            # mark column as parsed
+            if used_column_name not in parsed_columns: parsed_columns.append(used_column_name)
+
+        # check if only either diameter or bare w/h is set and check if original conductor type is the right one
+        original_conductor_type = self.model_data.Conductors[new_Conductor.index_of_conductor_in_modelData].strand.type
+        if original_conductor_type == 'Round':
+            if new_Conductor.strand_geometry.bare_width or new_Conductor.strand_geometry.bare_height:
+                raise Exception(f'Tried to change bare with/height of Round conductor named {cond_name}')
+        elif original_conductor_type == 'Rectangular':
+            if new_Conductor.strand_geometry.diameter:
+                raise Exception(f'Tried to change diameter of Rectangular conductor named {cond_name}')
+        else:
+            raise Exception(f'Unknown conductor type {original_conductor_type} for for conductor {cond_name}.')
 
+        # append new conductor instance to Conductors dictionary of ParsimConductor
+        self.data_parsim_conductor.ConductorSamples.update({cond_name: new_Conductor})
 
+    def __write_parsweep_half_turn_length(self, dict_sweeper):
+        # create empty list to later fill with optimized values
+        half_turn_length = [None for _ in range(self.number_of_groups)]
 
-    def __write_parsweep_magnet(self, dict_sweeper):
-        # TODO conversion of the conductor groups
-        # TODO Jc fit parameters from Ic measurements
-        # TODO calculate average f_Cu
-        # TODO calculate average RRR
-        # TODO calculate coil length based on RT resistance
-        pass
+        # looping through the conductor sample list
+        for name, conductor_sample in self.data_parsim_conductor.ConductorSamples.items():
+            original_conductor = self.model_data.Conductors[conductor_sample.index_of_conductor_in_modelData]
+            for index in conductor_sample.group_indices_in_modelData:
+                half_turn_length[index-1] = self.optimize_coil_length_with_resistance_meas(conductor_sample, original_conductor, dict_sweeper)
 
-    def __write_parsweep_coils(self, dict_sweeper):
-        pass
+        # raise Exception if there is still a None value in half_turn_length
+        if not all(item is not None for item in half_turn_length):
+            raise Exception('Something went wrong when calculating the half_turn_length. Not every listentry could be calculated.')
 
-    def __write_parsweep_conductors(self, dict_sweeper, dict_coilname_to_conductorindex):
+        # add the list to the sweeper dict as a string
+        dict_sweeper[f'CoilWindings.half_turn_length'] = '[' + ', '.join(str(x) for x in half_turn_length) + ']'
+
+    # TODO correction factor strand twist-pitch: f_twist_pitch = sqrt(wBare^2+(Lp_s/2)^2)/(Lp_s/2) , where w=wBare cable width, Lp_s=strand twist-pitch; if set to 2, take into account the increases of electrical resistance, ohmic loss per unit length, inter-filament and inter-strand coupling loss per unit length, and fractions of superconductor and stabilizer in the cable bare cross-section due to strand twist-pitch (default=0)
+    # R = C_rho_Cu_NIST_fit with the coil_resistance_room_T, T_ref_coil_resistance and RRR (between 273 and 4) - most people take between RT and 4K
+
+
+    def optimize_coil_length_with_resistance_meas(self, conductor_sample, original_conductor, dict_sweeper):
+        # calculate correction factor strand twist-pitch with bare cable width and strand twist pitch
+        f_twist_pitch = self.calculate_f_twist_pitch(conductor_sample, dict_sweeper, original_conductor)
+
+        # get number of half turns from map2d file if present
+        if self.model_data.Sources.magnetic_field_fromROXIE:
+            path_map2d = self.model_data.Sources.magnetic_field_fromROXIE
+            number_of_ht, _, _, _, _, _, _, _ = getParametersFromMap2d(map2dFile=path_map2d) # TODO test this in AnalysisSTEAM
+        else:
+            number_of_ht = self.model_data.CoilWindings.n_half_turn_in_group
+
+        # define function to solve
+        def resistance_as_function_of_L(L, *args):
+            fCu, A_cond, temperature, mag_field, RRR, Tup_RRR  = args  # unpack arguments
+            numpy2d = np.vstack((temperature, mag_field, RRR, Tup_RRR))  # create parameter v stack for c function
+            matpath = os.path.dirname(steammaterials.__file__)
+            CFUN_rhoCuNIST = STEAM_materials('CFUN_rhoCuNIST', numpy2d.shape[0], numpy2d.shape[1], matpath)
+            rho = CFUN_rhoCuNIST.evaluate(numpy2d)[0]
+            return rho * L / (fCu * A_cond) * f_twist_pitch
+
+        # define parameters needed for function
+        fCu = conductor_sample.Cu_noCu_resistance_meas / (1 + conductor_sample.Cu_noCu_resistance_meas)  # TODO is this formula correct?
+        key_RRR = f'Conductors[{conductor_sample.index_of_conductor_in_modelData}].strand.RRR'
+        if key_RRR in dict_sweeper: RRR = dict_sweeper[key_RRR]  # use RRR from database - if not existing use modelData
+        else: RRR = original_conductor.strand.RRR
+        A_cond = calc_strand_area(strand_geometry=conductor_sample.strand_geometry, original_conductor=original_conductor) # TODO is this right?
+        temperature = 273  # TODO hardcoded RT?
+        mag_field = 0  # TODO hardcoded?
+        Tup_RRR  = 273  # TODO i need to know what the function exactely needs
+
+        # solve equation for magnetic length
+        args = (fCu, A_cond, temperature, mag_field, RRR, Tup_RRR )
+        if self.model_data.GeneralParameters.magnetic_length:
+            initial_guess = [self.model_data.GeneralParameters.magnetic_length]
+        else: initial_guess = [10]
+        L = fsolve(func=resistance_as_function_of_L, x0=initial_guess, args=args)
+        L_ht = L[0] / number_of_ht
+        return L_ht
+    
+    def calculate_f_twist_pitch(self, conductor_sample, dict_sweeper, original_conductor):
+        # get the bare_cable_width from the database if it has been changed, if not: use the default one from model_data
+        key_bare_cable_width = f'Conductors[{conductor_sample.index_of_conductor_in_modelData}].cable.bare_cable_width'
+        if key_bare_cable_width in dict_sweeper:
+            bare_cable_width = dict_sweeper[key_bare_cable_width]
+        else:
+            bare_cable_width = original_conductor.cable.bare_cable_width
+
+        # get the strand_twist_pitch from the database if it has been changed, if not: use the default one from model_data
+        key_strand_twist_pitch = f'Conductors[{conductor_sample.index_of_conductor_in_modelData}].cable.strand_twist_pitch'
+        if key_strand_twist_pitch in dict_sweeper:
+            strand_twist_pitch = dict_sweeper[key_strand_twist_pitch]
+        else:
+            strand_twist_pitch = original_conductor.cable.strand_twist_pitch
+            
+        # calculate correction factor strand twist-pitch
+        f_twist_pitch = np.sqrt(bare_cable_width ** 2 + (strand_twist_pitch / 2) ** 2) / (strand_twist_pitch / 2)  # TODO should be around 1.03-1.05
+        return f_twist_pitch
+
+
+    def __write_parsweep_conductors(self, dict_sweeper):
         """
         Writes the Conductor parameter for a sweeper csv file to a dict.
 
         Parameters:
         - dict_sweeper (dict): input dict where the sweeper entries will be stored  int the format {columnName: value}
-        - dict_coilname_to_conductorindex (dict): input dict that specifies what column corresponds to what conductor index in the model {coilName: conductorIndex}
+        - dict_coilName_to_conductorIndex (dict): input dict that specifies what column corresponds to what conductor index in the model {coilName: conductorIndex}
 
         """
         # parameter dict for creating the column names of sweeper csv file
         dict_param = {
             # format {parameter_name_of_conductor_object: parameter_name_of_DataModelMagnet_object}
             'strand_geometry.diameter': 'strand.diameter',
+            'strand_geometry.bare_width': 'strand.bare_width',
+            'strand_geometry.bare_height': 'strand.bare_height',
             'RRR': 'strand.RRR',
+            'Cu_noCu': 'strand.Cu_noCu_in_strand',
             'width': 'cable.bare_cable_width',  # TODO is this correct?
             'filament_twist_pitch': 'strand.fil_twist_pitch',
             'strand_twist_pitch': 'cable.strand_twist_pitch',
         }
 
         # looping through the conductor list
-        for conductor_name, conductor in self.data_parsim_conductor.ConductorSamples.items():
-            # get the number of the conductor from his name
-            coil_name = conductor_name[len("conductor_"):]
-            if coil_name in dict_coilname_to_conductorindex:
-                idx = dict_coilname_to_conductorindex[coil_name]
-            else:
-                raise Exception(f'Conductor named "{coil_name}" could not be found in conductor database.')
+        for name, conductor_sample in self.data_parsim_conductor.ConductorSamples.items():
+            idx = conductor_sample.index_of_conductor_in_modelData
             sweeper_cond_name = f'Conductors[{idx}].'
 
             # parse data from DataParsimConductor to strings for sweeper csv and store them in dict_sweeper
-            for cond_object_name, sweeper_name in dict_param.items():
-                # skip parameters of strand_geometry if the geometry was never set, meaning no strand geometry value was provided
-                if 'strand_geometry' in cond_object_name and not conductor.strand_geometry:
-                    continue
-                if rgetattr(conductor, cond_object_name):
+            for sample_attribute_name, conductor_attribute_name in dict_param.items():
+                if rgetattr(conductor_sample, sample_attribute_name):
                     # check if conductor is rutherford before changing strand twist pitch
-                    if cond_object_name == 'strand_twist_pitch' and self.model_data_conductors[idx].cable.type != 'Rutherford':
+                    if sample_attribute_name == 'strand_twist_pitch' and self.model_data.Conductors[idx].cable.type != 'Rutherford':
                         raise Exception(f'Tried to change strand twist pitch property of a non Rutherford cable.')
                     # add value to the sweeper dict
-                    dict_sweeper[sweeper_cond_name + sweeper_name] = rgetattr(conductor, cond_object_name)
+                    val = rgetattr(conductor_sample, sample_attribute_name)
+                    if sample_attribute_name in conductor_sample.names_of_attributes_to_weight:
+                        dict_sweeper[sweeper_cond_name + conductor_attribute_name] = weight_list(val, conductor_sample.weight_factors)
+                    else:
+                        dict_sweeper[sweeper_cond_name + conductor_attribute_name] = val
 
             # insert Jc fit value(s) depending on their fitting function (usual Bottura, CUDI1, CUDI3 for NbTi and Summers, Bordini for Nb3Sn)
-            Jc_dict = get_Jc_fit_params(original_conductor=self.model_data_conductors[idx], strand_geometry=conductor.strand_geometry,
-                                        Ic_measurements=conductor.Ic_measurements, Tc0=conductor.Tc0, Bc20=conductor.Bc20,
-                                        coil_name=coil_name, mag_name=self.data_parsim_conductor.GeneralParameters.magnet_name)
+            Jc_dict = get_Jc_fit_params(original_conductor=self.model_data.Conductors[idx], strand_geometry=conductor_sample.strand_geometry,
+                                        Ic_measurements=conductor_sample.Ic_measurements, Tc0=conductor_sample.Tc0, Bc20=conductor_sample.Bc20,
+                                        sample_name=name, mag_name=self.data_parsim_conductor.GeneralParameters.magnet_name)
             for name, val in Jc_dict.items():
                 if val: dict_sweeper[sweeper_cond_name + 'Jc_fit.' + name] = val
 
+            # TODO
+            if self.groups_to_coil_length:
+                val = self.optimize_fCu_with_resistance_meas(conductor_sample, self.model_data.Conductors[idx], dict_sweeper)
+                dict_sweeper[sweeper_cond_name + 'strand.Cu_noCu_in_strand'] = val
+
+    def optimize_fCu_with_resistance_meas(self, conductor_sample, original_conductor, dict_sweeper):
+        # calculate correction factor strand twist-pitch with bare cable width and strand twist pitch
+        f_twist_pitch = self.calculate_f_twist_pitch(conductor_sample, dict_sweeper, original_conductor)
+
+        # define function to solve
+        def resistance_as_function_of_fCu(fCu, *args):
+            L, A_cond, temperature, mag_field, RRR, RRR_ref = args  # unpack arguments
+            numpy2d = np.vstack((temperature, mag_field, RRR, RRR_ref))  # create parameter v stack for c function
+            matpath = os.path.dirname(steammaterials.__file__)
+            CFUN_rhoCuNIST = STEAM_materials('CFUN_rhoCuNIST', numpy2d.shape[0], numpy2d.shape[1], matpath)
+            rho = CFUN_rhoCuNIST.evaluate(numpy2d)  # TODO check dimension (1x1 array)
+            return rho * L / (fCu * A_cond) * f_twist_pitch
+
+        # solve equation for fraction of Copper
+        args = (1, 0.2, 273, 0, 100, 1)  # TODO: copy from optimize_L_with_resistance_meas if working
+        if original_conductor.strand.Cu_noCu_in_strand:
+            initial_guess = [original_conductor.strand.Cu_noCu_in_strand]
+        else: initial_guess = [0.1]
+        fCu = fsolve(func=resistance_as_function_of_fCu, x0=initial_guess, args=args)
+        Cu_noCu = fCu[0] / (1 - fCu[0])
+        if Cu_noCu < 0.01:
+            Cu_noCu = 0.01  # TODO delete this and find cause of problem
+        return Cu_noCu
+
+
 
-def get_Jc_fit_params(original_conductor, strand_geometry, Tc0, Bc20, Ic_measurements, coil_name, mag_name):
+def get_Jc_fit_params(original_conductor, strand_geometry, Tc0, Bc20, Ic_measurements, sample_name, mag_name):
     # TODO: use C-python-wrapper functions(see steam-materials-library) - ask Mariusz how to set it up (when it is implemented)
     if original_conductor.Jc_fit.type == 'Summers':
         # check inputs
-        if not original_conductor.strand.type: raise Exception(f'Strand type of conductor in coil {coil_name} is not specified in modelData.')
+        if not original_conductor.strand.type: raise Exception(f'Strand type of conductor in coil {sample_name} is not specified in modelData.')
         if len(Ic_measurements) > 1:
-            raise Exception(f'More then one Measurement for Summers fit provided for coil {coil_name}. Please only provide 1 or 0.')
+            # TODO we could solve the overdetermined system of equations with Least Squares algorithms, like numpy.linalg.lstsq
+            raise Exception(f'More then one Measurement for Summers fit provided for coil {sample_name}. Please only provide 1 or 0.')
         elif len(Ic_measurements) < 1:
-            warnings.warn(f'No Measurement for Summers fit provided for coil {coil_name}. Calculation of new Summers parameters will be skipped.')
+            warnings.warn(f'No Measurement for Summers fit provided for coil {sample_name}. Calculation of new Summers parameters will be skipped.')
             return {}
         else:
             Ic_measurement = Ic_measurements[0]
-            if not Ic_measurement.Ic: raise Exception(f'No measured critical current (Ic) for Summers fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
-            if not Ic_measurement.B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for Summers fit provided for coil {coil_name}.')
-            if not Ic_measurement.T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for Summers fit provided for coil {coil_name}.')
-            if not Ic_measurement.Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for Summers fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+            if not Ic_measurement.Ic: raise Exception(f'No measured critical current (Ic) for Summers fit could be found in conductor database for coil {sample_name}. Please check column name in step definition.')
+            if not Ic_measurement.B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for Summers fit provided for coil {sample_name}.')
+            if not Ic_measurement.T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for Summers fit provided for coil {sample_name}.')
+            if not Ic_measurement.Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for Summers fit could be found in conductor database for coil {sample_name}. Please check column name in step definition.')
         
         # use parameters of modelData if they are not changed with the conductor database
         if not Tc0: Tc0 = original_conductor.Jc_fit.Tc0_Summers
         if not Bc20: Bc20 = original_conductor.Jc_fit.Bc20_Summers
 
         # calculate critical current density from critical current by using the area of
         fCu = Ic_measurement.Cu_noCu_sample / (Ic_measurement.Cu_noCu_sample+1)
         A = calc_strand_area(strand_geometry, original_conductor)
         A_noCu = A * (1-fCu)
         Jc_Tref_Bref = Ic_measurement.Ic/A_noCu
 
-        # search for the best C0
+        # search for the best C0  # TODO use np.linalg.solve?
         tol = 1e-6  # hardcoded
         if original_conductor.Jc_fit.Jc0_Summers:
             val_range = [original_conductor.Jc_fit.Jc0_Summers / 1000, original_conductor.Jc_fit.Jc0_Summers * 1000]
             print(val_range)
         else: val_range = [1e6, 1e14]
         n_iterations = math.ceil(np.log((val_range[1]-val_range[0])/tol) / np.log(10))  # from formula: width/(10**n_iterations) = tol
-        start_time = time.time()
-        print(f'number of iterations: {n_iterations}')
         for _ in range(n_iterations):
             try_CO_Summers = np.linspace(val_range[0], val_range[1], 10)
             tryJc_Summers = np.zeros(len(try_CO_Summers))
             # calculate Jc for every selected C0 value
             for j in range(len(try_CO_Summers)):
                 tryJc_Summers[j] = Jc_Nb3Sn_Summer_new(Ic_measurement.T_ref_Ic, Ic_measurement.B_ref_Ic, try_CO_Summers[j], Tc0, Bc20)
             # find indices of the list values that are higher than Jc_Tref_Bref
             tempIdx = np.where(np.array(tryJc_Summers) >= Jc_Tref_Bref)[0]
             if len(tempIdx) == 0: raise Exception('No C0 for Jc Summers fit could be found in specified value range.')
             # set new value range for net iteration
             val_range = [try_CO_Summers[tempIdx[0]-1], try_CO_Summers[tempIdx[0]]]
             C0 = try_CO_Summers[tempIdx[0]-1]
-        end_time = time.time()
-        elapsed_time = end_time - start_time
-        print(f"Elapsed time for summers: {elapsed_time:.2f} seconds")
 
         return {
                 'Jc0_Summers': C0,
                 'Tc0_Summers': Tc0,
                 'Bc20_Summers': Bc20,
                 }
     elif original_conductor.Jc_fit.type == 'Bordini':
@@ -448,147 +465,169 @@
                 'Tc0_Bordini': todo(),
                 'Bc20_Bordini': todo(),
                 }
     elif original_conductor.Jc_fit.type == 'CUDI1':
         # general equation for CUDI1: Ic = (C1 + C2*B) * (1 - T/Tc0*(1-B/Bc20)^-.59)
 
         # depending on the number of critical current measurements, use different ways to calculate C1 and C2 parameter
-        if len(Ic_measurements) > 2:
-            raise Exception(f'More then two measurements for CUDI1 fit provided in coil {coil_name}. Please only provide 2, 1 or 0.')
+        if len(Ic_measurements) not in [0, 1, 2]:
+            # TODO we could solve the overdetermined system of equations with Least Squares algorithms, like numpy.linalg.lstsq
+            raise Exception(f'More then two measurements for CUDI1 fit provided in coil {sample_name}. Please only provide 2, 1 or 0 measurements.')
         elif len(Ic_measurements) == 2:
             # if two measurements are specified, we have 2 equations and 2 unknowns -> system can be solved
 
             # check inputs and use parameters of modelData if they are not changed with the conductor database
             for Ic_measurement in Ic_measurements:
-                if not Ic_measurement.Ic: raise Exception(f'No measured critical current (Ic) for CUDI1 fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
-                if not Ic_measurement.B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
-                if not Ic_measurement.T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
-                if not Ic_measurement.Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for CUDI1 fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+                if not Ic_measurement.Ic: raise Exception(f'No measured critical current (Ic) for CUDI1 fit could be found in conductor database for coil {sample_name}. Please check column name in step definition.')
+                if not Ic_measurement.B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for CUDI1 fit provided for coil {sample_name}.')
+                if not Ic_measurement.T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for CUDI1 fit provided for coil {sample_name}.')
+                # if not Ic_measurement.Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for CUDI1 fit could be found in conductor database for coil {sample_name}. Please check column name in step definition.')
             if not original_conductor.cable.n_strands: raise Exception('No number of strands specified in modelData of the conductor that should be changed.')
             if not original_conductor.Jc_fit.Tc0_CUDI1: raise Exception('No Tc0 specified in modelData of the conductor that should be changed.')
             if not original_conductor.Jc_fit.Bc20_CUDI1: raise Exception('No Bc02 specified in modelData of the conductor that should be changed.')
             if not Tc0: Tc0 = original_conductor.Jc_fit.Tc0_CUDI1
             if not Bc20: Bc20 = original_conductor.Jc_fit.Bc20_CUDI1
 
             # convert critical current of strand to critical current of conductor by multiplying with number of strands
-            Ic_cable1 = Ic_measurements[0].Ic * original_conductor.cable.n_strands
-            Ic_cable2 = Ic_measurements[1].Ic * original_conductor.cable.n_strands
+            Ic_cable1 = Ic_measurements[0].Ic # TODO * original_conductor.cable.n_strands
+            Ic_cable2 = Ic_measurements[1].Ic # TODO * original_conductor.cable.n_strands
+
+            # # # solve system of linear equations: A*x = b - redundant way
+            # A = np.array([[1, Ic_measurements[0].B_ref_Ic], [1, Ic_measurements[1].B_ref_Ic]])
+            # b_1 = Ic_cable1 / (1 - Ic_measurements[0].T_ref_Ic / Tc0 * (1 - Ic_measurements[0].B_ref_Ic / Bc20) ** -0.59)
+            # b_2 = Ic_cable2 / (1 - Ic_measurements[1].T_ref_Ic / Tc0 * (1 - Ic_measurements[1].B_ref_Ic / Bc20) ** -0.59)
+            # b = np.array([b_1, b_2])
+            # x = np.linalg.solve(A, b,)
+
+            def CUDI1_equation_fixed_ratio(C, *args):
+                C1, C2 = C
+                Ic1, Ic2, T1, T2, Tc0, B1, B2, Bc20 = args
+
+                eq1 = Ic1 - (C1 + C2 * B1) * (1 - T1 / (Tc0 * (1 - B1 / Bc20) ** 0.59))
+                eq2 = Ic2 - (C1 + C2 * B2) * (1 - T2 / (Tc0 * (1 - B2 / Bc20) ** 0.59))
+
+                return [eq1, eq2]
+
+            initial_values = [787.327, -63.073]  # values come from magnet "MQML" in csv file "Strand and cable characteristics"
+            args = (Ic_cable1, Ic_cable2, Ic_measurements[0].T_ref_Ic, Ic_measurements[1].T_ref_Ic, Tc0,
+                    Ic_measurements[0].B_ref_Ic, Ic_measurements[1].B_ref_Ic, Bc20)
+            x = fsolve(func=CUDI1_equation_fixed_ratio, x0=initial_values, args=args)
 
-            # solve system of linear equations: A*x = b
-            A = np.array([[1, Ic_measurements[0].B_ref_Ic], [1, Ic_measurements[1].B_ref_Ic]])
-            b_1 = Ic_cable1 / (1 - Ic_measurements[0].T_ref_Ic / Tc0 * (1 - Ic_measurements[0].B_ref_Ic / Bc20) ** -0.59)
-            b_2 = Ic_cable2 / (1 - Ic_measurements[1].T_ref_Ic / Tc0 * (1 - Ic_measurements[1].B_ref_Ic / Bc20) ** -0.59)
-            b = np.array([b_1, b_2])
-            x = np.linalg.solve(A, b)
             if len(x) == 2:
                 C1, C2 = x
             else:
-                raise Exception(f'No valid solution for CUDI fitting parameters C1 and C2 could be found for coil {coil_name}.')
+                raise Exception(f'No valid solution for CUDI1 fitting parameters C1 and C2 could be found for coil {sample_name}.')
         elif len(Ic_measurements) == 1:
             # if only one measurement is provided use one equation and the ratio of C1 and C2 according to modelData and warn the user
-            warnings.warn(f'Only one Measurement for CUDI fit provided for coil {coil_name}. Ratio of C1 and C2 from modelData is used as a second equation.')
+            warnings.warn(f'Only one Measurement for CUDI1 fit provided for coil {sample_name}. Ratio of C1 and C2 from modelData is used as a second equation.')
 
             # check inputs and use parameters of modelData if they are not changed with the conductor database
-            if not Ic_measurements[0].Ic: raise Exception(f'No measured critical current (Ic) for CUDI1 fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
-            if not Ic_measurements[0].B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
-            if not Ic_measurements[0].T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
-            if not Ic_measurements[0].Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for CUDI1 fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+            if not Ic_measurements[0].Ic: raise Exception(f'No measured critical current (Ic) for CUDI1 fit could be found in conductor database for coil {sample_name}. Please check column name in step definition.')
+            if not Ic_measurements[0].B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for CUDI1 fit provided for coil {sample_name}.')
+            if not Ic_measurements[0].T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for CUDI1 fit provided for coil {sample_name}.')
+            # if not Ic_measurements[0].Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for CUDI1 fit could be found in conductor database for coil {sample_name}. Please check column name in step definition.')
             if not original_conductor.cable.n_strands: raise Exception('No number of strands specified in modelData of the conductor that should be changed.')
             if not original_conductor.Jc_fit.Tc0_CUDI1: raise Exception('No Tc0 specified in modelData of the conductor that should be changed.')
             if not original_conductor.Jc_fit.Bc20_CUDI1: raise Exception('No Bc02 specified in modelData of the conductor that should be changed.')
             if not original_conductor.Jc_fit.C1_CUDI1: raise Exception('No C1_CUDI1 specified in modelData of the conductor that should be changed.')
             if not original_conductor.Jc_fit.C2_CUDI1: raise Exception('No C2_CUDI1 specified in modelData of the conductor that should be changed.')
             if not Tc0: Tc0 = original_conductor.Jc_fit.Tc0_CUDI1
             if not Bc20: Bc20 = original_conductor.Jc_fit.Bc20_CUDI1
 
             # convert critical current of strand to critical current of conductor by multiplying with number of strands
-            Ic_cable1 = Ic_measurements[0].Ic * original_conductor.cable.n_strands
+            Ic_cable = Ic_measurements[0].Ic  # TODO why delete this "* original_conductor.cable.n_strands" - in csv we only use n_strands=1
 
             # try to read C1 over C2 ratio from modelData - if not existing use usual ratio for NbTi superconductors
             if not original_conductor.Jc_fit.C1_CUDI1 or not original_conductor.Jc_fit.C2_CUDI1:
-                warnings.warn(f'No C1 or C2 parameter defined in modelData for coil {coil_name}. Using usual ratio for NbTi superconductors.')
-                # 92073.5 and -6869.4 are hardcoded values come from magnet "MB inner layer" in csv file "Strand and cable characteristics"
-                # atan2 is a tangens calcualtion that also saves the sign of the angle
-                angle_C1_C2 = math.atan2(92073.5, -6869.4)  # saving signed angle instead of ratio to have correct signs - tan(angle_C1_C2) = C1/C2
+                warnings.warn(f'No C1 or C2 parameter defined in modelData for coil {sample_name}. Using usual ratio for NbTi superconductors.')
+                # 787.327 and -63.073 are hardcoded values come from magnet "MQML" in csv file "Strand and cable characteristics"
+                # saving signed angle instead of ratio to keep track of signs - tan(angle_C1_C2) = C1/C2
+                angle_C1_C2 = math.atan2(787.327, -63.073)  # atan2 is a tangens calcualtion that also saves the sign of the angle depending on the quadrant
+                initial_guess = [787.327, -63.073]
             else:
                 angle_C1_C2 = math.atan2(original_conductor.Jc_fit.C1_CUDI1, original_conductor.Jc_fit.C2_CUDI1)
+                initial_guess = [original_conductor.Jc_fit.C1_CUDI1, original_conductor.Jc_fit.C2_CUDI1]
 
-            # Ic = (C1 + C2*B) * (1 - T/Tc0*(1-B/Bc20)^-.59) where only C1 and C2 are unknown - second equation: tan(angle_C1_C2) = C1/C2
-            C2 = Ic_cable1 / (1 - Ic_measurements[0].T_ref_Ic / (Tc0 * (1 - Ic_measurements[0].B_ref_Ic / Bc20) ** 0.59)) / (Ic_measurements[0].B_ref_Ic + math.tan(angle_C1_C2))
-            C1 = C2 * math.tan(angle_C1_C2)
+            def CUDI1_equation_fixed_ratio(C, *args):
+                C1, C2 = C
+                Ic, T, Tc0, B, Bc20, angle_C1_C2 = args
+
+                eq1 = Ic - (C1 + C2 * B) * (1 - T / (Tc0 * (1 - B / Bc20) ** 0.59))
+                eq2 = C1 - C2 * math.tan(angle_C1_C2)
+
+                return [eq1, eq2]
+
+            # Solve the equation system
+            args = (Ic_cable, Ic_measurements[0].T_ref_Ic, Tc0, Ic_measurements[0].B_ref_Ic, Bc20, angle_C1_C2)
+            C = fsolve(func=CUDI1_equation_fixed_ratio, x0=initial_guess, args=args)
+            C1, C2 = C[0], C[1]
+
+            # old approach with analytical solution
+            # # Ic = (C1 + C2*B) * (1 - T/Tc0*(1-B/Bc20)^-.59) where only C1 and C2 are unknown - second equation: tan(angle_C1_C2) = C1/C2
+            # C2 = Ic_cable / (1 - Ic_measurements[0].T_ref_Ic / (Tc0 * (1 - Ic_measurements[0].B_ref_Ic / Bc20) ** 0.59)) / (Ic_measurements[0].B_ref_Ic + math.tan(angle_C1_C2))
+            # C1 = C2 * math.tan(angle_C1_C2)
         elif len(Ic_measurements) == 0:
             # if no measurement is provided use the usual ratio for NbTi superconductors and scale that value by cross section of superconductor and warn the user
-            warnings.warn(f'No Measurement for CUDI1 fit provided for coil {coil_name}. Usual ratio for NbTi superconductors of C1 and C2 is used and scaled by cross section of superconductor. Copper-non-copper ratio of magnet model will be used.')
+            warnings.warn(f'No Measurement for CUDI1 fit provided for coil {sample_name}. Usual ratio for NbTi superconductors of C1 and C2 is used and scaled by cross section of superconductor. Copper-non-copper ratio of magnet model will be used.')
 
             # check inputs
             if not original_conductor.cable.n_strands: raise Exception('No n_strands specified in modelData of the conductor that should be changed.')
             if not original_conductor.strand.Cu_noCu_in_strand: raise Exception('No n_strands specified in modelData of the conductor that should be changed.')
 
-            # hardcoded values come from magnet "MB inner layer" in csv file "Strand and cable characteristics"
-            C1_per_square_meter = 92073.5 / 9.41242e-06   # C1_cab/(Cable Section NbTi) #  = strandArea * nStrands * (1-fCu)
-            C2_per_square_meter = -6869.4 / 9.41242e-06   # C2_cab/(Cable Section NbTi) #  = strandArea * nStrands * (1-fCu)
+            # hardcoded values come from magnet "MQML" in csv file "Strand and cable characteristics"
             # NOTE: cab...cable, str...strand, C1_cab = C1_str * nStrands  and  C1_str = C1_str_MB / A_MB * A_thisMagnet
+            C1_per_square_meter_of_NbTi = 787.327 / 6.580e-08  # C1_cab/(Cable Section NbTi) #  = strandArea * nStrands * (1-fCu)
+            C2_per_square_meter_of_NbTi = -63.073 / 6.580e-08  # C2_cab/(Cable Section NbTi) #  = strandArea * nStrands * (1-fCu)
 
-            # scale it with the cross section of superconductor
+            # scale it with the cross-section of superconductor
             strand_cross_section = calc_strand_area(strand_geometry, original_conductor)
-            fraction_of_superconductor = 1 - original_conductor.strand.Cu_noCu_in_strand / (original_conductor.strand.Cu_noCu_in_strand+1)
-            total_NbTi_area = original_conductor.cable.n_strands * fraction_of_superconductor * strand_cross_section
-            C1 = C1_per_square_meter * total_NbTi_area
-            C2 = C2_per_square_meter * total_NbTi_area
+            fraction_of_superconductor = 1 / (original_conductor.strand.Cu_noCu_in_strand+1)
+            total_NbTi_area =  fraction_of_superconductor * strand_cross_section  # TODO why do i have to delete this? "* original_conductor.cable.n_strands" (AH97)
+            C1 = C1_per_square_meter_of_NbTi * total_NbTi_area
+            C2 = C2_per_square_meter_of_NbTi * total_NbTi_area
 
         # check if values are real and not imaginary (e.g. when Bc20 is bigger than B_ref_Ic)
         if np.iscomplex(complex(C1)) or np.iscomplex(complex(C2)):
             raise Exception(f'When calculating CUDI1 parameters (C1, C2) the values turned out to have an imaginary part. Please check the inputs.')
 
         return {
+            # TODO: shall we add a plausibility check - e.g. if the value will be changed by many orders of magnitude
             'Tc0_CUDI1': Tc0,
             'Bc20_CUDI1': Bc20,
             'C1_CUDI1': C1,
             'C2_CUDI1': C2,
                 }
     else:
         raise Exception(f'No implementation for fit type "{original_conductor.Jc_fit.type}" defined in ParsimConductor.')
 
 
 def calc_strand_area(strand_geometry, original_conductor):
     if original_conductor.strand.type == 'Round':
-        # check conductor type
-        if strand_geometry and strand_geometry.type != 'Round':
-            raise Exception(f'Type of conductor cannot be changed. Tried to change Round conductor to "{strand_geometry.type}".')
 
         # if diameter is not changed in conductor database, use the one form modeldata
-        if not strand_geometry or not strand_geometry.diameter: diameter = original_conductor.strand.diameter
+        if not strand_geometry.diameter: diameter = original_conductor.strand.diameter
         else: diameter = strand_geometry.diameter
 
         # calculate area of circle
         A = np.pi * diameter ** 2 / 4
     elif original_conductor.strand.type == 'Rectangular':
-        # check conductor type
-        if strand_geometry and strand_geometry.type != 'Rectangular':
-            raise Exception(f'Type of conductor cannot be changed. Tried to change Rectangular conductor to "{strand_geometry.type}".')
 
         # if height/width is not changed in conductor database, use the one form modeldata
-        if not strand_geometry or not strand_geometry.bare_height: h = original_conductor.strand.bare_height
+        if not strand_geometry.bare_height: h = original_conductor.strand.bare_height
         else: h = strand_geometry.bare_height
-        if not strand_geometry or not strand_geometry.bare_width: w = original_conductor.strand.bare_width
+        if not strand_geometry.bare_width: w = original_conductor.strand.bare_width
         else: w = strand_geometry.bare_width
 
         # calculate area of circle
         A = w * h
     else:
-        raise Exception(f'Unknown type of conductor: {original_conductor.strand.type}!')
+        raise Exception(f'Unknown type of conductor strand: {original_conductor.strand.type}!')
     return A
 
 
-# TODO correction factor strand twist-pitch = sqrt(wBare^2+(Lp_s/2)^2)/(Lp_s/2) , where w=wBare cable width, Lp_s=strand twist-pitch; if set to 2, take into account the increases of electrical resistance, ohmic loss per unit length, inter-filament and inter-strand coupling loss per unit length, and fractions of superconductor and stabilizer in the cable bare cross-section due to strand twist-pitch (default=0)
-# Resistance_RT = R * L / (f_Cu * A_cond) * f_twist_pitch
-# R = C_NIST_fit with the coil_resistance_room_T,  T_ref_coil_resistance and RRR (between 273 and 4))
-# search L or f_Cu - set flag what to calculate
-# L is coil length and f_Cu from csv file
-
 def Jc_Nb3Sn_Summer_new(T, B, C, Tc0, Bc20):
     if T==0: T=0.001
     if B==0: B=0.001
     frac_T = T / Tc0
     if frac_T > 1: frac_T=1
     Bc2 = Bc20 * (1 - frac_T ** 2) * (1 - 0.31 * frac_T ** 2 * (1 - 1.77 * np.log(frac_T)))
     frac_B = B / Bc2
@@ -631,14 +670,30 @@
     return Jc_T_B
 
 
 def todo():
     #TODO make functions whereever this function is used
     return None
 
+def weight_list(val, weight_factors):
+    # if there is only one entry, dont calculate
+    if len(val) == 1:
+        return val[0]
+
+    # if no weight factor specified or if weight factor length is different, take the average
+    if not weight_factors or len(val) != len(weight_factors):
+        # TODO should an exception be raised when length is different?
+        weight_factors = [1.0 for _ in val]
+
+    # Normalize the weight_factors
+    weight_sum = sum(weight_factors)
+    normalized_weights = [w / weight_sum for w in weight_factors]
+
+    return sum([v * w for v, w in zip(val, normalized_weights)])
+
 def make_value_SI(val: float, dim: str):
     if dim in ['mm', 'mOhm', 'mV']:
         return val / 1000
     elif dim in ['m', 'T', 'K', 'Ohm', 'V', '', ' ', '-']:
         return val
     elif dim in ['kA', 'kV', 'km']:
         return val * 1000
```

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsims/ParsimDakota.py` & `steam_sdk-2023.4.2/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsims/ParsimEventCircuit.py` & `steam_sdk-2023.4.2/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files 13% similar despite different names*

```diff
@@ -136,23 +136,31 @@
                 f'length of input simulation numbers ({len(simulation_numbers)}) differs from length of events found in the input file ({len(self.list_events)})')
 
         # Make target folder if it is missing
         make_folder_if_not_existing(os.path.dirname(path_outputfile_event_csv))
 
         # open file in writing mode
         all_rows = []
-
         list_paramerers = []
+
         # Loop trough each element of self.list_events and write parameters to csv
         for i, event in enumerate(self.list_events):
             print(i, event)
             new_row = {'simulation_name': simulation_name, 'simulation_number': simulation_numbers[i]}
-            new_row.update(self.__write_event(event))
-            all_rows.append(new_row)
-            list_paramerers = list(set(list_paramerers + list(new_row.keys())))  # keep track of the parameter names
+            event_data = self.__write_event(event)
+            if isinstance(event_data, list):
+                for data in event_data:
+                    new_row.update(data)
+                    all_rows.append(new_row.copy())
+                    list_paramerers = list(set(list_paramerers + list(new_row.keys())))
+            else:
+                new_row.update(event_data)
+                all_rows.append(new_row)
+                list_paramerers = list(set(list_paramerers + list(new_row.keys())))
+
         # TODO reorder the columns
         # Write file
         with open(path_outputfile_event_csv, 'w', newline='') as csv_file:
             writer = csv.DictWriter(csv_file, fieldnames=list_paramerers)
             writer.writeheader()
             for new_row in all_rows:
                 writer.writerow(new_row)
@@ -812,14 +820,18 @@
 
     def __write_event(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
         circuit_type = event.GeneralParameters.circuit_type
         if circuit_type in ['RCBH', 'RCBV']:
             event_dict = self.__write_RCB(event, t_after_PC_off=t_after_PC_off)
         elif circuit_type in ["RD1", "RD2", "RD3", "RD4"]:
             event_dict = self.__write_IPD(event, t_after_PC_off=t_after_PC_off)
+        elif circuit_type == "RQ":
+            event_dict = self.__write_RQ(event, t_after_PC_off=t_after_PC_off)
+        elif circuit_type == "RQX":
+            event_dict = self.__write_RQX(event, t_after_PC_off=t_after_PC_off)
         return event_dict
 
     def __write_RCB(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
         """
         Extract the information for an event of circuit type RCB.
 
         Parameters:
@@ -984,14 +996,186 @@
         event_dict['GlobalParameters.global_parameters.t_PC_off'] = t_PC_off
         event_dict['Analysis.simulation_time.time_end'] = t_PC_off + t_after_PC_off
         event_dict['Analysis.simulation_time.time_schedule'] = dict_time_schedule
         event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off
 
         return event_dict
 
+    def __write_RQ(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
+        """
+        Extract the information for an event of circuit type RQ.
+
+        Parameters:
+            event (DataEventCircuit): The data event object to read the data.
+
+        Returns:
+            list[dict]: A list of dictionaries containing the RQ information.
+
+        """
+        circuit_name = event.GeneralParameters.name
+        list= []
+        for i in range(2):
+            event_dict = dict()
+            t_start = 0  # hard-coded
+            I_start = 0.0  # hard-coded
+            dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
+            dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge[i]
+
+            current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge[i]
+            if dI_dt == 0:
+                I_end = current_at_discharge
+                dI_dt = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt'])
+                time_to_reach_I = self.__time_to_reach_I(I=I_end, dI_dt=dI_dt, dI_dt2=dI_dt2, I_start=I_start)
+                t_plateau = event.PoweredCircuits[circuit_name].plateau_duration[i]
+                t_PC_off = t_start + time_to_reach_I + t_plateau
+                #event_dict['GlobalParameters.global_parameters.t_plateau'] = t_plateau
+                event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end
+                event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
+
+            elif dI_dt < 0:
+                I_end_1 = 1.2*current_at_discharge
+                I_end_2 = current_at_discharge
+                t_plateau = 10  # hard-coded
+                t_PC_off = calculate_t_PC_off(t_start, I_start, [I_end_1, I_end_2], [-dI_dt, dI_dt], [dI_dt2, -dI_dt2], [t_plateau, t_plateau], I_end_2)
+                event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end_1
+                event_dict['GlobalParameters.global_parameters.I_end_2'] = I_end_2
+                event_dict['GlobalParameters.global_parameters.dI_dt'] = -dI_dt  # setting dI_dt
+                event_dict['GlobalParameters.global_parameters.dI_dt2'] = dI_dt2  # setting dI_dt2
+
+            else:
+                I_end = str(current_at_discharge) + " + 100.0"
+                I_target = current_at_discharge + 100.0
+                t_plateau = t_start + 2 * dI_dt / dI_dt2 + (I_target - I_start - dI_dt ** 2 / dI_dt2) / dI_dt
+                t_PC_off = calculate_t_PC_off(t_start, I_start,  I_target, [dI_dt], [dI_dt2], [t_plateau], I_target - 100)
+                event_dict['GlobalParameters.global_parameters.dI_dt'] = dI_dt  #setting dI_dt
+                event_dict['GlobalParameters.global_parameters.I_end_1'] = I_target - 100.0
+                event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
+
+            dict_time_schedule = {
+                '0.0': '0.5',
+                f'{t_PC_off - 1.000}': '0.100',
+                f'{t_PC_off - 0.100}': '0.010',
+                f'{t_PC_off - 0.010}': '0.001',
+                f'{t_PC_off - 0.001}': '0.0001',
+                f'{t_PC_off + 0.020}': '0.001',
+                f'{t_PC_off + 1.000}': '0.010',
+                f'{t_PC_off + 3.000}': '0.500'
+            }
+            event_dict['GlobalParameters.global_parameters.I_start'] = I_start
+            event_dict['GlobalParameters.global_parameters.t_start'] = t_start
+            event_dict['GlobalParameters.global_parameters.t_plateau'] = t_plateau
+            event_dict['GlobalParameters.global_parameters.t_PC_off'] = t_PC_off
+            event_dict['Analysis.simulation_time.time_end'] = t_PC_off + t_after_PC_off
+            event_dict['Analysis.simulation_time.time_schedule'] = dict_time_schedule
+            event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off
+
+            list.append(event_dict)
+
+        return list
+
+    def __write_RQX(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
+        """
+        Extract the information for an event of circuit type RQX.
+
+        Parameters:
+            event (DataEventCircuit): The data event object to read the data.
+
+        Returns:
+            list[dict]: A list of dictionaries containing the RQX information.
+
+        """
+        circuit_name = event.GeneralParameters.name
+        list= []
+        t_PC_off_list = []
+        acceleration_list = ["dI_dt2_PC1", "dI_dt2_PC2", "dI_dt2_PC3"]
+        ramp_rate_list = ["dI_dt_PC1", "dI_dt_PC2", "dI_dt_PC3"]
+
+        #loop to calculate list of t_PC_off
+        for i in range(3):
+            #event_dict = dict()
+            t_start = 0  # hard-coded
+            I_start = 0.0  # hard-coded
+            dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')[acceleration_list[i]])  # read dI/dt2 from the STEAM model
+            dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge[i]
+
+            current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge[i]
+
+            if dI_dt == 0:
+                I_end = current_at_discharge
+                dI_dt = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')[ramp_rate_list[i]])
+                time_to_reach_I = self.__time_to_reach_I(I=I_end, dI_dt=dI_dt, dI_dt2=dI_dt2, I_start=I_start)
+                t_plateau = event.PoweredCircuits[circuit_name].plateau_duration[i]
+                t_PC_off = t_start + time_to_reach_I + t_plateau
+
+            elif dI_dt < 0:
+                I_end_1 = 1.2*current_at_discharge
+                I_end_2 = current_at_discharge
+                t_plateau = 10  # hard-coded
+                t_PC_off = calculate_t_PC_off(t_start, I_start, [I_end_1, I_end_2], [-dI_dt, dI_dt], [dI_dt2, -dI_dt2], [t_plateau, t_plateau], I_end_2)
+
+            else:
+                I_end = str(current_at_discharge) + " + 100.0"
+                I_target = current_at_discharge + 100.0
+                t_plateau = t_start + 2 * dI_dt / dI_dt2 + (I_target - I_start - dI_dt ** 2 / dI_dt2) / dI_dt
+                t_PC_off = calculate_t_PC_off(t_start, I_start,  I_target, [dI_dt], [dI_dt2], [t_plateau], I_target - 100)
+
+            t_PC_off_list.append(t_PC_off)
+
+        t_PC_off = max(t_PC_off_list)
+        dict_time_schedule = {
+            '0.0': '0.5',
+            f'{t_PC_off - 1.000}': '0.100',
+            f'{t_PC_off - 0.100}': '0.010',
+            f'{t_PC_off - 0.010}': '0.001',
+            f'{t_PC_off - 0.001}': '0.0001',
+            f'{t_PC_off + 0.020}': '0.001',
+            f'{t_PC_off + 1.000}': '0.010',
+            f'{t_PC_off + 3.000}': '0.500'
+        }
+        #loop to write events
+        for i in range(3):
+            event_dict = dict()
+            dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge[i]
+            dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')[acceleration_list[i]])
+            current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge[i]
+            if t_PC_off_list[i] < t_PC_off:
+                t_start = t_PC_off - t_PC_off_list[i]
+            else:
+                t_start = 0
+            I_start = 0.0  # hard-coded
+            if dI_dt == 0:
+                event_dict[f'GlobalParameters.global_parameters.I_end_1_PC{i+1}'] = current_at_discharge
+                event_dict[f'GlobalParameters.global_parameters.I_end_2_PC{i+1}'] = 0.0
+                t_plateau = event.PoweredCircuits[circuit_name].plateau_duration[i]
+            elif dI_dt < 0:
+                I_end_1 = 1.2*current_at_discharge
+                I_end_2 = current_at_discharge
+                event_dict[f'GlobalParameters.global_parameters.I_end_1_PC{i+1}'] = I_end_1
+                event_dict[f'GlobalParameters.global_parameters.I_end_2_PC{i+1}'] = I_end_2
+                event_dict[f'GlobalParameters.global_parameters.dI_dt_PC{i+1}'] = -dI_dt  # setting dI_dt
+                event_dict[f'GlobalParameters.global_parameters.dI_dt2_PC{i+1}'] = dI_dt2  # setting dI_dt2
+                t_plateau = 10  # hard-coded
+            else:
+                I_target = current_at_discharge + 100.0
+                event_dict[f'GlobalParameters.global_parameters.dI_dt_PC{i+1}'] = dI_dt  #setting dI_dt
+                event_dict[f'GlobalParameters.global_parameters.I_end_1_PC{i+1}'] = I_target - 100.0
+                event_dict[f'GlobalParameters.global_parameters.I_end_2_PC{i+1}'] = 0.0
+                t_plateau = t_start + 2 * dI_dt / dI_dt2 + (I_target - I_start - dI_dt ** 2 / dI_dt2) / dI_dt
+
+            event_dict[f'GlobalParameters.global_parameters.t_PC_off_PC{i+1}'] = t_PC_off
+            event_dict['Analysis.simulation_time.time_end'] = t_PC_off + t_after_PC_off
+            event_dict['Analysis.simulation_time.time_schedule'] = dict_time_schedule
+            event_dict[f'GlobalParameters.global_parameters.I_start_PC{i+1}'] = I_start
+            event_dict[f'GlobalParameters.global_parameters.t_start_PC{i+1}'] = t_start
+            event_dict[f'GlobalParameters.global_parameters.t_plateau_PC{i + 1}'] = t_plateau
+            list.append(event_dict)
+
+        event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off
+        return list
+
     @staticmethod
     def __time_to_reach_I(I: float, dI_dt: float, dI_dt2: float, I_start: float):
         '''
         Calculate the time to reach a current assuming a parabolic, linear, and parabolic profile
         :return: time [s]
         '''
         t_parabolic = dI_dt / dI_dt2
```

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsims/ParsimEventMagnet.py` & `steam_sdk-2023.4.2/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/parsims/ParsimSweep.py` & `steam_sdk-2023.4.2/steam_sdk/parsims/ParsimSweep.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/plotters/PlotterModel.py` & `steam_sdk-2023.4.2/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/plotters/PlotterParametric.py` & `steam_sdk-2023.4.2/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/plotters/PlotterRoxie.py` & `steam_sdk-2023.4.2/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/plotters/PlotterSIGMA.py` & `steam_sdk-2023.4.2/steam_sdk/plotters/PlotterSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/postprocs/PostprocsMetrics.py` & `steam_sdk-2023.4.2/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/utils/MTF_reading_functions.py` & `steam_sdk-2023.4.2/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/utils/ModifyModelData.py` & `steam_sdk-2023.4.2/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam_sdk-2023.4.2/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/utils/ModifyModelDataconductor.py` & `steam_sdk-2023.4.2/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/utils/clean_NaN_from_signal.py` & `steam_sdk-2023.4.2/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/utils/compare_two_parameters.py` & `steam_sdk-2023.4.2/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/utils/misc.py` & `steam_sdk-2023.4.2/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/utils/tic_toc.py` & `steam_sdk-2023.4.2/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/utils/utils_PC.py` & `steam_sdk-2023.4.2/steam_sdk/utils/utils_PC.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,19 +98,22 @@
     time = Time_Current[0]
     current = Time_Current[1]
     return np.round(time[np.argmin(abs(current - I_final))], 4)
 
 
 
 def calculate_t_PC_off_one(t_start: float, I_start: float, I_end: float, dI_dt: float, dI_dt_2: float, t_plateau: float, I_off: float):
-    delta_t_parabolic = dI_dt / dI_dt_2
+    delta_t_parabolic = abs(dI_dt / dI_dt_2)
     delta_I_parabolic = 0.5 * dI_dt_2 * delta_t_parabolic ** 2
     delta_I_linear = I_end - I_start - 2 * delta_I_parabolic
-    delta_t_linear = delta_I_linear / dI_dt
-    if delta_I_parabolic < 0:
+    delta_t_linear = abs(delta_I_linear / dI_dt)
+    if I_off < 2 * delta_I_parabolic:
+        I_off = 0
+        raise Exception('I_target < 2 * I_parabolic')
+    elif delta_I_parabolic < 0: # case to be discussed before removal
         delta_t_linear = (I_end - I_start - delta_I_parabolic)/dI_dt
         t_PC_off = t_start + delta_t_parabolic + delta_t_linear
     elif I_off < I_start + delta_I_parabolic:
         t_PC_off = t_start + np.sqrt( (I_off - I_start) / 0.5 / dI_dt_2)
     elif I_off < I_start + delta_I_parabolic + delta_I_linear:
         t_PC_off = t_start + delta_t_parabolic + (I_off - I_start - delta_I_parabolic) / dI_dt
     elif I_off < I_start + delta_I_parabolic + delta_I_linear + delta_I_parabolic:
```

### Comparing `steam_sdk-2023.4.1/steam_sdk/viewers/Viewer.py` & `steam_sdk-2023.4.2/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/viewers/ViewerMeas.py` & `steam_sdk-2023.4.2/steam_sdk/viewers/ViewerMeas.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/viewers/ViewerSim.py` & `steam_sdk-2023.4.2/steam_sdk/viewers/ViewerSim.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/wrappers/java/SING/jars/steam-sing.jar` & `steam_sdk-2023.4.2/steam_sdk/wrappers/java/SING/jars/steam-sing.jar`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk/wrappers/wrapper_yaml.py` & `steam_sdk-2023.4.2/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.1/steam_sdk.egg-info/PKG-INFO` & `steam_sdk-2023.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: steam-sdk
-Version: 2023.4.1
+Name: steam_sdk
+Version: 2023.4.2
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: STEAM,CERN,SDK,API
+Keywords: CERN,API,STEAM,SDK
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam_sdk-2023.4.1/steam_sdk.egg-info/SOURCES.txt` & `steam_sdk-2023.4.2/steam_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 steam_sdk/parsims/ParsimConductor.py
 steam_sdk/parsims/ParsimDakota.py
 steam_sdk/parsims/ParsimEventCircuit.py
 steam_sdk/parsims/ParsimEventMagnet.py
 steam_sdk/parsims/ParsimSweep.py
 steam_sdk/parsims/Readme.md
 steam_sdk/parsims/__init__.py
+steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
 steam_sdk/plotters/PlotterModel.py
 steam_sdk/plotters/PlotterParametric.py
 steam_sdk/plotters/PlotterRoxie.py
 steam_sdk/plotters/PlotterSIGMA.py
 steam_sdk/plotters/Readme.md
 steam_sdk/plotters/__init__.py
 steam_sdk/postprocs/PostprocsMetrics.py
@@ -141,17 +142,19 @@
 steam_sdk/utils/ModifyModelData.py
 steam_sdk/utils/ModifyModelDataMagnet.py
 steam_sdk/utils/ModifyModelDataconductor.py
 steam_sdk/utils/NumpyEncoder.py
 steam_sdk/utils/__init__.py
 steam_sdk/utils/clean_NaN_from_signal.py
 steam_sdk/utils/compare_two_parameters.py
+steam_sdk/utils/get_attribute_type.py
 steam_sdk/utils/isNaN.py
 steam_sdk/utils/make_folder_if_not_existing.py
 steam_sdk/utils/misc.py
+steam_sdk/utils/parse_str_to_list.py
 steam_sdk/utils/rgetattr.py
 steam_sdk/utils/rhasattr.py
 steam_sdk/utils/sgetattr.py
 steam_sdk/utils/tic_toc.py
 steam_sdk/utils/unique.py
 steam_sdk/utils/utils_PC.py
 steam_sdk/viewers/Viewer.py
```

### Comparing `steam_sdk-2023.4.1/steam_sdk.egg-info/requires.txt` & `steam_sdk-2023.4.2/steam_sdk.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 ruamel.yaml==0.17.21
 ruamel.yaml.clib==0.2.6
 scipy==1.9.1
 seaborn==0.12.0
 six==1.16.0
 smmap==5.0.0
 stack-data==0.5.0
-STEAM-materials==0.0.2
+STEAM-materials==0.0.33
 svglib==1.5.1
 tomli==2.0.1
 tqdm==4.64.1
 traitlets==5.4.0
 typing_extensions==4.3.0
 urllib3==1.26.12
 watchdog==2.1.9
```

