# Comparing `tmp/orbit_database-0.99.90.tar.gz` & `tmp/orbit_database-0.99.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_database-0.99.90.tar", max compression
+gzip compressed data, was "orbit_database-0.99.91.tar", max compression
```

## Comparing `orbit_database-0.99.90.tar` & `orbit_database-0.99.91.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rwxr-xr-x   0        0        0     1087 2023-04-19 17:27:34.642403 orbit_database-0.99.90/LICENSE
--rw-r--r--   0        0        0     3697 2023-04-20 10:49:00.663307 orbit_database-0.99.90/README.md
--rwxr-xr-x   0        0        0     1917 2023-04-19 17:00:11.187330 orbit_database-0.99.90/orbit_database/__init__.py
--rw-r--r--   0        0        0     5830 2023-04-19 16:49:38.441534 orbit_database-0.99.90/orbit_database/audit.py
--rwxr-xr-x   0        0        0     2419 2022-11-15 12:12:28.501599 orbit_database-0.99.90/orbit_database/bitmap.py
--rwxr-xr-x   0        0        0    10460 2023-04-19 17:29:46.099444 orbit_database-0.99.90/orbit_database/compression.py
--rwxr-xr-x   0        0        0     1880 2023-04-19 16:50:03.108978 orbit_database-0.99.90/orbit_database/cursor.py
--rw-r--r--   0        0        0     3059 2023-04-19 16:53:13.576693 orbit_database-0.99.90/orbit_database/daemon.py
--rwxr-xr-x   0        0        0    16046 2023-04-19 16:52:09.982122 orbit_database-0.99.90/orbit_database/database.py
--rwxr-xr-x   0        0        0     4817 2022-12-19 12:08:17.236425 orbit_database-0.99.90/orbit_database/decorators.py
--rwxr-xr-x   0        0        0     9978 2023-04-19 16:54:12.783363 orbit_database-0.99.90/orbit_database/doc.py
--rwxr-xr-x   0        0        0     1104 2021-03-29 14:51:15.628206 orbit_database-0.99.90/orbit_database/exceptions.py
--rwxr-xr-x   0        0        0     3322 2023-04-19 16:54:12.787363 orbit_database-0.99.90/orbit_database/filterresult.py
--rwxr-xr-x   0        0        0    10268 2023-04-19 16:54:12.787363 orbit_database-0.99.90/orbit_database/index.py
--rwxr-xr-x   0        0        0    13295 2023-04-19 16:54:12.787363 orbit_database-0.99.90/orbit_database/invertedwordindex.py
--rwxr-xr-x   0        0        0     2896 2023-04-19 16:54:12.787363 orbit_database-0.99.90/orbit_database/manager.py
--rwxr-xr-x   0        0        0    12179 2023-04-19 16:54:12.787363 orbit_database-0.99.90/orbit_database/metadata.py
--rwxr-xr-x   0        0        0     4432 2023-04-19 16:54:12.787363 orbit_database-0.99.90/orbit_database/objectid.py
--rwxr-xr-x   0        0        0     6867 2023-04-19 16:54:12.787363 orbit_database-0.99.90/orbit_database/serialiser.py
--rwxr-xr-x   0        0        0    42290 2023-04-19 17:30:10.202902 orbit_database-0.99.90/orbit_database/table.py
--rwxr-xr-x   0        0        0      387 2023-04-19 16:53:52.467819 orbit_database-0.99.90/orbit_database/types_.py
--rw-r--r--   0        0        0      942 2023-04-20 11:49:52.657350 orbit_database-0.99.90/pyproject.toml
--rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 orbit_database-0.99.90/PKG-INFO
+-rwxr-xr-x   0        0        0     1087 2023-04-19 17:27:34.642403 orbit_database-0.99.91/LICENSE
+-rw-r--r--   0        0        0     3643 2023-04-20 12:26:13.473567 orbit_database-0.99.91/README.md
+-rwxr-xr-x   0        0        0     1917 2023-04-20 11:57:07.111022 orbit_database-0.99.91/orbit_database/__init__.py
+-rw-r--r--   0        0        0     5884 2023-04-20 12:12:44.156774 orbit_database-0.99.91/orbit_database/audit.py
+-rwxr-xr-x   0        0        0     2473 2023-04-20 12:13:03.900306 orbit_database-0.99.91/orbit_database/bitmap.py
+-rwxr-xr-x   0        0        0    10513 2023-04-20 12:13:14.200061 orbit_database-0.99.91/orbit_database/compression.py
+-rwxr-xr-x   0        0        0     1880 2023-04-19 16:50:03.108978 orbit_database-0.99.91/orbit_database/cursor.py
+-rwxr-xr-x   0        0        0    16046 2023-04-19 16:52:09.982122 orbit_database-0.99.91/orbit_database/database.py
+-rwxr-xr-x   0        0        0     4817 2022-12-19 12:08:17.236425 orbit_database-0.99.91/orbit_database/decorators.py
+-rwxr-xr-x   0        0        0    10060 2023-04-20 12:17:22.514168 orbit_database-0.99.91/orbit_database/doc.py
+-rwxr-xr-x   0        0        0     1104 2021-03-29 14:51:15.628206 orbit_database-0.99.91/orbit_database/exceptions.py
+-rwxr-xr-x   0        0        0     3322 2023-04-19 16:54:12.787363 orbit_database-0.99.91/orbit_database/filterresult.py
+-rwxr-xr-x   0        0        0    10268 2023-04-19 16:54:12.787363 orbit_database-0.99.91/orbit_database/index.py
+-rwxr-xr-x   0        0        0    13227 2023-04-20 12:18:37.912378 orbit_database-0.99.91/orbit_database/invertedwordindex.py
+-rwxr-xr-x   0        0        0     2896 2023-04-19 16:54:12.787363 orbit_database-0.99.91/orbit_database/manager.py
+-rwxr-xr-x   0        0        0    12179 2023-04-19 16:54:12.787363 orbit_database-0.99.91/orbit_database/metadata.py
+-rwxr-xr-x   0        0        0     4432 2023-04-19 16:54:12.787363 orbit_database-0.99.91/orbit_database/objectid.py
+-rwxr-xr-x   0        0        0     6867 2023-04-19 16:54:12.787363 orbit_database-0.99.91/orbit_database/serialiser.py
+-rwxr-xr-x   0        0        0    42289 2023-04-20 12:13:54.815097 orbit_database-0.99.91/orbit_database/table.py
+-rwxr-xr-x   0        0        0      387 2023-04-20 12:13:59.678982 orbit_database-0.99.91/orbit_database/types_.py
+-rw-r--r--   0        0        0      817 2023-04-20 12:22:44.374529 orbit_database-0.99.91/pyproject.toml
+-rw-r--r--   0        0        0     4124 1970-01-01 00:00:00.000000 orbit_database-0.99.91/PKG-INFO
```

### Comparing `orbit_database-0.99.90/LICENSE` & `orbit_database-0.99.91/LICENSE`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.90/README.md` & `orbit_database-0.99.91/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Orbit Database
 
-<i>This projects is the NoSQL database that underpins the Orbit Framework. The interface is written in Python3 and uses LMDB as it's back-end key/value store. Please don't be put off by the <i>written in Python</i> statement, the database performs well and in many cases surpasses what you might expect from a dedicated database engine such as MariaDB or Postgres</i>
+This project is the NoSQL database that underpins the Orbit Framework. The interface is written in Python3 and uses LMDB as it's back-end key/value store. Please don't be put off by the <i>written in Python</i> statement, the database performs well and in many cases surpasses what you might expect from a dedicated database engine such as MariaDB or Postgres.
 
 <img style="height:350px" src="https://gitlab.com/madpenguin/orbit-database/-/raw/main/images/orbit_database.png" />
 
 ### Primary design goals
 
 * Must perform well in a Python multi-processing environment
 * Must integrate well with Python based microservices
@@ -29,15 +29,14 @@
 
 ### What does it look like?
 
 As a basic example, if we wanted to have a database with a table called people, and within that table store records of individuals, we might have something like the following. We would start by setting up an ORM model for the table which consists of two classes. The first is uses to represent an individual, or a single records within the table, the second to represent a collection of individuals, or a collection of records.
 
 ```python
 from orbit_orm import BaseTable, BaseCollection
