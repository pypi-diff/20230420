# Comparing `tmp/mapchete-2023.1.1.tar.gz` & `tmp/mapchete-2023.4.0.tar.gz`

## Comparing `mapchete-2023.1.1.tar` & `mapchete-2023.4.0.tar`

### file list

```diff
@@ -1,79 +1,80 @@
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/__init__.py
--rw-r--r--   0        0        0    28465 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/_core.py
--rw-r--r--   0        0        0    26312 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/_executor.py
--rw-r--r--   0        0        0    32385 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/_processing.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/_registered.py
--rw-r--r--   0        0        0    16735 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/_tasks.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/_timer.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/_user_process.py
--rw-r--r--   0        0        0    48221 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/config.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/errors.py
--rw-r--r--   0        0        0    19026 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/index.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/log.py
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/stac.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/testing.py
--rw-r--r--   0        0        0    15520 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/tile.py
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/cli/__init__.py
--rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/cli/main.py
--rw-r--r--   0        0        0    11120 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/cli/options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/cli/default/__init__.py
--rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/cli/default/convert.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/cli/default/cp.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/cli/default/create.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/cli/default/execute.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/cli/default/formats.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/cli/default/index.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/cli/default/processes.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/cli/default/rm.py
--rwxr-xr-x   0        0        0     4936 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/cli/default/serve.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/cli/default/stac.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/commands/__init__.py
--rw-r--r--   0        0        0    15925 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/commands/_convert.py
--rw-r--r--   0        0        0     8477 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/commands/_cp.py
--rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/commands/_execute.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/commands/_index.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/commands/_rm.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/commons/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/commons/clip.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/commons/contours.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/commons/hillshade.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/__init__.py
--rw-r--r--   0        0        0    20950 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/base.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/drivers.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/loaders.py
--rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/default/__init__.py
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/default/_fiona_base.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/default/flatgeobuf.py
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/default/geobuf.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/default/geojson.py
--rw-r--r--   0        0        0    22169 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/default/gtiff.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/default/mapchete_input.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/default/png.py
--rw-r--r--   0        0        0     6698 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/default/png_hillshade.py
--rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/default/raster_file.py
--rw-r--r--   0        0        0    15375 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/default/tile_directory.py
--rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/formats/default/vector_file.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/io/__init__.py
--rw-r--r--   0        0        0    11006 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/io/_geometry_operations.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/io/_json.py
--rw-r--r--   0        0        0     8243 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/io/_misc.py
--rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/io/_path.py
--rw-r--r--   0        0        0    43449 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/io/raster.py
--rw-r--r--   0        0        0    18422 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/io/vector.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/processes/__init__.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/processes/contours.py
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/processes/convert.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/processes/hillshade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/processes/examples/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/processes/examples/example_process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/static/__init__.py
--rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/static/index.html
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/static/mapchete_template.mapchete
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.1.1/mapchete/static/process_template.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mapchete-2023.1.1/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.1.1/LICENSE
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.1.1/README.rst
--rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 mapchete-2023.1.1/pyproject.toml
--rw-r--r--   0        0        0     8922 2020-02-02 00:00:00.000000 mapchete-2023.1.1/PKG-INFO
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/__init__.py
+-rw-r--r--   0        0        0    28539 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/_core.py
+-rw-r--r--   0        0        0    26312 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/_executor.py
+-rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/_processing.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/_registered.py
+-rw-r--r--   0        0        0    16735 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/_tasks.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/_timer.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/_user_process.py
+-rw-r--r--   0        0        0    48250 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/config.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/errors.py
+-rw-r--r--   0        0        0    17249 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/index.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/log.py
+-rw-r--r--   0        0        0    17536 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/stac.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/testing.py
+-rw-r--r--   0        0        0    15520 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/tile.py
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/types.py
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/cli/__init__.py
+-rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/cli/main.py
+-rw-r--r--   0        0        0    11120 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/cli/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/cli/default/__init__.py
+-rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/cli/default/convert.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/cli/default/cp.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/cli/default/create.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/cli/default/execute.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/cli/default/formats.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/cli/default/index.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/cli/default/processes.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/cli/default/rm.py
+-rwxr-xr-x   0        0        0     4936 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/cli/default/serve.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/cli/default/stac.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/commands/__init__.py
+-rw-r--r--   0        0        0    15925 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/commands/_convert.py
+-rw-r--r--   0        0        0     8477 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/commands/_cp.py
+-rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/commands/_execute.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/commands/_index.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/commands/_rm.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/commons/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/commons/clip.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/commons/contours.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/commons/hillshade.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/__init__.py
+-rw-r--r--   0        0        0    20950 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/base.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/drivers.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/loaders.py
+-rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/default/__init__.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/default/_fiona_base.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/default/flatgeobuf.py
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/default/geobuf.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/default/geojson.py
+-rw-r--r--   0        0        0    22206 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/default/gtiff.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/default/mapchete_input.py
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/default/png.py
+-rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/default/png_hillshade.py
+-rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/default/raster_file.py
+-rw-r--r--   0        0        0    15375 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/default/tile_directory.py
+-rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/formats/default/vector_file.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/io/__init__.py
+-rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/io/_geometry_operations.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/io/_json.py
+-rw-r--r--   0        0        0     8048 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/io/_misc.py
+-rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/io/_path.py
+-rw-r--r--   0        0        0    43386 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/io/raster.py
+-rw-r--r--   0        0        0    17903 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/io/vector.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/processes/__init__.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/processes/contours.py
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/processes/convert.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/processes/hillshade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/processes/examples/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/processes/examples/example_process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/static/__init__.py
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/static/index.html
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/static/mapchete_template.mapchete
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.4.0/mapchete/static/process_template.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mapchete-2023.4.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.4.0/LICENSE
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.4.0/README.rst
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 mapchete-2023.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 mapchete-2023.4.0/PKG-INFO
```

### Comparing `mapchete-2023.1.1/mapchete/__init__.py` & `mapchete-2023.4.0/mapchete/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,11 +16,11 @@
     "ProcessInfo",
     "Timer",
     "Executor",
     "FakeFuture",
     "SkippedFuture",
     "Job",
 ]
-__version__ = "2023.1.1"
+__version__ = "2023.4.0"
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
```

### Comparing `mapchete-2023.1.1/mapchete/_core.py` & `mapchete-2023.4.0/mapchete/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
                 self.config.area_at_zoom(zoom),
                 zoom=zoom,
                 batch_by=batch_by,
                 exact=True,
             ):
                 yield tile
         else:
-            for i in reversed(self.config.zoom_levels):
+            for i in self.config.zoom_levels.descending():
                 for tile in self.config.process_pyramid.tiles_from_geom(
                     self.config.area_at_zoom(i), zoom=i, batch_by=batch_by, exact=True
                 ):
                     yield tile
 
     def skip_tiles(self, tiles=None, tiles_batches=None):
         """
@@ -419,15 +419,15 @@
                 process=self,
                 tile=self.config.process_pyramid.tile(*tuple(tile)),
             ).result()
         # run area
         else:
             for future in _run_area(
                 process=self,
-                zoom_levels=list(_get_zoom_level(zoom, self)),
+                zoom_levels=_get_zoom_level(zoom, self),
                 dask_scheduler=dask_scheduler,
                 dask_max_submitted_tasks=dask_max_submitted_tasks,
                 dask_chunksize=dask_chunksize,
                 workers=workers or multiprocessing.cpu_count(),
                 multiprocessing_module=multiprocessing_module or multiprocessing,
                 multiprocessing_start_method=multiprocessing_start_method,
                 skip_output_check=skip_output_check,
@@ -469,16 +469,16 @@
         init_zoom : int
             initial zoom level used for tile count algorithm
 
         Returns
         -------
         number of tiles
         """
