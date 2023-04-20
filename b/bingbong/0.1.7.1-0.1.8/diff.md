# Comparing `tmp/bingbong-0.1.7.1-py3-none-any.whl.zip` & `tmp/bingbong-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 11158 bytes, number of entries: 15
--rw-rw-rw-  2.0 unx       55 b- defN 23-Apr-17 23:22 pingpong/__init__.py
--rw-rw-rw-  2.0 unx     1681 b- defN 23-Apr-17 23:21 pingpong/alpaca.py
--rw-rw-rw-  2.0 unx     1287 b- defN 23-Apr-17 22:59 pingpong/dolly.py
--rw-rw-rw-  2.0 unx      987 b- defN 23-Apr-14 05:26 pingpong/gradio.py
--rw-rw-rw-  2.0 unx     1212 b- defN 23-Apr-17 22:55 pingpong/pingpong.py
--rw-rw-rw-  2.0 unx      173 b- defN 23-Apr-12 04:36 pingpong/context/__init__.py
--rw-rw-rw-  2.0 unx      589 b- defN 23-Apr-12 00:59 pingpong/context/auto_summary_strategy.py
--rw-rw-rw-  2.0 unx      789 b- defN 23-Apr-17 22:54 pingpong/context/last_window_strategy.py
--rw-rw-rw-  2.0 unx      840 b- defN 23-Apr-12 04:54 pingpong/context/search_window_strategy.py
--rw-rw-rw-  2.0 unx      119 b- defN 23-Apr-11 14:54 pingpong/context/strategy.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-17 23:22 bingbong-0.1.7.1.dist-info/LICENSE
--rw-rw-rw-  2.0 unx     3348 b- defN 23-Apr-17 23:22 bingbong-0.1.7.1.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-17 23:22 bingbong-0.1.7.1.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        9 b- defN 23-Apr-17 23:22 bingbong-0.1.7.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1235 b- defN 23-Apr-17 23:22 bingbong-0.1.7.1.dist-info/RECORD
-15 files, 23773 bytes uncompressed, 9104 bytes compressed:  61.7%
+Zip file size: 11979 bytes, number of entries: 16
+-rw-rw-r--  2.0 unx       53 b- defN 23-Apr-20 20:04 pingpong/__init__.py
+-rw-rw-r--  2.0 unx     1681 b- defN 23-Apr-20 19:34 pingpong/alpaca.py
+-rw-rw-r--  2.0 unx     1287 b- defN 23-Apr-20 19:34 pingpong/dolly.py
+-rw-rw-r--  2.0 unx     1399 b- defN 23-Apr-20 19:47 pingpong/gradio.py
+-rw-rw-r--  2.0 unx     1212 b- defN 23-Apr-20 19:34 pingpong/pingpong.py
+-rw-rw-r--  2.0 unx     1496 b- defN 23-Apr-20 19:59 pingpong/stablelm.py
+-rw-rw-r--  2.0 unx      173 b- defN 23-Apr-20 19:34 pingpong/context/__init__.py
+-rw-rw-r--  2.0 unx      589 b- defN 23-Apr-20 19:34 pingpong/context/auto_summary_strategy.py
+-rw-rw-r--  2.0 unx      789 b- defN 23-Apr-20 19:34 pingpong/context/last_window_strategy.py
+-rw-rw-r--  2.0 unx      840 b- defN 23-Apr-20 19:34 pingpong/context/search_window_strategy.py
+-rw-rw-r--  2.0 unx      119 b- defN 23-Apr-20 19:34 pingpong/context/strategy.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-20 20:04 bingbong-0.1.8.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3346 b- defN 23-Apr-20 20:04 bingbong-0.1.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 20:04 bingbong-0.1.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-20 20:04 bingbong-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1303 b- defN 23-Apr-20 20:04 bingbong-0.1.8.dist-info/RECORD
+16 files, 25745 bytes uncompressed, 9829 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: pingpong/gradio.py
 Comment: 
 
 Filename: pingpong/pingpong.py
 Comment: 
 
+Filename: pingpong/stablelm.py
+Comment: 
+
 Filename: pingpong/context/__init__.py
 Comment: 
 
 Filename: pingpong/context/auto_summary_strategy.py
 Comment: 
 
 Filename: pingpong/context/last_window_strategy.py
@@ -24,23 +27,23 @@
 
 Filename: pingpong/context/search_window_strategy.py
 Comment: 
 
 Filename: pingpong/context/strategy.py
 Comment: 
 
-Filename: bingbong-0.1.7.1.dist-info/LICENSE
+Filename: bingbong-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: bingbong-0.1.7.1.dist-info/METADATA
+Filename: bingbong-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: bingbong-0.1.7.1.dist-info/WHEEL
+Filename: bingbong-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: bingbong-0.1.7.1.dist-info/top_level.txt
+Filename: bingbong-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: bingbong-0.1.7.1.dist-info/RECORD
+Filename: bingbong-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pingpong/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.1.7.1'
+__version__ = '0.1.8'
 
 from .pingpong import PingPong