-from orbit_database import SerialiserType, Doc
 
 class PeopleTable (BaseTable):
     norm_table_name = 'people'
 
 class PeopleCollection (BaseCollection):
     table_class = PeopleTable
 ```
```

### Comparing `orbit_database-0.99.90/orbit_database/__init__.py` & `orbit_database-0.99.91/orbit_database/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #####################################################################################
 #
 #  Copyright (c) 2020 - Mad Penguin Consulting Ltd
 #
 #####################################################################################
 
-__version__ = '0.9.90'
+__version__ = '0.9.91'
 
 from orbit_database.manager import Manager
 from orbit_database.database import Database
 from orbit_database.table import Table
 from orbit_database.filterresult import FilterResult, MatchResult
 from orbit_database.index import Index
 from orbit_database.doc import Doc, JournalType
```

### Comparing `orbit_database-0.99.90/orbit_database/audit.py` & `orbit_database-0.99.91/orbit_database/audit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from enum import Enum
 from uuid import uuid4 as get_uuid
-from loguru import logger as log
 from posix_ipc import Semaphore, ExistentialError, O_CREAT, SignalError
 from time import sleep as sync_sleep
 from threading import Thread
 from orbit_database.doc import Doc
 from orbit_database.serialiser import SerialiserType
 from struct import pack, unpack
 from time import sleep
 from getpass import getuser
 import asyncio
 
