# Comparing `tmp/ma-nish-0.8.0.tar.gz` & `tmp/ma-nish-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ma-nish-0.8.0.tar", last modified: Wed Apr 19 21:26:56 2023, max compression
+gzip compressed data, was "ma-nish-0.9.0.tar", last modified: Thu Apr 20 08:33:44 2023, max compression
```

## Comparing `ma-nish-0.8.0.tar` & `ma-nish-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:26:56.735392 ma-nish-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-19 21:26:44.000000 ma-nish-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-04-19 21:26:56.735392 ma-nish-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-04-19 21:26:44.000000 ma-nish-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:26:56.735392 ma-nish-0.8.0/ma_nish.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-04-19 21:26:56.000000 ma-nish-0.8.0/ma_nish.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-19 21:26:56.000000 ma-nish-0.8.0/ma_nish.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:26:56.000000 ma-nish-0.8.0/ma_nish.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 21:26:56.000000 ma-nish-0.8.0/ma_nish.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 21:26:56.000000 ma-nish-0.8.0/ma_nish.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:26:56.735392 ma-nish-0.8.0/manish/
--rw-r--r--   0 runner    (1001) docker     (123)    38717 2023-04-19 21:26:44.000000 ma-nish-0.8.0/manish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-19 21:26:44.000000 ma-nish-0.8.0/manish/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-19 21:26:44.000000 ma-nish-0.8.0/manish/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-19 21:26:44.000000 ma-nish-0.8.0/manish/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-19 21:26:44.000000 ma-nish-0.8.0/manish/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-19 21:26:44.000000 ma-nish-0.8.0/manish/template.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 21:26:56.735392 ma-nish-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-19 21:26:44.000000 ma-nish-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:33:44.719652 ma-nish-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 08:33:33.000000 ma-nish-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-04-20 08:33:44.719652 ma-nish-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-04-20 08:33:33.000000 ma-nish-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:33:44.715652 ma-nish-0.9.0/ma_nish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-04-20 08:33:44.000000 ma-nish-0.9.0/ma_nish.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-20 08:33:44.000000 ma-nish-0.9.0/ma_nish.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 08:33:44.000000 ma-nish-0.9.0/ma_nish.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-20 08:33:44.000000 ma-nish-0.9.0/ma_nish.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 08:33:44.000000 ma-nish-0.9.0/ma_nish.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:33:44.715652 ma-nish-0.9.0/manish/
+-rw-r--r--   0 runner    (1001) docker     (123)    38987 2023-04-20 08:33:33.000000 ma-nish-0.9.0/manish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-20 08:33:33.000000 ma-nish-0.9.0/manish/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-20 08:33:33.000000 ma-nish-0.9.0/manish/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-20 08:33:33.000000 ma-nish-0.9.0/manish/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-20 08:33:33.000000 ma-nish-0.9.0/manish/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-20 08:33:33.000000 ma-nish-0.9.0/manish/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 08:33:44.719652 ma-nish-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-20 08:33:33.000000 ma-nish-0.9.0/setup.py
```

### Comparing `ma-nish-0.8.0/LICENSE` & `ma-nish-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ma-nish-0.8.0/PKG-INFO` & `ma-nish-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma-nish
-Version: 0.8.0
+Version: 0.9.0
 Summary: manish is an unofficial python wrapper for Whatsapp cloud api
 Home-page: https://github.com/t0mer/ma-nish
 Download-URL: https://pypi.org/project/ma-nish/
 Author: Tomer Klein
 Author-email: tomer.klein@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/t0mer/ma-nish
```

### Comparing `ma-nish-0.8.0/README.md` & `ma-nish-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ma-nish-0.8.0/ma_nish.egg-info/PKG-INFO` & `ma-nish-0.9.0/ma_nish.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma-nish
-Version: 0.8.0
+Version: 0.9.0
 Summary: manish is an unofficial python wrapper for Whatsapp cloud api
 Home-page: https://github.com/t0mer/ma-nish
 Download-URL: https://pypi.org/project/ma-nish/
 Author: Tomer Klein
 Author-email: tomer.klein@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/t0mer/ma-nish
```

### Comparing `ma-nish-0.8.0/manish/__init__.py` & `ma-nish-0.9.0/manish/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -607,15 +607,15 @@
             logger.info(f"Status code: {r.status_code}")
             logger.info(f"Response: {r.json()}")
             return None
         except Exception as e:
             logger.error("aw snap something went wrong: " + str(e))
             return '{"error":"' + str(e)  + '"}'
 
-    def download_media(self, media_url: str, mime_type: str, file_path: str = "temp"):
+    def download_media(self, media_url: str, mime_type: str, file_path: str = ""):
         """
         Download media from media url obtained either by manually uploading media or received media
         Args:
             media_url[str]: Media url of the media
             mime_type[str]: Mime type of the media
             file_path[str]: Path of the file to be downloaded to. Default is "temp"
                             Do not include the file extension. It will be added automatically.
@@ -627,17 +627,22 @@
             >>> manish.download_media("media_url", "image/jpeg")
             >>> manish.download_media("media_url", "video/mp4", "path/to/file") #do not include the file extension
         """
         try:
             r = requests.get(media_url, headers=self.headers)
             content = r.content
             extension = mime_type.split("/")[1]
+            if ";" in extension:
+                extension = extension.split(";")[0]
             # create a temporary file
             try:
-
+                if file_path == "":
+                    save_file_here = f"/tmp/temp.{extension}"
+                else:
+                    save_file_here = f"{file_path}/temp.{extension}"
                 save_file_here = (
                     f"{file_path}.{extension}" if file_path else f"temp.{extension}"
                 )
                 with open(save_file_here, "wb") as f:
                     f.write(content)
                 logger.info(f"Media downloaded to {save_file_here}")
                 return f.name
@@ -645,14 +650,15 @@
                 print(e)
                 logger.info(f"Error downloading media to {save_file_here}")
                 return None
         except Exception as e:
             logger.error("aw snap something went wrong: " + str(e))
             return '{"error":"' + str(e)  + '"}'
 
+
     def get_name(self, data):
         """
         Extracts the name of the sender from the data received from the webhook.
         Args:
             data[dict]: The data received from the webhook
         Returns:
             str: The name of the sender
```

### Comparing `ma-nish-0.8.0/manish/button.py` & `ma-nish-0.9.0/manish/button.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.8.0/manish/contact.py` & `ma-nish-0.9.0/manish/contact.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.8.0/manish/helpers.py` & `ma-nish-0.9.0/manish/helpers.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.8.0/manish/location.py` & `ma-nish-0.9.0/manish/location.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.8.0/manish/template.py` & `ma-nish-0.9.0/manish/template.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.8.0/setup.py` & `ma-nish-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r", encoding="UTF-8") as f:
      readme = f.read()
 
 
 setup_args = dict(
     name='ma-nish',
-    version='0.8.0',
+    version='0.9.0',
     description='manish is an unofficial python wrapper for Whatsapp cloud api',
     long_description_content_type="text/markdown",
     long_description=readme,
     license='MIT',
     packages=find_packages(),
     author='Tomer Klein',
     author_email='tomer.klein@gmail.com',
```

