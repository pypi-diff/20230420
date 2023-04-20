# Comparing `tmp/siibra-0.4a33.tar.gz` & `tmp/siibra-0.4a35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siibra-0.4a33.tar", last modified: Thu Feb  9 11:30:00 2023, max compression
+gzip compressed data, was "siibra-0.4a35.tar", last modified: Fri Feb 24 14:12:11 2023, max compression
```

## Comparing `siibra-0.4a33.tar` & `siibra-0.4a35.tar`

### file list

```diff
@@ -1,99 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.076230 siibra-0.4a33/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-09 11:28:37.000000 siibra-0.4a33/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-09 11:28:37.000000 siibra-0.4a33/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-02-09 11:30:00.076230 siibra-0.4a33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-02-09 11:28:37.000000 siibra-0.4a33/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 11:30:00.076230 siibra-0.4a33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-02-09 11:28:37.000000 siibra-0.4a33/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.068230 siibra-0.4a33/siibra/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.068230 siibra-0.4a33/siibra/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/configuration/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.068230 siibra-0.4a33/siibra/core/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/core/atlas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/core/concept.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/core/parcellation.py
--rw-r--r--   0 runner    (1001) docker     (123)    26181 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/core/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.068230 siibra-0.4a33/siibra/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/anchor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.068230 siibra-0.4a33/siibra/features/basetypes/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/basetypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/basetypes/cortical_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/basetypes/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/basetypes/regional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/basetypes/tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/basetypes/volume_of_interest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.068230 siibra-0.4a33/siibra/features/cellular/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/cellular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/cellular/bigbrain_intensity_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/cellular/cell_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/cellular/layerwise_bigbrain_intensities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/cellular/layerwise_cell_density.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.072230 siibra-0.4a33/siibra/features/connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/connectivity/functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/connectivity/streamline_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/connectivity/streamline_lengths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.072230 siibra-0.4a33/siibra/features/external/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/external/ebrains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.072230 siibra-0.4a33/siibra/features/fibres/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/fibres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.072230 siibra-0.4a33/siibra/features/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.072230 siibra-0.4a33/siibra/features/molecular/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/molecular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/molecular/gene_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/molecular/receptor_density_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/features/molecular/receptor_density_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.072230 siibra-0.4a33/siibra/livequeries/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/livequeries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/livequeries/allen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/livequeries/bigbrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/livequeries/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/livequeries/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.072230 siibra-0.4a33/siibra/locations/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/locations/boundingbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/locations/location.py
--rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/locations/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/locations/pointset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.072230 siibra-0.4a33/siibra/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/retrieval/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/retrieval/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.072230 siibra-0.4a33/siibra/retrieval/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/retrieval/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26023 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/retrieval/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/retrieval/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.072230 siibra-0.4a33/siibra/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/samplers/bigbrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.076230 siibra-0.4a33/siibra/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/vocabularies/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)  1647972 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/vocabularies/gene_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/vocabularies/receptor_symbols.json
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/vocabularies/region_aliases.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.076230 siibra-0.4a33/siibra/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/volumes/gifti.py
--rw-r--r--   0 runner    (1001) docker     (123)    23462 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/volumes/neuroglancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/volumes/nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)    38349 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/volumes/parcellationmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    17605 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/volumes/sparsemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-02-09 11:28:37.000000 siibra-0.4a33/siibra/volumes/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.068230 siibra-0.4a33/siibra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-02-09 11:30:00.000000 siibra-0.4a33/siibra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-02-09 11:30:00.000000 siibra-0.4a33/siibra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 11:30:00.000000 siibra-0.4a33/siibra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-09 11:30:00.000000 siibra-0.4a33/siibra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-09 11:30:00.000000 siibra-0.4a33/siibra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:30:00.076230 siibra-0.4a33/test/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-09 11:28:37.000000 siibra-0.4a33/test/test_siibra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.383820 siibra-0.4a35/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-24 14:11:06.000000 siibra-0.4a35/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-24 14:11:06.000000 siibra-0.4a35/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-02-24 14:12:11.383820 siibra-0.4a35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-02-24 14:11:06.000000 siibra-0.4a35/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 14:12:11.383820 siibra-0.4a35/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-02-24 14:11:06.000000 siibra-0.4a35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.371819 siibra-0.4a35/siibra/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23759 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.375820 siibra-0.4a35/siibra/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/configuration/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.375820 siibra-0.4a35/siibra/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/core/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/core/concept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/core/parcellation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26364 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/core/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.375820 siibra-0.4a35/siibra/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/anchor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.375820 siibra-0.4a35/siibra/features/connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/connectivity/functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12361 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/connectivity/regional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/connectivity/streamline_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/connectivity/streamline_lengths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.375820 siibra-0.4a35/siibra/features/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/dataset/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.375820 siibra-0.4a35/siibra/features/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/image/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/image/volume_of_interest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.379819 siibra-0.4a35/siibra/features/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/tabular/bigbrain_intensity_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/tabular/cell_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/tabular/cortical_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/tabular/gene_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/tabular/layerwise_bigbrain_intensities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/tabular/layerwise_cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/tabular/receptor_density_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/tabular/receptor_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/features/tabular/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.379819 siibra-0.4a35/siibra/livequeries/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/livequeries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/livequeries/allen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/livequeries/bigbrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/livequeries/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/livequeries/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.379819 siibra-0.4a35/siibra/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/locations/boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/locations/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/locations/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/locations/pointset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.379819 siibra-0.4a35/siibra/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/retrieval/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/retrieval/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.379819 siibra-0.4a35/siibra/retrieval/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/retrieval/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26024 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/retrieval/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/retrieval/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.383820 siibra-0.4a35/siibra/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/vocabularies/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1647972 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/vocabularies/gene_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/vocabularies/receptor_symbols.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/vocabularies/region_aliases.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.383820 siibra-0.4a35/siibra/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/volumes/gifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/volumes/neuroglancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/volumes/nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39738 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/volumes/parcellationmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18138 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/volumes/sparsemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-02-24 14:11:06.000000 siibra-0.4a35/siibra/volumes/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.375820 siibra-0.4a35/siibra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-02-24 14:12:11.000000 siibra-0.4a35/siibra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-02-24 14:12:11.000000 siibra-0.4a35/siibra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 14:12:11.000000 siibra-0.4a35/siibra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-24 14:12:11.000000 siibra-0.4a35/siibra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-24 14:12:11.000000 siibra-0.4a35/siibra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:12:11.383820 siibra-0.4a35/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-24 14:11:06.000000 siibra-0.4a35/test/test_siibra.py
```

### Comparing `siibra-0.4a33/LICENSE` & `siibra-0.4a35/LICENSE`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/PKG-INFO` & `siibra-0.4a35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 0.4a33
+Version: 0.4a35
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -27,24 +27,24 @@
 Medicine (INM-1), Forschungszentrum Jülich GmbH*
 
 .. intro-start
 
 ``siibra`` is a Python client to a brain atlas framework that integrates brain parcellations and reference spaces at different spatial scales, and connects them with a broad range of multimodal regional data features. 
 It aims to facilitate programmatic and reproducible incorporation of brain parcellations and brain region features from different sources into neuroscience workflows.
 
-    **Note:** *``siibra-python`` is still in development. While care is taken that it works reliably, its API is not yet stable and you may still encounter bugs when using it.*
+    **Note:** ``siibra-python`` *is still in development. While care is taken that it works reliably, its API is not yet stable and you may still encounter bugs when using it.*
 
 ``siibra`` provides structured access to parcellation schemes in different brain reference spaces, including volumetric reference templates at  macroscopic and microscopic resolutions as well as surface representations. 
 It supports both discretely labelled and statistical (probabilistic) parcellation maps, which can be used to assign brain regions to spatial locations and image signals, to retrieve region-specific neuroscience datasets from multiple online repositories, and to sample information from high-resolution image data. 
 The datasets anchored to brain regions address features of molecular, cellular and architecture as well as connectivity, and are complemented with live queries to external repositories as well as dynamic extraction from "big" image volumes such as the 20 micrometer BigBrain model.
 
 ``siibra`` was developed in the frame of the `Human Brain Project <https://humanbrainproject.eu>`__ for accessing the `EBRAINS
 human brain atlas <https://ebrains.eu/service/human-brain-atlas>`__. 
 It stores most of its contents as sustainable and open datasets in the `EBRAINS Knowledge Graph <https://kg.ebrains.eu>`__, and is designed to support the `OpenMINDS metadata standards <https://github.com/HumanBrainProject/openMINDS_SANDS>`__. 
-Its functionalities include common actions known from the interactive viewer ``siibra explorer`` `hosted at EBRAINS <https://atlases.ebrains.eu/viewer>`__. 
+Its functionalities include common actions known from the interactive viewer ``siibra-explorer`` `hosted at EBRAINS <https://atlases.ebrains.eu/viewer>`__. 
 In fact, the viewer is a good resource for exploring ``siibra``\ ’s core functionalities interactively: Selecting different parcellations, browsing and searching brain region hierarchies, downloading maps, identifying brain regions, and accessing multimodal features and connectivity information associated with brain regions. 
 Feature queries in ``siibra`` are parameterized by data modality and anatomical location, while the latter could be a brain region, brain parcellation, or location in reference space. 
 Beyond the explorative focus of ``siibra-explorer``, the Python library supports a range of data analysis functions suitable for typical neuroscience workflows.
 
 ``siibra`` hides much of the complexity that would be required to collect and interact with the individual parcellations, templates and data repositories.
 By encapsulating many aspects of interacting with different maps and reference templates spaces, it also minimizes common errors like misinterpretation of coordinates from different reference spaces, confusing label indices of brain regions, or using inconsistent versions of parcellation maps. 
 It aims to provide a safe way of using maps defined across multiple spatial scales for reproducible analysis.
```

### Comparing `siibra-0.4a33/README.rst` & `siibra-0.4a35/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 Medicine (INM-1), Forschungszentrum Jülich GmbH*
 
 .. intro-start
 
 ``siibra`` is a Python client to a brain atlas framework that integrates brain parcellations and reference spaces at different spatial scales, and connects them with a broad range of multimodal regional data features. 
 It aims to facilitate programmatic and reproducible incorporation of brain parcellations and brain region features from different sources into neuroscience workflows.
 
-    **Note:** *``siibra-python`` is still in development. While care is taken that it works reliably, its API is not yet stable and you may still encounter bugs when using it.*
+    **Note:** ``siibra-python`` *is still in development. While care is taken that it works reliably, its API is not yet stable and you may still encounter bugs when using it.*
 
 ``siibra`` provides structured access to parcellation schemes in different brain reference spaces, including volumetric reference templates at  macroscopic and microscopic resolutions as well as surface representations. 
 It supports both discretely labelled and statistical (probabilistic) parcellation maps, which can be used to assign brain regions to spatial locations and image signals, to retrieve region-specific neuroscience datasets from multiple online repositories, and to sample information from high-resolution image data. 
 The datasets anchored to brain regions address features of molecular, cellular and architecture as well as connectivity, and are complemented with live queries to external repositories as well as dynamic extraction from "big" image volumes such as the 20 micrometer BigBrain model.
 
 ``siibra`` was developed in the frame of the `Human Brain Project <https://humanbrainproject.eu>`__ for accessing the `EBRAINS
 human brain atlas <https://ebrains.eu/service/human-brain-atlas>`__. 
 It stores most of its contents as sustainable and open datasets in the `EBRAINS Knowledge Graph <https://kg.ebrains.eu>`__, and is designed to support the `OpenMINDS metadata standards <https://github.com/HumanBrainProject/openMINDS_SANDS>`__. 
-Its functionalities include common actions known from the interactive viewer ``siibra explorer`` `hosted at EBRAINS <https://atlases.ebrains.eu/viewer>`__. 
+Its functionalities include common actions known from the interactive viewer ``siibra-explorer`` `hosted at EBRAINS <https://atlases.ebrains.eu/viewer>`__. 
 In fact, the viewer is a good resource for exploring ``siibra``\ ’s core functionalities interactively: Selecting different parcellations, browsing and searching brain region hierarchies, downloading maps, identifying brain regions, and accessing multimodal features and connectivity information associated with brain regions. 
 Feature queries in ``siibra`` are parameterized by data modality and anatomical location, while the latter could be a brain region, brain parcellation, or location in reference space. 
 Beyond the explorative focus of ``siibra-explorer``, the Python library supports a range of data analysis functions suitable for typical neuroscience workflows.
 
 ``siibra`` hides much of the complexity that would be required to collect and interact with the individual parcellations, templates and data repositories.
 By encapsulating many aspects of interacting with different maps and reference templates spaces, it also minimizes common errors like misinterpretation of coordinates from different reference spaces, confusing label indices of brain regions, or using inconsistent versions of parcellation maps. 
 It aims to provide a safe way of using maps defined across multiple spatial scales for reproducible analysis.
```

### Comparing `siibra-0.4a33/setup.py` & `siibra-0.4a35/setup.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/siibra/__init__.py` & `siibra-0.4a35/siibra/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,8 +126,9 @@
         "PointSet",
         "QUIET",
         "VERBOSE",
         "fetch_ebrains_token",
         "set_ebrains_token",
         "vocabularies",
         "__version__",
+        "cache",
     ]
```

### Comparing `siibra-0.4a33/siibra/commons.py` & `siibra-0.4a35/siibra/commons.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,14 +346,29 @@
     unit_lengths = []
     for vec in np.identity(3):
         vec_phys = np.dot(affine, np.r_[vec, 1])
         unit_lengths.append(np.linalg.norm(orig - vec_phys))
     return np.prod(unit_lengths)
 
 
