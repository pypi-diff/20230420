# Comparing `tmp/nwebclient-1.0.74.tar.gz` & `tmp/nwebclient-1.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.74.tar", last modified: Thu Apr 20 10:42:23 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.75.tar", last modified: Thu Apr 20 19:27:27 2023, max compression
```

## Comparing `nwebclient-1.0.74.tar` & `nwebclient-1.0.75.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 10:42:23.288970 nwebclient-1.0.74/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.74/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-20 10:42:23.298970 nwebclient-1.0.74/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.74/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 10:42:23.288970 nwebclient-1.0.74/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.74/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.74/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3104 2023-03-29 20:50:31.000000 nwebclient-1.0.74/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7748 2023-04-20 10:41:58.000000 nwebclient-1.0.74/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5582 2023-03-29 09:33:58.000000 nwebclient-1.0.74/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3218 2023-03-27 16:42:32.000000 nwebclient-1.0.74/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 10:42:23.288970 nwebclient-1.0.74/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-20 10:42:23.000000 nwebclient-1.0.74/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-04-20 10:42:23.000000 nwebclient-1.0.74/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-20 10:42:23.000000 nwebclient-1.0.74/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       84 2023-04-20 10:42:23.000000 nwebclient-1.0.74/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-04-20 10:42:23.000000 nwebclient-1.0.74/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-04-20 10:42:23.000000 nwebclient-1.0.74/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-20 10:42:23.298970 nwebclient-1.0.74/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      829 2023-04-20 10:42:06.000000 nwebclient-1.0.74/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 19:27:27.083393 nwebclient-1.0.75/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.75/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-20 19:27:27.083393 nwebclient-1.0.75/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.75/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 19:27:27.083393 nwebclient-1.0.75/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.75/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.75/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3104 2023-03-29 20:50:31.000000 nwebclient-1.0.75/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     9281 2023-04-20 18:14:27.000000 nwebclient-1.0.75/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     5582 2023-03-29 09:33:58.000000 nwebclient-1.0.75/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3218 2023-03-27 16:42:32.000000 nwebclient-1.0.75/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 19:27:27.083393 nwebclient-1.0.75/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-20 19:27:26.000000 nwebclient-1.0.75/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-04-20 19:27:26.000000 nwebclient-1.0.75/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-20 19:27:26.000000 nwebclient-1.0.75/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       84 2023-04-20 19:27:26.000000 nwebclient-1.0.75/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-04-20 19:27:26.000000 nwebclient-1.0.75/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-04-20 19:27:26.000000 nwebclient-1.0.75/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-20 19:27:27.083393 nwebclient-1.0.75/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      829 2023-04-20 18:14:48.000000 nwebclient-1.0.75/setup.py
```

### Comparing `nwebclient-1.0.74/LICENSE` & `nwebclient-1.0.75/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.74/PKG-INFO` & `nwebclient-1.0.75/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.74
+Version: 1.0.75
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.74/README.md` & `nwebclient-1.0.75/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.74/nwebclient/__init__.py` & `nwebclient-1.0.75/nwebclient/__init__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.74/nwebclient/__main__.py` & `nwebclient-1.0.75/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.74/nwebclient/crypt.py` & `nwebclient-1.0.75/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.74/nwebclient/sd.py` & `nwebclient-1.0.75/nwebclient/sd.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 from nwebclient import ticker
 import json
 import os
 import requests
 import time
 
 from diffusers import PNDMScheduler, DDIMScheduler, LMSDiscreteScheduler, EulerDiscreteScheduler, DPMSolverMultistepScheduler
+from diffusers import UniPCMultistepScheduler
 import torch
 from diffusers import StableDiffusionPipeline
