# Comparing `tmp/Mongeasy-0.1.5.tar.gz` & `tmp/Mongeasy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mongeasy-0.1.5.tar", last modified: Tue Apr 18 16:45:56 2023, max compression
+gzip compressed data, was "Mongeasy-0.1.6.tar", last modified: Thu Apr 20 12:03:53 2023, max compression
```

## Comparing `Mongeasy-0.1.5.tar` & `Mongeasy-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 16:45:56.783573 Mongeasy-0.1.5/
--rw-rw-rw-   0        0        0     1096 2023-04-17 10:50:01.000000 Mongeasy-0.1.5/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-18 16:45:56.760436 Mongeasy-0.1.5/Mongeasy.egg-info/
--rw-rw-rw-   0        0        0     8057 2023-04-18 16:45:56.000000 Mongeasy-0.1.5/Mongeasy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-04-18 16:45:56.000000 Mongeasy-0.1.5/Mongeasy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 16:45:56.000000 Mongeasy-0.1.5/Mongeasy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-18 16:45:56.000000 Mongeasy-0.1.5/Mongeasy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-18 16:45:56.000000 Mongeasy-0.1.5/Mongeasy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-18 16:45:56.000000 Mongeasy-0.1.5/Mongeasy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8057 2023-04-18 16:45:56.783573 Mongeasy-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     7254 2023-04-18 16:45:19.000000 Mongeasy-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 16:45:56.774957 Mongeasy-0.1.5/mongeasy/
--rw-rw-rw-   0        0        0     2035 2023-04-18 15:29:50.000000 Mongeasy-0.1.5/mongeasy/__init__.py
--rw-rw-rw-   0        0        0     2775 2023-03-03 13:34:30.000000 Mongeasy-0.1.5/mongeasy/base_dict.py
--rw-rw-rw-   0        0        0    11368 2023-04-17 11:54:55.000000 Mongeasy-0.1.5/mongeasy/document.py
--rw-rw-rw-   0        0        0     2643 2023-04-18 15:29:29.000000 Mongeasy-0.1.5/mongeasy/dynamics.py
--rw-rw-rw-   0        0        0     1851 2023-03-09 08:28:25.000000 Mongeasy-0.1.5/mongeasy/exceptions.py
--rw-rw-rw-   0        0        0       20 2023-04-17 07:50:37.000000 Mongeasy-0.1.5/mongeasy/mongeasy.py
--rw-rw-rw-   0        0        0     4963 2023-04-17 10:49:05.000000 Mongeasy-0.1.5/mongeasy/resultlist.py
--rw-rw-rw-   0        0        0     1865 2023-04-17 08:02:18.000000 Mongeasy-0.1.5/mongeasy/utils.py
--rw-rw-rw-   0        0        0       91 2023-04-17 11:07:53.000000 Mongeasy-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0     1057 2023-04-18 16:45:56.784573 Mongeasy-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1076 2023-04-18 16:45:23.000000 Mongeasy-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:45:56.782573 Mongeasy-0.1.5/tests/
--rw-rw-rw-   0        0        0       39 2023-04-17 07:50:37.000000 Mongeasy-0.1.5/tests/__init__.py
--rw-rw-rw-   0        0        0     9850 2023-04-17 09:38:19.000000 Mongeasy-0.1.5/tests/test_mongeasy.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.363582 Mongeasy-0.1.6/
+-rw-rw-rw-   0        0        0     1096 2023-04-17 10:50:01.000000 Mongeasy-0.1.6/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.345055 Mongeasy-0.1.6/Mongeasy.egg-info/
+-rw-rw-rw-   0        0        0     8684 2023-04-20 12:03:53.000000 Mongeasy-0.1.6/Mongeasy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2023-04-20 12:03:53.000000 Mongeasy-0.1.6/Mongeasy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 12:03:53.000000 Mongeasy-0.1.6/Mongeasy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-20 12:03:53.000000 Mongeasy-0.1.6/Mongeasy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-20 12:03:53.000000 Mongeasy-0.1.6/Mongeasy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-20 12:03:53.000000 Mongeasy-0.1.6/Mongeasy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8684 2023-04-20 12:03:53.363582 Mongeasy-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7881 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.356061 Mongeasy-0.1.6/mongeasy/
+-rw-rw-rw-   0        0        0     2164 2023-04-20 12:03:39.000000 Mongeasy-0.1.6/mongeasy/__init__.py
+-rw-rw-rw-   0        0        0     2775 2023-03-03 13:34:30.000000 Mongeasy-0.1.6/mongeasy/base_dict.py
+-rw-rw-rw-   0        0        0     2421 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/connection.py
+-rw-rw-rw-   0        0        0     1487 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/core.py
+-rw-rw-rw-   0        0        0    11815 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/document.py
+-rw-rw-rw-   0        0        0     2657 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/dynamics.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.357061 Mongeasy-0.1.6/mongeasy/examples/
+-rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/examples/__init__.py
+-rw-rw-rw-   0        0        0     1851 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.358061 Mongeasy-0.1.6/mongeasy/extensions/
+-rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/extensions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.359061 Mongeasy-0.1.6/mongeasy/plugins/
+-rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/plugins/__init__.py
+-rw-rw-rw-   0        0        0     4963 2023-04-20 11:49:23.000000 Mongeasy-0.1.6/mongeasy/resultlist.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.360571 Mongeasy-0.1.6/mongeasy/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/utils/__init__.py
+-rw-rw-rw-   0        0        0     1803 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/utils/utils.py
+-rw-rw-rw-   0        0        0       91 2023-04-17 11:07:53.000000 Mongeasy-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1057 2023-04-20 12:03:53.364582 Mongeasy-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2023-04-20 12:03:25.000000 Mongeasy-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.362577 Mongeasy-0.1.6/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-17 07:50:37.000000 Mongeasy-0.1.6/tests/__init__.py
+-rw-rw-rw-   0        0        0    10126 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/tests/test_mongeasy.py
```

### Comparing `Mongeasy-0.1.5/LICENSE` & `Mongeasy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.5/Mongeasy.egg-info/PKG-INFO` & `Mongeasy-0.1.6/Mongeasy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mongeasy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
 Project-URL: Bug Tracker, https://github.com/artheadsweden/mongeasy/issues
 Classifier: Development Status :: 4 - Beta