+try:
+    from loguru import logger as log
+except Exception:
+    import logging as log
+
 
 class AuditEntry(Enum):
     """
     """
     NONE = 0
     APPEND = 1
     SAVE = 2
```

### Comparing `orbit_database-0.99.90/orbit_database/bitmap.py` & `orbit_database-0.99.91/orbit_database/bitmap.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from struct import pack, unpack
 from lmdb import Transaction as TXN
 import re
 from functools import reduce
-from loguru import logger as log
+
+try:
+    from loguru import logger as log
+except Exception:
+    import logging as log
 
 
 class Bitmap:
 
     CHUNK_SIZE = 1000
     PAGE_SIZE = CHUNK_SIZE * 8
```

### Comparing `orbit_database-0.99.90/orbit_database/compression.py` & `orbit_database-0.99.91/orbit_database/compression.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 from enum import Enum
 from lmdb import Transaction as TXN
 from typing import Dict, Optional
 from sys import modules
 from orbit_database.doc import Doc
 from orbit_database.decorators import wrap_reader, transparent_resize, WriteTransaction
 from orbit_database.exceptions import TableNotOpen, TrainingDataExists
-from loguru import logger as log
 
+try:
+    from loguru import logger as log
+except Exception:
+    import logging as log
 
 try:
     from zstandard import ZstdCompressionDict, ZstdCompressor, ZstdDecompressor, \
         train_dictionary, ZstdError
 except ImportError:   # pragma: no cover
     pass  # pragma: no cover
