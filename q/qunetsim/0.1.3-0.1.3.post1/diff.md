# Comparing `tmp/qunetsim-0.1.3.tar.gz` & `tmp/qunetsim-0.1.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qunetsim-0.1.3.tar", last modified: Thu Apr 20 09:45:36 2023, max compression
+gzip compressed data, was "qunetsim-0.1.3.post1.tar", last modified: Thu Apr 20 09:59:35 2023, max compression
```

## Comparing `qunetsim-0.1.3.tar` & `qunetsim-0.1.3.post1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.282859 qunetsim-0.1.3/
--rw-r--r--   0 sdiadamo   (501) staff       (20)     1071 2023-04-20 09:41:28.000000 qunetsim-0.1.3/LICENSE
--rw-r--r--   0 sdiadamo   (501) staff       (20)     2741 2023-04-20 09:45:36.282194 qunetsim-0.1.3/PKG-INFO
--rw-r--r--   0 sdiadamo   (501) staff       (20)     1922 2023-04-20 09:41:31.000000 qunetsim-0.1.3/README.md
-drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.237203 qunetsim-0.1.3/bin/
--rwxr-xr-x   0 sdiadamo   (501) staff       (20)    13156 2023-04-20 09:41:28.000000 qunetsim-0.1.3/bin/template
-drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.238458 qunetsim-0.1.3/qunetsim/
--rw-r--r--   0 sdiadamo   (501) staff       (20)       61 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/__init__.py
-drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.253033 qunetsim-0.1.3/qunetsim/backends/
--rw-r--r--   0 sdiadamo   (501) staff       (20)      464 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/backends/__init__.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)    10088 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/backends/backend.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)    13636 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/backends/cqc_backend.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)    14348 2023-04-20 09:41:31.000000 qunetsim-0.1.3/qunetsim/backends/eqsn_backend.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)    11744 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/backends/projectq_backend.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)    17581 2023-04-20 09:41:31.000000 qunetsim-0.1.3/qunetsim/backends/qutip_backend.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)     1426 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/backends/rw_lock.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)      625 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/backends/safe_dict.py
-drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.259506 qunetsim-0.1.3/qunetsim/components/
--rw-r--r--   0 sdiadamo   (501) staff       (20)       52 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/components/__init__.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)    62513 2023-04-20 09:41:31.000000 qunetsim-0.1.3/qunetsim/components/host.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)    27379 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/components/network.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)    20364 2023-04-20 09:41:31.000000 qunetsim-0.1.3/qunetsim/components/protocols.py
-drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.264277 qunetsim-0.1.3/qunetsim/objects/
--rw-r--r--   0 sdiadamo   (501) staff       (20)      282 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/__init__.py
-drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.268250 qunetsim-0.1.3/qunetsim/objects/connections/
--rw-r--r--   0 sdiadamo   (501) staff       (20)      138 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/__init__.py
-drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.272413 qunetsim-0.1.3/qunetsim/objects/connections/channel_models/
--rw-r--r--   0 sdiadamo   (501) staff       (20)       67 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/channel_models/__init__.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)     1818 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/channel_models/binary_erasure.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)     1665 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/channel_models/classical_model.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)     2828 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/channel_models/fibre.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)      494 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/classical_connection.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)     1034 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/connection.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)      462 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/connections/quantum_connection.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)      368 2023-04-20 09:40:44.000000 qunetsim-0.1.3/qunetsim/objects/daemon_thread.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)      970 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/logger.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)     1981 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/message.py
-drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.275261 qunetsim-0.1.3/qunetsim/objects/packets/
--rw-r--r--   0 sdiadamo   (501) staff       (20)       69 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/packets/__init__.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)     3857 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/packets/packet.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)     3647 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/packets/routing_packet.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)     8976 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/qubit.py
-drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.278351 qunetsim-0.1.3/qunetsim/objects/storage/
--rw-r--r--   0 sdiadamo   (501) staff       (20)       92 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/storage/__init__.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)     9359 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/storage/classical_storage.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)    20478 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/objects/storage/quantum_storage.py
-drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.280686 qunetsim-0.1.3/qunetsim/utils/
--rw-r--r--   0 sdiadamo   (501) staff       (20)        0 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/utils/__init__.py
--rw-r--r--   0 sdiadamo   (501) staff       (20)     1184 2023-01-17 09:52:31.000000 qunetsim-0.1.3/qunetsim/utils/constants.py
-drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:45:36.242959 qunetsim-0.1.3/qunetsim.egg-info/
--rw-r--r--   0 sdiadamo   (501) staff       (20)     2741 2023-04-20 09:45:36.000000 qunetsim-0.1.3/qunetsim.egg-info/PKG-INFO
--rw-r--r--   0 sdiadamo   (501) staff       (20)     1465 2023-04-20 09:45:36.000000 qunetsim-0.1.3/qunetsim.egg-info/SOURCES.txt
--rw-r--r--   0 sdiadamo   (501) staff       (20)        1 2023-04-20 09:45:36.000000 qunetsim-0.1.3/qunetsim.egg-info/dependency_links.txt
--rw-r--r--   0 sdiadamo   (501) staff       (20)       50 2023-04-20 09:45:36.000000 qunetsim-0.1.3/qunetsim.egg-info/requires.txt
--rw-r--r--   0 sdiadamo   (501) staff       (20)        9 2023-04-20 09:45:36.000000 qunetsim-0.1.3/qunetsim.egg-info/top_level.txt
--rw-r--r--   0 sdiadamo   (501) staff       (20)       38 2023-04-20 09:45:36.283094 qunetsim-0.1.3/setup.cfg
--rw-r--r--   0 sdiadamo   (501) staff       (20)     1238 2023-04-20 09:42:26.000000 qunetsim-0.1.3/setup.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:59:35.737702 qunetsim-0.1.3.post1/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1071 2023-04-20 09:58:38.000000 qunetsim-0.1.3.post1/LICENSE
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     2747 2023-04-20 09:59:35.736582 qunetsim-0.1.3.post1/PKG-INFO
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1922 2023-04-20 09:41:31.000000 qunetsim-0.1.3.post1/README.md
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:59:35.678750 qunetsim-0.1.3.post1/bin/
+-rwxr-xr-x   0 sdiadamo   (501) staff       (20)    13156 2023-04-20 09:58:38.000000 qunetsim-0.1.3.post1/bin/template
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:59:35.680196 qunetsim-0.1.3.post1/qunetsim/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)       61 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/__init__.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:59:35.699075 qunetsim-0.1.3.post1/qunetsim/backends/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      464 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/backends/__init__.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    10088 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/backends/backend.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    13636 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/backends/cqc_backend.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    14348 2023-04-20 09:41:31.000000 qunetsim-0.1.3.post1/qunetsim/backends/eqsn_backend.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    11744 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/backends/projectq_backend.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    17581 2023-04-20 09:41:31.000000 qunetsim-0.1.3.post1/qunetsim/backends/qutip_backend.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1426 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/backends/rw_lock.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      625 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/backends/safe_dict.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:59:35.706166 qunetsim-0.1.3.post1/qunetsim/components/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)       52 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/components/__init__.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    62503 2023-04-20 09:58:45.000000 qunetsim-0.1.3.post1/qunetsim/components/host.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    27379 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/components/network.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    20364 2023-04-20 09:41:31.000000 qunetsim-0.1.3.post1/qunetsim/components/protocols.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:59:35.714957 qunetsim-0.1.3.post1/qunetsim/objects/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      282 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/__init__.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:59:35.720468 qunetsim-0.1.3.post1/qunetsim/objects/connections/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      138 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/connections/__init__.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:59:35.725691 qunetsim-0.1.3.post1/qunetsim/objects/connections/channel_models/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)       67 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/connections/channel_models/__init__.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1818 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/connections/channel_models/binary_erasure.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1665 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/connections/channel_models/classical_model.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     2828 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/connections/channel_models/fibre.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      494 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/connections/classical_connection.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1034 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/connections/connection.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      462 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/connections/quantum_connection.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      368 2023-04-20 09:40:44.000000 qunetsim-0.1.3.post1/qunetsim/objects/daemon_thread.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)      970 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/logger.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1981 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/message.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:59:35.729283 qunetsim-0.1.3.post1/qunetsim/objects/packets/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)       69 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/packets/__init__.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     3857 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/packets/packet.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     3647 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/packets/routing_packet.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     8976 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/qubit.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:59:35.732696 qunetsim-0.1.3.post1/qunetsim/objects/storage/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)       92 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/storage/__init__.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     9359 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/storage/classical_storage.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)    20478 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/objects/storage/quantum_storage.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:59:35.735413 qunetsim-0.1.3.post1/qunetsim/utils/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)        0 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/utils/__init__.py
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1184 2023-01-17 09:52:31.000000 qunetsim-0.1.3.post1/qunetsim/utils/constants.py
+drwxr-xr-x   0 sdiadamo   (501) staff       (20)        0 2023-04-20 09:59:35.685936 qunetsim-0.1.3.post1/qunetsim.egg-info/
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     2747 2023-04-20 09:59:35.000000 qunetsim-0.1.3.post1/qunetsim.egg-info/PKG-INFO
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1465 2023-04-20 09:59:35.000000 qunetsim-0.1.3.post1/qunetsim.egg-info/SOURCES.txt
+-rw-r--r--   0 sdiadamo   (501) staff       (20)        1 2023-04-20 09:59:35.000000 qunetsim-0.1.3.post1/qunetsim.egg-info/dependency_links.txt
+-rw-r--r--   0 sdiadamo   (501) staff       (20)       50 2023-04-20 09:59:35.000000 qunetsim-0.1.3.post1/qunetsim.egg-info/requires.txt
+-rw-r--r--   0 sdiadamo   (501) staff       (20)        9 2023-04-20 09:59:35.000000 qunetsim-0.1.3.post1/qunetsim.egg-info/top_level.txt
+-rw-r--r--   0 sdiadamo   (501) staff       (20)       38 2023-04-20 09:59:35.737922 qunetsim-0.1.3.post1/setup.cfg
+-rw-r--r--   0 sdiadamo   (501) staff       (20)     1244 2023-04-20 09:59:15.000000 qunetsim-0.1.3.post1/setup.py
```

### Comparing `qunetsim-0.1.3/LICENSE` & `qunetsim-0.1.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/PKG-INFO` & `qunetsim-0.1.3.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qunetsim
-Version: 0.1.3
+Version: 0.1.3.post1
 Summary: A Quantum Network Simulation Framework
 Home-page: https://github.com/tqsd/QuNetSim
 Download-URL: https://github.com/tqsd/QuNetSim/releases/tag/0.1.2
 Author: Stephen DiAdamo, Janis Nötzel, Benjamin Zanger, Mert Mehmet Bese
 Author-email: stephen.diadamo@gmail.com
 License: MIT
 Keywords: quantum,networks,simulator,internet,QuNetSim
