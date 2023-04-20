# Comparing `tmp/metaerg-2.3.8.tar.gz` & `tmp/metaerg-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaerg-2.3.8.tar", last modified: Mon Jan  9 17:07:16 2023, max compression
+gzip compressed data, was "metaerg-2.3.9.tar", last modified: Mon Jan 16 21:26:43 2023, max compression
```

## Comparing `metaerg-2.3.8.tar` & `metaerg-2.3.9.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 kinestetika  (1000) kinestetika  (1000)        0 2023-01-09 17:07:16.686556 metaerg-2.3.8/
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)    12585 2023-01-09 17:07:16.686556 metaerg-2.3.8/PKG-INFO
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)    11827 2023-01-06 16:23:41.000000 metaerg-2.3.8/README.md
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)      103 2022-04-15 17:59:02.000000 metaerg-2.3.8/pyproject.toml
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)       78 2023-01-09 17:07:16.686556 metaerg-2.3.8/setup.cfg
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     1475 2023-01-09 17:05:21.000000 metaerg-2.3.8/setup.py
-drwxr-xr-x   0 kinestetika  (1000) kinestetika  (1000)        0 2023-01-09 17:07:16.666556 metaerg-2.3.8/src/
-drwxr-xr-x   0 kinestetika  (1000) kinestetika  (1000)        0 2023-01-09 17:07:16.669890 metaerg-2.3.8/src/metaerg/
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)        0 2022-04-15 17:59:02.000000 metaerg-2.3.8/src/metaerg/__init__.py
-drwxr-xr-x   0 kinestetika  (1000) kinestetika  (1000)        0 2023-01-09 17:07:16.669890 metaerg-2.3.8/src/metaerg/calculations/
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)        0 2022-12-15 23:19:49.000000 metaerg-2.3.8/src/metaerg/calculations/__init__.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)    12971 2023-01-05 20:53:57.000000 metaerg-2.3.8/src/metaerg/calculations/codon_usage_bias.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)    13710 2023-01-09 15:41:25.000000 metaerg-2.3.8/src/metaerg/context.py
-drwxr-xr-x   0 kinestetika  (1000) kinestetika  (1000)        0 2023-01-09 17:07:16.673223 metaerg-2.3.8/src/metaerg/datatypes/
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)        0 2022-07-11 22:03:04.000000 metaerg-2.3.8/src/metaerg/datatypes/__init__.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     7040 2023-01-05 20:10:19.000000 metaerg-2.3.8/src/metaerg/datatypes/blast.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     6723 2022-12-15 23:19:49.000000 metaerg-2.3.8/src/metaerg/datatypes/fasta.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     4924 2022-12-15 23:19:49.000000 metaerg-2.3.8/src/metaerg/datatypes/gbk.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     2916 2022-12-15 23:19:49.000000 metaerg-2.3.8/src/metaerg/datatypes/gff.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     1528 2022-12-15 23:19:49.000000 metaerg-2.3.8/src/metaerg/datatypes/ncbi_ftp.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     5490 2023-01-05 20:10:19.000000 metaerg-2.3.8/src/metaerg/functional_gene_configuration.py
-drwxr-xr-x   0 kinestetika  (1000) kinestetika  (1000)        0 2023-01-09 17:07:16.676556 metaerg-2.3.8/src/metaerg/html/
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)       97 2022-11-26 21:23:15.000000 metaerg-2.3.8/src/metaerg/html/__init__.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     5915 2022-11-04 23:20:46.000000 metaerg-2.3.8/src/metaerg/html/html_all_genomes.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     6150 2022-12-15 23:19:49.000000 metaerg-2.3.8/src/metaerg/html/html_feature_details.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     7214 2022-12-15 23:19:49.000000 metaerg-2.3.8/src/metaerg/html/html_feature_table.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     4283 2022-12-15 23:19:49.000000 metaerg-2.3.8/src/metaerg/html/html_genome_properties_and_subsystems.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     9985 2022-12-15 23:19:49.000000 metaerg-2.3.8/src/metaerg/installation.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)    15032 2023-01-09 17:05:21.000000 metaerg-2.3.8/src/metaerg/main.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)       83 2022-06-25 03:18:44.000000 metaerg-2.3.8/src/metaerg/registry.py
-drwxr-xr-x   0 kinestetika  (1000) kinestetika  (1000)        0 2023-01-09 17:07:16.683223 metaerg-2.3.8/src/metaerg/run_and_read/
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)      172 2022-09-30 14:14:45.000000 metaerg-2.3.8/src/metaerg/run_and_read/__init__.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     4385 2023-01-09 15:13:03.000000 metaerg-2.3.8/src/metaerg/run_and_read/antismash.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     2617 2023-01-09 15:13:03.000000 metaerg-2.3.8/src/metaerg/run_and_read/aragorn.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     5471 2023-01-09 15:13:03.000000 metaerg-2.3.8/src/metaerg/run_and_read/cdd.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     6382 2023-01-09 15:13:03.000000 metaerg-2.3.8/src/metaerg/run_and_read/cmscan.py
-drwxr-xr-x   0 kinestetika  (1000) kinestetika  (1000)        0 2023-01-09 17:07:16.686556 metaerg-2.3.8/src/metaerg/run_and_read/data/
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)        0 2023-01-05 20:10:19.000000 metaerg-2.3.8/src/metaerg/run_and_read/data/__init__.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)    55692 2023-01-05 20:10:19.000000 metaerg-2.3.8/src/metaerg/run_and_read/data/functional_gene_data
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)    24848 2023-01-09 15:13:03.000000 metaerg-2.3.8/src/metaerg/run_and_read/diamond_and_blastn.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     9331 2023-01-09 15:13:03.000000 metaerg-2.3.8/src/metaerg/run_and_read/functional_genes.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     1894 2023-01-09 15:13:03.000000 metaerg-2.3.8/src/metaerg/run_and_read/gene_writer.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     1673 2023-01-09 15:13:03.000000 metaerg-2.3.8/src/metaerg/run_and_read/ltr_harvest.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     1491 2023-01-09 15:13:03.000000 metaerg-2.3.8/src/metaerg/run_and_read/minced.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     4400 2023-01-09 15:13:03.000000 metaerg-2.3.8/src/metaerg/run_and_read/prodigal.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     5410 2023-01-09 15:13:03.000000 metaerg-2.3.8/src/metaerg/run_and_read/repeat_masker.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     3252 2023-01-09 15:13:03.000000 metaerg-2.3.8/src/metaerg/run_and_read/signalp.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     2542 2023-01-09 15:13:34.000000 metaerg-2.3.8/src/metaerg/run_and_read/tmhmm.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     1991 2023-01-09 15:13:34.000000 metaerg-2.3.8/src/metaerg/run_and_read/trf.py
-drwxr-xr-x   0 kinestetika  (1000) kinestetika  (1000)        0 2023-01-09 17:07:16.669890 metaerg-2.3.8/src/metaerg.egg-info/
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)    12585 2023-01-09 17:07:16.000000 metaerg-2.3.8/src/metaerg.egg-info/PKG-INFO
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     1552 2023-01-09 17:07:16.000000 metaerg-2.3.8/src/metaerg.egg-info/SOURCES.txt
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)        1 2023-01-09 17:07:16.000000 metaerg-2.3.8/src/metaerg.egg-info/dependency_links.txt
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)       46 2023-01-09 17:07:16.000000 metaerg-2.3.8/src/metaerg.egg-info/entry_points.txt
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)      119 2023-01-09 17:07:16.000000 metaerg-2.3.8/src/metaerg.egg-info/requires.txt
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)        8 2023-01-09 17:07:16.000000 metaerg-2.3.8/src/metaerg.egg-info/top_level.txt
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2023-01-16 21:26:43.691232 metaerg-2.3.9/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    12070 2023-01-16 21:26:43.691232 metaerg-2.3.9/PKG-INFO
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    11312 2023-01-16 21:19:07.000000 metaerg-2.3.9/README.md
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)      103 2022-11-28 15:41:30.000000 metaerg-2.3.9/pyproject.toml
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)       78 2023-01-16 21:26:43.691232 metaerg-2.3.9/setup.cfg
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1475 2023-01-16 21:26:33.000000 metaerg-2.3.9/setup.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2023-01-16 21:26:43.687899 metaerg-2.3.9/src/
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2023-01-16 21:26:43.687899 metaerg-2.3.9/src/metaerg/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2022-11-28 15:41:30.000000 metaerg-2.3.9/src/metaerg/__init__.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2023-01-16 21:26:43.687899 metaerg-2.3.9/src/metaerg/calculations/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2022-11-30 16:59:09.000000 metaerg-2.3.9/src/metaerg/calculations/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    13510 2023-01-13 21:44:38.000000 metaerg-2.3.9/src/metaerg/calculations/codon_usage_bias.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    13395 2023-01-13 22:18:25.000000 metaerg-2.3.9/src/metaerg/context.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2023-01-16 21:26:43.687899 metaerg-2.3.9/src/metaerg/datatypes/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2022-11-28 15:41:30.000000 metaerg-2.3.9/src/metaerg/datatypes/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7040 2022-12-16 22:18:39.000000 metaerg-2.3.9/src/metaerg/datatypes/blast.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6351 2023-01-11 15:29:40.000000 metaerg-2.3.9/src/metaerg/datatypes/fasta.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4919 2023-01-11 15:29:40.000000 metaerg-2.3.9/src/metaerg/datatypes/gbk.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2947 2023-01-11 15:29:40.000000 metaerg-2.3.9/src/metaerg/datatypes/gff.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1528 2022-12-02 16:19:04.000000 metaerg-2.3.9/src/metaerg/datatypes/ncbi_ftp.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6802 2023-01-16 18:49:02.000000 metaerg-2.3.9/src/metaerg/datatypes/sqlite.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5528 2023-01-12 15:24:36.000000 metaerg-2.3.9/src/metaerg/functional_gene_configuration.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2023-01-16 21:26:43.687899 metaerg-2.3.9/src/metaerg/html/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)       97 2022-11-28 15:41:30.000000 metaerg-2.3.9/src/metaerg/html/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5915 2022-11-28 15:41:30.000000 metaerg-2.3.9/src/metaerg/html/html_all_genomes.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6257 2023-01-16 20:41:46.000000 metaerg-2.3.9/src/metaerg/html/html_feature_details.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6954 2023-01-16 20:15:22.000000 metaerg-2.3.9/src/metaerg/html/html_feature_table.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4183 2023-01-12 15:53:09.000000 metaerg-2.3.9/src/metaerg/html/html_genome_properties_and_subsystems.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     9985 2022-12-14 17:59:44.000000 metaerg-2.3.9/src/metaerg/installation.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    16840 2023-01-16 21:26:33.000000 metaerg-2.3.9/src/metaerg/main.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)       83 2022-11-28 15:41:30.000000 metaerg-2.3.9/src/metaerg/registry.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2023-01-16 21:26:43.691232 metaerg-2.3.9/src/metaerg/run_and_read/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)      172 2022-11-28 15:41:30.000000 metaerg-2.3.9/src/metaerg/run_and_read/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3714 2023-01-11 15:29:40.000000 metaerg-2.3.9/src/metaerg/run_and_read/antismash.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2546 2023-01-11 15:29:40.000000 metaerg-2.3.9/src/metaerg/run_and_read/aragorn.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5430 2023-01-11 15:29:40.000000 metaerg-2.3.9/src/metaerg/run_and_read/cdd.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6295 2023-01-11 15:29:40.000000 metaerg-2.3.9/src/metaerg/run_and_read/cmscan.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2023-01-16 21:26:43.691232 metaerg-2.3.9/src/metaerg/run_and_read/data/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2022-12-16 15:51:21.000000 metaerg-2.3.9/src/metaerg/run_and_read/data/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    55692 2022-12-16 22:31:12.000000 metaerg-2.3.9/src/metaerg/run_and_read/data/functional_gene_data
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    24825 2023-01-11 15:29:40.000000 metaerg-2.3.9/src/metaerg/run_and_read/diamond_and_blastn.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     9350 2023-01-11 15:29:40.000000 metaerg-2.3.9/src/metaerg/run_and_read/functional_genes.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1727 2023-01-16 17:27:22.000000 metaerg-2.3.9/src/metaerg/run_and_read/gene_writer.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1618 2023-01-11 15:29:40.000000 metaerg-2.3.9/src/metaerg/run_and_read/ltr_harvest.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1374 2023-01-11 15:29:40.000000 metaerg-2.3.9/src/metaerg/run_and_read/minced.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     4382 2023-01-13 22:20:29.000000 metaerg-2.3.9/src/metaerg/run_and_read/prodigal.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5491 2023-01-11 15:29:40.000000 metaerg-2.3.9/src/metaerg/run_and_read/repeat_masker.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     3327 2023-01-11 15:29:40.000000 metaerg-2.3.9/src/metaerg/run_and_read/signalp.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2649 2023-01-16 17:01:08.000000 metaerg-2.3.9/src/metaerg/run_and_read/tmhmm.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     2017 2023-01-11 15:29:40.000000 metaerg-2.3.9/src/metaerg/run_and_read/trf.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2023-01-16 21:26:43.687899 metaerg-2.3.9/src/metaerg.egg-info/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    12070 2023-01-16 21:26:43.000000 metaerg-2.3.9/src/metaerg.egg-info/PKG-INFO
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1584 2023-01-16 21:26:43.000000 metaerg-2.3.9/src/metaerg.egg-info/SOURCES.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        1 2023-01-16 21:26:43.000000 metaerg-2.3.9/src/metaerg.egg-info/dependency_links.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)       46 2023-01-16 21:26:43.000000 metaerg-2.3.9/src/metaerg.egg-info/entry_points.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)      119 2023-01-16 21:26:43.000000 metaerg-2.3.9/src/metaerg.egg-info/requires.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        8 2023-01-16 21:26:43.000000 metaerg-2.3.9/src/metaerg.egg-info/top_level.txt
```

### Comparing `metaerg-2.3.8/PKG-INFO` & `metaerg-2.3.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaerg
-Version: 2.3.8
+Version: 2.3.9
 Summary: Annotation of genomes and contigs
 Home-page: https://github.com/kinestetika/MetaErg
 Author: Marc Strous
 Author-email: mstrous@ucalgary.ca
 License: MIT
 Project-URL: Source, https://github.com/kinestetika/MetaErg
 Keywords: repeat-regions genes functions taxonomy
