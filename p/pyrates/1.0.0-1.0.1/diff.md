# Comparing `tmp/pyrates-1.0.0.tar.gz` & `tmp/pyrates-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrates-1.0.0.tar", last modified: Fri Feb  3 15:19:43 2023, max compression
+gzip compressed data, was "pyrates-1.0.1.tar", last modified: Thu Apr 20 21:11:31 2023, max compression
```

## Comparing `pyrates-1.0.0.tar` & `pyrates-1.0.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.491114 pyrates-1.0.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-02-03 15:19:31.000000 pyrates-1.0.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-02-03 15:19:31.000000 pyrates-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-02-03 15:19:43.491114 pyrates-1.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4246 2023-02-03 15:19:31.000000 pyrates-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.479114 pyrates-1.0.0/model_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.479114 pyrates-1.0.0/model_templates/CNS_2019_Tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4070 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/CNS_2019_Tutorial/templates.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/base_templates.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.479114 pyrates-1.0.0/model_templates/neural_mass_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/neural_mass_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/neural_mass_models/ik.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/neural_mass_models/jansenrit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/neural_mass_models/qif.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/neural_mass_models/synaptic_plasticity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/neural_mass_models/theta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/neural_mass_models/wilsoncowan.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.479114 pyrates-1.0.0/model_templates/oscillators/
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/oscillators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/oscillators/kuramoto.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/oscillators/stuartlandau.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/oscillators/vanderpol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.483114 pyrates-1.0.0/model_templates/test_resources/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/test_resources/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/test_resources/linear.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     4425 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/test_resources/test_backend.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-02-03 15:19:31.000000 pyrates-1.0.0/model_templates/test_resources/test_operator_caching_templates.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.483114 pyrates-1.0.0/pyrates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.483114 pyrates-1.0.0/pyrates/backend/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1522 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.483114 pyrates-1.0.0/pyrates/backend/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/base/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16686 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/base/base_backend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4322 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/base/base_funcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34712 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/computegraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.483114 pyrates-1.0.0/pyrates/backend/fortran/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/fortran/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18865 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/fortran/fortran_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/fortran/fortran_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.483114 pyrates-1.0.0/pyrates/backend/julia/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/julia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/julia/julia_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/julia/julia_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.487114 pyrates-1.0.0/pyrates/backend/matlab/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/matlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/matlab/matlab_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/matlab/matlab_funcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26490 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.487114 pyrates-1.0.0/pyrates/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/tensorflow/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10410 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/tensorflow/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/tensorflow/tensorflow_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.487114 pyrates-1.0.0/pyrates/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/torch/torch_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/backend/torch/torch_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.487114 pyrates-1.0.0/pyrates/frontend/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1708 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4091 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/dict.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3302 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.487114 pyrates-1.0.0/pyrates/frontend/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/fileio/pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/fileio/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.487114 pyrates-1.0.0/pyrates/frontend/template/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5426 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/template/_io.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4268 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/template/abc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    64196 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/template/circuit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/template/circuit.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/template/edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      929 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/template/edge.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/template/node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12467 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/template/operator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7957 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/frontend/template/operator_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.487114 pyrates-1.0.0/pyrates/ir/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1598 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/ir/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5572 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/ir/abc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    56222 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/ir/circuit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4084 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/ir/edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7049 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/ir/node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5162 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/ir/operator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10463 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/ir/operator_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    16294 2023-02-03 15:19:31.000000 pyrates-1.0.0/pyrates/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.483114 pyrates-1.0.0/pyrates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-02-03 15:19:43.000000 pyrates-1.0.0/pyrates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-02-03 15:19:43.000000 pyrates-1.0.0/pyrates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 15:19:43.000000 pyrates-1.0.0/pyrates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 15:19:43.000000 pyrates-1.0.0/pyrates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-03 15:19:43.000000 pyrates-1.0.0/pyrates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-03 15:19:43.000000 pyrates-1.0.0/pyrates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 15:19:43.491114 pyrates-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1997 2023-02-03 15:19:31.000000 pyrates-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 15:19:43.491114 pyrates-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-02-03 15:19:31.000000 pyrates-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-02-03 15:19:31.000000 pyrates-1.0.0/tests/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-02-03 15:19:31.000000 pyrates-1.0.0/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11835 2023-02-03 15:19:31.000000 pyrates-1.0.0/tests/test_backend_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22168 2023-02-03 15:19:31.000000 pyrates-1.0.0/tests/test_backend_simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-02-03 15:19:31.000000 pyrates-1.0.0/tests/test_file_io.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9518 2023-02-03 15:19:31.000000 pyrates-1.0.0/tests/test_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-02-03 15:19:31.000000 pyrates-1.0.0/tests/test_implemented_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.707143 pyrates-1.0.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-04-20 21:11:22.000000 pyrates-1.0.1/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-04-20 21:11:22.000000 pyrates-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-20 21:11:31.703143 pyrates-1.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5121 2023-04-20 21:11:22.000000 pyrates-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.695143 pyrates-1.0.1/model_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.695143 pyrates-1.0.1/model_templates/CNS_2019_Tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4070 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/CNS_2019_Tutorial/templates.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/base_templates.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/model_templates/neural_mass_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/neural_mass_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/neural_mass_models/ik.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/neural_mass_models/jansenrit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/neural_mass_models/qif.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/neural_mass_models/synaptic_plasticity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/neural_mass_models/theta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/neural_mass_models/wilsoncowan.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/model_templates/oscillators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/oscillators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/oscillators/kuramoto.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/oscillators/stuartlandau.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/oscillators/vanderpol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/model_templates/test_resources/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/test_resources/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/test_resources/linear.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4425 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/test_resources/test_backend.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/test_resources/test_operator_caching_templates.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates/backend/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1522 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates/backend/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/base/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16686 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/base/base_backend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4322 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/base/base_funcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34712 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/computegraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates/backend/fortran/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/fortran/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18865 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/fortran/fortran_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/fortran/fortran_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates/backend/julia/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/julia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/julia/julia_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/julia/julia_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates/backend/matlab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/matlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/matlab/matlab_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/matlab/matlab_funcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26490 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/tensorflow/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10410 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/tensorflow/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/tensorflow/tensorflow_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.703143 pyrates-1.0.1/pyrates/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/torch/torch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/torch/torch_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.703143 pyrates-1.0.1/pyrates/frontend/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1708 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4091 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/dict.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3302 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.703143 pyrates-1.0.1/pyrates/frontend/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/fileio/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/fileio/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.703143 pyrates-1.0.1/pyrates/frontend/template/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5426 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/_io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4268 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/abc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    64168 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/circuit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/circuit.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      929 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/edge.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/node.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12467 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/operator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7957 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/operator_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.703143 pyrates-1.0.1/pyrates/ir/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1598 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/ir/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5572 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/ir/abc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56222 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/ir/circuit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4084 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/ir/edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7049 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/ir/node.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5162 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/ir/operator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10463 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/ir/operator_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15933 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-20 21:11:31.000000 pyrates-1.0.1/pyrates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-20 21:11:31.000000 pyrates-1.0.1/pyrates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:11:31.000000 pyrates-1.0.1/pyrates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:11:31.000000 pyrates-1.0.1/pyrates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-20 21:11:31.000000 pyrates-1.0.1/pyrates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 21:11:31.000000 pyrates-1.0.1/pyrates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 21:11:31.707143 pyrates-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1997 2023-04-20 21:11:22.000000 pyrates-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.703143 pyrates-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11835 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/test_backend_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22168 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/test_backend_simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/test_file_io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/test_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/test_implemented_models.py
```

### Comparing `pyrates-1.0.0/LICENSE` & `pyrates-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/PKG-INFO` & `pyrates-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrates
-Version: 1.0.0
+Version: 1.0.1
 Summary: Dynamical Systems Modeling Framework
 Home-page: UNKNOWN
 Author: Richard Gast, Daniel Rose
 Author-email: richard.gast@northwestern.edu
 License: GPL v3
 Description: PyRates
         =======