+from diffusers import StableDiffusionControlNetPipeline, ControlNetModel
 
 def gen(pipe, prompt='photo', negative_prompt = None, prefix='sd',  guidance_scale = 7.5, num_inference_steps=30, height=800, width=640, num_images=1, dbfile='data.db'):
     # https://huggingface.co/docs/diffusers/v0.14.0/en/api/pipelines/stable_diffusion/text2img#diffusers.StableDiffusionPipeline.__call__
     images = pipe(
       prompt,
       height = 800,
       width = 640,
@@ -30,15 +32,15 @@
   ig = sd.ImageGen()
   ig.prompt = "photo"
   ig.loop(5)
   
   ig.executeFromUrl('https://...')
 """
 class ImageGen:
-    generator = 'diffusers' # diffusers or automatic1111 dummy cn_pose_1111
+    generator = 'diffusers' # diffusers or automatic1111 dummy cn_pose_1111 diffcn
     # scheduler
     pipe = None
     prompt = "photo"
     negative_prompt = "text, cartoon, anime, drawing, meme, postcard, painting, ((fuzzy)), ((blurred)), ((low resolution)), ((b&w)), ((monochrome)), ambiguous, ((deformed)), oversaturated, ((out of shot)), ((incoherent)), (((glitched))), (((3d render))), cgi, ((incorrect anatomy)), bad hands, lowres, long body, ((blurry)), double, ((duplicate body parts)), (disfigured), (extra limbs), fused fingers, extra fingers, malformed hands, ((((mutated hands and fingers)))), conjoined, ((missing limbs)), logo, signature, mutated, jpeg artifacts, low quality, bad eyes, oversized, disproportionate, (((incorrect proportions))), exaggerated, (((aliasing)))"
     guidance_scale = 7.5
     num_inference_steps=25
     height=800
@@ -48,14 +50,15 @@
     dbfile='data.db'
     # sdb jpg
     save_mode='sdb'
     loaded_model = None
     gen_count = 0
     api = None
     cn_image = None
+    diff_cn = None
     def __init__(self, model_id="XpucT/Deliberate"):
         self.model_id = model_id
     def load(self):
         if self.loaded_model == self.model_id:
             return
         self.scheduler = DPMSolverMultistepScheduler.from_pretrained(self.model_id, subfolder="scheduler")
         device = "cuda"
@@ -68,32 +71,52 @@
         if self.model_id=="XpucT/Deliberate" or self.model_id == "SG161222/Realistic_Vision_V1.4_Fantasy.ai":
             self.pipe.safety_checker = lambda images, clip_input: (images, False)
         self.load_model = self.model_id
     def initA1111(self):
         import webuiapi
         if self.api is None:
             self.api = webuiapi.WebUIApi()
+    def initDiffCn(self):
+        if self.diff_cn is None:
+            self.controlnet = ControlNetModel.from_pretrained("lllyasviel/sd-controlnet-openpose")#, ) lllyasviel/sd-controlnet-canny
+            self.diff_cn = StableDiffusionControlNetPipeline.from_pretrained(model_id, controlnet=controlnet) # , torch_dtype=torch.float16
+            self.diff_cn.scheduler = UniPCMultistepScheduler.from_config(controlnet_pipe.scheduler.config)
+            self.diff_cn.enable_model_cpu_offload()
+            #controlnet_pipe.enable_xformers_memory_efficient_attention()
+            self.diff_cn = self.diff_cn.to("cuda")
+            if self.model_id=="XpucT/Deliberate" or self.model_id == "SG161222/Realistic_Vision_V1.4_Fantasy.ai":
+                self.diff_cn.safety_checker = lambda images, clip_input: (images, False)
     def gen(self, loop_number=1):
         if self.generator == 'diffusers':
             self.genDiffusers(loop_number)
         elif self.generator == 'automatic1111':
             self.genA1111(loop_number)
         elif self.generator == 'cn_pose_1111':
             self.genA1111(loop_number)
+        elif self.generator == 'diffcn':
+            self.genDiffCn(loop_number)
         elif self.generator == 'dummy':
             time.sleep(1)
             print("Dummy Generation; " + str(loop_number))
+            self.gen_count = self.gen_count + 1
+    def genDiffCn(self, loop_number=1):
+        self.initDiffCn()
+        output= self.diff_cn(self.prompt, self.cn_image, negative_prompt=self.negative_prompt, num_inference_steps=25, num_images_per_prompt = 1, height = self.height, width = self.width)
+        self.save_image(output[0][0], 0,loop_number)
+        self.gen_count = self.gen_count + 1
     def genCnPose1111(self, loop_number=1):
         self.initA1111();
         result = self.api.txt2img(prompt=self.prompt,negative_prompt=self.negative_prompt, height=self.height, width=self.width, controlnet_units=[self.cn_image],cfg_scale=7)
         self.save_image(result.image, 0,loop_number)
+        self.gen_count = self.gen_count + 1
     def genA1111(self, loop_number=1):  
         self.initA1111();
         result = self.api.txt2img(prompt=self.prompt,negative_prompt=self.negative_prompt, height=self.height, width=self.width, cfg_scale=7)
         self.save_image(result.image, 0,loop_number)
+        self.gen_count = self.gen_count + 1
     def genDiffusers(self, loop_number=1):
         if self.pipe is None:
             self.load()
         images = self.pipe(self.prompt,
             height = self.height,
             width = self.width,
             num_inference_steps = self.num_inference_steps,      # higher better quali default=45
```

### Comparing `nwebclient-1.0.74/nwebclient/sdb.py` & `nwebclient-1.0.75/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.74/nwebclient/ticker.py` & `nwebclient-1.0.75/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.74/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.75/nwebclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.74
+Version: 1.0.75
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.74/setup.py` & `nwebclient-1.0.75/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.74",
+    version="1.0.75",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