+def iterate_connected_components(img: Nifti1Image):
+    """
+    Provide an iterator over masks of connected components in the given image.
+    """
+    from skimage import measure
+    imgdata = np.asanyarray(img.dataobj).squeeze()
+    components = measure.label(imgdata > 0)
+    component_labels = np.unique(components)
+    assert component_labels[0] == 0
+    return (
+        (label, Nifti1Image((components == label).astype('uint8'), img.affine))
+        for label in component_labels[1:]
+    )
+
+
 def compare_maps(map1: Nifti1Image, map2: Nifti1Image):
     """
     Compare two maps, given as Nifti1Image objects.
     This function exploits that nibabel's get_fdata() caches the numerical arrays,
     so we can use the object id to cache extraction of the nonzero coordinates.
     Repeated calls involving the same map will therefore be much faster as they
     will only access the image array if overlapping pixels are detected.
@@ -392,15 +407,22 @@
     X2, Y2, Z2 = colsplit(XYZnz2[valid, :])
 
     # intersection
     v1, v2 = a1[X1, Y1, Z1].squeeze(), a2[X2, Y2, Z2].squeeze()
     m1, m2 = ((_ > 0).astype("uint8") for _ in [v1, v2])
     intersection = np.minimum(m1, m2).sum()
     if intersection == 0:
-        return {"IoU": 0, "contained": 0, "contains": 0, "correlation": 0}
+        return {
+            "intersection over union": 0,
+            "intersection over first": 0,
+            "intersection over second": 0,
+            "correlation": 0,
+            "weighted mean of first": 0,
+            "weighted mean of second": 0,
+        }
 
     # Compute the nonzero voxels in map1 with their correspondences in map2
     XYZnz1 = nonzero_coordinates(a1)
     N1 = XYZnz1.shape[0]
     warp1on2 = np.dot(np.linalg.inv(map2.affine), map1.affine)
 
     # Voxels referring to the union of the nonzero pixels in both maps
@@ -428,18 +450,20 @@
     else:
         r = np.sum(np.multiply(x0, y0)) / dem
 
     bx = (x > 0).astype("uint8")
     by = (y > 0).astype("uint8")
 
     return {
-        "IoU": intersection / np.maximum(bx, by).sum(),
-        "contained": intersection / N1,
-        "contains": intersection / N2,
+        "intersection over union": intersection / np.maximum(bx, by).sum(),
+        "intersection over first": intersection / N1,
+        "intersection over second": intersection / N2,
         "correlation": r,
+        "weighted mean of first": np.sum(x * y) / np.sum(y),
+        "weighted mean of second": np.sum(x * y) / np.sum(x),
     }
 
 
 class PolyLine:
     """Simple polyline representation which allows equidistant sampling.."""
 
     def __init__(self, pts):
```

### Comparing `siibra-0.4a33/siibra/configuration/__init__.py` & `siibra-0.4a35/siibra/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/siibra/configuration/configuration.py` & `siibra-0.4a35/siibra/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/siibra/configuration/factory.py` & `siibra-0.4a35/siibra/configuration/factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,23 +10,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ..commons import logger, Species
-from ..features import anchor
-from ..features.molecular import receptor_density_fingerprint, receptor_density_profile
-from ..features.cellular import cell_density_profile, layerwise_cell_density
-from ..features.basetypes import volume_of_interest
+from ..features import anchor, connectivity
+from ..features.tabular import (
+    receptor_density_profile,
+    receptor_density_fingerprint,
+    cell_density_profile,
+    layerwise_cell_density
+)
+from ..features.image import sections, volume_of_interest
 from ..core import atlas, parcellation, space, region
 from ..locations import point, pointset
 from ..retrieval import datasets, repositories
 from ..volumes import gifti, volume, nifti, neuroglancer, sparsemap, parcellationmap
-from ..features import connectivity
 
 from os import path
 import json
 import numpy as np
 from typing import List, Type
 import pandas as pd
 from io import BytesIO
@@ -45,14 +48,15 @@
     "tmp/poly": "build_pointset",
     "siibra/location/pointset/v0.1": "build_pointset",
     "siibra/feature/profile/receptor/v0.1": "build_receptor_density_profile",
     "siibra/feature/profile/celldensity/v0.1": "build_cell_density_profile",
     "siibra/feature/fingerprint/receptor/v0.1": "build_receptor_density_fingerprint",
     "siibra/feature/fingerprint/celldensity/v0.1": "build_cell_density_fingerprint",
     "siibra/feature/connectivitymatrix/v0.2": "build_connectivity_matrix",
+    "siibra/feature/section/v0.1": "build_section",
     "siibra/feature/voi/v0.1": "build_volume_of_interest",
 }
 
 
 class Factory:
 
     _warnings_issued = []
@@ -60,14 +64,17 @@
     @classmethod
     def extract_datasets(cls, spec):
         result = []
         if "minds/core/dataset/v1.0.0" in spec.get("ebrains", {}):
             result.append(
                 datasets.EbrainsDataset(id=spec["ebrains"]["minds/core/dataset/v1.0.0"])
             )
+        if "openminds/Dataset" in spec.get("ebrains", {}):
+            # TODO add parser for ebrains kg v3 dataset. see EbrainsV3Dataset 
+            pass
         return result
 
     @classmethod
     def extract_volumes(cls, spec, space_id: str = None, name: str = None):
         volume_specs = spec.get("volumes", [])
         for vspec in volume_specs:
             if space_id:
@@ -241,14 +248,15 @@
 
         assert all([isinstance(provider, volume.VolumeProvider) for provider in providers])
         result = volume.Volume(
             space_spec=spec.get("space", {}),
             providers=providers,
             name=spec.get("name", {}),
             variant=spec.get("variant"),
+            datasets=cls.extract_datasets(spec),
         )
 
         return result
 
     @classmethod
     def build_map(cls, spec):
         # maps have no configured identifier - we require the spec filename to build one
@@ -361,24 +369,66 @@
             patch=spec['patch'],
             url=spec['file'],
             anchor=cls.extract_anchor(spec),
             datasets=cls.extract_datasets(spec),
         )
 
     @classmethod
+    def build_section(cls, spec):
+        vol = cls.build_volume(spec)
+        kwargs = {
+            "name": spec.get('name', ""),
+            "region": spec.get('region', None),
+            "space_spec": vol._space_spec,
+            "providers": vol._providers.values(),
+            "datasets": cls.extract_datasets(spec),
+        }
+        modality = spec.get('modality', "")
+        if modality == "cell body staining":
+            return sections.CellbodyStainedSection(**kwargs)
+        else:
+            raise ValueError(f"No method for building image section feature type {modality}.")
+
+    @classmethod
     def build_volume_of_interest(cls, spec):
         vol = cls.build_volume(spec)
-        return volume_of_interest.VolumeOfInterest(
-            name=vol.name,
-            modality=spec.get('modality', ""),
-            region=spec.get('region', None),
-            space_spec=vol._space_spec,
-            providers=vol._providers.values(),
-            datasets=cls.extract_datasets(spec),
-        )
+        kwargs = {
+            "name": spec.get('name', ""),
+            "region": spec.get('region', None),
+            "space_spec": vol._space_spec,
+            "providers": vol._providers.values(),
+            "datasets": cls.extract_datasets(spec),
+        }
+        modality = spec.get('modality', "")
+        if modality == "cell body staining":
+            return volume_of_interest.CellBodyStainedVolumeOfInterest(**kwargs)
+        elif modality == "blockface":
+            return volume_of_interest.BlockfaceVolumeOfInterest(**kwargs)
+        elif modality == "PLI HSV fibre orientation map":
+            return volume_of_interest.PLIVolumeOfInterest(
+                modality="HSV fibre orientation map", **kwargs
+            )
+        elif modality == "transmittance":
+            return volume_of_interest.PLIVolumeOfInterest(
+                modality="transmittance", **kwargs
+            )
+        elif modality == "segmentation":
+            return volume_of_interest.SegmentedVolumeOfInterest(**kwargs)
+        elif modality == "T2 weighted MRI":
+            return volume_of_interest.MRIVolumeOfInterest(
+                modality="T2", **kwargs
+            )
+        elif modality == "T1 weighted MRI":
+            return volume_of_interest.MRIVolumeOfInterest(
+                modality="T1", **kwargs
+            )
+        elif modality == "segmentation":
+            return volume_of_interest.SegmentedVolumeOfInterest(**kwargs)
+        else:
+            raise ValueError(f"No method for building image section feature type {modality}.")
 
     @classmethod
     def build_connectivity_matrix(cls, spec):
         modality = spec["modality"]
         kwargs = {
             "cohort": spec["cohort"],
             "modality": modality,
@@ -394,18 +444,18 @@
             return connectivity.StreamlineCounts(**kwargs)
         elif modality == "StreamlineLengths":
             return connectivity.StreamlineLengths(**kwargs)
         elif modality == "Functional":
             kwargs["paradigm"] = spec.get("paradigm")
             return connectivity.FunctionalConnectivity(**kwargs)
         elif modality == "RestingState":
-            kwargs["paradigm"] = "RestingState"
+            kwargs["paradigm"] = spec.get("paradigm", "RestingState")
             return connectivity.FunctionalConnectivity(**kwargs)
         else:
-            raise ValueError(f"Do not know how to build connectivity matrix of type {modality}.")
+            raise ValueError(f"No method for building connectivity matrix of type {modality}.")
 
     @classmethod
     def from_json(cls, spec: dict):
 
         if isinstance(spec, str):
             if path.isfile(spec):
                 fname = spec
```

### Comparing `siibra-0.4a33/siibra/core/__init__.py` & `siibra-0.4a35/siibra/core/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/siibra/core/atlas.py` & `siibra-0.4a35/siibra/core/atlas.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/siibra/core/concept.py` & `siibra-0.4a35/siibra/core/concept.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,20 +131,26 @@
     @classmethod
     def clear_registry(cls):
         cls._registry_cached = None
 
     @classmethod
     def get_instance(cls, spec: str):
         """
-        Returns an instance of this class matching the given specification
-        from its registry, if possible, otherwise None.
-
-        Raises
+        Parameters
+        ----------
+            spec: str
+                Specification of the class the instance is requested.
+        Returns
         -------
-        IndexError: if spec cannot match any instance
+            an instance of this class matching the given specification from its
+            registry if possible, otherwise None.
+        Raises
+        ------
+            IndexError
+                If spec cannot match any instance
         """
         if cls.registry() is not None:
             return cls.registry().get(spec)
 
     @property
     def id(self):
         # allows derived classes to assign the id dynamically
@@ -164,15 +170,22 @@
         return super().__init_subclass__()
 
     def __str__(self):
         return f"{self.__class__.__name__}: {self.name}"
 
     def matches(self, spec):
         """
-        Test if the given specification matches the name, key or id of the concept.
+        Parameters
+        ----------
+            spec: str
+                Specification checked within the concept name, key or id
+        Returns
+        -------
+            bool
+                Whether the given specification matches the name, key or id of the concept.
         """
         if isinstance(spec, self.__class__) and (spec == self):
             return True
         elif isinstance(spec, str):
             if spec == self.key:
                 return True
             elif spec == self.id:
```

### Comparing `siibra-0.4a33/siibra/core/parcellation.py` & `siibra-0.4a35/siibra/core/parcellation.py`

 * *Files 7% similar despite different names*

```diff
@@ -92,23 +92,24 @@
             Unique identifier of the parcellation
         name : str
             Human-readable name of the parcellation
         species: str or Species
             Specification of the species
         regions: list or Region
         shortname: str
-            Shortform of human-readable name (optional)
+            Short form of human-readable name (optional)
         description: str
             Textual description of the parcellation
         version : str or None
             Version specification, optional
         modality  :  str or None
             Specification of the modality used for creating the parcellation
         publications: list
-            List of ssociated publications, each a dictionary with "doi" and/or "citation" fields
+            List of associated publications, each a dictionary with "doi"
+            and/or "citation" fields
         datasets : list
             datasets associated with this region
         """
         region.Region.__init__(
             self,
             name=name,
             children=regions,
@@ -134,31 +135,35 @@
                 for w in re.split(r'\s+', spec.lower())
             ):
                 return True
         return super().matches(spec)
 
     def get_map(self, space=None, maptype: Union[str, MapType] = MapType.LABELLED):
         """
-        Get the maps for the parcellation in the requested
-        template space. This might in general include multiple
-        3D volumes. For example, the Julich-Brain atlas provides two separate
-        maps, one per hemisphere. Per default, multiple maps are concatenated into a 4D
-        array, but you can choose to retrieve a dict of 3D volumes instead using `return_dict=True`.
+        Get the maps for the parcellation in the requested template space.
+
+        This might in general include multiple 3D volumes. For example,
+        the Julich-Brain atlas provides two separate maps, one per hemisphere.
+        Per default, multiple maps are concatenated into a 4D array, but you
+        can choose to retrieve a dict of 3D volumes instead using
+        `return_dict=True`.
 
         Parameters
         ----------
-        space : Space or str
+        space: Space or str
             template space specification
-        maptype : MapType (default: MapType.LABELLED)
-            Type of map requested (e.g., continous or labelled, see _commons.MapType)
+        maptype: MapType
+            Type of map requested (e.g., statistical or labelled).
             Use MapType.STATISTICAL to request probability maps.
-
-        Yields
-        ------
-        A ParcellationMap representing the volumetric map.
+            Defaults to MapType.LABELLED.
+        Returns
+        -------
+        parcellationmap.Map or SparseMap
+            A ParcellationMap representing the volumetric map or
+            a SparseMap representing the list of statistical maps.
         """
         if not isinstance(maptype, MapType):
             maptype = MapType[maptype.upper()]
 
         candidates = [
             m for m in parcellationmap.Map.registry()
             if m.space.matches(space)
@@ -171,14 +176,30 @@
             return None
         if len(candidates) > 1:
             logger.warning(f"Multiple {maptype} maps in {space} available for {str(self)}, choosing the first.")
         return candidates[0]
 
     @classmethod
     def find_regions(cls, region_spec: str, parents_only=True):
+        """
+        Find regions that match the given region specification in the subtree
+        headed by this region.
+
+        Parameters
+        ----------
+        regionspec: str
+            a string with a possibly inexact name, which is matched both
+            against the name and the identifier key,
+        parents_only: bool
+            If true, children of matched parents will not be returned
+        Returns
+        -------
+        List[Region]
+            list of matching regions
+        """
         MEM = cls._CACHED_REGION_SEARCHES
         if region_spec not in MEM:
             MEM[region_spec] = [
                 r
                 for p in cls.registry()
                 for r in p.find(regionspec=region_spec)
             ]
@@ -212,48 +233,58 @@
             for s in re.split(r', *', spec)
         })
         if len(candidates) > 0:
             return candidates
         else:
             return [spec]
 
-    def get_region(self, regionspec: Union[str, int, MapIndex, region.Region], find_topmost=True, allow_tuple=False):
+    def get_region(
+        self,
+        regionspec: Union[str, int, MapIndex, region.Region],
+        find_topmost: bool = True,
+        allow_tuple: bool = False
+    ):
         """
         Given a unique specification, return the corresponding region.
+
         The spec could be a label index, a (possibly incomplete) name, or a
-        region object.
-        This method is meant to definitely determine a valid region. Therefore,
-        if no match is found, it raises a ValueError.
-        If multiple matches are found, the method tries to return only the common parent node.
-        If there is no common parent, an exception is raised, except when
-        allow_tuple=True - then a tuple of matched regions is returned
+        region object. This method is meant to definitely determine a valid
+        region. Therefore, if no match is found, it raises a ValueError.
+        If multiple matches are found, the method tries to return only the
+        common parent node. If there is no common parent, an exception is
+        raised, except when allow_tuple=True - then a tuple of matched regions
+        is returned.
 
         Parameters
         ----------
-        regionspec : any of
-            - a string with a possibly inexact name, which is matched both
-              against the name and the identifier key,
-            - an integer, which is interpreted as a labelindex,
-            - a region object
-            - a full MapIndex
-        find_topmost : Bool, default: True
+        regionspec: str, regex, int, Region, MapIndex
+            - a string with a possibly inexact name (matched both against the name and the identifier key)
+            - a string in '/pattern/flags' format to use regex search (acceptable flags: aiLmsux)
+            - a regex applied to region names
+            - an integer (interpreted as a labelindex)
+            - a Region object
+            - a full MapIndex object
+        find_topmost: bool, default: True
             If True, will automatically return the parent of a decoded region
             the decoded region is its only child.
-        allow_tuple: Bool, default: False
+        allow_tuple: bool, default: False
             If multiple candidates without a common parent are found,
             return a tuple of matches instead of raising an exception.
-
-        Return
-        ------
-        Region object
+            
+        Returns
+        -------
+        Region
+            A region object defined in the parcellation
 
         Raises
         ------
-        RuntimeError: if the spec matches multiple regions
-        ValueError: if the spec cannot be matched against any region
+        RuntimeError
+            If the spec matches multiple regions
+        ValueError
+            If the spec cannot be matched against any region
         """
         if isinstance(regionspec, region.Region) and (regionspec.parcellation == self):
             return regionspec
 
         if regionspec.startswith("Group"):  # backwards compatibility with old "Group: <region a>, <region b>" specs
             candidates = {
                 r
```

### Comparing `siibra-0.4a33/siibra/core/region.py` & `siibra-0.4a35/siibra/core/region.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from ..locations import boundingbox, point, pointset
 from ..volumes import parcellationmap
 
 from ..commons import (
     logger,
     MapIndex,
     MapType,
-    compare_maps,
     affine_scaling,
     create_key,
     clear_name,
     InstanceTable,
     SIIBRA_DEFAULT_MAPTYPE,
     SIIBRA_DEFAULT_MAP_THRESHOLD
 )
@@ -67,27 +66,28 @@
         """
         Constructs a new Region object.
 
         Parameters
         ----------
         name : str
             Human-readable name of the region
-        children: list of Regions,
+        children: list[Region]
         parent: Region
         shortname: str
             Shortform of human-readable name (optional)
         description: str
             Textual description of the parcellation
-        modality  :  str or None
+        modality:  str or None
             Specification of the modality used for specifying this region
         publications: list
-            List of ssociated publications, each a dictionary with "doi" and/or "citation" fields
-        datasets : list
+            List of associated publications, each a dictionary with "doi"
+            and/or "citation" fields
+        datasets: list
             datasets associated with this region
-        rgb: str, default None
+        rgb: str, default: None
             Hexcode of preferred color of this region (e.g. "#9FE770")
         """
         anytree.NodeMixin.__init__(self)
         concept.AtlasConcept.__init__(
             self,
             identifier=None,  # lazy property implementation below
             name=clear_name(name),
@@ -130,15 +130,15 @@
         if self._species_cached is None:
             self._species_cached = self.parcellation.species
         return self._species_cached
 
     @staticmethod
     def copy(other: 'Region'):
         """
-        copy contructor must detach the parent to avoid problems with
+        copy constructor must detach the parent to avoid problems with
         the Anytree implementation.
         """
         # create an isolated object, detached from the other's tree
         region = Region(
             name=other.name,
             children=[Region.copy(c) for c in other.children],
             parent=None,
@@ -179,15 +179,23 @@
         return hash(self.id)
 
     def has_parent(self, parent):
         return parent in [a for a in self.ancestors]
 
     def includes(self, region):
         """
-        Determine wether this regiontree includes the given region.
+        Determine whether this region-tree includes the given region.
+
+        Parameters
+        ----------
+        region: Region
+        Returns
+        -------
+            bool
+                True if the region is in the region-tree.
         """
         return region == self or region in self.descendants
 
     def find(
         self,
         regionspec,
         filter_children=False,
@@ -195,31 +203,33 @@
     ) -> List['Region']:
         """
         Find regions that match the given region specification in the subtree
         headed by this region.
 
         Parameters
         ----------
-        regionspec : any of
-            - a string with a possibly inexact name, which is matched both
-              against the name and the identifier key,
-            - a string in '/pattern/flags' format to use regex search (acceptable flags: aiLmsux),
-            - a regex applied to region names,
-            - an integer, which is interpreted as a labelindex,
-            - a full MapIndex
-            - a region object
-        filter_children : Boolean
-            If true, children of matched parents will not be returned
-        find_topmost : Bool, default: True
+        regionspec: str, regex, int, Region, MapIndex
+            - a string with a possibly inexact name (matched both against the name and the identifier key)
+            - a string in '/pattern/flags' format to use regex search (acceptable flags: aiLmsux)
+            - a regex applied to region names
+            - an integer (interpreted as a labelindex)
+            - a Region object
+            - a full MapIndex object
+        filter_children : bool, default: False
+            If True, children of matched parents will not be returned
+        find_topmost : bool, default: True
             If True, will return parent structures if all children are matched,
             even though the parent itself might not match the specification.
-
-        Yield
-        -----
-        list of matching regions
+        Returns
+        -------
+        list[Region]
+            list of regions matching to the regionspec
+        Tip
+        ---
+        See example 01-003 find regions
         """
         key = (regionspec, filter_children, find_topmost)
         MEM = self._CACHED_REGION_SEARCHES
         if key in MEM:
             return MEM[key]
 
         if isinstance(regionspec, str):
@@ -310,28 +320,27 @@
             else found_regions
         )
 
         return MEM[key]
 
     def matches(self, regionspec):
         """
-        Checks wether this region matches the given region specification.
+        Checks whether this region matches the given region specification.
 
         Parameters
-        ---------
-
-        regionspec : any of
-            - a string with a possibly inexact name, which is matched both
-              against the name and the identifier key,
+        ----------
+        regionspec: str, regex, Region
+            - a string with a possibly inexact name, which is matched both against the name and the identifier key,
             - a regex applied to region names,
             - a region object
 
-        Yield
-        -----
-        True or False
+        Returns
+        -------
+        bool
+            If the regionspec matches to the Region.
         """
         if regionspec is None:
             return False
 
         def splitstr(s):
             return [w for w in re.split(r"[^a-zA-Z0-9.\-]", s) if len(w) > 0]
 
@@ -356,49 +365,61 @@
                     for w in W
                 ) for q in Q])
 
         # TODO since dropping 3.6 support, maybe reimplement as re.Pattern ?
         elif isinstance(regionspec, REGEX_TYPE):
             # match regular expression
             return any(regionspec.search(s) is not None for s in [self.name, self.key])
