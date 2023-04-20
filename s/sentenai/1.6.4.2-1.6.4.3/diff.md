# Comparing `tmp/sentenai-1.6.4.2.tar.gz` & `tmp/sentenai-1.6.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sentenai-1.6.4.2.tar", last modified: Mon Apr  3 14:29:31 2023, max compression
+gzip compressed data, was "sentenai-1.6.4.3.tar", last modified: Thu Apr 20 15:55:32 2023, max compression
```

## Comparing `sentenai-1.6.4.2.tar` & `sentenai-1.6.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-03 14:29:31.000000 sentenai-1.6.4.2/
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.4.2/LICENSE
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-03 14:29:31.000000 sentenai-1.6.4.2/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.4.2/README.md
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-03 14:29:31.000000 sentenai-1.6.4.2/sentenai/
--rw-r--r--   0 xnomagichash   (501) staff       (20)     7529 2023-03-30 18:41:36.000000 sentenai-1.6.4.2/sentenai/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     9729 2023-03-30 18:29:31.000000 sentenai-1.6.4.2/sentenai/api.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-03 14:29:31.000000 sentenai-1.6.4.2/sentenai/stream/
--rw-r--r--   0 xnomagichash   (501) staff       (20)       53 2022-10-04 21:43:28.000000 sentenai-1.6.4.2/sentenai/stream/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.4.2/sentenai/stream/events.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     2161 2023-02-13 21:49:04.000000 sentenai-1.6.4.2/sentenai/stream/metadata.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)    24315 2023-04-03 14:28:14.000000 sentenai-1.6.4.2/sentenai/stream/streams.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-03 14:29:31.000000 sentenai-1.6.4.2/sentenai.egg-info/
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-03 14:29:31.000000 sentenai-1.6.4.2/sentenai.egg-info/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      341 2023-04-03 14:29:31.000000 sentenai-1.6.4.2/sentenai.egg-info/SOURCES.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-04-03 14:29:31.000000 sentenai-1.6.4.2/sentenai.egg-info/dependency_links.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-04-03 14:29:31.000000 sentenai-1.6.4.2/sentenai.egg-info/requires.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-04-03 14:29:31.000000 sentenai-1.6.4.2/sentenai.egg-info/top_level.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-04-03 14:29:31.000000 sentenai-1.6.4.2/setup.cfg
--rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-04-03 14:29:18.000000 sentenai-1.6.4.2/setup.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-20 15:55:32.683889 sentenai-1.6.4.3/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.4.3/LICENSE
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-20 15:55:32.683968 sentenai-1.6.4.3/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.4.3/README.md
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-20 15:55:32.682102 sentenai-1.6.4.3/sentenai/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     9052 2023-04-20 15:49:21.000000 sentenai-1.6.4.3/sentenai/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     9729 2023-03-30 18:29:31.000000 sentenai-1.6.4.3/sentenai/api.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-20 15:55:32.683723 sentenai-1.6.4.3/sentenai/stream/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       53 2022-10-04 21:43:28.000000 sentenai-1.6.4.3/sentenai/stream/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.4.3/sentenai/stream/events.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     2161 2023-02-13 21:49:04.000000 sentenai-1.6.4.3/sentenai/stream/metadata.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)    24211 2023-04-20 15:49:17.000000 sentenai-1.6.4.3/sentenai/stream/streams.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-20 15:55:32.682738 sentenai-1.6.4.3/sentenai.egg-info/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-20 15:55:32.000000 sentenai-1.6.4.3/sentenai.egg-info/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      341 2023-04-20 15:55:32.000000 sentenai-1.6.4.3/sentenai.egg-info/SOURCES.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-04-20 15:55:32.000000 sentenai-1.6.4.3/sentenai.egg-info/dependency_links.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-04-20 15:55:32.000000 sentenai-1.6.4.3/sentenai.egg-info/requires.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-04-20 15:55:32.000000 sentenai-1.6.4.3/sentenai.egg-info/top_level.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-04-20 15:55:32.684202 sentenai-1.6.4.3/setup.cfg
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-04-20 15:49:43.000000 sentenai-1.6.4.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sentenai-1.6.4.2/LICENSE` & `sentenai-1.6.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.2/PKG-INFO` & `sentenai-1.6.4.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.4.2
+Version: 1.6.4.3
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.4.2/README.md` & `sentenai-1.6.4.3/README.md`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.2/sentenai/__init__.py` & `sentenai-1.6.4.3/sentenai/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from sentenai.api import *
 from sentenai.stream import Database
 if PANDAS: import pandas as pd
 from datetime import datetime
+import io
+import uuid
+from pathlib import Path
 
 import time
 
 __all__ = ['Sentenai']
 
 if PANDAS:
     def df(events):
@@ -113,29 +116,51 @@
             return repr(list(self._tspl.values())[0])
         else:
             return "\n".join([f'{key} = {value!r}' for key, value in self._tspl.items()])
     
     def explain(self):
         return self._post("debug", json=self._tspl['value']).json()
 
+    def plan(self):
+        from IPython.display import IFrame
+         
+        def js_ui(data, template, out_fn = None, out_path='.',
+                  width="800px", height="600px", **kwargs):
+            """Generate an IFrame containing a templated javascript package."""
+            if not out_fn:
+                out_fn = Path(f"{uuid.uuid4()}.html")
+                 
+            # Generate the path to the output file
+            out_path = Path(out_path)
+            filepath = out_path / out_fn
+            # Check the required directory path exists
+            filepath.parent.mkdir(parents=True, exist_ok=True)
+         
+            # The open "wt" parameters are: write, text mode;
+            with io.open(filepath, 'wt', encoding='utf8') as outfile:
+                # The data is passed in as a dictionary so we can pass different
+                # arguments to the template
+                outfile.write(template.format(**data))
+         
+            return IFrame(src=filepath, width=width, height=height)
+        
+        return js_ui({'src': self.explain()['tsvm']}, TEMPLATE_MERMAIDJS)
+
+
     @property
     def range(self):
         if self._info:
             return {'start': dt64(self._info['start']), 'end': dt64(self._info['end'])}
         else:
             self._info = self._post("range", json=self._tspl['value']).json()
             return self.range
 
     @property
     def origin(self):
-        if self._info:
-            return dt64(self._info.get('origin'))
-        else:
-            self._info = self._post("range", json=self._tspl['value']).json()
-            return self.origin
+        return dt64(self._post("debug", json=self._tspl['value']).json().get('origin'))
 
     @property
     def type(self):
         if self._info:
             return self._info.get('type')
         else:
             self._info = self._post("range", json=self._tspl['value']).json()
@@ -222,7 +247,24 @@
 
 
         else:
             raise Exception("wrong type")
     
 
 
+TEMPLATE_MERMAIDJS="""<html>
+    <head>
+            <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">
+    <head>
+    <body>
+        <script type="module">
+            import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
+            mermaid.initialize({{ startOnLoad: true }});
+        </script>
+ 
+        <pre class="mermaid">
+            {src}
+        </pre>
+ 
+    </body>
+</html>
+"""
```

