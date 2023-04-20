# Comparing `tmp/siriuspy-2.72.0.tar.gz` & `tmp/siriuspy-2.73.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siriuspy-2.72.0.tar", last modified: Tue Mar 28 20:50:47 2023, max compression
+gzip compressed data, was "siriuspy-2.73.0.tar", last modified: Thu Apr 20 19:20:58 2023, max compression
```

## Comparing `siriuspy-2.72.0.tar` & `siriuspy-2.73.0.tar`

### file list

```diff
@@ -1,387 +1,387 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.367050 siriuspy-2.72.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-03-28 20:50:37.000000 siriuspy-2.72.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-03-28 20:50:37.000000 siriuspy-2.72.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-03-28 20:50:47.367050 siriuspy-2.72.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-03-28 20:50:37.000000 siriuspy-2.72.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-03-28 20:50:37.000000 siriuspy-2.72.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-28 20:50:47.367050 siriuspy-2.72.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-03-28 20:50:37.000000 siriuspy-2.72.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.331050 siriuspy-2.72.0/siriuspy/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.335049 siriuspy-2.72.0/siriuspy/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/bsmp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/bsmp/serial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/bsmp/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.335049 siriuspy-2.72.0/siriuspy/clientarch/
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientarch/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientarch/devices.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientarch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    19930 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientarch/pvarch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientarch/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.335049 siriuspy-2.72.0/siriuspy/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/configdb_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/configdb_document.py
--rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/pvsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.339050 siriuspy-2.72.0/siriuspy/clientconfigdb/types/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    55711 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/as_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/as_pwrstate.py
--rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/as_rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/bo_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/bo_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/bo_ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)   122392 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/global_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_bbadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_bbbproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_idff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/tb_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/tb_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/ts_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.339050 siriuspy-2.72.0/siriuspy/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/clientweb/implementation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.339050 siriuspy-2.72.0/siriuspy/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/currinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/currinfo/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.339050 siriuspy-2.72.0/siriuspy/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/currinfo/lifetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/currinfo/lifetime/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/currinfo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.339050 siriuspy-2.72.0/siriuspy/cycle/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/cycle/bo_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/cycle/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/cycle/fc_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/cycle/li_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/cycle/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     3567 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/cycle/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.343050 siriuspy-2.72.0/siriuspy/devices/
--rw-r--r--   0 runner    (1001) docker     (122)     1696 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/bbb.py
--rw-r--r--   0 runner    (1001) docker     (122)    40979 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/bpm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/currinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/dcct.py
--rw-r--r--   0 runner    (1001) docker     (122)    12553 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (122)     6472 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/dvf.py
--rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/egun.py
--rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/energy.py
--rw-r--r--   0 runner    (1001) docker     (122)    50026 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/ict.py
--rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/idff.py
--rw-r--r--   0 runner    (1001) docker     (122)    17197 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/ids.py
--rw-r--r--   0 runner    (1001) docker     (122)    20741 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/injctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    36024 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/injsys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/lienergy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/lillrf.py
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/machshift.py
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/modltr.py
--rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/orbit_interlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/posang.py
--rw-r--r--   0 runner    (1001) docker     (122)     9576 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/psconv.py
--rw-r--r--   0 runner    (1001) docker     (122)    12042 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/pstesters.py
--rw-r--r--   0 runner    (1001) docker     (122)    28050 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/pwrsupply.py
--rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/screen.py
--rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/sofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/syncd.py
--rw-r--r--   0 runner    (1001) docker     (122)    17572 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/timing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/devices/tune.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.343050 siriuspy-2.72.0/siriuspy/diagbeam/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagbeam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.343050 siriuspy-2.72.0/siriuspy/diagbeam/bpm/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagbeam/bpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagbeam/bpm/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.343050 siriuspy-2.72.0/siriuspy/diagbeam/dcct/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagbeam/dcct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagbeam/dcct/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.343050 siriuspy-2.72.0/siriuspy/diagbeam/ict/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagbeam/ict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagbeam/ict/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.343050 siriuspy-2.72.0/siriuspy/diagbeam/screen/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagbeam/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagbeam/screen/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.343050 siriuspy-2.72.0/siriuspy/diagbeam/slit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagbeam/slit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagbeam/slit/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.343050 siriuspy-2.72.0/siriuspy/diagsys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.343050 siriuspy-2.72.0/siriuspy/diagsys/lidiag/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/lidiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/lidiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/lidiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/lidiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.347050 siriuspy-2.72.0/siriuspy/diagsys/psdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/psdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/psdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     4299 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/psdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     6705 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/psdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.347050 siriuspy-2.72.0/siriuspy/diagsys/pudiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/pudiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/pudiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/pudiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/pudiag/pvs.py
--rw-r--r--   0 runner    (1001) docker     (122)     6824 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.347050 siriuspy-2.72.0/siriuspy/diagsys/rfdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/rfdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/rfdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/rfdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/diagsys/rfdiag/pvs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/envars.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.347050 siriuspy-2.72.0/siriuspy/epics/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/epics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/epics/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/epics/properties.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/epics/pv.py
--rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/epics/pv_fake.py
--rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/epics/pv_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/epics/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.347050 siriuspy-2.72.0/siriuspy/fofb/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/fofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18873 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/fofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    79118 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/fofb/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.347050 siriuspy-2.72.0/siriuspy/idff/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/idff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4539 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/idff/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.347050 siriuspy-2.72.0/siriuspy/injctrl/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/injctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15244 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/injctrl/bias_feedback.py
--rw-r--r--   0 runner    (1001) docker     (122)    23521 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/injctrl/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    58514 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/injctrl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.351050 siriuspy-2.72.0/siriuspy/machshift/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/machshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/machshift/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    77640 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/machshift/macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     8913 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/machshift/macschedule.py
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/machshift/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5429 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/machshift/test_macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/machshift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.351050 siriuspy-2.72.0/siriuspy/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/magnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/magnet/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/magnet/excdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/magnet/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/magnet/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/magnet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.351050 siriuspy-2.72.0/siriuspy/meas/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/meas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/meas/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.351050 siriuspy-2.72.0/siriuspy/meas/liemit/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/meas/liemit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/meas/liemit/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/meas/liemit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.351050 siriuspy-2.72.0/siriuspy/meas/lienergy/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/meas/lienergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/meas/lienergy/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/meas/lienergy/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/meas/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.351050 siriuspy-2.72.0/siriuspy/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/namesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/namesys/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.351050 siriuspy-2.72.0/siriuspy/optics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/optics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/optics/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     6906 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/optics/lattice_survey.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.351050 siriuspy-2.72.0/siriuspy/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/opticscorr/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/opticscorr/chrom.py
--rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/opticscorr/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/opticscorr/opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/opticscorr/tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/opticscorr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.351050 siriuspy-2.72.0/siriuspy/oscilloscope/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/oscilloscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6544 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/oscilloscope/keysight.py
--rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/oscilloscope/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.351050 siriuspy-2.72.0/siriuspy/posang/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/posang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/posang/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/posang/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/posang/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.355050 siriuspy-2.72.0/siriuspy/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/beaglebone.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.355050 siriuspy-2.72.0/siriuspy/pwrsupply/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    19620 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    54163 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/bsmp/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)   145811 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10620 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.355050 siriuspy-2.72.0/siriuspy/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/pructrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/pructrl/pru.py
--rw-r--r--   0 runner    (1001) docker     (122)    26340 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/pructrl/prucontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/pructrl/prucparms.py
--rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/pructrl/psdevstate.py
--rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/pructrl/udc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.355050 siriuspy-2.72.0/siriuspy/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/psctrl/pscontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/psctrl/pscreaders.py
--rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/psctrl/pscstatus.py
--rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/psctrl/pscwriters.py
--rw-r--r--   0 runner    (1001) docker     (122)    42458 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/psctrl/psmodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    33182 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/pwrsupply/siggen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.355050 siriuspy-2.72.0/siriuspy/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/ramp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/ramp/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/ramp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/ramp/magnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/ramp/ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/ramp/reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/ramp/test_reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/ramp/testwfm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/ramp/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/ramp/waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.359050 siriuspy-2.72.0/siriuspy/search/
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/search/bpms_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/search/hl_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     4499 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/search/id_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/search/ioc_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/search/ll_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/search/ma_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    23538 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/search/ps_search.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.359050 siriuspy-2.72.0/siriuspy/simul/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/simul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/simul/simfactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/simul/simps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/simul/simpv.py
--rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/simul/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/simul/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.359050 siriuspy-2.72.0/siriuspy/sofb/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/sofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4646 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/sofb/base_class.py
--rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/sofb/bpms.py
--rw-r--r--   0 runner    (1001) docker     (122)    32149 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/sofb/correctors.py
--rw-r--r--   0 runner    (1001) docker     (122)    47045 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/sofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    45797 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/sofb/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    12220 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/sofb/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    39653 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/sofb/orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/sofb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.359050 siriuspy-2.72.0/siriuspy/stabinfo/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/stabinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/stabinfo/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/stabinfo/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.359050 siriuspy-2.72.0/siriuspy/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/timesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/timesys/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/timesys/hl_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    33256 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/timesys/ll_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/timesys/plot_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/timesys/static_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-03-28 20:50:37.000000 siriuspy-2.72.0/siriuspy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.335049 siriuspy-2.72.0/siriuspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-03-28 20:50:47.000000 siriuspy-2.72.0/siriuspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9900 2023-03-28 20:50:47.000000 siriuspy-2.72.0/siriuspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-28 20:50:47.000000 siriuspy-2.72.0/siriuspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-28 20:50:47.000000 siriuspy-2.72.0/siriuspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-03-28 20:50:47.000000 siriuspy-2.72.0/siriuspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-03-28 20:50:47.000000 siriuspy-2.72.0/siriuspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.359050 siriuspy-2.72.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.363050 siriuspy-2.72.0/tests/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/bsmp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/bsmp/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/bsmp/test_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/bsmp/test_entities.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/bsmp/test_serial.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/bsmp/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.363050 siriuspy-2.72.0/tests/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/clientconfigdb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/clientconfigdb/test_configdb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.363050 siriuspy-2.72.0/tests/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/clientweb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/clientweb/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.363050 siriuspy-2.72.0/tests/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/currinfo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.363050 siriuspy-2.72.0/tests/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/currinfo/lifetime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/currinfo/lifetime/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/currinfo/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/currinfo/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.363050 siriuspy-2.72.0/tests/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/magnet/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/magnet/test_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/magnet/tests_normalizer.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/mock_servweb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.363050 siriuspy-2.72.0/tests/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/namesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/namesys/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.363050 siriuspy-2.72.0/tests/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/opticscorr/test_chrom.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/opticscorr/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/opticscorr/test_opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/opticscorr/test_tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/opticscorr/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.363050 siriuspy-2.72.0/tests/posang/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/posang/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/posang/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/posang/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.363050 siriuspy-2.72.0/tests/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/pwrsupply/db.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.363050 siriuspy-2.72.0/tests/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/pwrsupply/pructrl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/pwrsupply/pructrl/test_pru.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.363050 siriuspy-2.72.0/tests/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/pwrsupply/psctrl/test_pscwriters.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/pwrsupply/test_beaglebone.py
--rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/pwrsupply/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6410 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/pwrsupply/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/pwrsupply/test_data.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/pwrsupply/test_siggen.py
--rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/pwrsupply/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.363050 siriuspy-2.72.0/tests/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/ramp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/ramp/test_magnet.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/ramp/test_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.367050 siriuspy-2.72.0/tests/search/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/search/test_hl_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/search/test_init.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/search/test_ll_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/search/test_ma_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13468 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/search/test_ps_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/test_callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-03-28 20:50:37.000000 siriuspy-2.72.0/tests/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-03-28 20:50:38.000000 siriuspy-2.72.0/tests/test_envars.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-03-28 20:50:38.000000 siriuspy-2.72.0/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:47.367050 siriuspy-2.72.0/tests/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 20:50:38.000000 siriuspy-2.72.0/tests/timesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-03-28 20:50:38.000000 siriuspy-2.72.0/tests/timesys/test_csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-03-28 20:50:38.000000 siriuspy-2.72.0/tests/timesys/test_plot_network.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.852560 siriuspy-2.73.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-04-20 19:20:44.000000 siriuspy-2.73.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-04-20 19:20:44.000000 siriuspy-2.73.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-04-20 19:20:58.848559 siriuspy-2.73.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-04-20 19:20:44.000000 siriuspy-2.73.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-04-20 19:20:44.000000 siriuspy-2.73.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 19:20:58.852560 siriuspy-2.73.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-04-20 19:20:44.000000 siriuspy-2.73.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.784550 siriuspy-2.73.0/siriuspy/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.788551 siriuspy-2.73.0/siriuspy/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/bsmp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/bsmp/serial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/bsmp/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.788551 siriuspy-2.73.0/siriuspy/clientarch/
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientarch/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientarch/devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientarch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientarch/pvarch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientarch/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.788551 siriuspy-2.73.0/siriuspy/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/configdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/configdb_document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/pvsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.792551 siriuspy-2.73.0/siriuspy/clientconfigdb/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57636 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_pwrstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)   122432 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/global_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_bbadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_bbbproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/ts_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.792551 siriuspy-2.73.0/siriuspy/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/clientweb/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.792551 siriuspy-2.73.0/siriuspy/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/currinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/currinfo/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.792551 siriuspy-2.73.0/siriuspy/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/currinfo/lifetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/currinfo/lifetime/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/currinfo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.792551 siriuspy-2.73.0/siriuspy/cycle/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/cycle/bo_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/cycle/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/cycle/fc_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/cycle/li_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/cycle/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3567 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/cycle/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.796552 siriuspy-2.73.0/siriuspy/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)     1696 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/bbb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40979 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/bpm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/currinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/dcct.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12731 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6799 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/dvf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/egun.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/energy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48527 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/ict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17197 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20741 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/injctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36024 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/injsys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/lienergy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/lillrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/machshift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/modltr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/orbit_interlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/posang.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9576 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/psconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12042 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/pstesters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28397 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/pwrsupply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/screen.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/sofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/syncd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/timing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/devices/tune.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.796552 siriuspy-2.73.0/siriuspy/diagbeam/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.796552 siriuspy-2.73.0/siriuspy/diagbeam/bpm/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/bpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/bpm/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.796552 siriuspy-2.73.0/siriuspy/diagbeam/dcct/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/dcct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/dcct/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.796552 siriuspy-2.73.0/siriuspy/diagbeam/ict/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/ict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/ict/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.796552 siriuspy-2.73.0/siriuspy/diagbeam/screen/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/screen/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.796552 siriuspy-2.73.0/siriuspy/diagbeam/slit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/slit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagbeam/slit/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/diagsys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/diagsys/lidiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/lidiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/lidiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/lidiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/lidiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/diagsys/psdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/psdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/psdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4299 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/psdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6705 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/psdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/diagsys/pudiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/pudiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/pudiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/pudiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/pudiag/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6824 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/diagsys/rfdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/rfdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/rfdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/rfdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/diagsys/rfdiag/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/envars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/epics/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/epics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/epics/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/epics/properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/epics/pv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/epics/pv_fake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/epics/pv_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/epics/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/fofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/fofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18873 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/fofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    80150 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/fofb/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/idff/
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/idff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4539 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/idff/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.800552 siriuspy-2.73.0/siriuspy/injctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/injctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15244 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/injctrl/bias_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26067 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/injctrl/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    67948 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/injctrl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/machshift/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/machshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/machshift/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    77640 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/machshift/macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8913 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/machshift/macschedule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/machshift/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5429 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/machshift/test_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/machshift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/magnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/magnet/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/magnet/excdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/magnet/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/magnet/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/magnet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/meas/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/meas/liemit/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/liemit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/liemit/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/liemit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/meas/lienergy/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/lienergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/lienergy/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/lienergy/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/meas/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/namesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/namesys/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/optics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/optics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/optics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6906 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/optics/lattice_survey.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.804553 siriuspy-2.73.0/siriuspy/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/opticscorr/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/opticscorr/chrom.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/opticscorr/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/opticscorr/opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/opticscorr/tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/opticscorr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.808554 siriuspy-2.73.0/siriuspy/oscilloscope/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/oscilloscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6544 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/oscilloscope/keysight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/oscilloscope/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.808554 siriuspy-2.73.0/siriuspy/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/posang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/posang/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/posang/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/posang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.808554 siriuspy-2.73.0/siriuspy/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/beaglebone.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.808554 siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)   150426 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10620 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.808554 siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/pru.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26340 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/prucontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/prucparms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/psdevstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/udc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.808554 siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscreaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscstatus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscwriters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/psmodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33182 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/pwrsupply/siggen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.816555 siriuspy-2.73.0/siriuspy/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/magnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/test_reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/testwfm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/ramp/waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.820555 siriuspy-2.73.0/siriuspy/search/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/bpms_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/hl_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4499 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/id_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/ioc_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/ll_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/ma_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/search/ps_search.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.824556 siriuspy-2.73.0/siriuspy/simul/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/simul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/simul/simfactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/simul/simps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/simul/simpv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/simul/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/simul/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.828556 siriuspy-2.73.0/siriuspy/sofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4646 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/bpms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32149 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47045 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45797 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12220 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39653 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/sofb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.832557 siriuspy-2.73.0/siriuspy/stabinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/stabinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/stabinfo/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/stabinfo/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.832557 siriuspy-2.73.0/siriuspy/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/timesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/timesys/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/timesys/hl_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33256 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/timesys/ll_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/timesys/plot_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/timesys/static_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-04-20 19:20:44.000000 siriuspy-2.73.0/siriuspy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.784550 siriuspy-2.73.0/siriuspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-04-20 19:20:58.000000 siriuspy-2.73.0/siriuspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9900 2023-04-20 19:20:58.000000 siriuspy-2.73.0/siriuspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 19:20:58.000000 siriuspy-2.73.0/siriuspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 19:20:58.000000 siriuspy-2.73.0/siriuspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-04-20 19:20:58.000000 siriuspy-2.73.0/siriuspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-20 19:20:58.000000 siriuspy-2.73.0/siriuspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.836557 siriuspy-2.73.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.840558 siriuspy-2.73.0/tests/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/bsmp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/bsmp/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/bsmp/test_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/bsmp/test_entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/bsmp/test_serial.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/bsmp/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.840558 siriuspy-2.73.0/tests/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/clientconfigdb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/clientconfigdb/test_configdb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.840558 siriuspy-2.73.0/tests/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/clientweb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/clientweb/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.840558 siriuspy-2.73.0/tests/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/currinfo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.840558 siriuspy-2.73.0/tests/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/currinfo/lifetime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/currinfo/lifetime/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/currinfo/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/currinfo/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.840558 siriuspy-2.73.0/tests/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/magnet/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/magnet/test_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/magnet/tests_normalizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/mock_servweb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.840558 siriuspy-2.73.0/tests/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/namesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/namesys/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.844559 siriuspy-2.73.0/tests/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/opticscorr/test_chrom.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/opticscorr/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/opticscorr/test_opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/opticscorr/test_tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/opticscorr/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.844559 siriuspy-2.73.0/tests/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/posang/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/posang/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/posang/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.844559 siriuspy-2.73.0/tests/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/db.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.848559 siriuspy-2.73.0/tests/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/pructrl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/pructrl/test_pru.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.848559 siriuspy-2.73.0/tests/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/psctrl/test_pscwriters.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/test_beaglebone.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/test_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/test_siggen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/pwrsupply/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.848559 siriuspy-2.73.0/tests/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/ramp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/ramp/test_magnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/ramp/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.848559 siriuspy-2.73.0/tests/search/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/search/test_hl_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/search/test_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/search/test_ll_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/search/test_ma_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/search/test_ps_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/test_callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/test_envars.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:58.848559 siriuspy-2.73.0/tests/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/timesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/timesys/test_csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-04-20 19:20:44.000000 siriuspy-2.73.0/tests/timesys/test_plot_network.py
```

### Comparing `siriuspy-2.72.0/LICENSE` & `siriuspy-2.73.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/PKG-INFO` & `siriuspy-2.73.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.72.0
+Version: 2.73.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.72.0/README.md` & `siriuspy-2.73.0/README.md`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/setup.py` & `siriuspy-2.73.0/setup.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/bsmp/commands.py` & `siriuspy-2.73.0/siriuspy/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/bsmp/constants.py` & `siriuspy-2.73.0/siriuspy/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/bsmp/entities.py` & `siriuspy-2.73.0/siriuspy/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/bsmp/exceptions.py` & `siriuspy-2.73.0/siriuspy/bsmp/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/bsmp/serial.py` & `siriuspy-2.73.0/siriuspy/bsmp/serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/bsmp/types.py` & `siriuspy-2.73.0/siriuspy/bsmp/types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/callbacks.py` & `siriuspy-2.73.0/siriuspy/callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientarch/client.py` & `siriuspy-2.73.0/siriuspy/clientarch/client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientarch/devices.py` & `siriuspy-2.73.0/siriuspy/clientarch/devices.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientarch/exceptions.py` & `siriuspy-2.73.0/siriuspy/clientarch/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientarch/pvarch.py` & `siriuspy-2.73.0/siriuspy/clientarch/pvarch.py`

 * *Files 4% similar despite different names*

```diff
@@ -397,14 +397,19 @@
         self._pvdata = self._init_pvdatas(pvnames, self.connector)
 
     @property
     def pvnames(self):
         """PV names."""
         return _dcopy(self._pvnames)
 
+    @pvnames.setter
+    def pvnames(self, new_pvnames):
+        self._pvnames = new_pvnames
+        self._pvdata = self._init_pvdatas(new_pvnames, self.connector)
+
     @property
     def is_archived(self):
         """Is archived."""
         self.connect()
         for pvn in self._pvnames:
             if self.connector.getPVDetails(pvn) is None:
                 return False
@@ -513,19 +518,24 @@
             return
         if len(self._pvnames) == 1:
             pvname = self._pvnames[0]
             data = {pvname: data}
         for pvname in self._pvnames:
             self._pvdata[pvname].set_data(**data[pvname])
 
-    @staticmethod
-    def _init_pvdatas(pvnames, connector):
+    def _init_pvdatas(self, pvnames, connector):
         pvdata = dict()
         for pvname in pvnames:
             pvdata[pvname] = PVData(pvname, connector)
+            pvdata[pvname].parallel_query_bin_interval = \
+                self._parallel_query_bin_interval
+            if self._time_start is not None:
+                pvdata[pvname].time_start = self._time_start
+            if self._time_stop is not None:
+                pvdata[pvname].time_stop = self._time_stop
         return pvdata
 
     def __getitem__(self, val):
         """Get item."""
         if isinstance(val, str):
             return self._pvdata[val]
         elif isinstance(val, int):
```

### Comparing `siriuspy-2.72.0/siriuspy/clientarch/time.py` & `siriuspy-2.73.0/siriuspy/clientarch/time.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/_templates.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/_templates.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/configdb_client.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/configdb_document.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/configdb_document.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/pvsconfig.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/pvsconfig.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/as_corrloop_params.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_corrloop_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/as_diagnostics.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1409,18 +1409,80 @@
     ['SI-Glob:DI-TuneProc-V:TrkGenLvlOffset-SP', 0.0, 0],
     ['SI-Glob:DI-TuneProc-V:GetSpectrum-Sel', 0, 0],
     ['SI-Glob:DI-TuneProc-V:TrigSrc-Sel', 0, 0],
     ['SI-Glob:DI-TuneProc-V:DispRange-SP', 0.0, 0],
     ['SI-Glob:DI-TuneProc-V:FiltType-Sel', 0, 0],
     ]
 
+_fofbctrls = [
+    'IA-01RaBPM:BS-FOFBCtrl',
+    'IA-02RaBPM:BS-FOFBCtrl',
+    'IA-03RaBPM:BS-FOFBCtrl',
+    'IA-04RaBPM:BS-FOFBCtrl',
+    'IA-05RaBPM:BS-FOFBCtrl',
+    'IA-06RaBPM:BS-FOFBCtrl',
+    'IA-07RaBPM:BS-FOFBCtrl',
+    'IA-08RaBPM:BS-FOFBCtrl',
+    'IA-09RaBPM:BS-FOFBCtrl',
+    'IA-10RaBPM:BS-FOFBCtrl',
+    'IA-11RaBPM:BS-FOFBCtrl',
+    'IA-12RaBPM:BS-FOFBCtrl',
+    'IA-13RaBPM:BS-FOFBCtrl',
+    'IA-14RaBPM:BS-FOFBCtrl',
+    'IA-15RaBPM:BS-FOFBCtrl',
+    'IA-16RaBPM:BS-FOFBCtrl',
+    'IA-17RaBPM:BS-FOFBCtrl',
+    'IA-18RaBPM:BS-FOFBCtrl',
+    'IA-19RaBPM:BS-FOFBCtrl',
+    'IA-20RaBPM:BS-FOFBCtrl',
+]
+_fofb_propts = [
+    [':TRIGGER0Dir-Sel', 1, 0.0],
+    [':TRIGGER0DirPol-Sel', 1, 0.0],
+    [':TRIGGER0RcvLen-SP', 1, 0.0],
+    [':TRIGGER0TrnLen-SP', 1, 0.0],
+    [':TRIGGER1Dir-Sel', 1, 0.0],
+    [':TRIGGER1DirPol-Sel', 1, 0.0],
+    [':TRIGGER1RcvLen-SP', 1, 0.0],
+    [':TRIGGER1TrnLen-SP', 1, 0.0],
+    [':TRIGGER2Dir-Sel', 0, 0.0],
+    [':TRIGGER2DirPol-Sel', 1, 0.0],
+    [':TRIGGER2RcvLen-SP', 1, 0.0],
+    [':TRIGGER2TrnLen-SP', 1, 0.0],
+    [':TRIGGER3Dir-Sel', 0, 0.0],
+    [':TRIGGER3DirPol-Sel', 1, 0.0],
+    [':TRIGGER3RcvLen-SP', 1, 0.0],
+    [':TRIGGER3TrnLen-SP', 1, 0.0],
+    [':TRIGGER4Dir-Sel', 1, 0.0],
+    [':TRIGGER4DirPol-Sel', 1, 0.0],
+    [':TRIGGER4RcvLen-SP', 1, 0.0],
+    [':TRIGGER4TrnLen-SP', 1, 0.0],
+    [':TRIGGER5Dir-Sel', 1, 0.0],
+    [':TRIGGER5DirPol-Sel', 1, 0.0],
+    [':TRIGGER5RcvLen-SP', 1, 0.0],
+    [':TRIGGER5TrnLen-SP', 1, 0.0],
+    [':TRIGGER6Dir-Sel', 1, 0.0],
+    [':TRIGGER6DirPol-Sel', 1, 0.0],
+    [':TRIGGER6RcvLen-SP', 1, 0.0],
+    [':TRIGGER6TrnLen-SP', 1, 0.0],
+    [':TRIGGER7Dir-Sel', 1, 0.0],
+    [':TRIGGER7DirPol-Sel', 1, 0.0],
+    [':TRIGGER7RcvLen-SP', 1, 0.0],
+    [':TRIGGER7TrnLen-SP', 1, 0.0],
+    ]
+_fofb_pvs = list()
+for dev in _fofbctrls:
+    for ppt, val, dly in _fofb_propts:
+        _fofb_pvs.append([dev+ppt, val, dly])
+
+
 # When using this type of configuration to set the machine,
 # the list of PVs should be processed in the same order they are stored
 # in the configuration. The second numeric parameter in the pair is the
 # delay [s] the client should wait before setting the next PV.
 
 _template_dict = {
     'pvs':
         _li_diags + _amcfpgaevr_pvs + _bpm_pvs + _scrn_pvs + _vlightcam_pvs +
-        _dcct_pvs + _slit_pvs + _tune_pvs
+        _dcct_pvs + _slit_pvs + _tune_pvs + _fofb_pvs
         # + _ict_pvs  # commented out becaus IOC is down.
         }