@@ -220,14 +220,34 @@
         user_id = ObjectId(user_id)
         user = User.find(_id=user_id).first()
         return user
 
     return app
 
 ```
+### Query objects
+To simplify queries to the database you can use the mongeasy query object. You construct it and make your query using normal python syntax.
+
+Instead of using a mongodb query like this
+```python
+query = {'$or': [{'$or': [{'name': {'$eq': 'John'}}, {'age': {'$lt': 40}}]}, {'$and': [{'name': {'$eq': 'Jane'}}, {'age': {'$gt': 20}}]}]}
+```
+
+you can accomplish the same thing by using the Query object
+
+```python
+query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
+```
+
+The query can then be used in your queries like this:
+
+```python
+result = User.find(query)
+```
+
 
 ### ResultList
 All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
 
 
 ```python
 from mongeasy import create_document_class
```

### Comparing `Mongeasy-0.1.5/PKG-INFO` & `Mongeasy-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mongeasy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
 Project-URL: Bug Tracker, https://github.com/artheadsweden/mongeasy/issues
 Classifier: Development Status :: 4 - Beta
@@ -220,14 +220,34 @@
         user_id = ObjectId(user_id)
         user = User.find(_id=user_id).first()
         return user
 
     return app
 
 ```
+### Query objects
+To simplify queries to the database you can use the mongeasy query object. You construct it and make your query using normal python syntax.
+
+Instead of using a mongodb query like this
+```python
+query = {'$or': [{'$or': [{'name': {'$eq': 'John'}}, {'age': {'$lt': 40}}]}, {'$and': [{'name': {'$eq': 'Jane'}}, {'age': {'$gt': 20}}]}]}
+```
+
+you can accomplish the same thing by using the Query object
+
+```python
+query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
+```
+
+The query can then be used in your queries like this:
+
+```python
+result = User.find(query)
+```
+
 
 ### ResultList
 All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
 
 
 ```python
 from mongeasy import create_document_class
```

### Comparing `Mongeasy-0.1.5/README.md` & `Mongeasy-0.1.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -200,14 +200,34 @@
         user_id = ObjectId(user_id)
         user = User.find(_id=user_id).first()
         return user
 
     return app
 
 ```
+### Query objects
+To simplify queries to the database you can use the mongeasy query object. You construct it and make your query using normal python syntax.
+
+Instead of using a mongodb query like this
+```python
+query = {'$or': [{'$or': [{'name': {'$eq': 'John'}}, {'age': {'$lt': 40}}]}, {'$and': [{'name': {'$eq': 'Jane'}}, {'age': {'$gt': 20}}]}]}
+```
+
+you can accomplish the same thing by using the Query object
+
+```python
+query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
+```
+
+The query can then be used in your queries like this:
+
+```python
+result = User.find(query)
+```
+
 
 ### ResultList
 All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
 
 
 ```python
 from mongeasy import create_document_class
```

### Comparing `Mongeasy-0.1.5/mongeasy/__init__.py` & `Mongeasy-0.1.6/mongeasy/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 """Top-level package for Mongeasy."""
 
 __author__ = """Joakim Wassberg"""
 __email__ = 'joakim.wassberg@arthead.se'
-__version__ = '0.1.5'
+__version__ = '0.1.6'
 
-import os
-import configparser
-import pymongo
-from mongeasy.exceptions import MongEasyDBConnectionError
+from mongeasy.connection import MongeasyConnection
+from mongeasy.exceptions import MongeasyDBConnectionError
 from mongeasy.dynamics import create_document_class
 
-connection = None
+connection = MongeasyConnection()
 
+# connection = None
 
-def get_connection():
-    return connection
 
+# def get_connection():
+#     return connection
 
-def connect(connection_str: str=None, db_name: str=None):
-    global connection
-    if connection is not None:
-        return connection
 
-    try:
-        # Try connecting using connect function
-        if connection_str and db_name:
-            connection = pymongo.MongoClient(connection_str)[db_name]
-            return connection
-    except Exception as e:
-        print(e)
+# def connect(connection_str: str=None, db_name: str=None):
+#     global connection
+#     if connection is not None:
+#         return connection
+
+#     try:
+#         # Try connecting using connect function
+#         if connection_str and db_name:
+#             connection = pymongo.MongoClient(connection_str)[db_name]
+#             return connection
+#     except Exception as e:
+#         print(e)
     
-    connect_from_env()
-    connect_from_config()
+#     connect_from_env()
+#     connect_from_config()
 
-    if connection is None:
-        raise MongEasyDBConnectionError("Failed to connect to database using environment variables or config file.")
+#     if connection is None:
+#         raise MongEasyDBConnectionError("Failed to connect to database using environment variables or config file.")
 
-    return connection
+#     return connection
 
