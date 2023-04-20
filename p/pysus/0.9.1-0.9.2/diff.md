# Comparing `tmp/pysus-0.9.1.tar.gz` & `tmp/pysus-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysus-0.9.1.tar", max compression
+gzip compressed data, was "pysus-0.9.2.tar", max compression
```

## Comparing `pysus-0.9.1.tar` & `pysus-0.9.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0    35149 2023-04-12 20:41:44.705570 pysus-0.9.1/LICENSE
--rw-r--r--   0        0        0     1372 2023-04-12 20:43:37.110119 pysus-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     8421 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/Notebooks/Analyzing SIH.ipynb
--rw-r--r--   0        0        0    15450 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/Notebooks/Analyzing SIM.ipynb
--rw-r--r--   0        0        0    14877 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/Notebooks/Analyzing SINASC Data.ipynb
--rw-r--r--   0        0        0    47374 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/Notebooks/Getting_CNES_Data.ipynb
--rw-r--r--   0        0        0     3057 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/Notebooks/Processing SIM with municipality.ipynb
--rw-r--r--   0        0        0    27870 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/Notebooks/Processing SIM.ipynb
--rw-r--r--   0        0        0    59869 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/Notebooks/SINAN.ipynb
--rw-r--r--   0        0        0      422 2023-04-12 20:43:37.106119 pysus-0.9.1/pysus/__init__.py
--rw-r--r--   0        0        0   165526 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/dataset/geocode_by_cities.json
--rw-r--r--   0        0        0     3931 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/ANIM.tar.gz
--rw-r--r--   0        0        0     7064 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/BOTU.tar.gz
--rw-r--r--   0        0        0     5341 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/CHAG.tar.gz
--rw-r--r--   0        0        0     5439 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/CHIK.tar.gz
--rw-r--r--   0        0        0     5290 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/COLE.tar.gz
--rw-r--r--   0        0        0     4496 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/COQU.tar.gz
--rw-r--r--   0        0        0     5439 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/DENG.tar.gz
--rw-r--r--   0        0        0     5093 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/DIFT.tar.gz
--rw-r--r--   0        0        0     2953 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/ESQU.tar.gz
--rw-r--r--   0        0        0     5257 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/FAMA.tar.gz
--rw-r--r--   0        0        0     4638 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/FMAC.tar.gz
--rw-r--r--   0        0        0     6354 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/FTIF.tar.gz
--rw-r--r--   0        0        0     4247 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/HANS.tar.gz
--rw-r--r--   0        0        0     6202 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/HANT.tar.gz
--rw-r--r--   0        0        0     5603 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/HEPA.tar.gz
--rw-r--r--   0        0        0     4554 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/IEXO.tar.gz
--rw-r--r--   0        0        0     4214 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/LEIV.tar.gz
--rw-r--r--   0        0        0     4958 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/LEPT.tar.gz
--rw-r--r--   0        0        0     4293 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/LTAN.tar.gz
--rw-r--r--   0        0        0     3614 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/MALA.tar.gz
--rw-r--r--   0        0        0     5652 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/MENI.tar.gz
--rw-r--r--   0        0        0     3114 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/PEST.tar.gz
--rw-r--r--   0        0        0     5404 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/RAIV.tar.gz
--rw-r--r--   0        0        0     5439 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/SIFC.tar.gz
--rw-r--r--   0        0        0     1952 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/SIFG.tar.gz
--rw-r--r--   0        0        0     4189 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/TETA.tar.gz
--rw-r--r--   0        0        0     5518 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/TETN.tar.gz
--rw-r--r--   0        0        0     5659 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/TUBE.tar.gz
--rw-r--r--   0        0        0    35103 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/metadata/SINAN/typecast.py
--rw-r--r--   0        0        0      766 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/CIHA.py
--rw-r--r--   0        0        0     2277 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/CNES.py
--rw-r--r--   0        0        0     3074 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/ESUS.py
--rw-r--r--   0        0        0    13567 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/IBGE.py
--rw-r--r--   0        0        0     3170 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/Infodengue.py
--rw-r--r--   0        0        0      695 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/Infogripe.py
--rw-r--r--   0        0        0     1016 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/PNI.py
--rw-r--r--   0        0        0     2382 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/SIA.py
--rw-r--r--   0        0        0      847 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/SIH.py
--rw-r--r--   0        0        0     6675 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/SIM.py
--rw-r--r--   0        0        0     1688 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/SINAN.py
--rw-r--r--   0        0        0    24424 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/__init__.py
--rw-r--r--   0        0        0      790 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/sinasc.py
--rw-r--r--   0        0        0     3677 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/vaccine.py
--rw-r--r--   0        0        0     1922 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/preprocessing/ESUS.py
--rw-r--r--   0        0        0     6289 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/preprocessing/SIM.py
--rw-r--r--   0        0        0      128 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/preprocessing/__init__.py
--rw-r--r--   0        0        0    10109 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/preprocessing/decoders.py
--rw-r--r--   0        0        0     2402 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/preprocessing/geodata.py
--rw-r--r--   0        0        0     3878 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/preprocessing/sinan.py
--rw-r--r--   0        0        0      128 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/tests/__init__.py
--rw-r--r--   0        0        0      505 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/tests/test_SIA.py
--rw-r--r--   0        0        0      722 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/tests/test_cnes.py
--rw-r--r--   0        0        0  9175254 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/EPR-2016-06-01-2016.dbf
--rw-r--r--   0        0        0       66 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/__init__.py
--rw-r--r--   0        0        0     3126 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_Infodengue.py
--rw-r--r--   0        0        0      330 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_Infogripe.py
--rw-r--r--   0        0        0      640 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_PNI.py
--rw-r--r--   0        0        0      795 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_ciha.py
--rw-r--r--   0        0        0     2265 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_sia.py
--rw-r--r--   0        0        0      547 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_sih.py
--rw-r--r--   0        0        0     1249 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_sim.py
--rw-r--r--   0        0        0     4624 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_sinan.py
--rw-r--r--   0        0        0      785 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_sinasc.py
--rw-r--r--   0        0        0      419 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_vaccine.py
--rw-r--r--   0        0        0     6975 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_decoders.py
--rw-r--r--   0        0        0      304 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_esus.py
--rw-r--r--   0        0        0     1382 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_ibge.py
--rw-r--r--   0        0        0      741 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_init.py
--rw-r--r--   0        0        0      642 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_sih.py
--rw-r--r--   0        0        0     2123 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_sim.py
--rw-r--r--   0        0        0      758 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_utilities.py
--rw-r--r--   0        0        0        0 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/utilities/__init__.py
--rw-r--r--   0        0        0     2766 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/utilities/readdbc.py
--rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 pysus-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-20 16:36:07.142828 pysus-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1372 2023-04-20 16:38:14.796192 pysus-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     8421 2023-04-20 16:36:07.182829 pysus-0.9.2/pysus/Notebooks/Analyzing SIH.ipynb
+-rw-r--r--   0        0        0    15450 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/Notebooks/Analyzing SIM.ipynb
+-rw-r--r--   0        0        0    14877 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/Notebooks/Analyzing SINASC Data.ipynb
+-rw-r--r--   0        0        0    47374 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/Notebooks/Getting_CNES_Data.ipynb
+-rw-r--r--   0        0        0     3057 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/Notebooks/Processing SIM with municipality.ipynb
+-rw-r--r--   0        0        0    27870 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/Notebooks/Processing SIM.ipynb
+-rw-r--r--   0        0        0    59869 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/Notebooks/SINAN.ipynb
+-rw-r--r--   0        0        0      422 2023-04-20 16:38:14.792191 pysus-0.9.2/pysus/__init__.py
+-rw-r--r--   0        0        0   165526 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/dataset/geocode_by_cities.json
+-rw-r--r--   0        0        0     3931 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/ANIM.tar.gz
+-rw-r--r--   0        0        0     7064 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/BOTU.tar.gz
+-rw-r--r--   0        0        0     5341 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/CHAG.tar.gz
+-rw-r--r--   0        0        0     5439 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/CHIK.tar.gz
+-rw-r--r--   0        0        0     5290 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/COLE.tar.gz
+-rw-r--r--   0        0        0     4496 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/COQU.tar.gz
+-rw-r--r--   0        0        0     5439 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/DENG.tar.gz
+-rw-r--r--   0        0        0     5093 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/DIFT.tar.gz
+-rw-r--r--   0        0        0     2953 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/ESQU.tar.gz
+-rw-r--r--   0        0        0     5257 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/FAMA.tar.gz
+-rw-r--r--   0        0        0     4638 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/FMAC.tar.gz
+-rw-r--r--   0        0        0     6354 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/FTIF.tar.gz
+-rw-r--r--   0        0        0     4247 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/HANS.tar.gz
+-rw-r--r--   0        0        0     6202 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/HANT.tar.gz
+-rw-r--r--   0        0        0     5603 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/HEPA.tar.gz
+-rw-r--r--   0        0        0     4554 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/IEXO.tar.gz
+-rw-r--r--   0        0        0     4214 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/LEIV.tar.gz
+-rw-r--r--   0        0        0     4958 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/LEPT.tar.gz
+-rw-r--r--   0        0        0     4293 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/LTAN.tar.gz
+-rw-r--r--   0        0        0     3614 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/MALA.tar.gz
+-rw-r--r--   0        0        0     5652 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/MENI.tar.gz
+-rw-r--r--   0        0        0     3114 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/PEST.tar.gz
+-rw-r--r--   0        0        0     5404 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/RAIV.tar.gz
+-rw-r--r--   0        0        0     5439 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/SIFC.tar.gz
+-rw-r--r--   0        0        0     1952 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/SIFG.tar.gz
+-rw-r--r--   0        0        0     4189 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/TETA.tar.gz
+-rw-r--r--   0        0        0     5518 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/TETN.tar.gz
+-rw-r--r--   0        0        0     5659 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/TUBE.tar.gz
+-rw-r--r--   0        0        0    35103 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/metadata/SINAN/typecast.py
+-rw-r--r--   0        0        0      766 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/online_data/CIHA.py
+-rw-r--r--   0        0        0     2277 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/online_data/CNES.py
+-rw-r--r--   0        0        0     3078 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/online_data/ESUS.py
+-rw-r--r--   0        0        0    13567 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/online_data/IBGE.py
+-rw-r--r--   0        0        0     3170 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/online_data/Infodengue.py
+-rw-r--r--   0        0        0      696 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/online_data/Infogripe.py
+-rw-r--r--   0        0        0     1016 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/online_data/PNI.py
+-rw-r--r--   0        0        0     2382 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/online_data/SIA.py
+-rw-r--r--   0        0        0      847 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/online_data/SIH.py
+-rw-r--r--   0        0        0     6675 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/online_data/SIM.py
+-rw-r--r--   0        0        0     1688 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/online_data/SINAN.py
+-rw-r--r--   0        0        0    24411 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/online_data/__init__.py
+-rw-r--r--   0        0        0      790 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/online_data/sinasc.py
+-rw-r--r--   0        0        0     3677 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/online_data/vaccine.py
+-rw-r--r--   0        0        0     1922 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/preprocessing/ESUS.py
+-rw-r--r--   0        0        0     6289 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/preprocessing/SIM.py
+-rw-r--r--   0        0        0      128 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/preprocessing/__init__.py
+-rw-r--r--   0        0        0    10109 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/preprocessing/decoders.py
+-rw-r--r--   0        0        0     2402 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/preprocessing/geodata.py
+-rw-r--r--   0        0        0     3878 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/preprocessing/sinan.py
+-rw-r--r--   0        0        0      128 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/tests/__init__.py
+-rw-r--r--   0        0        0      505 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/tests/test_SIA.py
+-rw-r--r--   0        0        0      722 2023-04-20 16:36:07.186828 pysus-0.9.2/pysus/tests/test_cnes.py
+-rw-r--r--   0        0        0  9175254 2023-04-20 16:36:07.214829 pysus-0.9.2/pysus/tests/test_data/EPR-2016-06-01-2016.dbf
+-rw-r--r--   0        0        0       66 2023-04-20 16:36:07.214829 pysus-0.9.2/pysus/tests/test_data/__init__.py
+-rw-r--r--   0        0        0     3126 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_data/test_Infodengue.py
+-rw-r--r--   0        0        0      330 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_data/test_Infogripe.py
+-rw-r--r--   0        0        0      640 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_data/test_PNI.py
+-rw-r--r--   0        0        0      795 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_data/test_ciha.py
+-rw-r--r--   0        0        0     2265 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_data/test_sia.py
+-rw-r--r--   0        0        0      547 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_data/test_sih.py
+-rw-r--r--   0        0        0     1249 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_data/test_sim.py
+-rw-r--r--   0        0        0     4624 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_data/test_sinan.py
+-rw-r--r--   0        0        0      785 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_data/test_sinasc.py
+-rw-r--r--   0        0        0      419 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_data/test_vaccine.py
+-rw-r--r--   0        0        0     6975 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_decoders.py
+-rw-r--r--   0        0        0      304 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_esus.py
+-rw-r--r--   0        0        0     1382 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_ibge.py
+-rw-r--r--   0        0        0      741 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_init.py
+-rw-r--r--   0        0        0      642 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_sih.py
+-rw-r--r--   0        0        0     2123 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_sim.py
+-rw-r--r--   0        0        0      758 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/tests/test_utilities.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/utilities/__init__.py
+-rw-r--r--   0        0        0     2766 2023-04-20 16:36:07.218829 pysus-0.9.2/pysus/utilities/readdbc.py
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 pysus-0.9.2/PKG-INFO
```

### Comparing `pysus-0.9.1/LICENSE` & `pysus-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pyproject.toml` & `pysus-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysus"
-version = "0.9.1"  # changed by semantic-release
+version = "0.9.2"  # changed by semantic-release
 description = "Tools for dealing with Brazil's Public health data"
 authors = ["Flavio Codeco Coelho <fccoelho@gmail.com>"]
 license = "GPL"
 
 packages = [{include='pysus'}]
 
 [tool.poetry.dependencies]
