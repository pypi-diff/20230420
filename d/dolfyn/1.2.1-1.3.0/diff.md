# Comparing `tmp/dolfyn-1.2.1.tar.gz` & `tmp/dolfyn-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolfyn-1.2.1.tar", last modified: Mon Feb 20 20:55:27 2023, max compression
+gzip compressed data, was "dolfyn-1.3.0.tar", last modified: Thu Apr 20 17:35:28 2023, max compression
```

## Comparing `dolfyn-1.2.1.tar` & `dolfyn-1.3.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-02-20 20:55:27.799636 dolfyn-1.2.1/
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     1832 2023-02-20 20:53:55.000000 dolfyn-1.2.1/LICENSE.txt
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      495 2023-02-20 20:55:27.797679 dolfyn-1.2.1/PKG-INFO
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     3089 2023-02-20 20:53:55.000000 dolfyn-1.2.1/README.md
-drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-02-20 20:55:27.454636 dolfyn-1.2.1/dolfyn/
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      959 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/__init__.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      433 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/_version.py
-drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-02-20 20:55:27.496495 dolfyn-1.2.1/dolfyn/adp/
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       19 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/adp/__init__.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      118 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/adp/api.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    12560 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/adp/clean.py
-drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-02-20 20:55:27.555622 dolfyn-1.2.1/dolfyn/adv/
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       17 2021-10-05 23:11:45.000000 dolfyn-1.2.1/dolfyn/adv/__init__.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      250 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/adv/api.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    10401 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/adv/clean.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    18926 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/adv/motion.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    17593 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/adv/turbulence.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    16992 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/binned.py
-drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-02-20 20:55:27.571965 dolfyn-1.2.1/dolfyn/example_data/
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       22 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/example_data/__init__.py
-drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-02-20 20:55:27.688118 dolfyn-1.2.1/dolfyn/io/
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       18 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/io/__init__.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    12334 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/io/api.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    12324 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/io/base.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    41758 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/io/nortek.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    22473 2023-02-20 20:53:55.000000 dolfyn-1.2.1/dolfyn/io/nortek2.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    14414 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/io/nortek2_defs.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    15609 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/io/nortek2_lib.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    12657 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/io/nortek_defs.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    54533 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/io/rdi.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     9730 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/io/rdi_defs.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     5780 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/io/rdi_lib.py
-drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-02-20 20:55:27.746154 dolfyn-1.2.1/dolfyn/rotate/
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       19 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/rotate/__init__.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    10626 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/rotate/api.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       79 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/rotate/awac.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     9862 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/rotate/base.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     6042 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/rotate/rdi.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     4672 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/rotate/signature.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     9183 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/rotate/vector.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     6739 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/time.py
-drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-02-20 20:55:27.772206 dolfyn-1.2.1/dolfyn/tools/
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2021-08-13 22:12:42.000000 dolfyn-1.2.1/dolfyn/tools/__init__.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     9917 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/tools/misc.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    13086 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/tools/psd.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    38848 2023-02-20 20:53:56.000000 dolfyn-1.2.1/dolfyn/velocity.py
-drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-02-20 20:55:27.477952 dolfyn-1.2.1/dolfyn.egg-info/
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      495 2023-02-20 20:55:27.000000 dolfyn-1.2.1/dolfyn.egg-info/PKG-INFO
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      997 2023-02-20 20:55:27.000000 dolfyn-1.2.1/dolfyn.egg-info/SOURCES.txt
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        1 2023-02-20 20:55:27.000000 dolfyn-1.2.1/dolfyn.egg-info/dependency_links.txt
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       66 2023-02-20 20:55:27.000000 dolfyn-1.2.1/dolfyn.egg-info/requires.txt
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        7 2023-02-20 20:55:27.000000 dolfyn-1.2.1/dolfyn.egg-info/top_level.txt
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      104 2023-02-20 20:53:56.000000 dolfyn-1.2.1/pyproject.toml
-drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-02-20 20:55:27.786955 dolfyn-1.2.1/scripts/
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      596 2023-02-20 20:53:56.000000 dolfyn-1.2.1/scripts/binary2mat.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     5809 2023-02-20 20:53:56.000000 dolfyn-1.2.1/scripts/motcorrect_vector.py
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       38 2023-02-20 20:55:27.799636 dolfyn-1.2.1/setup.cfg
--rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     1670 2023-02-20 20:53:56.000000 dolfyn-1.2.1/setup.py
+drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-04-20 17:35:28.119614 dolfyn-1.3.0/
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     1832 2023-04-20 17:34:13.000000 dolfyn-1.3.0/LICENSE.txt
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      495 2023-04-20 17:35:28.117601 dolfyn-1.3.0/PKG-INFO
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     2645 2023-04-20 17:34:13.000000 dolfyn-1.3.0/README.md
+drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-04-20 17:35:27.679502 dolfyn-1.3.0/dolfyn/
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      959 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/__init__.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      433 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/_version.py
+drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-04-20 17:35:27.738927 dolfyn-1.3.0/dolfyn/adp/
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       19 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/adp/__init__.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      176 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/adp/api.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    13133 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/adp/clean.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    33327 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/adp/turbulence.py
+drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-04-20 17:35:27.801747 dolfyn-1.3.0/dolfyn/adv/
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       17 2023-04-19 15:45:19.000000 dolfyn-1.3.0/dolfyn/adv/__init__.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      250 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/adv/api.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    10401 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/adv/clean.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    19816 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/adv/motion.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    22283 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/adv/turbulence.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    18068 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/binned.py
+drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-04-20 17:35:27.818753 dolfyn-1.3.0/dolfyn/example_data/
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       22 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/example_data/__init__.py
+drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-04-20 17:35:27.994332 dolfyn-1.3.0/dolfyn/io/
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       18 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/io/__init__.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    11941 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/io/api.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    12324 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/io/base.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    41729 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/io/nortek.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    22748 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/io/nortek2.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    14414 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/io/nortek2_defs.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    15609 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/io/nortek2_lib.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    12657 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/io/nortek_defs.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    54809 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/io/rdi.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     9926 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/io/rdi_defs.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     5758 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/io/rdi_lib.py
+drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-04-20 17:35:28.065972 dolfyn-1.3.0/dolfyn/rotate/
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       19 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/rotate/__init__.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    10626 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/rotate/api.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       79 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/rotate/awac.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    10753 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/rotate/base.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     6296 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/rotate/rdi.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     4622 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/rotate/signature.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     9331 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/rotate/vector.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     6739 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/time.py
+drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-04-20 17:35:28.094726 dolfyn-1.3.0/dolfyn/tools/
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-04-19 15:45:20.000000 dolfyn-1.3.0/dolfyn/tools/__init__.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     9917 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/tools/misc.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    13086 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/tools/psd.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)    40450 2023-04-20 17:34:14.000000 dolfyn-1.3.0/dolfyn/velocity.py
+drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-04-20 17:35:27.712537 dolfyn-1.3.0/dolfyn.egg-info/
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      495 2023-04-20 17:35:27.000000 dolfyn-1.3.0/dolfyn.egg-info/PKG-INFO
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     1022 2023-04-20 17:35:27.000000 dolfyn-1.3.0/dolfyn.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        1 2023-04-20 17:35:27.000000 dolfyn-1.3.0/dolfyn.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       66 2023-04-20 17:35:27.000000 dolfyn-1.3.0/dolfyn.egg-info/requires.txt
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        7 2023-04-20 17:35:27.000000 dolfyn-1.3.0/dolfyn.egg-info/top_level.txt
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      104 2023-04-20 17:34:14.000000 dolfyn-1.3.0/pyproject.toml
+drwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)        0 2023-04-20 17:35:28.114380 dolfyn-1.3.0/scripts/
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)      596 2023-04-20 17:34:14.000000 dolfyn-1.3.0/scripts/binary2mat.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     5809 2023-04-20 17:34:14.000000 dolfyn-1.3.0/scripts/motcorrect_vector.py
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)       38 2023-04-20 17:35:28.120143 dolfyn-1.3.0/setup.cfg
+-rwxrwxrwx   0 jmcvey3   (1000) jmcvey3   (1000)     1670 2023-04-20 17:34:14.000000 dolfyn-1.3.0/setup.py
```

### Comparing `dolfyn-1.2.1/LICENSE.txt` & `dolfyn-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolfyn-1.2.1/README.md` & `dolfyn-1.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,36 @@
 <img src="img/logo.png" width="70"> DOLfYN
 =======================
 ![Build](https://github.com/lkilcher/dolfyn/actions/workflows/build.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/lkilcher/dolfyn/badge.svg?branch=master)](https://coveralls.io/github/lkilcher/dolfyn?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/dolfyn/badge/?version=latest)](https://dolfyn.readthedocs.io/en/latest/?badge=latest)
 
-BIG NEWS!!!
-------
+Update from Version 0.12 to 1.0+
+-------------------------------
 
-Hello everyone! Just so that you know, we have released
-dolfyn 1.0! This is a MAJOR REFACTOR of the code so that DOLfYN is
+Hello everyone! This is a MAJOR REFACTOR of the code so that DOLfYN is
 now built on xarray, rather than the somewhat contrived and
 purpose-built `pyDictH5` package.
 
 This means that DOLfYN 1.0 is _not_ backwards compatible with
 earlier version. This, in turn, means two things:
 
 1. The data files (`.h5` files) you created with earlier versions
-of DOLfYN will no longer load with DOLfYN 1.0.0.
+of DOLfYN will no longer load with DOLfYN > v1.0.0.
 2. The syntax of DOLfYN 1.0 is completely different from earlier version.
 
 Because of this, it's probably easiest to continue using earlier
 versions of DOLfYN for your old data. If you want to bring some data
 into DOLfYN 1.0, you will need to
 `dolfyn.read(binary_source_file.ext)`, and then refactor your code to
 work properly with DOLfYN's new syntax. I may be providing some
 updates to dolfyn 0.12 via the v0.12-backports branch (and associated
 releases), but I doubt that will last long. If you are
 using 0.13, we recommend switching to 1.0.
 
-Very sorry that we didn't communicate the plan for this change, but
-the truth is that we simply don't know who our users are. The good
-news is that I think in the long run this will make DOLfYN a much more
-robust, powerful, and compatible tool -- especially because we now
-write/load xarray-formatted netcdf4 files, which is becoming a
-standard.
-
-A **HUGE THANK YOU** to @jmcvey3 who did the vast majority of the work
-to make this happen.
-
-
 Summary
 ------
 
 DOLfYN is the Doppler Oceanography Library for pYthoN.
 
 It is designed to read and work with Acoustic Doppler Velocimeter
 (ADV) and Acoustic Doppler Profiler (ADP/ADCP) data. DOLfYN includes
```

### Comparing `dolfyn-1.2.1/dolfyn/__init__.py` & `dolfyn-1.3.0/dolfyn/__init__.py`

 * *Files identical despite different names*

### Comparing `dolfyn-1.2.1/dolfyn/adp/clean.py` & `dolfyn-1.3.0/dolfyn/adp/clean.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,85 +103,96 @@
                                attrs={'units': 'm',
                                       'long_name': 'Depth',
                                       'standard_name': 'depth',
                                       'positive': 'down'})
 
 
 def find_surface_from_P(ds, salinity=35):
-    """Calculates the distance to the water surface. Temperature and salinity
-    are used to calculate seawater density, which is in turn used with the
-    pressure data to calculate depth.
+    """Calculates the distance to the water surface. Temperature, salinity,
+    and pressure are used to calculate seawater density, which is in turn 
+    used to calculate depth.
 
     Parameters
     ----------
     ds : xarray.Dataset
       The full adcp dataset
     salinity: numeric (default: 35)
