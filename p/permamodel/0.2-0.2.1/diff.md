# Comparing `tmp/permamodel-0.2.tar.gz` & `tmp/permamodel-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permamodel-0.2.tar", last modified: Tue Apr 11 21:08:54 2023, max compression
+gzip compressed data, was "permamodel-0.2.1.tar", last modified: Thu Apr 20 21:24:50 2023, max compression
```

## Comparing `permamodel-0.2.tar` & `permamodel-0.2.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-11 21:08:54.534577 permamodel-0.2/
--rw-r--r--   0 mpiper     (501) staff       (20)      924 2023-04-11 21:02:41.000000 permamodel-0.2/CITATION.cff
--rw-r--r--   0 mpiper     (501) staff       (20)     1077 2023-04-11 21:02:41.000000 permamodel-0.2/LICENSE
--rw-r--r--   0 mpiper     (501) staff       (20)      331 2023-04-11 21:02:41.000000 permamodel-0.2/MANIFEST.in
--rw-r--r--   0 mpiper     (501) staff       (20)     4506 2023-04-11 21:08:54.534662 permamodel-0.2/PKG-INFO
--rw-r--r--   0 mpiper     (501) staff       (20)     2341 2023-04-11 21:02:41.000000 permamodel-0.2/README.md
--rw-r--r--   0 mpiper     (501) staff       (20)     4945 2023-04-11 21:02:41.000000 permamodel-0.2/noxfile.py
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-11 21:08:54.506278 permamodel-0.2/permamodel/
--rw-r--r--   0 mpiper     (501) staff       (20)      613 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/__init__.py
--rw-r--r--   0 mpiper     (501) staff       (20)       20 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/_version.py
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-11 21:08:54.509093 permamodel-0.2/permamodel/components/
--rw-r--r--   0 mpiper     (501) staff       (20)    22202 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/components/Ku.py
--rw-r--r--   0 mpiper     (501) staff       (20)    52201 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/components/Ku_method.py
--rw-r--r--   0 mpiper     (501) staff       (20)       25 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/components/__init__.py
--rw-r--r--   0 mpiper     (501) staff       (20)    11585 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/components/bmi_Ku.py
--rw-r--r--   0 mpiper     (501) staff       (20)    16862 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/components/bmi_Ku_component.py
--rw-r--r--   0 mpiper     (501) staff       (20)    12954 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/components/bmi_frost_number.py
--rw-r--r--   0 mpiper     (501) staff       (20)    11379 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/components/bmi_frost_number_Geo.py
--rw-r--r--   0 mpiper     (501) staff       (20)    14052 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/components/frost_number.py
--rw-r--r--   0 mpiper     (501) staff       (20)    42982 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/components/frost_number_Geo.py
--rw-r--r--   0 mpiper     (501) staff       (20)    29955 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/components/perma_base.py
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-11 21:08:54.528738 permamodel-0.2/permamodel/data/
--rwxr-xr-x   0 mpiper     (501) staff       (20)  2195333 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/data/T_CLAY.nc4
--rwxr-xr-x   0 mpiper     (501) staff       (20)  2629756 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/data/T_OC.nc4
--rwxr-xr-x   0 mpiper     (501) staff       (20)  2329260 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/data/T_SAND.nc4
--rwxr-xr-x   0 mpiper     (501) staff       (20)  2266288 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/data/T_SILT.nc4
--rwxr-xr-x   0 mpiper     (501) staff       (20)      196 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/data/Typical_Thermal_Parameters.csv
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-11 21:08:54.503937 permamodel-0.2/permamodel/data/test_directory/
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-11 21:08:54.530522 permamodel-0.2/permamodel/data/test_directory/inputs/
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/data/test_directory/inputs/air_temperature.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/data/test_directory/inputs/frozen_vegetation_diffusivity.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/data/test_directory/inputs/frozen_vegetation_height.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/data/test_directory/inputs/snow_density.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/data/test_directory/inputs/snow_thickness.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/data/test_directory/inputs/soil_water_content.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/data/test_directory/inputs/temperature_amplitude.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/data/test_directory/inputs/thawed_vegetation_diffusivity.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/data/test_directory/inputs/thawed_vegetation_height.nc
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-11 21:08:54.531316 permamodel-0.2/permamodel/examples/
--rw-r--r--   0 mpiper     (501) staff       (20)     1540 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/examples/Frostnumber_example_singlesite_singleyear.cfg
--rw-r--r--   0 mpiper     (501) staff       (20)     1668 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/examples/Ku_bmi_example_config.toml
--rw-r--r--   0 mpiper     (501) staff       (20)     1668 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/examples/Ku_example_config.toml
--rw-r--r--   0 mpiper     (501) staff       (20)     3517 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/examples/Ku_method.cfg
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-11 21:08:54.533021 permamodel-0.2/permamodel/tests/
--rw-r--r--   0 mpiper     (501) staff       (20)       40 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/tests/__init__.py
--rw-r--r--   0 mpiper     (501) staff       (20)     7003 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/tests/test_Ku.py
--rw-r--r--   0 mpiper     (501) staff       (20)      746 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/tests/test_Ku_method.py
--rw-r--r--   0 mpiper     (501) staff       (20)     3709 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/tests/test_frost_number.py
--rw-r--r--   0 mpiper     (501) staff       (20)    10122 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/tests/test_frost_number_Geo.py
--rw-r--r--   0 mpiper     (501) staff       (20)    11856 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/tests/test_frost_number_Geo_bmi.py
--rw-r--r--   0 mpiper     (501) staff       (20)     8485 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/tests/test_frost_number_bmi.py
--rw-r--r--   0 mpiper     (501) staff       (20)      820 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/tests/test_package_directories.py
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-11 21:08:54.534382 permamodel-0.2/permamodel/utils/
--rwxr-xr-x   0 mpiper     (501) staff       (20)    83475 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/utils/BMI_base.py
--rwxr-xr-x   0 mpiper     (501) staff       (20)       26 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/utils/__init__.py
--rwxr-xr-x   0 mpiper     (501) staff       (20)     6817 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/utils/file_utils.py
--rwxr-xr-x   0 mpiper     (501) staff       (20)    14005 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/utils/model_input.py
--rwxr-xr-x   0 mpiper     (501) staff       (20)     8788 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/utils/outlets.py
--rwxr-xr-x   0 mpiper     (501) staff       (20)    14496 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/utils/pixels.py
--rwxr-xr-x   0 mpiper     (501) staff       (20)    24124 2023-04-11 21:02:41.000000 permamodel-0.2/permamodel/utils/rti_files.py
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-11 21:08:54.506924 permamodel-0.2/permamodel.egg-info/
--rw-r--r--   0 mpiper     (501) staff       (20)     4506 2023-04-11 21:08:54.000000 permamodel-0.2/permamodel.egg-info/PKG-INFO
--rw-r--r--   0 mpiper     (501) staff       (20)     2112 2023-04-11 21:08:54.000000 permamodel-0.2/permamodel.egg-info/SOURCES.txt
--rw-r--r--   0 mpiper     (501) staff       (20)        1 2023-04-11 21:08:54.000000 permamodel-0.2/permamodel.egg-info/dependency_links.txt
--rw-r--r--   0 mpiper     (501) staff       (20)      181 2023-04-11 21:08:54.000000 permamodel-0.2/permamodel.egg-info/requires.txt
--rw-r--r--   0 mpiper     (501) staff       (20)       11 2023-04-11 21:08:54.000000 permamodel-0.2/permamodel.egg-info/top_level.txt
--rw-r--r--   0 mpiper     (501) staff       (20)     2419 2023-04-11 21:02:41.000000 permamodel-0.2/pyproject.toml
--rw-r--r--   0 mpiper     (501) staff       (20)       62 2023-04-11 21:02:41.000000 permamodel-0.2/requirements.txt
--rw-r--r--   0 mpiper     (501) staff       (20)      286 2023-04-11 21:08:54.534947 permamodel-0.2/setup.cfg
--rw-r--r--   0 mpiper     (501) staff       (20)       63 2023-04-11 21:02:41.000000 permamodel-0.2/setup.py
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.373119 permamodel-0.2.1/
+-rw-r--r--   0 mpiper     (501) staff       (20)      924 2023-04-20 21:17:39.000000 permamodel-0.2.1/CITATION.cff
+-rw-r--r--   0 mpiper     (501) staff       (20)     1077 2023-04-20 21:17:39.000000 permamodel-0.2.1/LICENSE
+-rw-r--r--   0 mpiper     (501) staff       (20)      331 2023-04-20 21:17:39.000000 permamodel-0.2.1/MANIFEST.in
+-rw-r--r--   0 mpiper     (501) staff       (20)     3318 2023-04-20 21:24:50.373193 permamodel-0.2.1/PKG-INFO
+-rw-r--r--   0 mpiper     (501) staff       (20)     1151 2023-04-20 21:17:39.000000 permamodel-0.2.1/README.md
+-rw-r--r--   0 mpiper     (501) staff       (20)     4945 2023-04-20 21:17:39.000000 permamodel-0.2.1/noxfile.py
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.342115 permamodel-0.2.1/permamodel/
+-rw-r--r--   0 mpiper     (501) staff       (20)      613 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/__init__.py
+-rw-r--r--   0 mpiper     (501) staff       (20)       22 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/_version.py
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.344673 permamodel-0.2.1/permamodel/components/
+-rw-r--r--   0 mpiper     (501) staff       (20)    22202 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/Ku.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    52201 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/Ku_method.py
+-rw-r--r--   0 mpiper     (501) staff       (20)       25 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/__init__.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    11499 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/bmi_Ku.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    16862 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/bmi_Ku_component.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    12954 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/bmi_frost_number.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    11379 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/bmi_frost_number_Geo.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    14052 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/frost_number.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    42982 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/frost_number_Geo.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    29955 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/perma_base.py
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.366952 permamodel-0.2.1/permamodel/data/
+-rwxr-xr-x   0 mpiper     (501) staff       (20)  2195333 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/T_CLAY.nc4
+-rwxr-xr-x   0 mpiper     (501) staff       (20)  2629756 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/T_OC.nc4
+-rwxr-xr-x   0 mpiper     (501) staff       (20)  2329260 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/T_SAND.nc4
+-rwxr-xr-x   0 mpiper     (501) staff       (20)  2266288 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/T_SILT.nc4
+-rwxr-xr-x   0 mpiper     (501) staff       (20)      196 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/Typical_Thermal_Parameters.csv
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.340057 permamodel-0.2.1/permamodel/data/test_directory/
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.368928 permamodel-0.2.1/permamodel/data/test_directory/inputs/
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/air_temperature.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/frozen_vegetation_diffusivity.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/frozen_vegetation_height.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/snow_density.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/snow_thickness.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/soil_water_content.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/temperature_amplitude.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/thawed_vegetation_diffusivity.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/thawed_vegetation_height.nc
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.369885 permamodel-0.2.1/permamodel/examples/
+-rw-r--r--   0 mpiper     (501) staff       (20)     1540 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/examples/Frostnumber_example_singlesite_singleyear.cfg
+-rw-r--r--   0 mpiper     (501) staff       (20)     1668 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/examples/Ku_bmi_example_config.toml
+-rw-r--r--   0 mpiper     (501) staff       (20)     1668 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/examples/Ku_example_config.toml
+-rw-r--r--   0 mpiper     (501) staff       (20)     3517 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/examples/Ku_method.cfg
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.371422 permamodel-0.2.1/permamodel/tests/
+-rw-r--r--   0 mpiper     (501) staff       (20)       40 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/__init__.py
+-rw-r--r--   0 mpiper     (501) staff       (20)     7003 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/test_Ku.py
+-rw-r--r--   0 mpiper     (501) staff       (20)      746 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/test_Ku_method.py
+-rw-r--r--   0 mpiper     (501) staff       (20)     3709 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/test_frost_number.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    10122 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/test_frost_number_Geo.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    11856 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/test_frost_number_Geo_bmi.py
+-rw-r--r--   0 mpiper     (501) staff       (20)     8485 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/test_frost_number_bmi.py
+-rw-r--r--   0 mpiper     (501) staff       (20)      820 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/test_package_directories.py
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.372940 permamodel-0.2.1/permamodel/utils/
+-rwxr-xr-x   0 mpiper     (501) staff       (20)    83475 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/utils/BMI_base.py
+-rwxr-xr-x   0 mpiper     (501) staff       (20)       26 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/utils/__init__.py
+-rwxr-xr-x   0 mpiper     (501) staff       (20)     6817 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/utils/file_utils.py
+-rwxr-xr-x   0 mpiper     (501) staff       (20)    14005 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/utils/model_input.py
+-rwxr-xr-x   0 mpiper     (501) staff       (20)     8788 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/utils/outlets.py
+-rwxr-xr-x   0 mpiper     (501) staff       (20)    14496 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/utils/pixels.py
+-rwxr-xr-x   0 mpiper     (501) staff       (20)    24124 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/utils/rti_files.py
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.342697 permamodel-0.2.1/permamodel.egg-info/
+-rw-r--r--   0 mpiper     (501) staff       (20)     3318 2023-04-20 21:24:50.000000 permamodel-0.2.1/permamodel.egg-info/PKG-INFO
+-rw-r--r--   0 mpiper     (501) staff       (20)     2112 2023-04-20 21:24:50.000000 permamodel-0.2.1/permamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 mpiper     (501) staff       (20)        1 2023-04-20 21:24:50.000000 permamodel-0.2.1/permamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 mpiper     (501) staff       (20)      181 2023-04-20 21:24:50.000000 permamodel-0.2.1/permamodel.egg-info/requires.txt
+-rw-r--r--   0 mpiper     (501) staff       (20)       11 2023-04-20 21:24:50.000000 permamodel-0.2.1/permamodel.egg-info/top_level.txt
+-rw-r--r--   0 mpiper     (501) staff       (20)     2419 2023-04-20 21:17:39.000000 permamodel-0.2.1/pyproject.toml
+-rw-r--r--   0 mpiper     (501) staff       (20)       62 2023-04-20 21:17:39.000000 permamodel-0.2.1/requirements.txt
+-rw-r--r--   0 mpiper     (501) staff       (20)      286 2023-04-20 21:24:50.373445 permamodel-0.2.1/setup.cfg
+-rw-r--r--   0 mpiper     (501) staff       (20)       63 2023-04-20 21:17:39.000000 permamodel-0.2.1/setup.py
```

### Comparing `permamodel-0.2/CITATION.cff` & `permamodel-0.2.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/LICENSE` & `permamodel-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/noxfile.py` & `permamodel-0.2.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/__init__.py` & `permamodel-0.2.1/permamodel/__init__.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/components/Ku.py` & `permamodel-0.2.1/permamodel/components/Ku.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/components/Ku_method.py` & `permamodel-0.2.1/permamodel/components/Ku_method.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/components/bmi_Ku.py` & `permamodel-0.2.1/permamodel/components/bmi_Ku.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 
         self._values = {
             var: getattr(self._model, var).values for var in self._input_var_names
         }
         for var in self._output_var_names:
             self._values[var] = np.empty(
                 (
-                    self._model.number_of_years,
                     self._model.grid_shape[0],
                     self._model.grid_shape[1],
                 )
             )
 
         self._var_units = self._var_units_map.copy()
 