```

### Comparing `pysus-0.9.1/pysus/Notebooks/Analyzing SIH.ipynb` & `pysus-0.9.2/pysus/Notebooks/Analyzing SIH.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/Notebooks/Analyzing SIM.ipynb` & `pysus-0.9.2/pysus/Notebooks/Analyzing SIM.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/Notebooks/Analyzing SINASC Data.ipynb` & `pysus-0.9.2/pysus/Notebooks/Analyzing SINASC Data.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/Notebooks/Getting_CNES_Data.ipynb` & `pysus-0.9.2/pysus/Notebooks/Getting_CNES_Data.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/Notebooks/Processing SIM with municipality.ipynb` & `pysus-0.9.2/pysus/Notebooks/Processing SIM with municipality.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/Notebooks/Processing SIM.ipynb` & `pysus-0.9.2/pysus/Notebooks/Processing SIM.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/Notebooks/SINAN.ipynb` & `pysus-0.9.2/pysus/Notebooks/SINAN.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/dataset/geocode_by_cities.json` & `pysus-0.9.2/pysus/dataset/geocode_by_cities.json`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/ANIM.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/ANIM.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/BOTU.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/BOTU.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/CHAG.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/CHAG.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/CHIK.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/CHIK.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/COLE.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/COLE.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/COQU.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/COQU.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/DENG.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/DENG.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/DIFT.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/DIFT.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/ESQU.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/ESQU.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/FAMA.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/FAMA.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/FMAC.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/FMAC.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/FTIF.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/FTIF.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/HANS.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/HANS.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/HANT.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/HANT.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/HEPA.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/HEPA.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/IEXO.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/IEXO.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/LEIV.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/LEIV.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/LEPT.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/LEPT.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/LTAN.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/LTAN.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/MALA.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/MALA.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/MENI.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/MENI.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/PEST.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/PEST.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/RAIV.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/RAIV.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/SIFC.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/SIFC.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/SIFG.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/SIFG.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/TETA.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/TETA.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/TETN.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/TETN.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/TUBE.tar.gz` & `pysus-0.9.2/pysus/metadata/SINAN/TUBE.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/metadata/SINAN/typecast.py` & `pysus-0.9.2/pysus/metadata/SINAN/typecast.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/online_data/CIHA.py` & `pysus-0.9.2/pysus/online_data/CIHA.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,13 +19,13 @@
 ) -> list:
     """
     Download CIHA records for state, year and month and returns dataframe
     :param months: 1 to 12, can be a list
     :param states: 2 letter state code,
     :param years: 4 digit integer
     """
-    return FTP_Downloader("CIHA").download(
+    return FTP_Downloader('CIHA').download(
         UFs=states,
         years=years,
         months=months,
         local_dir=data_dir,
     )
```