+        elif isinstance(regionspec, (list, tuple)):
+            return any(self.matches(_) for _ in regionspec)
         else:
             raise TypeError(
                 f"Cannot interpret region specification of type '{type(regionspec)}'"
             )
 
     def fetch_regional_map(
         self,
         space: Union[str, _space.Space],
         maptype: MapType = SIIBRA_DEFAULT_MAPTYPE,
         threshold: float = SIIBRA_DEFAULT_MAP_THRESHOLD,
         via_space: Union[str, _space.Space] = None
     ):
         """
         Attempts to build a binary mask of this region in the given space,
-        using the specified maptypes.
+        using the specified MapTypes.
 
         Parameters
         ----------
-        space: Space object or space name
+        space: Space or str
             The requested reference space
-        maptype: MapType
-            the type of map to be used (labelled or statistical)
-        threshold: float
-            (optional) When fetching a statistical map, use this
-            threshold to convert it to a binary mask
-        via_space: Space object or space name
+        maptype: MapType, default: SIIBRA_DEFAULT_MAPTYPE
+            The type of map to be used ('labelled' or 'statistical')
+        threshold: float, optional
+            When fetching a statistical map, use this threshold to convert
+            it to a binary mask
+        via_space: Space or str
             If specified, fetch the map in this space first, and then perform
             a linear warping from there to the requested space.
-            You might want to use this if a map in the requested space is not available.
-            Note that this linear warping is an affine approximation of the
-            nonlinear deformation, computed from the warped corenr points
-            of the bounding box (see siibra.location.BoundingBox.estimate_affine()).
-            It does not require voxel resampling,
-            just replaces the affine matrix, but is less accurate than a full
-            nonlinear warping, which is not supported in siibra-python for images so far.
+
+            Tip
+            ---
+                You might want to use this if a map in the requested space
+                is not available.
+
+            Note
+            ----
+                This linear warping is an affine approximation of the
+                nonlinear deformation, computed from the warped corner points
+                of the bounding box (see siibra.locations.BoundingBox.estimate_affine()).
+                It does not require voxel resampling, just replaces the affine
+                matrix, but is less accurate than a full nonlinear warping,
+                which is currently not supported in siibra-python for images.
+        Returns
+        -------
+        Nifti1Image
         """
         if isinstance(maptype, str):
             maptype = MapType[maptype.upper()]
         result = None
 
         # prepare space instances
         if isinstance(space, str):
@@ -462,14 +483,24 @@
             )
 
         return result
 
     def mapped_in_space(self, space, recurse: bool = True) -> bool:
         """
         Verifies wether this region is defined by an explicit map in the given space.
+
+        Parameters
+        ----------
+        space: Space or str
+            reference space
+        recurse: bool, default: True
+            If True, check if all child regions are mapped instead
+        Returns
+        -------
+        bool
         """
         from ..volumes.parcellationmap import Map
         for m in Map.registry():
             # Use and operant for efficiency (short circuiting logic)
             # Put the most inexpensive logic first
             if (
                 self.name in m.regions
@@ -504,26 +535,25 @@
             matchfunc=_space.Space.matches,
             elements={s.key: s for s in self.supported_spaces},
         )
 
     def __getitem__(self, labelindex):
         """
         Given an integer label index, return the corresponding region.
+
         If multiple matches are found, return the unique parent if possible.
-        Otherwise, return None
+        Otherwise, returns None.
 
         Parameters
         ----------
-
         regionlabel: int
-            label index of the desired region.
-
-        Return
-        ------
-        Region object
+            Label index of the desired region.
+        Returns
+        -------
+        Region
         """
         if not isinstance(labelindex, int):
             raise TypeError(
                 "Index access into the regiontree expects label indices of integer type"
             )
 
         # first test this head node
@@ -544,44 +574,47 @@
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return self.name
 
     def tree2str(self):
+        """Render region-tree as a string"""
         return "\n".join(
             "%s%s" % (pre, node.name)
             for pre, _, node
             in anytree.RenderTree(self, style=anytree.render.ContRoundStyle)
         )
 
     def render_tree(self):
+        """Prints the tree representation of the region"""
         print(self.tree2str())
 
     def get_bounding_box(
         self,
         space: _space.Space,
         maptype: MapType = MapType.LABELLED,
         threshold_statistical=None,
     ):
         """Compute the bounding box of this region in the given space.
 
         Parameters
         ----------
-        space : Space or str):
+        space: Space or str
             Requested reference space
-        maptype: MapType
+        maptype: MapType, default: MapType.LABELLED
             Type of map to build ('labelled' will result in a binary mask,
             'statistical' attempts to build a statistical mask, possibly by
-            elementwise maximum of statistical maps of children )
+            elementwise maximum of statistical maps of children)
         threshold_statistical: float, or None
             if not None, masks will be preferably constructed by thresholding
             statistical maps with the given value.
-        Returns:
-            BoundingBox
+        Returns
+        -------
+        BoundingBox
         """
         spaceobj = _space.Space.get_instance(space)
         try:
             mask = self.fetch_regional_map(
                 spaceobj, maptype=maptype, threshold=threshold_statistical
             )
             return boundingbox.BoundingBox.from_image(mask, space=spaceobj)
@@ -602,18 +635,29 @@
                         return bbox.warp(spaceobj)
                 except RuntimeError:
                     continue
         logger.error(f"Could not compute bounding box for {self.name}.")
         return None
 
     def compute_centroids(self, space: _space.Space) -> pointset.PointSet:
-        """Compute the centroids of the region in the given space.
+        """
+        Compute the centroids of the region in the given space.
 
-        Note that a region can generally have multiple centroids
-        if it has multiple connected components in the map.
+        Parameters
+        ----------
+        space: Space
+            reference space in which the computation will be performed
+        Returns
+        -------
+        PointSet
+            Found centroids (as Point objects) in a PointSet
+        Note
+        ----
+        A region can generally have multiple centroids if it has multiple
+        connected components in the map.
         """
         props = self.spatial_props(space)
         return pointset.PointSet(
             [tuple(c["centroid"]) for c in props["components"] if "centroid" in c],
             space=space
         )
 
@@ -624,27 +668,28 @@
         threshold_statistical=None,
     ):
         """
         Compute spatial properties for connected components of this region in the given space.
 
         Parameters
         ----------
-        space : _space.Space
-            the space in which the computation shall be performed
-        maptype: MapType
+        space: Space
+            reference space in which the computation will be performed
+        maptype: MapType, default: MapType.LABELLED
             Type of map to build ('labelled' will result in a binary mask,
             'statistical' attempts to build a statistical mask, possibly by
-            elementwise maximum of statistical maps of children )
+            elementwise maximum of statistical maps of children)
         threshold_statistical: float, or None
             if not None, masks will be preferably constructed by thresholding
             statistical maps with the given value.
 
-        Return
-        ------
-        dictionary of regionprops.
+        Returns
+        -------
+        Dict
+            Dictionary of region's spatial properties
         """
         result = {"space": space, "components": []}
         from skimage import measure
 
         if not isinstance(space, _space.Space):
             space = _space.Space.get_instance(space)
 
@@ -677,46 +722,13 @@
             )
             props["volume"] = nonzero.shape[0] * scale
 
             result["components"].append(props)
 
         return result
 
-    def compare(
-        self,
-        img: Nifti1Image,
-        space: _space.Space,
-        use_maptype: MapType = MapType.STATISTICAL,
-        threshold_statistical: float = None,
-        resolution_mm: float = None,
-    ):
-        """
-        Compare the given image to the map of this region in the specified space.
-
-        Parameters:
-        -----------
-        img: Nifti1Image
-            Image to compare with
-        space: Space
-            Reference space to use
-        use_maptype: MapType
-            Type of map to build ('labelled' will result in a binary mask,
-            'statistical' attempts to build a statistical mask, possibly by
-            elementwise maximum of statistical maps of children )
-        threshold_statistical: float, or None
-            if not None, masks will be preferably constructed by thresholding
-            statistical maps with the given value.
-        """
-        mask = self.fetch_regional_map(
-            space,
-            resolution_mm,
-            maptype=use_maptype,
-            threshold=threshold_statistical,
-        )
-        return compare_maps(mask, img)
-
     def __iter__(self):
         """
         Returns an iterator that goes through all regions in this subtree
         (including this parent region)
         """
         return anytree.PreOrderIter(self)
```

### Comparing `siibra-0.4a33/siibra/core/space.py` & `siibra-0.4a35/siibra/core/space.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,32 +41,33 @@
         datasets: list = [],
     ):
         """
         Constructs a new parcellation object.
 
         Parameters
         ----------
-        identifier : str
-            Unique identifier of the space
-        name : str
-            Human-readable name of the space
-        species: str or Species
-            Specification of the species
-        volumes: list of template volumes
-        shortname: str
-            Shortform of human-readable name (optional)
-        description: str
-            Textual description of the parcellation
-        modality  :  str or None
-            Specification of the modality representing this reference space
-        publications: list
-            List of ssociated publications, each a dictionary with "doi" and/or "citation" fields
-        ebrains_ids : dict
-            Identifiers of EBRAINS entities corresponding to this Parcellation.
-            Key: EBRAINS KG schema, value: EBRAINS KG @id
+            identifier : str
+                Unique identifier of the space
+            name : str
+                Human-readable name of the space
+            species: str or Species
+                Specification of the species
+            volumes: list[Volume]
+                list of template volumes
+            shortname: str, optional
+                Shortform of human-readable name
+            description: str, optional
+                Textual description of the parcellation
+            modality  :  str or None
+                Specification of the modality representing this reference space
+            publications: list
+                List of associated publications, each a dictionary with "doi" and/or "citation" fields
+            ebrains_ids : dict
+                Identifiers of EBRAINS entities corresponding to this Parcellation.
+                Key: EBRAINS KG schema, value: EBRAINS KG @id
         """
 
         AtlasConcept.__init__(
             self,
             identifier=identifier,
             name=name,
             species=species,
@@ -82,27 +83,28 @@
 
     def get_template(self, variant: str = None, format: str = None):
         """
         Get the volumetric reference template for this space.
 
         Parameters
         ----------
-        variant: str (optional)
-            Some templates are provided in different variants, e.g.
-            freesurfer is available as either white matter, pial or
-            inflated surface for left and right hemispheres (6 variants).
-            This field could be used to request a specific variant.
-            Per default, the first found variant is returned.
-        format: str (optional)
-            Volumes are typically available in multiple formats.
-            Use this to select a specific one, if needed.
-
-        Yields
-        ------
-        A VolumeSrc object representing the reference template, or None if not available.
+            variant: str, optional
+                Some templates are provided in different variants, e.g.
+                freesurfer is available as either white matter, pial or
+                inflated surface for left and right hemispheres (6 variants).
+                This field could be used to request a specific variant.
+                Per default, the first found variant is returned.
+            format: str, optional
+                Volumes are typically available in multiple formats.
+                Use this to select a specific one, if needed.
+
+        Returns
+        -------
+            Volume
+                representing the reference template, or None if not available.
         """
         tests = []
         if variant is not None:
             tests.append(lambda v: hasattr(v, 'variant') and variant.lower() in v.variant.lower())
         candidates = [v for v in self.volumes if all(t(v) for t in tests)]
 
         if len(candidates) == 0:
@@ -127,18 +129,18 @@
     def provides_image(self):
         return any(v.provides_image for v in self.volumes)
 
     def __getitem__(self, slices):
         """
         Get a volume of interest specification from this space.
 
-        Arguments
-        ---------
-        slices: triple of slice
-            defines the x, y and z range
+        Parameters
+        ----------
+            slices: triple of slice
+                Defines the x, y and z range
         """
         if len(slices) != 3:
             raise TypeError(
                 "Slice access to spaces needs to define x,y and z ranges (e.g. Space[10:30,0:10,200:300])"
             )
         point1 = [0 if s.start is None else s.start for s in slices]
         point2 = [s.stop for s in slices]
@@ -149,13 +151,16 @@
             point2 = [shape[i] if v is None else v for i, v in enumerate(point2)]
         return self.get_bounding_box(point1, point2)
 
     def get_bounding_box(self, point1, point2):
         """
         Get a volume of interest specification from this space.
 
-        Arguments
-        ---------
-        point1: 3D tuple defined in physical coordinates of this reference space
-        point2: 3D tuple defined in physical coordinates of this reference space
+        Parameters
+        ----------
+            point1: 3D tuple defined in physical coordinates of this reference space
+            point2: 3D tuple defined in physical coordinates of this reference space
+        Returns
+        -------
+            BoundingBox
         """
         return BoundingBox(point1, point2, self)
```

### Comparing `siibra-0.4a33/siibra/features/anchor.py` & `siibra-0.4a35/siibra/features/anchor.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,19 +140,19 @@
 
     @property
     def location(self):
         # allow to overwrite in derived classes
         return self._location_cached
 
     @property
-    def parcellations(self):
+    def parcellations(self) -> List[Parcellation]:
         return list({region.root for region in self.regions})
 
     @property
-    def space(self):
+    def space(self) -> Space:
         # may be overriden by derived classes, e.g. in features.VolumeOfInterest
         if self.location is None:
             return None
         else:
             return self.location.space
 
     @property
```

### Comparing `siibra-0.4a33/siibra/features/basetypes/__init__.py` & `siibra-0.4a35/siibra/features/dataset/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,7 +8,9 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+from .ebrains import EbrainsDataFeature
```

### Comparing `siibra-0.4a33/siibra/features/basetypes/cortical_profile.py` & `siibra-0.4a35/siibra/features/tabular/cortical_profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from . import feature
+from . import tabular
 
 from .. import anchor as _anchor
 
 import pandas as pd
 from typing import Union, Dict, Tuple
 from textwrap import wrap
 import numpy as np
 
 
-class CorticalProfile(feature.Feature):
+class CorticalProfile(tabular.Tabular):
     """
     Represents a 1-dimensional profile of measurements along cortical depth,
     measured at relative depths between 0 representing the pial surface,
     and 1 corresponding to the gray/white matter boundary.
 
     Mandatory attributes are the list of depth coordinates and the list of
     corresponding measurement values, which have to be of equal length,
@@ -52,54 +52,53 @@
         values: Union[list, np.ndarray] = None,
         unit: str = None,
         boundary_positions: Dict[Tuple[int, int], float] = None,
         datasets: list = []
     ):
         """Initialize profile.
 
-        Args:
-            description (str):
-                Human-readable of the modality of the measurements.
-            modality (str):
-                Short textual description of the modaility of measurements
-            anchor: AnatomicalAnchor
-            depths (list, optional):
-                List of cortical depthh positions corresponding to each
-                measurement, all in the range [0..1].
-                Defaults to None.
-            values (list, optional):
-                List of the actual measurements at each depth position.
-                Length must correspond to 'depths'.
-                Defaults to None.
-            unit (str, optional):
-                Textual identifier for the unit of measurements.
-                Defaults to None.
-            boundary_positions (dict, optional):
-                Dictionary of depths at which layer boundaries were identified.
-                Keys are tuples of layer numbers, e.g. (1,2), values are cortical
-                depth positions in the range [0..1].
-                Defaults to None.
-            datasets : list
-                list of datasets corresponding to this feature
+        Parameters
+        ----------
+        description: str
+            Human-readable of the modality of the measurements.
+        modality: str
+            Short textual description of the modality of measurements.
+        anchor: AnatomicalAnchor
+        depths: list, default: None
+            List of cortical depth positions corresponding to each
+            measurement, all in the range [0..1]
+        values: list, default: None
+            List of the actual measurements at each depth position.
+            Length must correspond to 'depths'.
+        unit: str, default: None
+            Textual identifier for the unit of measurements.
+        boundary_positions: dict, default: None
+            Dictionary of depths at which layer boundaries were identified.
+            Keys are tuples of layer numbers, e.g. (1,2), and values are
+            cortical depth positions in the range [0..1].
+        datasets : list[Dataset]
+            list of datasets corresponding to this feature
         """
-        feature.Feature.__init__(
-            self,
-            modality=modality,
-            description=description,
-            anchor=anchor,
-            datasets=datasets
-        )
 
         # cached properties will be revealed as property functions,
         # so derived classes may choose to override for lazy loading.
         self._unit = unit
         self._depths_cached = depths
         self._values_cached = values
         self._boundary_positions = boundary_positions
 
+        tabular.Tabular.__init__(
+            self,
+            modality=modality,
+            description=description,
+            anchor=anchor,
+            data=None,  # lazy loader below
+            datasets=datasets
+        )
+
     def _check_sanity(self):
         # check plausibility of the profile
         assert isinstance(self._depths, (list, np.ndarray))
         assert isinstance(self._values, (list, np.ndarray))
         assert len(self._values) == len(self._depths)
         assert all(0 <= d <= 1 for d in self._depths)
         if self.boundaries_mapped:
@@ -113,15 +112,15 @@
     def unit(self) -> str:
         """Optionally overridden in derived classes."""
         if self._unit is None:
             raise NotImplementedError(f"'unit' not set for {self.__class__.__name__}.")
         return self._unit
 
     @property
-    def boundary_positions(self):
+    def boundary_positions(self) -> Dict[Tuple[int, int], float]:
         if self._boundary_positions is None:
             return {}
         else:
             return self._boundary_positions
 
     def assign_layer(self, depth: float):
         """Compute the cortical layer for a given depth from the
@@ -152,20 +151,22 @@
         else:
             return None
 
     @property
     def data(self):
         """Return a pandas Series representing the profile."""
         self._check_sanity()
-        return pd.Series(
-            self._values, index=self._depths, name=f"{self.modality} ({self.unit})"
+        return pd.DataFrame(
+            self._values, index=self._depths, columns=[f"{self.modality} ({self.unit})"]
         )
 
     def plot(self, **kwargs):
-        """Plot the profile.
+        """
+        Plot the profile.
+
         Keyword arguments are passed on to the plot command.
         'layercolor' can be used to specify a color for cortical layer shading.
         """
         wrapwidth = kwargs.pop("textwrap") if "textwrap" in kwargs else 40
 
         kwargs["title"] = kwargs.get("title", "\n".join(wrap(self.name, wrapwidth)))
         kwargs["xlabel"] = kwargs.get("xlabel", "Cortical depth")
@@ -190,24 +191,30 @@
 
         axs.set_title(axs.get_title(), fontsize="medium")
 
         return axs
 
     @property
     def _depths(self):
-        """Returns a list of the relative cortical depths of the measured values in the range [0..1].
-        To be implemented in derived class."""
+        """
+        Returns a list of the relative cortical depths of the measured values in the range [0..1].
+
+        To be implemented in derived class.
+        """
         if self._depths_cached is None:
             raise NotImplementedError(
                 f"'_depths' not available for {self.__class__.__name__}."
             )
         return self._depths_cached
 
     @property
     def _values(self):
-        """Returns a list of the measured values per depth.
-        To be implemented in derived class."""
+        """
+        Returns a list of the measured values per depth.
+
+        To be implemented in derived class.
+        """
         if self._values_cached is None:
             raise NotImplementedError(
                 f"'_values' not available for {self.__class__.__name__}."
             )
         return self._values_cached
