# Comparing `tmp/mobspy-2.0.1.tar.gz` & `tmp/mobspy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobspy-2.0.1.tar", last modified: Wed Apr 19 11:46:42 2023, max compression
+gzip compressed data, was "mobspy-2.0.2.tar", last modified: Thu Apr 20 10:34:06 2023, max compression
```

## Comparing `mobspy-2.0.1.tar` & `mobspy-2.0.2.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.917449 mobspy-2.0.1/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.767707 mobspy-2.0.1/.github/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.776416 mobspy-2.0.1/.github/workflows/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-04-03 11:45:17.000000 mobspy-2.0.1/.github/workflows/python-app.yml
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      265 2023-04-05 11:22:48.000000 mobspy-2.0.1/.gitignore
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-03-26 13:05:39.000000 mobspy-2.0.1/LICENSE
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7015 2023-04-19 11:46:42.915662 mobspy-2.0.1/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5825 2023-03-29 14:16:39.000000 mobspy-2.0.1/README.md
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.768156 mobspy-2.0.1/example_models/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.785863 mobspy-2.0.1/example_models/application_models/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      573 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/application_models/AB_2CD.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1446 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/application_models/AND_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2653 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/application_models/CRISPR_Oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1435 2023-04-18 11:26:50.000000 mobspy-2.0.1/example_models/application_models/For_The_Trees.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1297 2023-03-31 13:18:09.000000 mobspy-2.0.1/example_models/application_models/NOR_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1244 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/application_models/donor_receptor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1372 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/application_models/oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2901 2023-04-18 11:26:50.000000 mobspy-2.0.1/example_models/application_models/random_walk.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      565 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/application_models/simple_repressor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3855 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/application_models/toggle_switch.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.803619 mobspy-2.0.1/example_models/tutorial_models/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1602 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/01_Getting_Started.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1863 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/02_Reaction_Inheritance.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1769 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/03_Queries.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      946 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/03_Queries.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      989 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/04_Characteristic_Restriction.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1121 2023-03-31 13:18:09.000000 mobspy-2.0.1/example_models/tutorial_models/05_C_Query.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2284 2023-03-31 13:18:09.000000 mobspy-2.0.1/example_models/tutorial_models/06_Round_Robin.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2255 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/07_Rates.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2125 2023-03-31 13:18:09.000000 mobspy-2.0.1/example_models/tutorial_models/08_Units.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      866 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/09_Count_Assignment.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1042 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/09_Count_Assignment.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1589 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/10_Species_Loop.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2074 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/11_Results.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2128 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/12_Hierarchical_plot.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      982 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/13_Born_Species.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      101 2023-04-19 11:43:11.000000 mobspy-2.0.1/for_local_use.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.804603 mobspy-2.0.1/images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-03-26 13:05:39.000000 mobspy-2.0.1/images/img.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.807293 mobspy-2.0.1/mobspy/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/_version.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.813584 mobspy-2.0.1/mobspy/data_handler/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/data_handler/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2207 2023-04-05 18:57:56.000000 mobspy-2.0.1/mobspy/data_handler/process_result_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5233 2023-04-19 11:42:57.000000 mobspy-2.0.1/mobspy/data_handler/time_series_object.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.833692 mobspy-2.0.1/mobspy/modules/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/modules/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4355 2023-04-17 14:42:37.000000 mobspy-2.0.1/mobspy/modules/event_functions.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12456 2023-04-18 20:56:31.000000 mobspy-2.0.1/mobspy/modules/function_rate_code.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12663 2023-04-12 21:11:32.000000 mobspy-2.0.1/mobspy/modules/logic_operator_objects.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    57088 2023-04-18 20:51:04.000000 mobspy-2.0.1/mobspy/modules/meta_class.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5239 2023-04-13 11:40:51.000000 mobspy-2.0.1/mobspy/modules/meta_class_utils.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14961 2023-04-13 12:13:54.000000 mobspy-2.0.1/mobspy/modules/order_operators.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16482 2023-04-13 12:24:44.000000 mobspy-2.0.1/mobspy/modules/reaction_construction_nb.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3988 2023-04-17 11:11:45.000000 mobspy-2.0.1/mobspy/modules/set_counts_module.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4143 2023-04-11 11:59:50.000000 mobspy-2.0.1/mobspy/modules/species_string_generator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6615 2023-04-18 21:25:28.000000 mobspy-2.0.1/mobspy/modules/unit_handler.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.834921 mobspy-2.0.1/mobspy/parameter_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/parameter_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2211 2023-04-07 15:35:28.000000 mobspy-2.0.1/mobspy/parameter_scripts/parameter_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.839087 mobspy-2.0.1/mobspy/parameters/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/parameters/README.md
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/parameters/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1035 2023-03-28 13:07:30.000000 mobspy-2.0.1/mobspy/parameters/default_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1117 2023-04-07 15:35:28.000000 mobspy-2.0.1/mobspy/parameters/example_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.843351 mobspy-2.0.1/mobspy/plot_params/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/plot_params/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/plot_params/default_plot_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1232 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/plot_params/example_plot_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.850288 mobspy-2.0.1/mobspy/plot_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/plot_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6445 2023-04-19 11:27:03.000000 mobspy-2.0.1/mobspy/plot_scripts/default_plots.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14387 2023-04-17 13:43:18.000000 mobspy-2.0.1/mobspy/plot_scripts/hierarchical_plot.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1736 2023-04-18 13:30:54.000000 mobspy-2.0.1/mobspy/plot_scripts/process_plot_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3566 2023-04-08 16:53:54.000000 mobspy-2.0.1/mobspy/plot_scripts/statistics_calculations.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.855000 mobspy-2.0.1/mobspy/sbml_simulator/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8118 2023-04-08 16:53:54.000000 mobspy-2.0.1/mobspy/sbml_simulator/SBMLWriter.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/sbml_simulator/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      936 2023-04-08 16:40:14.000000 mobspy-2.0.1/mobspy/sbml_simulator/builder.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12536 2023-04-17 15:49:48.000000 mobspy-2.0.1/mobspy/sbml_simulator/run.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    26192 2023-04-19 08:48:20.000000 mobspy-2.0.1/mobspy/simulation.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.856697 mobspy-2.0.1/mobspy/simulation_logging/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/simulation_logging/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2023-04-13 12:13:25.000000 mobspy-2.0.1/mobspy/simulation_logging/log_scripts.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.811622 mobspy-2.0.1/mobspy.egg-info/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7015 2023-04-19 11:46:42.000000 mobspy-2.0.1/mobspy.egg-info/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3563 2023-04-19 11:46:42.000000 mobspy-2.0.1/mobspy.egg-info/SOURCES.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2023-04-19 11:46:42.000000 mobspy-2.0.1/mobspy.egg-info/dependency_links.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2023-04-19 11:46:42.000000 mobspy-2.0.1/mobspy.egg-info/requires.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2023-04-19 11:46:42.000000 mobspy-2.0.1/mobspy.egg-info/top_level.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-03-26 13:05:39.000000 mobspy-2.0.1/requirements.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2023-04-19 11:46:42.918064 mobspy-2.0.1/setup.cfg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-03-26 13:05:39.000000 mobspy-2.0.1/setup.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18793 2023-04-18 21:34:52.000000 mobspy-2.0.1/test_script.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.910475 mobspy-2.0.1/test_tools/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-03-26 13:05:39.000000 mobspy-2.0.1/test_tools/model_1.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      239 2023-03-28 14:54:04.000000 mobspy-2.0.1/test_tools/model_10.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-03-29 10:35:15.000000 mobspy-2.0.1/test_tools/model_11.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-03-31 14:53:54.000000 mobspy-2.0.1/test_tools/model_12.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-03-31 16:58:04.000000 mobspy-2.0.1/test_tools/model_13.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-03-31 17:23:20.000000 mobspy-2.0.1/test_tools/model_14.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-04-03 08:42:24.000000 mobspy-2.0.1/test_tools/model_15.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-04-04 18:39:28.000000 mobspy-2.0.1/test_tools/model_16.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-04-05 14:12:52.000000 mobspy-2.0.1/test_tools/model_17.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-04-06 11:09:14.000000 mobspy-2.0.1/test_tools/model_18.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-04-06 13:23:26.000000 mobspy-2.0.1/test_tools/model_19.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-03-26 13:05:39.000000 mobspy-2.0.1/test_tools/model_2.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-04-06 13:24:46.000000 mobspy-2.0.1/test_tools/model_20.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-04-11 12:17:19.000000 mobspy-2.0.1/test_tools/model_21.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      435 2023-04-11 15:31:51.000000 mobspy-2.0.1/test_tools/model_22.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-04-12 16:26:56.000000 mobspy-2.0.1/test_tools/model_23.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-04-17 14:45:24.000000 mobspy-2.0.1/test_tools/model_24.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-04-18 11:30:58.000000 mobspy-2.0.1/test_tools/model_25.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      507 2023-04-18 20:45:48.000000 mobspy-2.0.1/test_tools/model_26.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-04-18 21:30:11.000000 mobspy-2.0.1/test_tools/model_27.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-03-26 13:05:39.000000 mobspy-2.0.1/test_tools/model_3.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-03-26 13:05:39.000000 mobspy-2.0.1/test_tools/model_4.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-03-26 13:05:39.000000 mobspy-2.0.1/test_tools/model_5.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      353 2023-03-26 13:05:39.000000 mobspy-2.0.1/test_tools/model_6.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1352 2023-03-26 13:05:39.000000 mobspy-2.0.1/test_tools/model_7.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      443 2023-03-28 21:23:58.000000 mobspy-2.0.1/test_tools/model_8.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-03-28 08:26:08.000000 mobspy-2.0.1/test_tools/model_9.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-03-26 13:05:39.000000 mobspy-2.0.1/useful_parameters.json
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.850224 mobspy-2.0.2/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.696133 mobspy-2.0.2/.github/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.704212 mobspy-2.0.2/.github/workflows/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-04-03 11:45:17.000000 mobspy-2.0.2/.github/workflows/python-app.yml
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      265 2023-04-05 11:22:48.000000 mobspy-2.0.2/.gitignore
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-03-26 13:05:39.000000 mobspy-2.0.2/LICENSE
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7015 2023-04-20 10:34:06.849565 mobspy-2.0.2/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5825 2023-03-29 14:16:39.000000 mobspy-2.0.2/README.md
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.696455 mobspy-2.0.2/example_models/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.714243 mobspy-2.0.2/example_models/application_models/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      573 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/application_models/AB_2CD.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1446 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/application_models/AND_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2653 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/application_models/CRISPR_Oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1435 2023-04-18 11:26:50.000000 mobspy-2.0.2/example_models/application_models/For_The_Trees.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1297 2023-03-31 13:18:09.000000 mobspy-2.0.2/example_models/application_models/NOR_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1244 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/application_models/donor_receptor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1372 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/application_models/oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2901 2023-04-18 11:26:50.000000 mobspy-2.0.2/example_models/application_models/random_walk.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      565 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/application_models/simple_repressor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3855 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/application_models/toggle_switch.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.737946 mobspy-2.0.2/example_models/tutorial_models/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1602 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/01_Getting_Started.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1863 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/02_Reaction_Inheritance.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1769 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/03_Queries.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      946 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/03_Queries.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      989 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/04_Characteristic_Restriction.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1121 2023-03-31 13:18:09.000000 mobspy-2.0.2/example_models/tutorial_models/05_C_Query.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2284 2023-03-31 13:18:09.000000 mobspy-2.0.2/example_models/tutorial_models/06_Round_Robin.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2255 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/07_Rates.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2125 2023-03-31 13:18:09.000000 mobspy-2.0.2/example_models/tutorial_models/08_Units.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      866 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/09_Count_Assignment.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1042 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/09_Count_Assignment.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1589 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/10_Species_Loop.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2074 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/11_Results.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2128 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/12_Hierarchical_plot.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      982 2023-03-26 13:05:39.000000 mobspy-2.0.2/example_models/tutorial_models/13_Born_Species.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      596 2023-04-20 10:30:16.000000 mobspy-2.0.2/for_local_use.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.738959 mobspy-2.0.2/images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-03-26 13:05:39.000000 mobspy-2.0.2/images/img.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.742895 mobspy-2.0.2/mobspy/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2023-04-20 10:31:23.000000 mobspy-2.0.2/mobspy/_version.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.749383 mobspy-2.0.2/mobspy/data_handler/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/data_handler/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2207 2023-04-05 18:57:56.000000 mobspy-2.0.2/mobspy/data_handler/process_result_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5972 2023-04-20 09:08:12.000000 mobspy-2.0.2/mobspy/data_handler/time_series_object.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.765722 mobspy-2.0.2/mobspy/modules/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/modules/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4355 2023-04-17 14:42:37.000000 mobspy-2.0.2/mobspy/modules/event_functions.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12456 2023-04-18 20:56:31.000000 mobspy-2.0.2/mobspy/modules/function_rate_code.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12663 2023-04-12 21:11:32.000000 mobspy-2.0.2/mobspy/modules/logic_operator_objects.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    57088 2023-04-18 20:51:04.000000 mobspy-2.0.2/mobspy/modules/meta_class.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5239 2023-04-13 11:40:51.000000 mobspy-2.0.2/mobspy/modules/meta_class_utils.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14961 2023-04-13 12:13:54.000000 mobspy-2.0.2/mobspy/modules/order_operators.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16482 2023-04-13 12:24:44.000000 mobspy-2.0.2/mobspy/modules/reaction_construction_nb.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3988 2023-04-17 11:11:45.000000 mobspy-2.0.2/mobspy/modules/set_counts_module.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4143 2023-04-11 11:59:50.000000 mobspy-2.0.2/mobspy/modules/species_string_generator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6615 2023-04-18 21:25:28.000000 mobspy-2.0.2/mobspy/modules/unit_handler.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.768335 mobspy-2.0.2/mobspy/parameter_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/parameter_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2211 2023-04-07 15:35:28.000000 mobspy-2.0.2/mobspy/parameter_scripts/parameter_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.775603 mobspy-2.0.2/mobspy/parameters/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/parameters/README.md
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/parameters/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1035 2023-03-28 13:07:30.000000 mobspy-2.0.2/mobspy/parameters/default_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1117 2023-04-07 15:35:28.000000 mobspy-2.0.2/mobspy/parameters/example_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.778128 mobspy-2.0.2/mobspy/plot_params/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/plot_params/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/plot_params/default_plot_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1232 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/plot_params/example_plot_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.782813 mobspy-2.0.2/mobspy/plot_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/plot_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6445 2023-04-19 11:27:03.000000 mobspy-2.0.2/mobspy/plot_scripts/default_plots.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14387 2023-04-17 13:43:18.000000 mobspy-2.0.2/mobspy/plot_scripts/hierarchical_plot.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1846 2023-04-20 09:16:42.000000 mobspy-2.0.2/mobspy/plot_scripts/process_plot_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3566 2023-04-20 08:51:56.000000 mobspy-2.0.2/mobspy/plot_scripts/statistics_calculations.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.787807 mobspy-2.0.2/mobspy/sbml_simulator/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8118 2023-04-08 16:53:54.000000 mobspy-2.0.2/mobspy/sbml_simulator/SBMLWriter.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/sbml_simulator/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      936 2023-04-08 16:40:14.000000 mobspy-2.0.2/mobspy/sbml_simulator/builder.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12536 2023-04-17 15:49:48.000000 mobspy-2.0.2/mobspy/sbml_simulator/run.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    26192 2023-04-19 08:48:20.000000 mobspy-2.0.2/mobspy/simulation.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.789705 mobspy-2.0.2/mobspy/simulation_logging/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.2/mobspy/simulation_logging/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2023-04-13 12:13:25.000000 mobspy-2.0.2/mobspy/simulation_logging/log_scripts.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.747010 mobspy-2.0.2/mobspy.egg-info/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7015 2023-04-20 10:34:06.000000 mobspy-2.0.2/mobspy.egg-info/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3563 2023-04-20 10:34:06.000000 mobspy-2.0.2/mobspy.egg-info/SOURCES.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2023-04-20 10:34:06.000000 mobspy-2.0.2/mobspy.egg-info/dependency_links.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2023-04-20 10:34:06.000000 mobspy-2.0.2/mobspy.egg-info/requires.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2023-04-20 10:34:06.000000 mobspy-2.0.2/mobspy.egg-info/top_level.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-03-26 13:05:39.000000 mobspy-2.0.2/requirements.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2023-04-20 10:34:06.850385 mobspy-2.0.2/setup.cfg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-03-26 13:05:39.000000 mobspy-2.0.2/setup.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18793 2023-04-18 21:34:52.000000 mobspy-2.0.2/test_script.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-20 10:34:06.848113 mobspy-2.0.2/test_tools/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-03-26 13:05:39.000000 mobspy-2.0.2/test_tools/model_1.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      239 2023-03-28 14:54:04.000000 mobspy-2.0.2/test_tools/model_10.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-03-29 10:35:15.000000 mobspy-2.0.2/test_tools/model_11.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-03-31 14:53:54.000000 mobspy-2.0.2/test_tools/model_12.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-03-31 16:58:04.000000 mobspy-2.0.2/test_tools/model_13.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-03-31 17:23:20.000000 mobspy-2.0.2/test_tools/model_14.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-04-03 08:42:24.000000 mobspy-2.0.2/test_tools/model_15.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-04-04 18:39:28.000000 mobspy-2.0.2/test_tools/model_16.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-04-05 14:12:52.000000 mobspy-2.0.2/test_tools/model_17.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-04-06 11:09:14.000000 mobspy-2.0.2/test_tools/model_18.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-04-06 13:23:26.000000 mobspy-2.0.2/test_tools/model_19.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-03-26 13:05:39.000000 mobspy-2.0.2/test_tools/model_2.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-04-06 13:24:46.000000 mobspy-2.0.2/test_tools/model_20.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-04-11 12:17:19.000000 mobspy-2.0.2/test_tools/model_21.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      435 2023-04-11 15:31:51.000000 mobspy-2.0.2/test_tools/model_22.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-04-12 16:26:56.000000 mobspy-2.0.2/test_tools/model_23.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-04-17 14:45:24.000000 mobspy-2.0.2/test_tools/model_24.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-04-18 11:30:58.000000 mobspy-2.0.2/test_tools/model_25.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      507 2023-04-18 20:45:48.000000 mobspy-2.0.2/test_tools/model_26.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-04-18 21:30:11.000000 mobspy-2.0.2/test_tools/model_27.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-03-26 13:05:39.000000 mobspy-2.0.2/test_tools/model_3.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-03-26 13:05:39.000000 mobspy-2.0.2/test_tools/model_4.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-03-26 13:05:39.000000 mobspy-2.0.2/test_tools/model_5.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      353 2023-03-26 13:05:39.000000 mobspy-2.0.2/test_tools/model_6.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1352 2023-03-26 13:05:39.000000 mobspy-2.0.2/test_tools/model_7.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      443 2023-03-28 21:23:58.000000 mobspy-2.0.2/test_tools/model_8.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-03-28 08:26:08.000000 mobspy-2.0.2/test_tools/model_9.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-03-26 13:05:39.000000 mobspy-2.0.2/useful_parameters.json
```

### Comparing `mobspy-2.0.1/.github/workflows/python-app.yml` & `mobspy-2.0.2/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/LICENSE` & `mobspy-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/PKG-INFO` & `mobspy-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
```

### Comparing `mobspy-2.0.1/README.md` & `mobspy-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/application_models/AB_2CD.py` & `mobspy-2.0.2/example_models/application_models/AB_2CD.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/application_models/AND_gate.py` & `mobspy-2.0.2/example_models/application_models/AND_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/application_models/CRISPR_Oscillator.py` & `mobspy-2.0.2/example_models/application_models/CRISPR_Oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/application_models/For_The_Trees.py` & `mobspy-2.0.2/example_models/application_models/For_The_Trees.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/application_models/NOR_gate.py` & `mobspy-2.0.2/example_models/application_models/NOR_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/application_models/donor_receptor.py` & `mobspy-2.0.2/example_models/application_models/donor_receptor.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/application_models/oscillator.py` & `mobspy-2.0.2/example_models/application_models/oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/application_models/random_walk.py` & `mobspy-2.0.2/example_models/application_models/random_walk.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/application_models/simple_repressor.py` & `mobspy-2.0.2/example_models/application_models/simple_repressor.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/application_models/toggle_switch.py` & `mobspy-2.0.2/example_models/application_models/toggle_switch.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/01_Getting_Started.py` & `mobspy-2.0.2/example_models/tutorial_models/01_Getting_Started.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/02_Reaction_Inheritance.py` & `mobspy-2.0.2/example_models/tutorial_models/02_Reaction_Inheritance.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt` & `mobspy-2.0.2/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/03_Queries.py` & `mobspy-2.0.2/example_models/tutorial_models/03_Queries.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/03_Queries.txt` & `mobspy-2.0.2/example_models/tutorial_models/03_Queries.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/04_Characteristic_Restriction.py` & `mobspy-2.0.2/example_models/tutorial_models/04_Characteristic_Restriction.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/05_C_Query.py` & `mobspy-2.0.2/example_models/tutorial_models/05_C_Query.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/06_Round_Robin.py` & `mobspy-2.0.2/example_models/tutorial_models/06_Round_Robin.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/07_Rates.py` & `mobspy-2.0.2/example_models/tutorial_models/07_Rates.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/08_Units.py` & `mobspy-2.0.2/example_models/tutorial_models/08_Units.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/09_Count_Assignment.py` & `mobspy-2.0.2/example_models/tutorial_models/09_Count_Assignment.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/09_Count_Assignment.txt` & `mobspy-2.0.2/example_models/tutorial_models/09_Count_Assignment.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/10_Species_Loop.py` & `mobspy-2.0.2/example_models/tutorial_models/10_Species_Loop.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/11_Results.py` & `mobspy-2.0.2/example_models/tutorial_models/11_Results.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/12_Hierarchical_plot.py` & `mobspy-2.0.2/example_models/tutorial_models/12_Hierarchical_plot.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/example_models/tutorial_models/13_Born_Species.py` & `mobspy-2.0.2/example_models/tutorial_models/13_Born_Species.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/images/img.png` & `mobspy-2.0.2/images/img.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/data_handler/process_result_data.py` & `mobspy-2.0.2/mobspy/data_handler/process_result_data.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/data_handler/time_series_object.py` & `mobspy-2.0.2/mobspy/data_handler/time_series_object.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
     This module implements the class that stores the results from a MobsPy simulation
 """
 import pandas as pd
 from mobspy.modules.meta_class import *
 import inspect
 
+
 class MobsPyTimeSeries:
 
     def __init__(self, data_dict):
         """Creates the MobsPy timeseries object
 
             :param data: (dict) resulting dictionary from simulation
             {'data': ...., 'params':....., 'models':.......}