-      Water salinity in psu
+      Water salinity in parts per thousand (ppt) or practical salinity 
+      units (psu)
 
     Returns
     -------
     None, operates "in place" and adds the variables "water_density" and
     "depth" to the input dataset.
 
     Notes
     -----
     Requires that the instrument's pressure sensor was calibrated/zeroed
     before deployment to remove atmospheric pressure.
 
-    Calculates seawater density at normal atmospheric pressure according
-    to the UNESCO 1981 equation of state. Does not include hydrostatic pressure.
+    Calculates seawater density using a linear approximation of the sea
+    water equation of state:
+
+    .. math:: \\rho - \\rho_0 = -\\alpha (T-T_0) + \\beta (S-S_0) + \\kappa P
+
+    Where :math:`\\rho` is water density, :math:`T` is water temperature,
+    :math:`P` is water pressure, :math:`S` is practical salinity, 
+    :math:`\\alpha` is the thermal expansion coefficient, :math:`\\beta` is 
+    the haline contraction coefficient, and :math:`\\kappa` is adiabatic 
+    compressibility.
     """
 
     # Density calcation
-    T = ds.temp.values
-    S = salinity
-    # standard mean ocean water
-    rho_smow = 999.842594 + 6.793953e-2*T - 9.095290e-3*T**2 + \
-        1.001685e-4*T**3 - 1.120083e-6*T**4 + 6.536332e-9*T**5
-    # at water surface
-    B1 = 8.2449e-1 - 4.0899e-3*T + 7.6438e-5*T**2 - 8.2467e-7*T**3 + 5.3875e-9*T**4
-    C1 = -5.7246e-3 + 1.0227e-4*T - 1.6546e-6*T**2
-    d0 = 4.8314e-4
-    rho_atm0 = rho_smow + B1*S + C1*S**1.5 + d0*S**2
+    P = ds.pressure.values
+    T = ds.temp.values  # temperature, degC
+    S = salinity  # practical salinity
+    rho0 = 1027  # kg/m^3
+    T0 = 10  # degC
+    S0 = 35  # psu assumed equivalent to ppt
+    a = 0.15  # thermal expansion coefficient, kg/m^3/degC
+    b = 0.78  # haline contraction coefficient, kg/m^3/ppt
+    k = 4.5e-3  # adiabatic compressibility, kg/m^3/dbar
+    rho = rho0 - a*(T-T0) + b*(S-S0) + k*P
 
     # Depth = pressure (conversion from dbar to MPa) / water weight
-    d = (ds.pressure*10000)/(9.81*rho_atm0)
+    d = (ds.pressure*10000)/(9.81*rho)
 
     if hasattr(ds, 'h_deploy'):
         d += ds.h_deploy
         description = "Depth to Seafloor"
     else:
         description = "Depth to Instrument"
 
     ds['water_density'] = xr.DataArray(
-        rho_atm0.astype('float32'),
+        rho.astype('float32'),
         dims=['time'],
         attrs={'units': 'kg m-3',
                'long_name': 'Water Density',
                'standard_name': 'sea_water_density',
-               'description': 'Water density according to UNESCO 1981 equation of state'})
+               'description': 'Water density from linear approximation of sea water equation of state'})
     ds['depth'] = xr.DataArray(
         d.astype('float32'),
         dims=['time'],
         attrs={'units': 'm',
-              'long_name': description,
-              'standard_name': 'depth',
-              'positive': 'down'})
+               'long_name': description,
+               'standard_name': 'depth',
+               'positive': 'down'})
 
 
-def nan_beyond_surface(ds, val=np.nan, inplace=False):
+def nan_beyond_surface(ds, val=np.nan, beam_angle=None, inplace=False):
     """Mask the values of 3D data (vel, amp, corr, echo) that are beyond the surface.
 
     Parameters
     ----------
     ds : xarray.Dataset
       The adcp dataset to clean
     val : nan or numeric (default: np.nan)
       Specifies the value to set the bad values to
+    beam_angle : int (default: dataset.attrs['beam_angle'])
+      ADCP beam inclination angle
     inplace : bool (default: False)
       When True the existing data object is modified. When False
       a copy is returned.
 
     Returns
     -------
     ds : xarray.Dataset
@@ -196,21 +207,20 @@
 
     if not inplace:
         ds = ds.copy(deep=True)
 
     # Get all variables with 'range' coordinate
     var = [h for h in ds.keys() if any(s for s in ds[h].dims if 'range' in s)]
 
-    if 'nortek' in _make_model(ds):
-        beam_angle = 25 * (np.pi/180)
-    else:  # TRDI
-        try:
-            beam_angle = ds.beam_angle
-        except:
-            beam_angle = 20 * (np.pi/180)
+    if beam_angle is None:
+        if hasattr(ds, 'beam_angle'):
+            beam_angle = ds.beam_angle * (np.pi/180)
+        else:
+            raise Exception("'beam_angle` not found in dataset attributes. "
+                            "Please supply the ADCP's beam angle.")
 
     # Surface interference distance calculated from distance of transducers to surface
     if hasattr(ds, 'h_deploy'):
         range_limit = ((ds.depth-ds.h_deploy) * np.cos(beam_angle) -
                        ds.cell_size) + ds.h_deploy
     else:
         range_limit = ds.depth * np.cos(beam_angle) - ds.cell_size
```

### Comparing `dolfyn-1.2.1/dolfyn/adv/clean.py` & `dolfyn-1.3.0/dolfyn/adv/clean.py`

 * *Files identical despite different names*

### Comparing `dolfyn-1.2.1/dolfyn/adv/motion.py` & `dolfyn-1.3.0/dolfyn/adv/motion.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,21 @@
         if self.accel_filtfreq == 0:
             acc[:] = acc.mean(-1)[..., None]
         else:
             flt = ss.butter(1, self.accel_filtfreq / (self.ds.fs / 2))
             for idx in range(3):
                 acc[idx] = ss.filtfilt(flt[0], flt[1], acc[idx], axis=-1)
 
+            # Fill nan with zeros - happens for some filter frequencies
+            if np.isnan(acc).any():
+                warnings.warn(
+                    "Error filtering acceleration data. "
+                    "Please decrease `accel_filtfreq`.")
+                acc = np.nan_to_num(acc)
+
     def calc_velacc(self, ):
         """Calculates the translational velocity from the high-pass
         filtered acceleration signal.
 
         Returns
         -------
         velacc : numpy.ndarray (3 x n_time)
@@ -159,14 +166,21 @@
             # 2nd order Butterworth filter
             # Applied twice by 'filtfilt' = 4th order butterworth
             filt = ss.butter(2, float(filt_freq) / (samp_freq / 2))
             for idx in range(hp.shape[0]):
                 dat[idx] = dat[idx] - \
                     ss.filtfilt(filt[0], filt[1], dat[idx], axis=-1)
 
+            # Fill nan with zeros - happens for some filter frequencies
+            if np.isnan(dat).any():
+                warnings.warn("Error filtering acceleration data. "
+                              "Please decrease `vel_filtfreq`. "
+                              "(default is 1/3 `accel_filtfreq`)")
+                dat = np.nan_to_num(dat)
+
         if n:
             # remove reshape
             velacc_shaped = np.empty(self.angrt.shape)
             acclow_shaped = np.empty(self.angrt.shape)
             accel_shaped = np.empty(self.angrt.shape)
             for idx in range(hp.shape[0]):
                 velacc_shaped[idx] = np.ravel(dat[idx], 'C')
@@ -374,14 +388,20 @@
     bottom-tracking ADP, or from a ship's GPS), it may be possible to
     remove that sigal from the ADV sigal in post-processing.
     """
 
     # Ensure acting on new dataset
     ds = ds.copy(deep=True)
 
+    # Check that no nan's exist
+    if ds['accel'].isnull().sum():
+        raise Exception("There should be no missing data in `accel` variable")
+    if ds['angrt'].isnull().sum():
+        raise Exception("There should be no missing data in `angrt` variable")
+
     if hasattr(ds, 'velrot') or ds.attrs.get('motion corrected', False):
         raise Exception('The data appears to already have been '
                         'motion corrected.')
 
     if not hasattr(ds, 'has_imu') or ('accel' not in ds):
         raise Exception('The instrument does not appear to have an IMU.')
 
@@ -479,14 +499,13 @@
     # NOTE: The plus sign is because the measured-induced velocities
     #       are in the opposite direction of the head motion.
     #       i.e. when the head moves one way in stationary flow, it
     #       measures a velocity in the opposite direction.
 
     # use xarray to keep dimensions consistent
     velmot = ds['velrot'] + ds['velacc']
-    velmot = velmot.values
-    ds['vel'][:3] += velmot
+    ds['vel'].values += velmot.values
 
     ds.attrs['motion corrected'] = 1
     ds.attrs['motion accel_filtfreq Hz'] = calcobj.accel_filtfreq
 
     return ds
