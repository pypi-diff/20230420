# Comparing `tmp/rssfixer-0.0.5.tar.gz` & `tmp/rssfixer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssfixer-0.0.5.tar", last modified: Thu Apr 20 06:40:54 2023, max compression
+gzip compressed data, was "rssfixer-0.0.6.tar", last modified: Thu Apr 20 09:39:31 2023, max compression
```

## Comparing `rssfixer-0.0.5.tar` & `rssfixer-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 06:40:54.906153 rssfixer-0.0.5/
--rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-17 09:42:15.000000 rssfixer-0.0.5/LICENSE
--rw-r--r--   0 reuteras   (501) staff       (20)     4627 2023-04-20 06:40:54.906033 rssfixer-0.0.5/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)     4084 2023-04-20 06:30:06.000000 rssfixer-0.0.5/README.md
--rw-r--r--   0 reuteras   (501) staff       (20)      813 2023-04-19 11:00:15.000000 rssfixer-0.0.5/pyproject.toml
--rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-20 06:40:54.906196 rssfixer-0.0.5/setup.cfg
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 06:40:54.903735 rssfixer-0.0.5/src/
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 06:40:54.904843 rssfixer-0.0.5/src/rssfixer/
--rw-r--r--   0 reuteras   (501) staff       (20)       61 2023-04-18 04:00:23.000000 rssfixer-0.0.5/src/rssfixer/__init__.py
--rw-r--r--   0 reuteras   (501) staff       (20)     8946 2023-04-20 06:29:30.000000 rssfixer-0.0.5/src/rssfixer/rss.py
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 06:40:54.905617 rssfixer-0.0.5/src/rssfixer.egg-info/
--rw-r--r--   0 reuteras   (501) staff       (20)     4627 2023-04-20 06:40:54.000000 rssfixer-0.0.5/src/rssfixer.egg-info/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)      317 2023-04-20 06:40:54.000000 rssfixer-0.0.5/src/rssfixer.egg-info/SOURCES.txt
--rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-20 06:40:54.000000 rssfixer-0.0.5/src/rssfixer.egg-info/dependency_links.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-20 06:40:54.000000 rssfixer-0.0.5/src/rssfixer.egg-info/entry_points.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       65 2023-04-20 06:40:54.000000 rssfixer-0.0.5/src/rssfixer.egg-info/requires.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-20 06:40:54.000000 rssfixer-0.0.5/src/rssfixer.egg-info/top_level.txt
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 06:40:54.905735 rssfixer-0.0.5/src/tests/
--rw-r--r--   0 reuteras   (501) staff       (20)     2341 2023-04-18 10:59:41.000000 rssfixer-0.0.5/src/tests/test_rss.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 09:39:31.081700 rssfixer-0.0.6/
+-rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-17 09:42:15.000000 rssfixer-0.0.6/LICENSE
+-rw-r--r--   0 reuteras   (501) staff       (20)     4627 2023-04-20 09:39:31.081572 rssfixer-0.0.6/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)     4084 2023-04-20 06:30:06.000000 rssfixer-0.0.6/README.md
+-rw-r--r--   0 reuteras   (501) staff       (20)      813 2023-04-20 09:37:42.000000 rssfixer-0.0.6/pyproject.toml
+-rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-20 09:39:31.081744 rssfixer-0.0.6/setup.cfg
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 09:39:31.079666 rssfixer-0.0.6/src/
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 09:39:31.080521 rssfixer-0.0.6/src/rssfixer/
+-rw-r--r--   0 reuteras   (501) staff       (20)       61 2023-04-18 04:00:23.000000 rssfixer-0.0.6/src/rssfixer/__init__.py
+-rw-r--r--   0 reuteras   (501) staff       (20)     8882 2023-04-20 09:37:26.000000 rssfixer-0.0.6/src/rssfixer/rss.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 09:39:31.081283 rssfixer-0.0.6/src/rssfixer.egg-info/
+-rw-r--r--   0 reuteras   (501) staff       (20)     4627 2023-04-20 09:39:31.000000 rssfixer-0.0.6/src/rssfixer.egg-info/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)      317 2023-04-20 09:39:31.000000 rssfixer-0.0.6/src/rssfixer.egg-info/SOURCES.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-20 09:39:31.000000 rssfixer-0.0.6/src/rssfixer.egg-info/dependency_links.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-20 09:39:31.000000 rssfixer-0.0.6/src/rssfixer.egg-info/entry_points.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       65 2023-04-20 09:39:31.000000 rssfixer-0.0.6/src/rssfixer.egg-info/requires.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-20 09:39:31.000000 rssfixer-0.0.6/src/rssfixer.egg-info/top_level.txt
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 09:39:31.081411 rssfixer-0.0.6/src/tests/
+-rw-r--r--   0 reuteras   (501) staff       (20)     2341 2023-04-18 10:59:41.000000 rssfixer-0.0.6/src/tests/test_rss.py
```

### Comparing `rssfixer-0.0.5/LICENSE` & `rssfixer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rssfixer-0.0.5/PKG-INFO` & `rssfixer-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rssfixer-0.0.5/README.md` & `rssfixer-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rssfixer-0.0.5/pyproject.toml` & `rssfixer-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rssfixer"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Peter Reuterås", email="peter@reuteras.net" },
 ]
 description = "Generate RSS feed for Wordpress blog without it."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `rssfixer-0.0.5/src/rssfixer/rss.py` & `rssfixer-0.0.6/src/rssfixer/rss.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,30 +105,30 @@
     # Find the JSON string in the page
     for json_text in soup.find_all("script", type="application/json"):
         json_object = json.loads(json_text.text)
         entries = find_entries(json_object, arguments.json_entries)
         if entries is not None:
             break
 
-        # Extract the links from the JSON object
-        for entry in entries:
-            try:
-                url = entry[arguments.json_url]
-                title = entry[arguments.json_title]
-            except KeyError:
-                print("ERROR: Unable to find URL or title in JSON object")
-                sys.exit(1)
-            try:
-                description = entry[arguments.json_description]
-            except KeyError:
-                # Ignore description if it's not found
-                description = ""
-            if url not in unique_links:
-                unique_links.add(url)
-                links.append((url, title, description))
+    # Extract the links from the JSON object
+    for entry in entries:
+        try:
+            url = entry[arguments.json_url]
+            title = entry[arguments.json_title]
+        except KeyError:
+            print("ERROR: Unable to find URL or title in JSON object")
+            sys.exit(1)
+        try:
+            description = entry[arguments.json_description]
+        except KeyError:
+            # Ignore description if it's not found
+            description = ""
+        if url not in unique_links:
+            unique_links.add(url)
+            links.append((url, title, description))
 
     if links == []:
         print("ERROR: No links found")
         sys.exit(1)
     return links
```

### Comparing `rssfixer-0.0.5/src/rssfixer.egg-info/PKG-INFO` & `rssfixer-0.0.6/src/rssfixer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rssfixer-0.0.5/src/tests/test_rss.py` & `rssfixer-0.0.6/src/tests/test_rss.py`

 * *Files identical despite different names*