@@ -56,30 +57,46 @@
         code_line = inspect.stack()[1].code_context[0][:-1]
         if '[\'runs\']' in code_line:
             simlog.error('As of version 2.0.1 MobsPy has changed the data output format. \n'
                          'Now data can be accessed through the following syntax: \n'
                          'S.results[Meta-Species Object] or S.results[Meta-Species string name] \n'
                          'Both can perform queries', stack_index=2)
 
+        series_index = None
+        if type(item) == tuple:
+            if len(item) > 2 or type(item[1]) != int:
+                simlog.error('Only len 2 and ints allowed in tuple-based assignments', stack_index=2)
+            series_index = item[1]
+            item = item[0]
+
         to_return = []
         if type(item) == int:
             return self.ts_data[item]
         elif type(item) == str:
             try:
                 for ts in self.ts_data:
                     to_return.append(ts[item])
             except KeyError:
-                for i in range(len(self)):
-                    to_return.append(self._sum_reacting_species_data(item, i))
+                if series_index is None:
+                    for i in range(len(self)):
+                        to_return.append(self._sum_reacting_species_data(item, i))
+                else:
+                    to_return.append(self._sum_reacting_species_data(item, series_index))
         elif isinstance(item, Species):
-            for ts in self.ts_data:
-                to_return.append(ts[item.get_name()])
+            if series_index is None:
+                for ts in self.ts_data:
+                    to_return.append(ts[item.get_name()])
+            else:
+                to_return.append(self._sum_reacting_species_data(item, series_index))
         elif isinstance(item, Reacting_Species):