```

### Comparing `dolfyn-1.2.1/dolfyn/adv/turbulence.py` & `dolfyn-1.3.0/dolfyn/adv/turbulence.py`

 * *Files 13% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                  window='hann',
                  n_bin=None,
                  n_fft_coh=None):
         """Calculate the cross-spectral density of velocity components.
 
         Parameters
         ----------
-        veldat   : xarray.DataArray
+        veldat : xarray.DataArray
           The raw 3D velocity data.
         freq_units : string
           Frequency units of the returned spectra in either Hz or rad/s 
           (`f` or :math:`\\omega`)
         fs : float (optional)
           The sample rate (default: from the binner).
         window : string or array
@@ -121,64 +121,193 @@
         Returns
         -------
         csd : xarray.DataArray (3, M, N_FFT)
           The first-dimension of the cross-spectrum is the three
           different cross-spectra: 'uv', 'uw', 'vw'.
         """
 
-        fs = self._parse_fs(fs)
+        fs_in = self._parse_fs(fs)
         n_fft = self._parse_nfft_coh(n_fft_coh)
         time = self.mean(veldat.time.values)
         veldat = veldat.values
+        if len(np.shape(veldat)) != 2:
+            raise Exception("This function is only valid for calculating TKE using "
+                            "the 3D velocity vector from an ADV.")
 
-        out = np.empty(self._outshape_fft(veldat[:3].shape, n_fft=n_fft),
+        out = np.empty(self._outshape_fft(veldat[:3].shape, n_fft=n_fft, n_bin=n_bin),
                        dtype='complex')
 
         # Create frequency vector, also checks whether using f or omega
         if 'rad' in freq_units:
-            fs = 2*np.pi*fs
+            fs = 2*np.pi*fs_in
             freq_units = 'rad s-1'
             units = 'm2 s-1 rad-1'
         else:
+            fs = fs_in
             freq_units = 'Hz'
             units = 'm2 s-2 Hz-1'
-        coh_freq = xr.DataArray(self.calc_freq(units=freq_units, coh=True),
-                                dims=['freq'],
-                                name='freq',
+        coh_freq = xr.DataArray(self.calc_freq(fs=fs_in, units=freq_units, n_fft=n_fft, coh=True),
+                                dims=['coh_freq'],
+                                name='coh_freq',
                                 attrs={'units': freq_units,
                                       'long_name': 'FFT Frequency Vector',
                                       'coverage_content_type': 'coordinate'}
                                 ).astype('float32')
 
         for ip, ipair in enumerate(self._cross_pairs):
             out[ip] = self.calc_csd_base(veldat[ipair[0]],
                                          veldat[ipair[1]],
-                                         n_bin=n_bin,
-                                         n_fft=n_fft,
-                                         window=window)
+                                     fs=fs,
+                                     window=window,
+                                     n_bin=n_bin,
+                                     n_fft=n_fft)
 
         csd = xr.DataArray(out.astype('complex64'),
                            coords={'C': self.C,
                                    'time': time,
-                                   'freq': coh_freq},
-                           dims=['C', 'time', 'freq'],
+                                   'coh_freq': coh_freq},
+                           dims=['C', 'time', 'coh_freq'],
                            attrs={'units': units, 
                                   'n_fft_coh': n_fft,
                                   'long_name': 'Cross Spectral Density',
                                   'standard_name': 'cross_spectral_density_of_sea_water_velocity'})
-        csd['freq'].attrs['units'] = freq_units
+        csd['coh_freq'].attrs['units'] = freq_units
 
         return csd
 
+    def calc_doppler_noise(self, psd, pct_fN=0.8):
+        """Calculate bias due to Doppler noise using the noise floor
+        of the velocity spectra.
+
+        Parameters
+        ----------
+        psd : xarray.DataArray (dir, time, f)
+          The ADV velocity spectra
+        pct_fN : float
+          Percent of Nyquist frequency to calculate characeristic frequency
+
+        Returns
+        -------
+        doppler_noise (xarray.DataArray): 
+          Doppler noise level in units of m/s
+
+        Notes
+        -----
+        Approximates bias from
+
+        .. :math: \\sigma^{2}_{noise} = N x f_{c}
+
+        where :math: `\\sigma_{noise}` is the bias due to Doppler noise,
+        `N` is the constant variance or spectral density, and `f_{c}`
+        is the characteristic frequency.
+
+        The characteristic frequency is then found as 
+
+        .. :math: f_{c} = pct_fN * (f_{s}/2)
+
+        where `f_{s}/2` is the Nyquist frequency.
+
+
+        Richard, Jean-Baptiste, et al. "Method for identification of Doppler noise 
+        levels in turbulent flow measurements dedicated to tidal energy." International 
+        Journal of Marine Energy 3 (2013): 52-64.
+
+        Thiébaut, Maxime, et al. "Investigating the flow dynamics and turbulence at a 
+        tidal-stream energy site in a highly energetic estuary." Renewable Energy 195 
+        (2022): 252-262.
+        """
+        
+        # Characteristic frequency set to 80% of Nyquist frequency
+        fN = self.fs/2
+        fc = pct_fN * fN
+
+        # Get units right
+        if psd.freq.units == "Hz":
+            f_range = slice(fc, fN)
+        else:
+            f_range = slice(2*np.pi*fc, 2*np.pi*fN)
+
+        # Noise floor
+        N2 = psd.sel(freq=f_range) * psd.freq.sel(freq=f_range)
+        noise_level = np.sqrt(N2.mean(dim='freq'))
+
+        return xr.DataArray(
+            noise_level.values.astype('float32'),
+            dims=['dir', 'time'],
+            attrs={'units': 'm/s',
+                   'long_name': 'Doppler Noise Level',
+                   'description': 'Doppler noise level calculated '
+                   'from PSD white noise'})
+
+    def check_turbulence_cascade_slope(self, psd, freq_range=[6.28, 12.57]):
+        """This function calculates the slope of the PSD, the power spectra 
+        of velocity, within the given frequency range. The purpose of this
+        function is to check that the region of the PSD containing the 
+        isotropic turbulence cascade decreases at a rate of :math:`f^{-5/3}`.
+
+        Parameters
+        ----------
+        psd : xarray.DataArray ([time,] freq)
+          The power spectral density (1D or 2D)
+        freq_range : iterable(2) (default: [6.28, 12.57])
+          The range over which the isotropic turbulence cascade occurs, in 
+          units of the psd frequency vector (Hz or rad/s)
+
+        Returns
+        -------
+        (m, b): tuple (slope, y-intercept)
+          A tuple containing the coefficients of the log-adjusted linear 
+          regression between PSD and frequency 
+
+        Notes
+        -----
+        Calculates slope based on the `standard` formula for dissipation:
+
+        .. math:: S(k) = \\alpha \\epsilon^{2/3} k^{-5/3} + N
+
+        The slope of the isotropic turbulence cascade, which should be 
+        equal to :math:`k^{-5/3}` or :math:`f^{-5/3}`, where k and f are 
+        the wavenumber and frequency vectors, is estimated using linear 
+        regression with a log transformation:
+
+        .. math:: log10(y) = m*log10(x) + b
+
+        Which is equivalent to
+
+        .. math:: y = 10^{b} x^{m}
+        
+        Where :math:`y` is S(k) or S(f), :math:`x` is k or f, :math:`m` 
+        is the slope (ideally -5/3), and :math:`10^{b}` is the intercept of 
+        y at x^m=1.
+        """
+
+        idx = np.where((freq_range[0] < psd.freq) & (psd.freq < freq_range[1]))
+        idx = idx[0]
+
+        x = np.log10(psd['freq'].isel(freq=idx))
+        y = np.log10(psd.isel(freq=idx))
+
+        y_bar = y.mean('freq')
+        x_bar = x.mean('freq')
+
+        # using the formula to calculate the slope and intercept
+        n = np.sum((x - x_bar) * (y - y_bar), axis=0)
+        d = np.sum((x - x_bar)**2, axis=0)
+
+        m = n/d
+        b = y_bar - m*x_bar
+
+        return m, b
+
     def calc_epsilon_LT83(self, psd, U_mag, freq_range=[6.28, 12.57]):
         """Calculate the dissipation rate from the PSD
 
         Parameters
         ----------
-        psd : xarray.DataArray (...,time,f)
+        psd : xarray.DataArray (...,time,freq)
           The power spectral density
         U_mag : xarray.DataArray (...,time)
           The bin-averaged horizontal velocity [m s-1] (from dataset shortcut)
         freq_range : iterable(2) (default: [6.28, 12.57])
           The range over which to integrate/average the spectrum, in units 
           of the psd frequency vector (Hz or rad/s)
 
@@ -207,35 +336,38 @@
 
         .. math:: S(\\omega) = \\alpha \\epsilon^{2/3} f^{-5/3} (U/(2\\pi))^{2/3} + N
         
         LT83 : Lumley and Terray, "Kinematics of turbulence convected
         by a random wave field". JPO, 1983, vol13, pp2000-2007.
         """
 
-        freq = psd.freq
+        # Ensure time has been averaged
+        if len(psd.time)!=len(U_mag.time):
+            raise Exception("`U_mag` should be from ensembled-averaged dataset")
 
+        freq = psd.freq
         idx = np.where((freq_range[0] < freq) & (freq < freq_range[1]))
         idx = idx[0]
 
         if freq.units == 'Hz':
             U = U_mag/(2*np.pi)
         else:
             U = U_mag
 
         a = 0.5
         out = (psd.isel(freq=idx) *
                freq.isel(freq=idx)**(5/3) / a).mean(axis=-1)**(3/2) / U
 
         return xr.DataArray(
-          out.astype('float32'),
-          attrs={'units': 'm2 s-3',
-                  'long_name': 'TKE Dissipation Rate',
-                  'standard_name': 'specific_turbulent_kinetic_energy_dissipation_in_sea_water',
-                  'description': 'TKE dissipation rate calculated using the method from Lumley and Terray, 1983',
-                  })
+            out.astype('float32'),
+            attrs={'units': 'm2 s-3',
+                   'long_name': 'Dissipation Rate',
+                   'standard_name': 'specific_turbulent_kinetic_energy_dissipation_in_sea_water',
+                   'description': 'TKE dissipation rate calculated using the method from Lumley and Terray, 1983',
+                   })
 
     def calc_epsilon_SF(self, vel_raw, U_mag, fs=None, freq_range=[2., 4.]):
         """Calculate dissipation rate using the "structure function" (SF) method
         
         Parameters
         ----------
         vel_raw : xarray.DataArray
@@ -273,22 +405,22 @@
             for L in range(int(fs / freq_range[1]), int(fs / freq_range[0])):
                 DAA[L] = np.nanmean((up[L:] - up[:-L]) ** 2, dtype=np.float64)
             cv2 = DAA / (lag ** (2 / 3))
             cv2m = np.median(cv2[np.logical_not(np.isnan(cv2))])
             out[slc[:-1]] = (cv2m / 2.1) ** (3 / 2)
 
         return xr.DataArray(
-          out.astype('float32'),
-          coords=U_mag.coords,
-          dims=U_mag.dims,
-          attrs={'units': 'm2 s-3',
-                  'long_name': 'TKE Dissipation Rate',
-                  'standard_name': 'specific_turbulent_kinetic_energy_dissipation_in_sea_water',
-                  'description': 'TKE dissipation rate calculated using the "structure function" method',
-                  })
+            out.astype('float32'),
+            coords=U_mag.coords,
+            dims=U_mag.dims,
+            attrs={'units': 'm2 s-3',
+                   'long_name': 'Dissipation Rate',
+                   'standard_name': 'specific_turbulent_kinetic_energy_dissipation_in_sea_water',
+                   'description': 'TKE dissipation rate calculated using the "structure function" method',
+                   })
 
     def _up_angle(self, U_complex):
         """Calculate the angle of the turbulence fluctuations.
 
         Parameters
         ----------
         U_complex  : |np.ndarray| (..., n_time * n_bin)
@@ -375,22 +507,22 @@
         out += (np.nanmean(psd[2] * freq**(5/3), -1) /
                 (12/55 * alpha * intgrl))**(3/2) / U_mag
 
         # Average the two estimates
         out *= 0.5
 
         return xr.DataArray(
-          out.astype('float32'),
-          coords={'time': dat_avg.psd.time},
-          dims='time',
-          attrs={'units': 'm2 s-3',
-                  'long_name': 'TKE Dissipation Rate',
-                  'standard_name': 'specific_turbulent_kinetic_energy_dissipation_in_sea_water',
-                  'description': 'TKE dissipation rate calculated using the method from Trowbridge and Elgar, 2001'
-                  })
+            out.astype('float32'),
+            coords={'time': dat_avg.psd.time},
+            dims='time',
+            attrs={'units': 'm2 s-3',
+                   'long_name': 'Dissipation Rate',
+                   'standard_name': 'specific_turbulent_kinetic_energy_dissipation_in_sea_water',
+                   'description': 'TKE dissipation rate calculated using the method from Trowbridge and Elgar, 2001'
+                   })
 
     def calc_L_int(self, a_cov, U_mag, fs=None):
         """Calculate integral length scales.
 
         Parameters
         ----------
         a_cov : xarray.DataArray
@@ -415,19 +547,20 @@
 
         acov = a_cov.values
         fs = self._parse_fs(fs)
 
         scale = np.argmin((acov/acov[..., :1]) > (1/np.e), axis=-1)
         L_int = U_mag.values / fs * scale
 
-        return xr.DataArray(L_int.astype('float32'),
-                            coords={'dir': a_cov.dir, 'time': a_cov.time},
-                            attrs={'units': 'm',
-                                   'long_name': 'Integral Length Scale',
-                                   'standard_name': 'turbulent_mixing_length_of_sea_water'})
+        return xr.DataArray(
+            L_int.astype('float32'),
+            coords={'dir': a_cov.dir, 'time': a_cov.time},
+            attrs={'units': 'm',
+                   'long_name': 'Integral Length Scale',
+                   'standard_name': 'turbulent_mixing_length_of_sea_water'})
 
 
 def calc_turbulence(ds_raw, n_bin, fs, n_fft=None, freq_units='rad/s', window='hann'):
     """Functional version of `ADVBinner` that computes a suite of turbulence 
     statistics for the input dataset, and returns a `binned` data object.
     
     Parameters
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dolfyn-1.2.1/dolfyn/binned.py` & `dolfyn-1.3.0/dolfyn/binned.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,15 @@
           Instrument sampling frequency in Hz
         n_fft : int
           Number of data points to use for fft (`n_fft`<=`n_bin`).
           Default: `n_fft`=`n_bin`
         n_fft_coh : int
           Number of data points to use for coherence and cross-spectra ffts
           Default: `n_fft_coh`=`n_fft`
-        noise : list or ndarray
+        noise : float, list or numpy.ndarray
           Instrument's doppler noise in same units as velocity
         """
 
         self.n_bin = n_bin
         self.fs = fs
         self.n_fft = n_fft
         self.n_fft_coh = n_fft_coh
@@ -38,17 +38,17 @@
         elif n_fft > n_bin:
             self.n_fft = n_bin
             warnings.warn(
                 "n_fft must be smaller than n_bin, setting n_fft = n_bin")
         if n_fft_coh is None:
             self.n_fft_coh = int(self.n_fft)
         elif n_fft_coh > n_bin:
-            self.n_fft_coh = int(n_bin // 6)
+            self.n_fft_coh = int(n_bin)
             warnings.warn("n_fft_coh must be smaller than or equal to n_bin, "
-                          "setting n_fft_coh = n_bin/6")
+                          "setting n_fft_coh = n_bin")
 
     def _outshape(self, inshape, n_pad=0, n_bin=None):
         """Returns `outshape` (the 'reshape'd shape) for an `inshape` array.
         """
         n_bin = int(self._parse_nbin(n_bin))
         return list(inshape[:-1]) + [int(inshape[-1] // n_bin), int(n_bin + n_pad)]
 
@@ -56,31 +56,39 @@
         """Returns `outshape` (the fft 'reshape'd shape) for an `inshape` array.
         """
         n_fft = self._parse_nfft(n_fft)
         n_bin = self._parse_nbin(n_bin)
         return list(inshape[:-1]) + [int(inshape[-1] // n_bin), int(n_fft // 2)]
 
     def _parse_fs(self, fs=None):
-        if fs is not None:
-            return fs
-        return self.fs
+        if fs is None:
+            return self.fs
+        return fs
 
     def _parse_nbin(self, n_bin=None):
         if n_bin is None:
             return self.n_bin
         return n_bin
 
     def _parse_nfft(self, n_fft=None):
         if n_fft is None:
             return self.n_fft
+        if n_fft > self.n_bin:
+            n_fft = self.n_bin
+            warnings.warn(
+                "n_fft must be smaller than n_bin, setting n_fft = n_bin")
         return n_fft
 
     def _parse_nfft_coh(self, n_fft_coh=None):
         if n_fft_coh is None:
             return self.n_fft_coh
+        if n_fft_coh > self.n_bin:
+            n_fft_coh = int(self.n_bin)
+            warnings.warn("n_fft_coh must be smaller than or equal to n_bin, "
+                          "setting n_fft_coh = n_bin")
         return n_fft_coh
 
     def _check_ds(self, raw_ds, out_ds):
         """Check that the attributes between two datasets match up.
 
         Parameters
         ----------
@@ -154,40 +162,45 @@
 
     def reshape(self, arr, n_pad=0, n_bin=None):
         """Reshape the array `arr` to shape (...,n,n_bin+n_pad).
 
         Parameters
         ----------
         arr : numpy.ndarray
+          Input data
         n_pad : int
           Is used to add `n_pad`/2 points from the end of the previous
           ensemble to the top of the current, and `n_pad`/2 points
           from the top of the next ensemble to the bottom of the
           current.  Zeros are padded in the upper-left and lower-right
           corners of the matrix (beginning/end of timeseries).  In
           this case, the array shape will be (...,`n`,`n_pad`+`n_bin`)
         n_bin : int (default: self.n_bin)
           Override this binner's n_bin.
 
         Returns
         -------
         out : numpy.ndarray
+          Data in reshaped format, where the last axis is of length 
+          `int(n_bin)`.
 
         Notes
         -----
         `n_bin` can be non-integer, in which case the output array
         size will be `n_pad`+`n_bin`, and the decimal will
         cause skipping of some data points in `arr`.  In particular,
         every mod(`n_bin`,1) bins will have a skipped point. For
         example:
         - for n_bin=2048.2 every 1/5 bins will have a skipped point.
         - for n_bin=4096.9 every 9/10 bins will have a skipped point.
         """
 
         n_bin = self._parse_nbin(n_bin)
+        if arr.shape[-1] < n_bin:
+            raise Exception('n_bin is larger than length of input array')
         npd0 = int(n_pad // 2)
         npd1 = int((n_pad + 1) // 2)
         shp = self._outshape(arr.shape, n_pad=0, n_bin=n_bin)
         out = np.zeros(
             self._outshape(arr.shape, n_pad=n_pad, n_bin=n_bin),
             dtype=arr.dtype)
         if np.mod(n_bin, 1) == 0:
@@ -195,14 +208,19 @@
             n_bin = int(n_bin)
             # If n_bin is an integer, we can do this simply.
             out[..., npd0: n_bin + npd0] = (
                 arr[..., :(shp[-2] * shp[-1])]).reshape(shp, order='C')
         else:
             inds = (np.arange(np.prod(shp[-2:])) * n_bin // int(n_bin)
                     ).astype(int)
+            # If there are too many indices, drop one bin
+            if inds[-1] >= arr.shape[-1]:
+                inds = inds[:-int(n_bin)]
+                shp[-2] -= 1
+                out = out[..., 1:, :]
             n_bin = int(n_bin)
             out[..., npd0:n_bin + npd0] = (arr[..., inds]
                                            ).reshape(shp, order='C')
             n_bin = int(n_bin)
         if n_pad != 0:
             out[..., 1:, :npd0] = out[..., :-1, n_bin:n_bin + npd0]
             out[..., :-1, -npd1:] = out[..., 1:, npd0:npd0 + npd1]
@@ -212,14 +230,15 @@
     def detrend(self, arr, axis=-1, n_pad=0, n_bin=None):
         """Reshape the array `arr` to shape (...,n,n_bin+n_pad)
         and remove the best-fit trend line from each bin.
 
         Parameters
         ----------
         arr : numpy.ndarray
+          Input data
         axis : int (default: -1)
           Axis along which to take mean
         n_pad : int (default: 0)
           Is used to add `n_pad`/2 points from the end of the previous
           ensemble to the top of the current, and `n_pad`/2 points
           from the top of the next ensemble to the bottom of the
           current.  Zeros are padded in the upper-left and lower-right
@@ -227,25 +246,27 @@
           this case, the array shape will be (...,`n`,`n_pad`+`n_bin`)
         n_bin : int (default: self.n_bin)
           Override this binner's n_bin.
 
         Returns
         -------
         out : numpy.ndarray
+          Detrended data, where the last axis is of length `int(n_bin)`.
         """
 
         return detrend(self.reshape(arr, n_pad=n_pad, n_bin=n_bin), axis=axis)
 
     def demean(self, arr, axis=-1, n_pad=0, n_bin=None):
         """Reshape the array `arr` to shape (...,n,n_bin+n_pad)
         and remove the mean from each bin.
 
         Parameters
         ----------
         arr : numpy.ndarray
+          Input data
         axis : int (default: -1)
           Axis along which to take mean
         n_pad : int (default: 0)
           Is used to add `n_pad`/2 points from the end of the previous
           ensemble to the top of the current, and `n_pad`/2 points
           from the top of the next ensemble to the bottom of the
           current.  Zeros are padded in the upper-left and lower-right
@@ -253,83 +274,86 @@
           this case, the array shape will be (...,`n`,`n_pad`+`n_bin`)
         n_bin : int (default: self.n_bin)
           Override this binner's n_bin.
 
         Returns
         -------
         out : numpy.ndarray
+          Demeaned data, where the last axis is of length `int(n_bin)`.
         """
 
         dt = self.reshape(arr, n_pad=n_pad, n_bin=n_bin)
         return dt - np.nanmean(dt, axis)[..., None]
 
     def mean(self, arr, axis=-1, n_bin=None):
         """Reshape the array `arr` to shape (...,n,n_bin+n_pad)
         and take the mean of each bin along the specified `axis`.
 
         Parameters
         ----------
         arr : numpy.ndarray
+          Input data
         axis : int (default: -1)
           Axis along which to take mean
         n_bin : int (default: self.n_bin)
           Override this binner's n_bin.
 
         Returns
         -------
         out : numpy.ndarray
         """
 
         if np.issubdtype(arr.dtype, np.datetime64):
             return epoch2dt64(self.mean(dt642epoch(arr), axis=axis, n_bin=n_bin))
         if axis != -1:
             arr = np.swapaxes(arr, axis, -1)
-        n_bin = self._parse_nbin(n_bin)
         tmp = self.reshape(arr, n_bin=n_bin)
 
         return np.nanmean(tmp, -1)
 
     def var(self, arr, axis=-1, n_bin=None):
         """Reshape the array `arr` to shape (...,n,n_bin+n_pad)
         and take the variance of each bin along the specified `axis`.
 
         Parameters
         ----------
         arr : numpy.ndarray
+          Input data
         axis : int (default: -1)
           Axis along which to take variance
         n_bin : int (default: self.n_bin)
           Override this binner's n_bin.
 
         Returns
         -------
         out : numpy.ndarray
         """
 
-        return self.reshape(arr, n_bin=n_bin).var(axis)
+        return np.nanvar(self.reshape(arr, n_bin=n_bin), axis=axis, dtype=np.float32)
 
     def std(self, arr, axis=-1, n_bin=None):
         """Reshape the array `arr` to shape (...,n,n_bin+n_pad)
         and take the standard deviation of each bin along the 
         specified `axis`.
 
         Parameters
         ----------
         arr : numpy.ndarray
+          Input data
         axis : int (default: -1)
           Axis along which to take std dev
         n_bin : int (default: self.n_bin)
           Override this binner's n_bin.
 
         Returns
         -------
         out : numpy.ndarray
         """
 
-        return self.reshape(arr, n_bin=n_bin).std(axis)
+        return np.nanstd(self.reshape(arr, n_bin=n_bin), axis=axis, dtype=np.float32)
 
     def calc_psd_base(self, dat, fs=None, window='hann', noise=0,
                       n_bin=None, n_fft=None, n_pad=None, step=None):
         """Calculate power spectral density of `dat`
 
         Parameters
         ----------
```