-def connect_from_env():
-    global connection
-    try:
-        # Try connecting using environment variables
-        connection_string = os.environ.get('MONGOEASY_CONNECTION_STRING')
-        database_name = os.environ.get('MONGOEASY_DATABASE_NAME')
-        if connection_string and database_name:
-            connection = pymongo.MongoClient(connection_string)[database_name]
-    except Exception as e:
-        print(e)
-
-def connect_from_config():
-    global connection
-    try:
-        # Try connecting using config file
-        config = configparser.ConfigParser()
-        config.read('mongeasy.conf')
-        if 'mongoeasy' in config:
-            section = config['mongoeasy']
-            connection_string = section.get('connection_string')
-            database_name = section.get('database_name')
-            if connection_string and database_name:
-                connection = pymongo.MongoClient(connection_string)[database_name]
-    except Exception as e:
-        print(e)
+# def connect_from_env():
+#     global connection
+#     try:
+#         # Try connecting using environment variables
+#         connection_string = os.environ.get('MONGOEASY_CONNECTION_STRING')
+#         database_name = os.environ.get('MONGOEASY_DATABASE_NAME')
+#         if connection_string and database_name:
+#             connection = pymongo.MongoClient(connection_string)[database_name]
+#     except Exception as e:
+#         print(e)
+
+# def connect_from_config():
+#     global connection
+#     try:
+#         # Try connecting using config file
+#         config = configparser.ConfigParser()
+#         config.read('mongeasy.conf')
+#         if 'mongoeasy' in config:
+#             section = config['mongoeasy']
+#             connection_string = section.get('connection_string')
+#             database_name = section.get('database_name')
+#             if connection_string and database_name:
+#                 connection = pymongo.MongoClient(connection_string)[database_name]
+#     except Exception as e:
+#         print(e)
         
         
-connect()
+# connect()
```

### Comparing `Mongeasy-0.1.5/mongeasy/base_dict.py` & `Mongeasy-0.1.6/mongeasy/base_dict.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.5/mongeasy/document.py` & `Mongeasy-0.1.6/mongeasy/document.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,298 +1,301 @@
-"""
-This module contains the Document class for interacting with MongoDB collections.
-
-MIT License
-
-Copyright (c) 2023 Joakim Wassberg
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation
-files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use,
-copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom
-the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
-WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
-
-from datetime import datetime
-from copy import copy, deepcopy
-from typing import Union
-import logging
-import json
-import bson
-from .exceptions import MongEasyDBCollectionError, MongEasyFieldError, MongEasyDBDocumentError, MongEasyIndexException
-from .base_dict import BaseDict
-from .resultlist import ResultList
-import pymongo
-
-class Document(BaseDict):
-    """
-    This class acts as the base class for collection classes. Each instance of the subclasses
-    will represent a single document
-    """
-    collection = None
-    logger = logging.getLogger('mongeasy')
-
-    def __init__(self, *args, **kwargs):
-        super().__init__()
-
-        # Handle positional arguments
-        if len(args) == 1 and isinstance(args[0], dict):
-            as_dict = copy(args[0])
-        elif len(args) == 0:
-            as_dict = copy(kwargs)
-        else:
-            raise TypeError(f'Document() takes 1 positional argument or keyword arguments but {len(args) + len(kwargs)} were given')
-
-        # If _id is not present we add the _id attribute
-        if '_id' not in as_dict:
-            self._id = None
-        else:
-            try:
-                self._id = bson.ObjectId(str(as_dict['_id']))
-            except bson.errors.InvalidId:
-                raise MongEasyFieldError(f'Invalid _id: {as_dict["_id"]}')
-
-        # Update the object
-        self.__dict__.update(as_dict)
-
-    def has_changed(self) -> dict:
-        """
-        Checks if any of the fields in this document has changed
-        :return: dict, a dict with the changed fields, empty if no fields have changed
-        """
-        if self._id is None:
-            return self.__dict__
-
-        changed_fields = {}
-        for key, value in self.__dict__.items():
-            if key != '_id':
-                try:
-                    result = self.collection.find_one({'_id': self._id}, {key: 1})
-                except (pymongo.errors.OperationFailure, pymongo.errors.ServerSelectionTimeoutError) as e:
-                    Document.logger.error(f"Error querying the database: {e}")
-                    return {}
-
-                if result and key in result and result[key] != value:
-                    changed_fields[key] = value
-        return changed_fields
-
-    def is_saved(self) -> bool:
-        """
-        Checks if this document has been saved to the database
-        :return: bool, True if the document has been saved, False otherwise
-        """
-        return not bool(self.has_changed())
-
-    def save(self):
-        """
-        Saves the current object to the database
-        :return: The saved object
-        """
-        if self.collection is None:
-            Document.logger.error("The collection does not exist")
-            raise MongEasyDBCollectionError('The collection does not exist')
-
-        # If _id is None, this is a new document
-        if self._id is None:
-            del self._id
-            res = self.collection.insert_one(self.__dict__)
-            self._id = res.inserted_id
-            return self
-
-        # if no fields have changed, return the document unchanged
-        if not (changed_fields := self.has_changed()):
-            return self
-
-        # update the document
-        update_result = self.collection.update_one({'_id': self._id}, {'$set': changed_fields})
-        if update_result.matched_count == 0:
-            Document.logger.error(f"Document with _id {self._id} does not exist")
-            raise MongEasyDBDocumentError(f"Document with _id {self._id} does not exist")
-        else:
-            return self
-
-    def reload(self):
-        """
-        Fetches the latest state of the document from the database and updates the current instance with the changes.
-        """
-        if self._id is None:
-            raise MongEasyDBDocumentError('Cannot reload unsaved document')
-
-        # fetch the latest state of the document from the database
-        db_doc = self.collection.find_one({'_id': self._id})
-        if db_doc is None:
-            raise MongEasyDBDocumentError(f"Document with _id {self._id} does not exist")
-
-        self_before_reload = deepcopy(self)
-        # update the current instance with the changes
-        for key, value in db_doc.items():
-            if isinstance(value, dict) and not isinstance(value, Document):
-                # convert any embedded dictionary to an instance of BaseDict
-                self[key] = BaseDict(value)
-            else:
-                self[key] = value
-
-
-    def delete_field(self, field: str):
-        """
-        Removes a field from this document
-        :param field: str, the field to remove
-        :return: None
-        """
-        try:
-            self.collection.update_one({'_id': self._id}, {"$unset": {field: ""}})
-        except Exception as e:
-            Document.logger.error(f"Error deleting field '{field}' from document with id '{self._id}': {e}")
-        else:
-            Document.logger.info(f"Field '{field}' deleted from document with id '{self._id}'")
-
-    def delete(self):
-        """
-        Delete the current object from the database
-        :return: None
-        """
-        if self.collection is None:
-            raise MongEasyDBCollectionError('The collection does not exist')
-
-        if self._id is None:
-            raise MongEasyDBDocumentError('Cannot delete unsaved document')
-
-        self.collection.delete_one({'_id': self._id})
-
-    def to_json(self):
-        """
-        Serialize the document to JSON
-        :return: str, the JSON representation of the document
-        """
-        json_dict = {}
-        for key, value in self.__dict__.items():
-            if isinstance(value, bson.ObjectId):
-                json_dict[key] = str(value)
-            elif isinstance(value, datetime):
-                json_dict[key] = value.strftime('%Y-%m-%dT%H:%M:%S.%fZ')
-            else:
-                json_dict[key] = value
-        return json.dumps(json_dict)
-
-    @classmethod
-    def create_index(cls, keys: list[str], index_type: str = 'asc', unique: bool = False, name: Union[str, None] = None) -> None:
-        """
-        Creates an index on the specified keys
-        :param keys: The keys to index on
-        :param index_type: The index type, either 'asc' (default) or 'desc'
-        :param unique: Whether the index should be unique
-        :param name: The name of the index
-        :return: None
-        """
-        # Check that keys is a non-empty list of strings
-        if not isinstance(keys, list) or not all(isinstance(key, str) for key in keys) or len(keys) == 0:
-            raise MongEasyIndexException('keys must be a non-empty list of strings')
-
-        # Check that index_type is either 'asc' or 'desc'
-        if index_type not in ['asc', 'desc']:
-            raise MongEasyIndexException('index_type must be either "asc" or "desc"')
-
-        # Check that name is either None or a non-empty string
-        if name is not None and not isinstance(name, str):
-            raise MongEasyIndexException('name must be either None or a non-empty string')
-
-        index_name = name or '_'.join(keys) + '_' + index_type.lower()
-        index_type = pymongo.ASCENDING if index_type == 'asc' else pymongo.DESCENDING
-        cls.collection.create_index([(key, index_type) for key in keys], name=index_name, unique=unique)
-
-    @classmethod
-    def get_by_id(cls, _id:str) -> Union['Document', None]:
-        """
-        Get a document by its _id
-        :param _id: str, the id of the document
-        :return: The retrieved document or None
-        """
-        try:
-            return cls(cls.collection.find_one({'_id': bson.ObjectId(_id)}))
-        except bson.errors.InvalidId:
-            return None
-
-    @classmethod
-    def insert_many(cls, items: list[dict]) -> None:
-        """
-        Inserts a list of dictionaries into the database
-        :param items: list of dict, items to insert
-        :return: None
-        """
-        for item in items:
-            try:
-                cls(item).save()
-            except pymongo.errors.PyMongoError as e:
-                Document.logger.exception(f"Error inserting item: {item}. Exception: {e}")
-
-    @classmethod
-    def find(cls, *args, **kwargs):
-        """
-        Find a document that matches the keywords
-        :param arg: positional arguments
-        :param kwargs: keyword arguments or dict to match
-        :return: ResultList
-        """
-        # Handle positional arguments
-        if len(args) == 1 and isinstance(args[0], dict):
-            as_dict = copy(args[0])
-        elif len(args) == 0:
-            as_dict = copy(kwargs)
-
-        return ResultList(cls(item) for item in cls.collection.find(as_dict))
-
-    @classmethod
-    def find_in(cls, field:str, values:list) -> ResultList:
-        """
-        Find a document that matches the keywords
-        :param field: str, the field to search in
-        :param values: list, the values to search for
-        :return: ResultList
-        """
-        return ResultList(cls(item) for item in cls.collection.find({field: {"$in": values}}))
-
-    @classmethod
-    def all(cls) -> ResultList:
-        """
-        Returns all documents in the collection
-        :return: ResultList
-        """
-        return ResultList(cls(item) for item in cls.collection.find({}))
-
-    @classmethod
-    def all_iter(cls) -> dict:
-        """
-        Retrieve all documents from the collection as an iterator
-        :yields: dict representation of next document
-        """
-        for item in cls.collection.find({}):
-            yield cls(**item)
-
-    @classmethod
-    def delete(cls, *args, **kwargs) -> None:
-        """
-        Delete the document that matches the keywords
-
-        :param args: positional arguments
-        :param kwargs: keyword arguments or dict to match
-        :return: None
-        """
-        # Handle positional arguments
-        if len(args) == 1 and isinstance(args[0], dict):
-            as_dict = copy(args[0])
-        elif len(args) == 0:
-            as_dict = copy(kwargs)
-        cls.collection.delete_many(as_dict)
-
-    @classmethod
-    def document_count(cls) -> int:
-        """
-        Returns the total number of documents in the collection
-        :return: int
-        """
-        return cls.collection.count_documents({})
+"""
+This module contains the Document class for interacting with MongoDB collections.
+
+MIT License
+
+Copyright (c) 2023 Joakim Wassberg
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation
+files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use,
+copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom
+the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
+WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+"""
+
+from datetime import datetime
+from copy import copy, deepcopy
+from typing import Union, List, Dict, Any
+import logging
+import json
+import bson
+from .exceptions import MongeasyDBCollectionError, MongeasyFieldError, MongeasyDBDocumentError, MongeasyIndexException
+from .base_dict import BaseDict
+from .core import Query
+from .resultlist import ResultList
+import pymongo
+
+class Document(BaseDict):
+    """
+    This class acts as the base class for collection classes. Each instance of the subclasses
+    will represent a single document
+    """
+    collection = None
+    logger = logging.getLogger('mongeasy')
+
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+
+        # Handle positional arguments
+        if len(args) == 1 and isinstance(args[0], dict):
+            as_dict = copy(args[0])
+        elif len(args) == 0:
+            as_dict = copy(kwargs)
+        else:
+            raise TypeError(f'Document() takes 1 positional argument or keyword arguments but {len(args) + len(kwargs)} were given')
+
+        # If _id is not present we add the _id attribute
+        if '_id' not in as_dict:
+            self._id = None
+        else:
+            try:
+                self._id = bson.ObjectId(str(as_dict['_id']))
+            except bson.errors.InvalidId:
+                raise MongeasyFieldError(f'Invalid _id: {as_dict["_id"]}')
+
+        # Update the object
+        self.__dict__.update(as_dict)
+
+    def has_changed(self) -> dict:
+        """
+        Checks if any of the fields in this document has changed
+        :return: dict, a dict with the changed fields, empty if no fields have changed
+        """
+        if self._id is None:
+            return self.__dict__
+
+        changed_fields = {}
+        for key, value in self.__dict__.items():
+            if key != '_id':
+                try:
+                    result = self.collection.find_one({'_id': self._id}, {key: 1})
+                except (pymongo.errors.OperationFailure, pymongo.errors.ServerSelectionTimeoutError) as e:
+                    Document.logger.error(f"Error querying the database: {e}")
+                    return {}
+
+                if result and key in result and result[key] != value:
+                    changed_fields[key] = value
+        return changed_fields
+
+    def is_saved(self) -> bool:
+        """
+        Checks if this document has been saved to the database
+        :return: bool, True if the document has been saved, False otherwise
+        """
+        return not bool(self.has_changed())
+
+    def save(self):
+        """
+        Saves the current object to the database
+        :return: The saved object
+        """
+        if self.collection is None:
+            Document.logger.error("The collection does not exist")
+            raise MongeasyDBCollectionError('The collection does not exist')
+
+        # If _id is None, this is a new document
+        if self._id is None:
+            del self._id
+            res = self.collection.insert_one(self.__dict__)
+            self._id = res.inserted_id
+            return self
+
+        # if no fields have changed, return the document unchanged
+        if not (changed_fields := self.has_changed()):
+            return self
+
+        # update the document
+        update_result = self.collection.update_one({'_id': self._id}, {'$set': changed_fields})
+        if update_result.matched_count == 0:
+            Document.logger.error(f"Document with _id {self._id} does not exist")
+            raise MongeasyDBDocumentError(f"Document with _id {self._id} does not exist")
+        else:
+            return self
+
+    def reload(self):
+        """
+        Fetches the latest state of the document from the database and updates the current instance with the changes.
+        """
+        if self._id is None:
+            raise MongeasyDBDocumentError('Cannot reload unsaved document')
+
+        # fetch the latest state of the document from the database
+        db_doc = self.collection.find_one({'_id': self._id})
+        if db_doc is None:
+            raise MongeasyDBDocumentError(f"Document with _id {self._id} does not exist")
+
+        self_before_reload = deepcopy(self)
+        # update the current instance with the changes
+        for key, value in db_doc.items():
+            if isinstance(value, dict) and not isinstance(value, Document):
+                # convert any embedded dictionary to an instance of BaseDict
+                self[key] = BaseDict(value)
+            else:
+                self[key] = value
+
+
+    def delete_field(self, field: str):
+        """
+        Removes a field from this document
+        :param field: str, the field to remove
+        :return: None
+        """
+        try:
+            self.collection.update_one({'_id': self._id}, {"$unset": {field: ""}})
+        except Exception as e:
+            Document.logger.error(f"Error deleting field '{field}' from document with id '{self._id}': {e}")
+        else:
+            Document.logger.info(f"Field '{field}' deleted from document with id '{self._id}'")
+
+    def delete(self):
+        """
+        Delete the current object from the database
+        :return: None
+        """
+        if self.collection is None:
+            raise MongeasyDBCollectionError('The collection does not exist')
+
+        if self._id is None:
+            raise MongeasyDBDocumentError('Cannot delete unsaved document')
+
+        self.collection.delete_one({'_id': self._id})
+
+    def to_json(self):
+        """
+        Serialize the document to JSON
+        :return: str, the JSON representation of the document
+        """
+        json_dict = {}
+        for key, value in self.__dict__.items():
+            if isinstance(value, bson.ObjectId):
+                json_dict[key] = str(value)
+            elif isinstance(value, datetime):
+                json_dict[key] = value.strftime('%Y-%m-%dT%H:%M:%S.%fZ')
+            else:
+                json_dict[key] = value
+        return json.dumps(json_dict)
+
+    @classmethod
+    def create_index(cls, keys: List[str], index_type: str = 'asc', unique: bool = False, name: Union[str, None] = None) -> None:
+        """
+        Creates an index on the specified keys
+        :param keys: The keys to index on
+        :param index_type: The index type, either 'asc' (default) or 'desc'
+        :param unique: Whether the index should be unique
+        :param name: The name of the index
+        :return: None
+        """
+        # Check that keys is a non-empty list of strings
+        if not isinstance(keys, list) or not all(isinstance(key, str) for key in keys) or len(keys) == 0:
+            raise MongeasyIndexException('keys must be a non-empty list of strings')
+
+        # Check that index_type is either 'asc' or 'desc'
+        if index_type not in ['asc', 'desc']:
+            raise MongeasyIndexException('index_type must be either "asc" or "desc"')
+
+        # Check that name is either None or a non-empty string
+        if name is not None and not isinstance(name, str):
+            raise MongeasyIndexException('name must be either None or a non-empty string')
+
+        index_name = name or '_'.join(keys) + '_' + index_type.lower()
+        index_type = pymongo.ASCENDING if index_type == 'asc' else pymongo.DESCENDING
+        cls.collection.create_index([(key, index_type) for key in keys], name=index_name, unique=unique)
+
+    @classmethod
+    def get_by_id(cls, _id:str) -> Union['Document', None]:
+        """
+        Get a document by its _id
+        :param _id: str, the id of the document
+        :return: The retrieved document or None
+        """
+        try:
+            return cls(cls.collection.find_one({'_id': bson.ObjectId(_id)}))
+        except bson.errors.InvalidId:
+            return None
+
+    @classmethod
+    def insert_many(cls, items: List[dict]) -> None:
+        """
+        Inserts a list of dictionaries into the database
+        :param items: list of dict, items to insert
+        :return: None
+        """
+        for item in items:
+            try:
+                cls(item).save()
+            except pymongo.errors.PyMongoError as e:
+                Document.logger.exception(f"Error inserting item: {item}. Exception: {e}")
+
+    @classmethod
+    def find(cls, *args, **kwargs):
+        """
+        Find a document that matches the keywords
+        :param arg: positional arguments
+        :param kwargs: keyword arguments or dict to match
+        :return: ResultList
+        """
+        # Handle positional arguments
+        if len(args) == 1 and isinstance(args[0], dict):
+            as_dict = copy(args[0])
+        if len(args) == 1 and isinstance(args[0], Query):
+            as_dict = args[0].to_mongo_query()
+        elif len(args) == 0:
+            as_dict = copy(kwargs)
+
+        return ResultList(cls(item) for item in cls.collection.find(as_dict))
+
+    @classmethod
+    def find_in(cls, field:str, values:list) -> ResultList:
+        """
+        Find a document that matches the keywords
+        :param field: str, the field to search in
+        :param values: list, the values to search for
+        :return: ResultList
+        """
+        return ResultList(cls(item) for item in cls.collection.find({field: {"$in": values}}))
+
+    @classmethod
+    def all(cls) -> ResultList:
+        """
+        Returns all documents in the collection
+        :return: ResultList
+        """
+        return ResultList(cls(item) for item in cls.collection.find({}))
+
+    @classmethod
+    def all_iter(cls) -> dict:
+        """
+        Retrieve all documents from the collection as an iterator
+        :yields: dict representation of next document
+        """
+        for item in cls.collection.find({}):
+            yield cls(**item)
+
+    @classmethod
+    def delete(cls, *args, **kwargs) -> None:
+        """
+        Delete the document that matches the keywords
+
+        :param args: positional arguments
+        :param kwargs: keyword arguments or dict to match
+        :return: None
+        """
+        # Handle positional arguments
+        if len(args) == 1 and isinstance(args[0], dict):
+            as_dict = copy(args[0])
+        elif len(args) == 0:
+            as_dict = copy(kwargs)
+        cls.collection.delete_many(as_dict)
+
+    @classmethod
+    def document_count(cls) -> int:
+        """
+        Returns the total number of documents in the collection
+        :return: int
+        """
+        return cls.collection.count_documents({})
```

### Comparing `Mongeasy-0.1.5/mongeasy/dynamics.py` & `Mongeasy-0.1.6/mongeasy/dynamics.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, 
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 import inspect
 from typing import Union
-from .utils import pascal_to_snake
+from .utils.utils import pascal_to_snake
 from .document import Document
-from .exceptions import MongEasyValidationException, MongEasyFieldError
+from .exceptions import MongeasyValidationException, MongeasyFieldError
 
 
 def create_document_class(class_name: str, collection_name: str = None, base_classes: tuple = ()):
     """
     Dynamically create a document class and register it in the calling module's namespace.
     Args:
         class_name (str): Name of the class to create.
