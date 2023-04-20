# Comparing `tmp/mongoclass-1.2.tar.gz` & `tmp/mongoclass-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongoclass-1.2.tar", last modified: Tue Apr 18 14:45:01 2023, max compression
+gzip compressed data, was "mongoclass-1.3.tar", last modified: Thu Apr 20 04:05:05 2023, max compression
```

## Comparing `mongoclass-1.2.tar` & `mongoclass-1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 14:45:01.541619 mongoclass-1.2/
--rw-rw-rw-   0        0        0     1093 2022-10-28 01:48:28.000000 mongoclass-1.2/LICENSE
--rw-rw-rw-   0        0        0     3408 2023-04-18 14:45:01.542616 mongoclass-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2973 2022-10-28 01:48:28.000000 mongoclass-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 14:45:01.501618 mongoclass-1.2/mongoclass/
--rw-rw-rw-   0        0        0       58 2022-10-28 01:48:28.000000 mongoclass-1.2/mongoclass/__init__.py
--rw-rw-rw-   0        0        0     5420 2023-04-18 14:44:13.000000 mongoclass-1.2/mongoclass/cache.py
--rw-rw-rw-   0        0        0    24024 2023-04-18 14:44:13.000000 mongoclass-1.2/mongoclass/client.py
--rw-rw-rw-   0        0        0     2015 2022-10-28 01:48:58.000000 mongoclass-1.2/mongoclass/cursor.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:45:01.539616 mongoclass-1.2/mongoclass.egg-info/
--rw-rw-rw-   0        0        0     3408 2023-04-18 14:45:01.000000 mongoclass-1.2/mongoclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-04-18 14:45:01.000000 mongoclass-1.2/mongoclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 14:45:01.000000 mongoclass-1.2/mongoclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-18 14:45:01.000000 mongoclass-1.2/mongoclass.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-18 14:45:01.000000 mongoclass-1.2/mongoclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-18 14:45:01.550619 mongoclass-1.2/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-04-18 14:44:29.000000 mongoclass-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 04:05:05.221066 mongoclass-1.3/
+-rw-rw-rw-   0        0        0     1093 2022-10-28 01:48:28.000000 mongoclass-1.3/LICENSE
+-rw-rw-rw-   0        0        0     3408 2023-04-20 04:05:05.222067 mongoclass-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2973 2022-10-28 01:48:28.000000 mongoclass-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 04:05:05.198055 mongoclass-1.3/mongoclass/
+-rw-rw-rw-   0        0        0       58 2022-10-28 01:48:28.000000 mongoclass-1.3/mongoclass/__init__.py
+-rw-rw-rw-   0        0        0     5420 2023-04-18 14:44:13.000000 mongoclass-1.3/mongoclass/cache.py
+-rw-rw-rw-   0        0        0    24954 2023-04-20 04:04:18.000000 mongoclass-1.3/mongoclass/client.py
+-rw-rw-rw-   0        0        0     2015 2022-10-28 01:48:58.000000 mongoclass-1.3/mongoclass/cursor.py
+drwxrwxrwx   0        0        0        0 2023-04-20 04:05:05.219065 mongoclass-1.3/mongoclass.egg-info/
+-rw-rw-rw-   0        0        0     3408 2023-04-20 04:05:05.000000 mongoclass-1.3/mongoclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-04-20 04:05:05.000000 mongoclass-1.3/mongoclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 04:05:05.000000 mongoclass-1.3/mongoclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-20 04:05:05.000000 mongoclass-1.3/mongoclass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 04:05:05.000000 mongoclass-1.3/mongoclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-20 04:05:05.223059 mongoclass-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-04-20 04:04:46.000000 mongoclass-1.3/setup.py
```

### Comparing `mongoclass-1.2/LICENSE` & `mongoclass-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mongoclass-1.2/PKG-INFO` & `mongoclass-1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mongoclass
-Version: 1.2
+Version: 1.3
 Summary: A basic ORM like interface for mongodb in python that uses dataclasses.
 Home-page: https://github.com/bossauh/mongoclass
-Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_12.tar.gz
+Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_13.tar.gz
 Author: Philippe Mathew
 Author-email: philmattdev@gmail.com
 License: MIT
 Keywords: pymongo,orm
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mongoclass-1.2/README.md` & `mongoclass-1.3/README.md`

 * *Files identical despite different names*

### Comparing `mongoclass-1.2/mongoclass/cache.py` & `mongoclass-1.3/mongoclass/cache.py`

 * *Files identical despite different names*

### Comparing `mongoclass-1.2/mongoclass/client.py` & `mongoclass-1.3/mongoclass/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from mongita import MongitaClientDisk, MongitaClientMemory
 from pymongo import MongoClient
 
 from .cursor import Cursor
 
 
 def client_constructor(engine: str, *args, **kwargs):
-
     if engine == "pymongo":
         Engine = MongoClient
     elif engine == "mongita_disk":
         Engine = MongitaClientDisk
     elif engine == "mongita_memory":
         Engine = MongitaClientMemory
     else:
@@ -47,23 +46,24 @@
 
         def __choose_database(
             self,
             database: Optional[
                 Union[str, pymongo.database.Database, mongita.database.Database]
             ] = None,
         ) -> Union[pymongo.database.Database, mongita.database.Database]:
-
             if database is None:
                 return self.default_database
             if isinstance(
                 database, (pymongo.database.Database, mongita.database.Database)
             ):
                 return database
             return self[database]
 
+        choose_database = __choose_database
+
         def get_db(
             self, database: str
         ) -> Union[pymongo.database.Database, mongita.database.Database]:
             """
             Get a database. Equivalent to `client["database"]`. This method exists simply because type hinting seems to be broken, nothing more.
 
             Parameters
@@ -127,15 +127,14 @@
         def mongoclass(
             self,
             collection: Optional[str] = None,
             database: Optional[Union[str, pymongo.database.Database]] = None,
             insert_on_init: bool = False,
             nested: bool = False,
         ) -> Callable:
-
             """
             A decorator used to map a dataclass onto a collection.
             In other words, it converts the dataclass onto a mongoclass.
 
             Parameters
             ----------
             `collection` : str
@@ -149,26 +148,23 @@
             `nested` : bool
                 Whether this mongoclass has other mongoclasses inside it. Nesting is not automatically determined for performance purposes. Defaults to False.
 
             """
             db = self.__choose_database(database)
 
             def wrapper(cls):
-
                 collection_name = collection or cls.__name__.lower()
 
                 @functools.wraps(cls, updated=())
                 class Inner(cls):
-
                     COLLECTION_NAME = collection_name
                     DATABASE_NAME = db.name
 
                     # pylint:disable=no-self-argument
                     def __init__(this, *args, **kwargs) -> None:
-
                         # MongodDB Attributes
                         this._mongodb_collection = collection_name
                         this._mongodb_db = db
                         this._mongodb_id = kwargs.pop("_mongodb_id", None)
 
                         _insert = kwargs.pop("_insert", insert_on_init)
                         super().__init__(*args, **kwargs)
@@ -178,15 +174,14 @@
                             this.insert()
 
                     def insert(
                         this, *args, **kwargs
                     ) -> Union[
                         pymongo.results.InsertOneResult, mongita.results.InsertOneResult
                     ]:
-
                         """
                         Insert this mongoclass as a document in the collection.
 
                         Parameters
                         ----------
                         `*args, **kwargs` :
                             Other parameters to be passed onto `Database.insert_one`
@@ -206,15 +201,14 @@
                         this, operation: dict, *args, **kwargs
                     ) -> Tuple[
                         Union[
                             pymongo.results.UpdateResult, mongita.results.UpdateResult
                         ],
                         object,
                     ]:
