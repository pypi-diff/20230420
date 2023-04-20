# Comparing `tmp/mongoclass-1.3.tar.gz` & `tmp/mongoclass-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongoclass-1.3.tar", last modified: Thu Apr 20 04:05:05 2023, max compression
+gzip compressed data, was "mongoclass-1.4.tar", last modified: Thu Apr 20 07:44:18 2023, max compression
```

## Comparing `mongoclass-1.3.tar` & `mongoclass-1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 04:05:05.221066 mongoclass-1.3/
--rw-rw-rw-   0        0        0     1093 2022-10-28 01:48:28.000000 mongoclass-1.3/LICENSE
--rw-rw-rw-   0        0        0     3408 2023-04-20 04:05:05.222067 mongoclass-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2973 2022-10-28 01:48:28.000000 mongoclass-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 04:05:05.198055 mongoclass-1.3/mongoclass/
--rw-rw-rw-   0        0        0       58 2022-10-28 01:48:28.000000 mongoclass-1.3/mongoclass/__init__.py
--rw-rw-rw-   0        0        0     5420 2023-04-18 14:44:13.000000 mongoclass-1.3/mongoclass/cache.py
--rw-rw-rw-   0        0        0    24954 2023-04-20 04:04:18.000000 mongoclass-1.3/mongoclass/client.py
--rw-rw-rw-   0        0        0     2015 2022-10-28 01:48:58.000000 mongoclass-1.3/mongoclass/cursor.py
-drwxrwxrwx   0        0        0        0 2023-04-20 04:05:05.219065 mongoclass-1.3/mongoclass.egg-info/
--rw-rw-rw-   0        0        0     3408 2023-04-20 04:05:05.000000 mongoclass-1.3/mongoclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-04-20 04:05:05.000000 mongoclass-1.3/mongoclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 04:05:05.000000 mongoclass-1.3/mongoclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-20 04:05:05.000000 mongoclass-1.3/mongoclass.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 04:05:05.000000 mongoclass-1.3/mongoclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-20 04:05:05.223059 mongoclass-1.3/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-04-20 04:04:46.000000 mongoclass-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 07:44:18.079955 mongoclass-1.4/
+-rw-rw-rw-   0        0        0     1093 2022-10-28 01:48:28.000000 mongoclass-1.4/LICENSE
+-rw-rw-rw-   0        0        0     3408 2023-04-20 07:44:18.080953 mongoclass-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2973 2022-10-28 01:48:28.000000 mongoclass-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 07:44:18.045956 mongoclass-1.4/mongoclass/
+-rw-rw-rw-   0        0        0       58 2022-10-28 01:48:28.000000 mongoclass-1.4/mongoclass/__init__.py
+-rw-rw-rw-   0        0        0     5420 2023-04-18 14:44:13.000000 mongoclass-1.4/mongoclass/cache.py
+-rw-rw-rw-   0        0        0    25900 2023-04-20 07:43:12.000000 mongoclass-1.4/mongoclass/client.py
+-rw-rw-rw-   0        0        0     2015 2022-10-28 01:48:58.000000 mongoclass-1.4/mongoclass/cursor.py
+drwxrwxrwx   0        0        0        0 2023-04-20 07:44:18.078954 mongoclass-1.4/mongoclass.egg-info/
+-rw-rw-rw-   0        0        0     3408 2023-04-20 07:44:17.000000 mongoclass-1.4/mongoclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-04-20 07:44:17.000000 mongoclass-1.4/mongoclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 07:44:17.000000 mongoclass-1.4/mongoclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-20 07:44:17.000000 mongoclass-1.4/mongoclass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 07:44:17.000000 mongoclass-1.4/mongoclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-20 07:44:18.082957 mongoclass-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-04-20 07:43:42.000000 mongoclass-1.4/setup.py
```

### Comparing `mongoclass-1.3/LICENSE` & `mongoclass-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mongoclass-1.3/PKG-INFO` & `mongoclass-1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mongoclass
-Version: 1.3
+Version: 1.4
 Summary: A basic ORM like interface for mongodb in python that uses dataclasses.
 Home-page: https://github.com/bossauh/mongoclass
-Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_13.tar.gz
+Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_14.tar.gz
 Author: Philippe Mathew
 Author-email: philmattdev@gmail.com
 License: MIT
 Keywords: pymongo,orm
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mongoclass-1.3/README.md` & `mongoclass-1.4/README.md`

 * *Files identical despite different names*

### Comparing `mongoclass-1.3/mongoclass/cache.py` & `mongoclass-1.4/mongoclass/cache.py`

 * *Files identical despite different names*

### Comparing `mongoclass-1.3/mongoclass/client.py` & `mongoclass-1.4/mongoclass/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,14 +375,40 @@
                             self.map_document,
                             collection_name,
                             db.name,
                             self._engine_used,
                         )
 
                     @staticmethod
+                    def paginate(
+                        *args,
+                        database: Optional[
+                            Union[
+                                str,
+                                pymongo.database.Database,
+                                mongita.database.Database,
+                            ]
+                        ] = None,
+                        page: int,
+                        size: int,
+                        **kwargs,
+                    ) -> Cursor:
+                        skip = (page - 1) * size
+
+                        results = (
+                            self.find_classes(
+                                collection_name, *args, database, **kwargs
+                            )
+                            .skip(skip)
+                            .limit(size)
+                        )
+
+                        return results
+
+                    @staticmethod
                     def find_classes(
                         *args,
                         database: Optional[
                             Union[
                                 str,
                                 pymongo.database.Database,
                                 mongita.database.Database,
```

### Comparing `mongoclass-1.3/mongoclass/cursor.py` & `mongoclass-1.4/mongoclass/cursor.py`

 * *Files identical despite different names*

### Comparing `mongoclass-1.3/mongoclass.egg-info/PKG-INFO` & `mongoclass-1.4/mongoclass.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mongoclass
-Version: 1.3
+Version: 1.4
 Summary: A basic ORM like interface for mongodb in python that uses dataclasses.
 Home-page: https://github.com/bossauh/mongoclass
-Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_13.tar.gz
+Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_14.tar.gz
 Author: Philippe Mathew
 Author-email: philmattdev@gmail.com
 License: MIT
 Keywords: pymongo,orm
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mongoclass-1.3/setup.py` & `mongoclass-1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 install_requires = ["dnspython==2.2.1", "mongita==1.1.1"]
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="mongoclass",
     packages=["mongoclass"],
-    version="1.3",
+    version="1.4",
     license="MIT",
     description="A basic ORM like interface for mongodb in python that uses dataclasses.",
     author="Philippe Mathew",
     author_email="philmattdev@gmail.com",
     url="https://github.com/bossauh/mongoclass",
-    download_url="https://github.com/bossauh/mongoclass/archive/refs/tags/v_13.tar.gz",
+    download_url="https://github.com/bossauh/mongoclass/archive/refs/tags/v_14.tar.gz",
     keywords=["pymongo", "orm"],
     install_requires=install_requires,
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