@@ -42,15 +42,15 @@
 
     # Dynamically generate the document class
     from . import connection
     if collection_name is None:
         collection_name = pascal_to_snake(class_name) + 's'
     
     # Create the collection object
-    collection = connection[collection_name]
+    collection = connection.db[collection_name]
     
-    doc_class = type(class_name, base_classes + (Document,), {'collection':collection})
+    doc_class = type(class_name, base_classes + (Document, ), {'collection':collection})
 
     # Register the document class in the calling module's namespace
     setattr(calling_module, class_name, doc_class)
-
+    
     return doc_class
```

### Comparing `Mongeasy-0.1.5/mongeasy/exceptions.py` & `Mongeasy-0.1.6/mongeasy/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,46 +15,46 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, 
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 
-class MongEasyException(Exception):
+class MongeasyException(Exception):
     """
     Base exception class
     """
 
 
-class MongEasyDBConnectionError(MongEasyException):
+class MongeasyDBConnectionError(MongeasyException):
     """
     Database initialization exceptions
     """
 
 
-class MongEasyDBCollectionError(MongEasyException):
+class MongeasyDBCollectionError(MongeasyException):
     """
     Collection exceptions
     """
 
 
-class MongEasyDBDocumentError(MongEasyException):
+class MongeasyDBDocumentError(MongeasyException):
     """
     Document exceptions
     """
 
 
