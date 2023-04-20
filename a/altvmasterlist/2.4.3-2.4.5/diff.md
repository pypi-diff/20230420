# Comparing `tmp/altvmasterlist-2.4.3.tar.gz` & `tmp/altvmasterlist-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altvmasterlist-2.4.3.tar", max compression
+gzip compressed data, was "altvmasterlist-2.4.5.tar", max compression
```

## Comparing `altvmasterlist-2.4.3.tar` & `altvmasterlist-2.4.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    16725 2023-04-13 13:23:07.300956 altvmasterlist-2.4.3/LICENSE
--rw-r--r--   0        0        0      425 2023-04-13 13:23:07.300956 altvmasterlist-2.4.3/README.md
--rw-r--r--   0        0        0     1052 2023-04-13 13:23:07.300956 altvmasterlist-2.4.3/pyproject.toml
--rw-r--r--   0        0        0      402 2023-04-13 13:23:07.300956 altvmasterlist-2.4.3/src/altvmasterlist/__init__.py
--rw-r--r--   0        0        0     6982 2023-04-13 13:23:07.300956 altvmasterlist-2.4.3/src/altvmasterlist/altstats.py
--rw-r--r--   0        0        0     8327 2023-04-13 13:23:07.300956 altvmasterlist-2.4.3/src/altvmasterlist/masterlist.py
--rw-r--r--   0        0        0    10238 2023-04-13 13:23:07.304956 altvmasterlist-2.4.3/src/altvmasterlist/shared.py
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 altvmasterlist-2.4.3/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-04-20 11:21:43.722667 altvmasterlist-2.4.5/LICENSE
+-rw-r--r--   0        0        0      425 2023-04-20 11:21:43.722667 altvmasterlist-2.4.5/README.md
+-rw-r--r--   0        0        0     1053 2023-04-20 11:21:43.722667 altvmasterlist-2.4.5/pyproject.toml
+-rw-r--r--   0        0        0      402 2023-04-20 11:21:43.722667 altvmasterlist-2.4.5/src/altvmasterlist/__init__.py
+-rw-r--r--   0        0        0     6982 2023-04-20 11:21:43.722667 altvmasterlist-2.4.5/src/altvmasterlist/altstats.py
+-rw-r--r--   0        0        0     9681 2023-04-20 11:21:43.722667 altvmasterlist-2.4.5/src/altvmasterlist/masterlist.py
+-rw-r--r--   0        0        0    10516 2023-04-20 11:21:43.722667 altvmasterlist-2.4.5/src/altvmasterlist/shared.py
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 altvmasterlist-2.4.5/PKG-INFO
```

### Comparing `altvmasterlist-2.4.3/LICENSE` & `altvmasterlist-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `altvmasterlist-2.4.3/pyproject.toml` & `altvmasterlist-2.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "altvmasterlist"
-version = "2.4.3"
+version = "2.4.5"
 description = "A package to use the alt:V Masterlist api."
 authors = ["Nickwasused <contact.nickwasused.fa6c8@simplelogin.co>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository = "https://github.com/Nickwasused/altv-python-masterlist"
 documentation = "https://nickwasused.github.io/altv-python-masterlist/"
 classifiers = [
@@ -27,8 +27,8 @@
 
 [build-system]
 requires = ["poetry-core>=1.3.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Nickwasused/altv-python-masterlist/issues"
-"Documentation" = "https://nickwasused.github.io/altv-python-masterlist/"
+"Documentation" = "https://nickwasused.github.io/altv-python-masterlist/"
```

### Comparing `altvmasterlist-2.4.3/src/altvmasterlist/altstats.py` & `altvmasterlist-2.4.5/src/altvmasterlist/altstats.py`

 * *Files identical despite different names*

### Comparing `altvmasterlist-2.4.3/src/altvmasterlist/masterlist.py` & `altvmasterlist-2.4.5/src/altvmasterlist/masterlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -215,10 +215,60 @@
     result = regex.match(server_id)
     if result is not None:
         return True
     else:
         return False
 
 