```

## pingpong/gradio.py

```diff
@@ -1,10 +1,11 @@
 from pingpong.pingpong import PromptFmt, UIFmt
-from pingpong.alpaca import AlpacaPromptFmt, AlpacaChatPPManager
+from pingpong.alpaca import AlpacaChatPPManager
 from pingpong.dolly import DollyChatPPManager
+from pingpong.stablelm import StableLMChatPPManager
 
 class GradioChatUIFmt(UIFmt):
   @classmethod
   def ui(cls, pingpong):
     return (pingpong.ping, pingpong.pong)
 
 class GradioAlpacaChatPPManager(AlpacaChatPPManager):
@@ -26,7 +27,19 @@
 
     results = []
 
     for pingpong in self.pingpongs[from_idx:to_idx]:
       results.append(fmt.ui(pingpong))
 
     return results
+
+class GradioStableLMChatPPManager(StableLMChatPPManager):
+    def build_uis(self, from_idx: int=0, to_idx: int=-1, fmt: UIFmt=GradioChatUIFmt):
+      if to_idx == -1 or to_idx >= len(self.pingpongs):
+        to_idx = len(self.pingpongs)
+
+      results = []
+
+      for pingpong in self.pingpongs[from_idx:to_idx]:
+        results.append(fmt.ui(pingpong))
+
+      return results
```

## Comparing `bingbong-0.1.7.1.dist-info/LICENSE` & `bingbong-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bingbong-0.1.7.1.dist-info/METADATA` & `bingbong-0.1.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingbong
-Version: 0.1.7.1
+Version: 0.1.8
 Summary: Ping pong management library for LLM applied application
 Home-page: https://github.com/deep-diver/PingPong
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,pingpong,prompt,context,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `bingbong-0.1.7.1.dist-info/RECORD` & `bingbong-0.1.8.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-pingpong/__init__.py,sha256=0J8K3p7tVxjO1aXvzCbcYLxzXrRxyYoo4EFT_JzFfGE,55
+pingpong/__init__.py,sha256=7HuUZUYPXV1B8IQ_7l4c1F_V-NdBC7QKOqwKUNZIOLI,53
 pingpong/alpaca.py,sha256=NLRBCMfyXmgL9S5SmVRUPPDsEjsw9Kv0iFYPTrPZVgs,1681
 pingpong/dolly.py,sha256=vMbHiwgeewzRAsruuMVnQc2w3KEKhWJUdOmaBbyazQo,1287
-pingpong/gradio.py,sha256=IchvS_gOuPk3TCATVKDWMaLEaIRqjPpi3MFnYwa0JwU,987
+pingpong/gradio.py,sha256=K474EiQbNmyvPhfnx-0yTBFrU2X61sVy5v7JcQivQHI,1399
 pingpong/pingpong.py,sha256=XfCYe-OdNkyrKOhAEaL4Q-HhZx829_i-ohDlY2GF7gM,1212
+pingpong/stablelm.py,sha256=UlFLilnxUuJpYwcA_aANTVkQERMSK44ULx1kl-K-L6k,1496
 pingpong/context/__init__.py,sha256=ksYP7nq8inYK7SHDwpd7Hs_h87gPKdP9Ac6E5w0X6zM,173
 pingpong/context/auto_summary_strategy.py,sha256=s2lrlGKzLFNBGdLMAkaC6d2VY8aJSdgtrwa_Rvmt3Fc,589
 pingpong/context/last_window_strategy.py,sha256=JN7pFDD2C8nGMUx-H3aHNQrXCT0E0S-FlBunOrQGX-w,789
 pingpong/context/search_window_strategy.py,sha256=OPd2xxiI9FrzU4w2R5luaDEKiNEj4KYr_EF53Qi6l_Q,840
 pingpong/context/strategy.py,sha256=xGoy7T92gYubrwekz0Kz2Vxv10njgXG44K48bC9BqAU,119
-bingbong-0.1.7.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-bingbong-0.1.7.1.dist-info/METADATA,sha256=trgkUPrydQyRLN4_BQdKRA3BSQyi2IVWoAr054Y0qSc,3348
-bingbong-0.1.7.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bingbong-0.1.7.1.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
-bingbong-0.1.7.1.dist-info/RECORD,,
+bingbong-0.1.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+bingbong-0.1.8.dist-info/METADATA,sha256=uZWiwivUq2GMwe4MgvfrjmraWdCNDg-cm2TNKvksCz8,3346
+bingbong-0.1.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bingbong-0.1.8.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
+bingbong-0.1.8.dist-info/RECORD,,
```

