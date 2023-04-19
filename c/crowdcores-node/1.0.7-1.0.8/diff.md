# Comparing `tmp/crowdcores-node-1.0.7.tar.gz` & `tmp/crowdcores-node-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdcores-node-1.0.7.tar", last modified: Wed Apr 19 21:48:42 2023, max compression
+gzip compressed data, was "crowdcores-node-1.0.8.tar", last modified: Wed Apr 19 21:52:35 2023, max compression
```

## Comparing `crowdcores-node-1.0.7.tar` & `crowdcores-node-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:48:42.468975 crowdcores-node-1.0.7/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 01:07:39.000000 crowdcores-node-1.0.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 21:48:42.468975 crowdcores-node-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2023-04-19 01:01:15.000000 crowdcores-node-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:48:42.468975 crowdcores-node-1.0.7/crowdcores_node/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-18 22:47:07.000000 crowdcores-node-1.0.7/crowdcores_node/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4026 2023-04-19 21:34:30.000000 crowdcores-node-1.0.7/crowdcores_node/crowdcores_node.py
--rw-r--r--   0 root         (0) root         (0)     2835 2023-04-19 21:48:22.000000 crowdcores-node-1.0.7/crowdcores_node/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:48:42.468975 crowdcores-node-1.0.7/crowdcores_node.egg-info/
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 21:48:42.000000 crowdcores-node-1.0.7/crowdcores_node.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2023-04-19 21:48:42.000000 crowdcores-node-1.0.7/crowdcores_node.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 21:48:42.000000 crowdcores-node-1.0.7/crowdcores_node.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-19 21:48:42.000000 crowdcores-node-1.0.7/crowdcores_node.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-19 21:48:42.000000 crowdcores-node-1.0.7/crowdcores_node.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-19 21:48:42.000000 crowdcores-node-1.0.7/crowdcores_node.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 21:48:42.468975 crowdcores-node-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      352 2023-04-19 21:48:31.000000 crowdcores-node-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:52:35.684201 crowdcores-node-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 01:07:39.000000 crowdcores-node-1.0.8/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 21:52:35.684201 crowdcores-node-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2023-04-19 01:01:15.000000 crowdcores-node-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:52:35.684201 crowdcores-node-1.0.8/crowdcores_node/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-18 22:47:07.000000 crowdcores-node-1.0.8/crowdcores_node/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4026 2023-04-19 21:34:30.000000 crowdcores-node-1.0.8/crowdcores_node/crowdcores_node.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-04-19 21:52:17.000000 crowdcores-node-1.0.8/crowdcores_node/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:52:35.684201 crowdcores-node-1.0.8/crowdcores_node.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 21:52:35.000000 crowdcores-node-1.0.8/crowdcores_node.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      356 2023-04-19 21:52:35.000000 crowdcores-node-1.0.8/crowdcores_node.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 21:52:35.000000 crowdcores-node-1.0.8/crowdcores_node.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-19 21:52:35.000000 crowdcores-node-1.0.8/crowdcores_node.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-19 21:52:35.000000 crowdcores-node-1.0.8/crowdcores_node.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-19 21:52:35.000000 crowdcores-node-1.0.8/crowdcores_node.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 21:52:35.684201 crowdcores-node-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      352 2023-04-19 21:52:26.000000 crowdcores-node-1.0.8/setup.py
```

### Comparing `crowdcores-node-1.0.7/LICENSE.txt` & `crowdcores-node-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crowdcores-node-1.0.7/crowdcores_node/crowdcores_node.py` & `crowdcores-node-1.0.8/crowdcores_node/crowdcores_node.py`

 * *Files identical despite different names*

### Comparing `crowdcores-node-1.0.7/crowdcores_node/manager.py` & `crowdcores-node-1.0.8/crowdcores_node/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     update()
     print("Starting CrowdCore Node...")
 
     script_dir = os.path.dirname(os.path.realpath(__file__))
     node_path = os.path.join(script_dir, "crowdcores_node", "crowdcores_node.py")
 
     with open(node_out_put_file, 'w') as f:
-        process = subprocess.Popen(["python3","-u","crowdcores_node.py"], stdout=f, stderr=f)
+        process = subprocess.Popen(["python3","-u",node_path], stdout=f, stderr=f)
     print("CrowdCore Node started with PID:", process.pid)
 
 def stop():
     print("Stopping CrowdCore Node...")
     pid = get_pid()
     if pid:
         os.kill(pid, signal.SIGTERM)
```

