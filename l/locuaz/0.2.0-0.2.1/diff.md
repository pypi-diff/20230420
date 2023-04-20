# Comparing `tmp/locuaz-0.2.0.tar.gz` & `tmp/locuaz-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locuaz-0.2.0.tar", last modified: Thu Apr 13 12:00:26 2023, max compression
+gzip compressed data, was "locuaz-0.2.1.tar", last modified: Thu Apr 20 13:30:57 2023, max compression
```

## Comparing `locuaz-0.2.0.tar` & `locuaz-0.2.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-13 12:00:26.208319 locuaz-0.2.0/
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-11 13:53:32.000000 locuaz-0.2.0/CHANGELOG.rst
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1069 2023-04-11 13:54:09.000000 locuaz-0.2.0/LICENSE.rst
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     8482 2023-04-13 12:00:26.208319 locuaz-0.2.0/PKG-INFO
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7121 2023-04-13 12:00:16.000000 locuaz-0.2.0/README.rst
-drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-13 12:00:26.204319 locuaz-0.2.0/locuaz/
-drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-13 12:00:26.208319 locuaz-0.2.0/locuaz/DLPacker/
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    26853 2023-03-28 09:11:07.000000 locuaz-0.2.0/locuaz/DLPacker/dlpacker.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    19402 2023-03-24 13:12:43.000000 locuaz-0.2.0/locuaz/DLPacker/utils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)       22 2023-04-07 11:50:26.000000 locuaz-0.2.0/locuaz/__init__.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      834 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/abstractmutationgenerator.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1793 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/abstractscoringfunction.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    13030 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/amberutils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4445 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/autodockvina.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3671 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/bach.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     6699 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/basemutator.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3089 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/basestatistic.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5788 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/bluues.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7149 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/bluuesbmf.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    18838 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/cli.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7908 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/complex.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5235 2023-04-12 12:37:10.000000 locuaz-0.2.0/locuaz/epochinitializer.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3051 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/evoef2.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5733 2023-03-06 14:28:36.000000 locuaz-0.2.0/locuaz/fileutils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     6862 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/fixbox.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4289 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/gmxmmpbsa.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    15101 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/gromacsutils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7679 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/haddock.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5427 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/interface.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    12458 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/molecules.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     6138 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/moleculesutils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1620 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/molutils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1541 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/mutation.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      323 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/mutationgenerators.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1256 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/mutatorbiobb.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3881 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/mutatordlp.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4694 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/mutatordlpr.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3681 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/mutatorevoef2.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      598 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/mutators.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4178 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/piepisa.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3048 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/pisa.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     2494 2023-04-04 10:50:21.000000 locuaz-0.2.0/locuaz/primitives.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    31226 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/projectutils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     2335 2023-04-12 12:44:46.000000 locuaz-0.2.0/locuaz/protocol.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3936 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/pruner.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1937 2023-04-12 11:04:33.000000 locuaz-0.2.0/locuaz/pruners.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3871 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/rosetta.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4641 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/run.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     8885 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/runutils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5774 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/scoring.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      681 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/scoringfunctions.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     6688 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/spm4.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4421 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/spm4i.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7877 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/spm4mmpbsa.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1363 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/statisticcmdistance.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     2053 2023-04-12 10:58:14.000000 locuaz-0.2.0/locuaz/statisticinterface.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      956 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/stats.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4805 2023-04-12 10:58:15.000000 locuaz-0.2.0/locuaz/utils_scoring.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    10044 2023-04-07 12:45:26.000000 locuaz-0.2.0/locuaz/validatore.py
-drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-13 12:00:26.208319 locuaz-0.2.0/locuaz.egg-info/
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     8482 2023-04-13 12:00:26.000000 locuaz-0.2.0/locuaz.egg-info/PKG-INFO
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1362 2023-04-13 12:00:26.000000 locuaz-0.2.0/locuaz.egg-info/SOURCES.txt
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)        1 2023-04-13 12:00:26.000000 locuaz-0.2.0/locuaz.egg-info/dependency_links.txt
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)       57 2023-04-13 12:00:26.000000 locuaz-0.2.0/locuaz.egg-info/entry_points.txt
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      187 2023-04-13 12:00:26.000000 locuaz-0.2.0/locuaz.egg-info/requires.txt
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)        7 2023-04-13 12:00:26.000000 locuaz-0.2.0/locuaz.egg-info/top_level.txt
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)       95 2023-04-12 11:27:33.000000 locuaz-0.2.0/pyproject.toml
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      835 2023-04-13 12:00:26.208319 locuaz-0.2.0/setup.cfg
-drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-13 12:00:26.208319 locuaz-0.2.0/tests/
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      536 2023-02-21 12:12:48.000000 locuaz-0.2.0/tests/test_locuaz.py
+drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-20 13:30:57.951101 locuaz-0.2.1/
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-11 13:53:32.000000 locuaz-0.2.1/CHANGELOG.rst
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1069 2023-04-11 13:54:09.000000 locuaz-0.2.1/LICENSE.rst
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     8856 2023-04-20 13:30:57.951101 locuaz-0.2.1/PKG-INFO
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7475 2023-04-20 13:30:34.000000 locuaz-0.2.1/README.rst
+drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-20 13:30:57.951101 locuaz-0.2.1/locuaz/
+drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-20 13:30:57.951101 locuaz-0.2.1/locuaz/DLPacker/
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    26845 2023-04-19 14:49:18.000000 locuaz-0.2.1/locuaz/DLPacker/dlpacker.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    19402 2023-03-24 13:12:43.000000 locuaz-0.2.1/locuaz/DLPacker/utils.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)       22 2023-04-07 11:50:26.000000 locuaz-0.2.1/locuaz/__init__.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      849 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/abstractmutationgenerator.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1807 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/abstractscoringfunction.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    13051 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/amberutils.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4466 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/autodockvina.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3692 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/bach.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     6734 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/basemutator.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3096 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/basestatistic.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5809 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/bluues.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7170 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/bluuesbmf.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    18852 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/cli.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7929 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/complex.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5298 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/epochinitializer.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3072 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/evoef2.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5733 2023-04-19 13:31:58.000000 locuaz-0.2.1/locuaz/fileutils.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     6890 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/fixbox.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4317 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/gmxmmpbsa.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    15143 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/gromacsutils.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7700 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/haddock.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5441 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/interface.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    12472 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/molecules.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     6159 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/moleculesutils.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1641 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/molutils.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1548 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/mutation.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      351 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/mutationgenerators.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1284 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/mutatorbiobb.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3916 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/mutatordlp.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4722 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/mutatordlpr.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3709 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/mutatorevoef2.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      634 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/mutators.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4199 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/piepisa.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3069 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/pisa.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     2668 2023-04-20 10:23:58.000000 locuaz-0.2.1/locuaz/primitives.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    31268 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/projectutils.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     2383 2023-04-19 14:37:41.000000 locuaz-0.2.1/locuaz/protocol.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3943 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/pruner.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1951 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/pruners.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3892 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/rosetta.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4656 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/run.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     8927 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/runutils.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5816 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/scoring.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      758 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/scoringfunctions.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7125 2023-04-20 11:10:24.000000 locuaz-0.2.1/locuaz/spm4.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4608 2023-04-20 11:35:59.000000 locuaz-0.2.1/locuaz/spm4i.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     8177 2023-04-20 11:35:01.000000 locuaz-0.2.1/locuaz/spm4mmpbsa.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1384 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/statisticcmdistance.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     2074 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/statisticinterface.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      984 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/stats.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4820 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/utils_scoring.py
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    10044 2023-04-19 13:23:22.000000 locuaz-0.2.1/locuaz/validatore.py
+drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-20 13:30:57.951101 locuaz-0.2.1/locuaz.egg-info/
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     8856 2023-04-20 13:30:57.000000 locuaz-0.2.1/locuaz.egg-info/PKG-INFO
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1362 2023-04-20 13:30:57.000000 locuaz-0.2.1/locuaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)        1 2023-04-20 13:30:57.000000 locuaz-0.2.1/locuaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)       57 2023-04-20 13:30:57.000000 locuaz-0.2.1/locuaz.egg-info/entry_points.txt
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      208 2023-04-20 13:30:57.000000 locuaz-0.2.1/locuaz.egg-info/requires.txt
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)        7 2023-04-20 13:30:57.000000 locuaz-0.2.1/locuaz.egg-info/top_level.txt
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)       95 2023-04-12 11:27:33.000000 locuaz-0.2.1/pyproject.toml
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      866 2023-04-20 13:30:57.951101 locuaz-0.2.1/setup.cfg
+drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-20 13:30:57.951101 locuaz-0.2.1/tests/
+-rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      536 2023-02-21 12:12:48.000000 locuaz-0.2.1/tests/test_locuaz.py
```

### Comparing `locuaz-0.2.0/LICENSE.rst` & `locuaz-0.2.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.0/PKG-INFO` & `locuaz-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 Metadata-Version: 2.1
 Name: locuaz