### Comparing `pysus-0.9.1/pysus/online_data/CNES.py` & `pysus-0.9.2/pysus/online_data/CNES.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Union
 
 from pysus.online_data import CACHEPATH, FTP_Downloader
 
 group_dict = {
-    "LT": ["Leitos - A partir de Out/2005", 10, 2005],
-    "ST": ["Estabelecimentos - A partir de Ago/2005", 8, 2005],
-    "DC": ["Dados Complementares - A partir de Ago/2005", 8, 2005],
-    "EQ": ["Equipamentos - A partir de Ago/2005", 8, 2005],
-    "SR": ["Serviço Especializado - A partir de Ago/2005", 8, 2005],
-    "HB": ["Habilitação - A partir de Mar/2007", 3, 2007],
-    "PF": ["Profissional - A partir de Ago/2005", 8, 2005],
-    "EP": ["Equipes - A partir de Abr/2007", 5, 2007],
-    "IN": ["Incentivos - A partir de Nov/2007", 11, 2007],
-    "RC": ["Regra Contratual - A partir de Mar/2007", 3, 2007],
-    "EE": ["Estabelecimento de Ensino - A partir de Mar/2007", 3, 2007],
-    "EF": ["Estabelecimento Filantrópico - A partir de Mar/2007", 3, 2007],
-    "GM": ["Gestão e Metas - A partir de Jun/2007", 6, 2007],
+    'LT': ['Leitos - A partir de Out/2005', 10, 2005],
+    'ST': ['Estabelecimentos - A partir de Ago/2005', 8, 2005],
+    'DC': ['Dados Complementares - A partir de Ago/2005', 8, 2005],
+    'EQ': ['Equipamentos - A partir de Ago/2005', 8, 2005],
+    'SR': ['Serviço Especializado - A partir de Ago/2005', 8, 2005],
+    'HB': ['Habilitação - A partir de Mar/2007', 3, 2007],
+    'PF': ['Profissional - A partir de Ago/2005', 8, 2005],
+    'EP': ['Equipes - A partir de Abr/2007', 5, 2007],
+    'IN': ['Incentivos - A partir de Nov/2007', 11, 2007],
+    'RC': ['Regra Contratual - A partir de Mar/2007', 3, 2007],
+    'EE': ['Estabelecimento de Ensino - A partir de Mar/2007', 3, 2007],
+    'EF': ['Estabelecimento Filantrópico - A partir de Mar/2007', 3, 2007],
+    'GM': ['Gestão e Metas - A partir de Jun/2007', 6, 2007],
 }
 
 
 def download(
     group: str,
     states: Union[str, list],
     years: Union[str, list, int],
@@ -43,14 +43,14 @@
         EE - Estabelecimento de Ensino - A partir de Mar/2007
         EF - Estabelecimento Filantrópico - A partir de Mar/2007
         GM - Gestão e Metas - A partir de Jun/2007
     :param months: 1 to 12, can be a list of years
     :param states: 2 letter state code, can be a list of UFs
     :param years: 4 digit integer, can be a list of years
     """
-    return FTP_Downloader("CNES").download(
+    return FTP_Downloader('CNES').download(
         CNES_group=group,
         UFs=states,
         years=years,
         months=months,
         local_dir=data_dir,
     )
```

### Comparing `pysus-0.9.1/pysus/online_data/ESUS.py` & `pysus-0.9.2/pysus/online_data/ESUS.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,87 +13,87 @@
     Download ESUS data by UF
     :param uf: rj, mg, etc
     :param cache: if results should be cached on disk
     :return: DataFrame if data fits in memory,
         other an iterator of chunks of size 1000.
     """
     uf = uf.lower()
-    user = "user-public-notificacoes"
-    pwd = "Za4qNXdyQNSa9YaA"
+    user = 'user-public-notificacoes'
+    pwd = 'Za4qNXdyQNSa9YaA'
     today = date.today()
-    dt = today.strftime("_%d_%m_%Y")
-    base = f"desc-esus-notifica-estado-{uf}"  # desc-notificacoes-esusve-
-    url = f"https://{user}:{pwd}@elasticsearch-saps.saude.gov.br"
-    out = f"ESUS_{uf}_{dt}.parquet"
+    dt = today.strftime('_%d_%m_%Y')
+    base = f'desc-esus-notifica-estado-{uf}'  # desc-notificacoes-esusve-
+    url = f'https://{user}:{pwd}@elasticsearch-saps.saude.gov.br'
+    out = f'ESUS_{uf}_{dt}.parquet'
 
     cachefile = os.path.join(CACHEPATH, out)
-    tempfile = os.path.join(CACHEPATH, f"ESUS_temp_{uf.upper()}.csv.gz")
+    tempfile = os.path.join(CACHEPATH, f'ESUS_temp_{uf.upper()}.csv.gz')
     if os.path.exists(cachefile):
-        logger.info(f"Local parquet file found at {cachefile}")
+        logger.info(f'Local parquet file found at {cachefile}')
         df = pd.read_parquet(cachefile)
     elif os.path.exists(tempfile):
-        logger.info(f"Local csv file found at {tempfile}")
+        logger.info(f'Local csv file found at {tempfile}')
         df = pd.read_csv(tempfile, chunksize=1000)
     else:
         fname = fetch(base, uf, url)
         size = os.stat(fname).st_size
         if size > 50e6 and checkmemory:
-            print(f"Downloaded data is to large:{size / 1e6} MB compressed.")
+            print(f'Downloaded data is to large:{size / 1e6} MB compressed.')
             print(
-                "Only loading the first 1000 rows. If your computer has enough"
+                'Only loading the first 1000 rows. If your computer has enough'
                 + " memory, set 'checkmemory' to False"
             )
-            print(f"The full data is in {fname}")
+            print(f'The full data is in {fname}')
             df = pd.read_csv(fname, chunksize=1000)
         else:
             df = pd.read_csv(fname, low_memory=False)
-            print(f"{df.shape[0]} records downloaded.")
+            print(f'{df.shape[0]} records downloaded.')
             os.unlink(fname)
             if cache:
                 df.to_parquet(cachefile)
-                logger.info(f"Data stored as parquet at {cachefile}")
+                logger.info(f'Data stored as parquet at {cachefile}')
 
     return df
 
 
 def fetch(base, uf, url):
     UF = uf.upper()
-    print(f"Reading ESUS data for {UF}")
-    es = Elasticsearch([url], send_get_body_as="POST")
-    body = {"query": {"match_all": {}}}
+    print(f'Reading ESUS data for {UF}')
+    es = Elasticsearch([url], send_get_body_as='POST')
+    body = {'query': {'match_all': {}}}
     results = helpers.scan(es, query=body, index=base)
     # df = pd.DataFrame.from_dict(
     # [document['_source'] for document in results]
     # )
 
     chunker = chunky_fetch(results, 3000)
     h = 1
-    tempfile = os.path.join(CACHEPATH, f"ESUS_temp_{UF}.csv.gz")
+    tempfile = os.path.join(CACHEPATH, f'ESUS_temp_{UF}.csv.gz')
     for ch in chunker:
         df = pd.DataFrame.from_dict(ch)
-        df.sintomas = df["sintomas"].str.replace(
-            ";",
-            "",
+        df.sintomas = df['sintomas'].str.replace(
+            ';',
+            '',
         )  # remove os  ;
         if h:
             df.to_csv(tempfile)
             h = 0
         else:
-            df.to_csv(tempfile, mode="a", header=False)
+            df.to_csv(tempfile, mode='a', header=False)
     # df = pd.read_csv('temp.csv.gz')
 
     return tempfile
 
 
 def chunky_fetch(results, chunk_size=3000):
-    "Fetches data in chunks to preserve memory"
+    """Fetches data in chunks to preserve memory"""
     data = []
     i = 0
     for d in results:
-        data.append(d["_source"])
+        data.append(d['_source'])
         i += 1
         if i == chunk_size:
             yield data
             data = []
             i = 0
     else:
         yield data
```

### Comparing `pysus-0.9.1/pysus/online_data/IBGE.py` & `pysus-0.9.2/pysus/online_data/IBGE.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 import requests
 import pandas as pd
 
 # requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS = 'ALL:@SECLEVEL=1'
 
 from urllib.error import HTTPError
 
-APIBASE = "https://servicodados.ibge.gov.br/api/v3/"
+APIBASE = 'https://servicodados.ibge.gov.br/api/v3/'
 
 
 def get_sidra_table(
     table_id,
     territorial_level,
-    geocode="all",
+    geocode='all',
     period=None,
     variables=None,
     classification=None,
     categories=None,
     format=None,
     decimals=None,
     headers=None,
@@ -75,104 +75,104 @@
 
         Exemplo 1: /c81/2692,2702,2694 2695 – especifica os produtos da lavoura temporária arroz, feijão e (batata doce + batata inglesa)
     :param format:
     :param decimals:
     :param headers: `y` para receber o header (valor default, caso o parâmetro h não seja especificado). `n` para não receber o header.
     :return:
     """
-    base_url = "https://apisidra.ibge.gov.br/values"
-    query = f"/t/{table_id}/n{territorial_level}/{geocode}"
+    base_url = 'https://apisidra.ibge.gov.br/values'
+    query = f'/t/{table_id}/n{territorial_level}/{geocode}'
     if period is not None:
-        query += f"/p/{period}"
+        query += f'/p/{period}'
     if variables is not None:
-        query += f"/v/{variables}"
+        query += f'/v/{variables}'
     if classification is not None:
-        query += f"/c{classification}"
+        query += f'/c{classification}'
     if categories is not None:
-        query += f"/{categories}"
+        query += f'/{categories}'
     if format is not None:
-        query += f"/f/{format}"
+        query += f'/f/{format}'
     if decimals is not None:
-        query += f"/d/{decimals}"
+        query += f'/d/{decimals}'
     if headers is not None:
-        query += f"/h/{headers}"
+        query += f'/h/{headers}'
 
     url = base_url + query
-    print(f"Requesting data from {url}")
+    print(f'Requesting data from {url}')
     try:
         with (get_legacy_session() as s, s.get(url) as response):
             df = pd.DataFrame(response.json())
     except HTTPError as exc:
         response = requests.get(url)
-        print(f"Consulta falhou: {response.text}")
+        print(f'Consulta falhou: {response.text}')
         return None
     return df
 
 
 def list_agregados(**kwargs):
     """
     Lista de agregados agrupados por pesquisa.
     veja https://servicodados.ibge.gov.br/api/docs/agregados?versao=3#api-Agregados-agregadosGet
     para maiores detalhes
     :param kwargs: parâmetros válidos: período, assunto, classificacao, periodicidade,nivel.
     :return: Dataframe
     """
-    url = APIBASE + "agregados?"
-    url += "&".join([f"{k}={v}" for k, v in kwargs.items()])
-    print(f"Fetching Data groupings from {url}")
+    url = APIBASE + 'agregados?'
+    url += '&'.join([f'{k}={v}' for k, v in kwargs.items()])
+    print(f'Fetching Data groupings from {url}')
     try:
         with (get_legacy_session() as s, s.get(url) as response):
             table = pd.DataFrame(response.json())
     except requests.exceptions.SSLError as e:
-        print(f"Failed fetching aggregates: {e}")
+        print(f'Failed fetching aggregates: {e}')
         return pd.DataFrame()
     return table
 
 
 def localidades_por_agregado(agregado: int, nivel: str):
     """
     Obtém as localidades associadas ao agregado de acordo com um ou mais níveis geográficos.
     :param agregado: codigo numérico do agregado
     :param nivel: Identificador do nível geográfico ao qual pertence as localidades. Pode conter um ou mais níveis
     delimitados pelo caracter | (pipe). p.ex. N7|N6
     :return:
     """
-    url = APIBASE + f"agregados/{agregado}/localidades/{nivel}"
+    url = APIBASE + f'agregados/{agregado}/localidades/{nivel}'
     try:
         with (get_legacy_session() as s, s.get(url) as response):
             table = pd.DataFrame(response.json())
     except Exception as e:
-        print(f"Could not download from {url}\n{e}")
+        print(f'Could not download from {url}\n{e}')
         return None
     return table
 
 
 def metadados(agregado: int):
     """
     Obtém os metadados associados ao agregado
 
     :param agregado: Identificador do agregado
     """
-    url = APIBASE + f"agregados/{agregado}/metadados"
+    url = APIBASE + f'agregados/{agregado}/metadados'
     try:
         with (get_legacy_session() as s, s.get(url) as response):
             data = response.json()
     except Exception as e:
-        print(f"Could not download from {url}\n{e}")
+        print(f'Could not download from {url}\n{e}')
         return None
     return data
 
 
 def lista_periodos(agregado: int):
     """
     Obtém os períodos associados ao agregado
     :param agregado:
     :return: pd.DataFrame com os períodos de atualização
     """
-    url = APIBASE + f"agregados/{agregado}/periodos"
+    url = APIBASE + f'agregados/{agregado}/periodos'
     try:
         with (get_legacy_session() as s, s.get(url) as response):
             table = pd.DataFrame(response.json())
     except:
         return None
     return table
 
@@ -225,27 +225,27 @@
         - **view**: Modo de visualização. Caso deseje que a resposta seja renderizada usando notação OLAP, configure
             esse parâmetro com o valor OLAP - https://servicodados.ibge.gov.br/api/v3/agregados/1705/variaveis?view=OLAP&localidades=BR.
             A outra opção é configurar esse parâmetro com o valor flat. No modo flat, o primeiro elemento do Array são
             metadados, de forma que os resultados vêm a partir do segundo elemento
     """
 
     def __init__(
-        self, agregado: int, periodos: str, variavel: str = "allxp", **kwargs
+        self, agregado: int, periodos: str, variavel: str = 'allxp', **kwargs
     ):
         self.url = (
             APIBASE
-            + f"agregados/{agregado}/periodos/{periodos}/variaveis/{variavel}?"
+            + f'agregados/{agregado}/periodos/{periodos}/variaveis/{variavel}?'
         )
-        self.url += "&".join([f"{k}={v}" for k, v in kwargs.items()])
+        self.url += '&'.join([f'{k}={v}' for k, v in kwargs.items()])
         self.JSON = None
         self._fetch_JSON()
 
     def _fetch_JSON(self):
         try:
-            print(f"Fetching {self.url}")
+            print(f'Fetching {self.url}')
             with (get_legacy_session() as s, s.get(self.url) as response):
                 self.JSON = response.json()
         except Exception as e:
             print(f"Couldn't download data:\n{e}")
 
     def to_dataframe(self):
         return pd.DataFrame(self.JSON)
@@ -281,9 +281,9 @@
         )
 
 
 def get_legacy_session():
     ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
     ctx.options |= 0x4  # OP_LEGACY_SERVER_CONNECT
     session = requests.session()
-    session.mount("https://", CustomHttpAdapter(ctx))
+    session.mount('https://', CustomHttpAdapter(ctx))
     return session
```

### Comparing `pysus-0.9.1/pysus/online_data/Infodengue.py` & `pysus-0.9.2/pysus/online_data/Infodengue.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 import pandas as pd
 import unidecode
 
 # from loguru import logger
 
 APP_DIR = Path(__file__).resolve(strict=True).parent.parent
-CID10 = {"dengue": "A90", "chikungunya": "A92.0", "zika": "A928"}
+CID10 = {'dengue': 'A90', 'chikungunya': 'A92.0', 'zika': 'A928'}
 
-with open(APP_DIR / "dataset/geocode_by_cities.json", "r") as f:
+with open(APP_DIR / 'dataset/geocode_by_cities.json', 'r') as f:
     geocode_by_cities = json.load(f)
 
 
 def normalize(s):
     for p in string.punctuation:
-        s = s.replace(p, "")
+        s = s.replace(p, '')
 
     return unidecode.unidecode(s.lower().strip())
 
 
 def search_string(substr: str) -> Dict[str, int]:
     """
     Fetch geocode of the city name matching to the substring.
@@ -35,30 +35,30 @@
         dict: Dictionary with key and values
             with city name and IBGE codes of all municipalities in Brazil
     """
     normalized_list = [normalize(f) for f in list(geocode_by_cities.keys())]
 
     matching_cities = [
         get_close_matches(i, normalized_list, n=55)
-        for i in normalize(substr).split(".")
+        for i in normalize(substr).split('.')
     ]
 
     return {
         key: geocode_by_cities[key]
         for key in geocode_by_cities
         if normalize(key) in list(*matching_cities)
     }
 
 
 def download(
     disease: str,
     eyw_start: int,
     eyw_end: int,
     city_name: str,
-    format="csv",
+    format='csv',
 ) -> pd.DataFrame:
     """
     Download InfoDengue API data by municipality and disease
         in the epidemiological week.
 
     Parameters
     ----------
@@ -73,42 +73,42 @@
         pd: Pandas dataframe
     """
 
     geocode = geocode_by_cities.get(city_name)
 
     if disease not in CID10.keys():
         raise Exception(
-            f"The diseases available are: {[k for k in CID10.keys()]}"
+            f'The diseases available are: {[k for k in CID10.keys()]}'
         )
     elif len(str(eyw_start)) != 6 or len(str(eyw_end)) != 6:
         raise Exception(
-            "The epidemiological week must contain 6 digits, "
-            "started in the year 2010 until 2022. Example: 202248"
+            'The epidemiological week must contain 6 digits, '
+            'started in the year 2010 until 2022. Example: 202248'
         )
     elif geocode is None:
         list_of_cities = search_string(city_name)
-        print(f"You must choose one of these city names: {list_of_cities}")
+        print(f'You must choose one of these city names: {list_of_cities}')
     else:
         s_yw = str(eyw_start)
         e_yw = str(eyw_end)
         ew_start, ey_start = s_yw[-2:], s_yw[:4]
         ew_end, ey_end = e_yw[-2:], e_yw[:4]
-        url = "https://info.dengue.mat.br/api/alertcity"
+        url = 'https://info.dengue.mat.br/api/alertcity'
         params = (
-            "&disease="
-            + f"{disease}"
-            + "&geocode="
-            + f"{geocode}"
-            + "&format="
-            + f"{format}"
-            + "&ew_start="
-            + f"{ew_start}"
-            + "&ew_end="
-            + f"{ew_end}"
-            + "&ey_start="
-            + f"{ey_start}"
-            + "&ey_end="
-            + f"{ey_end}"
+            '&disease='
+            + f'{disease}'
+            + '&geocode='
+            + f'{geocode}'
+            + '&format='
+            + f'{format}'
+            + '&ew_start='
+            + f'{ew_start}'
+            + '&ew_end='
+            + f'{ew_end}'
+            + '&ey_start='
+            + f'{ey_start}'
+            + '&ey_end='
+            + f'{ey_end}'
         )
 
-        url_resp = "?".join([url, params])
-        return pd.read_csv(url_resp, index_col="SE").T
+        url_resp = '?'.join([url, params])
+        return pd.read_csv(url_resp, index_col='SE').T
```

### Comparing `pysus-0.9.1/pysus/online_data/Infogripe.py` & `pysus-0.9.2/pysus/online_data/Infogripe.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pandas as pd
 
 BASEURL = r'https://gitlab.fiocruz.br/marcelo.gomes/infogripe/-/raw/master/Dados/InfoGripe/'
 DATASETS = {
     'Alerta de situação': r'tabela_de_alerta.csv',
     'Casos por idade, sexo e virus': r'dados_semanais_faixa_etaria_sexo_virus.csv.gz',
     'Casos Totais e estimativas': r'serie_temporal_com_estimativas_recentes.csv.gz',
-    'Valores esperados por localidades': 'valores_esperados_por_localidade.csv'
+    'Valores esperados por localidades': 'valores_esperados_por_localidade.csv',
 }
 
 
 def list_datasets():
     return list(DATASETS.keys())
```

### Comparing `pysus-0.9.1/pysus/online_data/PNI.py` & `pysus-0.9.2/pysus/online_data/PNI.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     """
     Download imunization records for a given States and years.
     :param state: uf two letter code, can be a list
     :param year: year in 4 digits, can be a list
     :param data_dir: directory where data will be downloaded
     :return: list of downloaded parquet paths
     """
-    return FTP_Downloader("PNI").download(
-        PNI_group="CPNI", UFs=states, years=years, local_dir=data_dir
+    return FTP_Downloader('PNI').download(
+        PNI_group='CPNI', UFs=states, years=years, local_dir=data_dir
     )
 
 
 def get_available_years(state):
     """
     Fetch available years (dbf names) for the `state`.
     :param state: uf code
     :return: list of strings (filenames)
     """
-    return FTP_Inspect("PNI").list_available_years(UF=state, PNI_group="CPNI")
+    return FTP_Inspect('PNI').list_available_years(UF=state, PNI_group='CPNI')
 
 
 def available_docs():
-    return FTP_Inspect("PNI").list_all(PNI_group="CPNI")
+    return FTP_Inspect('PNI').list_all(PNI_group='CPNI')
```

### Comparing `pysus-0.9.1/pysus/online_data/SIA.py` & `pysus-0.9.2/pysus/online_data/SIA.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,39 +8,39 @@
 """
 from pprint import pprint
 from typing import Dict, Tuple, Union
 
 from pysus.online_data import CACHEPATH, FTP_Downloader
 
 group_dict: Dict[str, Tuple[str, int, int]] = {
-    "PA": ("Produção Ambulatorial", 7, 1994),
-    "BI": ("Boletim de Produção Ambulatorial individualizado", 1, 2008),
-    "AD": ("APAC de Laudos Diversos", 1, 2008),
-    "AM": ("APAC de Medicamentos", 1, 2008),
-    "AN": ("APAC de Nefrologia", 1, 2008),
-    "AQ": ("APAC de Quimioterapia", 1, 2008),
-    "AR": ("APAC de Radioterapia", 1, 2008),
-    "AB": ("APAC de Cirurgia Bariátrica", 1, 2008),
-    "ACF": ("APAC de Confecção de Fístula", 1, 2008),
-    "ATD": ("APAC de Tratamento Dialítico", 1, 2008),
-    "AMP": ("APAC de Acompanhamento Multiprofissional", 1, 2008),
-    "SAD": ("RAAS de Atenção Domiciliar", 1, 2008),
-    "PS": ("RAAS Psicossocial", 1, 2008),
+    'PA': ('Produção Ambulatorial', 7, 1994),
+    'BI': ('Boletim de Produção Ambulatorial individualizado', 1, 2008),
+    'AD': ('APAC de Laudos Diversos', 1, 2008),
+    'AM': ('APAC de Medicamentos', 1, 2008),
+    'AN': ('APAC de Nefrologia', 1, 2008),
+    'AQ': ('APAC de Quimioterapia', 1, 2008),
+    'AR': ('APAC de Radioterapia', 1, 2008),
+    'AB': ('APAC de Cirurgia Bariátrica', 1, 2008),
+    'ACF': ('APAC de Confecção de Fístula', 1, 2008),
+    'ATD': ('APAC de Tratamento Dialítico', 1, 2008),
+    'AMP': ('APAC de Acompanhamento Multiprofissional', 1, 2008),
+    'SAD': ('RAAS de Atenção Domiciliar', 1, 2008),
+    'PS': ('RAAS Psicossocial', 1, 2008),
 }
 
 
 def show_datatypes():
     pprint(group_dict)
 
 
 def download(
     states: Union[str, list],
     years: Union[str, list, int],
     months: Union[str, list, int],
-    group: str = "PA",
+    group: str = 'PA',
     data_dir: str = CACHEPATH,
 ) -> list:
     """
     Download SIASUS records for state year and month and returns dataframe
     :param months: 1 to 12, can be a list
     :param states: 2 letter state code, can be a list
     :param years: 4 digit integer, can be a list
@@ -58,14 +58,14 @@
         ACF - APAC de Confecção de Fístula
         ATD - APAC de Tratamento Dialítico
         AMP - APAC de Acompanhamento Multiprofissional
         SAD - RAAS de Atenção Domiciliar
         PS - RAAS Psicossocial
     :return: list of downloaded parquet paths
     """
-    return FTP_Downloader("SIA").download(
+    return FTP_Downloader('SIA').download(
         UFs=states,
         years=years,
         months=months,
         local_dir=data_dir,
         SIA_group=group,
     )
```

### Comparing `pysus-0.9.1/pysus/online_data/SIH.py` & `pysus-0.9.2/pysus/online_data/SIH.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,14 @@
     Download SIH records for state year and month and returns dataframe
     :param months: 1 to 12, can be a list
     :param states: 2 letter state code, can be alist
     :param years: 4 digit integer, can be a list
     :param data_dir: Directory where parquets will be downloaded.
     :return: a list of parquet paths
     """
-    return FTP_Downloader("SIH").download(
+    return FTP_Downloader('SIH').download(
         UFs=states,
         years=years,
         months=months,
-        SIH_group="RD",
+        SIH_group='RD',
         local_dir=data_dir,
     )
```

### Comparing `pysus-0.9.1/pysus/online_data/SIM.py` & `pysus-0.9.2/pysus/online_data/SIM.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,239 +22,239 @@
     """
     Downloads data directly from Datasus ftp server
     :param states: two-letter state identifier: MG == Minas Gerais
                    can be a list
     :param years: 4 digit integer, can be a list
     :return: a list of downloaded parquet paths
     """
-    return FTP_Downloader("SIM").download(
+    return FTP_Downloader('SIM').download(
         UFs=states, years=years, local_dir=data_dir
     )
 
 
 def get_CID10_chapters_table(cache=True):
     """
     Fetch the CID10 chapters table
     :param cache: If set to True, stores data as parquets.
     :return: Pandas DataFrame
     """
-    ftp = FTP("ftp.datasus.gov.br")
+    ftp = FTP('ftp.datasus.gov.br')
     ftp.login()
     logger.debug(
-        f"Stablishing connection with ftp.datasus.gov.br.\n{ftp.welcome}"
+        f'Stablishing connection with ftp.datasus.gov.br.\n{ftp.welcome}'
     )
-    ftp.cwd("/dissemin/publicos/SIM/CID10/TABELAS")
+    ftp.cwd('/dissemin/publicos/SIM/CID10/TABELAS')
     logger.debug(
-        "Changing FTP work dir to: /dissemin/publicos/SIM/CID10/TABELAS"
+        'Changing FTP work dir to: /dissemin/publicos/SIM/CID10/TABELAS'
     )
 
-    fname = "CIDCAP10.DBF"
+    fname = 'CIDCAP10.DBF'
     cachefile = os.path.join(
-        CACHEPATH, "SIM_" + fname.split(".")[0] + "_.parquet"
+        CACHEPATH, 'SIM_' + fname.split('.')[0] + '_.parquet'
     )
 
     if os.path.exists(cachefile):
-        logger.info(f"Local parquet file found at {cachefile}")
+        logger.info(f'Local parquet file found at {cachefile}')
         df = pd.read_parquet(cachefile)
 
         return df
 
     try:
-        ftp.retrbinary("RETR {}".format(fname), open(fname, "wb").write)
+        ftp.retrbinary('RETR {}'.format(fname), open(fname, 'wb').write)
 
     except error_perm:
-        raise Exception("Could not download {}".format(fname))
+        raise Exception('Could not download {}'.format(fname))
 
-    dbf = DBF(fname, encoding="iso-8859-1")
+    dbf = DBF(fname, encoding='iso-8859-1')
     df = pd.DataFrame(list(dbf))
 
     if cache:
         df.to_parquet(cachefile)
-        logger.info(f"Data stored as parquet at {cachefile}")
+        logger.info(f'Data stored as parquet at {cachefile}')
 
     os.unlink(fname)
-    logger.debug(f"{fname} removed")
+    logger.debug(f'{fname} removed')
 
     return df
 
 
 def get_CID10_table(cache=True):
     """
     Fetch the CID10 table
     :param cache: If set to True, stores data as parquets.
     :return: Pandas DataFrame
     """
-    ftp = FTP("ftp.datasus.gov.br")
+    ftp = FTP('ftp.datasus.gov.br')
     ftp.login()
     logger.debug(
-        f"Stablishing connection with ftp.datasus.gov.br.\n{ftp.welcome}"
+        f'Stablishing connection with ftp.datasus.gov.br.\n{ftp.welcome}'
     )
-    ftp.cwd("/dissemin/publicos/SIM/CID10/TABELAS")
+    ftp.cwd('/dissemin/publicos/SIM/CID10/TABELAS')
     logger.debug(
-        "Changing FTP work dir to: /dissemin/publicos/SIM/CID10/TABELAS"
+        'Changing FTP work dir to: /dissemin/publicos/SIM/CID10/TABELAS'
     )
 
-    fname = "CID10.DBF"
+    fname = 'CID10.DBF'
     cachefile = os.path.join(
-        CACHEPATH, "SIM_" + fname.split(".")[0] + "_.parquet"
+        CACHEPATH, 'SIM_' + fname.split('.')[0] + '_.parquet'
     )
 
     if os.path.exists(cachefile):
-        logger.info(f"Local parquet file found at {cachefile}")
+        logger.info(f'Local parquet file found at {cachefile}')
         df = pd.read_parquet(cachefile)
 
         return df
 
     try:
-        ftp.retrbinary("RETR {}".format(fname), open(fname, "wb").write)
+        ftp.retrbinary('RETR {}'.format(fname), open(fname, 'wb').write)
 
     except error_perm:
-        raise Exception("Could not download {}".format(fname))
+        raise Exception('Could not download {}'.format(fname))
 
-    dbf = DBF(fname, encoding="iso-8859-1")
+    dbf = DBF(fname, encoding='iso-8859-1')
     df = pd.DataFrame(list(dbf))
 
     if cache:
         df.to_parquet(cachefile)
-        logger.info(f"Data stored as parquet at {cachefile}")
+        logger.info(f'Data stored as parquet at {cachefile}')
 
     os.unlink(fname)
-    logger.debug(f"{fname} removed")
+    logger.debug(f'{fname} removed')
 
     return df
 
 
 def get_CID9_table(cache=True):
     """
     Fetch the CID9 table
     :param cache: If set to True, stores data as parquets.
     :return: Pandas DataFrame
     """
-    ftp = FTP("ftp.datasus.gov.br")
+    ftp = FTP('ftp.datasus.gov.br')
     ftp.login()
     logger.debug(
-        f"Stablishing connection with ftp.datasus.gov.br.\n{ftp.welcome}"
+        f'Stablishing connection with ftp.datasus.gov.br.\n{ftp.welcome}'
     )
-    ftp.cwd("/dissemin/publicos/SIM/CID9/TABELAS")
+    ftp.cwd('/dissemin/publicos/SIM/CID9/TABELAS')
     logger.debug(
-        "Changing FTP work dir to: /dissemin/publicos/SIM/CID9/TABELAS"
+        'Changing FTP work dir to: /dissemin/publicos/SIM/CID9/TABELAS'
     )
 
-    fname = "CID9.DBF"
+    fname = 'CID9.DBF'
     cachefile = os.path.join(
-        CACHEPATH, "SIM_" + fname.split(".")[0] + "_.parquet"
+        CACHEPATH, 'SIM_' + fname.split('.')[0] + '_.parquet'
     )
 
     if os.path.exists(cachefile):
-        logger.info(f"Local parquet file found at {cachefile}")
+        logger.info(f'Local parquet file found at {cachefile}')
         df = pd.read_parquet(cachefile)
 
         return df
 
     try:
-        ftp.retrbinary("RETR {}".format(fname), open(fname, "wb").write)
+        ftp.retrbinary('RETR {}'.format(fname), open(fname, 'wb').write)
 
     except error_perm:
-        raise Exception("Could not download {}".format(fname))
+        raise Exception('Could not download {}'.format(fname))
 
-    dbf = DBF(fname, encoding="iso-8859-1")
+    dbf = DBF(fname, encoding='iso-8859-1')
     df = pd.DataFrame(list(dbf))
 
     if cache:
         df.to_parquet(cachefile)
-        logger.info(f"Data stored as parquet at {cachefile}")
+        logger.info(f'Data stored as parquet at {cachefile}')
 
     os.unlink(fname)
-    logger.debug(f"{fname} removed")
+    logger.debug(f'{fname} removed')
 
     return df
 
 
 def get_municipios(cache=True):
     """
     Get municipality metadata
     :param cache: If set to True, stores data as parquets.
     :return: Pandas DataFrame
     """
-    ftp = FTP("ftp.datasus.gov.br")
+    ftp = FTP('ftp.datasus.gov.br')
     ftp.login()
     logger.debug(
-        f"Stablishing connection with ftp.datasus.gov.br.\n{ftp.welcome}"
+        f'Stablishing connection with ftp.datasus.gov.br.\n{ftp.welcome}'
     )
-    ftp.cwd("/dissemin/publicos/SIM/CID10/TABELAS")
+    ftp.cwd('/dissemin/publicos/SIM/CID10/TABELAS')
     logger.debug(
-        "Changing FTP work dir to: /dissemin/publicos/SIM/CID10/TABELAS"
+        'Changing FTP work dir to: /dissemin/publicos/SIM/CID10/TABELAS'
     )
 
-    fname = "CADMUN.DBF"
+    fname = 'CADMUN.DBF'
     cachefile = os.path.join(
-        CACHEPATH, "SIM_" + fname.split(".")[0] + "_.parquet"
+        CACHEPATH, 'SIM_' + fname.split('.')[0] + '_.parquet'
     )
 
     if os.path.exists(cachefile):
-        logger.info(f"Local parquet file found at {cachefile}")
+        logger.info(f'Local parquet file found at {cachefile}')
         df = pd.read_parquet(cachefile)
 
         return df
 
     try:
-        ftp.retrbinary("RETR {}".format(fname), open(fname, "wb").write)
+        ftp.retrbinary('RETR {}'.format(fname), open(fname, 'wb').write)
 
     except:
-        raise Exception("Could not download {}".format(fname))
+        raise Exception('Could not download {}'.format(fname))
 
-    dbf = DBF(fname, encoding="iso-8859-1")
+    dbf = DBF(fname, encoding='iso-8859-1')
     df = pd.DataFrame(list(dbf))
 
     if cache:
         df.to_parquet(cachefile)
-        logger.info(f"Data stored as parquet at {cachefile}")
+        logger.info(f'Data stored as parquet at {cachefile}')
 
     os.unlink(fname)
-    logger.debug(f"{fname} removed")
+    logger.debug(f'{fname} removed')
 
     return df
 
 
 def get_ocupations(cache=True):
     """
     Fetch ocupations table
     :param cache: If set to True, stores data as parquets.
     :return: Pandas DataFrame
     """
-    ftp = FTP("ftp.datasus.gov.br")
+    ftp = FTP('ftp.datasus.gov.br')
     ftp.login()
     logger.debug(
-        f"Stablishing connection with ftp.datasus.gov.br.\n{ftp.welcome}"
+        f'Stablishing connection with ftp.datasus.gov.br.\n{ftp.welcome}'
     )
-    ftp.cwd("/dissemin/publicos/SIM/CID10/TABELAS")
+    ftp.cwd('/dissemin/publicos/SIM/CID10/TABELAS')
     logger.debug(
-        "Changing FTP work dir to: /dissemin/publicos/SIM/CID10/TABELAS"
+        'Changing FTP work dir to: /dissemin/publicos/SIM/CID10/TABELAS'
     )
-    fname = "TABOCUP.DBF"
+    fname = 'TABOCUP.DBF'
     cachefile = os.path.join(
-        CACHEPATH, "SIM_" + fname.split(".")[0] + "_.parquet"
+        CACHEPATH, 'SIM_' + fname.split('.')[0] + '_.parquet'
     )
 
     if os.path.exists(cachefile):
-        logger.info(f"Local parquet file found at {cachefile}")
+        logger.info(f'Local parquet file found at {cachefile}')
         df = pd.read_parquet(cachefile)
 
         return df
 
     try:
-        ftp.retrbinary("RETR {}".format(fname), open(fname, "wb").write)
+        ftp.retrbinary('RETR {}'.format(fname), open(fname, 'wb').write)
 
     except:
-        raise Exception("Could not download {}".format(fname))
+        raise Exception('Could not download {}'.format(fname))
 
-    dbf = DBF(fname, encoding="iso-8859-1")
+    dbf = DBF(fname, encoding='iso-8859-1')
     df = pd.DataFrame(list(dbf))
 
     if cache:
         df.to_parquet(cachefile)
-        logger.info(f"Data stored as parquet at {cachefile}")
+        logger.info(f'Data stored as parquet at {cachefile}')
 
     os.unlink(fname)
-    logger.debug(f"{fname} removed")
+    logger.debug(f'{fname} removed')
 
     return df
```

### Comparing `pysus-0.9.1/pysus/online_data/SINAN.py` & `pysus-0.9.2/pysus/online_data/SINAN.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,44 +11,44 @@
 
 def get_available_years(disease: str) -> list:
     """
     Fetch available years for data related to specific disease
     :param disease: Disease name. See `SINAN.list_diseases` for valid names
     :return: A list of DBC files from a specific disease found in the FTP Server.
     """
-    return FTP_Inspect("SINAN").list_available_years(SINAN_disease=disease)
+    return FTP_Inspect('SINAN').list_available_years(SINAN_disease=disease)
 
 
 def download(
     disease, years: Union[str, list, int], data_path: str = CACHEPATH
 ) -> list:
     """
     Downloads SINAN data directly from Datasus ftp server.
     :param disease: Disease according to `agravos`.
     :param years: 4 digit integer, can be a list of years.
     :param data_path: The directory where the chunks will be downloaded to.
     :return: list of downloaded parquet directories.
     """
-    return FTP_Downloader("SINAN").download(
+    return FTP_Downloader('SINAN').download(
         SINAN_disease=disease, years=years, local_dir=data_path
     )
 
 
 def metadata_df(disease: str) -> pd.DataFrame:
     code = FTP_SINAN(disease).code
     metadata_file = (
-        Path(__file__).parent.parent / "metadata" / "SINAN" / f"{code}.tar.gz"
+        Path(__file__).parent.parent / 'metadata' / 'SINAN' / f'{code}.tar.gz'
     )
     if metadata_file.exists():
         df = pd.read_csv(
             metadata_file,
-            compression="gzip",
+            compression='gzip',
             header=0,
-            sep=",",
+            sep=',',
             quotechar='"',
             error_bad_lines=False,
         )
 
         return df.iloc[:, 1:]
     else:
-        print(f"No metadata available for {disease}")
+        print(f'No metadata available for {disease}')
         return
```

### Comparing `pysus-0.9.1/pysus/online_data/__init__.py` & `pysus-0.9.2/pysus/online_data/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,50 +16,51 @@
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 from dbfread import DBF
 from pysus.utilities.readdbc import dbc2dbf
 
 CACHEPATH = os.getenv(
-    "PYSUS_CACHEPATH", os.path.join(str(Path.home()), "pysus")
+    'PYSUS_CACHEPATH', os.path.join(str(Path.home()), 'pysus')
 )
 
 # create pysus cache directory
 if not os.path.exists(CACHEPATH):
     os.mkdir(CACHEPATH)
 
 
 DB_PATHS = {
-    "SINAN": [
-        "/dissemin/publicos/SINAN/DADOS/FINAIS",
-        "/dissemin/publicos/SINAN/DADOS/PRELIM",
+    'SINAN': [
+        '/dissemin/publicos/SINAN/DADOS/FINAIS',
+        '/dissemin/publicos/SINAN/DADOS/PRELIM',
     ],
-    "SIM": [
-        "/dissemin/publicos/SIM/CID10/DORES",
-        "/dissemin/publicos/SIM/CID9/DORES",
+    'SIM': [
+        '/dissemin/publicos/SIM/CID10/DORES',
+        '/dissemin/publicos/SIM/CID9/DORES',
     ],
-    "SINASC": [
-        "/dissemin/publicos/SINASC/NOV/DNRES",
-        "/dissemin/publicos/SINASC/ANT/DNRES",
+    'SINASC': [
+        '/dissemin/publicos/SINASC/NOV/DNRES',
+        '/dissemin/publicos/SINASC/ANT/DNRES',
     ],
-    "SIH": [
-        "/dissemin/publicos/SIHSUS/199201_200712/Dados",
-        "/dissemin/publicos/SIHSUS/200801_/Dados",
+    'SIH': [
+        '/dissemin/publicos/SIHSUS/199201_200712/Dados',
+        '/dissemin/publicos/SIHSUS/200801_/Dados',
     ],
-    "SIA": [
-        "/dissemin/publicos/SIASUS/199407_200712/Dados",
-        "/dissemin/publicos/SIASUS/200801_/Dados",
+    'SIA': [
+        '/dissemin/publicos/SIASUS/199407_200712/Dados',
+        '/dissemin/publicos/SIASUS/200801_/Dados',
     ],
-    "PNI": ["/dissemin/publicos/PNI/DADOS"],
-    "CNES": ["dissemin/publicos/CNES/200508_/Dados"],
-    "CIHA": ["/dissemin/publicos/CIHA/201101_/Dados"],
+    'PNI': ['/dissemin/publicos/PNI/DADOS'],
+    'CNES': ['dissemin/publicos/CNES/200508_/Dados'],
+    'CIHA': ['/dissemin/publicos/CIHA/201101_/Dados'],
 }
 
+
 def FTP_datasus():
-    ftp = FTP("ftp.datasus.gov.br")
+    ftp = FTP('ftp.datasus.gov.br')
     ftp.login()
     return ftp
 
 
 def cache_contents():
     """
     List the files currently cached in ~/pysus
@@ -75,31 +76,31 @@
     """
     Receives a parquet directory path and returns it as a
     dataframe, trying to clean white spaces and convert to
     the correct data types. Can read only one parquet dir
     at time.
     """
 
-    parquets = list(map(str, Path(parquet_dir).glob("*.parquet")))
-    
+    parquets = list(map(str, Path(parquet_dir).glob('*.parquet')))
+
     try:
         chunks_list = [
-            pd.read_parquet(str(f), engine="fastparquet") for f in parquets
+            pd.read_parquet(str(f), engine='fastparquet') for f in parquets
         ]
         df = pd.concat(chunks_list, ignore_index=True)
 
         return _parse_dftypes(df)
 
     except Exception as e:
         logging.error(e)
 
     finally:
         if clean_after_read:
             shutil.rmtree(parquet_dir)
-            logging.info(f"{parquet_dir} removed")
+            logging.info(f'{parquet_dir} removed')
 
 
 def _parse_dftypes(df: pd.DataFrame) -> pd.DataFrame:
     """
     Parse DataFrame values, cleaning blank spaces if needed
     and converting dtypes into correct types.
     """
@@ -108,31 +109,31 @@
         # Maps a function to each value in each column
         columns = [c for c in df.columns if c in column_names]
         df[columns] = df[columns].applymap(func)
 
     def str_to_int(string: str) -> Union[int, float]:
         # If removing spaces, all characters are int,
         # return int(value). @warning it removes in between
-        # spaces as wel 
-        if str(string).replace(" ", "").isnumeric():
-            return int(string.replace(" ", ""))
+        # spaces as wel
+        if str(string).replace(' ', '').isnumeric():
+            return int(string.replace(' ', ''))
 
     def str_to_date(string: str) -> datetime.date:
         if isinstance(string, str):
             try:
-                return datetime.strptime(string, "%Y%m%d").date()
+                return datetime.strptime(string, '%Y%m%d').date()
             except Exception:
                 # Ignore errors, bad value
                 pass
 
-    map_column_func(["DT_NOTIFIC", "DT_SIN_PRI"], str_to_date)
-    map_column_func(["CODMUNRES", "SEXO"], str_to_int)
+    map_column_func(['DT_NOTIFIC', 'DT_SIN_PRI'], str_to_date)
+    map_column_func(['CODMUNRES', 'SEXO'], str_to_int)
 
     df = df.applymap(
-        lambda x: "" if str(x).isspace() else x
+        lambda x: '' if str(x).isspace() else x
     )  # Remove all space values
 
     df = df.convert_dtypes()
     return df
 
 
 class FTP_Inspect:
@@ -151,211 +152,211 @@
 
     list_all: Will list all DBC or DBF urls found on the FTP server
                     for the Database. Groups may be also required.
     """
 
     database: str
     _ds_paths: list
-    ftp_server: FTP = FTP("ftp.datasus.gov.br")
+    ftp_server: FTP = FTP('ftp.datasus.gov.br')
     available_dbs: list = list(DB_PATHS.keys())
 
     def __init__(self, database: str) -> None:
         self.database = self.__checkdatabase__(database)
         self._ds_paths = DB_PATHS[database]
 
     def __checkdatabase__(self, database):
         if database not in self.available_dbs:
             raise ValueError(
-                f"{database} not found"
-                f" available databases: {self.available_dbs}"
+                f'{database} not found'
+                f' available databases: {self.available_dbs}'
             )
         return database
 
     def last_update_df(self) -> pd.DataFrame:  # Legacy
         """
         Return the date of last update from the database specified.
 
         Parameters
         ----------
         database: Database to check
         """
         if self.database not in DB_PATHS:
             print(
-                f"Database {self.database} not supported try one of these"
-                "{list(DB_PATHS.keys())}"
+                f'Database {self.database} not supported try one of these'
+                '{list(DB_PATHS.keys())}'
             )
             return pd.DataFrame()
 
         ftp = FTP_datasus()
         response = {
-            "folder": [],
-            "date": [],
-            "file_size": [],
-            "file_name": [],
+            'folder': [],
+            'date': [],
+            'file_size': [],
+            'file_name': [],
         }
 
         def parse(line):
             data = line.strip().split()
-            response["folder"].append(pth)
-            response["date"].append(
-                pd.to_datetime(" ".join([data[0], data[1]]))
+            response['folder'].append(pth)
+            response['date'].append(
+                pd.to_datetime(' '.join([data[0], data[1]]))
             )
-            response["file_size"].append(
-                0 if data[2] == "<DIR>" else int(data[2])
+            response['file_size'].append(
+                0 if data[2] == '<DIR>' else int(data[2])
             )
-            response["file_name"].append(data[3])
+            response['file_name'].append(data[3])
 
         for pth in DB_PATHS[self.database]:
             ftp.cwd(pth)
-            flist = ftp.retrlines("LIST", parse)
-        
+            flist = ftp.retrlines('LIST', parse)
+
         ftp.close()
         return pd.DataFrame(response)
 
     def list_available_years(
         self,
         UF: str = None,
         SINAN_disease: str = None,
         CNES_group: str = None,
-        SIA_group: str = "PA",
-        PNI_group: str = "CPNI",
-        SIH_group: str = "RD",
+        SIA_group: str = 'PA',
+        PNI_group: str = 'CPNI',
+        SIH_group: str = 'RD',
     ):
         """
         Uses `list_all` and filters according to UF, disease (SINAN),
         or Database group if group is required.
         """
         available_years = set()
         get_filename = (
             lambda x: str(x)
-            .split("/")[-1]
+            .split('/')[-1]
             .upper()
-            .split(".DBC")[0]
-            .split(".DBF")[0]
+            .split('.DBC')[0]
+            .split('.DBF')[0]
         )  # Trim url paths
 
         def list_years(
             len_group: int, fslice: slice = slice(-2, None), **kwargs
         ):
             return [
                 available_years.add(get_filename(path)[fslice])
                 for path in self.list_all(**kwargs)
                 if UF in get_filename(path)[len_group:]
             ]
 
         if UF is not None and len(UF) > 2:
-            raise ValueError("Use UF abbreviation. Eg: RJ")
+            raise ValueError('Use UF abbreviation. Eg: RJ')
 
         # SINAN
-        if self.database == "SINAN":
+        if self.database == 'SINAN':
             if not SINAN_disease:
-                raise ValueError("No disease assigned to SINAN_disease")
+                raise ValueError('No disease assigned to SINAN_disease')
             dis = FTP_SINAN(SINAN_disease)
-            available_years = dis.get_years(stage="all")
+            available_years = dis.get_years(stage='all')
         # SINASC
-        elif self.database == "SINASC":
+        elif self.database == 'SINASC':
             list_years(2)
         # SIH
-        elif self.database == "SIH":
+        elif self.database == 'SIH':
             list_years(len(SIH_group), slice(-4, -2), SIH_group=SIH_group)
 
         # SIA
-        elif self.database == "SIA":
+        elif self.database == 'SIA':
             list_years(len(SIA_group), slice(-4, -2), SIA_group=SIA_group)
         # CNES
-        elif self.database == "CNES":
+        elif self.database == 'CNES':
             list_years(len(CNES_group), slice(-4, -2), CNES_group=CNES_group)
         # PNI
-        elif self.database == "PNI":
+        elif self.database == 'PNI':
             list_years(len(PNI_group), PNI_group=PNI_group)
         # CIHA
-        elif self.database == "CIHA":
+        elif self.database == 'CIHA':
             list_years(4)
         # SIM
-        elif self.database == "SIM":
+        elif self.database == 'SIM':
             dbcs = self.list_all()
             available_years = set()
             for path in dbcs:
-                if "/CID9/" in path:
+                if '/CID9/' in path:
                     available_years.add(get_filename(path)[-2:]) if str(path)[
                         -8:-6
                     ] == UF else None
-                elif "/CID10/" in path:
+                elif '/CID10/' in path:
                     available_years.add(get_filename(path)[-2:]) if str(path)[
                         -10:-8
                     ] == UF else None
 
         # Normalize years to {year:04d} and return sorted
         cur_year = str(datetime.now().year)[-2:]
         bef_2000 = lambda yrs: [
-            "19" + y for y in yrs if y > cur_year and y <= "99"
+            '19' + y for y in yrs if y > cur_year and y <= '99'
         ]
         aft_2000 = lambda yrs: [
-            "20" + y for y in yrs if y <= cur_year and y >= "00"
+            '20' + y for y in yrs if y <= cur_year and y >= '00'
         ]
         return sorted(bef_2000(available_years)) + sorted(
             aft_2000(available_years)
         )
 
     def list_all(
         self,
         SINAN_disease: str = None,
         CNES_group: str = None,
-        SIA_group: str = "PA",
-        PNI_group: str = "CPNI",
-        SIH_group: str = "RD",
+        SIA_group: str = 'PA',
+        PNI_group: str = 'CPNI',
+        SIH_group: str = 'RD',
     ) -> list:
         """
         Enters FTP server and lists all DBCs or DBFs files found for a
         Database group. Some Database require groups and SINAN DB requires
         a disease, more details can be found in their modules.
         This method will be later used to download these files into parquets
         chunks, to preserve memory, that are read using pandas and pyarrow.
         """
         available_dbs = list()
-        ftp = FTP("ftp.datasus.gov.br")
+        ftp = FTP('ftp.datasus.gov.br')
         ftp.login()
         for path in self._ds_paths:
             try:
                 # CNES
-                if self.database == "CNES":
+                if self.database == 'CNES':
                     if not CNES_group:
-                        raise ValueError(f"No group assigned to CNES_group")
+                        raise ValueError(f'No group assigned to CNES_group')
                     available_dbs.extend(
-                        ftp.nlst(f"{path}/{CNES_group}/*.DBC")
+                        ftp.nlst(f'{path}/{CNES_group}/*.DBC')
                     )
                 # SIA
-                elif self.database == "SIA":
+                elif self.database == 'SIA':
                     if not SIA_group:
-                        raise ValueError(f"No group assigned to SIA_group")
-                    available_dbs.extend(ftp.nlst(f"{path}/{SIA_group}*.DBC"))
+                        raise ValueError(f'No group assigned to SIA_group')
+                    available_dbs.extend(ftp.nlst(f'{path}/{SIA_group}*.DBC'))
                 # SIH
-                elif self.database == "SIH":
+                elif self.database == 'SIH':
                     if not SIH_group:
-                        raise ValueError(f"No group assigned to SIH_group")
-                    available_dbs.extend(ftp.nlst(f"{path}/{SIH_group}*.DBC"))
+                        raise ValueError(f'No group assigned to SIH_group')
+                    available_dbs.extend(ftp.nlst(f'{path}/{SIH_group}*.DBC'))
                 # PNI
-                elif self.database == "PNI":
+                elif self.database == 'PNI':
                     if not PNI_group:
-                        raise ValueError(f"No group assigned to PNI_group")
-                    available_dbs.extend(ftp.nlst(f"{path}/{PNI_group}*.DBF"))
+                        raise ValueError(f'No group assigned to PNI_group')
+                    available_dbs.extend(ftp.nlst(f'{path}/{PNI_group}*.DBF'))
                 # SINAN
-                elif self.database == "SINAN":
+                elif self.database == 'SINAN':
                     if not SINAN_disease:
                         raise ValueError(
-                            f"No disease assigned to SINAN_disease"
+                            f'No disease assigned to SINAN_disease'
                         )
                     disease = FTP_SINAN(SINAN_disease)
                     available_dbs = disease.get_ftp_paths(
-                        disease.get_years(stage="all")
+                        disease.get_years(stage='all')
                     )
                 # SIM, SINASC
                 else:
                     available_dbs.extend(
-                        ftp.nlst(f"{path}/*.DBC")  # case insensitive
+                        ftp.nlst(f'{path}/*.DBC')  # case insensitive
                     )
             except Exception as e:
                 raise e
         ftp.close()
         return available_dbs
 
 
@@ -394,17 +395,17 @@
     def download(
         self,
         UFs: Union[str, list] = None,
         years: Union[str, int, list] = None,
         months: Union[str, int, list] = None,
         SINAN_disease: str = None,
         CNES_group: str = None,
-        SIA_group: str = "PA",
-        SIH_group: str = "RD",
-        PNI_group: str = "CPNI",
+        SIA_group: str = 'PA',
+        SIH_group: str = 'RD',
+        PNI_group: str = 'CPNI',
         local_dir: str = cache_dir,
     ) -> Union[tuple[str], str]:
         dbc_paths = self._get_dbc_paths(
             UFs=UFs,
             years=years,
             months=months,
             SINAN_disease=SINAN_disease,
@@ -414,112 +415,113 @@
             PNI_group=PNI_group,
         )
         data_dir = Path(local_dir)
 
         downloaded_parquets = []
         for path in dbc_paths:
 
-            parquet_dir = data_dir / str(path).split("/")[-1].upper().replace(
-                ".DBC", ".parquet"
+            parquet_dir = data_dir / str(path).split('/')[-1].upper().replace(
+                '.DBC', '.parquet'
             )
 
             if Path(parquet_dir).exists():
                 downloaded_parquets.append(str(parquet_dir))
             else:
                 local_filepath = self._extract_dbc(path, local_dir=local_dir)
                 parquet_dir = self._dbfc_to_parquets(
                     local_filepath, local_dir=local_dir
                 )
                 downloaded_parquets.append(str(parquet_dir))
         return (
-            downloaded_parquets[0] 
-            if len(downloaded_parquets) == 1 
+            downloaded_parquets[0]
+            if len(downloaded_parquets) == 1
             else tuple(downloaded_parquets)
         )
 
     def _get_dbc_paths(
         self,
         UFs: Union[str, list] = None,
         years: Union[str, int, list] = None,
         months: Union[str, int, list] = None,
         SINAN_disease: str = None,
         CNES_group: str = None,
-        SIA_group: str = "PA",
-        SIH_group: str = "RD",
-        PNI_group: str = "CPNI",
+        SIA_group: str = 'PA',
+        SIH_group: str = 'RD',
+        PNI_group: str = 'CPNI',
     ) -> list:
         parse_to_list = lambda ite: [ite] if not isinstance(ite, list) else ite
         UFs = parse_to_list(UFs)
         years = parse_to_list(years)
         months = parse_to_list(months)
 
         db = self._ftp_db.database
         list_files = self._ftp_db.list_all
-        if db == "SINAN":
+        if db == 'SINAN':
             all_dbcs = list_files(SINAN_disease=SINAN_disease)
             sinan_dis = FTP_SINAN(SINAN_disease)
-        elif db == "CNES":
+        elif db == 'CNES':
             all_dbcs = list_files(CNES_group=CNES_group)
-        elif db == "SIA":
+        elif db == 'SIA':
             all_dbcs = list_files(SIA_group=SIA_group)
-        elif db == "SIH":
+        elif db == 'SIH':
             all_dbcs = list_files(SIH_group=SIH_group)
-        elif db == "PNI":
+        elif db == 'PNI':
             all_dbcs = list_files(PNI_group=PNI_group)
         else:
             all_dbcs = list_files()
 
         def url_regex(
             month: str = None, year: str = None, UF: str = None
         ) -> re.Pattern:
             """
             Each url case is matched using regex patterns, mostly databases
             have the same file pattern, but some discrepancies can be found,
             for instance, lowercase UF and entire years and shortened years
             at the same time.
             """
-            if db == "SINAN":
+            if db == 'SINAN':
                 if not year:
-                    raise ValueError("Missing year(s)")
+                    raise ValueError('Missing year(s)')
                 file_pattern = re.compile(
-                    f"{sinan_dis.code}BR{year}.dbc", re.I
+                    f'{sinan_dis.code}BR{year}.dbc', re.I
                 )
-            elif db == "SIM" or db == "SINASC":
+            elif db == 'SIM' or db == 'SINASC':
                 if not year or not UF:
-                    raise ValueError("Missing year(s) or UF(s)")
+                    raise ValueError('Missing year(s) or UF(s)')
                 file_pattern = re.compile(
-                    rf"[DON]+R?{UF}\d?\d?{year}.dbc", re.I
+                    rf'[DON]+R?{UF}\d?\d?{year}.dbc', re.I
                 )
-            elif db == "SIH":
+            elif db == 'SIH':
                 if not year or not month or not UF:
-                    raise ValueError("Missing year(s), month(s) or UF(s)")
+                    raise ValueError('Missing year(s), month(s) or UF(s)')
                 file_pattern = re.compile(
-                    rf"{SIH_group}{UF}{year}{month}.dbc", re.I
+                    rf'{SIH_group}{UF}{year}{month}.dbc', re.I
                 )
-            elif db == "SIA":
+            elif db == 'SIA':
                 if not year or not month or not UF:
-                    raise ValueError("Missing year(s), month(s) or UF(s)")
+                    raise ValueError('Missing year(s), month(s) or UF(s)')
                 file_pattern = re.compile(
-                    rf"{SIA_group}{UF}{year}{month}[abc]?.dbc", re.I
+                    rf'{SIA_group}{UF}{year}{month}[abc]?.dbc', re.I
                 )
-            elif db == "PNI":
+            elif db == 'PNI':
                 if not year or not UF:
-                    raise ValueError("Missing year(s) or UF(s)")
-                file_pattern = re.compile(rf"{PNI_group}{UF}{year}.dbf", re.I)
-            elif db == "CNES":
+                    raise ValueError('Missing year(s) or UF(s)')
+                file_pattern = re.compile(rf'{PNI_group}{UF}{year}.dbf', re.I)
+            elif db == 'CNES':
                 if not year or not month or not UF:
-                    raise ValueError("Missing year(s), month(s) or UF(s)")
+                    raise ValueError('Missing year(s), month(s) or UF(s)')
                 file_pattern = re.compile(
-                    rf"{CNES_group}/{CNES_group}{UF}{year}{month}.dbc", re.I
+                    rf'{CNES_group}/{CNES_group}{UF}{year}{month}.dbc', re.I
                 )
-            elif db == "CIHA":
+            elif db == 'CIHA':
                 if not year or not month or not UF:
-                    raise ValueError("Missing year(s), month(s) or UF(s)")
-                file_pattern = re.compile(rf"CIHA{UF}{year}{month}.dbc", re.I)
+                    raise ValueError('Missing year(s), month(s) or UF(s)')
+                file_pattern = re.compile(rf'CIHA{UF}{year}{month}.dbc', re.I)
             return file_pattern
+
         files = list()
         for y, m, uf in product(
             years or [], months or [], UFs or []
         ):  # Allows None
             norm = lambda y: str(y)[-2:].zfill(2)
             regex = url_regex(year=norm(y), month=norm(m), UF=str(uf))
             filtered = list(filter(regex.search, all_dbcs))
@@ -528,63 +530,63 @@
 
     def _extract_dbc(self, DBC_path: str, local_dir: str = cache_dir) -> str:
         """
         Enters in the FTP server and retrieve the DBC(F) path into
         local machine.
         """
         Path(local_dir).mkdir(exist_ok=True, parents=True)
-        filename = DBC_path.split("/")[-1]
-        filedir = DBC_path.replace(filename, "")
+        filename = DBC_path.split('/')[-1]
+        filedir = DBC_path.replace(filename, '')
         filepath = Path(local_dir) / filename
         if Path(filepath).exists():
             return str(filepath)
         try:
-            ftp = ftp = FTP("ftp.datasus.gov.br")
+            ftp = ftp = FTP('ftp.datasus.gov.br')
             ftp.login()
             ftp.cwd(filedir)
             ftp.retrbinary(
-                f"RETR {filename}",
-                open(f"{filepath}", "wb").write,
+                f'RETR {filename}',
+                open(f'{filepath}', 'wb').write,
             )
             ftp.close()
             return str(filepath)
         except error_perm as e:
-            logging.error(f"Not able to download {filename}")
+            logging.error(f'Not able to download {filename}')
             raise e
 
     def _dbfc_to_parquets(self, fpath: str, local_dir: str) -> str(PosixPath):
         """DBC/DBF files to parquets using Pandas & PyArrow"""
         db_path = Path(local_dir) / fpath
-        dbfile = str(db_path.absolute()).split("/")[-1]
-        if Path(dbfile).suffix in [".dbc", ".DBC"] and db_path.exists():
-            outpath = f"{fpath[:-4]}.dbf"
+        dbfile = str(db_path.absolute()).split('/')[-1]
+        if Path(dbfile).suffix in ['.dbc', '.DBC'] and db_path.exists():
+            outpath = f'{fpath[:-4]}.dbf'
             try:
                 dbc2dbf(fpath, outpath)
                 if Path(fpath).exists():
                     Path(fpath).unlink()
                 fpath = outpath
             except Exception as e:
                 logging.error(e)
                 raise e
 
-        parquet_dir = f"{fpath[:-4]}.parquet"
+        parquet_dir = f'{fpath[:-4]}.parquet'
         if Path(parquet_dir).exists() and any(os.listdir(parquet_dir)):
             return parquet_dir
         Path(parquet_dir).mkdir(exist_ok=True, parents=True)
 
         def decode_column(value):
             # https://stackoverflow.com/questions/57371164/django-postgres-a-string-literal-cannot-contain-nul-0x00-characters
             if isinstance(value, bytes):
-                return value.decode(encoding="iso-8859-1").replace("\x00", "")
+                return value.decode(encoding='iso-8859-1').replace('\x00', '')
             elif isinstance(value, str):
-                return str(value).replace("\x00", "")
+                return str(value).replace('\x00', '')
             else:
                 return value
 
-        for d in self._stream_DBF(DBF(fpath, encoding="iso-8859-1", raw=True)):
+        for d in self._stream_DBF(DBF(fpath, encoding='iso-8859-1', raw=True)):
             try:
                 df = pd.DataFrame(d)
                 table = pa.Table.from_pandas(df.applymap(decode_column))
                 pq.write_to_dataset(table, root_path=parquet_dir)
 
             except Exception as e:
                 logging.error(e)
@@ -608,95 +610,95 @@
         else:
             yield data
 
 
 class FTP_SINAN:
     name: str
     diseases: dict = {
-        "Animais Peçonhentos": "ANIM",
-        "Botulismo": "BOTU",
-        "Cancer": "CANC",
-        "Chagas": "CHAG",
-        "Chikungunya": "CHIK",
-        "Colera": "COLE",
-        "Coqueluche": "COQU",
-        "Contact Communicable Disease": "ACBI",
-        "Acidentes de Trabalho": "ACGR",
-        "Dengue": "DENG",
-        "Difteria": "DIFT",
-        "Esquistossomose": "ESQU",
-        "Febre Amarela": "FAMA",
-        "Febre Maculosa": "FMAC",
-        "Febre Tifoide": "FTIF",
-        "Hanseniase": "HANS",
-        "Hantavirose": "HANT",
-        "Hepatites Virais": "HEPA",
-        "Intoxicação Exógena": "IEXO",
-        "Leishmaniose Visceral": "LEIV",
-        "Leptospirose": "LEPT",
-        "Leishmaniose Tegumentar": "LTAN",
-        "Malaria": "MALA",
-        "Meningite": "MENI",
-        "Peste": "PEST",
-        "Poliomielite": "PFAN",
-        "Raiva Humana": "RAIV",
-        "Sífilis Adquirida": "SIFA",
-        "Sífilis Congênita": "SIFC",
-        "Sífilis em Gestante": "SIFG",
-        "Tétano Acidental": "TETA",
-        "Tétano Neonatal": "TETN",
-        "Tuberculose": "TUBE",
-        "Violência Domestica": "VIOL",
-        "Zika": "ZIKA",
+        'Animais Peçonhentos': 'ANIM',
+        'Botulismo': 'BOTU',
+        'Cancer': 'CANC',
+        'Chagas': 'CHAG',
+        'Chikungunya': 'CHIK',
+        'Colera': 'COLE',
+        'Coqueluche': 'COQU',
+        'Contact Communicable Disease': 'ACBI',
+        'Acidentes de Trabalho': 'ACGR',
+        'Dengue': 'DENG',
+        'Difteria': 'DIFT',
+        'Esquistossomose': 'ESQU',
+        'Febre Amarela': 'FAMA',
+        'Febre Maculosa': 'FMAC',
+        'Febre Tifoide': 'FTIF',
+        'Hanseniase': 'HANS',
+        'Hantavirose': 'HANT',
+        'Hepatites Virais': 'HEPA',
+        'Intoxicação Exógena': 'IEXO',
+        'Leishmaniose Visceral': 'LEIV',
+        'Leptospirose': 'LEPT',
+        'Leishmaniose Tegumentar': 'LTAN',
+        'Malaria': 'MALA',
+        'Meningite': 'MENI',
+        'Peste': 'PEST',
+        'Poliomielite': 'PFAN',
+        'Raiva Humana': 'RAIV',
+        'Sífilis Adquirida': 'SIFA',
+        'Sífilis Congênita': 'SIFC',
+        'Sífilis em Gestante': 'SIFG',
+        'Tétano Acidental': 'TETA',
+        'Tétano Neonatal': 'TETN',
+        'Tuberculose': 'TUBE',
+        'Violência Domestica': 'VIOL',
+        'Zika': 'ZIKA',
     }
 
     def __init__(self, name: str) -> None:
         self.name = self.__diseasecheck__(name)
         ftp = FTP_datasus()
         code = self.diseases[self.name]
         self.finals = ftp.nlst(f"{DB_PATHS['SINAN'][0]}/{code}BR*.dbc")
         self.prelims = ftp.nlst(f"{DB_PATHS['SINAN'][1]}/{code}BR*.dbc")
 
     def __diseasecheck__(self, name: str) -> str:
         return (
             name
             if name in self.diseases.keys()
-            else ValueError(f"{name} not found.")
+            else ValueError(f'{name} not found.')
         )
 
     def __repr__(self) -> str:
-        return f"SINAN Disease ({self.name})"
+        return f'SINAN Disease ({self.name})'
 
     def __str__(self) -> str:
         return self.name
 
     @property
     def code(self) -> str:
         return self.diseases[self.name]
 
-    def get_years(self, stage: str = "all") -> list:
+    def get_years(self, stage: str = 'all') -> list:
         """
         Returns the available years to download, if no stage
         is assigned, it will return years from both finals and
         preliminaries datasets.
         stage (str): 'finais' | 'prelim' | 'all'
         """
 
         def extract_years(paths):
             return [
-                str(path).split("/")[-1].split(".dbc")[0][-2:]
+                str(path).split('/')[-1].split('.dbc')[0][-2:]
                 for path in paths
             ]
 
         prelim_years = extract_years(self.prelims)
         finais_years = extract_years(self.finals)
 
-        if stage == "prelim":
+        if stage == 'prelim':
             return sorted(prelim_years)
-        elif stage == "finais":
+        elif stage == 'finais':
             return sorted(finais_years)
         return sorted(prelim_years + finais_years)
 
     def get_ftp_paths(self, years: list) -> list:
         """
         Returns the FTP path available for years to download.
         years (list): a list with years to download, if year
```

### Comparing `pysus-0.9.1/pysus/online_data/sinasc.py` & `pysus-0.9.2/pysus/online_data/sinasc.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,14 @@
     """
     Downloads data directly from Datasus ftp server
     :param state: two-letter state identifier: MG == Minas Gerais,
                   can be a list
     :param year: 4 digit integer, can be a list
     :return: list of downloaded parquet paths
     """
-    return FTP_Downloader("SINASC").download(
+    return FTP_Downloader('SINASC').download(
         UFs=states, years=years, local_dir=data_dir
     )
 
 
 def get_available_years(state):
-    return FTP_Inspect("SINASC").list_available_years(UF=state)
+    return FTP_Inspect('SINASC').list_available_years(UF=state)
```

### Comparing `pysus-0.9.1/pysus/online_data/vaccine.py` & `pysus-0.9.2/pysus/online_data/vaccine.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,99 +20,99 @@
 def download_covid(uf=None, only_header=False):
     """
     Download covid vaccination data for a give UF
     :param uf: 'RJ' | 'SP', etc.
     :param only_header: Used to see the header of the data before downloading.
     :return: dataframe iterator as returned by pandas `read_csv('Vaccine_temp_<uf>.csv.gz', chunksize=5000)`
     """
-    user = "imunizacao_public"
-    pwd = "qlto5t&7r_@+#Tlstigi"
-    index = "desc-imunizacao"
-    url = f"https://imunizacao-es.saude.gov.br/_search?scroll=1m"
+    user = 'imunizacao_public'
+    pwd = 'qlto5t&7r_@+#Tlstigi'
+    index = 'desc-imunizacao'
+    url = f'https://imunizacao-es.saude.gov.br/_search?scroll=1m'
     if uf is None:
-        query = {"query": {"match_all": {}}, "size": 10000}
-        UF = "BR"
+        query = {'query': {'match_all': {}}, 'size': 10000}
+        UF = 'BR'
     else:
         UF = uf.upper()
         query = {
-            "query": {"match": {"paciente_endereco_uf": UF}},
-            "size": 10000,
+            'query': {'match': {'paciente_endereco_uf': UF}},
+            'size': 10000,
         }
 
-    logger.info(f"Searching for COVID data of {UF}")
-    tempfile = os.path.join(CACHEPATH, f"Vaccine_temp_{UF}.csv.gz")
+    logger.info(f'Searching for COVID data of {UF}')
+    tempfile = os.path.join(CACHEPATH, f'Vaccine_temp_{UF}.csv.gz')
     if os.path.exists(tempfile):
         print(
-            "loading from cache. Returning an iterator of Dataframes in chunks of 5000."
+            'loading from cache. Returning an iterator of Dataframes in chunks of 5000.'
         )
         return pd.read_csv(tempfile, chunksize=5000)
 
     auth = HTTPBasicAuth(user, pwd)
     data_gen = elasticsearch_fetch(url, auth, query)
 
     if only_header:
         df = pd.DataFrame(next(data_gen))
         logger.warning(
-            f"Downloading data sample for visualization of {df.shape[0]} rows..."
+            f'Downloading data sample for visualization of {df.shape[0]} rows...'
         )
         return df
 
     h = 1
     for dt in data_gen:
         df = pd.DataFrame(dt)
         if h:
             df.to_csv(tempfile)
             h = 0
         else:
-            df.to_csv(tempfile, mode="a", header=False)
+            df.to_csv(tempfile, mode='a', header=False)
 
-    logger.info(f"{tempfile} stored at {CACHEPATH}.")
+    logger.info(f'{tempfile} stored at {CACHEPATH}.')
     df = pd.read_csv(tempfile, chunksize=5000)
 
     return df
 
 
 def elasticsearch_fetch(uri, auth, json_body={}):
     headers = {
-        "Content-Type": "application/json",
+        'Content-Type': 'application/json',
     }
 
-    scroll_id = ""
+    scroll_id = ''
     total = 0
     while True:
         if scroll_id:
-            uri = "https://imunizacao-es.saude.gov.br/_search/scroll"
-            json_body["scroll_id"] = scroll_id
-            json_body["scroll"] = "1m"
-            if "query" in json_body:
+            uri = 'https://imunizacao-es.saude.gov.br/_search/scroll'
+            json_body['scroll_id'] = scroll_id
+            json_body['scroll'] = '1m'
+            if 'query' in json_body:
                 del json_body[
-                    "query"
+                    'query'
                 ]  # for the continuation of the download, query parameter is not allowed
-                del json_body["size"]
+                del json_body['size']
         try:
             s = requests.Session()
             response = s.post(uri, auth=auth, headers=headers, json=json_body)
             text = response.text
             try:
                 resp = json.loads(text)
             except JSONDecodeError:
                 resp = text
         except Exception as error:
-            print("\nelasticsearch_fetch() error:", error)
+            print('\nelasticsearch_fetch() error:', error)
             raise error
         try:
-            if resp["hits"]["hits"] == []:
+            if resp['hits']['hits'] == []:
                 break
         except KeyError as e:
             logger.error(e)
             print(resp)
-        total += len(resp["hits"]["hits"])
-        print(f"Downloaded {total} records\r", end="")
+        total += len(resp['hits']['hits'])
+        print(f'Downloaded {total} records\r', end='')
         # print(resp)
         # print(uri)
-        yield [h["_source"] for h in resp["hits"]["hits"]]
-        if "_scroll_id" in resp:
-            scroll_id = resp["_scroll_id"]
+        yield [h['_source'] for h in resp['hits']['hits']]
+        if '_scroll_id' in resp:
+            scroll_id = resp['_scroll_id']
 
 
-if __name__ == "__main__":
-    print(download_covid("ba", only_header=True))
+if __name__ == '__main__':
+    print(download_covid('ba', only_header=True))
```

### Comparing `pysus-0.9.1/pysus/preprocessing/ESUS.py` & `pysus-0.9.2/pysus/preprocessing/ESUS.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/preprocessing/SIM.py` & `pysus-0.9.2/pysus/preprocessing/SIM.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/preprocessing/decoders.py` & `pysus-0.9.2/pysus/preprocessing/decoders.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/preprocessing/geodata.py` & `pysus-0.9.2/pysus/preprocessing/geodata.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/preprocessing/sinan.py` & `pysus-0.9.2/pysus/preprocessing/sinan.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_cnes.py` & `pysus-0.9.2/pysus/tests/test_cnes.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_data/EPR-2016-06-01-2016.dbf` & `pysus-0.9.2/pysus/tests/test_data/EPR-2016-06-01-2016.dbf`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_data/test_Infodengue.py` & `pysus-0.9.2/pysus/tests/test_data/test_Infodengue.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_data/test_PNI.py` & `pysus-0.9.2/pysus/tests/test_data/test_PNI.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_data/test_ciha.py` & `pysus-0.9.2/pysus/tests/test_data/test_ciha.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_data/test_sia.py` & `pysus-0.9.2/pysus/tests/test_data/test_sia.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_data/test_sih.py` & `pysus-0.9.2/pysus/tests/test_data/test_sih.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_data/test_sim.py` & `pysus-0.9.2/pysus/tests/test_data/test_sim.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_data/test_sinan.py` & `pysus-0.9.2/pysus/tests/test_data/test_sinan.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_data/test_sinasc.py` & `pysus-0.9.2/pysus/tests/test_data/test_sinasc.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_decoders.py` & `pysus-0.9.2/pysus/tests/test_decoders.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_ibge.py` & `pysus-0.9.2/pysus/tests/test_ibge.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_init.py` & `pysus-0.9.2/pysus/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_sih.py` & `pysus-0.9.2/pysus/tests/test_sih.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_sim.py` & `pysus-0.9.2/pysus/tests/test_sim.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/tests/test_utilities.py` & `pysus-0.9.2/pysus/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/pysus/utilities/readdbc.py` & `pysus-0.9.2/pysus/utilities/readdbc.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.1/PKG-INFO` & `pysus-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysus
-Version: 0.9.1
+Version: 0.9.2
 Summary: Tools for dealing with Brazil's Public health data
 License: GPL
 Author: Flavio Codeco Coelho
 Author-email: fccoelho@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

