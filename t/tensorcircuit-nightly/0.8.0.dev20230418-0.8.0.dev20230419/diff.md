# Comparing `tmp/tensorcircuit-nightly-0.8.0.dev20230418.tar.gz` & `tmp/tensorcircuit-nightly-0.8.0.dev20230419.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.8.0.dev20230418.tar", last modified: Tue Apr 18 12:40:08 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.8.0.dev20230419.tar", last modified: Wed Apr 19 12:41:21 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.8.0.dev20230418.tar` & `tensorcircuit-nightly-0.8.0.dev20230419.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.415832 tensorcircuit-nightly-0.8.0.dev20230418/
--rw-r--r--   0 runner    (1001) docker     (122)    23109 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-18 12:40:08.411832 tensorcircuit-nightly-0.8.0.dev20230418/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.403832 tensorcircuit-nightly-0.8.0.dev20230418/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.403832 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27001 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6229 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-18 12:40:08.415832 tensorcircuit-nightly-0.8.0.dev20230418/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-04-18 12:40:03.000000 tensorcircuit-nightly-0.8.0.dev20230418/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.407832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-04-18 12:40:03.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.407832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.407832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    56998 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14944 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24632 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    30672 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36236 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.407832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17566 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.407832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    28754 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29161 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.411832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     9942 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     5032 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     9975 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34398 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11878 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.411832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31378 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.411832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27351 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.411832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-18 12:40:08.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3438 2023-04-18 12:40:08.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 12:40:08.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-18 12:40:08.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-18 12:40:08.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.411832 tensorcircuit-nightly-0.8.0.dev20230418/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33200 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    45826 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13296 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:41:21.863269 tensorcircuit-nightly-0.8.0.dev20230419/
+-rw-r--r--   0 runner    (1001) docker     (122)    23108 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-19 12:41:21.863269 tensorcircuit-nightly-0.8.0.dev20230419/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:41:21.851269 tensorcircuit-nightly-0.8.0.dev20230419/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:41:21.851269 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27001 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 12:41:21.863269 tensorcircuit-nightly-0.8.0.dev20230419/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-04-19 12:41:16.000000 tensorcircuit-nightly-0.8.0.dev20230419/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:41:21.855269 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-04-19 12:41:16.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:41:21.855269 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:41:21.859269 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56998 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14944 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24632 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30672 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36236 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:41:21.859269 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17566 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:41:21.859269 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28754 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29161 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:41:21.859269 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9942 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5046 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9975 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34398 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11878 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:41:21.859269 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31378 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:41:21.859269 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27351 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:41:21.863269 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-19 12:41:21.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3438 2023-04-19 12:41:21.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 12:41:21.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-19 12:41:21.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-19 12:41:21.000000 tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:41:21.863269 tensorcircuit-nightly-0.8.0.dev20230419/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33200 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45826 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13296 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-04-19 12:17:08.000000 tensorcircuit-nightly-0.8.0.dev20230419/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/CHANGELOG.md` & `tensorcircuit-nightly-0.8.0.dev20230419/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Change Log
 
 ## Unreleased
 
 ### Added
 
-- Add `tc.about()` to print related software versions and configs.
+- Add `tc.about()` to print related software versions and configs
 
 - Torch support is updraded to 2.0, and now support native vmap and native functional grad, and thus `vvag`. Still jit support is conflict with these functional transformations and be turned off by default
 
 - Add `torch_interfaces_kws` that support static keyword arguments when wrapping with the interface
 
 ### Fixed
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/HISTORY.md` & `tensorcircuit-nightly-0.8.0.dev20230419/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/LICENSE` & `tensorcircuit-nightly-0.8.0.dev20230419/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/PKG-INFO` & `tensorcircuit-nightly-0.8.0.dev20230419/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.8.0.dev20230418
+Version: 0.8.0.dev20230419
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/README.md` & `tensorcircuit-nightly-0.8.0.dev20230419/README.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/README_cn.md` & `tensorcircuit-nightly-0.8.0.dev20230419/README_cn.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/advance.rst` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/cnconf.py` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/conf.py` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/contribution.rst` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/faq.rst` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/index.rst` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/infras.rst` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/modules.rst` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/sharpbits.rst`

 * *Files 19% similar despite different names*

```diff
@@ -137,14 +137,61 @@
         c.conditional_gate(a, [tc.gates.z(), tc.gates.x()], 0)
         return c.state()
 
     f()
     # <tf.Tensor: shape=(2,), dtype=complex64, numpy=array([0.99999994+0.j, 0.        +0.j], dtype=complex64)>
 
 
