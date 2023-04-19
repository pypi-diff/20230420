# Comparing `tmp/crowdcores-node-1.0.9.tar.gz` & `tmp/crowdcores-node-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdcores-node-1.0.9.tar", last modified: Wed Apr 19 22:02:18 2023, max compression
+gzip compressed data, was "crowdcores-node-1.1.0.tar", last modified: Wed Apr 19 22:05:01 2023, max compression
```

## Comparing `crowdcores-node-1.0.9.tar` & `crowdcores-node-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:02:18.938215 crowdcores-node-1.0.9/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 01:07:39.000000 crowdcores-node-1.0.9/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 22:02:18.938215 crowdcores-node-1.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2023-04-19 01:01:15.000000 crowdcores-node-1.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:02:18.934215 crowdcores-node-1.0.9/crowdcores_node/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-18 22:47:07.000000 crowdcores-node-1.0.9/crowdcores_node/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4026 2023-04-19 21:34:30.000000 crowdcores-node-1.0.9/crowdcores_node/crowdcores_node.py
--rw-r--r--   0 root         (0) root         (0)     2816 2023-04-19 22:00:58.000000 crowdcores-node-1.0.9/crowdcores_node/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:02:18.938215 crowdcores-node-1.0.9/crowdcores_node.egg-info/
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 22:02:18.000000 crowdcores-node-1.0.9/crowdcores_node.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2023-04-19 22:02:18.000000 crowdcores-node-1.0.9/crowdcores_node.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 22:02:18.000000 crowdcores-node-1.0.9/crowdcores_node.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-19 22:02:18.000000 crowdcores-node-1.0.9/crowdcores_node.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-19 22:02:18.000000 crowdcores-node-1.0.9/crowdcores_node.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-19 22:02:18.000000 crowdcores-node-1.0.9/crowdcores_node.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 22:02:18.938215 crowdcores-node-1.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      352 2023-04-19 22:01:27.000000 crowdcores-node-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:05:01.717643 crowdcores-node-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 01:07:39.000000 crowdcores-node-1.1.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 22:05:01.717643 crowdcores-node-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2023-04-19 01:01:15.000000 crowdcores-node-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:05:01.717643 crowdcores-node-1.1.0/crowdcores_node/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-18 22:47:07.000000 crowdcores-node-1.1.0/crowdcores_node/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4028 2023-04-19 22:04:35.000000 crowdcores-node-1.1.0/crowdcores_node/crowdcores_node.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2023-04-19 22:00:58.000000 crowdcores-node-1.1.0/crowdcores_node/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:05:01.717643 crowdcores-node-1.1.0/crowdcores_node.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 22:05:01.000000 crowdcores-node-1.1.0/crowdcores_node.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      356 2023-04-19 22:05:01.000000 crowdcores-node-1.1.0/crowdcores_node.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 22:05:01.000000 crowdcores-node-1.1.0/crowdcores_node.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-19 22:05:01.000000 crowdcores-node-1.1.0/crowdcores_node.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-19 22:05:01.000000 crowdcores-node-1.1.0/crowdcores_node.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-19 22:05:01.000000 crowdcores-node-1.1.0/crowdcores_node.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 22:05:01.717643 crowdcores-node-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      352 2023-04-19 22:04:56.000000 crowdcores-node-1.1.0/setup.py
```

### Comparing `crowdcores-node-1.0.9/LICENSE.txt` & `crowdcores-node-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crowdcores-node-1.0.9/crowdcores_node/crowdcores_node.py` & `crowdcores-node-1.1.0/crowdcores_node/crowdcores_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                 )
                 for task in pending:
                     task.cancel()
                 #await asyncio.Future()
         #except (OSError, websockets.exceptions.ConnectionClosed) as e:
         except Exception as e:
             print(f"Connection failed: {e}")
-            print("Retrying in 5 seconds...")
+            print("Retrying in 5 seconds.....")
             time.sleep(5)
 
 def main():
     asyncio.run(client())
 
 if __name__ == "__main__":
     main()
```

### Comparing `crowdcores-node-1.0.9/crowdcores_node/manager.py` & `crowdcores-node-1.1.0/crowdcores_node/manager.py`

 * *Files identical despite different names*