-class MongEasyFieldError(MongEasyException):
+class MongeasyFieldError(MongeasyException):
     """
     Field exceptions
     """
     
-class MongEasyValidationException(MongEasyException):
+class MongeasyValidationException(MongeasyException):
     """
     Validation exceptions
     """
     
-class MongEasyIndexException(MongEasyException):
+class MongeasyIndexException(MongeasyException):
     """
     Index exceptions
     """
```

### Comparing `Mongeasy-0.1.5/mongeasy/resultlist.py` & `Mongeasy-0.1.6/mongeasy/resultlist.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.5/mongeasy/utils.py` & `Mongeasy-0.1.6/mongeasy/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, 
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
-from typing import Union
-from .resultlist import ResultList
 
 def snake_to_pascal(s: str):
     """
     Convert a snake_case string to PascalCase.
 
     Example:
     snake_to_pascal('my_snake_string') -> 'MySnakeString'
```

### Comparing `Mongeasy-0.1.5/setup.cfg` & `Mongeasy-0.1.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f6e 6765 6173 790d 0a76 6572   = mongeasy..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e35 0d0a 6175  sion = 0.1.5..au
+00000020: 7369 6f6e 203d 2030 2e31 2e36 0d0a 6175  sion = 0.1.6..au
 00000030: 7468 6f72 203d 204a 6f61 6b69 6d20 5761  thor = Joakim Wa
 00000040: 7373 6265 7267 0d0a 6175 7468 6f72 5f65  ssberg..author_e
 00000050: 6d61 696c 203d 206a 6f61 6b69 6d2e 7761  mail = joakim.wa
 00000060: 7373 6265 7267 4061 7274 6865 6164 2e73  ssberg@arthead.s
 00000070: 650d 0a64 6573 6372 6970 7469 6f6e 203d  e..description =
 00000080: 2045 6173 7920 746f 2075 7365 2077 7261   Easy to use wra
 00000090: 7070 6572 2061 726f 756e 6420 7079 6d6f  pper around pymo
```

### Comparing `Mongeasy-0.1.5/setup.py` & `Mongeasy-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     readme = f.read()
 
 with open("LICENSE", encoding="utf8") as f:
     license = f.read()
 
 setup(
     name="Mongeasy",
-    version="0.1.5",
+    version="0.1.6",
     author="Joakim Wassberg",
     author_email="joakim.wassberg@arthead.se",
     description="Easy to use wrapper around pymongo for easy access to MongoDB.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/artheadsweden/mongeasy",
     license="MIT",
```

### Comparing `Mongeasy-0.1.5/tests/test_mongeasy.py` & `Mongeasy-0.1.6/tests/test_mongeasy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,276 +1,276 @@
-#!/usr/bin/env python
-
-"""Tests for `mongeasy` package."""
-# Do this before importing mongeasy as it will try to connect to the database
-import os
-os.environ['MONGOEASY_CONNECTION_STRING'] = 'mongodb://localhost:27017'
-os.environ['MONGOEASY_DATABASE_NAME'] = 'mongeasy_pytest'
-from pymongo import MongoClient
-import pytest
-
-
-from mongeasy import create_document_class
-
-
-@pytest.fixture(scope='function')
-def clean_mongo():
-    # Connect to MongoDB
-    client = MongoClient('mongodb://localhost:27017')
-    db = client['mongeasy_pytest']
-
-    # Clean all collections in the test database
-    for collection_name in db.list_collection_names():
-        db[collection_name].delete_many({})
-
-
-
-def test_document_init_with_dict(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    stored_user = User.find({'first_name': 'John'}).first()
-    assert user.first_name == stored_user.first_name
-    assert user.last_name == stored_user.last_name
-    assert user.age == stored_user.age
-
-
-def test_document_init_with_kwargs(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User(first_name='Pete', last_name='Doe', age=30)
-    user.save()
-    stored_user = User.find({'first_name': 'Pete'}).first()
-    assert user.first_name == stored_user.first_name
-    assert user.last_name == stored_user.last_name
-    assert user.age == stored_user.age
-    assert True
-
-
-# def test_document_init_with_positional_arguments(clean_mongo):
-#     assert True
-
-
-# def test_document_init_with_invalid_arguments(clean_mongo):
-#     assert True
-
-
-def test_document_has_changed_with_no_changes(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    assert not user.has_changed()
-
-
-def test_document_has_changed_with_changes(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    user.age += 1
-    assert user.has_changed()
-
-
-def test_document_has_changed_with_new_document(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-
-    assert user.has_changed()
-
-
-def test_document_is_saved_with_no_changes(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    assert user.is_saved()
-
-def test_document_is_saved_with_changes(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    user.age += 1
-    assert not user.is_saved()
-
-
-def test_document_save_new_document(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    stored_user = User.find({'first_name': 'John'}).first()
-    assert user.first_name == stored_user.first_name
-    assert user.last_name == stored_user.last_name
-    assert user.age == stored_user.age
-
-
-def test_document_save_existing_document_with_no_changes(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    user.save()
-    stored_user = User.find({'first_name': 'John'}).first()
-    assert user.first_name == stored_user.first_name
-    assert user.last_name == stored_user.last_name
-    assert user.age == stored_user.age
-
-
-def test_document_save_existing_document_with_changes(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    user.age += 1
-    user.save()
-    stored_user = User.find({'first_name': 'John'}).first()
-    assert user.first_name == stored_user.first_name
-    assert user.last_name == stored_user.last_name
-    assert user.age == stored_user.age
-
-
-def test_document_reload_existing_document(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    user.age += 1
-    user.reload()
-    assert user.age == 30
-
-
-def test_document_reload_unsaved_document(clean_mongo):
-    from mongeasy.exceptions import MongEasyDBDocumentError
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    with pytest.raises(MongEasyDBDocumentError):
-        user.reload()
-
-def test_document_delete_field(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    user.delete_field('age')
-    user.save()
-    stored_user = User.find({'first_name': 'John'}).first()
-    assert 'age' not in stored_user
-
-
-def test_document_delete_existing_document(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    user.delete()
-    stored_user = User.find({'first_name': 'John'}).first()
-    assert stored_user is None
-
-
-def test_document_delete_unsaved_document(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.delete()
-    stored_user = User.find({'first_name': 'John'}).first()
-    assert stored_user is None
-
-
-def test_document_to_json(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    json_user = user.to_json()
-    assert isinstance(json_user, str)
-    assert 'John' in json_user
-    assert 'Doe' in json_user
-    assert '30' in json_user
-    assert str(user._id) in json_user
-
-
-def test_document_get_by_id_with_valid_id(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    stored_user = User.get_by_id(user._id)
-    assert user.first_name == stored_user.first_name
-    assert user.last_name == stored_user.last_name
-    assert user.age == stored_user.age
-
-
-def test_document_get_by_id_with_invalid_id(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    stored_user = User.get_by_id('123')
-    assert stored_user is None
-
-
-def test_document_insert_many(clean_mongo):
-    users = [
-    {'first_name': 'Alice', 'last_name': 'Smith', 'age': 25},
-    {'first_name': 'Bob', 'last_name': 'Jones', 'age': 35},
-    {'first_name': 'Charlie', 'last_name': 'Brown', 'age': 45},
-    {'first_name': 'Dave', 'last_name': 'Smith', 'age': 55}
-]
-    User = create_document_class('User', 'users')
-    User.insert_many(users)
-    stored_users = User.all()
-    assert len(stored_users) == 4
-
-def test_document_find(clean_mongo):
-    User = create_document_class('User', 'users')
-    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.save()
-    stored_user = User.find({'first_name': 'John'}).first()
-    assert user.first_name == stored_user.first_name
-    assert user.last_name == stored_user.last_name
-    assert user.age == stored_user.age
-
-
-def test_document_find_in(clean_mongo):
-    User = create_document_class('User', 'users')
-    user1 = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user1.save()
-    user2 = User({'first_name': 'Alice', 'last_name': 'Smith', 'age': 25})
-    user2.save()
-    user3 = User({'first_name': 'Bob', 'last_name': 'Jones', 'age': 35})
-    user3.save()
-    stored_users = User.find_in('first_name', ['John', 'Bob'])
-    assert len(stored_users) == 2
-    assert user1.first_name in [user.first_name for user in stored_users]
-    assert user2.first_name not in [user.first_name for user in stored_users]
-    assert user3.first_name in [user.first_name for user in stored_users]
-
-
-def test_document_all(clean_mongo):
-    User = create_document_class('User', 'users')
-    user1 = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user1.save()
-    user2 = User({'first_name': 'Alice', 'last_name': 'Smith', 'age': 25})
-    user2.save()
-    user3 = User({'first_name': 'Bob', 'last_name': 'Jones', 'age': 35})
-    user3.save()
-    stored_users = User.all()
-    assert len(stored_users) == 3
-    assert user1.first_name in [user.first_name for user in stored_users]
-    assert user2.first_name in [user.first_name for user in stored_users]
-    assert user3.first_name in [user.first_name for user in stored_users]
-
-
-def test_document_delete(clean_mongo):
-    User = create_document_class('User', 'users')
-    user1 = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user1.save()
-    user2 = User({'first_name': 'Alice', 'last_name': 'Smith', 'age': 25})
-    user2.save()
-    user3 = User({'first_name': 'Bob', 'last_name': 'Jones', 'age': 35})
-    user3.save()
-    User.delete({'first_name': 'Alice'})
-    stored_users = User.all()
-    assert len(stored_users) == 2
-    assert user1.first_name in [user.first_name for user in stored_users]
-    assert user2.first_name not in [user.first_name for user in stored_users]
-    assert user3.first_name in [user.first_name for user in stored_users]
-
-
-def test_document_document_count(clean_mongo):
-    User = create_document_class('User', 'users')
-    user1 = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user1.save()
-    user2 = User({'first_name': 'Alice', 'last_name': 'Smith', 'age': 25})
-    user2.save()
-    user3 = User({'first_name': 'Bob', 'last_name': 'Jones', 'age': 35})
-    user3.save()
-    count = User.document_count()
-    assert count == 3
-
+#!/usr/bin/env python
+
+"""Tests for `mongeasy` package."""
+# Do this before importing mongeasy as it will try to connect to the database
+import os
+os.environ['MONGOEASY_CONNECTION_STRING'] = 'mongodb://localhost:27017'
+os.environ['MONGOEASY_DATABASE_NAME'] = 'mongeasy_pytest'
+from pymongo import MongoClient
+import pytest
+
+
+from mongeasy import create_document_class
+
+
+@pytest.fixture(scope='function')
+def clean_mongo():
+    # Connect to MongoDB
+    client = MongoClient('mongodb://localhost:27017')
+    db = client['mongeasy_pytest']
+
+    # Clean all collections in the test database
+    for collection_name in db.list_collection_names():
+        db[collection_name].delete_many({})
+
+
+
+def test_document_init_with_dict(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    stored_user = User.find({'first_name': 'John'}).first()
+    assert user.first_name == stored_user.first_name
+    assert user.last_name == stored_user.last_name
+    assert user.age == stored_user.age
+
+
+def test_document_init_with_kwargs(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User(first_name='Pete', last_name='Doe', age=30)
+    user.save()
+    stored_user = User.find({'first_name': 'Pete'}).first()
+    assert user.first_name == stored_user.first_name
+    assert user.last_name == stored_user.last_name
+    assert user.age == stored_user.age
+    assert True
+
+
+# def test_document_init_with_positional_arguments(clean_mongo):
+#     assert True
+
+
+# def test_document_init_with_invalid_arguments(clean_mongo):
+#     assert True
+
+
+def test_document_has_changed_with_no_changes(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    assert not user.has_changed()
+
+
+def test_document_has_changed_with_changes(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    user.age += 1
+    assert user.has_changed()
+
+
+def test_document_has_changed_with_new_document(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+
+    assert user.has_changed()
+
+
+def test_document_is_saved_with_no_changes(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    assert user.is_saved()
+
+def test_document_is_saved_with_changes(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    user.age += 1
+    assert not user.is_saved()
+
+
+def test_document_save_new_document(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    stored_user = User.find({'first_name': 'John'}).first()
+    assert user.first_name == stored_user.first_name
+    assert user.last_name == stored_user.last_name
+    assert user.age == stored_user.age
+
+
+def test_document_save_existing_document_with_no_changes(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    user.save()
+    stored_user = User.find({'first_name': 'John'}).first()
+    assert user.first_name == stored_user.first_name
+    assert user.last_name == stored_user.last_name
+    assert user.age == stored_user.age
+
+
+def test_document_save_existing_document_with_changes(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    user.age += 1
+    user.save()
+    stored_user = User.find({'first_name': 'John'}).first()
+    assert user.first_name == stored_user.first_name
+    assert user.last_name == stored_user.last_name
+    assert user.age == stored_user.age
+
+
+def test_document_reload_existing_document(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    user.age += 1
+    user.reload()
+    assert user.age == 30
+
+
+def test_document_reload_unsaved_document(clean_mongo):
+    from mongeasy.exceptions import MongeasyDBDocumentError
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    with pytest.raises(MongeasyDBDocumentError):
+        user.reload()
+
+def test_document_delete_field(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    user.delete_field('age')
+    user.save()
+    stored_user = User.find({'first_name': 'John'}).first()
+    assert 'age' not in stored_user
+
+
+def test_document_delete_existing_document(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    user.delete()
+    stored_user = User.find({'first_name': 'John'}).first()
+    assert stored_user is None
+
+
+def test_document_delete_unsaved_document(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.delete()
+    stored_user = User.find({'first_name': 'John'}).first()
+    assert stored_user is None
+
+
+def test_document_to_json(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    json_user = user.to_json()
+    assert isinstance(json_user, str)
+    assert 'John' in json_user
+    assert 'Doe' in json_user
+    assert '30' in json_user
+    assert str(user._id) in json_user
+
+
+def test_document_get_by_id_with_valid_id(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    stored_user = User.get_by_id(user._id)
+    assert user.first_name == stored_user.first_name
+    assert user.last_name == stored_user.last_name
+    assert user.age == stored_user.age
+
+
+def test_document_get_by_id_with_invalid_id(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    stored_user = User.get_by_id('123')
+    assert stored_user is None
+
+
+def test_document_insert_many(clean_mongo):
+    users = [
+    {'first_name': 'Alice', 'last_name': 'Smith', 'age': 25},
+    {'first_name': 'Bob', 'last_name': 'Jones', 'age': 35},
+    {'first_name': 'Charlie', 'last_name': 'Brown', 'age': 45},
+    {'first_name': 'Dave', 'last_name': 'Smith', 'age': 55}
+]
+    User = create_document_class('User', 'users')
+    User.insert_many(users)
+    stored_users = User.all()
+    assert len(stored_users) == 4
+
+def test_document_find(clean_mongo):
+    User = create_document_class('User', 'users')
+    user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user.save()
+    stored_user = User.find({'first_name': 'John'}).first()
+    assert user.first_name == stored_user.first_name
+    assert user.last_name == stored_user.last_name
+    assert user.age == stored_user.age
+
+
+def test_document_find_in(clean_mongo):
+    User = create_document_class('User', 'users')
+    user1 = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user1.save()
+    user2 = User({'first_name': 'Alice', 'last_name': 'Smith', 'age': 25})
+    user2.save()
+    user3 = User({'first_name': 'Bob', 'last_name': 'Jones', 'age': 35})
+    user3.save()
+    stored_users = User.find_in('first_name', ['John', 'Bob'])
+    assert len(stored_users) == 2
+    assert user1.first_name in [user.first_name for user in stored_users]
+    assert user2.first_name not in [user.first_name for user in stored_users]
+    assert user3.first_name in [user.first_name for user in stored_users]
+
+
+def test_document_all(clean_mongo):
+    User = create_document_class('User', 'users')
+    user1 = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user1.save()
+    user2 = User({'first_name': 'Alice', 'last_name': 'Smith', 'age': 25})
+    user2.save()
+    user3 = User({'first_name': 'Bob', 'last_name': 'Jones', 'age': 35})
+    user3.save()
+    stored_users = User.all()
+    assert len(stored_users) == 3
+    assert user1.first_name in [user.first_name for user in stored_users]
+    assert user2.first_name in [user.first_name for user in stored_users]
+    assert user3.first_name in [user.first_name for user in stored_users]
+
+
+def test_document_delete(clean_mongo):
+    User = create_document_class('User', 'users')
+    user1 = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user1.save()
+    user2 = User({'first_name': 'Alice', 'last_name': 'Smith', 'age': 25})
+    user2.save()
+    user3 = User({'first_name': 'Bob', 'last_name': 'Jones', 'age': 35})
+    user3.save()
+    User.delete({'first_name': 'Alice'})
+    stored_users = User.all()
+    assert len(stored_users) == 2
+    assert user1.first_name in [user.first_name for user in stored_users]
+    assert user2.first_name not in [user.first_name for user in stored_users]
+    assert user3.first_name in [user.first_name for user in stored_users]
+
+
+def test_document_document_count(clean_mongo):
+    User = create_document_class('User', 'users')
+    user1 = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
+    user1.save()
+    user2 = User({'first_name': 'Alice', 'last_name': 'Smith', 'age': 25})
+    user2.save()
+    user3 = User({'first_name': 'Bob', 'last_name': 'Jones', 'age': 35})
+    user3.save()
+    count = User.document_count()
+    assert count == 3
+
```