-Version: 0.2.0
+Version: 0.2.1
 Summary: Antibody optimization protocol
 Author: Patricio Barletta
 Author-email: pbarletta@gmail.com
 Keywords: molecular,dynamics,antibody,antibodies
-Requires-Python: ==3.10.10
+Requires-Python: >=3.9.15
 Description-Content-Type: text/x-rst
+Provides-Extra: docs
 License-File: LICENSE.rst
 
 ========
 locuaz
 ========
 
 
 .. image:: https://img.shields.io/pypi/v/locuaz.svg
         :target: https://pypi.python.org/pypi/locuaz
 
-.. image:: https://img.shields.io/travis/pgbarletta/locuaz.svg
-        :target: https://app.travis-ci.com/github/pgbarletta/locuaz/builds
-
 .. image:: https://readthedocs.org/projects/locuaz/badge/?version=latest
         :target: https://locuaz.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 Looping Uniquely Catered Amino Acid Sequences
 
 
 * Free software: MIT license
 * Documentation: https://locuaz.readthedocs.io.
 
 Install
 --------
 
+Check the `Installation <https://locuaz.readthedocs.io/en/latest/installation.html>`_ section on the docs..
+
 Mambaforge is recommended instead of pure conda. Download Mambaforge from:
 
 https://github.com/conda-forge/miniforge
 
-Clone this repo and, optionally, get the **DLPacker**  submodule as well::
-
-    git clone https://github.com/pgbarletta/locuaz
-    git submodule int
-    git submodule update
 
-You'll also have to get DLPacker's `weights <https://drive.google.com/file/d/1J4fV9aAr2nssrWN8mQ7Ui-9PVQseE0LQ/view?usp=sharing>`_.
+Why there's no straight pip or conda install
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Being this a high-level protocol, there are many dependencies to it and, unfortunately, python packaging has its quirks so
+different developers have solved their issues in different ways.
+A straight `pip install` is out of the question given the tensorflow (for DLPacker) and ambertools (for tleap) dependencies.
+On the other hand, not all packages have a conda recipe (freesasa), and while the biobb packages do show up on the bioconda
+channel, when installed in this manner, they bring over many unwanted, heavy dependencies, like GROMACS itself.
+So, in summary, a mix of pip and conda is needed.
 
 Post-Install
 -------------
 If on MDAnalysis 2.4.3 or older, edit the file ``MDAnalysis/topology/tpr/utils.py`` line 330::
     
   segid = f"seg_{i}_{molblock}"
```

### Comparing `locuaz-0.2.0/README.rst` & `locuaz-0.2.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,42 +2,43 @@
 locuaz
 ========
 
 
 .. image:: https://img.shields.io/pypi/v/locuaz.svg
         :target: https://pypi.python.org/pypi/locuaz
 
-.. image:: https://img.shields.io/travis/pgbarletta/locuaz.svg
-        :target: https://app.travis-ci.com/github/pgbarletta/locuaz/builds
-
 .. image:: https://readthedocs.org/projects/locuaz/badge/?version=latest
         :target: https://locuaz.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 Looping Uniquely Catered Amino Acid Sequences
 
 
 * Free software: MIT license
 * Documentation: https://locuaz.readthedocs.io.
 
 Install
 --------
 
+Check the `Installation <https://locuaz.readthedocs.io/en/latest/installation.html>`_ section on the docs..
+
 Mambaforge is recommended instead of pure conda. Download Mambaforge from:
 
 https://github.com/conda-forge/miniforge
 
-Clone this repo and, optionally, get the **DLPacker**  submodule as well::
-
-    git clone https://github.com/pgbarletta/locuaz
-    git submodule int
-    git submodule update
 
-You'll also have to get DLPacker's `weights <https://drive.google.com/file/d/1J4fV9aAr2nssrWN8mQ7Ui-9PVQseE0LQ/view?usp=sharing>`_.
+Why there's no straight pip or conda install
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Being this a high-level protocol, there are many dependencies to it and, unfortunately, python packaging has its quirks so
+different developers have solved their issues in different ways.
+A straight `pip install` is out of the question given the tensorflow (for DLPacker) and ambertools (for tleap) dependencies.
+On the other hand, not all packages have a conda recipe (freesasa), and while the biobb packages do show up on the bioconda
+channel, when installed in this manner, they bring over many unwanted, heavy dependencies, like GROMACS itself.
+So, in summary, a mix of pip and conda is needed.
 
 Post-Install
 -------------
 If on MDAnalysis 2.4.3 or older, edit the file ``MDAnalysis/topology/tpr/utils.py`` line 330::
     
   segid = f"seg_{i}_{molblock}"
```

### Comparing `locuaz-0.2.0/locuaz/DLPacker/dlpacker.py` & `locuaz-0.2.1/locuaz/DLPacker/dlpacker.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 # ==============================================================================
 from pathlib import Path
 from io import StringIO
 
 import numpy as np
 from Bio.PDB import PDBParser, Selection, Superimposer, PDBIO, Atom, Residue, Structure
 
-from DLPacker.utils import DLPModel, InputBoxReader, DataGenerator, THE20, SCH_ATOMS, BB_ATOMS, SIDE_CHAINS, BOX_SIZE
+from .utils import DLPModel, InputBoxReader, DataGenerator, THE20, SCH_ATOMS, BB_ATOMS, SIDE_CHAINS, BOX_SIZE
 
 class DLPacker():
     # This is the meat of our code.
     # This class reads in PDB files using biopython
     # and implements various operations on them
     # using DLPModel's predictions.
     # You might need to change this class if you
```

### Comparing `locuaz-0.2.0/locuaz/DLPacker/utils.py` & `locuaz-0.2.1/locuaz/DLPacker/utils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.0/locuaz/abstractmutationgenerator.py` & `locuaz-0.2.1/locuaz/abstractmutationgenerator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import Set, Iterator
 from collections.abc import Mapping
 from logging import Logger
 