-        minzoom = min(self.config.init_zoom_levels) if minzoom is None else minzoom
-        maxzoom = max(self.config.init_zoom_levels) if maxzoom is None else maxzoom
+        minzoom = self.config.init_zoom_levels.min if minzoom is None else minzoom
+        maxzoom = self.config.init_zoom_levels.max if maxzoom is None else maxzoom
         if (minzoom, maxzoom) not in self._count_tiles_cache:
             logger.debug("counting tiles...")
             with Timer() as t:
                 self._count_tiles_cache[(minzoom, maxzoom)] = count_tiles(
                     self.config.area_at_zoom(),
                     self.config.process_pyramid,
                     minzoom,
@@ -765,14 +765,15 @@
         # run input drivers cleanup
         for ip in self.config.input.values():
             if ip is not None:
                 logger.debug(f"running cleanup on {ip}...")
                 ip.cleanup()
         # run output driver cleanup
         logger.debug(f"closing output driver {self.config.output}...")
+        # HINT: probably cleaner to use the outputs __exit__ function and use a contextmanager interface
         self.config.output.close(
             exc_type=exc_type, exc_value=exc_value, exc_traceback=exc_traceback
         )
         # clean up internal cache
         if self.with_cache:
             self.process_tile_cache = None
             self.current_processes = None
@@ -780,10 +781,8 @@
 
     def __repr__(self):  # pragma: no cover
         return f"Mapchete <process_name={self.process_name}>"
 
 
 def _get_zoom_level(zoom, process):
     """Determine zoom levels."""
-    return (
-        reversed(process.config.zoom_levels) if zoom is None else validate_zooms(zoom)
-    )
+    return process.config.zoom_levels if zoom is None else validate_zooms(zoom)
```

### Comparing `mapchete-2023.1.1/mapchete/_executor.py` & `mapchete-2023.4.0/mapchete/_executor.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/_processing.py` & `mapchete-2023.4.0/mapchete/_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 """Internal processing classes and functions."""
 
 from collections import namedtuple
 from contextlib import ExitStack
-from itertools import chain
 import logging
 import multiprocessing
 import os
 from shapely.geometry import mapping
-from tilematrix._funcs import Bounds
-from traceback import format_exc
 from typing import Generator
 
 from mapchete.config import get_process_func
 from mapchete._executor import (
     DaskExecutor,
     Executor,
     SkippedFuture,
     FinishedFuture,
     future_raise_exception,
 )
 from mapchete.errors import MapcheteNodataTile, MapcheteTaskFailed
 from mapchete._tasks import to_dask_collection, TileTaskBatch, TileTask, TaskBatch
 from mapchete._timer import Timer
-from mapchete.validate import validate_zooms
+from mapchete.types import Bounds, ZoomLevels
 
 FUTURE_TIMEOUT = float(os.environ.get("MP_FUTURE_TIMEOUT", 10))
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -159,28 +156,29 @@
             tasks=process.config.preprocessing_tasks().values(),
             func=_preprocess_task_wrapper,
         )
     logger.debug("preprocessing tasks batch generated in %s", duration)
 
     with Timer() as duration:
         if tile:
-            zoom_levels = [tile.zoom]
+            zoom_levels = ZoomLevels.from_inp(tile.zoom)
             skip_output_check = True
             tiles = {tile.zoom: [(tile, False)]}
         else:
-            zoom_levels = list(
-                process.config.zoom_levels if zoom is None else validate_zooms(zoom)
+            zoom_levels = (
+                process.config.zoom_levels
+                if zoom is None
+                else ZoomLevels.from_inp(zoom)
             )
-            zoom_levels.sort(reverse=True)
             tiles = {}
 
             # here we store the parents of tiles about to be processed so we can update overviews
             # also in "continue" mode in case there were updates at the baselevel
             overview_parents = set()
-            for i, zoom in enumerate(zoom_levels):
+            for i, zoom in enumerate(zoom_levels.descending()):
                 tiles[zoom] = []
 
                 for tile, skip, _ in _filter_skipable(
                     process=process,
                     tiles_batches=process.get_process_tiles(zoom, batch_by="row"),
                     target_set=(
                         overview_parents if process.config.baselevels and i else None
@@ -206,15 +204,15 @@
         else:
             func = _execute_and_write
             fkwargs = dict(
                 append_data=propagate_results, output_writer=process.config.output
             )
 
         # tile tasks
-        for zoom in zoom_levels:
+        for zoom in zoom_levels.descending():
             yield TileTaskBatch(
                 id=f"zoom_{zoom}",
                 tasks=(
                     TileTask(
                         tile=tile,
                         config=process.config,
                         skip=(
@@ -266,20 +264,21 @@
                 )
             )
 
         logger.info("run process on area")
         duration = exit_stack.enter_context(Timer())
         if tile:
             tile = process.config.process_pyramid.tile(*tile)
-            zoom_levels = [tile.zoom]
+            zoom_levels = ZoomLevels.from_inp(tile.zoom)
         else:
-            zoom_levels = list(
-                process.config.zoom_levels if zoom is None else validate_zooms(zoom)
+            zoom_levels = (
+                process.config.zoom_levels
+                if zoom is None
+                else ZoomLevels.from_inp(zoom)
             )
-        zoom_levels.sort(reverse=True)
         if dask_compute_graph and isinstance(executor, DaskExecutor):
             for num_processed, future in enumerate(
                 _compute_task_graph(
                     executor=executor,
                     process=process,
                     zoom_levels=zoom_levels,
                     tile=tile,
@@ -429,16 +428,14 @@
     dask_chunksize=None,
     workers=None,
     multiprocessing_module=None,
     multiprocessing_start_method=None,
     skip_output_check=False,
 ):
     logger.info("run process on area")
-    zoom_levels.sort(reverse=True)
-
     # for output drivers requiring writing data in parent process
     if process.config.output.write_in_parent_process:
         for future in _run_multi(
             executor=executor,
             func=_execute,
             zoom_levels=zoom_levels,
             process=process,
@@ -500,16 +497,15 @@
     workers=None,
     multiprocessing_start_method=None,
     multiprocessing_module=None,
     write_in_parent_process=False,
     fkwargs=None,
     skip_output_check=False,
 ):
-    zoom_levels.sort(reverse=True)
-    total_tiles = process.count_tiles(min(zoom_levels), max(zoom_levels))
+    total_tiles = process.count_tiles(zoom_levels.min, zoom_levels.max)
     workers = min([workers, total_tiles])
     num_processed = 0
 
     # If an Executor is passed on, don't close after processing. If no Executor is passed on,
     # create one and properly close it afterwards.
     with ExitStack() as exit_stack:
         # create fresh Executor if it was not passed on
@@ -703,15 +699,15 @@
     dask_chunksize=None,
     write_in_parent_process=None,
 ):
     # here we store the parents of processed tiles so we can update overviews
     # also in "continue" mode in case there were updates at the baselevel
     overview_parents = set()
 
-    for i, zoom in enumerate(zoom_levels):
+    for i, zoom in enumerate(zoom_levels.descending()):
 
         logger.debug("sending tasks to executor %s...", executor)
         # get generator list of tiles, whether they are to be skipped and skip_info
         # from _filter_skipable and pass on to executor
         for future in executor.as_completed(
             func=func,
             iterable=(
@@ -810,15 +806,15 @@
                 skip,
                 process_msg,
             )
             for tile, skip, process_msg in _filter_skipable(
                 process=process,
                 tiles_batches=(
                     batch
-                    for zoom in zoom_levels
+                    for zoom in zoom_levels.descending()
                     for batch in process.get_process_tiles(zoom, batch_by="row")
                 ),
                 target_set=None,
                 skip_output_check=skip_output_check,
             )
         ),
         fkwargs=fkwargs,
```

### Comparing `mapchete-2023.1.1/mapchete/_registered.py` & `mapchete-2023.4.0/mapchete/_registered.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/_tasks.py` & `mapchete-2023.4.0/mapchete/_tasks.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/_timer.py` & `mapchete-2023.4.0/mapchete/_timer.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/_user_process.py` & `mapchete-2023.4.0/mapchete/_user_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/config.py` & `mapchete-2023.4.0/mapchete/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 import py_compile
 from shapely import wkt
 from shapely.geometry import box, Point, shape
 from shapely.geometry.base import BaseGeometry
 from shapely.ops import unary_union
 import sys
 from tempfile import NamedTemporaryFile
-from tilematrix._funcs import Bounds
 import warnings
 
 from mapchete.validate import (
     validate_bounds,
     validate_zooms,
     validate_values,
     validate_bufferedtilepyramid,
@@ -52,14 +51,15 @@
     available_output_formats,
     load_input_reader,
 )
 from mapchete.io import absolute_path
 from mapchete.io.vector import clean_geometry_type, reproject_geometry
 from mapchete.log import add_module_logger
 from mapchete.tile import BufferedTilePyramid
+from mapchete.types import Bounds
 
 
 logger = logging.getLogger(__name__)
 
 # parameters which have to be provided in the configuration and their types
 _MANDATORY_PARAMETERS = [
     ("process", (str, list, type(None))),  # path to .py file or module path
@@ -390,14 +390,15 @@
         """
         try:
             return get_zoom_levels(
                 process_zoom_levels=self._raw["zoom_levels"],
                 init_zoom_levels=self._raw["init_zoom_levels"],
             )
         except Exception as e:
+            logger.exception(e)
             raise MapcheteConfigError(e)
 
     @cached_property
     def effective_bounds(self):
         """
         Effective process bounds required to initialize inputs.
```

### Comparing `mapchete-2023.1.1/mapchete/errors.py` & `mapchete-2023.4.0/mapchete/errors.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/index.py` & `mapchete-2023.4.0/mapchete/index.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 from rasterio.dtypes import _gdal_typename
 from shapely.geometry import mapping
 import xml.etree.ElementTree as ET
 from xml.dom import minidom
 
 from mapchete.config import get_zoom_levels
 from mapchete.io import (
+    fs_from_path,
     path_exists,
     path_is_remote,
-    get_boto3_bucket,
     raster,
     relative_path,
     tiles_exist,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -279,107 +279,69 @@
 
 
 class TextFileWriter:
     """Writes tile paths into text file."""
 
     def __init__(self, out_path=None):
         self.path = out_path
-        self._bucket = (
-            self.path.split("/")[2] if self.path.startswith("s3://") else None
-        )
-        self.bucket_resource = get_boto3_bucket(self._bucket) if self._bucket else None
         logger.debug("initialize TXT writer")
+        self.fs = fs_from_path(out_path)
         if path_exists(self.path):
-            if self._bucket:
-                key = "/".join(self.path.split("/")[3:])
-                for obj in self.bucket_resource.objects.filter(Prefix=key):
-                    if obj.key == key:
-                        self._existing = {
-                            l + "\n"
-                            for l in obj.get()["Body"].read().decode().split("\n")
-                            if l
-                        }
-            else:
-                with open(self.path) as src:
-                    self._existing = {l for l in src}
+            with self.fs.open(self.path, "r") as src:
+                self._existing = {l for l in src.readlines()}
         else:
             self._existing = {}
         self.new_entries = 0
-        if self._bucket:
-            self.sink = ""
-        else:
-            self.sink = open(self.path, "w")
+        self.sink = self.fs.open(self.path, "w")
         for l in self._existing:
             self._write_line(l)
 
     def __repr__(self):
         return "TextFileWriter(%s)" % self.path
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.close()
 
     def _write_line(self, line):
-        if self._bucket:
-            self.sink += line
-        else:
-            self.sink.write(line)
+        self.sink.write(line)
 
     def write(self, tile, path):
         if not self.entry_exists(path=path):
             logger.debug("write %s to %s", path, self)
             self._write_line(path + "\n")
             self.new_entries += 1
 
     def entry_exists(self, tile=None, path=None):
         exists = path + "\n" in self._existing
         logger.debug("tile %s with path %s exists: %s", tile, path, exists)
         return exists
 
     def close(self):
         logger.debug("%s new entries in %s", self.new_entries, self)
-        if self._bucket:
-            key = "/".join(self.path.split("/")[3:])
-            logger.debug("upload %s", key)
-            self.bucket_resource.put_object(Key=key, Body=self.sink)
-        else:
-            self.sink.close()
+        self.sink.close()
 
 
 class VRTFileWriter:
     """Generates GDAL-style VRT file."""
 
     def __init__(self, out_path=None, output=None, out_pyramid=None):
         # see if lxml is installed before checking all output tiles
         from lxml.builder import ElementMaker
 
         self.path = out_path
         self._tp = out_pyramid
         self._output = output
-        self._bucket = (
-            self.path.split("/")[2] if self.path.startswith("s3://") else None
-        )
-        self.bucket_resource = get_boto3_bucket(self._bucket) if self._bucket else None
+        self.fs = fs_from_path(out_path)
         logger.debug("initialize VRT writer for %s", self.path)
         if path_exists(self.path):
-            if self._bucket:
-                key = "/".join(self.path.split("/")[3:])
-                for obj in self.bucket_resource.objects.filter(Prefix=key):
-                    if obj.key == key:
-                        self._existing = {
-                            k: v
-                            for k, v in self._xml_to_entries(
-                                obj.get()["Body"].read().decode()
-                            )
-                        }
-            else:
-                with open(self.path) as src:
-                    self._existing = {k: v for k, v in self._xml_to_entries(src.read())}
+            with self.fs.open(self.path) as src:
+                self._existing = {k: v for k, v in self._xml_to_entries(src.read())}
         else:
             self._existing = {}
         logger.debug("%s existing entries", len(self._existing))
         self.new_entries = 0
         self._new = {}
 
     def __repr__(self):
@@ -508,15 +470,10 @@
                 for b_idx in range(1, self._output.profile()["count"] + 1)
             ],
             rasterXSize=str(vrt_shape.width),
             rasterYSize=str(vrt_shape.height),
         )
         # generate pretty XML and write
         xmlstr = minidom.parseString(ET.tostring(vrt)).toprettyxml(indent="  ")
-        if self._bucket:
-            key = "/".join(self.path.split("/")[3:])
-            logger.debug("upload %s", key)
-            self.bucket_resource.put_object(Key=key, Body=xmlstr)
-        else:
-            logger.debug("write to %s", self.path)
-            with open(self.path, "w") as dst:
-                dst.write(xmlstr)
+        logger.debug("write to %s", self.path)
+        with self.fs.open(self.path, "w") as dst:
+            dst.write(xmlstr)
```

### Comparing `mapchete-2023.1.1/mapchete/log.py` & `mapchete-2023.4.0/mapchete/log.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/stac.py` & `mapchete-2023.4.0/mapchete/stac.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 import logging
 import numpy as np
 import numpy.ma as ma
 import os
 from pyproj import CRS
 from shapely.geometry import box, mapping
 
-from tilematrix._funcs import Bounds
-
 from mapchete.errors import ReprojectionFailed
 from mapchete.io import makedirs
 from mapchete.io.raster import write_raster_window
 from mapchete.io.vector import reproject_geometry
 from mapchete.tile import BufferedTilePyramid
+from mapchete.types import Bounds
 
 
 logger = logging.getLogger(__name__)
 
 OUT_PIXEL_SIZE = 0.28e-3
 UNIT_TO_METER = {"mercator": 1, "geodetic": 111319.4907932732}
 KNOWN_MATRIX_PROPERTIES = {
```

### Comparing `mapchete-2023.1.1/mapchete/testing.py` & `mapchete-2023.4.0/mapchete/testing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/tile.py` & `mapchete-2023.4.0/mapchete/tile.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/validate.py` & `mapchete-2023.4.0/mapchete/validate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,48 @@
 """Convenience validator functions for core and extension packages."""
 
 
+from collections.abc import Iterable
 import numpy.ma as ma
 from rasterio.crs import CRS
-from tilematrix._funcs import Bounds
+from typing import Union, List, Dict
 import warnings
 
 from mapchete.tile import BufferedTile, BufferedTilePyramid
+from mapchete.types import Bounds, ZoomLevels
 
 ########################
 # validator functionrs #
 ########################
 
 
-def validate_zooms(zooms, expand=True):
+def validate_zooms(
+    zooms: Union[int, Dict[str, int], List[int]], **kwargs
+) -> ZoomLevels:
     """
     Return a list of zoom levels.
 
     Following inputs are converted:
     - int --> [int]
     - dict{min, max} --> [min ... max + 1]
     - [int] --> [int]
     - [int, int] --> [smaller int, bigger int + 1]
 
     Parameters
     ----------
     zoom : dict, int or list
-    expand : bool
-        Return full list of zoom levels instead of [min, max]
 
     Returns
     -------
     List of zoom levels.
     """
-    if isinstance(zooms, dict):
-        if any([a not in zooms for a in ["min", "max"]]):
-            raise TypeError("min and max zoom required: %s" % str(zooms))
-        zmin = validate_zoom(zooms["min"])
-        zmax = validate_zoom(zooms["max"])
-        if zmin > zmax:
-            raise TypeError(
-                "max zoom must not be smaller than min zoom: %s" % str(zooms)
-            )
-        return list(range(zmin, zmax + 1)) if expand else zooms
-    elif isinstance(zooms, list):
-        if len(zooms) == 1:
-            return zooms
-        elif len(zooms) == 2:
-            zmin, zmax = sorted([validate_zoom(z) for z in zooms])
-            return list(range(zmin, zmax + 1)) if expand else zooms
-        else:
-            return zooms
-    else:
-        return [validate_zoom(zooms)] if expand else zooms
+    return ZoomLevels.from_inp(zooms)
 
 
-def validate_zoom(zoom):
-    """
-    Return validated zoom.
-
-    Assert zoom value is positive integer.
-
-    Returns
-    -------
-    zoom
-
-    Raises
-    ------
-    TypeError if type is invalid.
-    """
-    if any([not isinstance(zoom, int), zoom < 0]):
-        raise TypeError("zoom must be a positive integer: %s" % zoom)
-    return zoom
-
-
-def validate_bounds(bounds) -> Bounds:
+def validate_bounds(bounds: Iterable) -> Bounds:
     """
     Return validated bounds.
 
     Bounds must be a list or tuple with exactly four elements.
 
     Parameters
     ----------
@@ -88,19 +52,15 @@
     -------
     Bounds
 
     Raises
     ------
     TypeError if type is invalid.
     """
-    if not isinstance(bounds, (tuple, list)):
-        raise TypeError("bounds must be either a tuple or a list: %s" % str(bounds))
-    if len(bounds) != 4:
-        raise ValueError("bounds has to have exactly four values: %s" % str(bounds))
-    return Bounds(*bounds)
+    return Bounds.from_inp(bounds)
 
 
 def validate_values(config, values):
     """
     Return True if all values are given and have the desired type.
 
     Parameters
```

### Comparing `mapchete-2023.1.1/mapchete/cli/options.py` & `mapchete-2023.4.0/mapchete/cli/options.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/cli/default/convert.py` & `mapchete-2023.4.0/mapchete/cli/default/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/cli/default/cp.py` & `mapchete-2023.4.0/mapchete/cli/default/cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/cli/default/create.py` & `mapchete-2023.4.0/mapchete/cli/default/create.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/cli/default/execute.py` & `mapchete-2023.4.0/mapchete/cli/default/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/cli/default/formats.py` & `mapchete-2023.4.0/mapchete/cli/default/formats.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/cli/default/index.py` & `mapchete-2023.4.0/mapchete/cli/default/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/cli/default/processes.py` & `mapchete-2023.4.0/mapchete/cli/default/processes.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/cli/default/rm.py` & `mapchete-2023.4.0/mapchete/cli/default/rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/cli/default/serve.py` & `mapchete-2023.4.0/mapchete/cli/default/serve.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/cli/default/stac.py` & `mapchete-2023.4.0/mapchete/cli/default/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/commands/_convert.py` & `mapchete-2023.4.0/mapchete/commands/_convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/commands/_cp.py` & `mapchete-2023.4.0/mapchete/commands/_cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/commands/_execute.py` & `mapchete-2023.4.0/mapchete/commands/_execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/commands/_index.py` & `mapchete-2023.4.0/mapchete/commands/_index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/commands/_rm.py` & `mapchete-2023.4.0/mapchete/commands/_rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/commons/clip.py` & `mapchete-2023.4.0/mapchete/commons/clip.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/commons/contours.py` & `mapchete-2023.4.0/mapchete/commons/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/commons/hillshade.py` & `mapchete-2023.4.0/mapchete/commons/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/formats/__init__.py` & `mapchete-2023.4.0/mapchete/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/formats/base.py` & `mapchete-2023.4.0/mapchete/formats/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/formats/loaders.py` & `mapchete-2023.4.0/mapchete/formats/loaders.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/formats/tools.py` & `mapchete-2023.4.0/mapchete/formats/tools.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/formats/default/_fiona_base.py` & `mapchete-2023.4.0/mapchete/formats/default/_fiona_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import fiona
 from fiona.errors import DriverError
 import logging
 import types
 
 from mapchete.config import validate_values
 from mapchete.formats import base
-from mapchete.io import get_boto3_bucket
 from mapchete.io.vector import write_vector_window
 from mapchete.tile import BufferedTile
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -158,29 +157,25 @@
                 "vector driver data has to be a list or generator of GeoJSON objects"
             )
 
         data = list(data)
         if not len(data):  # pragma: no cover
             logger.debug("no features to write")
         else:
-            # in case of S3 output, create an boto3 resource
-            bucket_resource = get_boto3_bucket(self._bucket) if self._bucket else None
-
             # Convert from process_tile to output_tiles
             for tile in self.pyramid.intersecting(process_tile):
                 out_path = self.get_path(tile)
                 self.prepare_path(tile)
                 out_tile = BufferedTile(tile, self.pixelbuffer)
                 write_vector_window(
                     in_data=data,
                     out_driver=self.METADATA["driver_name"],
                     out_schema=self.output_params["schema"],
                     out_tile=out_tile,
                     out_path=out_path,
-                    bucket_resource=bucket_resource,
                     allow_multipart_geometries=(
                         self.output_params["schema"]["geometry"].startswith("Multi")
                     ),
                 )
 
 
 class InputTile(base.InputTile):
```

### Comparing `mapchete-2023.1.1/mapchete/formats/default/flatgeobuf.py` & `mapchete-2023.4.0/mapchete/formats/default/flatgeobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/formats/default/geobuf.py` & `mapchete-2023.4.0/mapchete/formats/default/geobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/formats/default/geojson.py` & `mapchete-2023.4.0/mapchete/formats/default/geojson.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/formats/default/gtiff.py` & `mapchete-2023.4.0/mapchete/formats/default/gtiff.py`

 * *Files 1% similar despite different names*

```diff
@@ -642,15 +642,15 @@
                     )
                     self.dst.update_tags(
                         OVR_RESAMPLING_ALG=Resampling[
                             self.overviews_resampling
                         ].name.upper()
                     )
         finally:
-            self._ctx.close()
+            self._ctx.__exit__(exc_type, exc_value, exc_traceback)
 
 
 def _window_in_out_file(window, rio_file):
     return all(
         [
             window.row_off >= 0,
             window.col_off >= 0,
```

### Comparing `mapchete-2023.1.1/mapchete/formats/default/mapchete_input.py` & `mapchete-2023.4.0/mapchete/formats/default/mapchete_input.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/formats/default/png.py` & `mapchete-2023.4.0/mapchete/formats/default/png_hillshade.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
-PNG process output.
+Special PNG process output for hillshades.
+
+Writes inverted hillshade into alpha channel of black image, so that hillshade
+can be used as overlay over other data.
 
 output configuration parameters
 -------------------------------
 
 mandatory
 ~~~~~~~~~
 
-bands: integer
-    number of output bands to be written
 path: string
     output directory
 
 optional
 ~~~~~~~~
 
 nodata: integer or float
@@ -21,48 +22,48 @@
 
 import logging
 import numpy as np
 import numpy.ma as ma
 
 from mapchete.config import validate_values
 from mapchete.formats import base
-from mapchete.io import get_boto3_bucket
 from mapchete.io.raster import (
     write_raster_window,
     prepare_array,
     memory_file,
     read_raster_no_crs,
 )
 from mapchete.tile import BufferedTile
 
 
 logger = logging.getLogger(__name__)
-METADATA = {"driver_name": "PNG", "data_type": "raster", "mode": "w"}
-PNG_DEFAULT_PROFILE = {"dtype": "uint8", "driver": "PNG", "count": 4, "nodata": 0}
+METADATA = {"driver_name": "PNG_hillshade", "data_type": "raster", "mode": "w"}
+PNG_DEFAULT_PROFILE = {"dtype": "uint8", "driver": "PNG", "count": 2, "nodata": 255}
 
 
 class OutputDataReader(base.TileDirectoryOutputReader):
     """
-    PNG output class.
+    PNG_hillshade output class.
 
     Parameters
     ----------
     output_params : dictionary
         output parameters from Mapchete file
 
     Attributes
     ----------
     path : string
         path to output directory
     file_extension : string
-        file extension for output files (.png)
+        file extension for output files (.tif)
     output_params : dictionary
         output parameters from Mapchete file
-    nodata : integer or float
-        nodata value used when writing PNGs
+    old_band_num : bool
+        in prior versions, 4 channels (3x gray 1x alpha) were written, now
+        2 channels (1x gray, 1x alpha)
     pixelbuffer : integer
         buffer around output tiles
     pyramid : ``tilematrix.TilePyramid``
         output ``TilePyramid``
     crs : ``rasterio.crs.CRS``
         object describing the process coordinate reference system
     srid : string
@@ -77,17 +78,21 @@
         self.path = output_params["path"]
         self.file_extension = ".png"
         self.output_params = dict(
             output_params,
             nodata=output_params.get("nodata", PNG_DEFAULT_PROFILE["nodata"]),
             dtype=PNG_DEFAULT_PROFILE["dtype"],
         )
-        self._bucket = (
-            self.path.split("/")[2] if self.path.startswith("s3://") else None
-        )
+        self._profile = dict(PNG_DEFAULT_PROFILE)
+        try:
+            self.old_band_num = output_params["old_band_num"]
+            self._profile.update(count=4)
+        except KeyError:
+            self.old_band_num = False
+        self.output_params.update(dtype=self._profile["dtype"])
 
     def read(self, output_tile, **kwargs):
         """
         Read existing process output.
 
         Parameters
         ----------
@@ -95,15 +100,20 @@
             must be member of output ``TilePyramid``
 
         Returns
         -------
         process output : ``BufferedTile`` with appended data
         """
         try:
-            return read_raster_no_crs(self.get_path(output_tile))
+            return ma.masked_values(
+                read_raster_no_crs(
+                    self.get_path(output_tile), indexes=(4 if self.old_band_num else 2)
+                ),
+                0,
+            )
         except FileNotFoundError:
             return self.empty(output_tile)
 
     def is_valid_with_config(self, config):
         """
         Check if output format is valid with other process parameters.
 
@@ -127,129 +137,92 @@
         tile : ``BufferedTile``
 
         Returns
         -------
         metadata : dictionary
             output profile dictionary used for rasterio.
         """
-        dst_metadata = PNG_DEFAULT_PROFILE
-        dst_metadata.pop("transform", None)
+        dst_metadata = dict(self._profile)
         if tile is not None:
             dst_metadata.update(
-                width=tile.width, height=tile.height, affine=tile.affine, crs=tile.crs
+                width=tile.width,
+                height=tile.height,
+                affine=tile.affine,
+                driver="PNG",
+                crs=tile.crs,
             )
-        try:
-            dst_metadata.update(count=self.output_params["count"])
-        except KeyError:
-            pass
         return dst_metadata
 
     def for_web(self, data):
         """
         Convert data to web output.
 
         Parameters
         ----------
         data : array
 
         Returns
         -------
-        web data : array
+        MemoryFile(), MIME type
         """
-        rgba = self._prepare_array_for_png(data)
-        data = ma.masked_where(rgba == self.output_params["nodata"], rgba)
-        return memory_file(data, self.profile()), "image/png"
+        return (
+            memory_file(self._prepare_array(data), self.profile()),
+            "image/png",
+        )  # pragma: no cover
 
     def empty(self, process_tile):
         """
         Return empty data.
 
         Parameters
         ----------
         process_tile : ``BufferedTile``
             must be member of process ``TilePyramid``
 
         Returns
         -------
-        empty data : array
-            empty array with data type given in output parameters
-        """
-        bands = (
-            self.output_params["bands"]
-            if "bands" in self.output_params
-            else PNG_DEFAULT_PROFILE["count"]
-        )
-        return ma.masked_array(
-            data=ma.zeros((bands,) + process_tile.shape),
-            mask=ma.zeros((bands,) + process_tile.shape),
-            dtype=PNG_DEFAULT_PROFILE["dtype"],
-        )
-
-    def _prepare_array_for_png(self, data):
-        data = prepare_array(data, dtype=np.uint8)
-        # Create 3D NumPy array with alpha channel.
-        if len(data) == 1:
-            rgba = np.stack(
-                (
-                    data[0],
-                    data[0],
-                    data[0],
-                    np.where(
-                        data[0].data == self.output_params["nodata"], 0, 255
-                    ).astype("uint8"),
-                )
-            )
-        elif len(data) == 2:
-            rgba = np.stack((data[0], data[0], data[0], data[1]))
-        elif len(data) == 3:
-            rgba = np.stack(
-                (
-                    data[0],
-                    data[1],
-                    data[2],
-                    np.where(
-                        data[0].data == self.output_params["nodata"], 0, 255
-                    ).astype("uint8", copy=False),
-                )
-            )
-        elif len(data) == 4:
-            rgba = np.array(data).astype("uint8", copy=False)
+        empty data : array or list
+            empty array with correct data type for raster data or empty list
+            for vector data
+        """
+        return ma.masked_values(np.zeros(process_tile.shape), 0)
+
+    def _prepare_array(self, data):
+        data = prepare_array(-(data - 255), dtype="uint8", masked=False, nodata=0)[0]
+        zeros = np.zeros(data.shape)
+        if self.old_band_num:
+            data = np.stack([zeros, zeros, zeros, data])
         else:
-            raise TypeError("invalid number of bands: %s" % len(data))
-        return rgba
+            data = np.stack([zeros, data])
+        return prepare_array(data, dtype="uint8", masked=True, nodata=255)
 
 
 class OutputDataWriter(base.OutputDataWriter, OutputDataReader):
 
     METADATA = METADATA
 
     def write(self, process_tile, data):
         """
-        Write data from one or more process tiles.
+        Write data from process tiles into PNG file(s).
 
         Parameters
         ----------
         process_tile : ``BufferedTile``
             must be member of process ``TilePyramid``
         """
-        rgba = self._prepare_array_for_png(data)
-        data = ma.masked_where(rgba == self.output_params["nodata"], rgba)
+        data = self._prepare_array(data)
 
-        if data.mask.all():
+        if data.mask.all():  # pragma: no cover
             logger.debug("data empty, nothing to write")
         else:
-            # in case of S3 output, create an boto3 resource
-            bucket_resource = get_boto3_bucket(self._bucket) if self._bucket else None
-
             # Convert from process_tile to output_tiles and write
             for tile in self.pyramid.intersecting(process_tile):
                 out_path = self.get_path(tile)
                 self.prepare_path(tile)
                 out_tile = BufferedTile(tile, self.pixelbuffer)
                 write_raster_window(
                     in_tile=process_tile,
                     in_data=data,
                     out_profile=self.profile(out_tile),
                     out_tile=out_tile,
                     out_path=out_path,
-                    bucket_resource=bucket_resource,
                 )
```

### Comparing `mapchete-2023.1.1/mapchete/formats/default/raster_file.py` & `mapchete-2023.4.0/mapchete/formats/default/raster_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/formats/default/tile_directory.py` & `mapchete-2023.4.0/mapchete/formats/default/tile_directory.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/formats/default/vector_file.py` & `mapchete-2023.4.0/mapchete/formats/default/vector_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/io/__init__.py` & `mapchete-2023.4.0/mapchete/io/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/io/_geometry_operations.py` & `mapchete-2023.4.0/mapchete/io/_geometry_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import fiona
 from fiona.transform import transform_geom
 import logging
 import pyproj
 from rasterio.crs import CRS
 from shapely.errors import TopologicalError
 from shapely.geometry import (
     box,
@@ -30,26 +31,60 @@
     # unknown source
     "epsg:3857": (-180.0, -85.0511, 180.0, 85.0511),
     # http://spatialreference.org/ref/epsg/3035/
     "epsg:3035": (-10.6700, 34.5000, 31.5500, 71.0500),
 }
 
 
+def _reproject_geom(
+    geometry, src_crs, dst_crs, validity_check, antimeridian_cutting, fiona_env
+):
+    if geometry.is_empty:
+        return geometry
+    else:
+        with fiona.env.Env(**fiona_env):
+            try:
+                transformed = transform_geom(
+                    src_crs.to_dict(),
+                    dst_crs.to_dict(),
+                    mapping(geometry),
+                    antimeridian_cutting=antimeridian_cutting,
+                )
+            except Exception as exc:
+                raise ReprojectionFailed(
+                    f"fiona.transform.transform_geom could not transform geometry from {src_crs} to {dst_crs}"
+                ) from exc
+        # Fiona >1.9 returns None if transformation errored
+        if transformed is None:  # pragma: no cover
+            raise ReprojectionFailed(
+                f"fiona.transform.transform_geom could not transform geometry from {src_crs} to {dst_crs}"
+            )
+        out_geom = to_shape(transformed)
+        return _repair(out_geom) if validity_check else out_geom
+
+
+def _segmentize_value(geometry, segmentize_fraction):
+    height = geometry.bounds[3] - geometry.bounds[1]
+    width = geometry.bounds[2] - geometry.bounds[0]
+    return min([height, width]) / segmentize_fraction
+
+
 def reproject_geometry(
     geometry,
     src_crs=None,
     dst_crs=None,
     clip_to_crs_bounds=True,
     error_on_clip=False,
     segmentize_on_clip=False,
     segmentize=False,
     segmentize_fraction=100,
     validity_check=True,
     antimeridian_cutting=False,
     retry_with_clip=True,
+    fiona_env=None,
 ):
     """
     Reproject a geometry to target CRS.
 
     Also, clips geometry if it lies outside the destination CRS boundary.
     Supported destination CRSes for clipping: 4326 (WGS84), 3857 (Spherical
     Mercator) and 3035 (ETRS89 / ETRS-LAEA).
@@ -74,44 +109,22 @@
 
     Returns
     -------
     geometry : ``shapely.geometry``
     """
     src_crs = validate_crs(src_crs)
     dst_crs = validate_crs(dst_crs)
+    fiona_env = fiona_env or {}
     try:
         geometry = (
             geometry if isinstance(geometry, base.BaseGeometry) else shape(geometry)
         )
     except Exception:  # pragma: no cover
         raise TypeError(f"invalid geometry type: {type(geometry)}")
 
-    def _reproject_geom(geometry, src_crs, dst_crs):
-        if geometry.is_empty:
-            return geometry
-        else:
-            transformed = transform_geom(
-                src_crs.to_dict(),
-                dst_crs.to_dict(),
-                mapping(geometry),
-                antimeridian_cutting=antimeridian_cutting,
-            )
-            # Fiona >1.9 returns None if transformation errored
-            if transformed is None:  # pragma: no cover
-                raise ReprojectionFailed(
-                    f"fiona.transform.transform_geom could not transform geometry from {src_crs} to {dst_crs}"
-                )
-            out_geom = to_shape(transformed)
-            return _repair(out_geom) if validity_check else out_geom
-
-    def _segmentize_value(geometry, segmentize_fraction):
-        height = geometry.bounds[3] - geometry.bounds[1]
-        width = geometry.bounds[2] - geometry.bounds[0]
-        return min([height, width]) / segmentize_fraction
-
     # return repaired geometry if no reprojection needed
     if src_crs == dst_crs or geometry.is_empty:
         return _repair(geometry)
     # geometry needs to be clipped to its CRS bounds
     elif (
         clip_to_crs_bounds
         and dst_crs.is_epsg_code
@@ -126,44 +139,63 @@
         # get dst_crs boundaries
         crs_bbox = box(
             *CRS_BOUNDS.get(
                 dst_crs.get("init"), pyproj.CRS(dst_crs.to_epsg()).area_of_use.bounds
             )
         )
         # reproject geometry to WGS84
-        geometry_4326 = _reproject_geom(geometry, src_crs, wgs84_crs)
+        geometry_4326 = _reproject_geom(
+            geometry,
+            src_crs,
+            wgs84_crs,
+            validity_check,
+            antimeridian_cutting,
+            fiona_env,
+        )
         # raise error if geometry has to be clipped
         if error_on_clip and not geometry_4326.within(crs_bbox):
             raise RuntimeError("geometry outside target CRS bounds")
 
         clipped = crs_bbox.intersection(geometry_4326)
 
         # segmentize clipped geometry using one 100th of with or height depending on
         # which is shorter
         if segmentize_on_clip or segmentize:
             clipped = segmentize_geometry(
                 clipped, _segmentize_value(clipped, segmentize_fraction)
             )
 
         # clip geometry dst_crs boundaries and return
-        return _reproject_geom(clipped, wgs84_crs, dst_crs)
+        return _reproject_geom(
+            clipped, wgs84_crs, dst_crs, validity_check, antimeridian_cutting, fiona_env
+        )
 
     # return without clipping if destination CRS does not have defined bounds
     else:
         try:
             if segmentize:
                 return _reproject_geom(
                     segmentize_geometry(
                         geometry, _segmentize_value(geometry, segmentize_fraction)
                     ),
                     src_crs,
                     dst_crs,
+                    validity_check,
+                    antimeridian_cutting,
+                    fiona_env,
                 )
             else:
-                return _reproject_geom(geometry, src_crs, dst_crs)
+                return _reproject_geom(
+                    geometry,
+                    src_crs,
+                    dst_crs,
+                    validity_check,
+                    antimeridian_cutting,
+                    fiona_env,
+                )
         except TopologicalError:  # pragma: no cover
             raise
         except ValueError as exc:  # pragma: no cover
             if retry_with_clip:
                 logger.error(
                     "error when transforming %s from %s to %s: %s, trying to use CRS bounds clip",
                     geometry,
@@ -250,15 +282,20 @@
     ----------
     geom : shapely geometry or GeoJSON mapping
 
     Returns
     -------
     shapely geometry
     """
-    return shape(geom) if not isinstance(geom, base.BaseGeometry) else geom
+    if isinstance(geom, base.BaseGeometry):
+        return geom
+    elif hasattr(geom, "__geo_interface__") and geom.__geo_interface__.get("geometry"):
+        return shape(geom.__geo_interface__["geometry"])
+    else:
+        return shape(geom)
 
 
 def multipart_to_singleparts(geom):
     """
     Yield single part geometries if geom is multipart, otherwise yield geom.
 
     Parameters
```

### Comparing `mapchete-2023.1.1/mapchete/io/_json.py` & `mapchete-2023.4.0/mapchete/io/_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import logging
 import os
 
 from mapchete.io._path import fs_from_path, path_exists
-from mapchete.io._misc import get_boto3_bucket
 
 
 logger = logging.getLogger(__name__)
 
 
 def write_json(path, params, fs=None, **kwargs):
     """Write local or remote."""
```

### Comparing `mapchete-2023.1.1/mapchete/io/_misc.py` & `mapchete-2023.4.0/mapchete/io/_misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,27 +186,17 @@
             zoom += 1
         logger.debug(
             "target zoom for %s: %s (%s)", tile_resolution, zoom, td_resolution
         )
         return zoom
 
 
-def get_boto3_bucket(bucket_name):
+def get_boto3_bucket(bucket_name):  # pragma: no cover
     """Return boto3.Bucket object from bucket name."""
-    import boto3
-
-    url = os.environ.get("AWS_S3_ENDPOINT")
-    return boto3.resource(
-        "s3",
-        endpoint_url=(
-            "https://" + url
-            if url and not url.startswith(("http://", "https://"))
-            else url
-        ),
-    ).Bucket(bucket_name)
+    raise DeprecationWarning("get_boto3_bucket() is deprecated")
 
 
 def get_gdal_options(opts, is_remote=False, allowed_remote_extensions=[]):
     """
     Return a merged set of custom and default GDAL/rasterio Env options.
 
     If is_remote is set to True, the default GDAL_HTTP_OPTS are appended.
```

### Comparing `mapchete-2023.1.1/mapchete/io/_path.py` & `mapchete-2023.4.0/mapchete/io/_path.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/io/raster.py` & `mapchete-2023.4.0/mapchete/io/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,15 +317,15 @@
         except FileNotFoundError:  # pragma: no cover
             if skip_missing_files:
                 logger.debug("skip missing file %s", input_file)
                 return _empty_array()
             else:
                 raise
         except Exception as exc:  # pragma: no cover
-            raise IOError(f"failed to read {input_file}") from exc
+            raise OSError(f"failed to read {input_file}") from exc
 
 
 def _get_warped_edge_array(
     tile=None,
     input_file=None,
     indexes=None,
     dst_shape=None,
@@ -475,77 +475,34 @@
                     return vrt.read(
                         window=vrt.window(*dst_bounds),
                         out_shape=dst_shape,
                         indexes=indexes,
                         masked=True,
                     )
 
-    if isinstance(input_file, str):
-        try:
-            with Timer() as t:
-                with rasterio.open(input_file, "r") as src:
-                    logger.debug("read from %s...", input_file)
-                    out = _read(
-                        src,
-                        indexes,
-                        dst_bounds,
-                        dst_shape,
-                        dst_crs,
-                        resampling,
-                        src_nodata,
-                        dst_nodata,
-                    )
-            logger.debug("read %s in %s", input_file, t)
-            return out
-        except RasterioIOError as e:
-            # rasterio errors which indicate file does not exist
-            for i in (
-                "does not exist in the file system",
-                "No such file or directory",
-                "The specified key does not exist",
-            ):
-                if i in str(e):
-                    raise FileNotFoundError(
-                        "%s not found and cannot be opened with rasterio" % input_file
-                    )
-            else:
-                try:
-                    # NOTE: this can cause addional S3 requests
-                    exists = path_exists(input_file)
-                except Exception:  # pragma: no cover
-                    # in order not to mask the original rasterio exception, raise it
-                    raise e
-                if exists:
-                    # raise rasterio exception
-                    raise e
-                else:  # pragma: no cover
-                    # file does not exist
-                    raise FileNotFoundError(
-                        "%s not found and cannot be opened with rasterio" % input_file
-                    )
-
-    else:  # pragma: no cover
-        logger.debug("assuming file object %s", input_file)
-        warnings.warn(
-            "passing on a rasterio dataset object is not recommended, see "
-            "https://github.com/mapbox/rasterio/issues/1309"
-        )
-        return _read(
-            input_file,
-            indexes,
-            dst_bounds,
-            dst_shape,
-            dst_crs,
-            resampling,
-            src_nodata,
-            dst_nodata,
-        )
+    try:
+        with Timer() as t:
+            with rasterio.open(input_file, "r") as src:
+                logger.debug("read from %s...", input_file)
+                out = _read(
+                    src,
+                    indexes,
+                    dst_bounds,
+                    dst_shape,
+                    dst_crs,
+                    resampling,
+                    src_nodata,
+                    dst_nodata,
+                )
+        logger.debug("read %s in %s", input_file, t)
+        return out
+    except RasterioIOError as rio_exc:
+        _extract_filenotfound_exception(rio_exc, input_file)
 
 
-@retry(logger=logger, exceptions=RasterioIOError, **MAPCHETE_IO_RETRY_SETTINGS)
 def read_raster_no_crs(input_file, indexes=None, gdal_opts=None):
     """
     Wrapper function around rasterio.open().read().
 
     Parameters
     ----------
     input_file : str
@@ -559,34 +516,70 @@
     -------
     MaskedArray
 
     Raises
     ------
     FileNotFoundError if file cannot be found.
     """
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore")
-        try:
-            with rasterio.Env(
-                **get_gdal_options(
-                    gdal_opts,
-                    is_remote=path_is_remote(input_file, s3=True),
-                    allowed_remote_extensions=os.path.splitext(input_file)[1],
-                ),
-            ) as env:
-                logger.debug("reading %s with GDAL options %s", input_file, env.options)
-                with rasterio.open(input_file, "r") as src:
-                    return src.read(indexes=indexes, masked=True)
-        except RasterioIOError as e:
+
+    @retry(logger=logger, exceptions=RasterioIOError, **MAPCHETE_IO_RETRY_SETTINGS)
+    def _read():
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
             try:
-                if path_exists(input_file):
-                    raise MapcheteIOError(e)
-            except Exception:
-                raise MapcheteIOError(e)
-            raise FileNotFoundError("%s not found" % input_file)
+                with rasterio.Env(
+                    **get_gdal_options(
+                        gdal_opts,
+                        is_remote=path_is_remote(input_file, s3=True),
+                        allowed_remote_extensions=os.path.splitext(input_file)[1],
+                    ),
+                ) as env:
+                    logger.debug(
+                        "reading %s with GDAL options %s", input_file, env.options
+                    )
+                    with rasterio.open(input_file, "r") as src:
+                        return src.read(indexes=indexes, masked=True)
+            except RasterioIOError as rio_exc:
+                _extract_filenotfound_exception(rio_exc, input_file)
+
+    try:
+        return _read()
+    except Exception as exc:
+        if isinstance(exc, FileNotFoundError):
+            raise
+        else:
+            raise MapcheteIOError(exc)
+
+
+def _extract_filenotfound_exception(rio_exc, path):
+    """
+    Extracts and raises FileNotFoundError from RasterioIOError if applicable.
+    """
+    filenotfound_msg = f"{path} not found and cannot be opened with rasterio"
+    # rasterio errors which indicate file does not exist
+    for i in (
+        "does not exist in the file system",
+        "No such file or directory",
+        "The specified key does not exist",
+    ):
+        if i in str(rio_exc):
+            raise FileNotFoundError(filenotfound_msg)
+    else:
+        try:
+            # NOTE: this can cause addional S3 requests
+            exists = path_exists(path)
+        except Exception:  # pragma: no cover
+            # in order not to mask the original rasterio exception, raise it as is
+            raise rio_exc
+        if exists:
+            # raise original rasterio exception
+            raise rio_exc
+        else:  # pragma: no cover
+            # file does not exist
+            raise FileNotFoundError(filenotfound_msg)
 
 
 class RasterWindowMemoryFile:
     """Context manager around rasterio.io.MemoryFile."""
 
     def __init__(
         self, in_tile=None, in_data=None, out_profile=None, out_tile=None, tags=None
@@ -713,14 +706,18 @@
         Keyword arguments to be passed on to rasterio.open()
 
     Returns
     -------
     RasterioRemoteWriter if target is remote, otherwise return rasterio.open().
     """
     if path.startswith("s3://"):
+        try:  # pragma: no cover
+            import boto3
+        except ImportError:  # pragma: no cover
+            raise ImportError("please install [s3] extra to write remote files")
         return RasterioRemoteWriter(path, fs=fs, in_memory=in_memory, *args, **kwargs)
     else:
         return rasterio.open(path, mode=mode, *args, **kwargs)
 
 
 class RasterioRemoteMemoryWriter:
     def __init__(self, path, *args, fs=None, **kwargs):
@@ -732,20 +729,21 @@
         self._open_kwargs = kwargs
         self._sink = None
 
     def __enter__(self):
         self._sink = self._dst.open(*self._open_args, **self._open_kwargs)
         return self._sink
 
-    def __exit__(self, *args):
+    def __exit__(self, exc_type, exc_value, exc_traceback):
         try:
             self._sink.close()
-            logger.debug("write rasterio MemoryFile to %s", self.path)
-            with self.fs.open(self.path, "wb") as dst:
-                dst.write(self._dst.getbuffer())
+            if exc_value is None:
+                logger.debug("upload rasterio MemoryFile to %s", self.path)
+                with self.fs.open(self.path, "wb") as dst:
+                    dst.write(self._dst.getbuffer())
         finally:
             logger.debug("close rasterio MemoryFile")
             self._dst.close()
 
 
 class RasterioRemoteTempFileWriter:
     def __init__(self, path, *args, fs=None, **kwargs):
@@ -759,18 +757,20 @@
 
     def __enter__(self):
         self._sink = rasterio.open(
             self._dst.name, "w+", *self._open_args, **self._open_kwargs
         )
         return self._sink
 
-    def __exit__(self, *args):
+    def __exit__(self, exc_type, exc_value, exc_traceback):
         try:
             self._sink.close()
-            self.fs.put_file(self._dst.name, self.path)
+            if exc_value is None:
+                logger.debug("upload TempFile %s to %s", self._dst.name, self.path)
+                self.fs.put_file(self._dst.name, self.path)
         finally:
             logger.debug("close and remove tempfile")
             self._dst.close()
 
 
 class RasterioRemoteWriter:
     def __new__(self, path, *args, fs=None, in_memory=True, **kwargs):
@@ -1249,15 +1249,15 @@
     skip_exists : bool
         Skip conversion if outpu already exists. (default: True)
     kwargs : mapping
         Creation parameters passed on to output file.
     """
     if path_exists(out):
         if not exists_ok:
-            raise IOError(f"{out} already exists")
+            raise OSError(f"{out} already exists")
         elif not overwrite:
             logger.debug("output %s already exists and will not be overwritten")
             return
     kwargs = kwargs or {}
     if kwargs:
         logger.debug("convert raster file %s to %s using %s", inp, out, kwargs)
         with rasterio.open(inp, "r") as src:
```

### Comparing `mapchete-2023.1.1/mapchete/io/vector.py` & `mapchete-2023.4.0/mapchete/io/vector.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,35 +2,34 @@
 
 from contextlib import ExitStack
 import os
 import logging
 import fiona
 from fiona.errors import DriverError, FionaError, FionaValueError
 from fiona.io import MemoryFile
-import json
 from retry import retry
 from rasterio.crs import CRS
-from shapely.geometry import box, mapping, shape
+from shapely.geometry import base, box, mapping
 from shapely.errors import TopologicalError
 from tilematrix import clip_geometry_to_srs_bounds
-from tilematrix._funcs import Bounds
 from itertools import chain
 import warnings
 
 from mapchete.errors import NoGeoError, MapcheteIOError
 from mapchete.io._misc import MAPCHETE_IO_RETRY_SETTINGS
 from mapchete.io._path import fs_from_path, path_exists, makedirs, copy
 from mapchete.io._geometry_operations import (
     reproject_geometry,
     segmentize_geometry,
     to_shape,
     multipart_to_singleparts,
     clean_geometry_type,
     _repair,
 )
+from mapchete.types import Bounds
 from mapchete.validate import validate_bounds
 
 __all__ = [
     "reproject_geometry",
     "segmentize_geometry",
     "to_shape",
     "multipart_to_singleparts",
@@ -121,16 +120,16 @@
 
 def write_vector_window(
     in_data=None,
     out_driver="GeoJSON",
     out_schema=None,
     out_tile=None,
     out_path=None,
-    bucket_resource=None,
     allow_multipart_geometries=True,
+    **kwargs,
 ):
     """
     Write features to file.
 
     When the output driver is 'Geobuf', the geobuf library will be used otherwise the
     driver will be passed on to Fiona.
 
@@ -333,35 +332,15 @@
                     }
             # this can be handled quietly
             except TopologicalError as e:  # pragma: no cover
                 logger.warning("feature omitted: %s", e)
 
 
 def bounds_intersect(bounds1, bounds2):
-    bounds1 = validate_bounds(bounds1)
-    bounds2 = validate_bounds(bounds2)
-    horizontal = (
-        # partial overlap
-        bounds1.left <= bounds2.left <= bounds1.right
-        or bounds1.left <= bounds2.right <= bounds1.right
-        # bounds 1 within bounds 2
-        or bounds2.left <= bounds1.left < bounds1.right <= bounds2.right
-        # bounds 2 within bounds 1
-        or bounds1.left <= bounds2.left < bounds2.right <= bounds1.right
-    )
-    vertical = (
-        # partial overlap
-        bounds1.bottom <= bounds2.bottom <= bounds1.top
-        or bounds1.bottom <= bounds2.top <= bounds1.top
-        # bounds 1 within bounds 2
-        or bounds2.bottom <= bounds1.bottom < bounds1.top <= bounds2.top
-        # bounds 2 within bounds 1
-        or bounds1.bottom <= bounds2.bottom < bounds2.top <= bounds1.top
-    )
-    return horizontal and vertical
+    return Bounds.from_inp(bounds1).intersects(bounds2)
 
 
 class FakeIndex:
     """Provides a fake spatial index in case rtree is not installed."""
 
     def __init__(self):
         self._items = []
@@ -488,33 +467,45 @@
         else:
             try:
                 return hash(feature)
             except TypeError:
                 raise TypeError("features need to have an id or have to be hashable")
 
 
+def object_geometry(obj) -> base.BaseGeometry:
+    """
+    Determine geometry from object if available.
+    """
+    try:
+        if hasattr(obj, "__geo_interface__"):
+            return to_shape(obj)
+        elif hasattr(obj, "geometry"):
+            return to_shape(obj.geometry)
+        elif hasattr(obj, "get") and obj.get("geometry"):
+            return to_shape(obj["geometry"])
+        else:
+            raise TypeError("no geometry")
+    except Exception as exc:
+        logger.exception(exc)
+        raise NoGeoError(f"cannot determine geometry from object: {obj}") from exc
+
+
 def object_bounds(obj) -> Bounds:
     """
     Determine geographic bounds from object if available.
     """
     try:
         if hasattr(obj, "bounds"):
             return validate_bounds(obj.bounds)
-        elif hasattr(obj, "__geo_interface__"):
-            return validate_bounds(shape(obj).bounds)
-        elif hasattr(obj, "geometry"):
-            return validate_bounds(to_shape(obj.geometry).bounds)
         elif hasattr(obj, "bbox"):
             return validate_bounds(obj.bbox)
-        elif obj.get("bounds"):
+        elif hasattr(obj, "get") and obj.get("bounds"):
             return validate_bounds(obj["bounds"])
-        elif obj.get("geometry"):
-            return validate_bounds(to_shape(obj["geometry"]).bounds)
         else:
-            raise TypeError("no bounds")
+            return validate_bounds(object_geometry(obj).bounds)
     except Exception as exc:
         logger.exception(exc)
         raise NoGeoError(f"cannot determine bounds from object: {obj}") from exc
 
 
 def convert_vector(inp, out, overwrite=False, exists_ok=True, **kwargs):
     """
```

### Comparing `mapchete-2023.1.1/mapchete/processes/__init__.py` & `mapchete-2023.4.0/mapchete/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/processes/contours.py` & `mapchete-2023.4.0/mapchete/processes/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/processes/convert.py` & `mapchete-2023.4.0/mapchete/processes/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/processes/hillshade.py` & `mapchete-2023.4.0/mapchete/processes/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/processes/examples/example_process.py` & `mapchete-2023.4.0/mapchete/processes/examples/example_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/static/index.html` & `mapchete-2023.4.0/mapchete/static/index.html`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/mapchete/static/process_template.py` & `mapchete-2023.4.0/mapchete/static/process_template.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/LICENSE` & `mapchete-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/README.rst` & `mapchete-2023.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `mapchete-2023.1.1/pyproject.toml` & `mapchete-2023.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -40,28 +40,26 @@
     "tilematrix>=2022.12.0",
     "tqdm",
 ]
 
 [project.optional-dependencies]
 complete = [
     "aiohttp",
-    "boto3",
     "dask",
     "distributed",
     "flask",
     "fsspec[http]",
     "fsspec[s3]",
     "geobuf",
     "lxml",
     "matplotlib",
     "protobuf<=3.20.1",
     "pystac",
     "requests",
     "rtree",
-    "s3fs>=0.5.1",
     "werkzeug>=0.15",
 ]
 contours = [
     "matplotlib",
 ]
 dask = [
     "dask",
@@ -73,23 +71,23 @@
 ]
 http = [
     "aiohttp",
     "fsspec[http]",
     "requests",
 ]
 s3 = [
-    "boto3",
     "fsspec[s3]",
-    "s3fs>=0.5.1",
+    "boto3>=1.14.44",
+    "aiobotocore>=1.1.2",
 ]
 serve = [
     "flask",
     "werkzeug>=0.15",
 ]
-spatial_index = [
+spatial-index = [
     "rtree",
 ]
 stac = [
     "pystac",
 ]
 vrt = [
     "lxml",
```

### Comparing `mapchete-2023.1.1/PKG-INFO` & `mapchete-2023.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapchete
-Version: 2023.1.1
+Version: 2023.4.0
 Summary: Tile-based geodata processing using rasterio & Fiona
 Project-URL: Homepage, https://github.com/ungarj/mapchete
 Author-email: Joachim Ungar <joachim.ungar@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -29,45 +29,43 @@
 Requires-Dist: rasterio>1.2.10
 Requires-Dist: retry
 Requires-Dist: shapely
 Requires-Dist: tilematrix>=2022.12.0
 Requires-Dist: tqdm
 Provides-Extra: complete
 Requires-Dist: aiohttp; extra == 'complete'
-Requires-Dist: boto3; extra == 'complete'
 Requires-Dist: dask; extra == 'complete'
 Requires-Dist: distributed; extra == 'complete'
 Requires-Dist: flask; extra == 'complete'
 Requires-Dist: fsspec[http]; extra == 'complete'
 Requires-Dist: fsspec[s3]; extra == 'complete'
 Requires-Dist: geobuf; extra == 'complete'
 Requires-Dist: lxml; extra == 'complete'
 Requires-Dist: matplotlib; extra == 'complete'
 Requires-Dist: protobuf<=3.20.1; extra == 'complete'
 Requires-Dist: pystac; extra == 'complete'
 Requires-Dist: requests; extra == 'complete'
 Requires-Dist: rtree; extra == 'complete'
-Requires-Dist: s3fs>=0.5.1; extra == 'complete'
 Requires-Dist: werkzeug>=0.15; extra == 'complete'
 Provides-Extra: contours
 Requires-Dist: matplotlib; extra == 'contours'
 Provides-Extra: dask
 Requires-Dist: dask; extra == 'dask'
 Requires-Dist: distributed; extra == 'dask'
 Provides-Extra: geobuf
 Requires-Dist: geobuf; extra == 'geobuf'
 Requires-Dist: protobuf<=3.20.1; extra == 'geobuf'
 Provides-Extra: http
 Requires-Dist: aiohttp; extra == 'http'
 Requires-Dist: fsspec[http]; extra == 'http'
 Requires-Dist: requests; extra == 'http'
 Provides-Extra: s3
-Requires-Dist: boto3; extra == 's3'
+Requires-Dist: aiobotocore>=1.1.2; extra == 's3'
+Requires-Dist: boto3>=1.14.44; extra == 's3'
 Requires-Dist: fsspec[s3]; extra == 's3'
-Requires-Dist: s3fs>=0.5.1; extra == 's3'
 Provides-Extra: serve
 Requires-Dist: flask; extra == 'serve'
 Requires-Dist: werkzeug>=0.15; extra == 'serve'
 Provides-Extra: spatial-index
 Requires-Dist: rtree; extra == 'spatial-index'
 Provides-Extra: stac
 Requires-Dist: pystac; extra == 'stac'
```