@@ -28,15 +28,15 @@
 classifications.
 
 You can interact with a sample visualization [here](https://htmlpreview.github.io/?https://github.com/kinestetika/MetaErg/blob/master/visualization/index.html) and [here](https://htmlpreview.github.io/?https://raw.githubusercontent.com/kinestetika/MetaErg/master/visualization/index_of_features.html). These visualizations show the annotation of a cyanobacterial genome, Candidatus Phormidium alkaliphilum.
 Unfortunately the interacive search box does not work with the github html visualization, so you need to download the html \
 files to your computer (i.e. using "git clone ..."), to try out the interactive part.
 
 Metaerg was originally developed in perl. It was relatively challenging to install and comes with complex database 
-dependencies. This new python version 2.2 overcomes some of those issues. Also, the annotation pipeline has further 
+dependencies. This new python version 2.3 overcomes some of those issues. Also, the annotation pipeline has further 
 evolved and has become more refined.
 
 By using gtdbtk for taxonomic classification of genes and transferring functional annotations from the NCBI, metaerg.py
 uses a controlled vocabulary for taxonomy and a relatively clean vocabulary for functions. This makes annotations much
 more concise than the original version of metaerg and many other annotation tools. In addition, metaerg uses NCBI's
 conserved domain database and RPSBlast to assign genes to subsystems for effective data exploration. Subsystems are a 
 work in progress, and can be expanded and customized as needed.
@@ -52,15 +52,15 @@
 * annotates taxonomy and functions of RNA and protein genes using [Diamond](https://github.com/bbuchfink/diamond), [NCBI blastn](https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/LATEST/) and a database of 62,296 bacterial, 3,406 archaeal 11,569 viral and 139 eukaryotic genomes.
 * annotates gene functions using [RPSBlast](https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/LATEST/) and NCBI's Conserved Domain Database (CDD).
 * annotates genes involved in production of secondary metabolites using [Antismash](https://dl.secondarymetabolites.org/releases).
 * annotates membrane amd translocated proteins using [TMHMM and SignalP](https://services.healthtech.dtu.dk/software.php).
 * assigns genes to a built-in set of functions using [HMMER](http://hmmer.org) and commmunity contributed HMM profiles (see below).
 * estimates doubling times of a genome's host based on [codon usage bias](https://www.pnas.org/doi/epdf/10.1073/pnas.2016810118)
 * presents annotations in [datatables/jQuery](https://www.datatables.net/)-based intuititve, searchable, colorful HTML that can be explored in a web browser and copy/pasted into excel.
-* saves annotations as a fasta-amino-acid file, a genbank file and in [Apache Feather format](https://arrow.apache.org/docs/python/feather.html) for effective exploration, statistics and visualization with python or R.
+* saves annotations as a fasta-amino-acid file, a genbank file, as a sqlite database and in [Apache Feather format](https://arrow.apache.org/docs/python/feather.html) for effective exploration, statistics and visualization with python or R.
 * saves an overview of all annotated genomes' properties and functions as an excel file. 
 * enables the user to add custom HMMs and expand the set of functional genes as needed.
 
 When using metaerg, please cite [Xiaoli Dong and Marc Strous (2019) Frontiers in Genetics](https://www.frontiersin.org/articles/10.3389/fgene.2019.00999/full)
 
 ## Usage:
 ```
@@ -128,17 +128,17 @@
 * E - build eukaryotes
 * B - build PVE blast databases
 * R - build RFAM
 * C - build CDD
 * S - build/update community contributed HMM databases
 * A - build antismash database
 
-## Using the .feather output
-[Apache Feather format](https://arrow.apache.org/docs/python/feather.html) is a binary file format for tables. You can for example load these data as a pandas dataframe. In **R**, use the [arrow](https://arrow.apache.org/docs/r/) package. 
-Each table row contains a single gene or feature, defines by the following columns:
+## Accessing the .feather and .mysql files
+[Apache Feather format](https://arrow.apache.org/docs/python/feather.html) is a binary file format for tables. Sqlite is a database format. You can for example load these data as a pandas dataframe. In **R**, use the [arrow](https://arrow.apache.org/docs/r/) package. 
+Each table/database row contains a single gene or feature, defined by the following columns:
 
 ```
 id                  the feature's unique identifier
 genome              the identifier of the genome the feature belongs to
 contig              the identifier of the contig the feature belongs to
 start               the start position of the feature (inclusive)
 end                 the start position of the feature (exclusive)
@@ -155,47 +155,41 @@
 tmh                 the number of transmembrane helixes found
 tmh_topology        how the protein is oriented in the membrane, if tmh were found 
 blast               the top ten blast hits
 cdd                 the top ten cdd hits
 hmm                 the top ten hits to the functional gene hmm database 
 ```
 
-You can for example use python and pandas to inspect the distribution of subsystems, such as denitrification, hydrogen oxidation or the Calvin Cycle across a large set of MAGs, as follows:
+You can for example use python and pandas to inspect annotations:
 
-```commandline
+``` python
 from pathlib import Path
 import pandas as pd
 
-from metaerg import functional_gene_configuration
-from metaerg.main import load_contigs, compute_genome_properties
+data_dir = Path('/path/to/my/data')
+feather_file = data_dir / 'my-genome.annotations.feather'
+contig_file =  data_dir / 'my-genome.fna'
+
+contig_dict = load_contigs('my-genome', contig_file, delimiter='xxxx')
+feature_data = pd.read_feather(feather_file)
+feature_data.set_index('id', inplace=True)
 
-functional_gene_configuration.init_functional_gene_config()
+for f in feature_data.itertuples():
+    for k, v in f._asdict().items():
+        print(f'{k:20}:{v}')
+    break  # comment out to iterate through all the genes...
+```
+
+Using the .mysql database is even easier:
+
+``` python
+from pathlib import Path
+from metaerg.datatypes import sqlite
 
 data_dir = Path('/path/to/my/data')
-feather_dir = data_dir / 'all_genes.feather'
-contig_dir =  data_dir / 'contig_fna_files_one_per_genome'
+sqlite_file = data_dir / 'my-genome.annotations.sqlite'
 
-genome_properties = {}
-for f in sorted(feather_dir.glob('*')):
-    genome_name = f.name
-    contig_dict = load_contigs(genome_name, contig_dir / genome_name, delimiter='xxxx')
-    feature_data = pd.read_feather(f)
-    genome_properties[genome_name] = compute_genome_properties(contig_dict, feature_data)
-    
-all_genome_feature_data = None
-for k, v in genome_properties.items():
-    subsystems_df = v['subsystems'].rename(columns={'genes': k})
-    try:
-        subsystems_df.drop('', level=0, axis=0, inplace=True)
-        subsystems_df.drop('secondary-metabolites', level=0, axis=0, inplace=True)
-    except Exception:
-        pass
-    if all_genome_feature_data is None:
-        all_genome_feature_data = subsystems_df
-    else:
-        all_genome_feature_data[k] = subsystems_df[k]
-    all_genome_feature_data = all_genome_feature_data.copy()
-del all_genome_feature_data['profiles']
-#print(all_genome_feature_data.columns)
-    
-all_genome_feature_data.to_excel(data_dir / 'functional_gene_heatmap.xls')
+db_connection = sqlite.connect_to_db(sqlite_file)
+for feature in sqlite.read_all_features(db_connection): 
+    print(feature)
+    break  # comment out to iterate through all the genes...
 ```
```

### Comparing `metaerg-2.3.8/README.md` & `metaerg-2.3.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 classifications.
 
 You can interact with a sample visualization [here](https://htmlpreview.github.io/?https://github.com/kinestetika/MetaErg/blob/master/visualization/index.html) and [here](https://htmlpreview.github.io/?https://raw.githubusercontent.com/kinestetika/MetaErg/master/visualization/index_of_features.html). These visualizations show the annotation of a cyanobacterial genome, Candidatus Phormidium alkaliphilum.
 Unfortunately the interacive search box does not work with the github html visualization, so you need to download the html \
 files to your computer (i.e. using "git clone ..."), to try out the interactive part.
 
 Metaerg was originally developed in perl. It was relatively challenging to install and comes with complex database 
-dependencies. This new python version 2.2 overcomes some of those issues. Also, the annotation pipeline has further 
+dependencies. This new python version 2.3 overcomes some of those issues. Also, the annotation pipeline has further 
 evolved and has become more refined.
 
 By using gtdbtk for taxonomic classification of genes and transferring functional annotations from the NCBI, metaerg.py
 uses a controlled vocabulary for taxonomy and a relatively clean vocabulary for functions. This makes annotations much
 more concise than the original version of metaerg and many other annotation tools. In addition, metaerg uses NCBI's
 conserved domain database and RPSBlast to assign genes to subsystems for effective data exploration. Subsystems are a 
 work in progress, and can be expanded and customized as needed.
@@ -30,15 +30,15 @@
 * annotates taxonomy and functions of RNA and protein genes using [Diamond](https://github.com/bbuchfink/diamond), [NCBI blastn](https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/LATEST/) and a database of 62,296 bacterial, 3,406 archaeal 11,569 viral and 139 eukaryotic genomes.
 * annotates gene functions using [RPSBlast](https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/LATEST/) and NCBI's Conserved Domain Database (CDD).
 * annotates genes involved in production of secondary metabolites using [Antismash](https://dl.secondarymetabolites.org/releases).
 * annotates membrane amd translocated proteins using [TMHMM and SignalP](https://services.healthtech.dtu.dk/software.php).
 * assigns genes to a built-in set of functions using [HMMER](http://hmmer.org) and commmunity contributed HMM profiles (see below).
 * estimates doubling times of a genome's host based on [codon usage bias](https://www.pnas.org/doi/epdf/10.1073/pnas.2016810118)
 * presents annotations in [datatables/jQuery](https://www.datatables.net/)-based intuititve, searchable, colorful HTML that can be explored in a web browser and copy/pasted into excel.
-* saves annotations as a fasta-amino-acid file, a genbank file and in [Apache Feather format](https://arrow.apache.org/docs/python/feather.html) for effective exploration, statistics and visualization with python or R.
+* saves annotations as a fasta-amino-acid file, a genbank file, as a sqlite database and in [Apache Feather format](https://arrow.apache.org/docs/python/feather.html) for effective exploration, statistics and visualization with python or R.
 * saves an overview of all annotated genomes' properties and functions as an excel file. 
 * enables the user to add custom HMMs and expand the set of functional genes as needed.
 
 When using metaerg, please cite [Xiaoli Dong and Marc Strous (2019) Frontiers in Genetics](https://www.frontiersin.org/articles/10.3389/fgene.2019.00999/full)
 
 ## Usage:
 ```
@@ -106,17 +106,17 @@
 * E - build eukaryotes
 * B - build PVE blast databases
 * R - build RFAM
 * C - build CDD
 * S - build/update community contributed HMM databases
 * A - build antismash database
 
-## Using the .feather output
-[Apache Feather format](https://arrow.apache.org/docs/python/feather.html) is a binary file format for tables. You can for example load these data as a pandas dataframe. In **R**, use the [arrow](https://arrow.apache.org/docs/r/) package. 
-Each table row contains a single gene or feature, defines by the following columns:
+## Accessing the .feather and .mysql files
+[Apache Feather format](https://arrow.apache.org/docs/python/feather.html) is a binary file format for tables. Sqlite is a database format. You can for example load these data as a pandas dataframe. In **R**, use the [arrow](https://arrow.apache.org/docs/r/) package. 
+Each table/database row contains a single gene or feature, defined by the following columns:
 
 ```
 id                  the feature's unique identifier
 genome              the identifier of the genome the feature belongs to
 contig              the identifier of the contig the feature belongs to
 start               the start position of the feature (inclusive)
 end                 the start position of the feature (exclusive)
@@ -133,47 +133,41 @@
 tmh                 the number of transmembrane helixes found
 tmh_topology        how the protein is oriented in the membrane, if tmh were found 
 blast               the top ten blast hits
 cdd                 the top ten cdd hits
 hmm                 the top ten hits to the functional gene hmm database 
 ```
 
-You can for example use python and pandas to inspect the distribution of subsystems, such as denitrification, hydrogen oxidation or the Calvin Cycle across a large set of MAGs, as follows:
+You can for example use python and pandas to inspect annotations:
 
-```commandline
+``` python
 from pathlib import Path
 import pandas as pd
 
-from metaerg import functional_gene_configuration
-from metaerg.main import load_contigs, compute_genome_properties
+data_dir = Path('/path/to/my/data')
+feather_file = data_dir / 'my-genome.annotations.feather'
+contig_file =  data_dir / 'my-genome.fna'
+
+contig_dict = load_contigs('my-genome', contig_file, delimiter='xxxx')
+feature_data = pd.read_feather(feather_file)
+feature_data.set_index('id', inplace=True)
 
-functional_gene_configuration.init_functional_gene_config()
+for f in feature_data.itertuples():
+    for k, v in f._asdict().items():
+        print(f'{k:20}:{v}')
+    break  # comment out to iterate through all the genes...
+```
+
+Using the .mysql database is even easier:
+
+``` python
+from pathlib import Path
+from metaerg.datatypes import sqlite
 
 data_dir = Path('/path/to/my/data')
-feather_dir = data_dir / 'all_genes.feather'
-contig_dir =  data_dir / 'contig_fna_files_one_per_genome'
+sqlite_file = data_dir / 'my-genome.annotations.sqlite'
 
-genome_properties = {}
-for f in sorted(feather_dir.glob('*')):
-    genome_name = f.name
-    contig_dict = load_contigs(genome_name, contig_dir / genome_name, delimiter='xxxx')
-    feature_data = pd.read_feather(f)
-    genome_properties[genome_name] = compute_genome_properties(contig_dict, feature_data)
-    
-all_genome_feature_data = None
-for k, v in genome_properties.items():
-    subsystems_df = v['subsystems'].rename(columns={'genes': k})
-    try:
-        subsystems_df.drop('', level=0, axis=0, inplace=True)
-        subsystems_df.drop('secondary-metabolites', level=0, axis=0, inplace=True)
-    except Exception:
-        pass
-    if all_genome_feature_data is None:
-        all_genome_feature_data = subsystems_df
-    else:
-        all_genome_feature_data[k] = subsystems_df[k]
-    all_genome_feature_data = all_genome_feature_data.copy()
-del all_genome_feature_data['profiles']
-#print(all_genome_feature_data.columns)
-    
-all_genome_feature_data.to_excel(data_dir / 'functional_gene_heatmap.xls')
+db_connection = sqlite.connect_to_db(sqlite_file)
+for feature in sqlite.read_all_features(db_connection): 
+    print(feature)
+    break  # comment out to iterate through all the genes...
 ```
```

### Comparing `metaerg-2.3.8/setup.py` & `metaerg-2.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='metaerg',
-    version='2.3.8',
+    version='2.3.9',
     packages=setuptools.find_packages(where='src'),
     url='https://github.com/kinestetika/MetaErg',
     license='MIT',
     author='Marc Strous',
     author_email='mstrous@ucalgary.ca',
     description='Annotation of genomes and contigs',
     long_description=long_description,
```

### Comparing `metaerg-2.3.8/src/metaerg/calculations/codon_usage_bias.py` & `metaerg-2.3.9/src/metaerg/calculations/codon_usage_bias.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import math
 
-import pandas as pd
 import re
 from time import sleep
 from statistics import median, mean
 from math import log, log10
 from pathlib import Path
 from collections import namedtuple
 
 from tqdm import tqdm
 
 from metaerg import context
 from metaerg.datatypes.fasta import FastaParser
 from metaerg.datatypes import ncbi_ftp
+from metaerg.datatypes import sqlite
 
 CUBData = namedtuple('CUBData', ['genome_id', 'nHE', 'CUBHE', 'consistency', 'CPB', 'filtered', 'd'])
 
-def compute_feature_codon_counts_by_aa(feature, codon_counts_by_aa = 0):
+def compute_feature_codon_counts_by_aa(feature, codon_counts_by_aa: dict|int = 0):
     if not isinstance(codon_counts_by_aa, dict):
         codon_counts_by_aa = {}
 
     # to deal with start codon, always translated as M:
     aa_seq = feature.aa_seq[0:1].lower() + feature.aa_seq[1:].upper()
     nt_seq = feature.nt_seq[0:3].lower() + feature.nt_seq[3:].upper()
 
@@ -52,17 +52,17 @@
         codon_freq_by_aa[aa] = {}
         total_counts_for_aa = sum(codons_for_aa.values())
         for codon, count in codons_for_aa.items():
             codon_freq_by_aa[aa][codon] = count / total_counts_for_aa
     return codon_freq_by_aa
 
 
-def compute_codon_frequencies_for_feature_data(feature_data: pd.DataFrame) -> dict:
+def compute_codon_frequencies_for_feature_data(db_connection, additional_sql: str = '') -> dict:
     genome_wide_codon_counts_by_aa = {}
-    for feature in feature_data.itertuples():
+    for feature in sqlite.read_all_features(db_connection, type='CDS', additional_sql=additional_sql):
         compute_feature_codon_counts_by_aa(feature, genome_wide_codon_counts_by_aa)
     genome_wide_codon_freq_by_aa = convert_counts_to_frequencies(genome_wide_codon_counts_by_aa)
     return genome_wide_codon_freq_by_aa
 
 
 def compute_codon_usage_bias_for_feature(feature, genome_wide_codon_frequencies_by_aa) -> float:
     # see https://link.springer.com/article/10.1186/1471-2105-6-182, https://github.com/BioinfoHR/coRdon/blob/master/R/codonUsage.R, lines 218-255
@@ -75,24 +75,24 @@
         for codon, freq in codons_for_aa.items():
             milc += 2 * cds_codon_counts_by_aa[aa][codon] * log(freq / genome_wide_codon_frequencies_by_aa [aa][codon])
     milc /= len(feature.aa_seq) - 1
     correction_factor = correction_factor / (len(feature.aa_seq) - 1) - 0.5  # -0.5 as in coRdon, not +0.5 as in paper
     return milc - correction_factor
 
 
-def compute_codon_pair_scores_for_feature_data(genome_id: str, feature_data: pd.DataFrame) -> dict:
+def compute_codon_pair_scores_for_feature_data(genome_id: str, db_connection, additional_sql: str = '') -> dict:
     # see https://www.science.org/doi/full/10.1126/science.1155761, supplement, Fig. 1
     codon_pair_counts = {}
     aa_pair_counts = {}
     aa_counts = {}
     codon_counts = {}
     codon2aa = {}
 
     ambiguous_codon_warnings = 0
-    for feature in feature_data.itertuples():
+    for feature in sqlite.read_all_features(db_connection, type='CDS', additional_sql=additional_sql):
         # to deal with start codon, always translated as M:
         aa_seq = feature.aa_seq[0:1].lower() + feature.aa_seq[1:].upper()
         nt_seq = feature.nt_seq[0:3].lower() + feature.nt_seq[3:].upper()
 
         for i in range(1, len(aa_seq)):
             x = aa_seq[i]
             a = nt_seq[i * 3:i * 3 + 3]
@@ -159,51 +159,52 @@
         try:
             cpb += codon_pair_scores[codon_pair]
         except KeyError:
             pass  # can happen, a codon pair that was not seen before
     return cpb / len(feature.aa_seq)
 
 
-def compute_codon_usage_bias_for_genome(genome_id, feature_data: pd.DataFrame) -> CUBData:
-    feature_data = feature_data[feature_data['type'] == 'CDS']
-    filtered_feature_data = feature_data[feature_data['aa_seq'].str.len() >= 80]
-    ribosomal_proteins = feature_data[feature_data['subsystems'].str.contains('ribosomal protein')]
+def compute_codon_usage_bias_for_genome(genome_id, db_connection) -> CUBData:
     # codon usage bias
-    background_frequencies = compute_codon_frequencies_for_feature_data(filtered_feature_data)
-    codon_usage_bias = median([compute_codon_usage_bias_for_feature(rp, background_frequencies)
-                               for rp in ribosomal_proteins.itertuples()])
-    # consistency in codon usage bias
-    background_frequencies = compute_codon_frequencies_for_feature_data(ribosomal_proteins)
-    consistency = mean([compute_codon_usage_bias_for_feature(rp, background_frequencies)
-                        for rp in ribosomal_proteins.itertuples()])
-    # codon pair bias
-    codon_pair_scores = compute_codon_pair_scores_for_feature_data(genome_id, filtered_feature_data)
-    # codon_pair_bias = sum(codon_pair_scores.values()) / (len(codon_pair_scores) - 1)
-    codon_pair_bias = median([compute_codon_pair_bias_for_cds(rp, codon_pair_scores)
-                              for rp in ribosomal_proteins.itertuples()])
-    # keep track of # too short proteins filtered out and ribosomal proteins
-    filtered_out = len(feature_data[feature_data['aa_seq'].str.len() < 80])
-
-    return CUBData(genome_id, len(ribosomal_proteins.index), codon_usage_bias,
-                   consistency, codon_pair_bias, filtered_out, 0)
-
-
-def compute_codon_bias_estimate_doubling_time(feature_data: pd.DataFrame):
-    feature_data = feature_data[feature_data['type'] == 'CDS']
-    filtered_feature_data = feature_data[feature_data['aa_seq'].str.len() >= 80]
-    ribosomal_proteins = feature_data[feature_data['subsystems'].str.contains('ribosomal protein')]
-    if not len(ribosomal_proteins.index):
+    background_frequencies = compute_codon_frequencies_for_feature_data(db_connection, additional_sql='end - start >= 240')
+    cub_ribosomal = [compute_codon_usage_bias_for_feature(rp, background_frequencies)
+                               for rp in sqlite.read_all_features(db_connection, type='CDS',
+                               additional_sql='end - start >= 240 AND subsystems LIKE "%ribosomal protein%"')]
+    if len(cub_ribosomal):
+        codon_usage_bias = median(cub_ribosomal)
+        # consistency in codon usage bias
+        background_frequencies = compute_codon_frequencies_for_feature_data(db_connection,
+                                 additional_sql='end - start >= 240 AND subsystems LIKE "%ribosomal protein%"')
+        consistency = mean([compute_codon_usage_bias_for_feature(rp, background_frequencies)
+                               for rp in sqlite.read_all_features(db_connection, type='CDS',
+                               additional_sql='end - start >= 240 AND subsystems LIKE "%ribosomal protein%"')])
+        # codon pair bias
+        codon_pair_scores = compute_codon_pair_scores_for_feature_data(genome_id, db_connection, additional_sql='end - start >= 240')
+        # codon_pair_bias = sum(codon_pair_scores.values()) / (len(codon_pair_scores) - 1)
+        codon_pair_bias = median([compute_codon_pair_bias_for_cds(rp, codon_pair_scores)
+                                  for rp in sqlite.read_all_features(type='CDS', additional_sql='end - start >= 240 AND subsystems LIKE "%ribosomal protein%"')])
+        # keep track of # too short proteins filtered out and ribosomal proteins
+        filtered_out = sum(1 for feature in sqlite.read_all_features(db_connection, type='CDS', additional_sql='end - start < 240'))
+        return CUBData(genome_id, len(cub_ribosomal), codon_usage_bias, consistency, codon_pair_bias, filtered_out, 0)
+    else:
+        return CUBData(genome_id, 0, 0, 0, 0, 0, 0)
+
+
+def compute_codon_bias_estimate_doubling_time(db_connection):
+    background_frequencies = compute_codon_frequencies_for_feature_data(db_connection, additional_sql='end - start >= 240')
+    cub_ribosomal = [compute_codon_usage_bias_for_feature(rp, background_frequencies)
+                               for rp in sqlite.read_all_features(db_connection, type='CDS',
+                               additional_sql='end - start >= 240 AND subsystems LIKE "%ribosomal protein%"')]
+    if len(cub_ribosomal):
+        codon_usage_bias = median(cub_ribosomal)
+        doubling_time = math.pow(10, codon_usage_bias * -2.41937374 + 2.00361692)
+        return codon_usage_bias, doubling_time
+    else:
         context.log('Warning: No ribosomomal proteins for genome.')
         return 0, 0
-    # codon usage bias
-    background_frequencies = compute_codon_frequencies_for_feature_data(filtered_feature_data)
-    codon_usage_bias = median([compute_codon_usage_bias_for_feature(rp, background_frequencies)
-                               for rp in ribosomal_proteins.itertuples()])
-    doubling_time = math.pow(10, codon_usage_bias * -2.41937374 + 2.00361692)
-    return codon_usage_bias, doubling_time
 
 
 def parse_training_data(list_file) -> list[CUBData]:
     training_data = []
     refseq_acc_pattern = re.compile(r'(GCF_\d+)')
     with open(list_file) as reader:
         for line in reader:
```

### Comparing `metaerg-2.3.8/src/metaerg/context.py` & `metaerg-2.3.9/src/metaerg/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,14 @@
 from pathlib import Path
 
 import pandas as pd
 import httpx
 
 from metaerg import registry
 
-DATAFRAME_COLUMNS = 'id genome contig start end strand type inference subsystems descr taxon notes aa_seq nt_seq ' \
-                    'antismash signal_peptide tmh tmh_topology blast cdd hmm'.split()
-
-RNA_TARGETS = set("rRNA tRNA tmRNA ncRNA retrotransposon".split())
-
 BASE_DIR = Path()
 TEMP_DIR = Path()
 HTML_DIR = Path()
 DATABASE_DIR = Path()
 CHECKM_DIR = Path()
 GTDBTK_DIR = Path()
 GENOME_NAME_MAPPING_FILE = ''
@@ -211,15 +206,14 @@
 
 
 def run_external(exec, stdin=None, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL, log_cmd=True):
     if log_cmd:
         log(exec)
     result = subprocess.run(exec.split(), stdout=stdout, stdin=stdin, stderr=stderr)
     if result.returncode != 0:
-        print(result.stderr)
         raise Exception(f'WARNING: "{exec}" exited with non-zero status')
 
 
 def download(url: str, file: Path):
     log(f'Started downloading {url} to {file}...')
     with httpx.stream('GET', url, timeout=6.1, follow_redirects=True) as data_stream, open(file, 'wb') as handle:
         for data in data_stream.iter_bytes():
@@ -307,15 +301,15 @@
                 results_complete = False
         # (7) Report success, update progress
         current_progress = current_progress.replace('{}=started'.format(param['annotator_key']),
                                                     '{}=complete'.format(param['annotator_key']))
         write_metaerg_progress(genome_name, current_progress)
         positive_count = 0
         if results_complete:
-            feature_data, positive_count = param['read'](genome_name, contig_dict, feature_data, result_files)
+            positive_count = param['read'](genome_name, contig_dict, feature_data, result_files)
         log('({}) {} complete. Found {}.', (genome_name, param['purpose'], positive_count))
         return feature_data
 
     registry.ANNOTATOR_REGISTRY[param['pipeline_position']] = annotator
     return annotator
```

### Comparing `metaerg-2.3.8/src/metaerg/datatypes/blast.py` & `metaerg-2.3.9/src/metaerg/datatypes/blast.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.3.8/src/metaerg/datatypes/fasta.py` & `metaerg-2.3.9/src/metaerg/datatypes/fasta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import gzip
 import re
 import numpy as np
-import pandas as pd
 from pathlib import Path
 from metaerg import context
+from metaerg.datatypes import sqlite
 
 NON_IUPAC_RE_NT = re.compile(r'[^ACTGN]')
 NON_IUPAC_RE_AA = re.compile(r'[^RHKDESTNQCUGPAVILMFYW]')
 ALL_MASK_TARGETS = set('CDS rRNA tRNA tmRNA ncRNA repeat crispr_repeat retrotransposon'.split())
 COMPLEMENT = {'A': 'T', 'C': 'G', 'G': 'C', 'T': 'A',}
 
 
@@ -75,33 +75,26 @@
             seq = ''.join(seq.split())
             if self.alphabet:
                 seq = self.alphabet.sub(self.unknown_char, seq)
         return seq
 
 
 class Masker:
-    def __init__(self, feature_data, targets=None, min_length=50):
-        if targets:
-            self.feature_data = feature_data[feature_data['type'].isin(targets)]
-            self.apply_mask = True
-        else:
-            self.feature_data = feature_data
-            self.apply_mask = False
-        self.min_length = min_length
+    def __init__(self, db_connection, targets=None):
+        self.db_connection = db_connection
+        self.targets = targets
         self.nt_total = 0
         self.nt_masked = 0
 
     def mask(self, seq_record):
         seq = seq_record['seq']
-        if self.apply_mask:
-            feature_data = self.feature_data.loc[lambda df: df['contig'] == seq_record['id'], :]
-            for feature in feature_data.itertuples():
-                feature_length = feature.end - feature.start
-                seq = seq[:feature.start] + 'N' * feature_length + seq[feature.end:]
-                self.nt_masked += feature_length
+        if self.targets:
+            for feature in sqlite.read_all_features(self.db_connection,  contig=seq_record['id'], type=self.targets):
+                seq = seq[:feature.start] + 'N' * feature.length_nt() + seq[feature.end:]
+                self.nt_masked += feature.length_nt()
 
         self.nt_total += len(seq)
 
         masked_record = seq_record.copy()
         masked_record['seq'] = seq
         return masked_record
 
@@ -130,53 +123,51 @@
         pass
     handle.write('\n')
     for i in range(0, len(fasta['seq']), line_length):
         handle.write(fasta['seq'][i:i+line_length])
         handle.write('\n')
 
 
-def write_features_to_fasta(feature_data: pd.DataFrame, seq_type: str, base_file: Path, split=1, targets = None):
-    if targets:
-        feature_data = feature_data[feature_data['type'].isin(targets)]
-    number_of_records = len(feature_data.index)
+def write_features_to_fasta(db_connection, seq_type: str, base_file: Path, split=1, targets = None):
+    number_of_records = sum(1 for f in sqlite.read_all_features(db_connection, type=targets))
     split = min(split, number_of_records)
     records_per_file = number_of_records / split if split else number_of_records
     if split > 1:
         paths = [Path(base_file.parent, f'{base_file.name}.{i}') for i in range(split)]
     else:
         paths = base_file,
     filehandles = [open(p, 'w') for p in paths]
     records_written = 0
-    for feature in feature_data.itertuples():
+    for feature in sqlite.read_all_features(db_connection, type=targets):
         fasta_rec = {'id': feature.id, 'descr': feature.descr}
         if 'aa' == seq_type:
             fasta_rec['seq'] = feature.aa_seq
         elif 'nt' == seq_type:
             fasta_rec['seq'] = feature.nt_seq
         write_fasta(filehandles[int(records_written / records_per_file)], fasta_rec)
         records_written += 1
-    if not len(feature_data):
+    if not number_of_records:
         context.log(f'WARNING: No [{", ".join(targets)}] features in genome, '
                     f'fasta file(s) {", ".join([str(p.name) for p in paths])} are empty!')
     return paths
 
 
-def write_contigs_to_fasta(contig_dict: dict, base_file: Path, feature_data: pd.DataFrame = None, genome_name='',
-                           split=1, mask_targets=None, mask_min_length=50):
+def write_contigs_to_fasta(contig_dict: dict, base_file: Path, db_connection, genome_name='',
+                           split=1, mask_targets=None):
     """writes contigs to fasta file(s), optionally masking features with N"""
     number_of_records = len(contig_dict)
     split = min(split, number_of_records)
     records_per_file = number_of_records / split
     if split > 1:
         paths = [Path(base_file.parent, f'{base_file.name}.{i}') for i in range(split)]
     else:
         paths = base_file,
     filehandles = [open(p, 'w') for p in paths]
     records_written = 0
-    masker = Masker(feature_data, targets=mask_targets, min_length=mask_min_length)
+    masker = Masker(db_connection, targets=mask_targets)
     for contig in contig_dict.values():
         write_fasta(filehandles[int(records_written / records_per_file)], masker.mask(contig))
         records_written += 1
     for f in filehandles:
         f.close()
     if mask_targets:
         context.log(f'({genome_name}) {masker.stats()}')
```

### Comparing `metaerg-2.3.8/src/metaerg/datatypes/gbk.py` & `metaerg-2.3.9/src/metaerg/datatypes/gbk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import gzip
 import textwrap
-import pandas as pd
-import numpy as np
+
+from metaerg.datatypes import sqlite
 
 GBK_LINEWIDTH = 80
 GBK_INDENT = 21
 GBK_HEADER = '''LOCUS       {:<15} {:>12} bp    DNA              UNK 01-JAN-1980
 DEFINITION  {}.
 ACCESSION   {}
 VERSION     {}
@@ -14,15 +14,15 @@
 SOURCE      .
   ORGANISM  .
             .
 FEATURES             Location/Qualifiers
 '''
 
 
-def gbk_write_feature(writer, feature):
+def gbk_write_feature(writer, feature: sqlite.Feature):
     indent = ' '*GBK_INDENT
     if feature.strand >= 0:
         location = f'{int(feature.start) + 1}..{int(feature.end)}'
     else:
         location = f'complement({int(feature.start) + 1}..{int(feature.end)})'
 
     writer.write('     {:<16}{}\n'.format(feature.type, textwrap.fill(location, width = GBK_LINEWIDTH,
@@ -42,19 +42,18 @@
     for k, v in gbk_keys.items():
         if v:
             writer.write(textwrap.fill(f'/{k}="{v}"', width = GBK_LINEWIDTH,
                                        initial_indent = indent, subsequent_indent = indent))
             writer.write('\n')
 
 
-def gbk_write_genome(writer, contig_dict: dict, feature_data: pd.DataFrame):
-    for id, contig in contig_dict.items():
-        writer.write(GBK_HEADER.format(id, len(contig['seq']), id, id, id))
-        sub_data = feature_data[feature_data['contig'] == id]
-        for feature in sub_data.itertuples(name = 'Feature'):
+def gbk_write_genome(writer, contig_dict: dict, db_connection):
+    for contig_id, contig in contig_dict.items():
+        writer.write(GBK_HEADER.format(contig_id, len(contig['seq']), contig_id, contig_id, contig_id))
+        for feature in sqlite.read_all_features(db_connection, contig=contig_id):
             gbk_write_feature(writer, feature)
         writer.write('ORIGIN\n')
         lw = ((GBK_LINEWIDTH - 20) // 10) * 10
         for i in range(0, len(contig['seq']), lw):
             line_seq = contig['seq'][i:i + lw].lower()
             writer.write(f'{i+1:>9}')
             for j in range(lw // 10):
```

### Comparing `metaerg-2.3.8/src/metaerg/datatypes/gff.py` & `metaerg-2.3.9/src/metaerg/datatypes/gff.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from urllib.parse import unquote
 import re
 import gzip
 from metaerg.datatypes import fasta
+from metaerg.datatypes.sqlite import Feature
 
 class GffParser:
     def __init__(self, path, contig_dict, target_feature_type_dict:dict=None, inference:str=None):
         self.path = path
         self.contig_dict = contig_dict
         self.target_feature_type_dict = target_feature_type_dict  # should be a dictionary to convert feature types
         self.inference = inference
@@ -41,21 +42,21 @@
                         seq = fasta.reverse_complement(seq)
                     inference = self.inference if self.inference else inference
                     qualifiers = re.split(r"[=;]", qualifiers)
                     qualifiers = [unquote(str) for str in qualifiers]
                     if len(qualifiers) % 2 != 0:
                         qualifiers = qualifiers[:-1]  # this happens for example with prodigal, ending with ";"
                     qualifiers = {qualifiers[i].lower(): qualifiers[i + 1] for i in range(0, len(qualifiers), 2)}
-                    feature = {'contig': contig_name,
-                               'start': start,
-                               'end': end,
-                               'strand': strand,
-                               'type': self.target_feature_type_dict[feature_type],
-                               'inference': inference,
-                               'nt_seq': seq}
+                    feature = Feature(contig=contig_name,
+                               start=start,
+                               end=end,
+                               strand=strand,
+                               type=self.target_feature_type_dict[feature_type],
+                               inference=inference,
+                               nt_seq=seq)
                     yield feature
 
 
 def parse_feature_qualifiers_from_gff(qualifier_str) -> {}:
     qal = re.split(r"[=;]", qualifier_str)
     qal = [unquote(str) for str in qal]
     if len(qal) % 2 != 0:
```

### Comparing `metaerg-2.3.8/src/metaerg/datatypes/ncbi_ftp.py` & `metaerg-2.3.9/src/metaerg/datatypes/ncbi_ftp.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.3.8/src/metaerg/functional_gene_configuration.py` & `metaerg-2.3.9/src/metaerg/functional_gene_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 import pandas as pd
 from pathlib import Path
 
 from metaerg import context
+from metaerg.datatypes import sqlite
 from metaerg.datatypes.blast import BlastResult, BlastHit
 
 DATAFRAME_INDEX = None
 SUBSYSTEM_DATA = pd.DataFrame()
 CONFIG_DATA_FILE_EXTENSION = '.config.txt'
 
 
@@ -89,18 +90,18 @@
         else:
             collected_subsystems[s] = 0
     subsystem_str = ' '.join((f'[{val[0]}|{val[1]:.1f}]' for val in sorted(collected_subsystems.items(),
                                                                            key=lambda x: (-x[1], x[0]))))
     return subsystem_str.strip()
 
 
-def aggregate(feature_data: pd.DataFrame):
+def aggregate(db_connection):
     aggregated_subsystem_data = SUBSYSTEM_DATA.copy().sort_index()
     unstructured_subsystems = {}
-    for feature in feature_data.itertuples():
+    for feature in sqlite.read_all_features(db_connection):
         if not len(feature.subsystems):
             continue
         for s in re.split(r'\s(?=\[)', feature.subsystems):  # split at space if followed b y [
             s = s[1:-1]
             try:
                 gene_subsystem, gene_function, confidence = s.split('|')
                 try:
```

### Comparing `metaerg-2.3.8/src/metaerg/html/html_all_genomes.py` & `metaerg-2.3.9/src/metaerg/html/html_all_genomes.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.3.8/src/metaerg/html/html_feature_details.py` & `metaerg-2.3.9/src/metaerg/html/html_feature_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from pathlib import Path
-import pandas as pd
 from math import log10
+
+from metaerg.datatypes import sqlite
 from metaerg.datatypes.blast import DBentry, BlastHit, BlastResult, taxon_at_genus
 from metaerg import context
 
 MAX_BLAST_HITS = 10
 COLORS = 'id=cr id=cr id=co id=cb id=cg'.split()
 
 
 @context.register_html_writer
-def write_html(genome_name, feature_data: pd.DataFrame, genome_properties:dict, dir):
+def write_html(genome_name, db_connection, genome_properties:dict, dir):
     """Writes a html file for each feature to dir <file>"""
     dir = Path(dir, genome_name)
     dir.mkdir(exist_ok=True, parents=True)
     file = dir / 'feature-details.html'
 
     feature_html = ''
-    for feature in feature_data.itertuples():
+    for feature in sqlite.read_all_features(db_connection, type=('CDS', 'rRNA', 'ncRNA', 'retrotransposon')):
         if feature.type in ('CDS', 'rRNA', 'ncRNA', 'retrotransposon'):
             feature_html += make_feature_html(feature, genome_properties['dominant taxon'])
 
     html = _make_html_template().replace('FEATURE_HTML', feature_html)
     with open(file, 'w') as handle:
         handle.write(html)
 
 
-def make_blast_table_html(blast_result: str, f_length, dominant_taxon, include_id, title: str,
+def make_blast_table_html(blast_result: BlastResult, f_length, dominant_taxon, include_id, title: str,
                           headers: str ='percent id|query align|hit align|description|taxon') -> str:
     if blast_result:
-        blast_result = eval(blast_result)
         html = f'<h3>{title}</h3>\n'
         html += '<table><thead><tr>\n'
         columns = headers.split('|')
         for column in columns:
             if column == 'description':
                 html += f'<th id=al>{column}</th>\n'
             else:
@@ -98,15 +98,17 @@
     html = html.replace('CDD_TABLE', make_blast_table_html(f.cdd, length, dominant_taxon, include_id = True,
                                                            title='Top Conserved Domain Database Hits',
                                                            headers='percent id|query align|hit align|description| '))
     html = html.replace('HMM_TABLE', make_blast_table_html(f.hmm, length, dominant_taxon, include_id = True,
                                                            title='Top Functional Gene HMM Hits',
                                                            headers='evalue|query align|hit align|description| '))
     attribute_html = '<table>\n'
-    attribute_html += ''.join(f'<tr><td id=al>{k}</td><td id=al>{f._asdict()[k]}</td></tr>\n' for k in
+    f.tmh = '' if not f.tmh else f.tmh
+    f_as_dict = {k:v for k,v in f}
+    attribute_html += ''.join(f'<tr><td id=al>{k}</td><td id=al>{f_as_dict[k]}</td></tr>\n' for k in
                               ('start', 'end', 'strand', 'type', 'inference', 'subsystems', 'descr', 'taxon', 'notes',
                                'antismash', 'signal_peptide', 'tmh', 'tmh_topology'))
     attribute_html += f'<tr><td id=al>length</td><td id=al>{length} {length_unit}</td></tr>\n'
     attribute_html += '</table>\n'
     html = html.replace('ATTRIBUTE_TABLE', attribute_html)
     return html
```

### Comparing `metaerg-2.3.8/src/metaerg/html/html_feature_table.py` & `metaerg-2.3.9/src/metaerg/html/html_feature_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from pathlib import Path
-import pandas as pd
+
 from metaerg import context
-from metaerg.datatypes.blast import taxon_at_genus, DBentry, BlastHit, BlastResult
+from metaerg.datatypes import sqlite
+from metaerg.datatypes.blast import taxon_at_genus
 
 
 @context.register_html_writer
-def write_html(genome_name, feature_data: pd.DataFrame, genome_properties:dict, dir):
+def write_html(genome_name, db_connection, genome_properties:dict, dir):
     dir.mkdir(exist_ok=True, parents=True)
     file = Path(dir, genome_name, "feature_table.html")
     file.parent.mkdir(exist_ok=True, parents=True)
     with open(Path(file), 'w') as handle:
-        handle.write(make_html(genome_name, feature_data, genome_properties))
+        handle.write(make_html(genome_name, db_connection, genome_properties))
 
 
 def get_empty_format_dict():
     return {'f_id': '',
             'strand': '',
             'length': 0,
             'type': '',
@@ -25,15 +26,15 @@
             'align': '',
             'recall': '',
             'description': '',
             'taxon': '',
             'ci': '', 'ca': '', 'cr': '', 'ct': ''}
 
 
-def format_feature(f, format_hash, dominant_taxon, colors, path_to_feature_html):
+def format_feature(f: sqlite.Feature, format_hash, dominant_taxon, colors):
     format_hash['f_id'] = f.id
     format_hash['taxon'] = taxon_at_genus(f.taxon)
     format_hash['type'] = f.type
     if f.type in ('CDS', 'rRNA', 'ncRNA', 'retrotransposon'):
         format_hash['description'] = '<a target="Gene Details" href="feature-details.html#{}">{}</a>'.format(
             f'{f.id}', f.descr)
     else:
@@ -54,40 +55,36 @@
             format_hash['destination'] = 'envelope'
         case [_, _, 'CDS']:
             format_hash['destination'] = 'cytoplasm'
         case [*_]:
             format_hash['destination'] = ''
     format_hash['subsystem'] = f.subsystems
     format_hash['has_cdd'] = 'Y' if f.cdd is not None else ''
-    try:
-        if len(f.blast):
-            blast_result = eval(f.blast)
-            format_hash['ident'] = f'{blast_result.hits[0].percent_id:.1f}'
-            format_hash['ci'] = colors[min(int(blast_result.hits[0].percent_id / 20), len(colors) - 1)]
-            format_hash['align'] = f'{blast_result.percent_aligned():.1f}'
-            format_hash['ca'] = colors[min(int(blast_result.percent_aligned() / 20), len(colors) - 1)]
-            format_hash['recall'] = f'{blast_result.percent_recall():.1f}'
-            format_hash['cr'] = colors[min(int(blast_result.percent_recall() / 20), len(colors) - 1)]
-    except SyntaxError:
-        print(f.blast)
+    if f.blast:
+        format_hash['ident'] = f'{f.blast.hits[0].percent_id:.1f}'
+        format_hash['ci'] = colors[min(int(f.blast.hits[0].percent_id / 20), len(colors) - 1)]
+        format_hash['align'] = f'{f.blast.percent_aligned():.1f}'
+        format_hash['ca'] = colors[min(int(f.blast.percent_aligned() / 20), len(colors) - 1)]
+        format_hash['recall'] = f'{f.blast.percent_recall():.1f}'
+        format_hash['cr'] = colors[min(int(f.blast.percent_recall() / 20), len(colors) - 1)]
     dominant_taxon = dominant_taxon.split()
     taxon = f.taxon.split()
     format_hash['ct'] = colors[int(len(colors) * len(set(taxon) & set(dominant_taxon)) / (len(taxon) + 1))]
 
 
 def format_hash_to_html(format_hash):
     return '''<tr>
     <td id=al>{f_id}</td> <td>{strand}</td> <td>{length:,}</td> <td>{type}</td> <td>{destination}</td> 
     <td>{subsystem}</td> <td>{has_cdd}</td> <td{ci}>{ident}</td> <td{ca}>{align}</td> <td{cr}>{recall}</td> 
     <td id=al>{description}</td>
     <td{ct}>{taxon}</td>
     </tr>'''.format(**format_hash)
 
 
-def make_html(genome_name, feature_data: pd.DataFrame, genome_properties:dict, path_to_feature_html='') -> str:
+def make_html(genome_name, db_connection, genome_properties:dict) -> str:
     """Injects the content into the html base, returns the html."""
     html = _make_html_template()
     html = html.replace('GENOME_NAME', genome_name)
     colors = [' id=cr', ' id=cr', ' id=co', ' id=cb', ' id=cg']
 
     # table header
     table_headers = ''
@@ -97,34 +94,34 @@
         else:
             table_headers += f'<th>{column}</th>\n'
     html = html.replace('TABLE_HEADERS', table_headers)
     # table body
     table_body = ''
     previous_repeats = []
     prev_f = None
-    for f in feature_data.itertuples():
-        if f.type in ('crispr_repeat', 'repeat') and (not len(previous_repeats) or (f and f.type is prev_f.type)):
+    for f in sqlite.read_all_features(db_connection):
+        if f.type in ('crispr_repeat', 'repeat') and (not len(previous_repeats) or (f and f.type == prev_f.type)):
             previous_repeats.append(f)
         elif len(previous_repeats):
             format_hash = get_empty_format_dict()
             format_hash['description'] = previous_repeats[0].id + ' ... ' + previous_repeats[-1].id
             format_hash['type'] = f'[{len(previous_repeats)} {prev_f.type}s]' if len(previous_repeats) > 1 \
                                   else prev_f.type
             format_hash['length'] = previous_repeats[-1].end - previous_repeats[0].start
             previous_repeats.clear()
             table_body += format_hash_to_html(format_hash)
             if f.type in ('crispr_repeat', 'repeat'):
                 previous_repeats.append(f)
             else:
                 format_hash = get_empty_format_dict()
-                format_feature(f, format_hash, genome_properties['dominant taxon'], colors, path_to_feature_html)
+                format_feature(f, format_hash, genome_properties['dominant taxon'], colors)
                 table_body += format_hash_to_html(format_hash)
         else:
             format_hash = get_empty_format_dict()
-            format_feature(f, format_hash, genome_properties['dominant taxon'], colors, path_to_feature_html)
+            format_feature(f, format_hash, genome_properties['dominant taxon'], colors)
             table_body += format_hash_to_html(format_hash)
         prev_f = f
     html = html.replace('TABLE_BODY', table_body)
     return html
 
 
 def _make_html_template() -> str:
```

### Comparing `metaerg-2.3.8/src/metaerg/html/html_genome_properties_and_subsystems.py` & `metaerg-2.3.9/src/metaerg/html/html_genome_properties_and_subsystems.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from pathlib import Path
-import pandas as pd
 from metaerg import context
 
 GENOME_PROPERTY_FORMATS = {'size': ',',
                            '% GC': '.1%',
                            'N50': ',',
                            '# proteins': ',',
                            '% coding': '.1%',
@@ -20,22 +19,22 @@
                            '% of CDS classified to dominant taxon': '.1%',
                            'dominant taxon': '<',
                            'codon usage bias': '.3f',
                            'doubling_time (days)': '.1f'
                            }
 
 @context.register_html_writer
-def write_html(genome_name, feature_data: pd.DataFrame, genome_properties:dict, dir):
+def write_html(genome_name, db_connection, genome_properties:dict, dir):
     dir.mkdir(exist_ok=True, parents=True)
     file = Path(dir, genome_name, 'index.html')
     with open(file, 'w') as handle:
-        handle.write(make_html(genome_name, feature_data, genome_properties))
+        handle.write(make_html(genome_name, genome_properties))
 
 
-def make_html(genome_name, feature_data: pd.DataFrame, genome_properties:dict, path_to_feature_html='') -> str:
+def make_html(genome_name, genome_properties:dict) -> str:
     """injects the content into the html base, returns the html"""
     html = _make_html_template()
     html = html.replace('GENOME_NAME', genome_name)
     # genome properties
     html = html.replace('CONTENT_PROPERTIES', ''.join((f'<tr><td>{k}</td><td>{genome_properties[k]:{GENOME_PROPERTY_FORMATS[k]}}</td></tr>\n'
                                                        for k in GENOME_PROPERTY_FORMATS.keys())))
     subsystem_html = ''
```

### Comparing `metaerg-2.3.8/src/metaerg/installation.py` & `metaerg-2.3.9/src/metaerg/installation.py`

 * *Files identical despite different names*

### Comparing `metaerg-2.3.8/src/metaerg/main.py` & `metaerg-2.3.9/src/metaerg/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import argparse
 import tarfile
-
-import pandas
-import pandas as pd
 from pathlib import Path
 from concurrent import futures
 from hashlib import md5
+from collections import Counter
+
+import pandas as pd
 
 import metaerg.run_and_read.diamond_and_blastn
 import metaerg.run_and_read.functional_genes
 import metaerg.run_and_read.antismash
+from metaerg.datatypes import sqlite
 from metaerg import context
 from metaerg import registry
 from metaerg import functional_gene_configuration
 from metaerg.datatypes import fasta, gbk
 from metaerg.html import html_all_genomes
 from metaerg.run_and_read import tmhmm
 from metaerg.installation import install_all_helper_programs
 from metaerg.calculations.codon_usage_bias import compute_codon_bias_estimate_doubling_time
 from metaerg.run_and_read import *
 from metaerg.html import *
 
-VERSION = "2.3.8"
+VERSION = "2.3.9"
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description='metaerg.py. (C) Marc Strous, Xiaoli Dong 2019, 2022')
     parser.add_argument('--contig_file', help='Fasta nucleotide file of the contigs, or dir that '
                                               'contains multiple fasta nucleotide files.')
     parser.add_argument('--database_dir', help='Dir that contains the annotation databases.')
@@ -42,15 +43,18 @@
     parser.add_argument('--translation_table', default=11, help='Which translation table to use (default 11).')
     parser.add_argument('--delimiter', default='.', help='Separater character used in feature ids.')
     parser.add_argument('--prefix', default='g', help='Prefix used when renaming genomes (default: g).')
     parser.add_argument('--checkm_dir', default='checkm', help='Dir with the checkm results (default: checkm)')
     parser.add_argument('--gtdbtk_dir', default='gtdbtk', help='Dir with the gtdbtk results (default: gtdbtk).')
     parser.add_argument('--download_database', default=False, action="store_true",
                         help='Download ready-made metaerg database.')
-    parser.add_argument('--create_database', default='', help='Create metaerg database from scratch.')
+    parser.add_argument('--create_database', default='all', help='Create metaerg database from scratch (default: all, '
+                                                                 'to create all components of the database.). Use '
+                                                                 'any combination of PVEBRCSA to only create specific '
+                                                                 'parts of the database (see README)')
     parser.add_argument('--install_deps', default='', help='Dir for installation of all dependencies '
                                                            '(helper programs). Dependencies will be installed here.')
     parser.add_argument('--path_to_signalp', default='', help='Path to signalp-6.0g.fast.tar.gz.')
     parser.add_argument('--path_to_tmhmm', default='', help='Path to tmhmm-2.0c.Linux.tar.gz.')
 
     return parser.parse_args()
 
@@ -88,115 +92,150 @@
             if delimiter in c_id:
                 raise Exception(f'Contig id {c_id} contains "{delimiter}"; change delimiter with '
                                 f'--delimiter [new delimiter] or use --rename_contigs')
     contigs = {c['id']: c for c in contigs}
     return contigs
 
 
-def compute_genome_properties(contig_dict: dict[str, dict], feature_data: pd.DataFrame) -> dict:
-    properties = {}
+def compute_genome_properties(contig_dict: dict[str, dict], db_connection) -> dict:
+    properties = {'# total features':         0,
+                  '# proteins':               0,
+                  '# ribosomal RNA':          0,
+                  '# transfer RNA':           0,
+                  '# non-coding RNA':         0,
+                  '# retrotransposons':       0,
+                  '# CRISPR repeats':         0,
+                  '# other repeats':          0,
+                  '% coding':                 0.0,
+                  '% repeats':                0.0,
+                  'mean protein length (aa)': 0.0,}
     contigs:list[dict] = list(contig_dict.values())
     contigs.sort(key=lambda c:len(c['seq']), reverse=True)
     properties['size'] = sum(len(c['seq']) for c in contigs)
     properties['% GC'] = sum((c['seq'].count('G') + c['seq'].count('G') for c in contigs)) / \
                                (properties['size'] - sum((c['seq'].count('N') for c in contigs)))
     cum_size = 0
     for c in contigs:
         cum_size += len(c['seq'])
         if cum_size >+ properties['size'] / 2:
             properties['N50'] = len(c['seq'])
             break
 
-    feature_data = feature_data.assign(length=feature_data['end'] - feature_data['start'])
-    feature_data_cds = feature_data[feature_data['type'] == 'CDS']
-    feature_data_repeats = feature_data[feature_data['type'].isin(('retrotransposon', 'crispr_repeat', 'repeat'))]
-
-    properties['# proteins'] = len(feature_data_cds.index)
-    properties['% coding'] = feature_data_cds['length'].sum() / properties['size']
-    properties['mean protein length (aa)'] = feature_data_cds['length'].mean() / 3
-    properties['# ribosomal RNA'] = len(feature_data[feature_data['type'] == 'rRNA'].index)
-    properties['# transfer RNA'] = len(feature_data[feature_data['type'] == 'tRNA'].index)
-    properties['# non-coding RNA'] = len(feature_data[feature_data['type'] == 'ncRNA'].index)
-    properties['# retrotransposons'] = len(feature_data[feature_data['type'] == 'retrotransposon'].index)
-    properties['# CRISPR repeats'] = len(feature_data[feature_data['type'] == 'crispr_repeat'].index)
-    properties['# other repeats'] = len(feature_data[feature_data['type'] == 'repeat'].index)
-    properties['% repeats'] = feature_data_repeats['length'].sum() / properties['size']
-    properties['# total features'] = len(feature_data.index)
-    taxon_counts = dict(feature_data_cds.taxon.value_counts(normalize=True))
-    properties['% CDS classified to taxon'] = 1 - taxon_counts['']
+    #feature_data = feature_data.assign(length=feature_data['end'] - feature_data['start'])
+    #feature_data_cds = feature_data[feature_data['type'] == 'CDS']
+    #feature_data_repeats = feature_data[feature_data['type'].isin(('retrotransposon', 'crispr_repeat', 'repeat'))]
+    taxon_counts = Counter()
+    for feature in sqlite.read_all_features(db_connection):
+        properties['# total features'] += 1
+        if feature.type == 'CDS':
+            properties['# proteins'] += 1
+            properties['% coding'] += feature.length_nt()
+            properties['mean protein length (aa)'] += feature.length_aa()
+            taxon_counts.update((feature.taxon,))
+        elif feature.type == 'rRNA':
+            properties['# ribosomal RNA'] += 1
+            taxon_counts.update((feature.taxon,))
+        elif feature.type == 'tRNA':
+            properties['# transfer RNA'] += 1
+            taxon_counts.update((feature.taxon,))
+        elif feature.type == 'ncRNA':
+            properties['# non-coding RNA'] += 1
+            taxon_counts.update((feature.taxon,))
+        elif feature.type == 'retrotransposon':
+            properties['# retrotransposons'] += 1
+            properties['% repeats'] += feature.length_nt()
+        elif feature.type == 'crispr_repeat':
+            properties['# CRISPR repeats'] += 1
+            properties['% repeats'] += feature.length_nt()
+        elif feature.type == 'repeat':
+            properties['# other repeats'] += 1
+            properties['% repeats'] += feature.length_nt()
+    properties['% coding'] /= properties['size']
+    properties['mean protein length (aa)'] /= properties['# proteins']
+    properties['% repeats'] /= properties['size']
+    properties['% CDS classified to taxon'] = 1 - taxon_counts[''] / taxon_counts.total()
     properties['dominant taxon'] = ''
     properties['% of CDS classified to dominant taxon'] = 0.0
     del taxon_counts['']
     for k, v in taxon_counts.items():
-        properties['% of CDS classified to dominant taxon'] = v / properties['% CDS classified to taxon']
+        properties['% of CDS classified to dominant taxon'] = v / taxon_counts.total()
         properties['dominant taxon'] = k
         break
-    codon_usage_bias, doubling_time = compute_codon_bias_estimate_doubling_time(feature_data)
+    codon_usage_bias, doubling_time = compute_codon_bias_estimate_doubling_time(db_connection)
     properties['codon usage bias'] = codon_usage_bias
     properties['doubling_time (days)'] = doubling_time
-    properties['subsystems'] = functional_gene_configuration.aggregate(feature_data)
+    properties['subsystems'] = functional_gene_configuration.aggregate(db_connection)
     return properties
 
 
 def annotate_genome(genome_name, input_fasta_file: Path):
     context.log(f'Started annotation of {genome_name}...')
     current_progress = context.parse_metaerg_progress(genome_name)
     if 'visualization=complete' in current_progress:
         context.log(f'({genome_name}) already completed!')
         return
-    # (1) prepare dataframe
-    feature_data = pd.DataFrame(columns=context.DATAFRAME_COLUMNS)
+    # (1) prepare sqlite3 database
+    db_file = context.spawn_file('annotations.sqlite', genome_name, context.BASE_DIR)
+    sqlite.create_db(db_file)
+    db_connection = sqlite.connect_to_db(db_file)
     # (2) load sequence data
     contig_dict = load_contigs(genome_name, input_fasta_file, delimiter=context.DELIMITER,
                                min_contig_length=context.MIN_CONTIG_LENGTH, rename_contigs=context.RENAME_CONTIGS)
     # (3) now annotate
     for annotator in context.sorted_annotators():
-        feature_data = annotator(genome_name, contig_dict, feature_data)
+        annotator(genome_name, contig_dict, db_connection)
     # feather_file = context.spawn_file("all_genes.feather", genome_name, context.BASE_DIR)
     # feature_data = pd.read_feather(feather_file)
     # feature_data = feature_data.set_index('id', drop=False)
 
     # (4) save results
-    context.log(f'({genome_name}) Now writing annotations to .fasta, .gbk and .feather...')
+    context.log(f'({genome_name}) Now writing annotations to .fasta, .gbk...')
     faa_file = context.spawn_file("faa", genome_name, context.BASE_DIR)
     rna_file = context.spawn_file("rna.fna", genome_name, context.BASE_DIR)
     gbk_file = context.spawn_file("gbk", genome_name, context.BASE_DIR)
     fna_file = context.spawn_file("fna", genome_name, context.BASE_DIR)
-    feather_file = context.spawn_file("all_genes.feather", genome_name, context.BASE_DIR)
-    fasta.write_features_to_fasta(feature_data, 'aa', faa_file, targets=('CDS',))
-    fasta.write_features_to_fasta(feature_data, 'nt', rna_file, targets=('rRNA tRNA tmRNA ncRNA retrotransposon'.split()))
-    fasta.write_contigs_to_fasta(contig_dict, fna_file)
+    fasta.write_features_to_fasta(db_connection, 'aa', faa_file, targets=('CDS',))
+    fasta.write_features_to_fasta(db_connection, 'nt', rna_file, targets=('rRNA tRNA tmRNA ncRNA retrotransposon'.split()))
+    fasta.write_contigs_to_fasta(contig_dict, fna_file, db_connection)
     with open(gbk_file, 'w') as gbk_writer:
-        gbk.gbk_write_genome(gbk_writer, contig_dict, feature_data)
-    feature_data = feature_data.reset_index(drop=True)
-    feature_data.to_feather(feather_file)
+        gbk.gbk_write_genome(gbk_writer, contig_dict, db_connection)
+    feature_count = sqlite.count_features(db_connection)
+    if feature_count < 1e6:
+        context.log(f'({genome_name}) Writing {feature_count} annotations to .feather format...')
+        feather_file = context.spawn_file("annotations.feather", genome_name, context.BASE_DIR)
+        rows = []
+        for feature in sqlite.read_all_features(db_connection):
+            rows.append({k: str(v) for k, v in feature})
+        pd.DataFrame(rows).to_feather(feather_file)
+    else:
+        context.log(f'({genome_name}) Skipping feather format, too many ({feature_count}) annotations...')
     # (5) visualize
-    genome_properties = compute_genome_properties(contig_dict, feature_data)
+    genome_properties = compute_genome_properties(contig_dict, db_connection)
     context.log(f'({genome_name}) Now writing final result as .html for visualization...')
     for html_writer in registry.HTML_WRITER_REGISTRY:
-        html_writer(genome_name, feature_data, genome_properties, context.HTML_DIR)
+        html_writer(genome_name, db_connection, genome_properties, context.HTML_DIR)
     # (5) update progress
     current_progress = context.parse_metaerg_progress(genome_name)
     current_progress += 'visualization=complete\n'
     context.write_metaerg_progress(genome_name, current_progress)
     context.log(f'({genome_name}) Completed html visualization.')
 
 
 def write_functional_genes_to_xls():
     excel_file = context.BASE_DIR / 'functional_genes.xls'
-    feather_files = [context.spawn_file("all_genes.feather", genome_name, context.BASE_DIR)
+    db_files = [context.spawn_file('annotations.sqlite', genome_name, context.BASE_DIR)
                      for genome_name in context.GENOME_NAMES]
     fna_files = [context.spawn_file("fna", genome_name, context.BASE_DIR)
                  for genome_name in context.GENOME_NAMES]
     genome_properties = {}
-    for feather_file, contig_file in zip(feather_files, fna_files):
+    for db_file, contig_file in zip(db_files, fna_files):
         genome_name = contig_file.stem
         contig_dict = load_contigs(genome_name, contig_file, delimiter='xxxx')
-        feature_data = pd.read_feather(feather_file)
-        genome_properties[genome_name] = compute_genome_properties(contig_dict, feature_data)
+        db_connection = sqlite.connect_to_db(db_file)
+        genome_properties[genome_name] = compute_genome_properties(contig_dict, db_connection)
 
     all_genome_feature_data = None
     for genome_name, genome_property_hash in genome_properties.items():
         subsystems_df = genome_property_hash['subsystems'].rename(columns={'genes': genome_name})
         try:
             subsystems_df.drop('', level=0, axis=0, inplace=True)
             subsystems_df.drop('secondary-metabolites', level=0, axis=0, inplace=True)
```

### Comparing `metaerg-2.3.8/src/metaerg/run_and_read/antismash.py` & `metaerg-2.3.9/src/metaerg/run_and_read/antismash.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,67 @@
 import shutil
 import os
-import pandas as pd
 from pathlib import Path
 
 from metaerg import context
 from metaerg.datatypes import gbk
+from metaerg.datatypes import sqlite
 
 
-def _run_programs(genome_name, contig_dict, feature_data: pd.DataFrame, result_files):
+def _run_programs(genome_name, contig_dict, db_connection, result_files):
     """Should execute the helper programs to complete the analysis"""
     gbk_file = context.spawn_file('gbk', genome_name)
     if context.MULTI_MODE:
         gbk_file = Path(gbk_file.parent, gbk_file.name + '.gbk')
     with open(gbk_file, 'w') as handle:
-        gbk.gbk_write_genome(handle, contig_dict, feature_data)
+        gbk.gbk_write_genome(handle, contig_dict, db_connection)
     context.run_external(f'antismash --genefinding-tool none --output-dir {result_files[0]} {gbk_file}')
 
 
-def _read_results(genome_name, contig_dict, feature_data: pd.DataFrame, result_files) -> tuple:
+def _read_results(genome_name, contig_dict, db_connection, result_files) -> int:
     """Should parse the result files and return the # of positives."""
     antismash_hit_count = 0
     for f in sorted(result_files[0].glob('*region*.gbk')):
         with gbk.GbkFeatureParser(f) as reader:
             antismash_region_name = ''
             antismash_region_number = 0
             for f_as_dict in reader:
-                antismash_hit_count += 1
                 if 'region' == f_as_dict['type']:
                     antismash_region_name = '{} {}'.format(f_as_dict['product'], f_as_dict['rules'])
                     antismash_region_number = int(f_as_dict['region_number'])
                 elif 'CDS' == f_as_dict['type']:
                     antismash_gene_function = f_as_dict.get('gene_functions', '')
                     antismash_gene_category = f_as_dict.get('gene_kind', '')
                     if antismash_region_name:
-                        try:
-                            if not f_as_dict['locus_tag'] in feature_data.index:
-                                # antismash sometimes predicts a new ORF, for example for a lassopeptide
-                                # we do not add this to the feature table
-                                continue
-                        except KeyError:
+                        feature = sqlite.read_feature_by_id(db_connection, f_as_dict['locus_tag'])
+                        if not feature:
+                            # antismash sometimes predicts a new ORF, for example for a lassopeptide
+                            # we do not add this to the feature table
                             continue
-                        feature_data.at[f_as_dict['locus_tag'], 'antismash'] = \
-                            ' '.join((f'(region {antismash_region_number})', antismash_region_name,
-                                      antismash_gene_function, antismash_gene_category))
-                        prev_subsystem_text = feature_data.at[f_as_dict['locus_tag'], 'subsystems']
-                        if type(prev_subsystem_text) == str and '[secondary-metabolites]' not in prev_subsystem_text:
-                                feature_data.at[f_as_dict['locus_tag'], 'subsystems'] += ' [secondary-metabolites]'
-                        elif f_as_dict['locus_tag'] in feature_data.index:
-                            print(f"starting: '{f_as_dict['locus_tag']}'")
-                            feature_data.at[f_as_dict['locus_tag'], 'subsystems'] = '[secondary-metabolites]'
-    if not antismash_hit_count:
-        result_files[0].mkdir(exist_ok=True)  # to prevent re-doing fruitless searches
-    return feature_data, antismash_hit_count
+                        feature.antismash =  ' '.join((f'(region {antismash_region_number})', antismash_region_name,
+                                                       antismash_gene_function, antismash_gene_category))
+                        feature.subsystems = (feature.subsystems + ' [secondary-metabolites]').strip()
+                        sqlite.update_feature_in_db(db_connection, feature)
+                        antismash_hit_count += 1
+    return antismash_hit_count
 
 
 @context.register_annotator
 def run_and_read_antismash():
     return ({'pipeline_position': 91,
              'annotator_key': 'antismash',
              'purpose': 'prediction of secondary metabolite genes with antismash',
              'programs': ('antismash',),
              'result_files': ('antismash',),
              'run': _run_programs,
              'read': _read_results})
 
 
 @context.register_html_writer
-def write_html(genome_name, feature_data: pd.DataFrame, genome_properties:dict, dir):
+def write_html(genome_name, db_connection, genome_properties:dict, dir):
     """need to copy the antismash result dir to the metaerg html dir."""
     dir.mkdir(exist_ok=True, parents=True)
     antismash_result_dir = context.spawn_file('antismash', genome_name)
     antismash_html_parent = Path(dir, genome_name, 'antismash')
     if antismash_html_parent.exists():
         shutil.rmtree(antismash_html_parent)
     if antismash_result_dir.exists():
```

### Comparing `metaerg-2.3.8/src/metaerg/run_and_read/aragorn.py` & `metaerg-2.3.9/src/metaerg/run_and_read/aragorn.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import re
-import pandas as pd
+
 from metaerg import context
 from metaerg.datatypes import fasta
+from metaerg.datatypes import sqlite
 
 
-def _run_programs(genome_name, contig_dict, feature_data: pd.DataFrame, result_files):
+def _run_programs(genome_name, contig_dict, db_connection, result_files):
     fasta_file = context.spawn_file('masked', genome_name)
-    fasta.write_contigs_to_fasta(contig_dict, fasta_file, feature_data, genome_name,
+    fasta.write_contigs_to_fasta(contig_dict, fasta_file, db_connection, genome_name,
                                       mask_targets=fasta.ALL_MASK_TARGETS)
     context.run_external(f'aragorn -l -t -gc{context.TRANSLATION_TABLE} {fasta_file} -w -o {result_files[0]}')
 
-def _read_results(genome_name, contig_dict, feature_data: pd.DataFrame, result_files) -> tuple:
-    new_features = []
+def _read_results(genome_name, contig_dict, db_connection, result_files) -> int:
+    count = 0
     current_contig = None
     coord_regexp = re.compile(r'(c*)\[(\d+),(\d+)]')
     with open(result_files[0]) as aragorn_handle:
         for line in aragorn_handle:
             words = line.strip().split()
             match words:
                 case ['>end']:
@@ -26,26 +27,26 @@
                     if coord_match := coord_regexp.fullmatch(coordinates):
                         strand = -1 if 'c' == coord_match.group(1) else 1
                         start = max(0, int(coord_match.group(2)) - 1)
                         end = min(len(current_contig['seq']), int(coord_match.group(3)))
                         seq = current_contig['seq'][start:end]
                         if strand < 0:
                             seq = fasta.reverse_complement(seq)
-                        feature = {'genome': genome_name,
-                                   'contig': current_contig['id'],
-                                   'start': start,
-                                   'end': end,
-                                   'strand': strand,
-                                   'type': 'tRNA',
-                                   'inference': 'aragorn',
-                                   'nt_seq': seq,
-                                   'descr': f'{trna}-{codon}'}
-                        new_features.append(feature)
-    feature_data = pd.concat([feature_data, pd.DataFrame(new_features)], ignore_index=True)
-    return feature_data, len(new_features)
+                        feature = sqlite.Feature(genome = genome_name,
+                                   contig = current_contig['id'],
+                                   start = start,
+                                   end = end,
+                                   strand = strand,
+                                   type = 'tRNA',
+                                   inference = 'aragorn',
+                                   nt_seq = seq,
+                                   descr = f'{trna}-{codon}')
+                        sqlite.add_new_feature_to_db(db_connection, feature)
+                        count += 1
+    return count
 
 
 @context.register_annotator
 def run_and_read_aragorn():
     return ({'pipeline_position': 11,
              'annotator_key': 'aragorn',
              'purpose': 'tRNA prediction with aragorn',
```

### Comparing `metaerg-2.3.8/src/metaerg/run_and_read/cdd.py` & `metaerg-2.3.9/src/metaerg/run_and_read/cdd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 import shutil
-import pandas as pd
 from pathlib import Path
 from concurrent.futures import ProcessPoolExecutor
 
 from metaerg import context
 from metaerg import functional_gene_configuration
 from metaerg.datatypes import fasta
+from metaerg.datatypes import sqlite
 from metaerg.datatypes.blast import DBentry, TabularBlastParser
 
 
-def _run_programs(genome_name, contig_dict, feature_data: pd.DataFrame, result_files):
+def _run_programs(genome_name, contig_dict, db_connection, result_files):
     cds_aa_file = context.spawn_file('cds.faa', genome_name)
     cdd_database = Path(context.DATABASE_DIR, 'cdd', 'Cdd')
     if context.CPUS_PER_GENOME > 1:
-        split_fasta_files = fasta.write_features_to_fasta(feature_data, 'aa', cds_aa_file, targets=('CDS',),
+        split_fasta_files = fasta.write_features_to_fasta(db_connection, 'aa', cds_aa_file, targets=('CDS',),
                                                                split=context.CPUS_PER_GENOME)
         split_cdd_files = [Path(result_files[0].parent, f'{result_files[0].name}.{i}')
                            for i in range(len(split_fasta_files))]
         with ProcessPoolExecutor(max_workers=context.CPUS_PER_GENOME) as executor:
             for split_input, split_output in zip(split_fasta_files, split_cdd_files):
                 executor.submit(context.run_external, f'rpsblast -db {cdd_database} -query {split_input} '
                                                       f'-out {split_output} -outfmt 6 -evalue 1e-7')
@@ -29,15 +29,15 @@
                     shutil.copyfileobj(input, output)
                 split_input_file.unlink()
                 split_output_file.unlink()
     else:
         context.run_external(f'rpsblast -db {cdd_database} -query {cds_aa_file} -out {result_files[0]} -outfmt 6 -evalue 1e-7')
 
 
-def _read_results(genome_name, contig_dict, feature_data: pd.DataFrame, result_files) -> tuple:
+def _read_results(genome_name, contig_dict, db_connection, result_files) -> int:
     # load cdd index
     cdd = {}
     cdd_index = Path(context.DATABASE_DIR, 'cdd', 'cddid.tbl')
     with open(cdd_index) as db_handle:
         for line in db_handle:
             words = line.strip().split("\t")
             cdd[int(words[0])] = DBentry(domain='cdd', accession=words[1], gene=words[2], descr=words[3],
@@ -46,28 +46,29 @@
     # parse cdd results
     cdd_result_count = 0
     def get_cdd_db_entry(id: str) -> DBentry:
         return cdd[int(id[4:])]
 
     with TabularBlastParser(result_files[0], 'BLAST', get_cdd_db_entry) as handle:
         for cdd_result in handle:
-            if cdd_result.query() not in feature_data.index:
+            feature = sqlite.read_feature_by_id(db_connection, cdd_result.query())
+            if not feature:
                 raise Exception(f'Found results for unknown feature {cdd_result.query()}, '
                                 f'may need to rerun metaerg with --force')
-            feature_data.at[cdd_result.query(), 'cdd'] = str(cdd_result)
+            feature.cdd = cdd_result
             cdd_result_count += 1
             if new_subsystem := functional_gene_configuration.match(cdd_result):
-                feature_data.at[cdd_result.query(), 'subsystems'] = functional_gene_configuration.cleanup_subsystem_str(
-                    feature_data.at[cdd_result.query(), 'subsystems'].strip() + ' ' + new_subsystem)
+                feature.subsystems = functional_gene_configuration.cleanup_subsystem_str(
+                    feature.subsystems.strip() + ' ' + new_subsystem)
             top_entry: DBentry = cdd_result.hits[0].hit
-            descr = f'{top_entry.accession}|{top_entry.gene} {top_entry.descr}'
-            if len(descr) > 35:
-                descr = descr[:35] + '...'
-            feature_data.at[cdd_result.query(), 'descr'] = descr
-    return feature_data, cdd_result_count
+            feature.descr = f'{top_entry.accession}|{top_entry.gene} {top_entry.descr}'
+            if len(feature.descr) > 35:
+                feature.descr = feature.descr[:35] + '...'
+            sqlite.update_feature_in_db(db_connection, feature)
+    return cdd_result_count
 
 
 @context.register_annotator
 def run_and_read_cdd():
     return ({'pipeline_position': 71,
              'annotator_key': 'cdd',
              'purpose': 'function prediction using RPSBlast and the conserved domain database',
```

### Comparing `metaerg-2.3.8/src/metaerg/run_and_read/cmscan.py` & `metaerg-2.3.9/src/metaerg/run_and_read/cmscan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import shutil
-import pandas as pd
 from pathlib import Path
 from concurrent.futures import ProcessPoolExecutor
 from collections import namedtuple
 
 from metaerg import context
 from metaerg.datatypes import fasta
+from metaerg.datatypes import sqlite
 
 
-def _run_programs(genome_name, contig_dict, feature_data: pd.DataFrame, result_files):
+def _run_programs(genome_name, contig_dict, db_connection, result_files):
     fasta_file = context.spawn_file('masked', genome_name)
     rfam_database = Path(context.DATABASE_DIR, 'rfam', 'Rfam.cm')
     if context.CPUS_PER_GENOME > 1:
-        split_fasta_files = fasta.write_contigs_to_fasta(contig_dict, fasta_file, feature_data, genome_name,
+        split_fasta_files = fasta.write_contigs_to_fasta(contig_dict, fasta_file, db_connection, genome_name,
                                                          mask_targets=fasta.ALL_MASK_TARGETS,
                                                          split=context.CPUS_PER_GENOME)
         split_cmscan_files = [Path(result_files[0].parent, f'{result_files[0].name}.{i}')
                               for i in range(len(split_fasta_files))]
         with ProcessPoolExecutor(max_workers=context.CPUS_PER_GENOME) as executor:
             for split_input, split_output in zip(split_fasta_files, split_cmscan_files):
                 executor.submit(context.run_external, f'cmscan --rfam --tblout {split_output} {rfam_database} '
@@ -24,20 +24,20 @@
         with open(result_files[0], 'wb') as output:
             for split_input_file, split_output_file in zip(split_fasta_files, split_cmscan_files):
                 with open(split_output_file, 'rb') as input:
                     shutil.copyfileobj(input, output)
                 split_input_file.unlink()
                 split_output_file.unlink()
     else:
-        fasta.write_contigs_to_fasta(contig_dict, fasta_file, feature_data, genome_name,
+        fasta.write_contigs_to_fasta(contig_dict, fasta_file, db_connection, genome_name,
                                      mask_targets=fasta.ALL_MASK_TARGETS)
         context.run_external(f'cmscan --rfam --tblout {result_files[0]} {rfam_database} {fasta_file}')
 
 
-def _read_results(genome_name, contig_dict, feature_data: pd.DataFrame, result_files) -> tuple:
+def _read_results(genome_name, contig_dict, db_connection, result_files) -> int:
     NON_CODING_RNA_TYPES = {'LSU_rRNA_bacteria': 'rRNA',
                             'LSU_rRNA_archaea': 'rRNA',
                             'LSU_rRNA_eukarya': 'rRNA',
                             'SSU_rRNA_bacteria': 'rRNA',
                             'SSU_rRNA_archaea': 'rRNA',
                             'SSU_rRNA_eukarya': 'rRNA',
                             'SSU_rRNA_microsporidia': 'rRNA',
@@ -69,38 +69,38 @@
                     break
             if overlap:
                 if hit.score > overlap.score:
                     hits.remove(overlap)
                     hits.append(hit)
             else:
                 hits.append(hit)
-    new_features = []
+    count = 0
     for hit in hits:
         if hit.hit_id in NON_CODING_RNA_TYPES.keys():
             f_type = NON_CODING_RNA_TYPES[hit.hit_id]
         elif hit.hit_id.startswith('CRISPR'):
             f_type = 'crispr_repeat'
         else:
             f_type = 'ncRNA'
         contig = contig_dict[hit.query_id]
         seq = contig['seq'][hit.query_start - 1:hit.query_end]
         if hit.query_strand < 0:
             seq = fasta.reverse_complement(seq)
-        feature = {'genome': genome_name,
-                   'contig': hit.query_id,
-                   'start': hit.query_start - 1,
-                   'end': hit.query_end,
-                   'strand': hit.query_strand,
-                   'type': f_type,
-                   'inference': 'cmscan',
-                   'nt_seq': seq,
-                   'descr': "{} {}".format(hit.hit_id, hit.descr)}
-        new_features.append(feature)
-    feature_data = pd.concat([feature_data, pd.DataFrame(new_features)], ignore_index=True)
-    return feature_data, len(new_features)
+        feature = sqlite.Feature(genome = genome_name,
+                   contig = hit.query_id,
+                   start = hit.query_start - 1,
+                   end = hit.query_end,
+                   strand = hit.query_strand,
+                   type = f_type,
+                   inference = 'cmscan',
+                   nt_seq = seq,
+                   descr = "{} {}".format(hit.hit_id, hit.descr))
+        sqlite.add_new_feature_to_db(db_connection, feature)
+        count += 1
+    return count
 
 
 @context.register_annotator
 def run_and_read_cmscan():
     return ({'pipeline_position': 21,
              'annotator_key': 'cmscan',
              'purpose': 'noncoding (RNA) gene prediction with cmscan',
```

### Comparing `metaerg-2.3.8/src/metaerg/run_and_read/data/functional_gene_data` & `metaerg-2.3.9/src/metaerg/run_and_read/data/functional_gene_data`

 * *Files identical despite different names*

### Comparing `metaerg-2.3.8/src/metaerg/run_and_read/diamond_and_blastn.py` & `metaerg-2.3.9/src/metaerg/run_and_read/diamond_and_blastn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import re
 import gzip
 import shutil
-import pandas as pd
 from os import chdir
 from ftplib import FTP
 from pathlib import Path
 
 from Bio import SeqIO
 from Bio.SeqRecord import SeqRecord
 from Bio.Seq import Seq
 import ncbi.datasets
 
 from metaerg import context
 from metaerg.datatypes import fasta
+from metaerg.datatypes import sqlite
 from metaerg.datatypes.blast import BlastResult, DBentry, TabularBlastParser
 from metaerg.datatypes import ncbi_ftp
 
 DB_DESCRIPTIONS_FILENAME = 'db_descriptions.txt'
 DB_TAXONOMY_FILENAME = 'db_taxonomy.txt'
 DB_PROTEINS_FILENAME = 'db_protein.faa'
 DB_RNA_FILENAME = 'db_rna.fna'
@@ -26,15 +26,15 @@
                          'autocatalytically_spliced_intron'.split()
 IGNORED_FEATURE_TYPES = 'gene pseudogene exon direct_repeat region sequence_feature pseudogenic_tRNA pseudogenic_rRNA ' \
                         'repeat_region ribosome_entry_site minus_10_signal minus_35_signal protein_binding_site ' \
                         'regulatory transcript mRNA gap assembly_gap source misc_feature variation misc_structure ' \
                         'transcript 3\'UTR 5\'UTR intron signal_peptide_region_of_CDS sequence_alteration'.split()
 
 
-def _run_programs(genome_name, contig_dict, feature_data: pd.DataFrame, result_files):
+def _run_programs(genome_name, contig_dict, db_connection, result_files):
     rna_nt_file = context.spawn_file('rna.fna', genome_name)
     blastn_result_file = context.spawn_file('blastn', genome_name)
     if rna_nt_file.exists() and rna_nt_file.stat().st_size:
         if context.FORCE or not blastn_result_file.exists() or not blastn_result_file.stat().st_size:
             blastn_db = Path(context.DATABASE_DIR, DB_RNA_FILENAME)
             context.run_external(f'blastn -db {blastn_db} -query {rna_nt_file} -out {blastn_result_file} -max_target_seqs 10 '
                                  f'-outfmt 6')
@@ -43,15 +43,15 @@
 
     cds_aa_file = context.spawn_file('cds.faa', genome_name)
     diamond_db = Path(context.DATABASE_DIR, DB_PROTEINS_FILENAME)
     context.run_external(f'diamond blastp -d {diamond_db} -q {cds_aa_file} -o {result_files[0]} -f 6 '
                          f'--threads {context.CPUS_PER_GENOME} --fast --max-target-seqs 10')
 
 
-def _read_results(genome_name, contig_dict, feature_data: pd.DataFrame, result_files) -> tuple:
+def _read_results(genome_name, contig_dict, db_connection, result_files) -> int:
     # (1) load databse descriptions
     db_descr = Path(context.DATABASE_DIR, DB_DESCRIPTIONS_FILENAME)
     descriptions = {'p': {}, 'e': {}, 'v': {}}
     entries_without_descr = 0
     with open(db_descr) as descr_handle:
         for line in descr_handle:
             words = line.split('\t')
@@ -69,20 +69,22 @@
             words = line.split('\t')
             taxonomy[words[0]][int(words[1])] = words[2].strip().replace('~', '; ')
     context.log(f'({genome_name}) Parsed ({len(taxonomy["p"])}, {len(taxonomy["e"])}, {len(taxonomy["v"])}) '
                 f'taxa from db for (prokaryotes, eukaryotes and viruses) respectively.')
     # (3) parse diamond blast results
 
     def process_blast_result(blast_result: BlastResult):
-        if blast_result.query() not in feature_data.index:
+        feature = sqlite.read_feature_by_id(db_connection, blast_result.query())
+        if not feature:
             raise Exception(f'Found results for unknown feature {blast_result.query()}, '
                             f'may need to rerun metaerg with --force')
-        feature_data.at[blast_result.query(), 'blast'] = str(blast_result)
-        feature_data.at[blast_result.query(), 'descr'] = blast_result.hits[0].hit.descr
-        feature_data.at[blast_result.query(), 'taxon'] =  blast_result.hits[0].hit.taxon
+        feature.blast = blast_result
+        feature.descr = blast_result.hits[0].hit.descr
+        feature.taxon =  blast_result.hits[0].hit.taxon
+        sqlite.update_feature_in_db(db_connection, feature)
 
     def dbentry_from_string(db_id: str) -> DBentry:
         w = db_id.split('~')
         return DBentry(domain=w[0], taxon=taxonomy[w[0]][int(w[1])], descr=descriptions[w[0]][int(w[2])],
                        accession=w[3], gene=w[4], length=int(w[5]), pos=int(w[6]))
 
     blast_result_count = 0
@@ -92,15 +94,15 @@
             process_blast_result(blast_result)
 
     blastn_result_file = context.spawn_file('blastn', genome_name)
     with TabularBlastParser(blastn_result_file, 'BLAST', dbentry_from_string) as handle:
         for blast_result in handle:
             blast_result_count += 1
             process_blast_result(blast_result)
-    return feature_data, blast_result_count
+    return blast_result_count
 
 
 @context.register_annotator
 def run_and_read_diamond_blastn():
     return ({'pipeline_position': 81,
              'annotator_key': 'diamond_and_blastn',
              'purpose': 'function prediction and taxonomic classification of genes with diamond and blastn',
```

### Comparing `metaerg-2.3.8/src/metaerg/run_and_read/functional_genes.py` & `metaerg-2.3.9/src/metaerg/run_and_read/functional_genes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 import gzip
 import shutil
-import pandas as pd
 from math import log10
 from pathlib import Path
 from concurrent import futures
 
 from metaerg.datatypes.blast import DBentry, TabularBlastParser
+from metaerg.datatypes import sqlite
 from metaerg import context
 from metaerg import functional_gene_configuration
 
 
-def _run_programs(genome_name, contig_dict, feature_data: pd.DataFrame, result_files):
+def _run_programs(genome_name, contig_dict, db_connection, result_files):
     cds_aa_file = context.spawn_file('cds.faa', genome_name)
     hmm_db = context.DATABASE_DIR / 'hmm' / 'functional_genes.hmm'
     # the domtbl format includes alignment starts and ends, so we can use that information...
     context.run_external(f'hmmscan -o /dev/null -E 1e-6 --domtblout {result_files[0]} {hmm_db} {cds_aa_file}')
 
 
-def _read_results(genome_name, contig_dict, feature_data: pd.DataFrame, result_files) -> tuple:
+def _read_results(genome_name, contig_dict, db_connection, result_files) -> int:
     db_entry = None
     hmm_db = context.DATABASE_DIR / 'hmm' / 'functional_genes.hmm'
     functional_gene_db = {}
     with open(hmm_db) as handle:
         for line in handle:
             if line.startswith('NAME'):
                 name = line.split()[1]
@@ -42,37 +42,39 @@
 
     def get_db_entry(db_id) -> DBentry:
         return functional_gene_db[db_id]
 
     with TabularBlastParser(result_files[0], 'HMMSCAN_DOM_TABLE', get_db_entry) as handle:
         hit_count = 0
         for blast_result in handle:
-            if blast_result.query() not in feature_data.index:
+            feature = sqlite.read_feature_by_id(db_connection, blast_result.query())
+            if not feature:
                 raise Exception(f'Found results for unknown feature {blast_result.query()}, '
                                 f'may need to rerun metaerg with --force')
             blast_result.hits = blast_result.hits[:10]
-            feature_data.at[blast_result.query(), 'hmm'] = str(blast_result)
+            feature.hmm = blast_result
             for h in blast_result.hits:
                 db_entry = h.hit
                 confidence = 1.0
                 if h.aligned_length / db_entry.length < 0.7:
                     continue
                 if db_entry.min_score:
                     if h.score < db_entry.min_score:
                         continue
                     confidence = h.score / db_entry.min_t_score
                 else:
                     if h.evalue > 0:
                         confidence = min(1.0, - log10(h.evalue) / 100)
                 if new_subsystem := functional_gene_configuration.match_hit(h, confidence):
                     hit_count += 1
-                    feature_data.at[blast_result.query(), 'subsystems'] = functional_gene_configuration.cleanup_subsystem_str(
-                        feature_data.at[blast_result.query(), 'subsystems'].strip() + ' ' + new_subsystem)
+                    feature.subsystems = functional_gene_configuration.cleanup_subsystem_str(
+                        feature.subsystems.strip() + ' ' + new_subsystem)
                 break
-    return feature_data, hit_count
+            sqlite.update_feature_in_db(db_connection, feature)
+    return hit_count
 
 
 @context.register_annotator
 def run_and_read_canthyd():
     return ({'pipeline_position': 101,
              'annotator_key': 'hmm',
              'purpose': 'identification of functional genes with HMMs',
@@ -199,7 +201,8 @@
             if f == all_hmms_file:
                 continue
             add_hmm_file_to_db(hmm_file, output, names_done, all_target_hmm_names)
         for f in (hmm_dir / 'user_hmm').glob('*.hmm'):
             hmm_file = f.absolute()
             add_hmm_file_to_db(hmm_file, output, names_done, all_target_hmm_names)
     context.run_external(f'hmmpress -f {hmm_dir / "functional_genes.hmm"}')
+    os.chdir(current_working_dir)
```

### Comparing `metaerg-2.3.8/src/metaerg/run_and_read/ltr_harvest.py` & `metaerg-2.3.9/src/metaerg/run_and_read/ltr_harvest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-import pandas as pd
 from metaerg import context
 from metaerg.datatypes import fasta, gff
+from metaerg.datatypes import gff
+from metaerg.datatypes import sqlite
 
 
-def _run_programs(genome_name, contig_dict, feature_data: pd.DataFrame, result_files):
+def _run_programs(genome_name, contig_dict, db_connection, result_files):
     fasta_file = context.spawn_file('masked', genome_name)
-    fasta.write_contigs_to_fasta(contig_dict, fasta_file, feature_data, genome_name,
+    fasta.write_contigs_to_fasta(contig_dict, fasta_file, db_connection, genome_name,
                                  mask_targets=fasta.ALL_MASK_TARGETS)
     ltr_index_file = context.spawn_file('ltr_index', genome_name)
 
     context.run_external(f'gt suffixerator -db {fasta_file} -indexname {ltr_index_file} -tis -suf -lcp -des -ssp -sds -dna')
     context.run_external(f'gt ltrharvest -index {ltr_index_file} -gff3 {result_files[0]} -seqids')
     # remove index files
     for file in ltr_index_file.parent.glob(f'{genome_name}.ltr_index*'):
         file.unlink()
 
 
-def _read_results(genome_name, contig_dict, feature_data: pd.DataFrame, result_files) -> tuple:
-    new_features = []
+def _read_results(genome_name, contig_dict, db_connection, result_files) -> int:
+    count = 0
     with gff.GffParser(result_files[0], contig_dict, inference='ltr_harvest',
                        target_feature_type_dict={'repeat_region': 'retrotransposon'}) as parser:
         for feature in parser:
-            new_features.append(feature)
-    feature_data = pd.concat([feature_data, pd.DataFrame(new_features)], ignore_index=True)
-    return feature_data, len(new_features)
+            sqlite.add_new_feature_to_db(db_connection, feature)
+            count += 1
+    return count
 
 
 @context.register_annotator
 def run_and_read_ltr_harvest():
     return ({'pipeline_position': 31,
              'annotator_key': 'ltr_harvest',
              'purpose': 'retrotransposon prediction with ltrharvest',
```

### Comparing `metaerg-2.3.8/src/metaerg/run_and_read/minced.py` & `metaerg-2.3.9/src/metaerg/run_and_read/trf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,47 @@
-import pandas as pd
 from metaerg import context
-from metaerg.datatypes import fasta, gff
+from metaerg.datatypes import fasta
+from metaerg.datatypes import sqlite
 
 
-def _run_programs(genome_name, contig_dict, feature_data: pd.DataFrame, result_files):
-    """Executes the helper programs to complete the analysis"""
+def _run_programs(genome_name, contig_dict, db_connection, result_files):
     fasta_file = context.spawn_file('masked', genome_name)
-    fasta.write_contigs_to_fasta(contig_dict, fasta_file, feature_data, genome_name,
+    fasta.write_contigs_to_fasta(contig_dict, fasta_file, db_connection, genome_name,
                                  mask_targets=fasta.ALL_MASK_TARGETS)
-    context.run_external(f'minced -gffFull {fasta_file} {result_files[0]}')
-
-
-def _read_results(genome_name, contig_dict, feature_data: pd.DataFrame, result_files) -> tuple:
-    """Should parse the result files and return the # of positives"""
-    new_features = []
-    with gff.GffParser(result_files[0], contig_dict, inference='minced',
-                       target_feature_type_dict={'repeat_unit': 'crispr_repeat'}) as gff_parser:
-        for feature in gff_parser:
-            feature['genome'] = genome_name
-            new_features.append(feature)
-    feature_data = pd.concat([feature_data, pd.DataFrame(new_features)], ignore_index=True)
-    return feature_data, len(new_features)
+    with open(result_files[0], 'w') as output:
+        context.run_external(f'trf {fasta_file} 2 7 7 80 10 50 500 -d -h -ngs', stdout=output)
 
+def _read_results(genome_name, contig_dict, db_connection, result_files) -> int:
+    count = 0
+    with open(result_files[0]) as trf_handle:
+        for line in trf_handle:
+            if line.startswith("@"):
+                contig = contig_dict[line[1:].strip()]
+                continue
+            if not contig:
+                continue
+            words = line.split()
+            start = int(words[0]) - 1
+            end = int(words[1])
+            seq = contig['seq'][start:end]
+            feature = sqlite.Feature(genome = genome_name,
+                                     contig = contig['id'],
+                                     start = start,
+                                     end = end,
+                                     strand = 1,
+                                     type = 'repeat',
+                                     inference = 'tandem-repeat-finder',
+                                     nt_seq = seq,
+                                     notes = f'period size {words[2]}; copies {words[3]}')
+            sqlite.add_new_feature_to_db(db_connection, feature)
+            count += 1
+    return count
 
 @context.register_annotator
-def run_and_read_minced():
-    return ({'pipeline_position': 1,
-             'annotator_key': 'minced',
-             'purpose': 'CRISPR prediction with minced',
-             'programs': ('minced',),
-             'result_files': ("minced",),
+def run_and_read_trf():
+    return ({'pipeline_position': 41,
+             'annotator_key': 'trf',
+             'purpose': 'tandem repeat prediction with trf',
+             'programs': ('trf',),
+             'result_files': ('tandem-repeat-finder',),
              'run': _run_programs,
              'read': _read_results})
-
```

### Comparing `metaerg-2.3.8/src/metaerg/run_and_read/repeat_masker.py` & `metaerg-2.3.9/src/metaerg/run_and_read/repeat_masker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import shutil
-import pandas as pd
 from pathlib import Path
 
 from metaerg import context
 from metaerg.datatypes import fasta
+from metaerg.datatypes import sqlite
 
-
-def _run_programs(genome_name, contig_dict, feature_data: pd.DataFrame, result_files):
+def _run_programs(genome_name, contig_dict, db_connection, result_files):
     fasta_file = context.spawn_file('masked', genome_name)
-    fasta.write_contigs_to_fasta(contig_dict, fasta_file, feature_data, genome_name,
+    fasta.write_contigs_to_fasta(contig_dict, fasta_file, db_connection, genome_name,
                                  mask_targets=fasta.ALL_MASK_TARGETS)
     lmer_table_file = context.spawn_file('lmer-table', genome_name)
     repeatscout_file_raw = context.spawn_file('repeatscout-raw', genome_name)
     repeatscout_file_filtered = context.spawn_file('repeatscout-filtered', genome_name)
     repeatscout_file_filtered2 = context.spawn_file('repeatscout-filtered2', genome_name)
 
     context.run_external(f'build_lmer_table -sequence {fasta_file} -freq {lmer_table_file}')
@@ -51,61 +50,62 @@
     for file in fasta_input_file.parent.glob(f'{fasta_input_file.name}.*'):
         if file.is_dir():
             shutil.rmtree(file)
         else:
             file.unlink()
 
 
-def words2feature(words: list[str], contig, genome_name:str):
+def words2feature(words: list[str], contig, genome_name:str) -> sqlite.Feature:
     start = int(words[5]) - 1
     end = int(words[6])
     strand = -1 if 'C' == words[8] else 1
     seq = contig['seq'][start:end]
     if strand < 0:
         seq = fasta.reverse_complement(seq)
-    return {'genome': genome_name,
-            'contig': contig['id'],
-            'start': start,
-            'end': end,
-            'strand': strand,
-            'type': 'repeat',
-            'inference': 'repeatmasker',
-            'nt_seq': seq}
+    return sqlite.Feature(genome = genome_name,
+                          contig = contig['id'],
+                          start = start,
+                          end = end,
+                          strand = strand,
+                          type = 'repeat',
+                          inference = 'repeatmasker',
+                          nt_seq = seq)
 
 
-def _read_results(genome_name, contig_dict, feature_data: pd.DataFrame, result_files) -> tuple:
+def _read_results(genome_name, contig_dict, db_connection, result_files) -> int:
     """(1) simple repeats, these are consecutive
        (2) unspecified repeats, these occur scattered and are identified by an id in words[9]. We only
            add those when they occur 10 or more times."""
-    new_features = []
+    count = 0
     repeat_hash = dict()
     with open(result_files[0]) as repeatmasker_handle:
         for line in repeatmasker_handle:
             words = line.split()
             if len(words) < 11 or words[0] in ('SW', 'score'):
                 continue
             try:
                 contig = contig_dict[words[4]]
             except KeyError:
                 context.log(f'({genome_name}) Warning: Unknown contig id "{words[4]}"')
                 continue
             if 'Simple_repeat' == words[10]:
                 feature = words2feature(words, contig, genome_name)
-                new_features.append(feature)
-                feature['notes'] = f'repeat {words[9]}'
+                feature.notes = f'repeat {words[9]}'
+                sqlite.add_new_feature_to_db(db_connection, feature)
+                count += 1
             else:
                 repeat_list = repeat_hash.setdefault(words[9], list())
                 repeat_list.append(words2feature(words, contig, genome_name))
     for repeat_list in repeat_hash.values():
         if len(repeat_list) >= 10:
             for feature in repeat_list:
-                new_features.append(feature)
-                feature['notes'] = f' (occurs {len(repeat_list)}x)'
-    feature_data = pd.concat([feature_data, pd.DataFrame(new_features)], ignore_index=True)
-    return feature_data, len(new_features)
+                feature.notes = f' (occurs {len(repeat_list)}x)'
+                sqlite.add_new_feature_to_db(db_connection, feature)
+                count += 1
+    return count
 
 
 @context.register_annotator
 def run_and_read_repeatmasker():
     return ({'pipeline_position': 51,
              'annotator_key': 'repeat_masker',
              'purpose': 'repeat prediction with repeatmasker',
```

### Comparing `metaerg-2.3.8/src/metaerg/run_and_read/signalp.py` & `metaerg-2.3.9/src/metaerg/run_and_read/signalp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import shutil
-import pandas as pd
 from pathlib import Path
 from concurrent.futures import ProcessPoolExecutor
 
 from metaerg import context
 from metaerg.datatypes import fasta
+from metaerg.datatypes import sqlite
 
 
-def _run_programs(genome_name, contig_dict, feature_data: pd.DataFrame, result_files):
+def _run_programs(genome_name, contig_dict, db_connection, result_files):
     cds_aa_file = context.spawn_file('cds.faa', genome_name)
     if context.CPUS_PER_GENOME > 1:
-        split_fasta_files = fasta.write_features_to_fasta(feature_data, 'aa', cds_aa_file, context.CPUS_PER_GENOME,
+        split_fasta_files = fasta.write_features_to_fasta(db_connection, 'aa', cds_aa_file, context.CPUS_PER_GENOME,
                                                           targets=('CDS',))
         split_signalp_files = [result_files[0].parent / f'{result_files[0].name}.{i}'
                                for i in range(len(split_fasta_files))]
         with ProcessPoolExecutor(max_workers=context.CPUS_PER_GENOME) as executor:
             for split_input, split_output in zip(split_fasta_files, split_signalp_files):
                 executor.submit(context.run_external, f'signalp6 --fastafile {split_input} --output_dir '
                                                     f'{split_output} --format none --organism other')
@@ -31,32 +31,34 @@
                 if split_signalp_dir.exists():
                     shutil.rmtree(split_signalp_dir)
                 split_cds_aa_file.unlink(missing_ok=True)
     else:
         context.run_external(f'signalp6 --fastafile {cds_aa_file} --output_dir {result_files[0]} --format none --organism other')
 
 
-def _read_results(genome_name, contig_dict, feature_data: pd.DataFrame, result_files) -> tuple:
+def _read_results(genome_name, contig_dict, db_connection, result_files) -> int:
     count = 0
     signalp_result_file = result_files[0] / 'prediction_results.txt'
     if signalp_result_file.exists():
         with open(signalp_result_file) as signalp_handle:
             for line in signalp_handle:
                 if line.startswith("#"):
                     continue
                 words = line.split("\t")
                 if "OTHER" == words[1]:
                     continue
                 feature_id = words[0].split()[0]
-                if feature_id not in feature_data.index:
+                feature = sqlite.read_feature_by_id(db_connection, feature_id)
+                if not feature:
                     raise Exception(f'Found results for unknown feature {feature_id}, '
                                     f'may need to rerun metaerg with --force')
-                feature_data.at[feature_id, 'signal_peptide'] = words[1]
+                feature.signal_peptide = words[1]
+                sqlite.update_feature_in_db(db_connection, feature)
                 count += 1
-    return feature_data, count
+    return count
 
 
 @context.register_annotator
 def run_and_read_signalp():
     return ({'pipeline_position': 121,
              'annotator_key': 'signalp',
              'purpose': 'signal peptide prediction with signalp',
```

### Comparing `metaerg-2.3.8/src/metaerg.egg-info/PKG-INFO` & `metaerg-2.3.9/src/metaerg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaerg
-Version: 2.3.8
+Version: 2.3.9
 Summary: Annotation of genomes and contigs
 Home-page: https://github.com/kinestetika/MetaErg
 Author: Marc Strous
 Author-email: mstrous@ucalgary.ca
 License: MIT
 Project-URL: Source, https://github.com/kinestetika/MetaErg
 Keywords: repeat-regions genes functions taxonomy
@@ -28,15 +28,15 @@
 classifications.
 
 You can interact with a sample visualization [here](https://htmlpreview.github.io/?https://github.com/kinestetika/MetaErg/blob/master/visualization/index.html) and [here](https://htmlpreview.github.io/?https://raw.githubusercontent.com/kinestetika/MetaErg/master/visualization/index_of_features.html). These visualizations show the annotation of a cyanobacterial genome, Candidatus Phormidium alkaliphilum.
 Unfortunately the interacive search box does not work with the github html visualization, so you need to download the html \
 files to your computer (i.e. using "git clone ..."), to try out the interactive part.
 
 Metaerg was originally developed in perl. It was relatively challenging to install and comes with complex database 
-dependencies. This new python version 2.2 overcomes some of those issues. Also, the annotation pipeline has further 
+dependencies. This new python version 2.3 overcomes some of those issues. Also, the annotation pipeline has further 
 evolved and has become more refined.
 
 By using gtdbtk for taxonomic classification of genes and transferring functional annotations from the NCBI, metaerg.py
 uses a controlled vocabulary for taxonomy and a relatively clean vocabulary for functions. This makes annotations much
 more concise than the original version of metaerg and many other annotation tools. In addition, metaerg uses NCBI's
 conserved domain database and RPSBlast to assign genes to subsystems for effective data exploration. Subsystems are a 
 work in progress, and can be expanded and customized as needed.
@@ -52,15 +52,15 @@
 * annotates taxonomy and functions of RNA and protein genes using [Diamond](https://github.com/bbuchfink/diamond), [NCBI blastn](https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/LATEST/) and a database of 62,296 bacterial, 3,406 archaeal 11,569 viral and 139 eukaryotic genomes.
 * annotates gene functions using [RPSBlast](https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/LATEST/) and NCBI's Conserved Domain Database (CDD).
 * annotates genes involved in production of secondary metabolites using [Antismash](https://dl.secondarymetabolites.org/releases).
 * annotates membrane amd translocated proteins using [TMHMM and SignalP](https://services.healthtech.dtu.dk/software.php).
 * assigns genes to a built-in set of functions using [HMMER](http://hmmer.org) and commmunity contributed HMM profiles (see below).
 * estimates doubling times of a genome's host based on [codon usage bias](https://www.pnas.org/doi/epdf/10.1073/pnas.2016810118)
 * presents annotations in [datatables/jQuery](https://www.datatables.net/)-based intuititve, searchable, colorful HTML that can be explored in a web browser and copy/pasted into excel.
-* saves annotations as a fasta-amino-acid file, a genbank file and in [Apache Feather format](https://arrow.apache.org/docs/python/feather.html) for effective exploration, statistics and visualization with python or R.
+* saves annotations as a fasta-amino-acid file, a genbank file, as a sqlite database and in [Apache Feather format](https://arrow.apache.org/docs/python/feather.html) for effective exploration, statistics and visualization with python or R.
 * saves an overview of all annotated genomes' properties and functions as an excel file. 
 * enables the user to add custom HMMs and expand the set of functional genes as needed.
 
 When using metaerg, please cite [Xiaoli Dong and Marc Strous (2019) Frontiers in Genetics](https://www.frontiersin.org/articles/10.3389/fgene.2019.00999/full)
 
 ## Usage:
 ```
@@ -128,17 +128,17 @@
 * E - build eukaryotes
 * B - build PVE blast databases
 * R - build RFAM
 * C - build CDD
 * S - build/update community contributed HMM databases
 * A - build antismash database
 
-## Using the .feather output
-[Apache Feather format](https://arrow.apache.org/docs/python/feather.html) is a binary file format for tables. You can for example load these data as a pandas dataframe. In **R**, use the [arrow](https://arrow.apache.org/docs/r/) package. 
-Each table row contains a single gene or feature, defines by the following columns:
+## Accessing the .feather and .mysql files
+[Apache Feather format](https://arrow.apache.org/docs/python/feather.html) is a binary file format for tables. Sqlite is a database format. You can for example load these data as a pandas dataframe. In **R**, use the [arrow](https://arrow.apache.org/docs/r/) package. 
+Each table/database row contains a single gene or feature, defined by the following columns:
 
 ```
 id                  the feature's unique identifier
 genome              the identifier of the genome the feature belongs to
 contig              the identifier of the contig the feature belongs to
 start               the start position of the feature (inclusive)
 end                 the start position of the feature (exclusive)
@@ -155,47 +155,41 @@
 tmh                 the number of transmembrane helixes found
 tmh_topology        how the protein is oriented in the membrane, if tmh were found 
 blast               the top ten blast hits
 cdd                 the top ten cdd hits
 hmm                 the top ten hits to the functional gene hmm database 
 ```
 
-You can for example use python and pandas to inspect the distribution of subsystems, such as denitrification, hydrogen oxidation or the Calvin Cycle across a large set of MAGs, as follows:
+You can for example use python and pandas to inspect annotations:
 
-```commandline
+``` python
 from pathlib import Path
 import pandas as pd
 
-from metaerg import functional_gene_configuration
-from metaerg.main import load_contigs, compute_genome_properties
+data_dir = Path('/path/to/my/data')
+feather_file = data_dir / 'my-genome.annotations.feather'
+contig_file =  data_dir / 'my-genome.fna'
+
+contig_dict = load_contigs('my-genome', contig_file, delimiter='xxxx')
+feature_data = pd.read_feather(feather_file)
+feature_data.set_index('id', inplace=True)
 
-functional_gene_configuration.init_functional_gene_config()
+for f in feature_data.itertuples():
+    for k, v in f._asdict().items():
+        print(f'{k:20}:{v}')
+    break  # comment out to iterate through all the genes...
+```
+
+Using the .mysql database is even easier:
+
+``` python
+from pathlib import Path
+from metaerg.datatypes import sqlite
 
 data_dir = Path('/path/to/my/data')
-feather_dir = data_dir / 'all_genes.feather'
-contig_dir =  data_dir / 'contig_fna_files_one_per_genome'
+sqlite_file = data_dir / 'my-genome.annotations.sqlite'
 
-genome_properties = {}
-for f in sorted(feather_dir.glob('*')):
-    genome_name = f.name
-    contig_dict = load_contigs(genome_name, contig_dir / genome_name, delimiter='xxxx')
-    feature_data = pd.read_feather(f)
-    genome_properties[genome_name] = compute_genome_properties(contig_dict, feature_data)
-    
-all_genome_feature_data = None
-for k, v in genome_properties.items():
-    subsystems_df = v['subsystems'].rename(columns={'genes': k})
-    try:
-        subsystems_df.drop('', level=0, axis=0, inplace=True)
-        subsystems_df.drop('secondary-metabolites', level=0, axis=0, inplace=True)
-    except Exception:
-        pass
-    if all_genome_feature_data is None:
-        all_genome_feature_data = subsystems_df
-    else:
-        all_genome_feature_data[k] = subsystems_df[k]
-    all_genome_feature_data = all_genome_feature_data.copy()
-del all_genome_feature_data['profiles']
-#print(all_genome_feature_data.columns)
-    
-all_genome_feature_data.to_excel(data_dir / 'functional_gene_heatmap.xls')
+db_connection = sqlite.connect_to_db(sqlite_file)
+for feature in sqlite.read_all_features(db_connection): 
+    print(feature)
+    break  # comment out to iterate through all the genes...
 ```
```

### Comparing `metaerg-2.3.8/src/metaerg.egg-info/SOURCES.txt` & `metaerg-2.3.9/src/metaerg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 src/metaerg/calculations/codon_usage_bias.py
 src/metaerg/datatypes/__init__.py
 src/metaerg/datatypes/blast.py
 src/metaerg/datatypes/fasta.py
 src/metaerg/datatypes/gbk.py
 src/metaerg/datatypes/gff.py
 src/metaerg/datatypes/ncbi_ftp.py
+src/metaerg/datatypes/sqlite.py
 src/metaerg/html/__init__.py
 src/metaerg/html/html_all_genomes.py
 src/metaerg/html/html_feature_details.py
 src/metaerg/html/html_feature_table.py
 src/metaerg/html/html_genome_properties_and_subsystems.py
 src/metaerg/run_and_read/__init__.py
 src/metaerg/run_and_read/antismash.py
```

