# Comparing `tmp/nwebclient-1.0.72.tar.gz` & `tmp/nwebclient-1.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.72.tar", last modified: Thu Apr 20 09:48:56 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.73.tar", last modified: Thu Apr 20 09:57:33 2023, max compression
```

## Comparing `nwebclient-1.0.72.tar` & `nwebclient-1.0.73.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 09:48:56.008598 nwebclient-1.0.72/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.72/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-20 09:48:56.008598 nwebclient-1.0.72/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.72/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 09:48:56.008598 nwebclient-1.0.72/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.72/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.72/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3104 2023-03-29 20:50:31.000000 nwebclient-1.0.72/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7297 2023-04-20 09:48:43.000000 nwebclient-1.0.72/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5582 2023-03-29 09:33:58.000000 nwebclient-1.0.72/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3218 2023-03-27 16:42:32.000000 nwebclient-1.0.72/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 09:48:56.008598 nwebclient-1.0.72/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-20 09:48:55.000000 nwebclient-1.0.72/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-04-20 09:48:55.000000 nwebclient-1.0.72/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-20 09:48:55.000000 nwebclient-1.0.72/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       84 2023-04-20 09:48:55.000000 nwebclient-1.0.72/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-04-20 09:48:55.000000 nwebclient-1.0.72/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-04-20 09:48:55.000000 nwebclient-1.0.72/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-20 09:48:56.008598 nwebclient-1.0.72/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      829 2023-04-20 09:48:53.000000 nwebclient-1.0.72/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 09:57:33.721127 nwebclient-1.0.73/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.73/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-20 09:57:33.721127 nwebclient-1.0.73/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.73/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 09:57:33.721127 nwebclient-1.0.73/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.73/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.73/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3104 2023-03-29 20:50:31.000000 nwebclient-1.0.73/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7293 2023-04-20 09:51:31.000000 nwebclient-1.0.73/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     5582 2023-03-29 09:33:58.000000 nwebclient-1.0.73/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3218 2023-03-27 16:42:32.000000 nwebclient-1.0.73/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 09:57:33.721127 nwebclient-1.0.73/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-20 09:57:33.000000 nwebclient-1.0.73/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-04-20 09:57:33.000000 nwebclient-1.0.73/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-20 09:57:33.000000 nwebclient-1.0.73/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       84 2023-04-20 09:57:33.000000 nwebclient-1.0.73/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-04-20 09:57:33.000000 nwebclient-1.0.73/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-04-20 09:57:33.000000 nwebclient-1.0.73/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-20 09:57:33.721127 nwebclient-1.0.73/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      829 2023-04-20 09:51:19.000000 nwebclient-1.0.73/setup.py
```

### Comparing `nwebclient-1.0.72/LICENSE` & `nwebclient-1.0.73/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.72/PKG-INFO` & `nwebclient-1.0.73/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.72
+Version: 1.0.73
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.72/README.md` & `nwebclient-1.0.73/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.72/nwebclient/__init__.py` & `nwebclient-1.0.73/nwebclient/__init__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.72/nwebclient/__main__.py` & `nwebclient-1.0.73/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.72/nwebclient/crypt.py` & `nwebclient-1.0.73/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.72/nwebclient/sd.py` & `nwebclient-1.0.73/nwebclient/sd.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
            self.pipe = StableDiffusionPipeline.from_pretrained(self.model_id, scheduler=self.scheduler, custom_pipeline="lpw_stable_diffusion", torch_dtype=torch.float16, revision=model_revision)
         self.pipe = self.pipe.to(device)
         if self.model_id=="XpucT/Deliberate" or self.model_id == "SG161222/Realistic_Vision_V1.4_Fantasy.ai":
             self.pipe.safety_checker = lambda images, clip_input: (images, False)
         self.load_model = self.model_id
     def initA1111(self):
         import webuiapi
-        if not self.api is None:
+        if self.api is None:
             self.api = webuiapi.WebUIApi()
     def gen(self, loop_number=1):
         if self.generator == 'diffusers':
             self.genDiffusers(loop_number)
         elif self.generator == 'automatic1111':
             self.genA1111(loop_number)
         elif self.generator == 'dummy':
```

### Comparing `nwebclient-1.0.72/nwebclient/sdb.py` & `nwebclient-1.0.73/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.72/nwebclient/ticker.py` & `nwebclient-1.0.73/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.72/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.73/nwebclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.72
+Version: 1.0.73
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.72/setup.py` & `nwebclient-1.0.73/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.72",
+    version="1.0.73",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