-            for i in range(len(self)):
-                to_return.append(self._sum_reacting_species_data(item, i))
+            if series_index is None:
+                for i in range(len(self)):
+                    to_return.append(self._sum_reacting_species_data(item, i))
+            else:
+                to_return.append(self._sum_reacting_species_data(item, series_index))
 
         if len(to_return) == 1:
             return to_return[0]
         else:
             return to_return
 
     def _sum_reacting_species_data(self, item, ts_index):
```

### Comparing `mobspy-2.0.1/mobspy/modules/event_functions.py` & `mobspy-2.0.2/mobspy/modules/event_functions.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/modules/function_rate_code.py` & `mobspy-2.0.2/mobspy/modules/function_rate_code.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/modules/logic_operator_objects.py` & `mobspy-2.0.2/mobspy/modules/logic_operator_objects.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/modules/meta_class.py` & `mobspy-2.0.2/mobspy/modules/meta_class.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/modules/meta_class_utils.py` & `mobspy-2.0.2/mobspy/modules/meta_class_utils.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/modules/order_operators.py` & `mobspy-2.0.2/mobspy/modules/order_operators.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/modules/reaction_construction_nb.py` & `mobspy-2.0.2/mobspy/modules/reaction_construction_nb.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/modules/set_counts_module.py` & `mobspy-2.0.2/mobspy/modules/set_counts_module.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/modules/species_string_generator.py` & `mobspy-2.0.2/mobspy/modules/species_string_generator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/modules/unit_handler.py` & `mobspy-2.0.2/mobspy/modules/unit_handler.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/parameter_scripts/parameter_reader.py` & `mobspy-2.0.2/mobspy/parameter_scripts/parameter_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/parameters/README.md` & `mobspy-2.0.2/mobspy/parameters/README.md`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/parameters/default_reader.py` & `mobspy-2.0.2/mobspy/parameters/default_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/parameters/example_reader.py` & `mobspy-2.0.2/mobspy/parameters/example_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/plot_params/example_plot_reader.py` & `mobspy-2.0.2/mobspy/plot_params/example_plot_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/plot_scripts/default_plots.py` & `mobspy-2.0.2/mobspy/plot_scripts/default_plots.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/plot_scripts/hierarchical_plot.py` & `mobspy-2.0.2/mobspy/plot_scripts/hierarchical_plot.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/plot_scripts/process_plot_data.py` & `mobspy-2.0.2/mobspy/plot_scripts/process_plot_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,19 +19,22 @@
             if key in species:
                 species_to_plot.add(key)
 
     for spe in species:
         if spe in species_to_plot:
             continue
 
+        temp_list = [0 for _ in range(len(new_data.ts_data))]
         for i, ts in enumerate(new_data.ts_data):
-            new_data.time_series_number = i
-            ts[spe] = new_data[spe]
+            temp_list[i] = new_data[spe, i]
             species_to_plot.add(spe)
 
+        for res, ts in zip(temp_list, new_data.ts_data):
+            ts[spe] = res
+
     return species_to_plot, new_data
 
 
 def check_plot_parameters(species, plot_params):
     """
         Performs a check of the plot_parameters given. To see if the parameters are correctly named
```

