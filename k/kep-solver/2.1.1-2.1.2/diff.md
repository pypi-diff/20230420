# Comparing `tmp/kep_solver-2.1.1.tar.gz` & `tmp/kep_solver-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kep_solver-2.1.1.tar", last modified: Tue Nov 22 09:51:08 2022, max compression
+gzip compressed data, was "kep_solver-2.1.2.tar", last modified: Thu Apr 20 14:39:08 2023, max compression
```

## Comparing `kep_solver-2.1.1.tar` & `kep_solver-2.1.2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 09:51:08.828848 kep_solver-2.1.1/
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-11-22 09:50:58.000000 kep_solver-2.1.1/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       53 2022-11-22 09:50:58.000000 kep_solver-2.1.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1252 2022-11-22 09:50:58.000000 kep_solver-2.1.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      232 2022-11-22 09:50:58.000000 kep_solver-2.1.1/.readthedocs.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4097 2022-11-22 09:50:58.000000 kep_solver-2.1.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     8779 2022-11-22 09:50:58.000000 kep_solver-2.1.1/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)    34462 2022-11-22 09:50:58.000000 kep_solver-2.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5292 2022-11-22 09:51:08.828848 kep_solver-2.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4480 2022-11-22 09:50:58.000000 kep_solver-2.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 09:51:08.795845 kep_solver-2.1.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)       68 2022-11-22 09:50:58.000000 kep_solver-2.1.1/docs/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      634 2022-11-22 09:50:58.000000 kep_solver-2.1.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     2717 2022-11-22 09:50:58.000000 kep_solver-2.1.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2022-11-22 09:50:58.000000 kep_solver-2.1.1/docs/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 09:51:08.797679 kep_solver-2.1.1/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)    11080 2022-11-22 09:50:58.000000 kep_solver-2.1.1/docs/source/formats.rst
--rw-rw-rw-   0 root         (0) root         (0)     5405 2022-11-22 09:50:58.000000 kep_solver-2.1.1/docs/source/terms.rst
--rw-rw-rw-   0 root         (0) root         (0)     1685 2022-11-22 09:50:58.000000 kep_solver-2.1.1/docs/source/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 09:51:08.799512 kep_solver-2.1.1/kep_solver/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-22 09:50:58.000000 kep_solver-2.1.1/kep_solver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19271 2022-11-22 09:50:58.000000 kep_solver-2.1.1/kep_solver/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     9099 2022-11-22 09:50:58.000000 kep_solver-2.1.1/kep_solver/fileio.py
--rw-rw-rw-   0 root         (0) root         (0)    35788 2022-11-22 09:50:58.000000 kep_solver-2.1.1/kep_solver/generation.py
--rw-rw-rw-   0 root         (0) root         (0)    22946 2022-11-22 09:50:58.000000 kep_solver-2.1.1/kep_solver/graph.py
--rw-rw-rw-   0 root         (0) root         (0)    18245 2022-11-22 09:50:58.000000 kep_solver-2.1.1/kep_solver/model.py
--rw-rw-rw-   0 root         (0) root         (0)     7152 2022-11-22 09:50:58.000000 kep_solver-2.1.1/kep_solver/pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 09:51:08.800429 kep_solver-2.1.1/kep_solver.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5292 2022-11-22 09:51:08.000000 kep_solver-2.1.1/kep_solver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2815 2022-11-22 09:51:08.000000 kep_solver-2.1.1/kep_solver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 09:51:08.000000 kep_solver-2.1.1/kep_solver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2022-11-22 09:51:08.000000 kep_solver-2.1.1/kep_solver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-11-22 09:51:08.000000 kep_solver-2.1.1/kep_solver.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-11-22 09:50:58.000000 kep_solver-2.1.1/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 09:51:08.801345 kep_solver-2.1.1/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)     6159 2022-11-22 09:50:58.000000 kep_solver-2.1.1/notebooks/Match Run.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1485 2022-11-22 09:50:58.000000 kep_solver-2.1.1/notebooks/README.md
--rw-rw-rw-   0 root         (0) root         (0)    23889 2022-11-22 09:50:58.000000 kep_solver-2.1.1/notebooks/Statistical Analysis.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 09:51:08.802262 kep_solver-2.1.1/paper/
--rw-rw-rw-   0 root         (0) root         (0)     3189 2022-11-22 09:50:58.000000 kep_solver-2.1.1/paper/paper.bib
--rw-rw-rw-   0 root         (0) root         (0)     7233 2022-11-22 09:50:58.000000 kep_solver-2.1.1/paper/paper.md
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-11-22 09:50:58.000000 kep_solver-2.1.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-11-22 09:50:58.000000 kep_solver-2.1.1/runtime.txt
--rw-rw-rw-   0 root         (0) root         (0)     1056 2022-11-22 09:51:08.828848 kep_solver-2.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       83 2022-11-22 09:50:58.000000 kep_solver-2.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 09:51:08.804096 kep_solver-2.1.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4581 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_fileio.py
--rw-rw-rw-   0 root         (0) root         (0)    21534 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    16083 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 09:51:08.828848 kep_solver-2.1.1/tests/test_instances/
--rw-rw-rw-   0 root         (0) root         (0)   514090 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/large-1.json
--rw-rw-rw-   0 root         (0) root         (0)   590458 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/large-10.json
--rw-rw-rw-   0 root         (0) root         (0)   610079 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/large-2.json
--rw-rw-rw-   0 root         (0) root         (0)   590792 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/large-3.json
--rw-rw-rw-   0 root         (0) root         (0)   550366 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/large-4.json
--rw-rw-rw-   0 root         (0) root         (0)   575193 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/large-5.json
--rw-rw-rw-   0 root         (0) root         (0)   660843 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/large-6.json
--rw-rw-rw-   0 root         (0) root         (0)   665457 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/large-7.json
--rw-rw-rw-   0 root         (0) root         (0)   684308 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/large-8.json
--rw-rw-rw-   0 root         (0) root         (0)   686677 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/large-9.json
--rw-rw-rw-   0 root         (0) root         (0)    40468 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/medium-1.json
--rw-rw-rw-   0 root         (0) root         (0)    32770 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/medium-10.json
--rw-rw-rw-   0 root         (0) root         (0)    43595 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/medium-2.json
--rw-rw-rw-   0 root         (0) root         (0)    33837 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/medium-3.json
--rw-rw-rw-   0 root         (0) root         (0)    34664 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/medium-4.json
--rw-rw-rw-   0 root         (0) root         (0)    38406 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/medium-5.json
--rw-rw-rw-   0 root         (0) root         (0)    33991 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/medium-6.json
--rw-rw-rw-   0 root         (0) root         (0)    35438 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/medium-7.json
--rw-rw-rw-   0 root         (0) root         (0)    37158 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/medium-8.json
--rw-rw-rw-   0 root         (0) root         (0)    46046 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/medium-9.json
--rw-rw-rw-   0 root         (0) root         (0)     1096 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test1.json
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test1.txt
--rw-rw-rw-   0 root         (0) root         (0)     1131 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test1.xml
--rw-rw-rw-   0 root         (0) root         (0)     1193 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test10.json
--rw-rw-rw-   0 root         (0) root         (0)     2598 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test10_output.json
--rw-rw-rw-   0 root         (0) root         (0)      659 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test1_output.json
--rw-rw-rw-   0 root         (0) root         (0)     1299 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test2.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test2.txt
--rw-rw-rw-   0 root         (0) root         (0)     1746 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test2.xml
--rw-rw-rw-   0 root         (0) root         (0)      591 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test3.json
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test3.txt
--rw-rw-rw-   0 root         (0) root         (0)      813 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test3.xml
--rw-rw-rw-   0 root         (0) root         (0)     1031 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test3b.json
--rw-rw-rw-   0 root         (0) root         (0)       56 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test3b.txt
--rw-rw-rw-   0 root         (0) root         (0)     1385 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test3b.xml
--rw-rw-rw-   0 root         (0) root         (0)      827 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test4.json
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test4.txt
--rw-rw-rw-   0 root         (0) root         (0)     1124 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test4.xml
--rw-rw-rw-   0 root         (0) root         (0)      654 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test5.json
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test5.txt
--rw-rw-rw-   0 root         (0) root         (0)      896 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test5.xml
--rw-rw-rw-   0 root         (0) root         (0)      485 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test5b.json
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test5b.txt
--rw-rw-rw-   0 root         (0) root         (0)       31 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test6.txt
--rw-rw-rw-   0 root         (0) root         (0)      759 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test6a.json
--rw-rw-rw-   0 root         (0) root         (0)     1037 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test6a.xml
--rw-rw-rw-   0 root         (0) root         (0)      691 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test6b.json
--rw-rw-rw-   0 root         (0) root         (0)      950 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test6b.xml
--rw-rw-rw-   0 root         (0) root         (0)   116023 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test7.json
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test7.txt
--rw-rw-rw-   0 root         (0) root         (0)      691 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test8.json
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test8.txt
--rw-rw-rw-   0 root         (0) root         (0)      963 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test8b.json
--rw-rw-rw-   0 root         (0) root         (0)      128 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test8b.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test9.json
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test9_output.json
--rw-rw-rw-   0 root         (0) root         (0)      438 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test_simple_chains.json
--rw-rw-rw-   0 root         (0) root         (0)       67 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_instances/test_simple_chains.txt
--rw-rw-rw-   0 root         (0) root         (0)    10969 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1813 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_output.py
--rw-rw-rw-   0 root         (0) root         (0)     8826 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_pool.py
--rw-rw-rw-   0 root         (0) root         (0)     4097 2022-11-22 09:50:58.000000 kep_solver-2.1.1/tests/test_statistics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.156268 kep_solver-2.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-20 14:38:57.000000 kep_solver-2.1.2/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-04-20 14:38:57.000000 kep_solver-2.1.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2023-04-20 14:38:57.000000 kep_solver-2.1.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-04-20 14:38:57.000000 kep_solver-2.1.2/.readthedocs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4566 2023-04-20 14:38:57.000000 kep_solver-2.1.2/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     8779 2023-04-20 14:38:57.000000 kep_solver-2.1.2/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)    34462 2023-04-20 14:38:57.000000 kep_solver-2.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-04-20 14:39:08.156268 kep_solver-2.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4482 2023-04-20 14:38:57.000000 kep_solver-2.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.122262 kep_solver-2.1.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-20 14:38:57.000000 kep_solver-2.1.2/docs/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-04-20 14:38:57.000000 kep_solver-2.1.2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     2717 2023-04-20 14:38:57.000000 kep_solver-2.1.2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-04-20 14:38:57.000000 kep_solver-2.1.2/docs/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.122262 kep_solver-2.1.2/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)    11079 2023-04-20 14:38:57.000000 kep_solver-2.1.2/docs/source/formats.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5405 2023-04-20 14:38:57.000000 kep_solver-2.1.2/docs/source/terms.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2023-04-20 14:38:57.000000 kep_solver-2.1.2/docs/source/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.125265 kep_solver-2.1.2/kep_solver/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 14:38:57.000000 kep_solver-2.1.2/kep_solver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19271 2023-04-20 14:38:57.000000 kep_solver-2.1.2/kep_solver/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     9106 2023-04-20 14:38:57.000000 kep_solver-2.1.2/kep_solver/fileio.py
+-rw-rw-rw-   0 root         (0) root         (0)    35842 2023-04-20 14:38:57.000000 kep_solver-2.1.2/kep_solver/generation.py
+-rw-rw-rw-   0 root         (0) root         (0)    23791 2023-04-20 14:38:57.000000 kep_solver-2.1.2/kep_solver/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    19222 2023-04-20 14:38:57.000000 kep_solver-2.1.2/kep_solver/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     7152 2023-04-20 14:38:57.000000 kep_solver-2.1.2/kep_solver/pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.126265 kep_solver-2.1.2/kep_solver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-04-20 14:39:08.000000 kep_solver-2.1.2/kep_solver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2815 2023-04-20 14:39:08.000000 kep_solver-2.1.2/kep_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 14:39:08.000000 kep_solver-2.1.2/kep_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-04-20 14:39:08.000000 kep_solver-2.1.2/kep_solver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-20 14:39:08.000000 kep_solver-2.1.2/kep_solver.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-04-20 14:38:57.000000 kep_solver-2.1.2/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.127265 kep_solver-2.1.2/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)     6159 2023-04-20 14:38:57.000000 kep_solver-2.1.2/notebooks/Match Run.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1485 2023-04-20 14:38:57.000000 kep_solver-2.1.2/notebooks/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    23889 2023-04-20 14:38:57.000000 kep_solver-2.1.2/notebooks/Statistical Analysis.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.128265 kep_solver-2.1.2/paper/
+-rw-rw-rw-   0 root         (0) root         (0)     2848 2023-04-20 14:38:57.000000 kep_solver-2.1.2/paper/paper.bib
+-rw-rw-rw-   0 root         (0) root         (0)     6286 2023-04-20 14:38:57.000000 kep_solver-2.1.2/paper/paper.md
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-20 14:38:57.000000 kep_solver-2.1.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-20 14:38:57.000000 kep_solver-2.1.2/runtime.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-04-20 14:39:08.157268 kep_solver-2.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-04-20 14:38:57.000000 kep_solver-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.130266 kep_solver-2.1.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4581 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_fileio.py
+-rw-rw-rw-   0 root         (0) root         (0)    21574 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    16083 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.156268 kep_solver-2.1.2/tests/test_instances/
+-rw-rw-rw-   0 root         (0) root         (0)   514090 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-1.json
+-rw-rw-rw-   0 root         (0) root         (0)   590458 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-10.json
+-rw-rw-rw-   0 root         (0) root         (0)   610079 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-2.json
+-rw-rw-rw-   0 root         (0) root         (0)   590792 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-3.json
+-rw-rw-rw-   0 root         (0) root         (0)   550366 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-4.json
+-rw-rw-rw-   0 root         (0) root         (0)   575193 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-5.json
+-rw-rw-rw-   0 root         (0) root         (0)   660843 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-6.json
+-rw-rw-rw-   0 root         (0) root         (0)   665457 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-7.json
+-rw-rw-rw-   0 root         (0) root         (0)   684308 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-8.json
+-rw-rw-rw-   0 root         (0) root         (0)   686677 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-9.json
+-rw-rw-rw-   0 root         (0) root         (0)    40468 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-1.json
+-rw-rw-rw-   0 root         (0) root         (0)    32770 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-10.json
+-rw-rw-rw-   0 root         (0) root         (0)    43595 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-2.json
+-rw-rw-rw-   0 root         (0) root         (0)    33837 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-3.json
+-rw-rw-rw-   0 root         (0) root         (0)    34664 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-4.json
+-rw-rw-rw-   0 root         (0) root         (0)    38406 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-5.json
+-rw-rw-rw-   0 root         (0) root         (0)    33991 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-6.json
+-rw-rw-rw-   0 root         (0) root         (0)    35438 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-7.json
+-rw-rw-rw-   0 root         (0) root         (0)    37158 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-8.json
+-rw-rw-rw-   0 root         (0) root         (0)    46046 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-9.json
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test1.json
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test1.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test1.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test10.json
+-rw-rw-rw-   0 root         (0) root         (0)     2598 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test10_output.json
+-rw-rw-rw-   0 root         (0) root         (0)      659 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test1_output.json
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test2.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test2.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test2.xml
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test3.json
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test3.txt
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test3.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test3b.json
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test3b.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test3b.xml
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test4.json
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test4.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test4.xml
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test5.json
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test5.txt
+-rw-rw-rw-   0 root         (0) root         (0)      896 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test5.xml
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test5b.json
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test5b.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test6.txt
+-rw-rw-rw-   0 root         (0) root         (0)      759 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test6a.json
+-rw-rw-rw-   0 root         (0) root         (0)     1037 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test6a.xml
+-rw-rw-rw-   0 root         (0) root         (0)      691 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test6b.json
+-rw-rw-rw-   0 root         (0) root         (0)      950 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test6b.xml
+-rw-rw-rw-   0 root         (0) root         (0)   116023 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test7.json
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test7.txt
+-rw-rw-rw-   0 root         (0) root         (0)      691 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test8.json
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test8.txt
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test8b.json
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test8b.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test9.json
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test9_output.json
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test_simple_chains.json
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test_simple_chains.txt
+-rw-rw-rw-   0 root         (0) root         (0)    10969 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1813 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     8826 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     4097 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_statistics.py
```

### Comparing `kep_solver-2.1.1/.gitlab-ci.yml` & `kep_solver-2.1.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/CHANGELOG.md` & `kep_solver-2.1.2/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 # Changelog
 
 ## [Unreleased]
 
