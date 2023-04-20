# Comparing `tmp/zappix-1.0.0.tar.gz` & `tmp/zappix-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zappix-1.0.0.tar", last modified: Wed Apr 19 21:43:18 2023, max compression
+gzip compressed data, was "zappix-1.0.1.tar", last modified: Thu Apr 20 16:24:16 2023, max compression
```

## Comparing `zappix-1.0.0.tar` & `zappix-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:43:18.958181 zappix-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1054 2023-04-19 21:43:17.000000 zappix-1.0.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     3771 2023-04-19 21:43:18.958181 zappix-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3005 2023-04-19 21:43:17.000000 zappix-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 21:43:18.958181 zappix-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-04-19 21:43:17.000000 zappix-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:43:18.956181 zappix-1.0.0/zappix/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 21:43:17.000000 zappix-1.0.0/zappix/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2358 2023-04-19 21:43:17.000000 zappix-1.0.0/zappix/agent_active.py
--rw-rw-rw-   0 root         (0) root         (0)     5558 2023-04-19 21:43:17.000000 zappix-1.0.0/zappix/dstream.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2023-04-19 21:43:17.000000 zappix-1.0.0/zappix/get.py
--rw-rw-rw-   0 root         (0) root         (0)     6736 2023-04-19 21:43:17.000000 zappix-1.0.0/zappix/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     6889 2023-04-19 21:43:17.000000 zappix-1.0.0/zappix/sender.py
--rw-rw-rw-   0 root         (0) root         (0)     2031 2023-04-19 21:43:17.000000 zappix-1.0.0/zappix/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:43:18.957181 zappix-1.0.0/zappix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3771 2023-04-19 21:43:18.000000 zappix-1.0.0/zappix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2023-04-19 21:43:18.000000 zappix-1.0.0/zappix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 21:43:18.000000 zappix-1.0.0/zappix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-19 21:43:18.000000 zappix-1.0.0/zappix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-19 21:43:18.000000 zappix-1.0.0/zappix.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 16:24:16.251573 zappix-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2023-04-20 16:24:14.000000 zappix-1.0.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-04-20 16:24:16.251573 zappix-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3005 2023-04-20 16:24:14.000000 zappix-1.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 16:24:16.251573 zappix-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-04-20 16:24:14.000000 zappix-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 16:24:16.249573 zappix-1.0.1/zappix/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 16:24:14.000000 zappix-1.0.1/zappix/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2358 2023-04-20 16:24:14.000000 zappix-1.0.1/zappix/agent_active.py
+-rw-rw-rw-   0 root         (0) root         (0)     5564 2023-04-20 16:24:14.000000 zappix-1.0.1/zappix/dstream.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-04-20 16:24:14.000000 zappix-1.0.1/zappix/get.py
+-rw-rw-rw-   0 root         (0) root         (0)     6736 2023-04-20 16:24:14.000000 zappix-1.0.1/zappix/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     6889 2023-04-20 16:24:14.000000 zappix-1.0.1/zappix/sender.py
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-04-20 16:24:14.000000 zappix-1.0.1/zappix/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 16:24:16.251573 zappix-1.0.1/zappix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-04-20 16:24:16.000000 zappix-1.0.1/zappix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2023-04-20 16:24:16.000000 zappix-1.0.1/zappix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 16:24:16.000000 zappix-1.0.1/zappix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-20 16:24:16.000000 zappix-1.0.1/zappix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-20 16:24:16.000000 zappix-1.0.1/zappix.egg-info/top_level.txt
```

### Comparing `zappix-1.0.0/LICENSE.txt` & `zappix-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zappix-1.0.0/PKG-INFO` & `zappix-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zappix
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python replacement for Zabbix sender and get.
 Home-page: https://gitlab.com/szuro/zappix
 Author: Robert Szulist
 Author-email: r.szulist@gmail.com
 Keywords: zabbix get sender
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `zappix-1.0.0/README.md` & `zappix-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `zappix-1.0.0/setup.py` & `zappix-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open(path.join(here, 'README.md'), 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='zappix',
-    version='1.0.0',
+    version='1.0.1',
     description='A Python replacement for Zabbix sender and get.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://gitlab.com/szuro/zappix',
     author='Robert Szulist',
     author_email='r.szulist@gmail.com',
     classifiers=[
```

### Comparing `zappix-1.0.0/zappix/agent_active.py` & `zappix-1.0.1/zappix/agent_active.py`

 * *Files identical despite different names*

### Comparing `zappix-1.0.0/zappix/dstream.py` & `zappix-1.0.1/zappix/dstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self._ip = target
         self._port = port
         self._source_address = source_address
         self._timeout = None
         self._psk = b''
         self._psk_identity = b''
 
-    def set_timeout(timeout: float):
+    def set_timeout(self, timeout: float):
         """
         Set timeout for the network connection
 
         Parameters
         ----------
         :timeout:
             Timeout in seconds.
```

### Comparing `zappix-1.0.0/zappix/get.py` & `zappix-1.0.1/zappix/get.py`

 * *Files identical despite different names*

### Comparing `zappix-1.0.0/zappix/protocol.py` & `zappix-1.0.1/zappix/protocol.py`

 * *Files identical despite different names*

### Comparing `zappix-1.0.0/zappix/sender.py` & `zappix-1.0.1/zappix/sender.py`

 * *Files identical despite different names*

### Comparing `zappix-1.0.0/zappix/server.py` & `zappix-1.0.1/zappix/server.py`

 * *Files identical despite different names*

### Comparing `zappix-1.0.0/zappix.egg-info/PKG-INFO` & `zappix-1.0.1/zappix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zappix
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python replacement for Zabbix sender and get.
 Home-page: https://gitlab.com/szuro/zappix
 Author: Robert Szulist
 Author-email: r.szulist@gmail.com
 Keywords: zabbix get sender
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
```

