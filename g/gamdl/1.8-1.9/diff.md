# Comparing `tmp/gamdl-1.8.tar.gz` & `tmp/gamdl-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-1.8.tar", last modified: Thu Apr  6 02:45:56 2023, max compression
+gzip compressed data, was "gamdl-1.9.tar", last modified: Thu Apr 20 01:50:40 2023, max compression
```

## Comparing `gamdl-1.8.tar` & `gamdl-1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1137 2023-04-06 02:45:46.980782 gamdl-1.8/.github/workflows/main.yml
--rw-r--r--   0        0        0       56 2023-04-06 02:45:46.980782 gamdl-1.8/.gitignore
--rw-r--r--   0        0        0     4041 2023-04-06 02:45:46.980782 gamdl-1.8/README.md
--rw-r--r--   0        0        0     7185 2023-04-06 02:45:46.980782 gamdl-1.8/gamdl/__init__.py
--rw-r--r--   0        0        0       58 2023-04-06 02:45:46.980782 gamdl-1.8/gamdl/__main__.py
--rw-r--r--   0        0        0    17639 2023-04-06 02:45:46.980782 gamdl-1.8/gamdl/gamdl.py
--rw-r--r--   0        0        0     2975 2023-04-06 02:45:46.980782 gamdl-1.8/gamdl/storefront_ids.py
--rw-r--r--   0        0        0      508 2023-04-06 02:45:46.980782 gamdl-1.8/pyproject.toml
--rw-r--r--   0        0        0       30 2023-04-06 02:45:46.980782 gamdl-1.8/requirements.txt
--rw-r--r--   0        0        0     4445 1970-01-01 00:00:00.000000 gamdl-1.8/PKG-INFO
+-rw-r--r--   0        0        0     1137 2023-04-20 01:50:35.698213 gamdl-1.9/.github/workflows/main.yml
+-rw-r--r--   0        0        0       56 2023-04-20 01:50:35.698213 gamdl-1.9/.gitignore
+-rw-r--r--   0        0        0     4041 2023-04-20 01:50:35.698213 gamdl-1.9/README.md
+-rw-r--r--   0        0        0     7185 2023-04-20 01:50:35.698213 gamdl-1.9/gamdl/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-20 01:50:35.698213 gamdl-1.9/gamdl/__main__.py
+-rw-r--r--   0        0        0    17627 2023-04-20 01:50:35.698213 gamdl-1.9/gamdl/gamdl.py
+-rw-r--r--   0        0        0     2975 2023-04-20 01:50:35.698213 gamdl-1.9/gamdl/storefront_ids.py
+-rw-r--r--   0        0        0      508 2023-04-20 01:50:35.698213 gamdl-1.9/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-04-20 01:50:35.698213 gamdl-1.9/requirements.txt
+-rw-r--r--   0        0        0     4445 1970-01-01 00:00:00.000000 gamdl-1.9/PKG-INFO
```

### Comparing `gamdl-1.8/.github/workflows/main.yml` & `gamdl-1.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-1.8/README.md` & `gamdl-1.9/README.md`

 * *Files identical despite different names*

### Comparing `gamdl-1.8/gamdl/__init__.py` & `gamdl-1.9/gamdl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import shutil
 import argparse
 import traceback
 from .gamdl import Gamdl
 
-__version__ = '1.8'
+__version__ = '1.9'
 
 
 def main():
     if not shutil.which('mp4decrypt'):
         raise Exception('mp4decrypt is not on PATH')
     if not shutil.which('MP4Box'):
         raise Exception('MP4Box is not on PATH')
```

### Comparing `gamdl-1.8/gamdl/gamdl.py` & `gamdl-1.9/gamdl/gamdl.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,16 @@
             'Connection': 'keep-alive',
             'Sec-Fetch-Dest': 'empty',
             'Sec-Fetch-Mode': 'cors',
             'Sec-Fetch-Site': 'same-site',
             'origin': 'https://beta.music.apple.com',
         })
         web_page = self.session.get('https://beta.music.apple.com').text
-        index_js_uri = re.search('(?<=index\.)(.*?)(?=\.js")', web_page).group(1)
-        index_js_page = self.session.get(f'https://beta.music.apple.com/assets/index.{index_js_uri}.js').text
+        index_js_uri = re.search(r"/assets/index-legacy-[^/]+\.js", web_page).group(0)
+        index_js_page = self.session.get(f'https://beta.music.apple.com{index_js_uri}').text
         token = re.search('(?=eyJh)(.*?)(?=")', index_js_page).group(1)
         self.session.headers.update({"authorization": f'Bearer {token}'})
         self.country = self.session.cookies.get_dict()['itua']
         self.storefront = getattr(gamdl.storefront_ids, self.country.upper())
     
 
     def get_download_queue(self, url):
```

### Comparing `gamdl-1.8/gamdl/storefront_ids.py` & `gamdl-1.9/gamdl/storefront_ids.py`

 * *Files identical despite different names*

### Comparing `gamdl-1.8/PKG-INFO` & `gamdl-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 1.8
+Version: 1.9
 Summary: Download Apple Music songs/music videos/albums/playlists
 Author: glomatico
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pywidevine
 Requires-Dist: pyyaml
 Requires-Dist: m3u8
```