### Comparing `dolfyn-1.2.1/dolfyn/io/api.py` & `dolfyn-1.3.0/dolfyn/io/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,33 +159,27 @@
     'encoding' in kwargs. The values in encoding will take precedence
     over whatever is set according to the compression option above.
     See the xarray.to_netcdf documentation for more details.
     """
 
     filename = _check_file_ext(filename, 'nc')
 
-    # Dropping the detailed configuration stats because netcdf can't save it
-    for key in list(ds.attrs.keys()):
-        if 'config' in key:
-            ds.attrs.pop(key)
-
     # Handling complex values for netCDF4
     ds.attrs['complex_vars'] = []
     for var in ds.data_vars:
         if np.iscomplexobj(ds[var]):
             ds[var+'_real'] = ds[var].real
             ds[var+'_imag'] = ds[var].imag
 
             ds = ds.drop_vars(var)
             ds.attrs['complex_vars'].append(var)
 
-    # For variables that get rewritten to float64
-    for v in ds.data_vars:
-        ds[v].encoding = {}
-        ds[v] = ds[v].astype('float32')
+        # For variables that get rewritten to float64
+        elif ds[var].dtype == np.float64:
+            ds[var] = ds[var].astype('float32')
 
     if compression:
         enc = dict()
         for ky in ds.variables:
             enc[ky] = dict(zlib=True, complevel=1)
         if 'encoding' in kwargs:
             # Overwrite ('update') values in enc with whatever is in kwargs['encoding']
@@ -229,19 +223,14 @@
         if len(ds.complex_vars[0]) == 1:
             ds.attrs['complex_vars'] = [ds.complex_vars]
         for var in ds.complex_vars:
             ds[var] = ds[var+'_real'] + ds[var+'_imag'] * 1j
             ds = ds.drop_vars([var+'_real', var+'_imag'])
     ds.attrs.pop('complex_vars')
 
-    # Return units attribute for time
-    for variable in ds.variables.values():
-        if np.issubdtype(variable.data.dtype, np.datetime64):
-            variable.attrs["units"] = "seconds since 1970-01-01 00:00:00"
-
     return ds
 
 
 def save_mat(ds, filename, datenum=True):
     """Save xarray dataset as a MATLAB (.mat) file
 
     Parameters