```

### Comparing `siibra-0.4a33/siibra/features/basetypes/feature.py` & `siibra-0.4a35/siibra/features/feature.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,37 +9,41 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .. import anchor as _anchor
+from . import anchor as _anchor
 
-from ...commons import logger
-from ...core import concept
-from ...core import space, region, parcellation
+from ..commons import logger, InstanceTable
+from ..core import concept
+from ..core import space, region, parcellation
 
 from typing import Union, TYPE_CHECKING, List, Dict, Type
 from tqdm import tqdm
 from hashlib import md5
 from collections import defaultdict
 
 if TYPE_CHECKING:
-    from ...retrieval.datasets import EbrainsDataset
+    from ..retrieval.datasets import EbrainsDataset
     TypeDataset = EbrainsDataset
 
 
 class Feature:
     """
     Base class for anatomically anchored data features.
     """
 
     SUBCLASSES: Dict[Type['Feature'], List[Type['Feature']]] = defaultdict(list)
 
+    CATEGORIZED: Dict[str, Type['InstanceTable']] = defaultdict(InstanceTable)
+    
+    category: str = None
+
     def __init__(
         self,
         modality: str,
         description: str,
         anchor: _anchor.AnatomicalAnchor,
         datasets: List['TypeDataset'] = []
     ):
@@ -57,35 +61,38 @@
         self._modality_cached = modality
         self._description = description
         self._anchor_cached = anchor
         self.datasets = datasets
 
     @property
     def modality(self):
-        # allows subclasses to implement lazy loading of an anchor
+        # allows subclasses to implement lazy loading of the modality
         return self._modality_cached
 
     @property
     def anchor(self):
         # allows subclasses to implement lazy loading of an anchor
         return self._anchor_cached
 
-    def __init_subclass__(cls, configuration_folder=None):
+    def __init_subclass__(cls, configuration_folder=None, category=None):
         # extend the subclass lists
 
         # Iterate over all mro, not just immediate base classes
         for BaseCls in cls.__mro__:
             # some base classes may not be sub class of feature, ignore these
             if not issubclass(BaseCls, Feature):
                 continue
             cls.SUBCLASSES[BaseCls].append(cls)
 
         cls._live_queries = []
         cls._preconfigured_instances = None
         cls._configuration_folder = configuration_folder
+        cls.category = category
+        if category is not None:
+            cls.CATEGORIZED[category].add(cls.__name__, cls)
         return super().__init_subclass__()
 
     @classmethod
     def _get_subclasses(cls):
         return {Cls.__name__: Cls for Cls in cls.SUBCLASSES}
 
     @property
@@ -101,36 +108,37 @@
     @classmethod
     def get_instances(cls, **kwargs) -> List['Feature']:
         """
         Retrieve objects of a particular feature subclass.
         Objects can be preconfigured in the configuration,
         or delivered by Live queries.
         """
-        result = []
+        if not hasattr(cls, "_preconfigured_instances"):
+            return []
 
-        if hasattr(cls, "_preconfigured_instances"):
-            if cls._preconfigured_instances is None:
-                if cls._configuration_folder is None:
-                    cls._preconfigured_instances = []
-                else:
-                    from ...configuration.configuration import Configuration
-                    conf = Configuration()
-                    Configuration.register_cleanup(cls.clean_instances)
-                    assert cls._configuration_folder in conf.folders
-                    cls._preconfigured_instances = [
-                        o for o in conf.build_objects(cls._configuration_folder)
-                        if isinstance(o, cls)
-                    ]
-                    logger.debug(
-                        f"Built {len(cls._preconfigured_instances)} preconfigured {cls.__name__} "
-                        f"objects from {cls._configuration_folder}."
-                    )
-            result.extend(cls._preconfigured_instances)
+        if cls._preconfigured_instances is not None:
+            return cls._preconfigured_instances
 
-        return result
+        if cls._configuration_folder is None:
+            cls._preconfigured_instances = []
+            return cls._preconfigured_instances
+
+        from ..configuration.configuration import Configuration
+        conf = Configuration()
+        Configuration.register_cleanup(cls.clean_instances)
+        assert cls._configuration_folder in conf.folders
+        cls._preconfigured_instances = [
+            o for o in conf.build_objects(cls._configuration_folder)
+            if isinstance(o, cls)
+        ]
+        logger.debug(
+            f"Built {len(cls._preconfigured_instances)} preconfigured {cls.__name__} "
+            f"objects from {cls._configuration_folder}."
+        )
+        return cls._preconfigured_instances
 
     @classmethod
     def clean_instances(cls):
         """ Removes all instantiated object instances"""
         cls._preconfigured_instances = None
 
     def matches(self, concept: concept.AtlasConcept) -> bool:
@@ -231,15 +239,15 @@
         from anytree.importer import DictImporter
         from anytree import RenderTree
 
         def create_treenode(feature_type):
             return {
                 'name': feature_type.__name__,
                 'children': [
-                    create_treenode(c) 
+                    create_treenode(c)
                     for c in feature_type.__subclasses__()
                 ]
             }
         D = create_treenode(cls)
         importer = DictImporter()
         tree = importer.import_(D)
         return "\n".join(
```

### Comparing `siibra-0.4a33/siibra/features/basetypes/regional_connectivity.py` & `siibra-0.4a35/siibra/features/connectivity/regional_connectivity.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .feature import Feature
-from .tabular import Tabular
+from ..feature import Feature
+from ..tabular.tabular import Tabular
 
 from .. import anchor as _anchor
 
 from ...commons import logger, QUIET
 from ...core import region as _region
 from ...locations import pointset
 from ...retrieval.repositories import RepositoryConnector
@@ -27,55 +27,54 @@
 import pandas as pd
 import numpy as np
 from tqdm import tqdm
 
 
 class RegionalConnectivity(Feature):
     """
-    Parcellation-averaged connectivity, providing one or more
-    matrices of a given modality for a given parcellation.
-
+    Parcellation-averaged connectivity, providing one or more matrices of a
+    given modality for a given parcellation.
     """
 
     def __init__(
         self,
         cohort: str,
         modality: str,
         regions: list,
         connector: RepositoryConnector,
         decode_func: Callable,
         files: Dict[str, str],
         anchor: _anchor.AnatomicalAnchor,
         description: str = "",
         datasets: list = [],
     ):
-        """j
-        Construct a parcellation-averaged connectivty matrix.
+        """
+        Construct a parcellation-averaged connectivity matrix.
 
         Parameters
         ----------
         cohort: str
             Name of the cohort used for computing the connectivity.
         modality: str
             Connectivity modality, typically set by derived classes.
-        regions: list of str
+        regions: list[str]
             Names of the regions from the parcellation
         connector: Connector
             Repository connector for loading the actual data array(s).
         decode_func: function
             Function to convert the bytestream of a loaded file into an array
         files: dict
             A dictionary linking names of matrices (typically subject ids)
             to the relative filenames of the data array(s) in the repository connector.
         anchor: AnatomicalAnchor
             anatomical localization of the matrix, expected to encode the parcellation
             in the region attribute.
-        description: str (optional)
+        description: str, optional
             textual description of this connectivity matrix.
-        datasets : list
+        datasets : list[Dataset]
             list of datasets corresponding to this feature.
         """
         Feature.__init__(
             self,
             modality=modality,
             description=description,
             anchor=anchor,
@@ -97,18 +96,22 @@
 
     def get_matrix(self, subject: str = None):
         """
         Returns a matrix as a pandas dataframe.
 
         Parameters
         ----------
-        subject: str
+        subject: str, default: None
             Name of the subject (see ConnectivityMatrix.subjects for available names).
             If "mean" or None is given, the mean is taken in case of multiple
             available matrices.
+        Returns
+        -------
+        pd.DataFrame
+            A square matrix with region names as the column and row names.
         """
         assert len(self) > 0
         if (subject is None) and (len(self) > 1):
             # multiple matrices available, but no subject given - return mean matrix
             logger.info(
                 f"No subject name supplied, returning mean connectivity across {len(self)} subjects. "
                 "You might alternatively specify an individual subject."
@@ -177,17 +180,25 @@
         subject: str = None,
         min_connectivity: float = 0,
         max_rows: int = None
     ):
         """
         Extract a regional profile from the matrix, to obtain a tabular data feature
         with the connectivity as the single column.
+
         Rows will be sorted by descending connection strength.
         Regions with connectivity smaller than "min_connectivity" will be discarded.
         If max_rows is given, only the subset of regions with highest connectivity is returned.
+
+        Parameters
+        ----------
+        region: str, Region
+        subject: str, default: None
+        min_connectivity: float, default: 0
+        max_rows: int, default: None
         """
         matrix = self.get_matrix(subject)
 
         def matches(r1, r2):
             if isinstance(r1, tuple):
                 return any(r.matches(r2) for r in r1)
             else:
@@ -232,16 +243,23 @@
             "_".join(p.name for p in self.anchor.parcellations),
             self.cohort,
             len(self._files),
         )
 
     def compute_centroids(self, space):
         """
-        compute the list of centroid coordinates corresponding to
-        matrix rows, in the given space.
+        Computes the list of centroid coordinates corresponding to
+        matrix rows, in the given reference space.
+
+        Parameters
+        ----------
+        space: Space, str
+        Returns
+        -------
+        list[tuple(float, float, float)]
         """
         result = []
         parcellations = self.anchor.represented_parcellations()
         assert len(parcellations) == 1
         parcmap = next(iter(parcellations)).get_map(space)
         all_centroids = parcmap.compute_centroids()
         for regionname in self.regions:
@@ -257,15 +275,15 @@
                 ).centroid)
             )
         return result
 
     def _array_to_dataframe(self, array: np.ndarray) -> pd.DataFrame:
         """
         Convert a numpy array with the connectivity matrix to
-        a dataframe with regions as column and row headers.
+        a DataFrame with regions as column and row headers.
         """
         df = pd.DataFrame(array)
         parcellations = self.anchor.represented_parcellations()
         assert len(parcellations) == 1
         parc = next(iter(parcellations))
         with QUIET:
             indexmap = {
```

### Comparing `siibra-0.4a33/siibra/features/basetypes/tabular.py` & `siibra-0.4a35/siibra/features/tabular/tabular.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,36 +9,35 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from . import feature
+from .. import feature
 
 from .. import anchor as _anchor
 
 from ... import commons
 
 import pandas as pd
 from textwrap import wrap
 
 
 class Tabular(feature.Feature):
     """
     Represents a table of different measures anchored to a brain location.
 
-    Columns represent different types of values, while rows represent
-    different samples. The number of columns might thus be intrepreted
-    as the feature dimension.
-
-    As an example, receptor fingerprints use rows
-    to represent different neurotransmitter receptors, and separate
-    columns for the mean and standard deviations measure across multiple
-    tissue samples.
+    Columns represent different types of values, while rows represent different
+    samples. The number of columns might thus be interpreted as the feature
+    dimension.
+
+    As an example, receptor fingerprints use rows to represent different
+    neurotransmitter receptors, and separate columns for the mean and standard
+    deviations measure across multiple tissue samples.
     """
 
     def __init__(
         self,
         description: str,
         modality: str,
         anchor: _anchor.AnatomicalAnchor,
@@ -55,15 +54,21 @@
         self._data_cached = data
 
     @property
     def data(self):
         return self._data_cached
 
     def plot(self, **kwargs):
-        """ Create a bar plot of a columns of the data."""
+        """
+        Create a bar plot of a columns of the data.
+        Parameters
+        ----------
+        **kwargs
+            takes Matplotlib.pyplot keyword arguments
+        """
 
         try:
             import matplotlib.pyplot as plt
         except ImportError:
             commons.logger.error("matplotlib not available. Plotting of fingerprints disabled.")
             return None
```

### Comparing `siibra-0.4a33/siibra/features/basetypes/volume_of_interest.py` & `siibra-0.4a35/siibra/features/image/image.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,50 +9,52 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from . import feature
+from .. import feature
 
 from .. import anchor as _anchor
 
 from ...volumes import volume as _volume
 
 from typing import List
 
 
-class VolumeOfInterestAnchor(_anchor.AnatomicalAnchor):
+class ImageAnchor(_anchor.AnatomicalAnchor):
 
     def __init__(self, volume: _volume.Volume, region: str = None):
         _anchor.AnatomicalAnchor.__init__(
             self,
             species=volume.space.species,
             location=None,
             region=region
         )
         self.volume = volume
 
     @property
     def location(self):
-        """ loads the bounding box only if required, since it demands image data access. """
+        """
+        Loads the bounding box only if required, since it demands image data access.
+        """
         if self._location_cached is None:
             self._location_cached = self.volume.boundingbox
         return self._location_cached
 
     @property
     def space(self):
         return self.volume.space
 
     def __str__(self):
-        return "bounding box of volume"
+        return f"Bounding box of image in {self.space.name}"
 
 
-class VolumeOfInterest(feature.Feature, _volume.Volume, configuration_folder="features/volumes"):
+class Image(feature.Feature, _volume.Volume):
 
     def __init__(
         self,
         name: str,
         modality: str,
         space_spec: dict,
         providers: List[_volume.VolumeProvider],
@@ -62,32 +64,34 @@
         feature.Feature.__init__(
             self,
             modality=modality,
             description=None,  # lazy implementation below!
             anchor=None,  # lazy implementation below!
             datasets=datasets
         )
+
         _volume.Volume.__init__(
             self,
             space_spec=space_spec,
             providers=providers,
             name=name,
         )
-        self._anchor_cached = VolumeOfInterestAnchor(self, region=region)
+
+        self._anchor_cached = ImageAnchor(self, region=region)
         self._description_cached = None
         self._name_cached = name
 
     @property
     def name(self):
         if self._name_cached is None:
             return feature.Feature.name(self)
         else:
             return f"{self._name_cached} ({self.modality})"
 
     @property
     def description(self):
         if self._description_cached is None:
             self._description_cached = (
-                f"Volume of interest with modality {self.modality} "
+                f"Image feature with modality {self.modality} "
                 f"at {self.anchor}"
             )
         return self._description_cached
```

### Comparing `siibra-0.4a33/siibra/features/cellular/bigbrain_intensity_profile.py` & `siibra-0.4a35/siibra/features/tabular/bigbrain_intensity_profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,23 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ..basetypes import cortical_profile
+from . import cortical_profile
 
 from ...locations import point
 
 
-class BigBrainIntensityProfile(cortical_profile.CorticalProfile):
+class BigBrainIntensityProfile(
+    cortical_profile.CorticalProfile,
+    category='cellular'
+):
 
     DESCRIPTION = (
         "Cortical profiles of BigBrain staining intensities computed by Konrad Wagstyl, "
         "as described in the publication 'Wagstyl, K., et al (2020). BigBrain 3D atlas of "
         "cortical layers: Cortical and laminar thickness gradients diverge in sensory and "
         "motor cortices. PLoS Biology, 18(4), e3000678. "
         "http://dx.doi.org/10.1371/journal.pbio.3000678'."
```

### Comparing `siibra-0.4a33/siibra/features/cellular/cell_density_profile.py` & `siibra-0.4a35/siibra/features/tabular/cell_density_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,27 +10,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .. import anchor as _anchor
-from ..basetypes import cortical_profile
+from . import cortical_profile
 
 from ...commons import PolyLine, logger, create_key
 from ...retrieval import requests
 
 from skimage.draw import polygon
 from skimage.transform import resize
 from io import BytesIO
 import numpy as np
 import pandas as pd
 
 
-class CellDensityProfile(cortical_profile.CorticalProfile, configuration_folder="features/profiles/celldensity"):
+class CellDensityProfile(
+    cortical_profile.CorticalProfile,
+    configuration_folder="features/tabular/corticalprofiles/celldensity",
+    category='cellular'
+):
 
     DESCRIPTION = (
         "Cortical profile of estimated densities of detected cell bodies (in detected cells per 0.1 cube millimeter) "
         "obtained by applying a Deep Learning based instance segmentation algorithm (Contour Proposal Network; Upschulte "
         "et al., Neuroimage 2022) to a 1 micron resolution cortical image patch prepared with modified Silver staining. "
         "Densities have been computed per cortical layer after manual layer segmentation, by dividing the number of "
         "detected cells in that layer with the area covered by the layer. Therefore, each profile contains 6 measurement points. "
```

### Comparing `siibra-0.4a33/siibra/features/cellular/layerwise_bigbrain_intensities.py` & `siibra-0.4a35/siibra/features/tabular/layerwise_bigbrain_intensities.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ..basetypes import cortical_profile, tabular
+from . import cortical_profile
+from . import tabular
 
 import pandas as pd
 import numpy as np
 
 
-class LayerwiseBigBrainIntensities(tabular.Tabular):
+class LayerwiseBigBrainIntensities(
+    tabular.Tabular,
+    category='cellular'
+):
 
     DESCRIPTION = (
         "Layerwise averages and standard deviations of of BigBrain staining intensities "
         "computed by Konrad Wagstyl, as described in the publication "
         "'Wagstyl, K., et al (2020). BigBrain 3D atlas of "
         "cortical layers: Cortical and laminar thickness gradients diverge in sensory and "
         "motor cortices. PLoS Biology, 18(4), e3000678. "
```

### Comparing `siibra-0.4a33/siibra/features/cellular/layerwise_cell_density.py` & `siibra-0.4a35/siibra/features/tabular/layerwise_cell_density.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,31 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from . import cortical_profile
 from .. import anchor as _anchor
-from ..basetypes import cortical_profile, tabular
+from . import tabular
 
 from ... import commons
 from ...retrieval import requests
 
 import pandas as pd
 import numpy as np
 from io import BytesIO
 
 
-class LayerwiseCellDensity(tabular.Tabular, configuration_folder="features/fingerprints/celldensity"):
+class LayerwiseCellDensity(
+    tabular.Tabular,
+    configuration_folder="features/tabular/layerstatistics/celldensity",
+    category='cellular'
+):
 
     DESCRIPTION = (
         "Layerwise estimated densities of detected cell bodies  (in detected cells per 0.1 cube millimeter) "
         "obtained by applying a Deep Learning based instance segmentation algorithm (Contour Proposal Network; Upschulte "
         "et al., Neuroimage 2022) to a 1 micron resolution cortical image patch prepared with modified Silver staining. "
         "Densities have been computed per cortical layer after manual layer segmentation, by dividing the number of "
         "detected cells in that layer with the area covered by the layer. Therefore, each profile contains 6 measurement points. "
@@ -72,15 +77,16 @@
                 layers = requests.HttpRequest(layerfile, func=self.LAYER_READER).data
             except requests.SiibraHttpRequestError as e:
                 print(str(e))
                 commons.logger.error(f"Skipping to bootstrap a {self.__class__.__name__} feature, cannot access file resource.")
                 continue
             counts = cells.layer.value_counts()
             areas = layers["Area(micron**2)"]
-            density_dict[i] = counts[areas.index] / areas * 100 ** 2 * 5
+            indices = np.intersect1d(areas.index, counts.index)
+            density_dict[i] = counts[indices] / areas * 100 ** 2 * 5
         return pd.DataFrame(density_dict)
 
     @property
     def data(self):
         if self._data_cached is None:
             densities = self._load_densities()
             self._data_cached = pd.DataFrame(
```

### Comparing `siibra-0.4a33/siibra/features/connectivity/__init__.py` & `siibra-0.4a35/siibra/features/connectivity/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,7 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .functional_connectivity import FunctionalConnectivity
 from .streamline_counts import StreamlineCounts
 from .streamline_lengths import StreamlineLengths
-
-
-def __dir__():
-    return [
-        "FunctionalConnectivity",
-        "StreamlineCounts",
-        "StreamlineLengths",
-    ]
```

### Comparing `siibra-0.4a33/siibra/features/connectivity/functional_connectivity.py` & `siibra-0.4a35/siibra/features/connectivity/functional_connectivity.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ..basetypes import regional_connectivity
+from . import regional_connectivity
 
 
 class FunctionalConnectivity(
     regional_connectivity.RegionalConnectivity,
-    configuration_folder="features/connectivitymatrix/functional"
+    configuration_folder="features/connectivity/regional/functional",
+    category="connectivity"
 ):
     """Functional connectivity matrix grouped by a parcellation."""
 
     def __init__(self, paradigm: str, **kwargs):
         regional_connectivity.RegionalConnectivity.__init__(self, **kwargs)
         self.paradigm = paradigm
```

### Comparing `siibra-0.4a33/siibra/features/connectivity/streamline_counts.py` & `siibra-0.4a35/siibra/features/connectivity/streamline_lengths.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ..basetypes import regional_connectivity
+from . import regional_connectivity
 
 
-class StreamlineCounts(
+class StreamlineLengths(
     regional_connectivity.RegionalConnectivity,
-    configuration_folder="features/connectivitymatrix/streamlinecounts"
+    configuration_folder="features/connectivity/regional/streamlinelengths",
+    category="connectivity"
 ):
-    """Structural connectivity matrix of streamline counts grouped by a parcellation."""
+    """Structural connectivity matrix of streamline lengths grouped by a parcellation."""
 
     def __init__(self, **kwargs):
         regional_connectivity.RegionalConnectivity.__init__(self, **kwargs)
```

### Comparing `siibra-0.4a33/siibra/features/connectivity/streamline_lengths.py` & `siibra-0.4a35/siibra/features/connectivity/streamline_counts.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ..basetypes import regional_connectivity
+from . import regional_connectivity
 
 
-class StreamlineLengths(
+class StreamlineCounts(
     regional_connectivity.RegionalConnectivity,
-    configuration_folder="features/connectivitymatrix/streamlinelengths"
+    configuration_folder="features/connectivity/regional/streamlinecounts",
+    category="connectivity"
 ):
-    """Structural connectivity matrix of streamline lengths grouped by a parcellation."""
+    """Structural connectivity matrix of streamline counts grouped by a parcellation."""
 
     def __init__(self, **kwargs):
         regional_connectivity.RegionalConnectivity.__init__(self, **kwargs)
```

### Comparing `siibra-0.4a33/siibra/features/external/__init__.py` & `siibra-0.4a35/siibra/volumes/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,12 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .ebrains import EbrainsDataFeature
 
-
-def __dir__():
-    return [
-        "EbrainsDataFeature",
-    ]
+from .parcellationmap import Map
+from .neuroglancer import NeuroglancerProvider, NeuroglancerMesh
+from .nifti import NiftiProvider
+from .gifti import GiftiSurfaceLabeling, GiftiMesh
```

### Comparing `siibra-0.4a33/siibra/features/external/ebrains.py` & `siibra-0.4a35/siibra/features/dataset/ebrains.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # simple data features anchored to a point in space
 
 from .. import anchor as _anchor
-from ..basetypes import feature
+from .. import feature
 
 from ...retrieval import datasets
 
 
-class EbrainsDataFeature(feature.Feature, datasets.EbrainsDataset):
+class EbrainsDataFeature(feature.Feature, datasets.EbrainsDataset, category='dataset'):
 
     def __init__(
         self,
         dataset_id: str,
         name: str,
         anchor: _anchor.AnatomicalAnchor,
         embargo_status: str = None,
@@ -60,15 +60,15 @@
 
     @property
     def description(self):
         return self.detail.get("description", "")
 
     @property
     def name(self):
-        return self._name_cached
+        return self._name
 
     @property
     def version_history(self):
         if self._prev is None:
             return [self.version]
         else:
             return [self.version] + self._prev.version_history
```

### Comparing `siibra-0.4a33/siibra/features/molecular/__init__.py` & `siibra-0.4a35/siibra/features/tabular/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,18 +9,14 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .receptor_density_profile import ReceptorDensityProfile
-from .receptor_density_fingerprint import ReceptorDensityFingerprint
+from .bigbrain_intensity_profile import BigBrainIntensityProfile
+from .cell_density_profile import CellDensityProfile
 from .gene_expression import GeneExpressions
-
-
-def __dir__():
-    return [
-        "ReceptorDensityProfile",
-        "ReceptorDensityFingerprint",
-        "GeneExpressions",
-    ]
+from .layerwise_bigbrain_intensities import LayerwiseBigBrainIntensities
+from .layerwise_cell_density import LayerwiseCellDensity
+from .receptor_density_fingerprint import ReceptorDensityFingerprint
+from .receptor_density_profile import ReceptorDensityProfile
```

### Comparing `siibra-0.4a33/siibra/features/molecular/gene_expression.py` & `siibra-0.4a35/siibra/features/tabular/gene_expression.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .. import anchor as _anchor
-from ..basetypes import tabular
+from . import tabular
 
 from ... import commons
 
 import pandas as pd
 from textwrap import wrap
 from typing import List
 try:
     from typing import TypedDict
 except ImportError:
     from typing_extensions import TypedDict
 
 
-class GeneExpressions(tabular.Tabular):
+class GeneExpressions(
+    tabular.Tabular,
+    category='molecular'
+):
     """
     A set gene expressions for different candidate genes
     measured inside a brain structure.
     """
 
     DESCRIPTION = """
     Gene expressions extracted from microarray data in the Allen Atlas.
```

### Comparing `siibra-0.4a33/siibra/features/molecular/receptor_density_fingerprint.py` & `siibra-0.4a35/siibra/features/tabular/receptor_density_fingerprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .. import anchor as _anchor
-from ..basetypes import tabular
+from . import tabular
 
 from ... import commons, vocabularies
 from ...retrieval import requests
 
 import pandas as pd
 import numpy as np
 from textwrap import wrap
 from typing import List
 
 
 class ReceptorDensityFingerprint(
     tabular.Tabular,
-    configuration_folder="features/fingerprints/receptor"
+    configuration_folder="features/tabular/fingerprints/receptor",
+    category='molecular'
 ):
 
     DESCRIPTION = (
         "Fingerprint of densities (in fmol/mg protein) of receptors for classical neurotransmitters "
         "obtained by means of quantitative in vitro autoradiography. The fingerprint provides average "
         "density measurments for different receptors measured in tissue samples from different subjects "
         "together with the corresponding standard deviations. "
```

### Comparing `siibra-0.4a33/siibra/features/molecular/receptor_density_profile.py` & `siibra-0.4a35/siibra/features/tabular/receptor_density_profile.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .. import anchor as _anchor
-from ..basetypes import cortical_profile
+from . import cortical_profile
 
 from ... import vocabularies
 from ...commons import create_key
 from ...retrieval import requests
 
 
-class ReceptorDensityProfile(cortical_profile.CorticalProfile, configuration_folder="features/profiles/receptor"):
+class ReceptorDensityProfile(
+    cortical_profile.CorticalProfile,
+    configuration_folder="features/tabular/corticalprofiles/receptor",
+    category='molecular'
+):
 
     DESCRIPTION = (
         "Cortical profile of densities (in fmol/mg protein) of receptors for classical neurotransmitters "
         "obtained by means of quantitative in vitro autoradiography. The profiles provide, for a "
         "single tissue sample, an exemplary density distribution for a single receptor from the pial surface "
         "to the border between layer VI and the white matter."
     )
```

### Comparing `siibra-0.4a33/siibra/livequeries/__init__.py` & `siibra-0.4a35/siibra/livequeries/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/siibra/livequeries/allen.py` & `siibra-0.4a35/siibra/livequeries/allen.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .query import LiveQuery
 
 from ..core import space as _space
 from ..features import anchor as _anchor
-from ..features.molecular.gene_expression import GeneExpressions
+from ..features.tabular.gene_expression import GeneExpressions
 from ..commons import logger, Species, MapType
 from ..locations import Point, PointSet
 from ..core.region import Region
 from ..retrieval import HttpRequest
 from ..vocabularies import GENE_NAMES
 
 from typing import Iterable, List
```

### Comparing `siibra-0.4a33/siibra/livequeries/bigbrain.py` & `siibra-0.4a35/siibra/livequeries/bigbrain.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from . import query
 
-from ..features.cellular import bigbrain_intensity_profile, layerwise_bigbrain_intensities
-
+from ..features.tabular import bigbrain_intensity_profile, layerwise_bigbrain_intensities
 from ..commons import logger
 from ..locations import point, pointset
 from ..core import space, region
 from ..retrieval import requests, cache
 
 import numpy as np
 from typing import List
@@ -154,15 +153,15 @@
 
             # compute array of layer labels for all coefficients in profiles_left
             N = matched_profiles.shape[1]
             prange = np.arange(N)
             region_labels = 7 - np.array([
                 [np.array([[(prange < T) * 1] for i, T in enumerate((b * N).astype('int'))]).squeeze().sum(0)]
                 for b in boundary_depths
-            ]).squeeze()
+            ]).reshape((-1, 200))
 
             fp = layerwise_bigbrain_intensities.LayerwiseBigBrainIntensities(
                 regionname=subregion.name,
                 means=[matched_profiles[region_labels == _].mean() for _ in range(1, 7)],
                 stds=[matched_profiles[region_labels == _].std() for _ in range(1, 7)],
             )
             assert fp.matches(subregion)  # to create an assignment result