```

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/as_pwrstate.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_pwrstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/as_rf.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/as_rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/bo_normalized.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/bo_orbit.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/bo_ramp.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/global_config.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/global_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,22 +559,22 @@
     ['SI-01SA:TI-InjNLKckr:NrPulses-SP', 0, 0.0],
     ['SI-01SA:TI-InjNLKckr:Polarity-Sel', 0, 0.0],
     ['SI-01SA:TI-InjNLKckr:Src-Sel', 0, 0.0],
     ['SI-01SA:TI-InjNLKckr:State-Sel', 0, 0.0],
     ['SI-01SA:TI-InjNLKckr:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['SI-01SA:TI-InjNLKckr:LowLvlLock-Sel', 0, 0.0],
 
-    ['SI-01SA:TI-PingH:DelayRaw-SP', 0, 0],
-    ['SI-01SA:TI-PingH:WidthRaw-SP', 0, 0.0],
-    ['SI-01SA:TI-PingH:NrPulses-SP', 0, 0.0],
-    ['SI-01SA:TI-PingH:Polarity-Sel', 0, 0.0],
-    ['SI-01SA:TI-PingH:Src-Sel', 0, 0.0],
-    ['SI-01SA:TI-PingH:State-Sel', 0, 0.0],
-    ['SI-01SA:TI-PingH:DeltaDelayRaw-SP', 30*[0, ], 0],
-    ['SI-01SA:TI-PingH:LowLvlLock-Sel', 0, 0.0],
+    ['AS-Glob:TI-Osc-InjSI2:DelayRaw-SP', 0, 0],
+    ['AS-Glob:TI-Osc-InjSI2:WidthRaw-SP', 0, 0.0],
+    ['AS-Glob:TI-Osc-InjSI2:NrPulses-SP', 0, 0.0],
+    ['AS-Glob:TI-Osc-InjSI2:Polarity-Sel', 0, 0.0],
+    ['AS-Glob:TI-Osc-InjSI2:Src-Sel', 0, 0.0],
+    ['AS-Glob:TI-Osc-InjSI2:State-Sel', 0, 0.0],
+    ['AS-Glob:TI-Osc-InjSI2:DeltaDelayRaw-SP', 30*[0, ], 0],
+    ['AS-Glob:TI-Osc-InjSI2:LowLvlLock-Sel', 0, 0.0],
 
     ['SI-13C4:TI-DCCT:DelayRaw-SP', 0, 0],
     ['SI-13C4:TI-DCCT:WidthRaw-SP', 0, 0.0],
     ['SI-13C4:TI-DCCT:NrPulses-SP', 0, 0.0],
     ['SI-13C4:TI-DCCT:Polarity-Sel', 0, 0.0],
     ['SI-13C4:TI-DCCT:RFDelayType-Sel', 0, 0.0],
     ['SI-13C4:TI-DCCT:Src-Sel', 0, 0.0],
```

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_bbadata.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_bbadata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_bbbproc.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_bbbproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_fofb.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_id.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_id.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_idff.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_idff.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_orbit.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/tb_normalized.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/tb_orbit.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/tb_posang_respm.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/tb_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/ts_orbit.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/ts_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientconfigdb/types/ts_posang_respm.py` & `siriuspy-2.73.0/siriuspy/clientconfigdb/types/ts_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/clientweb/implementation.py` & `siriuspy-2.73.0/siriuspy/clientweb/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/csdev.py` & `siriuspy-2.73.0/siriuspy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/currinfo/csdev.py` & `siriuspy-2.73.0/siriuspy/currinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/currinfo/lifetime/main.py` & `siriuspy-2.73.0/siriuspy/currinfo/lifetime/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/currinfo/main.py` & `siriuspy-2.73.0/siriuspy/currinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/cycle/__init__.py` & `siriuspy-2.73.0/siriuspy/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/cycle/bo_cycle_data.py` & `siriuspy-2.73.0/siriuspy/cycle/bo_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/cycle/conn.py` & `siriuspy-2.73.0/siriuspy/cycle/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/cycle/fc_cycle_data.py` & `siriuspy-2.73.0/siriuspy/cycle/fc_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/cycle/li_cycle_data.py` & `siriuspy-2.73.0/siriuspy/cycle/li_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/cycle/main.py` & `siriuspy-2.73.0/siriuspy/cycle/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/cycle/util.py` & `siriuspy-2.73.0/siriuspy/cycle/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/__init__.py` & `siriuspy-2.73.0/siriuspy/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/bbb.py` & `siriuspy-2.73.0/siriuspy/devices/bbb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/bpm.py` & `siriuspy-2.73.0/siriuspy/devices/bpm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/currinfo.py` & `siriuspy-2.73.0/siriuspy/devices/currinfo.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/dcct.py` & `siriuspy-2.73.0/siriuspy/devices/dcct.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/device.py` & `siriuspy-2.73.0/siriuspy/devices/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -375,30 +375,35 @@
             self, devices, propty, values, comp='eq',
             timeout=_DEF_TIMEOUT, return_prob=False):
         """Wait for devices property to reach value(s)."""
         if isinstance(comp, str):
             comp = getattr(_opr, comp)
         dev2val = self._get_dev_2_val(devices, values)
 
+        tini = _time.time()
         for _ in range(int(timeout/_TINY_INTERVAL)):
             okdevs = set()
             for k, v in dev2val.items():
                 boo = comp(k[propty], v)
                 if isinstance(boo, _np.ndarray):
                     boo = _np.all(boo)
                 if boo:
                     okdevs.add(k)
+                if _time.time() - tini > timeout:
+                    break
             list(map(dev2val.__delitem__, okdevs))
             if not dev2val:
                 break
+            if _time.time() - tini > timeout:
+                break
             _time.sleep(_TINY_INTERVAL)
 
         allok = not dev2val
         if return_prob:
-            return allok, [dev.devname+':'+propty for dev in dev2val]
+            return allok, [dev.pv_object(propty).pvname for dev in dev2val]
         return allok
 
     def _get_dev_2_val(self, devices, values):
         """Get devices to values dict."""
         # always use an iterable object
         if not isinstance(devices, (tuple, list)):
             devices = [devices, ]
