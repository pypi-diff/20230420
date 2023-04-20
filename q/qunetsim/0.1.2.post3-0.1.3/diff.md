# Comparing `tmp/qunetsim-0.1.2.post3.tar.gz` & `tmp/qunetsim-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qunetsim-0.1.2.post3.tar", last modified: Sat May 22 18:01:37 2021, max compression
+gzip compressed data, was "qunetsim-0.1.3.tar", last modified: Thu Apr 20 09:45:36 2023, max compression
```

## Comparing `qunetsim-0.1.2.post3.tar` & `qunetsim-0.1.3.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 stephendiadamo   (501) staff       (20)        0 2021-05-22 18:01:37.000000 qunetsim-0.1.2.post3/
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     3201 2021-05-22 18:01:37.000000 qunetsim-0.1.2.post3/PKG-INFO
-drwxr-xr-x   0 stephendiadamo   (501) staff       (20)        0 2021-05-22 18:01:37.000000 qunetsim-0.1.2.post3/bin/
--rwxr-xr-x   0 stephendiadamo   (501) staff       (20)    13156 2021-05-22 17:43:28.000000 qunetsim-0.1.2.post3/bin/template
-drwxr-xr-x   0 stephendiadamo   (501) staff       (20)        0 2021-05-22 18:01:37.000000 qunetsim-0.1.2.post3/qunetsim/
-drwxr-xr-x   0 stephendiadamo   (501) staff       (20)        0 2021-05-22 18:01:37.000000 qunetsim-0.1.2.post3/qunetsim/backends/
--rw-r--r--   0 stephendiadamo   (501) staff       (20)    13636 2021-03-17 13:48:20.000000 qunetsim-0.1.2.post3/qunetsim/backends/cqc_backend.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)    10088 2021-03-17 13:48:20.000000 qunetsim-0.1.2.post3/qunetsim/backends/backend.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)    16620 2021-05-05 12:19:08.000000 qunetsim-0.1.2.post3/qunetsim/backends/qutip_backend.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     1426 2021-03-17 13:48:20.000000 qunetsim-0.1.2.post3/qunetsim/backends/rw_lock.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)      464 2021-05-05 12:19:08.000000 qunetsim-0.1.2.post3/qunetsim/backends/__init__.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)    11744 2021-03-17 13:48:20.000000 qunetsim-0.1.2.post3/qunetsim/backends/projectq_backend.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)    13933 2021-05-05 12:19:08.000000 qunetsim-0.1.2.post3/qunetsim/backends/eqsn_backend.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)      625 2021-02-20 09:36:44.000000 qunetsim-0.1.2.post3/qunetsim/backends/safe_dict.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)       61 2021-03-17 13:48:20.000000 qunetsim-0.1.2.post3/qunetsim/__init__.py
-drwxr-xr-x   0 stephendiadamo   (501) staff       (20)        0 2021-05-22 18:01:37.000000 qunetsim-0.1.2.post3/qunetsim/objects/
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     8976 2021-03-17 13:48:20.000000 qunetsim-0.1.2.post3/qunetsim/objects/qubit.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)      368 2020-06-23 16:47:30.000000 qunetsim-0.1.2.post3/qunetsim/objects/daemon_thread.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)      282 2021-03-17 13:48:20.000000 qunetsim-0.1.2.post3/qunetsim/objects/__init__.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     1981 2021-02-20 09:36:44.000000 qunetsim-0.1.2.post3/qunetsim/objects/message.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)      970 2020-11-12 09:34:30.000000 qunetsim-0.1.2.post3/qunetsim/objects/logger.py
-drwxr-xr-x   0 stephendiadamo   (501) staff       (20)        0 2021-05-22 18:01:37.000000 qunetsim-0.1.2.post3/qunetsim/objects/storage/
--rw-r--r--   0 stephendiadamo   (501) staff       (20)    20478 2021-04-15 11:24:18.000000 qunetsim-0.1.2.post3/qunetsim/objects/storage/quantum_storage.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)       92 2020-11-12 09:34:30.000000 qunetsim-0.1.2.post3/qunetsim/objects/storage/__init__.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     9359 2021-03-17 13:48:20.000000 qunetsim-0.1.2.post3/qunetsim/objects/storage/classical_storage.py
-drwxr-xr-x   0 stephendiadamo   (501) staff       (20)        0 2021-05-22 18:01:37.000000 qunetsim-0.1.2.post3/qunetsim/objects/connections/
--rw-r--r--   0 stephendiadamo   (501) staff       (20)      138 2020-11-12 09:34:30.000000 qunetsim-0.1.2.post3/qunetsim/objects/connections/__init__.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)      462 2021-03-17 13:48:20.000000 qunetsim-0.1.2.post3/qunetsim/objects/connections/quantum_connection.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     1034 2021-03-18 13:32:42.000000 qunetsim-0.1.2.post3/qunetsim/objects/connections/connection.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)      494 2020-11-12 09:34:30.000000 qunetsim-0.1.2.post3/qunetsim/objects/connections/classical_connection.py
-drwxr-xr-x   0 stephendiadamo   (501) staff       (20)        0 2021-05-22 18:01:37.000000 qunetsim-0.1.2.post3/qunetsim/objects/connections/channel_models/
--rw-r--r--   0 stephendiadamo   (501) staff       (20)       67 2020-11-12 09:34:30.000000 qunetsim-0.1.2.post3/qunetsim/objects/connections/channel_models/__init__.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     1665 2021-03-17 13:48:20.000000 qunetsim-0.1.2.post3/qunetsim/objects/connections/channel_models/classical_model.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     2828 2021-03-17 13:48:20.000000 qunetsim-0.1.2.post3/qunetsim/objects/connections/channel_models/fibre.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     1818 2021-03-17 13:48:20.000000 qunetsim-0.1.2.post3/qunetsim/objects/connections/channel_models/binary_erasure.py
-drwxr-xr-x   0 stephendiadamo   (501) staff       (20)        0 2021-05-22 18:01:37.000000 qunetsim-0.1.2.post3/qunetsim/objects/packets/
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     3647 2020-11-12 09:34:30.000000 qunetsim-0.1.2.post3/qunetsim/objects/packets/routing_packet.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)       69 2020-11-12 09:34:30.000000 qunetsim-0.1.2.post3/qunetsim/objects/packets/__init__.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     3857 2021-02-20 09:36:44.000000 qunetsim-0.1.2.post3/qunetsim/objects/packets/packet.py
-drwxr-xr-x   0 stephendiadamo   (501) staff       (20)        0 2021-05-22 18:01:37.000000 qunetsim-0.1.2.post3/qunetsim/utils/
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     1184 2021-02-20 09:36:44.000000 qunetsim-0.1.2.post3/qunetsim/utils/constants.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)        0 2020-06-23 16:47:30.000000 qunetsim-0.1.2.post3/qunetsim/utils/__init__.py
-drwxr-xr-x   0 stephendiadamo   (501) staff       (20)        0 2021-05-22 18:01:37.000000 qunetsim-0.1.2.post3/qunetsim/components/
--rw-r--r--   0 stephendiadamo   (501) staff       (20)    20384 2021-02-20 09:36:44.000000 qunetsim-0.1.2.post3/qunetsim/components/protocols.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)    59246 2021-04-15 11:24:22.000000 qunetsim-0.1.2.post3/qunetsim/components/host.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)       52 2020-06-23 16:47:30.000000 qunetsim-0.1.2.post3/qunetsim/components/__init__.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)    27379 2021-05-22 17:37:40.000000 qunetsim-0.1.2.post3/qunetsim/components/network.py
-drwxr-xr-x   0 stephendiadamo   (501) staff       (20)        0 2021-05-22 18:01:37.000000 qunetsim-0.1.2.post3/qunetsim.egg-info/
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     3201 2021-05-22 18:01:36.000000 qunetsim-0.1.2.post3/qunetsim.egg-info/PKG-INFO
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     1457 2021-05-22 18:01:36.000000 qunetsim-0.1.2.post3/qunetsim.egg-info/SOURCES.txt
--rw-r--r--   0 stephendiadamo   (501) staff       (20)       50 2021-05-22 18:01:36.000000 qunetsim-0.1.2.post3/qunetsim.egg-info/requires.txt
--rw-r--r--   0 stephendiadamo   (501) staff       (20)        9 2021-05-22 18:01:36.000000 qunetsim-0.1.2.post3/qunetsim.egg-info/top_level.txt
--rw-r--r--   0 stephendiadamo   (501) staff       (20)        1 2021-05-22 18:01:36.000000 qunetsim-0.1.2.post3/qunetsim.egg-info/dependency_links.txt
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     1879 2020-11-12 09:34:30.000000 qunetsim-0.1.2.post3/README.md
--rw-r--r--   0 stephendiadamo   (501) staff       (20)     1243 2021-05-22 18:01:25.000000 qunetsim-0.1.2.post3/setup.py
--rw-r--r--   0 stephendiadamo   (501) staff       (20)       38 2021-05-22 18:01:37.000000 qunetsim-0.1.2.post3/setup.cfg
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.282859 qunetsim-0.1.3/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1071 2023-04-20 09:41:28.000000 qunetsim-0.1.3/LICENSE
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     2741 2023-04-20 09:45:36.282194 qunetsim-0.1.3/PKG-INFO
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1922 2023-04-20 09:41:31.000000 qunetsim-0.1.3/README.md
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.237203 qunetsim-0.1.3/bin/
+-rwxr-xr-x   0 sdiadamo   (501) staff       (20)    13156 2023-04-20 09:41:28.000000 qunetsim-0.1.3/bin/template
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.238458 qunetsim-0.1.3/qunetsim/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)       61 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/__init__.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.253033 qunetsim-0.1.3/qunetsim/backends/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      464 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/backends/__init__.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    10088 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/backends/backend.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    13636 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/backends/cqc_backend.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    14348 2023-04-20 09:41:31.000000 qunetsim-0.1.3/qunetsim/backends/eqsn_backend.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    11744 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/backends/projectq_backend.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    17581 2023-04-20 09:41:31.000000 qunetsim-0.1.3/qunetsim/backends/qutip_backend.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1426 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/backends/rw_lock.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      625 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/backends/safe_dict.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.259506 qunetsim-0.1.3/qunetsim/components/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)       52 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/components/__init__.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    62513 2023-04-20 09:41:31.000000 qunetsim-0.1.3/qunetsim/components/host.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    27379 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/components/network.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    20364 2023-04-20 09:41:31.000000 qunetsim-0.1.3/qunetsim/components/protocols.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.264277 qunetsim-0.1.3/qunetsim/objects/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      282 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/__init__.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.268250 qunetsim-0.1.3/qunetsim/objects/connections/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      138 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/__init__.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.272413 qunetsim-0.1.3/qunetsim/objects/connections/channel_models/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)       67 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/channel_models/__init__.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1818 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/channel_models/binary_erasure.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1665 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/channel_models/classical_model.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     2828 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/channel_models/fibre.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      494 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/classical_connection.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1034 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/connection.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      462 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/quantum_connection.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      368 2023-04-20 09:40:44.000000 qunetsim-0.1.3/qunetsim/objects/daemon_thread.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      970 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/logger.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1981 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/message.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.275261 qunetsim-0.1.3/qunetsim/objects/packets/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)       69 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/packets/__init__.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     3857 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/packets/packet.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     3647 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/packets/routing_packet.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     8976 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/qubit.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.278351 qunetsim-0.1.3/qunetsim/objects/storage/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)       92 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/storage/__init__.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     9359 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/storage/classical_storage.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    20478 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/storage/quantum_storage.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.280686 qunetsim-0.1.3/qunetsim/utils/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)        0 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/utils/__init__.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1184 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/utils/constants.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.242959 qunetsim-0.1.3/qunetsim.egg-info/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     2741 2023-04-20 09:45:36.000000 qunetsim-0.1.3/qunetsim.egg-info/PKG-INFO
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1465 2023-04-20 09:45:36.000000 qunetsim-0.1.3/qunetsim.egg-info/SOURCES.txt
+-rw-r--r--   0 sdiadamo   (501) staff       (20)        1 2023-04-20 09:45:36.000000 qunetsim-0.1.3/qunetsim.egg-info/dependency_links.txt
+-rw-r--r--   0 sdiadamo   (501) staff       (20)       50 2023-04-20 09:45:36.000000 qunetsim-0.1.3/qunetsim.egg-info/requires.txt
+-rw-r--r--   0 sdiadamo   (501) staff       (20)        9 2023-04-20 09:45:36.000000 qunetsim-0.1.3/qunetsim.egg-info/top_level.txt
+-rw-r--r--   0 sdiadamo   (501) staff       (20)       38 2023-04-20 09:45:36.283094 qunetsim-0.1.3/setup.cfg
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1238 2023-04-20 09:42:26.000000 qunetsim-0.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qunetsim-0.1.2.post3/PKG-INFO` & `qunetsim-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 Metadata-Version: 2.1
 Name: qunetsim
