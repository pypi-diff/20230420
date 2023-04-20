# Comparing `tmp/phiflow-2.3.3.tar.gz` & `tmp/phiflow-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiflow-2.3.3.tar", last modified: Thu Apr 13 11:47:15 2023, max compression
+gzip compressed data, was "dist\phiflow-2.3.4.tar", last modified: Thu Apr 20 17:29:57 2023, max compression
```

## Comparing `phiflow-2.3.3.tar` & `phiflow-2.3.4.tar`

### file list

```diff
@@ -1,121 +1,116 @@
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.781157 phiflow-2.3.3/
--rw-rw-r--   0 holl      (1001) holl      (1001)     1085 2022-01-28 11:41:32.000000 phiflow-2.3.3/LICENSE.txt
--rw-rw-r--   0 holl      (1001) holl      (1001)       95 2022-08-29 12:54:06.000000 phiflow-2.3.3/MANIFEST.in
--rw-rw-r--   0 holl      (1001) holl      (1001)     2290 2023-04-13 11:47:15.781157 phiflow-2.3.3/PKG-INFO
--rw-rw-r--   0 holl      (1001) holl      (1001)     8330 2023-04-13 11:46:51.000000 phiflow-2.3.3/README.md
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.769157 phiflow-2.3.3/phi/
--rw-rw-r--   0 holl      (1001) holl      (1001)        5 2023-04-13 11:46:55.000000 phiflow-2.3.3/phi/VERSION
--rw-rw-r--   0 holl      (1001) holl      (1001)     1944 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     8988 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/_troubleshoot.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.773157 phiflow-2.3.3/phi/field/
--rw-rw-r--   0 holl      (1001) holl      (1001)     2349 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/field/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     2486 2023-04-11 10:15:31.000000 phiflow-2.3.3/phi/field/_angular_velocity.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3553 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/field/_embed.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    17860 2023-04-13 11:46:55.000000 phiflow-2.3.3/phi/field/_field.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     5093 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/field/_field_io.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    40385 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/field/_field_math.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    33090 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/field/_grid.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     1554 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/field/_mask.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     2837 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/field/_noise.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    12374 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/field/_point_cloud.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    21224 2023-04-13 11:46:55.000000 phiflow-2.3.3/phi/field/_scene.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     1549 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/flow.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.773157 phiflow-2.3.3/phi/geom/
--rw-rw-r--   0 holl      (1001) holl      (1001)      538 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/geom/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    21213 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/geom/_box.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    19879 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/geom/_geom.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     4410 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/geom/_sphere.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3929 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/geom/_stack.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     7884 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/geom/_transform.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3458 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/geom/_union.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.773157 phiflow-2.3.3/phi/jax/
--rw-rw-r--   0 holl      (1001) holl      (1001)      463 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/jax/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    20030 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/jax/_jax_backend.py
--rw-rw-r--   0 holl      (1001) holl      (1001)      907 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/jax/flow.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.773157 phiflow-2.3.3/phi/jax/stax/
--rw-rw-r--   0 holl      (1001) holl      (1001)        0 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/jax/stax/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)      795 2023-03-30 12:42:58.000000 phiflow-2.3.3/phi/jax/stax/flow.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    46153 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/jax/stax/nets.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.773157 phiflow-2.3.3/phi/math/
--rw-rw-r--   0 holl      (1001) holl      (1001)     4221 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3842 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/math/_fit.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    56756 2023-04-13 11:46:55.000000 phiflow-2.3.3/phi/math/_functional.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    35805 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/_magic_ops.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    32322 2023-03-30 12:42:58.000000 phiflow-2.3.3/phi/math/_nd.py
--rw-rw-r--   0 holl      (1001) holl      (1001)   109536 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/_ops.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    33258 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/_optimize.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    73037 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/_shape.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    37387 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/_sparse.py
--rw-rw-r--   0 holl      (1001) holl      (1001)   109308 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/_tensors.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    18437 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/_trace.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/math/backend/
--rw-rw-r--   0 holl      (1001) holl      (1001)      787 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/math/backend/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    58953 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/backend/_backend.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     6140 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/math/backend/_dtype.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    22293 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/math/backend/_linalg.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     9054 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/math/backend/_minimize.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    21102 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/backend/_numpy_backend.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    22448 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/math/backend/_profile.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    59061 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/extrapolation.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    31605 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/math/magic.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    15528 2022-08-30 18:09:37.000000 phiflow-2.3.3/phi/net.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/physics/
--rw-rw-r--   0 holl      (1001) holl      (1001)      480 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/physics/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    18206 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/physics/_boundaries.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     8446 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/physics/advect.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     4795 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/physics/diffuse.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    15513 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/physics/fluid.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/tf/
--rw-rw-r--   0 holl      (1001) holl      (1001)     1224 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/tf/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     4228 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/tf/_compile_cuda.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     2085 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/tf/_profiling.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    29887 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/tf/_tf_backend.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3280 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/tf/_tf_cuda_resample.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.769157 phiflow-2.3.3/phi/tf/cuda/
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/tf/cuda/build/
--rw-rw-r--   0 holl      (1001) holl      (1001)   888280 2022-08-08 09:28:29.000000 phiflow-2.3.3/phi/tf/cuda/build/resample.cu.o
--rw-rw-r--   0 holl      (1001) holl      (1001)     1175 2023-03-30 12:42:58.000000 phiflow-2.3.3/phi/tf/flow.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    34671 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/tf/nets.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/torch/
--rw-rw-r--   0 holl      (1001) holl      (1001)      498 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/torch/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    55629 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/torch/_torch_backend.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     1145 2023-03-30 12:42:58.000000 phiflow-2.3.3/phi/torch/flow.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    39365 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/torch/nets.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/vis/
--rw-rw-r--   0 holl      (1001) holl      (1001)     1089 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/__init__.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/vis/_console/
--rw-rw-r--   0 holl      (1001) holl      (1001)       36 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_console/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     6865 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_console/_console_gui.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3140 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/vis/_console/_console_plot.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     2360 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_console/_console_util.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/vis/_dash/
--rw-rw-r--   0 holl      (1001) holl      (1001)        0 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_dash/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    21970 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_dash/_plotly_plots.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     7826 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/vis/_dash/board.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     4222 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_dash/colormaps.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     2954 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_dash/dash_app.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     7143 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/vis/_dash/dash_gui.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     2075 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_dash/info.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     1228 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_dash/log.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     5359 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/vis/_dash/model_controls.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3462 2022-08-02 08:31:06.000000 phiflow-2.3.3/phi/vis/_dash/player_controls.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     2710 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/vis/_dash/viewer.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     5890 2023-04-13 08:09:47.000000 phiflow-2.3.3/phi/vis/_dash/viewsettings.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     3016 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_log.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.777157 phiflow-2.3.3/phi/vis/_matplotlib/
--rw-rw-r--   0 holl      (1001) holl      (1001)      108 2023-03-13 10:22:43.000000 phiflow-2.3.3/phi/vis/_matplotlib/__init__.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    23769 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_matplotlib/_matplotlib_plots.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     7426 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_matplotlib/_scalars.py
--rw-rw-r--   0 holl      (1001) holl      (1001)      793 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_plot_util.py
--rw-rw-r--   0 holl      (1001) holl      (1001)     7184 2022-08-29 12:54:06.000000 phiflow-2.3.3/phi/vis/_user_namespace.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    10673 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_viewer.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    26967 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_vis.py
--rw-rw-r--   0 holl      (1001) holl      (1001)    17042 2023-04-13 11:46:51.000000 phiflow-2.3.3/phi/vis/_vis_base.py
-drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2023-04-13 11:47:15.781157 phiflow-2.3.3/phiflow.egg-info/
--rw-rw-r--   0 holl      (1001) holl      (1001)     2290 2023-04-13 11:47:15.000000 phiflow-2.3.3/phiflow.egg-info/PKG-INFO
--rw-rw-r--   0 holl      (1001) holl      (1001)     2333 2023-04-13 11:47:15.000000 phiflow-2.3.3/phiflow.egg-info/SOURCES.txt
--rw-rw-r--   0 holl      (1001) holl      (1001)        1 2023-04-13 11:47:15.000000 phiflow-2.3.3/phiflow.egg-info/dependency_links.txt
--rw-rw-r--   0 holl      (1001) holl      (1001)       30 2023-04-13 11:47:15.000000 phiflow-2.3.3/phiflow.egg-info/requires.txt
--rw-rw-r--   0 holl      (1001) holl      (1001)        4 2023-04-13 11:47:15.000000 phiflow-2.3.3/phiflow.egg-info/top_level.txt
--rw-rw-r--   0 holl      (1001) holl      (1001)       79 2023-04-13 11:47:15.781157 phiflow-2.3.3/setup.cfg
--rw-rw-r--   0 holl      (1001) holl      (1001)     7119 2023-03-13 10:22:43.000000 phiflow-2.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.395654 phiflow-2.3.4/
+-rw-rw-rw-   0        0        0       95 2022-04-20 10:42:57.000000 phiflow-2.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2453 2023-04-20 17:29:57.395654 phiflow-2.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8330 2023-02-26 20:09:34.000000 phiflow-2.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.075367 phiflow-2.3.4/phi/
+-rw-rw-rw-   0        0        0        5 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/VERSION
+-rw-rw-rw-   0        0        0     1944 2023-02-26 20:09:34.000000 phiflow-2.3.4/phi/__init__.py
+-rw-rw-rw-   0        0        0     8988 2023-02-26 20:09:34.000000 phiflow-2.3.4/phi/_troubleshoot.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.106392 phiflow-2.3.4/phi/field/
+-rw-rw-rw-   0        0        0     2349 2023-02-26 20:09:34.000000 phiflow-2.3.4/phi/field/__init__.py
+-rw-rw-rw-   0        0        0     2499 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/field/_angular_velocity.py
+-rw-rw-rw-   0        0        0     3553 2023-02-26 20:09:34.000000 phiflow-2.3.4/phi/field/_embed.py
+-rw-rw-rw-   0        0        0    17883 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/field/_field.py
+-rw-rw-rw-   0        0        0     5129 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/field/_field_io.py
+-rw-rw-rw-   0        0        0    40467 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/field/_field_math.py
+-rw-rw-rw-   0        0        0    33185 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/field/_grid.py
+-rw-rw-rw-   0        0        0     1584 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/field/_mask.py
+-rw-rw-rw-   0        0        0     2837 2023-02-26 20:09:34.000000 phiflow-2.3.4/phi/field/_noise.py
+-rw-rw-rw-   0        0        0    12380 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/field/_point_cloud.py
+-rw-rw-rw-   0        0        0    21286 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/field/_scene.py
+-rw-rw-rw-   0        0        0     1549 2023-03-17 11:48:14.000000 phiflow-2.3.4/phi/flow.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.131415 phiflow-2.3.4/phi/geom/
+-rw-rw-rw-   0        0        0      538 2023-01-12 19:29:54.000000 phiflow-2.3.4/phi/geom/__init__.py
+-rw-rw-rw-   0        0        0    21250 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/geom/_box.py
+-rw-rw-rw-   0        0        0    19954 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/geom/_geom.py
+-rw-rw-rw-   0        0        0     4456 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/geom/_sphere.py
+-rw-rw-rw-   0        0        0     3929 2023-02-26 20:09:34.000000 phiflow-2.3.4/phi/geom/_stack.py
+-rw-rw-rw-   0        0        0     7916 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/geom/_transform.py
+-rw-rw-rw-   0        0        0     3458 2023-02-26 20:09:34.000000 phiflow-2.3.4/phi/geom/_union.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.144427 phiflow-2.3.4/phi/jax/
+-rw-rw-rw-   0        0        0      463 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/jax/__init__.py
+-rw-rw-rw-   0        0        0    20075 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/jax/_jax_backend.py
+-rw-rw-rw-   0        0        0      907 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/jax/flow.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.151433 phiflow-2.3.4/phi/jax/stax/
+-rw-rw-rw-   0        0        0        0 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/jax/stax/__init__.py
+-rw-rw-rw-   0        0        0      795 2023-03-17 11:48:14.000000 phiflow-2.3.4/phi/jax/stax/flow.py
+-rw-rw-rw-   0        0        0    46154 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/jax/stax/nets.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.179459 phiflow-2.3.4/phi/math/
+-rw-rw-rw-   0        0        0     4221 2023-04-04 14:12:05.000000 phiflow-2.3.4/phi/math/__init__.py
+-rw-rw-rw-   0        0        0     3842 2023-02-26 18:31:51.000000 phiflow-2.3.4/phi/math/_fit.py
+-rw-rw-rw-   0        0        0    57009 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/_functional.py
+-rw-rw-rw-   0        0        0    35833 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/_magic_ops.py
+-rw-rw-rw-   0        0        0    32377 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/_nd.py
+-rw-rw-rw-   0        0        0   109916 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/_ops.py
+-rw-rw-rw-   0        0        0    33308 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/_optimize.py
+-rw-rw-rw-   0        0        0    73123 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/_shape.py
+-rw-rw-rw-   0        0        0    37406 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/_sparse.py
+-rw-rw-rw-   0        0        0   109375 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/_tensors.py
+-rw-rw-rw-   0        0        0    18445 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/_trace.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.200477 phiflow-2.3.4/phi/math/backend/
+-rw-rw-rw-   0        0        0      787 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/math/backend/__init__.py
+-rw-rw-rw-   0        0        0    59048 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/backend/_backend.py
+-rw-rw-rw-   0        0        0     6172 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/backend/_dtype.py
+-rw-rw-rw-   0        0        0    22325 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/backend/_linalg.py
+-rw-rw-rw-   0        0        0     9054 2023-02-26 20:09:34.000000 phiflow-2.3.4/phi/math/backend/_minimize.py
+-rw-rw-rw-   0        0        0    21139 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/backend/_numpy_backend.py
+-rw-rw-rw-   0        0        0    22490 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/backend/_profile.py
+-rw-rw-rw-   0        0        0    59082 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/extrapolation.py
+-rw-rw-rw-   0        0        0    31622 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/math/magic.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.210486 phiflow-2.3.4/phi/physics/
+-rw-rw-rw-   0        0        0      480 2023-02-26 20:09:34.000000 phiflow-2.3.4/phi/physics/__init__.py
+-rw-rw-rw-   0        0        0    18286 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/physics/_boundaries.py
+-rw-rw-rw-   0        0        0     8477 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/physics/advect.py
+-rw-rw-rw-   0        0        0     4850 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/physics/diffuse.py
+-rw-rw-rw-   0        0        0    15532 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/physics/fluid.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.249522 phiflow-2.3.4/phi/tf/
+-rw-rw-rw-   0        0        0     1224 2022-05-20 17:17:38.000000 phiflow-2.3.4/phi/tf/__init__.py
+-rw-rw-rw-   0        0        0     4228 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/tf/_compile_cuda.py
+-rw-rw-rw-   0        0        0     2085 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/tf/_profiling.py
+-rw-rw-rw-   0        0        0    29927 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/tf/_tf_backend.py
+-rw-rw-rw-   0        0        0     3280 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/tf/_tf_cuda_resample.py
+-rw-rw-rw-   0        0        0     1175 2023-03-17 11:48:14.000000 phiflow-2.3.4/phi/tf/flow.py
+-rw-rw-rw-   0        0        0    34622 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/tf/nets.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.262534 phiflow-2.3.4/phi/torch/
+-rw-rw-rw-   0        0        0      498 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/torch/__init__.py
+-rw-rw-rw-   0        0        0    55689 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/torch/_torch_backend.py
+-rw-rw-rw-   0        0        0     1145 2023-03-17 11:48:14.000000 phiflow-2.3.4/phi/torch/flow.py
+-rw-rw-rw-   0        0        0    39392 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/torch/nets.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.284554 phiflow-2.3.4/phi/vis/
+-rw-rw-rw-   0        0        0     1089 2023-03-17 11:48:08.000000 phiflow-2.3.4/phi/vis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.312580 phiflow-2.3.4/phi/vis/_console/
+-rw-rw-rw-   0        0        0       36 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/vis/_console/__init__.py
+-rw-rw-rw-   0        0        0     6865 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/vis/_console/_console_gui.py
+-rw-rw-rw-   0        0        0     3140 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/vis/_console/_console_plot.py
+-rw-rw-rw-   0        0        0     2360 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/vis/_console/_console_util.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.372633 phiflow-2.3.4/phi/vis/_dash/
+-rw-rw-rw-   0        0        0        0 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/vis/_dash/__init__.py
+-rw-rw-rw-   0        0        0    21982 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/vis/_dash/_plotly_plots.py
+-rw-rw-rw-   0        0        0     7826 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/vis/_dash/board.py
+-rw-rw-rw-   0        0        0     4222 2023-03-17 11:48:08.000000 phiflow-2.3.4/phi/vis/_dash/colormaps.py
+-rw-rw-rw-   0        0        0     2954 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/vis/_dash/dash_app.py
+-rw-rw-rw-   0        0        0     7143 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/vis/_dash/dash_gui.py
+-rw-rw-rw-   0        0        0     2075 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/vis/_dash/info.py
+-rw-rw-rw-   0        0        0     1228 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/vis/_dash/log.py
+-rw-rw-rw-   0        0        0     5359 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/vis/_dash/model_controls.py
+-rw-rw-rw-   0        0        0     3493 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/vis/_dash/player_controls.py
+-rw-rw-rw-   0        0        0     2710 2023-02-26 20:09:34.000000 phiflow-2.3.4/phi/vis/_dash/viewer.py
+-rw-rw-rw-   0        0        0     5890 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/vis/_dash/viewsettings.py
+-rw-rw-rw-   0        0        0     3046 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/vis/_log.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.379642 phiflow-2.3.4/phi/vis/_matplotlib/
+-rw-rw-rw-   0        0        0      108 2023-02-26 20:09:34.000000 phiflow-2.3.4/phi/vis/_matplotlib/__init__.py
+-rw-rw-rw-   0        0        0    23781 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/vis/_matplotlib/_matplotlib_plots.py
+-rw-rw-rw-   0        0        0     7439 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/vis/_matplotlib/_scalars.py
+-rw-rw-rw-   0        0        0      793 2023-03-17 11:48:08.000000 phiflow-2.3.4/phi/vis/_plot_util.py
+-rw-rw-rw-   0        0        0     7184 2022-04-20 10:42:57.000000 phiflow-2.3.4/phi/vis/_user_namespace.py
+-rw-rw-rw-   0        0        0    10690 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/vis/_viewer.py
+-rw-rw-rw-   0        0        0    27058 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/vis/_vis.py
+-rw-rw-rw-   0        0        0    17070 2023-04-20 17:29:41.000000 phiflow-2.3.4/phi/vis/_vis_base.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:29:57.394654 phiflow-2.3.4/phiflow.egg-info/
+-rw-rw-rw-   0        0        0     2453 2023-04-20 17:29:56.000000 phiflow-2.3.4/phiflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2278 2023-04-20 17:29:56.000000 phiflow-2.3.4/phiflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 17:29:56.000000 phiflow-2.3.4/phiflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-20 17:29:56.000000 phiflow-2.3.4/phiflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-20 17:29:56.000000 phiflow-2.3.4/phiflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-20 17:29:57.396656 phiflow-2.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     7119 2023-02-26 18:31:51.000000 phiflow-2.3.4/setup.py
```

### Comparing `phiflow-2.3.3/PKG-INFO` & `phiflow-2.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: phiflow
-Version: 2.3.3
-Summary: Differentiable PDE solving framework for machine learning
-Home-page: https://github.com/tum-pbs/PhiFlow
-Download-URL: https://github.com/tum-pbs/PhiFlow/archive/2.3.3.tar.gz
-Author: Philipp Holl
-Author-email: philipp.holl@tum.de
-License: MIT
-Keywords: Differentiable,Simulation,Fluid,Machine Learning,Deep Learning
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# PhiFlow
-
-[**Homepage**](https://github.com/tum-pbs/PhiFlow)
-&nbsp;&nbsp;&nbsp; [**Documentation**](https://tum-pbs.github.io/PhiFlow/)
-&nbsp;&nbsp;&nbsp; [**API**](https://tum-pbs.github.io/PhiFlow/phi)
-&nbsp;&nbsp;&nbsp; [**Demos**](https://github.com/tum-pbs/PhiFlow/tree/master/demos)
-&nbsp;&nbsp;&nbsp; [<img src="https://www.tensorflow.org/images/colab_logo_32px.png" height=16> **Fluids Tutorial**](https://colab.research.google.com/github/tum-pbs/PhiFlow/blob/develop/docs/Fluids_Tutorial.ipynb#offline=true&sandboxMode=true)
-&nbsp;&nbsp;&nbsp; [<img src="https://www.tensorflow.org/images/colab_logo_32px.png" height=16> **Playground**](https://colab.research.google.com/drive/1zBlQbmNguRt-Vt332YvdTqlV4DBcus2S#offline=true&sandboxMode=true)
-
-PhiFlow is an open-source simulation toolkit built for optimization and machine learning applications.
-It is written mostly in Python and can be used with NumPy, TensorFlow, Jax or PyTorch.
-The close integration with machine learning frameworks allows it to leverage their automatic differentiation functionality,
-making it easy to build end-to-end differentiable functions involving both learning models and physics simulations.
-
-See the [installation Instructions](https://tum-pbs.github.io/PhiFlow/Installation_Instructions.html) on how to compile the optional custom CUDA operations.
+Metadata-Version: 2.1
+Name: phiflow
+Version: 2.3.4
+Summary: Differentiable PDE solving framework for machine learning
+Home-page: https://github.com/tum-pbs/PhiFlow
+Author: Philipp Holl
+Author-email: philipp.holl@tum.de
+License: MIT
+Download-URL: https://github.com/tum-pbs/PhiFlow/archive/2.3.4.tar.gz
+Description: # PhiFlow
+        
+        [**Homepage**](https://github.com/tum-pbs/PhiFlow)
+        &nbsp;&nbsp;&nbsp; [**Documentation**](https://tum-pbs.github.io/PhiFlow/)
+        &nbsp;&nbsp;&nbsp; [**API**](https://tum-pbs.github.io/PhiFlow/phi)
+        &nbsp;&nbsp;&nbsp; [**Demos**](https://github.com/tum-pbs/PhiFlow/tree/master/demos)
+        &nbsp;&nbsp;&nbsp; [<img src="https://www.tensorflow.org/images/colab_logo_32px.png" height=16> **Fluids Tutorial**](https://colab.research.google.com/github/tum-pbs/PhiFlow/blob/develop/docs/Fluids_Tutorial.ipynb#offline=true&sandboxMode=true)
+        &nbsp;&nbsp;&nbsp; [<img src="https://www.tensorflow.org/images/colab_logo_32px.png" height=16> **Playground**](https://colab.research.google.com/drive/1zBlQbmNguRt-Vt332YvdTqlV4DBcus2S#offline=true&sandboxMode=true)
+        
+        PhiFlow is an open-source simulation toolkit built for optimization and machine learning applications.
+        It is written mostly in Python and can be used with NumPy, TensorFlow, Jax or PyTorch.
+        The close integration with machine learning frameworks allows it to leverage their automatic differentiation functionality,
+        making it easy to build end-to-end differentiable functions involving both learning models and physics simulations.
+        
+        See the [installation Instructions](https://tum-pbs.github.io/PhiFlow/Installation_Instructions.html) on how to compile the optional custom CUDA operations.
+        
+Keywords: Differentiable,Simulation,Fluid,Machine Learning,Deep Learning
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
```

### Comparing `phiflow-2.3.3/README.md` & `phiflow-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/__init__.py` & `phiflow-2.3.4/phi/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/_troubleshoot.py` & `phiflow-2.3.4/phi/_troubleshoot.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/field/__init__.py` & `phiflow-2.3.4/phi/field/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/field/_angular_velocity.py` & `phiflow-2.3.4/phi/field/_angular_velocity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable
+from typing import Callable, Union
 from numbers import Number
 
 from phi import math
 
 from ._field import Field
 from ..geom import Geometry
 from ..math import Shape, spatial, instance, Tensor, wrap
@@ -14,16 +14,16 @@
     The falloff of the velocity magnitude can be controlled.
 
     Without a specified falloff, the velocity increases linearly with the distance from the vortex center.
     This is the case with rotating rigid bodies, for example.
     """
 
     def __init__(self,
-                 location: Tensor or tuple or list or Number,
-                 strength: Tensor or Number = 1.0,
+                 location: Union[Tensor, tuple, list, Number],
+                 strength: Union[Tensor, Number] = 1.0,
                  falloff: Callable = None,
                  component: str = None):
         location = wrap(location)
         strength = wrap(strength)
         assert location.shape.channel.names == ('vector',), "location must have a single channel dimension called 'vector'"
         assert location.shape.spatial.is_empty, "location tensor cannot have any spatial dimensions"
         assert not instance(location), "AngularVelocity does not support instance dimensions"
```

### Comparing `phiflow-2.3.3/phi/field/_embed.py` & `phiflow-2.3.4/phi/field/_embed.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/field/_field.py` & `phiflow-2.3.4/phi/field/_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,16 +139,16 @@
     """
     Base class for fields that are sampled at specific locations such as grids or point clouds.
     """
 
     def __init__(self,
                  elements: Union[Geometry, Tensor],
                  values: Tensor,
-                 extrapolation: float or Extrapolation or Field or None,
-                 bounds: Box or None):
+                 extrapolation: Union[float, Extrapolation, Field, None],
+                 bounds: Union[Box, None]):
         """
         Args:
           elements: Geometry object specifying the sample points and sizes
           values: values corresponding to elements
           extrapolation: values outside elements
         """
         if isinstance(elements, Tensor):
@@ -293,16 +293,16 @@
                 other = math.wrap(other, self.points.shape['vector'])
             else:
                 other = math.wrap(other)
             values = operator(self._values, other)
             return self.with_values(values)
 
 
-def sample(field: Field or Geometry,
-           geometry: Geometry or SampledField or Tensor,
+def sample(field: Union[Field, Geometry],
+           geometry: Union[Geometry, SampledField, Tensor],
            **kwargs) -> math.Tensor:
     """
     Computes the field value inside the volume of the (batched) `geometry`.
 
     The field value may be determined by integrating over the volume, sampling the central value or any other way.
 
     The batch dimensions of `geometry` are matched with this field.
@@ -335,16 +335,16 @@
     if geom_ch:
         sampled = [field._sample(p, **kwargs) for p in geometry.unstack(geom_ch.name)]
         return math.stack(sampled, geom_ch)
     else:
         return field._sample(geometry, **kwargs)
 
 
-def reduce_sample(field: Field or Geometry,
-                  geometry: Geometry or SampledField or Tensor,
+def reduce_sample(field: Union[Field, Geometry],
+                  geometry: Union[Geometry, SampledField, Tensor],
                   dim=channel('vector'),
                   **kwargs) -> math.Tensor:
     """
     Similar to `sample()`, but matches channel dimensions of `geometry` with channel dimensions of this field.
     Currently, `geometry` may have at most one channel dimension.
 
     See Also:
@@ -440,15 +440,15 @@
         raise ValueError(f"A Geometry, SampledField or location Tensor is required but got {geometry}")
 
 
 FieldType = TypeVar('FieldType', bound=Field)
 SampledFieldType = TypeVar('SampledFieldType', bound=SampledField)
 
 
-def as_extrapolation(obj: Extrapolation or float or Field or None) -> Extrapolation:
+def as_extrapolation(obj: Union[Extrapolation, float, Field, None]) -> Extrapolation:
     """
     Returns an `Extrapolation` representing `obj`.
 
     Args:
         obj: One of
 
             * `float` or `Tensor`: Extrapolate with a constant value
```

### Comparing `phiflow-2.3.3/phi/field/_field_io.py` & `phiflow-2.3.4/phi/field/_field_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from typing import Union
+
 import numpy as np
 
 from phi import geom
 from ._field import SampledField
 from ._grid import Grid, CenteredGrid, StaggeredGrid, unstack_staggered_tensor
 from ._field_math import stack
 from ..math import extrapolation, wrap, tensor, Shape, channel, Tensor, spatial
 
 
-def write(field: SampledField, file: str or Tensor):
+def write(field: SampledField, file: Union[str, Tensor]):
     """
     Writes a field to disc using a NumPy file format.
     Depending on `file`, the data may be split up into multiple files.
 
     All characteristics of the field are serialized so that it can be fully restored using `read()`.
 
     See Also:
@@ -60,15 +62,15 @@
                             bounds_item_names=bounds_item_names,
                             extrapolation=extrap,
                             data=data)
     else:
         raise NotImplementedError(f"{type(field)} not implemented. Only Grid allowed.")
 
 
-def read(file: str or Tensor, convert_to_backend=True) -> SampledField:
+def read(file: Union[str, Tensor], convert_to_backend=True) -> SampledField:
     """
     Loads a previously saved `SampledField` from disc.
 
     See Also:
         `write()`.
 
     Args:
```

### Comparing `phiflow-2.3.3/phi/field/_field_math.py` & `phiflow-2.3.4/phi/field/_field_math.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import warnings
 from numbers import Number
-from typing import Callable, List, Tuple, Optional
+from typing import Callable, List, Tuple, Optional, Union
 
 from phi import geom
 from phi import math
 from phi.geom import Box, Geometry
 from phi.math import Tensor, spatial, instance, tensor, channel, Shape, unstack, solve_linear, jit_compile_linear, shape, Solve, extrapolation, jit_compile
 from ._field import Field, SampledField, SampledFieldType, as_extrapolation
 from ._grid import CenteredGrid, Grid, StaggeredGrid, GridType
@@ -38,15 +38,15 @@
         raise ValueError(f"Not a valid grid: {grid}")
 
 
 def laplace(field: GridType,
             axes=spatial,
             order=2,
             implicit: math.Solve = None,
-            weights: Tensor or Field = None) -> GridType:
+            weights: Union[Tensor, Field] = None) -> GridType:
     """
     Spatial Laplace operator for scalar grid.
     If a vector grid is passed, it is assumed to be centered and the laplace is computed component-wise.
 
     Args:
         field: n-dimensional `CenteredGrid`
         axes: The second derivative along these dimensions is summed over
@@ -252,15 +252,15 @@
         new_bounds = Box(grid.box.lower - w_lower * grid.dx, grid.box.upper - w_upper * grid.dx)
     data = math.shift(grid.values, offsets, dims=dims, padding=padding, stack_dim=stack_dim)
     return [type(grid)(data[i], bounds=new_bounds, extrapolation=grid.extrapolation) for i in range(len(offsets))]
 
 
 def stagger(field: CenteredGrid,
             face_function: Callable,
-            extrapolation: float or math.extrapolation.Extrapolation,
+            extrapolation: Union[float, math.extrapolation.Extrapolation],
             type: type = StaggeredGrid):
     """
     Creates a new grid by evaluating `face_function` given two neighbouring cells.
     One layer of missing cells is inferred from the extrapolation.
     
     This method returns a Field of type `type` which must be either StaggeredGrid or CenteredGrid.
     When returning a StaggeredGrid, the new values are sampled at the faces of neighbouring cells.
@@ -428,15 +428,15 @@
 def fourier_poisson(grid: GridType, times=1) -> GridType:
     """ See `phi.math.fourier_poisson()` """
     assert grid.extrapolation.spatial_gradient() == math.extrapolation.PERIODIC
     values = math.fourier_poisson(grid.values, dx=grid.dx, times=times)
     return type(grid)(values=values, bounds=grid.bounds, extrapolation=grid.extrapolation)
 
 
-def native_call(f, *inputs, channels_last=None, channel_dim='vector', extrapolation=None) -> SampledField or Tensor:
+def native_call(f, *inputs, channels_last=None, channel_dim='vector', extrapolation=None) -> Union[SampledField, Tensor]:
     """
     Similar to `phi.math.native_call()`.
 
     Args:
         f: Function to be called on native tensors of `inputs.values`.
             The function output must have the same dimension layout as the inputs and the batch size must be identical.
         *inputs: `SampledField` or `phi.Tensor` instances.
@@ -453,15 +453,15 @@
             if extrapolation is not None:
                 result = result.with_extrapolation(extrapolation)
             return result
     else:
         raise AssertionError("At least one input must be a SampledField.")
 
 
-def data_bounds(loc: SampledField or Tensor) -> Box:
+def data_bounds(loc: Union[SampledField, Tensor]) -> Box:
     if isinstance(loc, SampledField):
         loc = loc.points
     assert isinstance(loc, Tensor), f"loc must be a Tensor or SampledField but got {type(loc)}"
     min_vec = math.min(loc, dim=loc.shape.non_batch.non_channel)
     max_vec = math.max(loc, dim=loc.shape.non_batch.non_channel)
     return Box(min_vec, max_vec)
 
@@ -495,15 +495,15 @@
     Returns:
         `Tensor` holding only batch dimensions.
     """
     assert 'vector' not in density.shape
     return mean(density.points * density) / mean(density)
 
 
-def pad(grid: GridType, widths: int or tuple or list or dict) -> GridType:
+def pad(grid: GridType, widths: Union[int, tuple, list, dict]) -> GridType:
     """
     Pads a `Grid` using its extrapolation.
 
     Unlike `phi.math.pad()`, this function also affects the `bounds` of the grid, changing its size and origin depending on `widths`.
 
     Args:
         grid: `CenteredGrid` or `StaggeredGrid`
@@ -576,15 +576,15 @@
         return CenteredGrid(values, bounds=grid.bounds, extrapolation=grid.extrapolation)
     elif isinstance(grid, StaggeredGrid):
         raise NotImplementedError()
     else:
         raise ValueError(type(grid))
 
 
-def concat(fields: List[SampledFieldType] or Tuple[SampledFieldType, ...], dim: str or Shape) -> SampledFieldType:
+def concat(fields: Union[List[SampledFieldType], Tuple[SampledFieldType, ...]], dim: Union[str, Shape]) -> SampledFieldType:
     """
     Concatenates the given `SampledField`s along `dim`.
 
     See Also:
         `stack()`.
 
     Args:
@@ -638,26 +638,26 @@
     elif isinstance(fields[0], PointCloud):
         elements = geom.stack([f.elements for f in fields], dim)
         values = math.stack([f.values for f in fields], dim)
         return PointCloud(elements=elements, values=values, extrapolation=fields[0].extrapolation, add_overlapping=fields[0]._add_overlapping, bounds=fields[0]._bounds)
     raise NotImplementedError(type(fields[0]))
 
 
-def assert_close(*fields: SampledField or Tensor or Number,
+def assert_close(*fields: Union[SampledField, Tensor, Number],
                  rel_tolerance: float = 1e-5,
                  abs_tolerance: float = 0,
                  msg: str = "",
                  verbose: bool = True):
     """ Raises an AssertionError if the `values` of the given fields are not close. See `phi.math.assert_close()`. """
     f0 = next(filter(lambda t: isinstance(t, SampledField), fields))
     values = [(f @ f0).values if isinstance(f, SampledField) else math.wrap(f) for f in fields]
     math.assert_close(*values, rel_tolerance=rel_tolerance, abs_tolerance=abs_tolerance, msg=msg, verbose=verbose)
 
 
-def where(mask: Field or Geometry or float, field_true: Field or float, field_false: Field or float) -> SampledFieldType:
+def where(mask: Union[Field, Geometry, float], field_true: Union[Field, float], field_false: Union[Field, float]) -> SampledFieldType:
     """
     Element-wise where operation.
     Picks the value of `field_true` where `mask=1 / True` and the value of `field_false` where `mask=0 / False`.
 
     The fields are automatically resampled if necessary, preferring the sample points of `mask`.
     At least one of the arguments must be a `SampledField`.
 
@@ -670,15 +670,15 @@
         `SampledField`
     """
     field_true, field_false, mask = _auto_resample(field_true, field_false, mask)
     values = math.where(mask.values, field_true.values, field_false.values)
     return field_true.with_values(values)
 
 
-def maximum(f1: Field or Geometry or float, f2: Field or Geometry or float):
+def maximum(f1: Union[Field, Geometry, float], f2: Union[Field, Geometry, float]):
     """
     Element-wise maximum.
     One of the given fields needs to be an instance of `SampledField` and the the result will be sampled at the corresponding points.
     If both are `SampledFields` but have different points, `f1` takes priority.
 
     Args:
         f1: `Field` or `Geometry` or constant.
@@ -687,15 +687,15 @@
     Returns:
         `SampledField`
     """
     f1, f2 = _auto_resample(f1, f2)
     return f1.with_values(math.maximum(f1.values, f2.values))
 
 
-def minimum(f1: Field or Geometry or float, f2: Field or Geometry or float):
+def minimum(f1: Union[Field, Geometry, float], f2: Union[Field, Geometry, float]):
     """
     Element-wise minimum.
     One of the given fields needs to be an instance of `SampledField` and the the result will be sampled at the corresponding points.
     If both are `SampledFields` but have different points, `f1` takes priority.
 
     Args:
         f1: `Field` or `Geometry` or constant.
@@ -784,17 +784,17 @@
     """
     if not isinstance(field, CenteredGrid):
         raise NotImplementedError()
     return field._sample(region, **kwargs) * region.volume
 
 
 def pack_dims(field: SampledFieldType,
-              dims: Shape or tuple or list or str,
+              dims: Union[Shape, tuple, list, str],
               packed_dim: Shape,
-              pos: int or None = None) -> SampledFieldType:
+              pos: Union[int, None] = None) -> SampledFieldType:
     """
     Currently only supports grids and non-spatial dimensions.
 
     See Also:
         `phi.math.pack_dims()`.
 
     Args:
@@ -807,29 +807,29 @@
         if spatial(field.shape.only(dims)):
             raise NotImplementedError("Packing spatial dimensions not supported for grids")
         return field.with_values(math.pack_dims(field.values, dims, packed_dim, pos))
     else:
         raise NotImplementedError()
 
 
-def support(field: SampledField, list_dim: Shape or str = instance('nonzero')) -> Tensor:
+def support(field: SampledField, list_dim: Union[Shape, str] = instance('nonzero')) -> Tensor:
     """
     Returns the points at which the field values are non-zero.
 
     Args:
         field: `SampledField`
         list_dim: Dimension to list the non-zero values.
 
     Returns:
         `Tensor` with shape `(list_dim, vector)`
     """
     return field.points[math.nonzero(field.values, list_dim=list_dim)]
 
 
-def mask(obj: SampledFieldType or Geometry) -> SampledFieldType:
+def mask(obj: Union[SampledFieldType, Geometry]) -> SampledFieldType:
     """
     Returns a `Field` that masks the inside (or non-zero values when `obj` is a grid) of a physical object.
     The mask takes the value 1 inside the object and 0 outside.
     For `CenteredGrid` and `StaggeredGrid`, the mask labels non-zero non-NaN entries as 1 and all other values as 0
 
     Returns:
         `Grid` type or `PointCloud`
```

### Comparing `phiflow-2.3.3/phi/field/_grid.py` & `phiflow-2.3.4/phi/field/_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Any, Tuple, List
+from typing import TypeVar, Any, Tuple, List, Union
 
 from phi.math import Solve
 
 from phi import math, geom
 from phi.geom import Box, Geometry, GridCell
 from ._embed import FieldEmbedding
 from ._field import SampledField, Field, sample, reduce_sample, as_extrapolation
@@ -15,15 +15,15 @@
 
 
 class Grid(SampledField):
     """
     Base class for `CenteredGrid` and `StaggeredGrid`.
     """
 
-    def __init__(self, elements: Geometry, values: Tensor, extrapolation: float or Extrapolation, resolution: Shape or int, bounds: Box or float):
+    def __init__(self, elements: Geometry, values: Tensor, extrapolation: Union[float, Extrapolation], resolution: Union[Shape, int], bounds: Union[Box, float]):
         assert isinstance(bounds, Box)
         assert isinstance(resolution, Shape)
         if bounds.size.vector.item_names is None:
             with NUMPY:
                 bounds = bounds.shifted(math.zeros(channel(vector=spatial(values).names)))
         SampledField.__init__(self, elements, values, extrapolation, bounds)
         assert values.shape.spatial_rank == elements.spatial_rank, f"Spatial dimensions of values ({values.shape}) do not match elements {elements}"
@@ -155,17 +155,17 @@
         `Field`,
         module documentation at https://tum-pbs.github.io/PhiFlow/Fields.html
     """
 
     def __init__(self,
                  values: Any = 0.,
                  extrapolation: Any = 0.,
-                 bounds: Box or float = None,
-                 resolution: int or Shape = None,
-                 **resolution_: int or Tensor):
+                 bounds: Union[Box, float] = None,
+                 resolution: Union[int, Shape] = None,
+                 **resolution_: Union[int, Tensor]):
         """
         Args:
             values: Values to use for the grid.
                 Has to be one of the following:
 
                 * `phi.geom.Geometry`: sets inside values to 1, outside to 0
                 * `Field`: resamples the Field to the staggered sample points
@@ -292,18 +292,18 @@
         `SampledField`,
         `Field`,
         module documentation at https://tum-pbs.github.io/PhiFlow/Fields.html
     """
 
     def __init__(self,
                  values: Any = 0.,
-                 extrapolation: float or Extrapolation = 0,
-                 bounds: Box or float = None,
-                 resolution: Shape or int = None,
-                 **resolution_: int or Tensor):
+                 extrapolation: Union[float, Extrapolation] = 0,
+                 bounds: Union[Box, float] = None,
+                 resolution: Union[Shape, int] = None,
+                 **resolution_: Union[int, Tensor]):
         """
         Args:
             values: Values to use for the grid.
                 Has to be one of the following:
 
                 * `phi.geom.Geometry`: sets inside values to 1, outside to 0
                 * `Field`: resamples the Field to the staggered sample points
@@ -514,42 +514,41 @@
     ext_lower, ext_upper = extrapolation.valid_outer_faces(any_dim)
     delta = int(ext_lower) + int(ext_upper) - 1
     resolution = x_shape.spatial._replace_single_size(any_dim, x_shape.get_size(any_dim) - delta)
     return resolution
 
 
 def _sample_function(f, elements: Geometry):
-    import inspect
+    from phi.math._functional import get_function_parameters
     try:
-        signature = inspect.signature(f)
-        params = dict(signature.parameters)
+        params = get_function_parameters(f)
         dims = elements.shape.get_size('vector')
         names_match = tuple(params.keys())[:dims] == elements.shape.get_item_names('vector')
         num_positional = 0
         has_varargs = False
         for n, p in params.items():
             if p.default is p.empty:
                 num_positional += 1
             if p.kind == 2:  # _ParameterKind.VAR_POSITIONAL
                 has_varargs = True
-        assert num_positional <= dims, f"Cannot sample {f.__name__}{signature} on physical space {elements.shape.get_item_names('vector')}"
+        assert num_positional <= dims, f"Cannot sample {f.__name__}({', '.join(tuple(params))}) on physical space {elements.shape.get_item_names('vector')}"
         pass_varargs = has_varargs or names_match or num_positional > 1 or num_positional == dims
         if num_positional > 1 and not has_varargs:
-            assert names_match, f"Positional arguments of {f.__name__}{signature} should match physical space {elements.shape.get_item_names('vector')}"
+            assert names_match, f"Positional arguments of {f.__name__}({', '.join(tuple(params))}) should match physical space {elements.shape.get_item_names('vector')}"
     except ValueError as err:  # signature not available for all functions
         pass_varargs = False
     if pass_varargs:
         values = math.map_s2b(f)(*elements.center.vector)
     else:
         values = math.map_s2b(f)(elements.center)
     assert isinstance(values, math.Tensor), f"values function must return a Tensor but returned {type(values)}"
     return values
 
 
-def _get_bounds(bounds: Box or float or None, resolution: Shape):
+def _get_bounds(bounds: Union[Box, float, None], resolution: Shape):
     if bounds is None:
         return Box(math.const_vec(0, resolution), math.wrap(resolution, channel(vector=resolution.names)))
     if isinstance(bounds, Box):
         assert set(bounds.vector.item_names) == set(resolution.names), f"bounds dimensions {bounds.vector.item_names} must match resolution {resolution}"
         return bounds
     if isinstance(bounds, (int, float)):
         return Box(math.const_vec(0, resolution), math.const_vec(bounds, resolution))
```

### Comparing `phiflow-2.3.3/phi/field/_mask.py` & `phiflow-2.3.4/phi/field/_mask.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import warnings
+from typing import Union
 
 from phi import math
 from phi.geom import Geometry
 from ._field import Field
 from ..math import Tensor
 
 
@@ -27,15 +28,15 @@
         return HardGeometryMask(self.geometry[item])
 
 
 class SoftGeometryMask(HardGeometryMask):
     """
     Deprecated since version 1.3. Use `phi.field.mask()` or `phi.field.resample()` instead.
     """
-    def __init__(self, geometry: Geometry, balance: Tensor or float = 0.5):
+    def __init__(self, geometry: Geometry, balance: Union[Tensor, float] = 0.5):
         warnings.warn("HardGeometryMask and SoftGeometryMask are deprecated. Use field.mask or field.resample instead.", DeprecationWarning, stacklevel=2)
         super().__init__(geometry)
         self.balance = balance
 
     def _sample(self, geometry: Geometry, **kwargs) -> Tensor:
         return self.geometry.approximate_fraction_inside(geometry, self.balance)
```

### Comparing `phiflow-2.3.3/phi/field/_noise.py` & `phiflow-2.3.4/phi/field/_noise.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/field/_point_cloud.py` & `phiflow-2.3.4/phi/field/_point_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,20 +188,20 @@
 
 def nonzero(field: SampledField):
     indices = math.nonzero(field.values, list_dim=instance('points'))
     elements = field.elements[indices]
     return PointCloud(elements, values=math.tensor(1.), extrapolation=math.extrapolation.ZERO, add_overlapping=False, bounds=field.bounds)
 
 
-def distribute_points(geometries: tuple or list or Geometry or float,
+def distribute_points(geometries: Union[tuple, list, Geometry, float],
                       dim: Shape = instance('points'),
                       points_per_cell: int = 8,
                       center: bool = False,
                       radius: float = None,
-                      extrapolation: float or Extrapolation = math.NAN,
+                      extrapolation: Union[float, Extrapolation] = math.NAN,
                       **domain) -> PointCloud:
     """
     Transforms `Geometry` objects into a PointCloud.
 
     Args:
         geometries: Geometry objects marking the cells which should contain points
         dim: Dimension along which the points are listed.
```

### Comparing `phiflow-2.3.3/phi/field/_scene.py` & `phiflow-2.3.4/phi/field/_scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 import json
 import os
 import re
 import shutil
 import sys
 import warnings
 from os.path import join, isfile, isdir, abspath, expanduser, basename, split
-from typing import Tuple
+from typing import Tuple, Union
 
 import numpy as np
 
 from phi import math, __version__ as phi_version
 from ._field import SampledField
 from ._field_io import read, write
 from ..math import Shape, batch, stack, unpack_dim, wrap
 from ..math.magic import BoundDim
 
 
+typing_list = list
+
+
 def _filename(simpath, name, frame):
     return join(simpath, f"{slugify(name)}_{frame:06d}.npz")
 
 
 def _str(bytes_or_str):  # on Linux, os.listdir returns bytes instead of strings
     if isinstance(bytes_or_str, str):
         return bytes_or_str
@@ -56,17 +59,17 @@
     The data of the scene is organized into NumPy files by *name* and *frame*.
 
     To create a new scene, use `Scene.create()`.
     To reference an existing scene, use `Scene.at()`.
     To list all scenes within a directory, use `Scene.list()`.
     """
 
-    def __init__(self, paths: str or math.Tensor):
+    def __init__(self, paths: Union[str, math.Tensor]):
         self._paths = math.wrap(paths)
-        self._properties: dict or None = None
+        self._properties: Union[dict, None] = None
 
     def __getitem__(self, item):
         return Scene(self._paths[item])
 
     def __getattr__(self, name: str) -> BoundDim:
         return BoundDim(self, name)
 
@@ -147,15 +150,15 @@
                 warnings.warn(f"Failed to copy calling script to scene during Scene.create(): {err}", RuntimeWarning)
         return scene
 
     @staticmethod
     def list(parent_directory: str,
              name='sim',
              include_other: bool = False,
-             dim: Shape or None = None) -> 'Scene' or tuple:
+             dim: Union[Shape, None] = None) -> Union['Scene', tuple]:
         """
         Lists all scenes inside the given directory.
 
         See Also:
             `Scene.at()`, `Scene.create()`.
 
         Args:
@@ -175,15 +178,15 @@
         if dim is None:
             return tuple(Scene(join(parent_directory, n)) for n in names)
         else:
             paths = math.wrap([join(parent_directory, n) for n in names], dim)
             return Scene(paths)
 
     @staticmethod
-    def at(directory: str or tuple or list or math.Tensor or 'Scene', id: int or math.Tensor or None = None) -> 'Scene':
+    def at(directory: Union[str, tuple, typing_list, math.Tensor, 'Scene'], id: Union[int, math.Tensor, None] = None) -> 'Scene':
         """
         Creates a `Scene` for an existing directory.
 
         See Also:
             `Scene.create()`, `Scene.list()`.
 
         Args:
@@ -206,15 +209,15 @@
             paths = math.map(lambda d, i: join(d, f"sim_{i:06d}"), directory, id)
         # test all exist
         for path in math.flatten(paths, flatten_batch=True):
             if not isdir(path):
                 raise IOError(f"There is no scene at '{path}'")
         return Scene(paths)
 
-    def subpath(self, name: str, create=False, create_parent=False) -> str or tuple:
+    def subpath(self, name: str, create=False, create_parent=False) -> Union[str, tuple]:
         """
         Resolves the relative path `name` with this `Scene` as the root folder.
 
         Args:
             name: Relative path with this `Scene` as the root folder.
             create: Whether to create a directory of that name.
             create_parent: Whether to create the parent directory.
```

### Comparing `phiflow-2.3.3/phi/flow.py` & `phiflow-2.3.4/phi/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/geom/__init__.py` & `phiflow-2.3.4/phi/geom/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/geom/_box.py` & `phiflow-2.3.4/phi/geom/_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import Dict, Tuple
+from typing import Dict, Tuple, Union
 
 import numpy as np
 
 from phi import math
 from ._geom import Geometry, _keep_vector
 from ..math import wrap, INF, Shape, channel, spatial, copy_with, Tensor
 from ..math._shape import parse_dim_order
@@ -76,15 +76,15 @@
 
     def lies_inside(self, location):
         bool_inside = (location >= self.lower) & (location <= self.upper)
         bool_inside = math.all(bool_inside, 'vector')
         bool_inside = math.any(bool_inside, self.shape.instance)  # union for instance dimensions
         return bool_inside
 
-    def approximate_signed_distance(self, location: Tensor or tuple):
+    def approximate_signed_distance(self, location: Union[Tensor, tuple]):
         """
         Computes the signed L-infinity norm (manhattan distance) from the location to the nearest side of the box.
         For an outside location `l` with the closest surface point `s`, the distance is `max(abs(l - s))`.
         For inside locations it is `-max(abs(l - s))`.
 
         Args:
           location: float tensor of shape (batch_size, ..., rank)
@@ -133,15 +133,15 @@
         """ Tests if the other box lies fully inside this box. """
         return np.all(other.lower >= self.lower) and np.all(other.upper <= self.upper)
 
     def rotated(self, angle) -> Geometry:
         from ._transform import rotate
         return rotate(self, angle)
 
-    def scaled(self, factor: float or Tensor) -> 'Geometry':
+    def scaled(self, factor: Union[float, Tensor]) -> 'Geometry':
         return Cuboid(self.center, self.half_size * factor)
 
 
 class BoxType(type):
     """ Deprecated. Does not support item names. """
 
     def __getitem__(self, item):
@@ -174,15 +174,15 @@
 
         The slicing constructor was updated in version 2.2 and now requires the dimension order as the first argument.
 
         >>> Box['x,y', 0:1, 0:1]  # creates a two-dimensional unit box with `lower=(0, 0)` and `upper=(1, 1)`.
         >>> Box['x,y', :1, 0:]  # creates a Box with `lower=(-inf, 0)` and `upper=(1, inf)`.
     """
 
-    def __init__(self, lower: Tensor = None, upper: Tensor = None, **size: int or Tensor):
+    def __init__(self, lower: Tensor = None, upper: Tensor = None, **size: Union[int, Tensor]):
         """
         Args:
           lower: physical location of lower corner
           upper: physical location of upper corner
           **size: Specify size by dimension, either as `int` or `tuple` containing (lower, upper).
         """
         if lower is not None:
@@ -306,16 +306,16 @@
 class Cuboid(BaseBox):
     """
     Box specified by center position and half size.
     """
 
     def __init__(self,
                  center: Tensor = 0,
-                 half_size: float or Tensor = None,
-                 **size: float or Tensor):
+                 half_size: Union[float, Tensor] = None,
+                 **size: Union[float, Tensor]):
         if half_size is not None:
             assert isinstance(half_size, Tensor), "half_size must be a Tensor"
             assert 'vector' in half_size.shape, f"Cuboid size must have a 'vector' dimension."
             assert half_size.shape.get_item_names('vector') is not None, f"Vector dimension must list spatial dimensions as item names. Use the syntax Cuboid(x=x, y=y) to assign names."
             self._half_size = half_size
         else:
             self._half_size = math.wrap(tuple(size.values()), math.channel(vector=tuple(size.keys()))) * 0.5
@@ -467,15 +467,15 @@
                 lower = bounds.lower + start * dim_mask * dx
                 upper = bounds.upper + (stop - self.resolution.get_size(dim)) * dim_mask * dx
                 bounds = Box(lower, upper)
                 gather_dict[dim] = slice(start, stop)
         resolution = self._resolution.after_gather(gather_dict)
         return GridCell(resolution, bounds[{d: s for d, s in item.items() if d != 'vector'}])
 
-    def __pack_dims__(self, dims: Tuple[str, ...], packed_dim: Shape, pos: int or None, **kwargs) -> 'Cuboid':
+    def __pack_dims__(self, dims: Tuple[str, ...], packed_dim: Shape, pos: Union[int, None], **kwargs) -> 'Cuboid':
         return math.pack_dims(self.center_representation(), dims, packed_dim, pos, **kwargs)
 
     @staticmethod
     def __stack__(values: tuple, dim: Shape, **kwargs) -> 'Geometry':
         from ._stack import GeometryStack
         return GeometryStack(math.layout(values, dim))
```

### Comparing `phiflow-2.3.3/phi/geom/_geom.py` & `phiflow-2.3.4/phi/geom/_geom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from numbers import Number
+from typing import Union
 
 from phi import math
 from phi.math import Tensor, Shape, EMPTY_SHAPE, non_channel, wrap, shape
 from phi.math._magic_ops import variable_attributes, expand
 from phi.math.magic import BoundDim, slicing_dict
 
 
@@ -89,15 +90,15 @@
 
         Returns:
           bool tensor of shape (*location.shape[:-1], 1).
 
         """
         raise NotImplementedError(self.__class__)
 
-    def approximate_signed_distance(self, location: Tensor or tuple) -> Tensor:
+    def approximate_signed_distance(self, location: Union[Tensor, tuple]) -> Tensor:
         """
         Computes the approximate distance from location to the surface of the geometry.
         Locations outside return positive values, inside negative values and zero exactly at the boundary.
 
         The exact distance metric used depends on the geometry.
         The approximation holds close to the surface and the distance grows to infinity as the location is moved infinitely far from the geometry.
         The distance metric is differentiable and its gradients are bounded at every point in space.
@@ -111,15 +112,15 @@
 
         Returns:
           float tensor of shape (*location.shape[:-1], 1).
 
         """
         raise NotImplementedError(self.__class__)
 
-    def approximate_fraction_inside(self, other_geometry: 'Geometry', balance: Tensor or Number = 0.5) -> Tensor:
+    def approximate_fraction_inside(self, other_geometry: 'Geometry', balance: Union[Tensor, Number] = 0.5) -> Tensor:
         """
         Computes the approximate overlap between the geometry and a small other geometry.
         Returns 1.0 if `other_geometry` is fully enclosed in this geometry and 0.0 if there is no overlap.
         Close to the surface of this geometry, the fraction filled is differentiable w.r.t. the location and size of `other_geometry`.
 
         To call this method on batches of geometries of same shape, pass a batched Geometry instance.
         The result tensor will match the batch shape of `other_geometry`.
@@ -247,28 +248,28 @@
             `Geometry`.
         """
         raise NotImplementedError
 
     def __matmul__(self, other):
         return self.at(other)
 
-    def rotated(self, angle: float or Tensor) -> 'Geometry':
+    def rotated(self, angle: Union[float, Tensor]) -> 'Geometry':
         """
         Returns a rotated version of this geometry.
         The geometry is rotated about its center point.
 
         Args:
           angle: scalar (2d) or vector (3D+) representing delta angle
 
         Returns:
             Rotated `Geometry`
         """
         raise NotImplementedError(self.__class__)
 
-    def scaled(self, factor: float or Tensor) -> 'Geometry':
+    def scaled(self, factor: Union[float, Tensor]) -> 'Geometry':
         """
         Scales each individual geometry by `factor`.
         The individual `center` points act as pivots for the operation.
 
         Args:
             factor:
 
@@ -369,15 +370,15 @@
     @property
     def shape_type(self) -> Tensor:
         raise NotImplementedError
 
     def sample_uniform(self, *shape: math.Shape) -> Tensor:
         raise NotImplementedError
 
-    def scaled(self, factor: float or Tensor) -> 'Geometry':
+    def scaled(self, factor: Union[float, Tensor]) -> 'Geometry':
         return _InvertedGeometry(self.geometry.scaled(factor))
 
     def __getitem__(self, item: dict):
         return _InvertedGeometry(self.geometry[item])
 
     @property
     def center(self):
@@ -389,15 +390,15 @@
 
     def lies_inside(self, location: Tensor) -> Tensor:
         return ~self.geometry.lies_inside(location)
 
     def approximate_signed_distance(self, location: Tensor) -> Tensor:
         return -self.geometry.approximate_signed_distance(location)
 
-    def approximate_fraction_inside(self, other_geometry: 'Geometry', balance: Tensor or Number = 0.5) -> Tensor:
+    def approximate_fraction_inside(self, other_geometry: 'Geometry', balance: Union[Tensor, Number] = 0.5) -> Tensor:
         return 1 - self.geometry.approximate_fraction_inside(other_geometry, 1 - balance)
 
     def push(self, positions: Tensor, outward: bool = True, shift_amount: float = 0) -> Tensor:
         return self.geometry.push(positions, outward=not outward, shift_amount=shift_amount)
 
     def bounding_radius(self) -> Tensor:
         raise NotImplementedError()
@@ -442,15 +443,15 @@
 
     def push(self, positions: Tensor, outward: bool = True, shift_amount: float = 0) -> Tensor:
         return positions
 
     def sample_uniform(self, *shape: math.Shape) -> Tensor:
         raise NotImplementedError
 
-    def scaled(self, factor: float or Tensor) -> 'Geometry':
+    def scaled(self, factor: Union[float, Tensor]) -> 'Geometry':
         return self
 
     def __getitem__(self, item: dict):
         return self
 
     @property
     def shape(self):
@@ -472,15 +473,15 @@
 
     def approximate_signed_distance(self, location):
         return math.expand(math.INF, non_channel(location))
 
     def lies_inside(self, location):
         return math.zeros(non_channel(location), dtype=bool)
 
-    def approximate_fraction_inside(self, other_geometry: 'Geometry', balance: Tensor or Number = 0.5) -> Tensor:
+    def approximate_fraction_inside(self, other_geometry: 'Geometry', balance: Union[Tensor, Number] = 0.5) -> Tensor:
         return math.zeros(other_geometry.shape)
 
     def at(self, center: Tensor) -> 'Geometry':
         return self
 
     def rotated(self, angle):
         return self
@@ -519,15 +520,15 @@
 
     def unstack(self, dimension: str) -> tuple:
         return tuple(Point(loc) for loc in self._location.unstack(dimension))
 
     def lies_inside(self, location: Tensor) -> Tensor:
         return expand(math.wrap(False), shape(location).without('vector'))
 
-    def approximate_signed_distance(self, location: Tensor or tuple) -> Tensor:
+    def approximate_signed_distance(self, location: Union[Tensor, tuple]) -> Tensor:
         return math.vec_abs(location - self._location)
 
     def push(self, positions: Tensor, outward: bool = True, shift_amount: float = 0) -> Tensor:
         return positions
 
     def bounding_radius(self) -> Tensor:
         return math.zeros()
@@ -554,15 +555,15 @@
     @property
     def shape_type(self) -> Tensor:
         return math.tensor('P')
 
     def sample_uniform(self, *shape: math.Shape) -> Tensor:
         raise NotImplementedError
 
-    def scaled(self, factor: float or Tensor) -> 'Geometry':
+    def scaled(self, factor: Union[float, Tensor]) -> 'Geometry':
         return self
 
     def __getitem__(self, item):
         return Point(self._location[_keep_vector(slicing_dict(self, item))])
 
 
 def assert_same_rank(rank1, rank2, error_message):
```

### Comparing `phiflow-2.3.3/phi/geom/_sphere.py` & `phiflow-2.3.4/phi/geom/_sphere.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from typing import Union
+
 from phi import math
 from ._geom import Geometry, _keep_vector
 from ..math import wrap, Tensor, expand
 from ..math.magic import slicing_dict
 
 
 class Sphere(Geometry):
     """
     N-dimensional sphere.
     Defined through center position and radius.
     """
 
     def __init__(self,
                  center: Tensor = None,
-                 radius: float or Tensor = None,
-                 **center_: float or Tensor):
+                 radius: Union[float, Tensor] = None,
+                 **center_: Union[float, Tensor]):
         """
         Args:
             center: Sphere center as `Tensor` with `vector` dimension.
                 The spatial dimension order should be specified in the `vector` dimension via item names.
             radius: Sphere radius as `float` or `Tensor`
             **center_: Specifies center when the `center` argument is not given. Center position by dimension, e.g. `x=0.5, y=0.2`.
         """
@@ -63,15 +65,15 @@
     def shape_type(self) -> Tensor:
         return math.tensor('S')
 
     def lies_inside(self, location):
         distance_squared = math.sum((location - self.center) ** 2, dim='vector')
         return math.any(distance_squared <= self.radius ** 2, self.shape.instance)  # union for instance dimensions
 
-    def approximate_signed_distance(self, location: Tensor or tuple):
+    def approximate_signed_distance(self, location: Union[Tensor, tuple]):
         """
         Computes the exact distance from location to the closest point on the sphere.
         Very close to the sphere center, the distance takes a constant value.
 
         Args:
           location: float tensor of shape (batch_size, ..., rank)
 
@@ -95,15 +97,15 @@
 
     def at(self, center: Tensor) -> 'Geometry':
         return Sphere(center, self._radius)
 
     def rotated(self, angle):
         return self
 
-    def scaled(self, factor: float or Tensor) -> 'Geometry':
+    def scaled(self, factor: Union[float, Tensor]) -> 'Geometry':
         return Sphere(self.center, self.radius * factor)
 
     def __variable_attrs__(self):
         return '_center', '_radius'
 
     def __getitem__(self, item):
         item = slicing_dict(self, item)
```

### Comparing `phiflow-2.3.3/phi/geom/_stack.py` & `phiflow-2.3.4/phi/geom/_stack.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/geom/_transform.py` & `phiflow-2.3.4/phi/geom/_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from numbers import Number
-from typing import Tuple
+from typing import Tuple, Union
 
 from phi import math
 from phi.math import Tensor, Shape
 from . import BaseBox, Box
 from ._geom import Geometry
 from ._sphere import Sphere
 from ..math._shape import parse_dim_order
 
 
 class RotatedGeometry(Geometry):
 
-    def __init__(self, geometry: Geometry, angle: float or math.Tensor):
+    def __init__(self, geometry: Geometry, angle: Union[float, math.Tensor]):
         assert not isinstance(geometry, RotatedGeometry)
         self._geometry = geometry
         self._angle = math.wrap(angle)
 
     @property
     def shape(self):
         return self._geometry.shape
@@ -79,15 +79,15 @@
 
     def at(self, center: Tensor) -> 'Geometry':
         return RotatedGeometry(self._geometry.at(center), self._angle)
 
     def rotated(self, angle) -> Geometry:
         return RotatedGeometry(self._geometry, self._angle + angle)
 
-    def scaled(self, factor: float or Tensor) -> 'Geometry':
+    def scaled(self, factor: Union[float, Tensor]) -> 'Geometry':
         return RotatedGeometry(self._geometry.scaled(factor), self._angle)
 
     def unstack(self, dimension: str) -> tuple:
         return tuple([RotatedGeometry(g, self._angle) for g in self._geometry.unstack(dimension)])
 
     def sample_uniform(self, *shape: math.Shape) -> Tensor:
         loc = self._geometry.sample_uniform(*shape)
@@ -96,15 +96,15 @@
     def __hash__(self):
         return hash(self._angle) + hash(self._geometry)
 
     def __repr__(self):
         return f"rot({self._geometry}, angle={self._angle})"
 
 
-def rotate(geometry: Geometry, angle: Number or Tensor) -> Geometry:
+def rotate(geometry: Geometry, angle: Union[Number, Tensor]) -> Geometry:
     """ Package-internal rotation function. Users should use Geometry.rotated() instead. """
     assert isinstance(geometry, Geometry)
     if isinstance(geometry, RotatedGeometry):
         total_rotation = geometry.angle + angle  # ToDo concatenate rotations
         return RotatedGeometry(geometry.geometry, total_rotation)
     else:
         return RotatedGeometry(geometry, angle)
@@ -169,25 +169,25 @@
 
     def shifted(self, delta: Tensor) -> 'Geometry':
         raise NotImplementedError()
 
     def at(self, center: Tensor) -> 'Geometry':
         raise NotImplementedError()
 
-    def rotated(self, angle: float or Tensor) -> 'Geometry':
+    def rotated(self, angle: Union[float, Tensor]) -> 'Geometry':
         raise NotImplementedError()
 
-    def scaled(self, factor: float or Tensor) -> 'Geometry':
+    def scaled(self, factor: Union[float, Tensor]) -> 'Geometry':
         raise NotImplementedError()
 
     def __hash__(self):
         return hash(self.geometry) + hash(self.axes)
 
 
-def embed(geometry: Geometry, projected_dims: math.Shape or str or tuple or list or None) -> Geometry:
+def embed(geometry: Geometry, projected_dims: Union[math.Shape, str, tuple, list, None]) -> Geometry:
     """
     Adds fake spatial dimensions to a geometry.
     The geometry value will be constant along the added dimensions, as if it had infinite length in these directions.
 
     Dimensions that are already present with `geometry` are ignored.
 
     Args:
@@ -208,15 +208,15 @@
             axes = (name,) + axes
     if isinstance(geometry, BaseBox):
         box = geometry.corner_representation()
         return box * Box(**{dim: None for dim in embedded_axes})
     return _EmbeddedGeometry(geometry, axes)
 
 
-def infinite_cylinder(center=None, radius=None, inf_dim: str or Shape or tuple or list = None, **center_) -> Geometry:
+def infinite_cylinder(center=None, radius=None, inf_dim: Union[str, Shape, tuple, list] = None, **center_) -> Geometry:
     """
     Creates an infinite cylinder.
     This is equal to embedding an `n`-dimensional `Sphere` in `n+1` dimensions.
 
     See Also:
         `Sphere`, `embed`
```

### Comparing `phiflow-2.3.3/phi/geom/_union.py` & `phiflow-2.3.4/phi/geom/_union.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/jax/_jax_backend.py` & `phiflow-2.3.4/phi/jax/_jax_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numbers
 import warnings
 from functools import wraps
-from typing import List, Callable, Tuple
+from typing import List, Callable, Tuple, Union
 from packaging import version
 
 import jax
 import jax.numpy as jnp
 import jax.scipy as scipy
 import numpy as np
 from jax import random
@@ -174,15 +174,15 @@
     def block_until_ready(self, values):
         if isinstance(values, DeviceArray):
             values.block_until_ready()
         if isinstance(values, (tuple, list)):
             for v in values:
                 self.block_until_ready(v)
 
-    def jacobian(self, f, wrt: tuple or list, get_output: bool, is_f_scalar: bool):
+    def jacobian(self, f, wrt: Union[tuple, list], get_output: bool, is_f_scalar: bool):
         if get_output:
             jax_grad_f = jax.value_and_grad(f, argnums=wrt, has_aux=True)
             @wraps(f)
             def unwrap_outputs(*args):
                 args = [self.to_float(arg) if self.dtype(arg).kind in (bool, int) else arg for arg in args]
                 (_, output_tuple), grads = jax_grad_f(*args)
                 return (*output_tuple, *grads)
@@ -209,15 +209,15 @@
         jax_fun.defvjp(forward, backward)
         return jax_fun
 
     def divide_no_nan(self, x, y):
         return jnp.where(y == 0, 0, x / y)
         # jnp.nan_to_num(x / y, copy=True, nan=0) covers up NaNs from before
 
-    def random_uniform(self, shape, low, high, dtype: DType or None):
+    def random_uniform(self, shape, low, high, dtype: Union[DType, None]):
         self._check_float64()
         self.rnd_key, subkey = jax.random.split(self.rnd_key)
 
         dtype = dtype or self.float_type
         jdt = to_numpy_dtype(dtype)
         if dtype.kind == float:
             tensor = random.uniform(subkey, shape, minval=low, maxval=high, dtype=jdt)
@@ -297,15 +297,15 @@
     def linspace(self, start, stop, number):
         self._check_float64()
         return jax.device_put(jnp.linspace(start, stop, number, dtype=to_numpy_dtype(self.float_type)), self._default_device.ref)
 
     def mean(self, value, axis=None, keepdims=False):
         return jnp.mean(value, axis, keepdims=keepdims)
 
-    def tensordot(self, a, a_axes: tuple or list, b, b_axes: tuple or list):
+    def tensordot(self, a, a_axes: Union[tuple, list], b, b_axes: Union[tuple, list]):
         return jnp.tensordot(a, b, (a_axes, b_axes))
 
     def mul(self, a, b):
         # if scipy.sparse.issparse(a):  # TODO sparse?
         #     return a.multiply(b)
         # elif scipy.sparse.issparse(b):
         #     return b.multiply(a)
@@ -318,15 +318,15 @@
             return(A @ b.T).T
         return jnp.stack([A.dot(b[i]) for i in range(b.shape[0])])
 
     def get_diagonal(self, matrices, offset=0):
         result = jnp.diagonal(matrices, offset=offset, axis1=1, axis2=2)
         return jnp.transpose(result, [0, 2, 1])
 
-    def while_loop(self, loop: Callable, values: tuple, max_iter: int or Tuple[int, ...] or List[int]):
+    def while_loop(self, loop: Callable, values: tuple, max_iter: Union[int, Tuple[int, ...], List[int]]):
         if all(self.is_available(t) for t in values):
             return self.stop_gradient_tree(Backend.while_loop(self, loop, values, max_iter))
         if isinstance(max_iter, (tuple, list)):  # stack traced trajectory, unroll until max_iter
             values = self.stop_gradient_tree(values)
             trj = [values] if 0 in max_iter else []
             for i in range(1, max(max_iter) + 1):
                 values = loop(*values)
@@ -428,26 +428,26 @@
             b_values = values[min(b, values.shape[0] - 1), ...]
             result.append(scatter(b_grid, b_indices, b_values, dnums))
         return jnp.stack(result)
 
     def quantile(self, x, quantiles):
         return jnp.quantile(x, quantiles, axis=-1)
 
-    def fft(self, x, axes: tuple or list):
+    def fft(self, x, axes: Union[tuple, list]):
         x = self.to_complex(x)
         if not axes:
             return x
         if len(axes) == 1:
             return jnp.fft.fft(x, axis=axes[0]).astype(x.dtype)
         elif len(axes) == 2:
             return jnp.fft.fft2(x, axes=axes).astype(x.dtype)
         else:
             return jnp.fft.fftn(x, axes=axes).astype(x.dtype)
 
-    def ifft(self, k, axes: tuple or list):
+    def ifft(self, k, axes: Union[tuple, list]):
         if not axes:
             return k
         if len(axes) == 1:
             return jnp.fft.ifft(k, axis=axes[0]).astype(k.dtype)
         elif len(axes) == 2:
             return jnp.fft.ifft2(k, axes=axes).astype(k.dtype)
         else:
@@ -469,12 +469,12 @@
         return solution, residuals, rank, singular_values
 
     def solve_triangular_dense(self, matrix, rhs, lower: bool, unit_diagonal: bool):
         matrix, rhs = self.auto_cast(matrix, rhs, int_to_float=True, bool_to_int=True)
         x = jax.lax.linalg.triangular_solve(matrix, rhs, lower=lower, unit_diagonal=unit_diagonal, left_side=True)
         return x
 
-    def sparse_coo_tensor(self, indices: tuple or list, values, shape: tuple):
+    def sparse_coo_tensor(self, indices: Union[tuple, list], values, shape: tuple):
         return BCOO((values, indices), shape=shape)
 
 
 lstsq_batched = jax.vmap(jnp.linalg.lstsq)  # map first dimension, required for JaxBackend.matrix_solve_least_squares()
```

### Comparing `phiflow-2.3.3/phi/jax/flow.py` & `phiflow-2.3.4/phi/jax/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/jax/stax/flow.py` & `phiflow-2.3.4/phi/jax/stax/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/jax/stax/nets.py` & `phiflow-2.3.4/phi/jax/stax/nets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 """
 Stax implementation of the unified machine learning API.
 Equivalent functions also exist for the other frameworks.
 
 For API documentation, see https://tum-pbs.github.io/PhiFlow/Network_API .
 """
 import functools
-import inspect
 import warnings
-from typing import Callable, Tuple, List
+from typing import Callable, Union, Sequence
 
-import numpy
 import jax
 import jax.numpy as jnp
 import keras
 import numpy
 import numpy as np
 from jax import random
-
 from packaging import version
 
 if version.parse(jax.__version__) >= version.parse(
         '0.2.25'):  # Stax and Optimizers were moved to jax.example_libraries on Oct 20, 2021
     from jax.example_libraries import stax
     import jax.example_libraries.optimizers as optim
     from jax.example_libraries.optimizers import OptimizerState
@@ -172,15 +169,15 @@
             elif rank == 5:
                 phi_tensor = math.wrap(param, math.channel('x,y,z,input,output'))
             else:
                 raise NotImplementedError(rank)
             result[name] = phi_tensor
 
 
-def save_state(obj: StaxNet or JaxOptimizer, path: str):
+def save_state(obj: Union[StaxNet, JaxOptimizer], path: str):
     """
     Write the state of a module or optimizer to a file.
 
     See Also:
         `load_state()`
 
     Args:
@@ -192,15 +189,15 @@
     if isinstance(obj, StaxNet):
         numpy.save(path, obj.parameters)
     else:
         raise NotImplementedError  # ToDo
         # numpy.save(path, obj._state)
 
 
-def load_state(obj: StaxNet or JaxOptimizer, path: str):
+def load_state(obj: Union[StaxNet, JaxOptimizer], path: str):
     """
     Read the state of a module or optimizer from a file.
 
     See Also:
         `save_state()`
 
     Args:
@@ -281,15 +278,15 @@
         opt = JaxOptimizer(*optim.rmsprop_momentum(learning_rate, alpha, eps, momentum))
     opt.initialize(net.parameters)
     return opt
 
 
 def dense_net(in_channels: int,
               out_channels: int,
-              layers: Tuple[int, ...] or List[int],
+              layers: Sequence[int],
               batch_norm=False,
               activation='ReLU',
               softmax=False) -> StaxNet:
     """
     Fully-connected neural networks are available in ΦFlow via dense_net().
     Arguments:
         in_channels : size of input layer, int
@@ -316,18 +313,18 @@
     net.initialize()
     return net
 
 
 def u_net(in_channels: int,
           out_channels: int,
           levels: int = 4,
-          filters: int or tuple or list = 16,
+          filters: Union[int, tuple, list] = 16,
           batch_norm: bool = True,
           activation='ReLU',
-          in_spatial: tuple or int = 2,
+          in_spatial: Union[tuple, int] = 2,
           periodic=False,
           use_res_blocks: bool = False) -> StaxNet:
     """
      ΦFlow provides a built-in U-net architecture, classically popular for Semantic Segmentation in Computer Vision, composed of downsampling and upsampling layers.
 
      Arguments:
 
@@ -465,15 +462,15 @@
         x = math.upsample2x(x)
         return x.native(x.shape)
 
     return NotImplemented, upsample_apply
 
 
 def conv_classifier(in_features: int,
-                    in_spatial: tuple or list,
+                    in_spatial: Union[tuple, list],
                     num_classes: int,
                     blocks=(64, 128, 256, 256, 512, 512),
                     dense_layers=(4096, 4096, 100),
                     batch_norm=True,
                     activation='ReLU',
                     softmax=True,
                     periodic=False):
@@ -541,19 +538,19 @@
     net = StaxNet(net_init, net_apply, (1,) + in_spatial + (in_features,))
     net.initialize()
     return net
 
 
 def conv_net(in_channels: int,
              out_channels: int,
-             layers: Tuple[int, ...] or List[int],
+             layers: Sequence[int],
              batch_norm: bool = False,
-             activation: str or Callable = 'ReLU',
+             activation: Union[str, Callable] = 'ReLU',
              periodic=False,
-             in_spatial: int or tuple = 2) -> StaxNet:
+             in_spatial: Union[int, tuple] = 2) -> StaxNet:
     """
     Built in Conv-Nets are also provided. Contrary to the classical convolutional neural networks, the feature map spatial size remains the same throughout the layers. Each layer of the network is essentially a convolutional block comprising of two conv layers. A filter size of 3 is used in the convolutional layers.
     Arguments:
 
         in_channels : input channels of the feature map, dtype : int
         out_channels : output channels of the feature map, dtype : int
         layers : list or tuple of output channels for each intermediate layer between the input and final output channels, dtype : list or tuple
@@ -612,19 +609,19 @@
     net = StaxNet(net_init, net_apply, (1,) + in_spatial + (in_channels,))
     net.initialize()
     return net
 
 
 def res_net(in_channels: int,
             out_channels: int,
-            layers: Tuple[int, ...] or List[int],
+            layers: Sequence[int],
             batch_norm: bool = False,
-            activation: str or Callable = 'ReLU',
+            activation: Union[str, Callable] = 'ReLU',
             periodic=False,
-            in_spatial: int or tuple = 2) -> StaxNet:
+            in_spatial: Union[int, tuple] = 2) -> StaxNet:
     """
     Built in Res-Nets are provided in the ΦFlow framework. Similar to the conv-net, the feature map spatial size remains the same throughout the layers.
     These networks use residual blocks composed of two conv layers with a skip connection added from the input to the output feature map.
     A default filter size of 3 is used in the convolutional layers.
 
     Arguments:
 
@@ -662,16 +659,16 @@
     return net
 
 
 def resnet_block(in_channels: int,
                  out_channels: int,
                  periodic: bool,
                  batch_norm: bool,
-                 activation: str or Callable = 'ReLU',
-                 d: int or tuple = 2):
+                 activation: Union[str, Callable] = 'ReLU',
+                 d: Union[int, tuple] = 2):
     activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
     init_fn, apply_fn = {}, {}
     init_fn['conv1'], apply_fn['conv1'] = stax.serial(
         CONV[d](out_channels, (3,) * d, padding='valid'),
         stax.BatchNorm(axis=tuple(range(d + 1))) if batch_norm else stax.Identity,
         activation)
     init_fn['conv2'], apply_fn['conv2'] = stax.serial(
@@ -753,15 +750,15 @@
 
     return checker
 
 
 def Dense_resnet_block(in_channels: int,
                        mid_channels: int,
                        batch_norm: bool = False,
-                       activation: str or Callable = 'ReLU'):
+                       activation: Union[str, Callable] = 'ReLU'):
     inputs = keras.Input(shape=(in_channels,))
     x_1 = inputs
 
     activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
     init_fn, apply_fn = {}, {}
     init_fn['dense1'], apply_fn['dense1'] = stax.serial(stax.Dense(mid_channels),
                                                         stax.BatchNorm(axis=(0,)),
@@ -791,19 +788,19 @@
         return out
 
     return net_init, net_apply
 
 
 def conv_net_unit(in_channels: int,
                   out_channels: int,
-                  layers: Tuple[int, ...] or List[int, ...],
+                  layers: Sequence[int],
                   periodic: bool = False,
                   batch_norm: bool = False,
-                  activation: str or Callable = 'ReLU',
-                  in_spatial: int or tuple = 2, **kwargs):
+                  activation: Union[str, Callable] = 'ReLU',
+                  in_spatial: Union[int, tuple] = 2, **kwargs):
     """ Conv-net unit for Invertible Nets"""
     if isinstance(in_spatial, int):
         d = in_spatial
     else:
         assert isinstance(in_spatial, tuple)
         d = len(in_spatial)
     if isinstance(activation, str):
@@ -859,19 +856,19 @@
 
     return net_init, net_apply
 
 
 def u_net_unit(in_channels: int,
                out_channels: int,
                levels: int = 4,
-               filters: int or tuple or list = 16,
+               filters: Union[int, tuple, list] = 16,
                batch_norm: bool = True,
                activation='ReLU',
                periodic=False,
-               in_spatial: tuple or int = 2,
+               in_spatial: Union[tuple, int] = 2,
                use_res_blocks: bool = False, **kwargs):
     """ U-net unit for Invertible Nets"""
     if isinstance(filters, (tuple, list)):
         assert len(filters) == levels, f"List of filters has length {len(filters)} but u-net has {levels} levels."
     else:
         filters = (filters,) * levels
     activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
@@ -932,19 +929,19 @@
         return x
 
     return net_init, net_apply
 
 
 def res_net_unit(in_channels: int,
                  out_channels: int,
-                 layers: Tuple[int, ...] or List[int],
+                 layers: Sequence[int],
                  batch_norm: bool = False,
-                 activation: str or Callable = 'ReLU',
+                 activation: Union[str, Callable] = 'ReLU',
                  periodic=False,
-                 in_spatial: int or tuple = 2, **kwargs):
+                 in_spatial: Union[int, tuple] = 2, **kwargs):
     """ Res-net unit for Invertible Nets"""
     if isinstance(in_spatial, int):
         d = in_spatial
     else:
         assert isinstance(in_spatial, tuple)
         d = len(in_spatial)
     activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
@@ -958,17 +955,17 @@
     return stax.serial(*stax_layers)
 
 
 NET = {'u_net': u_net_unit, 'res_net': res_net_unit, 'conv_net': conv_net_unit}
 
 
 def coupling_layer(in_channels: int,
-                   activation: str or Callable = 'ReLU',
+                   activation: Union[str, Callable] = 'ReLU',
                    batch_norm: bool = False,
-                   in_spatial: int or tuple = 2,
+                   in_spatial: Union[int, tuple] = 2,
                    net: str = 'u_net',
                    reverse_mask: bool = False,
                    **kwargs):
     if isinstance(in_spatial, int):
         d = in_spatial
     else:
         assert isinstance(in_spatial, tuple)
@@ -1041,16 +1038,16 @@
     return net_init, net_apply
 
 
 def invertible_net(in_channels: int,
                    num_blocks: int,
                    batch_norm: bool = False,
                    net: str = 'u_net',
-                   activation: str or type = 'ReLU',
-                   in_spatial: tuple or int = 2, **kwargs):
+                   activation: Union[str, type] = 'ReLU',
+                   in_spatial: Union[tuple, int] = 2, **kwargs):
     """
     ΦFlow also provides invertible neural networks that are capable of inverting the output tensor back to the input tensor initially passed.\ These networks have far reaching applications in predicting input parameters of a problem given its observations.\ Invertible nets are composed of multiple concatenated coupling blocks wherein each such block consists of arbitrary neural networks.
 
     Currently, these arbitrary neural networks could be set to u_net(default), conv_net, res_net or dense_net blocks with in_channels = out_channels.
     The architecture used is popularized by ["Real NVP"](https://arxiv.org/abs/1605.08803).
 
     Arguments:
```

### Comparing `phiflow-2.3.3/phi/math/__init__.py` & `phiflow-2.3.4/phi/math/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/math/_fit.py` & `phiflow-2.3.4/phi/math/_fit.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/math/_functional.py` & `phiflow-2.3.4/phi/math/_functional.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import types
 import warnings
 from functools import wraps, partial
-from typing import Tuple, Callable, Dict, Generic, List, TypeVar, Any, Set
+from typing import Tuple, Callable, Dict, Generic, List, TypeVar, Any, Set, Union
 
 import numpy as np
 
 from ._sparse import SparseCoordinateTensor, CompressedSparseMatrix
 from ._trace import ShiftLinTracer, matrix_from_function, LinearTraceInProgress
 from .backend import Backend, NUMPY
 from .backend._backend import get_spatial_derivative_order, functional_derivative_evaluation, PHI_LOGGER
@@ -19,18 +19,18 @@
 X = TypeVar('X')
 Y = TypeVar('Y')
 
 
 class SignatureKey:
 
     def __init__(self,
-                 source_function: Callable or None,
+                 source_function: Union[Callable, None],
                  tree: Dict[str, Any],
-                 shapes: Shape or Tuple[Shape],
-                 specs: Tuple[Shape] or None,
+                 shapes: Union[Shape, Tuple[Shape]],
+                 specs: Union[Tuple[Shape], None],
                  backend: Backend,
                  tracing: bool,
                  condition: Any = None):
         if source_function is None:  # this is an input signature
             assert isinstance(shapes, tuple)
         self.source_function = source_function
         self.tree: Dict[str, Any] = tree
@@ -122,32 +122,36 @@
 #     natives = [math.reshaped_native(t, [batch_shape, *t.shape.non_batch], force_expand=True) for t in tensors]
 #     natives, shapes, specs = disassemble_tensors(tensors, expand=cache)
 #     shapes = tuple([math.concat_shapes(batch(batch=batch_shape.volume), *t.shape.non_batch) for t in tensors])
 #     key = SignatureKey(None, tree, shapes, specs, backend, tracing, {})
 #     return key, tensors, natives, kwargs, batch_shape
 
 
-def function_parameters(f):
+def function_parameters(f) -> Tuple[str]:
+    return tuple(get_function_parameters(f).keys())
+
+
+def get_function_parameters(f) -> Dict[str, inspect.Parameter]:
     if isinstance(f, (JitFunction, GradientFunction, HessianFunction, CustomGradientFunction, LinearFunction)):
-        return f.f_params
+        return get_function_parameters(f.f)
     elif hasattr(f, '__wrapped__') and f.__wrapped__ is not None:
-        inner_params = function_parameters(f.__wrapped__)
+        inner_params = get_function_parameters(f.__wrapped__)
         outer_parameters = dict(inspect.signature(f, follow_wrapped=False).parameters)
         args_param = [name for name, param in outer_parameters.items() if param.kind == inspect.Parameter.VAR_POSITIONAL]
         assert args_param, f"Wrapping function {f.__name__} must have a varargs parameter"
         kwargs_param = [name for name, param in outer_parameters.items() if param.kind == inspect.Parameter.VAR_KEYWORD]
-        outer_params = list(outer_parameters.keys())
+        outer_names: List[str] = list(outer_parameters.keys())
         if kwargs_param:
-            outer_params.remove(kwargs_param[0])
-        index = outer_params.index(args_param[0])
-        return tuple(outer_params[:index]) + inner_params + tuple(outer_params[index + 1:])
+            outer_names.remove(kwargs_param[0])
+        index = outer_names.index(args_param[0])
+        return dict(**{n: outer_parameters[n] for n in outer_names[:index]}, **inner_params, **{n: outer_parameters[n] for n in outer_names[index + 1:]})
     else:
-        params = inspect.signature(f).parameters.keys()
+        params = dict(inspect.signature(f).parameters)
         assert 'args' not in params, f"Failed to determine signature of {f}. If it wraps another function, decorate it with @functools.wraps(func_with_signature)"
-        return tuple(params)
+        return params
 
 
 def f_name(f):
     assert callable(f), f
     if hasattr(f, '__name__'):
         return f.__name__
     if isinstance(f, partial):
@@ -405,15 +409,15 @@
     else:
         assert auxiliary_args is None
         f_params = function_parameters(f)
         auxiliary_args = f_params[1:]
     return f if isinstance(f, LinearFunction) and f.auxiliary_args == auxiliary_args else LinearFunction(f, auxiliary_args, forget_traces or False)
 
 
-def simplify_wrt(f, wrt: str or int or tuple or list):
+def simplify_wrt(f, wrt: Union[str, int, tuple, list]):
     f_params = function_parameters(f)
     if wrt is None:  # Old default
         wrt = f_params[0],
     elif isinstance(wrt, (tuple, list)) and all(isinstance(i, str) for i in wrt):
         wrt = tuple(wrt)
     elif isinstance(wrt, str) and ',' in wrt:
         wrt = tuple(i.strip() for i in wrt.split(',') if i.strip())
@@ -430,15 +434,15 @@
                       SyntaxWarning, stacklevel=4)
     return f_params, wrt
 
 
 class GradientFunction:
     """ Jacobian or Gradient of a function. """
 
-    def __init__(self, f: Callable, f_params, wrt: str or Tuple[str, ...], get_output: bool, is_f_scalar: bool, jit=False):
+    def __init__(self, f: Callable, f_params, wrt: Union[str, Tuple[str, ...]], get_output: bool, is_f_scalar: bool, jit=False):
         self.f = f
         self.f_params = f_params
         self.wrt = wrt
         self._wrt_tuple = wrt if isinstance(wrt, tuple) else (wrt,)
         self.get_output = get_output
         self.is_f_scalar = is_f_scalar
         self.traces: Dict[SignatureKey, Callable] = {}
@@ -958,15 +962,15 @@
     if traced_key.backend != key.backend:
         return False, f"Function was not traced with backend {key.backend}"
     if traced_key.spatial_derivative_order != key.spatial_derivative_order:
         return False, f"Different in spatial_derivative_order. This is likely an internal problem."
     return True
 
 
-def map_types(f: Callable, dims: Shape or tuple or list or str or Callable, dim_type: Callable or str) -> Callable:
+def map_types(f: Callable, dims: Union[Shape, tuple, list, str, Callable], dim_type: Union[Callable, str]) -> Callable:
     """
     Wraps a function to change the dimension types of its `Tensor` and `phi.math.magic.PhiTreeNode` arguments.
 
     Args:
         f: Function to wrap.
         dims: Concrete dimensions or dimension type, such as `spatial` or `batch`.
             These dimensions will be mapped to `dim_type` for all positional function arguments.
@@ -1017,15 +1021,15 @@
 
 def map_i2b(f: Callable) -> Callable:
     """ Map instance dimensions to batch dimensions. Short for `map_types(f, instance, batch)`. """
     return map_types(f, instance, batch)
 
 
 def iterate(f: Callable,
-            iterations: int or Shape,
+            iterations: Union[int, Shape],
             *x0,
             f_kwargs: dict = None,
             range: Callable = range,
             measure: Callable = None,
             **f_kwargs_):
     """
     Repeatedly call `function`, passing the previous output as the next input.
```

### Comparing `phiflow-2.3.3/phi/math/_magic_ops.py` & `phiflow-2.3.4/phi/math/_magic_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 def _any_uniform_dim(dims: Shape):
     for dim in dims:
         if dim.is_uniform:
             return dim
     raise ValueError(f"Uniform dimension required but found only non-uniform dimensions {dims}")
 
 
-def stack(values: tuple or list or dict, dim: Shape, expand_values=False, **kwargs):
+def stack(values: Union[tuple, list, dict], dim: Shape, expand_values=False, **kwargs):
     """
     Stacks `values` along the new dimension `dim`.
     All values must have the same spatial, instance and channel dimensions. If the dimension sizes vary, the resulting tensor will be non-uniform.
     Batch dimensions will be added as needed.
 
     Stacking tensors is performed lazily, i.e. the memory is allocated only when needed.
     This makes repeated stacking and slicing along the same dimension very efficient, i.e. jit-compiled functions will not perform these operations.
@@ -229,15 +229,15 @@
                         return reshaped
         # --- Fallback: multi-level stack ---
         for dim_ in reversed(dim):
             values = [stack(values[i:i + dim_.size], dim_, **kwargs) for i in range(0, len(values), dim_.size)]
         return values[0]
 
 
-def concat(values: tuple or list, dim: str or Shape, **kwargs):
+def concat(values: Union[tuple, list], dim: Union[str, Shape], **kwargs):
     """
     Concatenates a sequence of `phi.math.magic.Shapable` objects, e.g. `Tensor`, along one dimension.
     All values must have the same spatial, instance and channel dimensions and their sizes must be equal, except for `dim`.
     Batch dimensions will be added as needed.
 
     Args:
         values: Tuple or list of `phi.math.magic.Shapable`, such as `phi.math.Tensor`
@@ -415,15 +415,15 @@
     if shape(value).only(existing_dims).volume > 8:
         warnings.warn(f"rename_dims() default implementation is slow on large dimensions ({shape(value).only(dims)}). Please implement __replace_dims__() for {type(value).__name__} as defined in phi.math.magic", RuntimeWarning, stacklevel=2)
     for old_name, new_dim in zip(existing_dims.names, existing_names):
         value = stack(unstack(value, old_name), new_dim, **kwargs)
     return value
 
 
-def pack_dims(value, dims: DimFilter, packed_dim: Shape, pos: int or None = None, **kwargs):
+def pack_dims(value, dims: DimFilter, packed_dim: Shape, pos: Union[int, None] = None, **kwargs):
     """
     Compresses multiple dimensions into a single dimension by concatenating the elements.
     Elements along the new dimensions are laid out according to the order of `dims`.
     If the order of `dims` differs from the current dimension order, the tensor is transposed accordingly.
     This function replaces the traditional `reshape` for these cases.
 
     The type of the new dimension will be equal to the types of `dims`.
@@ -473,15 +473,15 @@
     if shape(value).only(dims).volume > 8:
         warnings.warn(f"pack_dims() default implementation is slow on large dimensions ({shape(value).only(dims)}). Please implement __pack_dims__() for {type(value).__name__} as defined in phi.math.magic", RuntimeWarning, stacklevel=2)
     return stack(unstack(value, dims), packed_dim, **kwargs)
 
 
 
 
-def unpack_dim(value, dim: str or Shape, *unpacked_dims: Shape, **kwargs):
+def unpack_dim(value, dim: Union[str, Shape], *unpacked_dims: Shape, **kwargs):
     """
     Decompresses a dimension by unstacking the elements along it.
     This function replaces the traditional `reshape` for these cases.
     The compressed dimension `dim` is assumed to contain elements laid out according to the order of `unpacked_dims`.
 
     If `dim` does not exist on `value`, this function will return `value` as-is. This includes primitive types.
 
@@ -647,15 +647,15 @@
 
 # Other Ops
 
 MagicType = TypeVar('MagicType')
 OtherMagicType = TypeVar('OtherMagicType')
 
 
-def cast(x: MagicType, dtype: DType or type) -> OtherMagicType:
+def cast(x: MagicType, dtype: Union[DType, type]) -> OtherMagicType:
     """
     Casts `x` to a different data type.
 
     Implementations:
 
     * NumPy: [`x.astype()`](numpy.ndarray.astype)
     * PyTorch: [`x.to()`](https://pytorch.org/docs/stable/tensors.html#torch.Tensor.to)
```

### Comparing `phiflow-2.3.3/phi/math/_nd.py` & `phiflow-2.3.4/phi/math/_nd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from functools import partial
-from typing import Tuple, Optional, List
+from typing import Tuple, Optional, List, Union
 
 import numpy as np
 
 from ._shape import Shape, channel, batch, spatial, DimFilter, parse_dim_order, shape, instance
 from .magic import PhiTreeNode
 from ._magic_ops import stack, rename_dims, concat, variable_values
 from ._tensors import Tensor, wrap, tensor
 from . import extrapolation as extrapolation
 from .extrapolation import Extrapolation
 from . import _ops as math
 from ._functional import jit_compile_linear
 from ._optimize import solve_linear
 
 
-def vec(name: str or Shape = 'vector', *sequence, tuple_dim=spatial('sequence'), list_dim=instance('sequence'), **components) -> Tensor:
+def vec(name: Union[str, Shape] = 'vector', *sequence, tuple_dim=spatial('sequence'), list_dim=instance('sequence'), **components) -> Tensor:
     """
     Lay out the given values along a channel dimension without converting them to the current backend.
 
     Args:
         name: Dimension name.
         *sequence: Component values that will also be used as item names.
             If specified, `components` must be empty.
@@ -62,15 +62,15 @@
                 return wrap(value, list_dim)
             else:
                 return value
         components = {n: wrap_sequence(v) for n, v in components.items()}
         return stack(components, dim, expand_values=True)
 
 
-def const_vec(value: float or Tensor, dim: Shape or tuple or list or str):
+def const_vec(value: Union[float, Tensor], dim: Union[Shape, tuple, list, str]):
     """
     Creates a single-dimension tensor with all values equal to `value`.
     `value` is not converted to the default backend, even when it is a Python primitive.
 
     Args:
         value: Value for filling the vector.
         dim: Either single-dimension non-spatial Shape or `Shape` consisting of any number of spatial dimensions.
@@ -88,15 +88,15 @@
             shape = dim
     else:
         dims = parse_dim_order(dim)
         shape = channel(vector=dims)
     return wrap([value] * shape.size, shape)
 
 
-def vec_abs(vec: Tensor, vec_dim: DimFilter = channel, eps: float or Tensor = None):
+def vec_abs(vec: Tensor, vec_dim: DimFilter = channel, eps: Union[float, Tensor] = None):
     """
     Computes the vector length of `vec`.
 
     Args:
         eps: Minimum vector length. Use to avoid `inf` gradients for zero-length vectors.
     """
     if vec.dtype.kind == complex:
@@ -142,15 +142,15 @@
             return vec1 * math.stack_tensors([-v2_y, v2_x], channel('vector'))
     elif spatial_rank == 3:  # Curl in 3D
         raise NotImplementedError(f'spatial_rank={spatial_rank} not yet implemented')
     else:
         raise AssertionError(f'dims = {spatial_rank}. Vector product not available in > 3 dimensions')
 
 
-def rotate_vector(vector: math.Tensor, angle: float or math.Tensor) -> Tensor:
+def rotate_vector(vector: math.Tensor, angle: Union[float, math.Tensor]) -> Tensor:
     """
     Rotates `vector` around the origin.
 
     Args:
         vector: n-dimensional vector with a channel dimension called `'vector'`
         angle: Euler angle. The direction is the rotation axis and the length is the amount (in radians).
 
@@ -167,15 +167,15 @@
         return math.stack_tensors([rot_x, rot_y], channel(vector=vector.vector.item_names))
     elif vector.vector.size == 1:
         raise AssertionError(f"Cannot rotate a 1D vector. shape={vector.shape}")
     else:
         raise NotImplementedError(f"Rotation in {vector.vector.size}D not yet implemented.")
 
 
-def dim_mask(all_dims: Shape or tuple or list, dims: DimFilter, mask_dim=channel('vector')) -> Tensor:
+def dim_mask(all_dims: Union[Shape, tuple, list], dims: DimFilter, mask_dim=channel('vector')) -> Tensor:
     """
     Creates a masked vector with 1 elements for `dims` and 0 for all other dimensions in `all_dims`.
 
     Args:
         all_dims: All dimensions for which the vector should have an entry.
         dims: Dimensions marked as 1.
         mask_dim: Dimension of the masked vector. Item names are assigned automatically.
@@ -189,15 +189,15 @@
         all_dims = spatial(*all_dims)
     dims = all_dims.only(dims)
     mask = [1 if dim in dims else 0 for dim in all_dims]
     mask_dim = mask_dim.with_size(all_dims.names)
     return wrap(mask, mask_dim)
 
 
-def normalize_to(target: Tensor, source: float or Tensor, epsilon=1e-5):
+def normalize_to(target: Tensor, source: Union[float, Tensor], epsilon=1e-5):
     """
     Multiplies the target so that its sum matches the source.
 
     Args:
         target: `Tensor`
         source: `Tensor` or constant
         epsilon: Small number to prevent division by zero.
@@ -357,15 +357,15 @@
 #         components.append(upper - lower)
 #     return math.sum_(components, 0)
 
 
 def shift(x: Tensor,
           offsets: tuple,
           dims: DimFilter = math.spatial,
-          padding: Extrapolation or Tensor or float or None = extrapolation.BOUNDARY,
+          padding: Union[Extrapolation, Tensor, float, None] = extrapolation.BOUNDARY,
           stack_dim: Optional[Shape] = channel('shift'),
           extend_bounds=0) -> list:
     """
     shift Tensor by a fixed offset and abiding by extrapolation
 
     Args:
         x: Input data
@@ -473,19 +473,19 @@
             values = math.where(math.is_finite(values), values, avg_neighbors)
     return values
 
 
 # Gradient
 
 def spatial_gradient(grid: Tensor,
-                     dx: float or Tensor = 1,
+                     dx: Union[float, Tensor] = 1,
                      difference: str = 'central',
-                     padding: Extrapolation or None = extrapolation.BOUNDARY,
+                     padding: Union[Extrapolation, None] = extrapolation.BOUNDARY,
                      dims: DimFilter = spatial,
-                     stack_dim: Shape or None = channel('gradient'),
+                     stack_dim: Union[Shape, None] = channel('gradient'),
                      pad=0) -> Tensor:
     """
     Calculates the spatial_gradient of a scalar channel from finite differences.
     The spatial_gradient vectors are in reverse order, lowest dimension first.
 
     Args:
         grid: grid values
@@ -523,15 +523,15 @@
     else:
         raise ValueError('Invalid difference type: {}. Can be CENTRAL or FORWARD'.format(difference))
 
 
 # Laplace
 
 def laplace(x: Tensor,
-            dx: Tensor or float = 1,
+            dx: Union[Tensor, float] = 1,
             padding: Extrapolation = extrapolation.BOUNDARY,
             dims: DimFilter = spatial,
             weights: Tensor = None):
     """
     Spatial Laplace operator as defined for scalar fields.
     If a vector field is passed, the laplace is computed component-wise.
 
@@ -560,15 +560,15 @@
         assert set(channel(weights).item_names[0]) >= set(dim_names), f"the channel dim of weights must contain all laplace dims {dim_names} but only has {channel(weights).item_names}"
         result *= rename_dims(weights, channel, batch('_laplace'))
     result = math.sum_(result, '_laplace')
     return result
 
 
 def fourier_laplace(grid: Tensor,
-                    dx: Tensor or Shape or float or list or tuple,
+                    dx: Union[Tensor, Shape, float, list, tuple],
                     times: int = 1):
     """
     Applies the spatial laplace operator to the given tensor with periodic boundary conditions.
     
     *Note:* The results of `fourier_laplace` and `laplace` are close but not identical.
     
     This implementation computes the laplace operator in Fourier space.
@@ -590,15 +590,15 @@
     k_squared = math.sum_(math.fftfreq(grid.shape) ** 2, 'vector')
     fft_laplace = -(2 * np.pi) ** 2 * k_squared
     result = math.real(math.ifft(frequencies * fft_laplace ** times))
     return math.cast(result / wrap(dx) ** 2, grid.dtype)
 
 
 def fourier_poisson(grid: Tensor,
-                    dx: Tensor or Shape or float or list or tuple,
+                    dx: Union[Tensor, Shape, float, list, tuple],
                     times: int = 1):
     """
     Inverse operation to `fourier_laplace`.
 
     Args:
       grid: Tensor: 
       dx: Tensor or Shape or float or list or tuple:
```

### Comparing `phiflow-2.3.3/phi/math/_ops.py` & `phiflow-2.3.4/phi/math/_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 import math
 import warnings
 from numbers import Number
-from typing import Tuple, Callable, Any
+from typing import Tuple, Callable, Any, Union
 
 import numpy as np
 
 from . import extrapolation as e_
 from ._magic_ops import expand, pack_dims, unpack_dim, cast, copy_with, value_attributes, bool_to_int
 from ._shape import (Shape, EMPTY_SHAPE,
                      spatial, batch, channel, instance, merge_shapes, parse_dim_order, concat_shapes,
@@ -97,15 +97,15 @@
     """
     for backend in BACKENDS:
         backend.seed(seed)
     import random
     random.seed(0)
 
 
-def native(value: Tensor or Number or tuple or list or Any):
+def native(value: Union[Tensor, Number, tuple, list, Any]):
     """
     Returns the native tensor representation of `value`.
     If `value` is a `phi.math.Tensor`, this is equal to calling `phi.math.Tensor.native()`.
     Otherwise, checks that `value` is a valid tensor object and returns it.
 
     Args:
         value: `Tensor` or native tensor or tensor-like.
@@ -119,15 +119,15 @@
     if isinstance(value, Tensor):
         return value.native()
     else:
         choose_backend(value)  # check that value is a native tensor
         return value
 
 
-def numpy(value: Tensor or Number or tuple or list or Any):
+def numpy(value: Union[Tensor, Number, tuple, list, Any]):
     """
     Converts `value` to a `numpy.ndarray` where value must be a `Tensor`, backend tensor or tensor-like.
     If `value` is a `phi.math.Tensor`, this is equal to calling `phi.math.Tensor.numpy()`.
 
     *Note*: Using this function breaks the autograd chain. The returned tensor is not differentiable.
     To get a differentiable tensor, use `Tensor.native()` instead.
 
@@ -146,15 +146,15 @@
         return value.numpy()
     else:
         backend = choose_backend(value)
         return backend.numpy(value)
 
 
 def reshaped_native(value: Tensor,
-                    groups: tuple or list,
+                    groups: Union[tuple, list],
                     force_expand: Any = False,
                     to_numpy=False):
     """
     Returns a native representation of `value` where dimensions are laid out according to `groups`.
 
     See Also:
         `native()`, `pack_dims()`, `reshaped_tensor()`, `reshaped_numpy()`.
@@ -190,15 +190,15 @@
         else:
             assert isinstance(group, str), f"Groups must be either single-dim str or Shape but got {group}"
             assert ',' not in group, f"When packing multiple dimensions, pass a well-defined Shape instead of a comma-separated str. Got {group}"
             order.append(group)
     return value.numpy(order) if to_numpy else value.native(order)
 
 
-def reshaped_numpy(value: Tensor, groups: tuple or list, force_expand: Any = False):
+def reshaped_numpy(value: Tensor, groups: Union[tuple, list], force_expand: Any = False):
     """
     Returns the NumPy representation of `value` where dimensions are laid out according to `groups`.
 
     See Also:
         `numpy()`, `reshaped_native()`, `pack_dims()`, `reshaped_tensor()`.
 
     Args:
@@ -212,15 +212,15 @@
     Returns:
         NumPy `ndarray` with dimensions matching `groups`.
     """
     return reshaped_native(value, groups, force_expand=force_expand, to_numpy=True)
 
 
 def reshaped_tensor(value: Any,
-                    groups: tuple or list,
+                    groups: Union[tuple, list],
                     check_sizes=False,
                     convert=True):
     """
     Creates a `Tensor` from a native tensor or tensor-like whereby the dimensions of `value` are split according to `groups`.
 
     See Also:
         `phi.math.tensor()`, `reshaped_native()`, `unpack_dim()`.
@@ -324,15 +324,15 @@
             groups = (batch, *spatial_dim, channel_dim) if channels_last else (batch, channel_dim, *spatial_dim)
         result = reshaped_tensor(output, groups, convert=False)
         if result.shape.get_size(channel_dim.name) == 1:
             result = result.dimension(channel_dim.name)[0]  # remove vector dim if not required
         return result
 
 
-def print_(obj: Tensor or PhiTreeNode or Number or tuple or list or None = None, name: str = ""):
+def print_(obj: Union[Tensor, PhiTreeNode, Number, tuple, list, None] = None, name: str = ""):
     """
     Print a tensor with no more than two spatial dimensions, slicing it along all batch and channel dimensions.
     
     Unlike NumPy's array printing, the dimensions are sorted.
     Elements along the alphabetically first dimension is printed to the right, the second dimension upward.
     Typically, this means x right, y up.
 
@@ -362,15 +362,15 @@
     elif isinstance(obj, PhiTreeNode):
         for n, val in variables(obj).items():
             print_(val, name + n)
     else:
         print(f"{wrap(obj):full}")
 
 
-def map_(function, *values, range=range, **kwargs) -> Tensor or None:
+def map_(function, *values, range=range, **kwargs) -> Union[Tensor, None]:
     """
     Calls `function` on all elements of `values`.
 
     Args:
         function: Function to be called on single elements contained in `value`. Must return a value that can be stored in tensors.
         *values: `Tensors` containing positional arguments for `function`.
             Number of tensors must match `function` signature.
@@ -434,15 +434,15 @@
 
     Returns:
         `Tensor`
     """
     return _initialize(lambda shape: expand_tensor(NativeTensor(default_backend().zeros((), dtype=DType.as_dtype(dtype)), EMPTY_SHAPE), shape), shape)
 
 
-def zeros_like(obj: Tensor or PhiTreeNode) -> Tensor or PhiTreeNode:
+def zeros_like(obj: Union[Tensor, PhiTreeNode]) -> Union[Tensor, PhiTreeNode]:
     """ Create a `Tensor` containing only `0.0` / `0` / `False` with the same shape and dtype as `obj`. """
     nest, values = disassemble_tree(obj)
     zeros_ = []
     for val in values:
         val = wrap(val)
         with val.default_backend:
             zeros_.append(zeros(val.shape, dtype=val.dtype))
@@ -496,17 +496,17 @@
         native = choose_backend(*shape.sizes, prefer_default=True).random_normal(shape.sizes, DType.as_dtype(dtype))
         return NativeTensor(native, shape)
 
     return _initialize(uniform_random_normal, shape)
 
 
 def random_uniform(*shape: Shape,
-                   low: Tensor or float = 0,
-                   high: Tensor or float = 1,
-                   dtype: DType or tuple = None) -> Tensor:
+                   low: Union[Tensor, float] = 0,
+                   high: Union[Tensor, float] = 1,
+                   dtype: Union[DType, tuple] = None) -> Tensor:
     """
     Creates a `Tensor` with the specified shape, filled with random values sampled from a uniform distribution.
 
     Args:
         *shape: This (possibly empty) sequence of `Shape`s is concatenated, preserving the order.
         dtype: (optional) `DType` or `(kind, bits)`.
             The dtype kind must be one of `float`, `int`, `complex`.
@@ -569,15 +569,15 @@
     dim = x.shape.only(dim)
     assert len(dim) == 1, f"dim must be a single dimension but got {dim}"
     native_x = x.native(x.shape)
     native_result = choose_backend(native_x).cumsum(native_x, x.shape.index(dim))
     return NativeTensor(native_result, x.shape)
 
 
-def fftfreq(resolution: Shape, dx: Tensor or float = 1, dtype: DType = None):
+def fftfreq(resolution: Shape, dx: Union[Tensor, float] = 1, dtype: DType = None):
     """
     Returns the discrete Fourier transform sample frequencies.
     These are the frequencies corresponding to the components of the result of `math.fft` on a tensor of shape `resolution`.
 
     Args:
         resolution: Grid resolution measured in cells
         dx: Distance between sampling points in real space.
@@ -587,15 +587,15 @@
         `Tensor` holding the frequencies of the corresponding values computed by math.fft
     """
     k = meshgrid(**{dim: np.fft.fftfreq(int(n)) for dim, n in resolution.spatial._named_sizes})
     k /= dx
     return to_float(k) if dtype is None else cast(k, dtype)
 
 
-def meshgrid(dim_type=spatial, stack_dim=channel('vector'), assign_item_names=True, **dimensions: int or Tensor) -> Tensor:
+def meshgrid(dim_type=spatial, stack_dim=channel('vector'), assign_item_names=True, **dimensions: Union[int, Tensor]) -> Tensor:
     """
     Generate a mesh-grid `Tensor` from keyword dimensions.
 
     Args:
         **dimensions: Mesh-grid dimensions, mapping names to values.
             Values may be `int`, 1D `Tensor` or 1D native tensor.
         dim_type: Dimension type of mesh-grid dimensions, one of `spatial`, `channel`, `batch`, `instance`.
@@ -628,15 +628,15 @@
     channels = [NativeTensor(t, grid_shape) for t in indices_list]
     if assign_item_names:
         return stack_tensors(channels, stack_dim.with_size(tuple(dimensions.keys())))
     else:
         return stack_tensors(channels, stack_dim)
 
 
-def linspace(start: int or Tensor, stop, dim: Shape) -> Tensor:
+def linspace(start: Union[int, Tensor], stop, dim: Shape) -> Tensor:
     """
     Returns `number` evenly spaced numbers between `start` and `stop`.
 
     See Also:
         `arange()`, `meshgrid()`.
 
     Args:
@@ -664,15 +664,15 @@
             stop = stop.native()
         native_linspace = choose_backend(start, stop, prefer_default=True).linspace(start, stop, dim.size)
         return NativeTensor(native_linspace, dim)
     else:
         return map_(linspace, start, stop, dim=dim)
 
 
-def arange(dim: Shape, start_or_stop: int or None = None, stop: int or None = None, step=1):
+def arange(dim: Shape, start_or_stop: Union[int, None] = None, stop: Union[int, None] = None, step=1):
     """
     Returns evenly spaced values between `start` and `stop`.
     If only one limit is given, `0` is used for the start.
 
     See Also:
         `range_tensor()`, `linspace()`, `meshgrid()`.
 
@@ -713,15 +713,15 @@
         `Tensor`
     """
     shape = concat_shapes(*shape)
     data = arange(spatial('range'), 0, shape.volume)
     return unpack_dim(data, 'range', shape)
 
 
-def stack_tensors(values: tuple or list, dim: Shape):
+def stack_tensors(values: Union[tuple, list], dim: Shape):
     if len(values) == 1 and not dim:
         return values[0]
     values = [wrap(v) for v in values]
     values = cast_same(*values)
 
     def inner_stack(*values):
         if len(values) > 1:
@@ -729,15 +729,15 @@
         else:
             return CollapsedTensor(values[0], values[0].shape & dim.with_size(1))
 
     result = broadcast_op(inner_stack, values)
     return result
 
 
-def concat_tensor(values: tuple or list, dim: str) -> Tensor:
+def concat_tensor(values: Union[tuple, list], dim: str) -> Tensor:
     assert len(values) > 0, "concat() got empty sequence"
     assert isinstance(dim, str), f"dim must be a single-dimension Shape but got '{dim}' of type {type(dim)}"
 
     def inner_concat(*values):
         broadcast_shape: Shape = values[0].shape  # merge_shapes(*[t.shape.with_sizes([None] * t.shape.rank) for t in values])
         dim_index = broadcast_shape.index(dim)
         natives = [v.native(order=broadcast_shape.names) for v in values]
@@ -748,15 +748,15 @@
             broadcast_shape = broadcast_shape.with_dim_size(dim, sum([v.shape.get_size(dim) for v in values]))
         return NativeTensor(concatenated, broadcast_shape)
 
     result = broadcast_op(inner_concat, values)
     return result
 
 
-def pad(value: Tensor, widths: dict, mode: 'e_.Extrapolation' or Tensor or Number, **kwargs) -> Tensor:
+def pad(value: Tensor, widths: dict, mode: Union['e_.Extrapolation', Tensor, Number], **kwargs) -> Tensor:
     """
     Pads a tensor along the specified dimensions, determining the added values using the given extrapolation.
     Unlike `Extrapolation.pad()`, this function can handle negative widths which slice off outer values.
 
     Args:
         value: `Tensor` to be padded
         widths: `dict` mapping dimension name (`str`) to `(lower, upper)`
@@ -862,15 +862,15 @@
     Returns:
         `Tensor` with channel dimensions of `grid`, spatial and instance dimensions of `coordinates` and combined batch dimensions.
     """
     result = broadcast_op(functools.partial(_grid_sample, extrap=extrap, pad_kwargs=kwargs), [grid, coordinates])
     return result
 
 
-def _grid_sample(grid: Tensor, coordinates: Tensor, extrap: 'e_.Extrapolation' or None, pad_kwargs: dict):
+def _grid_sample(grid: Tensor, coordinates: Tensor, extrap: Union['e_.Extrapolation', None], pad_kwargs: dict):
     if grid.shape.batch == coordinates.shape.batch or grid.shape.batch.volume == 1 or coordinates.shape.batch.volume == 1:
         # call backend.grid_sample()
         batch = grid.shape.batch & coordinates.shape.batch
         backend = choose_backend_t(grid, coordinates)
         result = NotImplemented
         if extrap is None:
             result = backend.grid_sample(reshaped_native(grid, [batch, *grid.shape.spatial, grid.shape.channel]),
@@ -903,16 +903,16 @@
     right_weights = coordinates % 1
     weights = prod(binary * right_weights + (1 - binary) * (1 - right_weights), 'vector')
     result = sum_(neighbors * weights, dim=[f"_closest_{dim}" for dim in grid.shape.spatial.names])
     return result
 
 
 def broadcast_op(operation: Callable,
-                 tensors: tuple or list,
-                 iter_dims: set or tuple or list or Shape = None,
+                 tensors: Union[tuple, list],
+                 iter_dims: Union[set, tuple, list, Shape] = None,
                  no_return=False):
     if iter_dims is None:
         iter_dims = set()
         for tensor in tensors:
             if isinstance(tensor, TensorStack) and tensor.requires_broadcast:
                 iter_dims.add(tensor._stack_dim.name)
     if len(iter_dims) == 0:
@@ -943,15 +943,15 @@
         for i in range(size):
             gathered = [t[i] if isinstance(t, tuple) else t for t in unstacked]
             result_unstacked.append(broadcast_op(operation, gathered, iter_dims=set(iter_dims) - {dim}))
         if not no_return:
             return TensorStack(result_unstacked, Shape((None,), (dim,), (dim_type,), (item_names,)))
 
 
-def where(condition: Tensor or float or int, value_true: Tensor or float or int, value_false: Tensor or float or int):
+def where(condition: Union[Tensor, float, int], value_true: Union[Tensor, float, int], value_false: Union[Tensor, float, int]):
     """
     Builds a tensor by choosing either values from `value_true` or `value_false` depending on `condition`.
     If `condition` is not of type boolean, non-zero values are interpreted as True.
     
     This function requires non-None values for `value_true` and `value_false`.
     To get the indices of True / non-zero values, use :func:`nonzero`.
 
@@ -973,15 +973,15 @@
         shape, (c, vt, vf) = broadcastable_native_tensors(c, vt, vf)
         result = choose_backend(c, vt, vf).where(c, vt, vf)
         return NativeTensor(result, shape)
 
     return broadcast_op(inner_where, [condition, value_true, value_false])
 
 
-def nonzero(value: Tensor, list_dim: Shape or str = instance('nonzero'), index_dim: Shape = channel('vector')):
+def nonzero(value: Tensor, list_dim: Union[Shape, str] = instance('nonzero'), index_dim: Shape = channel('vector')):
     """
     Get spatial indices of non-zero / True values.
     
     Batch dimensions are preserved by this operation.
     If channel dimensions are present, this method returns the indices where any component is nonzero.
 
     Implementations:
@@ -1036,15 +1036,15 @@
             value = wrap(value)
         dims = value.shape.only(dims)
         if require_all_dims_present and any(d not in value.shape for d in dims):
             raise ValueError(f"Cannot sum dimensions {dims} because tensor {value.shape} is missing at least one of them")
         return f(value._simplify(), dims)
 
 
-def sum_(value: Tensor or list or tuple, dim: DimFilter = non_batch) -> Tensor:
+def sum_(value: Union[Tensor, list, tuple], dim: DimFilter = non_batch) -> Tensor:
     """
     Sums `values` along the specified dimensions.
 
     Args:
         value: `Tensor` or `list` / `tuple` of Tensors.
         dim: Dimension or dimensions to be reduced. One of
 
@@ -1088,15 +1088,15 @@
             return dot(value, dims, ones(dims), dims)  # this is what SciPy does in both axes, actually.
         return value
         # first sum value dims that are not part of indices
     else:
         raise ValueError(type(value))
 
 
-def prod(value: Tensor or list or tuple, dim: DimFilter = non_batch) -> Tensor:
+def prod(value: Union[Tensor, list, tuple], dim: DimFilter = non_batch) -> Tensor:
     """
     Multiplies `values` along the specified dimensions.
 
     Args:
         value: `Tensor` or `list` / `tuple` of Tensors.
         dim: Dimension or dimensions to be reduced. One of
 
@@ -1123,15 +1123,15 @@
     elif isinstance(value, TensorStack):
         reduced_inners = [_prod(t, dims.without(value._stack_dim)) for t in value._tensors]
         return functools.reduce(lambda x, y: x * y, reduced_inners) if value._stack_dim in dims else TensorStack(reduced_inners, value._stack_dim)
     else:
         raise ValueError(type(value))
 
 
-def mean(value: Tensor or list or tuple, dim: DimFilter = non_batch) -> Tensor:
+def mean(value: Union[Tensor, list, tuple], dim: DimFilter = non_batch) -> Tensor:
     """
     Computes the mean over `values` along the specified dimensions.
 
     Args:
         value: `Tensor` or `list` / `tuple` of Tensors.
         dim: Dimension or dimensions to be reduced. One of
 
@@ -1160,15 +1160,15 @@
     elif isinstance(value, TensorStack):
         reduced_inners = [_mean(t, dims.without(value._stack_dim)) for t in value._tensors]
         return functools.reduce(lambda x, y: x + y, reduced_inners) / len(reduced_inners) if value._stack_dim in dims else TensorStack(reduced_inners, value._stack_dim)
     else:
         raise ValueError(type(value))
 
 
-def std(value: Tensor or list or tuple, dim: DimFilter = non_batch) -> Tensor:
+def std(value: Union[Tensor, list, tuple], dim: DimFilter = non_batch) -> Tensor:
     """
     Computes the standard deviation over `values` along the specified dimensions.
 
     *Warning*: The standard deviation of non-uniform tensors along the stack dimension is undefined.
 
     Args:
         value: `Tensor` or `list` / `tuple` of Tensors.
@@ -1188,15 +1188,15 @@
 
 
 def _std(value: Tensor, dims: Shape) -> Tensor:
     result = value.default_backend.std(value.native(value.shape), value.shape.indices(dims))
     return NativeTensor(result, value.shape.without(dims))
 
 
-def any_(boolean_tensor: Tensor or list or tuple, dim: DimFilter = non_batch) -> Tensor:
+def any_(boolean_tensor: Union[Tensor, list, tuple], dim: DimFilter = non_batch) -> Tensor:
     """
     Tests whether any entry of `boolean_tensor` is `True` along the specified dimensions.
 
     Args:
         boolean_tensor: `Tensor` or `list` / `tuple` of Tensors.
         dim: Dimension or dimensions to be reduced. One of
 
@@ -1223,15 +1223,15 @@
     elif isinstance(value, TensorStack):
         reduced_inners = [_any(t, dims.without(value._stack_dim)) for t in value._tensors]
         return functools.reduce(lambda x, y: x | y, reduced_inners) if value._stack_dim in dims else TensorStack(reduced_inners, value._stack_dim)
     else:
         raise ValueError(type(value))
 
 
-def all_(boolean_tensor: Tensor or list or tuple, dim: DimFilter = non_batch) -> Tensor:
+def all_(boolean_tensor: Union[Tensor, list, tuple], dim: DimFilter = non_batch) -> Tensor:
     """
     Tests whether all entries of `boolean_tensor` are `True` along the specified dimensions.
 
     Args:
         boolean_tensor: `Tensor` or `list` / `tuple` of Tensors.
         dim: Dimension or dimensions to be reduced. One of
 
@@ -1258,15 +1258,15 @@
     elif isinstance(value, TensorStack):
         reduced_inners = [_all(t, dims.without(value._stack_dim)) for t in value._tensors]
         return functools.reduce(lambda x, y: x & y, reduced_inners) if value._stack_dim in dims else TensorStack(reduced_inners, value._stack_dim)
     else:
         raise ValueError(type(value))
 
 
-def max_(value: Tensor or list or tuple, dim: DimFilter = non_batch) -> Tensor:
+def max_(value: Union[Tensor, list, tuple], dim: DimFilter = non_batch) -> Tensor:
     """
     Determines the maximum value of `values` along the specified dimensions.
 
     Args:
         value: `Tensor` or `list` / `tuple` of Tensors.
         dim: Dimension or dimensions to be reduced. One of
 
@@ -1293,15 +1293,15 @@
     elif isinstance(value, TensorStack):
         reduced_inners = [_max(t, dims.without(value._stack_dim)) for t in value._tensors]
         return functools.reduce(lambda x, y: maximum(x, y), reduced_inners) if value._stack_dim in dims else TensorStack(reduced_inners, value._stack_dim)
     else:
         raise ValueError(type(value))
 
 
-def min_(value: Tensor or list or tuple, dim: DimFilter = non_batch) -> Tensor:
+def min_(value: Union[Tensor, list, tuple], dim: DimFilter = non_batch) -> Tensor:
     """
     Determines the minimum value of `values` along the specified dimensions.
 
     Args:
         value: `Tensor` or `list` / `tuple` of Tensors.
         dim: Dimension or dimensions to be reduced. One of
 
@@ -1328,15 +1328,15 @@
     elif isinstance(value, TensorStack):
         reduced_inners = [_min(t, dims.without(value._stack_dim)) for t in value._tensors]
         return functools.reduce(lambda x, y: minimum(x, y), reduced_inners) if value._stack_dim in dims else TensorStack(reduced_inners, value._stack_dim)
     else:
         raise ValueError(type(value))
 
 
-def finite_min(value, dim: DimFilter = non_batch, default: complex or float = float('NaN')):
+def finite_min(value, dim: DimFilter = non_batch, default: Union[complex, float] = float('NaN')):
     """
     Finds the minimum along `dim` ignoring all non-finite values.
 
     Args:
         value: `Tensor` or `list` / `tuple` of Tensors.
         dim: Dimension or dimensions to be reduced. One of
 
@@ -1353,15 +1353,15 @@
         `Tensor` without the reduced dimensions.
     """
     value_inf = where(is_finite(value), value, float('inf'))
     result_inf = min_(value_inf, dim)
     return where(is_finite(result_inf), result_inf, default)
 
 
-def finite_max(value, dim: DimFilter = non_batch, default: complex or float = float('NaN')):
+def finite_max(value, dim: DimFilter = non_batch, default: Union[complex, float] = float('NaN')):
     """
     Finds the maximum along `dim` ignoring all non-finite values.
 
     Args:
         value: `Tensor` or `list` / `tuple` of Tensors.
         dim: Dimension or dimensions to be reduced. One of
 
@@ -1378,15 +1378,15 @@
         `Tensor` without the reduced dimensions.
     """
     value_inf = where(is_finite(value), value, float('-inf'))
     result_inf = max_(value_inf, dim)
     return where(is_finite(result_inf), result_inf, default)
 
 
-def finite_sum(value, dim: DimFilter = non_batch, default: complex or float = float('NaN')):
+def finite_sum(value, dim: DimFilter = non_batch, default: Union[complex, float] = float('NaN')):
     """
     Sums all finite values in `value` along `dim`.
 
     Args:
         value: `Tensor` or `list` / `tuple` of Tensors.
         dim: Dimension or dimensions to be reduced. One of
 
@@ -1403,15 +1403,15 @@
         `Tensor` without the reduced dimensions.
     """
     finite = is_finite(value)
     summed = sum_(where(finite, value, 0), dim)
     return where(any_(finite, dim), summed, default)
 
 
-def finite_mean(value, dim: DimFilter = non_batch, default: complex or float = float('NaN')):
+def finite_mean(value, dim: DimFilter = non_batch, default: Union[complex, float] = float('NaN')):
     """
     Computes the mean value of all finite values in `value` along `dim`.
 
     Args:
         value: `Tensor` or `list` / `tuple` of Tensors.
         dim: Dimension or dimensions to be reduced. One of
 
@@ -1431,15 +1431,15 @@
     summed = sum_(where(finite, value, 0), dim)
     count = sum_(finite, dim)
     mean_nan = summed / count
     return where(is_finite(mean_nan), mean_nan, default)
 
 
 def quantile(value: Tensor,
-             quantiles: float or tuple or list or Tensor,
+             quantiles: Union[float, tuple, list, Tensor],
              dim: DimFilter = non_batch):
     """
     Compute the q-th quantile of `value` along `dim` for each q in `quantiles`.
 
     Implementations:
 
     * NumPy: [`quantile`](https://numpy.org/doc/stable/reference/generated/numpy.quantile.html)
@@ -1577,30 +1577,30 @@
                     y_letters.append(next_letter)
         keep_letters = [letter_map[dim] for dim in result_shape.names]
         subscripts = f'{"".join(x_letters)},{"".join(y_letters)}->{"".join(keep_letters)}'
         result_native = backend.einsum(subscripts, x_native, y_native)
     return NativeTensor(result_native, result_shape)
 
 
-def _backend_op1(x, unbound_method) -> Tensor or PhiTreeNode:
+def _backend_op1(x, unbound_method) -> Union[Tensor, PhiTreeNode]:
     if isinstance(x, Tensor):
         def apply_op(native_tensor):
             backend = choose_backend(native_tensor)
             return getattr(backend, unbound_method.__name__)(backend.auto_cast(native_tensor)[0])
         apply_op.__name__ = unbound_method.__name__
         return x._op1(apply_op)
     elif isinstance(x, PhiTreeNode):
         return copy_with(x, **{a: _backend_op1(getattr(x, a), unbound_method) for a in value_attributes(x)})
     else:
         backend = choose_backend(x)
         y = getattr(backend, unbound_method.__name__)(backend.auto_cast(x)[0])
         return y
 
 
-def abs_(x) -> Tensor or PhiTreeNode:
+def abs_(x) -> Union[Tensor, PhiTreeNode]:
     """
     Computes *||x||<sub>1</sub>*.
     Complex `x` result in matching precision float values.
 
     *Note*: The gradient of this operation is undefined for *x=0*.
     TensorFlow and PyTorch return 0 while Jax returns 1.
 
@@ -1609,54 +1609,54 @@
 
     Returns:
         Absolute value of `x` of same type as `x`.
     """
     return _backend_op1(x, Backend.abs)
 
 
-def sign(x) -> Tensor or PhiTreeNode:
+def sign(x) -> Union[Tensor, PhiTreeNode]:
     """
     The sign of positive numbers is 1 and -1 for negative numbers.
     The sign of 0 is undefined.
 
     Args:
         x: `Tensor` or `phi.math.magic.PhiTreeNode`
 
     Returns:
         `Tensor` or `phi.math.magic.PhiTreeNode` matching `x`.
     """
     return _backend_op1(x, Backend.sign)
 
 
-def round_(x) -> Tensor or PhiTreeNode:
+def round_(x) -> Union[Tensor, PhiTreeNode]:
     """ Rounds the `Tensor` or `phi.math.magic.PhiTreeNode` `x` to the closest integer. """
     return _backend_op1(x, Backend.round)
 
 
-def ceil(x) -> Tensor or PhiTreeNode:
+def ceil(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes *⌈x⌉* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.ceil)
 
 
-def floor(x) -> Tensor or PhiTreeNode:
+def floor(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes *⌊x⌋* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.floor)
 
 
-def sqrt(x) -> Tensor or PhiTreeNode:
+def sqrt(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes *sqrt(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.sqrt)
 
 
-def exp(x) -> Tensor or PhiTreeNode:
+def exp(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes *exp(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.exp)
 
 
-def to_float(x) -> Tensor or PhiTreeNode:
+def to_float(x) -> Union[Tensor, PhiTreeNode]:
     """
     Converts the given tensor to floating point format with the currently specified precision.
     
     The precision can be set globally using `math.set_global_precision()` and locally using `with math.precision()`.
     
     See the `phi.math` module documentation at https://tum-pbs.github.io/PhiFlow/Math.html
 
@@ -1668,25 +1668,25 @@
 
     Returns:
         `Tensor` or `phi.math.magic.PhiTreeNode` matching `x`.
     """
     return _backend_op1(x, Backend.to_float)
 
 
-def to_int32(x) -> Tensor or PhiTreeNode:
+def to_int32(x) -> Union[Tensor, PhiTreeNode]:
     """ Converts the `Tensor` or `phi.math.magic.PhiTreeNode` `x` to 32-bit integer. """
     return _backend_op1(x, Backend.to_int32)
 
 
-def to_int64(x) -> Tensor or PhiTreeNode:
+def to_int64(x) -> Union[Tensor, PhiTreeNode]:
     """ Converts the `Tensor` or `phi.math.magic.PhiTreeNode` `x` to 64-bit integer. """
     return _backend_op1(x, Backend.to_int64)
 
 
-def to_complex(x) -> Tensor or PhiTreeNode:
+def to_complex(x) -> Union[Tensor, PhiTreeNode]:
     """
     Converts the given tensor to complex floating point format with the currently specified precision.
 
     The precision can be set globally using `math.set_global_precision()` and locally using `with math.precision()`.
 
     See the `phi.math` module documentation at https://tum-pbs.github.io/PhiFlow/Math.html
 
@@ -1698,34 +1698,34 @@
 
     Returns:
         `Tensor` of same shape as `x`
     """
     return _backend_op1(x, Backend.to_complex)
 
 
-def is_finite(x) -> Tensor or PhiTreeNode:
+def is_finite(x) -> Union[Tensor, PhiTreeNode]:
     """ Returns a `Tensor` or `phi.math.magic.PhiTreeNode` matching `x` with values `True` where `x` has a finite value and `False` otherwise. """
     return _backend_op1(x, Backend.isfinite)
 
 
-def real(x) -> Tensor or PhiTreeNode:
+def real(x) -> Union[Tensor, PhiTreeNode]:
     """
     See Also:
         `imag()`, `conjugate()`.
 
     Args:
         x: `Tensor` or `phi.math.magic.PhiTreeNode` or native tensor.
 
     Returns:
         Real component of `x`.
     """
     return _backend_op1(x, Backend.real)
 
 
-def imag(x) -> Tensor or PhiTreeNode:
+def imag(x) -> Union[Tensor, PhiTreeNode]:
     """
     Returns the imaginary part of `x`.
     If `x` does not store complex numbers, returns a zero tensor with the same shape and dtype as this tensor.
 
     See Also:
         `real()`, `conjugate()`.
 
@@ -1734,15 +1734,15 @@
 
     Returns:
         Imaginary component of `x` if `x` is complex, zeros otherwise.
     """
     return _backend_op1(x, Backend.imag)
 
 
-def conjugate(x) -> Tensor or PhiTreeNode:
+def conjugate(x) -> Union[Tensor, PhiTreeNode]:
     """
     See Also:
         `imag()`, `real()`.
 
     Args:
         x: Real or complex `Tensor` or `phi.math.magic.PhiTreeNode` or native tensor.
 
@@ -1753,44 +1753,44 @@
 
 
 def degrees(deg):
     """ Convert degrees to radians. """
     return deg * (3.1415 / 180.)
 
 
-def sin(x) -> Tensor or PhiTreeNode:
+def sin(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes *sin(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.sin)
 
 
-def arcsin(x) -> Tensor or PhiTreeNode:
+def arcsin(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes the inverse of *sin(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`.
     For real arguments, the result lies in the range [-π/2, π/2].
     """
     return _backend_op1(x, Backend.arcsin)
 
 
-def cos(x) -> Tensor or PhiTreeNode:
+def cos(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes *cos(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.cos)
 
 
-def arccos(x) -> Tensor or PhiTreeNode:
+def arccos(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes the inverse of *cos(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`.
     For real arguments, the result lies in the range [0, π].
     """
     return _backend_op1(x, Backend.cos)
 
 
-def tan(x) -> Tensor or PhiTreeNode:
+def tan(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes *tan(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.tan)
 
 
-def arctan(x, divide_by=None) -> Tensor or PhiTreeNode:
+def arctan(x, divide_by=None) -> Union[Tensor, PhiTreeNode]:
     """
     Computes the inverse of *tan(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`.
 
     Args:
         x: Input. The single-argument `arctan` function cannot output π/2 or -π/2 since tan(π/2) is infinite.
         divide_by: If specified, computes `arctan(x/divide_by)` so that it can return π/2 and -π/2.
             This is equivalent to the common `arctan2` function.
@@ -1798,60 +1798,60 @@
     if divide_by is None:
         return _backend_op1(x, Backend.arctan)
     else:
         divide_by = to_float(divide_by)
         return custom_op2(x, divide_by, arctan, lambda a, b: choose_backend(a, b).arctan2(a, b), 'arctan')
 
 
-def sinh(x) -> Tensor or PhiTreeNode:
+def sinh(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes *sinh(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.sinh)
 
 
-def arcsinh(x) -> Tensor or PhiTreeNode:
+def arcsinh(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes the inverse of *sinh(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.arcsinh)
 
 
-def cosh(x) -> Tensor or PhiTreeNode:
+def cosh(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes *cosh(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.cosh)
 
 
-def arccosh(x) -> Tensor or PhiTreeNode:
+def arccosh(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes the inverse of *cosh(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.arccosh)
 
 
-def tanh(x) -> Tensor or PhiTreeNode:
+def tanh(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes *tanh(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.tanh)
 
 
-def arctanh(x) -> Tensor or PhiTreeNode:
+def arctanh(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes the inverse of *tanh(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.arctanh)
 
 
-def log(x) -> Tensor or PhiTreeNode:
+def log(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes the natural logarithm of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.log)
 
 
-def log2(x) -> Tensor or PhiTreeNode:
+def log2(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes *log(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x` with base 2. """
     return _backend_op1(x, Backend.log2)
 
 
-def log10(x) -> Tensor or PhiTreeNode:
+def log10(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes *log(x)* of the `Tensor` or `phi.math.magic.PhiTreeNode` `x` with base 10. """
     return _backend_op1(x, Backend.log10)
 
 
-def sigmoid(x) -> Tensor or PhiTreeNode:
+def sigmoid(x) -> Union[Tensor, PhiTreeNode]:
     """ Computes the sigmoid function of the `Tensor` or `phi.math.magic.PhiTreeNode` `x`. """
     return _backend_op1(x, Backend.sigmoid)
 
 
 def cast_same(*values: Tensor) -> Tuple[Tensor]:
     """
     Casts all tensors to the same `DType`.
@@ -1869,35 +1869,35 @@
     if any(dt != dtypes[0] for dt in dtypes):
         common_type = combine_types(*dtypes, fp_precision=get_precision())
         return tuple([cast(v, common_type) for v in values])
     else:
         return values
 
 
-def divide_no_nan(x: float or Tensor, y: float or Tensor):
+def divide_no_nan(x: Union[float, Tensor], y: Union[float, Tensor]):
     """ Computes *x/y* with the `Tensor`s `x` and `y` but returns 0 where *y=0*. """
     return custom_op2(x, y,
                       l_operator=divide_no_nan,
                       l_native_function=lambda x_, y_: choose_backend(x_, y_).divide_no_nan(x_, y_),
                       r_operator=lambda y_, x_: divide_no_nan(x_, y_),
                       r_native_function=lambda y_, x_: choose_backend(x_, y_).divide_no_nan(x_, y_),
                       op_name='divide_no_nan')
 
 
-def maximum(x: Tensor or float, y: Tensor or float):
+def maximum(x: Union[Tensor, float], y: Union[Tensor, float]):
     """ Computes the element-wise maximum of `x` and `y`. """
     return custom_op2(x, y, maximum, lambda x_, y_: choose_backend(x_, y_).maximum(x_, y_), op_name='maximum')
 
 
-def minimum(x: Tensor or float, y: Tensor or float):
+def minimum(x: Union[Tensor, float], y: Union[Tensor, float]):
     """ Computes the element-wise minimum of `x` and `y`. """
     return custom_op2(x, y, minimum, lambda x_, y_: choose_backend(x_, y_).minimum(x_, y_), op_name='minimum')
 
 
-def clip(x: Tensor, lower_limit: float or Tensor, upper_limit: float or Tensor):
+def clip(x: Tensor, lower_limit: Union[float, Tensor], upper_limit: Union[float, Tensor]):
     """ Limits the values of the `Tensor` `x` to lie between `lower_limit` and `upper_limit` (inclusive). """
     if isinstance(lower_limit, Number) and isinstance(upper_limit, Number):
 
         def clip_(x):
             return x._op1(lambda native: choose_backend(native).clip(native, lower_limit, upper_limit))
 
         return broadcast_op(clip_, [x])
@@ -1973,15 +1973,15 @@
             total = int(sum_(to_int64(mask_1d), mask_1d.shape))
             new_shape = mask_1d.shape.with_sizes([total])
             return expand(x, new_shape)
 
     return broadcast_op(uniform_boolean_mask, [x, mask], iter_dims=mask.shape.without(dim))
 
 
-def gather(values: Tensor, indices: Tensor, dims: DimFilter or None = None):
+def gather(values: Tensor, indices: Tensor, dims: Union[DimFilter, None] = None):
     """
     Gathers the entries of `values` at positions described by `indices`.
     All non-channel dimensions of `indices` that are part of `values` but not indexed are treated as batch dimensions.
 
     See Also:
         `scatter()`.
 
@@ -2023,17 +2023,17 @@
     native_result = backend.batched_gather_nd(native_values, native_indices)
     result = reshaped_tensor(native_result, [batch_, *index_list_dims, channel_], convert=False)
     if squeeze_index_list:
         result = result[{'_single_index': 0}]
     return result
 
 
-def scatter(base_grid: Tensor or Shape,
+def scatter(base_grid: Union[Tensor, Shape],
             indices: Tensor,
-            values: Tensor or float,
+            values: Union[Tensor, float],
             mode: str = 'update',
             outside_handling: str = 'discard',
             indices_gradient=False):
     """
     Scatters `values` into `base_grid` at `indices`.
     instance dimensions of `indices` and/or `values` are reduced during scattering.
     Depending on `mode`, this method has one of the following effects:
@@ -2202,15 +2202,15 @@
     """
     if isinstance(x, Tensor):
         return x.dtype
     else:
         return choose_backend(x).dtype(x)
 
 
-def expand_tensor(value: float or Tensor, dims: Shape):
+def expand_tensor(value: Union[float, Tensor], dims: Shape):
     if not dims:
         return value
     value = wrap(value)
     shape = value.shape
     for dim in reversed(dims):
         if dim in value.shape:
             shape &= dim  # checks sizes, copies item names
@@ -2386,15 +2386,15 @@
         nest, values = disassemble_tree(x)
         new_values = [stop_gradient(v) for v in values]
         return assemble_tree(nest, new_values)
     else:
         return wrap(choose_backend(x).stop_gradient(x))
 
 
-def pairwise_distances(positions: Tensor, max_distance: float or Tensor = None, others_dims=instance('others'), format='dense') -> Tensor:
+def pairwise_distances(positions: Tensor, max_distance: Union[float, Tensor] = None, others_dims=instance('others'), format='dense') -> Tensor:
     """
     Computes the distance matrix containing the pairwise position differences between each pair of points.
     Points that are further apart than `max_distance` are assigned a distance value of `0`.
     The diagonal of the matrix (self-distance) also consists purely of zero-vectors.
 
     Args:
         positions: `Tensor`.
```

### Comparing `phiflow-2.3.3/phi/math/_optimize.py` & `phiflow-2.3.4/phi/math/_optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 
 class Solve(Generic[X, Y]):
     """
     Specifies parameters and stopping criteria for solving a minimization problem or system of equations.
     """
 
     def __init__(self,
-                 method: str or None = 'auto',
-                 rel_tol: float or Tensor = None,
-                 abs_tol: float or Tensor = None,
-                 x0: X or Any = None,
+                 method: Union[str, None] = 'auto',
+                 rel_tol: Union[float, Tensor] = None,
+                 abs_tol: Union[float, Tensor] = None,
+                 x0: Union[X, Any] = None,
                  max_iterations: Union[int, Tensor] = 1000,
-                 suppress: tuple or list = (),
+                 suppress: Union[tuple, list] = (),
                  preprocess_y: Callable = None,
                  preprocess_y_args: tuple = (),
-                 gradient_solve: 'Solve[Y, X]' or None = None):
+                 gradient_solve: Union['Solve[Y, X]', None] = None):
         method = method or 'auto'
         assert isinstance(method, str)
         self.method: str = method
         """ Optimization method to use. Available solvers depend on the solve function that is used to perform the solve. """
         self.rel_tol: Tensor = math.to_float(wrap(rel_tol)) if rel_tol is not None else None
         """Relative tolerance for linear solves only, defaults to 1e-5 for singe precision solves and 1e-12 for double precision solves.
         This must be unset or `0` for minimization problems.
@@ -134,17 +134,17 @@
 
     When representing the full optimization trajectory, all tracked quantities will have an additional `trajectory` batch dimension.
     """
 
     def __init__(self,
                  solve: Solve,
                  x: X,
-                 residual: Y or None,
-                 iterations: Tensor or None,
-                 function_evaluations: Tensor or None,
+                 residual: Union[Y, None],
+                 iterations: Union[Tensor, None],
+                 function_evaluations: Union[Tensor, None],
                  converged: Tensor,
                  diverged: Tensor,
                  method: str,
                  msg: Tensor,
                  solve_time: float):
         # tuple.__new__(SolveInfo, (x, residual, iterations, function_evaluations, converged, diverged))
         self.solve: Solve[X, Y] = solve
@@ -451,15 +451,15 @@
     from ._nd import l2_loss
     solve = solve.with_defaults('solve')
     tol = math.maximum(solve.rel_tol * l2_loss(y), solve.abs_tol)
     min_solve = copy_with(solve, abs_tol=tol, rel_tol=0, preprocess_y=None)
     return minimize(min_func, min_solve)
 
 
-def solve_linear(f: Callable[[X], Y] or Tensor,
+def solve_linear(f: Union[Callable[[X], Y], Tensor],
                  y: Y,
                  solve: Solve[X, Y],
                  *f_args,
                  grad_for_f=False,
                  f_kwargs: dict = None,
                  **f_kwargs_) -> X:
     """
```

### Comparing `phiflow-2.3.3/phi/math/_shape.py` & `phiflow-2.3.4/phi/math/_shape.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         """
         Ordered dimension names as `tuple[str]`.
         
         See Also:
             `Shape.name`.
         """
         self.types: Tuple[str] = types  # undocumented, may be private
-        self.item_names: Tuple[str or 'Shape'] = (None,) * len(sizes) if item_names is None else item_names  # undocumented
+        self.item_names: Tuple[Union[str, 'Shape']] = (None,) * len(sizes) if item_names is None else item_names  # undocumented
         if DEBUG_CHECKS:
             assert len(sizes) == len(names) == len(types) == len(item_names), f"sizes={sizes}, names={names}, types={types}, item_names={item_names}"
             assert len(set(names)) == len(names), f"Duplicate dimension names: {names}"
             assert all(isinstance(n, str) for n in names), f"All names must be of type string but got {names}"
             assert isinstance(self.item_names, tuple)
             assert all([items is None or isinstance(items, tuple) for items in self.item_names])
             assert all([items is None or all([isinstance(n, str) for n in items]) for items in self.item_names])
@@ -124,23 +124,23 @@
             dims = parse_dim_order(item)
             return all(dim in self.names for dim in dims)
         elif isinstance(item, Shape):
             return all([d in self.names for d in item.names])
         else:
             raise ValueError(item)
 
-    def isdisjoint(self, other: 'Shape' or tuple or list or str):
+    def isdisjoint(self, other: Union['Shape', tuple, list, str]):
         """ Shapes are disjoint if all dimension names of one shape do not occur in the other shape. """
         other = parse_dim_order(other)
         return not any(dim in self.names for dim in other)
 
     def __iter__(self):
         return iter(self[i] for i in range(self.rank))
 
-    def index(self, dim: str or 'Shape' or None) -> int:
+    def index(self, dim: Union[str, 'Shape', None]) -> int:
         """
         Finds the index of the dimension within this `Shape`.
 
         See Also:
             `Shape.indices()`.
 
         Args:
@@ -157,15 +157,15 @@
             return self.names.index(dim)
         elif isinstance(dim, Shape):
             assert dim.rank == 1, f"index() requires a single dimension as input but got {dim}. Use indices() for multiple dimensions."
             return self.names.index(dim.name)
         else:
             raise ValueError(f"index() requires a single dimension as input but got {dim}")
 
-    def indices(self, dims: tuple or list or 'Shape') -> Tuple[int]:
+    def indices(self, dims: Union[tuple, list, 'Shape']) -> Tuple[int]:
         """
         Finds the indices of the given dimensions within this `Shape`.
 
         See Also:
             `Shape.index()`.
 
         Args:
@@ -177,15 +177,15 @@
         if isinstance(dims, (list, tuple, set)):
             return tuple([self.index(n) for n in dims])
         elif isinstance(dims, Shape):
             return tuple([self.index(n) for n in dims.names])
         else:
             raise ValueError(f"indices() requires a sequence of dimensions but got {dims}")
 
-    def get_size(self, dim: str or 'Shape' or int, default=None):
+    def get_size(self, dim: Union[str, 'Shape', int], default=None):
         """
         See Also:
             `Shape.get_sizes()`, `Shape.size`
 
         Args:
             dim: Dimension, either as name `str` or single-dimension `Shape` or index `int`.
             default: (Optional) If the dim does not exist, return this value instead of raising an error.
@@ -205,58 +205,58 @@
                     raise KeyError(f"get_size() failed because '{dim}' is not part of Shape {self} and no default value was provided")
                 else:
                     return default
             return self.sizes[self.names.index(dim)]
         else:
             raise ValueError(f"get_size() requires a single dimension but got {dim}. Use indices() to get multiple sizes.")
 
-    def get_sizes(self, dims: tuple or list or 'Shape') -> tuple:
+    def get_sizes(self, dims: Union[tuple, list, 'Shape']) -> tuple:
         """
         See Also:
             `Shape.get_size()`
 
         Args:
             dims: Dimensions as `tuple`, `list` or `Shape`.
 
         Returns:
             `tuple`
         """
         assert isinstance(dims, (tuple, list, Shape)), f"get_sizes() requires a sequence of dimensions but got {dims}"
         return tuple([self.get_size(dim) for dim in dims])
 
-    def get_type(self, dim: str or 'Shape') -> str:
+    def get_type(self, dim: Union[str, 'Shape']) -> str:
         # undocumented, use get_dim_type() instead.
         if isinstance(dim, str):
             return self.types[self.names.index(dim)]
         elif isinstance(dim, Shape):
             assert dim.rank == 1, f"Shape.get_type() only accepts single-dimension Shapes but got {dim}"
             return self.types[self.names.index(dim.name)]
         else:
             raise ValueError(dim)
 
-    def get_dim_type(self, dim: str or 'Shape') -> Callable:
+    def get_dim_type(self, dim: Union[str, 'Shape']) -> Callable:
         """
         Args:
             dim: Dimension, either as name `str` or single-dimension `Shape`.
 
         Returns:
             Dimension type, one of `batch`, `spatial`, `instance`, `channel`.
         """
         return {BATCH_DIM: batch, SPATIAL_DIM: spatial, INSTANCE_DIM: instance, CHANNEL_DIM: channel}[self.get_type(dim)]
 
-    def get_types(self, dims: tuple or list or 'Shape') -> tuple:
+    def get_types(self, dims: Union[tuple, list, 'Shape']) -> tuple:
         # undocumented, do not use
         if isinstance(dims, (tuple, list)):
             return tuple(self.get_type(n) for n in dims)
         elif isinstance(dims, Shape):
             return tuple(self.get_type(n) for n in dims.names)
         else:
             raise ValueError(dims)
 
-    def get_item_names(self, dim: str or 'Shape' or int, fallback_spatial=False) -> tuple or None:
+    def get_item_names(self, dim: Union[str, 'Shape', int], fallback_spatial=False) -> Union[tuple, None]:
         """
         Args:
             fallback_spatial: If `True` and no item names are defined for `dim` and `dim` is a channel dimension, the spatial dimension names are interpreted as item names along `dim` in the order they are listed in this `Shape`.
             dim: Dimension, either as `int` index, `str` name or single-dimension `Shape`.
 
         Returns:
             Item names as `tuple` or `None` if not defined.
@@ -273,15 +273,15 @@
         if result is not None:
             return result
         elif fallback_spatial and self.spatial_rank == self.get_size(dim) and self.get_type(dim) == CHANNEL_DIM:
             return self.spatial.names
         else:
             return None
 
-    def flipped(self, dims: List[str] or Tuple[str]):
+    def flipped(self, dims: Union[List[str], Tuple[str]]):
         item_names = list(self.item_names)
         for dim in dims:
             if dim in self.names:
                 dim_i_n = self.get_item_names(dim)
                 if dim_i_n is not None:
                     item_names[self.index(dim)] = tuple(reversed(dim_i_n))
         return Shape(self.sizes, self.names, self.types, tuple(item_names))
@@ -530,15 +530,15 @@
         assert self.rank == 1, "Shape.type is only defined for shapes of rank 1."
         return self.types[0]
 
     def __int__(self):
         assert self.rank == 1, "int(Shape) is only defined for shapes of rank 1."
         return self.sizes[0]
 
-    def mask(self, names: tuple or list or set or 'Shape'):
+    def mask(self, names: Union[tuple, list, set, 'Shape']):
         """
         Returns a binary sequence corresponding to the names of this Shape.
         A value of 1 means that a dimension of this Shape is contained in `names`.
 
         Args:
           names: instance of dimension
           names: tuple or list or set: 
@@ -586,22 +586,22 @@
 
     def __ne__(self, other):
         return not self == other
 
     def __bool__(self):
         return self.rank > 0
 
-    def _reorder(self, names: tuple or list or 'Shape') -> 'Shape':
+    def _reorder(self, names: Union[tuple, list, 'Shape']) -> 'Shape':
         assert len(names) == self.rank
         if isinstance(names, Shape):
             names = names.names
         order = [self.index(n) for n in names]
         return self[order]
 
-    def _order_group(self, names: tuple or list or 'Shape') -> list:
+    def _order_group(self, names: Union[tuple, list, 'Shape']) -> list:
         """ Reorders the dimensions of this `Shape` so that `names` are clustered together and occur in the specified order. """
         if isinstance(names, Shape):
             names = names.names
         result = []
         for dim in self.names:
             if dim not in result:
                 if dim in names:
@@ -792,15 +792,15 @@
         """
         Returns only the non-uniform dimensions of this shape, i.e. the dimensions whose size varies along another dimension.
         """
         from phi.math import Tensor
         indices = [i for i, size in enumerate(self.sizes) if isinstance(size, Tensor) and size.rank > 0]
         return self[indices]
 
-    def with_size(self, size: int or None):
+    def with_size(self, size: Union[int, None]):
         """
         Only for single-dimension shapes.
         Returns a `Shape` representing this dimension but with a different size.
 
         See Also:
             `Shape.with_sizes()`.
 
@@ -809,15 +809,15 @@
 
         Returns:
             `Shape`
         """
         assert self.rank == 1, "Shape.with_size() is only defined for shapes of rank 1."
         return self.with_sizes([size])
 
-    def with_sizes(self, sizes: tuple or list or 'Shape' or int, keep_item_names=True):
+    def with_sizes(self, sizes: Union[tuple, list, 'Shape', int], keep_item_names=True):
         """
         Returns a new `Shape` matching the dimension names and types of `self` but with different sizes.
 
         See Also:
             `Shape.with_size()`.
 
         Args:
@@ -869,15 +869,15 @@
         return Shape((None,) * self.rank, self.names, self.types, (None,) * self.rank)
 
     def _replace_single_size(self, dim: str, size: int, keep_item_names: bool = False):
         new_sizes = list(self.sizes)
         new_sizes[self.index(dim)] = size
         return self.with_sizes(new_sizes, keep_item_names=keep_item_names)
 
-    def with_dim_size(self, dim: str or 'Shape', size: int or 'math.Tensor' or str or tuple or list, keep_item_names=True):
+    def with_dim_size(self, dim: Union[str, 'Shape'], size: Union[int, 'math.Tensor', str, tuple, list], keep_item_names=True):
         """
         Returns a new `Shape` that has a different size for `dim`.
 
         Args:
             dim: Dimension for which to replace the size, `Shape` or `str`.
             size: New size, `int` or `Tensor`
 
@@ -886,23 +886,23 @@
         """
         if isinstance(dim, Shape):
             dim = dim.name
         assert isinstance(dim, str)
         new_size, new_item_names = Shape._size_and_item_names_from_obj(size, self.get_size(dim), self.get_item_names(dim), keep_item_names)
         return self.replace(dim, Shape((new_size,), (dim,), (self.get_type(dim),), (new_item_names,)))
 
-    def _with_names(self, names: str or tuple or list):
+    def _with_names(self, names: Union[str, tuple, list]):
         if isinstance(names, str):
             names = parse_dim_names(names, self.rank)
             names = [n if n is not None else o for n, o in zip(names, self.names)]
         return Shape(self.sizes, tuple(names), self.types, self.item_names)
 
     def _replace_names_and_types(self,
-                                 dims: 'Shape' or str or tuple or list,
-                                 new: 'Shape' or str or tuple or list) -> 'Shape':
+                                 dims: Union['Shape', str, tuple, list],
+                                 new: Union['Shape', str, tuple, list]) -> 'Shape':
         """
         Returns a copy of `self` with `dims` replaced by `new`.
         Dimensions that are not present in `self` are ignored.
 
         The dimension order is preserved.
 
         Args:
@@ -925,15 +925,15 @@
                     names[self.index(old_name)] = new_dim.name
                     types[self.index(old_name)] = new_dim.type
                     item_names[self.index(old_name)] = new_dim.item_names[0]
                 else:
                     names[self.index(old_name)] = new_dim
         return Shape(tuple(sizes), tuple(names), tuple(types), tuple(item_names))
 
-    def replace(self, dims: 'Shape' or str or tuple or list, new: 'Shape') -> 'Shape':
+    def replace(self, dims: Union['Shape', str, tuple, list], new: 'Shape') -> 'Shape':
         """
         Returns a copy of `self` with `dims` replaced by `new`.
         Dimensions that are not present in `self` are ignored.
 
         The dimension order is preserved.
 
         Args:
@@ -962,15 +962,15 @@
                 sizes[self.index(old_name)] = new_dim.size
         replaced = Shape(tuple(sizes), tuple(names), tuple(types), tuple(item_names))
         if len(new) == len(dims):
             return replaced
         to_remove = dims[-(len(dims) - len(new)):]
         return replaced.without(to_remove)
 
-    def _with_types(self, types: 'Shape' or str):
+    def _with_types(self, types: Union['Shape', str]):
         """
         Only for internal use.
         Note: This method does not rename dimensions to comply with type requirements (e.g. ~ for dual dims).
         """
         if isinstance(types, Shape):
             return Shape(self.sizes, self.names, tuple([types.get_type(name) if name in types else self_type for name, self_type in zip(self.names, self.types)]), self.item_names)
         elif isinstance(types, str):
@@ -992,15 +992,15 @@
         assert len(set(names)) == len(names), f"No duplicates allowed but got {names}"
         assert len(names) >= len(self.names), f"Cannot find permutation for {self} given {names} because names {set(self.names) - set(names)} are missing"
         assert len(names) <= len(self.names), f"Cannot find permutation for {self} given {names} because too many names were passed: {names}"
         perm = [self.names.index(name) for name in names]
         return perm
 
     @property
-    def volume(self) -> int or None:
+    def volume(self) -> Union[int, None]:
         """
         Returns the total number of values contained in a tensor of this shape.
         This is the product of all dimension sizes.
 
         Returns:
             volume as `int` or `Tensor` or `None` if the shape is not `Shape.well_defined`
         """
@@ -1125,15 +1125,15 @@
                     break
             else:
                 return
 
     def first_index(self, names=False):
         return next(iter(self.meshgrid(names=names)))
 
-    def are_adjacent(self, dims: str or tuple or list or set or 'Shape'):
+    def are_adjacent(self, dims: Union[str, tuple, list, set, 'Shape']):
         indices = self.indices(dims)
         return (max(indices) - min(indices)) == len(dims) - 1
 
     def __add__(self, other):
         return self._op2(other, lambda s, o: s + o, 0)
 
     def __radd__(self, other):
@@ -1192,15 +1192,15 @@
     Raised when the shape of a tensor does not match the other arguments.
     """
     def __init__(self, message, *shapes: Shape):
         Exception.__init__(self, message)
         self.shapes = shapes
 
 
-def parse_dim_names(obj: str or tuple or list or Shape, count: int) -> tuple:
+def parse_dim_names(obj: Union[str, tuple, list, Shape], count: int) -> tuple:
     if isinstance(obj, str):
         parts = obj.split(',')
         result = []
         for part in parts:
             part = part.strip()
             if part == '...':
                 result.extend([None] * (count - len(parts) + 1))
@@ -1215,15 +1215,15 @@
         return obj.names
     elif isinstance(obj, (tuple, list)):
         assert len(obj) == count, f"Number of specified names in {obj} does not match number of dimensions ({count})"
         return tuple(obj)
     raise ValueError(obj)
 
 
-def parse_dim_order(order: str or tuple or list or Shape or None, check_rank: int = None) -> tuple or None:
+def parse_dim_order(order: Union[str, tuple, list, Shape, None], check_rank: int = None) -> Union[tuple, None]:
     if order is None:
         if check_rank is not None:
             assert check_rank <= 1, "When calling Tensor.native() or Tensor.numpy(), the dimension order must be specified for Tensors with more than one dimension. The listed default dimension order can vary depending on the chosen backend. Consider using math.reshaped_native(Tensor) instead."
         return None
     elif isinstance(order, Shape):
         return order.names
     if isinstance(order, list):
@@ -1329,15 +1329,15 @@
                 return channel('vector')
             else:
                 raise ValueError(f"Cannot auto-complete shape of {backend} tensor with shape {shape_tuple}. Only 0D and 1D tensors have a Φ-Flow shape by default.")
         except NoBackendFound:
             raise ValueError(f'shape() requires Shaped or Shape argument but got {type(obj)}')
 
 
-def spatial(*args, **dims: int or str or tuple or list or Shape) -> Shape:
+def spatial(*args, **dims: Union[int, str, tuple, list, Shape]) -> Shape:
     """
     Returns the spatial dimensions of an existing `Shape` or creates a new `Shape` with only spatial dimensions.
 
     Usage for filtering spatial dimensions:
     >>> spatial_dims = spatial(shape)
     >>> spatial_dims = spatial(tensor)
 
@@ -1371,15 +1371,15 @@
         return args[0].spatial
     elif len(args) == 1 and isinstance(args[0], Shaped):
         return shape(args[0]).spatial
     else:
         raise AssertionError(f"spatial() must be called either as a selector spatial(Shape) or spatial(Tensor) or as a constructor spatial(*names, **dims). Got *args={args}, **dims={dims}")
 
 
-def channel(*args, **dims: int or str or tuple or list or Shape) -> Shape:
+def channel(*args, **dims: Union[int, str, tuple, list, Shape]) -> Shape:
     """
     Returns the channel dimensions of an existing `Shape` or creates a new `Shape` with only channel dimensions.
 
     Usage for filtering channel dimensions:
     >>> channel_dims = channel(shape)
     >>> channel_dims = channel(tensor)
 
@@ -1413,15 +1413,15 @@
         return args[0].channel
     elif len(args) == 1 and isinstance(args[0], Shaped):
         return shape(args[0]).channel
     else:
         raise AssertionError(f"channel() must be called either as a selector channel(Shape) or channel(Tensor) or as a constructor channel(*names, **dims). Got *args={args}, **dims={dims}")
 
 
-def batch(*args, **dims: int or str or tuple or list or Shape) -> Shape:
+def batch(*args, **dims: Union[int, str, tuple, list, Shape]) -> Shape:
     """
     Returns the batch dimensions of an existing `Shape` or creates a new `Shape` with only batch dimensions.
 
     Usage for filtering batch dimensions:
     >>> batch_dims = batch(shape)
     >>> batch_dims = batch(tensor)
 
@@ -1455,15 +1455,15 @@
         return args[0].batch
     elif len(args) == 1 and isinstance(args[0], Shaped):
         return shape(args[0]).batch
     else:
         raise AssertionError(f"batch() must be called either as a selector batch(Shape) or batch(Tensor) or as a constructor batch(*names, **dims). Got *args={args}, **dims={dims}")
 
 
-def instance(*args, **dims: int or str or tuple or list or Shape) -> Shape:
+def instance(*args, **dims: Union[int, str, tuple, list, Shape]) -> Shape:
     """
     Returns the instance dimensions of an existing `Shape` or creates a new `Shape` with only instance dimensions.
 
     Usage for filtering instance dimensions:
     >>> instance_dims = instance(shape)
     >>> instance_dims = instance(tensor)
 
@@ -1497,15 +1497,15 @@
         return args[0].instance
     elif len(args) == 1 and isinstance(args[0], Shaped):
         return shape(args[0]).instance
     else:
         raise AssertionError(f"instance() must be called either as a selector instance(Shape) or instance(Tensor) or as a constructor instance(*names, **dims). Got *args={args}, **dims={dims}")
 
 
-def dual(*args, **dims: int or str or tuple or list or Shape) -> Shape:
+def dual(*args, **dims: Union[int, str, tuple, list, Shape]) -> Shape:
     """
     Returns the dual dimensions of an existing `Shape` or creates a new `Shape` with only dual dimensions.
 
     Dual dimensions are assigned the prefix `~` to distinguish them from regular dimensions.
     This way, a regular and dual dimension of the same name can exist in one `Shape`.
 
     Dual dimensions represent the input space and are typically only present on matrices or higher-order matrices.
@@ -1548,15 +1548,15 @@
         return args[0].dual
     elif len(args) == 1 and isinstance(args[0], Shaped):
         return shape(args[0]).dual
     else:
         raise AssertionError(f"dual() must be called either as a selector dual(Shape) or dual(Tensor) or as a constructor dual(*names, **dims). Got *args={args}, **dims={dims}")
 
 
-def merge_shapes(*objs: Shape or Any, order=(batch, dual, instance, spatial, channel), allow_varying_sizes=False):
+def merge_shapes(*objs: Union[Shape, Any], order=(batch, dual, instance, spatial, channel), allow_varying_sizes=False):
     """
     Combines `shapes` into a single `Shape`, grouping dimensions by type.
     If dimensions with equal names are present in multiple shapes, their types and sizes must match.
 
     The shorthand `shape1 & shape2` merges shapes with `check_exact=[spatial]`.
 
     See Also:
@@ -1706,15 +1706,15 @@
         return s2 is None
     if isinstance(s1, int):
         return isinstance(s2, int) and s2 == s1
     else:
         return math.close(s1, s2)
 
 
-def concat_shapes(*shapes: Shape or Any) -> Shape:
+def concat_shapes(*shapes: Union[Shape, Any]) -> Shape:
     """
     Creates a `Shape` listing the dimensions of all `shapes` in the given order.
 
     See Also:
         `merge_shapes()`.
 
     Args:
```

### Comparing `phiflow-2.3.3/phi/math/_sparse.py` & `phiflow-2.3.4/phi/math/_sparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import warnings
 from numbers import Number
-from typing import List, Callable, Tuple
+from typing import List, Callable, Tuple, Union
 
 import numpy as np
 import scipy.sparse
 
 from ._shape import Shape, non_batch, merge_shapes, instance, batch, non_instance, shape, channel, spatial, DimFilter, concat_shapes, EMPTY_SHAPE, dual, DUAL_DIM, SPATIAL_DIM
 from ._magic_ops import concat, pack_dims, expand, rename_dims
 from ._tensors import Tensor, TensorStack, CollapsedTensor, NativeTensor, cached, wrap
@@ -55,15 +55,15 @@
     def shape(self) -> Shape:
         return self._shape
 
     @property
     def dtype(self) -> DType:
         return self._values.dtype
 
-    def native(self, order: str or tuple or list or Shape = None):
+    def native(self, order: Union[str, tuple, list, Shape] = None):
         raise RuntimeError("Sparse tensors do not have a native representation. Use math.dense(tensor).native() instead")
 
     @property
     def _is_tracer(self) -> bool:
         return self._indices._is_tracer or self._values._is_tracer
 
     def _with_values(self, new_values: Tensor):
@@ -163,15 +163,15 @@
         entries_dim = instance(self._values).name
         perm = {entries_dim: wrap(scipy_csr.data - 1, instance(entries_dim))}
         values = self._values[perm]  # Change order accordingly
         indices = wrap(scipy_csr.indices, instance(entries_dim))
         pointers = wrap(scipy_csr.indptr, instance('pointers'))
         return CompressedSparseMatrix(indices, pointers, values, u_dims, c_dims, uncompressed_indices=self._indices, uncompressed_indices_perm=perm)
 
-    def __pack_dims__(self, dims: Tuple[str, ...], packed_dim: Shape, pos: int or None, **kwargs) -> 'Tensor':
+    def __pack_dims__(self, dims: Tuple[str, ...], packed_dim: Shape, pos: Union[int, None], **kwargs) -> 'Tensor':
         dims = self._shape.only(dims)
         assert dims in self._dense_shape, f"Can only pack sparse dimensions on SparseCoordinateTensor but got {dims} of which {dims.without(self._dense_shape)} are not sparse"
         assert self._indices.default_backend is NUMPY, "Can only pack NumPy indices as of yet"
         from ._ops import reshaped_native
         idx = self._indices.vector[dims.names]
         idx_packed = np.ravel_multi_index(reshaped_native(idx, [channel, instance]), dims.sizes)
         idx_packed = expand(wrap(idx_packed, instance(self._indices)), channel(vector=packed_dim.name))
@@ -413,18 +413,18 @@
             self._uncompressed_indices = None
             raise NotImplementedError()
         if self._uncompressed_indices_perm is not None:
             self._uncompressed_indices = self._uncompressed_indices[self._uncompressed_indices_perm]
             self._uncompressed_indices_perm = None
         return SparseCoordinateTensor(self._uncompressed_indices, self._values, self._compressed_dims & self._uncompressed_dims, False, False)
 
-    def native(self, order: str or tuple or list or Shape = None):
+    def native(self, order: Union[str, tuple, list, Shape] = None):
         raise RuntimeError("Sparse tensors do not have a native representation. Use math.dense(tensor).native() instead")
 
-    def __pack_dims__(self, dims: Tuple[str, ...], packed_dim: Shape, pos: int or None, **kwargs) -> 'Tensor':
+    def __pack_dims__(self, dims: Tuple[str, ...], packed_dim: Shape, pos: Union[int, None], **kwargs) -> 'Tensor':
         assert all(d in self._shape for d in dims)
         dims = self._shape.only(dims, reorder=True)
         if dims.only(self._compressed_dims).is_empty:  # pack cols
             assert self._uncompressed_dims.are_adjacent(dims), f"Can only compress adjacent dims but got {dims} for matrix {self._shape}"
             uncompressed_dims = self._uncompressed_dims.replace(dims, packed_dim.with_size(dims.volume))
             return CompressedSparseMatrix(self._indices, self._pointers, self._values, uncompressed_dims, self._compressed_dims, self._uncompressed_offset)
         elif dims.only(self._uncompressed_dims).is_empty:   # pack rows
```

### Comparing `phiflow-2.3.3/phi/math/_tensors.py` & `phiflow-2.3.4/phi/math/_tensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import numbers
 import warnings
 from collections import namedtuple
 from contextlib import contextmanager
-from typing import Tuple, Callable, List, TypeVar
+from typing import Tuple, Callable, List, TypeVar, Union
 
 from dataclasses import dataclass
 import numpy
 import numpy as np
 
 from .magic import Shapable
 from ._magic_ops import PhiTreeNodeType, variable_attributes, copy_with, stack, pack_dims, expand
@@ -36,15 +36,15 @@
     To construct a Tensor, use `phi.math.tensor()`, `phi.math.wrap()` or one of the basic tensor creation functions,
     see https://tum-pbs.github.io/PhiFlow/Math.html#tensor-creation .
 
     Tensors are not editable.
     When backed by an editable native tensor, e.g. a `numpy.ndarray`, do not edit the underlying data structure.
     """
 
-    def native(self, order: str or tuple or list or Shape = None):
+    def native(self, order: Union[str, tuple, list, Shape] = None):
         """
         Returns a native tensor object with the dimensions ordered according to `order`.
         
         Transposes the underlying tensor to match the name order and adds singleton dimensions for new dimension names.
         If a dimension of the tensor is not listed in `order`, a `ValueError` is raised.
 
         Args:
@@ -54,15 +54,15 @@
             Native tensor representation, such as PyTorch tensor or NumPy array.
 
         Raises:
             ValueError if the tensor cannot be transposed to match target_shape
         """
         raise NotImplementedError(self.__class__)
 
-    def numpy(self, order: str or tuple or list or Shape = None) -> np.ndarray:
+    def numpy(self, order: Union[str, tuple, list, Shape] = None) -> np.ndarray:
         """
         Converts this tensor to a `numpy.ndarray` with dimensions ordered according to `order`.
         
         *Note*: Using this function breaks the autograd chain. The returned tensor is not differentiable.
         To get a differentiable tensor, use `Tensor.native()` instead.
         
         Transposes the underlying tensor to match the name order and adds singleton dimensions for new dimension names.
@@ -342,15 +342,15 @@
         if self._is_tracer:
             return False
         natives = self._natives()
         natives_available = [choose_backend(native).is_available(native) for native in natives]
         return all(natives_available)
 
     @property
-    def device(self) -> ComputeDevice or None:
+    def device(self) -> Union[ComputeDevice, None]:
         """
         Returns the `ComputeDevice` that this tensor is allocated on.
         The device belongs to this tensor's `default_backend`.
 
         See Also:
             `Tensor.default_backend`.
         """
@@ -426,15 +426,15 @@
         return sliced._getitem(selections) if selections else sliced
 
     def _getitem(self, selection: dict) -> 'Tensor':
         """
         Slice the tensor along specified dimensions.
 
         Args:
-          selection: dim_name: str -> int or slice
+          selection: dim_name: str -> Union[int, slice]
           selection: dict: 
 
         Returns:
 
         """
         raise NotImplementedError()
 
@@ -511,15 +511,15 @@
             if dim == self._stack_dim.name:
                 for udim in unpacked_dims:
                     tensors = [TensorStack(tensors[o::len(tensors)//udim.size], udim) for o in range(len(tensors)//udim.size)]
                 assert len(tensors) == 1
                 return tensors[0]
             raise NotImplementedError
 
-    def __pack_dims__(self, dims: Tuple[str, ...], packed_dim: Shape, pos: int or None, **kwargs) -> 'Tensor':
+    def __pack_dims__(self, dims: Tuple[str, ...], packed_dim: Shape, pos: Union[int, None], **kwargs) -> 'Tensor':
         order = self.shape._order_group(dims)
         if self.shape.is_uniform:
             native = self.native(order)
             if pos is None:
                 pos = min(self.shape.indices(dims))
             new_shape = self.shape.without(dims)._expand(packed_dim.with_sizes([self.shape.only(dims).volume]), pos)
             native = choose_backend(native).reshape(native, new_shape.sizes)
@@ -532,15 +532,15 @@
             assert value._stack_dim.name in dims
             inner_packed = [pack_dims(t, dims, packed_dim) for t in value._tensors]
             return concat_tensor(inner_packed, packed_dim.name)
 
     def __cast__(self, dtype: DType):
         return self._op1(lambda native: choose_backend(native).cast(native, dtype=dtype))
 
-    def dimension(self, name: str or Shape) -> 'TensorDim':
+    def dimension(self, name: Union[str, Shape]) -> 'TensorDim':
         """
         Returns a reference to a specific dimension of this tensor.
         This is equivalent to the syntax `tensor.<name>`.
 
         The dimension need not be part of the `Tensor.shape` in which case its size is 1.
 
         Args:
@@ -826,18 +826,18 @@
         """ Returns a shallow copy of the `Tensor` where the type of this dimension is *channel*. """
         return self._as(CHANNEL_DIM, name)
 
     def as_instance(self, name: str = None):
         """ Returns a shallow copy of the `Tensor` where the type of this dimension is *instance*. """
         return self._as(INSTANCE_DIM, name)
 
-    def as_type(self, dim_type: Callable or str):
+    def as_type(self, dim_type: Union[Callable, str]):
         return self._as(dim_type('d').type if callable(dim_type) else dim_type, None)
 
-    def _as(self, dim_type: str, name: str or None):
+    def _as(self, dim_type: str, name: Union[str, None]):
         if not self.exists:
             return self.tensor
         shape = self.tensor.shape
         new_types = list(shape.types)
         new_types[shape.index(self.name)] = dim_type
         new_names = shape.names
         if name is not None:
@@ -923,20 +923,20 @@
         else:
             return DType(object)
 
     @property
     def default_backend(self):
         return None
 
-    def native(self, order: str or tuple or list or Shape = None):
+    def native(self, order: Union[str, tuple, list, Shape] = None):
         order = parse_dim_order(order)
         assert order is None or order == self._shape.names, "Layout.native() does not allow for changing the dimension order"
         return self._obj
 
-    def numpy(self, order: str or tuple or list or Shape = None) -> np.ndarray:
+    def numpy(self, order: Union[str, tuple, list, Shape] = None) -> np.ndarray:
         native = self.native(order=order)
         return numpy.asarray(native)
 
     def _getitem(self, selection: dict) -> 'Tensor':
         selection_list = [selection.get(dim, None) for dim in self._shape.names]
         native = self._getitem_recursive(self._obj, tuple(selection_list))
         new_shape = self._shape.after_gather(selection)
@@ -1019,15 +1019,15 @@
             obj = [obj] * dim.size
         return Layout(obj, concat_shapes(new_dims, self._shape))
 
     def __replace_dims__(self, dims: Tuple[str, ...], new_dims: Shape, **kwargs) -> 'Tensor':
         new_shape = self._shape.replace(dims, new_dims)
         return Layout(self._obj, new_shape)
 
-    def __pack_dims__(self, dims: Tuple[str, ...], packed_dim: Shape, pos: int or None, **kwargs) -> 'Layout':
+    def __pack_dims__(self, dims: Tuple[str, ...], packed_dim: Shape, pos: Union[int, None], **kwargs) -> 'Layout':
         if dims == self.shape.names:
             native = self._as_list()
             return Layout(native, packed_dim.with_size(len(native)))
         else:
             obj = []
             for i in self._shape.only(dims, reorder=True).meshgrid():
                 obj.append(self[i].native())
@@ -1129,15 +1129,15 @@
         assert isinstance(shape, Shape), f"Expected Shape but got '{type(shape)}'"
         backend = choose_backend(native_tensor)
         # if backend.is_available(native_tensor):
         assert backend.staticshape(native_tensor) == shape.sizes, f"Shape {shape} does not match native tensor with shape {backend.staticshape(native_tensor)}"
         self._native = native_tensor
         self._shape = shape
 
-    def native(self, order: str or tuple or list or Shape = None):
+    def native(self, order: Union[str, tuple, list, Shape] = None):
         order = parse_dim_order(order, check_rank=self.rank)
         if order is None or tuple(order) == self.shape.names:
             if self.dtype.precision in [None, get_precision()]:
                 return self._native
             else:
                 return self.default_backend.cast(self._native, DType(self.dtype.kind, precision=get_precision()))
         # --- Insert missing dims ---
@@ -1294,15 +1294,15 @@
 
     def _simplify(self):
         if self.is_cached:
             return self._cached
         else:
             return self
 
-    def native(self, order: str or tuple or list or Shape = None):
+    def native(self, order: Union[str, tuple, list, Shape] = None):
         if self.is_cached:
             return self._cached.native(order)
         order = parse_dim_order(order, check_rank=self.rank)
         if order is None or tuple(order) == self.shape.names:
             return self._cache().native(order)
         else:
             native = self._inner.native(order=order)
@@ -1435,15 +1435,15 @@
 
     Args:
 
     Returns:
 
     """
 
-    def __init__(self, components: tuple or list, stack_dim: Shape):
+    def __init__(self, components: Union[tuple, list], stack_dim: Shape):
         assert isinstance(stack_dim, Shape) and stack_dim.rank == 1, f"stack_dim must be a single-dimension Shape object but got {type(stack_dim)}"
         # assert len(components) > 1, "Use a CollapsedTensor instead"
         for t in components:
             assert isinstance(t, Tensor)
             assert stack_dim.name not in t.shape, f"Cannot stack along '{stack_dim.name}' because the dimension already exists."
         self._tensors = tuple(components)
         self._stack_dim = stack_dim.with_sizes([len(components)], keep_item_names=True)
@@ -1490,15 +1490,15 @@
     def dtype(self):
         return combine_types(*[t.dtype for t in self._tensors])
 
     @property
     def shape(self):
         return self._shape
 
-    def native(self, order: str or tuple or list or Shape = None):
+    def native(self, order: Union[str, tuple, list, Shape] = None):
         if self._cached is not None:
             return self._cached.native(order=order)
         else:
             order = parse_dim_order(order, check_rank=self.rank)
             # Is only the stack dimension shifted?
             if order is not None and self._shape.without(self._stack_dim).names == tuple(filter(lambda name: name != self._stack_dim.name, order)):
                 inner_order = [dim for dim in order if dim != self._stack_dim.name]
@@ -1556,16 +1556,15 @@
         if self._cached is not None:
             return self._cached.unstack(dimension)
         if dimension == self._stack_dim.name:
             return self._tensors
         else:
             if self.requires_broadcast:
                 unstacked = [t.unstack(dimension) for t in self._tensors]
-                result = [TensorStack(items, self._stack_dim) for items in zip(*unstacked)]
-                return result
+                return tuple([TensorStack(items, self._stack_dim) for items in zip(*unstacked)])
             else:
                 return self._cache().unstack(dimension=dimension)
 
     def _op1(self, native_function):
         if self.requires_broadcast:
             tensors = [t._op1(native_function) for t in self._tensors]
             return TensorStack(tensors, self._stack_dim)
@@ -1625,15 +1624,15 @@
     def _simplify(self):
         if self.is_cached:
             return self._cached
         else:
             return self
 
 
-def tensor(data: Tensor or Shape or tuple or list or numbers.Number,
+def tensor(data: Union[Tensor, Shape, tuple, list, numbers.Number],
            *shape: Shape,
            convert: bool = True,
            default_list_dim=channel('vector')) -> Tensor:  # TODO assume convert_unsupported, add convert_external=False for constants
     """
     Create a Tensor from the specified `data`.
     If `convert=True`, converts `data` to the preferred format of the default backend.
 
@@ -1752,15 +1751,15 @@
         if convert:
             data = convert_(data, use_dlpack=False)
         return NativeTensor(data, shape)
     except NoBackendFound:
         raise ValueError(f"{type(data)} is not supported. Only (Tensor, tuple, list, np.ndarray, native tensors) are allowed.\nCurrent backends: {BACKENDS}")
 
 
-def wrap(data: Tensor or Shape or tuple or list or numbers.Number,
+def wrap(data: Union[Tensor, Shape, tuple, list, numbers.Number],
          *shape: Shape) -> Tensor:
     """ Short for `phi.math.tensor()` with `convert=False`. """
     return tensor(data, *shape, convert=False)  # TODO inline, simplify
 
 
 def layout(objects, *shape: Shape) -> Tensor:
     """
@@ -1881,15 +1880,15 @@
 
 def op2_native(x: Tensor, y: Tensor, native_function: Callable):
     new_shape, (native1, native2) = broadcastable_native_tensors(x, y)
     result_tensor = native_function(native1, native2)
     return NativeTensor(result_tensor, new_shape)
 
 
-def custom_op2(x: Tensor or float, y: Tensor or float, l_operator, l_native_function, r_operator=None, r_native_function=None, op_name: str = 'unknown', op_symbol: str = None) -> Tensor:
+def custom_op2(x: Union[Tensor, float], y: Union[Tensor, float], l_operator, l_native_function, r_operator=None, r_native_function=None, op_name: str = 'unknown', op_symbol: str = None) -> Tensor:
     """
     Perform a custom operator on two tensors.
     This method first tries calling _op2() on the first tensor and if that fails, tries it on the second tensor.
 
     Args:
       x: Left argument
       y: Right argument
@@ -1915,15 +1914,15 @@
             r_native_function = lambda a, b: l_native_function(b, a)
         result = y._op2(x, r_operator, r_native_function, f'r{op_name}', op_symbol)
         if result is NotImplemented:
             raise NotImplementedError(f"Operation not supported between {type(x)} and {type(y)}")
     return result
 
 
-def disassemble_tensors(tensors: Tuple[Tensor, ...] or List[Tensor], expand: bool) -> Tuple[tuple, Tuple[Shape], tuple]:
+def disassemble_tensors(tensors: Union[Tuple[Tensor, ...], List[Tensor]], expand: bool) -> Tuple[tuple, Tuple[Shape], tuple]:
     """
     Args:
         tensors: Tuple or list of Tensors.
         expand: Whether to add collapsed dimensions to the native tensors.
 
     Returns:
         natives: tuple of native tensors
@@ -1935,15 +1934,15 @@
             t._expand()
     natives = sum([t._natives() for t in tensors], ())
     shapes = tuple([t.shape for t in tensors])
     specs = tuple([t._spec_dict() for t in tensors])
     return natives, shapes, specs
 
 
-def assemble_tensors(natives: tuple or list, specs: Tuple[dict, ...] or List[dict]):
+def assemble_tensors(natives: Union[tuple, list], specs: Union[Tuple[dict, ...], List[dict]]):
     natives = list(natives)
     result = []
     for spec in specs:
         t = spec['type']._from_spec_and_natives(spec, natives)
         result.append(t)
     return result
 
@@ -2029,15 +2028,15 @@
         attributes = variable_attributes(obj)
         values = {a: assemble_tree(getattr(obj, a), values) for a in attributes}
         return copy_with(obj, **values)
     else:
         return obj
 
 
-def cached(t: Tensor or 'PhiTreeNode') -> Tensor or 'PhiTreeNode':
+def cached(t: Union[Tensor, 'PhiTreeNode']) -> Union[Tensor, 'PhiTreeNode']:
     assert isinstance(t, (Tensor, PhiTreeNode)), f"All arguments must be Tensors but got {type(t)}"
     if isinstance(t, NativeTensor):
         return t
     elif isinstance(t, CollapsedTensor):
         if t.is_cached:
             return t._cached
         if t._inner._is_tracer:
@@ -2237,15 +2236,15 @@
 
     # --- overridden methods ---
 
     def copy(self):
         return Dict(self)
 
 
-def to_dict(value: Tensor or Shape):
+def to_dict(value: Union[Tensor, Shape]):
     """
     Returns a serializable form of a `Tensor` or `Shape`.
     The result can be written to a JSON file, for example.
 
     See Also:
         `from_dict()`.
```

### Comparing `phiflow-2.3.3/phi/math/_trace.py` & `phiflow-2.3.4/phi/math/_trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import namedtuple
-from typing import Callable, Dict, Set, Tuple
+from typing import Callable, Dict, Set, Tuple, Union
 
 import numpy
 import numpy as np
 
 from .backend import choose_backend, NUMPY, Backend
 from ._shape import Shape, parse_dim_order, merge_shapes, spatial, instance, batch, concat_shapes, EMPTY_SHAPE, dual, channel, non_batch
 from ._magic_ops import stack, expand
@@ -42,15 +42,15 @@
             assert shift_.only(sorted(shift_.names), reorder=True) == shift_
         self.bias = bias
         self._shape = shape
 
     def __repr__(self):
         return f"Linear tracer {self._shape}"
 
-    def native(self, order: str or tuple or list or Shape = None):
+    def native(self, order: Union[str, tuple, list, Shape] = None):
         """
         Evaluates the value of the linear operation applied to the original source tensor.
 
         This is done by building a sparse matrix for all dimensions that are affected by the linear operation.
         These dimensions are detected automatically during the creation of the linear operation.
         All other dimensions (independent dimensions) are combined into a single batch dimensions for the sparse matrix multiplication.
```

### Comparing `phiflow-2.3.3/phi/math/backend/__init__.py` & `phiflow-2.3.4/phi/math/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/math/backend/_backend.py` & `phiflow-2.3.4/phi/math/backend/_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import warnings
 from collections import namedtuple
 from contextlib import contextmanager
-from typing import List, Callable, TypeVar, Tuple, Any
+from typing import List, Callable, TypeVar, Tuple, Any, Union
 
 import logging
 import numpy
 
 from ._dtype import DType, combine_types, to_numpy_dtype
 
 
@@ -79,15 +79,15 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         _DEFAULT.pop(-1)
 
     @property
     def name(self) -> str:
         return self._name
 
-    def supports(self, feature: str or Callable) -> bool:
+    def supports(self, feature: Union[str, Callable]) -> bool:
         """
         Tests if this backend supports the given feature.
         Features correspond to a method of this backend that must be implemented if the feature is supported.
 
         Possible features:
 
         * `sparse_coo_tensor`
@@ -159,15 +159,15 @@
 
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return self.name
 
-    def list_devices(self, device_type: str or None = None) -> List[ComputeDevice]:
+    def list_devices(self, device_type: Union[str, None] = None) -> List[ComputeDevice]:
         """
         Fetches information about all available compute devices this backend can use.
 
         Implementations:
 
         * NumPy: [`os.cpu_count`](https://docs.python.org/3/library/os.html#os.cpu_count)
         * PyTorch: [`torch.cuda.get_device_properties`](https://pytorch.org/docs/stable/cuda.html#torch.cuda.get_device_properties)
@@ -188,15 +188,15 @@
         else:
             assert device_type in ('CPU', 'GPU', 'TPU'), "Device"
             return [d for d in self._devices if d.device_type == device_type]
 
     def get_default_device(self) -> ComputeDevice:
         return self._default_device
 
-    def set_default_device(self, device: ComputeDevice or str) -> bool:
+    def set_default_device(self, device: Union[ComputeDevice, str]) -> bool:
         """
         Sets the device new tensors will be allocated on.
         This function will do nothing if the target device type is not available.
 
         See Also:
             `Backend.list_devices()`, `Backend.get_default_device()`.
 
@@ -355,30 +355,30 @@
 
     def block_until_ready(self, values):
         pass
 
     def jit_compile(self, f: Callable) -> Callable:
         return NotImplemented
 
-    def jacobian(self, f: Callable, wrt: tuple or list, get_output: bool, is_f_scalar: bool):
+    def jacobian(self, f: Callable, wrt: Union[tuple, list], get_output: bool, is_f_scalar: bool):
         """
         Args:
             f: Function to differentiate. Returns a tuple containing `(reduced_loss, output)`
             wrt: Argument indices for which to compute the gradient.
             get_output: Whether the derivative function should return the output of `f` in addition to the gradient.
             is_f_scalar: Whether `f` is guaranteed to return a scalar output.
 
         Returns:
             A function `g` with the same arguments as `f`.
             If `get_output=True`, `g` returns a `tuple`containing the outputs of `f` followed by the gradients.
             The gradients retain the dimensions of `reduced_loss` in order as outer (first) dimensions.
         """
         raise NotImplementedError(self)
 
-    def hessian(self, f: Callable, wrt: tuple or list, get_output: bool, get_gradient: bool) -> tuple:
+    def hessian(self, f: Callable, wrt: Union[tuple, list], get_output: bool, get_gradient: bool) -> tuple:
         """
         First dimension of all inputs/outputs of `f` is assumed to be a batch dimension.
         Element-wise Hessians will be computed along the batch dimension.
         All other dimensions are parameter dimensions and will appear twice in the Hessian matrices.
 
         Args:
             f: Function whose first output is a scalar float or complex value.
@@ -401,36 +401,36 @@
             gradient: Function for backprop. Will be called as `gradient(*d_out)` to compute the gradient of `f`.
 
         Returns:
             Function with similar signature and return values as `f`. However, the returned function does not support keyword arguments.
         """
         return NotImplemented
 
-    def jit_compile_grad(self, f: Callable, wrt: tuple or list, get_output: bool, is_f_scalar: bool):
+    def jit_compile_grad(self, f: Callable, wrt: Union[tuple, list], get_output: bool, is_f_scalar: bool):
         raise NotImplementedError()
 
-    def jit_compile_hessian(self, f: Callable, wrt: tuple or list, get_output: bool, get_gradient: bool):
+    def jit_compile_hessian(self, f: Callable, wrt: Union[tuple, list], get_output: bool, get_gradient: bool):
         raise NotImplementedError()
 
     def transpose(self, tensor, axes):
         """ Transposes the dimensions of `tensor` given the new axes order. The tensor will be cast to the default precision in the process. """
         raise NotImplementedError()
 
-    def random_uniform(self, shape, low, high, dtype: DType or None):
+    def random_uniform(self, shape, low, high, dtype: Union[DType, None]):
         """ Float tensor of selected precision containing random values in the range [0, 1) """
         raise NotImplementedError(self)
 
     def random_normal(self, shape, dtype: DType):
         """ Float tensor of selected precision containing random values sampled from a normal distribution with mean 0 and std 1. """
         raise NotImplementedError(self)
 
     def stack(self, values, axis=0):
         raise NotImplementedError(self)
 
-    def stack_leaves(self, trees: tuple or list, axis=0):
+    def stack_leaves(self, trees: Union[tuple, list], axis=0):
         tree0 = trees[0]
         if isinstance(tree0, tuple):
             return tuple([self.stack_leaves([tree[i] for tree in trees], axis=axis) for i in range(len(tree0))])
         elif isinstance(tree0, list):
             return [self.stack_leaves([tree[i] for tree in trees], axis=axis) for i in range(len(tree0))]
         elif isinstance(tree0, dict):
             return {k: self.stack_leaves([tree[k] for tree in trees], axis=axis) for k in tree0}
@@ -458,15 +458,15 @@
 
         """
         raise NotImplementedError(self)
 
     def reshape(self, value, shape):
         raise NotImplementedError(self)
 
-    def flip(self, value, axes: tuple or list):
+    def flip(self, value, axes: Union[tuple, list]):
         slices = tuple(slice(None, None, -1 if i in axes else None) for i in range(self.ndims(value)))
         return value[slices]
 
     def sum(self, value, axis=None, keepdims=False):
         raise NotImplementedError(self)
 
     def prod(self, value, axis=None):
@@ -509,28 +509,28 @@
 
     def meshgrid(self, *coordinates):
         raise NotImplementedError(self)
 
     def linspace(self, start, stop, number):
         raise NotImplementedError(self)
 
-    def tensordot(self, a, a_axes: tuple or list, b, b_axes: tuple or list):
+    def tensordot(self, a, a_axes: Union[tuple, list], b, b_axes: Union[tuple, list]):
         """ Multiply-sum-reduce a_axes of a with b_axes of b. """
         raise NotImplementedError(self)
 
     def mul_matrix_batched_vector(self, A, b):
         raise NotImplementedError(self)
 
     def einsum(self, equation, *tensors):
         raise NotImplementedError(self)
 
     def cumsum(self, x, axis: int):
         raise NotImplementedError(self)
 
-    def while_loop(self, loop: Callable, values: tuple, max_iter: int or Tuple[int, ...] or List[int]):
+    def while_loop(self, loop: Callable, values: tuple, max_iter: Union[int, Tuple[int, ...], List[int]]):
         """
         If `max_iter is None`, runs
 
         ```python
         while any(values[0]):
             values = loop(*values)
         return values
@@ -762,28 +762,28 @@
             quantiles: List or 1D tensor of quantiles to compute.
 
         Returns:
             Tensor with shape (quantiles, *x.shape[:-1])
         """
         raise NotImplementedError(self)
 
-    def fft(self, x, axes: tuple or list):
+    def fft(self, x, axes: Union[tuple, list]):
         """
         Computes the n-dimensional FFT along all but the first and last dimensions.
 
         Args:
           x: tensor of dimension 3 or higher
           axes: Along which axes to perform the FFT
 
         Returns:
             Complex tensor `k`
         """
         raise NotImplementedError(self)
 
-    def ifft(self, k, axes: tuple or list):
+    def ifft(self, k, axes: Union[tuple, list]):
         """
         Computes the n-dimensional inverse FFT along all but the first and last dimensions.
 
         Args:
           k: tensor of dimension 3 or higher
           axes: Along which axes to perform the inverse FFT
 
@@ -904,15 +904,15 @@
             axis: Axis along which to sum
 
         Returns:
             Tensor with `len(indices)` elements along `axis`. (batch, ..., indices, ...)
         """
         raise NotImplementedError(self)
 
-    def sparse_coo_tensor(self, indices: tuple or list, values, shape: tuple):
+    def sparse_coo_tensor(self, indices: Union[tuple, list], values, shape: tuple):
         """
         Create a sparse matrix in coordinate list (COO) format.
 
         Optional feature.
 
         See Also:
             `Backend.csr_matrix()`, `Backend.csc_matrix()`.
@@ -923,15 +923,15 @@
             shape: Shape of the sparse matrix
 
         Returns:
             Native representation of the sparse matrix
         """
         raise NotImplementedError(self)
 
-    def sparse_coo_tensor_batched(self, indices: tuple or list, values, shape: tuple):
+    def sparse_coo_tensor_batched(self, indices: Union[tuple, list], values, shape: tuple):
         """
         Args:
             indices: shape (batch_size, dims, nnz)
             values: Values tensor matching `indices`, shape (batch_size, nnz)
             shape: tuple of two ints representing the dense shape, (dims...)
         """
         raise NotImplementedError(self)
@@ -1410,15 +1410,15 @@
 
     Returns:
         current default `Backend`
     """
     return _DEFAULT[-1]
 
 
-def context_backend() -> Backend or None:
+def context_backend() -> Union[Backend, None]:
     """
     Returns the backend set by the inner-most surrounding `with backend:` block.
     If called outside a backend context, returns `None`.
 
     Returns:
         `Backend` or `None`
     """
```

### Comparing `phiflow-2.3.3/phi/math/backend/_dtype.py` & `phiflow-2.3.4/phi/math/backend/_dtype.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Union
+
 import numpy as np
 import sys
 
 
 class DType:
     """
     Instances of `DType` represent the kind and size of data elements.
@@ -73,15 +75,15 @@
     def __hash__(self):
         return hash(self.kind) + hash(self.bits)
 
     def __repr__(self):
         return f"{self.kind.__name__}{self.bits}"
 
     @staticmethod
-    def as_dtype(value: 'DType' or tuple or type or None) -> 'DType' or None:
+    def as_dtype(value: Union['DType', tuple, type, None]) -> Union['DType', None]:
         if isinstance(value, DType):
             return value
         elif value is int:
             return DType(int, 32)
         elif value is float:
             from phi.math import get_precision
             return DType(float, get_precision())
```

### Comparing `phiflow-2.3.3/phi/math/backend/_linalg.py` & `phiflow-2.3.4/phi/math/backend/_linalg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from functools import partial
-from typing import Tuple, Callable
+from typing import Tuple, Callable, Union
 
 import numpy as np
 
 from ._backend import Backend, SolveResult, List, DType, spatial_derivative_evaluation
 
 
 def identity(x):
     return x
 
 
-def stop_on_l2(b: Backend, tolerance_squared, max_iter: np.ndarray, on_diverged: Exception or None = None):
+def stop_on_l2(b: Backend, tolerance_squared, max_iter: np.ndarray, on_diverged: Union[Exception, None] = None):
     max_iter = b.as_tensor(max_iter[-1, :])
     rsq0 = []
     def check_progress(iterations, residual_squared):
         converged = b.all(residual_squared <= tolerance_squared, axis=(1,))
         if not rsq0:
             diverged = b.any(~b.isfinite(residual_squared), axis=(1,))
             rsq0.append(residual_squared)
@@ -23,24 +23,24 @@
         continue_ = ~converged & ~diverged & (iterations < max_iter)
         if on_diverged is not None and b.any(diverged):
             on_diverged(iterations)
         return continue_, converged, diverged
     return check_progress
 
 
-def _max_iter(max_iter: np.ndarray) -> int or list:
+def _max_iter(max_iter: np.ndarray) -> Union[int, list]:
     trj_size, batch_size = max_iter.shape
     if trj_size == 1:
         return int(np.max(max_iter))
     else:
         assert np.all(max_iter == max_iter[:, :1]), "When recording a trajectory, max_iter must be equal for all batch entries"
         return max_iter[:, 0].tolist()
 
 
-def cg(b: Backend, lin, y, x0, check_progress: Callable, max_iter, pre: Callable = identity) -> SolveResult or List[SolveResult]:
+def cg(b: Backend, lin, y, x0, check_progress: Callable, max_iter, pre: Callable = identity) -> Union[SolveResult, List[SolveResult]]:
     """
     Based on "An Introduction to the Conjugate Gradient Method Without the Agonizing Pain" by Jonathan Richard Shewchuk
     symbols: dx=d, dy=q, step_size=alpha, residual_squared=delta, residual=r, y=b, pre=M
     """
     batch_size = b.staticshape(y)[0]
     y = b.to_float(y)
     x = b.copy(b.to_float(x0), only_mutable=True)
@@ -68,15 +68,15 @@
         continue_, converged, diverged = check_progress(iterations, residual_squared)
         return continue_, x, dx, residual_squared, residual, iterations, function_evaluations, converged, diverged
 
     _, x, _, _, residual, iterations, function_evaluations, converged, diverged = b.while_loop(cg_loop_body, (continue_, x, dx, residual_squared, residual, iterations, function_evaluations, converged, diverged), _max_iter(max_iter))
     return SolveResult(f"Φ-Flow CG ({b.name})", x, residual, iterations, function_evaluations, converged, diverged, [""] * batch_size)
 
 
-def cg_adaptive(b, lin, y, x0, check_progress: Callable, max_iter) -> SolveResult or List[SolveResult]:
+def cg_adaptive(b, lin, y, x0, check_progress: Callable, max_iter) -> Union[SolveResult, List[SolveResult]]:
     """
     Based on the variant described in "Methods of Conjugate Gradients for Solving Linear Systems" by Magnus R. Hestenes and Eduard Stiefel https://nvlpubs.nist.gov/nistpubs/jres/049/jresv49n6p409_A1b.pdf
     """
     y = b.to_float(y)
     x0 = b.copy(b.to_float(x0), only_mutable=True)
     batch_size = b.staticshape(y)[0]
     x = x0
@@ -102,15 +102,15 @@
         continue_, converged, diverged = check_progress(iterations, residual_squared)
         return continue_, x, dx, dy, residual, iterations, function_evaluations, converged, diverged
 
     _, x, _, _, residual, iterations, function_evaluations, converged, diverged = b.while_loop(acg_loop_body, (continue_, x, dx, dy, residual, iterations, function_evaluations, converged, diverged), _max_iter(max_iter))
     return SolveResult(f"Φ-Flow CG-adaptive ({b.name})", x, residual, iterations, function_evaluations, converged, diverged, [""] * batch_size)
 
 
-def bicg(b: Backend, lin, y, x0, check_progress: Callable, max_iter, poly_order: int) -> SolveResult or List[SolveResult]:
+def bicg(b: Backend, lin, y, x0, check_progress: Callable, max_iter, poly_order: int) -> Union[SolveResult, List[SolveResult]]:
     """ Adapted from [BiCGstab for linear equations involving unsymmetric matrices with complex spectrum](https://dspace.library.uu.nl/bitstream/handle/1874/16827/sleijpen_93_bicgstab.pdf) """
     # Based on "BiCGstab(L) for linear equations involving unsymmetric matrices with complex spectrum" by Gerard L.G. Sleijpen
     y = b.to_float(y)
     x = b.copy(b.to_float(x0), only_mutable=True)
     batch_size = b.staticshape(y)[0]
     r0_tild = residual = y - b.linear(lin, x)
     iterations = b.zeros([batch_size], DType(int, 32))
```

### Comparing `phiflow-2.3.3/phi/math/backend/_minimize.py` & `phiflow-2.3.4/phi/math/backend/_minimize.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/math/backend/_numpy_backend.py` & `phiflow-2.3.4/phi/math/backend/_numpy_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numbers
 import os
 import sys
-from typing import List, Any, Callable
+from typing import List, Any, Callable, Union
 
 import numpy as np
 import numpy.random
 import scipy.signal
 import scipy.sparse
 from scipy.sparse import issparse
 from scipy.sparse.linalg import cg, spsolve
@@ -135,15 +135,15 @@
         return np.equal(x, y)
 
     def divide_no_nan(self, x, y):
         with np.errstate(divide='ignore', invalid='ignore'):
             result = x / y
         return np.where(y == 0, 0, result)
 
-    def random_uniform(self, shape, low, high, dtype: DType or None):
+    def random_uniform(self, shape, low, high, dtype: Union[DType, None]):
         dtype = dtype or self.float_type
         if dtype.kind == float:
             return np.random.uniform(low, high, shape).astype(to_numpy_dtype(dtype))
         elif dtype.kind == complex:
             return (np.random.uniform(low.real, high.real, shape) + 1j * np.random.uniform(low.imag, high.imag, shape)).astype(to_numpy_dtype(dtype))
         elif dtype.kind == int:
             return numpy.random.randint(low, high, shape, dtype=to_numpy_dtype(dtype))
@@ -195,15 +195,15 @@
 
     def linspace(self, start, stop, number):
         return np.linspace(start, stop, number, dtype=to_numpy_dtype(self.float_type))
 
     def mean(self, value, axis=None, keepdims=False):
         return np.mean(value, axis, keepdims=keepdims)
 
-    def tensordot(self, a, a_axes: tuple or list, b, b_axes: tuple or list):
+    def tensordot(self, a, a_axes: Union[tuple, list], b, b_axes: Union[tuple, list]):
         return np.tensordot(a, b, (a_axes, b_axes))
 
     def mul(self, a, b):
         if scipy.sparse.issparse(a):
             return a.multiply(b)
         elif scipy.sparse.issparse(b):
             return b.multiply(a)
@@ -305,26 +305,26 @@
         #     count = np.maximum(1, count)
         #     return array / count
         return result
 
     def quantile(self, x, quantiles):
         return np.quantile(x, quantiles, axis=-1)
 
-    def fft(self, x, axes: tuple or list):
+    def fft(self, x, axes: Union[tuple, list]):
         x = self.to_complex(x)
         if not axes:
             return x
         if len(axes) == 1:
             return np.fft.fft(x, axis=axes[0]).astype(x.dtype)
         elif len(axes) == 2:
             return np.fft.fft2(x, axes=axes).astype(x.dtype)
         else:
             return np.fft.fftn(x, axes=axes).astype(x.dtype)
 
-    def ifft(self, k, axes: tuple or list):
+    def ifft(self, k, axes: Union[tuple, list]):
         if not axes:
             return k
         if len(axes) == 1:
             return np.fft.ifft(k, axis=axes[0]).astype(k.dtype)
         elif len(axes) == 2:
             return np.fft.ifft2(k, axes=axes).astype(k.dtype)
         else:
@@ -367,15 +367,15 @@
 
     def csc_matrix(self, column_pointers, row_indices, values, shape: tuple):
         return scipy.sparse.csc_matrix((values, row_indices, column_pointers), shape=shape)
 
     def stop_gradient(self, value):
         return value
 
-    # def jacobian(self, f, wrt: tuple or list, get_output: bool):
+    # def jacobian(self, f, wrt: Union[tuple, list], get_output: bool):
     #     warnings.warn("NumPy does not support analytic gradients and will use differences instead. This may be slow!", RuntimeWarning)
     #     eps = {64: 1e-9, 32: 1e-4, 16: 1e-1}[self.precision]
     #
     #     def gradient(*args, **kwargs):
     #         output = f(*args, **kwargs)
     #         loss = output[0] if isinstance(output, (tuple, list)) else output
     #         grads = []
```

### Comparing `phiflow-2.3.3/phi/math/backend/_profile.py` & `phiflow-2.3.4/phi/math/backend/_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import json
 from contextlib import contextmanager
 from time import perf_counter
-from typing import Optional, Callable
+from typing import Optional, Callable, Union
 
 from ._backend import Backend, BACKENDS, _DEFAULT
 
 
 class BackendCall:
 
     def __init__(self, start: float, stop: float, backend: 'ProfilingBackend', function_name):
@@ -54,19 +54,19 @@
         self._args[key] = value
 
 
 class ExtCall:
     """ Function invocation that is not a Backend method but internally calls Backend methods. """
 
     def __init__(self,
-                 parent: 'ExtCall' or None,
+                 parent: Union['ExtCall', None],
                  name: str,
                  level: int,
                  function: str,
-                 code_context: list or None,
+                 code_context: Union[list, None],
                  file_name: str,
                  line_number: int):
         """
         Args:
             parent: Parent call.
             name: Name of this call, see `ExtCall.determine_name()`.
             level: Number of parent stack items including this one.
@@ -228,15 +228,15 @@
     Stores information about calls to backends and their timing.
 
     Profile may be created through `profile()` or `profile_function()`.
 
     Profiles can be printed or saved to disc.
     """
 
-    def __init__(self, trace: bool, backends: tuple or list, subtract_trace_time: bool):
+    def __init__(self, trace: bool, backends: Union[tuple, list], subtract_trace_time: bool):
         self._start = perf_counter()
         self._stop = None
         self._root = ExtCall(None, "", 0, "", "", "", -1)
         self._last_ext_call = self._root
         self._messages = []
         self._trace = trace
         self._backend_calls = []
@@ -465,15 +465,15 @@
         return hash(self._backend)
 
 
 _PROFILE = []
 
 
 @contextmanager
-def profile(backends=None, trace=True, subtract_trace_time=True, save: str or None = None) -> Profile:
+def profile(backends=None, trace=True, subtract_trace_time=True, save: Union[str, None] = None) -> Profile:
     """
     To be used in `with` statements, `with math.backend.profile() as prof: ...`.
     Creates a `Profile` for the code executed within the context by tracking calls to the `backends` and optionally tracing the call.
 
     Args:
         backends: List of backends to profile, `None` to profile all.
         trace: Whether to perform a full stack trace for each backend call. If true, groups backend calls by function.
@@ -491,16 +491,16 @@
     finally:
         _stop_profiling(prof, *restore_data)
         if save is not None:
             prof.save(save)
 
 
 def profile_function(fun: Callable,
-                     args: tuple or list = (),
-                     kwargs: dict or None = None,
+                     args: Union[tuple, list] = (),
+                     kwargs: Union[dict, None] = None,
                      backends=None,
                      trace=True,
                      subtract_trace_time=True,
                      retime=True,
                      warmup=1,
                      call_count=1) -> Profile:
     """
@@ -534,15 +534,15 @@
     if call_count > 1:
         with prof._accumulate_average(call_count):
             for _ in range(call_count - 1):
                 fun(*args, **kwargs)
     return prof
 
 
-def _start_profiling(prof: Profile, backends: tuple or list):
+def _start_profiling(prof: Profile, backends: Union[tuple, list]):
     _PROFILE.append(prof)
     original_default = _DEFAULT[-1]
     original_backends = tuple(BACKENDS)
     for i, backend in enumerate(backends):
         prof_backend = ProfilingBackend(prof, backend, i)
         BACKENDS[BACKENDS.index(backend)] = prof_backend
         if _DEFAULT[-1] == backend:
```

### Comparing `phiflow-2.3.3/phi/math/extrapolation.py` & `phiflow-2.3.4/phi/math/extrapolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
 
 class ConstantExtrapolation(Extrapolation):
     """
     Extrapolate with a constant value.
     """
 
-    def __init__(self, value: Tensor or float):
+    def __init__(self, value: Union[Tensor, float]):
         Extrapolation.__init__(self, 5)
         self.value = wrap(value)
         """ Extrapolation value """
         assert self.value.dtype.kind in (bool, int, float, complex), f"Numeric value required for constant extrapolation but got '{value}'"
 
     @property
     def shape(self):
@@ -1053,15 +1053,15 @@
             return combine_by_direction(normal=normal, tangential=tangential)
         else:
             ext = {dim: (as_extrapolation(spec[0]), as_extrapolation(spec[1])) if isinstance(spec, tuple) else as_extrapolation(spec) for dim, spec in obj.items()}
             return combine_sides(**ext)
     return ConstantExtrapolation(obj)
 
 
-def combine_sides(**extrapolations: Extrapolation or tuple) -> Extrapolation:
+def combine_sides(**extrapolations: Union[Extrapolation, tuple]) -> Extrapolation:
     """
     Specify extrapolations for each side / face of a box.
 
     Args:
         **extrapolations: map from dim: str -> `Extrapolation` or `tuple` (lower, upper)
 
     Returns:
@@ -1338,15 +1338,15 @@
     def __abs__(self):
         return combine_by_direction(normal=abs(self.normal), tangential=abs(self.tangential))
 
     def __neg__(self):
         return combine_by_direction(normal=-self.normal, tangential=-self.tangential)
 
 
-def combine_by_direction(normal: Extrapolation or float or Tensor, tangential: Extrapolation or float or Tensor) -> Extrapolation:
+def combine_by_direction(normal: Union[Extrapolation, float, Tensor], tangential: Union[Extrapolation, float, Tensor]) -> Extrapolation:
     """
     Use a different extrapolation for the normal component of vector-valued tensors.
 
     Args:
         normal: Extrapolation for the component that is orthogonal to the boundary.
         tangential: Extrapolation for the component that is tangential to the boundary.
 
@@ -1386,15 +1386,15 @@
     elif etype == 'undefined':
         derived_from = from_dict(dictionary['derived_from'])
         return Undefined(derived_from)
     else:
         raise ValueError(dictionary)
 
 
-def order_by_shape(shape: Shape, sequence, default=None) -> tuple or list:
+def order_by_shape(shape: Shape, sequence, default=None) -> Union[tuple, list]:
     """
     If sequence is a dict with dimension names as keys, orders its values according to this shape.
 
     Otherwise, the sequence is returned unchanged.
 
     Args:
       sequence: Sequence or dict to be ordered
```

### Comparing `phiflow-2.3.3/phi/math/magic.py` & `phiflow-2.3.4/phi/math/magic.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 An object implements one of the types defined here by implementing one or more of the related magic methods.
 Instance checks can be performed via `isinstance(obj, <MagicClass>)`.
 
 This is analogous to interfaces defined in the built-in `collections` package, such as `Sized, Iterable, Hashable, Callable`.
 To check whether `len(obj)` can be performed, you check `isinstance(obj, Sized)`.
 """
 import warnings
-from typing import Tuple, Callable
+from typing import Tuple, Callable, Union
 
 import dataclasses
 
 from ._shape import Shape, shape, channel, non_batch, batch, spatial, instance, concat_shapes, dual
 from .backend._dtype import DType
 
 
@@ -238,15 +238,15 @@
                 Adding batch dimensions must always work without keyword arguments.
 
         Returns:
             New instance of `Shapable` or `NotImplemented` to revert to default behavior for this object.
         """
         raise NotImplementedError
 
-    def __pack_dims__(self, dims: Tuple[str, ...], packed_dim: Shape, pos: int or None, **kwargs) -> 'Shapable':
+    def __pack_dims__(self, dims: Tuple[str, ...], packed_dim: Shape, pos: Union[int, None], **kwargs) -> 'Shapable':
         """
         Compresses multiple dimensions into a single dimension by concatenating the elements.
         Elements along the new dimensions are laid out according to the order of `dims`.
 
         The type of the new dimension will be equal to the types of `dims`.
         If `dims` have varying types, the new dimension will be a batch dimension.
 
@@ -518,15 +518,15 @@
 
     def __setitem__(self, key, value):
         self.obj[{self.name: key}] = value
 
     def __getattr__(self, item):
         return _BoundDims(self.obj, (self.name, item))
 
-    def unstack(self, size: int or None = None) -> tuple:
+    def unstack(self, size: Union[int, None] = None) -> tuple:
         """
         Lists the slices along this dimension as a `tuple`.
 
         Args:
             size: (optional) If given as `int`, this dimension can be unstacked even if it is not present on the object.
                 In that case, `size` copies of the object are returned.
```

### Comparing `phiflow-2.3.3/phi/physics/_boundaries.py` & `phiflow-2.3.4/phi/physics/_boundaries.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import warnings
 from numbers import Number
+from typing import Union
 
 from phi import math, field
 from phi.field import CenteredGrid, StaggeredGrid, PointCloud, Field, mask
 from phi.geom import Box, GridCell, Sphere, union, assert_same_rank
 from phi.geom import Geometry
 from phi.math import Tensor, channel, instance
 from phi.math.extrapolation import ZERO, ONE, PERIODIC, BOUNDARY
@@ -14,15 +15,15 @@
 
 warnings.warn("""Domain (phi.physics._boundaries) is deprecated and will be removed in a future release.
 Please create grids directly, replacing the domain with a dict, e.g.
     domain = dict(x=64, y=128, bounds=Box(x=1, y=1))
     grid = CenteredGrid(0, **domain)""", FutureWarning, stacklevel=2)
 
 
-def _create_boundary_conditions(obj: dict or tuple or list, spatial_dims: tuple) -> dict:
+def _create_boundary_conditions(obj: Union[dict, tuple, list], spatial_dims: tuple) -> dict:
     """
     Construct mixed boundary conditions from from a sequence of boundary conditions.
 
     Args:
       obj: single boundary condition or sequence of boundary conditions
 
     Returns:
@@ -66,15 +67,15 @@
     'active': PERIODIC,
     'accessible': PERIODIC,
 }
 
 
 class Domain:
 
-    def __init__(self, resolution: math.Shape or tuple or list = math.EMPTY_SHAPE, boundaries: dict or tuple or list = OPEN, bounds: Box = None, **resolution_):
+    def __init__(self, resolution: Union[math.Shape, tuple, list] = math.EMPTY_SHAPE, boundaries: Union[dict, tuple, list] = OPEN, bounds: Box = None, **resolution_):
         """
         The Domain specifies the grid resolution, physical size and boundary conditions of a simulation.
 
         It provides convenience methods for creating Grids fitting the domain, e.g. `grid()`, `vector_grid()` and `staggered_grid()`.
 
         Also see the `phi.physics` module documentation at https://tum-pbs.github.io/PhiFlow/Physics.html
 
@@ -128,17 +129,17 @@
         This is equivalent to calling `domain.cells.center`.
         
         The shape of the returned Tensor extends the domain resolution by one vector dimension.
         """
         return self.cells.center
 
     def grid(self,
-             value: Field or Tensor or Number or Geometry or callable = 0.,
+             value: Union[Field, Tensor, Number, Geometry, callable] = 0.,
              type: type = CenteredGrid,
-             extrapolation: math.Extrapolation = 'scalar') -> CenteredGrid or StaggeredGrid:
+             extrapolation: math.Extrapolation = 'scalar') -> Union[CenteredGrid, StaggeredGrid]:
         """
         Creates a grid matching the resolution and bounds of the domain.
         The grid is created from the given `value` which must be one of the following:
         
         * Number (int, float, complex or zero-dimensional tensor): all grid values will be equal to `value`. This has a near-zero memory footprint.
         * Field: the given value is resampled to the grid cells of this Domain.
         * Tensor with spatial dimensions matching the domain resolution: grid values will equal `value`.
@@ -153,16 +154,16 @@
         Returns:
             Grid of specified type
         """
         extrapolation = extrapolation if isinstance(extrapolation, math.Extrapolation) else self.boundaries[extrapolation]
         return type(value, resolution=self.resolution, bounds=self.bounds, extrapolation=extrapolation)
 
     def scalar_grid(self,
-                    value: Field or Tensor or Number or Geometry or callable = 0.,
-                    extrapolation: str or math.Extrapolation = 'scalar') -> CenteredGrid:
+                    value: Union[Field, Tensor, Number, Geometry, callable] = 0.,
+                    extrapolation: Union[str, math.Extrapolation] = 'scalar') -> CenteredGrid:
         """
         Creates a scalar grid matching the resolution and bounds of the domain.
         The grid is created from the given `value` which must be one of the following:
 
         * Number (int, float, complex or zero-dimensional tensor): all grid values will be equal to `value`. This has a near-zero memory footprint.
         * Scalar `Field`: the given value is resampled to the grid cells of this Domain.
         * Tensor with spatial dimensions matching the domain resolution: grid values will equal `value`.
@@ -193,17 +194,17 @@
                 pass
             value = math.wrap(value)
         result = CenteredGrid(value, resolution=self.resolution, bounds=self.bounds, extrapolation=extrapolation)
         assert result.shape.channel_rank == 0
         return result
 
     def vector_grid(self,
-                    value: Field or Tensor or Number or Geometry or callable = 0.,
+                    value: Union[Field, Tensor, Number, Geometry, callable] = 0.,
                     type: type = CenteredGrid,
-                    extrapolation: math.Extrapolation or str = 'vector') -> CenteredGrid or StaggeredGrid:
+                    extrapolation: Union[math.Extrapolation, str] = 'vector') -> Union[CenteredGrid, StaggeredGrid]:
         """
         Creates a vector grid matching the resolution and bounds of the domain.
         The grid is created from the given `value` which must be one of the following:
         
         * Number (int, float, complex or zero-dimensional tensor): all grid values will be equal to `value`. This has a near-zero memory footprint.
         * Field: the given value is resampled to the grid cells of this Domain.
         * Tensor with spatial dimensions matcing the domain resolution: grid values will equal `value`.
@@ -225,16 +226,16 @@
         if result.shape.channel_rank == 0:
             result = result.with_values(math.expand(result.values, channel(vector=self.rank)))
         else:
             assert result.shape.get_size('vector') == self.rank
         return result
 
     def staggered_grid(self,
-                       value: Field or Tensor or Number or Geometry or callable = 0.,
-                       extrapolation: math.Extrapolation or str = 'vector') -> StaggeredGrid:
+                       value: Union[Field, Tensor, Number, Geometry, callable] = 0.,
+                       extrapolation: Union[math.Extrapolation, str] = 'vector') -> StaggeredGrid:
         """
         Creates a staggered grid matching the resolution and bounds of the domain.
         This is equal to calling `vector_grid()` with `type=StaggeredGrid`.
         
         The grid is created from the given `value` which must be one of the following:
         
         * Number (int, float, complex or zero-dimensional tensor): all grid values will be equal to `value`. This has a near-zero memory footprint.
@@ -251,24 +252,24 @@
 
         Returns:
           Grid of specified type
         """
         return self.vector_grid(value, type=StaggeredGrid, extrapolation=extrapolation)
 
     def vector_potential(self,
-                         value: Field or Tensor or Number or Geometry or callable = 0.,
-                         extrapolation: str or math.Extrapolation = 'scalar',
+                         value: Union[Field, Tensor, Number, Geometry, callable] = 0.,
+                         extrapolation: Union[str, math.Extrapolation] = 'scalar',
                          curl_type=CenteredGrid):
         if self.rank == 2 and curl_type == StaggeredGrid:
             pot_bounds = Box(self.bounds.lower - 0.5 * self.dx, self.bounds.upper + 0.5 * self.dx)
             alt_domain = Domain(self.boundaries, self.resolution + 1, bounds=pot_bounds)
             return alt_domain.scalar_grid(value, extrapolation=extrapolation)
         raise NotImplementedError()
 
-    def accessible_mask(self, not_accessible: tuple or list, type: type = CenteredGrid, extrapolation='accessible') -> CenteredGrid or StaggeredGrid:
+    def accessible_mask(self, not_accessible: Union[tuple, list], type: type = CenteredGrid, extrapolation='accessible') -> Union[CenteredGrid, StaggeredGrid]:
         """
         Unifies domain and Obstacle or Geometry objects into a binary StaggeredGrid mask which can be used
         to enforce boundary conditions.
 
         Args:
             not_accessible: blocked region(s) of space specified by geometries
             type: class of Grid to create, must be either CenteredGrid or StaggeredGrid
@@ -283,19 +284,19 @@
             return accessible_mask
         elif type is StaggeredGrid:
             return field.stagger(accessible_mask, math.minimum, extrapolation)
         else:
             raise ValueError('Unknown grid type: %s' % type)
 
     def points(self,
-               points: Tensor or Number or tuple or list,
-               values: Tensor or Number = None,
-               radius: Tensor or float or int or None = None,
+               points: Union[Tensor, Number, tuple, list],
+               values: Union[Tensor, Number] = None,
+               radius: Union[Tensor, float, int, None] = None,
                extrapolation: math.Extrapolation = math.extrapolation.ZERO,
-               color: str or Tensor or tuple or list or None = None) -> PointCloud:
+               color: Union[str, Tensor, tuple, list, None] = None) -> PointCloud:
         """
         Create a `phi.field.PointCloud` from the given `points`.
         The created field has no channel dimensions and all points carry the value `1`.
 
         Args:
             points: point locations in physical units
             values: (optional) values of the particles, defaults to 1.
@@ -319,15 +320,15 @@
                 points = math.tensor(points, instance('points'), channel('vector'))
         elements = Sphere(points, radius)
         if values is None:
             values = math.tensor(1.)
         return PointCloud(elements, values, extrapolation, add_overlapping=False, bounds=self.bounds, color=color)
 
     def distribute_points(self,
-                          geometries: tuple or list,
+                          geometries: Union[tuple, list],
                           points_per_cell: int = 8,
                           color: str = None,
                           center: bool = False) -> PointCloud:
         """
         Transforms `Geometry` objects into a PointCloud.
 
         Args:
```

### Comparing `phiflow-2.3.3/phi/physics/advect.py` & `phiflow-2.3.4/phi/physics/advect.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 Examples:
 
 * semi_lagrangian (grid)
 * mac_cormack (grid)
 * runge_kutta_4 (particle)
 """
+from typing import Union
+
 from phi.math import Solve, channel
 
 from phi import math
 from phi.field import SampledField, Field, PointCloud, Grid, sample, reduce_sample, spatial_gradient, unstack, stack, CenteredGrid, StaggeredGrid
 from phi.field._field import FieldType
 from phi.field._field_math import GridType
 from phi.geom import Geometry
@@ -44,15 +46,15 @@
     vel_nan = math.where(math.is_finite(vel_rk4), vel_rk4, v0)
     return elements.shifted(dt * vel_nan)
 
 
 
 def advect(field: SampledField,
            velocity: Field,
-           dt: float or math.Tensor,
+           dt: Union[float, math.Tensor],
            integrator=euler) -> FieldType:
     """
     Advect `field` along the `velocity` vectors using the specified integrator.
 
     The behavior depends on the type of `field`:
 
     * `phi.field.PointCloud`: Points are advected forward, see `points`.
```

### Comparing `phiflow-2.3.3/phi/physics/diffuse.py` & `phiflow-2.3.4/phi/physics/diffuse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Functions to simulate diffusion processes on `phi.field.Field` objects.
 """
+from typing import Union
+
 from phi import math
 from phi.field import Grid, Field, laplace, solve_linear, jit_compile_linear
 from phi.field._field import FieldType
 from phi.field._grid import GridType
 from phi.math import copy_with, shape, Solve
 
 
 def explicit(field: FieldType,
-             diffusivity: float or math.Tensor or Field,
-             dt: float or math.Tensor,
+             diffusivity: Union[float, math.Tensor, Field],
+             dt: Union[float, math.Tensor],
              substeps: int = 1) -> FieldType:
     """
     Simulate a finite-time diffusion process of the form dF/dt = α · ΔF on a given `Field` FieldType with diffusion coefficient α.
 
     Args:
         field: CenteredGrid, StaggeredGrid or ConstantField
         diffusivity: Diffusion per time. `diffusion_amount = diffusivity * dt`
@@ -33,16 +35,16 @@
     for i in range(substeps):
         delta = laplace(field, weights=amount) if 'vector' in shape(amount) else amount * laplace(field)
         field = (field + delta.with_extrapolation(ext)).with_extrapolation(ext)
     return field
 
 
 def implicit(field: FieldType,
-             diffusivity: float or math.Tensor or Field,
-             dt: float or math.Tensor,
+             diffusivity: Union[float, math.Tensor, Field],
+             dt: Union[float, math.Tensor],
              order: int = 1,
              solve=Solve('CG')) -> FieldType:
     """
     Diffusion by solving a linear system of equations.
 
     Args:
         order: Order of method, 1=first order. This translates to `substeps` for the explicit sharpening.
@@ -60,15 +62,15 @@
 
     if not solve.x0:
         solve = copy_with(solve, x0=field)
     return solve_linear(sharpen, y=field, solve=solve)
 
 
 def finite_difference(grid: Grid,
-                      diffusivity: float or math.Tensor or Field,
+                      diffusivity: Union[float, math.Tensor, Field],
                       order: int,
                       implicit: math.Solve) -> FieldType:
 
     """
     Diffusion by using a finite difference scheme.
     In contrast to `explicit` and `implicit` accuracy can be increased by using stencils of higher-order rather than calculating substeps.
     This is controlled by the `scheme` passed.
@@ -86,16 +88,16 @@
         Diffused grid of same type as `grid`.
     """
     diffusivity = diffusivity.at(grid) if isinstance(diffusivity, Field) else diffusivity
     return diffusivity * laplace(grid, order=order, implicit=implicit).with_extrapolation(grid.extrapolation)
 
 
 def fourier(field: GridType,
-            diffusivity: float or math.Tensor,
-            dt: float or math.Tensor) -> FieldType:
+            diffusivity: Union[float, math.Tensor],
+            dt: Union[float, math.Tensor]) -> FieldType:
     """
     Exact diffusion of a periodic field in frequency space.
 
     For non-periodic fields or non-constant diffusivity, use another diffusion function such as `explicit()`.
 
     Args:
         field:
```

### Comparing `phiflow-2.3.3/phi/physics/fluid.py` & `phiflow-2.3.4/phi/physics/fluid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Functions for simulating incompressible fluids, both grid-based and particle-based.
 
 The main function for incompressible fluids (Eulerian as well as FLIP / PIC) is `make_incompressible()` which removes the divergence of a velocity field.
 """
 import warnings
-from typing import Tuple, Callable
+from typing import Tuple, Callable, Union
 
 from phi import math, field
 from phi.math import wrap, channel, Solve
 from phi.field import AngularVelocity, Grid, divergence, spatial_gradient, where, CenteredGrid, PointCloud, Field, resample
 from phi.geom import union, Geometry
 from ..field._embed import FieldEmbedding
 from ..field._grid import GridType, StaggeredGrid
@@ -59,15 +59,15 @@
     obstacles = [Obstacle(o) if isinstance(o, Geometry) else o for o in obstacles]
     for obstacle in obstacles:
         assert obstacle.geometry.vector.item_names == space.vector.item_names, f"Obstacles must live in the same physical space as the velocity field {space.vector.item_names} but got {type(obstacle.geometry).__name__} obstacle with order {obstacle.geometry.vector.item_names}"
     return obstacles
 
 
 def make_incompressible(velocity: GridType,
-                        obstacles: Obstacle or Geometry or tuple or list = (),
+                        obstacles: Union[Obstacle, Geometry, tuple, list] = (),
                         solve: Solve = Solve(),
                         active: CenteredGrid = None,
                         order: int = 2) -> Tuple[GridType, CenteredGrid]:
     """
     Projects the given velocity field by solving for the pressure and subtracting its spatial_gradient.
     
     This method is similar to :func:`field.divergence_free()` but differs in how the boundary conditions are specified.
@@ -153,15 +153,15 @@
     return laplace
 
 
 def _balance_divergence(div, active):
     return div - active * (field.mean(div) / field.mean(active))
 
 
-def apply_boundary_conditions(velocity: Grid or PointCloud, obstacles: Obstacle or Geometry or tuple or list):
+def apply_boundary_conditions(velocity: Union[Grid, PointCloud], obstacles: Union[Obstacle, Geometry, tuple, list]):
     """
     Enforces velocities boundary conditions on a velocity grid.
     Cells inside obstacles will get their velocity from the obstacle movement.
     Cells outside far away will be unaffected.
 
     Args:
       velocity: Velocity `Grid`.
@@ -181,15 +181,15 @@
             velocity = (1 - obs_mask) * velocity
         else:
             angular_velocity = AngularVelocity(location=obstacle.geometry.center, strength=obstacle.angular_velocity, falloff=None) @ velocity
             velocity = (1 - obs_mask) * velocity + obs_mask * (angular_velocity + obstacle.velocity)
     return velocity
 
 
-def boundary_push(particles: PointCloud, obstacles: tuple or list, offset: float = 0.5) -> PointCloud:
+def boundary_push(particles: PointCloud, obstacles: Union[tuple, list], offset: float = 0.5) -> PointCloud:
     """
     Enforces boundary conditions by correcting possible errors of the advection step and shifting particles out of
     obstacles or back into the domain.
 
     Args:
         particles: PointCloud holding particle positions as elements
         obstacles: List of `Obstacle` or `Geometry` objects where any particles inside should get shifted outwards
```

### Comparing `phiflow-2.3.3/phi/tf/__init__.py` & `phiflow-2.3.4/phi/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/tf/_compile_cuda.py` & `phiflow-2.3.4/phi/tf/_compile_cuda.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/tf/_profiling.py` & `phiflow-2.3.4/phi/tf/_profiling.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/tf/_tf_backend.py` & `phiflow-2.3.4/phi/tf/_tf_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numbers
 from contextlib import contextmanager
 from functools import wraps, partial
-from typing import List, Callable, Tuple
+from typing import List, Callable, Tuple, Union
 
 import keras
 import numpy as np
 import os
 import tensorflow as tf
 from tensorflow.python.client import device_lib
 from tensorflow.python.framework.errors_impl import NotFoundError
@@ -127,15 +127,15 @@
             return tf.equal(x, y)
 
     def divide_no_nan(self, x, y):
         with self._device_for(x, y):
             x, y = self.auto_cast(x, y)
             return tf.math.divide_no_nan(x, y)
 
-    def random_uniform(self, shape, low, high, dtype: DType or None):
+    def random_uniform(self, shape, low, high, dtype: Union[DType, None]):
         dtype = dtype or self.float_type
         tdt = to_numpy_dtype(dtype)
         with tf.device(self._default_device.ref):
             if dtype.kind != complex:
                 return tf.random.uniform(shape, low, high, dtype=tdt)
             else:
                 real = tf.cast(tf.random.uniform(shape, low.real, high.real, dtype=to_numpy_dtype(DType(float, dtype.precision))), tdt)
@@ -259,15 +259,15 @@
             result = tf.meshgrid(*coordinates, indexing='ij')
             return result
 
     def linspace(self, start, stop, number):
         with tf.device(self._default_device.ref):
             return self.to_float(tf.linspace(start, stop, number))
 
-    def tensordot(self, a, a_axes: tuple or list, b, b_axes: tuple or list):
+    def tensordot(self, a, a_axes: Union[tuple, list], b, b_axes: Union[tuple, list]):
         with self._device_for(a, b):
             a, b = self.auto_cast(a, b, bool_to_int=True)
             return tf.tensordot(a, b, (a_axes, b_axes))
 
     def mul_matrix_batched_vector(self, A, b):
         with self._device_for(A, b):
             if isinstance(A, tf.SparseTensor):
@@ -282,15 +282,15 @@
         with self._device_for(*tensors):
             return tf.einsum(equation, *tensors)
 
     def cumsum(self, x, axis: int):
         with tf.device(x.device):
             return tf.cumsum(x, axis=axis, exclusive=False)
 
-    def while_loop(self, loop: Callable, values: tuple, max_iter: int or Tuple[int, ...] or List[int]):
+    def while_loop(self, loop: Callable, values: tuple, max_iter: Union[int, Tuple[int, ...], List[int]]):
         with self._device_for(*values):
             if isinstance(max_iter, (tuple, list)):  # stack traced trajectory, unroll until max_iter
                 values = self.stop_gradient_tree(values)
                 trj = [values] if 0 in max_iter else []
                 for i in range(1, max(max_iter) + 1):
                     values = loop(*values)
                     if i in max_iter:
@@ -475,15 +475,15 @@
             for b in range(batch_size):
                 b_grid = base_grid[b, ...]
                 b_indices = indices[min(b, indices.shape[0] - 1), ...]
                 b_values = values[min(b, values.shape[0] - 1), ...]
                 result.append(scatter(b_grid, b_indices, b_values))
             return self.stack(result, axis=0)
 
-    def fft(self, x, axes: tuple or list):
+    def fft(self, x, axes: Union[tuple, list]):
         if not axes:
             return x
         x = self.to_complex(x)
         perm = (*[i for i in range(self.ndims(x)) if i not in axes], *axes)
         iperm = np.argsort(perm)
         with tf.device(x.device):
             if len(axes) == 1:
@@ -493,15 +493,15 @@
             elif len(axes) == 3:
                 return tf.transpose(tf.signal.fft3d(tf.transpose(x, perm)), iperm)
             else:
                 for axis in axes:
                     x = self.fft(x, [axis])
                 return x
 
-    def ifft(self, k, axes: tuple or list):
+    def ifft(self, k, axes: Union[tuple, list]):
         if not axes:
             return k
         k = self.to_complex(k)
         perm = (*[i for i in range(self.ndims(k)) if i not in axes], *axes)
         iperm = np.argsort(perm)
         with tf.device(k.device):
             if len(axes) == 1:
@@ -696,15 +696,15 @@
             return a ^ b
 
     def floordiv(self, a, b):
         with self._device_for(a, b):
             a, b = self.auto_cast(a, b)
             return a // b
 
-    def jacobian(self, f, wrt: tuple or list, get_output: bool, is_f_scalar: bool):
+    def jacobian(self, f, wrt: Union[tuple, list], get_output: bool, is_f_scalar: bool):
         @wraps(f)
         def eval_grad(*args):
             args = [self.as_tensor(arg, True) if i in wrt else arg for i, arg in enumerate(args)]
             args = [self.to_float(arg) if self.dtype(arg).kind in (bool, int) else arg for arg in args]
             wrt_args = [arg for i, arg in enumerate(args) if i in wrt]
             with tf.GradientTape(watch_accessed_variables=False) as tape:
                 for arg in wrt_args:
```

### Comparing `phiflow-2.3.3/phi/tf/_tf_cuda_resample.py` & `phiflow-2.3.4/phi/tf/_tf_cuda_resample.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/tf/flow.py` & `phiflow-2.3.4/phi/tf/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/tf/nets.py` & `phiflow-2.3.4/phi/tf/nets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """
 Jax implementation of the unified machine learning API.
 Equivalent functions also exist for the other frameworks.
 
 For API documentation, see https://tum-pbs.github.io/PhiFlow/Network_API .
 """
-from typing import Callable, Tuple, List
 import pickle
 from typing import Callable
-from typing import Tuple, List
+from typing import Union, Sequence
 
 import numpy
 import numpy as np
 import tensorflow as tf
 from tensorflow import Tensor
 from tensorflow import keras
 from tensorflow.keras import layers as kl
-from tensorflow import Tensor
 
 from .. import math
 
 
 def parameter_count(model: keras.Model):
     """
     Counts the number of parameters in a model.
@@ -68,15 +66,15 @@
                 phi_tensor = math.wrap(var, math.channel('output'))
             else:
                 raise NotImplementedError(name, var)
             result[name] = phi_tensor
     return result
 
 
-def save_state(obj: keras.models.Model or keras.optimizers.Optimizer, path: str):
+def save_state(obj: Union[keras.models.Model, keras.optimizers.Optimizer], path: str):
     """
     Write the state of a module or optimizer to a file.
 
     See Also:
         `load_state()`
 
     Args:
@@ -93,15 +91,15 @@
         weights = obj.get_weights()
         with open(path, 'wb') as f:
             pickle.dump(weights, f)
     else:
         raise ValueError("obj must be a Keras model or optimizer")
 
 
-def load_state(obj: keras.models.Model or keras.optimizers.Optimizer, path: str):
+def load_state(obj: Union[keras.models.Model, keras.optimizers.Optimizer], path: str):
     """
     Read the state of a module or optimizer from a file.
 
     See Also:
         `save_state()`
 
     Args:
@@ -176,15 +174,15 @@
     Analogous functions exist for other learning frameworks.
     """
     return keras.optimizers.RMSprop(learning_rate, alpha, momentum, eps, centered)
 
 
 def dense_net(in_channels: int,
               out_channels: int,
-              layers: Tuple[int, ...] or List[int],
+              layers: Sequence[int],
               batch_norm=False,
               activation='ReLU',
               softmax=False) -> keras.Model:
     """
     Fully-connected neural networks are available in ΦFlow via dense_net().
     Arguments:
         in_channels : size of input layer, int
@@ -207,18 +205,18 @@
                                     kl.Dense(out_channels, activation='linear'),
                                     *([kl.Softmax()] if softmax else [])])
 
 
 def u_net(in_channels: int,
           out_channels: int,
           levels: int = 4,
-          filters: int or tuple or list = 16,
+          filters: Union[int, tuple, list] = 16,
           batch_norm: bool = True,
-          activation: str or Callable = 'ReLU',
-          in_spatial: tuple or int = 2,
+          activation: Union[str, Callable] = 'ReLU',
+          in_spatial: Union[tuple, int] = 2,
           periodic=False,
           use_res_blocks: bool = False, **kwargs) -> keras.Model:
     """
     ΦFlow provides a built-in U-net architecture, classically popular for Semantic Segmentation in Computer Vision, composed of downsampling and upsampling layers.
 
     Arguments:
 
@@ -291,19 +289,19 @@
         x = kl.BatchNormalization()(x)
     x = activation(x)
     return x
 
 
 def conv_net(in_channels: int,
              out_channels: int,
-             layers: Tuple[int, ...] or List[int],
+             layers: Sequence[int],
              batch_norm: bool = False,
-             activation: str or Callable = 'ReLU',
+             activation: Union[str, Callable] = 'ReLU',
              periodic=False,
-             in_spatial: int or tuple = 2, **kwargs) -> keras.Model:
+             in_spatial: Union[int, tuple] = 2, **kwargs) -> keras.Model:
     """
     Built in Conv-Nets are also provided. Contrary to the classical convolutional neural networks, the feature map spatial size remains the same throughout the layers. Each layer of the network is essentially a convolutional block comprising of two conv layers. A filter size of 3 is used in the convolutional layers.
     Arguments:
 
         in_channels : input channels of the feature map, dtype : int
         out_channels : output channels of the feature map, dtype : int
         layers : list or tuple of output channels for each intermediate layer between the input and final output channels, dtype : list or tuple
@@ -334,16 +332,16 @@
     return keras.Model(inputs, x)
 
 
 def resnet_block(in_channels: int,
                  out_channels: int,
                  periodic: bool,
                  batch_norm: bool = False,
-                 activation: str or Callable = 'ReLU',
-                 in_spatial: int or tuple = 2):
+                 activation: Union[str, Callable] = 'ReLU',
+                 in_spatial: Union[int, tuple] = 2):
     activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
     if isinstance(in_spatial, int):
         d = in_spatial
     else:
         assert isinstance(in_spatial, tuple)
         d = len(in_spatial)
     x = x_1 = inputs = keras.Input(shape=(None,) * d + (in_channels,))
@@ -361,19 +359,19 @@
             x_1 = kl.BatchNormalization()(x_1)
     x = kl.Add()([x, x_1])
     return keras.Model(inputs, x)
 
 
 def res_net(in_channels: int,
             out_channels: int,
-            layers: Tuple[int, ...] or List[int],
+            layers: Sequence[int],
             batch_norm: bool = False,
-            activation: str or Callable = 'ReLU',
+            activation: Union[str, Callable] = 'ReLU',
             periodic=False,
-            in_spatial: int or tuple = 2, **kwargs):
+            in_spatial: Union[int, tuple] = 2, **kwargs):
     """
     Built in Res-Nets are provided in the ΦFlow framework. Similar to the conv-net, the feature map spatial size remains the same throughout the layers.
     These networks use residual blocks composed of two conv layers with a skip connection added from the input to the output feature map.
     A default filter size of 3 is used in the convolutional layers.
 
     Arguments:
 
@@ -402,15 +400,15 @@
     for i in range(1, len(layers)):
         out = resnet_block(layers[i - 1], layers[i], periodic, batch_norm, activation, d)(out)
     out = CONV[d](out_channels, 1)(out)
     return keras.Model(inputs, out)
 
 
 def conv_classifier(in_features: int,
-                    in_spatial: tuple or list,
+                    in_spatial: Union[tuple, list],
                     num_classes: int,
                     blocks=(64, 128, 256, 256, 512, 512),
                     dense_layers=(4096, 4096, 100),
                     batch_norm=True,
                     activation='ReLU',
                     softmax=True,
                     periodic=False):
@@ -476,15 +474,15 @@
 
     return checker
 
 
 def Dense_resnet_block(in_channels: int,
                        mid_channels: int,
                        batch_norm: bool = False,
-                       activation: str or Callable = 'ReLU'):
+                       activation: Union[str, Callable] = 'ReLU'):
     inputs = keras.Input(shape=(in_channels,))
     x_1 = inputs
     activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
 
     x = kl.Dense(mid_channels)(inputs)
     if batch_norm:
         x = kl.BatchNormalization()(x)
@@ -576,16 +574,16 @@
         return x
 
 
 def invertible_net(in_channels: int,
                    num_blocks: int,
                    batch_norm: bool = False,
                    net: str = 'u_net',
-                   activation: str or type = 'ReLU',
-                   in_spatial: tuple or int = 2, **kwargs):
+                   activation: Union[str, type] = 'ReLU',
+                   in_spatial: Union[tuple, int] = 2, **kwargs):
     """
     ΦFlow also provides invertible neural networks that are capable of inverting the output tensor back to the input tensor initially passed.\ These networks have far reaching applications in predicting input parameters of a problem given its observations.\ Invertible nets are composed of multiple concatenated coupling blocks wherein each such block consists of arbitrary neural networks.
 
     Currently, these arbitrary neural networks could be set to u_net(default), conv_net, res_net or dense_net blocks with in_channels = out_channels.
     The architecture used is popularized by ["Real NVP"](https://arxiv.org/abs/1605.08803).
 
     Arguments:
@@ -776,16 +774,16 @@
 
         return x
 
 
 def fno(in_channels: int,
         out_channels: int,
         mid_channels: int,
-        modes: Tuple[int, ...] or List[int],
-        activation: str or type = 'ReLU',
+        modes: Sequence[int],
+        activation: Union[str, type] = 'ReLU',
         batch_norm: bool = False,
         in_spatial: int = 2):
     """
     ["Fourier Neural Operator"](https://github.com/zongyi-li/fourier_neural_operator) network contains 4 layers of the Fourier layer.
     1. Lift the input to the desire channel dimension by self.fc0 .
     2. 4 layers of the integral operators u' = (W + K)(u). W defined by self.w; K defined by self.conv .
     3. Project from the channel space to the output space by self.fc1 and self.fc2.
```

### Comparing `phiflow-2.3.3/phi/torch/_torch_backend.py` & `phiflow-2.3.4/phi/torch/_torch_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numbers
 import warnings
 from contextlib import contextmanager
 from functools import wraps
-from typing import List, Callable, Optional, Set, Tuple, Any
+from typing import List, Callable, Optional, Set, Tuple, Any, Union
 
 import numpy as np
 import torch
 import torch.fft
 import torch.nn.functional as torchf
 from packaging import version
 
@@ -184,15 +184,15 @@
     def transpose(self, tensor, axes):
         return tensor.permute(axes)
 
     def equal(self, x, y):
         x, y = self.auto_cast(x, y)
         return x == y
 
-    def random_uniform(self, shape, low, high, dtype: DType or None):
+    def random_uniform(self, shape, low, high, dtype: Union[DType, None]):
         dtype = dtype or self.float_type
         if dtype.kind == float:
             return low + (high - low) * torch.rand(size=shape, dtype=to_torch_dtype(dtype), device=self.get_default_device().ref)
         elif dtype.kind == complex:
             real = low.real + (high.real - low.real) * torch.rand(size=shape, dtype=to_torch_dtype(DType(float, dtype.precision)), device=self.get_default_device().ref)
             imag = low.imag + (high.imag - low.imag) * torch.rand(size=shape, dtype=to_torch_dtype(DType(float, dtype.precision)), device=self.get_default_device().ref)
             return real + 1j * imag
@@ -381,15 +381,15 @@
     def linspace(self, start, stop, number):
         if self.is_tensor(stop, only_native=True) or self.is_tensor(start, only_native=True):
             unit = torch.linspace(0, 1, number, dtype=to_torch_dtype(self.float_type), device=self.get_default_device().ref)
             return unit * (stop - start) + start
         else:
             return torch.linspace(start, stop, number, dtype=to_torch_dtype(self.float_type), device=self.get_default_device().ref)
 
-    def tensordot(self, a, a_axes: tuple or list, b, b_axes: tuple or list):
+    def tensordot(self, a, a_axes: Union[tuple, list], b, b_axes: Union[tuple, list]):
         a, b = self.auto_cast(a, b)
         return torch.tensordot(a, b, (a_axes, b_axes))
 
     def mul_matrix_batched_vector(self, A, b):
         A, b = self.auto_cast(A, b)
         if isinstance(A, torch.Tensor) and (A.is_sparse or A.is_sparse_csr):
             result = torch.sparse.mm(A, torch.transpose(b, 0, 1))
@@ -399,15 +399,15 @@
 
     def get_diagonal(self, matrices, offset=0):
         return torch.transpose(torch.diagonal(matrices, offset=offset, dim1=1, dim2=2), 1, 2)
 
     def cumsum(self, x, axis: int):
         return torch.cumsum(x, dim=axis)
 
-    def while_loop(self, loop: Callable, values: tuple, max_iter: int or Tuple[int, ...] or List[int]):
+    def while_loop(self, loop: Callable, values: tuple, max_iter: Union[int, Tuple[int, ...], List[int]]):
         tracing = torch._C._get_tracing_state() is not None
         if not tracing:
             return Backend.while_loop(self, loop, values, max_iter)
         # --- We are tracing ---
         warnings.warn("PyTorch while_loop always iterates until max_iter. Please put a while loop into a torch.ScriptFunction instead.", RuntimeWarning)
         values = self.stop_gradient_tree(values)
         if isinstance(max_iter, (tuple, list)):
@@ -583,22 +583,22 @@
         result = scatter(base_grid_flat, dim=1, index=indices, src=values)
         return torch.reshape(result, base_grid.shape)
 
     def arctan2(self, y, x):
         y, x = self.auto_cast(y, x)
         return torch.arctan2(y, x)
 
-    def fft(self, x, axes: tuple or list):
+    def fft(self, x, axes: Union[tuple, list]):
         if not x.is_complex():
             x = self.to_complex(x)
         for i in axes:
             x = torch.fft.fft(x, dim=i)
         return x
 
-    def ifft(self, k, axes: tuple or list):
+    def ifft(self, k, axes: Union[tuple, list]):
         if not k.is_complex():
             k = self.to_complex(k)
         for i in axes:
             k = torch.fft.ifft(k, dim=i)
         return k
 
     def imag(self, x):
@@ -757,15 +757,15 @@
 
     def solve_triangular_dense(self, matrix, rhs, lower: bool, unit_diagonal: bool):
         matrix, rhs = self.auto_cast(matrix, rhs, int_to_float=True, bool_to_int=True)
         rhs = self.expand_dims(rhs, -1)
         x = torch.linalg.solve_triangular(matrix, rhs, upper=not lower, unitriangular=unit_diagonal)
         return x[..., 0]
 
-    def _prepare_graph_inputs(self, args: tuple, wrt: tuple or list):
+    def _prepare_graph_inputs(self, args: tuple, wrt: Union[tuple, list]):
         args = [self.as_tensor(arg, True) if i in wrt else arg for i, arg in enumerate(args)]
         args = [self.to_float(arg) if self.dtype(arg).kind == int else arg for arg in args]
         for i, arg in enumerate(args):
             if self.is_tensor(arg, True) and arg.requires_grad and not arg.is_leaf:
                 arg = torch.clone(arg).detach()
                 arg.requires_grad = i in wrt
                 args[i] = arg
@@ -775,28 +775,28 @@
                 arg.requires_grad = True
                 args[i] = arg
         wrt_args = [arg for i, arg in enumerate(args) if i in wrt]
         for t in wrt_args:
             assert t.requires_grad
         return args, wrt_args
 
-    def jacobian(self, f, wrt: tuple or list, get_output: bool, is_f_scalar: bool):
+    def jacobian(self, f, wrt: Union[tuple, list], get_output: bool, is_f_scalar: bool):
         @wraps(f)
         def eval_grad(*args):
             args, wrt_args = self._prepare_graph_inputs(args, wrt)
             loss, output = f(*args)
             if np.prod(self.staticshape(loss)) == 1:
                 grads = torch.autograd.grad(loss, wrt_args)  # grad() cannot be called during jit trace
             else:
                 raise NotImplementedError()
                 grads = torch.autograd.grad(loss, wrt_args, retain_graph=True)
             return (*output, *grads) if get_output else grads
         return eval_grad
 
-    def hessian(self, f: Callable, wrt: tuple or list, get_output: bool, get_gradient: bool):
+    def hessian(self, f: Callable, wrt: Union[tuple, list], get_output: bool, get_gradient: bool):
         # if not get_output and not get_gradient:
         # @wraps(f)
         # def eval_hessian(*args):
         #     batch_size = args[0].shape[0]
         #     for arg in args:
         #         assert arg.shape[0] == batch_size, f"All arguments must have a matching batch dimension as their first dimension. Got shapes {[arg.shape for arg in args]}"
         #
@@ -876,19 +876,19 @@
             if get_gradient:
                 result += tuple([g.detach() for g in grads]),
             result += hessian,
             return result
 
         return eval_hessian
 
-    def jit_compile_grad(self, f, wrt: tuple or list, get_output: bool, is_f_scalar: bool):
+    def jit_compile_grad(self, f, wrt: Union[tuple, list], get_output: bool, is_f_scalar: bool):
         jit = self.jit_compile(f)
         return self.jacobian(jit, wrt, get_output, is_f_scalar)
 
-    def jit_compile_hessian(self, f, wrt: tuple or list, get_output: bool, get_gradient: bool):
+    def jit_compile_hessian(self, f, wrt: Union[tuple, list], get_output: bool, get_gradient: bool):
         jit = self.jit_compile(f)
         return self.hessian(jit, wrt, get_output, get_gradient)
 
     def stop_gradient(self, value):
         return value.detach()
```

### Comparing `phiflow-2.3.3/phi/torch/flow.py` & `phiflow-2.3.4/phi/torch/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/torch/nets.py` & `phiflow-2.3.4/phi/torch/nets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 PyTorch implementation of the unified machine learning API.
 Equivalent functions also exist for the other frameworks.
 
 For API documentation, see https://tum-pbs.github.io/PhiFlow/Network_API .
 """
-from typing import Callable, List, Tuple
+from typing import Callable, Union, Sequence
 
 import numpy
 import numpy as np
 import torch
 import torch.nn as nn
 from torch import optim
 
@@ -52,15 +52,15 @@
             phi_tensor = math.wrap(param, channel('output'))
         else:
             raise NotImplementedError
         result[name] = phi_tensor
     return result
 
 
-def save_state(obj: nn.Module or optim.Optimizer, path: str):
+def save_state(obj: Union[nn.Module, optim.Optimizer], path: str):
     """
     Write the state of a module or optimizer to a file.
 
     See Also:
         `load_state()`
 
     Args:
@@ -68,15 +68,15 @@
         path: File path as `str`.
     """
     if not path.endswith('.pth'):
         path += '.pth'
     torch.save(obj.state_dict(), path)
 
 
-def load_state(obj: nn.Module or optim.Optimizer, path: str):
+def load_state(obj: Union[nn.Module, optim.Optimizer], path: str):
     """
     Read the state of a module or optimizer from a file.
 
     See Also:
         `save_state()`
 
     Args:
@@ -157,17 +157,17 @@
 CONV = [None, _bias0(nn.Conv1d), _bias0(nn.Conv2d), _bias0(nn.Conv3d)]
 NORM = [None, nn.BatchNorm1d, nn.BatchNorm2d, nn.BatchNorm3d]
 ACTIVATIONS = {'ReLU': nn.ReLU, 'Sigmoid': nn.Sigmoid, 'tanh': nn.Tanh, 'SiLU': nn.SiLU, 'GeLU': nn.GELU}
 
 
 def dense_net(in_channels: int,
               out_channels: int,
-              layers: Tuple[int, ...] or List[int],
+              layers: Sequence[int],
               batch_norm=False,
-              activation: str or Callable = 'ReLU',
+              activation: Union[str, Callable] = 'ReLU',
               softmax=False) -> nn.Module:
     """
     Fully-connected neural networks are available in Φ-Flow via dense_net().
     Arguments:
         in_channels : size of input layer, int
         out_channels = size of output layer, int
         layers : tuple of linear layers between input and output neurons, list or tuple
@@ -213,18 +213,18 @@
             x = self.softmax(x)
         return x
 
 
 def u_net(in_channels: int,
           out_channels: int,
           levels: int = 4,
-          filters: int or tuple or list = 16,
+          filters: Union[int, tuple, list] = 16,
           batch_norm: bool = True,
-          activation: str or type = 'ReLU',
-          in_spatial: tuple or int = 2,
+          activation: Union[str, type] = 'ReLU',
+          in_spatial: Union[tuple, int] = 2,
           periodic=False,
           use_res_blocks: bool = False,
           **kwargs) -> nn.Module:
     """
     ΦFlow provides a built-in U-net architecture, classically popular for Semantic Segmentation in Computer Vision, composed of downsampling and upsampling layers.
 
     Arguments:
@@ -306,15 +306,15 @@
 
 MAX_POOL = [None, nn.MaxPool1d, nn.MaxPool2d, nn.MaxPool3d]
 
 
 class Down(nn.Module):
     """Downscaling with maxpool then double conv or resnet_block"""
 
-    def __init__(self, d: int, in_channels: int, out_channels: int, batch_norm: bool, activation: str or type, use_res_blocks: bool, periodic):
+    def __init__(self, d: int, in_channels: int, out_channels: int, batch_norm: bool, activation: Union[str, type], use_res_blocks: bool, periodic):
         super().__init__()
         self.add_module('maxpool', MAX_POOL[d](2))
         if use_res_blocks:
             self.add_module('conv', resnet_block(d, in_channels, out_channels, batch_norm, activation, periodic))
         else:
             self.add_module('conv', DoubleConv(d, in_channels, out_channels, out_channels, batch_norm, activation, periodic))
 
@@ -376,18 +376,18 @@
             x = getattr(self, f'Conv{i}')(x)
         x = getattr(self, f'Conv_out')(x)
         return x
 
 
 def conv_net(in_channels: int,
              out_channels: int,
-             layers: Tuple[int, ...] or List[int],
+             layers: Sequence[int],
              batch_norm: bool = False,
-             activation: str or type = 'ReLU',
-             in_spatial: int or tuple = 2,
+             activation: Union[str, type] = 'ReLU',
+             in_spatial: Union[int, tuple] = 2,
              periodic=False,
              **kwargs) -> nn.Module:
     """
     Built in Conv-Nets are also provided. Contrary to the classical convolutional neural networks, the feature map spatial size remains the same throughout the layers. Each layer of the network is essentially a convolutional block comprising of two conv layers. A filter size of 3 is used in the convolutional layers.
     Arguments:
 
         in_channels : input channels of the feature map, dtype : int
@@ -511,18 +511,18 @@
             x = getattr(self, f'Res{i}')(x)
         x = getattr(self, 'Res_out')(x)
         return x
 
 
 def res_net(in_channels: int,
             out_channels: int,
-            layers: Tuple[int, ...] or List[int],
+            layers: Sequence[int],
             batch_norm: bool = False,
-            activation: str or type = 'ReLU',
-            in_spatial: int or tuple = 2,
+            activation: Union[str, type] = 'ReLU',
+            in_spatial: Union[int, tuple] = 2,
             periodic=False,
             **kwargs) -> nn.Module:
     """
     Built in Res-Nets are provided in the ΦFlow framework. Similar to the conv-net, the feature map spatial size remains the same throughout the layers.
     These networks use residual blocks composed of two conv layers with a skip connection added from the input to the output feature map.
     A default filter size of 3 is used in the convolutional layers.
 
@@ -547,15 +547,15 @@
         d = len(in_spatial)
     net = ResNet(d, in_channels, out_channels, layers, batch_norm, activation, periodic)
     net = net.to(TORCH.get_default_device().ref)
     return net
 
 
 def conv_classifier(in_features: int,
-                    in_spatial: tuple or list,
+                    in_spatial: Union[tuple, list],
                     num_classes: int,
                     blocks=(64, 128, 256, 256, 512, 512),
                     dense_layers=(4096, 4096, 100),
                     batch_norm=True,
                     activation='ReLU',
                     softmax=True,
                     periodic=False):
@@ -668,16 +668,16 @@
         return x
 
 
 def invertible_net(in_channels: int,
                    num_blocks: int,
                    batch_norm: bool = False,
                    net: str = 'u_net',
-                   activation: str or type = 'ReLU',
-                   in_spatial: tuple or int = 2, **kwargs):
+                   activation: Union[str, type] = 'ReLU',
+                   in_spatial: Union[tuple, int] = 2, **kwargs):
     """
     Phiflow also provides invertible neural networks that are capable of inverting the output tensor back to the input tensor initially passed.\ These networks have far reaching applications in predicting input parameters of a problem given its observations.\ Invertible nets are composed of multiple concatenated coupling blocks wherein each such block consists of arbitrary neural networks.
 
     Currently, these arbitrary neural networks could be set to u_net(default), conv_net, res_net or dense_net blocks with in_channels = out_channels.
     The architecture used is popularized by ["Real NVP"](https://arxiv.org/abs/1605.08803).
 
     Arguments:
@@ -700,18 +700,18 @@
     if isinstance(in_spatial, tuple):
         in_spatial = len(in_spatial)
 
     return InvertibleNet(in_channels, num_blocks, activation, batch_norm, in_spatial, net).to(TORCH.get_default_device().ref)
 
 
 def coupling_layer(in_channels: int,
-                   activation: str or type = 'ReLU',
+                   activation: Union[str, type] = 'ReLU',
                    batch_norm=False,
                    reverse_mask=False,
-                   in_spatial: tuple or int = 2):
+                   in_spatial: Union[tuple, int] = 2):
     if isinstance(in_spatial, tuple):
         in_spatial = len(in_spatial)
 
     net = CouplingLayer(in_channels, activation, batch_norm, in_spatial, reverse_mask)
     net = net.to(TORCH.get_default_device().ref)
     return net
 
@@ -877,16 +877,16 @@
 
         return x
 
 
 def fno(in_channels: int,
         out_channels: int,
         mid_channels: int,
-        modes: Tuple[int, ...] or List[int],
-        activation: str or type = 'ReLU',
+        modes: Sequence[int],
+        activation: Union[str, type] = 'ReLU',
         batch_norm: bool = False,
         in_spatial: int = 2):
     """
     ["Fourier Neural Operator"](https://github.com/zongyi-li/fourier_neural_operator) network contains 4 layers of the Fourier layer.
     1. Lift the input to the desire channel dimension by self.fc0 .
     2. 4 layers of the integral operators u' = (W + K)(u). W defined by self.w; K defined by self.conv .
     3. Project from the channel space to the output space by self.fc1 and self.fc2.
```

### Comparing `phiflow-2.3.3/phi/vis/__init__.py` & `phiflow-2.3.4/phi/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_console/_console_gui.py` & `phiflow-2.3.4/phi/vis/_console/_console_gui.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_console/_console_plot.py` & `phiflow-2.3.4/phi/vis/_console/_console_plot.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_console/_console_util.py` & `phiflow-2.3.4/phi/vis/_console/_console_util.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_dash/_plotly_plots.py` & `phiflow-2.3.4/phi/vis/_dash/_plotly_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import Tuple, Any, Dict, List, Callable
+from typing import Tuple, Any, Dict, List, Callable, Union
 
 import numpy
 import numpy as np
 from plotly import graph_objects, figure_factory
 from plotly.subplots import make_subplots
 from plotly.tools import DEFAULT_PLOTLY_COLORS
 
@@ -374,15 +374,15 @@
         else:
             x = (val - color1[0]) / (color2[0] - color1[0])  # weight of row2
             center = color1 * (1 - x) + color2 * x
     center[0] = val
     return center
 
 
-def plot_scalars(curves: tuple or list, labels, subplots=True, log_scale='', smooth: int = 1):
+def plot_scalars(curves: Union[tuple, list], labels, subplots=True, log_scale='', smooth: int = 1):
     if not curves:
         return graph_objects.Figure()
     if subplots:
         fig = make_subplots(rows=1, cols=len(curves), subplot_titles=labels)
         for col, (label, (x, y)) in enumerate(zip(labels, curves)):
             for trace in _graph(label, x, y, smooth, col):
                 fig.add_trace(trace, row=1, col=1 + col)
```

### Comparing `phiflow-2.3.3/phi/vis/_dash/board.py` & `phiflow-2.3.4/phi/vis/_dash/board.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_dash/colormaps.py` & `phiflow-2.3.4/phi/vis/_dash/colormaps.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_dash/dash_app.py` & `phiflow-2.3.4/phi/vis/_dash/dash_app.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_dash/dash_gui.py` & `phiflow-2.3.4/phi/vis/_dash/dash_gui.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_dash/info.py` & `phiflow-2.3.4/phi/vis/_dash/info.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_dash/log.py` & `phiflow-2.3.4/phi/vis/_dash/log.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_dash/model_controls.py` & `phiflow-2.3.4/phi/vis/_dash/model_controls.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_dash/player_controls.py` & `phiflow-2.3.4/phi/vis/_dash/player_controls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Union
+
 import dash_core_components as dcc
 import dash_html_components as html
 from dash.dependencies import Output, Input, State
 from dash.exceptions import PreventUpdate
 
 from .dash_app import DashApp
 from .._vis_base import display_name
@@ -76,15 +78,15 @@
             if n_clicks is not None:
                 app.model.run_action(action.name)
             raise PreventUpdate()
 
     return layout
 
 
-def parse_step_count(step_count, app, default: int or None = 1):
+def parse_step_count(step_count, app, default: Union[int, None] = 1):
     if step_count is None:
         return default
     try:
         step_count = step_count.strip()
         if step_count.startswith('*'):
             step_count = app.model.sequence_stride * int(step_count[1:].strip())
         else:
```

### Comparing `phiflow-2.3.3/phi/vis/_dash/viewer.py` & `phiflow-2.3.4/phi/vis/_dash/viewer.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_dash/viewsettings.py` & `phiflow-2.3.4/phi/vis/_dash/viewsettings.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_log.py` & `phiflow-2.3.4/phi/vis/_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import sys
 from os.path import isfile
+from typing import Union
 
 import numpy as np
 
 from phi import math
 from phi.field import Scene
 
 
@@ -39,15 +40,15 @@
             self.logger.addHandler(file_handler)
         else:
             self.log_file = None
 
     def log(self, message):
         self.logger.info(message)
 
-    def log_scalars(self, frame: int, **values: float or math.Tensor):
+    def log_scalars(self, frame: int, **values: Union[float, math.Tensor]):
         """
         Adds `values` to the curves by name.
         This can be used to log the evolution of scalar quantities or summaries.
 
         The values are stored in a text file within the scene directory.
         The curves may also be directly viewed in the user interface.
```

### Comparing `phiflow-2.3.3/phi/vis/_matplotlib/_matplotlib_plots.py` & `phiflow-2.3.4/phi/vis/_matplotlib/_matplotlib_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 import warnings
-from typing import Callable, Tuple, Any, Dict
+from typing import Callable, Tuple, Any, Dict, Union
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import animation
 from matplotlib import rc
 from matplotlib.patches import Patch
@@ -415,15 +415,15 @@
         # col = tuple(int(col.lstrip('#')[i:i+2], 16) for i in (0, 2, 4))
     col = np.asarray(col)
     if col.dtype.kind == 'i':
         col = col / 255.
     return col
 
 
-def matplotlib_colors(color: Tensor, dims: Shape, default=None) -> list or None:
+def matplotlib_colors(color: Tensor, dims: Shape, default=None) -> Union[list, None]:
     if color.rank == 0 and color.native() is None:
         if default is None:
             return None
         else:
             color = math.wrap(default)
     color = color[math.shape(color).without(dims).first_index()]  # Select first color along unlisted dimensions
     if color.dtype.kind == int:
```

### Comparing `phiflow-2.3.3/phi/vis/_matplotlib/_scalars.py` & `phiflow-2.3.4/phi/vis/_matplotlib/_scalars.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from numbers import Number
-from typing import Callable
+from typing import Callable, Union
 
 import matplotlib.pyplot as plt
 import numpy
 import numpy as np
 
 from phi import math
 from phi.field import Scene
@@ -12,25 +12,25 @@
 from phi.math import Tensor, batch
 from phi.math.backend import PHI_LOGGER
 from phi.vis._plot_util import smooth_uniform_curve
 from phi.vis._vis_base import display_name
 from ._matplotlib_plots import MATPLOTLIB
 
 
-def plot_scalars(scene: str or tuple or list or Scene or math.Tensor,
-                 names: str or tuple or list or math.Tensor = None,
-                 reduce: str or tuple or list or math.Shape = 'names',
+def plot_scalars(scene: Union[str, tuple, list, Scene, math.Tensor],
+                 names: Union[str, tuple, list, math.Tensor] = None,
+                 reduce: Union[str, tuple, list, math.Shape] = 'names',
                  down='',
                  smooth=1,
                  smooth_alpha=0.2,
                  smooth_linewidth=2.,
                  size=(8, 6),
                  transform: Callable = None,
                  tight_layout=True,
-                 grid: str or dict = 'y',
+                 grid: Union[str, dict] = 'y',
                  log_scale='',
                  legend='upper right',
                  x='steps',
                  xlim=None,
                  ylim=None,
                  titles=True,
                  labels: math.Tensor = None,
```

### Comparing `phiflow-2.3.3/phi/vis/_plot_util.py` & `phiflow-2.3.4/phi/vis/_plot_util.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_user_namespace.py` & `phiflow-2.3.4/phi/vis/_user_namespace.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.3.3/phi/vis/_viewer.py` & `phiflow-2.3.4/phi/vis/_viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import itertools
 import sys
 import time
 import warnings
 from functools import partial
 from threading import Event
-from typing import Tuple
+from typing import Tuple, Union
 
 from ._log import SceneLog
 from ._user_namespace import UserNamespace
 from ._vis_base import VisModel, Control, Action
 from .. import field
 from ..field import Scene, SampledField
 from ..math import batch, Tensor
 from ..math.backend import PHI_LOGGER
 
 
 def create_viewer(namespace: UserNamespace,
                   fields: dict,
                   name: str,
                   description: str,
-                  scene: Scene or None,
+                  scene: Union[Scene, None],
                   asynchronous: bool,
                   controls: tuple,
                   actions: dict,
                   log_performance: bool) -> 'Viewer':
     cls = AsyncViewer if asynchronous else Viewer
     viewer = cls(namespace, fields, name, description, scene, controls, actions, log_performance)
     return viewer
@@ -273,15 +273,15 @@
 
     def can_progress(self) -> bool:
         return True
 
 
 class Record:
 
-    def __init__(self, dim: str or None):
+    def __init__(self, dim: Union[str, None]):
         self.dim = dim
         self.history = {}
 
     def append(self, variables: dict, warn_missing=True):
         if not self.history:
             self.history = {name: [] for name in variables.keys()}
         for name, val in variables.items():
```

### Comparing `phiflow-2.3.3/phi/vis/_vis.py` & `phiflow-2.3.4/phi/vis/_vis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import inspect
 import os
 import sys
 import warnings
 from contextlib import contextmanager
 from threading import Thread
-from typing import Tuple, List, Dict
+from typing import Tuple, List, Dict, Union
 
 from ._user_namespace import get_user_namespace, UserNamespace, DictNamespace
 from ._viewer import create_viewer, Viewer
 from ._vis_base import Control, value_range, Action, VisModel, Gui, PlottingLibrary, tensor_as_field, common_index, index_label, title_label
 from .. import math
 from ..field import SampledField, Scene, Field, PointCloud
 from ..field._scene import _slugify_filename
 from ..geom import Geometry, Box, embed
 from ..math import Tensor, layout, batch, Shape, wrap, merge_shapes, EMPTY_SHAPE
 from ..math._shape import parse_dim_order, DimFilter
 
 
-def show(*model: VisModel or SampledField or tuple or list or Tensor or Geometry,
+def show(*model: Union[VisModel, SampledField, tuple, list, Tensor, Geometry],
          play=True,
-         gui: Gui or str = None,
-         lib: Gui or str = None,
+         gui: Union[Gui, str] = None,
+         lib: Union[Gui, str] = None,
          keep_alive=True,
          **config):
     """
     If `model` is a user interface model, launches the registered user interface.
     This will typically be the Dash web interface or the console interface if dash is not available.
     This method prepares the `model` before showing it. No more fields should be added to the vis after this method is invoked.
 
@@ -96,32 +96,32 @@
         plots.close(figure)
 
 
 
 RECORDINGS = {}
 
 
-def record(*fields: str or SampledField) -> Viewer:
+def record(*fields: Union[str, SampledField]) -> Viewer:
     user_namespace = get_user_namespace(1)
     variables = _default_field_variables(user_namespace, fields)
     viewer = create_viewer(user_namespace, variables, "record", "", scene=None, asynchronous=False, controls=(),
                            actions={}, log_performance=False)
     viewer.post_step.append(lambda viewer: print(viewer.steps, end=" "))
     viewer.progress_unavailable.append(lambda viewer: print())
     return viewer
 
 
-def view(*fields: str or SampledField,
+def view(*fields: Union[str, SampledField],
          play: bool = True,
          gui=None,
          name: str = None,
          description: str = None,
-         scene: bool or Scene = False,
+         scene: Union[bool, Scene] = False,
          keep_alive=True,
-         select: str or tuple or list = '',
+         select: Union[str, tuple, list] = '',
          framerate=None,
          namespace=None,
          log_performance=True,
          **config) -> Viewer:
     """
     Show `fields` in a graphical user interface.
 
@@ -262,27 +262,27 @@
     Returns the figure that was most recently created using `plot()`.
 
     The type of the figure depends on which library was used, e.g. `matplotlib.figure.Figure` or `plotly.graph_objs.Figure`.
     """
     return LAST_FIGURE[0]
 
 
-def plot(*fields: SampledField or Tensor,
-         lib: str or PlottingLibrary = None,
+def plot(*fields: Union[SampledField, Tensor, Geometry],
+         lib: Union[str, PlottingLibrary] = None,
          row_dims: DimFilter = None,
          col_dims: DimFilter = batch,
          animate: DimFilter = None,
          overlay: DimFilter = 'overlay',
-         title: str or Tensor = None,
+         title: Union[str, Tensor] = None,
          size=(12, 5),
          same_scale=True,
-         log_dims: str or tuple or list or Shape = '',
+         log_dims: Union[str, tuple, list, Shape] = '',
          show_color_bar=True,
-         color: str or int or Tensor = None,
-         alpha: float or Tensor = 1.,
+         color: Union[str, int, Tensor] = None,
+         alpha: Union[float, Tensor] = 1.,
          frame_time=100,
          repeat=True):
     """
     Creates one or multiple figures and sub-figures and plots the given fields.
 
     To show the figures, use `show()`.
 
@@ -385,24 +385,24 @@
     elif isinstance(data, list):
         return layout(data, batch('list'))
     elif isinstance(data, dict):
         return layout(data, batch('dict'))
     return wrap(data) if wrap_leaf else data
 
 
-def layout_sub_figures(data: Tensor or SampledField,
+def layout_sub_figures(data: Union[Tensor, SampledField],
                        row_dims: DimFilter,
                        col_dims: DimFilter,
                        animate: DimFilter,  # do not reduce these dims, has priority
                        overlay: DimFilter,
                        offset_row: int,
                        offset_col: int,
                        positioning: Dict[Tuple[int, int], List],
                        indices: Dict[Tuple[int, int], List[dict]],
-                       base_index: Dict[str, int or str]) -> Tuple[int, int, Shape, Shape]:  # rows, cols
+                       base_index: Dict[str, Union[int, str]]) -> Tuple[int, int, Shape, Shape]:  # rows, cols
     if data is None:
         raise ValueError(f"Cannot layout figure for '{data}'")
     data = layout_pytree_node(data)
     if isinstance(data, Tensor) and data.dtype.kind == object:  # layout
         rows, cols = 0, 0
         non_reduced = math.EMPTY_SHAPE
         dim0 = reduced = data.shape[0]
@@ -466,15 +466,15 @@
         return all_bounds[0]
     bounds: Box = math.stack(all_bounds, batch('_fields'))
     lower = math.finite_min(bounds.lower, '_fields', default=-math.INF)
     upper = math.finite_max(bounds.upper, '_fields', default=math.INF)
     return Box(lower, upper)
 
 
-def overlay(*fields: SampledField or Tensor) -> Tensor:
+def overlay(*fields: Union[SampledField, Tensor]) -> Tensor:
     """
     Specify that multiple fields should be drawn on top of one another in the same figure.
     The fields will be plotted in the order they are given, i.e. the last field on top.
 
     >>> plot(vis.overlay(heatmap, points, velocity))
 
     Args:
@@ -514,15 +514,15 @@
         try:
             return get_gui(option)
         except ImportError as import_error:
             warnings.warn(f"{option} user interface is unavailable because of missing dependency: {import_error}.", ImportWarning)
     raise RuntimeError("No user interface available.")
 
 
-def get_gui(gui: str or Gui) -> Gui:
+def get_gui(gui: Union[str, Gui]) -> Gui:
     if GUI_OVERRIDES:
         return GUI_OVERRIDES[-1]
     if isinstance(gui, str):
         if gui == 'dash':
             from ._dash.dash_gui import DashGui
             return DashGui()
         elif gui == 'console':
@@ -560,15 +560,15 @@
         try:
             return get_plots(option)
         except ImportError as import_error:
             warnings.warn(f"{option} user interface is unavailable because of missing dependency: {import_error}.", ImportWarning)
     raise RuntimeError("No user interface available.")
 
 
-def get_plots(lib: str or PlottingLibrary) -> PlottingLibrary:
+def get_plots(lib: Union[str, PlottingLibrary]) -> PlottingLibrary:
     if isinstance(lib, PlottingLibrary):
         return lib
     for loaded_lib in _LOADED_PLOTTING_LIBRARIES:
         if loaded_lib.name == lib:
             return loaded_lib
     if lib == 'matplotlib':
         from ._matplotlib._matplotlib_plots import MATPLOTLIB
```

### Comparing `phiflow-2.3.3/phi/vis/_vis_base.py` & `phiflow-2.3.4/phi/vis/_vis_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import threading
 import time
 from collections import namedtuple
 from math import log10
 from threading import Lock
-from typing import Tuple, Any, Optional, Dict, Callable
+from typing import Tuple, Any, Optional, Dict, Callable, Union
 
 from phi import field, math
 from phi.field import SampledField, Scene, PointCloud, CenteredGrid
 from phi.field._field_math import data_bounds
 from phi.geom import Box, Cuboid
 from phi.math import Shape, EMPTY_SHAPE, Tensor, spatial, instance, wrap, channel
 
@@ -217,15 +217,15 @@
     def __bool__(self):
         return not self._finished
 
     def __repr__(self):
         return status_message(self.model, self)
 
 
-def status_message(model: VisModel, play_status: AsyncPlay or None):
+def status_message(model: VisModel, play_status: Union[AsyncPlay, None]):
     pausing = "/Pausing" if (play_status and play_status.paused) else ""
     current_action = "Running" if model.is_progressing else "Waiting"
     action = current_action if play_status else "Idle"
     message = f" - {model.message}" if model.message else ""
     return f"{action}{pausing} ({model.steps} steps){message}"
 
 
@@ -318,15 +318,15 @@
         If no Gui is specified, `App.run()` is called instead.
         """
         raise NotImplementedError(self)
 
 
 class PlottingLibrary:
 
-    def __init__(self, name: str, figure_classes: tuple or list):
+    def __init__(self, name: str, figure_classes: Union[tuple, list]):
         self.name = name
         self.figure_classes = tuple(figure_classes)
         self.current_figure = None
         self.recipes = []
 
     def __repr__(self):
         return self.name
@@ -424,15 +424,15 @@
     text = "".join(n)
     if "Reset" in text:
         return f"⏮ {text}"
     else:
         return text
 
 
-def index_label(idx: dict) -> str or None:
+def index_label(idx: dict) -> Union[str, None]:
     if len(idx) == 0:
         return None
     elif len(idx) == 1:
         return display_name(next(iter(idx.values())))
     else:
         number_unlabelled_dims = len([1 for k, v in idx.items() if isinstance(v, int)])
         if number_unlabelled_dims <= 1:
@@ -456,15 +456,15 @@
 
 
 
 def common_index(*indices: dict, exclude=()):
     return {k: v for k, v in indices[0].items() if k not in exclude and all(i[k] == v for i in indices)}
 
 
-def select_channel(value: SampledField or Tensor or tuple or list, channel: str or None):
+def select_channel(value: Union[SampledField, Tensor, tuple, list], channel: Union[str, None]):
     if isinstance(value, (tuple, list)):
         return [select_channel(v, channel) for v in value]
     if channel is None:
         return value
     elif channel == 'abs':
         if value.vector.exists:
             return field.vec_abs(value) if isinstance(value, SampledField) else math.vec_length(value)
```

### Comparing `phiflow-2.3.3/phiflow.egg-info/PKG-INFO` & `phiflow-2.3.4/phiflow.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: phiflow
-Version: 2.3.3
-Summary: Differentiable PDE solving framework for machine learning
-Home-page: https://github.com/tum-pbs/PhiFlow
-Download-URL: https://github.com/tum-pbs/PhiFlow/archive/2.3.3.tar.gz
-Author: Philipp Holl
-Author-email: philipp.holl@tum.de
-License: MIT
-Keywords: Differentiable,Simulation,Fluid,Machine Learning,Deep Learning
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# PhiFlow
-
-[**Homepage**](https://github.com/tum-pbs/PhiFlow)
-&nbsp;&nbsp;&nbsp; [**Documentation**](https://tum-pbs.github.io/PhiFlow/)
-&nbsp;&nbsp;&nbsp; [**API**](https://tum-pbs.github.io/PhiFlow/phi)
-&nbsp;&nbsp;&nbsp; [**Demos**](https://github.com/tum-pbs/PhiFlow/tree/master/demos)
-&nbsp;&nbsp;&nbsp; [<img src="https://www.tensorflow.org/images/colab_logo_32px.png" height=16> **Fluids Tutorial**](https://colab.research.google.com/github/tum-pbs/PhiFlow/blob/develop/docs/Fluids_Tutorial.ipynb#offline=true&sandboxMode=true)
-&nbsp;&nbsp;&nbsp; [<img src="https://www.tensorflow.org/images/colab_logo_32px.png" height=16> **Playground**](https://colab.research.google.com/drive/1zBlQbmNguRt-Vt332YvdTqlV4DBcus2S#offline=true&sandboxMode=true)
-
-PhiFlow is an open-source simulation toolkit built for optimization and machine learning applications.
-It is written mostly in Python and can be used with NumPy, TensorFlow, Jax or PyTorch.
-The close integration with machine learning frameworks allows it to leverage their automatic differentiation functionality,
-making it easy to build end-to-end differentiable functions involving both learning models and physics simulations.
-
-See the [installation Instructions](https://tum-pbs.github.io/PhiFlow/Installation_Instructions.html) on how to compile the optional custom CUDA operations.
+Metadata-Version: 2.1
+Name: phiflow
+Version: 2.3.4
+Summary: Differentiable PDE solving framework for machine learning
+Home-page: https://github.com/tum-pbs/PhiFlow
+Author: Philipp Holl
+Author-email: philipp.holl@tum.de
+License: MIT
+Download-URL: https://github.com/tum-pbs/PhiFlow/archive/2.3.4.tar.gz
+Description: # PhiFlow
+        
+        [**Homepage**](https://github.com/tum-pbs/PhiFlow)
+        &nbsp;&nbsp;&nbsp; [**Documentation**](https://tum-pbs.github.io/PhiFlow/)
+        &nbsp;&nbsp;&nbsp; [**API**](https://tum-pbs.github.io/PhiFlow/phi)
+        &nbsp;&nbsp;&nbsp; [**Demos**](https://github.com/tum-pbs/PhiFlow/tree/master/demos)
+        &nbsp;&nbsp;&nbsp; [<img src="https://www.tensorflow.org/images/colab_logo_32px.png" height=16> **Fluids Tutorial**](https://colab.research.google.com/github/tum-pbs/PhiFlow/blob/develop/docs/Fluids_Tutorial.ipynb#offline=true&sandboxMode=true)
+        &nbsp;&nbsp;&nbsp; [<img src="https://www.tensorflow.org/images/colab_logo_32px.png" height=16> **Playground**](https://colab.research.google.com/drive/1zBlQbmNguRt-Vt332YvdTqlV4DBcus2S#offline=true&sandboxMode=true)
+        
+        PhiFlow is an open-source simulation toolkit built for optimization and machine learning applications.
+        It is written mostly in Python and can be used with NumPy, TensorFlow, Jax or PyTorch.
+        The close integration with machine learning frameworks allows it to leverage their automatic differentiation functionality,
+        making it easy to build end-to-end differentiable functions involving both learning models and physics simulations.
+        
+        See the [installation Instructions](https://tum-pbs.github.io/PhiFlow/Installation_Instructions.html) on how to compile the optional custom CUDA operations.
+        
+Keywords: Differentiable,Simulation,Fluid,Machine Learning,Deep Learning
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
```

### Comparing `phiflow-2.3.3/phiflow.egg-info/SOURCES.txt` & `phiflow-2.3.4/phiflow.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 phi/VERSION
 phi/__init__.py
 phi/_troubleshoot.py
 phi/flow.py
-phi/net.py
 phi/field/__init__.py
 phi/field/_angular_velocity.py
 phi/field/_embed.py
 phi/field/_field.py
 phi/field/_field_io.py
 phi/field/_field_math.py
 phi/field/_grid.py
@@ -60,15 +58,14 @@
 phi/tf/__init__.py
 phi/tf/_compile_cuda.py
 phi/tf/_profiling.py
 phi/tf/_tf_backend.py
 phi/tf/_tf_cuda_resample.py
 phi/tf/flow.py
 phi/tf/nets.py
-phi/tf/cuda/build/resample.cu.o
 phi/torch/__init__.py
 phi/torch/_torch_backend.py
 phi/torch/flow.py
 phi/torch/nets.py
 phi/vis/__init__.py
 phi/vis/_log.py
 phi/vis/_plot_util.py
```

### Comparing `phiflow-2.3.3/setup.py` & `phiflow-2.3.4/setup.py`

 * *Files identical despite different names*

