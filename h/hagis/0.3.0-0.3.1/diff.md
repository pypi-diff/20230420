# Comparing `tmp/hagis-0.3.0.tar.gz` & `tmp/hagis-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.3.0.tar", last modified: Wed Apr 19 12:51:07 2023, max compression
+gzip compressed data, was "hagis-0.3.1.tar", last modified: Thu Apr 20 00:35:24 2023, max compression
```

## Comparing `hagis-0.3.0.tar` & `hagis-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:51:07.625820 hagis-0.3.0/
--rw-rw-rw-   0        0        0      941 2023-04-19 12:51:07.617810 hagis-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 12:51:07.583418 hagis-0.3.0/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.3.0/hagis/__init__.py
--rw-rw-rw-   0        0        0    13034 2023-04-19 12:48:44.000000 hagis-0.3.0/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:51:07.609763 hagis-0.3.0/hagis.egg-info/
--rw-rw-rw-   0        0        0      941 2023-04-19 12:51:07.000000 hagis-0.3.0/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-19 12:51:07.000000 hagis-0.3.0/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:51:07.000000 hagis-0.3.0/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 12:51:07.000000 hagis-0.3.0/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-19 12:50:32.000000 hagis-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 12:51:07.625820 hagis-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 00:35:24.333327 hagis-0.3.1/
+-rw-rw-rw-   0        0        0      941 2023-04-20 00:35:24.328545 hagis-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 00:35:24.287274 hagis-0.3.1/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.3.1/hagis/__init__.py
+-rw-rw-rw-   0        0        0    13056 2023-04-20 00:34:48.000000 hagis-0.3.1/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-20 00:35:24.315546 hagis-0.3.1/hagis.egg-info/
+-rw-rw-rw-   0        0        0      941 2023-04-20 00:35:24.000000 hagis-0.3.1/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-20 00:35:24.000000 hagis-0.3.1/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 00:35:24.000000 hagis-0.3.1/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 00:35:24.000000 hagis-0.3.1/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-20 00:34:33.000000 hagis-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 00:35:24.333327 hagis-0.3.1/setup.cfg
```

### Comparing `hagis-0.3.0/PKG-INFO` & `hagis-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.3.0
+Version: 0.3.1
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.3.0/hagis/hagis.py` & `hagis-0.3.1/hagis/hagis.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,28 +114,31 @@
             where_clause (str, optional): Where clause.  Defaults to "1=1".
             record_count (Optional[int], optional): Maximum record count.  Defaults to None.
             wkid (Optional[int], optional): Spatial reference.  Defaults to None.
 
         Returns:
             Iterable[T]: Items.
         """
+        if record_count == 0:
+            return
+
         if self._is_dynamic:
             # If dynamic, request all fields.
             fields = "*"
         else:
             # Otherwise, request only what is used by the model.
             fields = ",".join([f for (_, f) in self._fields.items() if f != self._shape_property_name.lower()])
             if not self._shape_property_name:
                 kwargs["returnGeometry"] = False
 
-        if record_count is None:
-            keep_querying = False
-        else:
+        if record_count:
             keep_querying = True
-            kwargs["resultRecordCount"] = record_count if record_count else 1
+            kwargs["resultRecordCount"] = record_count
+        else:
+            keep_querying = False
 
         if wkid:
             kwargs["outSR"] = wkid
 
         for row in islice(self._query(where_clause, fields, keep_querying, **kwargs), record_count):
             if self._is_dynamic:
                 yield row  # type: ignore
```

### Comparing `hagis-0.3.0/hagis.egg-info/PKG-INFO` & `hagis-0.3.1/hagis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.3.0
+Version: 0.3.1
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.3.0/pyproject.toml` & `hagis-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