```

### Comparing `siibra-0.4a33/siibra/livequeries/ebrains.py` & `siibra-0.4a35/siibra/livequeries/ebrains.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ..features.external import ebrains as _ebrains
+from ..features.dataset import ebrains as _ebrains
 from . import query
 
 from ..commons import logger
 from ..features import anchor as _anchor
 from ..retrieval import requests, datasets
 from ..core import parcellation, region
 
@@ -44,19 +44,14 @@
     }
 
     loader = requests.MultiSourcedRequest(
         requests=[
             requests.GitlabProxy(
                 flavour=requests.GitlabProxyEnum.PARCELLATIONREGION_V1,
             ),
-            requests.EbrainsKgQuery(
-                query_id="siibra-kg-feature-summary-0_0_4",
-                schema="parcellationregion",
-                params={"vocab": "https://schema.hbp.eu/myQuery/"},
-            )
         ]
     )
 
     parcellation_ids = None
 
     def __init__(self, **kwargs):
         query.LiveQuery.__init__(self, **kwargs)
```

### Comparing `siibra-0.4a33/siibra/livequeries/query.py` & `siibra-0.4a35/siibra/livequeries/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ..commons import logger
-from ..features.basetypes.feature import Feature
+from ..features.feature import Feature
 from ..core.concept import AtlasConcept
 
 from abc import ABC, abstractmethod
 from typing import List
 
 
 class LiveQuery(ABC):
```

### Comparing `siibra-0.4a33/siibra/locations/__init__.py` & `siibra-0.4a35/siibra/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/siibra/locations/boundingbox.py` & `siibra-0.4a35/siibra/locations/boundingbox.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/siibra/locations/location.py` & `siibra-0.4a35/siibra/locations/location.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/siibra/locations/point.py` & `siibra-0.4a35/siibra/locations/point.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,34 +21,33 @@
 from nibabel import Nifti1Image
 from urllib.parse import quote
 import re
 import numpy as np
 import json
 import numbers
 import hashlib
-from typing import Union
+from typing import Union, Tuple
 
 
 class Point(location.Location):
     """A single 3D point in reference space."""
 
     @staticmethod
-    def parse(spec, unit="mm"):
+    def parse(spec, unit="mm") -> Tuple[float, float, float]:
         """Converts a 3D coordinate specification into a 3D tuple of floats.
 
         Parameters
         ----------
-        spec : Any of str, tuple(float,float,float)
+        spec: Any of str, tuple(float,float,float)
             For string specifications, comma separation with decimal points are expected.
-        unit : str
+        unit: str
             specification of the unit (only 'mm' supported so far)
-
         Returns
         -------
-        tuple(float,float,float)
+        tuple(float, float, float)
         """
         if unit != "mm":
             raise NotImplementedError(
                 "Coordinate parsing from strings is only supported for mm specifications so far."
             )
         if isinstance(spec, str):
             pat = r"([-\d\.]*)" + unit
@@ -73,21 +72,24 @@
 
     def __init__(self, coordinatespec, space=None, sigma_mm: float = 0.0):
         """
         Construct a new 3D point set in the given reference space.
 
         Parameters
         ----------
-        coordinate : 3-tuple of int/float, or string specification
+        coordinatespec: 3-tuple of int/float, or string specification
             Coordinate in mm of the given space
-        space : reference space specification (id, object, or name)
-            The reference space
-        sigma_mm : float
-            Optional location uncertainy of the point
-            (will be interpreted as the isotropic standard deviation of location)
+        space: Space or str
+            The reference space (id, object, or name)
+        sigma_mm : float, optional
+            Location uncertainty of the point
+
+            Note
+            ----
+                Interpreted as the isotropic standard deviation of location.
         """
         location.Location.__init__(self, space)
         self.coordinate = Point.parse(coordinatespec)
         self.sigma = sigma_mm
         if isinstance(coordinatespec, Point):
             assert coordinatespec.sigma == sigma_mm
             assert coordinatespec.space == space
@@ -243,20 +245,22 @@
 
     def transform(self, affine: np.ndarray, space=None):
         """Returns a new Point obtained by transforming the
         coordinate of this one with the given affine matrix.
 
         Parameters
         ----------
-        affine : numpy 4x4 ndarray
+        affine: numpy 4x4 ndarray
             affine matrix
-        space : reference space, (str, Space, or None))
-            Target reference space which is reached after
-            applying the transform. Note that the consistency
-            of this cannot be checked and is up to the user.
+        space: str, Space, or None
+            Target reference space which is reached after applying the transform
+
+            Note
+            ----
+            The consistency of this cannot be checked and is up to the user.
         """
         from ..core.space import Space
         spaceobj = Space.get_instance(space)
         x, y, z, h = np.dot(affine, self.homogeneous)
         if h != 1:
             logger.warning(f"Homogeneous coordinate is not one: {h}")
         return self.__class__((x / h, y / h, z / h), spaceobj)
```

### Comparing `siibra-0.4a33/siibra/locations/pointset.py` & `siibra-0.4a35/siibra/locations/pointset.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/siibra/retrieval/__init__.py` & `siibra-0.4a35/siibra/retrieval/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,10 +17,10 @@
     GitlabConnector,
     OwncloudConnector,
     EbrainsHdgConnector,
     EbrainsPublicDatasetConnector,
     LocalFileRepository,
     ZipfileConnector
 )
-from .requests import HttpRequest, ZipfileRequest, EbrainsRequest, EbrainsKgQuery, SiibraHttpRequestError
+from .requests import HttpRequest, ZipfileRequest, EbrainsRequest, SiibraHttpRequestError
 from .cache import CACHE
 from .exceptions import NoSiibraConfigMirrorsAvailableException, TagNotFoundException
```

### Comparing `siibra-0.4a33/siibra/retrieval/cache.py` & `siibra-0.4a35/siibra/retrieval/cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,16 +89,22 @@
             if targetsize <= self.SIZE_GIB:
                 break
             targetsize -= st.st_size / 1024**3
 
         if index > 0:
             logger.debug(f"Removing the {index+1} oldest files to keep cache size below {targetsize:.2f} GiB.")
             for fn, st in sfiles[:index + 1]:
-                size_gib -= st.st_size / 1024**3
-                os.remove(fn)
+                if os.path.isdir(fn):
+                    import shutil
+                    size = sum(os.path.getsize(f) for f in os.listdir(fn) if os.path.isfile(f))
+                    shutil.rmtree(fn)
+                else:
+                    size = st.st_size
+                    os.remove(fn)
+                size_gib -= size / 1024**3
 
     @property
     def size(self):
         """ Return size of the cache in GiB. """
         return sum(os.path.getsize(fn) for fn in self) / 1024**3
 
     def __iter__(self):
```

### Comparing `siibra-0.4a33/siibra/retrieval/repositories.py` & `siibra-0.4a35/siibra/retrieval/repositories.py`

 * *Files 0% similar despite different names*

```diff
@@ -606,17 +606,17 @@
 
         Parameters
         ----------
         dataset_id : str
             EBRAINS dataset id of a public dataset in KG v3.
         title: str
             Part of dataset title as an alternative dataset specification (will ignore dataset_id then)
-        in_progress: bool (default:False)
+        in_progress: bool, default: False
             If true, will request datasets that are still under curation.
