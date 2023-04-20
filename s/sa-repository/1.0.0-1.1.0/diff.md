# Comparing `tmp/sa_repository-1.0.0.tar.gz` & `tmp/sa_repository-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sa_repository-1.0.0.tar", max compression
+gzip compressed data, was "sa_repository-1.1.0.tar", max compression
```

## Comparing `sa_repository-1.0.0.tar` & `sa_repository-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-02-13 22:38:44.227169 sa_repository-1.0.0/LICENSE
--rw-r--r--   0        0        0      869 2023-03-02 22:12:13.947089 sa_repository-1.0.0/README.md
--rw-r--r--   0        0        0      848 2023-04-07 20:22:41.527326 sa_repository-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       57 2023-04-07 20:22:59.470188 sa_repository-1.0.0/sa_repository/__init__.py
--rw-r--r--   0        0        0     4269 2023-04-03 21:36:31.615729 sa_repository-1.0.0/sa_repository/base.py
--rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 sa_repository-1.0.0/setup.py
--rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 sa_repository-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-13 22:38:44.227169 sa_repository-1.1.0/LICENSE
+-rw-r--r--   0        0        0      869 2023-03-02 22:12:13.947089 sa_repository-1.1.0/README.md
+-rw-r--r--   0        0        0     1088 2023-04-20 21:21:27.249019 sa_repository-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-04-20 21:03:35.824517 sa_repository-1.1.0/sa_repository/__init__.py
+-rw-r--r--   0        0        0     4699 2023-04-20 21:03:00.923292 sa_repository-1.1.0/sa_repository/base.py
+-rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 sa_repository-1.1.0/setup.py
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 sa_repository-1.1.0/PKG-INFO
```

### Comparing `sa_repository-1.0.0/LICENSE` & `sa_repository-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sa_repository-1.0.0/README.md` & `sa_repository-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sa_repository-1.0.0/pyproject.toml` & `sa_repository-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 [tool.poetry]
 name = "sa-repository"