```

### Comparing `qunetsim-0.1.3/README.md` & `qunetsim-0.1.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/bin/template` & `qunetsim-0.1.3.post1/bin/template`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/backends/backend.py` & `qunetsim-0.1.3.post1/qunetsim/backends/backend.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/backends/cqc_backend.py` & `qunetsim-0.1.3.post1/qunetsim/backends/cqc_backend.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/backends/eqsn_backend.py` & `qunetsim-0.1.3.post1/qunetsim/backends/eqsn_backend.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/backends/projectq_backend.py` & `qunetsim-0.1.3.post1/qunetsim/backends/projectq_backend.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/backends/qutip_backend.py` & `qunetsim-0.1.3.post1/qunetsim/backends/qutip_backend.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/backends/rw_lock.py` & `qunetsim-0.1.3.post1/qunetsim/backends/rw_lock.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/backends/safe_dict.py` & `qunetsim-0.1.3.post1/qunetsim/backends/safe_dict.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/components/host.py` & `qunetsim-0.1.3.post1/qunetsim/components/host.py`

 * *Files 0% similar despite different names*

```diff
@@ -1361,15 +1361,14 @@
         Args:
             host_id (str): The ID of the host to pair the qubit
             qubit (Qubit): The data Qubit to be added.
             q_id (str): the ID to set the qubit ID to
         Returns:
             (str): The qubit ID
         """
-        )
         if q_id is not None:
             qubit.id = q_id
 
         self._qubit_storage.add_qubit_from_host(qubit, Qubit.DATA_QUBIT, host_id)
         return qubit.id
 
     def add_ghz_qubit(self, host_id, qubit, q_id=None):
```