-
                         """
                         Update this mongoclass document in the collection.
 
                         Parameters
                         ----------
                         `operation` : dict
                             The operation to be made.
@@ -358,14 +352,37 @@
                         """
 
                         return self.find_class(
                             collection_name, *args, database, **kwargs
                         )
 
                     @staticmethod
+                    def aggregate(
+                        *args,
+                        database: Optional[
+                            Union[
+                                str,
+                                pymongo.database.Database,
+                                mongita.database.Database,
+                            ]
+                        ] = None,
+                        **kwargs,
+                    ) -> Cursor:
+                        db = self.choose_database(database)
+                        query = db[collection_name].aggregate(*args, **kwargs)
+
+                        return Cursor(
+                            query,
+                            self.map_document,
+                            collection_name,
+                            db.name,
+                            self._engine_used,
+                        )
+
+                    @staticmethod
                     def find_classes(
                         *args,
                         database: Optional[
                             Union[
                                 str,
                                 pymongo.database.Database,
                                 mongita.database.Database,
@@ -392,15 +409,14 @@
                         """
 
                         return self.find_classes(
                             collection_name, *args, database, **kwargs
                         )
 
                     def as_json(this, perform_nesting: bool = nested) -> dict:
-
                         """
                         Convert this mongoclass into a json serializable object. This will pop mongodb and mongoclass reserved attributes such as _mongodb_id, _mongodb_collection, etc.
                         """
 
                         x = copy.copy(this.__dict__)
                         x.pop("_mongodb_collection", None)
                         x.pop("_mongodb_db", None)
@@ -462,15 +478,14 @@
             collection: str,
             *args,
             database: Optional[
                 Union[str, pymongo.database.Database, mongita.database.Database]
             ] = None,
             **kwargs,
         ) -> Optional[object]:
-
             """
             Find a single document and convert it onto a mongoclass that maps to the collection of the document.
 
             Parameters
             ----------
             `collection` : str
                 The collection to use.
@@ -498,15 +513,14 @@
             collection: str,
             *args,
             database: Optional[
                 Union[str, pymongo.database.Database, mongita.database.Database]
             ] = None,
             **kwargs,
         ) -> Cursor:
-
             """
             Find multiple documents and return a `Cursor` that you can iterate over that contains the documents as a mongoclass.
 
             Parameters
             ----------
             `collection` : str
                 The collection to use.
```

### Comparing `mongoclass-1.2/mongoclass/cursor.py` & `mongoclass-1.3/mongoclass/cursor.py`

 * *Files identical despite different names*

### Comparing `mongoclass-1.2/mongoclass.egg-info/PKG-INFO` & `mongoclass-1.3/mongoclass.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mongoclass
-Version: 1.2
+Version: 1.3
 Summary: A basic ORM like interface for mongodb in python that uses dataclasses.
 Home-page: https://github.com/bossauh/mongoclass
-Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_12.tar.gz
+Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_13.tar.gz
 Author: Philippe Mathew
 Author-email: philmattdev@gmail.com
 License: MIT
 Keywords: pymongo,orm
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mongoclass-1.2/setup.py` & `mongoclass-1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 install_requires = ["dnspython==2.2.1", "mongita==1.1.1"]
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="mongoclass",
     packages=["mongoclass"],
-    version="1.2",
+    version="1.3",
     license="MIT",
     description="A basic ORM like interface for mongodb in python that uses dataclasses.",
     author="Philippe Mathew",
     author_email="philmattdev@gmail.com",
     url="https://github.com/bossauh/mongoclass",
-    download_url="https://github.com/bossauh/mongoclass/archive/refs/tags/v_12.tar.gz",
+    download_url="https://github.com/bossauh/mongoclass/archive/refs/tags/v_13.tar.gz",
     keywords=["pymongo", "orm"],
     install_requires=install_requires,
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