@@ -117,22 +116,21 @@
         self._grid_type = {
             i: "uniform_rectilinear" for i in range(len(self._var_units_map.keys()))
         }
 
         self._start_time = 0.0
         self._end_time = self._model.number_of_years
         self._grid_shape = (
-            self._model.number_of_years,
             self._model.grid_shape[0],
             self._model.grid_shape[1],
         )
 
     def update(self):
         """Run the model for the current time step."""
-        self._model.run_one_step(self._current_time)
+        self._model.run_one_step(int(self._current_time))
         self._current_time += 1.0
 
     def update_until(self, end_time: int):
         """Update the model until a certain year (inclusive)."""
         years = self._current_time + end_time
 
         for t in np.arange(self._current_time, end_time + 1, 1):
@@ -263,26 +261,26 @@
         """Given a grid ID, return the distance between grid elements in each direction."""
         var = self._grids[grid]
 
         dims = getattr(self._model, var).dims
         coords = [getattr(self._model, var)[dim] for dim in dims]
         diffs = [np.diff(array)[0] for array in coords]
 
-        spacing[:] = diffs
+        spacing[:] = diffs[-2:]
         return spacing
 
     def get_grid_origin(self, grid: int, origin: np.ndarray) -> np.ndarray:
         """Given a grid ID, return the [y, x] coordinates of the lower-left corner."""
         var = self._grids[grid]
 
         ydim = getattr(self._model, var).dims[1]
         xdim = getattr(self._model, var).dims[2]
 