```

### Comparing `siriuspy-2.72.0/siriuspy/devices/dvf.py` & `siriuspy-2.73.0/siriuspy/devices/dvf.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,33 +15,34 @@
         CAX_DVF1 = 'CAX:A:BASLER01'
         CAX_DVF2 = 'CAX:B:BASLER01'
         ALL = (CAX_DVF1, CAX_DVF2)
 
     _default_timeout = 10  # [s]
 
     _dvfparam_fields = (
+        'MAX_INTENSITY_NR_BITS',
         'ACQUISITION_TIME_MIN',  # [s]
         'ACQUISITION_TIME_DEFAULT',  # [s]
         'EXPOSURE_TIME_DEFAULT',  # [s]
         'IMAGE_SIZE_Y',  # [pixel]
         'IMAGE_SIZE_X',  # [pixel]
         'IMAGE_PIXEL_SIZE',  # [um]
         'OPTICS_MAGNIFICATION_FACTOR',  # source to image
     )
     #   DVF device :       ((sizey, sizex), pixel_size_um mag_factor
     _dev2params = {
         DEVICES.CAX_DVF1 :
             # DVF1 Today: pixel size 4.8 um; magnification factor 0.5
             _get_namedtuple('DVFParameters',
-            _dvfparam_fields, (0.5, 0.5, 0.005, 1024, 1280, 4.8, 0.5)),
+            _dvfparam_fields, (8, 0.5, 0.5, 0.005, 1024, 1280, 4.8, 0.5)),
         DEVICES.CAX_DVF2 :
             # DVF2 today: pixel size 4.8 um; magnification factor 5.0
             # DVF2 future hifi: pixel size 2.4 um; magnification factor 5.0
             _get_namedtuple('DVFParameters',
-            _dvfparam_fields, (0.5, 0.5, 0.005, 1024, 1280, 4.8, 5.0)),
+            _dvfparam_fields, (8, 0.5, 0.5, 0.005, 1024, 1280, 4.8, 5.0)),
         }
 
     _properties = (
         'ffmstream1:EnableCallbacks', 'ffmstream1:EnableCallbacks_RBV',
         'Trans1:EnableCallbacks', 'Trans1:EnableCallbacks_RBV',
         'cam1:ArrayCallbacks', 'cam1:ArrayCallbacks_RBV',
         'cam1:AcquireTime', 'cam1:AcquireTime_RBV',
@@ -69,14 +70,21 @@
 
     @property
     def parameters(self):
         """Return DVF parameters."""
         return DVF._dev2params[self.devname]
 
     @property
+    def intensity_saturation_value(self):
+        """Image intensity saturation value."""
+        # NOTE: a PV will be added to the IOC to select nr bits of intensity
+        intensity_nr_bits = self.parameters.MAX_INTENSITY_NR_BITS
+        return 2**intensity_nr_bits - 1
+
+    @property
     def exposure_time(self):
         """Camera exposure time [s]."""
         return self['cam1:AcquireTime']
 
     @exposure_time.setter
     def exposure_time(self, value):
         """Camera exposure time [s]."""
```

### Comparing `siriuspy-2.72.0/siriuspy/devices/egun.py` & `siriuspy-2.73.0/siriuspy/devices/egun.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/energy.py` & `siriuspy-2.73.0/siriuspy/devices/energy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/fofb.py` & `siriuspy-2.73.0/siriuspy/devices/fofb.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     DEVICES = _get_namedtuple('DEVICES', *zip(*_devices.items()))
 
 
 class FOFBCtrlRef(_Device, _FOFBCtrlBase):
     """FOFB reference orbit controller device."""
 
     _properties = (
-        'RefOrb-SP', 'RefOrb-RB',
+        'RefOrbX-SP', 'RefOrbX-RB',
+        'RefOrbY-SP', 'RefOrbY-RB',
         'MaxOrbDistortion-SP', 'MaxOrbDistortion-RB',
         'MaxOrbDistortionEnbl-Sel', 'MaxOrbDistortionEnbl-Sts',
         'MinBPMCnt-SP', 'MinBPMCnt-RB',
         'MinBPMCntEnbl-Sel', 'MinBPMCntEnbl-Sts',
         'LoopIntlk-Mon', 'LoopIntlkReset-Cmd',
     )
 
@@ -42,85 +43,40 @@
         if devname not in self.DEVICES:
             raise NotImplementedError(devname)
 
         # call base class constructor
         super().__init__(devname, properties=FOFBCtrlRef._properties)
 
     @property
-    def ref(self):
-        """Reference orbit, first half reference for X, second, for Y."""
-        ref = self['RefOrb-RB']
-        if ref is None:
-            return None
-        ref = ref.copy()
-        # handle initial state of RefOrb PVs
-        if len(ref) < 2*NR_BPM:
-            value = _np.zeros(2*NR_BPM, dtype=int)
-            value[:len(ref)] = ref
-            ref = value
-        return ref
-
-    @ref.setter
-    def ref(self, value):
-        self['RefOrb-SP'] = _np.array(value, dtype=int)
-
-    @property
     def refx(self):
         """Reference orbit X."""
-        return self.ref[:NR_BPM]
+        return self['RefOrbX-RB']
 
     @refx.setter
     def refx(self, value):
-        var = self.ref
-        var[:NR_BPM] = _np.array(value, dtype=int)
-        self.ref = var
+        self['RefOrbX-SP'] = _np.array(value, dtype=int)
 
     @property
     def refy(self):
         """Reference orbit Y."""
-        return self.ref[NR_BPM:]
+        return self['RefOrbY-RB']
 
     @refy.setter
     def refy(self, value):
-        var = self.ref
-        var[NR_BPM:] = _np.array(value, dtype=int)
-        self.ref = var
+        self['RefOrbY-SP'] = _np.array(value, dtype=int)
 
-    def set_ref(self, value):
-        """Set RefOrb."""
-        self.ref = value
-        return True
-
-    def set_refx(self, value):
-        """Set RefOrb X."""
-        self.refx = value
-        return True
-
-    def set_refy(self, value):
-        """Set RefOrb Y."""
-        self.refy = value
-        return True
-
-    def check_ref(self, value):
-        """Check whether RefOrb is equal to value."""
-        if not _np.all(self.ref == value):
+    def check_refx(self, value):
+        """Check whether RefOrbX is equal to value."""
+        if not _np.all(self.refx == value):
             return False
         return True
 
-    def check_refx(self, value):
-        """Check whether first half of RefOrb is equal to value."""
-        return self._check_reforbit('x', value)
-
     def check_refy(self, value):
-        """Check whether second half of RefOrb is equal to value."""
-        return self._check_reforbit('y', value)
-
-    def _check_reforbit(self, plane, value):
-        refval = getattr(self, 'ref'+plane.lower())
-        if not _np.all(refval == value):
+        """Check whether RefOrbY is equal to value."""
+        if not _np.all(self.refy == value):
             return False
         return True
 
     @property
     def max_orb_distortion(self):
         """Orbit distortion threshold [nm]."""
         return self['MaxOrbDistortion-RB']
@@ -172,15 +128,15 @@
 
     DEF_TIMEOUT = 1
     DEF_FMC_BPMCNT = NR_BPM
     DEF_P2P_BPMCNT = 8
 
     _properties = (
         'BPMId-SP', 'BPMId-RB', 'BPMCnt-Mon',
-        'CCEnable-SP', 'CCEnable-RB',
+        'CCEnable-Sel', 'CCEnable-Sts',
         'TimeFrameLen-SP', 'TimeFrameLen-RB',
     )
     _properties_fmc = (
         'LinkPartnerCH0-Mon', 'LinkPartnerCH1-Mon',
         'LinkPartnerCH2-Mon', 'LinkPartnerCH3-Mon',
     )
 
@@ -212,19 +168,19 @@
     def bpm_count(self):
         """BPM count."""
         return self['BPMCnt-Mon']
 
     @property
     def cc_enable(self):
         """Communication enable."""
-        return self['CCEnable-RB']
+        return self['CCEnable-Sts']
 
     @cc_enable.setter
     def cc_enable(self, value):
-        self['CCEnable-SP'] = value
+        self['CCEnable-Sel'] = value
 
     @property
     def time_frame_len(self):
         """Time frame length."""
         return self['TimeFrameLen-RB']
 
     @time_frame_len.setter
@@ -358,57 +314,41 @@
         return self._bpm_trgs
 
     @property
     def fofbevtdev(self):
         """FOFBS Event device."""
         return self._evt_fofb
 
-    def set_reforb(self, value):
-        """Set RefOrb for all FOFB controllers."""
-        for ctrl in self._ctl_refs.values():
-            ctrl.set_ref(value)
-        return True
-
     def set_reforbx(self, value):
         """Set RefOrbX for all FOFB controllers."""
-        return self._set_reforb('x', value)
+        for ctrl in self._ctl_refs.values():
+            ctrl.refx = value
+        return True
 
     def set_reforby(self, value):
         """Set RefOrbY for all FOFB controllers."""
-        return self._set_reforb('y', value)
-
-    def _set_reforb(self, plane, value):
         for ctrl in self._ctl_refs.values():
-            fun = getattr(ctrl, 'set_ref' + plane.lower())
-            fun(value)
+            ctrl.refy = value
         return True
 
-    def check_reforb(self, value):
-        """Check whether RefOrb is equal to value."""
+    def check_reforbx(self, value):
+        """Check whether RefOrbX is equal to value."""
         if not self.connected:
             return False
         for ctrl in self._ctl_refs.values():
-            if not ctrl.check_ref(value):
+            if not ctrl.check_refx(value):
                 return False
         return True
 
-    def check_reforbx(self, value):
-        """Check whether RefOrbX is equal to value."""
-        return self._check_reforb('x', value)
-
     def check_reforby(self, value):
         """Check whether RefOrbY is equal to value."""
-        return self._check_reforb('y', value)
-
-    def _check_reforb(self, plane, value):
         if not self.connected:
             return False
         for ctrl in self._ctl_refs.values():
-            fun = getattr(ctrl, 'check_ref' + plane.lower())
-            if not fun(value):
+            if not ctrl.check_refy(value):
                 return False
         return True
 
     @property
     def max_orb_distortion(self):
         """Orbit distortion threshold [nm].
 
@@ -597,26 +537,26 @@
         if bpms is None:
             bpms = self._bpmnames
         for bpm in bpms:
             enbdccs.append(self._bpm_dccs[bpm])
 
         # temporary solution: disable BPM DCCs that are not in FOFB network
         dcc2dsbl = list(self._bpmdcc2dsbl.values())
-        self._set_devices_propty(dcc2dsbl, 'CCEnable-SP', 0)
+        self._set_devices_propty(dcc2dsbl, 'CCEnable-Sel', 0)
         if not self._wait_devices_propty(
-                dcc2dsbl, 'CCEnable-RB', 0, timeout=timeout/2):
+                dcc2dsbl, 'CCEnable-Sts', 0, timeout=timeout/2):
             return False
 
-        self._set_devices_propty(alldccs, 'CCEnable-SP', 0)
+        self._set_devices_propty(alldccs, 'CCEnable-Sel', 0)
         if not self._wait_devices_propty(
-                alldccs, 'CCEnable-RB', 0, timeout=timeout/2):
+                alldccs, 'CCEnable-Sts', 0, timeout=timeout/2):
             return False
-        self._set_devices_propty(enbdccs, 'CCEnable-SP', 1)
+        self._set_devices_propty(enbdccs, 'CCEnable-Sel', 1)
         if not self._wait_devices_propty(
-                enbdccs, 'CCEnable-RB', 1, timeout=timeout/2):
+                enbdccs, 'CCEnable-Sts', 1, timeout=timeout/2):
             return False
         self._evt_fofb.cmd_external_trigger()
         return True
 
     def check_net_synced(self, bpms=None):
         """Check whether DCCs are synchronized."""
         if not self.connected:
@@ -925,36 +865,39 @@
         return False
 
     def set_invrespmat_row(self, values, psnames=None, psindices=None):
         """Command to set power supply correction coefficients value."""
         if not isinstance(values, (list, tuple, _np.ndarray)):
             raise ValueError('Value must be iterable.')
         devs = self._get_devices(psnames, psindices)
+        if not len(values) == len(devs):
+            raise ValueError('Values and indices must have the same size.')
         if any([len(v) != 2*NR_BPM for v in values]):
             raise ValueError(f'Value must have size {2*NR_BPM}.')
         for i, dev in enumerate(devs):
-            dev.invrespmat_row = values[i]
+            dev.invrespmat_row_x = values[i][:NR_BPM]
+            dev.invrespmat_row_y = values[i][NR_BPM:]
         return True
 
     def check_invrespmat_row(
             self, values, psnames=None, psindices=None,
             atol=DEF_ATOL_INVRESPMATROW):
         """Check power supplies correction coefficients."""
         if not self.connected:
             return False
         if not isinstance(values, (list, tuple, _np.ndarray)):
             raise ValueError('Value must be iterable.')
-        values = _np.asarray(values)
         devs = self._get_devices(psnames, psindices)
-        if not values.shape[0] == len(devs):
+        if not len(values) == len(devs):
             raise ValueError('Values and indices must have the same size.')
-        impltd = _np.asarray([d.invrespmat_row for d in devs])
-        if _np.allclose(values, impltd, atol=atol):
-            return True
-        return False
+        for i, dev in enumerate(devs):
+            impltd = _np.hstack([dev.invrespmat_row_x, dev.invrespmat_row_y])
+            if not _np.allclose(values[i], impltd, atol=atol):
+                return False
+        return True
 
     def set_fofbacc_gain(self, values, psnames=None, psindices=None):
         """Command to set power supply correction gain."""
         if not isinstance(values, (list, tuple, _np.ndarray)):
             raise ValueError('Value must be iterable.')
         devs = self._get_devices(psnames, psindices)
         for i, dev in enumerate(devs):
```

### Comparing `siriuspy-2.72.0/siriuspy/devices/ict.py` & `siriuspy-2.73.0/siriuspy/devices/ict.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/idff.py` & `siriuspy-2.73.0/siriuspy/devices/idff.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/ids.py` & `siriuspy-2.73.0/siriuspy/devices/ids.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/injctrl.py` & `siriuspy-2.73.0/siriuspy/devices/injctrl.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/injsys.py` & `siriuspy-2.73.0/siriuspy/devices/injsys.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/lienergy.py` & `siriuspy-2.73.0/siriuspy/devices/lienergy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/lillrf.py` & `siriuspy-2.73.0/siriuspy/devices/lillrf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/machshift.py` & `siriuspy-2.73.0/siriuspy/devices/machshift.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/modltr.py` & `siriuspy-2.73.0/siriuspy/devices/modltr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/orbit_interlock.py` & `siriuspy-2.73.0/siriuspy/devices/orbit_interlock.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/posang.py` & `siriuspy-2.73.0/siriuspy/devices/posang.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/psconv.py` & `siriuspy-2.73.0/siriuspy/devices/psconv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/pssofb.py` & `siriuspy-2.73.0/siriuspy/devices/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/pstesters.py` & `siriuspy-2.73.0/siriuspy/devices/pstesters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/pwrsupply.py` & `siriuspy-2.73.0/siriuspy/devices/pwrsupply.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,16 @@
         'CurrLoopMode-Sts', 'CurrLoopMode-Sel',
         'CurrGain-RB', 'CurrGain-SP', 'CurrOffset-RB', 'CurrOffset-SP',
         'Current-RB', 'Current-SP', 'Current-Mon', 'CurrentRef-Mon',
         'TestLimA-RB', 'TestLimA-SP', 'TestLimB-RB', 'TestLimB-SP',
         'TestWavePeriod-RB', 'TestWavePeriod-SP',
         'Voltage-RB', 'Voltage-SP', 'Voltage-Mon',
         'VoltGain-RB', 'VoltGain-SP', 'VoltOffset-RB', 'VoltOffset-SP',
-        'InvRespMatRow-SP', 'InvRespMatRow-RB',
+        'InvRespMatRowX-SP', 'InvRespMatRowX-RB',
+        'InvRespMatRowY-SP', 'InvRespMatRowY-RB',
         'FOFBAccGain-SP', 'FOFBAccGain-RB',
         'FOFBAccFreeze-Sel', 'FOFBAccFreeze-Sts',
         'FOFBAccClear-Cmd',
         'FOFBAccSatMax-SP', 'FOFBAccSatMax-RB',
         'FOFBAccSatMin-SP', 'FOFBAccSatMin-RB',
     )
     _properties_pulsed = (
@@ -906,21 +907,30 @@
         return self._set_opmode(mode=self.OPMODE_SEL.fofb, timeout=timeout)
 
     def _set_opmode(self, mode, timeout):
         self['OpMode-Sel'] = mode
         return self._wait('OpMode-Sts', mode, timeout=timeout)
 
     @property
-    def invrespmat_row(self):
-        """Correction coefficient value."""
-        return self['InvRespMatRow-RB']
-
-    @invrespmat_row.setter
-    def invrespmat_row(self, value):
-        self['InvRespMatRow-SP'] = _np.array(value, dtype=float)
+    def invrespmat_row_x(self):
+        """Horizontal correction coefficient value."""
+        return self['InvRespMatRowX-RB']
+
+    @invrespmat_row_x.setter
+    def invrespmat_row_x(self, value):
+        self['InvRespMatRowX-SP'] = _np.array(value, dtype=float)
+
+    @property
+    def invrespmat_row_y(self):
+        """Vertical correction coefficient value."""
+        return self['InvRespMatRowY-RB']
+
+    @invrespmat_row_y.setter
+    def invrespmat_row_y(self, value):
+        self['InvRespMatRowY-SP'] = _np.array(value, dtype=float)
 
     @property
     def fofbacc_gain(self):
         """FOFB accumulator gain."""
         return self['FOFBAccGain-RB']
 
     @fofbacc_gain.setter
```

### Comparing `siriuspy-2.72.0/siriuspy/devices/rf.py` & `siriuspy-2.73.0/siriuspy/devices/rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/screen.py` & `siriuspy-2.73.0/siriuspy/devices/screen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/sofb.py` & `siriuspy-2.73.0/siriuspy/devices/sofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/syncd.py` & `siriuspy-2.73.0/siriuspy/devices/syncd.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/devices/timing.py` & `siriuspy-2.73.0/siriuspy/devices/timing.py`

 * *Files 4% similar despite different names*

```diff
@@ -350,15 +350,17 @@
     @source.setter
     def source(self, value):
         self._enum_setter('Src-Sel', value, self._source_options)
 
     @property
     def source_str(self):
         """Source string."""
-        return self._source_options[self['Src-Sts']]
+        if self['Src-Sts'] is not None:
+            return self._source_options[self['Src-Sts']]
+        return
 
     @property
     def source_options(self):
         """Source options."""
         return self._source_options
 
     @property
@@ -526,22 +528,26 @@
         """."""
         map_evt2table = {n: o.mode_str for n, o in self.events.items()}
         map_table2evt = {}
         for k, v in map_evt2table.items():
             map_table2evt[v] = map_table2evt.get(v, []) + [k]
         return map_table2evt
 
-    def change_triggers_source(self, trigs, new_src='Linac') -> list:
+    def change_triggers_source(
+            self, trigs, new_src='Linac', printlog=True) -> list:
         """."""
         notchanged = list()
         for tn in trigs:
             tr = self.triggers[tn]
 
             if new_src not in tr.source_options:
-                print(f'{tn:25s} -> No Change: {new_src:s} is not an option.')
+                if printlog:
+                    print(
+                        f'{tn:25s} -> No Change: {new_src:s}'
+                        ' is not an option.')
                 notchanged.append(tn)
                 continue
 
             dly_newsrc = 0
             if new_src in self.events:
                 dly_newsrc = self.events[new_src].delay_raw
 
@@ -552,43 +558,47 @@
 
             dly = tr.delay_raw
             delta_dly = dly_oldsrc
             delta_dly -= dly_newsrc
             dly += delta_dly
             if dly < 0:
                 notchanged.append(tn)
-                print(f'{tn:25s} -> No Change: total delay not constant!')
+                if printlog:
+                    print(f'{tn:25s} -> No Change: total delay not constant!')
                 continue
 
             tr.delay_raw = dly
             tr.source = new_src
-            print(f'{tn:25s} -> Change OK: .')
+            if printlog:
+                print(f'{tn:25s} -> Change OK: .')
         return notchanged
 
-    def change_event_delay(self, new_dly, event='Linac'):
+    def change_event_delay(self, new_dly, event='Linac', printlog=True):
         """."""
         if event not in self.events:
-            print(f'{event} is not a valid event!')
+            if printlog:
+                print(f'{event} is not a valid event!')
             return False
         new_dly = int(new_dly)
         old_dly = self.events[event].delay_raw
         dlt_dly = old_dly - new_dly
 
         trigs = self.get_mapping_events2triggers()[event]
         for trn in trigs:
             dly = self.triggers[trn].delay_raw + dlt_dly
             if dly < 0:
-                print(f'cannot change delay: {trn:s} would change!')
+                if printlog:
+                    print(f'cannot change delay: {trn:s} would change!')
                 return False
 
         for trn in trigs:
             self.triggers[trn].delay_raw += dlt_dly
         self.events[event].delay_raw = new_dly
-
-        print('Delay changed!')
+        if printlog:
+            print('Delay changed!')
         return True
 
     def print_injtable_mapping(self, only_enabled=False):
         """."""
         map_evt2trig = self.get_mapping_events2triggers()
         map_table2evt = self.get_mapping_injtable2events()
         tabs = {'Continuous', 'Injection', 'OneShot'}
```

### Comparing `siriuspy-2.72.0/siriuspy/devices/tune.py` & `siriuspy-2.73.0/siriuspy/devices/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagbeam/bpm/csdev.py` & `siriuspy-2.73.0/siriuspy/diagbeam/bpm/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagbeam/dcct/csdev.py` & `siriuspy-2.73.0/siriuspy/diagbeam/dcct/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagbeam/ict/csdev.py` & `siriuspy-2.73.0/siriuspy/diagbeam/ict/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagbeam/screen/csdev.py` & `siriuspy-2.73.0/siriuspy/diagbeam/screen/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagbeam/slit/csdev.py` & `siriuspy-2.73.0/siriuspy/diagbeam/slit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagsys/app.py` & `siriuspy-2.73.0/siriuspy/diagsys/app.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagsys/lidiag/csdev.py` & `siriuspy-2.73.0/siriuspy/diagsys/lidiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagsys/lidiag/main.py` & `siriuspy-2.73.0/siriuspy/diagsys/lidiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagsys/lidiag/pvs.py` & `siriuspy-2.73.0/siriuspy/diagsys/lidiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagsys/psdiag/csdev.py` & `siriuspy-2.73.0/siriuspy/diagsys/psdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagsys/psdiag/main.py` & `siriuspy-2.73.0/siriuspy/diagsys/psdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagsys/psdiag/pvs.py` & `siriuspy-2.73.0/siriuspy/diagsys/psdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagsys/pudiag/csdev.py` & `siriuspy-2.73.0/siriuspy/diagsys/pudiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagsys/pudiag/main.py` & `siriuspy-2.73.0/siriuspy/diagsys/pudiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagsys/pudiag/pvs.py` & `siriuspy-2.73.0/siriuspy/diagsys/pudiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagsys/pvs.py` & `siriuspy-2.73.0/siriuspy/diagsys/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagsys/rfdiag/csdev.py` & `siriuspy-2.73.0/siriuspy/diagsys/rfdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagsys/rfdiag/main.py` & `siriuspy-2.73.0/siriuspy/diagsys/rfdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/diagsys/rfdiag/pvs.py` & `siriuspy-2.73.0/siriuspy/diagsys/rfdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/envars.py` & `siriuspy-2.73.0/siriuspy/envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/epics/multiproc.py` & `siriuspy-2.73.0/siriuspy/epics/multiproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/epics/properties.py` & `siriuspy-2.73.0/siriuspy/epics/properties.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/epics/pv_fake.py` & `siriuspy-2.73.0/siriuspy/epics/pv_fake.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/epics/pv_time_serie.py` & `siriuspy-2.73.0/siriuspy/epics/pv_time_serie.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/fofb/csdev.py` & `siriuspy-2.73.0/siriuspy/fofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/fofb/main.py` & `siriuspy-2.73.0/siriuspy/fofb/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,16 @@
 
         self._kick_buffer = []
         self._kick_buffer_size = self._const.DEF_KICK_BUFFER_SIZE
         for idx, pso in enumerate(self._corrs_dev.psdevs):
             pvo = pso.pv_object('CurrentRef-Mon')
             pvo.auto_monitor = True
             self._kick_buffer.append([])
-            pvo.add_callback(_part(self._update_kick_buffer, ps_index=idx))
+            pvo.add_callback(
+                _part(self._update_kick_buffer, ps_index=idx))
 
         self._rf_dev = _RFGen()
 
         self._llfofb_dev = _FamFOFBCtrls()
 
         self._intlk_pvs = list()
         self._intlk_values = dict()
@@ -198,17 +199,20 @@
             'MeasRespMatKickRF-SP': _part(self.set_respmat_meas_kick, 'rf'),
             'MeasRespMatWait-SP': self.set_respmat_meas_wait_time,
         }
 
         # configuration scanning
         self.quit = False
         self.scanning = False
-        self.thread_check_configs = _epics.ca.CAThread(
-            target=self._check_configs, daemon=True)
-        self.thread_check_configs.start()
+        self.thread_check_corrs_configs = _epics.ca.CAThread(
+            target=self._check_corrs_configs, daemon=True)
+        self.thread_check_corrs_configs.start()
+        self.thread_check_ctrls_configs = _epics.ca.CAThread(
+            target=self._check_ctrls_configs, daemon=True)
+        self.thread_check_ctrls_configs.start()
 
     def init_database(self):
         """Set initial PV values."""
         self.run_callbacks('LoopState-Sel', self._loop_state)
         self.run_callbacks('LoopState-Sts', self._loop_state)
         self.run_callbacks('LoopGainH-SP', self._loop_gain_h)
         self.run_callbacks('LoopGainH-RB', self._loop_gain_h)
@@ -874,18 +878,19 @@
 
     def cmd_fofbctrl_syncreforb(self, _):
         """Sync FOFB RefOrb command."""
         self._update_log('Received sync FOFB RefOrb command...')
         if not self._check_fofbctrl_connection():
             return False
         self._update_log('Checking...')
-        reforb = _np.hstack([self._reforbhw_x, self._reforbhw_y])
-        if not self._llfofb_dev.check_reforb(reforb):
+        if not self._llfofb_dev.check_reforbx(self._reforbhw_x) or not \
+                self._llfofb_dev.check_reforby(self._reforbhw_y):
             self._update_log('Syncing FOFB RefOrb...')
-            self._llfofb_dev.set_reforb(reforb)
+            self._llfofb_dev.set_reforbx(self._reforbhw_x)
+            self._llfofb_dev.set_reforby(self._reforbhw_y)
             self._update_log('...done!')
         else:
             self._update_log('FOFB RefOrb already synced.')
 
         self._fofbctrl_syncref_count += 1
         self.run_callbacks(
             'CtrlrSyncRefOrb-Cmd', self._fofbctrl_syncref_count)
@@ -1074,14 +1079,18 @@
         setattr(self, '_reforb_' + plane.lower(), ref)
         # hardware units
         refhw = ref * self._const.CONV_UM_2_NM
         refhw = _np.round(refhw)  # round, low level expect it to be int
         refhw = _np.roll(refhw, 1)  # make BPM 01M1 the first element
         setattr(self, '_reforbhw_' + plane.lower(), refhw)
 
+        # set reforb to FOFB controllers
+        func = getattr(self._llfofb_dev, 'set_reforb' + plane.lower())
+        func(refhw)
+
         # update readback PV
         self.run_callbacks(f'RefOrb{plane.upper()}-RB', list(ref.ravel()))
         self.run_callbacks(f'RefOrbHw{plane.upper()}-Mon', refhw)
         self._update_log('...done!')
         return True
 
     # --- matrix manipulation ---
@@ -1833,15 +1842,15 @@
             _log.error(msg[6:])
         elif 'WARN' in msg:
             _log.warning(msg[5:])
         else:
             _log.info(msg)
         self.run_callbacks('Log-Mon', msg)
 
-    def _check_configs(self):
+    def _check_corrs_configs(self):
         tplanned = 1.0/App.SCAN_FREQUENCY
         while not self.quit:
             if not self.scanning:
                 _time.sleep(tplanned)
                 continue
 
             _t0 = _time.time()
@@ -1884,30 +1893,48 @@
                     value = _updt_bit(value, 6, 1)
             else:
                 value = 0b1111111
 
             self._corr_status = value
             self.run_callbacks('CorrStatus-Mon', self._corr_status)
 
+            ttook = _time.time() - _t0
+            tsleep = tplanned - ttook
+            if tsleep > 0:
+                _time.sleep(tsleep)
+            else:
+                _log.warning(
+                    'Corrector configuration check took more than planned... '
+                    '{0:.3f}/{1:.3f} s'.format(ttook, tplanned))
+
+    def _check_ctrls_configs(self):
+        tplanned = 1.0/App.SCAN_FREQUENCY
+        while not self.quit:
+            if not self.scanning:
+                _time.sleep(tplanned)
+                continue
+
+            _t0 = _time.time()
+
             # FOFB controllers status
             value = 0
             if self._llfofb_dev.connected:
                 # BPMIdsConfigured
                 if not self._llfofb_dev.bpm_id_configured:
                     value = _updt_bit(value, 1, 1)
                 # NetSynced
                 bpms = self._get_fofbctrl_bpmdcc_enbl()
                 if not self._llfofb_dev.check_net_synced(bpms=bpms):
                     value = _updt_bit(value, 2, 1)
                 # LinkPartnerConnected
                 if not self._llfofb_dev.linkpartners_connected:
                     value = _updt_bit(value, 3, 1)
                 # RefOrbSynced
-                reforb = _np.hstack([self._reforbhw_x, self._reforbhw_y])
-                if not self._llfofb_dev.check_reforb(reforb):
+                if not self._llfofb_dev.check_reforbx(self._reforbhw_x) or not\
+                        self._llfofb_dev.check_reforby(self._reforbhw_y):
                     value = _updt_bit(value, 4, 1)
                 # TimeFrameLenSynced
                 tframelen = self._time_frame_len
                 if not _np.all(self._llfofb_dev.time_frame_len == tframelen):
                     value = _updt_bit(value, 5, 1)
                 # BPMLogTrigsConfigured
                 if not self._llfofb_dev.bpm_trigs_configured:
@@ -1937,9 +1964,9 @@
 
             ttook = _time.time() - _t0
             tsleep = tplanned - ttook
             if tsleep > 0:
                 _time.sleep(tsleep)
             else:
                 _log.warning(
-                    'Configuration check took more than planned... '
+                    'Controllers configuration check took more than planned... '
                     '{0:.3f}/{1:.3f} s'.format(ttook, tplanned))
```

### Comparing `siriuspy-2.72.0/siriuspy/idff/config.py` & `siriuspy-2.73.0/siriuspy/idff/config.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/injctrl/bias_feedback.py` & `siriuspy-2.73.0/siriuspy/injctrl/bias_feedback.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/injctrl/csdev.py` & `siriuspy-2.73.0/siriuspy/injctrl/csdev.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     PUMODE = ('Accumulation', 'Optimization', 'OnAxis')
     PUMODE_MON = PUMODE + ('Undefined', )
     TOPUPSTS = (
         'Off', 'Waiting', 'TurningOn', 'Injecting', 'TurningOff', 'Skipping')
     INJSYSCMDSTS = ('Idle', 'On', 'Off')
     RFKILLBEAMMON = ('Idle', 'Kill')
     IDLERUNNING = ('Idle', 'Running')
+    IDLEINJECTING = ('Idle', 'Injecting')
     BIASFB_MODEL_TYPES = ('Linear', 'GaussianProcess')
+    STANDBY_INJECT = ('Standby', 'Inject')
 
 
 _et = ETypes
 
 
 # --- Const class ---
 
@@ -34,16 +36,18 @@
     InjTypeMon = _csdev.Const.register('InjTypeMon', _et.INJTYPE_MON)
     PUMode = _csdev.Const.register('PUMode', _et.PUMODE)
     PUModeMon = _csdev.Const.register('PUModeMon', _et.PUMODE_MON)
     TopUpSts = _csdev.Const.register('TopUpSts', _et.TOPUPSTS)
     InjSysCmdSts = _csdev.Const.register('InjSysCmdSts', _et.INJSYSCMDSTS)
     RFKillBeamMon = _csdev.Const.register('RFKillBeamMon', _et.RFKILLBEAMMON)
     IdleRunning = _csdev.Const.register('IdleRunning', _et.IDLERUNNING)
+    IdleInjecting = _csdev.Const.register('IdleInjecting', _et.IDLEINJECTING)
     BiasFBModelTypes = _csdev.Const.register(
         'ModelTypes', _et.BIASFB_MODEL_TYPES)
+    StandbyInject = _csdev.Const.register('StandbyInject', _et.STANDBY_INJECT)
 
     GEN_STATUS_LABELS = ('LI', 'TB', 'BO', 'TS', 'SI', 'AS')
     LI_STATUS_LABELS = ('Egun', 'PS', 'PU', 'RF', 'TI')
     TL_STATUS_LABELS = ('PS', 'PU', 'TI')
     SR_STATUS_LABELS = ('PS', 'PU', 'RF', 'TI')
     AS_STATUS_LABELS = ('TI', )
     INJ_STATUS_LABELS = (
@@ -68,17 +72,14 @@
     BIAS_MULTI_BUNCH = -56.0  # [V]
     FILACURR_OPVALUE = 1.39  # [A]
     HV_OPVALUE = 90.0  # [kV]
 
     INJSYS_DEF_ON_ORDER = ['bo_rf', 'as_pu', 'bo_ps', 'injbo', 'li_rf']
     INJSYS_DEF_OFF_ORDER = ['bo_rf', 'li_rf', 'injbo', 'as_pu', 'bo_ps']
 
-    PU_VOLTAGE_UP_TIME = 30  # [s]
-    LI_STDBY_CONF_TIME = 30  # [s]
-
     BIASFB_AHEADSETIME = 10  # [s]
     BIASFB_MINIMUM_LIFETIME = 1800  # [s]
     BIASFB_PROPTY_PREFIX = 'BiasFB'
     BIASFB_MAX_DATA_SIZE = 1000
 
 
 _ct = Const
@@ -226,14 +227,29 @@
             'lolim': _ct.MIN_BKT, 'hilim': _ct.MAX_BKT},
         'BucketListStep-SP': {
             'type': 'int', 'value': 15, 'unit': 'buckets',
             'lolim': -_ct.MAX_BKT+1, 'hilim': _ct.MAX_BKT-1},
         'BucketListStep-RB': {
             'type': 'int', 'value': 15, 'unit': 'buckets',
             'lolim': -_ct.MAX_BKT+1, 'hilim': _ct.MAX_BKT-1},
+        'IsInjecting-Mon': {
+            'type': 'enum', 'value': _ct.IdleInjecting.Idle,
+            'enums': _et.IDLEINJECTING, 'unit': 'Idle_Inj'},
+        'IsInjDelay-SP': {
+            'type': 'int', 'value': 0, 'unit': 'ms',
+            'lolim': 0, 'hilim': 1000},
+        'IsInjDelay-RB': {
+            'type': 'int', 'value': 0, 'unit': 'ms',
+            'lolim': 0, 'hilim': 1000},
+        'IsInjDuration-SP': {
+            'type': 'int', 'value': 300, 'unit': 'ms',
+            'lolim': 0, 'hilim': 1000},
+        'IsInjDuration-RB': {
+            'type': 'int', 'value': 300, 'unit': 'ms',
+            'lolim': 0, 'hilim': 1000},
 
         'TopUpState-Sel': {
             'type': 'enum', 'value': _ct.OffOn.Off,
             'enums': _et.OFF_ON, 'unit': 'Off_On'},
         'TopUpState-Sts': {
             'type': 'enum', 'value': _ct.TopUpSts.Off, 'enums': _et.TOPUPSTS,
             'unit': 'Off_Wai_TOn_Inj_TOff_Skip'},
@@ -251,20 +267,56 @@
             'lolim': 0, 'hilim': 2*60},
         'TopUpPUStandbyEnbl-Sel': {
             'type': 'enum', 'value': _ct.DsblEnbl.Dsbl,
             'enums': _et.DSBL_ENBL, 'unit': 'Dsbl_Enbl'},
         'TopUpPUStandbyEnbl-Sts': {
             'type': 'enum', 'value': _ct.DsblEnbl.Dsbl,
             'enums': _et.DSBL_ENBL, 'unit': 'Dsbl_Enbl'},
-        'TopUpLIStandbyEnbl-Sel': {
+        'TopUpPUWarmUpTime-SP': {
+            'type': 'float', 'value': 30, 'unit': 's', 'prec': 1,
+            'lolim': 0, 'hilim': 2*60},
+        'TopUpPUWarmUpTime-RB': {
+            'type': 'float', 'value': 30, 'unit': 's', 'prec': 1,
+            'lolim': 0, 'hilim': 2*60},
+        'TopUpLIWarmUpEnbl-Sel': {
+            'type': 'enum', 'value': _ct.DsblEnbl.Dsbl,
+            'enums': _et.DSBL_ENBL, 'unit': 'Dsbl_Enbl'},
+        'TopUpLIWarmUpEnbl-Sts': {
+            'type': 'enum', 'value': _ct.DsblEnbl.Dsbl,
+            'enums': _et.DSBL_ENBL, 'unit': 'Dsbl_Enbl'},
+        'TopUpLIWarmUpTime-SP': {
+            'type': 'float', 'value': 30, 'unit': 's', 'prec': 1,
+            'lolim': 0, 'hilim': 2*60},
+        'TopUpLIWarmUpTime-RB': {
+            'type': 'float', 'value': 30, 'unit': 's', 'prec': 1,
+            'lolim': 0, 'hilim': 2*60},
+        'TopUpBOPSStandbyEnbl-Sel': {
             'type': 'enum', 'value': _ct.DsblEnbl.Dsbl,
             'enums': _et.DSBL_ENBL, 'unit': 'Dsbl_Enbl'},
-        'TopUpLIStandbyEnbl-Sts': {
+        'TopUpBOPSStandbyEnbl-Sts': {
             'type': 'enum', 'value': _ct.DsblEnbl.Dsbl,
             'enums': _et.DSBL_ENBL, 'unit': 'Dsbl_Enbl'},
+        'TopUpBOPSWarmUpTime-SP': {
+            'type': 'float', 'value': 10, 'unit': 's', 'prec': 1,
+            'lolim': 0, 'hilim': 2*60},
+        'TopUpBOPSWarmUpTime-RB': {
+            'type': 'float', 'value': 10, 'unit': 's', 'prec': 1,
+            'lolim': 0, 'hilim': 2*60},
+        'TopUpBORFStandbyEnbl-Sel': {
+            'type': 'enum', 'value': _ct.DsblEnbl.Dsbl,
+            'enums': _et.DSBL_ENBL, 'unit': 'Dsbl_Enbl'},
+        'TopUpBORFStandbyEnbl-Sts': {
+            'type': 'enum', 'value': _ct.DsblEnbl.Dsbl,
+            'enums': _et.DSBL_ENBL, 'unit': 'Dsbl_Enbl'},
+        'TopUpBORFWarmUpTime-SP': {
+            'type': 'float', 'value': 10, 'unit': 's', 'prec': 1,
+            'lolim': 0, 'hilim': 2*60},
+        'TopUpBORFWarmUpTime-RB': {
+            'type': 'float', 'value': 10, 'unit': 's', 'prec': 1,
+            'lolim': 0, 'hilim': 2*60},
         'TopUpNextInj-Mon': {
             'type': 'float', 'value': 0.0, 'unit': 's'},
         'TopUpNrPulses-SP': {
             'type': 'int', 'value': 1, 'unit': 'pulses',
             'lolim': _ct.MIN_BKT, 'hilim': _ct.MAX_BKT},
         'TopUpNrPulses-RB': {
             'type': 'int', 'value': 1, 'unit': 'pulses',
```

### Comparing `siriuspy-2.72.0/siriuspy/injctrl/main.py` & `siriuspy-2.73.0/siriuspy/injctrl/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,27 +57,39 @@
             },
         }
         self._thread_watdev = None
         self._target_current = 100.0
         self._bucketlist_start = 1
         self._bucketlist_stop = 864
         self._bucketlist_step = 15
+        self._isinj_delay = 0
+        self._isinj_duration = 300
 
-        self._topupstate_sel = _Const.OffOn.Off
-        self._topupstate_sts = _Const.TopUpSts.Off
-        self._topupperiod = 5*60  # [s]
-        self._topupheadstarttime = 0
-        self._topuppustandbyenbl = _Const.DsblEnbl.Dsbl
-        self._topuplistandbyenbl = _Const.DsblEnbl.Dsbl
+        self._topup_state_sel = _Const.OffOn.Off
+        self._topup_state_sts = _Const.TopUpSts.Off
+        self._topup_period = 5*60  # [s]
+        self._topup_headstarttime = 0
+        self._topup_pustandbyenbl = _Const.DsblEnbl.Dsbl
+        self._topup_puwarmuptime = 30
+        self._topup_pu_prepared = True
+        self._topup_liwarmupenbl = _Const.DsblEnbl.Dsbl
+        self._topup_liwarmuptime = 30
+        self._topup_li_prepared = True
+        self._topup_bopsstandbyenbl = _Const.DsblEnbl.Dsbl
+        self._topup_bopswarmuptime = 10
+        self._topup_bops_prepared = True
+        self._topup_borfstandbyenbl = _Const.DsblEnbl.Dsbl
+        self._topup_borfwarmuptime = 10
+        self._topup_borf_prepared = True
         now = _Time.now().timestamp()
-        self._topupnext = now - (now % (24*60*60)) + 3*60*60
-        self._topupnrpulses = 1
+        self._topup_next = now - (now % (24*60*60)) + 3*60*60
+        self._topup_nrpulses = 1
         self._topup_thread = None
-        self._topup_pu_prepared = False
         self._abort = False
+        self._setting_mode = False
 
         self._rfkillbeam_mon = _Const.RFKillBeamMon.Idle
 
         self._thread_autostop = None
 
         secs = ['LI', 'TB', 'BO', 'TS', 'SI', 'AS']
         self._status = {
@@ -129,14 +141,28 @@
                     for n in _LIDiagConst.DEV_2_LINAME if 'EG' in n}
 
             if sec in ['BO', 'SI']:
                 self._pvs_diag[sec]['RF'] = {
                     n: _PV(n+':DiagStatus-Mon', connection_timeout=0.05)
                     for n in _RFDiagConst.ALL_DEVICES if n.startswith(sec)}
 
+        # auxiliary injsys PVs
+        self._pvs_injsys = dict()
+        punames = _PSSearch.get_psnames({
+            'sec': '(SI|TS)', 'dev': 'Inj(Sept.*|NLKckr)',
+            'propty_name': '(?!:CCoil).*'})
+        for pun in punames:
+            pv_pulse = _PV(pun+':Pulse-Sts', connection_timeout=0.05)
+            pv_trigg = _PV(
+                pun.replace('PU', 'TI')+':State-Sts', connection_timeout=0.05)
+            self._pvs_injsys[pun] = [pv_pulse, pv_trigg]
+        ffname = _HLTimeSearch.get_hl_triggers({'sec': 'SI', 'idx': 'FF.*'})[0]
+        self._pvs_injsys[ffname] = [
+            _PV(ffname+':State-Sts', connection_timeout=0.05), ]
+
         # auxiliary devices
         self.egun_dev = EGun(
             print_log=False, callback=self._update_dev_status)
         self._init_egun = False
         self.egun_dev.trigps.pv_object('enable').add_callback(
             self._callback_watch_eguntrig)
 
@@ -145,14 +171,17 @@
 
         self._evg_dev = EVG()
         self._init_injevt = False
         self._evg_dev.pv_object('InjectionEvt-Sel').add_callback(
             self._callback_watch_injectionevt)
         self._evg_dev.pv_object('RepeatBucketList-RB').add_callback(
             self._callback_watch_repeatbucketlist)
+        self._evg_dev.set_auto_monitor('TotalInjCount-Mon', True)
+        self._evg_dev.pv_object('TotalInjCount-Mon').add_callback(
+            self._callback_is_injecting)
 
         self._injsys_dev = InjSysStandbyHandler()
 
         self.currinfo_dev = CurrInfoSI()
         self.currinfo_dev.set_auto_monitor('Current-Mon', True)
         curr_pvo = self.currinfo_dev.pv_object('Current-Mon')
         curr_pvo.add_callback(self._callback_autostop)
@@ -170,14 +199,23 @@
             pvo.add_callback(self._callback_update_pu_refvolt)
 
         self._rfkillbeam = RFKillBeam()
 
         self._li_trig_names = _HLTimeSearch.get_hl_triggers(
             {'sec': 'LI', 'dev': '(Mod|LLRF|SSAmp|Osc)'})
         self._li_trig_devs = [Trigger(tin) for tin in self._li_trig_names]
+
+        self._bops_trig_names = _HLTimeSearch.get_hl_triggers(
+            {'sec': 'BO', 'dev': 'Mags'})
+        self._bops_trig_devs = [Trigger(tin) for tin in self._bops_trig_names]
+
+        self._borf_trig_names = _HLTimeSearch.get_hl_triggers(
+            {'sec': 'BO', 'dev': 'LLRF', 'idx': 'Rmp'})
+        self._borf_trig_devs = [Trigger(tin) for tin in self._borf_trig_names]
+
         self._hlti_dev = HLTiming()
 
         # pvname to write method map
         self.map_pv2write = {
             'Mode-Sel': self.set_mode,
             'Type-Sel': self.set_type,
             'SglBunBiasVolt-SP': self.set_sglbunbiasvolt,
@@ -188,20 +226,28 @@
             'PUModeDeltaPosAng-SP': self.set_pumode_delta_posang,
             'PUModeDpKckrDlyRef-SP': self.set_pumode_dpkckr_dlyref,
             'PUModeDpKckrKick-SP': self.set_pumode_dpkckr_kick,
             'TargetCurrent-SP': self.set_target_current,
             'BucketListStart-SP': self.set_bucketlist_start,
             'BucketListStop-SP': self.set_bucketlist_stop,
             'BucketListStep-SP': self.set_bucketlist_step,
-            'TopUpState-Sel': self.set_topupstate,
-            'TopUpPeriod-SP': self.set_topupperiod,
-            'TopUpHeadStartTime-SP': self.set_topupheadstarttime,
-            'TopUpPUStandbyEnbl-Sel': self.set_topuppustandbyenbl,
-            'TopUpLIStandbyEnbl-Sel': self.set_topuplistandbyenbl,
-            'TopUpNrPulses-SP': self.set_topupnrpulses,
+            'IsInjDelay-SP': self.set_isinj_delay,
+            'IsInjDuration-SP': self.set_isinj_duration,
+            'TopUpState-Sel': self.set_topup_state,
+            'TopUpPeriod-SP': self.set_topup_period,
+            'TopUpHeadStartTime-SP': self.set_topup_headstarttime,
+            'TopUpPUStandbyEnbl-Sel': self.set_topup_pustandbyenbl,
+            'TopUpPUWarmUpTime-SP': self.set_topup_puwarmuptime,
+            'TopUpLIWarmUpEnbl-Sel': self.set_topup_liwarmupenbl,
+            'TopUpLIWarmUpTime-SP': self.set_topup_liwarmuptime,
+            'TopUpBOPSStandbyEnbl-Sel': self.set_topup_bopsstandbyenbl,
+            'TopUpBOPSWarmUpTime-SP': self.set_topup_bopswarmuptime,
+            'TopUpBORFStandbyEnbl-Sel': self.set_topup_borfstandbyenbl,
+            'TopUpBORFWarmUpTime-SP': self.set_topup_borfwarmuptime,
+            'TopUpNrPulses-SP': self.set_topup_nrpulses,
             'InjSysTurnOn-Cmd': self.cmd_injsys_turn_on,
             'InjSysTurnOff-Cmd': self.cmd_injsys_turn_off,
             'InjSysTurnOnOrder-SP': self.set_injsys_on_order,
             'InjSysTurnOffOrder-SP': self.set_injsys_off_order,
             'RFKillBeam-Cmd': self.cmd_rfkillbeam,
         }
 
@@ -244,16 +290,88 @@
         self._pvs_database.update(self._bias_feedback.database)
         for prop, write in self._bias_feedback.map_pv2write.items():
             pvname = _Const.BIASFB_PROPTY_PREFIX + prop
             self.map_pv2write[pvname] = write
 
     def init_database(self):
         """Set initial PV values."""
-        self.run_callbacks('Mode-Sel', self._mode)
-        self.run_callbacks('Mode-Sts', self._mode)
+        pvn2vals = {
+            'Mode-Sel': self._mode,
+            'Mode-Sts': self._mode,
+            'TypeCmdSts-Mon': self._p2w['Type']['status'],
+            'SglBunBiasVolt-SP': self._sglbunbiasvolt,
+            'SglBunBiasVolt-RB': self._sglbunbiasvolt,
+            'MultBunBiasVolt-SP': self._multbunbiasvolt,
+            'MultBunBiasVolt-RB': self._multbunbiasvolt,
+            'BiasVoltCmdSts-Mon': _Const.IdleRunning.Idle,
+            'FilaOpCurr-SP': self._filaopcurr,
+            'FilaOpCurr-RB': self._filaopcurr,
+            'FilaOpCurrCmdSts-Mon': self._p2w['FilaOpCurr']['status'],
+            'HVOpVolt-SP': self._hvopvolt,
+            'HVOpVolt-RB': self._hvopvolt,
+            'HVOpVoltCmdSts-Mon': self._p2w['HVOpVolt']['status'],
+            'PUModeDeltaPosAng-SP': self._pumode_dev.delta_posang,
+            'PUModeDeltaPosAng-RB': self._pumode_dev.delta_posang,
+            'PUModeDpKckrDlyRef-SP': self._pumode_dev.dpkckr_dlyref,
+            'PUModeDpKckrDlyRef-RB': self._pumode_dev.dpkckr_dlyref,
+            'PUModeDpKckrKick-SP': self._pumode_dev.dpkckr_kick,
+            'PUModeDpKckrKick-RB': self._pumode_dev.dpkckr_kick,
+            'PUModeCmdSts-Mon': self._p2w['PUMode']['status'],
+            'TargetCurrent-SP': self._target_current,
+            'TargetCurrent-RB': self._target_current,
+            'BucketListStart-SP': self._bucketlist_start,
+            'BucketListStart-RB': self._bucketlist_start,
+            'BucketListStop-SP': self._bucketlist_stop,
+            'BucketListStop-RB': self._bucketlist_stop,
+            'BucketListStep-SP': self._bucketlist_step,
+            'BucketListStep-RB': self._bucketlist_step,
+            'IsInjecting-Mon': _Const.IdleInjecting.Idle,
+            'IsInjDelay-SP': self._isinj_delay,
+            'IsInjDelay-RB': self._isinj_delay,
+            'IsInjDuration-SP': self._isinj_duration,
+            'IsInjDuration-RB': self._isinj_duration,
+            'TopUpState-Sel': self._topup_state_sel,
+            'TopUpState-Sts': self._topup_state_sts,
+            'TopUpPeriod-SP': self._topup_period/60,
+            'TopUpPeriod-RB': self._topup_period/60,
+            'TopUpHeadStartTime-SP': self._topup_headstarttime,
+            'TopUpHeadStartTime-RB': self._topup_headstarttime,
+            'TopUpPUStandbyEnbl-Sel': self._topup_pustandbyenbl,
+            'TopUpPUStandbyEnbl-Sts': self._topup_pustandbyenbl,
+            'TopUpPUWarmUpTime-SP': self._topup_puwarmuptime,
+            'TopUpPUWarmUpTime-RB': self._topup_puwarmuptime,
+            'TopUpLIWarmUpEnbl-Sel': self._topup_liwarmupenbl,
+            'TopUpLIWarmUpEnbl-Sts': self._topup_liwarmupenbl,
+            'TopUpLIWarmUpTime-SP': self._topup_liwarmuptime,
+            'TopUpLIWarmUpTime-RB': self._topup_liwarmuptime,
+            'TopUpBOPSStandbyEnbl-Sel': self._topup_bopsstandbyenbl,
+            'TopUpBOPSStandbyEnbl-Sts': self._topup_bopsstandbyenbl,
+            'TopUpBOPSWarmUpTime-SP': self._topup_bopswarmuptime,
+            'TopUpBOPSWarmUpTime-RB': self._topup_bopswarmuptime,
+            'TopUpBORFStandbyEnbl-Sel': self._topup_bopsstandbyenbl,
+            'TopUpBORFStandbyEnbl-Sts': self._topup_bopsstandbyenbl,
+            'TopUpBORFWarmUpTime-SP': self._topup_bopswarmuptime,
+            'TopUpBORFWarmUpTime-RB': self._topup_bopswarmuptime,
+            'TopUpNextInj-Mon': self._topup_next,
+            'TopUpNrPulses-SP': self._topup_nrpulses,
+            'TopUpNrPulses-RB': self._topup_nrpulses,
+            'InjSysCmdDone-Mon': ','.join(self._injsys_dev.done),
+            'InjSysCmdSts-Mon': _Const.InjSysCmdSts.Idle,
+            'RFKillBeam-Mon': _Const.RFKillBeamMon.Idle,
+            'DiagStatusLI-Mon': self._status['LI'],
+            'DiagStatusTB-Mon': self._status['TB'],
+            'DiagStatusBO-Mon': self._status['BO'],
+            'DiagStatusTS-Mon': self._status['TS'],
+            'DiagStatusSI-Mon': self._status['SI'],
+            'DiagStatus-Mon': self._status['AS'],
+            'InjStatus-Mon': self._injstatus,
+        }
+        for pvn, val in pvn2vals.items():
+            self.run_callbacks(pvn, val)
+
         self._callback_update_type(init=True)
         self.egun_dev.pulse.pv_object('multiselstatus').add_callback(
             self._callback_update_type)
         self.egun_dev.pulse.pv_object('multiswstatus').add_callback(
             self._callback_update_type)
         self.egun_dev.pulse.pv_object('singleselstatus').add_callback(
             self._callback_update_type)
@@ -261,28 +379,14 @@
             self._callback_update_type)
         self.egun_dev.trigmultipre.pv_object('State-Sts').add_callback(
             self._callback_update_type)
         self.egun_dev.trigmulti.pv_object('State-Sts').add_callback(
             self._callback_update_type)
         self.egun_dev.trigsingle.pv_object('State-Sts').add_callback(
             self._callback_update_type)
-        self.run_callbacks('TypeCmdSts-Mon', self._p2w['Type']['status'])
-        self.run_callbacks('SglBunBiasVolt-SP', self._sglbunbiasvolt)
-        self.run_callbacks('SglBunBiasVolt-RB', self._sglbunbiasvolt)
-        self.run_callbacks('MultBunBiasVolt-SP', self._multbunbiasvolt)
-        self.run_callbacks('MultBunBiasVolt-RB', self._multbunbiasvolt)
-        self.run_callbacks('BiasVoltCmdSts-Mon', _Const.IdleRunning.Idle)
-        self.run_callbacks('FilaOpCurr-SP', self._filaopcurr)
-        self.run_callbacks('FilaOpCurr-RB', self._filaopcurr)
-        self.run_callbacks(
-            'FilaOpCurrCmdSts-Mon', self._p2w['FilaOpCurr']['status'])
-        self.run_callbacks('HVOpVolt-SP', self._hvopvolt)
-        self.run_callbacks('HVOpVolt-RB', self._hvopvolt)
-        self.run_callbacks(
-            'HVOpVoltCmdSts-Mon', self._p2w['HVOpVolt']['status'])
         self._callback_update_pumode(init=True)
         self._pumode_dev.trigdpk.pv_object('Src-Sts').add_callback(
             self._callback_update_pumode)
         self._pumode_dev.trigdpk.pv_object('DelayRaw-RB').add_callback(
             self._callback_update_pumode)
         self._pumode_dev.pudpk.pv_object('Kick-RB').add_callback(
             self._callback_update_pumode)
@@ -290,57 +394,14 @@
             self._callback_update_pumode)
         self._pumode_dev.pudpk.pv_object('Pulse-Sts').add_callback(
             self._callback_update_pumode)
         self._pumode_dev.punlk.pv_object('PwrState-Sts').add_callback(
             self._callback_update_pumode)
         self._pumode_dev.punlk.pv_object('Pulse-Sts').add_callback(
             self._callback_update_pumode)
-        self.run_callbacks(
-            'PUModeDeltaPosAng-SP', self._pumode_dev.delta_posang)
-        self.run_callbacks(
-            'PUModeDeltaPosAng-RB', self._pumode_dev.delta_posang)
-        self.run_callbacks(
-            'PUModeDpKckrDlyRef-SP', self._pumode_dev.dpkckr_dlyref)
-        self.run_callbacks(
-            'PUModeDpKckrDlyRef-RB', self._pumode_dev.dpkckr_dlyref)
-        self.run_callbacks('PUModeDpKckrKick-SP', self._pumode_dev.dpkckr_kick)
-        self.run_callbacks('PUModeDpKckrKick-RB', self._pumode_dev.dpkckr_kick)
-        self.run_callbacks('PUModeCmdSts-Mon', self._p2w['PUMode']['status'])
-        self.run_callbacks('TargetCurrent-SP', self._target_current)
-        self.run_callbacks('TargetCurrent-RB', self._target_current)
-        self.run_callbacks('BucketListStart-SP', self._bucketlist_start)
-        self.run_callbacks('BucketListStart-RB', self._bucketlist_start)
-        self.run_callbacks('BucketListStop-SP', self._bucketlist_stop)
-        self.run_callbacks('BucketListStop-RB', self._bucketlist_stop)
-        self.run_callbacks('BucketListStep-SP', self._bucketlist_step)
-        self.run_callbacks('BucketListStep-RB', self._bucketlist_step)
-        self.run_callbacks('TopUpState-Sel', self._topupstate_sel)
-        self.run_callbacks('TopUpState-Sts', self._topupstate_sts)
-        self.run_callbacks('TopUpPeriod-SP', self._topupperiod/60)
-        self.run_callbacks('TopUpPeriod-RB', self._topupperiod/60)
-        self.run_callbacks('TopUpHeadStartTime-SP', self._topupheadstarttime)
-        self.run_callbacks('TopUpHeadStartTime-RB', self._topupheadstarttime)
-        self.run_callbacks('TopUpPUStandbyEnbl-Sel', self._topuppustandbyenbl)
-        self.run_callbacks('TopUpPUStandbyEnbl-Sts', self._topuppustandbyenbl)
-        self.run_callbacks('TopUpLIStandbyEnbl-Sel', self._topuplistandbyenbl)
-        self.run_callbacks('TopUpLIStandbyEnbl-Sts', self._topuplistandbyenbl)
-        self.run_callbacks('TopUpNextInj-Mon', self._topupnext)
-        self.run_callbacks('TopUpNrPulses-SP', self._topupnrpulses)
-        self.run_callbacks('TopUpNrPulses-RB', self._topupnrpulses)
-        self.run_callbacks(
-            'InjSysCmdDone-Mon', ','.join(self._injsys_dev.done))
-        self.run_callbacks('InjSysCmdSts-Mon', _Const.InjSysCmdSts.Idle)
-        self.run_callbacks('RFKillBeam-Mon', _Const.RFKillBeamMon.Idle)
-        self.run_callbacks('DiagStatusLI-Mon', self._status['LI'])
-        self.run_callbacks('DiagStatusTB-Mon', self._status['TB'])
-        self.run_callbacks('DiagStatusBO-Mon', self._status['BO'])
-        self.run_callbacks('DiagStatusTS-Mon', self._status['TS'])
-        self.run_callbacks('DiagStatusSI-Mon', self._status['SI'])
-        self.run_callbacks('DiagStatus-Mon', self._status['AS'])
-        self.run_callbacks('InjStatus-Mon', self._injstatus)
         self._bias_feedback.init_database()
         self.run_callbacks('Log-Mon', 'Started.')
 
     @property
     def pvs_database(self):
         """Return pvs_database."""
         return self._pvs_database
@@ -369,21 +430,23 @@
 
     def set_mode(self, value):
         """Set injection mode."""
         if not 0 <= value < len(_ETypes.INJMODE):
             return False
 
         if value == _Const.InjMode.TopUp and \
-                self._topupstate_sts == _Const.TopUpSts.Off:
+                self._topup_state_sts == _Const.TopUpSts.Off:
             self._update_log('Configuring EVG RepeatBucketList...')
             self._evg_dev['RepeatBucketList-SP'] = 1
             self._update_log('...done. Waiting to start top-up.')
         else:
             if self._topup_thread and self._topup_thread.is_alive():
+                self._setting_mode = True
                 self._stop_topup_thread()
+                self._setting_mode = False
 
         self._mode = value
         self.run_callbacks('Mode-Sts', self._mode)
         return True
 
     def set_type(self, value):
         """Set injection type."""
@@ -552,28 +615,30 @@
 
     def set_bucketlist_start(self, start):
         """Set bucketlist_start."""
         if not _Const.MIN_BKT <= start <= _Const.MAX_BKT:
             return False
         stop = self._bucketlist_stop
         step = self._bucketlist_step
-        if not self._cmd_bucketlist_fill(stop, start, step):
-            return False
+        if self._mode != _Const.InjMode.TopUp:
+            if not self._cmd_bucketlist_fill(stop, start, step):
+                return False
         self._bucketlist_start = start
         self.run_callbacks('BucketListStart-RB', start)
         return True
 
     def set_bucketlist_stop(self, stop):
         """Set bucketlist_stop."""
         if not _Const.MIN_BKT <= stop <= _Const.MAX_BKT:
             return False
         start = self._bucketlist_start
         step = self._bucketlist_step
-        if not self._cmd_bucketlist_fill(stop, start, step):
-            return False
+        if self._mode != _Const.InjMode.TopUp:
+            if not self._cmd_bucketlist_fill(stop, start, step):
+                return False
         self._bucketlist_stop = stop
         self.run_callbacks('BucketListStop-RB', stop)
         return True
 
     def set_bucketlist_step(self, step):
         """Set bucketlist_step."""
         if not -_Const.MAX_BKT+1 <= step <= _Const.MAX_BKT-1:
@@ -586,114 +651,209 @@
             stop = self._bucketlist_stop
             if not self._cmd_bucketlist_fill(stop, start, step):
                 return False
         self._bucketlist_step = step
         self.run_callbacks('BucketListStep-RB', step)
         return True
 
+    def set_isinj_delay(self, value):
+        """Set IsInjecting-Mon flag delay."""
+        if not 0 <= value <= 1000:
+            return False
+        self._isinj_delay = value
+        self._update_log(f'Changed IsInjecting-Mon flag delay to {value}ms.')
+        self.run_callbacks('IsInjDelay-RB', value)
+        return True
+
+    def set_isinj_duration(self, value):
+        """Set IsInjecting-Mon flag duration."""
+        if not 0 <= value <= 1000:
+            return False
+        self._isinj_duration = value
+        self._update_log(
+            f'Changed IsInjecting-Mon flag duration to {value}ms.')
+        self.run_callbacks('IsInjDuration-RB', value)
+        return True
+
     def _cmd_bucketlist_fill(self, stop, start, step):
         """Set bucket list PV."""
         if not self._evg_dev.connected:
             self._update_log('ERR:Could not update bucket list,')
             self._update_log('ERR:EVG is disconnected.')
             return False
         if self._evg_dev.fill_bucketlist(stop, start, step, timeout=3):
             self._update_log('Updated BucketList.')
             return True
         self._update_log('WARN:Timed out waiting for BucketList.')
         return False
 
-    def set_topupstate(self, value):
+    def set_topup_state(self, value):
         """Set top-up state."""
         if self._mode != _Const.InjMode.TopUp:
-            return
+            return False
 
-        self._topupstate_sel = value
+        self._topup_state_sel = value
         if value == _Const.OffOn.On:
             self._update_log('Start received!')
             if not self._check_allok_2_inject():
-                return
+                return False
             if self._topup_thread is not None and \
                     not self._topup_thread.is_alive() or\
                     self._topup_thread is None:
                 self._launch_topup_thread()
         else:
             self._update_log('Stop received!')
             if self._topup_thread is not None and \
                     self._topup_thread.is_alive():
                 self._stop_topup_thread()
 
         return True
 
-    def set_topupperiod(self, value):
+    def set_topup_period(self, value):
         """Set top-up period [min]."""
         if not 1 <= value <= 6*60:
             return False
 
         sec = value*60
-        if self._topupstate_sts != _Const.TopUpSts.Off:
+        if self._topup_state_sts != _Const.TopUpSts.Off:
             now = _Time.now().timestamp()
-            self._topupnext = now - (now % sec) + sec
-            self.run_callbacks('TopUpNextInj-Mon', self._topupnext)
+            self._topup_next = now - (now % sec) + sec
+            self.run_callbacks('TopUpNextInj-Mon', self._topup_next)
 
-        self._topupperiod = sec
+        self._topup_period = sec
         self._update_log('Changed top-up period to '+str(value)+'min.')
         self.run_callbacks('TopUpPeriod-RB', value)
         return True
 
-    def set_topupheadstarttime(self, value):
+    def set_topup_headstarttime(self, value):
         """Set top-up head start time [s]."""
         if not 0 <= value <= 10*60:
             return False
-
-        self._topupheadstarttime = value
+        self._topup_headstarttime = value
         self._update_log('Changed top-up head start time to '+str(value)+'s.')
-        self.run_callbacks('TopUpHeadStartTime-RB', self._topupheadstarttime)
+        self.run_callbacks('TopUpHeadStartTime-RB', self._topup_headstarttime)
+
+        minwut = _np.ceil(value+1)
+        self._topup_puwarmuptime = max(minwut, self._topup_puwarmuptime)
+        self._topup_liwarmuptime = max(minwut, self._topup_liwarmuptime)
+        self._topup_bopswarmuptime = max(minwut, self._topup_bopswarmuptime)
+        self._topup_borfwarmuptime = max(minwut, self._topup_borfwarmuptime)
+        pvn2val = {
+            'TopUpPUWarmUpTime-': self._topup_puwarmuptime,
+            'TopUpLIWarmUpTime-': self._topup_liwarmuptime,
+            'TopUpBOPSWarmUpTime-': self._topup_bopswarmuptime,
+            'TopUpBORFWarmUpTime-': self._topup_borfwarmuptime,
+        }
+        for pvn, val in pvn2val.items():
+            self.run_callbacks(pvn+'SP', val)
+            self.run_callbacks(pvn+'RB', val)
         return True
 
-    def set_topuppustandbyenbl(self, value):
-        """Set PU standby between top-up injections."""
+    def set_topup_pustandbyenbl(self, value):
+        """Enable/disable PU standby between top-up injections."""
         if not 0 <= value < len(_ETypes.DSBL_ENBL):
             return False
 
         if value:
             if not self._update_topup_pu_refvolt():
                 return False
         else:
-            self._handle_topup_puvoltage('inject')
-        self._topuppustandbyenbl = value
+            self._handle_topup_pu_voltage(_Const.StandbyInject.Inject)
+        self._topup_pustandbyenbl = value
         text = 'En' if value else 'Dis'
         self._update_log(text+'abled PU standby between injections.')
-        self.run_callbacks('TopUpPUStandbyEnbl-Sts', self._topuppustandbyenbl)
+        self.run_callbacks('TopUpPUStandbyEnbl-Sts', self._topup_pustandbyenbl)
+        return True
+
+    def set_topup_puwarmuptime(self, value):
+        """Set PU warm up time before top-up injections."""
+        if not self._topup_headstarttime+1 <= value < 2*60:
+            return False
+        self._topup_puwarmuptime = value
+        self.run_callbacks('TopUpPUWarmUpTime-RB', self._topup_puwarmuptime)
         return True
 
-    def set_topuplistandbyenbl(self, value):
-        """Set LI standby between top-up injections."""
+    def set_topup_liwarmupenbl(self, value):
+        """Enable/disable LI warm up before top-up injections."""
         if not 0 <= value < len(_ETypes.DSBL_ENBL):
             return False
 
         if value == _Const.DsblEnbl.Dsbl:
-            self._handle_topup_linac_timing(state='inject')
-        self._topuplistandbyenbl = value
+            self._handle_topup_linac_timing(state=_Const.StandbyInject.Inject)
+        self._topup_liwarmupenbl = value
         text = 'En' if value else 'Dis'
-        self._update_log(text+'abled LI standby between injections.')
-        self.run_callbacks('TopUpLIStandbyEnbl-Sts', self._topuplistandbyenbl)
+        self._update_log(text+'abled LI warm up before injections.')
+        self.run_callbacks('TopUpLIWarmUpEnbl-Sts', self._topup_liwarmupenbl)
+        return True
+
+    def set_topup_liwarmuptime(self, value):
+        """Set LI warm up time before top-up injections."""
+        if not self._topup_headstarttime+1 <= value < 2*60:
+            return False
+        self._topup_liwarmuptime = value
+        self.run_callbacks('TopUpLIWarmUpTime-RB', self._topup_liwarmuptime)
         return True
 
-    def set_topupnrpulses(self, value):
+    def set_topup_bopsstandbyenbl(self, value):
+        """Enable/disable BO PS standby between top-up injections."""
+        if not 0 <= value < len(_ETypes.DSBL_ENBL):
+            return False
+
+        if value == _Const.DsblEnbl.Dsbl:
+            self._handle_topup_bops_timing(state=_Const.StandbyInject.Inject)
+        self._topup_bopsstandbyenbl = value
+        text = 'En' if value else 'Dis'
+        self._update_log(text+'abled BO PS standby between injections.')
+        self.run_callbacks(
+            'TopUpBOPSStandbyEnbl-Sts', self._topup_bopsstandbyenbl)
+        return True
+
+    def set_topup_bopswarmuptime(self, value):
+        """Set BO PS warm up time before top-up injections."""
+        if not self._topup_headstarttime+1 <= value < 2*60:
+            return False
+        self._topup_bopswarmuptime = value
+        self.run_callbacks(
+            'TopUpBOPSWarmUpTime-RB', self._topup_bopswarmuptime)
+        return True
+
+    def set_topup_borfstandbyenbl(self, value):
+        """Enable/disable BO RF standby between top-up injections."""
+        if not 0 <= value < len(_ETypes.DSBL_ENBL):
+            return False
+
+        if value == _Const.DsblEnbl.Dsbl:
+            self._handle_topup_borf_timing(state=_Const.StandbyInject.Inject)
+        self._topup_borfstandbyenbl = value
+        text = 'En' if value else 'Dis'
+        self._update_log(text+'abled BO RF standby between injections.')
+        self.run_callbacks(
+            'TopUpBORFStandbyEnbl-Sts', self._topup_borfstandbyenbl)
+        return True
+
+    def set_topup_borfwarmuptime(self, value):
+        """Set BO RF warm up time before top-up injections."""
+        if not self._topup_headstarttime+1 <= value < 2*60:
+            return False
+        self._topup_borfwarmuptime = value
+        self.run_callbacks(
+            'TopUpBORFWarmUpTime-RB', self._topup_borfwarmuptime)
+        return True
+
+    def set_topup_nrpulses(self, value):
         """Set top-up number of injection pulses."""
         if not 1 <= value <= 1000:
             return False
 
-        self._topupnrpulses = value
+        self._topup_nrpulses = value
         if self._mode == _Const.InjMode.TopUp:
             if not self._update_bucket_list_topup():
                 return False
         self._update_log('Changed top-up nr.pulses to '+str(value)+'.')
-        self.run_callbacks('TopUpNrPulses-RB', self._topupnrpulses)
+        self.run_callbacks('TopUpNrPulses-RB', self._topup_nrpulses)
         return True
 
     def cmd_injsys_turn_on(self, value=None, wait_finish=False):
         """Set turn on Injection System."""
         run = self._injsys_dev.is_running
         if run:
             self._update_log('ERR:Still processing turn '+run+' InjSystem')
@@ -931,14 +1091,41 @@
             return
         if self._topup_puref_ignore:
             return
         devname = _PVName(pvname).device_name
         index = self._pu_names.index(devname)
         self._pu_refvolt[index] = value
 
+    def _callback_is_injecting(self, value, **kws):
+        if value is None:
+            return
+        thread = _epics.ca.CAThread(
+            target=self._thread_is_injecting, daemon=True)
+        thread.start()
+
+    def _thread_is_injecting(self):
+        # check if any InjSI PU is pulsing
+        is_injecting = False
+        for pvs in self._pvs_injsys.values():
+            if not all(pvo.connected for pvo in pvs):
+                is_injecting = True  # assume the worst scenario
+                break
+            if all(pvo.value for pvo in pvs):
+                is_injecting = True
+                break
+
+        if not is_injecting:
+            return
+
+        # if True, raise IsInjecting flag after {delay}ms for {duration}ms
+        _time.sleep(self._isinj_delay/1000)
+        self.run_callbacks('IsInjecting-Mon', _Const.IdleInjecting.Injecting)
+        _time.sleep(self._isinj_duration/1000)
+        self.run_callbacks('IsInjecting-Mon', _Const.IdleInjecting.Idle)
+
     # --- auxiliary injection methods ---
 
     def _check_allok_2_inject(self, show_warn=True):
         if show_warn:
             if self._status['All'] != 0:
                 self._update_log('WARN:DiagStatus not ok:')
                 for prob in self._status_problems:
@@ -1032,15 +1219,15 @@
         if step is None:
             step = self._bucketlist_step
 
         lastfilledbucket = self._evg_dev.bucketlist_mon[-1]
         if not _Const.MIN_BKT <= lastfilledbucket <= _Const.MAX_BKT:
             lastfilledbucket = 1
 
-        bucket = _np.arange(self._topupnrpulses) + 1
+        bucket = _np.arange(self._topup_nrpulses) + 1
         bucket *= step
         bucket += lastfilledbucket - 1
         bucket %= 864
         bucket += 1
         return self._set_bucket_list(bucket)
 
     def _set_bucket_list(self, value):
@@ -1054,15 +1241,15 @@
         return False
 
     # --- auxiliary top-up methods ---
 
     def _launch_topup_thread(self):
         while self._abort:
             _time.sleep(0.1)
-        self._update_log('Launchig top-up thread...')
+        self._update_log('Launching top-up thread...')
         self._topup_thread = _epics.ca.CAThread(
             target=self._do_topup, daemon=True)
         self._topup_thread.start()
 
     def _stop_topup_thread(self):
         if self._abort:
             return
@@ -1071,44 +1258,28 @@
         self._topup_thread.join()
         self._topup_thread = None
         self._update_log('Stopped top-up thread.')
         self._abort = False
 
         # reset next injection schedule
         now = _Time.now().timestamp()
-        self._topupnext = now - (now % (24*60*60)) + 3*60*60
-        self.run_callbacks('TopUpNextInj-Mon', self._topupnext)
+        self._topup_next = now - (now % (24*60*60)) + 3*60*60
+        self.run_callbacks('TopUpNextInj-Mon', self._topup_next)
 
     def _do_topup(self):
         # update bucket list according to settings
         self._update_bucket_list_topup()
 
         # update next injection schedule
-        now, period = _Time.now().timestamp(), self._topupperiod
-        self._topupnext = now - (now % period) + period
-        self.run_callbacks('TopUpNextInj-Mon', self._topupnext)
-
-        # if PU standby is enabled
-        if self._topuppustandbyenbl:
-            if not self._update_topup_pu_refvolt():
-                self._update_log('ERR:...aborted top-up loop.')
-                return
-
-            # if remaining time is short, do not handle PU voltage
-            if self._topupnext - _time.time() <= _Const.PU_VOLTAGE_UP_TIME*2:
-                self._topup_pu_prepared = True
-            else:
-                # else, set PU voltage to 50%
-                self._handle_topup_puvoltage('standby')
-        else:
-            self._topup_pu_prepared = True
+        now, period = _Time.now().timestamp(), self._topup_period
+        self._topup_next = now - (now % period) + period
+        self.run_callbacks('TopUpNextInj-Mon', self._topup_next)
 
-        # handle LI timing
-        if self._topupnext - _time.time() > _Const.LI_STDBY_CONF_TIME*2:
-            self._handle_topup_linac_timing(state='standby')
+        # prepare subsystems state
+        self._prepare_topup()
 
         self._bias_feedback.do_update_models = True
 
         while self._mode == _Const.InjMode.TopUp:
             if not self._check_allok_2_inject():
                 break
 
@@ -1136,94 +1307,124 @@
                 self._update_topupsts(_Const.TopUpSts.TurningOff)
                 self._update_bucket_list_topup()
             else:
                 self._update_topupsts(_Const.TopUpSts.Skipping)
                 self._update_log('Skipping injection...')
                 _time.sleep(2)
 
-            self._handle_topup_puvoltage('standby')
-            self._handle_topup_linac_timing('standby')
-
-            self._topupnext += self._topupperiod
-            self.run_callbacks('TopUpNextInj-Mon', self._topupnext)
-
-        self._handle_topup_puvoltage('inject')
-        self._handle_topup_linac_timing('inject')
+            self._handle_topup_pu_voltage(_Const.StandbyInject.Standby)
+            self._handle_topup_linac_timing(_Const.StandbyInject.Standby)
+            self._handle_topup_bops_timing(_Const.StandbyInject.Standby)
+            self._handle_topup_borf_timing(_Const.StandbyInject.Standby)
+
+            self._topup_next += self._topup_period
+            self.run_callbacks('TopUpNextInj-Mon', self._topup_next)
+
+        self._handle_topup_pu_voltage(_Const.StandbyInject.Inject)
+        self._handle_topup_linac_timing(_Const.StandbyInject.Inject)
+        self._handle_topup_bops_timing(_Const.StandbyInject.Inject)
+        self._handle_topup_borf_timing(_Const.StandbyInject.Inject)
 
         self._bias_feedback.do_update_models = False
 
         # update top-up status
         self._update_topupsts(_Const.TopUpSts.Off)
         self._update_log('Stopped top-up loop.')
-        if not self._abort:
-            self._topupstate_sel = _Const.OffOn.Off
-            self.run_callbacks('TopUpState-Sel', self._topupstate_sel)
+        if not self._abort or self._setting_mode:
+            self._topup_state_sel = _Const.OffOn.Off
+            self.run_callbacks('TopUpState-Sel', self._topup_state_sel)
 
     def _wait_topup_period(self):
-        while _time.time() < self._topupnext:
+        while _time.time() < self._topup_next:
             if not self._check_allok_2_inject(show_warn=False):
                 return False
             _time.sleep(1)
 
-            remaining = round(self._topupnext - _time.time())
+            remaining = round(self._topup_next - _time.time())
             text = 'Remaining time: {}s'.format(remaining)
             self.run_callbacks('Log-Mon', text)
             if remaining % 60 == 0:
                 _log.info(text)
 
-            if remaining <= _Const.PU_VOLTAGE_UP_TIME and \
-                    not self._topup_pu_prepared:
-                self._handle_topup_puvoltage('inject')
-
-            if remaining <= _Const.LI_STDBY_CONF_TIME:
-                self._handle_topup_linac_timing('inject')
+            # prepare subsystems
+            if remaining <= self._topup_puwarmuptime:
+                self._handle_topup_pu_voltage(_Const.StandbyInject.Inject)
+            if remaining <= self._topup_liwarmuptime:
+                self._handle_topup_linac_timing(_Const.StandbyInject.Inject)
+            if remaining <= self._topup_bopswarmuptime:
+                self._handle_topup_bops_timing(_Const.StandbyInject.Inject)
+            if remaining <= self._topup_borfwarmuptime:
+                self._handle_topup_borf_timing(_Const.StandbyInject.Inject)
 
+            # bias fb
             cond = remaining <= _Const.BIASFB_AHEADSETIME
             cond &= bool(self._bias_feedback.loop_state)
             cond &= not self._bias_feedback.already_set
             if cond and self.currinfo_dev.connected:
                 dcur = self._bias_feedback.get_delta_current_per_pulse(
-                    per=self._topupperiod, nrpul=self._topupnrpulses,
+                    per=self._topup_period, nrpul=self._topup_nrpulses,
                     curr_avg=self._target_current,
                     curr_now=self.currinfo_dev.current,
                     ltime=self.currinfo_dev.lifetime)
                 self._update_log(f'BiasFB required InjCurr: {dcur:.3f}mA')
                 bias = self._bias_feedback.get_bias_voltage(dcur)
                 self.run_callbacks('MultBunBiasVolt-SP', bias)
                 self.set_multbunbiasvolt(bias)
                 self._bias_feedback.already_set = True
 
-            if _time.time() >= self._topupnext - self._topupheadstarttime:
+            if _time.time() >= self._topup_next - self._topup_headstarttime:
                 return True
 
         self._update_log('Remaining time: 0s')
         return True
 
-    def _handle_topup_puvoltage(self, state='inject'):
-        if not self._topuppustandbyenbl:
+    def _prepare_topup(self):
+        # PU
+        if self._topup_pustandbyenbl:
+            if not self._update_topup_pu_refvolt():
+                self._update_log('ERR:...aborted top-up loop.')
+                return
+            # set PU voltage standby if remaining time is not too short
+            if self._topup_next - _time.time() > self._topup_puwarmuptime*2:
+                self._handle_topup_pu_voltage(_Const.StandbyInject.Standby)
+
+        # LI
+        if self._topup_liwarmupenbl:
+            if self._topup_next - _time.time() > self._topup_liwarmuptime*2:
+                self._handle_topup_linac_timing(
+                    state=_Const.StandbyInject.Standby)
+
+        # BO PS
+        if self._topup_bopsstandbyenbl:
+            if self._topup_next - _time.time() > self._topup_bopswarmuptime*2:
+                self._handle_topup_bops_timing(
+                    state=_Const.StandbyInject.Standby)
+
+        # BO RF
+        if self._topup_borfstandbyenbl:
+            if self._topup_next - _time.time() > self._topup_borfwarmuptime*2:
+                self._handle_topup_borf_timing(
+                    state=_Const.StandbyInject.Standby)
+
+    def _handle_topup_pu_voltage(self, state):
+        if not self._topup_pustandbyenbl:
+            return
+        is_inj = state == _Const.StandbyInject.Inject
+        if is_inj and self._topup_pu_prepared:
             return
         self._topup_puref_ignore = True
-        if state == 'inject':
-            self._topup_pu_prepared = True
-            self._update_log('Setting PU Voltage to 100%...')
-            for idx, dev in enumerate(self._pu_devs):
-                if not dev.connected:
-                    self._update_log('WARN:'+dev.devname+' disconnected.')
-                    continue
-                dev.voltage = self._pu_refvolt[idx]
-            self._update_log('...done.')
-        elif state == 'standby':
-            self._topup_pu_prepared = False
-            self._update_log('Setting PU Voltage to 50%...')
-            for idx, dev in enumerate(self._pu_devs):
-                if not dev.connected:
-                    self._update_log('WARN:'+dev.devname+' disconnected.')
-                    continue
-                dev.voltage = self._pu_refvolt[idx] * 0.5
-            self._update_log('...done.')
+        self._topup_pu_prepared = is_inj
+        factor = 1 if is_inj else 0.5
+        self._update_log(f'Setting PU Voltage to {factor*100}%...')
+        for idx, dev in enumerate(self._pu_devs):
+            if not dev.connected:
+                self._update_log('WARN:'+dev.devname+' disconnected.')
+                continue
+            dev.voltage = self._pu_refvolt[idx] * factor
+        self._update_log('...done.')
         _time.sleep(1)
         self._topup_puref_ignore = False
 
     def _update_topup_pu_refvolt(self):
         # get PU voltage reference
         for idx, dev in enumerate(self._pu_devs):
             spv = dev['Voltage-SP']
@@ -1231,28 +1432,51 @@
                 self._update_topupsts(_Const.TopUpSts.Off)
                 self._update_log('ERR:Could not read voltage of')
                 self._update_log('ERR:'+dev.devname+'...')
                 return False
             self._pu_refvolt[idx] = dev['Voltage-SP']
         return True
 
-    def _handle_topup_linac_timing(self, state='inject'):
-        if not self._topuplistandbyenbl:
+    def _handle_topup_linac_timing(self, state):
+        if not self._topup_liwarmupenbl:
             return
-        event = 'RmpBO' if state == 'inject' else 'Linac'
-        allok = all([trig.source_str == event for trig in self._li_trig_devs])
-        if allok:
+        is_inj = state == _Const.StandbyInject.Inject
+        if is_inj and self._topup_li_prepared:
             return
-        self._update_log('Configuring LI timing...')
-        # move triggers to new event
+        self._topup_li_prepared = is_inj
+        event = 'RmpBO' if is_inj else 'Linac'
         self._hlti_dev.change_triggers_source(
             self._li_trig_names, new_src=event, printlog=False)
-        # update events
-        self._evg_dev.cmd_update_events()
-        self._update_log('...done.')
+        self._update_log('LI timing configured.')
+        return
+
+    def _handle_topup_bops_timing(self, state):
+        if not self._topup_bopsstandbyenbl:
+            return
+        is_inj = state == _Const.StandbyInject.Inject
+        if is_inj and self._topup_bops_prepared:
+            return
+        self._topup_bops_prepared = is_inj
+        trigstate = int(is_inj)
+        for trig in self._bops_trig_devs:
+            trig.state = trigstate
+        self._update_log('BO PS timing configured.')
+        return
+
+    def _handle_topup_borf_timing(self, state):
+        if not self._topup_borfstandbyenbl:
+            return
+        is_inj = state == _Const.StandbyInject.Inject
+        if is_inj and self._topup_borf_prepared:
+            return
+        self._topup_borf_prepared = is_inj
+        trigstate = int(is_inj)
+        for trig in self._borf_trig_devs:
+            trig.state = trigstate
+        self._update_log('BO RF timing configured.')
         return
 
     # --- auxiliary log methods ---
 
     def _launch_watch_dev_thread(self):
         if self._thread_watdev is None or not self._thread_watdev.is_alive():
             self._thread_watdev = _epics.ca.CAThread(
@@ -1292,15 +1516,15 @@
         elif 'WARN' in msg:
             _log.warning(msg[5:])
         else:
             _log.info(msg)
         self.run_callbacks('Log-Mon', msg)
 
     def _update_topupsts(self, sts):
-        self._topupstate_sts = sts
+        self._topup_state_sts = sts
         self.run_callbacks('TopUpState-Sts', sts)
 
     # --- auxiliary update status methods ---
 
     def _update_diagstatus(self):
         """Run as a thread scanning PVs."""
         # constants of alarms to ignore
```

### Comparing `siriuspy-2.72.0/siriuspy/machshift/csdev.py` & `siriuspy-2.73.0/siriuspy/machshift/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/machshift/macreport.py` & `siriuspy-2.73.0/siriuspy/machshift/macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/machshift/macschedule.py` & `siriuspy-2.73.0/siriuspy/machshift/macschedule.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/machshift/main.py` & `siriuspy-2.73.0/siriuspy/machshift/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/machshift/test_macreport.py` & `siriuspy-2.73.0/siriuspy/machshift/test_macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/machshift/utils.py` & `siriuspy-2.73.0/siriuspy/machshift/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/magnet/data.py` & `siriuspy-2.73.0/siriuspy/magnet/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/magnet/excdata.py` & `siriuspy-2.73.0/siriuspy/magnet/excdata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/magnet/factory.py` & `siriuspy-2.73.0/siriuspy/magnet/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/magnet/normalizer.py` & `siriuspy-2.73.0/siriuspy/magnet/normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/magnet/util.py` & `siriuspy-2.73.0/siriuspy/magnet/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/meas/csdev.py` & `siriuspy-2.73.0/siriuspy/meas/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/meas/liemit/csdev.py` & `siriuspy-2.73.0/siriuspy/meas/liemit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/meas/liemit/main.py` & `siriuspy-2.73.0/siriuspy/meas/liemit/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/meas/lienergy/csdev.py` & `siriuspy-2.73.0/siriuspy/meas/lienergy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/meas/lienergy/main.py` & `siriuspy-2.73.0/siriuspy/meas/lienergy/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/meas/util.py` & `siriuspy-2.73.0/siriuspy/meas/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/namesys/implementation.py` & `siriuspy-2.73.0/siriuspy/namesys/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/optics/lattice_survey.py` & `siriuspy-2.73.0/siriuspy/optics/lattice_survey.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/opticscorr/base.py` & `siriuspy-2.73.0/siriuspy/opticscorr/base.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/opticscorr/chrom.py` & `siriuspy-2.73.0/siriuspy/opticscorr/chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/opticscorr/csdev.py` & `siriuspy-2.73.0/siriuspy/opticscorr/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/opticscorr/opticscorr.py` & `siriuspy-2.73.0/siriuspy/opticscorr/opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/opticscorr/tune.py` & `siriuspy-2.73.0/siriuspy/opticscorr/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/opticscorr/utils.py` & `siriuspy-2.73.0/siriuspy/opticscorr/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/oscilloscope/keysight.py` & `siriuspy-2.73.0/siriuspy/oscilloscope/keysight.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/oscilloscope/scopes.py` & `siriuspy-2.73.0/siriuspy/oscilloscope/scopes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/posang/csdev.py` & `siriuspy-2.73.0/siriuspy/posang/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/posang/main.py` & `siriuspy-2.73.0/siriuspy/posang/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/posang/utils.py` & `siriuspy-2.73.0/siriuspy/posang/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/beaglebone.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/beaglebone.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/bsmp/commands.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/bsmp/constants.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,25 +310,25 @@
     V_PS_SOFT_INTERLOCKS = 31
     V_PS_HARD_INTERLOCKS = 32
     V_I_LOAD_MEAN = 33
     V_I_LOAD1 = 34
     V_I_LOAD2 = 35
     V_V_CAPBANK = 36
     V_DUTY_CYCLE = 37
-    V_V_INPUT_IIB = 38
-    V_I_INPUT_IIB = 39
-    V_I_OUTPUT_IIB = 40
-    V_TEMP_IGBT_1_IIB = 41
-    V_TEMP_IGBT_2_IIB = 42
-    V_TEMP_INDUCTOR_IIB = 43
-    V_TEMP_HEATSINK_IIB = 44
-    V_V_DRIVER_IIB = 45
-    V_I_DRIVER_1_IIB = 46
-    V_I_DRIVER_2_IIB = 47
-    V_I_LEAKAGE_IIB = 48
+    V_I_LEAKAGE = 38
+    V_V_INPUT_IIB = 39
+    V_I_INPUT_IIB = 40
+    V_I_OUTPUT_IIB = 41
+    V_TEMP_IGBT_1_IIB = 42
+    V_TEMP_IGBT_2_IIB = 43
+    V_TEMP_INDUCTOR_IIB = 44
+    V_TEMP_HEATSINK_IIB = 45
+    V_V_DRIVER_IIB = 46
+    V_I_DRIVER_1_IIB = 47
+    V_I_DRIVER_2_IIB = 48
     V_TEMP_BOARD_IIB = 49
     V_RH_IIB = 50
     V_IIB_INTERLOCKS = 51
     V_IIB_ALARMS = 52
     V_PS_ALARMS = 53
 
 
@@ -495,26 +495,26 @@
     V_DUTY_CYCLE_2_1 = 51
     V_DUTY_CYCLE_1_2 = 52
     V_DUTY_CYCLE_2_2 = 53
     V_DUTY_CYCLE_1_3 = 54
     V_DUTY_CYCLE_2_3 = 55
     V_DUTY_CYCLE_1_4 = 56
     V_DUTY_CYCLE_2_4 = 57
-    V_V_INPUT_IIB_1 = 58
-    V_V_OUTPUT_IIB_1 = 59
-    V_I_IGBT_1_IIB_1 = 60
-    V_I_IGBT_2_IIB_1 = 61
-    V_TEMP_IGBT_1_IIB_1 = 62
-    V_TEMP_IGBT_2_IIB_1 = 63
-    V_V_DRIVER_IIB_1 = 64
-    V_I_DRIVER_1_IIB_1 = 65
-    V_I_DRIVER_2_IIB_1 = 66
-    V_TEMP_INDUCTOR_IIB_1 = 67
-    V_TEMP_HEATSINK_IIB_1 = 68
-    V_I_LEAKAGE_IIB_1 = 69
+    V_I_LEAKAGE = 58
+    V_V_INPUT_IIB_1 = 59
+    V_V_OUTPUT_IIB_1 = 60
+    V_I_IGBT_1_IIB_1 = 61
+    V_I_IGBT_2_IIB_1 = 62
+    V_TEMP_IGBT_1_IIB_1 = 63
+    V_TEMP_IGBT_2_IIB_1 = 64
+    V_V_DRIVER_IIB_1 = 65
+    V_I_DRIVER_1_IIB_1 = 66
+    V_I_DRIVER_2_IIB_1 = 67
+    V_TEMP_INDUCTOR_IIB_1 = 68
+    V_TEMP_HEATSINK_IIB_1 = 69
     V_TEMP_BOARD_IIB_1 = 70
     V_RH_IIB_1 = 71
     V_IIB_INTERLOCKS_1 = 72
     V_IIB_ALARMS_1 = 73
     V_V_INPUT_IIB_2 = 74
     V_V_OUTPUT_IIB_2 = 75
     V_I_IGBT_1_IIB_2 = 76
@@ -522,52 +522,49 @@
     V_TEMP_IGBT_1_IIB_2 = 78
     V_TEMP_IGBT_2_IIB_2 = 79
     V_V_DRIVER_IIB_2 = 80
     V_I_DRIVER_1_IIB_2 = 81
     V_I_DRIVER_2_IIB_2 = 82
     V_TEMP_INDUCTOR_IIB_2 = 83
     V_TEMP_HEATSINK_IIB_2 = 84
-    V_I_LEAKAGE_IIB_2 = 85
-    V_TEMP_BOARD_IIB_2 = 86
-    V_RH_IIB_2 = 87
-    V_IIB_INTERLOCKS_2 = 88
-    V_IIB_ALARMS_2 = 89
-    V_V_INPUT_IIB_3 = 90
-    V_V_OUTPUT_IIB_3 = 91
-    V_I_IGBT_1_IIB_3 = 92
-    V_I_IGBT_2_IIB_3 = 93
-    V_TEMP_IGBT_1_IIB_3 = 94
-    V_TEMP_IGBT_2_IIB_3 = 95
-    V_V_DRIVER_IIB_3 = 96
-    V_I_DRIVER_1_IIB_3 = 97
-    V_I_DRIVER_2_IIB_3 = 98
-    V_TEMP_INDUCTOR_IIB_3 = 99
-    V_TEMP_HEATSINK_IIB_3 = 100
-    V_I_LEAKAGE_IIB_3 = 101
-    V_TEMP_BOARD_IIB_3 = 102
-    V_RH_IIB_3 = 103
-    V_IIB_INTERLOCKS_3 = 104
-    V_IIB_ALARMS_3 = 105
-    V_V_INPUT_IIB_4 = 106
-    V_V_OUTPUT_IIB_4 = 107
-    V_I_IGBT_1_IIB_4 = 108
-    V_I_IGBT_2_IIB_4 = 109
-    V_TEMP_IGBT_1_IIB_4 = 110
-    V_TEMP_IGBT_2_IIB_4 = 111
-    V_V_DRIVER_IIB_4 = 112
-    V_I_DRIVER_1_IIB_4 = 113
-    V_I_DRIVER_2_IIB_4 = 114
-    V_TEMP_INDUCTOR_IIB_4 = 115
-    V_TEMP_HEATSINK_IIB_4 = 116
-    V_I_LEAKAGE_IIB_4 = 117
-    V_TEMP_BOARD_IIB_4 = 118
-    V_RH_IIB_4 = 119
-    V_IIB_INTERLOCKS_4 = 120
-    V_IIB_ALARMS_4 = 121
-    V_PS_ALARMS = 122
+    V_TEMP_BOARD_IIB_2 = 85
+    V_RH_IIB_2 = 86
+    V_IIB_INTERLOCKS_2 = 87
+    V_IIB_ALARMS_2 = 88
+    V_V_INPUT_IIB_3 = 89
+    V_V_OUTPUT_IIB_3 = 90
+    V_I_IGBT_1_IIB_3 = 91
+    V_I_IGBT_2_IIB_3 = 92
+    V_TEMP_IGBT_1_IIB_3 = 93
+    V_TEMP_IGBT_2_IIB_3 = 94
+    V_V_DRIVER_IIB_3 = 95
+    V_I_DRIVER_1_IIB_3 = 96
+    V_I_DRIVER_2_IIB_3 = 97
+    V_TEMP_INDUCTOR_IIB_3 = 98
+    V_TEMP_HEATSINK_IIB_3 = 99
+    V_TEMP_BOARD_IIB_3 = 100
+    V_RH_IIB_3 = 101
+    V_IIB_INTERLOCKS_3 = 102
+    V_IIB_ALARMS_3 = 103
+    V_V_INPUT_IIB_4 = 104
+    V_V_OUTPUT_IIB_4 = 105
+    V_I_IGBT_1_IIB_4 = 106
+    V_I_IGBT_2_IIB_4 = 107
+    V_TEMP_IGBT_1_IIB_4 = 108
+    V_TEMP_IGBT_2_IIB_4 = 109
+    V_V_DRIVER_IIB_4 = 110
+    V_I_DRIVER_1_IIB_4 = 111
+    V_I_DRIVER_2_IIB_4 = 112
+    V_TEMP_INDUCTOR_IIB_4 = 113
+    V_TEMP_HEATSINK_IIB_4 = 114
+    V_TEMP_BOARD_IIB_4 = 115
+    V_RH_IIB_4 = 116
+    V_IIB_INTERLOCKS_4 = 117
+    V_IIB_ALARMS_4 = 118
+    V_PS_ALARMS = 119
 
 
 class ConstFAP_2P2S(ConstPSBSMP):
     """Namespace for organizing power supply FAP_2P2S BSMP constants."""
 
     # --- FAP_2P2S variables ---
     V_PS_SOFT_INTERLOCKS = 31
@@ -599,26 +596,26 @@
     V_DUTY_CYCLE_2_1 = 57
     V_DUTY_CYCLE_1_2 = 58
     V_DUTY_CYCLE_2_2 = 59
     V_DUTY_CYCLE_1_3 = 60
     V_DUTY_CYCLE_2_3 = 61
     V_DUTY_CYCLE_1_4 = 62
     V_DUTY_CYCLE_2_4 = 63
-    V_V_INPUT_IIB_1 = 64
-    V_V_OUTPUT_IIB_1 = 65
-    V_I_IGBT_1_IIB_1 = 66
-    V_I_IGBT_2_IIB_1 = 67
-    V_TEMP_IGBT_1_IIB_1 = 68
-    V_TEMP_IGBT_2_IIB_1 = 69
-    V_V_DRIVER_IIB_1 = 70
-    V_I_DRIVER_1_IIB_1 = 71
-    V_I_DRIVER_2_IIB_1 = 72
-    V_TEMP_INDUCTOR_IIB_1 = 73
-    V_TEMP_HEATSINK_IIB_1 = 74
-    V_I_LEAKAGE_IIB_1 = 75
+    V_I_LEAKAGE = 64
+    V_V_INPUT_IIB_1 = 65
+    V_V_OUTPUT_IIB_1 = 66
+    V_I_IGBT_1_IIB_1 = 67
+    V_I_IGBT_2_IIB_1 = 68
+    V_TEMP_IGBT_1_IIB_1 = 69
+    V_TEMP_IGBT_2_IIB_1 = 70
+    V_V_DRIVER_IIB_1 = 71
+    V_I_DRIVER_1_IIB_1 = 72
+    V_I_DRIVER_2_IIB_1 = 73
+    V_TEMP_INDUCTOR_IIB_1 = 74
+    V_TEMP_HEATSINK_IIB_1 = 75
     V_TEMP_BOARD_IIB_1 = 76
     V_RH_IIB_1 = 77
     V_IIB_INTERLOCKS_1 = 78
     V_IIB_ALARMS_1 = 79
     V_V_INPUT_IIB_2 = 80
     V_V_OUTPUT_IIB_2 = 81
     V_I_IGBT_1_IIB_2 = 82
@@ -626,51 +623,49 @@
     V_TEMP_IGBT_1_IIB_2 = 84
     V_TEMP_IGBT_2_IIB_2 = 85
     V_V_DRIVER_IIB_2 = 86
     V_I_DRIVER_1_IIB_2 = 87
     V_I_DRIVER_2_IIB_2 = 88
     V_TEMP_INDUCTOR_IIB_2 = 89
     V_TEMP_HEATSINK_IIB_2 = 90
-    V_PS_ALARMS = 91
-    V_TEMP_BOARD_IIB_2 = 92
-    V_RH_IIB_2 = 93
-    V_IIB_INTERLOCKS_2 = 94
-    V_IIB_ALARMS_2 = 95
-    V_V_INPUT_IIB_3 = 96
-    V_V_OUTPUT_IIB_3 = 97
-    V_I_IGBT_1_IIB_3 = 98
-    V_I_IGBT_2_IIB_3 = 99
-    V_TEMP_IGBT_1_IIB_3 = 100
-    V_TEMP_IGBT_2_IIB_3 = 101
-    V_V_DRIVER_IIB_3 = 102
-    V_I_DRIVER_1_IIB_3 = 103
-    V_I_DRIVER_2_IIB_3 = 104
-    V_TEMP_INDUCTOR_IIB_3 = 105
-    V_TEMP_HEATSINK_IIB_3 = 106
-    V_I_LEAKAGE_IIB_3 = 107
-    V_TEMP_BOARD_IIB_3 = 108
-    V_RH_IIB_3 = 109
-    V_IIB_INTERLOCKS_3 = 110
-    V_IIB_ALARMS_3 = 111
-    V_V_INPUT_IIB_4 = 112
-    V_V_OUTPUT_IIB_4 = 113
-    V_I_IGBT_1_IIB_4 = 114
-    V_I_IGBT_2_IIB_4 = 115
-    V_TEMP_IGBT_1_IIB_4 = 116
-    V_TEMP_IGBT_2_IIB_4 = 117
-    V_V_DRIVER_IIB_4 = 118
-    V_I_DRIVER_1_IIB_4 = 119
-    V_I_DRIVER_2_IIB_4 = 120
-    V_TEMP_INDUCTOR_IIB_4 = 121
-    V_TEMP_HEATSINK_IIB_4 = 122
-    V_I_LEAKAGE_IIB_4 = 123
-    V_TEMP_BOARD_IIB_4 = 124
-    V_RH_IIB_4 = 125
-    V_IIB_INTERLOCKS_4 = 126
-    V_IIB_ALARMS_4 = 127
+    V_TEMP_BOARD_IIB_2 = 91
+    V_RH_IIB_2 = 92
+    V_IIB_INTERLOCKS_2 = 93
+    V_IIB_ALARMS_2 = 94
+    V_V_INPUT_IIB_3 = 95
+    V_V_OUTPUT_IIB_3 = 96
+    V_I_IGBT_1_IIB_3 = 97
+    V_I_IGBT_2_IIB_3 = 98
+    V_TEMP_IGBT_1_IIB_3 = 99
+    V_TEMP_IGBT_2_IIB_3 = 100
+    V_V_DRIVER_IIB_3 = 101
+    V_I_DRIVER_1_IIB_3 = 102
+    V_I_DRIVER_2_IIB_3 = 103
+    V_TEMP_INDUCTOR_IIB_3 = 104
+    V_TEMP_HEATSINK_IIB_3 = 105
+    V_TEMP_BOARD_IIB_3 = 106
+    V_RH_IIB_3 = 107
+    V_IIB_INTERLOCKS_3 = 108
+    V_IIB_ALARMS_3 = 109
+    V_V_INPUT_IIB_4 = 110
+    V_V_OUTPUT_IIB_4 = 111
+    V_I_IGBT_1_IIB_4 = 112
+    V_I_IGBT_2_IIB_4 = 113
+    V_TEMP_IGBT_1_IIB_4 = 114
+    V_TEMP_IGBT_2_IIB_4 = 115
+    V_V_DRIVER_IIB_4 = 116
+    V_I_DRIVER_1_IIB_4 = 117
+    V_I_DRIVER_2_IIB_4 = 118
+    V_TEMP_INDUCTOR_IIB_4 = 119
+    V_TEMP_HEATSINK_IIB_4 = 120
+    V_TEMP_BOARD_IIB_4 = 121
+    V_RH_IIB_4 = 122
+    V_IIB_INTERLOCKS_4 = 123
+    V_IIB_ALARMS_4 = 124
+    V_PS_ALARMS = 125
 
 
 # --- Const ACDC ---
 
 class ConstFBP_DCLink(ConstPSBSMP):
     """Namespace for organizing power supply FBP_DCLink BSMP constants."""
```

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/bsmp/entities.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -649,50 +649,47 @@
         {'eid': 80, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 81, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 82, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 83, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 84, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 85, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 86, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 87, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
+        {'eid': 87, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
         {'eid': 88, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
-        {'eid': 89, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 89, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 90, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 91, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 92, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 93, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 94, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 95, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 96, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 97, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 98, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 99, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 100, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 101, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 102, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 103, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 104, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
-        {'eid': 105, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 102, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 103, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 104, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
+        {'eid': 105, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 106, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 107, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 108, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 109, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 110, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 111, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 112, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 113, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 114, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 115, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 116, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 117, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 118, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 119, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 120, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
-        {'eid': 121, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
-        {'eid': 122, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 117, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 118, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 119, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
     )
 
 
 class EntitiesFAP_2P2S(EntitiesPS):
     """FAP_2P2S-type power supply entities."""
 
     _ps_variables = EntitiesPS._ps_variables + (
@@ -753,51 +750,49 @@
         {'eid': 84, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 85, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 86, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 87, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 88, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 89, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 90, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 91, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 91, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 92, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 93, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
+        {'eid': 93, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
         {'eid': 94, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
-        {'eid': 95, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 95, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 96, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 97, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 98, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 99, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 100, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 101, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 102, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 103, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 104, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 105, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 106, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 107, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 108, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 109, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 110, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
-        {'eid': 111, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 108, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 109, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 110, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
+        {'eid': 111, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 112, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 113, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 114, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 115, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 116, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 117, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 118, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 119, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 120, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 121, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
         {'eid': 122, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 123, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 124, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 125, 'waccess': False, 'count': 1, 'var_type': _Types.T_FLOAT},
-        {'eid': 126, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
-        {'eid': 127, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 123, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 124, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
+        {'eid': 125, 'waccess': False, 'count': 1, 'var_type': _Types.T_UINT32},
     )
 
 
 # --- Entities ACDC ---
 
 
 class EntitiesFBP_DCLink(EntitiesPS):
```

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/bsmp/factory.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/bsmp/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/csdev.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/csdev.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         'Bit24', 'Bit25', 'Bit26', 'Bit27',
         'Bit28', 'Bit29', 'Bit30', 'Bit31')
     HARD_INTLCK_FAC_DCDC = (
         'Sobre-corrente na carga',
         'Sobre-tensao no DC-Link', 'Sub-tensao no DC-Link',
         'Interlock da placa IIB',
         'Interlock externo', 'Interlock do rack',
-        'Bit6', 'Bit7',
+        'Alta corrente de fuga', 'Bit7',
         'Bit8', 'Bit9', 'Bit10', 'Bit11',
         'Bit12', 'Bit13', 'Bit14', 'Bit15',
         'Bit16', 'Bit17', 'Bit18', 'Bit19',
         'Bit20', 'Bit21', 'Bit22', 'Bit23',
         'Bit24', 'Bit25', 'Bit26', 'Bit27',
         'Bit28', 'Bit29', 'Bit30', 'Bit31')
     ALARMS_FAC_DCDC = ALARMS_FBP
@@ -180,35 +180,33 @@
         'Sobre-corrente no driver do IGBT 2',
         'Erro no driver do IGBT Top 1',
         'Erro no driver do IGBT Bottom 1',
         'Erro no driver do IGBT Top 2',
         'Erro no driver do IGBT Bottom 2',
         'Sobre-temperatura nos indutores',
         'Sobre-temperatura no dissipador',
-        'Alta corrente de fuga',
         'Sobre-temperatura da placa IIB',
-        'Alta umidade relativa', 'Bit19',
+        'Alta umidade relativa', 'Bit18', 'Bit19',
         'Bit20', 'Bit21', 'Bit22', 'Bit23',
         'Bit24', 'Bit25', 'Bit26', 'Bit27',
         'Bit28', 'Bit29', 'Bit30', 'Bit31')
     IIB_ALARMS_FAC_DCDC = (
         'Sobre-tensao de entrada',
         'Sobre-corrente de entrada',
         'Sobre-corrente de saida',
         'Sobre-temperatura no IGBT 1',
         'Sobre-temperatura no IGBT 2',
         'Sobre-tensao dos drivers dos IGBTs',
         'Sobre-corrente no driver do IGBT 1',
         'Sobre-corrente no driver do IGBT 2',
         'Sobre-temperatura nos indutores',
         'Sobre-temperatura no dissipador',
-        'Alta corrente de fuga',
         'Sobre-temperatura da placa IIB',
         'Alta umidade relativa',
-        'Bit13', 'Bit14', 'Bit15',
+        'Bit12', 'Bit13', 'Bit14', 'Bit15',
         'Bit16', 'Bit17', 'Bit18', 'Bit19',
         'Bit20', 'Bit21', 'Bit22', 'Bit23',
         'Bit24', 'Bit25', 'Bit26', 'Bit27',
         'Bit28', 'Bit29', 'Bit30', 'Bit31')
     SOFT_INTLCK_FAC_2S_DCDC = (
         'Falha no DCCT1', 'Falha no DCCT2',
         'Alta diferenca entre DCCTs',
@@ -250,35 +248,34 @@
         'Sobre-corrente no driver do IGBT 2',
         'Erro no driver do IGBT Top 1',
         'Erro no driver do IGBT Bottom 1',
         'Erro no driver do IGBT Top 2',
         'Erro no driver do IGBT Bottom 2',
         'Sobre-temperatura nos indutores',
         'Sobre-temperatura no dissipador',
-        'Alta corrente de fuga',
         'Sobre-temperatura da placa IIB',
-        'Alta umidade relativa', 'Bit19',
+        'Alta umidade relativa',
+        'Bit18', 'Bit19',
         'Bit20', 'Bit21', 'Bit22', 'Bit23',
         'Bit24', 'Bit25', 'Bit26', 'Bit27',
         'Bit28', 'Bit29', 'Bit30', 'Bit31')
     IIB_ALARMS_FAC_2S_DCDC = (
         'Sobre-tensao de entrada',
         'Sobre-corrente de entrada',
         'Sobre-corrente de saida',
         'Sobre-temperatura no IGBT 1',
         'Sobre-temperatura no IGBT 2',
         'Sobre-tensao dos drivers dos IGBTs',
         'Sobre-corrente no driver do IGBT 1',
         'Sobre-corrente no driver do IGBT 2',
         'Sobre-temperatura nos indutores',
         'Sobre-temperatura no dissipador',
-        'Alta corrente de fuga',
         'Sobre-temperatura da placa IIB',
         'Alta umidade relativa',
-        'Bit13', 'Bit14', 'Bit15',
+        'Bit12', 'Bit13', 'Bit14', 'Bit15',
         'Bit16', 'Bit17', 'Bit18', 'Bit19',
         'Bit20', 'Bit21', 'Bit22', 'Bit23',
         'Bit24', 'Bit25', 'Bit26', 'Bit27',
         'Bit28', 'Bit29', 'Bit30', 'Bit31')
     SOFT_INTLCK_FAC_2S_ACDC = _UNDEF_INTLCK
     HARD_INTLCK_FAC_2S_ACDC = (
         'Sobre-tensao no banco de capacitores',
@@ -418,30 +415,32 @@
         'Sobre-corrente no driver do IGBT 2',
         'Erro no driver do IGBT Top 1',
         'Erro no driver do IGBT Bottom 1',
         'Erro no driver do IGBT Top 2',
         'Erro no driver do IGBT Bottom 2',
         'Sobre-temperatura nos indutores',
         'Sobre-temperatura no dissipador',
-        'Alta corrente de fuga', 'Sobre-temperatura da placa IIB',
-        'Alta umidade relativa', 'Bit19',
+        'Sobre-temperatura da placa IIB',
+        'Alta umidade relativa',
+        'Bit18', 'Bit19',
         'Bit20', 'Bit21', 'Bit22', 'Bit23',
         'Bit24', 'Bit25', 'Bit26', 'Bit27',
         'Bit28', 'Bit29', 'Bit30', 'Bit31')
     IIB_ALARMS_FAC_2P4S_DCDC = (
         'Sobre-tensao de entrada', 'Sobre-corrente de entrada',
         'Sobre-corrente de saida',
         'Sobre-temperatura no IGBT 1', 'Sobre-temperatura no IGBT 2',
         'Sobre-tensao dos drivers dos IGBTs',
         'Sobre-corrente no driver do IGBT 1',
         'Sobre-corrente no driver do IGBT 2',
         'Sobre-temperatura nos indutores',
         'Sobre-temperatura no dissipador',
-        'Alta corrente de fuga', 'Sobre-temperatura da placa IIB',
-        'Alta umidade relativa', 'Bit13', 'Bit14', 'Bit15',
+        'Sobre-temperatura da placa IIB',
+        'Alta umidade relativa',
+        'Bit12', 'Bit13', 'Bit14', 'Bit15',
         'Bit16', 'Bit17', 'Bit18', 'Bit19',
         'Bit20', 'Bit21', 'Bit22', 'Bit23',
         'Bit24', 'Bit25', 'Bit26', 'Bit27',
         'Bit28', 'Bit29', 'Bit30', 'Bit31')
     SOFT_INTLCK_FAC_2P4S_ACDC = _UNDEF_INTLCK
     HARD_INTLCK_FAC_2P4S_ACDC = (
         'Sobre-tensao no banco de capacitores',
@@ -605,30 +604,61 @@
         'Sub-tensao do DC-Link do modulo 4',
         'Interlock da placa IIB do modulo 1',
         'Interlock da placa IIB do modulo 2',
         'Interlock da placa IIB do modulo 3',
         'Interlock da placa IIB do modulo 4',
         'Bit30', 'Bit31')
     ALARMS_FAP_4P = ALARMS_FBP
-    IIB_INTLCK_FAP_4P = IIB_INTLCK_FAP
-    IIB_ALARMS_FAP_4P = (
+    IIB_INTLCK_FAP_4P_MOD1 = IIB_INTLCK_FAP
+    IIB_ALARMS_FAP_4P_MOD1 = (
         'Sobre-tensao de entrada', 'Sobre-tensao de saida',
         'Sobre-corrente no IGBT 1', 'Sobre-corrente no IGBT 2',
         'Sobre-temperatura no IGBT 1', 'Sobre-temperatura no IGBT 2',
         'Sobre-tensao dos drivers dos IGBTs',
         'Sobre-corrente no driver do IGBT 1',
         'Sobre-corrente no driver do IGBT 2',
         'Sobre-temperatura nos indutores',
         'Sobre-temperatura no dissipador', 'Alta corrente de fuga',
         'Sobre-temperatura da placa IIB', 'Alta umidade relativa',
         'Bit14', 'Bit15',
         'Bit16', 'Bit17', 'Bit18', 'Bit19',
         'Bit20', 'Bit21', 'Bit22', 'Bit23',
         'Bit24', 'Bit25', 'Bit26', 'Bit27',
         'Bit28', 'Bit29', 'Bit30', 'Bit31')
+    IIB_INTLCK_FAP_4P_MOD234 = (
+        'Sobre-tensao de entrada', 'Sobre-tensao de saida',
+        'Sobre-corrente no IGBT 1', 'Sobre-corrente no IGBT 2',
+        'Sobre-temperatura no IGBT 1', 'Sobre-temperatura no IGBT 2',
+        'Sobre-tensao dos drivers dos IGBTs',
+        'Sobre-corrente do driver do IGBT 1',
+        'Sobre-corrente do driver do IGBT 2', 'Erro no driver do IGBT 1',
+        'Erro no driver do IGBT 2', 'Sobre-temperatura nos indutores',
+        'Sobre-temperatura no dissipador',
+        'Falha no contator de entrada do DC-Link',
+        'Contator de entrada do DC-Link colado', 'Interlock externo',
+        'Interlock do rack', 'Bit17',
+        'Sobre-temperatura da placa IIB', 'Alta umidade relativa',
+        'Bit20', 'Bit21', 'Bit22', 'Bit23',
+        'Bit24', 'Bit25', 'Bit26', 'Bit27',
+        'Bit28', 'Bit29', 'Bit30', 'Bit31')
+    IIB_ALARMS_FAP_4P_MOD234 = (
+        'Sobre-tensao de entrada', 'Sobre-tensao de saida',
+        'Sobre-corrente no IGBT 1', 'Sobre-corrente no IGBT 2',
+        'Sobre-temperatura no IGBT 1', 'Sobre-temperatura no IGBT 2',
+        'Sobre-tensao dos drivers dos IGBTs',
+        'Sobre-corrente no driver do IGBT 1',
+        'Sobre-corrente no driver do IGBT 2',
+        'Sobre-temperatura nos indutores',
+        'Sobre-temperatura no dissipador', 'Bit11',
+        'Sobre-temperatura da placa IIB', 'Alta umidade relativa',
+        'Bit14', 'Bit15',
+        'Bit16', 'Bit17', 'Bit18', 'Bit19',
+        'Bit20', 'Bit21', 'Bit22', 'Bit23',
+        'Bit24', 'Bit25', 'Bit26', 'Bit27',
+        'Bit28', 'Bit29', 'Bit30', 'Bit31')
     SOFT_INTLCK_FAP_2P2S = (
         'Falha no DCCT 1', 'Falha no DCCT 2',
         'Alta diferenca entre DCCTs',
         'Falha de leitura da corrente na carga do DCCT 1',
         'Falha de leitura da corrente na carga do DCCT 2',
         'Alta diferenca entre a corrente dos bracos',
         'Alta diferenca entre a corrente dos IGBTs',
@@ -669,15 +699,15 @@
         'Interlock da placa IIB do modulo 2',
         'Interlock da placa IIB do modulo 3',
         'Interlock da placa IIB do modulo 4',
         'Sobre-corrente no braco 1',
         'Sobre-corrente no braco 2',
         'Bit31')
     ALARMS_FAP_2P2S = ALARMS_FBP
-    IIB_INTLCK_FAP_2P2S = (
+    IIB_INTLCK_FAP_2P2S_MOD1 = (
         'Sobre-tensao de entrada',
         'Sobre-tensao de saida',
         'Sobre-corrente no IGBT 1',
         'Sobre-corrente no IGBT 2',
         'Sobre-temperatura no IGBT 1',
         'Sobre-temperatura no IGBT 2',
         'Sobre-tensao dos drivers dos IGBTs',
@@ -693,15 +723,15 @@
         'Interlock do Rack',
         'Alta corrente de fuga',
         'Sobre-temperatura da placa IIB',
         'Alta umidade relativa',
         'Bit20', 'Bit21', 'Bit22', 'Bit23',
         'Bit24', 'Bit25', 'Bit26', 'Bit27',
         'Bit28', 'Bit29', 'Bit30', 'Bit31')
-    IIB_ALARMS_FAP_2P2S = (
+    IIB_ALARMS_FAP_2P2S_MOD1 = (
         'Sobre-tensao de entrada',
         'Sobre-tensao de saida',
         'Sobre-corrente no IGBT 1',
         'Sobre-corrente no IGBT 2',
         'Sobre-temperatura no IGBT 1',
         'Sobre-temperatura no IGBT 2',
         'Sobre-tensao nos drivers dos IGBTs',
@@ -713,14 +743,58 @@
         'Sobre-temperatura na placa IIB',
         'Alta umidade relativa',
         'Bit14', 'Bit15',
         'Bit16', 'Bit17', 'Bit18', 'Bit19',
         'Bit20', 'Bit21', 'Bit22', 'Bit23',
         'Bit24', 'Bit25', 'Bit26', 'Bit27',
         'Bit28', 'Bit29', 'Bit30', 'Bit31')
+    IIB_INTLCK_FAP_2P2S_MOD234 = (
+        'Sobre-tensao de entrada',
+        'Sobre-tensao de saida',
+        'Sobre-corrente no IGBT 1',
+        'Sobre-corrente no IGBT 2',
+        'Sobre-temperatura no IGBT 1',
+        'Sobre-temperatura no IGBT 2',
+        'Sobre-tensao dos drivers dos IGBTs',
+        'Sobre-corrente no driver do IGBT 1',
+        'Sobre-corrente no driver do IGBT 2',
+        'Erro no driver do IGBT 1',
+        'Erro no driver do IGBT 2',
+        'Sobre-temperatura nos indutores',
+        'Sobre-temperatura no dissipador',
+        'Falha no contator de entrada do DC-Link',
+        'Contator de entrada do DC-Link colado',
+        'Interlock Externo',
+        'Interlock do Rack',
+        'Bit17',
+        'Sobre-temperatura da placa IIB',
+        'Alta umidade relativa',
+        'Bit20', 'Bit21', 'Bit22', 'Bit23',
+        'Bit24', 'Bit25', 'Bit26', 'Bit27',
+        'Bit28', 'Bit29', 'Bit30', 'Bit31')
+    IIB_ALARMS_FAP_2P2S_MOD234 = (
+        'Sobre-tensao de entrada',
+        'Sobre-tensao de saida',
+        'Sobre-corrente no IGBT 1',
+        'Sobre-corrente no IGBT 2',
+        'Sobre-temperatura no IGBT 1',
+        'Sobre-temperatura no IGBT 2',
+        'Sobre-tensao nos drivers dos IGBTs',
+        'Sobre-corrente no driver do IGBT 1',
+        'Sobre-corrente no driver do IGBT 2',
+        'Sobre-temperatura nos indutores',
+        'Sobre-temperatura no dissipador',
+        'Bit11',
+        'Sobre-temperatura na placa IIB',
+        'Alta umidade relativa',
+        'Bit14', 'Bit15',
+        'Bit16', 'Bit17', 'Bit18', 'Bit19',
+        'Bit20', 'Bit21', 'Bit22', 'Bit23',
+        'Bit24', 'Bit25', 'Bit26', 'Bit27',
+        'Bit28', 'Bit29', 'Bit30', 'Bit31')
 
     CYCLE_TYPES = ['', ] * 5
     CYCLE_TYPES[_ConstPSBSMP.E_SIGGENTYPE_SINE] = 'Sine'
     CYCLE_TYPES[_ConstPSBSMP.E_SIGGENTYPE_DAMPEDSINE] = 'DampedSine'
     CYCLE_TYPES[_ConstPSBSMP.E_SIGGENTYPE_TRAPEZOIDAL] = 'Trapezoidal'
     CYCLE_TYPES[_ConstPSBSMP.E_SIGGENTYPE_DAMPEDSQUAREDSINE] = \
         'DampedSquaredSine'
@@ -862,14 +936,82 @@
             aux = k.split('Mod')
             aux = aux[1].split('Labels-Cte')
             mod = aux[0]
             modules.add(mod)
     return sorted(modules)
 
 
+def get_ps_scopesourcemap(psname):
+    """Return PS modules for a power supply model."""
+    psmodel = _PSSearch.conv_psname_2_psmodel(psname)
+    psudcindex = _PSSearch.conv_psname_2_udcindex(psname)
+    if psmodel == 'FBP':
+        return {
+            'Output current [A]': 0xD000 + 2*psudcindex,
+            'Output voltage [V]': 0xC008 + 2*psudcindex,
+            'Tracking error [A or V]': 0xD008 + 2*psudcindex,
+            'DCLink voltage [V]': 0xC000 + 2*psudcindex,
+            'PWM duty cycle [p.u.]': 0xD040 + 2*psudcindex,
+        }
+    if psmodel == 'FAC_DCDC':
+        return {
+            'Output current [A]': 0xD006,
+            'Output voltage [V]': 0xC000,
+            'Tracking error [A or V]': 0xD008,
+            'DCLink voltage [V]': 0xD004,
+            'PWM duty cycle [p.u.]': 0xD040,
+        }
+    if psmodel == 'FAC_2S_DCDC':
+        return {
+            'Output current [A]': 0xD008,
+            'Tracking error [A or V]': 0xD00A,
+            'PWM duty cycle [p.u.]': 0xD040,
+        }
+    if psmodel == 'FAC_2S_ACDC':
+        return {
+            'Output voltage [V]': 0xD000 + 2*psudcindex,
+            'Tracking error [A or V]': 0xD00C + 14*psudcindex,
+            'PWM duty cycle [p.u.]': 0xD040 + 2*psudcindex,
+        }
+    if psmodel == 'FAC_2P4S_DCDC':
+        return {
+            'Output current [A]': 0xD008,
+            'Tracking error [A or V]': 0xD00A,
+            'PWM duty cycle [p.u.]': 0xD040,
+        }
+    if psmodel == 'FAC_2P4S_ACDC':
+        return {
+            'Output voltage [V]': 0xD000 + 2*psudcindex,
+            'Tracking error [A or V]': 0xD00C + 14*psudcindex,
+            'DCLink voltage [V]': 0xC000 + 2*psudcindex,
+            'PWM duty cycle [p.u.]': 0xD040 + 2*psudcindex,
+        }
+    if psmodel == 'FAP':
+        return {
+            'Output current [A]': 0xD006,
+            'Output voltage [V]': 0xC004,
+            'Tracking error [A or V]': 0xD008,
+            'DCLink voltage [V]': 0xD004,
+            'PWM duty cycle [p.u.]': 0xD040,
+        }
+    if psmodel == 'FAP_2P2S':
+        return {
+            'Output current [A]': 0xD008,
+            'Tracking error [A or V]': 0xD00A,
+            'PWM duty cycle [p.u.]': 0xD040,
+        }
+    if psmodel == 'FAP_4P':
+        return {
+            'Output current [A]': 0xD006,
+            'Tracking error [A or V]': 0xD008,
+            'PWM duty cycle [p.u.]': 0xD040,
+        }
+    return dict()
+
+
 # --- Auxiliary functions ---
 
 
 def _get_ps_common_propty_database():
     """Return database entries to all BSMP-like devices."""
     dbase = {
         'Version-Cte': {'type': 'str', 'value': 'UNDEF'},
@@ -1428,15 +1570,14 @@
             'lolo': 0, 'low': 0, 'lolim': 0,
             'hilim': 4194303, 'high': 4194303, 'hihi': 4194303},
         'TestWavePeriod-RB': {
             'type': 'int', 'value': 0,
             'lolo': 0, 'low': 0, 'lolim': 0,
             'hilim': 4194303, 'high': 4194303, 'hihi': 4194303},
         # Status and Alarms
-        'PSStatus-Mon': {'type': 'int', 'value': 0},
         'AlarmsAmp-Mon': {'type': 'int', 'value': 0},
         'AlarmsAmpLabels-Cte': {
             'type': 'string', 'count': len(_et.FOFB_ALARMS_AMP),
             'value': _et.FOFB_ALARMS_AMP},
         # PI control
         'CurrLoopKp-SP': {'type': 'int', 'value': 0},
         'CurrLoopKp-RB': {'type': 'int', 'value': 0},
@@ -1623,14 +1764,17 @@
         'CapacitorBankVoltage-Mon': {'type': 'float', 'value': 0.0,
                                      'prec': PS_CURRENT_PRECISION,
                                      'lolim': 0.0, 'hilim': 1.0,
                                      'unit': 'V'},
         'PWMDutyCycle-Mon': {'type': 'float', 'value': 0.0,
                              'prec': PS_CURRENT_PRECISION,
                              'unit': 'p.u.'},
+        'LeakCurrent-Mon': {'type': 'float', 'value': 0.0,
+                            'prec': PS_CURRENT_PRECISION,
+                            'unit': 'A'},
         'VoltageInputIIB-Mon': {'type': 'float', 'value': 0.0,
                                 'prec': PS_CURRENT_PRECISION,
                                 'unit': 'V'},
         'CurrentInputIIB-Mon': {'type': 'float', 'value': 0.0,
                                 'prec': PS_CURRENT_PRECISION,
                                 'unit': 'A'},
         'CurrentOutputIIB-Mon': {'type': 'float', 'value': 0.0,
@@ -1649,17 +1793,14 @@
                                      'unit': 'V'},
         'IGBT1DriverCurrentIIB-Mon': {'type': 'float', 'value': 0.0,
                                       'prec': PS_CURRENT_PRECISION,
                                       'unit': 'A'},
         'IGBT2DriverCurrentIIB-Mon': {'type': 'float', 'value': 0.0,
                                       'prec': PS_CURRENT_PRECISION,
                                       'unit': 'A'},
-        'LeakCurrentIIB-Mon': {'type': 'float', 'value': 0.0,
-                               'prec': PS_CURRENT_PRECISION,
-                               'unit': 'A'},
         'BoardTemperatureIIB-Mon': {'type': 'float', 'value': 0.0,
                                     'prec': 2, 'unit': 'C'},
         'RelativeHumidityIIB-Mon': {'type': 'float', 'value': 0.0,
                                     'unit': '%'},
         'IntlkIIB-Mon': {'type': 'int', 'value': 0, 'unit': 'interlock'},
         'IntlkIIBLabels-Cte': {
             'type': 'string',
@@ -2345,14 +2486,17 @@
                                       'unit': 'p.u.'},
         'IGBT1PWMDutyCycleMod4-Mon': {'type': 'float', 'value': 0.0,
                                       'prec': PS_CURRENT_PRECISION,
                                       'unit': 'p.u.'},
         'IGBT2PWMDutyCycleMod4-Mon': {'type': 'float', 'value': 0.0,
                                       'prec': PS_CURRENT_PRECISION,
                                       'unit': 'p.u.'},
+        'LeakCurrent-Mon': {'type': 'float', 'value': 0.0,
+                            'prec': PS_CURRENT_PRECISION,
+                            'unit': 'A'},
         'VoltageInputIIBMod1-Mon': {'type': 'float', 'value': 0.0,
                                     'prec': PS_CURRENT_PRECISION,
                                     'unit': 'V'},
         'VoltageOutputIIBMod1-Mon': {'type': 'float', 'value': 0.0,
                                      'prec': PS_CURRENT_PRECISION,
                                      'unit': 'V'},
         'IGBT1CurrentIIBMod1-Mon': {'type': 'float', 'value': 0.0,
@@ -2374,33 +2518,30 @@
         'IGBT2DriverCurrentIIBMod1-Mon': {'type': 'float', 'value': 0.0,
                                           'prec': PS_CURRENT_PRECISION,
                                           'unit': 'A'},
         'InductorTemperatureIIBMod1-Mon': {'type': 'float', 'value': 0.0,
                                            'prec': 2, 'unit': 'C'},
         'HeatSinkTemperatureIIBMod1-Mon': {'type': 'float', 'value': 0.0,
                                            'prec': 2, 'unit': 'C'},
-        'LeakageCurrentIIBMod1-Mon': {'type': 'float', 'value': 0.0,
-                                      'prec': PS_CURRENT_PRECISION,
-                                      'unit': 'A'},
         'TemperatureIIBMod1-Mon': {'type': 'float', 'value': 0.0,
                                    'prec': 2, 'unit': 'C'},
         'RelativeHumidityIIBMod1-Mon': {
             'type': 'float', 'value': 0.0,
             'prec': 2,
             'unit': '%'},
         'IntlkIIBMod1-Mon': {'type': 'int', 'value': 0, 'unit': 'interlock'},
         'IntlkIIBMod1Labels-Cte': {
             'type': 'string',
-            'count': len(_et.IIB_INTLCK_FAP_4P),
-            'value': _et.IIB_INTLCK_FAP_4P,
+            'count': len(_et.IIB_INTLCK_FAP_4P_MOD1),
+            'value': _et.IIB_INTLCK_FAP_4P_MOD1,
             'unit': 'interlock'},
         'AlarmsIIBMod1-Mon': {'type': 'int', 'value': 0},
         'AlarmsIIBMod1Labels-Cte': {'type': 'string',
-                                    'count': len(_et.IIB_ALARMS_FAP_4P),
-                                    'value': _et.IIB_ALARMS_FAP_4P},
+                                    'count': len(_et.IIB_ALARMS_FAP_4P_MOD1),
+                                    'value': _et.IIB_ALARMS_FAP_4P_MOD1},
         'VoltageInputIIBMod2-Mon': {'type': 'float', 'value': 0.0,
                                     'prec': PS_CURRENT_PRECISION,
                                     'unit': 'V'},
         'VoltageOutputIIBMod2-Mon': {'type': 'float', 'value': 0.0,
                                      'prec': PS_CURRENT_PRECISION,
                                      'unit': 'V'},
         'IGBT1CurrentIIBMod2-Mon': {'type': 'float', 'value': 0.0,
@@ -2422,34 +2563,31 @@
         'IGBT2DriverCurrentIIBMod2-Mon': {'type': 'float', 'value': 0.0,
                                           'prec': PS_CURRENT_PRECISION,
                                           'unit': 'A'},
         'InductorTemperatureIIBMod2-Mon': {'type': 'float', 'value': 0.0,
                                            'prec': 2, 'unit': 'C'},
         'HeatSinkTemperatureIIBMod2-Mon': {'type': 'float', 'value': 0.0,
                                            'prec': 2, 'unit': 'C'},
-        'LeakageCurrentIIBMod2-Mon': {'type': 'float', 'value': 0.0,
-                                      'prec': PS_CURRENT_PRECISION,
-                                      'unit': 'A'},
         'TemperatureIIBMod2-Mon': {'type': 'float', 'value': 0.0,
                                    'prec': 2, 'unit': 'C'},
         'RelativeHumidityIIBMod2-Mon': {
             'type': 'float', 'value': 0.0,
             'prec': 2,
             'unit': '%'},
         'IntlkIIBMod2-Mon': {
             'type': 'int', 'value': 0, 'unit': 'interlock'},
         'IntlkIIBMod2Labels-Cte': {
             'type': 'string',
-            'count': len(_et.IIB_INTLCK_FAP_4P),
-            'value': _et.IIB_INTLCK_FAP_4P,
+            'count': len(_et.IIB_INTLCK_FAP_4P_MOD234),
+            'value': _et.IIB_INTLCK_FAP_4P_MOD234,
             'unit': 'interlock'},
         'AlarmsIIBMod2-Mon': {'type': 'int', 'value': 0},
         'AlarmsIIBMod2Labels-Cte': {'type': 'string',
-                                    'count': len(_et.IIB_ALARMS_FAP_4P),
-                                    'value': _et.IIB_ALARMS_FAP_4P},
+                                    'count': len(_et.IIB_ALARMS_FAP_4P_MOD234),
+                                    'value': _et.IIB_ALARMS_FAP_4P_MOD234},
         'VoltageInputIIBMod3-Mon': {'type': 'float', 'value': 0.0,
                                     'prec': PS_CURRENT_PRECISION,
                                     'unit': 'V'},
         'VoltageOutputIIBMod3-Mon': {'type': 'float', 'value': 0.0,
                                      'prec': PS_CURRENT_PRECISION,
                                      'unit': 'V'},
         'IGBT1CurrentIIBMod3-Mon': {'type': 'float', 'value': 0.0,
@@ -2471,33 +2609,31 @@
         'IGBT2DriverCurrentIIBMod3-Mon': {'type': 'float', 'value': 0.0,
                                           'prec': PS_CURRENT_PRECISION,
                                           'unit': 'A'},
         'InductorTemperatureIIBMod3-Mon': {'type': 'float', 'value': 0.0,
                                            'prec': 2, 'unit': 'C'},
         'HeatSinkTemperatureIIBMod3-Mon': {'type': 'float', 'value': 0.0,
                                            'prec': 2, 'unit': 'C'},
-        'LeakageCurrentIIBMod3-Mon': {'type': 'float', 'value': 0.0,
-                                      'prec': PS_CURRENT_PRECISION,
-                                      'unit': 'A'},
         'TemperatureIIBMod3-Mon': {'type': 'float', 'value': 0.0,
                                    'prec': 2, 'unit': 'C'},
         'RelativeHumidityIIBMod3-Mon': {
             'type': 'float', 'value': 0.0,
             'prec': 2,
             'unit': '%'},
         'IntlkIIBMod3-Mon': {'type': 'int', 'value': 0, 'unit': 'interlock'},
         'IntlkIIBMod3Labels-Cte': {
             'type': 'string',
-            'count': len(_et.IIB_INTLCK_FAP_4P),
-            'value': _et.IIB_INTLCK_FAP_4P,
+            'count': len(_et.IIB_INTLCK_FAP_4P_MOD234),
+            'value': _et.IIB_INTLCK_FAP_4P_MOD234,
             'unit': 'interlock'},
         'AlarmsIIBMod3-Mon': {'type': 'int', 'value': 0},
-        'AlarmsIIBMod3Labels-Cte': {'type': 'string',
-                                    'count': len(_et.IIB_ALARMS_FAP_4P),
-                                    'value': _et.IIB_ALARMS_FAP_4P},
+        'AlarmsIIBMod3Labels-Cte': {
+            'type': 'string',
+            'count': len(_et.IIB_ALARMS_FAP_4P_MOD234),
+            'value': _et.IIB_ALARMS_FAP_4P_MOD234},
         'VoltageInputIIBMod4-Mon': {'type': 'float', 'value': 0.0,
                                     'prec': PS_CURRENT_PRECISION,
                                     'unit': 'V'},
         'VoltageOutputIIBMod4-Mon': {'type': 'float', 'value': 0.0,
                                      'prec': PS_CURRENT_PRECISION,
                                      'unit': 'V'},
         'IGBT1CurrentIIBMod4-Mon': {'type': 'float', 'value': 0.0,
@@ -2519,33 +2655,31 @@
         'IGBT2DriverCurrentIIBMod4-Mon': {'type': 'float', 'value': 0.0,
                                           'prec': PS_CURRENT_PRECISION,
                                           'unit': 'A'},
         'InductorTemperatureIIBMod4-Mon': {'type': 'float', 'value': 0.0,
                                            'prec': 2, 'unit': 'C'},
         'HeatSinkTemperatureIIBMod4-Mon': {'type': 'float', 'value': 0.0,
                                            'prec': 2, 'unit': 'C'},
-        'LeakageCurrentIIBMod4-Mon': {'type': 'float', 'value': 0.0,
-                                      'prec': PS_CURRENT_PRECISION,
-                                      'unit': 'A'},
         'TemperatureIIBMod4-Mon': {'type': 'float', 'value': 0.0,
                                    'prec': 2, 'unit': 'C'},
         'RelativeHumidityIIBMod4-Mon': {
             'type': 'float', 'value': 0.0,
             'prec': 2,
             'unit': '%'},
         'IntlkIIBMod4-Mon': {'type': 'int', 'value': 0, 'unit': 'interlock'},
         'IntlkIIBMod4Labels-Cte': {
             'type': 'string',
-            'count': len(_et.IIB_INTLCK_FAP_4P),
-            'value': _et.IIB_INTLCK_FAP_4P,
+            'count': len(_et.IIB_INTLCK_FAP_4P_MOD234),
+            'value': _et.IIB_INTLCK_FAP_4P_MOD234,
             'unit': 'interlock'},
         'AlarmsIIBMod4-Mon': {'type': 'int', 'value': 0},
-        'AlarmsIIBMod4Labels-Cte': {'type': 'string',
-                                    'count': len(_et.IIB_ALARMS_FAP_4P),
-                                    'value': _et.IIB_ALARMS_FAP_4P},
+        'AlarmsIIBMod4Labels-Cte': {
+            'type': 'string',
+            'count': len(_et.IIB_ALARMS_FAP_4P_MOD234),
+            'value': _et.IIB_ALARMS_FAP_4P_MOD234},
         }
     propty_db.update(db_ps)
     return propty_db
 
 
 def _get_ps_FAP_2P2S_propty_database():
     """Return database with FAP_2P2S pwrsupply model PVs."""
@@ -2652,14 +2786,17 @@
                                       'unit': 'p.u.'},
         'IGBT1PWMDutyCycleMod4-Mon': {'type': 'float', 'value': 0.0,
                                       'prec': PS_CURRENT_PRECISION,
                                       'unit': 'p.u.'},
         'IGBT2PWMDutyCycleMod4-Mon': {'type': 'float', 'value': 0.0,
                                       'prec': PS_CURRENT_PRECISION,
                                       'unit': 'p.u.'},
+        'LeakCurrent-Mon': {'type': 'float', 'value': 0.0,
+                            'prec': PS_CURRENT_PRECISION,
+                            'unit': 'A'},
         'VoltageInputIIBMod1-Mon': {'type': 'float', 'value': 0.0,
                                     'prec': PS_CURRENT_PRECISION,
                                     'unit': 'V'},
         'VoltageOutputIIBMod1-Mon': {'type': 'float', 'value': 0.0,
                                      'prec': PS_CURRENT_PRECISION,
                                      'unit': 'V'},
         'IGBT1CurrentIIBMod1-Mon': {'type': 'float', 'value': 0.0,
@@ -2685,27 +2822,24 @@
                                            'prec': 2, 'unit': 'C'},
         'HeatSinkTemperatureIIBMod1-Mon': {'type': 'float', 'value': 0.0,
                                            'prec': 2, 'unit': 'C'},
         'TemperatureIIBMod1-Mon': {'type': 'float', 'value': 0.0,
                                    'prec': 2, 'unit': 'C'},
         'RelativeHumidityIIBMod1-Mon': {'type': 'float', 'value': 0.0,
                                         'prec': 2, 'unit': '%'},
-        'LeakageCurrentIIBMod1-Mon': {'type': 'float', 'value': 0.0,
-                                      'prec': PS_CURRENT_PRECISION,
-                                      'unit': 'A'},
         'IntlkIIBMod1-Mon': {'type': 'int', 'value': 0, 'unit': 'interlock'},
         'IntlkIIBMod1Labels-Cte':  {
             'type': 'string',
-            'count': len(_et.IIB_INTLCK_FAP_2P2S),
-            'value': _et.IIB_INTLCK_FAP_2P2S,
+            'count': len(_et.IIB_INTLCK_FAP_2P2S_MOD1),
+            'value': _et.IIB_INTLCK_FAP_2P2S_MOD1,
             'unit': 'interlock'},
         'AlarmsIIBMod1-Mon': {'type': 'int', 'value': 0},
         'AlarmsIIBMod1Labels-Cte': {'type': 'string',
-                                    'count': len(_et.IIB_ALARMS_FAP_2P2S),
-                                    'value': _et.IIB_ALARMS_FAP_2P2S},
+                                    'count': len(_et.IIB_ALARMS_FAP_2P2S_MOD1),
+                                    'value': _et.IIB_ALARMS_FAP_2P2S_MOD1},
         'VoltageInputIIBMod2-Mon': {'type': 'float', 'value': 0.0,
                                     'prec': PS_CURRENT_PRECISION,
                                     'unit': 'V'},
         'VoltageOutputIIBMod2-Mon': {'type': 'float', 'value': 0.0,
                                      'prec': PS_CURRENT_PRECISION,
                                      'unit': 'V'},
         'IGBT1CurrentIIBMod2-Mon': {'type': 'float', 'value': 0.0,
@@ -2736,21 +2870,22 @@
         'TemperatureIIBMod2-Mon': {'type': 'float', 'value': 0.0,
                                    'prec': 2, 'unit': 'C'},
         'RelativeHumidityIIBMod2-Mon': {'type': 'float', 'value': 0.0,
                                         'prec': 2, 'unit': '%'},
         'IntlkIIBMod2-Mon': {'type': 'int', 'value': 0, 'unit': 'interlock'},
         'IntlkIIBMod2Labels-Cte': {
             'type': 'string',
-            'count': len(_et.IIB_INTLCK_FAP_2P2S),
-            'value': _et.IIB_INTLCK_FAP_2P2S,
+            'count': len(_et.IIB_INTLCK_FAP_2P2S_MOD234),
+            'value': _et.IIB_INTLCK_FAP_2P2S_MOD234,
             'unit': 'interlock'},
         'AlarmsIIBMod2-Mon': {'type': 'int', 'value': 0},
-        'AlarmsIIBMod2Labels-Cte': {'type': 'string',
-                                    'count': len(_et.IIB_ALARMS_FAP_2P2S),
-                                    'value': _et.IIB_ALARMS_FAP_2P2S},
+        'AlarmsIIBMod2Labels-Cte': {
+            'type': 'string',
+            'count': len(_et.IIB_ALARMS_FAP_2P2S_MOD234),
+            'value': _et.IIB_ALARMS_FAP_2P2S_MOD234},
         'VoltageInputIIBMod3-Mon': {'type': 'float', 'value': 0.0,
                                     'prec': PS_CURRENT_PRECISION,
                                     'unit': 'V'},
         'VoltageOutputIIBMod3-Mon': {'type': 'float', 'value': 0.0,
                                      'prec': PS_CURRENT_PRECISION,
                                      'unit': 'V'},
         'IGBT1CurrentIIBMod3-Mon': {'type': 'float', 'value': 0.0,
@@ -2776,27 +2911,25 @@
                                            'prec': 2, 'unit': 'C'},
         'HeatSinkTemperatureIIBMod3-Mon': {'type': 'float', 'value': 0.0,
                                            'prec': 2, 'unit': 'C'},
         'TemperatureIIBMod3-Mon': {'type': 'float', 'value': 0.0,
                                    'prec': 2, 'unit': 'C'},
         'RelativeHumidityIIBMod3-Mon': {'type': 'float', 'value': 0.0,
                                         'prec': 2, 'unit': '%'},
-        'LeakageCurrentIIBMod3-Mon': {'type': 'float', 'value': 0.0,
-                                      'prec': PS_CURRENT_PRECISION,
-                                      'unit': 'A'},
         'IntlkIIBMod3-Mon': {'type': 'int', 'value': 0, 'unit': 'interlock'},
         'IntlkIIBMod3Labels-Cte':  {
             'type': 'string',
-            'count': len(_et.IIB_INTLCK_FAP_2P2S),
-            'value': _et.IIB_INTLCK_FAP_2P2S,
+            'count': len(_et.IIB_INTLCK_FAP_2P2S_MOD234),
+            'value': _et.IIB_INTLCK_FAP_2P2S_MOD234,
             'unit': 'interlock'},
         'AlarmsIIBMod3-Mon': {'type': 'int', 'value': 0},
-        'AlarmsIIBMod3Labels-Cte': {'type': 'string',
-                                    'count': len(_et.IIB_ALARMS_FAP_2P2S),
-                                    'value': _et.IIB_ALARMS_FAP_2P2S},
+        'AlarmsIIBMod3Labels-Cte': {
+            'type': 'string',
+            'count': len(_et.IIB_ALARMS_FAP_2P2S_MOD234),
+            'value': _et.IIB_ALARMS_FAP_2P2S_MOD234},
         'VoltageInputIIBMod4-Mon': {'type': 'float', 'value': 0.0,
                                     'prec': PS_CURRENT_PRECISION,
                                     'unit': 'V'},
         'VoltageOutputIIBMod4-Mon': {'type': 'float', 'value': 0.0,
                                      'prec': PS_CURRENT_PRECISION,
                                      'unit': 'V'},
         'IGBT1CurrentIIBMod4-Mon': {'type': 'float', 'value': 0.0,
@@ -2825,27 +2958,25 @@
         'HeatSinkTemperatureIIBMod4-Mon': {'type': 'float', 'value': 0.0,
                                            'prec': 2, 'unit': 'C'},
         'TemperatureIIBMod4-Mon': {'type': 'float', 'value': 0.0,
                                    'prec': 2,
                                    'unit': 'C'},
         'RelativeHumidityIIBMod4-Mon': {'type': 'float', 'value': 0.0,
                                         'prec': 2, 'unit': '%'},
-        'LeakageCurrentIIBMod4-Mon': {'type': 'float', 'value': 0.0,
-                                      'prec': PS_CURRENT_PRECISION,
-                                      'unit': 'A'},
         'IntlkIIBMod4-Mon': {'type': 'int', 'value': 0, 'unit': 'interlock'},
         'IntlkIIBMod4Labels-Cte':  {
             'type': 'string',
-            'count': len(_et.IIB_INTLCK_FAP_2P2S),
-            'value': _et.IIB_INTLCK_FAP_2P2S,
+            'count': len(_et.IIB_INTLCK_FAP_2P2S_MOD234),
+            'value': _et.IIB_INTLCK_FAP_2P2S_MOD234,
             'unit': 'interlock'},
         'AlarmsIIBMod4-Mon': {'type': 'int', 'value': 0},
-        'AlarmsIIBMod4Labels-Cte': {'type': 'string',
-                                    'count': len(_et.IIB_ALARMS_FAP_2P2S),
-                                    'value': _et.IIB_ALARMS_FAP_2P2S},
+        'AlarmsIIBMod4Labels-Cte': {
+            'type': 'string',
+            'count': len(_et.IIB_ALARMS_FAP_2P2S_MOD234),
+            'value': _et.IIB_ALARMS_FAP_2P2S_MOD234},
     }
     propty_db.update(db_ps)
     return propty_db
 
 
 # --- Others ---
```

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/data.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/factory.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/pructrl/__init__.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/pructrl/pru.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/pructrl/prucontroller.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/prucontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/pructrl/prucparms.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/prucparms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/pructrl/psdevstate.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/psdevstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/pructrl/udc.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/pructrl/udc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/psctrl/__init__.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/psctrl/pscontroller.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/psctrl/pscreaders.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscreaders.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/psctrl/pscstatus.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscstatus.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/psctrl/pscwriters.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/psctrl/psmodel.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/psctrl/psmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,25 +355,25 @@
         'IntlkSoft-Mon': _c.V_PS_SOFT_INTERLOCKS,
         'IntlkHard-Mon': _c.V_PS_HARD_INTERLOCKS,
         'Current-Mon': _c.V_I_LOAD_MEAN,
         'Current1-Mon': _c.V_I_LOAD1,
         'Current2-Mon': _c.V_I_LOAD2,
         'CapacitorBankVoltage-Mon': _c.V_V_CAPBANK,
         'PWMDutyCycle-Mon': _c.V_DUTY_CYCLE,
+        'LeakCurrent-Mon': _c.V_I_LEAKAGE,
         'VoltageInputIIB-Mon': _c.V_V_INPUT_IIB,
         'CurrentInputIIB-Mon': _c.V_I_INPUT_IIB,
         'CurrentOutputIIB-Mon': _c.V_I_OUTPUT_IIB,
         'IGBT1TemperatureIIB-Mon': _c.V_TEMP_IGBT_1_IIB,
         'IGBT2TemperatureIIB-Mon': _c.V_TEMP_IGBT_2_IIB,
         'InductorsTemperatureIIB-Mon': _c.V_TEMP_INDUCTOR_IIB,
         'HeatSinkTemperatureIIB-Mon': _c.V_TEMP_HEATSINK_IIB,
         'IGBTDriverVoltageIIB-Mon': _c.V_V_DRIVER_IIB,
         'IGBT1DriverCurrentIIB-Mon': _c.V_I_DRIVER_1_IIB,
         'IGBT2DriverCurrentIIB-Mon': _c.V_I_DRIVER_2_IIB,
-        'LeakCurrentIIB-Mon': _c.V_I_LEAKAGE_IIB,
         'BoardTemperatureIIB-Mon': _c.V_TEMP_BOARD_IIB,
         'RelativeHumidityIIB-Mon': _c.V_RH_IIB,
         'IntlkIIB-Mon': _c.V_IIB_INTERLOCKS,
         'AlarmsIIB-Mon': _c.V_IIB_ALARMS,
         'Alarms-Mon': _c.V_PS_ALARMS,
     }
 
@@ -572,26 +572,26 @@
         'IGBT2PWMDutyCycleMod1-Mon': _c.V_DUTY_CYCLE_2_1,
         'IGBT1PWMDutyCycleMod2-Mon': _c.V_DUTY_CYCLE_1_2,
         'IGBT2PWMDutyCycleMod2-Mon': _c.V_DUTY_CYCLE_2_2,
         'IGBT1PWMDutyCycleMod3-Mon': _c.V_DUTY_CYCLE_1_3,
         'IGBT2PWMDutyCycleMod3-Mon': _c.V_DUTY_CYCLE_2_3,
         'IGBT1PWMDutyCycleMod4-Mon': _c.V_DUTY_CYCLE_1_4,
         'IGBT2PWMDutyCycleMod4-Mon': _c.V_DUTY_CYCLE_2_4,
+        'LeakCurrent-Mon': _c.V_I_LEAKAGE,
         'VoltageInputIIBMod1-Mon': _c.V_V_INPUT_IIB_1,
         'VoltageOutputIIBMod1-Mon': _c.V_V_OUTPUT_IIB_1,
         'IGBT1CurrentIIBMod1-Mon': _c.V_I_IGBT_1_IIB_1,
         'IGBT2CurrentIIBMod1-Mon': _c.V_I_IGBT_2_IIB_1,
         'IGBT1TemperatureIIBMod1-Mon': _c.V_TEMP_IGBT_1_IIB_1,
         'IGBT2TemperatureIIBMod1-Mon': _c.V_TEMP_IGBT_2_IIB_1,
         'IGBTDriverVoltageIIBMod1-Mon': _c.V_V_DRIVER_IIB_1,
         'IGBT1DriverCurrentIIBMod1-Mon': _c.V_I_DRIVER_1_IIB_1,
         'IGBT2DriverCurrentIIBMod1-Mon': _c.V_I_DRIVER_2_IIB_1,
         'InductorTemperatureIIBMod1-Mon': _c.V_TEMP_INDUCTOR_IIB_1,
         'HeatSinkTemperatureIIBMod1-Mon': _c.V_TEMP_HEATSINK_IIB_1,
-        'LeakageCurrentIIBMod1-Mon': _c.V_I_LEAKAGE_IIB_1,
         'TemperatureIIBMod1-Mon': _c.V_TEMP_BOARD_IIB_1,
         'RelativeHumidityIIBMod1-Mon': _c.V_RH_IIB_1,
         'IntlkIIBMod1-Mon': _c.V_IIB_INTERLOCKS_1,
         'AlarmsIIBMod1-Mon': _c.V_IIB_ALARMS_1,
         'VoltageInputIIBMod2-Mon': _c.V_V_INPUT_IIB_2,
         'VoltageOutputIIBMod2-Mon': _c.V_V_OUTPUT_IIB_2,
         'IGBT1CurrentIIBMod2-Mon': _c.V_I_IGBT_1_IIB_2,
@@ -599,15 +599,14 @@
         'IGBT1TemperatureIIBMod2-Mon': _c.V_TEMP_IGBT_1_IIB_2,
         'IGBT2TemperatureIIBMod2-Mon': _c.V_TEMP_IGBT_2_IIB_2,
         'IGBTDriverVoltageIIBMod2-Mon': _c.V_V_DRIVER_IIB_2,
         'IGBT1DriverCurrentIIBMod2-Mon': _c.V_I_DRIVER_1_IIB_2,
         'IGBT2DriverCurrentIIBMod2-Mon': _c.V_I_DRIVER_2_IIB_2,
         'InductorTemperatureIIBMod2-Mon': _c.V_TEMP_INDUCTOR_IIB_2,
         'HeatSinkTemperatureIIBMod2-Mon': _c.V_TEMP_HEATSINK_IIB_2,
-        'LeakageCurrentIIBMod2-Mon': _c.V_I_LEAKAGE_IIB_2,
         'TemperatureIIBMod2-Mon': _c.V_TEMP_BOARD_IIB_2,
         'RelativeHumidityIIBMod2-Mon': _c.V_RH_IIB_2,
         'IntlkIIBMod2-Mon': _c.V_IIB_INTERLOCKS_2,
         'AlarmsIIBMod2-Mon': _c.V_IIB_ALARMS_2,
         'VoltageInputIIBMod3-Mon': _c.V_V_INPUT_IIB_3,
         'VoltageOutputIIBMod3-Mon': _c.V_V_OUTPUT_IIB_3,
         'IGBT1CurrentIIBMod3-Mon': _c.V_I_IGBT_1_IIB_3,
@@ -615,15 +614,14 @@
         'IGBT1TemperatureIIBMod3-Mon': _c.V_TEMP_IGBT_1_IIB_3,
         'IGBT2TemperatureIIBMod3-Mon': _c.V_TEMP_IGBT_2_IIB_3,
         'IGBTDriverVoltageIIBMod3-Mon': _c.V_V_DRIVER_IIB_3,
         'IGBT1DriverCurrentIIBMod3-Mon': _c.V_I_DRIVER_1_IIB_3,
         'IGBT2DriverCurrentIIBMod3-Mon': _c.V_I_DRIVER_2_IIB_3,
         'InductorTemperatureIIBMod3-Mon': _c.V_TEMP_INDUCTOR_IIB_3,
         'HeatSinkTemperatureIIBMod3-Mon': _c.V_TEMP_HEATSINK_IIB_3,
-        'LeakageCurrentIIBMod3-Mon': _c.V_I_LEAKAGE_IIB_3,
         'TemperatureIIBMod3-Mon': _c.V_TEMP_BOARD_IIB_3,
         'RelativeHumidityIIBMod3-Mon': _c.V_RH_IIB_3,
         'IntlkIIBMod3-Mon': _c.V_IIB_INTERLOCKS_3,
         'AlarmsIIBMod3-Mon': _c.V_IIB_ALARMS_3,
         'VoltageInputIIBMod4-Mon': _c.V_V_INPUT_IIB_4,
         'VoltageOutputIIBMod4-Mon': _c.V_V_OUTPUT_IIB_4,
         'IGBT1CurrentIIBMod4-Mon': _c.V_I_IGBT_1_IIB_4,
@@ -631,15 +629,14 @@
         'IGBT1TemperatureIIBMod4-Mon': _c.V_TEMP_IGBT_1_IIB_4,
         'IGBT2TemperatureIIBMod4-Mon': _c.V_TEMP_IGBT_2_IIB_4,
         'IGBTDriverVoltageIIBMod4-Mon': _c.V_V_DRIVER_IIB_4,
         'IGBT1DriverCurrentIIBMod4-Mon': _c.V_I_DRIVER_1_IIB_4,
         'IGBT2DriverCurrentIIBMod4-Mon': _c.V_I_DRIVER_2_IIB_4,
         'InductorTemperatureIIBMod4-Mon': _c.V_TEMP_INDUCTOR_IIB_4,
         'HeatSinkTemperatureIIBMod4-Mon': _c.V_TEMP_HEATSINK_IIB_4,
-        'LeakageCurrentIIBMod4-Mon': _c.V_I_LEAKAGE_IIB_4,
         'TemperatureIIBMod4-Mon': _c.V_TEMP_BOARD_IIB_4,
         'RelativeHumidityIIBMod4-Mon': _c.V_RH_IIB_4,
         'IntlkIIBMod4-Mon': _c.V_IIB_INTERLOCKS_4,
         'AlarmsIIBMod4-Mon': _c.V_IIB_ALARMS_4,
         'Alarms-Mon': _c.V_PS_ALARMS,
         }
 
@@ -684,26 +681,26 @@
         'IGBT2PWMDutyCycleMod1-Mon': _c.V_DUTY_CYCLE_2_1,
         'IGBT1PWMDutyCycleMod2-Mon': _c.V_DUTY_CYCLE_1_2,
         'IGBT2PWMDutyCycleMod2-Mon': _c.V_DUTY_CYCLE_2_2,
         'IGBT1PWMDutyCycleMod3-Mon': _c.V_DUTY_CYCLE_1_3,
         'IGBT2PWMDutyCycleMod3-Mon': _c.V_DUTY_CYCLE_2_3,
         'IGBT1PWMDutyCycleMod4-Mon': _c.V_DUTY_CYCLE_1_4,
         'IGBT2PWMDutyCycleMod4-Mon': _c.V_DUTY_CYCLE_2_4,
+        'LeakCurrent-Mon': _c.V_I_LEAKAGE,
         'VoltageInputIIBMod1-Mon': _c.V_V_INPUT_IIB_1,
         'VoltageOutputIIBMod1-Mon': _c.V_V_OUTPUT_IIB_1,
         'IGBT1CurrentIIBMod1-Mon': _c.V_I_IGBT_1_IIB_1,
         'IGBT2CurrentIIBMod1-Mon': _c.V_I_IGBT_2_IIB_1,
         'IGBT1TemperatureIIBMod1-Mon': _c.V_TEMP_IGBT_1_IIB_1,
         'IGBT2TemperatureIIBMod1-Mon': _c.V_TEMP_IGBT_2_IIB_1,
         'IGBTDriverVoltageIIBMod1-Mon': _c.V_V_DRIVER_IIB_1,
         'IGBT1DriverCurrentIIBMod1-Mon': _c.V_I_DRIVER_1_IIB_1,
         'IGBT2DriverCurrentIIBMod1-Mon': _c.V_I_DRIVER_2_IIB_1,
         'InductorTemperatureIIBMod1-Mon': _c.V_TEMP_INDUCTOR_IIB_1,
         'HeatSinkTemperatureIIBMod1-Mon': _c.V_TEMP_HEATSINK_IIB_1,
-        'LeakageCurrentIIBMod1-Mon': _c.V_I_LEAKAGE_IIB_1,
         'TemperatureIIBMod1-Mon': _c.V_TEMP_BOARD_IIB_1,
         'RelativeHumidityIIBMod1-Mon': _c.V_RH_IIB_1,
         'IntlkIIBMod1-Mon': _c.V_IIB_INTERLOCKS_1,
         'AlarmsIIBMod1-Mon': _c.V_IIB_ALARMS_1,
         'VoltageInputIIBMod2-Mon': _c.V_V_INPUT_IIB_2,
         'VoltageOutputIIBMod2-Mon': _c.V_V_OUTPUT_IIB_2,
         'IGBT1CurrentIIBMod2-Mon': _c.V_I_IGBT_1_IIB_2,
@@ -726,15 +723,14 @@
         'IGBT1TemperatureIIBMod3-Mon': _c.V_TEMP_IGBT_1_IIB_3,
         'IGBT2TemperatureIIBMod3-Mon': _c.V_TEMP_IGBT_2_IIB_3,
         'IGBTDriverVoltageIIBMod3-Mon': _c.V_V_DRIVER_IIB_3,
         'IGBT1DriverCurrentIIBMod3-Mon': _c.V_I_DRIVER_1_IIB_3,
         'IGBT2DriverCurrentIIBMod3-Mon': _c.V_I_DRIVER_2_IIB_3,
         'InductorTemperatureIIBMod3-Mon': _c.V_TEMP_INDUCTOR_IIB_3,
         'HeatSinkTemperatureIIBMod3-Mon': _c.V_TEMP_HEATSINK_IIB_3,
-        'LeakageCurrentIIBMod3-Mon': _c.V_I_LEAKAGE_IIB_3,
         'TemperatureIIBMod3-Mon': _c.V_TEMP_BOARD_IIB_3,
         'RelativeHumidityIIBMod3-Mon': _c.V_RH_IIB_3,
         'IntlkIIBMod3-Mon': _c.V_IIB_INTERLOCKS_3,
         'AlarmsIIBMod3-Mon': _c.V_IIB_ALARMS_3,
         'VoltageInputIIBMod4-Mon': _c.V_V_INPUT_IIB_4,
         'VoltageOutputIIBMod4-Mon': _c.V_V_OUTPUT_IIB_4,
         'IGBT1CurrentIIBMod4-Mon': _c.V_I_IGBT_1_IIB_4,
@@ -742,15 +738,14 @@
         'IGBT1TemperatureIIBMod4-Mon': _c.V_TEMP_IGBT_1_IIB_4,
         'IGBT2TemperatureIIBMod4-Mon': _c.V_TEMP_IGBT_2_IIB_4,
         'IGBTDriverVoltageIIBMod4-Mon': _c.V_V_DRIVER_IIB_4,
         'IGBT1DriverCurrentIIBMod4-Mon': _c.V_I_DRIVER_1_IIB_4,
         'IGBT2DriverCurrentIIBMod4-Mon': _c.V_I_DRIVER_2_IIB_4,
         'InductorTemperatureIIBMod4-Mon': _c.V_TEMP_INDUCTOR_IIB_4,
         'HeatSinkTemperatureIIBMod4-Mon': _c.V_TEMP_HEATSINK_IIB_4,
-        'LeakageCurrentIIBMod4-Mon': _c.V_I_LEAKAGE_IIB_4,
         'TemperatureIIBMod4-Mon': _c.V_TEMP_BOARD_IIB_4,
         'RelativeHumidityIIBMod4-Mon': _c.V_RH_IIB_4,
         'IntlkIIBMod4-Mon': _c.V_IIB_INTERLOCKS_4,
         'AlarmsIIBMod4-Mon': _c.V_IIB_ALARMS_4,
         'Alarms-Mon': _c.V_PS_ALARMS,
         }
```

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/pssofb.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/pwrsupply/siggen.py` & `siriuspy-2.73.0/siriuspy/pwrsupply/siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/ramp/conn.py` & `siriuspy-2.73.0/siriuspy/ramp/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/ramp/magnet.py` & `siriuspy-2.73.0/siriuspy/ramp/magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/ramp/ramp.py` & `siriuspy-2.73.0/siriuspy/ramp/ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/ramp/reconst_factory.py` & `siriuspy-2.73.0/siriuspy/ramp/reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/ramp/test_reconst_factory.py` & `siriuspy-2.73.0/siriuspy/ramp/test_reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/ramp/testwfm.py` & `siriuspy-2.73.0/siriuspy/ramp/testwfm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/ramp/util.py` & `siriuspy-2.73.0/siriuspy/ramp/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/ramp/waveform.py` & `siriuspy-2.73.0/siriuspy/ramp/waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/search/bpms_search.py` & `siriuspy-2.73.0/siriuspy/search/bpms_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/search/hl_time_search.py` & `siriuspy-2.73.0/siriuspy/search/hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/search/id_search.py` & `siriuspy-2.73.0/siriuspy/search/id_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/search/ioc_search.py` & `siriuspy-2.73.0/siriuspy/search/ioc_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/search/ll_time_search.py` & `siriuspy-2.73.0/siriuspy/search/ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/search/ma_search.py` & `siriuspy-2.73.0/siriuspy/search/ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/search/ps_search.py` & `siriuspy-2.73.0/siriuspy/search/ps_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,14 +321,23 @@
     def conv_dclink_2_psname(dclink, filter_auxps=True):
         """Return PS associated with a DCLink."""
         # NOTE: lock is being used within private method.
         dict_aux = PSSearch.get_dclink_2_psname_dict(filter_auxps)
         return dict_aux[dclink]
 
     @staticmethod
+    def conv_psname_2_udcindex(psname):
+        """Return power supply index in associated UDC."""
+        with PSSearch._lock:
+            PSSearch._reload_udc_2_bsmp_dict()
+        udc = PSSearch._bsmp_2_udc_dict[psname]
+        udcmap = PSSearch._udc_2_bsmp_dict[udc]
+        return [ps[0] for ps in udcmap].index(psname)
+
+    @staticmethod
     def get_linac_ps_sinap2sirius_dict():
         """Return PS name convertion dict."""
         return PSSearch._linac_ps_sinap2sirius
 
     @staticmethod
     def get_linac_ps_sirius2sinap_dict():
         """Return PS name convertion dict."""
```

### Comparing `siriuspy-2.72.0/siriuspy/simul/simfactory.py` & `siriuspy-2.73.0/siriuspy/simul/simfactory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/simul/simps.py` & `siriuspy-2.73.0/siriuspy/simul/simps.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/simul/simpv.py` & `siriuspy-2.73.0/siriuspy/simul/simpv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/simul/simulation.py` & `siriuspy-2.73.0/siriuspy/simul/simulation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/simul/simulator.py` & `siriuspy-2.73.0/siriuspy/simul/simulator.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/sofb/base_class.py` & `siriuspy-2.73.0/siriuspy/sofb/base_class.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/sofb/bpms.py` & `siriuspy-2.73.0/siriuspy/sofb/bpms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/sofb/correctors.py` & `siriuspy-2.73.0/siriuspy/sofb/correctors.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/sofb/csdev.py` & `siriuspy-2.73.0/siriuspy/sofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/sofb/main.py` & `siriuspy-2.73.0/siriuspy/sofb/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/sofb/matrix.py` & `siriuspy-2.73.0/siriuspy/sofb/matrix.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/sofb/orbit.py` & `siriuspy-2.73.0/siriuspy/sofb/orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/sofb/utils.py` & `siriuspy-2.73.0/siriuspy/sofb/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/stabinfo/csdev.py` & `siriuspy-2.73.0/siriuspy/stabinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/stabinfo/main.py` & `siriuspy-2.73.0/siriuspy/stabinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/thread.py` & `siriuspy-2.73.0/siriuspy/thread.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/timesys/csdev.py` & `siriuspy-2.73.0/siriuspy/timesys/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/timesys/hl_classes.py` & `siriuspy-2.73.0/siriuspy/timesys/hl_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/timesys/ll_classes.py` & `siriuspy-2.73.0/siriuspy/timesys/ll_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/timesys/plot_network.py` & `siriuspy-2.73.0/siriuspy/timesys/plot_network.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/timesys/static_table.py` & `siriuspy-2.73.0/siriuspy/timesys/static_table.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy/util.py` & `siriuspy-2.73.0/siriuspy/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/siriuspy.egg-info/PKG-INFO` & `siriuspy-2.73.0/siriuspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.72.0
+Version: 2.73.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.72.0/siriuspy.egg-info/SOURCES.txt` & `siriuspy-2.73.0/siriuspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/bsmp/test_bsmp.py` & `siriuspy-2.73.0/tests/bsmp/test_bsmp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/bsmp/test_commands.py` & `siriuspy-2.73.0/tests/bsmp/test_commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/bsmp/test_entities.py` & `siriuspy-2.73.0/tests/bsmp/test_entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/bsmp/test_serial.py` & `siriuspy-2.73.0/tests/bsmp/test_serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/bsmp/test_types.py` & `siriuspy-2.73.0/tests/bsmp/test_types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/clientconfigdb/test_configdb_client.py` & `siriuspy-2.73.0/tests/clientconfigdb/test_configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/clientweb/test_implementation.py` & `siriuspy-2.73.0/tests/clientweb/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/currinfo/lifetime/test_main.py` & `siriuspy-2.73.0/tests/currinfo/lifetime/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/currinfo/test_csdev.py` & `siriuspy-2.73.0/tests/currinfo/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/currinfo/test_main.py` & `siriuspy-2.73.0/tests/currinfo/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/magnet/test_factory.py` & `siriuspy-2.73.0/tests/magnet/test_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/magnet/tests_normalizer.py` & `siriuspy-2.73.0/tests/magnet/tests_normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/mock_servweb.py` & `siriuspy-2.73.0/tests/mock_servweb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/namesys/test_implementation.py` & `siriuspy-2.73.0/tests/namesys/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/opticscorr/test_chrom.py` & `siriuspy-2.73.0/tests/opticscorr/test_chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/opticscorr/test_csdev.py` & `siriuspy-2.73.0/tests/opticscorr/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/opticscorr/test_opticscorr.py` & `siriuspy-2.73.0/tests/opticscorr/test_opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/opticscorr/test_tune.py` & `siriuspy-2.73.0/tests/opticscorr/test_tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/opticscorr/test_utils.py` & `siriuspy-2.73.0/tests/opticscorr/test_utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/posang/test_csdev.py` & `siriuspy-2.73.0/tests/posang/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/posang/test_main.py` & `siriuspy-2.73.0/tests/posang/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/pwrsupply/db.py` & `siriuspy-2.73.0/tests/pwrsupply/db.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/pwrsupply/pructrl/test_pru.py` & `siriuspy-2.73.0/tests/pwrsupply/pructrl/test_pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/pwrsupply/psctrl/test_pscwriters.py` & `siriuspy-2.73.0/tests/pwrsupply/psctrl/test_pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/pwrsupply/test_csdev.py` & `siriuspy-2.73.0/tests/pwrsupply/test_csdev.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     'PS_LI_INTLK_THRS',
     'ETypes',
     'Const',
     'get_ps_propty_database',
     'get_conv_propty_database',
     'get_ps_interlocks',
     'get_ps_modules',
+    'get_ps_scopesourcemap',
 )
 
 
 class TestPwrSupplyCSDev(TestCase):
     """Test pwrsupply csdev module."""
 
     ps_alarm = ('Current-SP', 'Current-RB',
```

### Comparing `siriuspy-2.72.0/tests/pwrsupply/test_data.py` & `siriuspy-2.73.0/tests/pwrsupply/test_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/pwrsupply/test_siggen.py` & `siriuspy-2.73.0/tests/pwrsupply/test_siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/pwrsupply/variables.py` & `siriuspy-2.73.0/tests/pwrsupply/variables.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/ramp/test_magnet.py` & `siriuspy-2.73.0/tests/ramp/test_magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/ramp/test_waveform.py` & `siriuspy-2.73.0/tests/ramp/test_waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/search/test_hl_time_search.py` & `siriuspy-2.73.0/tests/search/test_hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/search/test_init.py` & `siriuspy-2.73.0/tests/search/test_init.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/search/test_ll_time_search.py` & `siriuspy-2.73.0/tests/search/test_ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/search/test_ma_search.py` & `siriuspy-2.73.0/tests/search/test_ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/search/test_ps_search.py` & `siriuspy-2.73.0/tests/search/test_ps_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         'conv_bbbname_2_freq',
         'conv_bbbname_2_udc',
         'conv_udc_2_bbbname',
         'conv_udc_2_bsmps',
         'conv_psname_2_udc',
         'conv_psname_2_dclink',
         'conv_dclink_2_psname',
+        'conv_psname_2_udcindex',
         'get_linac_ps_sinap2sirius_dict',
         'get_linac_ps_sirius2sinap_dict',
         'get_pstype_2_psnames_dict',
         'get_pstype_2_splims_dict',
         'get_splims_unit',
         'get_splims_labels',
         'get_psname_2_dclink_dict',
```

### Comparing `siriuspy-2.72.0/tests/test_callbacks.py` & `siriuspy-2.73.0/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/test_csdev.py` & `siriuspy-2.73.0/tests/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/test_envars.py` & `siriuspy-2.73.0/tests/test_envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/test_util.py` & `siriuspy-2.73.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/timesys/test_csdev.py` & `siriuspy-2.73.0/tests/timesys/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.72.0/tests/timesys/test_plot_network.py` & `siriuspy-2.73.0/tests/timesys/test_plot_network.py`

 * *Files identical despite different names*