```

### Comparing `orbit_database-0.99.90/orbit_database/cursor.py` & `orbit_database-0.99.91/orbit_database/cursor.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.90/orbit_database/daemon.py` & `orbit_database-0.99.91/orbit_database/filterresult.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,93 @@
-"""
+#####################################################################################
+#
+#  Copyright (c) 2020 - Mad Penguin Consulting Ltd
+#
+#####################################################################################
+from __future__ import annotations
+from lmdb import Transaction as TXN, Cursor
+from typing import TYPE_CHECKING, ClassVar
+from orbit_database.index import Index
+from orbit_database.doc import Doc
+
+
+if TYPE_CHECKING:
+    from .table import Table  # pragma: no cover
+
+
+class FilterResult:
+    """
+    Wrapper for results returned from the "filter" API call, use the "doc" method
+    to access the resulting data.
+    """
 
-    Copyright (c) 2021 - Mad Penguin Consulting Ltd
+    def __init__(self, table: Table, index: Index, cursor: Cursor, txn: TXN) -> None:
+        """
+        Instantiate a FilterResult instance, used by the filter() API call to
+        return a result to the caller. If we're searching on a primary key then
+        we effectively have the data we want already, but if we're searching on
+        an index, we implement a lazy-loader, so we store the real primary key
+        OID, then use it to recover the actual record when the user calls the
+        "doc" method.
+
+        index - the index we were searching on (None for primary key)
+        cursor - the LMDB cursor object we're using
+        txn - a transaction to wrap this operation
+        ---
+        Properties:
+
+        o count   the number of duplicate keys that apply to this result
+        o key     the key used to acquire this result
+        """
+        self._txn = txn
+        self._table = table
+        if index is None:
+            self._oid = cursor.key()
+            self._dat = cursor.value()
+        else:
+            self.key = cursor.key()  # this is used by filter() / context
+            self._oid = cursor.value()
+            self._dat = None
+            self.count = cursor.count() if index.duplicates else 1
+
+    @property
+    def oid(self) -> str:
+        return self._oid  # pragma: no cover
+
+    @property
+    def doc(self) -> ClassVar:
+        """
+        Returns the uncompressed data associted with this search result.
+        """
+        if not self._dat:
+            self._dat = self._txn.get(self._oid, db=self._table._db)
+        return self._table._cls(None, self._oid, self._table._decompressor(self._dat), integerkey=self._table.integerkey)
 
-"""
-from orbit_database import Manager
-from multiprocessing import Process
-from posix_ipc import Semaphore, O_CREAT, BusyError, SignalError
-from orbit_database import FullTextHandler
-from signal import signal, SIGTERM
-from time import sleep
-from struct import unpack
-from orbit_database import Progress, ProgressType
-from os import getpid
-
-try:
-    from loguru import logger as log
-except Exception:
-    import logging as log
-
-
-class Daemon:
-
-    MAX_BATCH_SIZE = 5000
-
-    def __init__(self, path, config, conf):
-        self._path = path
-        self._config = config
-        self._conf = conf
-        self._proc = Process(target=self.run, daemon=False)
-        signal(SIGTERM, self.handler)
-
-    def handler(self, *args):
-        self._running = False
-
-    def start(self):
-        self._proc.start()
-
-    def stop(self):
-        self._proc.terminate()
-        self._proc.join()
-
-    def run(self):
-        """
-        """
-        log.debug(f'[daemon] running (pid={getpid()}')
-        self._running = True
-        self._database = Manager().database('db', self._path, config=self._config)
-        self._env = self._database.env
-        self._semaphore = Semaphore(self._database.replication.semaphore_name, flags=O_CREAT)
-        try:
-            while self._running:
-                try:
-                    self._semaphore.acquire()
-                except KeyboardInterrupt:
-                    self._running = False
-                    continue
-                except (SignalError, BusyError):
-                    sleep(0.1)
-                    continue
-
-                journal = self._database.replication.table
-                documents = 0
-                batch = journal.records()
-                self._conf['outgoing'].put(Progress(ProgressType.MAX, 'INDX', batch))
-                while journal.records():
-                    keys = []
-                    page_size = min(journal.records(), self.MAX_BATCH_SIZE)
-                    documents += page_size
-                    keys = [unpack('=Q', result.oid)[0] for result in journal.filter(page_size=page_size)]
-                    log.debug(f'submitting batch of {page_size} documents to indexer (of {journal.records()})')
-                    with FullTextHandler(self._path, self._database) as handler:
-                        for key in keys:
-                            self._conf['outgoing'].put(Progress(ProgressType.PROGRESS, 'INDX', 1))
-                            handler.run(key)
-                    journal.delete(keys)
-                self._conf['outgoing'].put(Progress(ProgressType.FLUSH, 'INDX'))
-                sleep(1)
-                self._conf['outgoing'].put(Progress(ProgressType.END, 'INDX'))
-
-                for i in range(documents - 1):
-                    try:
-                        self._semaphore.acquire(timeout=0)
-                    except (SignalError, BusyError):
-                        break
-        except KeyboardInterrupt:
-            pass
-        log.debug(f'[daemon] stopped (pid={getpid()}')
+    @property
+    def raw(self) -> bytes:
+        """
+        Returns the raw serialised data directly from the KV store
+        """
+        if not self._dat:
+            self._dat = self._txn.get(self._oid, db=self._table._db)  # pragma: no cover
+        return self._dat
+
+
+class MatchResult:
+    """
+    Wrapper for full text search results, used by fulltext.py to (lazy) return
+    the matched object, and the search results information.
+    """
+
+    def __init__(self, table: Table, index: Index, result: int, txn: Transaction) -> None:
+        self._table = table
+        self._index = index
+        self._result = result
+        self._txn = txn
+        self._dat = None
+
+    @property
+    def doc(self) -> Doc:
+        if not self._dat:
+            self._oid = self._index.get_oid(self._result, self._txn)
+            self._dat = self._txn.get(self._oid, db=self._table._db)
+        return Doc(None, self._oid, self._table._decompressor(self._dat), integerkey=self._table.integerkey)
```

### Comparing `orbit_database-0.99.90/orbit_database/database.py` & `orbit_database-0.99.91/orbit_database/database.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.90/orbit_database/decorators.py` & `orbit_database-0.99.91/orbit_database/decorators.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.90/orbit_database/doc.py` & `orbit_database-0.99.91/orbit_database/doc.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 #####################################################################################
 from __future__ import annotations
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Optional, KeysView, ItemsView, ValuesView, Dict, List
 from lmdb import Transaction as TXN
 from struct import pack, unpack
 from orbit_database.objectid import ObjectId