-        y0 = getattr(self._model, var)[ydim][0, 0]
-        x0 = getattr(self._model, var)[xdim][0, 0]
+        y0 = getattr(self._model, var)[ydim][0]
+        x0 = getattr(self._model, var)[xdim][0]
 
         origin[:] = [y0, x0]
         return origin
 
     def get_grid_x(self, grid: int, xs: np.ndarray) -> np.ndarray:
         """Given a grid ID, return an array of x-coordinates."""
         var = self._grids[grid]
```

### Comparing `permamodel-0.2/permamodel/components/bmi_Ku_component.py` & `permamodel-0.2.1/permamodel/components/bmi_Ku_component.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/components/bmi_frost_number.py` & `permamodel-0.2.1/permamodel/components/bmi_frost_number.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/components/bmi_frost_number_Geo.py` & `permamodel-0.2.1/permamodel/components/bmi_frost_number_Geo.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/components/frost_number.py` & `permamodel-0.2.1/permamodel/components/frost_number.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/components/frost_number_Geo.py` & `permamodel-0.2.1/permamodel/components/frost_number_Geo.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/components/perma_base.py` & `permamodel-0.2.1/permamodel/components/perma_base.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/data/T_CLAY.nc4` & `permamodel-0.2.1/permamodel/data/T_CLAY.nc4`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/data/T_OC.nc4` & `permamodel-0.2.1/permamodel/data/T_OC.nc4`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/data/T_SAND.nc4` & `permamodel-0.2.1/permamodel/data/T_SAND.nc4`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/data/T_SILT.nc4` & `permamodel-0.2.1/permamodel/data/T_SILT.nc4`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/data/test_directory/inputs/air_temperature.nc` & `permamodel-0.2.1/permamodel/data/test_directory/inputs/air_temperature.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/data/test_directory/inputs/frozen_vegetation_diffusivity.nc` & `permamodel-0.2.1/permamodel/data/test_directory/inputs/frozen_vegetation_diffusivity.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/data/test_directory/inputs/frozen_vegetation_height.nc` & `permamodel-0.2.1/permamodel/data/test_directory/inputs/frozen_vegetation_height.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/data/test_directory/inputs/snow_density.nc` & `permamodel-0.2.1/permamodel/data/test_directory/inputs/snow_density.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/data/test_directory/inputs/snow_thickness.nc` & `permamodel-0.2.1/permamodel/data/test_directory/inputs/snow_thickness.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/data/test_directory/inputs/soil_water_content.nc` & `permamodel-0.2.1/permamodel/data/test_directory/inputs/soil_water_content.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/data/test_directory/inputs/temperature_amplitude.nc` & `permamodel-0.2.1/permamodel/data/test_directory/inputs/temperature_amplitude.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/data/test_directory/inputs/thawed_vegetation_diffusivity.nc` & `permamodel-0.2.1/permamodel/data/test_directory/inputs/thawed_vegetation_diffusivity.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/data/test_directory/inputs/thawed_vegetation_height.nc` & `permamodel-0.2.1/permamodel/data/test_directory/inputs/thawed_vegetation_height.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/examples/Frostnumber_example_singlesite_singleyear.cfg` & `permamodel-0.2.1/permamodel/examples/Frostnumber_example_singlesite_singleyear.cfg`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/examples/Ku_bmi_example_config.toml` & `permamodel-0.2.1/permamodel/examples/Ku_bmi_example_config.toml`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/examples/Ku_example_config.toml` & `permamodel-0.2.1/permamodel/examples/Ku_example_config.toml`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/examples/Ku_method.cfg` & `permamodel-0.2.1/permamodel/examples/Ku_method.cfg`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/tests/test_Ku.py` & `permamodel-0.2.1/permamodel/tests/test_Ku.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/tests/test_Ku_method.py` & `permamodel-0.2.1/permamodel/tests/test_Ku_method.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/tests/test_frost_number.py` & `permamodel-0.2.1/permamodel/tests/test_frost_number.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/tests/test_frost_number_Geo.py` & `permamodel-0.2.1/permamodel/tests/test_frost_number_Geo.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/tests/test_frost_number_Geo_bmi.py` & `permamodel-0.2.1/permamodel/tests/test_frost_number_Geo_bmi.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/tests/test_frost_number_bmi.py` & `permamodel-0.2.1/permamodel/tests/test_frost_number_bmi.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/tests/test_package_directories.py` & `permamodel-0.2.1/permamodel/tests/test_package_directories.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/utils/BMI_base.py` & `permamodel-0.2.1/permamodel/utils/BMI_base.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/utils/file_utils.py` & `permamodel-0.2.1/permamodel/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/utils/model_input.py` & `permamodel-0.2.1/permamodel/utils/model_input.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/utils/outlets.py` & `permamodel-0.2.1/permamodel/utils/outlets.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/utils/pixels.py` & `permamodel-0.2.1/permamodel/utils/pixels.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel/utils/rti_files.py` & `permamodel-0.2.1/permamodel/utils/rti_files.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/permamodel.egg-info/SOURCES.txt` & `permamodel-0.2.1/permamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `permamodel-0.2/pyproject.toml` & `permamodel-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Intended Audience :: Developers",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Education",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 dependencies = [
   "affine",
   "netCDF4",
   "scipy",
   "numpy",
   "pyyaml",
   "python-dateutil",
```