+Tensor variables consistency
+-------------------------------------------------------
+
+
+All tensor variables' backend (tf vs jax vs ..), dtype (float vs complex), shape and device (cpu vs gpu) must be compatible/consistent.
+
+Inspect the backend, dtype, shape and device using the following codes.
+
+.. code-block:: python
+
+    for backend in ["numpy", "tensorflow", "jax", "pytorch"]:
+        with tc.runtime_backend(backend):
+            a = tc.backend.ones([2, 3])
+            print("tensor backend:", tc.interfaces.which_backend(a))
+            print("tensor dtype:", tc.backend.dtype(a))
+            print("tensor shape:", tc.backend.shape_tuple(a))
+            print("tensor device:", tc.backend.device(a))
+
+If the backend is inconsistent, one can convert the tensor backend via :py:meth:`tensorcircuit.interfaces.tensortrans.general_args_to_backend`.
+
+.. code-block:: python
+
+    for backend in ["numpy", "tensorflow", "jax", "pytorch"]:
+        with tc.runtime_backend(backend):
+            a = tc.backend.ones([2, 3])
+            print("tensor backend:", tc.interfaces.which_backend(a))
+            b = tc.interfaces.general_args_to_backend(a, target_backend="jax", enable_dlpack=False)
+            print("tensor backend:", tc.interfaces.which_backend(b))
+
+If the dtype is inconsistent, one can convert the tensor dtype using ``tc.backend.cast``.
+
+.. code-block:: python
+
+    for backend in ["numpy", "tensorflow", "jax", "pytorch"]:
+        with tc.runtime_backend(backend):
+            a = tc.backend.ones([2, 3])
+            print("tensor dtype:", tc.backend.dtype(a))
+            b = tc.backend.cast(a, dtype="float64")
+            print("tensor dtype:", tc.backend.dtype(b))
+
+Also note the jax issue on float64/complex128, see `jax gotcha <https://github.com/google/jax#current-gotchas>`_.
+
+If the shape is not consistent, one can convert the shape by ``tc.backend.reshape``.
+
+If the device is not consistent, one can move the tensor between devices by ``tc.backend.device_move``.
+
+
 AD Consistency
 ---------------------
 
 TF and JAX backend manage the differentiation rules differently for complex-valued function (actually up to a complex conjuagte). See issue discussion `tensorflow issue <https://github.com/tensorflow/tensorflow/issues/3348>`_.
 
 In TensorCircuit, currently we make the difference in AD transparent, namely, when switching the backend, the AD behavior and result for complex valued function can be different and determined by the nature behavior of the corresponding backend framework.
 All AD relevant ops such as ``grad`` or ``jacrev`` may be affected. Therefore, the user must be careful when dealing with AD on complex valued function in a backend agnostic way in TensorCircuit.
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/tutorial.rst`

 * *Files 18% similar despite different names*

```diff
@@ -15,8 +15,9 @@
     tutorials/mera.ipynb
     tutorials/gradient_benchmark.ipynb
     tutorials/contractors.ipynb
     tutorials/operator_spreading.ipynb
     tutorials/optimization_and_expressibility.ipynb
     tutorials/vqex_mbl.ipynb
     tutorials/dqas.ipynb
-    tutorials/barren_plateaus.ipynb
+    tutorials/barren_plateaus.ipynb
+    tutorials/qaoa_portfolio_optimization.ipynb
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.8.0.dev20230419/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/setup.py` & `tensorcircuit-nightly-0.8.0.dev20230419/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0.dev20230418"
+__version__ = "0.8.0.dev20230419"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .about import about
 from .cons import (
     backend,
     set_backend,
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/about.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/jax_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cloud/apis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cloud/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/interfaces/torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
         def f(tensor, integer):
             r = 0.
             for i in range(integer):
                 r += tensor
             return r
 
-        fnew = torch_interface_kws(f)
+        fnew = tc.interfaces.torch_interface_kws(f)
 
         print(fnew(torch.ones([2]), integer=3))
         print(fnew(torch.ones([2]), integer=4))
 
     :param f: _description_
     :type f: Callable[..., Any]
     :param jit: _description_, defaults to True
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.8.0.dev20230418
+Version: 0.8.0.dev20230419
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.8.0.dev20230419/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/conftest.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_backends.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_calibrating.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_channels.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_circuit.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_ensemble.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_gates.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_interfaces.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_keras.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_miscs.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_qaoa.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_quantum.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_results.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_simplify.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_templates.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_torchnn.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_van.py` & `tensorcircuit-nightly-0.8.0.dev20230419/tests/test_van.py`

 * *Files identical despite different names*

