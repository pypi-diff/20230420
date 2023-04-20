# Comparing `tmp/pypop7-0.0.8.tar.gz` & `tmp/pypop7-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypop7-0.0.8.tar", last modified: Thu Jun 30 09:52:09 2022, max compression
+gzip compressed data, was "pypop7-0.0.9.tar", last modified: Sat Jul  2 11:01:35 2022, max compression
```

## Comparing `pypop7-0.0.8.tar` & `pypop7-0.0.9.tar`

### file list

```diff
@@ -1,162 +1,164 @@
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.618987 pypop7-0.0.8/
--rw-rw-rw-   0        0        0     1928 2021-01-26 19:36:05.000000 pypop7-0.0.8/.gitignore
--rw-rw-rw-   0        0        0    35823 2021-01-26 19:36:05.000000 pypop7-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    36126 2022-06-30 09:52:09.628986 pypop7-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    35458 2022-06-29 16:49:55.000000 pypop7-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.308985 pypop7-0.0.8/benchmarks/
--rw-rw-rw-   0        0        0    13006 2022-06-19 11:50:41.000000 pypop7-0.0.8/benchmarks/continuous_functions.py
--rw-rw-rw-   0        0        0     1169 2022-06-18 17:02:48.000000 pypop7-0.0.8/benchmarks/generate_rotation_matrices.py
--rw-rw-rw-   0        0        0      893 2022-06-18 17:02:48.000000 pypop7-0.0.8/benchmarks/generate_shift_vectors.py
--rw-rw-rw-   0        0        0    12748 2022-06-19 11:50:41.000000 pypop7-0.0.8/benchmarks/rotated_functions.py
--rw-rw-rw-   0        0        0    12229 2022-06-19 11:50:41.000000 pypop7-0.0.8/benchmarks/shifted_functions.py
--rw-rw-rw-   0        0        0     7675 2022-06-19 11:50:41.000000 pypop7-0.0.8/benchmarks/test_base_functions.py
--rw-rw-rw-   0        0        0    10426 2022-06-18 17:02:48.000000 pypop7-0.0.8/benchmarks/test_cases.py
--rw-rw-rw-   0        0        0     8836 2022-06-19 11:50:41.000000 pypop7-0.0.8/benchmarks/test_continuous_functions.py
--rw-rw-rw-   0        0        0     9129 2022-06-19 11:50:41.000000 pypop7-0.0.8/benchmarks/test_rotated_functions.py
--rw-rw-rw-   0        0        0     9184 2022-06-19 11:50:41.000000 pypop7-0.0.8/benchmarks/test_shifted_functions.py
--rw-rw-rw-   0        0        0      678 2022-06-19 11:50:41.000000 pypop7-0.0.8/benchmarks/test_utils.py
--rw-rw-rw-   0        0        0     1051 2022-06-18 17:02:48.000000 pypop7-0.0.8/benchmarks/utils.py
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.268994 pypop7-0.0.8/docs/
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.328987 pypop7-0.0.8/docs/demo/
--rw-rw-rw-   0        0        0   129142 2022-06-18 13:12:57.000000 pypop7-0.0.8/docs/demo/demo.gif
--rw-rw-rw-   0        0        0     2764 2022-06-18 13:09:39.000000 pypop7-0.0.8/docs/demo/demo.py
--rw-rw-rw-   0        0        0    31206 2022-06-28 13:37:15.000000 pypop7-0.0.8/docs/demo/demo_cem.gif
--rw-rw-rw-   0        0        0     3018 2022-06-28 13:37:15.000000 pypop7-0.0.8/docs/demo/demo_cem.py
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.328987 pypop7-0.0.8/docs/logo/
--rw-rw-rw-   0        0        0   247900 2021-10-09 19:39:00.000000 pypop7-0.0.8/docs/logo/PyPop-Logo-Small-0.png
--rw-rw-rw-   0        0        0   316805 2021-10-09 19:39:00.000000 pypop7-0.0.8/docs/logo/PyPop-Logo-Small.png
--rw-rw-rw-   0        0        0       10 2021-10-09 19:39:00.000000 pypop7-0.0.8/docs/logo/README.md
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.268994 pypop7-0.0.8/optimizers/
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.348984 pypop7-0.0.8/optimizers/es/
--rw-rw-rw-   0        0        0     2565 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/es/repeat_maes.py
--rw-rw-rw-   0        0        0     1727 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/es/repeat_mmes.py
--rw-rw-rw-   0        0        0     4308 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/es/repeat_r1es.py
--rw-rw-rw-   0        0        0     1568 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/es/repeat_rmes.py
--rw-rw-rw-   0        0        0     2663 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/es/repeat_rmes2.py
--rw-rw-rw-   0        0        0     2593 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/es/saes.py
--rw-rw-rw-   0        0        0     1328 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/es/test_saes.py
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.358992 pypop7-0.0.8/optimizers/nes/
--rw-rw-rw-   0        0        0     1179 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/nes/nes.py
--rw-rw-rw-   0        0        0     5050 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/nes/r1nes.py
--rw-rw-rw-   0        0        0     3420 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/nes/repeat_figure_1_jmlr_2014_nes.py
--rw-rw-rw-   0        0        0     3499 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/nes/snes.py
--rw-rw-rw-   0        0        0     1287 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/nes/test_r1nes.py
--rw-rw-rw-   0        0        0     1284 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/nes/test_snes.py
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.388985 pypop7-0.0.8/optimizers/pso/
--rw-rw-rw-   0        0        0     4153 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/pso/clpso.py
--rw-rw-rw-   0        0        0     2459 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/pso/opso.py
--rw-rw-rw-   0        0        0      811 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/pso/opsogt.py
--rw-rw-rw-   0        0        0      804 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/pso/opsort.py
--rw-rw-rw-   0        0        0     5035 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/pso/pso.py
--rw-rw-rw-   0        0        0      863 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/pso/psogt.py
--rw-rw-rw-   0        0        0     1145 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/pso/psort.py
--rw-rw-rw-   0        0        0     1331 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/pso/test_clpso.py
--rw-rw-rw-   0        0        0     1337 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/pso/test_opsogt.py
--rw-rw-rw-   0        0        0     1337 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/pso/test_opsort.py
--rw-rw-rw-   0        0        0     1331 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/pso/test_psogt.py
--rw-rw-rw-   0        0        0     1331 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/pso/test_psort.py
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.408986 pypop7-0.0.8/optimizers/rs/
--rw-rw-rw-   0        0        0     1255 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/rs/arhc.py
--rw-rw-rw-   0        0        0     1574 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/rs/prs.py
--rw-rw-rw-   0        0        0     1570 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/rs/rhc.py
--rw-rw-rw-   0        0        0     1826 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/rs/rs.py
--rw-rw-rw-   0        0        0     1285 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/rs/test_arhc.py
--rw-rw-rw-   0        0        0     2398 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/rs/test_prs.py
--rw-rw-rw-   0        0        0     1325 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/rs/test_rhc.py
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.418986 pypop7-0.0.8/optimizers/sa/
--rw-rw-rw-   0        0        0     4425 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/sa/csa.py
--rw-rw-rw-   0        0        0     5303 2022-06-18 17:02:48.000000 pypop7-0.0.8/optimizers/sa/esa.py
--rw-rw-rw-   0        0        0     1337 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/sa/test_csa.py
--rw-rw-rw-   0        0        0     1337 2022-06-19 11:50:41.000000 pypop7-0.0.8/optimizers/sa/test_esa.py
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.418986 pypop7-0.0.8/pypop7/
--rw-rw-rw-   0        0        0        0 2022-05-25 12:25:05.000000 pypop7-0.0.8/pypop7/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.438986 pypop7-0.0.8/pypop7/benchmarks/
--rw-rw-rw-   0        0        0        0 2021-01-26 19:41:00.000000 pypop7-0.0.8/pypop7/benchmarks/__init__.py
--rw-rw-rw-   0        0        0     6928 2022-06-19 11:52:10.000000 pypop7-0.0.8/pypop7/benchmarks/base_functions.py
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.278986 pypop7-0.0.8/pypop7/optimizers/
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.578986 pypop7-0.0.8/pypop7/optimizers/cem/
--rw-rw-rw-   0        0        0        0 2022-06-15 12:28:53.000000 pypop7-0.0.8/pypop7/optimizers/cem/__init__.py
--rw-rw-rw-   0        0        0     2371 2022-06-28 13:37:15.000000 pypop7-0.0.8/pypop7/optimizers/cem/cem.py
--rw-rw-rw-   0        0        0     2207 2022-06-28 13:37:15.000000 pypop7-0.0.8/pypop7/optimizers/cem/dcem.py
--rw-rw-rw-   0        0        0     2128 2022-06-28 13:37:15.000000 pypop7-0.0.8/pypop7/optimizers/cem/scem.py
--rw-rw-rw-   0        0        0     3645 2022-06-28 13:37:15.000000 pypop7-0.0.8/pypop7/optimizers/cem/secem.py
--rw-rw-rw-   0        0        0     1460 2022-06-28 13:37:15.000000 pypop7-0.0.8/pypop7/optimizers/cem/test_dcem.py
--rw-rw-rw-   0        0        0     1401 2022-06-28 13:37:15.000000 pypop7-0.0.8/pypop7/optimizers/cem/test_scem.py
--rw-rw-rw-   0        0        0     1477 2022-06-20 10:22:21.000000 pypop7-0.0.8/pypop7/optimizers/cem/test_secem.py
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.438986 pypop7-0.0.8/pypop7/optimizers/core/
--rw-rw-rw-   0        0        0        0 2021-03-18 13:24:53.000000 pypop7-0.0.8/pypop7/optimizers/core/__init__.py
--rw-rw-rw-   0        0        0     6358 2022-05-27 12:54:16.000000 pypop7-0.0.8/pypop7/optimizers/core/optimizer.py
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.598987 pypop7-0.0.8/pypop7/optimizers/ds/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:21:28.000000 pypop7-0.0.8/pypop7/optimizers/ds/__init__.py
--rw-rw-rw-   0        0        0     1699 2022-06-27 13:41:02.000000 pypop7-0.0.8/pypop7/optimizers/ds/dsm.py
--rw-rw-rw-   0        0        0     2033 2022-06-27 13:41:02.000000 pypop7-0.0.8/pypop7/optimizers/ds/hjdsm.py
--rw-rw-rw-   0        0        0     1786 2022-06-27 13:41:02.000000 pypop7-0.0.8/pypop7/optimizers/ds/srs.py
--rw-rw-rw-   0        0        0     1436 2022-06-22 11:07:31.000000 pypop7-0.0.8/pypop7/optimizers/ds/test_hjdsm.py
--rw-rw-rw-   0        0        0     1558 2022-06-27 13:41:02.000000 pypop7-0.0.8/pypop7/optimizers/ds/test_srs.py
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.568990 pypop7-0.0.8/pypop7/optimizers/es/
--rw-rw-rw-   0        0        0        0 2022-05-25 10:49:17.000000 pypop7-0.0.8/pypop7/optimizers/es/__init__.py
--rw-rw-rw-   0        0        0     4371 2022-06-15 09:23:57.000000 pypop7-0.0.8/pypop7/optimizers/es/ccmaes.py
--rw-rw-rw-   0        0        0     4766 2022-05-28 07:45:43.000000 pypop7-0.0.8/pypop7/optimizers/es/csaes.py
--rw-rw-rw-   0        0        0     4383 2022-05-28 13:22:12.000000 pypop7-0.0.8/pypop7/optimizers/es/dsaes.py
--rw-rw-rw-   0        0        0     5562 2022-05-28 07:44:37.000000 pypop7-0.0.8/pypop7/optimizers/es/es.py
--rw-rw-rw-   0        0        0     1238 2022-06-05 17:51:41.000000 pypop7-0.0.8/pypop7/optimizers/es/fmaes.py
--rw-rw-rw-   0        0        0     5108 2022-05-30 05:44:25.000000 pypop7-0.0.8/pypop7/optimizers/es/lmmaes.py
--rw-rw-rw-   0        0        0     6478 2022-05-28 08:22:30.000000 pypop7-0.0.8/pypop7/optimizers/es/maes.py
--rw-rw-rw-   0        0        0     6136 2022-05-30 06:55:35.000000 pypop7-0.0.8/pypop7/optimizers/es/mmes.py
--rw-rw-rw-   0        0        0     4412 2022-06-08 10:29:14.000000 pypop7-0.0.8/pypop7/optimizers/es/mvaes.py
--rw-rw-rw-   0        0        0     3957 2022-06-27 11:12:01.000000 pypop7-0.0.8/pypop7/optimizers/es/opoa.py
--rw-rw-rw-   0        0        0     5800 2022-06-29 22:23:40.000000 pypop7-0.0.8/pypop7/optimizers/es/opoa2015.py
--rw-rw-rw-   0        0        0     4188 2022-06-28 06:59:27.000000 pypop7-0.0.8/pypop7/optimizers/es/opoc.py
--rw-rw-rw-   0        0        0     4166 2022-06-14 07:18:06.000000 pypop7-0.0.8/pypop7/optimizers/es/opoc2009.py
--rw-rw-rw-   0        0        0     4778 2022-06-01 08:51:33.000000 pypop7-0.0.8/pypop7/optimizers/es/r1es.py
--rw-rw-rw-   0        0        0     3106 2022-06-19 12:05:13.000000 pypop7-0.0.8/pypop7/optimizers/es/repeat_ccmaes.py
--rw-rw-rw-   0        0        0     3392 2022-06-10 02:49:31.000000 pypop7-0.0.8/pypop7/optimizers/es/repeat_lmmaes.py
--rw-rw-rw-   0        0        0     4465 2022-05-31 08:15:21.000000 pypop7-0.0.8/pypop7/optimizers/es/repeat_maes.py
--rw-rw-rw-   0        0        0     3008 2022-05-31 05:43:11.000000 pypop7-0.0.8/pypop7/optimizers/es/repeat_mmes.py
--rw-rw-rw-   0        0        0     2918 2022-05-28 07:19:23.000000 pypop7-0.0.8/pypop7/optimizers/es/repeat_mvaes.py
--rw-rw-rw-   0        0        0     3829 2022-06-28 13:37:15.000000 pypop7-0.0.8/pypop7/optimizers/es/repeat_opoa_fig1.py
--rw-rw-rw-   0        0        0     2930 2022-06-30 09:47:26.000000 pypop7-0.0.8/pypop7/optimizers/es/repeat_opoa_fig2.py
--rw-rw-rw-   0        0        0     4331 2022-06-19 12:49:54.000000 pypop7-0.0.8/pypop7/optimizers/es/repeat_opoc.py
--rw-rw-rw-   0        0        0     3897 2022-06-15 12:08:59.000000 pypop7-0.0.8/pypop7/optimizers/es/repeat_opoc2009.py
--rw-rw-rw-   0        0        0     5281 2022-06-05 14:54:57.000000 pypop7-0.0.8/pypop7/optimizers/es/repeat_r1es.py
--rw-rw-rw-   0        0        0     2552 2022-06-06 10:55:27.000000 pypop7-0.0.8/pypop7/optimizers/es/repeat_rmes.py
--rw-rw-rw-   0        0        0     2555 2022-06-05 16:31:49.000000 pypop7-0.0.8/pypop7/optimizers/es/repeat_rmes2.py
--rw-rw-rw-   0        0        0     3272 2022-06-09 11:01:39.000000 pypop7-0.0.8/pypop7/optimizers/es/repeat_sepcmaes.py
--rw-rw-rw-   0        0        0     4005 2022-06-10 03:25:11.000000 pypop7-0.0.8/pypop7/optimizers/es/repeat_vdcma.py
--rw-rw-rw-   0        0        0     2931 2022-05-30 06:55:35.000000 pypop7-0.0.8/pypop7/optimizers/es/res.py
--rw-rw-rw-   0        0        0     4288 2022-06-07 07:40:06.000000 pypop7-0.0.8/pypop7/optimizers/es/rmes.py
--rw-rw-rw-   0        0        0     4203 2022-06-05 17:58:28.000000 pypop7-0.0.8/pypop7/optimizers/es/rmes2.py
--rw-rw-rw-   0        0        0     5690 2022-06-09 10:09:07.000000 pypop7-0.0.8/pypop7/optimizers/es/sepcmaes.py
--rw-rw-rw-   0        0        0     3170 2022-06-10 02:49:39.000000 pypop7-0.0.8/pypop7/optimizers/es/ssaes.py
--rw-rw-rw-   0        0        0     1750 2022-06-15 12:09:01.000000 pypop7-0.0.8/pypop7/optimizers/es/test_ccmaes.py
--rw-rw-rw-   0        0        0     1692 2022-05-28 07:46:55.000000 pypop7-0.0.8/pypop7/optimizers/es/test_csaes.py
--rw-rw-rw-   0        0        0     1692 2022-05-26 07:56:38.000000 pypop7-0.0.8/pypop7/optimizers/es/test_dsaes.py
--rw-rw-rw-   0        0        0     1394 2022-06-11 15:13:22.000000 pypop7-0.0.8/pypop7/optimizers/es/test_fmaes.py
--rw-rw-rw-   0        0        0     1750 2022-05-26 08:59:04.000000 pypop7-0.0.8/pypop7/optimizers/es/test_lmmaes.py
--rw-rw-rw-   0        0        0     1744 2022-05-28 13:17:13.000000 pypop7-0.0.8/pypop7/optimizers/es/test_maes.py
--rw-rw-rw-   0        0        0     1391 2022-06-10 02:49:40.000000 pypop7-0.0.8/pypop7/optimizers/es/test_mmes.py
--rw-rw-rw-   0        0        0     1787 2022-05-28 04:09:16.000000 pypop7-0.0.8/pypop7/optimizers/es/test_mvaes.py
--rw-rw-rw-   0        0        0     1746 2022-06-27 11:18:31.000000 pypop7-0.0.8/pypop7/optimizers/es/test_opoa.py
--rw-rw-rw-   0        0        0     1758 2022-06-29 22:26:34.000000 pypop7-0.0.8/pypop7/optimizers/es/test_opoa2015.py
--rw-rw-rw-   0        0        0     1746 2022-06-13 10:32:47.000000 pypop7-0.0.8/pypop7/optimizers/es/test_opoc.py
--rw-rw-rw-   0        0        0     1758 2022-06-13 15:10:32.000000 pypop7-0.0.8/pypop7/optimizers/es/test_opoc2009.py
--rw-rw-rw-   0        0        0     1688 2022-05-31 07:54:08.000000 pypop7-0.0.8/pypop7/optimizers/es/test_r1es.py
--rw-rw-rw-   0        0        0     1687 2022-05-26 07:01:48.000000 pypop7-0.0.8/pypop7/optimizers/es/test_res.py
--rw-rw-rw-   0        0        0     1688 2022-06-16 07:17:15.000000 pypop7-0.0.8/pypop7/optimizers/es/test_rmes.py
--rw-rw-rw-   0        0        0     1756 2022-06-08 11:00:02.000000 pypop7-0.0.8/pypop7/optimizers/es/test_sepcmaes.py
--rw-rw-rw-   0        0        0     1690 2022-06-10 02:49:39.000000 pypop7-0.0.8/pypop7/optimizers/es/test_ssaes.py
--rw-rw-rw-   0        0        0     1747 2022-06-02 16:48:17.000000 pypop7-0.0.8/pypop7/optimizers/es/test_vdcma.py
--rw-rw-rw-   0        0        0     8021 2022-06-02 17:14:38.000000 pypop7-0.0.8/pypop7/optimizers/es/vdcma.py
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.618987 pypop7-0.0.8/pypop7/optimizers/ga/
--rw-rw-rw-   0        0        0        0 2022-06-22 11:06:26.000000 pypop7-0.0.8/pypop7/optimizers/ga/__init__.py
--rw-rw-rw-   0        0        0     2973 2022-06-27 13:41:02.000000 pypop7-0.0.8/pypop7/optimizers/ga/ga.py
--rw-rw-rw-   0        0        0     2635 2022-06-27 13:41:02.000000 pypop7-0.0.8/pypop7/optimizers/ga/genitor.py
--rw-rw-rw-   0        0        0     1362 2022-06-27 13:41:02.000000 pypop7-0.0.8/pypop7/optimizers/ga/test_gentitor.py
-drwxrwxrwx   0        0        0        0 2022-06-30 09:52:09.438986 pypop7-0.0.8/pypop7.egg-info/
--rw-rw-rw-   0        0        0    36126 2022-06-30 09:52:08.000000 pypop7-0.0.8/pypop7.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6128 2022-06-30 09:52:09.000000 pypop7-0.0.8/pypop7.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-30 09:52:08.000000 pypop7-0.0.8/pypop7.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2022-06-30 09:52:08.000000 pypop7-0.0.8/pypop7.egg-info/requires.txt
--rw-rw-rw-   0        0        0       62 2022-06-30 09:52:08.000000 pypop7-0.0.8/pypop7.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      102 2022-06-18 17:03:15.000000 pypop7-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      901 2022-06-30 09:52:09.628986 pypop7-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:35.151208 pypop7-0.0.9/
+-rw-rw-rw-   0        0        0     1928 2021-01-26 19:36:05.000000 pypop7-0.0.9/.gitignore
+-rw-rw-rw-   0        0        0    35823 2021-01-26 19:36:05.000000 pypop7-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    36501 2022-07-02 11:01:35.151208 pypop7-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    35833 2022-07-02 10:53:34.000000 pypop7-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.761222 pypop7-0.0.9/benchmarks/
+-rw-rw-rw-   0        0        0    13006 2022-06-19 11:50:41.000000 pypop7-0.0.9/benchmarks/continuous_functions.py
+-rw-rw-rw-   0        0        0     1169 2022-06-18 17:02:48.000000 pypop7-0.0.9/benchmarks/generate_rotation_matrices.py
+-rw-rw-rw-   0        0        0      893 2022-06-18 17:02:48.000000 pypop7-0.0.9/benchmarks/generate_shift_vectors.py
+-rw-rw-rw-   0        0        0    12748 2022-06-19 11:50:41.000000 pypop7-0.0.9/benchmarks/rotated_functions.py
+-rw-rw-rw-   0        0        0    12229 2022-06-19 11:50:41.000000 pypop7-0.0.9/benchmarks/shifted_functions.py
+-rw-rw-rw-   0        0        0     7675 2022-06-19 11:50:41.000000 pypop7-0.0.9/benchmarks/test_base_functions.py
+-rw-rw-rw-   0        0        0    10426 2022-06-18 17:02:48.000000 pypop7-0.0.9/benchmarks/test_cases.py
+-rw-rw-rw-   0        0        0     8836 2022-06-19 11:50:41.000000 pypop7-0.0.9/benchmarks/test_continuous_functions.py
+-rw-rw-rw-   0        0        0     9129 2022-06-19 11:50:41.000000 pypop7-0.0.9/benchmarks/test_rotated_functions.py
+-rw-rw-rw-   0        0        0     9184 2022-06-19 11:50:41.000000 pypop7-0.0.9/benchmarks/test_shifted_functions.py
+-rw-rw-rw-   0        0        0      678 2022-06-19 11:50:41.000000 pypop7-0.0.9/benchmarks/test_utils.py
+-rw-rw-rw-   0        0        0     1051 2022-06-18 17:02:48.000000 pypop7-0.0.9/benchmarks/utils.py
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.701210 pypop7-0.0.9/docs/
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.771209 pypop7-0.0.9/docs/demo/
+-rw-rw-rw-   0        0        0   129142 2022-06-18 13:12:57.000000 pypop7-0.0.9/docs/demo/demo.gif
+-rw-rw-rw-   0        0        0     2764 2022-06-18 13:09:39.000000 pypop7-0.0.9/docs/demo/demo.py
+-rw-rw-rw-   0        0        0    31206 2022-06-28 13:37:15.000000 pypop7-0.0.9/docs/demo/demo_cem.gif
+-rw-rw-rw-   0        0        0     3018 2022-06-28 13:37:15.000000 pypop7-0.0.9/docs/demo/demo_cem.py
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.781210 pypop7-0.0.9/docs/logo/
+-rw-rw-rw-   0        0        0   247900 2021-10-09 19:39:00.000000 pypop7-0.0.9/docs/logo/PyPop-Logo-Small-0.png
+-rw-rw-rw-   0        0        0   316805 2021-10-09 19:39:00.000000 pypop7-0.0.9/docs/logo/PyPop-Logo-Small.png
+-rw-rw-rw-   0        0        0       10 2021-10-09 19:39:00.000000 pypop7-0.0.9/docs/logo/README.md
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.701210 pypop7-0.0.9/optimizers/
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.801209 pypop7-0.0.9/optimizers/es/
+-rw-rw-rw-   0        0        0     2565 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/es/repeat_maes.py
+-rw-rw-rw-   0        0        0     1727 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/es/repeat_mmes.py
+-rw-rw-rw-   0        0        0     4308 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/es/repeat_r1es.py
+-rw-rw-rw-   0        0        0     1568 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/es/repeat_rmes.py
+-rw-rw-rw-   0        0        0     2663 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/es/repeat_rmes2.py
+-rw-rw-rw-   0        0        0     2593 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/es/saes.py
+-rw-rw-rw-   0        0        0     1328 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/es/test_saes.py
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.821208 pypop7-0.0.9/optimizers/nes/
+-rw-rw-rw-   0        0        0     1179 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/nes/nes.py
+-rw-rw-rw-   0        0        0     5050 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/nes/r1nes.py
+-rw-rw-rw-   0        0        0     3420 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/nes/repeat_figure_1_jmlr_2014_nes.py
+-rw-rw-rw-   0        0        0     3499 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/nes/snes.py
+-rw-rw-rw-   0        0        0     1287 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/nes/test_r1nes.py
+-rw-rw-rw-   0        0        0     1284 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/nes/test_snes.py
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.851209 pypop7-0.0.9/optimizers/pso/
+-rw-rw-rw-   0        0        0     4153 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/pso/clpso.py
+-rw-rw-rw-   0        0        0     2459 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/pso/opso.py
+-rw-rw-rw-   0        0        0      811 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/pso/opsogt.py
+-rw-rw-rw-   0        0        0      804 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/pso/opsort.py
+-rw-rw-rw-   0        0        0     5035 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/pso/pso.py
+-rw-rw-rw-   0        0        0      863 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/pso/psogt.py
+-rw-rw-rw-   0        0        0     1145 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/pso/psort.py
+-rw-rw-rw-   0        0        0     1331 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/pso/test_clpso.py
+-rw-rw-rw-   0        0        0     1337 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/pso/test_opsogt.py
+-rw-rw-rw-   0        0        0     1337 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/pso/test_opsort.py
+-rw-rw-rw-   0        0        0     1331 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/pso/test_psogt.py
+-rw-rw-rw-   0        0        0     1331 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/pso/test_psort.py
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.871209 pypop7-0.0.9/optimizers/rs/
+-rw-rw-rw-   0        0        0     1255 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/rs/arhc.py
+-rw-rw-rw-   0        0        0     1574 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/rs/prs.py
+-rw-rw-rw-   0        0        0     1570 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/rs/rhc.py
+-rw-rw-rw-   0        0        0     1826 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/rs/rs.py
+-rw-rw-rw-   0        0        0     1285 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/rs/test_arhc.py
+-rw-rw-rw-   0        0        0     2398 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/rs/test_prs.py
+-rw-rw-rw-   0        0        0     1325 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/rs/test_rhc.py
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.901210 pypop7-0.0.9/optimizers/sa/
+-rw-rw-rw-   0        0        0     4425 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/sa/csa.py
+-rw-rw-rw-   0        0        0     5303 2022-06-18 17:02:48.000000 pypop7-0.0.9/optimizers/sa/esa.py
+-rw-rw-rw-   0        0        0     1337 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/sa/test_csa.py
+-rw-rw-rw-   0        0        0     1337 2022-06-19 11:50:41.000000 pypop7-0.0.9/optimizers/sa/test_esa.py
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.901210 pypop7-0.0.9/pypop7/
+-rw-rw-rw-   0        0        0        0 2022-05-25 12:25:05.000000 pypop7-0.0.9/pypop7/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.911208 pypop7-0.0.9/pypop7/benchmarks/
+-rw-rw-rw-   0        0        0        0 2021-01-26 19:41:00.000000 pypop7-0.0.9/pypop7/benchmarks/__init__.py
+-rw-rw-rw-   0        0        0     6928 2022-06-19 11:52:10.000000 pypop7-0.0.9/pypop7/benchmarks/base_functions.py
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.711221 pypop7-0.0.9/pypop7/optimizers/
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:35.091209 pypop7-0.0.9/pypop7/optimizers/cem/
+-rw-rw-rw-   0        0        0        0 2022-06-15 12:28:53.000000 pypop7-0.0.9/pypop7/optimizers/cem/__init__.py
+-rw-rw-rw-   0        0        0     2371 2022-06-28 13:37:15.000000 pypop7-0.0.9/pypop7/optimizers/cem/cem.py
+-rw-rw-rw-   0        0        0     2207 2022-06-28 13:37:15.000000 pypop7-0.0.9/pypop7/optimizers/cem/dcem.py
+-rw-rw-rw-   0        0        0     2128 2022-06-28 13:37:15.000000 pypop7-0.0.9/pypop7/optimizers/cem/scem.py
+-rw-rw-rw-   0        0        0     3645 2022-06-28 13:37:15.000000 pypop7-0.0.9/pypop7/optimizers/cem/secem.py
+-rw-rw-rw-   0        0        0     1460 2022-06-28 13:37:15.000000 pypop7-0.0.9/pypop7/optimizers/cem/test_dcem.py
+-rw-rw-rw-   0        0        0     1401 2022-06-28 13:37:15.000000 pypop7-0.0.9/pypop7/optimizers/cem/test_scem.py
+-rw-rw-rw-   0        0        0     1477 2022-06-20 10:22:21.000000 pypop7-0.0.9/pypop7/optimizers/cem/test_secem.py
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.921208 pypop7-0.0.9/pypop7/optimizers/core/
+-rw-rw-rw-   0        0        0        0 2021-03-18 13:24:53.000000 pypop7-0.0.9/pypop7/optimizers/core/__init__.py
+-rw-rw-rw-   0        0        0     6358 2022-05-27 12:54:16.000000 pypop7-0.0.9/pypop7/optimizers/core/optimizer.py
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:35.121209 pypop7-0.0.9/pypop7/optimizers/ds/
+-rw-rw-rw-   0        0        0        0 2022-06-20 10:21:28.000000 pypop7-0.0.9/pypop7/optimizers/ds/__init__.py
+-rw-rw-rw-   0        0        0     1699 2022-06-27 13:41:02.000000 pypop7-0.0.9/pypop7/optimizers/ds/dsm.py
+-rw-rw-rw-   0        0        0     2033 2022-06-27 13:41:02.000000 pypop7-0.0.9/pypop7/optimizers/ds/hjdsm.py
+-rw-rw-rw-   0        0        0     1786 2022-06-27 13:41:02.000000 pypop7-0.0.9/pypop7/optimizers/ds/srs.py
+-rw-rw-rw-   0        0        0     1436 2022-06-22 11:07:31.000000 pypop7-0.0.9/pypop7/optimizers/ds/test_hjdsm.py
+-rw-rw-rw-   0        0        0     1558 2022-06-27 13:41:02.000000 pypop7-0.0.9/pypop7/optimizers/ds/test_srs.py
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:35.071208 pypop7-0.0.9/pypop7/optimizers/es/
+-rw-rw-rw-   0        0        0        0 2022-05-25 10:49:17.000000 pypop7-0.0.9/pypop7/optimizers/es/__init__.py
+-rw-rw-rw-   0        0        0     4371 2022-06-15 09:23:57.000000 pypop7-0.0.9/pypop7/optimizers/es/ccmaes.py
+-rw-rw-rw-   0        0        0     3687 2022-07-01 20:02:40.000000 pypop7-0.0.9/pypop7/optimizers/es/ccmaes2016.py
+-rw-rw-rw-   0        0        0     4766 2022-05-28 07:45:43.000000 pypop7-0.0.9/pypop7/optimizers/es/csaes.py
+-rw-rw-rw-   0        0        0     4383 2022-05-28 13:22:12.000000 pypop7-0.0.9/pypop7/optimizers/es/dsaes.py
+-rw-rw-rw-   0        0        0     5562 2022-05-28 07:44:37.000000 pypop7-0.0.9/pypop7/optimizers/es/es.py
+-rw-rw-rw-   0        0        0     1238 2022-06-05 17:51:41.000000 pypop7-0.0.9/pypop7/optimizers/es/fmaes.py
+-rw-rw-rw-   0        0        0     5108 2022-05-30 05:44:25.000000 pypop7-0.0.9/pypop7/optimizers/es/lmmaes.py
+-rw-rw-rw-   0        0        0     6478 2022-05-28 08:22:30.000000 pypop7-0.0.9/pypop7/optimizers/es/maes.py
+-rw-rw-rw-   0        0        0     6136 2022-05-30 06:55:35.000000 pypop7-0.0.9/pypop7/optimizers/es/mmes.py
+-rw-rw-rw-   0        0        0     4412 2022-06-08 10:29:14.000000 pypop7-0.0.9/pypop7/optimizers/es/mvaes.py
+-rw-rw-rw-   0        0        0     3957 2022-06-27 11:12:01.000000 pypop7-0.0.9/pypop7/optimizers/es/opoa.py
+-rw-rw-rw-   0        0        0     5777 2022-07-01 20:26:58.000000 pypop7-0.0.9/pypop7/optimizers/es/opoa2015.py
+-rw-rw-rw-   0        0        0     4188 2022-06-28 06:59:27.000000 pypop7-0.0.9/pypop7/optimizers/es/opoc.py
+-rw-rw-rw-   0        0        0     4166 2022-06-14 07:18:06.000000 pypop7-0.0.9/pypop7/optimizers/es/opoc2009.py
+-rw-rw-rw-   0        0        0     4778 2022-06-01 08:51:33.000000 pypop7-0.0.9/pypop7/optimizers/es/r1es.py
+-rw-rw-rw-   0        0        0     3106 2022-06-19 12:05:13.000000 pypop7-0.0.9/pypop7/optimizers/es/repeat_ccmaes.py
+-rw-rw-rw-   0        0        0     3392 2022-06-10 02:49:31.000000 pypop7-0.0.9/pypop7/optimizers/es/repeat_lmmaes.py
+-rw-rw-rw-   0        0        0     4465 2022-05-31 08:15:21.000000 pypop7-0.0.9/pypop7/optimizers/es/repeat_maes.py
+-rw-rw-rw-   0        0        0     3008 2022-05-31 05:43:11.000000 pypop7-0.0.9/pypop7/optimizers/es/repeat_mmes.py
+-rw-rw-rw-   0        0        0     2918 2022-05-28 07:19:23.000000 pypop7-0.0.9/pypop7/optimizers/es/repeat_mvaes.py
+-rw-rw-rw-   0        0        0     3829 2022-06-28 13:37:15.000000 pypop7-0.0.9/pypop7/optimizers/es/repeat_opoa_fig1.py
+-rw-rw-rw-   0        0        0     2930 2022-06-30 09:47:26.000000 pypop7-0.0.9/pypop7/optimizers/es/repeat_opoa_fig2.py
+-rw-rw-rw-   0        0        0     4331 2022-06-19 12:49:54.000000 pypop7-0.0.9/pypop7/optimizers/es/repeat_opoc.py
+-rw-rw-rw-   0        0        0     3897 2022-06-15 12:08:59.000000 pypop7-0.0.9/pypop7/optimizers/es/repeat_opoc2009.py
+-rw-rw-rw-   0        0        0     5281 2022-06-05 14:54:57.000000 pypop7-0.0.9/pypop7/optimizers/es/repeat_r1es.py
+-rw-rw-rw-   0        0        0     2552 2022-06-06 10:55:27.000000 pypop7-0.0.9/pypop7/optimizers/es/repeat_rmes.py
+-rw-rw-rw-   0        0        0     2555 2022-06-05 16:31:49.000000 pypop7-0.0.9/pypop7/optimizers/es/repeat_rmes2.py
+-rw-rw-rw-   0        0        0     3272 2022-06-09 11:01:39.000000 pypop7-0.0.9/pypop7/optimizers/es/repeat_sepcmaes.py
+-rw-rw-rw-   0        0        0     4005 2022-06-10 03:25:11.000000 pypop7-0.0.9/pypop7/optimizers/es/repeat_vdcma.py
+-rw-rw-rw-   0        0        0     2931 2022-05-30 06:55:35.000000 pypop7-0.0.9/pypop7/optimizers/es/res.py
+-rw-rw-rw-   0        0        0     4288 2022-06-07 07:40:06.000000 pypop7-0.0.9/pypop7/optimizers/es/rmes.py
+-rw-rw-rw-   0        0        0     4203 2022-06-05 17:58:28.000000 pypop7-0.0.9/pypop7/optimizers/es/rmes2.py
+-rw-rw-rw-   0        0        0     5690 2022-06-09 10:09:07.000000 pypop7-0.0.9/pypop7/optimizers/es/sepcmaes.py
+-rw-rw-rw-   0        0        0     3170 2022-06-10 02:49:39.000000 pypop7-0.0.9/pypop7/optimizers/es/ssaes.py
+-rw-rw-rw-   0        0        0     1750 2022-06-15 12:09:01.000000 pypop7-0.0.9/pypop7/optimizers/es/test_ccmaes.py
+-rw-rw-rw-   0        0        0     1763 2022-07-02 10:47:43.000000 pypop7-0.0.9/pypop7/optimizers/es/test_ccmaes2016.py
+-rw-rw-rw-   0        0        0     1692 2022-05-28 07:46:55.000000 pypop7-0.0.9/pypop7/optimizers/es/test_csaes.py
+-rw-rw-rw-   0        0        0     1692 2022-05-26 07:56:38.000000 pypop7-0.0.9/pypop7/optimizers/es/test_dsaes.py
+-rw-rw-rw-   0        0        0     1394 2022-06-11 15:13:22.000000 pypop7-0.0.9/pypop7/optimizers/es/test_fmaes.py
+-rw-rw-rw-   0        0        0     1750 2022-05-26 08:59:04.000000 pypop7-0.0.9/pypop7/optimizers/es/test_lmmaes.py
+-rw-rw-rw-   0        0        0     1744 2022-05-28 13:17:13.000000 pypop7-0.0.9/pypop7/optimizers/es/test_maes.py
+-rw-rw-rw-   0        0        0     1391 2022-06-10 02:49:40.000000 pypop7-0.0.9/pypop7/optimizers/es/test_mmes.py
+-rw-rw-rw-   0        0        0     1787 2022-05-28 04:09:16.000000 pypop7-0.0.9/pypop7/optimizers/es/test_mvaes.py
+-rw-rw-rw-   0        0        0     1746 2022-06-27 11:18:31.000000 pypop7-0.0.9/pypop7/optimizers/es/test_opoa.py
+-rw-rw-rw-   0        0        0     1758 2022-06-29 22:26:34.000000 pypop7-0.0.9/pypop7/optimizers/es/test_opoa2015.py
+-rw-rw-rw-   0        0        0     1746 2022-06-13 10:32:47.000000 pypop7-0.0.9/pypop7/optimizers/es/test_opoc.py
+-rw-rw-rw-   0        0        0     1758 2022-06-13 15:10:32.000000 pypop7-0.0.9/pypop7/optimizers/es/test_opoc2009.py
+-rw-rw-rw-   0        0        0     1688 2022-05-31 07:54:08.000000 pypop7-0.0.9/pypop7/optimizers/es/test_r1es.py
+-rw-rw-rw-   0        0        0     1687 2022-05-26 07:01:48.000000 pypop7-0.0.9/pypop7/optimizers/es/test_res.py
+-rw-rw-rw-   0        0        0     1688 2022-06-16 07:17:15.000000 pypop7-0.0.9/pypop7/optimizers/es/test_rmes.py
+-rw-rw-rw-   0        0        0     1756 2022-06-08 11:00:02.000000 pypop7-0.0.9/pypop7/optimizers/es/test_sepcmaes.py
+-rw-rw-rw-   0        0        0     1690 2022-06-10 02:49:39.000000 pypop7-0.0.9/pypop7/optimizers/es/test_ssaes.py
+-rw-rw-rw-   0        0        0     1747 2022-06-02 16:48:17.000000 pypop7-0.0.9/pypop7/optimizers/es/test_vdcma.py
+-rw-rw-rw-   0        0        0     8021 2022-06-02 17:14:38.000000 pypop7-0.0.9/pypop7/optimizers/es/vdcma.py
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:35.151208 pypop7-0.0.9/pypop7/optimizers/ga/
+-rw-rw-rw-   0        0        0        0 2022-06-22 11:06:26.000000 pypop7-0.0.9/pypop7/optimizers/ga/__init__.py
+-rw-rw-rw-   0        0        0     2973 2022-06-27 13:41:02.000000 pypop7-0.0.9/pypop7/optimizers/ga/ga.py
+-rw-rw-rw-   0        0        0     2635 2022-06-27 13:41:02.000000 pypop7-0.0.9/pypop7/optimizers/ga/genitor.py
+-rw-rw-rw-   0        0        0     1362 2022-06-27 13:41:02.000000 pypop7-0.0.9/pypop7/optimizers/ga/test_gentitor.py
+drwxrwxrwx   0        0        0        0 2022-07-02 11:01:34.911208 pypop7-0.0.9/pypop7.egg-info/
+-rw-rw-rw-   0        0        0    36501 2022-07-02 11:01:33.000000 pypop7-0.0.9/pypop7.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6278 2022-07-02 11:01:34.000000 pypop7-0.0.9/pypop7.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-02 11:01:33.000000 pypop7-0.0.9/pypop7.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2022-07-02 11:01:34.000000 pypop7-0.0.9/pypop7.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       62 2022-07-02 11:01:34.000000 pypop7-0.0.9/pypop7.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      102 2022-06-18 17:03:15.000000 pypop7-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      918 2022-07-02 11:01:35.151208 pypop7-0.0.9/setup.cfg
```

### Comparing `pypop7-0.0.8/.gitignore` & `pypop7-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/LICENSE` & `pypop7-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/PKG-INFO` & `pypop7-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pypop7
-Version: 0.0.8
+Version: 0.0.9
 Summary: pypop7 (Pure-PYthon library of POPulation-based OPtimization)
 Home-page: https://github.com/Evolutionary-Intelligence/pypop
 Author: Evolutionary-Intelligence Team (from CSE@SUSTech, Shenzhen, China)
 Author-email: 11749325@mail.sustech.edu.cn
 Project-URL: Bug Tracker, https://github.com/Evolutionary-Intelligence/pypop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pypop7 (Pure-PYthon library of POPulation-based black-box OPtimization)
 
 [![GNU General Public License v3.0](https://img.shields.io/badge/license-GNU%20GPL--v3.0-green.svg)](https://github.com/Evolutionary-Intelligence/pypop/blob/main/LICENSE) [![gitter for pypop](https://img.shields.io/badge/gitter-pypop--go-brightgreen.svg)](https://gitter.im/pypop-go/community) [![PyPI for pypop7](https://img.shields.io/badge/PyPI-pypop7-yellowgreen.svg)](https://pypi.org/project/pypop7/)
 
@@ -99,19 +99,21 @@
 
   * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Rank-One Evolution Strategy (**[R1ES](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/r1es.py)**, R1-ES) [See [Li&Zhang, 2018, TEVC](https://ieeexplore.ieee.org/document/8080257)]
 
   * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Projection-based Covariance Matrix Adaptation (**VKDCMA**, VkD-CMA) [See [Akimoto&Hansen, 2016, GECCO](https://dl.acm.org/doi/abs/10.1145/2908812.2908863)]
 
   * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Linear Covariance Matrix Adaptation (**[VDCMA](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/vdcma.py)**, VD-CMA) [See [Akimoto et al., 2014, GECCO](https://dl.acm.org/doi/abs/10.1145/2576768.2598258)]
 
-  * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Active-Cholesky-CMA-ES-2015 (**[OPOA2015](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoa2015.py)**) [See [Krause&Igel, 2015, FOGA](https://dl.acm.org/doi/abs/10.1145/2725494.2725496)]
+  * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Cholesky-CMA-ES-2016 (**[CCMAES2016](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/ccmaes2016.py)**) [See [Krause et al., 2016, NeurIPS](https://proceedings.neurips.cc/paper/2016/hash/289dff07669d7a23de0ef88d2f7129e7-Abstract.html)]
+
+    * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Active-Cholesky-CMA-ES-2015 (**[OPOA2015](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoa2015.py)**) [See [Krause&Igel, 2015, FOGA](https://dl.acm.org/doi/abs/10.1145/2725494.2725496)]
 
     * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Active-Cholesky-CMA-ES (**[OPOA](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoa.py)**) [See [Arnold&Hansen, 2010, GECCO](https://dl.acm.org/doi/abs/10.1145/1830483.1830556)]
 
-  * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Cholesky-CMA-ES-2009 (**[CCMAES](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/ccmaes.py)**) [See [Suttorp et al., 2009, MLJ](https://link.springer.com/article/10.1007/s10994-009-5102-1)]
+  * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Cholesky-CMA-ES (**[CCMAES](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/ccmaes.py)**) [See [Suttorp et al., 2009, MLJ](https://link.springer.com/article/10.1007/s10994-009-5102-1)]
  
     * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Cholesky-CMA-ES-2009 (**[OPOC2009](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoc2009.py)**) [See [Suttorp et al., 2009, MLJ](https://link.springer.com/article/10.1007/s10994-009-5102-1)]
 
     * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Cholesky-CMA-ES (**[OPOC](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoc.py)**) [See [Igel et al., 2006, GECCO](https://dl.acm.org/doi/abs/10.1145/1143997.1144082)]
 
   * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Separable Covariance Matrix Adaptation Evolution Strategy (**[SEPCMAES](https://github.com/Evolutionary-Intelligence/pypop/blob/main/optimizers/es/sepcmaes.py)**, sep-CMA-ES) [See [Bäck et al., 2013](https://link.springer.com/book/10.1007/978-3-642-40137-4); [Ros&Hansen, 2008, PPSN](https://link.springer.com/chapter/10.1007/978-3-540-87700-4_30)]
```

### Comparing `pypop7-0.0.8/README.md` & `pypop7-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -84,19 +84,21 @@
 
   * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Rank-One Evolution Strategy (**[R1ES](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/r1es.py)**, R1-ES) [See [Li&Zhang, 2018, TEVC](https://ieeexplore.ieee.org/document/8080257)]
 
   * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Projection-based Covariance Matrix Adaptation (**VKDCMA**, VkD-CMA) [See [Akimoto&Hansen, 2016, GECCO](https://dl.acm.org/doi/abs/10.1145/2908812.2908863)]
 
   * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Linear Covariance Matrix Adaptation (**[VDCMA](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/vdcma.py)**, VD-CMA) [See [Akimoto et al., 2014, GECCO](https://dl.acm.org/doi/abs/10.1145/2576768.2598258)]
 
-  * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Active-Cholesky-CMA-ES-2015 (**[OPOA2015](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoa2015.py)**) [See [Krause&Igel, 2015, FOGA](https://dl.acm.org/doi/abs/10.1145/2725494.2725496)]
+  * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Cholesky-CMA-ES-2016 (**[CCMAES2016](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/ccmaes2016.py)**) [See [Krause et al., 2016, NeurIPS](https://proceedings.neurips.cc/paper/2016/hash/289dff07669d7a23de0ef88d2f7129e7-Abstract.html)]
+
+    * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Active-Cholesky-CMA-ES-2015 (**[OPOA2015](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoa2015.py)**) [See [Krause&Igel, 2015, FOGA](https://dl.acm.org/doi/abs/10.1145/2725494.2725496)]
 
     * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Active-Cholesky-CMA-ES (**[OPOA](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoa.py)**) [See [Arnold&Hansen, 2010, GECCO](https://dl.acm.org/doi/abs/10.1145/1830483.1830556)]
 
-  * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Cholesky-CMA-ES-2009 (**[CCMAES](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/ccmaes.py)**) [See [Suttorp et al., 2009, MLJ](https://link.springer.com/article/10.1007/s10994-009-5102-1)]
+  * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Cholesky-CMA-ES (**[CCMAES](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/ccmaes.py)**) [See [Suttorp et al., 2009, MLJ](https://link.springer.com/article/10.1007/s10994-009-5102-1)]
  
     * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Cholesky-CMA-ES-2009 (**[OPOC2009](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoc2009.py)**) [See [Suttorp et al., 2009, MLJ](https://link.springer.com/article/10.1007/s10994-009-5102-1)]
 
     * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Cholesky-CMA-ES (**[OPOC](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoc.py)**) [See [Igel et al., 2006, GECCO](https://dl.acm.org/doi/abs/10.1145/1143997.1144082)]
 
   * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Separable Covariance Matrix Adaptation Evolution Strategy (**[SEPCMAES](https://github.com/Evolutionary-Intelligence/pypop/blob/main/optimizers/es/sepcmaes.py)**, sep-CMA-ES) [See [Bäck et al., 2013](https://link.springer.com/book/10.1007/978-3-642-40137-4); [Ros&Hansen, 2008, PPSN](https://link.springer.com/chapter/10.1007/978-3-540-87700-4_30)]
```

### Comparing `pypop7-0.0.8/benchmarks/continuous_functions.py` & `pypop7-0.0.9/benchmarks/continuous_functions.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/benchmarks/generate_rotation_matrices.py` & `pypop7-0.0.9/benchmarks/generate_rotation_matrices.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/benchmarks/generate_shift_vectors.py` & `pypop7-0.0.9/benchmarks/generate_shift_vectors.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/benchmarks/rotated_functions.py` & `pypop7-0.0.9/benchmarks/rotated_functions.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/benchmarks/shifted_functions.py` & `pypop7-0.0.9/benchmarks/shifted_functions.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/benchmarks/test_base_functions.py` & `pypop7-0.0.9/benchmarks/test_base_functions.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/benchmarks/test_cases.py` & `pypop7-0.0.9/benchmarks/test_cases.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/benchmarks/test_continuous_functions.py` & `pypop7-0.0.9/benchmarks/test_continuous_functions.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/benchmarks/test_rotated_functions.py` & `pypop7-0.0.9/benchmarks/test_rotated_functions.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/benchmarks/test_shifted_functions.py` & `pypop7-0.0.9/benchmarks/test_shifted_functions.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/benchmarks/test_utils.py` & `pypop7-0.0.9/benchmarks/test_utils.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/benchmarks/utils.py` & `pypop7-0.0.9/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/docs/demo/demo.gif` & `pypop7-0.0.9/docs/demo/demo.gif`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/docs/demo/demo.py` & `pypop7-0.0.9/docs/demo/demo.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/docs/demo/demo_cem.gif` & `pypop7-0.0.9/docs/demo/demo_cem.gif`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/docs/demo/demo_cem.py` & `pypop7-0.0.9/docs/demo/demo_cem.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/docs/logo/PyPop-Logo-Small-0.png` & `pypop7-0.0.9/docs/logo/PyPop-Logo-Small-0.png`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/docs/logo/PyPop-Logo-Small.png` & `pypop7-0.0.9/docs/logo/PyPop-Logo-Small.png`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/es/repeat_maes.py` & `pypop7-0.0.9/optimizers/es/repeat_maes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/es/repeat_mmes.py` & `pypop7-0.0.9/optimizers/es/repeat_mmes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/es/repeat_r1es.py` & `pypop7-0.0.9/optimizers/es/repeat_r1es.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/es/repeat_rmes.py` & `pypop7-0.0.9/optimizers/es/repeat_rmes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/es/repeat_rmes2.py` & `pypop7-0.0.9/optimizers/es/repeat_rmes2.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/es/saes.py` & `pypop7-0.0.9/optimizers/es/saes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/es/test_saes.py` & `pypop7-0.0.9/optimizers/es/test_saes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/nes/nes.py` & `pypop7-0.0.9/optimizers/nes/nes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/nes/r1nes.py` & `pypop7-0.0.9/optimizers/nes/r1nes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/nes/repeat_figure_1_jmlr_2014_nes.py` & `pypop7-0.0.9/optimizers/nes/repeat_figure_1_jmlr_2014_nes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/nes/snes.py` & `pypop7-0.0.9/optimizers/nes/snes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/nes/test_r1nes.py` & `pypop7-0.0.9/optimizers/nes/test_r1nes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/nes/test_snes.py` & `pypop7-0.0.9/optimizers/nes/test_snes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/pso/clpso.py` & `pypop7-0.0.9/optimizers/pso/clpso.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/pso/opso.py` & `pypop7-0.0.9/optimizers/pso/opso.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/pso/opsogt.py` & `pypop7-0.0.9/optimizers/pso/opsogt.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/pso/opsort.py` & `pypop7-0.0.9/optimizers/pso/opsort.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/pso/pso.py` & `pypop7-0.0.9/optimizers/pso/pso.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/pso/psogt.py` & `pypop7-0.0.9/optimizers/pso/psogt.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/pso/psort.py` & `pypop7-0.0.9/optimizers/pso/psort.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/pso/test_clpso.py` & `pypop7-0.0.9/optimizers/pso/test_clpso.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/pso/test_opsogt.py` & `pypop7-0.0.9/optimizers/pso/test_opsogt.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/pso/test_opsort.py` & `pypop7-0.0.9/optimizers/pso/test_opsort.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/pso/test_psogt.py` & `pypop7-0.0.9/optimizers/pso/test_psogt.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/pso/test_psort.py` & `pypop7-0.0.9/optimizers/pso/test_psort.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/rs/arhc.py` & `pypop7-0.0.9/optimizers/rs/arhc.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/rs/prs.py` & `pypop7-0.0.9/optimizers/rs/prs.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/rs/rhc.py` & `pypop7-0.0.9/optimizers/rs/rhc.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/rs/rs.py` & `pypop7-0.0.9/optimizers/rs/rs.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/rs/test_arhc.py` & `pypop7-0.0.9/optimizers/rs/test_arhc.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/rs/test_prs.py` & `pypop7-0.0.9/optimizers/rs/test_prs.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/rs/test_rhc.py` & `pypop7-0.0.9/optimizers/rs/test_rhc.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/sa/csa.py` & `pypop7-0.0.9/optimizers/sa/csa.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/sa/esa.py` & `pypop7-0.0.9/optimizers/sa/esa.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/sa/test_csa.py` & `pypop7-0.0.9/optimizers/sa/test_csa.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/optimizers/sa/test_esa.py` & `pypop7-0.0.9/optimizers/sa/test_esa.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/benchmarks/base_functions.py` & `pypop7-0.0.9/pypop7/benchmarks/base_functions.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/cem/cem.py` & `pypop7-0.0.9/pypop7/optimizers/cem/cem.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/cem/dcem.py` & `pypop7-0.0.9/pypop7/optimizers/cem/dcem.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/cem/scem.py` & `pypop7-0.0.9/pypop7/optimizers/cem/scem.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/cem/secem.py` & `pypop7-0.0.9/pypop7/optimizers/cem/secem.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/cem/test_dcem.py` & `pypop7-0.0.9/pypop7/optimizers/cem/test_dcem.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/cem/test_scem.py` & `pypop7-0.0.9/pypop7/optimizers/cem/test_scem.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/cem/test_secem.py` & `pypop7-0.0.9/pypop7/optimizers/cem/test_secem.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/core/optimizer.py` & `pypop7-0.0.9/pypop7/optimizers/core/optimizer.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/ds/dsm.py` & `pypop7-0.0.9/pypop7/optimizers/ds/dsm.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/ds/hjdsm.py` & `pypop7-0.0.9/pypop7/optimizers/ds/hjdsm.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/ds/srs.py` & `pypop7-0.0.9/pypop7/optimizers/ds/srs.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/ds/test_hjdsm.py` & `pypop7-0.0.9/pypop7/optimizers/ds/test_hjdsm.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/ds/test_srs.py` & `pypop7-0.0.9/pypop7/optimizers/ds/test_srs.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/ccmaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/ccmaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/csaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/csaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/dsaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/dsaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/es.py` & `pypop7-0.0.9/pypop7/optimizers/es/es.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/fmaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/fmaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/lmmaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/lmmaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/maes.py` & `pypop7-0.0.9/pypop7/optimizers/es/maes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/mmes.py` & `pypop7-0.0.9/pypop7/optimizers/es/mmes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/mvaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/mvaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/opoa.py` & `pypop7-0.0.9/pypop7/optimizers/es/opoa.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/opoa2015.py` & `pypop7-0.0.9/pypop7/optimizers/es/opoa2015.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from pypop7.optimizers.es.es import ES
 
 
 @nb.jit(nopython=True)
 def cholesky_update(rm, z, downdate):
     # https://github.com/scipy/scipy/blob/d20f92fce9f1956bfa65365feeec39621a071932/
     #     scipy/linalg/_decomp_cholesky_update.py
-    rm, z = np.copy(rm.T), np.copy(z)
-    alpha, beta = np.empty_like(z), np.empty_like(z)
+    rm, z, alpha, beta = rm.T, z, np.empty_like(z), np.empty_like(z)
     alpha[-1], beta[-1] = 1., 1.
     sign = -1 if downdate else 1
     for r in range(len(z)):
         a = z[r] / rm[r, r]
         alpha[r] = alpha[r - 1] + sign * np.power(a, 2)
         beta[r] = np.sqrt(alpha[r])
         z[r + 1:] -= a * rm[r, r + 1:]
```

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/opoc.py` & `pypop7-0.0.9/pypop7/optimizers/es/opoc.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/opoc2009.py` & `pypop7-0.0.9/pypop7/optimizers/es/opoc2009.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/r1es.py` & `pypop7-0.0.9/pypop7/optimizers/es/r1es.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/repeat_ccmaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/repeat_ccmaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/repeat_lmmaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/repeat_lmmaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/repeat_maes.py` & `pypop7-0.0.9/pypop7/optimizers/es/repeat_maes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/repeat_mmes.py` & `pypop7-0.0.9/pypop7/optimizers/es/repeat_mmes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/repeat_mvaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/repeat_mvaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/repeat_opoa_fig1.py` & `pypop7-0.0.9/pypop7/optimizers/es/repeat_opoa_fig1.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/repeat_opoa_fig2.py` & `pypop7-0.0.9/pypop7/optimizers/es/repeat_opoa_fig2.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/repeat_opoc.py` & `pypop7-0.0.9/pypop7/optimizers/es/repeat_opoc.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/repeat_opoc2009.py` & `pypop7-0.0.9/pypop7/optimizers/es/repeat_opoc2009.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/repeat_r1es.py` & `pypop7-0.0.9/pypop7/optimizers/es/repeat_r1es.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/repeat_rmes.py` & `pypop7-0.0.9/pypop7/optimizers/es/repeat_rmes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/repeat_rmes2.py` & `pypop7-0.0.9/pypop7/optimizers/es/repeat_rmes2.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/repeat_sepcmaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/repeat_sepcmaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/repeat_vdcma.py` & `pypop7-0.0.9/pypop7/optimizers/es/repeat_vdcma.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/res.py` & `pypop7-0.0.9/pypop7/optimizers/es/res.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/rmes.py` & `pypop7-0.0.9/pypop7/optimizers/es/rmes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/rmes2.py` & `pypop7-0.0.9/pypop7/optimizers/es/rmes2.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/sepcmaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/sepcmaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/ssaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/ssaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_ccmaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_ccmaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_csaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_csaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_dsaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_dsaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_fmaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_fmaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_lmmaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_lmmaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_maes.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_maes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_mmes.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_mmes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_mvaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_mvaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_opoa.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_opoa.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_opoa2015.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_opoa2015.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_opoc.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_opoc.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_opoc2009.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_opoc2009.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_r1es.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_r1es.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_res.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_res.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_rmes.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_rmes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_sepcmaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_sepcmaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_ssaes.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_ssaes.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/test_vdcma.py` & `pypop7-0.0.9/pypop7/optimizers/es/test_vdcma.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/es/vdcma.py` & `pypop7-0.0.9/pypop7/optimizers/es/vdcma.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/ga/ga.py` & `pypop7-0.0.9/pypop7/optimizers/ga/ga.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/ga/genitor.py` & `pypop7-0.0.9/pypop7/optimizers/ga/genitor.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7/optimizers/ga/test_gentitor.py` & `pypop7-0.0.9/pypop7/optimizers/ga/test_gentitor.py`

 * *Files identical despite different names*

### Comparing `pypop7-0.0.8/pypop7.egg-info/PKG-INFO` & `pypop7-0.0.9/pypop7.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pypop7
-Version: 0.0.8
+Version: 0.0.9
 Summary: pypop7 (Pure-PYthon library of POPulation-based OPtimization)
 Home-page: https://github.com/Evolutionary-Intelligence/pypop
 Author: Evolutionary-Intelligence Team (from CSE@SUSTech, Shenzhen, China)
 Author-email: 11749325@mail.sustech.edu.cn
 Project-URL: Bug Tracker, https://github.com/Evolutionary-Intelligence/pypop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pypop7 (Pure-PYthon library of POPulation-based black-box OPtimization)
 
 [![GNU General Public License v3.0](https://img.shields.io/badge/license-GNU%20GPL--v3.0-green.svg)](https://github.com/Evolutionary-Intelligence/pypop/blob/main/LICENSE) [![gitter for pypop](https://img.shields.io/badge/gitter-pypop--go-brightgreen.svg)](https://gitter.im/pypop-go/community) [![PyPI for pypop7](https://img.shields.io/badge/PyPI-pypop7-yellowgreen.svg)](https://pypi.org/project/pypop7/)
 
@@ -99,19 +99,21 @@
 
   * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Rank-One Evolution Strategy (**[R1ES](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/r1es.py)**, R1-ES) [See [Li&Zhang, 2018, TEVC](https://ieeexplore.ieee.org/document/8080257)]
 
   * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Projection-based Covariance Matrix Adaptation (**VKDCMA**, VkD-CMA) [See [Akimoto&Hansen, 2016, GECCO](https://dl.acm.org/doi/abs/10.1145/2908812.2908863)]
 
   * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Linear Covariance Matrix Adaptation (**[VDCMA](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/vdcma.py)**, VD-CMA) [See [Akimoto et al., 2014, GECCO](https://dl.acm.org/doi/abs/10.1145/2576768.2598258)]
 
-  * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Active-Cholesky-CMA-ES-2015 (**[OPOA2015](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoa2015.py)**) [See [Krause&Igel, 2015, FOGA](https://dl.acm.org/doi/abs/10.1145/2725494.2725496)]
+  * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Cholesky-CMA-ES-2016 (**[CCMAES2016](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/ccmaes2016.py)**) [See [Krause et al., 2016, NeurIPS](https://proceedings.neurips.cc/paper/2016/hash/289dff07669d7a23de0ef88d2f7129e7-Abstract.html)]
+
+    * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Active-Cholesky-CMA-ES-2015 (**[OPOA2015](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoa2015.py)**) [See [Krause&Igel, 2015, FOGA](https://dl.acm.org/doi/abs/10.1145/2725494.2725496)]
 
     * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Active-Cholesky-CMA-ES (**[OPOA](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoa.py)**) [See [Arnold&Hansen, 2010, GECCO](https://dl.acm.org/doi/abs/10.1145/1830483.1830556)]
 
-  * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Cholesky-CMA-ES-2009 (**[CCMAES](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/ccmaes.py)**) [See [Suttorp et al., 2009, MLJ](https://link.springer.com/article/10.1007/s10994-009-5102-1)]
+  * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Cholesky-CMA-ES (**[CCMAES](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/ccmaes.py)**) [See [Suttorp et al., 2009, MLJ](https://link.springer.com/article/10.1007/s10994-009-5102-1)]
  
     * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Cholesky-CMA-ES-2009 (**[OPOC2009](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoc2009.py)**) [See [Suttorp et al., 2009, MLJ](https://link.springer.com/article/10.1007/s10994-009-5102-1)]
 
     * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) (1+1)-Cholesky-CMA-ES (**[OPOC](https://github.com/Evolutionary-Intelligence/pypop/blob/main/pypop7/optimizers/es/opoc.py)**) [See [Igel et al., 2006, GECCO](https://dl.acm.org/doi/abs/10.1145/1143997.1144082)]
 
   * ![large--scale--optimization](https://img.shields.io/badge/***-large--scale--optimization-orange.svg) Separable Covariance Matrix Adaptation Evolution Strategy (**[SEPCMAES](https://github.com/Evolutionary-Intelligence/pypop/blob/main/optimizers/es/sepcmaes.py)**, sep-CMA-ES) [See [Bäck et al., 2013](https://link.springer.com/book/10.1007/978-3-642-40137-4); [Ros&Hansen, 2008, PPSN](https://link.springer.com/chapter/10.1007/978-3-540-87700-4_30)]
```

### Comparing `pypop7-0.0.8/pypop7.egg-info/SOURCES.txt` & `pypop7-0.0.9/pypop7.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 pypop7.egg-info/top_level.txt
 pypop7/benchmarks/__init__.py
 pypop7/benchmarks/base_functions.py
 pypop7/optimizers/core/__init__.py
 pypop7/optimizers/core/optimizer.py
 pypop7/optimizers/es/__init__.py
 pypop7/optimizers/es/ccmaes.py
+pypop7/optimizers/es/ccmaes2016.py
 pypop7/optimizers/es/csaes.py
 pypop7/optimizers/es/dsaes.py
 pypop7/optimizers/es/es.py
 pypop7/optimizers/es/fmaes.py
 pypop7/optimizers/es/lmmaes.py
 pypop7/optimizers/es/maes.py
 pypop7/optimizers/es/mmes.py
@@ -99,14 +100,15 @@
 pypop7/optimizers/es/repeat_vdcma.py
 pypop7/optimizers/es/res.py
 pypop7/optimizers/es/rmes.py
 pypop7/optimizers/es/rmes2.py
 pypop7/optimizers/es/sepcmaes.py
 pypop7/optimizers/es/ssaes.py
 pypop7/optimizers/es/test_ccmaes.py
+pypop7/optimizers/es/test_ccmaes2016.py
 pypop7/optimizers/es/test_csaes.py
 pypop7/optimizers/es/test_dsaes.py
 pypop7/optimizers/es/test_fmaes.py
 pypop7/optimizers/es/test_lmmaes.py
 pypop7/optimizers/es/test_maes.py
 pypop7/optimizers/es/test_mmes.py
 pypop7/optimizers/es/test_mvaes.py
@@ -136,14 +138,15 @@
 pypop7/optimizers/ds/dsm.py
 pypop7/optimizers/ds/hjdsm.py
 pypop7/optimizers/ds/srs.py
 pypop7/optimizers/ds/test_hjdsm.py
 pypop7/optimizers/ds/test_srs.py
 pypop7/optimizers/es/__init__.py
 pypop7/optimizers/es/ccmaes.py
+pypop7/optimizers/es/ccmaes2016.py
 pypop7/optimizers/es/csaes.py
 pypop7/optimizers/es/dsaes.py
 pypop7/optimizers/es/es.py
 pypop7/optimizers/es/fmaes.py
 pypop7/optimizers/es/lmmaes.py
 pypop7/optimizers/es/maes.py
 pypop7/optimizers/es/mmes.py
@@ -169,14 +172,15 @@
 pypop7/optimizers/es/repeat_vdcma.py
 pypop7/optimizers/es/res.py
 pypop7/optimizers/es/rmes.py
 pypop7/optimizers/es/rmes2.py
 pypop7/optimizers/es/sepcmaes.py
 pypop7/optimizers/es/ssaes.py
 pypop7/optimizers/es/test_ccmaes.py
+pypop7/optimizers/es/test_ccmaes2016.py
 pypop7/optimizers/es/test_csaes.py
 pypop7/optimizers/es/test_dsaes.py
 pypop7/optimizers/es/test_fmaes.py
 pypop7/optimizers/es/test_lmmaes.py
 pypop7/optimizers/es/test_maes.py
 pypop7/optimizers/es/test_mmes.py
 pypop7/optimizers/es/test_mvaes.py
```

### Comparing `pypop7-0.0.8/setup.cfg` & `pypop7-0.0.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7970 6f70 370d 0a76 6572 7369   = pypop7..versi
-00000020: 6f6e 203d 2030 2e30 2e38 0d0a 6175 7468  on = 0.0.8..auth
+00000020: 6f6e 203d 2030 2e30 2e39 0d0a 6175 7468  on = 0.0.9..auth
 00000030: 6f72 203d 2045 766f 6c75 7469 6f6e 6172  or = Evolutionar
 00000040: 792d 496e 7465 6c6c 6967 656e 6365 2054  y-Intelligence T
 00000050: 6561 6d20 2866 726f 6d20 4353 4540 5355  eam (from CSE@SU
 00000060: 5354 6563 682c 2053 6865 6e7a 6865 6e2c  STech, Shenzhen,
 00000070: 2043 6869 6e61 290d 0a61 7574 686f 725f   China)..author_
 00000080: 656d 6169 6c20 3d20 3131 3734 3933 3235  email = 11749325
 00000090: 406d 6169 6c2e 7375 7374 6563 682e 6564  @mail.sustech.ed
@@ -41,17 +41,18 @@
 00000280: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
 00000290: 7061 636b 6167 6573 203d 200d 0a09 7079  packages = ...py
 000002a0: 706f 7037 2f62 656e 6368 6d61 726b 730d  pop7/benchmarks.
 000002b0: 0a09 7079 706f 7037 2f6f 7074 696d 697a  ..pypop7/optimiz
 000002c0: 6572 732f 636f 7265 0d0a 0970 7970 6f70  ers/core...pypop
 000002d0: 372f 6f70 7469 6d69 7a65 7273 2f65 730d  7/optimizers/es.
 000002e0: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-000002f0: 203d 203e 3d33 2e37 0d0a 696e 7374 616c   = >=3.7..instal
+000002f0: 203d 203e 3d33 2e35 0d0a 696e 7374 616c   = >=3.5..instal
 00000300: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
 00000310: 6e75 6d70 7920 3e3d 312e 3231 2e34 0d0a  numpy >=1.21.4..
 00000320: 0973 6369 7079 203e 3d31 2e38 2e31 0d0a  .scipy >=1.8.1..
 00000330: 096d 6174 706c 6f74 6c69 6220 3e3d 332e  .matplotlib >=3.
 00000340: 342e 320d 0a09 6365 6c6c 756c 6f69 6420  4.2...celluloid 
-00000350: 3e3d 302e 322e 300d 0a0d 0a5b 6567 675f  >=0.2.0....[egg_
-00000360: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000370: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000380: 300d 0a0d 0a                             0....
+00000350: 3e3d 302e 322e 300d 0a09 6e75 6d62 6120  >=0.2.0...numba 
+00000360: 3e3d 302e 3535 2e32 0d0a 0d0a 5b65 6767  >=0.55.2....[egg
+00000370: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000380: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000390: 2030 0d0a 0d0a                            0....
```

