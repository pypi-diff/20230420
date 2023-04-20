# Comparing `tmp/EdgeGPT-0.2.0.tar.gz` & `tmp/EdgeGPT-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.2.0.tar", last modified: Wed Apr 19 10:30:37 2023, max compression
+gzip compressed data, was "EdgeGPT-0.2.1.tar", last modified: Thu Apr 20 00:36:06 2023, max compression
```

## Comparing `EdgeGPT-0.2.0.tar` & `EdgeGPT-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:30:37.898569 EdgeGPT-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-19 10:30:02.000000 EdgeGPT-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-19 10:30:37.898569 EdgeGPT-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-04-19 10:30:37.000000 EdgeGPT-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 10:30:37.898569 EdgeGPT-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-19 10:30:02.000000 EdgeGPT-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:30:37.898569 EdgeGPT-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:30:37.898569 EdgeGPT-0.2.0/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-19 10:30:37.000000 EdgeGPT-0.2.0/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-19 10:30:37.000000 EdgeGPT-0.2.0/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:30:37.000000 EdgeGPT-0.2.0/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-19 10:30:37.000000 EdgeGPT-0.2.0/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 10:30:37.000000 EdgeGPT-0.2.0/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 10:30:37.000000 EdgeGPT-0.2.0/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18775 2023-04-19 10:30:02.000000 EdgeGPT-0.2.0/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 10:30:02.000000 EdgeGPT-0.2.0/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:36:06.431137 EdgeGPT-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-20 00:35:38.000000 EdgeGPT-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-20 00:36:06.431137 EdgeGPT-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-04-20 00:36:06.000000 EdgeGPT-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-20 00:36:06.431137 EdgeGPT-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-20 00:35:38.000000 EdgeGPT-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:36:06.431137 EdgeGPT-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:36:06.431137 EdgeGPT-0.2.1/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-20 00:36:06.000000 EdgeGPT-0.2.1/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-20 00:36:06.000000 EdgeGPT-0.2.1/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:36:06.000000 EdgeGPT-0.2.1/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 00:36:06.000000 EdgeGPT-0.2.1/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 00:36:06.000000 EdgeGPT-0.2.1/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 00:36:06.000000 EdgeGPT-0.2.1/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18768 2023-04-20 00:35:38.000000 EdgeGPT-0.2.1/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 00:35:38.000000 EdgeGPT-0.2.1/src/ImageGen.py
```

### Comparing `EdgeGPT-0.2.0/LICENSE` & `EdgeGPT-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.2.0/PKG-INFO` & `EdgeGPT-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.2.0
+Version: 0.2.1
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.2.0 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.2.1 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.2.0/README.md` & `EdgeGPT-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.2.0/setup.py` & `EdgeGPT-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.2.0",
+    version="0.2.1",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
@@ -30,15 +30,15 @@
     install_requires=[
         "httpx",
         "websockets",
         "rich",
         "certifi",
         "prompt_toolkit",
         "requests",
-        "BingImageCreator>=0.1.1.1",
+        "BingImageCreator>=0.1.2.1",
     ],
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["EdgeGPT", "ImageGen"],
     classifiers=[
         "License :: OSI Approved :: The Unlicense (Unlicense)",
         "Intended Audience :: Developers",
```

### Comparing `EdgeGPT-0.2.0/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.2.1/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.2.0
+Version: 0.2.1
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.2.0 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.2.1 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.2.0/src/EdgeGPT.py` & `EdgeGPT-0.2.1/src/EdgeGPT.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,26 +85,26 @@
     "x-forwarded-for": FORWARDED_IP,
 }
 
 ssl_context = ssl.create_default_context()
 ssl_context.load_verify_locations(certifi.where())
 
 
-class _NotAllowedToAccess(Exception):
+class NotAllowedToAccess(Exception):
     pass
 
 
-class _ConversationStyle(Enum):
+class ConversationStyle(Enum):
     creative = "h3imaginative,clgalileo,gencontentv3"
     balanced = "galileo"
     precise = "h3precise,clgalileo"
 
 
 CONVERSATION_STYLE_TYPE = Optional[
-    Union[_ConversationStyle, Literal["creative", "balanced", "precise"]]
+    Union[ConversationStyle, Literal["creative", "balanced", "precise"]]
 ]
 
 
 def _append_identifier(msg: dict) -> str:
     """
     Appends special character to end of message to identify end of message
     """
@@ -151,16 +151,16 @@
             options = [
                 "deepleo",
                 "enable_debug_commands",
                 "disable_emoji_spoken_text",
                 "enablemm",
             ]
         if conversation_style:
-            if not isinstance(conversation_style, _ConversationStyle):
-                conversation_style = getattr(_ConversationStyle, conversation_style)
+            if not isinstance(conversation_style, ConversationStyle):
+                conversation_style = getattr(ConversationStyle, conversation_style)
             options = [
                 "nlu_direct_response_filter",
                 "deepleo",
                 "disable_emoji_spoken_text",
                 "responsible_ai_policy_235",
                 "enablemm",
                 conversation_style.value,
@@ -248,20 +248,20 @@
         if response.status_code != 200:
             print(f"Status code: {response.status_code}")
             print(response.text)
             print(response.url)
             raise Exception("Authentication failed")
         try:
             self.struct = response.json()
-        except (json.decoder.JSONDecodeError, _NotAllowedToAccess) as exc:
+        except (json.decoder.JSONDecodeError, NotAllowedToAccess) as exc:
             raise Exception(
                 "Authentication failed. You have not been accepted into the beta.",
             ) from exc
         if self.struct["result"]["value"] == "UnauthorizedRequest":
-            raise _NotAllowedToAccess(self.struct["result"]["message"])
+            raise NotAllowedToAccess(self.struct["result"]["message"])
 
 
 class _ChatHub:
     """
     Chat API
     """
```