```

### Comparing `dolfyn-1.2.1/dolfyn/io/base.py` & `dolfyn-1.3.0/dolfyn/io/base.py`

 * *Files identical despite different names*

### Comparing `dolfyn-1.2.1/dolfyn/io/nortek.py` & `dolfyn-1.3.0/dolfyn/io/nortek.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import warnings
 import logging
 import numpy as np
-import xarray as xr
 from struct import unpack
 from pathlib import Path
 from datetime import datetime
 
 from . import nortek_defs
 from .. import time
 from .base import _find_userdata, _create_dataset, _handle_nan, _abspath
@@ -417,16 +416,15 @@
             else:
                 sz = 2 * unpack(self.endian + 'H', self.read(2))[0]
                 shift = sz - 4
             self.f.seek(shift, 1)
         return self.pos
 
     def code_spacing(self, searchcode, iternum=50):
-        """
-        Find the spacing, in bytes, between a specific hardware code.
+        """Find the spacing, in bytes, between a specific hardware code.
         Repeat this * iternum * times(default 50).
         Returns the average spacing, in bytes, between the code.
         """
         p0 = self.findnextid(searchcode)
         for i in range(iternum):
             try:
                 self.findnextid(searchcode)
@@ -593,16 +591,16 @@
         """Initialize the data object according to vardict.
 
         Parameters
         ----------
         vardict : (dict of :class:`<VarAttrs>`)
           The variable definitions in the :class:`<VarAttrs>` specify
           how to initialize each data variable.
-
         """
+
         shape_args = {'n': self.n_samp_guess}
         try:
             shape_args['nbins'] = self.config['usr']['n_bins']
         except KeyError:
             pass
         for nm, va in list(vardict.items()):
             if va.group is None:
```

### Comparing `dolfyn-1.2.1/dolfyn/io/nortek2.py` & `dolfyn-1.3.0/dolfyn/io/nortek2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
-import xarray as xr
 from struct import unpack, calcsize
 import warnings
 from pathlib import Path
 import logging
+import json
 
 from . import nortek2_defs as defs
 from . import nortek2_lib as lib
 from .base import _find_userdata, _create_dataset, _abspath
 from ..rotate.vector import _euler2orient
 from ..rotate.base import _set_coords
 from ..rotate.api import set_declination
@@ -97,14 +97,19 @@
     if 'orientmat' not in ds:
         ds['orientmat'] = _euler2orient(
             ds['time'], ds['heading'], ds['pitch'], ds['roll'])
 
     if declin is not None:
         set_declination(ds, declin, inplace=True)
 
+    # Convert config dictionary to json string
+    for key in list(ds.attrs.keys()):
+        if 'config' in key:
+            ds.attrs[key] = json.dumps(ds.attrs[key])
+
     # Close handler
     if debug:
         for handler in logging.root.handlers[:]:
             logging.root.removeHandler(handler)
             handler.close()
 
     return ds
@@ -565,14 +570,17 @@
         da['has_imu'] = 1  # logical
         # Signature AHRS rotation matrix returned in "inst->earth"
         # Change to dolfyn's "earth->inst"
         dv['orientmat'] = np.rollaxis(dv['orientmat'], 1)
     else:
         da['has_imu'] = 0
 
-    da['fs'] = da['filehead_config']['BURST'].pop('SR')
-    tmat = da['filehead_config'].pop('XFBURST')
+    da['fs'] = da['filehead_config']['BURST']['SR']
+    theta = da['filehead_config']['BEAMCFGLIST'][0]
+    if 'THETA=' in theta:
+        da['beam_angle'] = int(theta[13:15])
+    tmat = da['filehead_config']['XFBURST']
     tm = np.zeros((tmat['ROWS'], tmat['COLS']), dtype=np.float32)
     for irow in range(tmat['ROWS']):
         for icol in range(tmat['COLS']):
             tm[irow, icol] = tmat['M' + str(irow + 1) + str(icol + 1)]
     dv['beam2inst_orientmat'] = tm
```

### Comparing `dolfyn-1.2.1/dolfyn/io/nortek2_defs.py` & `dolfyn-1.3.0/dolfyn/io/nortek2_defs.py`

 * *Files identical despite different names*

### Comparing `dolfyn-1.2.1/dolfyn/io/nortek2_lib.py` & `dolfyn-1.3.0/dolfyn/io/nortek2_lib.py`

 * *Files identical despite different names*

### Comparing `dolfyn-1.2.1/dolfyn/io/nortek_defs.py` & `dolfyn-1.3.0/dolfyn/io/nortek_defs.py`

 * *Files identical despite different names*

### Comparing `dolfyn-1.2.1/dolfyn/io/rdi.py` & `dolfyn-1.3.0/dolfyn/io/rdi.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 from ..rotate.rdi import _calc_beam_orientmat, _calc_orientmat
 from ..rotate.base import _set_coords
 from ..rotate.api import set_declination
 
 
 def read_rdi(filename, userdata=None, nens=None, debug_level=-1,
              vmdas_search=False, winriver=False, **kwargs):
-    """
-    Read a TRDI binary data file.
+    """Read a TRDI binary data file.
 
     Parameters
     ----------
     filename : string
       Filename of TRDI file to read.
     userdata : True, False, or string of userdata.json filename (default ``True``)
       Whether to read the '<base-filename>.userdata.json' file.
@@ -37,16 +36,16 @@
       If file is winriver or not. Automatically set by dolfyn, this is helpful 
       for debugging
 
     Returns
     -------
     ds : xarray.Dataset
       An xarray dataset from the binary instrument data
-
     """