-            Will only work when autenticated with an appropriately privileged
+            Will only work when authenticated with an appropriately privileged
             user account.
         """
         stage = "IN_PROGRESS" if in_progress else "RELEASED"
         if title is None:
             assert dataset_id is not None
             self.dataset_id = dataset_id
             url = f"{self.base_url}/{self.QUERY_ID}/instances?databaseScope={stage}&dataset_id={dataset_id}"
```

### Comparing `siibra-0.4a33/siibra/retrieval/requests.py` & `siibra-0.4a35/siibra/retrieval/requests.py`

 * *Files 7% similar despite different names*

```diff
@@ -267,39 +267,63 @@
         if "device_authorization_endpoint" in json_resp:
             logger.debug(f"device_authorization_endpoint exists in .well-known/openid-configuration. setting _IAM_DEVICE_ENDPOINT to {json_resp.get('device_authorization_endpoint')}")
             cls._IAM_DEVICE_ENDPOINT = json_resp.get("device_authorization_endpoint")
         else:
             logger.warn("expected device_authorization_endpoint in .well-known/openid-configuration, but was not present")
 
     @classmethod
-    def fetch_token(cls):
-        """Fetch an EBRAINS token using commandline-supplied username/password
+    def fetch_token(cls, **kwargs):
+        """
+        Fetch an EBRAINS token using commandline-supplied username/password
         using the data proxy endpoint.
+        
         :ref:`Details on how to access EBRAINS are here.<accessEBRAINS>`
         """
-        cls.device_flow()
+        cls.device_flow(**kwargs)
         
     @classmethod
-    def device_flow(cls):
+    def device_flow(cls, **kwargs):
         if all([
             not sys.__stdout__.isatty(),  # if is tty, do not raise
             not any(k in ['JPY_INTERRUPT_EVENT', "JPY_PARENT_PID"] for k in os.environ),  # if is notebook environment, do not raise
             not os.getenv("SIIBRA_ENABLE_DEVICE_FLOW"),  # if explicitly enabled by env var, do not raise
         ]):
             raise EbrainsAuthenticationError(
                 "sys.stdout is not tty, SIIBRA_ENABLE_DEVICE_FLOW is not set,"
                 "and not running in a notebook. Are you running in batch mode?"
             )
 
         cls.init_oidc()
+
+        def get_scopes() -> str:
+            scopes = kwargs.get("scopes")
+            if not scopes:
+                return None
+            if not isinstance(scopes, list):
+                logger.warn(f"scopes needs to be a list, is but is not... skipping")
+                return None
+            if not all(isinstance(scope, str) for scope in scopes):
+                logger.warn(f"scopes needs to be all str, but is not")
+                return None
+            if len(scopes) == 0:
+                logger.warn(f'provided empty list as scopes... skipping')
+                return None
+            return "+".join(scopes)
+        
+        scopes = get_scopes()
+        
+        data = {
+            'client_id': cls._IAM_DEVICE_FLOW_CLIENTID
+        }
+
+        if scopes:
+            data['scopes'] = scopes
         resp = requests.post(
             url=cls._IAM_DEVICE_ENDPOINT,
-            data={
-                'client_id': cls._IAM_DEVICE_FLOW_CLIENTID
-            }
+            data=data
         )
         resp.raise_for_status()
         resp_json = resp.json()
         logger.debug("device flow, request full json:", resp_json)
 
         assert "verification_uri_complete" in resp_json
         assert "device_code" in resp_json
@@ -416,63 +440,14 @@
 
     def get(self):
         """Evaluate KG Token is evaluated only on execution of the request."""
         self.kwargs = {"headers": self.auth_headers, "params": self.params}
         return super().get()
 
 
-class EbrainsKgQuery(EbrainsRequest):
-    """Request outputs from a knowledge graph query."""
-
-    server = "https://kg.humanbrainproject.eu"
-    org = "minds"
-    domain = "core"
-    version = "v1.0.0"
-
-    SC_MESSAGES = {
-        401: "The provided EBRAINS authentication token is not valid",
-        403: "No permission to access the given query",
-        404: "Query with this id not found",
-    }
-
-    def __init__(self, query_id, instance_id=None, schema="dataset", params={}):
-        inst_tail = "/" + instance_id if instance_id is not None else ""
-        self.schema = schema
-        url = "{}/query/{}/{}/{}/{}/{}/instances{}?databaseScope=RELEASED".format(
-            self.server,
-            self.org,
-            self.domain,
-            self.schema,
-            self.version,
-            query_id,
-            inst_tail,
-        )
-        EbrainsRequest.__init__(
-            self,
-            url,
-            decoder=DECODERS[".json"],
-            params=params,
-            msg_if_not_cached=f"Executing EBRAINS KG query {query_id}{inst_tail}",
-        )
-
-    def get(self):
-        try:
-            result = EbrainsRequest.get(self)
-        except SiibraHttpRequestError as e:
-            if e.status_code in self.SC_MESSAGES:
-                raise RuntimeError(self.SC_MESSAGES[e.status_code])
-            else:
-                raise RuntimeError(
-                    f"Could not process HTTP request (status code: "
-                    f"{e.status_code}). Message was: {e.msg}"
-                    f"URL was: {e.url}"
-                )
-        return result
-
-
 def try_all_connectors():
     def outer(fn):
         @wraps(fn)
         def inner(self: 'GitlabProxyEnum', *args, **kwargs):
             exceptions = []
             for connector in self.connectors:
                 try:
@@ -511,16 +486,16 @@
         assert connector
         return connector.get(filename, "", decode_func)
 
 
 class GitlabProxy(HttpRequest):
 
     folder_dict = {
-        GitlabProxyEnum.DATASET_V1: "ebrainsquery/v1/datasets",
-        GitlabProxyEnum.DATASET_V3: "ebrainsquery/v3/datasets",
+        GitlabProxyEnum.DATASET_V1: "ebrainsquery/v1/dataset",
+        GitlabProxyEnum.DATASET_V3: "ebrainsquery/v3/Dataset",
         GitlabProxyEnum.PARCELLATIONREGION_V1: "ebrainsquery/v1/parcellationregions",
     }
 
     def __init__(
         self,
         flavour: GitlabProxyEnum,
         instance_id=None,
```

### Comparing `siibra-0.4a33/siibra/vocabularies/__init__.py` & `siibra-0.4a35/siibra/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/siibra/vocabularies/gene_names.json` & `siibra-0.4a35/siibra/vocabularies/gene_names.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/siibra/vocabularies/receptor_symbols.json` & `siibra-0.4a35/siibra/vocabularies/receptor_symbols.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/siibra/vocabularies/region_aliases.json` & `siibra-0.4a35/siibra/vocabularies/region_aliases.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a33/siibra/volumes/gifti.py` & `siibra-0.4a35/siibra/volumes/gifti.py`

 * *Files 22% similar despite different names*

```diff
@@ -51,20 +51,32 @@
 
     @property
     def fragments(self):
         return [k for k in self._loaders if k is not None]
 
     def fetch(self, fragment: str = None, **kwargs):
         """
-        Returns the mesh as a dictionary with two numpy arrays: An Nx3 array of vertex coordinates,
-        and an Mx3 array of face definitions using row indices of the vertex array.
+        Returns the mesh as a dictionary with two numpy arrays.
 
-        A fragment name can be specified to choose from multiple fragments.
-        If not specified, multiple fragments will be merged into one mesh. In such a case,
-        the verts and faces arrays of different fragments are appended to one another.
+        Parameters
+        ----------
+        fragment: str, default: None
+            A fragment name can be specified to choose from multiple fragments.
+
+            Note
+            ----
+            If not specified, multiple fragments will be merged into one mesh.
+            In such a case, the verts and faces arrays of different fragments
+            are appended to one another.
+
+        Returns
+        -------
+        dict
+            - 'verts': An Nx3 array of vertex coordinates,
+            - 'faces': an Mx3 array of face definitions using row indices of the vertex array
         """
         for arg in ["resolution_mm", "voi"]:
             if kwargs.get(arg):
                 raise NotImplementedError(f"Parameter {arg} ignored by {self.__class__}.")
 
         fragments_included = []
         meshes = []
@@ -89,19 +101,22 @@
 
     @property
     def variants(self):
         return list(self._loaders.keys())
 
     def fetch_iter(self):
         """
-        Iterator returning all submeshes, each represented as a dictionary
-        with elements
-        - 'verts': An Nx3 array of vertex coordinates,
-        - 'faces': an Mx3 array of face definitions using row indices of the vertex array
-        - 'name': Name of the of the mesh variant
+        Iterator returning all submeshes
+
+        Returns
+        -------
+        dict
+            - 'verts': An Nx3 array of vertex coordinates,
+            - 'faces': an Mx3 array of face definitions using row indices of the vertex array
+            - 'name': Name of the of the mesh variant
         """
         return (self.fetch(v) for v in self.variants)
 
 
 class GiftiSurfaceLabeling(volume.VolumeProvider, srctype="gii-label"):
     """
     A mesh labeling, specified by a gifti file.
```

### Comparing `siibra-0.4a33/siibra/volumes/neuroglancer.py` & `siibra-0.4a35/siibra/volumes/neuroglancer.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,22 +54,22 @@
         **kwargs
     ) -> nib.Nifti1Image:
         """
         Fetch 3D image data from neuroglancer volume.
 
         Parameters
         ----------
-        fragment: str
-            Optional name of a fragment volume to fetch, if any.
-            For example, some volumes are split into left and right hemisphere fragments.
-            see :func:`~siibra.volumes.Volume.fragments`
+        fragment: str, optional
+            The name of a fragment volume to fetch, if any. For example,
+            some volumes are split into left and right hemisphere fragments.
+            See :func:`~siibra.volumes.Volume.fragments`
         resolution_mm: float
-            Specify the resolugion
-        voi : BoundingBox
-            optional specification of a volume of interst to fetch.
+            Specify the resolution
+        voi: BoundingBox
+            optional specification of a volume of interest to fetch.
         """
 
         result = None
 
         if 'index' in kwargs:
             index = kwargs.pop('index')
             if fragment is not None:
@@ -531,17 +531,33 @@
         vertices, triangles = affine_transform_mesh(vertices_vox, triangles_vox, transform_nm)
         vertices /= 1e6
         return {'verts': vertices, 'faces': triangles}
 
     def fetch(self, label: int, fragment: str):
         """
         Fetches a particular mesh. Each mesh is a dictionary with keys:
-
-        - verts: an Nx3 array of coordinates (in nanometer)
-        - faces: an MX3 array containing connection data of vertices
+        
+        Parameters
+        ----------
+        label: int
+            Label of the volume
+        fragment: str, default: None
+            A fragment name can be specified to choose from multiple fragments.
+
+            Note
+            ----
+            If not specified, multiple fragments will be merged into one mesh.
+            In such a case, the verts and faces arrays of different fragments
+            are appended to one another.
+        Returns
+        -------
+        dict
+            - 'verts': An Nx3 array of vertex coordinates (in nanometer)
+            - 'faces': an MX3 array containing connection data of vertices
+            - 'name': Name of the of the mesh variant
         """
 
         # extract fragment information for the requested mesh
         fragment_infos = self._get_fragment_info(label)
 
         if fragment is None:
```

### Comparing `siibra-0.4a33/siibra/volumes/nifti.py` & `siibra-0.4a35/siibra/volumes/nifti.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,16 +129,16 @@
         Parameters
         ----------
         fragment: str
             Optional name of a fragment volume to fetch, if any.
             For example, some volumes are split into left and right hemisphere fragments.
             see :func:`~siibra.volumes.Volume.fragments`
         voi : BoundingBox
-            optional specification of a volume of interst to fetch.
-        label: int or None
+            optional specification of a volume of interest to fetch.
+        label: int, default: None
             Optional: a label index can be provided. Then the mask of the
             3D volume will be returned, where voxels matching this label
             are marked as "1".
         """
 
         result = None
         if len(self._img_loaders) > 1:
@@ -198,22 +198,22 @@
     def is_float(self):
         return self.image.dataobj.dtype.kind == "f"
 
     def find_peaks(self, min_distance_mm=5):
         """
         Find peaks in the image data.
 
-        Arguments:
+        Parameters
         ----------
         min_distance_mm : float
             Minimum distance between peaks in mm
 
         Returns:
         --------
-        peaks: PointSet
+        PointSet
         """
 
         from skimage.feature.peak import peak_local_max
         from ..commons import affine_scaling
 
         img = self.fetch()
         dist = int(min_distance_mm / affine_scaling(img.affine) + 0.5)
```

### Comparing `siibra-0.4a33/siibra/volumes/parcellationmap.py` & `siibra-0.4a35/siibra/volumes/parcellationmap.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Provides spatial representations for parcellations and regions."""
 
 from . import volume as _volume, nifti
 from .. import logger, QUIET
-from ..commons import MapIndex, MapType, compare_maps, clear_name, create_key, create_gaussian_kernel, Species
+from ..commons import (
+    MapIndex,
+    MapType,
+    compare_maps,
+    iterate_connected_components,
+    clear_name,
+    create_key,
+    create_gaussian_kernel,
+    Species
+)
 from ..core import concept, space, parcellation, region as _region
 from ..locations import point, pointset
 from ..retrieval import requests
 
 import numpy as np
 from tqdm import tqdm
 from typing import Union, Dict, List, TYPE_CHECKING, Iterable
@@ -42,14 +51,18 @@
     pass
 
 
 class ConflictingArgumentException(ValueError):
     pass
 
 
+class NonUniqueIndexError(RuntimeError):
+    pass
+
+
 class Map(concept.AtlasConcept, configuration_folder="maps"):
 
     def __init__(
         self,
         identifier: str,
         name: str,
         space_spec: dict,
@@ -63,40 +76,40 @@
         datasets: list = [],
     ):
         """
         Constructs a new parcellation object.
 
         Parameters
         ----------
-        identifier : str
+        identifier: str
             Unique identifier of the parcellation
-        name : str
+        name: str
             Human-readable name of the parcellation
         space_spec: dict
             Specification of the space (use @id or name fields)
         parcellation_spec: str
             Specification of the parcellation (use @id or name fields)
         indices: dict
             Dictionary of indices for the brain regions.
             Keys are exact region names.
             Per region name, a list of dictionaries with fields "volume" and "label" is expected,
             where "volume" points to the index of the Volume object where this region is mapped,
             and optional "label" is the voxel label for that region.
-            For contiuous / probability maps, the "label" can be null or omitted.
+            For continuous / probability maps, the "label" can be null or omitted.
             For single-volume labelled maps, the "volume" can be null or omitted.
-        volumes: list of Volume
+        volumes: list[Volume]
             parcellation volumes
-        shortname: str
-            Shortform of human-readable name (optional)
-        description: str
+        shortname: str, optional
+            Shortform of human-readable name
+        description: str, optional
             Textual description of the parcellation
-        modality  :  str or None
+        modality: str, default: None
             Specification of the modality used for creating the parcellation
         publications: list
-            List of ssociated publications, each a dictionary with "doi" and/or "citation" fields
+            List of associated publications, each a dictionary with "doi" and/or "citation" fields
         datasets : list
             datasets associated with this concept
         """
         concept.AtlasConcept.__init__(
             self,
             identifier=identifier,
             name=name,
@@ -151,36 +164,61 @@
         # lazy implementation
         if self._species_cached is None:
             self._species_cached = self.space.species
         return self.space._species_cached
 
     def get_index(self, region: Union[str, "Region"]):
         """
-        Returns the unique index corresponding to the specified region,
-        assuming that the specification matches one unique region
-        defined in this parcellation map.
-        If not unique, or not defined, an exception will be thrown.
-        See find_indices() for a less strict search returning all matches.
+        Returns the unique index corresponding to the specified region.
+
+        Tip
+        ----
+        Use find_indices() method for a less strict search returning all matches.
+
+        Parameters
+        ----------
+        region: str or Region
+
+        Returns
+        -------
+        MapIndex
+
+        Raises
+        ------
+        NonUniqueIndexError
+            If not unique or not defined in this parcellation map.
         """
         matches = self.find_indices(region)
         if len(matches) > 1:
-            raise RuntimeError(
+            raise NonUniqueIndexError(
                 f"The specification '{region}' matches multiple mapped "
                 f"structures in {str(self)}: {list(matches.values())}"
             )
         elif len(matches) == 0:
-            raise RuntimeError(
+            raise NonUniqueIndexError(
                 f"The specification '{region}' does not match to any structure mapped in {self}"
             )
         else:
             return next(iter(matches))
 
     def find_indices(self, region: Union[str, "Region"]):
-        """ Returns the volume/label indices in this map
-        which match the given region specification"""
+        """
+        Returns the volume/label indices in this map which match the given
+        region specification.
+
+        Parameters
+        ----------
+        region: str or Region
+
+        Returns
+        -------
+        dict
+            - keys: MapIndex
+            - values: region name
+        """
         if region in self._indices:
             return {
                 idx: region
                 for idx in self._indices[region]
             }
         regionname = region.name if isinstance(region, _region.Region) else region
         matched_region_names = set(_.name for _ in (self.parcellation.find(regionname)))
@@ -189,16 +227,33 @@
             logger.warn(f"Region {regionname} not defined in {self}")
         return {
             idx: regionname
             for regionname in matches
             for idx in self._indices[regionname]
         }
 
-    def get_region(self, label: int = None, volume: int = None, index: MapIndex = None):
-        """ Returns the region mapped by the given index, if any. """
+    def get_region(self, label: int = None, volume: int = 0, index: MapIndex = None):
+        """
+        Returns the region mapped by the given index, if any.
+
+        Tip
+        ----
+        Use get_index() or find_indices() methods to obtain the MapIndex.
+
+        Parameters
+        ----------
+        label: int, default: None
+        volume: int, default: 0
+        index: MapIndex, default: None
+
+        Returns
+        -------
+        Region
+            A region object defined in the parcellation map.
+        """
         if index is None:
             index = MapIndex(volume, label)
         matches = [
             regionname
             for regionname, indexlist in self._indices.items()
             if index in indexlist
         ]
@@ -228,16 +283,16 @@
             f"{self.name} from {self._parcellation_spec}"
         )
         return None
 
     @property
     def labels(self):
         """
-        The set of all label indices defined in this map,
-        including "None" if not defined for one or more regions.
+        The set of all label indices defined in this map, including "None" if
+        not defined for one or more regions.
         """
         return {d.label for v in self._indices.values() for d in v}
 
     @property
     def maptype(self) -> MapType:
         if all(isinstance(_, int) for _ in self.labels):
             return MapType.LABELLED
@@ -261,34 +316,49 @@
         *,
         index: MapIndex = None,
         region: Union[str, "Region"] = None,
         **kwargs
     ):
         """
         Fetches one particular volume of this parcellation map.
+
         If there's only one volume, this is the default, otherwise further
-        specication is requested:
+        specification is requested:
         - the volume index,
         - the MapIndex (which results in a regional map being returned)
 
-        You might also consider fetch_iter() to iterate the volumes, or compress()
-        to produce a single-volume parcellation map.
+        You might also consider fetch_iter() to iterate the volumes, or
+        compress() to produce a single-volume parcellation map.
 
         Parameters
         ----------
-        region_or_index: Union[str, Region, MapIndex]
+        region_or_index: str, Region, MapIndex
             Lazy match the specification.
         index: MapIndex
             Explicit specification of the map index, typically resulting
             in a regional map (mask or statistical map) to be returned.
             Note that supplying 'region' will result in retrieving the map index of that region
             automatically.
-        region: Union[str, Region]
+        region: str, Region
             Specification of a region name, resulting in a regional map
             (mask or statistical map) to be returned.
+        **kwargs
+            - resolution_mm: resolution in millimeters
+            - format: the format of the volume, like "mesh" or "nii"
+            - voi: a BoundingBox of interest
+
+
+            Note
+            ----
+            Not all keyword arguments are supported for volume formats. Format
+            is restricted by available formats (check formats property).
+
+        Returns
+        -------
+        An image or mesh
         """
         try:
             length = len([arg for arg in [region_or_index, region, index] if arg is not None])
             assert length == 1
         except AssertionError:
             if length > 1:
                 raise ExcessiveArgumentException("One and only one of region_or_index, region, index can be defined for fetch")
@@ -342,15 +412,16 @@
         if result is None:
             raise RuntimeError(f"Error fetching {mapindex} from {self} as {kwargs['format']}.")
         return result
 
     def fetch_iter(self, **kwargs):
         """
         Returns an iterator to fetch all mapped volumes sequentially.
-        All arguments are passed on to func:`~siibra.Map.fetch`
+
+        All arguments are passed on to function Map.fetch().
         """
         fragment = kwargs.pop('fragment') if 'fragment' in kwargs else None
         return (
             self.fetch(
                 index=MapIndex(volume=i, label=None, fragment=fragment), **kwargs
             )
             for i in range(len(self))
@@ -399,17 +470,25 @@
         return self._affine_cached
 
     def __iter__(self):
         return self.fetch_iter()
 
     def compress(self, **kwargs):
         """
-        Converts this map into a labelled 3D parcellation map, obtained
-        by taking the voxelwise maximum across the mapped volumes, and
-        re-labelling regions sequentially.
+        Converts this map into a labelled 3D parcellation map, obtained by
+        taking the voxelwise maximum across the mapped volumes and fragments,
+        and re-labelling regions sequentially.
+
+        Paramaters
+        ----------
+        **kwargs: Takes the fetch arguments of its space's template.
+
+        Returns
+        -------
+        parcellationmap.Map
         """
         if len(self.volumes) == 1 and (self.fragments is None):
             raise RuntimeError("The map cannot be merged since there are no multiple volumes or fragments.")
 
         # initialize empty volume according to the template
         template = self.space.get_template().fetch(**kwargs)
         result_data = np.zeros_like(np.asanyarray(template.dataobj))
@@ -470,14 +549,19 @@
                 )
             ]
         )
 
     def compute_centroids(self) -> Dict[str, point.Point]:
         """
         Compute a dictionary of the centroids of all regions in this map.
+
+        Returns
+        -------
+        Dict[str, point.Point]
+            Region names as keys and computed centroids as items.
         """
         centroids = {}
         # list of regions sorted by mapindex
         regions = sorted(self._indices.items(), key=lambda v: min(_.volume for _ in v[1]))
         current_vol_index = MapIndex(volume=0)
         maparr = None
         for regionname, indexlist in tqdm(regions, unit="regions", desc="Computing centroids"):
@@ -533,25 +617,22 @@
 
         return Nifti1Image(result, affine)
 
     def get_colormap(self, region_specs: Iterable = None):
         """
         Generate a matplotlib colormap from known rgb values of label indices.
 
-        The probability distribution is approximated from the region mask
-        based on the squared distance transform.
-
         Parameters
         ----------
-        region_specs: An iterable selection of regions
+        region_specs: iterable(regions), optional
             Optional parameter to only color the desired regions.
 
-        Return
-        ------
-        samples : PointSet in physcial coordinates corresponding to this parcellationmap.
+        Returns
+        -------
+        ListedColormap
         """
         from matplotlib.colors import ListedColormap
         import numpy as np
 
         colors = {}
         if region_specs is not None:
             include_region_names = {
@@ -579,26 +660,29 @@
             ]
         ) / [255, 255, 255, 1]
         return ListedColormap(pallette)
 
     def sample_locations(self, regionspec, numpoints: int):
         """ Sample 3D locations inside a given region.
 
-        The probability distribution is approximated from the region mask
-        based on the squared distance transform.
+        The probability distribution is approximated from the region mask based
+        on the squared distance transform.
 
-        regionspec: valid region specification
+        Parameters
+        ----------
+        regionspec: Region or str
             Region to be used
         numpoints: int
             Number of samples to draw
 
-        Return
-        ------
-        samples : PointSet in physcial coordinates corresponding to this parcellationmap.
-
+        Returns
+        -------
+        PointSet
+            Sample points in physcial coordinates corresponding to this
+            parcellationmap
         """
         index = self.get_index(regionspec)
         mask = self.fetch(index=index)
         arr = np.asanyarray(mask.dataobj)
         if arr.dtype.char in np.typecodes['AllInteger']:
             # a binary mask - use distance transform to get sampling weights
             W = distance_transform_edt(np.asanyarray(mask.dataobj))**2
@@ -608,31 +692,22 @@
         p = (W / W.sum()).ravel()
         XYZ_ = np.array(
             np.unravel_index(np.random.choice(len(p), numpoints, p=p), W.shape)
         ).T
         XYZ = np.dot(mask.affine, np.c_[XYZ_, np.ones(numpoints)].T)[:3, :].T
         return pointset.PointSet(XYZ, space=self.space)
 
-    @staticmethod
-    def iterate_connected_components(img: Nifti1Image):
-        """
-        Provide an iterator over masks of connected components in the given image.
+    def to_sparse(self):
         """
-        from skimage import measure
-        imgdata = np.asanyarray(img.dataobj).squeeze()
-        components = measure.label(imgdata > 0)
-        component_labels = np.unique(components)
-        assert component_labels[0] == 0
-        return (
-            (label, Nifti1Image((components == label).astype('uint8'), img.affine))
-            for label in component_labels[1:]
-        )
+        Creates a SparseMap object from this parcellation map object.
 
-    def to_sparse(self):
-        """ Creates a sparse parcellation map from this object. """
+        Returns
+        -------
+        SparseMap
+        """
         from .sparsemap import SparseMap
         indices = {
             regionname: [
                 {'volume': idx.volume, 'label': idx.label, 'fragment': idx.fragment}
                 for idx in indexlist
             ]
             for regionname, indexlist in self._indices.items()
@@ -682,105 +757,122 @@
         """Assign an input image to brain regions.
 
         The input image is assumed to be defined in the same coordinate space
         as this parcellation map.
 
         Parameters
         ----------
-        item: Point, PointSet, or Nifti1Image
-            A spatial object defined in the same physical reference space as this
-            parcellation map, which could be a point, set of points, or image.
-            If it is an image, it will be resampled to the same voxel space if its affine
-            transforation differs from that of the parcellation map.
-            Resampling will use linear interpolation for float image types,
-            otherwise nearest neighbor.
+        item: Point, PointSet, Nifti1Image
+            A spatial object defined in the same physical reference space as
+            this parcellation map, which could be a point, set of points, or
+            image. If it is an image, it will be resampled to the same voxel
+            space if its affine transformation differs from that of the
+            parcellation map. Resampling will use linear interpolation for float
+            image types, otherwise nearest neighbor.
         minsize_voxel: int, default: 1
             Minimum voxel size of image components to be taken into account.
         lower_threshold: float, default: 0
-            Lower threshold on values in the statistical map. Values smaller than
-            this threshold will be excluded from the assignment computation.
+            Lower threshold on values in the statistical map. Values smaller
+            than this threshold will be excluded from the assignment computation.
 
-        Return
-        ------
-        assignments : pandas Dataframe
-            A table of associated regions and their scores per component found in the input image,
-            or per coordinate provived.
-            The scores are:
-                - Value: Maximum value of the voxels in the map covered by an input coordinate or
-                  input image signal component.
-                - Pearson correlation coefficient between the brain region map and an input image signal
-                  component (NaN for exact coordinates)
-                - "Contains": Percentage of the brain region map contained in an input image signal component,
-                  measured from their binarized masks as the ratio between the volume of their interesection
-                  and the volume of the brain region (NaN for exact coordinates)
-                - "Contained"": Percentage of an input image signal component contained in the brain region map,
-                  measured from their binary masks as the ratio between the volume of their interesection
-                  and the volume of the input image signal component (NaN for exact coordinates)
-        components: Nifti1Image, or None
-            If the input was an image, this is a labelled volume mapping the detected components
-            in the input image, where pixel values correspond to the "component" column of the
-            assignment table. If the input was a Point or PointSet, this is None.
+        Returns
+        -------
+        assignments: pandas.DataFrame
+            A table of associated regions and their scores per component found
+            in the input image, or per coordinate provided. The scores are:
+
+                - Value: Maximum value of the voxels in the map covered by an
+                input coordinate or input image signal component.
+                - Pearson correlation coefficient between the brain region map
+                and an input image signal component (NaN for exact coordinates)
+                - Contains: Percentage of the brain region map contained in an
+                input image signal component, measured from their binarized
+                masks as the ratio between the volume of their intersection
+                and the volume of the brain region (NaN for exact coordinates)
+                - Contained: Percentage of an input image signal component
+                contained in the brain region map, measured from their binary
+                masks as the ratio between the volume of their intersection and
+                the volume of the input image signal component (NaN for exact
+                coordinates)
+        components: Nifti1Image or None
+            If the input was an image, this is a labelled volume mapping the
+            detected components in the input image, where pixel values correspond
+            to the "component" column of the assignment table. If the input was
+            a Point or PointSet, returns None.
         """
 
         if isinstance(item, point.Point):
             assignments = self._assign_points(pointset.PointSet([item], item.space, sigma_mm=item.sigma), lower_threshold)
         elif isinstance(item, pointset.PointSet):
             assignments = self._assign_points(item, lower_threshold)
         elif isinstance(item, Nifti1Image):
             assignments = self._assign_image(item, minsize_voxel, lower_threshold)
         else:
             raise RuntimeError(
                 f"Items of type {item.__class__.__name__} cannot be used for region assignment."
             )
 
         # format assignments as pandas dataframe
+        columns = [
+            "input structure",
+            "centroid",
+            "volume",
+            "fragment",
+            "region",
+            "correlation",
+            "intersection over union",
+            "map value",
+            "map weighted mean",
+            "map containedness",
+            "input weighted mean",
+            "input containedness"
+        ]
         if len(assignments) == 0:
-            df = pd.DataFrame(
-                columns=["Structure", "Centroid", "Volume", "Fragment", "Region", "Value", "Correlation", "IoU", "Contains", "Contained"]
-            )
+            df = pd.DataFrame(columns=columns)
         else:
-            result = np.array(assignments, dtype=object)
-            ind = np.lexsort((-result[:, -1].astype('float'), result[:, 0].astype('float')))
 
             # determine the unique set of observed indices in order to do region lookups
             # only once for each map index occuring in the point list
-            labelled = self.is_labelled  # avoid calling this in a long loop
-
-            def format_label(label):
-                return int(label) if (label != 'nan') and (labelled) else None
-
-            observed_indices = {
-                (v, f, format_label(l))
-                for _, _, v, f, l, _, _, _, _ in result[ind]
+            labelled = self.is_labelled  # avoid calling this in a loop
+            observed_indices = {  # unique set of observed map indices. NOTE: len(observed_indices) << len(assignments)
+                (
+                    a.get('volume'),
+                    a.get('fragment'),
+                    a.get('map value') if labelled else None
+                )
+                for a in assignments
             }
-            region_lut = {
+            region_lut = {  # lookup table of observed region objects
                 (v, f, l): self.get_region(
-                    index=MapIndex(volume=int(v), label=format_label(l), fragment=f)
+                    index=MapIndex(
+                        volume=int(v),
+                        label=l if l is None else int(l),
+                        fragment=f
+                    )
                 )
                 for v, f, l in observed_indices
             }
-            regions = [
-                region_lut[v, f, format_label(l)] for _, _, v, f, l, _, _, _, _ in result[ind]
-            ]
-            df = pd.DataFrame(
-                {
-                    "Structure": result[ind, 0].astype("int"),
-                    "Centroid": result[ind, 1],
-                    "Volume": result[ind, 2].astype("int"),
-                    "Fragment": result[ind, 3],
-                    "Region": regions,
-                    "Value": result[ind, 4],
-                    "Correlation": result[ind, 8],
-                    "IoU": result[ind, 5],
-                    "Contains": result[ind, 7],
-                    "Contained": result[ind, 6],
-                }
-            )
 
-        return df.convert_dtypes()  # convert will guess numeric column types
+            for a in assignments:
+                a["region"] = region_lut[
+                    a.get('volume'),
+                    a.get('fragment'),
+                    a.get('map value') if labelled else None
+                ]
+                a['map containedness'] = a.pop('intersection over first', None)
+                a['input containedness'] = a.pop('intersection over second', None)
+                a['map weighted mean'] = a.pop('weighted mean of first', None)
+                a['input weighted mean'] = a.pop('weighted mean of second', None)
+            df = pd.DataFrame(assignments)
+
+        return (
+            df
+            .convert_dtypes()  # convert will guess numeric column types
+            .reindex(columns=columns)
+        )
 
     def _assign_points(self, points, lower_threshold: float):
         """
         assign a PointSet to this parcellation map.
 
         Parameters:
         -----------
@@ -808,15 +900,21 @@
             if sigma_vox < 3:
                 pts_warped = points.warp(self.space.id)
                 X, Y, Z = (np.dot(phys2vox, pts_warped.homogeneous.T) + 0.5).astype("int")[:3]
                 for pointindex, vol, frag, value in self._read_voxel(X, Y, Z):
                     if value > lower_threshold:
                         position = pts_warped[pointindex].coordinate
                         assignments.append(
-                            [pointindex, tuple(np.array(position).round(2)), vol, frag, value, np.nan, np.nan, np.nan, np.nan]
+                            {
+                                "input structure": pointindex,
+                                "centroid": tuple(np.array(position).round(2)),
+                                "volume": vol,
+                                "fragment": frag,
+                                "map value": value
+                            }
                         )
                 return assignments
 
         # if we get here, we need to handle each point independently.
         # This is much slower but more precise in dealing with the uncertainties
         # of the coordinates.
         for pointindex, pt in tqdm(
@@ -829,35 +927,38 @@
                 N = len(self)
                 logger.debug(f"Assigning coordinate {tuple(pt)} to {N} maps")
                 x, y, z = (np.dot(phys2vox, pt.homogeneous) + 0.5).astype("int")[:3]
                 values = self._read_voxel(x, y, z)
                 for _, vol, frag, value in values:
                     if value > lower_threshold:
                         assignments.append(
-                            [pointindex, tuple(pt), vol, frag, value, np.nan, np.nan, np.nan, np.nan]
+                            {
+                                "input structure": pointindex,
+                                "centroid": tuple(pt),
+                                "volume": vol,
+                                "fragment": frag,
+                                "map value": value
+                            }
                         )
             else:
                 logger.info(
                     f"Assigning uncertain coordinate {tuple(pt)} to {len(self)} maps."
                 )
                 kernel = create_gaussian_kernel(sigma_vox, 3)
                 r = int(kernel.shape[0] / 2)  # effective radius
                 xyz_vox = (np.dot(phys2vox, pt.homogeneous) + 0.5).astype("int")
                 shift = np.identity(4)
                 shift[:3, -1] = xyz_vox[:3] - r
                 # build niftiimage with the Gaussian blob,
                 # then recurse into this method with the image input
                 W = Nifti1Image(dataobj=kernel, affine=np.dot(self.affine, shift))
-                T = self.assign(W, lower_threshold=lower_threshold)
-                assignments.extend(
-                    [
-                        [pointindex, tuple(pt), volume, fragment, value, iou, contained, contains, rho]
-                        for (_, _, volume, fragment, _, value, rho, iou, contains, contained) in T.values
-                    ]
-                )
+                for entry in self.assign(W, lower_threshold=lower_threshold).T.to_dict().values():
+                    entry["input structure"] = pointindex
+                    entry["centroid"] = tuple(pt)
+                    assignments.append(entry)
         return assignments
 
     def _assign_image(self, queryimg: Nifti1Image, minsize_voxel: int, lower_threshold: float):
         """
         Assign an image volume to this parcellation map.
 
         Parameters:
@@ -896,33 +997,29 @@
             for frag in self.fragments or {None}:
                 for vol, vol_img in progress(
                     enumerate(self.fetch_iter(fragment=frag)),
                     N=len(self),
                     desc=f"Assigning to {len(self)} volumes"
                 ):
                     queryimg_res = resample(queryimg, vol_img.affine, vol_img.shape)
-                    for mode, maskimg in Map.iterate_connected_components(queryimg_res):
+                    for mode, maskimg in iterate_connected_components(queryimg_res):
                         vol_data = np.asanyarray(vol_img.dataobj)
                         position = np.array(np.where(maskimg.get_fdata())).T.mean(0)
                         labels = {v.label for L in self._indices.values() for v in L if v.volume == vol}
                         for label in progress(
                             labels,
                             desc=f"Assigning to {len(labels)} labelled structures"
                         ):
                             targetimg = vol_img if label is None \
                                 else Nifti1Image((vol_data == label).astype('uint8'), vol_img.affine)
                             scores = compare_maps(maskimg, targetimg)
-                            if scores["IoU"] > 0:
-                                assignments.append(
-                                    [
-                                        mode,
-                                        tuple(position.round(2)),
-                                        vol,
-                                        frag,
-                                        label,
-                                        scores["IoU"],
-                                        scores["contained"],
-                                        scores["contains"],
-                                        scores["correlation"]]
-                                )
+                            if scores["intersection over union"] > 0:
+                                info = {
+                                    "input structure": mode,
+                                    "centroid": tuple(position.round(2)),
+                                    "volume": vol,
+                                    "fragment": frag,
+                                    "map value": label
+                                }
+                                assignments.append(dict(**info, **scores))
 
         return assignments
```

### Comparing `siibra-0.4a33/siibra/volumes/sparsemap.py` & `siibra-0.4a35/siibra/volumes/sparsemap.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Represents lists of probabilistic brain region maps."""
 from . import parcellationmap, volume as _volume
 
-from ..commons import MapIndex, logger
+from ..commons import MapIndex, logger, iterate_connected_components
 from ..locations import boundingbox
 from ..retrieval import cache
 
 from os import path
 import gzip
 from typing import Dict, Union, TYPE_CHECKING
 from nilearn import image
@@ -107,16 +107,18 @@
         # with the given index, together with their corresponding values v.
         assert volume in range(self.num_volumes)
         x, y, z = [v.squeeze() for v in np.split(self.coords(volume), 3)]
         v = [self.probs[i][volume] for i in self.voxels[x, y, z]]
         return x, y, z, v
 
     def to_cache(self, prefix: str):
-        """ Serialize this index to the cache,
-        using the given prefix for the cache filenames. """
+        """
+        Serialize this index to the cache, using the given prefix for the cache
+        filenames.
+        """
         probsfile = cache.CACHE.build_filename(f"{prefix}", suffix="probs.txt.gz")
         bboxfile = cache.CACHE.build_filename(f"{prefix}", suffix="bboxes.txt.gz")
         voxelfile = cache.CACHE.build_filename(f"{prefix}", suffix="voxels.nii.gz")
         Nifti1Image(self.voxels, self.affine).to_filename(voxelfile)
         with gzip.open(probsfile, 'wt') as f:
             for D in self.probs:
                 f.write("{}\n".format(" ".join(f"{i} {p}" for i, p in D.items())))
@@ -128,17 +130,26 @@
                         " ".join(map(str, bbox["maxpoint"])),
                     )
                 )
 
     @classmethod
     def from_cache(cls, prefix: str):
         """
-        Attemts to build a sparse index from the siibra cache,
-        looking for suitable cache files with the specified prefix.
-        Returns None if cached files are not found or suitable.
+        Attempts to build a sparse index from the siibra cache, looking for
+        suitable cache files with the specified prefix.
+
+        Parameters
+        ----------
+        prefix: str
+            Prefix of the filenames.
+
+        Returns
+        -------
+        SparseIndex
+            None if cached files are not found or suitable.
         """
 
         probsfile = cache.CACHE.build_filename(f"{prefix}", suffix="probs.txt.gz")
         bboxfile = cache.CACHE.build_filename(f"{prefix}", suffix="bboxes.txt.gz")
         voxelfile = cache.CACHE.build_filename(f"{prefix}", suffix="voxels.nii.gz")
         if not all(path.isfile(f) for f in [probsfile, bboxfile, voxelfile]):
             return None
@@ -175,29 +186,30 @@
                     }
                 )
 
         return result
 
 
 class SparseMap(parcellationmap.Map):
-    """A sparse representation of list of statistical (e.g. probabilistic) brain region maps.
+    """
+    A sparse representation of list of statistical (e.g. probabilistic) brain
+    region maps.
 
     It represents the 3D statistical maps of N brain regions by two data structures:
-        1) 'spatial_index', a 3D volume where non-negative values represent unique
-            indices into a list of region assignments
-        2) 'probs', a list of region assignments where each entry is a dict
-
-    More precisely, given
-        i = sparse_index.voxels[x, y, z]
-    we define that
-        - if i<0, no brain region is assigned at this location
-        - if i>=0, probs[i] defines the probabilities of brain regions.
+
+    1) 'spatial_index', a 3D volume where non-negative values represent unique indices into a list of region assignments
+    2) 'probs', a list of region assignments where each entry is a dict
+
+    More precisely, given ``i = sparse_index.voxels[x, y, z]`` we define that
+
+    - if `i<0`, no brain region is assigned at this location
+    - if `i>=0`, ``probs[i]`` defines the probabilities of brain regions.
 
     Each entry in probs is a dictionary that represents the region assignments for
-    the unique voxel where spatial_index==i. The assignment maps from a "mapindex"
+    the unique voxel where ``spatial_index == i``. The assignment maps from a MapIndex
     to the actual (probability) value.
     """
 
     # A gitlab instance with holds precomputed sparse indices
     _GITLAB_SERVER = 'https://jugit.fz-juelich.de'
     _GITLAB_PROJECT = 5779
 
@@ -274,23 +286,27 @@
         region: Union[str, 'Region'] = None,
         **kwargs
     ):
         """
         Recreate a particular volumetric map from the sparse
         representation.
 
-        Arguments
-        ---------
-        region_or_index: Union[str, Region, MapIndex]
+        Parameters
+        ----------
+        region_or_index: str, Region, MapIndex
             Lazy match the specification.
         index : MapIndex
             The index to be fetched.
-        region: Union[str, Region]
-            Region name specification. If given, will be used to
-            decode the map index of a particular region.
+        region: str, Region
+            Region name specification. If given, will be used to decode the map
+            index of a particular region.
+
+        Returns
+        -------
+        An image or mesh
         """
         if kwargs.get('format') in ['mesh'] + _volume.Volume.MESH_FORMATS:
             # a mesh is requested, this is not handled by the sparse map
             return super().fetch(region_or_index, index=index, region=region, **kwargs)
 
         try:
             length = len([arg for arg in [region_or_index, region, index] if arg is not None])
@@ -379,15 +395,15 @@
                 target_affine=self.affine,
                 target_shape=self.shape,
                 interpolation=interp,
             )
 
         querydata = np.asanyarray(queryimg.dataobj).squeeze()
 
-        for mode, modeimg in parcellationmap.Map.iterate_connected_components(queryimg):
+        for mode, modeimg in iterate_connected_components(queryimg):
 
             # determine bounding box of the mode
             modemask = np.asanyarray(modeimg.dataobj)
             XYZ2 = np.array(np.where(modemask)).T
             position = np.dot(modeimg.affine, np.r_[XYZ2.mean(0), 1])[:3]
             if XYZ2.shape[0] <= minsize_voxel:
                 components[modemask] == 0
@@ -443,33 +459,35 @@
                     (v1 > 0) & (v2 > 0)
                 )  # np.minimum(v1, v2).sum()
                 if intersection == 0:
                     continue
                 iou = intersection / np.sum(
                     (v1 > 0) | (v2 > 0)
                 )  # np.maximum(v1, v2).sum()
-                contains = intersection / (v1 > 0).sum()
-                contained = intersection / (v2 > 0).sum()
 
                 v1d = v1 - v1.mean()
                 v2d = v2 - v2.mean()
                 rho = (
                     (v1d * v2d).sum()
                     / np.sqrt((v1d ** 2).sum())
                     / np.sqrt((v2d ** 2).sum())
                 )
 
                 maxval = v1.max()
 
-                assignments.append([
-                    mode,
-                    tuple(position.round(2)),
-                    volume,
-                    None,
-                    maxval,
-                    iou,
-                    contained,
-                    contains,
-                    rho
-                ])
+                assignments.append(
+                    {
+                        "input structure": mode,
+                        "centroid": tuple(position.round(2)),
+                        "volume": volume,
+                        "fragment": None,
+                        "map value": maxval,
+                        "intersection over union": iou,
+                        "intersection over first": intersection / (v1 > 0).sum(),
+                        "intersection over second": intersection / (v2 > 0).sum(),
+                        "correlation": rho,
+                        "weighted mean of first": np.sum(v1 * v2) / np.sum(v2),
+                        "weighted mean of second": np.sum(v1 * v2) / np.sum(v1)
+                    }
+                )
 
         return assignments
```

### Comparing `siibra-0.4a33/siibra/volumes/volume.py` & `siibra-0.4a35/siibra/volumes/volume.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,17 +16,20 @@
 from .. import logger
 from ..retrieval import requests
 from ..locations import boundingbox as _boundingbox
 from ..core import space
 
 import nibabel as nib
 from abc import ABC, abstractmethod
-from typing import List, Dict, Union, Set
+from typing import List, Dict, Union, Set, TYPE_CHECKING
 import json
 
+if TYPE_CHECKING:
+    from ..retrieval.datasets import EbrainsDataset
+    TypeDataset = EbrainsDataset
 
 class ColorVolumeNotSupported(NotImplementedError):
     pass
 
 
 class Volume:
     """
@@ -51,35 +54,44 @@
 
     def __init__(
         self,
         space_spec: dict,
         providers: List['VolumeProvider'],
         name: str = "",
         variant: str = None,
+        datasets: List['TypeDataset'] = [],
     ):
         self._name_cached = name  # see lazy implementation below
         self._space_spec = space_spec
         self.variant = variant
         self._providers: Dict[str, 'VolumeProvider'] = {}
+        self.datasets = datasets
         for provider in providers:
             srctype = provider.srctype
             assert srctype not in self._providers
             self._providers[srctype] = provider
         if len(self._providers) == 0:
             logger.debug(f"No provider for volume {self}")
 
     @property
     def name(self):
-        """ allows derived classes to implemente a lazy name specification."""
+        """
+        Allows derived classes to implement a lazy name specification.
+        """
         return self._name_cached
 
     @property
     def providers(self):
+        def concat(url: Union[str, Dict[str, str]], concat: str):
+            if isinstance(url, str):
+                return url + concat
+            return { key: url[key] + concat for key in url }
         return {
-            srctype: prov._url for srctype, prov in self._providers.items()
+            srctype: concat(prov._url, f" {prov.label}" if hasattr(prov, "label") else "")
+            for srctype, prov in self._providers.items()
         }
 
     @property
     def boundingbox(self):
         for provider in self._providers.values():
             try:
                 bbox = provider.boundingbox
@@ -145,24 +157,24 @@
         """
         Fetch a volumetric or surface representation from one of the providers.
 
         Parameters
         ----------
         format: str
             Requested format. Per default, several formats are tried,
-            starting with volumetric formats. You may explicitly specify:
-            - 'surface' or 'mesh' to fetch a surface format
-            - 'volumetric' or 'voxel' to fetch a volumetric format
-            - supported format types, see :data:`Volume.SUPPORTED_FORMATS`. This includes:
-                :class:`'nii'<siibra.volumes.nifti.NiftiProvider()>`,
-                :class:`'zip/nii'<siibra.volumes.nifti.ZipContainedNiftiProvider()>`,
-                :class:`'neuroglancer/precomputed'<siibra.volumes.neuroglancer.NeuroglancerProvider()>`,
-                :class:`'gii-mesh'<siibra.volumes.gifti.GiftiMesh()>`,
-                :class:`'neuroglancer/precompmesh'<siibra.volumes.neuroglancer.NeuroglancerMesh()>`,
-                :class:`'gii-label'<siibra.volumes.gifti.GiftiSurfaceLabeling()>`
+            starting with volumetric formats. It can be explicitly specified as:
+                - 'surface' or 'mesh' to fetch a surface format
+                - 'volumetric' or 'voxel' to fetch a volumetric format
+                - supported format types, see SUPPORTED_FORMATS. This includes
+                'nii', 'zip/nii', 'neuroglancer/precomputed', 'gii-mesh',
+                'neuroglancer/precompmesh', 'gii-label'
+
+        Returns
+        -------
+        An image or mesh
         """
 
         if format is None:
             requested_formats = self.SUPPORTED_FORMATS
         elif format == 'mesh':
             requested_formats = self.MESH_FORMATS
         elif format == 'image':
```

### Comparing `siibra-0.4a33/siibra.egg-info/PKG-INFO` & `siibra-0.4a35/siibra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 0.4a33
+Version: 0.4a35
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -27,24 +27,24 @@
 Medicine (INM-1), Forschungszentrum Jülich GmbH*
 
 .. intro-start
 
 ``siibra`` is a Python client to a brain atlas framework that integrates brain parcellations and reference spaces at different spatial scales, and connects them with a broad range of multimodal regional data features. 
 It aims to facilitate programmatic and reproducible incorporation of brain parcellations and brain region features from different sources into neuroscience workflows.
 
-    **Note:** *``siibra-python`` is still in development. While care is taken that it works reliably, its API is not yet stable and you may still encounter bugs when using it.*
+    **Note:** ``siibra-python`` *is still in development. While care is taken that it works reliably, its API is not yet stable and you may still encounter bugs when using it.*
 
 ``siibra`` provides structured access to parcellation schemes in different brain reference spaces, including volumetric reference templates at  macroscopic and microscopic resolutions as well as surface representations. 
 It supports both discretely labelled and statistical (probabilistic) parcellation maps, which can be used to assign brain regions to spatial locations and image signals, to retrieve region-specific neuroscience datasets from multiple online repositories, and to sample information from high-resolution image data. 
 The datasets anchored to brain regions address features of molecular, cellular and architecture as well as connectivity, and are complemented with live queries to external repositories as well as dynamic extraction from "big" image volumes such as the 20 micrometer BigBrain model.
 
 ``siibra`` was developed in the frame of the `Human Brain Project <https://humanbrainproject.eu>`__ for accessing the `EBRAINS
 human brain atlas <https://ebrains.eu/service/human-brain-atlas>`__. 
 It stores most of its contents as sustainable and open datasets in the `EBRAINS Knowledge Graph <https://kg.ebrains.eu>`__, and is designed to support the `OpenMINDS metadata standards <https://github.com/HumanBrainProject/openMINDS_SANDS>`__. 
-Its functionalities include common actions known from the interactive viewer ``siibra explorer`` `hosted at EBRAINS <https://atlases.ebrains.eu/viewer>`__. 
+Its functionalities include common actions known from the interactive viewer ``siibra-explorer`` `hosted at EBRAINS <https://atlases.ebrains.eu/viewer>`__. 
 In fact, the viewer is a good resource for exploring ``siibra``\ ’s core functionalities interactively: Selecting different parcellations, browsing and searching brain region hierarchies, downloading maps, identifying brain regions, and accessing multimodal features and connectivity information associated with brain regions. 
 Feature queries in ``siibra`` are parameterized by data modality and anatomical location, while the latter could be a brain region, brain parcellation, or location in reference space. 
 Beyond the explorative focus of ``siibra-explorer``, the Python library supports a range of data analysis functions suitable for typical neuroscience workflows.
 
 ``siibra`` hides much of the complexity that would be required to collect and interact with the individual parcellations, templates and data repositories.
 By encapsulating many aspects of interacting with different maps and reference templates spaces, it also minimizes common errors like misinterpretation of coordinates from different reference spaces, confusing label indices of brain regions, or using inconsistent versions of parcellation maps. 
 It aims to provide a safe way of using maps defined across multiple spatial scales for reproducible analysis.
```

### Comparing `siibra-0.4a33/siibra.egg-info/SOURCES.txt` & `siibra-0.4a35/siibra.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -17,37 +17,36 @@
 siibra/core/atlas.py
 siibra/core/concept.py
 siibra/core/parcellation.py
 siibra/core/region.py
 siibra/core/space.py
 siibra/features/__init__.py
 siibra/features/anchor.py
-siibra/features/basetypes/__init__.py
-siibra/features/basetypes/cortical_profile.py
-siibra/features/basetypes/feature.py
-siibra/features/basetypes/regional_connectivity.py
-siibra/features/basetypes/tabular.py
-siibra/features/basetypes/volume_of_interest.py
-siibra/features/cellular/__init__.py
-siibra/features/cellular/bigbrain_intensity_profile.py
-siibra/features/cellular/cell_density_profile.py
-siibra/features/cellular/layerwise_bigbrain_intensities.py
-siibra/features/cellular/layerwise_cell_density.py
+siibra/features/feature.py
 siibra/features/connectivity/__init__.py
 siibra/features/connectivity/functional_connectivity.py
+siibra/features/connectivity/regional_connectivity.py
 siibra/features/connectivity/streamline_counts.py
 siibra/features/connectivity/streamline_lengths.py
-siibra/features/external/__init__.py
-siibra/features/external/ebrains.py
-siibra/features/fibres/__init__.py
-siibra/features/functional/__init__.py
-siibra/features/molecular/__init__.py
-siibra/features/molecular/gene_expression.py
-siibra/features/molecular/receptor_density_fingerprint.py
-siibra/features/molecular/receptor_density_profile.py
+siibra/features/dataset/__init__.py
+siibra/features/dataset/ebrains.py
+siibra/features/image/__init__.py
+siibra/features/image/image.py
+siibra/features/image/sections.py
+siibra/features/image/volume_of_interest.py
+siibra/features/tabular/__init__.py
+siibra/features/tabular/bigbrain_intensity_profile.py
+siibra/features/tabular/cell_density_profile.py
+siibra/features/tabular/cortical_profile.py
+siibra/features/tabular/gene_expression.py
+siibra/features/tabular/layerwise_bigbrain_intensities.py
+siibra/features/tabular/layerwise_cell_density.py
+siibra/features/tabular/receptor_density_fingerprint.py
+siibra/features/tabular/receptor_density_profile.py
+siibra/features/tabular/tabular.py
 siibra/livequeries/__init__.py
 siibra/livequeries/allen.py
 siibra/livequeries/bigbrain.py
 siibra/livequeries/ebrains.py
 siibra/livequeries/query.py
 siibra/locations/__init__.py
 siibra/locations/boundingbox.py
@@ -56,16 +55,14 @@
 siibra/locations/pointset.py
 siibra/retrieval/__init__.py
 siibra/retrieval/cache.py
 siibra/retrieval/datasets.py
 siibra/retrieval/repositories.py
 siibra/retrieval/requests.py
 siibra/retrieval/exceptions/__init__.py
-siibra/samplers/__init__.py
-siibra/samplers/bigbrain.py
 siibra/vocabularies/__init__.py
 siibra/vocabularies/gene_names.json
 siibra/vocabularies/receptor_symbols.json
 siibra/vocabularies/region_aliases.json
 siibra/volumes/__init__.py
 siibra/volumes/gifti.py
 siibra/volumes/neuroglancer.py
```

### Comparing `siibra-0.4a33/test/test_siibra.py` & `siibra-0.4a35/test/test_siibra.py`

 * *Files identical despite different names*