@@ -81,19 +81,33 @@
         
         Documentation
         =============
         
         For a full API of PyRates, see https://pyrates.readthedocs.io/en/latest/.
         For examplary simulations and model configurations, please have a look at the jupyter notebooks provided in the documenation folder.
         
-        Reference
-        =========
+        References
+        ==========
         
         If you use this framework, please cite:
-        [Gast, R., Rose, D., Salomon, C., Möller, H. E., Weiskopf, N., & Knösche, T. R. (2019). PyRates-A Python framework for rate-based neural simulations. PloS one, 14(12), e0225900.](https://doi.org/10.1371/journal.pone.0225900)
+        
+        [Gast, R., Knösche, T. R. & Kennedy, A. (2023). PyRates - A Code-Generation Tool for Dynamical Systems Modeling. arXiv:2302.03763.](https://arxiv.org/abs/2302.03763)
+        
+        and
+        
+        [Gast, R., Rose, D., Salomon, C., Möller, H. E., Weiskopf, N., & Knösche, T. R. (2019). PyRates-A Python framework for rate-based neural simulations. PloS one, 14(12):e0225900.](https://doi.org/10.1371/journal.pone.0225900)
+        
+        Other work that used PyRates:
+        
+        [Weise, K., Poßner, L., Müller, E., Gast, R. & Knösche, T. R. (2020) Software X, 11:100450.](https://www.sciencedirect.com/science/article/pii/S2352711020300078)
+        
+        [Gast, R., Gong, R., Schmidt, H., Meijer, H.G.E., & Knösche, T.R. (2021) On the Role of Arkypallidal and Prototypical Neurons for Phase Transitions in the External Pallidum. Journal of Neuroscience, 41(31):6673-6683.](https://www.jneurosci.org/content/41/31/6673.abstract)
+        
+        [Gast, R., Solla, S.A. & Kennedy, A. (2023). Macroscopic dynamics of neural networks with heterogeneous spiking thresholds. Physical Review E, 107(2):024306.](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.107.024306)
+        
         
         Contact
         =======
         
         If you have questions, problems or suggestions regarding PyRates, please contact [Richard Gast](https://www.richardgast.me).
         
 Platform: UNKNOWN
```

### Comparing `pyrates-1.0.0/README.md` & `pyrates-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -73,17 +73,31 @@
 
 Documentation
 =============
 
 For a full API of PyRates, see https://pyrates.readthedocs.io/en/latest/.
 For examplary simulations and model configurations, please have a look at the jupyter notebooks provided in the documenation folder.
 
-Reference
-=========
+References
+==========
 
 If you use this framework, please cite:
-[Gast, R., Rose, D., Salomon, C., Möller, H. E., Weiskopf, N., & Knösche, T. R. (2019). PyRates-A Python framework for rate-based neural simulations. PloS one, 14(12), e0225900.](https://doi.org/10.1371/journal.pone.0225900)
+
+[Gast, R., Knösche, T. R. & Kennedy, A. (2023). PyRates - A Code-Generation Tool for Dynamical Systems Modeling. arXiv:2302.03763.](https://arxiv.org/abs/2302.03763)
+
+and
+
+[Gast, R., Rose, D., Salomon, C., Möller, H. E., Weiskopf, N., & Knösche, T. R. (2019). PyRates-A Python framework for rate-based neural simulations. PloS one, 14(12):e0225900.](https://doi.org/10.1371/journal.pone.0225900)
+
+Other work that used PyRates:
+
+[Weise, K., Poßner, L., Müller, E., Gast, R. & Knösche, T. R. (2020) Software X, 11:100450.](https://www.sciencedirect.com/science/article/pii/S2352711020300078)
+
+[Gast, R., Gong, R., Schmidt, H., Meijer, H.G.E., & Knösche, T.R. (2021) On the Role of Arkypallidal and Prototypical Neurons for Phase Transitions in the External Pallidum. Journal of Neuroscience, 41(31):6673-6683.](https://www.jneurosci.org/content/41/31/6673.abstract)
+
+[Gast, R., Solla, S.A. & Kennedy, A. (2023). Macroscopic dynamics of neural networks with heterogeneous spiking thresholds. Physical Review E, 107(2):024306.](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.107.024306)
+
 
 Contact
 =======
 
 If you have questions, problems or suggestions regarding PyRates, please contact [Richard Gast](https://www.richardgast.me).
```

### Comparing `pyrates-1.0.0/model_templates/CNS_2019_Tutorial/templates.yaml` & `pyrates-1.0.1/model_templates/CNS_2019_Tutorial/templates.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/model_templates/base_templates.yaml` & `pyrates-1.0.1/model_templates/base_templates.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/model_templates/neural_mass_models/__init__.py` & `pyrates-1.0.1/model_templates/neural_mass_models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/model_templates/neural_mass_models/ik.yaml` & `pyrates-1.0.1/model_templates/neural_mass_models/ik.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -60,23 +60,24 @@
     r_in: input(0.0)
 
 # biophysical izhikevich model with distributed spike thresholds
 ik_theta_op:
   base: OperatorTemplate
   equations:
     - "r' = (Delta*k^2*(v-v_r)/(pi*C) + r*(k*(2.0*v - v_r - v_t) - g*s)) / C"
-    - "v' = (k*v*(v - v_r - v_t) + k*v_r*v_t + I_ext - u + g*s*(E_r - v) - pi*C*r*(Delta + pi*C*r/k)) / C"
+    - "v' = (k*v*(v - v_r - v_t) + k*v_r*v_t + I_ext + eta - u + g*s*(E_r - v) - pi*C*r*(Delta + pi*C*r/k)) / C"
     - "u' = a*(b*(v-v_r) - u) + d*r"
     - "s' = -s/tau_s + r_in"
   variables:
     r: output(0.0)
     v: variable(-60.0)
     u: variable(0.0)
     s: variable(0.0)
     Delta: 0.02
+    eta: 0.0
     k: 1.0
     C: 100.0
     v_r: -70.0
     v_t: -40.0
     g: 0.5
     E_r: 0.0
     b: -0.01
```

### Comparing `pyrates-1.0.0/model_templates/neural_mass_models/jansenrit.yaml` & `pyrates-1.0.1/model_templates/neural_mass_models/jansenrit.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/model_templates/neural_mass_models/qif.yaml` & `pyrates-1.0.1/model_templates/neural_mass_models/qif.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/model_templates/neural_mass_models/synaptic_plasticity.yaml` & `pyrates-1.0.1/model_templates/neural_mass_models/synaptic_plasticity.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/model_templates/neural_mass_models/theta.yaml` & `pyrates-1.0.1/model_templates/neural_mass_models/theta.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/model_templates/neural_mass_models/wilsoncowan.yaml` & `pyrates-1.0.1/model_templates/neural_mass_models/wilsoncowan.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/model_templates/oscillators/__init__.py` & `pyrates-1.0.1/model_templates/oscillators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/model_templates/oscillators/kuramoto.yaml` & `pyrates-1.0.1/model_templates/oscillators/kuramoto.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/model_templates/oscillators/stuartlandau.yaml` & `pyrates-1.0.1/model_templates/oscillators/stuartlandau.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/model_templates/test_resources/linear.yaml` & `pyrates-1.0.1/model_templates/test_resources/linear.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/model_templates/test_resources/test_backend.yaml` & `pyrates-1.0.1/model_templates/test_resources/test_backend.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/model_templates/test_resources/test_operator_caching_templates.yml` & `pyrates-1.0.1/model_templates/test_resources/test_operator_caching_templates.yml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/__init__.py` & `pyrates-1.0.1/pyrates/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,12 +28,12 @@
 # Richard Gast and Daniel Rose et. al. in preparation
 """Python package for building and simulating complex dynamical systems. Represents the dynamical systems as graphs,
 i.e. networks of nodes connected via edges.
 """
 
 __author__ = "Richard Gast, Daniel Rose"
 __status__ = "Development"
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 
 from pyrates.utility import integrate, grid_search, clear_frontend_caches, clear
 from pyrates.frontend import CircuitTemplate, NodeTemplate, EdgeTemplate, OperatorTemplate, save
```

### Comparing `pyrates-1.0.0/pyrates/backend/__init__.py` & `pyrates-1.0.1/pyrates/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/base/__init__.py` & `pyrates-1.0.1/pyrates/backend/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/base/base_backend.py` & `pyrates-1.0.1/pyrates/backend/base/base_backend.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/base/base_funcs.py` & `pyrates-1.0.1/pyrates/backend/base/base_funcs.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/computegraph.py` & `pyrates-1.0.1/pyrates/backend/computegraph.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/fortran/__init__.py` & `pyrates-1.0.1/pyrates/backend/fortran/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/fortran/fortran_backend.py` & `pyrates-1.0.1/pyrates/backend/fortran/fortran_backend.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/fortran/fortran_funcs.py` & `pyrates-1.0.1/pyrates/backend/fortran/fortran_funcs.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/julia/__init__.py` & `pyrates-1.0.1/pyrates/backend/julia/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/julia/julia_backend.py` & `pyrates-1.0.1/pyrates/backend/julia/julia_backend.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/julia/julia_funcs.py` & `pyrates-1.0.1/pyrates/backend/julia/julia_funcs.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/matlab/__init__.py` & `pyrates-1.0.1/pyrates/backend/matlab/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/matlab/matlab_backend.py` & `pyrates-1.0.1/pyrates/backend/matlab/matlab_backend.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/matlab/matlab_funcs.py` & `pyrates-1.0.1/pyrates/backend/matlab/matlab_funcs.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/parser.py` & `pyrates-1.0.1/pyrates/backend/parser.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/tensorflow/__init__.py` & `pyrates-1.0.1/pyrates/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/tensorflow/tensorflow_backend.py` & `pyrates-1.0.1/pyrates/backend/tensorflow/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/tensorflow/tensorflow_funcs.py` & `pyrates-1.0.1/pyrates/backend/tensorflow/tensorflow_funcs.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/torch/__init__.py` & `pyrates-1.0.1/pyrates/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/torch/torch_backend.py` & `pyrates-1.0.1/pyrates/backend/torch/torch_backend.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/backend/torch/torch_funcs.py` & `pyrates-1.0.1/pyrates/backend/torch/torch_funcs.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/frontend/__init__.py` & `pyrates-1.0.1/pyrates/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/frontend/dict.py` & `pyrates-1.0.1/pyrates/frontend/dict.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/frontend/file.py` & `pyrates-1.0.1/pyrates/frontend/file.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/frontend/fileio/__init__.py` & `pyrates-1.0.1/pyrates/frontend/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/frontend/fileio/yaml.py` & `pyrates-1.0.1/pyrates/frontend/fileio/yaml.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/frontend/template/__init__.py` & `pyrates-1.0.1/pyrates/frontend/template/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/frontend/template/_io.py` & `pyrates-1.0.1/pyrates/frontend/template/_io.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/frontend/template/abc.py` & `pyrates-1.0.1/pyrates/frontend/template/abc.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/frontend/template/circuit.py` & `pyrates-1.0.1/pyrates/frontend/template/circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,27 +283,29 @@
         # updates to edge variable values
         for source, target, edge_dict in edge_vars:
             _, _, _, base_dict = self.get_edge(source, target)
             base_dict.update(edge_dict)
 
         return self
 
-    def add_edges_from_matrix(self, source_var: str, target_var: str, nodes: list, weight=None, template=None,
-                              edge_attr: dict = None, min_weight: float = 1e-6) -> None:
+    def add_edges_from_matrix(self, source_var: str, target_var: str, source_nodes: list, target_nodes: list = None,
+                              weight=None, template=None, edge_attr: dict = None, min_weight: float = 1e-6) -> None:
         """Adds all possible edges between the `source_var` and `target_var` of all passed `nodes`. `Weight` and `Delay`
         need to be arrays containing scalars for each of those edges.
 
         Parameters
         ----------
         source_var
             Pointer to a variable on the source nodes ('op/var').
         target_var
             Pointer to a variable on the target nodes ('op/var').
-        nodes
-            List of node names that should be connected to each other
+        source_nodes
+            List of node names from which to extract the source variable.
+        target_nodes
+            List of node names to which to project the source variable. If `None`, `source_nodes` will be used instead.
         weight
             Optional N x N matrix with edge weights (N = number of nodes). If not passed, all edges receive a weight of
             1.0.
         template
             Can be link to edge template that should be used for each edge.
         edge_attr
             Additional edge attributes. Can either be N x N matrices or other scalars/objects.
@@ -314,21 +316,23 @@
         -------
         None
 
         """
 
         if edge_attr is None:
             edge_attr = dict()
+        if target_nodes is None:
+            target_nodes = source_nodes
 
         # construct edge attribute dictionary from arguments
         ####################################################
 
         # weights and delays
         if weight is None:
-            weight = np.ones((len(nodes), len(nodes)))
+            weight = np.ones((len(target_nodes), len(source_nodes)))
         edge_attributes = {'weight': weight}
 
         # add rest of the attributes
         edge_attributes.update(edge_attr)
 
         # construct edges list
         ######################
@@ -337,24 +341,19 @@
         matrix_attributes = dict()
         for key, attr in edge_attributes.copy().items():
             if hasattr(attr, 'shape') and len(attr.shape) >= 2:
                 matrix_attributes[key] = edge_attributes.pop(key)
 
         # create edge list
         edges = []
-        for i, source in enumerate(nodes):
-            for j, target in enumerate(nodes):
+        for i, source in enumerate(source_nodes):
+            for j, target in enumerate(target_nodes):
 
                 if np.abs(weight[j, i]) > min_weight:
 
-                    if source not in self.nodes:
-                        raise ValueError(f'Node {source} is not defined on this CircuitTemplate instance.')
-                    if target not in self.nodes:
-                        raise ValueError(f'Node {target} is not defined on this CircuitTemplate instance.')
-
                     edge_attributes_tmp = {}
 
                     # extract edge attribute value from matrices
                     for key, attr in matrix_attributes.items():
                         edge_attributes_tmp[key] = attr[j, i]
 
                     # add remaining attributes
```

### Comparing `pyrates-1.0.0/pyrates/frontend/template/edge.py` & `pyrates-1.0.1/pyrates/frontend/template/edge.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/frontend/template/edge.yaml` & `pyrates-1.0.1/pyrates/frontend/template/edge.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/frontend/template/node.py` & `pyrates-1.0.1/pyrates/frontend/template/node.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/frontend/template/operator.py` & `pyrates-1.0.1/pyrates/frontend/template/operator.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/frontend/template/operator_graph.py` & `pyrates-1.0.1/pyrates/frontend/template/operator_graph.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/ir/__init__.py` & `pyrates-1.0.1/pyrates/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/ir/abc.py` & `pyrates-1.0.1/pyrates/ir/abc.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/ir/circuit.py` & `pyrates-1.0.1/pyrates/ir/circuit.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/ir/edge.py` & `pyrates-1.0.1/pyrates/ir/edge.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/ir/node.py` & `pyrates-1.0.1/pyrates/ir/node.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/ir/operator.py` & `pyrates-1.0.1/pyrates/ir/operator.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/ir/operator_graph.py` & `pyrates-1.0.1/pyrates/ir/operator_graph.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/pyrates/utility.py` & `pyrates-1.0.1/pyrates/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         Simulation results stored in a multi-index data frame, and the mapping between the data frame column names and
         the parameter grid.
     """
 
     # argument pre-processing
     #########################
 
-    vectorization = kwargs.pop('vectorization', True)
+    vectorize = kwargs.pop('vectorize', True)
 
     # linearize parameter grid if necessary
     if type(param_grid) is dict:
         param_grid = linearize_grid(param_grid, permute_grid)
 
     # create grid-structure of network
     ##################################
@@ -264,24 +264,17 @@
 
     # simulate the circuits behavior
     results = circuit.run(simulation_time=simulation_time,
                           step_size=step_size,
                           sampling_step_size=sampling_step_size,
                           inputs=inputs,
                           outputs=outputs_new,
-                          vectorization=vectorization,
+                          vectorize=vectorize,
                           **kwargs)    # type: pd.DataFrame
 
-    # # create dataframe that maps between output names and parameter sets
-    # data, index = [], []
-    # for key in results.keys():
-    #     param_key = key[1].split('/')[0]
-    #     data.append(param_grid.loc[param_key, :].values)
-    # param_map = pd.DataFrame(data=np.asarray(data).T, columns=results.columns, index=param_grid.columns)
-
     # return results
     return results, param_grid
 
 
 class Interactive2DParamPlot(object):
     def __init__(self, data_map: np.array, data_series: pd.DataFrame, x_values: np.array, y_values: np.array,
                  x_key: str, y_key: str, param_map: pd.DataFrame, tmin=0., title=None, **kwargs):
```

### Comparing `pyrates-1.0.0/pyrates.egg-info/PKG-INFO` & `pyrates-1.0.1/pyrates.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrates
-Version: 1.0.0
+Version: 1.0.1
 Summary: Dynamical Systems Modeling Framework
 Home-page: UNKNOWN
 Author: Richard Gast, Daniel Rose
 Author-email: richard.gast@northwestern.edu
 License: GPL v3
 Description: PyRates
         =======
@@ -81,19 +81,33 @@
         
         Documentation
         =============
         
         For a full API of PyRates, see https://pyrates.readthedocs.io/en/latest/.
         For examplary simulations and model configurations, please have a look at the jupyter notebooks provided in the documenation folder.
         
-        Reference
-        =========
+        References
+        ==========
         
         If you use this framework, please cite:
-        [Gast, R., Rose, D., Salomon, C., Möller, H. E., Weiskopf, N., & Knösche, T. R. (2019). PyRates-A Python framework for rate-based neural simulations. PloS one, 14(12), e0225900.](https://doi.org/10.1371/journal.pone.0225900)
+        
+        [Gast, R., Knösche, T. R. & Kennedy, A. (2023). PyRates - A Code-Generation Tool for Dynamical Systems Modeling. arXiv:2302.03763.](https://arxiv.org/abs/2302.03763)
+        
+        and
+        
+        [Gast, R., Rose, D., Salomon, C., Möller, H. E., Weiskopf, N., & Knösche, T. R. (2019). PyRates-A Python framework for rate-based neural simulations. PloS one, 14(12):e0225900.](https://doi.org/10.1371/journal.pone.0225900)
+        
+        Other work that used PyRates:
+        
+        [Weise, K., Poßner, L., Müller, E., Gast, R. & Knösche, T. R. (2020) Software X, 11:100450.](https://www.sciencedirect.com/science/article/pii/S2352711020300078)
+        
+        [Gast, R., Gong, R., Schmidt, H., Meijer, H.G.E., & Knösche, T.R. (2021) On the Role of Arkypallidal and Prototypical Neurons for Phase Transitions in the External Pallidum. Journal of Neuroscience, 41(31):6673-6683.](https://www.jneurosci.org/content/41/31/6673.abstract)
+        
+        [Gast, R., Solla, S.A. & Kennedy, A. (2023). Macroscopic dynamics of neural networks with heterogeneous spiking thresholds. Physical Review E, 107(2):024306.](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.107.024306)
+        
         
         Contact
         =======
         
         If you have questions, problems or suggestions regarding PyRates, please contact [Richard Gast](https://www.richardgast.me).
         
 Platform: UNKNOWN
```

### Comparing `pyrates-1.0.0/pyrates.egg-info/SOURCES.txt` & `pyrates-1.0.1/pyrates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/setup.py` & `pyrates-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/tests/__init__.py` & `pyrates-1.0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/tests/benchmarks.py` & `pyrates-1.0.1/tests/benchmarks.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/tests/conftest.py` & `pyrates-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/tests/test_backend_parser.py` & `pyrates-1.0.1/tests/test_backend_parser.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/tests/test_backend_simulations.py` & `pyrates-1.0.1/tests/test_backend_simulations.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/tests/test_file_io.py` & `pyrates-1.0.1/tests/test_file_io.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.0/tests/test_frontend.py` & `pyrates-1.0.1/tests/test_frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
     # add the edges
     edge = EdgeTemplate.from_yaml("model_templates.oscillators.kuramoto.sin_edge")
     weights = np.random.randn(n, n)
     delays = np.random.uniform(low=1, high=2, size=(n, n))
     edge_attr = {'sin_edge/coupling_op/theta_s': 'source', 'sin_edge/coupling_op/theta_t': 'p2/phase_op/theta',
                  'delay': delays}
-    circuit.add_edges_from_matrix(source_var='phase_op/theta', target_var='phase_op/s_in', nodes=node_names,
+    circuit.add_edges_from_matrix(source_var='phase_op/theta', target_var='phase_op/s_in', source_nodes=node_names,
                                   weight=weights, template=edge, edge_attr=edge_attr, min_weight=0.0)
 
     # test whether edges have been added as expected
     edge_attr_tmp = deepcopy(edge_attr)
     edge_attr_tmp['weight'] = weights[1, 2]
     edge_attr_tmp['delay'] = delays[1, 2]
     assert len(circuit.edges) == int(n**2)
```

### Comparing `pyrates-1.0.0/tests/test_implemented_models.py` & `pyrates-1.0.1/tests/test_implemented_models.py`

 * *Files identical despite different names*