### Comparing `sentenai-1.6.4.2/sentenai/api.py` & `sentenai-1.6.4.3/sentenai/api.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.2/sentenai/stream/events.py` & `sentenai-1.6.4.3/sentenai/stream/events.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.2/sentenai/stream/metadata.py` & `sentenai-1.6.4.3/sentenai/stream/metadata.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.2/sentenai/stream/streams.py` & `sentenai-1.6.4.3/sentenai/stream/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,27 +250,25 @@
             return Stream(self, key)
 
     def __setitem__(self, key, content):
         workers = 32
         if isinstance(key, tuple):
             if isinstance(key[-1], slice):
                 path = key[:-1]
-                path.append(key[-1].start)
+                path += key[-1].start
                 workers = key[-1].stop
             else:
                 path = key
         elif isinstance(key, slice):
-            path = key[:-1]
-            path.append(key[-1].start)
-            workers = key[-1].stop
-
+            workers = key.stop
+            path = key.start
         else:
             path = (key,)
+
         del self[path]
-        path = key if isinstance(key, tuple) else (key,)
 
         if content is None:
             nid = self._put('paths', *path, json={'kind': 'directory'})
         elif type(content) == str:
             nid = self._put('paths', *path, json={'kind': 'virtual', 'tspl': content})
         elif isinstance(content, Stream):
             nid = content._node
```

### Comparing `sentenai-1.6.4.2/sentenai.egg-info/PKG-INFO` & `sentenai-1.6.4.3/sentenai.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.4.2
+Version: 1.6.4.3
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.4.2/setup.py` & `sentenai-1.6.4.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sentenai',
-    version='1.6.4.2',
+    version='1.6.4.3',
     description='Client library for Sentenai',
     long_description="",
     url='https://github.com/sentenai/py-sentenai',
 
     author='Sentenai, Inc.',
     author_email='info@sentenai.com',
```