+def get_launcher_skins() -> dict | None:
+    """Get a list of all available launcher skins.
+
+    Returns:
+        json: A json array of all launcher skins.
+
+    The elements have the following keys: serverId, xxHash64 and fileName.
+    """
+    skins = shared.request(shared.MasterlistUrls.launcher_skins)
+
+    if skins is None or skins == "{}":
+        return None
+    else:
+        return skins["indexEntries"]
+
+
+def get_launcher_skin(filename: str) -> dict | None:
+    """Get a specific launcher skin by filename
+
+    Args:
+        filename (str): filename of the launcher skin
+
+    Returns:
+        json: Object
+
+    The json object has the following keys:
+        - name: the name of the server
+        - id: the server id
+        - rss: the custom rss feed of the server
+        - primaryColor: the custom color of the server
+        - servers (array): list of servers
+            - name: server name
+            - url: direct connect url
+            - id: server id
+            - imageSplash64: base64 splash image
+            - imageLogo64: base64 Logo
+            - imageBackground64: base64 background image
+
+    """
+    if not filename or filename == "":
+        return None
+
+    skin = shared.request(shared.MasterlistUrls.launcher_file.format(filename))
+
+    if skin is None or skin == {}:
+        return None
+    else:
+        return skin
+
+
 if __name__ == "__main__":
     print("This is a Module!")
     sys.exit()
```

### Comparing `altvmasterlist-2.4.3/src/altvmasterlist/shared.py` & `altvmasterlist-2.4.5/src/altvmasterlist/shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 logging.getLogger().setLevel(logging.INFO)
 
 
 @dataclass
 class MasterlistUrls:
     """This class is used for the masterlist submodule. It provides all urls needed."""
     base_link: str = "https://api.alt-mp.com"
+    base_cdn: str = "https://cdn.alt-mp.com"
     all_server_stats_link: str = f"{base_link}/servers"
     all_servers_link: str = f"{base_link}/servers/list"
     server_link: str = f"{base_link}/server" + "/{}"
     server_average_link: str = f"{base_link}/avg" + "/{}/{}"
     server_max_link: str = f"{base_link}/max" + "/{}/{}"
+    launcher_skins: str = f"{base_cdn}/launcher-skins/index.json"
+    launcher_file: str = f"{base_cdn}/launcher-skins/files/" + "{}"
 
 
 @dataclass
 class AltstatsUrls:
     """This class is used for the altstats submodule. It provides all urls needed."""
     base_link: str = "https://api.altstats.net/api/v1/"
     all_server_stats_link: str = f"{base_link}/master"
@@ -276,13 +279,14 @@
         float: The size of the resource.
     """
     if use_cdn:
         resource_url = f"{cdn_url}/{resource}.resource"
     else:
         resource_url = f"http://{host}:{port}/{resource}.resource"
 
-    data = requests.head(resource_url, headers={"User-Agent": "AltPublicAgent"}, timeout=60)
+    size_request = Request(resource_url, headers={"User-Agent": "AltPublicAgent"}, method="HEAD")
 
-    if data.ok:
-        return round((int(data.headers["Content-Length"]) / 1048576), decimal)
-    else:
-        return None
+    with urlopen(size_request, timeout=60) as size_data:
+        if size_data.status == 200:
+            return round((int(size_data.headers["Content-Length"]) / 1048576), decimal)
+        else:
+            return None
```

### Comparing `altvmasterlist-2.4.3/PKG-INFO` & `altvmasterlist-2.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altvmasterlist
-Version: 2.4.3
+Version: 2.4.5
 Summary: A package to use the alt:V Masterlist api.
 Home-page: https://github.com/Nickwasused/altv-python-masterlist
 License: MPL-2.0
 Author: Nickwasused
 Author-email: contact.nickwasused.fa6c8@simplelogin.co
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved
```