-from loguru import logger as log
+try:
+    from loguru import logger as log
+except ModuleNotFoundError:
+    import logging as log
+    log.info("OK")
 
 if TYPE_CHECKING:
     from .table import Table  # pragma: no cover
 
 
 class JournalType(Enum):
     """
```

### Comparing `orbit_database-0.99.90/orbit_database/exceptions.py` & `orbit_database-0.99.91/orbit_database/exceptions.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.90/orbit_database/index.py` & `orbit_database-0.99.91/orbit_database/index.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.90/orbit_database/invertedwordindex.py` & `orbit_database-0.99.91/orbit_database/invertedwordindex.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 from functools import wraps
 from time import time
 from os import times
 
 try:
     from loguru import logger as log
 except Exception:  # pragma: no cover
-    from logging import log  # pragma: no cover
-    log.info('LOGURU not installed, using default python logger')
+    import logging as log  # pragma: no cover
 
 
 class InvertedWordIndex:
 
     REMOVE_TOKENS = ['iwx']
     MAX_WORDS = 65535
     MAX_WORD_SIZE = 128
```

### Comparing `orbit_database-0.99.90/orbit_database/manager.py` & `orbit_database-0.99.91/orbit_database/manager.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.90/orbit_database/metadata.py` & `orbit_database-0.99.91/orbit_database/metadata.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.90/orbit_database/objectid.py` & `orbit_database-0.99.91/orbit_database/objectid.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.90/orbit_database/serialiser.py` & `orbit_database-0.99.91/orbit_database/serialiser.py`

 * *Files identical despite different names*

### Comparing `orbit_database-0.99.90/orbit_database/table.py` & `orbit_database-0.99.91/orbit_database/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from orbit_database.filterresult import FilterResult, MatchResult
 from orbit_database.decorators import wrap_reader, wrap_reader_yield, WriteTransaction, ReadTransaction, transparent_resize
 from orbit_database.exceptions import IndexAlreadyExists, DocumentDoesntExist, InvalidKeySpecifier, NoSuchIndex
 from orbit_database.types_ import Config, OID, OIDS
 from pathlib import Path
 from operator import gt as greater, lt as less
 
-
 try:
     from loguru import logger as log
 except Exception:  # pragma: no cover
     from logging import log  # pragma: no cover
 
 
 ZERO = 0
```

### Comparing `orbit_database-0.99.90/pyproject.toml` & `orbit_database-0.99.91/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 [tool.poetry]
 name = "orbit_database"
-version = "0.99.90"
+version = "0.99.91"
 description = "Database library for Python based on LMDB storage engine"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-lmdb = "*"
-loguru = "*"
-ujson = "*"
 posix-ipc = "^1.1.1"
+lmdb = "^1.4.1"
 
 [tool.poetry.dev-dependencies]
 pipenv = "*"
 pytest = "*"
 pytest-cov = "*"
 coverage = "*"
-twine = "*"
 ujson = "*"
 orjson = "*"
 zstandard = "*"
 python-snappy = "*"
-deepdiff = {extras = [ "murmur",], version = "*"}
 tox = "*"
-setuptools-pipfile = "*"
 lxml = "*"
 nltk = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = "^0.20.3"
 bs4 = "^0.0.1"
-loguru = "^0.7.0"
 pytest = "^7.3.1"
 poetry = "^1.4.2"
 pip = "^23.1"
 pytest-cov = "^4.0.0"
 coverage = "^7.2.3"
 coverage-badge = "^1.1.0"
 unittest2 = "^1.1.0"
```

### Comparing `orbit_database-0.99.90/PKG-INFO` & `orbit_database-0.99.91/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: orbit-database
-Version: 0.99.90
+Version: 0.99.91
 Summary: Database library for Python based on LMDB storage engine
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: lmdb
-Requires-Dist: loguru
+Requires-Dist: lmdb (>=1.4.1,<2.0.0)
 Requires-Dist: posix-ipc (>=1.1.1,<2.0.0)
-Requires-Dist: ujson
 Description-Content-Type: text/markdown
 
 # Orbit Database
 
-<i>This projects is the NoSQL database that underpins the Orbit Framework. The interface is written in Python3 and uses LMDB as it's back-end key/value store. Please don't be put off by the <i>written in Python</i> statement, the database performs well and in many cases surpasses what you might expect from a dedicated database engine such as MariaDB or Postgres</i>
+This project is the NoSQL database that underpins the Orbit Framework. The interface is written in Python3 and uses LMDB as it's back-end key/value store. Please don't be put off by the <i>written in Python</i> statement, the database performs well and in many cases surpasses what you might expect from a dedicated database engine such as MariaDB or Postgres.
 
 <img style="height:350px" src="https://gitlab.com/madpenguin/orbit-database/-/raw/main/images/orbit_database.png" />
 
 ### Primary design goals
 
 * Must perform well in a Python multi-processing environment
 * Must integrate well with Python based microservices
@@ -45,15 +43,14 @@
 
 ### What does it look like?
 
 As a basic example, if we wanted to have a database with a table called people, and within that table store records of individuals, we might have something like the following. We would start by setting up an ORM model for the table which consists of two classes. The first is uses to represent an individual, or a single records within the table, the second to represent a collection of individuals, or a collection of records.
 
 ```python
 from orbit_orm import BaseTable, BaseCollection
-from orbit_database import SerialiserType, Doc
 
 class PeopleTable (BaseTable):
     norm_table_name = 'people'
 
 class PeopleCollection (BaseCollection):
     table_class = PeopleTable
 ```
```