-Version: 0.1.2.post3
+Version: 0.1.3
 Summary: A Quantum Network Simulation Framework
 Home-page: https://github.com/tqsd/QuNetSim
+Download-URL: https://github.com/tqsd/QuNetSim/releases/tag/0.1.2
 Author: Stephen DiAdamo, Janis Nötzel, Benjamin Zanger, Mert Mehmet Bese
 Author-email: stephen.diadamo@gmail.com
 License: MIT
-Download-URL: https://github.com/tqsd/QuNetSim/releases/tag/0.1.2
-Description: [![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=for-the-badge)](http://unitary.fund)
-        # QuNetSim 
-        
-        ![QuNetSim Tests](https://github.com/tqsd/QuNetSim/workflows/QuNetSim%20Tests/badge.svg)
-        
-        QuNetSim is a quantum-enabled network simulator that adds common quantum networking tasks like teleportation, superdense coding, sharing EPR pairs, etc. With QuNetSim, one can design and test robust quantum network protocols under various network conditions.
-        
-        ## Installation and Documentation
-        
-        See https://tqsd.github.io/QuNetSim/ for documentation. To install the latest release via pip:
-        ```
-        pip install qunetsim
-        ```
-        
-        ## Quick Start Guide
-        
-        ### Templater
-        
-        The QuNetSim pip package comes with a templater. After installing the library, simply type `template` and follow the instructions. A template QuNetSim example will be generated. 
-        
-        ### Quick Example
-        
-        ```
-        from qunetsim.components import Host, Network
-        
-        network = Network.get_instance()
-        network.start()
-        
-        alice = Host('Alice')
-        bob = Host('Bob')
-        
-        alice.add_connection(bob.host_id)
-        bob.add_connection(alice.host_id)
-        
-        alice.start()
-        bob.start()
-        
-        network.add_hosts([alice, bob])
-        
-        # Block Alice to wait for qubit arrive from Bob
-        alice.send_epr(bob.host_id, await_ack=True)
-        q_alice = alice.get_epr(bob.host_id)
-        q_bob = bob.get_epr(alice.host_id)
-        
-        print("EPR is in state: %d, %d" % (q_alice.measure(), q_bob.measure()))
-        network.stop(True)
-        ```
-        
-        ## Contributing 
-        
-        Feel free to contribute by adding Github issues and pull requests. Adding test cases for any contributions is a requirement for any pull request to be merged. 
-        
-        ## Citation
-        ```
-        @article{diadamo2020qunetsim,
-          title={QuNetSim: A Software Framework for Quantum Networks},
-          author={DiAdamo, Stephen and N{\"o}tzel, Janis and Zanger, Benjamin and Be{\c{s}}e, Mehmet Mert},
-          journal={arXiv preprint arXiv:2003.06397},
-          year={2020}
-        }
-        ```
-        
 Keywords: quantum,networks,simulator,internet,QuNetSim
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=for-the-badge)](http://unitary.fund)
+# QuNetSim 
+
+![QuNetSim Tests](https://github.com/tqsd/QuNetSim/workflows/QuNetSim%20Tests/badge.svg)
+
+QuNetSim is a quantum-enabled network simulator that adds common quantum networking tasks like teleportation, superdense coding, sharing EPR pairs, etc. With QuNetSim, one can design and test robust quantum network protocols under various network conditions.
+
+## Installation and Documentation
+
+See https://tqsd.github.io/QuNetSim/ for documentation. To install the latest release via pip:
+```
+pip install qunetsim
+```
+
+## Quick Start Guide
+
+### Templater
+
+The QuNetSim pip package comes with a templater. After installing the library, simply type `template` and follow the instructions. A template QuNetSim example will be generated. 
+
+### Quick Example
+
+```
+from qunetsim.components import Host, Network
+
+network = Network.get_instance()
+network.start()
+
+alice = Host('Alice')
+bob = Host('Bob')
+
+alice.add_connection(bob.host_id)
+bob.add_connection(alice.host_id)
+
+alice.start()
+bob.start()
+
+network.add_hosts([alice, bob])
+
+# Block Alice to wait for qubit arrive from Bob
+alice.send_epr(bob.host_id, await_ack=True)
+q_alice = alice.get_epr(bob.host_id)
+q_bob = bob.get_epr(alice.host_id)
+
+print("EPR is in state: %d, %d" % (q_alice.measure(), q_bob.measure()))
+network.stop(True)
+```
+
+## Contributing 
+
+Feel free to contribute by adding Github issues and pull requests. Adding test cases for any contributions is a requirement for any pull request to be merged. 
+
+## Citation
+```
+@article{diadamo2020qunetsim,
+  title={QuNetSim: A Software Framework for Quantum Networks},
+  author={DiAdamo, Stephen and N{\"o}tzel, Janis and Zanger, Benjamin and Be{\c{s}}e, Mehmet Mert},
+  journal={IEEE Transactions on Quantum Engineering},
+  year={2021},
+  doi={10.1109/TQE.2021.3092395}
+}
+```
```

### Comparing `qunetsim-0.1.2.post3/bin/template` & `qunetsim-0.1.3/bin/template`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/backends/cqc_backend.py` & `qunetsim-0.1.3/qunetsim/backends/cqc_backend.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/backends/backend.py` & `qunetsim-0.1.3/qunetsim/backends/backend.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/backends/qutip_backend.py` & `qunetsim-0.1.3/qunetsim/backends/qutip_backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from qunetsim.backends.safe_dict import SafeDict
-from qunetsim.backends.rw_lock import RWLock
+from .safe_dict import SafeDict
+from .rw_lock import RWLock
 from qunetsim.objects.qubit import Qubit
 from queue import Queue
 import numpy as np
 import uuid
 
 try:
     import qutip
@@ -26,19 +26,23 @@
         def __init__(self, name):
             # initialize as a qubit in state |0>
             self._rwlock = RWLock()
             self.N = 1
             self._qubit_names = [name]
             self.data = qutip.qutip.fock_dm(2, 0)
 
+        @property
+        def qubit_names(self):
+            return self._qubit_names
+
         def add_qubit(self, qubit):
             """
             Calculates the tensor product using the implementation
             of QuTip.
-            Modified vesion of qutip tensor function,
+            Modified version of qutip tensor function,
             See http://qutip.org/docs/4.0.2/modules/qutip/tensor.html
             """
             self._lock()
             self.data = qutip.tensor(self.data, qubit.data)
             self.N = self.N + qubit.N
             self._qubit_names = self._qubit_names + qubit._qubit_names
             self._unlock()
@@ -92,19 +96,26 @@
                     self.data = qutip.Qobj()
             self._unlock()
             return res
 
         def give_density_matrix(self, qubit_name):
             ret = None
             self._lock()
-            if qubit_name in self._qubit_names:
-                index = self._qubit_names.index(qubit_name)
-                ret = self.data.ptrace([index])
+            if isinstance(qubit_name, list):
+                indices = []
+                for q_name in qubit_name:
+                    if q_name in self._qubit_names:
+                        indices.append(self._qubit_names.index(q_name))
+                ret = self.data.ptrace(indices)
+            else:
+                if qubit_name in self._qubit_names:
+                    index = self._qubit_names.index(qubit_name)
+                    ret = self.data.ptrace([index])
             self._unlock()
-            return ret
+            return self.data #ret
 
         def _lock(self):
             self._rwlock.acquire_write()
 
         def _unlock(self):
             self._rwlock.release_write()
 
@@ -443,21 +454,32 @@
 
     def density_operator(self, qubit):
         """
         Returns the density operator of this qubit. If the qubit is entangled,
         the density operator will be in a mixed state.
 
         Args:
-            qubit (Qubit): Qubit of the density operator.
+            qubit (Qubit or list): Qubit of the density operator.
 
         Returns:
             np.ndarray: The density operator of the qubit.
         """
-        qubit_collection, q_name = qubit.qubit
-        return qubit_collection.give_density_matrix(q_name)
+        if isinstance(qubit, list):
+            names = [q.qubit[1] for q in qubit]
+            qubit_collections = set([q.qubit[0] for q in qubit])
+            density_matrices = []
+            for qubit_collection in qubit_collections:
+                needed_names = [name for name in qubit_collection.qubit_names if name in names]
+                density_matrices.append(qubit_collection.give_density_matrix(needed_names))
+            if len(density_matrices) == 1:
+                return density_matrices[0]
+            return density_matrices
+        else:
+            qubit_collection, q_name = qubit.qubit
+            return qubit_collection.give_density_matrix(q_name)
 
     def measure(self, qubit, non_destructive):
         """
         Perform a measurement on a qubit.
 
         Args:
             qubit (Qubit): Qubit which should be measured.
```

### Comparing `qunetsim-0.1.2.post3/qunetsim/backends/rw_lock.py` & `qunetsim-0.1.3/qunetsim/backends/rw_lock.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/backends/projectq_backend.py` & `qunetsim-0.1.3/qunetsim/backends/projectq_backend.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/backends/eqsn_backend.py` & `qunetsim-0.1.3/qunetsim/backends/eqsn_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -420,14 +420,27 @@
             density_operator = np.trace(density_operator, axis1=0, axis2=2)
         after = 2**(len(qubits) - index - 1)
         if after > 0:
             density_operator = density_operator.reshape([2, after, 2, after])
             density_operator = np.trace(density_operator, axis1=1, axis2=3)
         return density_operator
 
+    def statevector(self, qubit):
+        """
+        Returns the statevector of the passed qubit. If the qubit is entangled to others, 
+        the statevector of the whole entangled system is returned
+
+        Args:
+            qubit (Qubit): Qubit of the statevector.
+
+        Returns:
+            np.ndarray: The statevector of the qubit.
+        """
+        return self.eqsn.give_statevector_for(qubit.qubit)
+
     def measure(self, qubit, non_destructive):
         """
         Perform a measurement on a qubit.
 
         Args:
             qubit (Qubit): Qubit which should be measured.
             non_destructive (bool): If the qubit should be destroyed after measuring.
```

### Comparing `qunetsim-0.1.2.post3/qunetsim/backends/safe_dict.py` & `qunetsim-0.1.3/qunetsim/backends/safe_dict.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/objects/qubit.py` & `qunetsim-0.1.3/qunetsim/objects/qubit.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/objects/message.py` & `qunetsim-0.1.3/qunetsim/objects/message.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/objects/logger.py` & `qunetsim-0.1.3/qunetsim/objects/logger.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/objects/storage/quantum_storage.py` & `qunetsim-0.1.3/qunetsim/objects/storage/quantum_storage.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/objects/storage/classical_storage.py` & `qunetsim-0.1.3/qunetsim/objects/storage/classical_storage.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/objects/connections/connection.py` & `qunetsim-0.1.3/qunetsim/objects/connections/connection.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/objects/connections/channel_models/classical_model.py` & `qunetsim-0.1.3/qunetsim/objects/connections/channel_models/classical_model.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/objects/connections/channel_models/fibre.py` & `qunetsim-0.1.3/qunetsim/objects/connections/channel_models/fibre.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/objects/connections/channel_models/binary_erasure.py` & `qunetsim-0.1.3/qunetsim/objects/connections/channel_models/binary_erasure.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/objects/packets/routing_packet.py` & `qunetsim-0.1.3/qunetsim/objects/packets/routing_packet.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/objects/packets/packet.py` & `qunetsim-0.1.3/qunetsim/objects/packets/packet.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/utils/constants.py` & `qunetsim-0.1.3/qunetsim/utils/constants.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim/components/protocols.py` & `qunetsim-0.1.3/qunetsim/components/protocols.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     Args:
         packet (Packet): The packet in which to receive.
     """
     from_host = packet.sender
     receiver = packet.receiver
     qubit = packet.payload
     receiver = network.get_host(receiver)
-    receiver.add_data_qubit(from_host, qubit)
+    receiver.add_qubit(from_host, qubit)
 
     Logger.get_instance().log(
         packet.receiver + ' received qubit ' + packet.payload.id + ' from ' + packet.sender)
     # Send ACK if seq_num is not -1
 
     if packet.seq_num != -1:
         _send_ack(packet.sender, packet.receiver, packet.seq_num)
@@ -272,15 +272,15 @@
     if b == 1:
         q.X()
 
     if payload['type'] == Constants.EPR:
         host_receiver.add_epr(epr_host, q)
 
     elif payload['type'] == Constants.DATA:
-        host_receiver.add_data_qubit(epr_host, q, q_id=q_id)
+        host_receiver.add_qubit(epr_host, q, q_id=q_id)
 
     # Always send ACK!
     if 'o_seq_num' in payload and 'ack' in payload:
         _send_ack(epr_host, packet.receiver, payload['o_seq_num'])
 
     # Send an ACK if sequence number is not -1
     if packet.seq_num != -1:
@@ -497,17 +497,17 @@
     key_array = []
 
     while received_counter < key_size:
         # decide for a measurement base
         measurement_base = random.randint(0, 1)
 
         # wait for the qubit
-        q_bit = receiver.get_data_qubit(sender.host_id, wait=Constants.WAIT_TIME)
+        q_bit = receiver.get_qubit(sender.host_id, wait=Constants.WAIT_TIME)
         while q_bit is None:
-            q_bit = receiver.get_data_qubit(sender.host_id, wait=Constants.WAIT_TIME)
+            q_bit = receiver.get_qubit(sender.host_id, wait=Constants.WAIT_TIME)
 
         # measure qubit in right measurement basis
         if measurement_base == 1:
             q_bit.H()
         bit = q_bit.measure()
 
         # Send sender the base in which receiver has measured
```

### Comparing `qunetsim-0.1.2.post3/qunetsim/components/host.py` & `qunetsim-0.1.3/qunetsim/components/host.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import math
 import time
 import uuid
+import warnings
 from queue import Queue, Empty
 
 from .network import Network
 from qunetsim.backends import EQSNBackend
 from qunetsim.components import protocols
 from qunetsim.objects import Logger, DaemonThread, Message, Packet, Qubit, QuantumStorage, ClassicalStorage, \
     QuantumConnection, ClassicalConnection
@@ -1211,15 +1212,39 @@
         if host_id is None:
             raise ValueError("Host id has to be specified!")
         return self._qubit_storage.get_all_qubits_from_host(host_id, Qubit.EPR_QUBIT)
 
     def get_data_qubits(self, host_id, remove_from_storage=False):
         """
         Return the dictionary of data qubits stored, just for the information regarding which qubits are stored.
-        Optional to remove the qubits from storage like *get_data_qubit* does with *remove_from_storage* field.
+        Optional to remove the qubits from storage like *get_qubit* does with *remove_from_storage* field.
+
+        Args:
+            host_id (str): The host id from which the data qubit have been received.
+            remove_from_storage (bool): Get and remove from storage.
+
+        Returns:
+            (dict): If *host_id* is not set, then return the entire dictionary of data qubits.
+                  Else If *host_id* is set, then return the data qubits for that particular host if there are any.
+                  Return an empty list otherwise.
+        """
+        warnings.warn(
+            "The 'get_data_qubits' function has been renamed to"
+            " 'get_qubits'. The 'get_data_qubits' function will be removed in QuNetStim 1.0.",
+            DeprecationWarning,
+            stacklevel=3,
+        )
+        return self._qubit_storage.get_all_qubits_from_host(host_id,
+                                                            purpose=Qubit.DATA_QUBIT,
+                                                            remove=remove_from_storage)
+
+    def get_qubits(self, host_id, remove_from_storage=False):
+        """
+        Return the dictionary of data qubits stored, just for the information regarding which qubits are stored.
+        Optional to remove the qubits from storage like *get_qubit* does with *remove_from_storage* field.
 
         Args:
             host_id (str): The host id from which the data qubit have been received.
             remove_from_storage (bool): Get and remove from storage.
 
         Returns:
             (dict): If *host_id* is not set, then return the entire dictionary of data qubits.
@@ -1312,14 +1337,39 @@
         Args:
             host_id (str): The ID of the host to pair the qubit
             qubit (Qubit): The data Qubit to be added.
             q_id (str): the ID to set the qubit ID to
         Returns:
             (str): The qubit ID
         """
+        warnings.warn(
+            "The 'add_data_qubit' function has been renamed to"
+            " 'add_qubit'. The 'add_data_qubit' function will be removed in QuNetStim 1.0.",
+            DeprecationWarning,
+            stacklevel=3,
+        )
+        if q_id is not None:
+            qubit.id = q_id
+
+        self._qubit_storage.add_qubit_from_host(qubit, Qubit.DATA_QUBIT, host_id)
+        return qubit.id
+    
+    def add_qubit(self, host_id, qubit, q_id=None):
+        """
+        Adds the data qubit to the data qubit store of a host. If the qubit has an ID, adds the qubit with it,
+        otherwise generates an ID for the qubit and adds the qubit with that ID.
+
+        Args:
+            host_id (str): The ID of the host to pair the qubit
+            qubit (Qubit): The data Qubit to be added.
+            q_id (str): the ID to set the qubit ID to
+        Returns:
+            (str): The qubit ID
+        """
+        )
         if q_id is not None:
             qubit.id = q_id
 
         self._qubit_storage.add_qubit_from_host(qubit, Qubit.DATA_QUBIT, host_id)
         return qubit.id
 
     def add_ghz_qubit(self, host_id, qubit, q_id=None):
@@ -1439,14 +1489,39 @@
         """
         Gets the data qubit received from another host in the network. If qubit ID is specified,
         qubit with that ID is returned, else, the last qubit received is returned.
 
         Args:
             host_id (str): The ID of the host that data qubit to be returned is received from.
             q_id (str): The qubit ID of the data qubit to get.
+            wait (float): The amount of time to wait for the a qubit to arrive
+        Returns:
+            (Qubit): Qubit received from the host with *host_id* and *q_id*.
+        """
+
+        warnings.warn(
+            "The 'get_data_qubit' function has been renamed to"
+            " 'get_qubit'. The 'get_data_qubit' function will be removed in QuNetStim 1.0.",
+            DeprecationWarning,
+            stacklevel=3,
+        )
+
+        if not isinstance(wait, float) and not isinstance(wait, int):
+            raise Exception('wait parameter should be a number')
+
+        return _get_qubit(self._qubit_storage, host_id, q_id, Qubit.DATA_QUBIT, wait)
+
+    def get_qubit(self, host_id, q_id=None, wait=0):
+        """
+        Gets the data qubit received from another host in the network. If qubit ID is specified,
+        qubit with that ID is returned, else, the last qubit received is returned.
+
+        Args:
+            host_id (str): The ID of the host that data qubit to be returned is received from.
+            q_id (str): The qubit ID of the data qubit to get.
             wait (float): The amount of time to wait for the a qubit to arrive
         Returns:
             (Qubit): Qubit received from the host with *host_id* and *q_id*.
         """
         if not isinstance(wait, float) and not isinstance(wait, int):
             raise Exception('wait parameter should be a number')
```

### Comparing `qunetsim-0.1.2.post3/qunetsim/components/network.py` & `qunetsim-0.1.3/qunetsim/components/network.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.2.post3/qunetsim.egg-info/PKG-INFO` & `qunetsim-0.1.3/qunetsim.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 Metadata-Version: 2.1
 Name: qunetsim
-Version: 0.1.2.post3
+Version: 0.1.3
 Summary: A Quantum Network Simulation Framework
 Home-page: https://github.com/tqsd/QuNetSim
+Download-URL: https://github.com/tqsd/QuNetSim/releases/tag/0.1.2
 Author: Stephen DiAdamo, Janis Nötzel, Benjamin Zanger, Mert Mehmet Bese
 Author-email: stephen.diadamo@gmail.com
 License: MIT
-Download-URL: https://github.com/tqsd/QuNetSim/releases/tag/0.1.2
-Description: [![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=for-the-badge)](http://unitary.fund)
-        # QuNetSim 
-        
-        ![QuNetSim Tests](https://github.com/tqsd/QuNetSim/workflows/QuNetSim%20Tests/badge.svg)
-        
-        QuNetSim is a quantum-enabled network simulator that adds common quantum networking tasks like teleportation, superdense coding, sharing EPR pairs, etc. With QuNetSim, one can design and test robust quantum network protocols under various network conditions.
-        
-        ## Installation and Documentation
-        
-        See https://tqsd.github.io/QuNetSim/ for documentation. To install the latest release via pip:
-        ```
-        pip install qunetsim
-        ```
-        
-        ## Quick Start Guide
-        
-        ### Templater
-        
-        The QuNetSim pip package comes with a templater. After installing the library, simply type `template` and follow the instructions. A template QuNetSim example will be generated. 
-        
-        ### Quick Example
-        
-        ```
-        from qunetsim.components import Host, Network
-        
-        network = Network.get_instance()
-        network.start()
-        
-        alice = Host('Alice')
-        bob = Host('Bob')
-        
-        alice.add_connection(bob.host_id)
-        bob.add_connection(alice.host_id)
-        
-        alice.start()
-        bob.start()
-        
-        network.add_hosts([alice, bob])
-        
-        # Block Alice to wait for qubit arrive from Bob
-        alice.send_epr(bob.host_id, await_ack=True)
-        q_alice = alice.get_epr(bob.host_id)
-        q_bob = bob.get_epr(alice.host_id)
-        
-        print("EPR is in state: %d, %d" % (q_alice.measure(), q_bob.measure()))
-        network.stop(True)
-        ```
-        
-        ## Contributing 
-        
-        Feel free to contribute by adding Github issues and pull requests. Adding test cases for any contributions is a requirement for any pull request to be merged. 
-        
-        ## Citation
-        ```
-        @article{diadamo2020qunetsim,
-          title={QuNetSim: A Software Framework for Quantum Networks},
-          author={DiAdamo, Stephen and N{\"o}tzel, Janis and Zanger, Benjamin and Be{\c{s}}e, Mehmet Mert},
-          journal={arXiv preprint arXiv:2003.06397},
-          year={2020}
-        }
-        ```
-        
 Keywords: quantum,networks,simulator,internet,QuNetSim
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=for-the-badge)](http://unitary.fund)
+# QuNetSim 
+
+![QuNetSim Tests](https://github.com/tqsd/QuNetSim/workflows/QuNetSim%20Tests/badge.svg)
+
+QuNetSim is a quantum-enabled network simulator that adds common quantum networking tasks like teleportation, superdense coding, sharing EPR pairs, etc. With QuNetSim, one can design and test robust quantum network protocols under various network conditions.
+
+## Installation and Documentation
+
+See https://tqsd.github.io/QuNetSim/ for documentation. To install the latest release via pip:
+```
+pip install qunetsim
+```
+
+## Quick Start Guide
+
+### Templater
+
+The QuNetSim pip package comes with a templater. After installing the library, simply type `template` and follow the instructions. A template QuNetSim example will be generated. 
+
+### Quick Example
+
+```
+from qunetsim.components import Host, Network
+
+network = Network.get_instance()
+network.start()
+
+alice = Host('Alice')
+bob = Host('Bob')
+
+alice.add_connection(bob.host_id)
+bob.add_connection(alice.host_id)
+
+alice.start()
+bob.start()
+
+network.add_hosts([alice, bob])
+
+# Block Alice to wait for qubit arrive from Bob
+alice.send_epr(bob.host_id, await_ack=True)
+q_alice = alice.get_epr(bob.host_id)
+q_bob = bob.get_epr(alice.host_id)
+
+print("EPR is in state: %d, %d" % (q_alice.measure(), q_bob.measure()))
+network.stop(True)
+```
+
+## Contributing 
+
+Feel free to contribute by adding Github issues and pull requests. Adding test cases for any contributions is a requirement for any pull request to be merged. 
+
+## Citation
+```
+@article{diadamo2020qunetsim,
+  title={QuNetSim: A Software Framework for Quantum Networks},
+  author={DiAdamo, Stephen and N{\"o}tzel, Janis and Zanger, Benjamin and Be{\c{s}}e, Mehmet Mert},
+  journal={IEEE Transactions on Quantum Engineering},
+  year={2021},
+  doi={10.1109/TQE.2021.3092395}
+}
+```
```

### Comparing `qunetsim-0.1.2.post3/qunetsim.egg-info/SOURCES.txt` & `qunetsim-0.1.3/qunetsim.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 bin/template
 qunetsim/__init__.py
 qunetsim.egg-info/PKG-INFO
 qunetsim.egg-info/SOURCES.txt
 qunetsim.egg-info/dependency_links.txt
```

### Comparing `qunetsim-0.1.2.post3/README.md` & `qunetsim-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -51,11 +51,12 @@
 Feel free to contribute by adding Github issues and pull requests. Adding test cases for any contributions is a requirement for any pull request to be merged. 
 
 ## Citation
 ```
 @article{diadamo2020qunetsim,
   title={QuNetSim: A Software Framework for Quantum Networks},
   author={DiAdamo, Stephen and N{\"o}tzel, Janis and Zanger, Benjamin and Be{\c{s}}e, Mehmet Mert},
-  journal={arXiv preprint arXiv:2003.06397},
-  year={2020}
+  journal={IEEE Transactions on Quantum Engineering},
+  year={2021},
+  doi={10.1109/TQE.2021.3092395}
 }
 ```
```

### Comparing `qunetsim-0.1.2.post3/setup.py` & `qunetsim-0.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='qunetsim',
-    version='0.1.2post3',
+    version='0.1.3',
     scripts=['bin/template'],
     author="Stephen DiAdamo, Janis Nötzel, Benjamin Zanger, Mert Mehmet Bese",
     author_email="stephen.diadamo@gmail.com",
     description="A Quantum Network Simulation Framework",
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