+## [2.1.2]
+
+- RecipientGenerator now links a donor to their recipient correctly
+- CompatibilityGraph.findCycles() speed-ups
+- CompatibilityGraph.findChains() speed-ups
+- Cache Vertex.adjacent() list and hash(Exchange)
 - Update python version for notebooks
+- Added prototype functions to Model superclass for getting cycles, chains,
+	exchanges, and getting exchange values. These obviously might not be easily
+	implementable by all models, and may be left unimplemented.
+
+## [2.1.1]
+
+- Documentation updates
 
 ## [2.1.0]
 
 - Create random entity generators. Each of these can generate random instances
 	according to some given configuration. The configuration of each can be read
 	from a JSON object, and also be written to a JSON object (with the exception
 	of CompatibilityChanceGenerator when a function is used to define the
```

### Comparing `kep_solver-2.1.1/CONTRIBUTING.md` & `kep_solver-2.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/LICENSE` & `kep_solver-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/PKG-INFO` & `kep_solver-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kep_solver
-Version: 2.1.1
+Version: 2.1.2
 Summary: A Python package for reading and solving single instances of kidney exchange problems.
 Home-page: https://gitlab.com/wpettersson/kep_solver
 Author: William Pettersson
 Author-email: william@ewpettersson.se
 License: AGPLv3
 Keywords: kidney kidney_exchange
 Classifier: Programming Language :: Python :: 3
@@ -22,16 +22,16 @@
 
 # kep\_solver
 
 This Python package is devoted to various algorithms, procedures and mechanisms
 that are useful when studying kidney exchange programmes in general.  It is
 written and maintained by [William Pettersson](mailto:william.pettersson@glasgow.ac.uk).
 
-- [Full documentation](https://kep-solver.readthedocs.io/en/latest/).
-- [Pypi](https://pypi.org/project/kep-solver/).
+- [Full documentation](https://kep-solver.readthedocs.io/en/latest/)
+- [Pypi link](https://pypi.org/project/kep-solver/)
 
 ## Requirements
 
 kep\_solver runs on Python 3.9 or higher. As long as you install via pip, all
 other requirements will be handled by pip
 
 ## Quick start with notebooks
@@ -129,15 +129,15 @@
 * Implementation of faster models and modelling techniques
 
 
 ## Contributing
 
 I welcome input from others, whether you have ideas for improvements or want to
 submit code. Details on contributing can be found in
-[CONTRIBUTING.md](contributing.md)]. You can also get in touch directly, or
+[CONTRIBUTING.md](CONTRIBUTING.md). You can also get in touch directly, or
 raise an [issue](https://gitlab.com/wpettersson/kep_solver/-/issues)
 
 ## Acknowledgements
 
 This software has been supported by the Engineering and Physical Sciences
 Research Council (EPSRC) grant
 [EP/T004878/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/T004878/1)
```

### Comparing `kep_solver-2.1.1/README.md` & `kep_solver-2.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # kep\_solver
 
 This Python package is devoted to various algorithms, procedures and mechanisms
 that are useful when studying kidney exchange programmes in general.  It is
 written and maintained by [William Pettersson](mailto:william.pettersson@glasgow.ac.uk).
 
-- [Full documentation](https://kep-solver.readthedocs.io/en/latest/).
-- [Pypi](https://pypi.org/project/kep-solver/).
+- [Full documentation](https://kep-solver.readthedocs.io/en/latest/)
+- [Pypi link](https://pypi.org/project/kep-solver/)
 
 ## Requirements
 
 kep\_solver runs on Python 3.9 or higher. As long as you install via pip, all
 other requirements will be handled by pip
 
 ## Quick start with notebooks
@@ -107,15 +107,15 @@
 * Implementation of faster models and modelling techniques
 
 
 ## Contributing
 
 I welcome input from others, whether you have ideas for improvements or want to
 submit code. Details on contributing can be found in
-[CONTRIBUTING.md](contributing.md)]. You can also get in touch directly, or
+[CONTRIBUTING.md](CONTRIBUTING.md). You can also get in touch directly, or
 raise an [issue](https://gitlab.com/wpettersson/kep_solver/-/issues)
 
 ## Acknowledgements
 
 This software has been supported by the Engineering and Physical Sciences
 Research Council (EPSRC) grant
 [EP/T004878/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/T004878/1)
```

### Comparing `kep_solver-2.1.1/docs/Makefile` & `kep_solver-2.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/docs/conf.py` & `kep_solver-2.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/docs/source/formats.rst` & `kep_solver-2.1.2/docs/source/formats.rst`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
 The JSON contains three name/value pairs. The first is named `algorithm` and
 its value is a text description of the pool. This is currently user-configured.
 The next item is named `output`, and its value is a nested collection
 which contains exactly one element named `all_cycles`. This `all_cycles`
 element contains another nested collection, with one entry for each potential
 exchange. The name of each element is an identifier for the exchange, and these
-will commonly but not neccessarily be integers. Each exchange is then
+will commonly but not necessarily be integers. Each exchange is then
 represented by a collection, containing the following items. First, `alt` is an
 ordered list of exchange identifiers that correspond to alternate exchanges for
 this exchange. An alternate exchange is a different exchange that will still
 match exactly the same recipients. Next, `backarcs` contains the number of
 backarcs present in this exchange, and `weight` contains the weight (as
 calculated by the UK scoring mechanism) of this exchange. Lastly, the set of
 donor-recipient pairs is given as an ordered list of collections, named
```

### Comparing `kep_solver-2.1.1/docs/source/terms.rst` & `kep_solver-2.1.2/docs/source/terms.rst`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 .. _Blood groups:
 .. _Blood group:
 
 ------------
 Blood groups
 ------------
 
-Each person has a blood group (sometimes refered to as a blood type). In
+Each person has a blood group (sometimes referred to as a blood type). In
 particular, the four blood groups are A, B, AB, and O. Blood typing may also
 involve extra markers (such as +/- to indicate a presence or absence of the
 Rh(D) antigen), but for kep_solver we strictly use A, B, AB, and O. When
 determining compatibility, kep_solver follows the usual diamond of blood group
 compatibility. That is to say, a recipient with blood group O is only ever
 compatible with donors who have blood group O, a recipient with blood group AB
 can be compatible with donors who have any blood group, and a recipient with
@@ -54,15 +54,15 @@
 Note that kep_solver will not allow you to set a cPRA value outside of the
 range [0, 1], but will instead raise an exception.
 
 
 .. _compatibility chance:
 
 ---------------------
-Compatibiliity chance
+Compatibility chance
 ---------------------
 
 For a given recipient `R`, we say that their compatibility chance is the ratio of
 `number of blood group compatible donors who have a transplant with R` divided
 by `number of blood group compatible donors who appear in a matching run with R`.
 The goal with compatibility chance is to represent the possibility of a
 transplant being present once blood groups have been accounted for. Note that
```

### Comparing `kep_solver-2.1.1/docs/source/usage.rst` & `kep_solver-2.1.2/docs/source/usage.rst`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 Instances can be analysed for a number of properties, as can the Donor and
 Recipient entities they contain. These are documented in :doc:`kep_solver.entities`.
 ::
 
     print(f"This instance has {len(instance.recipients())} recipients")
 
-Analysing the compatibilty graph
+Analysing the compatibility graph
 ================================
 
 The underlying compatibility graph can be accessed by creating a
 :ref:`compatibility graph` object as follows. Specifics are documented in
 :doc:`kep_solver.graph`.
 ::
```

### Comparing `kep_solver-2.1.1/kep_solver/entities.py` & `kep_solver-2.1.2/kep_solver/entities.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/kep_solver/fileio.py` & `kep_solver-2.1.2/kep_solver/fileio.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
                 total_weight += tb + bonus + transplant.weight
                 if donor.NDD:
                     desired = set([recipient])
                 else:
                     desired = set([donor.recipient, recipient])
             if len(exchange) == 3:
                 # Search for a backarc only in exchanges with 3 vertices
-                best_score = -1
+                best_score: float = -1
                 # If there are multiple potential backarcs, we want the one
                 # with the best score
                 for backarc in exchange.backarc_exchanges_uk():
                     if set(backarc.all_recipients()) == desired:
                         if len(backarc) == 2:  # 2 vertices in the "backarc exchange"
                             new_score = self._model.exchange_values(backarc)[-1]
                             if new_score > best_score:
```

### Comparing `kep_solver-2.1.1/kep_solver/generation.py` & `kep_solver-2.1.2/kep_solver/generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,15 +346,17 @@
         band is the probability that this band is selected.
         """
         bands = {}
         for band in json_obj:
             entry, chance = band
             try:
                 low, high = entry
-            except ValueError:  # Only one value in list, must be both low and high value
+            except (
+                ValueError
+            ):  # Only one value in list, must be both low and high value
                 low = entry
                 high = entry
             bands[(low, high)] = chance
         return cls(bands=bands)
 
 
 CompatibilityChanceGeneratorConfig = list[tuple[float, float, FloatGeneratorConfig]]
@@ -411,15 +413,15 @@
                     )
         self._dists: list[
             tuple[float, float, Union[FloatGenerator, Callable[[float], float]]]
         ] = dists
 
     def draw(self, pra) -> float:
         """Draw a compatibility chance."""
-        for (low, high, gen) in self._dists:
+        for low, high, gen in self._dists:
             if low <= pra and pra < high:
                 if isinstance(gen, FloatGenerator):
                     return gen.draw()
                 else:
                     return gen(pra)
         raise Exception("Compatibility chance generation failed")
 
@@ -431,15 +433,15 @@
 
         :return: a list of [low, high, generator] lists such that if the recipient
             cPRA is between low and high, then generator is a configuration for a
             FloatGenerator that will generate the compatibility chance for this
             recipient.
         """
         res: list[tuple[float, float, FloatGeneratorConfig]] = []
-        for (low, high, band) in self._dists:
+        for low, high, band in self._dists:
             if not isinstance(band, FloatGenerator):
                 raise Exception(
                     "Cannot get configuration for a CompatibilityChanceGenerator that uses a function."
                 )
             res.append((low, high, band.config()))
         return res
 
@@ -453,15 +455,15 @@
         compatibility chance for this recipient.
 
         Currently, only linear functions can loaded from JSON.
         """
         dists: list[
             tuple[float, float, Union[FloatGenerator, Callable[[float], float]]]
         ] = []
-        for (low, high, config) in json_obj:
+        for low, high, config in json_obj:
             if "function" in config:
                 specification = config["function"]
                 function_type = specification["type"]
                 if function_type == "linear":
                     dists.append(
                         (
                             low,
@@ -675,14 +677,15 @@
         """
         r = Recipient(id=id_)
         r.bloodGroup = self._recipient_bloodgroup_generator.draw()
         donorCount = self._donor_count_generator.draw()
         compatible = False
         for _ in range(donorCount):
             d = self._donor_generator.draw(donor_id_function(r))
+            d.recipient = r
             r.addDonor(d)
         r.cPRA = self._cpra_generator.draw(r.hasBloodCompatibleDonor())
         r.compatibilityChance = self._compatibility_chance_generator.draw(r.cPRA)
         return r
 
     def config(self) -> RecipientGeneratorConfig:
         """Returns the configuration of this RecipientGenerator.
```

### Comparing `kep_solver-2.1.1/kep_solver/graph.py` & `kep_solver-2.1.2/kep_solver/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Describes a number of classes related to the compatibility graph."""
 from __future__ import annotations
 
 from collections import defaultdict
 from itertools import combinations
-from typing import Any, Union, Optional, Iterable
+from typing import Any, Union, Optional, Iterable, Callable
 
 from kep_solver.entities import Donor, Recipient
 
 
 class Vertex:
     """A vertex in a digraph representing a donor (directed or
     non-directed)."""
 
     def __init__(self, index: int, represents: Donor) -> None:
         self._index: int = index
         self._represents: Donor = represents
         self._properties: dict[str, Any] = {}
         self._edges_out: list[Edge] = []
         self._edges_in: list[Edge] = []
+        self._adj: Optional[list[Vertex]] = None
 
     @property
     def index(self) -> int:
         """Get the index (in the graph) of this vertex.
 
         :return: the index
         """
@@ -50,14 +51,15 @@
         self._edges_in.append(edge)
 
     def addEdgeOut(self, edge: Edge) -> None:
         """Add an edge leading out from this vertex.
 
         :param edge: the edge
         """
+        self._adj = None
         self._edges_out.append(edge)
 
     @property
     def edgesIn(self) -> list[Edge]:
         """Return the list of edges leading in to this vertex.
 
         :return: the list of edges leading in to this vertex.
@@ -73,15 +75,17 @@
         return self._edges_out
 
     def adjacent(self) -> list[Vertex]:
         """Return the neighbours of this vertex
 
         :return: the list of neighbouring vertices
         """
-        return [edge.end for edge in self.edgesOut]
+        if self._adj is None:
+            self._adj = [edge.end for edge in self.edgesOut]
+        return self._adj
 
     def __str__(self) -> str:
         """Return a string representation of the vertex."""
         if self.isNdd():
             return f"V({self.donor} ({self.index}))"
         else:
             return f"V({self.donor},{self.donor.recipient} ({self.index}))"
@@ -96,14 +100,15 @@
     """
 
     def __init__(self, _id: str, vertices: list[Vertex]):
         self._id: str = _id
         self._vertices: tuple[Vertex, ...] = tuple(vertices)
         self._alternates: list[Exchange] = []
         self._embedded: list[Exchange] = []
+        self._hash = hash(tuple([v.index for v in self.vertices]))
 
     @property
     def id(self) -> str:
         """The ID of the exchange."""
         return self._id
 
     @property
@@ -279,15 +284,15 @@
 
         :param embeds: The embedded exchanges.
         """
         for embed in embeds:
             self.add_embedded(embed)
 
     def __hash__(self):
-        return hash(tuple([v.index for v in self.vertices]))
+        return self._hash
 
 
 class Edge:
     """An edge in a digraph, representing a potential transplant. An
     edge is always associated with a donor.
     """
 
@@ -339,15 +344,15 @@
 class CompatibilityGraph:
     """A :ref:`compatibility graph` is a digraph representing a KEP instance.
     Note that each vertex is a donor. Each edge corresponds to a potential
     transplant, and thus is associated with a donor that is paired with the
     recipient at beginning of the arc.
     """
 
-    def __init__(self, instance=None):
+    def __init__(self, instance=None) -> None:
         self._vertices: list[Vertex] = []
         self._edges: list[Edge] = []
 
         # Map each recipient or ndd to a vertex object
         self._vertex_map: dict[Union[Donor, Recipient], Vertex] = {}
         if instance is not None:
             for donor in instance.donors():
@@ -429,87 +434,92 @@
         :param index_offset: By default, chains are given IDs starting at zero. By
           setting this parameter to a non-zero value, IDs start at this number. This
           can help avoid ID clashes.
         :returns: a list of chains, where each chain is represented as
             a list of vertices
         """
         chains: list[Exchange] = []
-        used = [False] * self.size
-        stack: list[Vertex] = []
+        used: set[int] = set()
+        stack: list[Vertex]
 
         def _extend(v: Vertex):
-            chains.append(
-                Exchange(f"{len(chains) + index_offset}", [vert for vert in stack])
-            )
+            chains.append(Exchange(f"{len(chains) + index_offset}", stack.copy()))
             if len(stack) == maxChainLength:
                 return
             for w in v.adjacent():
-                if not used[w.index]:
-                    used[w.index] = True
+                if w.index not in used:
+                    used.add(w.index)
                     stack.append(w)
                     _extend(w)
                     stack.pop()
-                    used[w.index] = False
+                    used.remove(w.index)
 
         for vert in self.vertices:
             if not vert.isNdd():
                 continue
-            used = [False] * self.size
             stack = [vert]
             _extend(vert)
         return chains
 
-    def findCycles(self, maxCycleLength: int, index_offset: int = 0) -> list[Exchange]:
+    def findCycles(
+        self,
+        maxCycleLength: int,
+        index_offset: int = 0,
+        considerConnectedComponents: bool = False,
+    ) -> list[Exchange]:
         """Finds and returns all cycles in this graph. Note that this
         is specifically cycles, and does not include chains.
 
         :param maxCycleLength: the maximum length of any cycle
         :param index_offset: By default, chains are given IDs starting at zero. By
           setting this parameter to a non-zero value, IDs start at this number. This
           can help avoid ID clashes.
+        :param considerConnectedComponents: If True, we use Tarjan's algorithm
+          to first split the graph into strongly connected components and never
+          follow edges that go between strongly connected components. This is
+          valid as any cycle must exist completely within one strongly connected
+          cycle, but the overhead of calculating strongly connected components is
+          generally not worth it. If False, we instead are allowed to follow any
+          edge.
         :returns: a list of cycles, where each cycle is represented as
           a list of vertices
         """
         # Implementing a variant of Johnson's algorithm from
         # Finding All The Elementary Circuits of a Directed Graph,
         # Donald B. Johnson, SIAM J.
         # Comput., 1975
         # There are some changes, however. Blocklists (B(n) in the
         # paper) aren't used, as since we limit cycle lengths we will
         # return when the stack is too long, but that doesn't mean we
         # must've created all cycles through a given vertex. For the
         # same reason, v is unblocked after each visit, regardless of
         # whether we find any cycles
-        blocked: list[bool] = [False] * self.size
+        blocked: set[int] = set()
         stack: list[int] = []
         cycles: list[list[int]] = []
 
-        def _unblock(u: int):
-            blocked[u] = False
-
-        def _circuit(v: int, component: list[int]) -> bool:
-            flag = False
-            if len(stack) == maxCycleLength:
-                return False
+        def _circuit(v: int, condition: Callable[[int], bool]) -> None:
             stack.append(v)
-            blocked[v] = True
             for w in self.vertices[v].adjacent():
-                if w.index not in component:
+                if w.index == stack[0]:
+                    cycles.append(stack.copy())
+                    # Have completed cycle, and cannot recurse as we are at the
+                    # max length, so no need to check other neighbours of v
+                    if len(stack) == maxCycleLength:
+                        stack.pop(-1)
+                        return
+                    continue
+                if condition(w.index):
+                    continue
+                if len(stack) == maxCycleLength:
                     continue
-                if w.index == s:
-                    flag = True
-                    cycles.append(list(stack + [s]))
-                elif not blocked[w.index]:
-                    if _circuit(w.index, component):
-                        flag = True
-            _unblock(v)
+                if w.index not in stack:
+                    _circuit(w.index, condition)
             stack.pop(-1)
-            return flag
-
-        s = 0
+            return
 
         def _tarjan(num_forbidden_vertices: int) -> Optional[list[int]]:
             index = 0
             component = None
             stack = list()
             indices = [-1] * self.size
             lowlink = [-1] * self.size
@@ -537,33 +547,35 @@
             for v in range(num_forbidden_vertices, self.size):
                 if indices[v] == -1:
                     index, component = _strongconnect(v, index)
                 if component is not None:
                     return component
             return None
 
-        while s < self.size:
-            # Let Ak be adj matrix of strongly connected component K of
-            # the induced graph on {s, s+1, ... , n} that contains the
-            # lowest vertex
-            component = _tarjan(s)
-            if component is None:
-                s = self.size
-            else:
-                s = component[0]
-                for i in component:
-                    blocked[i] = False
-                _circuit(s, component)
-                s += 1
+        if considerConnectedComponents:
+            s = 0
+            while s < self.size:
+                # Let Ak be adj matrix of strongly connected component K of
+                # the induced graph on {s, s+1, ... , n} that contains the
+                # lowest vertex
+                component = _tarjan(s)
+                if component is None:
+                    s = self.size
+                else:
+                    compset = set(component)
+                    s = component[0]
+                    _circuit(s, lambda v: v not in compset)
 
+        else:
+            for s in range(self.size):
+                if not self.vertices[s].isNdd():
+                    _circuit(s, lambda v: v < s)
         realCycles: list[Exchange] = []
         for indices in cycles:
-            # Johnson's always adds the first vertex onto the end as
-            # well, but we remove it
-            real = [self.vertices[i] for i in indices[:-1]]
+            real = [self.vertices[i] for i in indices]
             realCycles.append(Exchange(f"{len(realCycles) + index_offset}", real))
         return realCycles
 
 
 def build_alternates_and_embeds(exchanges: list[Exchange]) -> None:
     """Finds and adds alternate aned embedded exchanges based on the given exchanges. An
     alternate exchange is one that still matches exactly the same set of
```

### Comparing `kep_solver-2.1.1/kep_solver/model.py` & `kep_solver-2.1.2/kep_solver/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,14 +295,47 @@
     """
 
     supports: list[type[Objective]] = []
 
     def __init__(self):
         super().__init__()
 
+    @property
+    def cycles(self) -> ValuesView[Exchange]:
+        """Return the list of cycles in this model.
+
+        :return: the list of cycles
+        """
+        raise Exception("Not implemented")
+
+    @property
+    def chains(self) -> ValuesView[Exchange]:
+        """Return the list of chains in this model.
+
+        :return: the list of chains
+        """
+        raise Exception("Not implemented")
+
+    @property
+    def exchanges(self) -> list[Exchange]:
+        """Return the list of cycles and chains in this model.
+
+        :return: the list of cycles and chains
+        """
+        raise Exception("Not implemented")
+
+    def exchange_values(self, exchange: Exchange) -> list[float]:
+        """Given an exchange, return the value of the exchange for
+        each objective.
+
+        :param exchange: The exchange whose value is to be returned
+        :return: the list of values of this exchange
+        """
+        raise Exception("Not implemented")
+
     def support(self, objective: Objective) -> bool:
         """Can this model solve for the given objective.
 
         :param objective: The objective to solve
         :return: Can this model solve the given objective
         """
         return bool([isinstance(objective, supported) for supported in self.supports])
@@ -406,15 +439,15 @@
         """Given an exchange, get the variable representing it.
 
         :param exchange: the exchange to search for
         :return: the exchange's variable
         """
         return self._vars_by_exchange[exchange]
 
-    def build_model(self):
+    def build_model(self) -> None:
         """Build the model. That is, create all the variables and
         constraints."""
         # Track the chains each NDD can be in
         chains_by_ndd: dict[Donor, list[pulp.LpVariable]] = {}
         for nondirected in self._instance.donors():
             if not nondirected.NDD:
                 continue
```

### Comparing `kep_solver-2.1.1/kep_solver/pool.py` & `kep_solver-2.1.2/kep_solver/pool.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/kep_solver.egg-info/PKG-INFO` & `kep_solver-2.1.2/kep_solver.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kep-solver
-Version: 2.1.1
+Version: 2.1.2
 Summary: A Python package for reading and solving single instances of kidney exchange problems.
 Home-page: https://gitlab.com/wpettersson/kep_solver
 Author: William Pettersson
 Author-email: william@ewpettersson.se
 License: AGPLv3
 Keywords: kidney kidney_exchange
 Classifier: Programming Language :: Python :: 3
@@ -22,16 +22,16 @@
 
 # kep\_solver
 
 This Python package is devoted to various algorithms, procedures and mechanisms
 that are useful when studying kidney exchange programmes in general.  It is
 written and maintained by [William Pettersson](mailto:william.pettersson@glasgow.ac.uk).
 
-- [Full documentation](https://kep-solver.readthedocs.io/en/latest/).
-- [Pypi](https://pypi.org/project/kep-solver/).
+- [Full documentation](https://kep-solver.readthedocs.io/en/latest/)
+- [Pypi link](https://pypi.org/project/kep-solver/)
 
 ## Requirements
 
 kep\_solver runs on Python 3.9 or higher. As long as you install via pip, all
 other requirements will be handled by pip
 
 ## Quick start with notebooks
@@ -129,15 +129,15 @@
 * Implementation of faster models and modelling techniques
 
 
 ## Contributing
 
 I welcome input from others, whether you have ideas for improvements or want to
 submit code. Details on contributing can be found in
-[CONTRIBUTING.md](contributing.md)]. You can also get in touch directly, or
+[CONTRIBUTING.md](CONTRIBUTING.md). You can also get in touch directly, or
 raise an [issue](https://gitlab.com/wpettersson/kep_solver/-/issues)
 
 ## Acknowledgements
 
 This software has been supported by the Engineering and Physical Sciences
 Research Council (EPSRC) grant
 [EP/T004878/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/T004878/1)
```

### Comparing `kep_solver-2.1.1/kep_solver.egg-info/SOURCES.txt` & `kep_solver-2.1.2/kep_solver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/notebooks/Match Run.ipynb` & `kep_solver-2.1.2/notebooks/Match Run.ipynb`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/notebooks/README.md` & `kep_solver-2.1.2/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/notebooks/Statistical Analysis.ipynb` & `kep_solver-2.1.2/notebooks/Statistical Analysis.ipynb`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/paper/paper.bib` & `kep_solver-2.1.2/paper/paper.bib`

 * *Files 18% similar despite different names*

```diff
@@ -51,35 +51,28 @@
 year = {2022},
 issn = {0305-0548},
 doi = {10.1016/j.cor.2022.105707},
 author = {Maxence Delorme and Sergio García and Jacek Gondzio and Jörg Kalcsics and David Manlove and William Pettersson and James Trimble},
 keywords = {kidney exchange, Saidman generator, Matheuristic},
 }
 
-@inproceedings{Dickerson,
+@article{Dickerson,
 author = {Dickerson, John P. and Procaccia, Ariel D. and Sandholm, Tuomas},
 title = {Price of Fairness in Kidney Exchange},
+journal = {Transplantation},
 year = {2014},
-isbn = {9781450327381},
-publisher = {International Foundation for Autonomous Agents and Multiagent Systems},
-address = {Richland, SC},
-booktitle = {Proceedings of the 2014 International Conference on Autonomous Agents and Multi-Agent Systems},
-pages = {1013–1020},
-numpages = {8},
-doi = {10.5555/2615731.2617407},
-keywords = {kidney exchange, price of fairness, equity-efficiency tradeoff},
-location = {Paris, France},
-series = {AAMAS '14}
+pages = {815},
+volume = {98},
+doi = {10.1097/00007890-201407151-02779}
 }
 
-
 @article{Toulis,
 title = {Design and analysis of multi-hospital kidney exchange mechanisms using random graphs},
 journal = {Games and Economic Behavior},
 volume = {91},
 pages = {360-382},
 year = {2015},
 issn = {0899-8256},
-doi = {j.geb.2015.01.001},
+doi = {10.1016/j.geb.2015.01.001},
 author = {Panos Toulis and David C. Parkes},
 keywords = {Kidney exchange, Random graphs, Mechanism design, Maximum matching, Integer programming, Incentive compatible design},
 }
```

### Comparing `kep_solver-2.1.1/paper/paper.md` & `kep_solver-2.1.2/paper/paper.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   - kidney exchange
   - operations research
 authors:
   - name: William Pettersson
     orcid: 0000-0003-0040-2088
     affiliation: 1
 affiliations:
-  - name: School of Computing Science, University of Glasgow, UK
+  - name: School of Computing Science, University of Glasgow, United Kingdom
     index: 1
 date: 15 September 2022
 bibliography: paper.bib
 
 ---
 
 
@@ -121,29 +121,14 @@
 ```
 
 The first three lines simply import the necessary portions of `kep_solver`. We
 then read an instance from a file, create a pool with one optimisation
 objective (`TransplantCount()`), solve the single given instance and print out
 how many transplants are selected.
 
-
-Two notebooks are provided in the `notebooks/` folder with more complicated
-use cases. The first of these, titled `Match Run.ipynb`, gives a complete
-guide to configuring a kidney exchange pool, including setting
-different optimisation criteria and pool parameters such as maximum chain
-length and examining the selected transplants in closer detail. The second
-notebook, titled `Statistical Analysis.ipynb`, performs a number of in-depth
-statistical analyses on a set of instance files. These analyses are not
-performed by `kep_solver`, but other third-party modules. However, the results
-of these analyses is then used by `kep_solver` to create a complete instance
-generator which can be used to create randomly generated kidney exchange
-programme instances with properties determined by the analysis. The
-configuration for this instance generator can be exported as a JSON file for
-archival purposes or for publication or sharing with other researchers.
-
 # Acknowledgements
 
 This software has been supported by the Engineering and Physical Sciences
 Research Council (EPSRC) grant
 [EP/T004878/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/T004878/1)
 (Multilayer Algorithmics to Leverage Graph Structure).
```

### Comparing `kep_solver-2.1.1/setup.cfg` & `kep_solver-2.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_fileio.py` & `kep_solver-2.1.2/tests/test_fileio.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_generator.py` & `kep_solver-2.1.2/tests/test_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -583,14 +583,15 @@
     )
     recip_gen = generation.RecipientGenerator(bgen, dcgen, dgen, cpra_gen, compat_gen)
     random.seed(SEED)
     r = recip_gen.draw("1")
     assert r.id == "1"
     assert len(r.donors()) == 1
     assert r.donors()[0].id == "1_D1"
+    assert r.donors()[0].recipient == r
     r = recip_gen.draw("2")
     assert r.id == "2"
     assert len(r.donors()) == 1
     r = recip_gen.draw("3")
     assert r.id == "3"
     assert len(r.donors()) == 1
     r = recip_gen.draw("R4")
```

### Comparing `kep_solver-2.1.1/tests/test_graph.py` & `kep_solver-2.1.2/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/large-1.json` & `kep_solver-2.1.2/tests/test_instances/large-1.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/large-10.json` & `kep_solver-2.1.2/tests/test_instances/large-10.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/large-2.json` & `kep_solver-2.1.2/tests/test_instances/large-2.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/large-3.json` & `kep_solver-2.1.2/tests/test_instances/large-3.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/large-4.json` & `kep_solver-2.1.2/tests/test_instances/large-4.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/large-5.json` & `kep_solver-2.1.2/tests/test_instances/large-5.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/large-6.json` & `kep_solver-2.1.2/tests/test_instances/large-6.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/large-7.json` & `kep_solver-2.1.2/tests/test_instances/large-7.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/large-8.json` & `kep_solver-2.1.2/tests/test_instances/large-8.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/large-9.json` & `kep_solver-2.1.2/tests/test_instances/large-9.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/medium-1.json` & `kep_solver-2.1.2/tests/test_instances/medium-1.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/medium-10.json` & `kep_solver-2.1.2/tests/test_instances/medium-10.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/medium-2.json` & `kep_solver-2.1.2/tests/test_instances/medium-2.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/medium-3.json` & `kep_solver-2.1.2/tests/test_instances/medium-3.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/medium-4.json` & `kep_solver-2.1.2/tests/test_instances/medium-4.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/medium-5.json` & `kep_solver-2.1.2/tests/test_instances/medium-5.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/medium-6.json` & `kep_solver-2.1.2/tests/test_instances/medium-6.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/medium-7.json` & `kep_solver-2.1.2/tests/test_instances/medium-7.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/medium-8.json` & `kep_solver-2.1.2/tests/test_instances/medium-8.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/medium-9.json` & `kep_solver-2.1.2/tests/test_instances/medium-9.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test1.json` & `kep_solver-2.1.2/tests/test_instances/test1.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test1.xml` & `kep_solver-2.1.2/tests/test_instances/test1.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test10.json` & `kep_solver-2.1.2/tests/test_instances/test10.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test10_output.json` & `kep_solver-2.1.2/tests/test_instances/test10_output.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test1_output.json` & `kep_solver-2.1.2/tests/test_instances/test1_output.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test2.json` & `kep_solver-2.1.2/tests/test_instances/test2.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test2.xml` & `kep_solver-2.1.2/tests/test_instances/test2.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test3.json` & `kep_solver-2.1.2/tests/test_instances/test3.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test3.xml` & `kep_solver-2.1.2/tests/test_instances/test3.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test3b.json` & `kep_solver-2.1.2/tests/test_instances/test3b.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test3b.xml` & `kep_solver-2.1.2/tests/test_instances/test3b.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test4.json` & `kep_solver-2.1.2/tests/test_instances/test4.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test4.xml` & `kep_solver-2.1.2/tests/test_instances/test4.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test5.json` & `kep_solver-2.1.2/tests/test_instances/test5.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test5.xml` & `kep_solver-2.1.2/tests/test_instances/test5.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test6a.json` & `kep_solver-2.1.2/tests/test_instances/test6a.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test6a.xml` & `kep_solver-2.1.2/tests/test_instances/test6a.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test6b.json` & `kep_solver-2.1.2/tests/test_instances/test6b.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test6b.xml` & `kep_solver-2.1.2/tests/test_instances/test6b.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test7.json` & `kep_solver-2.1.2/tests/test_instances/test7.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test8.json` & `kep_solver-2.1.2/tests/test_instances/test8.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test8b.json` & `kep_solver-2.1.2/tests/test_instances/test8b.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_instances/test9_output.json` & `kep_solver-2.1.2/tests/test_instances/test9_output.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_model.py` & `kep_solver-2.1.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_output.py` & `kep_solver-2.1.2/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_pool.py` & `kep_solver-2.1.2/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.1/tests/test_statistics.py` & `kep_solver-2.1.2/tests/test_statistics.py`

 * *Files identical despite different names*