-from projectutils import Iteration, Epoch
-from mutation import Mutation
+from locuaz.projectutils import Iteration, Epoch
+from locuaz.mutation import Mutation
 
 
 class AbstractMutationGenerator(ABC, Mapping):
     @abstractmethod
     def __init__(
             self,
             epoch: Epoch,
@@ -28,8 +28,8 @@
 
     @abstractmethod
     def __iter__(self) -> Iterator:
         pass
 
     @abstractmethod
     def __contains__(self, value: Iteration) -> bool:
-        pass
+        pass
```

### Comparing `locuaz-0.2.0/locuaz/abstractscoringfunction.py` & `locuaz-0.2.1/locuaz/abstractscoringfunction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
 from typing import Any, Union, List
 
-from complex import GROComplex
-from fileutils import FileHandle, DirHandle
+from locuaz.complex import GROComplex
+from locuaz.fileutils import FileHandle, DirHandle
 
 
 class AbstractScoringFunction(metaclass=ABCMeta):
     name: str
     root_dir: DirHandle
     results_dir: DirHandle
     bin_path: Union[FileHandle, str]
```

### Comparing `locuaz-0.2.0/locuaz/amberutils.py` & `locuaz-0.2.1/locuaz/amberutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from typing import Tuple, Union, Optional, List, Generator, Deque, Set, TextIO
 from zipfile import ZipFile
 
 import MDAnalysis as mda
 import parmed as pmd
 from pdb4amber import AmberPDBFixer
 
-from fileutils import FileHandle, DirHandle
-from molecules import PDBStructure, GROStructure, ZipTopology
-from primitives import ext
+from locuaz.fileutils import FileHandle, DirHandle
+from locuaz.molecules import PDBStructure, GROStructure, ZipTopology
+from locuaz.primitives import ext
 
 warnings.filterwarnings("ignore")
 
 
 def chunk(f: TextIO) -> Generator:
     linea = " "
     while linea != "":
```

### Comparing `locuaz-0.2.0/locuaz/autodockvina.py` & `locuaz-0.2.1/locuaz/autodockvina.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import concurrent.futures as cf
 import subprocess as sp
 from pathlib import Path
 from typing import List, Tuple, Union
 import re
 
-from abstractscoringfunction import AbstractScoringFunction
-from complex import GROComplex
-from fileutils import DirHandle, FileHandle
+from locuaz.abstractscoringfunction import AbstractScoringFunction
+from locuaz.complex import GROComplex
+from locuaz.fileutils import DirHandle, FileHandle
 
 
 class AutodockVina(AbstractScoringFunction):
     CPU_TO_MEM_RATIO: int = 1000
     TIMEOUT_PER_FRAME: int = 1
 
     def __init__(self, sf_dir, *, nthreads=2, mpiprocs=2) -> None:
```

### Comparing `locuaz-0.2.0/locuaz/bach.py` & `locuaz-0.2.1/locuaz/bach.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import concurrent.futures as cf
 import subprocess as sp
 from pathlib import Path
 from typing import Tuple, List
 
-from abstractscoringfunction import AbstractScoringFunction
-from complex import GROComplex
-from fileutils import FileHandle, DirHandle
+from locuaz.abstractscoringfunction import AbstractScoringFunction
+from locuaz.complex import GROComplex
+from locuaz.fileutils import FileHandle, DirHandle
 
 
 class Bach(AbstractScoringFunction):
     parameters_handle: FileHandle
     atomic_parameters_handle: FileHandle
     TIMEOUT_PER_FRAME: int = 2
```

### Comparing `locuaz-0.2.0/locuaz/basemutator.py` & `locuaz-0.2.1/locuaz/basemutator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from typing import List, Iterable, Tuple, Optional, Union, Set
 import warnings
 
 import MDAnalysis as mda
 from Bio.PDB import PDBParser
 from Bio.PDB.PDBIO import PDBIO
 
-from fileutils import FileHandle
-from projectutils import WorkProject, Epoch
-from molecules import PDBStructure
-from mutation import Mutation
-from primitives import AA_MAP
+from locuaz.fileutils import FileHandle
+from locuaz.projectutils import WorkProject, Epoch
+from locuaz.molecules import PDBStructure
+from locuaz.mutation import Mutation
+from locuaz.primitives import AA_MAP
 
 
 class BaseMutator:
     """BaseMutator offers 4 static methods to help development of new mutators: split_solute_solvent(), fix_pdb(),
     port_mutation() and add_water().
     Args:
         bin_dir (Path): path to the binary file.
```

### Comparing `locuaz-0.2.0/locuaz/basestatistic.py` & `locuaz-0.2.1/locuaz/basestatistic.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from typing import Dict, Tuple, Callable
 from abc import abstractmethod
 
 import numpy as np
 from numpy.typing import NDArray
 
-from projectutils import Iteration
+from locuaz.projectutils import Iteration
 
 
 class BaseStatistic:
     frames_path: Path
     trj_suffix: str
     name: str
     result: NDArray[float]
```

### Comparing `locuaz-0.2.0/locuaz/bluues.py` & `locuaz-0.2.1/locuaz/bluues.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import concurrent.futures as cf
 import subprocess as sp
 from pathlib import Path
 from typing import Tuple, List, Union
 
-from abstractscoringfunction import AbstractScoringFunction
-from complex import GROComplex
-from fileutils import FileHandle, DirHandle
+from locuaz.abstractscoringfunction import AbstractScoringFunction
+from locuaz.complex import GROComplex
+from locuaz.fileutils import FileHandle, DirHandle
 
 
 class Bluues(AbstractScoringFunction):
     bmf_bin_path: FileHandle
     pdb2pqr_bin_path: str = "pdb2pqr30"
     TIMEOUT_PER_FRAME: int = 60
```

### Comparing `locuaz-0.2.0/locuaz/bluuesbmf.py` & `locuaz-0.2.1/locuaz/bluuesbmf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import concurrent.futures as cf
 import subprocess as sp
 from operator import itemgetter
 from pathlib import Path
 from typing import Tuple, List, Any
 
-from abstractscoringfunction import AbstractScoringFunction
-from complex import GROComplex
-from fileutils import FileHandle, DirHandle
+from locuaz.abstractscoringfunction import AbstractScoringFunction
+from locuaz.complex import GROComplex
+from locuaz.fileutils import FileHandle, DirHandle
 
 
 class BluuesBmf(AbstractScoringFunction):
     bmf_bin_path: FileHandle
     pdb2pqr_bin_path: str = "pdb2pqr30"
     TIMEOUT_PER_FRAME: int = 60
```

### Comparing `locuaz-0.2.0/locuaz/cli.py` & `locuaz-0.2.1/locuaz/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from itertools import product
 from pathlib import Path
 from queue import PriorityQueue
 from typing import Dict, List, Final, Set, Tuple, Union, Any
 
 import yaml
 
-from validatore import Validatore
-from primitives import UserInputError
+from locuaz.validatore import Validatore
+from locuaz.primitives import UserInputError
 
 
 def get_dir_size(folder: Path) -> float:
     B_TO_MB: Final = 1048576
     total_size = 0
     for path, _, files in os.walk(folder):
         for f in files:
```

### Comparing `locuaz-0.2.0/locuaz/complex.py` & `locuaz-0.2.1/locuaz/complex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from abc import ABCMeta, abstractmethod
 from collections.abc import Iterable
 from pathlib import Path
 from typing import Dict, Optional, Union
 
 from attrs import define, field
 
-from fileutils import DirHandle, FileHandle, copy_to
-from molecules import (
+from locuaz.fileutils import DirHandle, FileHandle, copy_to
+from locuaz.molecules import (
     PDBStructure,
     GROStructure,
     Topology,
     ZipTopology,
     TPRFile,
     Trajectory,
     XtcTrajectory,
     TrrTrajectory,
     generate_ndx,
     get_tpr,
     get_pdb_tpr,
     copy_mol_to,
     try_copy_to,
 )
-from moleculesutils import get_gro_ziptop_from_pdb, get_gro_ziptop_from_pdb_tleap
+from locuaz.moleculesutils import get_gro_ziptop_from_pdb, get_gro_ziptop_from_pdb_tleap
 
 
 @define(frozen=True)
 class AbstractComplex(metaclass=ABCMeta):
     name: str = field(converter=str)
     dir: Union[DirHandle, Path] = field(converter=DirHandle, kw_only=True)  # type: ignore
     pdb: PDBStructure = field(kw_only=True)
```

### Comparing `locuaz-0.2.0/locuaz/epochinitializer.py` & `locuaz-0.2.1/locuaz/epochinitializer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import shutil as sh
 import sys
 import warnings
 from logging import Logger
 from pathlib import Path
 
-from amberutils import fix_pdb
-from complex import GROComplex
-from fileutils import DirHandle
-from gromacsutils import remove_overlapping_solvent
-from molecules import PDBStructure
-from mutationgenerators import mutation_generators
-from basemutator import memorize_mutations
-from mutators import mutators
-from projectutils import WorkProject, Epoch, Iteration
+from locuaz.amberutils import fix_pdb
+from locuaz.complex import GROComplex
+from locuaz.fileutils import DirHandle
+from locuaz.gromacsutils import remove_overlapping_solvent
+from locuaz.molecules import PDBStructure
+from locuaz.mutationgenerators import mutation_generators
+from locuaz.basemutator import memorize_mutations
+from locuaz.mutators import mutators
+from locuaz.projectutils import WorkProject, Epoch, Iteration
 
 
 def initialize_new_epoch(work_pjct: WorkProject, log: Logger) -> None:
     """initialize_new_epoch(): This is a specific protocol, others will be added
 
     Args:
         work_pjct (WorkProject):
```

### Comparing `locuaz-0.2.0/locuaz/evoef2.py` & `locuaz-0.2.1/locuaz/evoef2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import concurrent.futures as cf
 import subprocess as sp
 from pathlib import Path
 from typing import List, Tuple
 
-from abstractscoringfunction import AbstractScoringFunction
-from complex import GROComplex
-from fileutils import DirHandle
+from locuaz.abstractscoringfunction import AbstractScoringFunction
+from locuaz.complex import GROComplex
+from locuaz.fileutils import DirHandle
 
 
 class Evoef2(AbstractScoringFunction):
     CPU_TO_MEM_RATIO: int = 1000
     TIMEOUT_PER_FRAME: int = 1
 
     def __init__(self, sf_dir, *, nthreads=2, mpiprocs=2) -> None:
```

### Comparing `locuaz-0.2.0/locuaz/fileutils.py` & `locuaz-0.2.1/locuaz/fileutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.0/locuaz/fixbox.py` & `locuaz-0.2.1/locuaz/fixbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from pathlib import Path
 from typing import Tuple
 
 import MDAnalysis as mda
 import numpy as np
 from biobb_analysis.gromacs.gmx_image import GMXImage
 
-from complex import GROComplex
-from fileutils import FileHandle
-from molecules import PDBStructure, read_ndx
-from primitives import launch_biobb
+from locuaz.complex import GROComplex
+from locuaz.fileutils import FileHandle
+from locuaz.molecules import PDBStructure, read_ndx
+from locuaz.primitives import launch_biobb
 
 
 def fix_box(uni: mda.Universe, *, target_indices: Iterable, binder_indices: Iterable,
             non_protein_indices: Iterable) -> Tuple[bool, mda.Universe]:
     """
     fix_box() wraps the atoms of a system around its box and then centers them.
     From: Baptista, A. M.; da Rocha, L.; Campos, S. R. R. FixBox: A General
```

### Comparing `locuaz-0.2.0/locuaz/gmxmmpbsa.py` & `locuaz-0.2.1/locuaz/gmxmmpbsa.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import shutil as sh
 import subprocess as sp
 import zipfile
 from pathlib import Path
 from typing import List, Union
 from warnings import warn
 
-from abstractscoringfunction import AbstractScoringFunction
-from complex import GROComplex
-from fileutils import DirHandle, FileHandle
-from molecules import ZipTopology
+from locuaz.abstractscoringfunction import AbstractScoringFunction
+from locuaz.complex import GROComplex
+from locuaz.fileutils import DirHandle, FileHandle
+from locuaz.molecules import ZipTopology
 
 
 class GmxMmpbsa(AbstractScoringFunction):
     bin_name = "gmx_MMPBSA"
     TIMEOUT_PER_FRAME: int = 20
 
     def __init__(self, sf_dir, *, nthreads=2, mpiprocs=2) -> None:
```

### Comparing `locuaz-0.2.0/locuaz/gromacsutils.py` & `locuaz-0.2.1/locuaz/gromacsutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 from Bio.PDB.PDBIO import PDBIO
 from biobb_analysis.gromacs.gmx_image import GMXImage
 from biobb_analysis.gromacs.gmx_trjconv_str import GMXTrjConvStr
 from biobb_gromacs.gromacs.genion import Genion
 from biobb_gromacs.gromacs.gmxselect import Gmxselect
 from biobb_gromacs.gromacs.solvate import Solvate
 
-from complex import AbstractComplex, GROComplex
-from fileutils import FileHandle, update_header, copy_to
-from molecules import (
+from locuaz.complex import AbstractComplex, GROComplex
+from locuaz.fileutils import FileHandle, update_header, copy_to
+from locuaz.molecules import (
     PDBStructure,
     XtcTrajectory,
     get_tpr,
 )
-from moleculesutils import get_gro_ziptop_from_pdb, fix_wat_naming
-from primitives import AA_MAP
-from primitives import launch_biobb
+from locuaz.moleculesutils import get_gro_ziptop_from_pdb, fix_wat_naming
+from locuaz.primitives import AA_MAP
+from locuaz.primitives import launch_biobb
 
 
 def image_traj(cpx: GROComplex, out_trj_fn: Path, use_tleap: bool = False, gmx_bin: str = "gmx") -> XtcTrajectory:
     wrk_dir = out_trj_fn.parent
 
     # I have to specify `fit_selection` and `center_selection` even though I'm not
     # fitting or centering anything or else biobb will throw an error.
```

### Comparing `locuaz-0.2.0/locuaz/haddock.py` & `locuaz-0.2.1/locuaz/haddock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import concurrent.futures as cf
 import os
 import re
 import subprocess as sp
 from pathlib import Path
 from typing import Tuple, List, Union
 
-from abstractscoringfunction import AbstractScoringFunction
-from complex import GROComplex
-from fileutils import FileHandle, DirHandle, copy_to
+from locuaz.abstractscoringfunction import AbstractScoringFunction
+from locuaz.complex import GROComplex
+from locuaz.fileutils import FileHandle, DirHandle, copy_to
 
 
 class Haddock(AbstractScoringFunction):
     template_scoring_inp_handle: FileHandle
     haddock_protocols_dir: DirHandle
     haddock_toppar_dir: DirHandle
     rescoring_scripts_dir: DirHandle
```

### Comparing `locuaz-0.2.0/locuaz/interface.py` & `locuaz-0.2.1/locuaz/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Union, List, Set, Optional, Tuple
 import py
 
 import freesasa
 import MDAnalysis as mda
 from Bio.SeqUtils import seq1
 
-from molecules import PDBStructure
-from fileutils import FileHandle
+from locuaz.molecules import PDBStructure
+from locuaz.fileutils import FileHandle
 
 
 def get_interfacing_residues(pdb_input: Union[PDBStructure, FileHandle, Path], chainIDs: List[str],
                              probe_radius: float = 1.4, use_tleap: bool = False) -> Set[int]:
     """
     get_interfacing_residues(): use freesasa to get the resSeq of the binder residues that are in contact with
     the target. These can be used to guide the 2choice of the next mutated position.
```

### Comparing `locuaz-0.2.0/locuaz/molecules.py` & `locuaz-0.2.1/locuaz/molecules.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import numpy as np
 from attrs import define, field
 from biobb_analysis.gromacs.gmx_trjconv_str import GMXTrjConvStr
 from biobb_gromacs.gromacs.gmxselect import Gmxselect
 from biobb_gromacs.gromacs.grompp import Grompp
 from biobb_gromacs.gromacs.pdb2gmx import Pdb2gmx
 
-from fileutils import FileHandle, DirHandle, copy_to, update_header
-from primitives import launch_biobb
+from locuaz.fileutils import FileHandle, DirHandle, copy_to, update_header
+from locuaz.primitives import launch_biobb
 
 
 @define
 class AbstractFileObject(metaclass=ABCMeta):
     file: FileHandle = field(converter=FileHandle)  # type: ignore
     name: str = field(init=False)
     ext: str = field(init=False)
```

### Comparing `locuaz-0.2.0/locuaz/moleculesutils.py` & `locuaz-0.2.1/locuaz/moleculesutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 import MDAnalysis as mda
 import numpy as np
 from biobb_analysis.gromacs.gmx_trjconv_str import GMXTrjConvStr
 from biobb_gromacs.gromacs.genion import Genion
 from biobb_gromacs.gromacs.pdb2gmx import Pdb2gmx
 
-from amberutils import create_tleap_script, fix_pdb, run_tleap, amb_to_gmx
-from molecules import PDBStructure, GROStructure, ZipTopology, get_tpr
-from primitives import launch_biobb
+from locuaz.amberutils import create_tleap_script, fix_pdb, run_tleap, amb_to_gmx
+from locuaz.molecules import PDBStructure, GROStructure, ZipTopology, get_tpr
+from locuaz.primitives import launch_biobb
 
 
 def get_gro_ziptop_from_pdb(
         *,
         pdb: PDBStructure,
         target_chains: Iterable,
         binder_chains: Iterable,
```

### Comparing `locuaz-0.2.0/locuaz/molutils.py` & `locuaz-0.2.1/locuaz/molutils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import Tuple
 
 from biobb_analysis.gromacs.gmx_trjconv_str import GMXTrjConvStr
 
-from complex import GROComplex
-from molecules import PDBStructure
-from primitives import launch_biobb
+from locuaz.complex import GROComplex
+from locuaz.molecules import PDBStructure
+from locuaz.primitives import launch_biobb
 
 
 def split_solute_and_solvent_old(
         cpx: GROComplex, gmx_bin: str
 ) -> Tuple[PDBStructure, PDBStructure]:
     """prepare_old_iter extract 2 PDBs from an input pdb, one with the protein
     and the other with the water and ions.
```

### Comparing `locuaz-0.2.0/locuaz/mutation.py` & `locuaz-0.2.1/locuaz/mutation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from attrs import define, field
 from typing import List, Tuple
 
-from projectutils import Iteration
+from locuaz.projectutils import Iteration
 
 
 @define(frozen=True)
 class Mutation:
     chainID: str = field(converter=str, kw_only=True)
     resSeq: int = field(converter=int, kw_only=True)
     old_aa: str = field(converter=str, kw_only=True)
```

### Comparing `locuaz-0.2.0/locuaz/mutatorbiobb.py` & `locuaz-0.2.1/locuaz/mutatorbiobb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 
 from Bio.SeqUtils import seq3
 from biobb_model.model.mutate import Mutate
 
-from molecules import PDBStructure
-from primitives import launch_biobb
-from basemutator import BaseMutator
-from mutation import Mutation
+from locuaz.molecules import PDBStructure
+from locuaz.primitives import launch_biobb
+from locuaz.basemutator import BaseMutator
+from locuaz.mutation import Mutation
 
 
 class MutatorBiobb(BaseMutator):
     def __init__(self, bin_dir: Path) -> None:
         pass
 
     def __biobb_string__(self, mut: Mutation) -> str:
```

### Comparing `locuaz-0.2.0/locuaz/mutatordlp.py` & `locuaz-0.2.1/locuaz/mutatordlp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from pathlib import Path
 from typing import Optional, Union
 
 import MDAnalysis as mda
 from MDAnalysis.analysis import align
 from Bio.SeqUtils import seq3
 
-from DLPacker.dlpacker import DLPacker
-from fileutils import FileHandle
-from molecules import PDBStructure
-from mutation import Mutation
-from basemutator import BaseMutator
+from locuaz.DLPacker.dlpacker import DLPacker
+from locuaz.fileutils import FileHandle
+from locuaz.molecules import PDBStructure
+from locuaz.mutation import Mutation
+from locuaz.basemutator import BaseMutator
 
 
 class MutatorDLPacker(BaseMutator):
     weights_path: FileHandle
     lib_path: FileHandle
     charges_path: FileHandle
```

### Comparing `locuaz-0.2.0/locuaz/mutatordlpr.py` & `locuaz-0.2.1/locuaz/mutatordlpr.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from pathlib import Path
 from typing import Optional, Union, Set, Tuple
 import numpy as np
 
 import MDAnalysis as mda
 from Bio.SeqUtils import seq3
 
-from DLPacker.dlpacker import DLPacker
-from molecules import PDBStructure
-from mutation import Mutation
-from mutatordlp import MutatorDLPacker
+from locuaz.DLPacker.dlpacker import DLPacker
+from locuaz.molecules import PDBStructure
+from locuaz.mutation import Mutation
+from locuaz.mutatordlp import MutatorDLPacker
 
 
 class MutatorDLPackerReconstruct(MutatorDLPacker):
     radius: float
 
     def __init__(self, bin_dir: Path, radius: float = 5) -> None:
         super().__init__(bin_dir, radius)
```

### Comparing `locuaz-0.2.0/locuaz/mutatorevoef2.py` & `locuaz-0.2.1/locuaz/mutatorevoef2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import shutil as sh
 import subprocess as sp
 from pathlib import Path
 from typing import Optional, Union
 
-from fileutils import FileHandle
-from molecules import PDBStructure
-from mutation import Mutation
-from basemutator import BaseMutator
+from locuaz.fileutils import FileHandle
+from locuaz.molecules import PDBStructure
+from locuaz.mutation import Mutation
+from locuaz.basemutator import BaseMutator
 
 
 class MutatorEvoEF2(BaseMutator):
     bin_path: FileHandle
 
     def __init__(self, bin_dir: Path, radius: float = 5) -> None:
         self.bin_path = FileHandle(Path(bin_dir, "EvoEF2"))
```

### Comparing `locuaz-0.2.0/locuaz/mutators.py` & `locuaz-0.2.1/locuaz/mutators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Dict, Type
 import warnings
 
-from basemutator import BaseMutator
-from mutatorbiobb import MutatorBiobb
-from mutatorevoef2 import MutatorEvoEF2
+from locuaz.basemutator import BaseMutator
+from locuaz.mutatorbiobb import MutatorBiobb
+from locuaz.mutatorevoef2 import MutatorEvoEF2
 
 __all__ = ("mutators",)
 
 mutators: Dict[str, Type[BaseMutator]] = {
     "biobb": MutatorBiobb,
     "evoef2": MutatorEvoEF2,
 }
 
 try:
-    from mutatordlpr import MutatorDLPackerReconstruct
-    from mutatordlp import MutatorDLPacker
+    from locuaz.mutatordlpr import MutatorDLPackerReconstruct
+    from locuaz.mutatordlp import MutatorDLPacker
 
     mutators["dlp"] = MutatorDLPacker
     mutators["dlpr"] = MutatorDLPackerReconstruct
 except ModuleNotFoundError:
-    warnings.warn("Could not import DLPacker, dlp and dlpr mutators won't be available.")
+    warnings.warn("Could not import DLPacker, dlp and dlpr mutators won't be available.")
```

### Comparing `locuaz-0.2.0/locuaz/piepisa.py` & `locuaz-0.2.1/locuaz/piepisa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import concurrent.futures as cf
 import subprocess as sp
 from pathlib import Path
 from typing import Tuple, List
 
-from abstractscoringfunction import AbstractScoringFunction
-from complex import GROComplex
-from fileutils import FileHandle, DirHandle
+from locuaz.abstractscoringfunction import AbstractScoringFunction
+from locuaz.complex import GROComplex
+from locuaz.fileutils import FileHandle, DirHandle
 
 
 class PiePisa(AbstractScoringFunction):
     parameters_handle: FileHandle
     TIMEOUT_PER_FRAME: int = 2
 
     def __init__(self, sf_dir, *, nthreads=2, mpiprocs=2) -> None:
```

### Comparing `locuaz-0.2.0/locuaz/pisa.py` & `locuaz-0.2.1/locuaz/pisa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import concurrent.futures as cf
 import subprocess as sp
 from pathlib import Path
 from typing import Tuple, List
 
-from abstractscoringfunction import AbstractScoringFunction
-from complex import GROComplex
-from fileutils import FileHandle, DirHandle
+from locuaz.abstractscoringfunction import AbstractScoringFunction
+from locuaz.complex import GROComplex
+from locuaz.fileutils import FileHandle, DirHandle
 
 
 class Pisa(AbstractScoringFunction):
     parameters_handle: FileHandle
     TIMEOUT_PER_FRAME: int = 2
 
     def __init__(self, sf_dir, *, nthreads=2, mpiprocs=2) -> None:
```

### Comparing `locuaz-0.2.0/locuaz/primitives.py` & `locuaz-0.2.1/locuaz/primitives.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,14 +36,23 @@
 class GromacsError(Exception):
     pass
 
 class UserInputError(Exception):
     pass
 
 def launch_biobb(biobb_obj, *, can_write_console_log: bool = False, backup_dict: Optional[Path] = None) -> None:
+    """
+
+    :param biobb_obj:
+    :type biobb_obj:
+    :param can_write_console_log:
+    :type can_write_console_log:
+    :param backup_dict:
+    :type backup_dict:
+    """
     biobb_obj.can_write_console_log = can_write_console_log
     err = biobb_obj.launch()
     if err == 0 or err is None:
         try:
             Path(biobb_obj.out_log.name).unlink()
             Path(biobb_obj.err_log.name).unlink()
         except (FileNotFoundError, Exception):
```

### Comparing `locuaz-0.2.0/locuaz/projectutils.py` & `locuaz-0.2.1/locuaz/projectutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 from numpy.typing import NDArray
 
 import MDAnalysis as mda
 import numpy as np
 from Bio.SeqUtils import seq1
 from attrs import define, field, validators
 
-from abstractscoringfunction import AbstractScoringFunction
-from complex import AbstractComplex, GROComplex
-from fileutils import FileHandle, DirHandle, copy_to
-from primitives import AA_MAP
-from scoringfunctions import scoringfunctions
-from interface import get_freesasa_residues
+from locuaz.abstractscoringfunction import AbstractScoringFunction
+from locuaz.complex import AbstractComplex, GROComplex
+from locuaz.fileutils import FileHandle, DirHandle, copy_to
+from locuaz.primitives import AA_MAP
+from locuaz.scoringfunctions import scoringfunctions
+from locuaz.interface import get_freesasa_residues
 
 
 # TODO: replace own pairwise with itertools' on 3.10
 def pairwise(iterable):
     # pairwise('ABCDEFG') --> AB BC CD DE EF FG
     a, b = tee(iterable)
     next(b, None)
```

### Comparing `locuaz-0.2.0/locuaz/protocol.py` & `locuaz-0.2.1/locuaz/protocol.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import logging
 import sys
 from pathlib import Path
 
-import cli
-from projectutils import set_logger, WorkProject
-from epochinitializer import initialize_new_epoch
-from pruners import prune
-from run import run_epoch, run_npt_epoch
-from scoring import score
-
+import locuaz.cli
+from locuaz.projectutils import set_logger, WorkProject
+from locuaz.epochinitializer import initialize_new_epoch
+from locuaz.pruners import prune
+from locuaz.run import run_epoch, run_npt_epoch
+from locuaz.scoring import score
 
 def main() -> int:
 
-    config, start = cli.main()
+    config, start = locuaz.cli.main()
     log = set_logger(config["main"]["name"], Path(config["paths"]["work"]))
     log.info("-----------------------------")
     log.info("Setting up work project.")
     work_pjct = WorkProject(config, start)
     log = logging.getLogger(work_pjct.name)
     log.info("Launching.")
```

### Comparing `locuaz-0.2.0/locuaz/pruner.py` & `locuaz-0.2.1/locuaz/pruner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Tuple, Dict
 from queue import PriorityQueue
 import logging
 
-from projectutils import Epoch, Iteration
+from locuaz.projectutils import Epoch, Iteration
 
 
 def beats_old_iter(
     old_iter: Iteration, new_iter: Iteration, threshold: int, log: logging.Logger
 ) -> Tuple[bool, int]:
 
     # Allow the user to change scoring functions mid-run and only use
```

### Comparing `locuaz-0.2.0/locuaz/pruners.py` & `locuaz-0.2.1/locuaz/pruners.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Callable, Set
 import logging
 
-from projectutils import WorkProject
-from pruner import choose_top_iters, adaptive_pruner, top_pruner, threshold_pruner
+from locuaz.projectutils import WorkProject
+from locuaz.pruner import choose_top_iters, adaptive_pruner, top_pruner, threshold_pruner
 
 
 pruners: Dict[str, Callable] = {
     "adaptive": adaptive_pruner,
     "top": top_pruner,
     "threshold": threshold_pruner,
 }
```

### Comparing `locuaz-0.2.0/locuaz/rosetta.py` & `locuaz-0.2.1/locuaz/rosetta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import concurrent.futures as cf
 import os
 import subprocess as sp
 from pathlib import Path
 from typing import Tuple, List, Union
 
-from abstractscoringfunction import AbstractScoringFunction
-from complex import GROComplex
-from fileutils import DirHandle, FileHandle
+from locuaz.abstractscoringfunction import AbstractScoringFunction
+from locuaz.complex import GROComplex
+from locuaz.fileutils import DirHandle, FileHandle
 
 
 class Rosetta(AbstractScoringFunction):
     TIMEOUT_PER_FRAME: int = 30
 
     def __init__(self, sf_dir, *, nthreads=2, mpiprocs=2) -> None:
         super().__init__(sf_dir, nthreads=nthreads, mpiprocs=mpiprocs)
```

### Comparing `locuaz-0.2.0/locuaz/run.py` & `locuaz-0.2.1/locuaz/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from pathlib import Path
 from concurrent.futures import ProcessPoolExecutor
 import concurrent.futures as cf
 
-from projectutils import WorkProject
-from runutils import MDrun
+from locuaz.projectutils import WorkProject
+from locuaz.runutils import MDrun
 
 def run_epoch(work_pjct: WorkProject) -> None:
     log = logging.getLogger(f"{work_pjct.name}")
     
     if not work_pjct.epochs[-1].nvt_done:
         run_min_nvt_epoch(work_pjct)
     else:
@@ -110,8 +110,8 @@
                 "This run may not be apt to continue.")
                 iter.outside_box = True
 
             
     epoch.npt_done = True
 
 
-        
+
```

### Comparing `locuaz-0.2.0/locuaz/runutils.py` & `locuaz-0.2.1/locuaz/runutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from typing import Tuple, Union
 import subprocess as sp
 
 from attrs import define, field
 from biobb_analysis.gromacs.gmx_trjconv_str import GMXTrjConvStr
 from biobb_gromacs.gromacs.grompp import Grompp
 
-from complex import AbstractComplex, GROComplex
-from fileutils import DirHandle, FileHandle
-from molecules import ZipTopology, copy_mol_to
-from fixbox import fix_box_cpx
-from primitives import launch_biobb, GromacsError
-from projectutils import WorkProject
+from locuaz.complex import AbstractComplex, GROComplex
+from locuaz.fileutils import DirHandle, FileHandle
+from locuaz.molecules import ZipTopology, copy_mol_to
+from locuaz.fixbox import fix_box_cpx
+from locuaz.primitives import launch_biobb, GromacsError
+from locuaz.projectutils import WorkProject
 
 
 @define(frozen=True)
 class MDrun:
     dir: DirHandle = field(converter=DirHandle)  # type: ignore
     binary_path: str = field(converter=str, kw_only=True)
     mdp: FileHandle = field(converter=FileHandle, kw_only=True)  # type: ignore
```

### Comparing `locuaz-0.2.0/locuaz/scoring.py` & `locuaz-0.2.1/locuaz/scoring.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import sys
 import time
 from pathlib import Path
 from typing import Optional, Tuple
 
 from biobb_analysis.gromacs.gmx_trjconv_str_ens import GMXTrjConvStrEns
 
-from fileutils import DirHandle
-from gromacsutils import image_traj
-from primitives import launch_biobb
-from projectutils import WorkProject, Iteration
-from utils_scoring import extract_pdbs, join_target_binder, rm_aux_scoring_files
-from stats import run_stats
+from locuaz.fileutils import DirHandle
+from locuaz.gromacsutils import image_traj
+from locuaz.primitives import launch_biobb
+from locuaz.projectutils import WorkProject, Iteration
+from locuaz.utils_scoring import extract_pdbs, join_target_binder, rm_aux_scoring_files
+from locuaz.stats import run_stats
 
 
 def initialize_scoring_folder(
         iteration: Iteration, config: dict, *, log: Optional[logging.Logger] = None
 ) -> Tuple[int, int]:
     """
     Creates scoring folder inside the iteration dir, fixes PBC issues with the original NPT trajectory
```

### Comparing `locuaz-0.2.0/locuaz/scoringfunctions.py` & `locuaz-0.2.1/locuaz/scoringfunctions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Dict, Type
 
-from abstractscoringfunction import AbstractScoringFunction
-from bach import Bach
-from bluues import Bluues
-from bluuesbmf import BluuesBmf
-from evoef2 import Evoef2
-from gmxmmpbsa import GmxMmpbsa
-from haddock import Haddock
-from pisa import Pisa
-from piepisa import PiePisa
-from rosetta import Rosetta
-from autodockvina import AutodockVina
+from locuaz.abstractscoringfunction import AbstractScoringFunction
+from locuaz.bach import Bach
+from locuaz.bluues import Bluues
+from locuaz.bluuesbmf import BluuesBmf
+from locuaz.evoef2 import Evoef2
+from locuaz.gmxmmpbsa import GmxMmpbsa
+from locuaz.haddock import Haddock
+from locuaz.pisa import Pisa
+from locuaz.piepisa import PiePisa
+from locuaz.rosetta import Rosetta
+from locuaz.autodockvina import AutodockVina
 
 scoringfunctions: Dict[str, Type[AbstractScoringFunction]] = {
     "bach": Bach,
     "bluues": Bluues,
     "bluuesbmf": BluuesBmf,
     "evoef2": Evoef2,
     "haddock": Haddock,
```

### Comparing `locuaz-0.2.0/locuaz/spm4.py` & `locuaz-0.2.1/locuaz/spm4.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from collections.abc import Iterable, ItemsView
 from typing import List, Tuple, Dict, Set, Iterator
 from random import choice, sample
 from collections import defaultdict
 from logging import Logger
 
-from projectutils import Iteration, Epoch
-from mutation import Mutation
-from abstractmutationgenerator import AbstractMutationGenerator
+from locuaz.projectutils import Iteration, Epoch
+from locuaz.mutation import Mutation
+from locuaz.abstractmutationgenerator import AbstractMutationGenerator
 
 
 class SPM4(AbstractMutationGenerator):
-    # Cystein is not included.
+    """
+    SPM4 generates mutations by splitting all amino acids (except CYS) in the following categories:
+    negative, positive, hydrophobic and ring-containing.
+    It will pick 1 amino acid from each category until it generates one for each branch and randomly pick a
+    position for all of them, hence SPM (Single Point Mutation).
+    """
     NEG_AAS: Tuple = ("D", "E", "S", "T")
     POS_AAS: Tuple = ("R", "N", "Q", "H", "K")
+    # Cystein is not included.
     PHO_AAS: Tuple = ("A", "G", "I", "M", "L", "V")
     RIN_AAS: Tuple = ("P", "F", "W", "Y")
     CAT_AAS: Tuple[Tuple, Tuple, Tuple, Tuple] = (
         NEG_AAS,
         POS_AAS,
         PHO_AAS,
         RIN_AAS,
@@ -48,25 +54,27 @@
 
         mut_idx_chain, mut_chainID, mut_idx_residue, mut_resSeq = self.__generate_position__(epoch, use_tleap, logger)
         self.__fill_mutations__(epoch, branches, mut_idx_chain, mut_chainID, mut_idx_residue, mut_resSeq)
 
     def __fill_mutations__(self, epoch: Epoch, branches: int, mut_idx_chain: int, mut_chainID: str,
                            mut_idx_residue: int, mut_resSeq: int):
         """
-        __fill_mutation__(): generates up to `branches` different mutations
-        Args:
-            epoch:
-            branches:
-            mut_idx_chain:
-            mut_chainID:
-            mut_idx_residue:
-            mut_resSeq:
-
-        Returns: None. It fills the Generator with Mutation objects.
-
+        generates up to `branches` different mutations
+        :param epoch:
+        :type epoch:
+        :param branches:
+        :type branches:
+        :param mut_idx_chain:
+        :type mut_idx_chain:
+        :param mut_chainID:
+        :type mut_chainID:
+        :param mut_idx_residue:
+        :type mut_idx_residue:
+        :param mut_resSeq:
+        :type mut_resSeq:
         """
         remaining_branches = branches
         remaining_iterations = set(epoch.top_iterations.keys())
         while remaining_branches != 0:
             iteration = epoch.top_iterations[remaining_iterations.pop()]
             old_aa, new_aa = self.__get_random_aa__(iteration, mut_idx_chain, mut_idx_residue)
             # Build the mutation object for this iteration.
```

### Comparing `locuaz-0.2.0/locuaz/spm4i.py` & `locuaz-0.2.1/locuaz/spm4i.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from collections.abc import Iterable, ItemsView
 from typing import List, Tuple, Set, Iterator
 from random import choice
 from collections import defaultdict
 from logging import Logger
 
-from projectutils import Iteration, Epoch
-from mutation import Mutation
-from interface import get_interfacing_residues
-from spm4 import SPM4
+from locuaz.projectutils import Iteration, Epoch
+from locuaz.mutation import Mutation
+from locuaz.interface import get_interfacing_residues
+from locuaz.spm4 import SPM4
 
 
 class SPM4i(SPM4):
-
+    """
+    overrides ``__generate_position__()``. It uses freesasa to get the interface to prevent mutations on positions
+    that are not in contact.
+    """
     def __init__(
             self,
             epoch: Epoch,
             branches: int,
             *,
             excluded_aas: Set[str],
             excluded_pos: Set[int],
```

### Comparing `locuaz-0.2.0/locuaz/spm4mmpbsa.py` & `locuaz-0.2.1/locuaz/spm4mmpbsa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from collections.abc import Iterable, ItemsView
 from typing import List, Tuple, Set, Iterator, Dict, Optional
 from collections import defaultdict
 from logging import Logger
 from pathlib import Path
 import csv
 
-from projectutils import Iteration, Epoch
-from mutation import Mutation
-from interface import get_interfacing_residues
-from spm4 import SPM4
+from locuaz.projectutils import Iteration, Epoch
+from locuaz.mutation import Mutation
+from locuaz.interface import get_interfacing_residues
+from locuaz.spm4 import SPM4
 
 
 class SPM4gmxmmpbsa(SPM4):
-
+    """
+        overrides ``__generate_position__()``. It uses freesasa to get the interface to prevent mutations on positions
+        that are not in contact and also sorts residues according to the binding ΔG, according to the gmxmmpbsa
+        scoring function
+    """
     def __init__(
             self,
             epoch: Epoch,
             branches: int,
             *,
             excluded_aas: Set[str],
             excluded_pos: Set[int],
```

### Comparing `locuaz-0.2.0/locuaz/statisticcmdistance.py` & `locuaz-0.2.1/locuaz/statisticcmdistance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Dict
 import numpy as np
 
 from numpy.typing import NDArray
 import MDAnalysis as mda
 from MDAnalysis.analysis.distances import distance_array
 
-from projectutils import Iteration
-from molecules import XtcTrajectory, PDBStructure
-from basestatistic import BaseStatistic
+from locuaz.projectutils import Iteration
+from locuaz.molecules import XtcTrajectory, PDBStructure
+from locuaz.basestatistic import BaseStatistic
 
 
 class StatisticCMDistance(BaseStatistic):
     pdb_top: PDBStructure
     trj: XtcTrajectory
 
     def __init__(self, iteration: Iteration, stats_config: Dict) -> None:
```

### Comparing `locuaz-0.2.0/locuaz/statisticinterface.py` & `locuaz-0.2.1/locuaz/statisticinterface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 from typing import List
 import concurrent.futures as cf
 import numpy as np
 from numpy.typing import NDArray
 
-from projectutils import Iteration
-from basestatistic import BaseStatistic
-from interface import get_interface_surface
+from locuaz.projectutils import Iteration
+from locuaz.basestatistic import BaseStatistic
+from locuaz.interface import get_interface_surface
 
 
 class StatisticInterface(BaseStatistic):
     TIMEOUT_PER_FRAME: int = 2
 
     def __init__(self, iteration: Iteration, stats_config: dict) -> None:
         super().__init__(iteration, stats_config)
```

### Comparing `locuaz-0.2.0/locuaz/stats.py` & `locuaz-0.2.1/locuaz/stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from typing import Dict, Optional, Type
 
-from projectutils import Iteration
-from basestatistic import BaseStatistic
-from statisticcmdistance import StatisticCMDistance
-from statisticinterface import StatisticInterface
+from locuaz.projectutils import Iteration
+from locuaz.basestatistic import BaseStatistic
+from locuaz.statisticcmdistance import StatisticCMDistance
+from locuaz.statisticinterface import StatisticInterface
 
 all_stats: Dict[str, Type[BaseStatistic]] = {
     "cmdistance": StatisticCMDistance,
     "interface": StatisticInterface,
 }
```

### Comparing `locuaz-0.2.0/locuaz/utils_scoring.py` & `locuaz-0.2.1/locuaz/utils_scoring.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 import re
 import zipfile
 from collections.abc import Iterable
 from pathlib import Path
 from typing import Optional, List, Tuple, Set
 
-from fileutils import DirHandle, FileHandle, catenate_pdbs
-from gromacsutils import fix_gromacs_pdb
+from locuaz.fileutils import DirHandle, FileHandle, catenate_pdbs
+from locuaz.gromacsutils import fix_gromacs_pdb
 
 
 def extract_pdbs(
         zip_file: Path,
         out_prefix: str,
         *,
         nprocs: int = 1,
@@ -131,8 +131,8 @@
             Path(inp_file).unlink()
 
     if "gmxmmpbsa" in scoring_functions:
         haddock_dir = frames_path / "gmxmmpbsa"
         for xtc_file in glob.glob(str(Path(haddock_dir, "*xtc"))):
             Path(xtc_file).unlink()
         for mdcrd_file in glob.glob(str(Path(haddock_dir, "*mdcrd*"))):
-            Path(mdcrd_file).unlink()
+            Path(mdcrd_file).unlink()
```

### Comparing `locuaz-0.2.0/locuaz/validatore.py` & `locuaz-0.2.1/locuaz/validatore.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.0/locuaz.egg-info/PKG-INFO` & `locuaz-0.2.1/locuaz.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 Metadata-Version: 2.1
 Name: locuaz
-Version: 0.2.0
+Version: 0.2.1
 Summary: Antibody optimization protocol
 Author: Patricio Barletta
 Author-email: pbarletta@gmail.com
 Keywords: molecular,dynamics,antibody,antibodies
-Requires-Python: ==3.10.10
+Requires-Python: >=3.9.15
 Description-Content-Type: text/x-rst
+Provides-Extra: docs
 License-File: LICENSE.rst
 
 ========
 locuaz
 ========
 
 
 .. image:: https://img.shields.io/pypi/v/locuaz.svg
         :target: https://pypi.python.org/pypi/locuaz
 
-.. image:: https://img.shields.io/travis/pgbarletta/locuaz.svg
-        :target: https://app.travis-ci.com/github/pgbarletta/locuaz/builds
-
 .. image:: https://readthedocs.org/projects/locuaz/badge/?version=latest
         :target: https://locuaz.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 Looping Uniquely Catered Amino Acid Sequences
 
 
 * Free software: MIT license
 * Documentation: https://locuaz.readthedocs.io.
 
 Install
 --------
 
+Check the `Installation <https://locuaz.readthedocs.io/en/latest/installation.html>`_ section on the docs..
+
 Mambaforge is recommended instead of pure conda. Download Mambaforge from:
 
 https://github.com/conda-forge/miniforge
 
-Clone this repo and, optionally, get the **DLPacker**  submodule as well::
-
-    git clone https://github.com/pgbarletta/locuaz
-    git submodule int
-    git submodule update
 
-You'll also have to get DLPacker's `weights <https://drive.google.com/file/d/1J4fV9aAr2nssrWN8mQ7Ui-9PVQseE0LQ/view?usp=sharing>`_.
+Why there's no straight pip or conda install
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Being this a high-level protocol, there are many dependencies to it and, unfortunately, python packaging has its quirks so
+different developers have solved their issues in different ways.
+A straight `pip install` is out of the question given the tensorflow (for DLPacker) and ambertools (for tleap) dependencies.
+On the other hand, not all packages have a conda recipe (freesasa), and while the biobb packages do show up on the bioconda
+channel, when installed in this manner, they bring over many unwanted, heavy dependencies, like GROMACS itself.
+So, in summary, a mix of pip and conda is needed.
 
 Post-Install
 -------------
 If on MDAnalysis 2.4.3 or older, edit the file ``MDAnalysis/topology/tpr/utils.py`` line 330::
     
   segid = f"seg_{i}_{molblock}"
```

### Comparing `locuaz-0.2.0/locuaz.egg-info/SOURCES.txt` & `locuaz-0.2.1/locuaz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.0/setup.cfg` & `locuaz-0.2.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 [metadata]
 name = locuaz
-version = 0.2.0
+version = 0.2.1
 author = Patricio Barletta
 author_email = pbarletta@gmail.com
 description = Antibody optimization protocol
 long_description = file: README.rst, CHANGELOG.rst, LICENSE.rst
 long_description_content_type = text/x-rst
 keywords = molecular, dynamics, antibody, antibodies
 
 [options]
-python_requires = ==3.10.10
-packages = locuaz, locuaz.DLPacker
+python_requires = >=3.9.15
+packages = locuaz
 install_requires = 
+	py
 	scipy
 	numpy >=1.21.0,<2.0.0
 	attrs
-	mdanalysis == 2.3.0
+	chemfiles
+	mdanalysis >= 2.3.0
 	biobb_common
 	biobb_analysis
 	biobb_model
 	biobb_io
 	biobb_gromacs
 	pdb2pqr
 	gmx-mmpbsa
 	tqdm
 	freesasa
 	pytest
+	cerberus
+
+[options.extras_require]
+docs = 
 	sphinx
 	sphinx-rtd-theme
-	cerberus
 
 [options.entry_points]
 console_scripts = 
 	executable-name = locuaz.protocol:main
 
 [build_sphinx]
 all-files = 1
 source-dir = docs/source
 build-dir = docs/build/html
-warning-is-error = 1
+warning-is-error = 0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `locuaz-0.2.0/tests/test_locuaz.py` & `locuaz-0.2.1/tests/test_locuaz.py`

 * *Files identical despite different names*