### Comparing `mobspy-2.0.1/mobspy/plot_scripts/statistics_calculations.py` & `mobspy-2.0.2/mobspy/plot_scripts/statistics_calculations.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/sbml_simulator/SBMLWriter.py` & `mobspy-2.0.2/mobspy/sbml_simulator/SBMLWriter.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/sbml_simulator/builder.py` & `mobspy-2.0.2/mobspy/sbml_simulator/builder.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/sbml_simulator/run.py` & `mobspy-2.0.2/mobspy/sbml_simulator/run.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/simulation.py` & `mobspy-2.0.2/mobspy/simulation.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy/simulation_logging/log_scripts.py` & `mobspy-2.0.2/mobspy/simulation_logging/log_scripts.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/mobspy.egg-info/PKG-INFO` & `mobspy-2.0.2/mobspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
```

### Comparing `mobspy-2.0.1/mobspy.egg-info/SOURCES.txt` & `mobspy-2.0.2/mobspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/setup.py` & `mobspy-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/test_script.py` & `mobspy-2.0.2/test_script.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/test_tools/model_15.txt` & `mobspy-2.0.2/test_tools/model_15.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/test_tools/model_19.txt` & `mobspy-2.0.2/test_tools/model_19.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/test_tools/model_21.txt` & `mobspy-2.0.2/test_tools/model_21.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/test_tools/model_24.txt` & `mobspy-2.0.2/test_tools/model_24.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/test_tools/model_3.txt` & `mobspy-2.0.2/test_tools/model_3.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/test_tools/model_4.txt` & `mobspy-2.0.2/test_tools/model_4.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/test_tools/model_5.txt` & `mobspy-2.0.2/test_tools/model_5.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/test_tools/model_7.txt` & `mobspy-2.0.2/test_tools/model_7.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.0.1/test_tools/model_9.txt` & `mobspy-2.0.2/test_tools/model_9.txt`

 * *Files identical despite different names*