### Comparing `qunetsim-0.1.3/qunetsim/components/network.py` & `qunetsim-0.1.3.post1/qunetsim/components/network.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/components/protocols.py` & `qunetsim-0.1.3.post1/qunetsim/components/protocols.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/objects/connections/channel_models/binary_erasure.py` & `qunetsim-0.1.3.post1/qunetsim/objects/connections/channel_models/binary_erasure.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/objects/connections/channel_models/classical_model.py` & `qunetsim-0.1.3.post1/qunetsim/objects/connections/channel_models/classical_model.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/objects/connections/channel_models/fibre.py` & `qunetsim-0.1.3.post1/qunetsim/objects/connections/channel_models/fibre.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/objects/connections/connection.py` & `qunetsim-0.1.3.post1/qunetsim/objects/connections/connection.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/objects/logger.py` & `qunetsim-0.1.3.post1/qunetsim/objects/logger.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/objects/message.py` & `qunetsim-0.1.3.post1/qunetsim/objects/message.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/objects/packets/packet.py` & `qunetsim-0.1.3.post1/qunetsim/objects/packets/packet.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/objects/packets/routing_packet.py` & `qunetsim-0.1.3.post1/qunetsim/objects/packets/routing_packet.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/objects/qubit.py` & `qunetsim-0.1.3.post1/qunetsim/objects/qubit.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/objects/storage/classical_storage.py` & `qunetsim-0.1.3.post1/qunetsim/objects/storage/classical_storage.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/objects/storage/quantum_storage.py` & `qunetsim-0.1.3.post1/qunetsim/objects/storage/quantum_storage.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim/utils/constants.py` & `qunetsim-0.1.3.post1/qunetsim/utils/constants.py`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/qunetsim.egg-info/PKG-INFO` & `qunetsim-0.1.3.post1/qunetsim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qunetsim
-Version: 0.1.3
+Version: 0.1.3.post1
 Summary: A Quantum Network Simulation Framework
 Home-page: https://github.com/tqsd/QuNetSim
 Download-URL: https://github.com/tqsd/QuNetSim/releases/tag/0.1.2
 Author: Stephen DiAdamo, Janis Nötzel, Benjamin Zanger, Mert Mehmet Bese
 Author-email: stephen.diadamo@gmail.com
 License: MIT
 Keywords: quantum,networks,simulator,internet,QuNetSim
```

### Comparing `qunetsim-0.1.3/qunetsim.egg-info/SOURCES.txt` & `qunetsim-0.1.3.post1/qunetsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qunetsim-0.1.3/setup.py` & `qunetsim-0.1.3.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='qunetsim',
-    version='0.1.3',
+    version='0.1.3.post1',
     scripts=['bin/template'],
     author="Stephen DiAdamo, Janis Nötzel, Benjamin Zanger, Mert Mehmet Bese",
     author_email="stephen.diadamo@gmail.com",
     description="A Quantum Network Simulation Framework",
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