+
     # Start debugger logging
     if debug_level >= 0:
         for handler in logging.root.handlers[:]:
             logging.root.removeHandler(handler)
         filepath = Path(filename)
         logfile = filepath.with_suffix('.log')
         logging.basicConfig(filename=str(logfile),
@@ -128,16 +127,15 @@
             logging.root.removeHandler(handler)
             handler.close()
 
     return dss[0]
 
 
 def _remove_gps_duplicates(dat):
-    """
-    Removes duplicate and nan timestamp values in 'time_gps' coordinate,
+    """Removes duplicate and nan timestamp values in 'time_gps' coordinate,
     and add hardware (ADCP DAQ) timestamp corresponding to GPS acquisition
     (in addition to the GPS unit's timestamp).
     """
 
     dat['data_vars']['hdwtime_gps'] = dat['coords']['time']
 
     # Remove duplicate timestamp values, if applicable
@@ -155,16 +153,15 @@
             if sum(nan) > 0:
                 dat['data_vars'][key] = dat['data_vars'][key][~nan]
 
     return dat
 
 
 def _set_rdi_declination(dat, fname, inplace):
-    """
-    If magnetic_var_deg is set, this means that the declination is already
+    """If magnetic_var_deg is set, this means that the declination is already
     included in the heading and in the velocity data.
     """
 
     declin = dat.attrs.pop('declination', None)  # userdata declination
 
     if dat.attrs['magnetic_var_deg'] != 0:  # from TRDI software if set
         dat.attrs['declination'] = dat.attrs['magnetic_var_deg']
@@ -485,16 +482,15 @@
             offset = hdr['nbyte'] + 2 - readbytes
             self.check_offset(offset, readbytes)
             self.print_pos(byte_offset=byte_offset)
 
         return True
 
     def search_buffer(self):
-        """
-        Check to see if the next bytes indicate the beginning of a
+        """Check to see if the next bytes indicate the beginning of a
         data block.  If not, search for the next data block, up to
         _search_num times.
         """
         id = self.f.read_ui8(2)
         if id is None:
             return False
         id1 = list(id)
@@ -1071,14 +1067,17 @@
                            'latitude_gps',
                            'longitude_gps',
                            'avg_speed_gps',
                            'avg_dir_gps',
                            'speed_made_good_gps',
                            'dir_made_good_gps',
                            'flags_gps',
+                           'pitch_gps',
+                           'roll_gps',
+                           'heading_gps',
                            ]
         # UTC date time
         utim = fd.read_ui8(4)
         date_utc = tmlib.datetime(utim[2] + utim[3] * 256, utim[1], utim[0])
 
         # 1st lat/lon position after previous ADCP ping
         # This byte is in hundredths of seconds (10s of milliseconds):
@@ -1107,15 +1106,19 @@
 
         # ADCP date time
         utim = fd.read_ui8(4)
         date_adcp = tmlib.datetime(utim[0] + utim[1] * 256, utim[3], utim[2])
         time_adcp = tmlib.timedelta(
             milliseconds=(int(fd.read_ui32(1) / 10)))
 
-        fd.seek(16, 1)
+        ens.pitch_gps[k] = fd.read_ui16(1) * 180 / 2 ** 15
+        ens.roll_gps[k] = fd.read_ui16(1) * 180 / 2 ** 15
+        ens.heading_gps[k] = fd.read_ui16(1) * 180 / 2 ** 15
+
+        fd.seek(10, 1)
         self._nbyte = 2 + 76
 
         if self._debug_level >= 0:
             logging.info('Read VMDAS')
         self._read_vmdas = True
 
     def read_winriver2(self, ):
```

### Comparing `dolfyn-1.2.1/dolfyn/io/rdi_defs.py` & `dolfyn-1.3.0/dolfyn/io/rdi_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,17 @@
              'fix_gps': ([], 'data_vars', 'int8', '1', 'GPS Fix', 'gps_fix_type'),
              'n_sat_gps': ([], 'data_vars', 'int8', 'count', 'Number of Satellites', 'number_of_satellites'),
              'hdop_gps': ([], 'data_vars', 'float32', '1', 'HDOP', 'horizontal_dilution_of_precision'),
              'elevation_gps': ([], 'data_vars', 'float32', 'm', 'Elevation', 'elevation_above_MLLW'),
              'rtk_age_gps': ([], 'data_vars', 'float32', 's', 'RTK Age', 'age_of_received_real_time_kinetic_signal'),
              'speed_over_grnd_gps': ([], 'data_vars', 'float32', 'm s-1', 'Platform Speed', 'platform_speed_wrt_ground'),
              'dir_over_grnd_gps': ([], 'data_vars', 'float32', 'degree', 'Platform Direction', 'platform_course'),
-             'heading_gps': ([], 'data_vars', 'float64', 'degree', 'GPS Heading', 'platform_course'),
+             'heading_gps': ([], 'data_vars', 'float32', 'degree', 'GPS Heading', 'platform_orientation'),
+             'pitch_gps': ([], 'data_vars', 'float32', 'degree', 'GPS Pitch', 'platform_pitch'),
+             'roll_gps': ([], 'data_vars', 'float32', 'degree', 'GPS Roll', 'platform_roll'),
              'dist_nmea': ([], 'data_vars', 'float32', 'm', 'Depth', 'depth_sounder_range'),
              'vel_sl': (['nc', 4], 'data_vars', 'float32', 'm s-1', 'Water Velocity',
                         'velocity_from_multibeam_acoustic_doppler_velocity_profiler_in_sea_water'),
              'corr_sl': (['nc', 4], 'data_vars', 'uint8', 'counts', 'Acoustic Signal Correlation',
                          'beam_consistency_indicator_from_multibeam_acoustic_doppler_velocity_profiler_in_sea_water'),
              'amp_sl': (['nc', 4], 'data_vars', 'uint8', 'counts', 'Acoustic Signal Amplitude',
                         'signal_intensity_from_multibeam_acoustic_doppler_velocity_profiler_in_sea_water'),
```

### Comparing `dolfyn-1.2.1/dolfyn/io/rdi_lib.py` & `dolfyn-1.3.0/dolfyn/io/rdi_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
 from struct import unpack
 from os.path import expanduser
 
 
 class bin_reader():
-    """
-    Reads binary data files. It is mostly for development purposes, to
+    """Reads binary data files. It is mostly for development purposes, to
     simplify learning a data file's format. Reading binary data files should
     minimize the number of calls to struct.unpack and file.read because many
     calls to these functions (i.e. using the code in this module) are slow.
     """
     _size_factor = {'B': 1, 'b': 1, 'H': 2,
                     'h': 2, 'L': 4, 'l': 4, 'f': 4, 'd': 8}
     _frmt = {np.uint8: 'B', np.int8: 'b',
@@ -26,16 +25,15 @@
     def __enter__(self,):
         return self
 
     def __exit__(self, type, value, traceback):
         self.close()
 
     def __init__(self, fname, endian='<', checksum_size=None, debug_level=0):
-        """
-        Default to little-endian '<'...
+        """Default to little-endian '<'...
         *checksum_size* is in bytes, if it is None or False, this
          function does not perform checksums.
         """
         self.endian = endian
         self.f = open(expanduser(fname), 'rb')
         self.f.seek(0, 2)
         self.fsize = self.tell()
@@ -61,16 +59,15 @@
     def tell(self,):
         return self.f.tell()
 
     def seek(self, pos, rel=1):
         return self.f.seek(pos, rel)
 
     def reads(self, n):
-        """
-        Read a string of n characters.
+        """Read a string of n characters.
         """
         val = self.f.read(n)
         self.cs and self.cs.add(val)
         try:
             val = val.decode('utf-8')
         except:
             if self.debug_level > 5:
@@ -111,15 +108,15 @@
 
     def read_ui32(self, n):
         return self.read(n, 'L')
 
     def read_i32(self, n):
         return self.read(n, 'l')
 
-#ics = 0  # This is a holder for the checksum index
+# ics = 0  # This is a holder for the checksum index
 # class checksum():
 #     # Checksum for TRDI
 #     def __init__(self, file, val, size, error_behavior='exception'):
 #         """
 #         Value *val* to initialize the checksum with,
 #         and the *size* of the checksum (in bytes, currently this can only be 1,2,4 or 8).
 #         """
```

### Comparing `dolfyn-1.2.1/dolfyn/rotate/api.py` & `dolfyn-1.3.0/dolfyn/rotate/api.py`

 * *Files identical despite different names*

### Comparing `dolfyn-1.2.1/dolfyn/rotate/base.py` & `dolfyn-1.3.0/dolfyn/rotate/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import xarray as xr
 from numpy.linalg import det, inv
 from scipy.spatial.transform import Rotation as R
+import warnings
 
 
 def _make_model(ds):
     """The make and model of the instrument that collected the data
     in this data object.
     """
     return '{} {}'.format(ds.attrs['inst_make'],
@@ -20,26 +21,37 @@
     Returns a boolean array.
     """
 
     if rotmat.ndim > 2:
         rotmat = np.transpose(rotmat)
     return np.abs(det(rotmat) - 1) < thresh
 
+def _check_rotate_vars(ds, rotate_vars):
+    if rotate_vars is None:
+        if 'rotate_vars' in ds.attrs:
+            rotate_vars = ds.rotate_vars
+        else:
+            warnings.warn("    'rotate_vars' attribute not found."
+                          "Rotating `vel`.")
+            rotate_vars = ['vel']
+
+    return rotate_vars
+
 
 def _set_coords(ds, ref_frame, forced=False):
     """Checks the current reference frame and adjusts xarray coords/dims 
     as necessary.
     Makes sure assigned dataarray coordinates match what DOLfYN is reading in.
     """
 
     make = _make_model(ds)
 
     XYZ = ['X', 'Y', 'Z']
     ENU = ['E', 'N', 'U']
-    beam = list(range(1, ds['vel'].shape[0]+1))
+    beam = ds.beam.values
     principal = ['streamwise', 'x-stream', 'vert']
 
     # check make/model
     if 'rdi' in make:
         inst = ['X', 'Y', 'Z', 'err']
         earth = ['E', 'N', 'U', 'err']
         princ = ['streamwise', 'x-stream', 'vert', 'err']
@@ -93,17 +105,17 @@
       The ADCP dataset
     reverse : bool (default: False)
       If True, this function performs the inverse rotation (inst->beam).
     force : bool (default: False), or list
       When true do not check which coordinate system the data is in
       prior to performing this rotation. When forced-rotations are
       applied, the string '-forced!' is appended to the
-      dat.props['coord_sys'] string. If force is a list, it contains
+      dat['coord_sys'] string. If force is a list, it contains
       a list of variables that should be rotated (rather than the
-      default values in adpo.props['rotate_vars']).
+      default values in adpo['rotate_vars']).
     """
 
     if not force:
         if not reverse and dat.coord_sys.lower() != 'beam':
             raise ValueError('The input must be in beam coordinates.')
         if reverse and dat.coord_sys != 'inst':
             raise ValueError('The input must be in inst coordinates.')
@@ -123,18 +135,15 @@
         # Can't use transpose because rotation is not between
         # orthogonal coordinate systems
         rotmat = inv(rotmat)
         cs = 'beam'
     for ky in rotate_vars:
         dat[ky].values = np.einsum('ij,j...->i...', rotmat, dat[ky].values)
 
-    if force:
-        dat = _set_coords(dat, cs, forced=True)
-    else:
-        dat = _set_coords(dat, cs)
+    dat = _set_coords(dat, cs)
 
     return dat
 
 
 def euler2orient(heading, pitch, roll, units='degrees'):
     """Calculate the orientation matrix from DOLfYN-defined euler angles.
 
@@ -295,7 +304,35 @@
     omat.values = np.rollaxis(omat.values, 1)
 
     earth = xr.DataArray(['E', 'N', 'U'], dims=['earth'], name='earth', attrs={
         'units': '1', 'long_name': 'Earth Reference Frame', 'coverage_content_type': 'coordinate'})
     inst = xr.DataArray(['X', 'Y', 'Z'], dims=['inst'], name='inst', attrs={
         'units': '1', 'long_name': 'Instrument Reference Frame', 'coverage_content_type': 'coordinate'})
     return omat.assign_coords({'earth': earth, 'inst': inst, 'time': quaternions.time})
+
+
+def calc_tilt(pitch, roll):
+    """Calculate "tilt", the vertical inclination, from pitch and roll.
+
+    Parameters
+    ----------
+    roll : numpy.ndarray or xarray.DataArray
+      Instrument roll
+    pitch : numpy.ndarray or xarray.DataArray
+      Instrument pitch
+
+    Returns
+    -------
+    tilt : numpy.ndarray
+      Vertical inclination of the instrument
+    """
+
+    if 'xarray' in type(pitch).__module__:
+        pitch = pitch.values
+    if 'xarray' in type(roll).__module__:
+        roll = roll.values
+
+    tilt = np.arctan(
+        np.sqrt(np.tan(np.deg2rad(roll)) ** 2 + np.tan(np.deg2rad(pitch)) ** 2)
+    )
+
+    return np.rad2deg(tilt)
```

### Comparing `dolfyn-1.2.1/dolfyn/rotate/rdi.py` & `dolfyn-1.3.0/dolfyn/rotate/rdi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import numpy as np
 import xarray as xr
 from .vector import _earth2principal
-from .base import _beam2inst, _set_coords
+from .base import _beam2inst, _set_coords, _check_rotate_vars
 
 
-def _inst2earth(adcpo, reverse=False, force=False):
+def _inst2earth(adcpo, reverse=False, rotate_vars=None, force=False):
     """Rotate velocities from the instrument to earth coordinates.
 
     This function also rotates data from the 'ship' frame, into the
     earth frame when it is in the ship frame (and
     ``adcpo.use_pitchroll == 'yes'``). It does not support the
     'reverse' rotation back into the ship frame.
 
     Parameters
     ----------
     adcpo : xarray.Dataset
       The adcp dataset containing the data.
     reverse : bool (default: False)
       If True, this function performs the inverse rotation (earth->inst).
+    rotate_vars : iterable (default: None, list in adcpo.rotate_vars)
+      The list of variables to rotate. By default this is taken from
+      adcpo.rotate_vars.
     force : bool (default: False)
       When true do not check which coordinate system the data is in
       prior to performing this rotation.
 
     Notes
     -----
     The rotation matrix is taken from the Teledyne RDI ADCP Coordinate
@@ -37,29 +40,31 @@
                          "coordinate system.".format(csin))
 
     if 'orientmat' in adcpo:
         omat = adcpo['orientmat']
     else:
         omat = _calc_orientmat(adcpo)
 
+    rotate_vars = _check_rotate_vars(adcpo, rotate_vars)
+
     # rollaxis gives transpose of orientation matrix.
     # The 'rotation matrix' is the transpose of the 'orientation matrix'
     # NOTE: the double 'rollaxis' within this function, and here, has
     # minimal computational impact because np.rollaxis returns a
     # view (not a new array)
     rotmat = np.rollaxis(omat.data, 1)
     if reverse:
         cs_new = 'inst'
         sumstr = 'jik,j...k->i...k'
     else:
         cs_new = 'earth'
         sumstr = 'ijk,j...k->i...k'
 
     # Only operate on the first 3-components, b/c the 4th is err_vel
-    for nm in adcpo.rotate_vars:
+    for nm in rotate_vars:
         dat = adcpo[nm].values
         dat[:3] = np.einsum(sumstr, rotmat, dat[:3])
         adcpo[nm].values = dat.copy()
 
     adcpo = _set_coords(adcpo, cs_new)
 
     return adcpo
```

### Comparing `dolfyn-1.2.1/dolfyn/rotate/signature.py` & `dolfyn-1.3.0/dolfyn/rotate/signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .vector import _earth2principal, _euler2orient
-from .base import _beam2inst
+from .base import _beam2inst, _check_rotate_vars
 from . import base as rotb
 import numpy as np
 import warnings
 from numpy.linalg import inv
 
 
 def _inst2earth(adcpo, reverse=False, rotate_vars=None, force=False):
@@ -37,19 +37,15 @@
 
     # if ADCP is upside down
     if adcpo.orientation == 'down':
         down = True
     else:  # orientation = 'up' or 'AHRS'
         down = False
 
-    if rotate_vars is None:
-        if 'rotate_vars' in adcpo.attrs:
-            rotate_vars = adcpo.rotate_vars
-        else:
-            rotate_vars = ['vel']
+    rotate_vars = _check_rotate_vars(adcpo, rotate_vars)
 
     cs = adcpo.coord_sys.lower()
     if not force:
         if cs == cs_new:
             print("Data is already in the '%s' coordinate system" % cs_new)
             return
         elif cs != cs_now:
@@ -90,15 +86,15 @@
     if reverse:
         # 3-element inverse handled by sumstr definition (transpose)
         rmd[4] = np.moveaxis(inv(np.moveaxis(rmd[4], -1, 0)), 0, -1)
 
     for nm in rotate_vars:
         dat = adcpo[nm].values
         n = dat.shape[0]
-        # Nortek documents sign change for upside-down instruments
+        # Nortek documents sign change for upside-down instruments (equiv to adding 180 deg to roll)
         if down:
             # This is equivalent to adding 180 degrees to roll axis in _calc_omat()
             sign = np.array([1, -1, -1, -1], ndmin=dat.ndim).T
             signIMU = np.array([1, -1, -1], ndmin=dat.ndim).T
             if not reverse:
                 if n == 3:
                     dat = np.einsum(sumstr, rmd[3], signIMU*dat)
```

### Comparing `dolfyn-1.2.1/dolfyn/rotate/vector.py` & `dolfyn-1.3.0/dolfyn/rotate/vector.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     ----------
     advo : xarray.Dataset
       The adv dataset containing the data.
     reverse : bool (default: False)
       If True, this function performs the inverse rotation (earth->inst).
     rotate_vars : iterable (default: None, list in advo.rotate_vars)
       The list of variables to rotate. By default this is taken from
-      advo.props['rotate_vars'].
+      advo.attrs['rotate_vars'].
     force : bool (default: False)
       Do not check which frame the data is in prior to performing 
       this rotation.
     """
 
     if reverse:  # earth->inst
         # The transpose of the rotation matrix gives the inverse
@@ -75,19 +75,15 @@
         cs_now = 'earth'
         cs_new = 'inst'
     else:  # inst->earth
         sumstr = 'ijk,j...k->i...k'
         cs_now = 'inst'
         cs_new = 'earth'
 
-    if rotate_vars is None:
-        if 'rotate_vars' in advo.attrs:
-            rotate_vars = advo.rotate_vars
-        else:
-            rotate_vars = ['vel']
+    rotate_vars = rotb._check_rotate_vars(advo, rotate_vars)
 
     cs = advo.coord_sys.lower()
     if not force:
         if cs == cs_new:
             print("Data is already in the '%s' coordinate system" % cs_new)
             return
         elif cs != cs_now:
@@ -122,15 +118,15 @@
         advo[nm].values = np.einsum(sumstr, rmat, advo[nm])
 
     advo = rotb._set_coords(advo, cs_new)
 
     return advo
 
 
-def _earth2principal(advo, reverse=False):
+def _earth2principal(advo, reverse=False, rotate_vars=None):
     """Rotate data in an ADV dataset to/from principal axes. Principal
     heading must be within the dataset.
 
     All data in the advo.attrs['rotate_vars'] list will be
     rotated by the principal heading, and also if the data objet has an
     orientation matrix (orientmat) it will be rotated so that it
     represents the orientation of the ADV in the principal
@@ -139,14 +135,17 @@
     Parameters
     ----------
     advo : xarray.Dataset
       The adv dataset containing the data.
     reverse : bool (default: False)
       If True, this function performs the inverse rotation
       (principal->earth).
+    rotate_vars : iterable (default: None, list in advo.rotate_vars)
+      The list of variables to rotate. By default this is taken from
+      advo.props['rotate_vars'].
     """
 
     # This is in degrees CW from North
     ang = np.deg2rad(90 - advo.principal_heading)
     # convert this to radians CCW from east (which is expected by
     # the rest of the function)
 
@@ -154,14 +153,16 @@
         cs_now = 'principal'
         cs_new = 'earth'
     else:
         ang *= -1
         cs_now = 'earth'
         cs_new = 'principal'
 
+    rotate_vars = rotb._check_rotate_vars(advo, rotate_vars)
+
     cs = advo.coord_sys.lower()
     if cs == cs_new:
         print('Data is already in the %s coordinate system' % cs_new)
         return
     elif cs != cs_now:
         raise ValueError(
             'Data must be in the {} frame '
@@ -170,15 +171,15 @@
     # Calculate the rotation matrix:
     cp, sp = np.cos(ang), np.sin(ang)
     rotmat = np.array([[cp, -sp, 0],
                        [sp, cp, 0],
                        [0, 0, 1]], dtype=np.float32)
 
     # Perform the rotation:
-    for nm in advo.rotate_vars:
+    for nm in rotate_vars:
         dat = advo[nm].values
         dat[:2] = np.einsum('ij,j...->i...', rotmat[:2, :2], dat[:2])
         advo[nm].values = dat.copy()
 
     # Finalize the output.
     advo = rotb._set_coords(advo, cs_new)
```

### Comparing `dolfyn-1.2.1/dolfyn/time.py` & `dolfyn-1.3.0/dolfyn/time.py`

 * *Files identical despite different names*

### Comparing `dolfyn-1.2.1/dolfyn/tools/misc.py` & `dolfyn-1.3.0/dolfyn/tools/misc.py`

 * *Files identical despite different names*

### Comparing `dolfyn-1.2.1/dolfyn/tools/psd.py` & `dolfyn-1.3.0/dolfyn/tools/psd.py`

 * *Files identical despite different names*

### Comparing `dolfyn-1.2.1/dolfyn/velocity.py` & `dolfyn-1.3.0/dolfyn/velocity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import xarray as xr
 from .binned import TimeBinner
 from .time import dt642epoch, dt642date
 from .rotate.api import rotate2, set_declination, set_inst2head_rotmat
 from .io.api import save
 from .tools.psd import coherence, phase_angle
-from .tools.misc import slice1d_along_axis
+from .tools.misc import slice1d_along_axis, convert_degrees
 
 
 @xr.register_dataset_accessor('velds')  # 'velocity dataset'
 class Velocity():
     """All ADCP and ADV xarray datasets wrap this base class.
     The turbulence-related attributes defined within this class 
     assume that the  ``'tke_vec'`` and ``'stress_vec'`` data entries are 
@@ -214,16 +214,15 @@
         # Specify which variable show up in this view here.
         # * indicates a wildcard
         # This list also sets the display order.
         # Only the first 12 matches are displayed.
         show_vars = ['time*', 'vel*', 'range', 'range_echo',
                      'orientmat', 'heading', 'pitch', 'roll',
                      'temp', 'press*', 'amp*', 'corr*',
-                     'accel', 'angrt', 'mag',
-                     'echo',
+                     'accel', 'angrt', 'mag', 'echo',
                      ]
         n = 0
         for v in show_vars:
             if n > 12:
                 break
             if v.endswith('*'):
                 v = v[:-1]  # Drop the '*'
@@ -267,43 +266,43 @@
         (self.attrs['coord_sys']), it is:
 
         - beam:      beam1
         - inst:      x
         - earth:     east
         - principal: streamwise
         """
-        return self.ds['vel'][0]
+        return self.ds['vel'][0].drop('dir')
 
     @property
     def v(self,):
         """The second velocity component.
 
         This is simply a shortcut to self['vel'][1]. Therefore,
         depending on the coordinate system of the data object
         (self.attrs['coord_sys']), it is:
 
         - beam:      beam2
         - inst:      y
         - earth:     north
         - principal: cross-stream
         """
-        return self.ds['vel'][1]
+        return self.ds['vel'][1].drop('dir')
 
     @property
     def w(self,):
         """The third velocity component.
         This is simply a shortcut to self['vel'][2]. Therefore,
         depending on the coordinate system of the data object
         (self.attrs['coord_sys']), it is:
         - beam:      beam3
         - inst:      z
         - earth:     up
         - principal: up
         """
-        return self.ds['vel'][2]
+        return self.ds['vel'][2].drop('dir')
 
     @property
     def U(self,):
         """Horizontal velocity as a complex quantity
         """
         return xr.DataArray(
             (self.u + self.v * 1j).astype('complex64'),
@@ -318,25 +317,39 @@
             np.abs(self.U).astype('float32'),
             attrs={'units': 'm s-1',
                    'long_name': 'Water Speed',
                    'standard_name': 'sea_water_speed'})
 
     @property
     def U_dir(self,):
-        """Angle of horizontal velocity vector, in degrees counterclockwise 
-        from X/East/streamwise. Direction is 'to', as opposed to 'from'.
-        """
+        """Angle of horizontal velocity vector. Direction is 'to', 
+        as opposed to 'from'. This function calculates angle as 
+        "degrees CCW from X/East/streamwise" and then converts it to 
+        "degrees CW from X/North/streamwise".
+        """
+        def convert_to_CW(angle):
+            if self.ds.coord_sys == 'earth':
+                # Convert "deg CCW from East" to "deg CW from North" [0, 360]
+                angle = convert_degrees(angle, tidal_mode=False)
+                relative_to = self.ds.dir[1].values
+            else:
+                # Switch to clockwise and from [-180, 180] to [0, 360]
+                angle *= -1
+                angle[angle < 0] += 360
+                relative_to = self.ds.dir[0].values
+            return angle, relative_to
+
         # Convert from radians to degrees
-        angle = np.angle(self.U)*(180/np.pi)
+        angle, rel = convert_to_CW(np.angle(self.U)*(180/np.pi))
 
         return xr.DataArray(
             angle.astype('float32'),
             dims=self.U.dims,
             coords=self.U.coords,
-            attrs={'units': 'degree',
+            attrs={'units': 'degrees_CW_from_' + str(rel),
                    'long_name': 'Water Direction',
                    'standard_name': 'sea_water_to_direction'})
 
     @property
     def E_coh(self,):
         """Coherent turbulence energy
 
@@ -399,45 +412,45 @@
         tke.attrs['standard_name'] = 'specific_turbulent_kinetic_energy_of_sea_water'
         return tke
 
     @property
     def upvp_(self,):
         """u'v'bar Reynolds stress
         """
-        return self.ds['stress_vec'].sel(tau="upvp_")
+        return self.ds['stress_vec'].sel(tau="upvp_").drop('tau')
 
     @property
     def upwp_(self,):
         """u'w'bar Reynolds stress
         """
-        return self.ds['stress_vec'].sel(tau="upwp_")
+        return self.ds['stress_vec'].sel(tau="upwp_").drop('tau')
 
     @property
     def vpwp_(self,):
         """v'w'bar Reynolds stress
         """
-        return self.ds['stress_vec'].sel(tau="vpwp_")
+        return self.ds['stress_vec'].sel(tau="vpwp_").drop('tau')
 
     @property
     def upup_(self,):
         """u'u'bar component of the tke
         """
-        return self.ds['tke_vec'].sel(tke="upup_")
+        return self.ds['tke_vec'].sel(tke="upup_").drop('tke')
 
     @property
     def vpvp_(self,):
         """v'v'bar component of the tke
         """
-        return self.ds['tke_vec'].sel(tke="vpvp_")
+        return self.ds['tke_vec'].sel(tke="vpvp_").drop('tke')
 
     @property
     def wpwp_(self,):
         """w'w'bar component of the tke
         """
-        return self.ds['tke_vec'].sel(tke="wpwp_")
+        return self.ds['tke_vec'].sel(tke="wpwp_").drop('tke')
 
 
 class VelBinner(TimeBinner):
     """This is the base binning (averaging) tool.
     All |dlfn| binning tools derive from this base class.
 
     Examples
@@ -483,29 +496,27 @@
     C = xr.DataArray(['Cxy', 'Cxz', 'Cyz'],
                      dims=['C'],
                      name='C',
                      attrs={'units': '1',
                             'long_name': 'Cross-Spectral Density Vector Components',
                             'coverage_content_type': 'coordinate'})
 
-    def do_avg(self, raw_ds, out_ds=None, names=None, noise=[0, 0, 0]):
+    def do_avg(self, raw_ds, out_ds=None, names=None):
         """Bin the dataset and calculate the ensemble averages of each 
         variable.
 
         Parameters
         ----------
         raw_ds : xarray.Dataset
            The raw data structure to be binned
         out_ds : xarray.Dataset
            The bin'd (output) data object to which averaged data is added.
         names : list of strings
            The names of variables to be averaged.  If `names` is None,
            all data in `raw_ds` will be binned.
-        noise : list or numpy.ndarray
-          Instrument's doppler noise in same units as velocity
 
         Returns
         -------
         out_ds : xarray.Dataset
           The new (or updated when out_ds is not None) dataset
           with the averages of all the variables in raw_ds.
 
@@ -545,17 +556,15 @@
                                               coords=coords_dict,
                                               dims=dims_list,
                                               attrs=raw_ds[ky].attrs
                                               ).astype('float32')
                 except:  # variables not needing averaging
                     pass
             # Add standard deviation
-            std = (np.nanstd(self.reshape(raw_ds.velds.U_mag.values),
-                             axis=-1,
-                             dtype=np.float64) - (noise[0] + noise[1])/2)
+            std = self.std(raw_ds.velds.U_mag.values)
             out_ds['U_std'] = xr.DataArray(
                 std.astype('float32'),
                 dims=raw_ds.vel.dims[1:],
                 attrs={'units': 'm s-1',
                        'long_name': 'Water Velocity Standard Deviation',
                        'standard_name': 'sea_water_velocity_standard_deviation'})
 
@@ -906,85 +915,95 @@
         da = xr.DataArray(out.astype('float32'),
                           coords=coords_dict,
                           dims=dims_list)
         da['dt'].attrs['units'] = 'timestep'
 
         return da
 
-    def calc_tke(self, veldat, noise=[0, 0, 0], detrend=True):
+    def calc_tke(self, veldat, noise=None, detrend=True):
         """Calculate the turbulent kinetic energy (TKE) (variances 
         of u,v,w).
 
         Parameters
         ----------
         veldat : xarray.DataArray
-            Velocity data array from ADV or single beam from ADCP. 
-            The last dimension is assumed to be time.
-        noise : float
-            a three-element vector of the noise levels of the
-            velocity data for ach component of velocity.
+          Velocity data array from ADV or single beam from ADCP. 
+          The last dimension is assumed to be time.
+        noise : float or array-like
+          A vector of the noise levels of the velocity data with 
+          the same first dimension as the velocity vector.
         detrend : bool (default: False)
-            detrend the velocity data (True), or simply de-mean it
-            (False), prior to computing tke. Note: the psd routines
-            use detrend, so if you want to have the same amount of
-            variance here as there use ``detrend=True``.
+          Detrend the velocity data (True), or simply de-mean it
+          (False), prior to computing tke. Note: the psd routines
+          use detrend, so if you want to have the same amount of
+          variance here as there use ``detrend=True``.
 
         Returns
         -------
-        ds : xarray.DataArray
-            dataArray containing u'u'_, v'v'_ and w'w'_
+        tke_vec : xarray.DataArray
+          dataArray containing u'u'_, v'v'_ and w'w'_
         """
 
-        if 'dir' in veldat.dims:
-            # will error for ADCP 4-beam, but not for single beam
-            vel = veldat.values
-        else:  # for single beam input
+        if 'xarray' in type(veldat).__module__:
             vel = veldat.values
+        if 'xarray' in type(noise).__module__:
+            noise = noise.values
 
-        if detrend:
-            vel = self.detrend(vel)
-        else:
-            vel = self.demean(vel)
+        if len(np.shape(vel)) > 2:
+            raise Exception("This function is only valid for calculating TKE using "
+                            "velocity from an ADV or a single ADCP beam.")
 
-        if 'time_b5' in veldat.dims:
-            time = self.mean(veldat.time_b5.values)
+        # Calc TKE
+        if detrend:
+            out = np.nanmean(self.detrend(vel)**2, axis=-1)
         else:
-            time = self.mean(veldat.time.values)
-
-        out = np.nanmean(vel**2, -1,
-                         dtype=np.float64,
-                         ).astype('float32')
-
-        out[0] -= noise[0] ** 2
-        out[1] -= noise[1] ** 2
-        out[2] -= noise[2] ** 2
-
-        da = xr.DataArray(out.astype('float32'),
-                          dims=veldat.dims,
-                          attrs={'units': 'm2 s-2',
-                                 'long_name': 'TKE Vector',
-                                 'standard_name': 'specific_turbulent_kinetic_energy_of_sea_water'})
+            out = np.nanmean(self.demean(vel)**2, axis=-1)
 
         if 'dir' in veldat.dims:
-            da = da.rename({'dir': 'tke'})
-            da = da.assign_coords({'tke': self.tke,
-                                   'time': time})
+            # Subtract noise
+            if noise is not None:
+                if np.shape(noise)[0] != 3:
+                    raise Exception(
+                        'Noise should have same first dimension as velocity')
+                out[0] -= noise[0] ** 2
+                out[1] -= noise[1] ** 2
+                out[2] -= noise[2] ** 2
+            # Set coords
+            dims = ['tke', 'time']
+            coords = {'tke': self.tke,
+                      'time': self.mean(veldat.time.values)}
         else:
-            if 'time_b5' in veldat.dims:
-                da = da.assign_coords({'time_b5': time})
-            else:
-                da = da.assign_coords({'time': time})
+            # Subtract noise
+            if noise is not None:
+                if np.shape(noise) > np.shape(vel):
+                    raise Exception(
+                        'Noise should have same or fewer dimensions as velocity')
+                out -= noise ** 2
+            # Set coords
+            dims = veldat.dims
+            coords = {}
+            for nm in veldat.dims:
+                if 'time' in nm:
+                    coords[nm] = self.mean(veldat[nm].values)
+                else:
+                    coords[nm] = veldat[nm].values
 
-        return da
+        return xr.DataArray(
+            out.astype('float32'),
+            dims=dims,
+            coords=coords,
+            attrs={'units': 'm2 s-2',
+                   'long_name': 'TKE Vector',
+                   'standard_name': 'specific_turbulent_kinetic_energy_of_sea_water'})
 
     def calc_psd(self, veldat,
                  freq_units='rad/s',
                  fs=None,
                  window='hann',
-                 noise=[0, 0, 0],
+                 noise=None,
                  n_bin=None, n_fft=None, n_pad=None,
                  step=None):
         """Calculate the power spectral density of velocity.
 
         Parameters
         ----------
         veldat : xr.DataArray
@@ -993,17 +1012,17 @@
           Frequency units of the returned spectra in either Hz or rad/s 
           (`f` or :math:`\\omega`)
         fs : float (optional)
           The sample rate (default: from the binner).
         window : string or array
           Specify the window function.
           Options: 1, None, 'hann', 'hamm'
-        noise : list(3 floats) (optional)
-          Noise level of each component's velocity measurement
-          (default 0).
+        noise : float or array-like
+          A vector of the noise levels of the velocity data with 
+          the same first dimension as the velocity vector.
         n_bin : int (optional)
           The bin-size (default: from the binner).
         n_fft : int (optional)
           The fft size (default: from the binner).
         n_pad : int (optional)
           The number of values to pad with zero (default: 0)
         step : int (optional)
@@ -1013,69 +1032,81 @@
 
         Returns
         -------
         psd : xarray.DataArray (3, M, N_FFT)
           The spectra in the 'u', 'v', and 'w' directions.
         """
 
-        if 'time_b5' in veldat.dims:
-            time = self.mean(veldat.time_b5.values)
-            time_str = 'time_b5'
-        else:
-            time = self.mean(veldat.time.values)
-            time_str = 'time'
-        fs = self._parse_fs(fs)
+        fs_in = self._parse_fs(fs)
         n_fft = self._parse_nfft(n_fft)
-        veldat = veldat.values
+        if 'xarray' in type(veldat).__module__:
+            vel = veldat.values
+        if 'xarray' in type(noise).__module__:
+            noise = noise.values
 
         # Create frequency vector, also checks whether using f or omega
         if 'rad' in freq_units:
-            fs = 2*np.pi*fs
+            fs = 2*np.pi*fs_in
             freq_units = 'rad s-1'
             units = 'm2 s-1 rad-1'
         else:
+            fs = fs_in
             freq_units = 'Hz'
             units = 'm2 s-2 Hz-1'
-        freq = xr.DataArray(self.calc_freq(units=freq_units),
+        freq = xr.DataArray(self.calc_freq(fs=fs_in, units=freq_units, n_fft=n_fft),
                             dims=['freq'],
                             name='freq',
                             attrs={'units': freq_units,
                                    'long_name': 'FFT Frequency Vector',
                                    'coverage_content_type': 'coordinate'}
                             ).astype('float32')
 
         # Spectra, if input is full velocity or a single array
-        if len(veldat.shape) == 2:
-            assert veldat.shape[0] == 3, "Function can only handle 1D or 3D arrays." \
+        if len(vel.shape) == 2:
+            assert vel.shape[0] == 3, "Function can only handle 1D or 3D arrays." \
                 " If ADCP data, please select a specific depth bin."
-            out = np.empty(self._outshape_fft(
-                veldat[:3].shape), dtype=np.float32)
+            if (noise is not None) and (np.shape(noise)[0] != 3):
+                raise Exception(
+                    'Noise should have same first dimension as velocity')
+            else:
+                noise = np.array([0, 0, 0])
+            out = np.empty(self._outshape_fft(vel[:3].shape, n_fft=n_fft, n_bin=n_bin),
+                           dtype=np.float32)
             for idx in range(3):
-                out[idx] = self.calc_psd_base(veldat[idx],
+                out[idx] = self.calc_psd_base(vel[idx],
                                               fs=fs,
                                               noise=noise[idx],
                                               window=window,
                                               n_bin=n_bin,
                                               n_pad=n_pad,
                                               n_fft=n_fft,
                                               step=step)
-            coords = {'S': self.S, time_str: time, 'freq': freq}
-            dims = ['S', time_str, 'freq']
+            coords = {'S': self.S,
+                      'time': self.mean(veldat['time'].values),
+                      'freq': freq}
+            dims = ['S', 'time', 'freq']
         else:
-            out = self.calc_psd_base(veldat,
+            if (noise is not None) and (len(np.shape(noise)) > 1):
+                raise Exception(
+                    'Noise should have same first dimension as velocity')
+            else:
+                noise = np.array(0)
+            out = self.calc_psd_base(vel,
                                      fs=fs,
-                                     noise=noise[0],
+                                     noise=noise,
                                      window=window,
                                      n_bin=n_bin,
                                      n_pad=n_pad,
                                      n_fft=n_fft,
                                      step=step)
-            coords = {time_str: time, 'freq': freq}
-            dims = [time_str, 'freq']
+            coords = {veldat.dims[-1]: self.mean(veldat[veldat.dims[-1]].values),
+                      'freq': freq}
+            dims = [veldat.dims[-1], 'freq']
 
-        return xr.DataArray(out.astype('float32'),
-                            coords=coords,
-                            dims=dims,
-                            attrs={'units': units,
-                                   'n_fft': n_fft,
-                                   'long_name': 'Power Spectral Density',
-                                   'standard_name': 'power_spectral_density_of_sea_water_velocity'})
+        return xr.DataArray(
+            out.astype('float32'),
+            coords=coords,
+            dims=dims,
+            attrs={'units': units,
+                   'n_fft': n_fft,
+                   'long_name': 'Power Spectral Density',
+                   'standard_name': 'power_spectral_density_of_sea_water_velocity'})
```

### Comparing `dolfyn-1.2.1/dolfyn.egg-info/SOURCES.txt` & `dolfyn-1.3.0/dolfyn.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 dolfyn.egg-info/SOURCES.txt
 dolfyn.egg-info/dependency_links.txt
 dolfyn.egg-info/requires.txt
 dolfyn.egg-info/top_level.txt
 dolfyn/adp/__init__.py
 dolfyn/adp/api.py
 dolfyn/adp/clean.py
+dolfyn/adp/turbulence.py
 dolfyn/adv/__init__.py
 dolfyn/adv/api.py
 dolfyn/adv/clean.py
 dolfyn/adv/motion.py
 dolfyn/adv/turbulence.py
 dolfyn/example_data/__init__.py
 dolfyn/io/__init__.py
```

### Comparing `dolfyn-1.2.1/scripts/binary2mat.py` & `dolfyn-1.3.0/scripts/binary2mat.py`

 * *Files identical despite different names*

### Comparing `dolfyn-1.2.1/scripts/motcorrect_vector.py` & `dolfyn-1.3.0/scripts/motcorrect_vector.py`

 * *Files identical despite different names*

### Comparing `dolfyn-1.2.1/setup.py` & `dolfyn-1.3.0/setup.py`

 * *Files identical despite different names*