-version = "1.0.0"
+version = "1.1.0"
 description = "Repository pattern for SQLAlchemy models"
 readme = "README.md"
 authors = ["Gasper3 <trzecik65@gmail.com>"]
 homepage = "https://github.com/Gasper3/sa-repository"
 repository = "https://github.com/Gasper3/sa-repository"
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "Topic :: Database",
+]
+license = "MIT"
+keywords = ["sqlalchemy", "repository-pattern", "orm", "repository"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sqlalchemy = "^2.0.2"
 more-itertools = "^9.1.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.1.0"
 pytest = "*"
 black = "^23.1.0"
 factory-boy = "^3.2.1"
 psycopg2 = "^2.9.5"
 mypy = "^1.1.1"
+pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `sa_repository-1.0.0/sa_repository/base.py` & `sa_repository-1.1.0/sa_repository/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as t
 
 import more_itertools
 import sqlalchemy as sa
 from sqlalchemy import ColumnElement
 from sqlalchemy.exc import NoResultFound
-from sqlalchemy.orm import Session, DeclarativeBase
+from sqlalchemy.orm import DeclarativeBase, Session, joinedload
 
 __all__ = ['BaseRepository']
 
 T = t.TypeVar('T', bound=DeclarativeBase)
 
 
 class BaseRepository(t.Generic[T]):
@@ -66,39 +66,48 @@
 
     def get_query(
         self,
         *where_args: ColumnElement,
         joins: list | None = None,
         select: t.Tuple[ColumnElement] | None = None,
         order_by=None,
+        joined_loads: tuple | None = None,
     ) -> sa.Select:
-        query = sa.select(select if select else self.MODEL_CLASS).where(*where_args).order_by(order_by)
+        query = sa.select(*select) if select else sa.select(self.MODEL_CLASS)
+        query = query.where(*where_args).order_by(order_by)
 
         if joins:
             for join in joins:
                 query = query.join(*join) if isinstance(join, tuple) else query.join(join)
+
+        if joined_loads:
+            query = query.options(*[joinedload(j) for j in joined_loads])
         return query
 
     # read methods
-    def get(self, *where: ColumnElement, joins: list | None = None) -> T:
+    def get(self, *where: ColumnElement, joins: list | None = None, joined_loads: tuple | None = None) -> T:
         """
         :returns: one
         :raises NoResultFound: if nothing was found
         :raises MultipleResultsFound: if found more than one record
         """
-        stmt = self.get_query(*where, joins=joins)
-        return self.session.scalars(stmt).one()
+        stmt = self.get_query(*where, joins=joins, joined_loads=joined_loads)
+        return self.session.scalars(stmt).unique().one()
 
-    def get_or_none(self, *where: ColumnElement, joins: list | None = None) -> T | None:
-        stmt = self.get_query(*where, joins=joins)
-        return self.session.scalars(stmt).one_or_none()
-
-    def find(self, *where, joins: list | None = None, order_by=None) -> t.Sequence[T]:
-        stmt = self.get_query(*where, joins=joins, order_by=order_by)
-        return self.session.scalars(stmt).all()
+    def get_or_none(
+        self, *where: ColumnElement, joins: list | None = None, joined_loads: tuple | None = None
+    ) -> T | None:
+        stmt = self.get_query(*where, joins=joins, joined_loads=joined_loads)
+        return self.session.scalars(stmt).unique().one_or_none()
+
+    def find(
+        self, *where, joins: list | None = None, order_by=None, joined_loads: tuple | None = None
+    ) -> t.Sequence[T]:
+        stmt = self.get_query(*where, joins=joins, order_by=order_by, joined_loads=joined_loads)
+        return self.session.scalars(stmt).unique().all()
 
     # write methods
     def create(self, **params) -> T:
         obj = self.MODEL_CLASS(**params)
         self._flush_obj(obj)
         return obj
```

### Comparing `sa_repository-1.0.0/setup.py` & `sa_repository-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['more-itertools>=9.1.0,<10.0.0', 'sqlalchemy>=2.0.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'sa-repository',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': 'Repository pattern for SQLAlchemy models',
     'long_description': "# SQLAlchemy Repository for models\n![tests workflow](https://github.com/Gasper3/sa-repository/actions/workflows/actions.yml/badge.svg)\n\nThis project contains simple Repository pattern for SQLAlchemy models.  \nAll you need to do is:\n1. Install this package `python -m pip install sa-repository`\n2. Use it in your project\n    ```python\n    from sa_repository import BaseRepository\n    from models import YourSAModel\n    \n    class SomeModelRepository(BaseRepository[YourSAModel]):\n        pass\n    ```\n\nBase class contains some general methods to simplify your work with sqlalchemy models e.x\n```python\nvar = SomeModelRepository(session).get(YourSAModel.attr == 'some_value')\n```\n\nIf you don't want to create new repository classes, you can use `get_repository_from_model` method\n```python\nrepository = BaseRepository.get_repository_from_model(db_session, SomeModel)\n```\n",
     'author': 'Gasper3',
     'author_email': 'trzecik65@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Gasper3/sa-repository',
```

### Comparing `sa_repository-1.0.0/PKG-INFO` & `sa_repository-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: sa-repository
-Version: 1.0.0
+Version: 1.1.0
 Summary: Repository pattern for SQLAlchemy models
 Home-page: https://github.com/Gasper3/sa-repository
+License: MIT
+Keywords: sqlalchemy,repository-pattern,orm,repository
 Author: Gasper3
 Author-email: trzecik65@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: sqlalchemy (>=2.0.2,<3.0.0)
 Project-URL: Repository, https://github.com/Gasper3/sa-repository
 Description-Content-Type: text/markdown
 
 # SQLAlchemy Repository for models
 ![tests workflow](https://github.com/Gasper3/sa-repository/actions/workflows/actions.yml/badge.svg)
```

