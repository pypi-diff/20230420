# Comparing `tmp/pvsite-datamodel-0.1.7.tar.gz` & `tmp/pvsite-datamodel-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvsite-datamodel-0.1.7.tar", last modified: Mon Jan 23 17:14:44 2023, max compression
+gzip compressed data, was "pvsite-datamodel-0.1.9.tar", last modified: Thu Jan 26 14:25:28 2023, max compression
```

## Comparing `pvsite-datamodel-0.1.7.tar` & `pvsite-datamodel-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 17:14:44.124383 pvsite-datamodel-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-01-23 17:14:44.124383 pvsite-datamodel-0.1.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 17:14:44.120383 pvsite-datamodel-0.1.7/pvsite_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-23 17:14:32.000000 pvsite-datamodel-0.1.7/pvsite_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-01-23 17:14:32.000000 pvsite-datamodel-0.1.7/pvsite_datamodel/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 17:14:44.124383 pvsite-datamodel-0.1.7/pvsite_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 17:14:32.000000 pvsite-datamodel-0.1.7/pvsite_datamodel/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-01-23 17:14:32.000000 pvsite-datamodel-0.1.7/pvsite_datamodel/read/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-01-23 17:14:32.000000 pvsite-datamodel-0.1.7/pvsite_datamodel/read/site.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-01-23 17:14:32.000000 pvsite-datamodel-0.1.7/pvsite_datamodel/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-01-23 17:14:32.000000 pvsite-datamodel-0.1.7/pvsite_datamodel/sqlmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 17:14:44.124383 pvsite-datamodel-0.1.7/pvsite_datamodel/write/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 17:14:32.000000 pvsite-datamodel-0.1.7/pvsite_datamodel/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-01-23 17:14:32.000000 pvsite-datamodel-0.1.7/pvsite_datamodel/write/datetime_intervals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-01-23 17:14:32.000000 pvsite-datamodel-0.1.7/pvsite_datamodel/write/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-01-23 17:14:32.000000 pvsite-datamodel-0.1.7/pvsite_datamodel/write/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-01-23 17:14:32.000000 pvsite-datamodel-0.1.7/pvsite_datamodel/write/upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-23 17:14:32.000000 pvsite-datamodel-0.1.7/pvsite_datamodel/write/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 17:14:44.120383 pvsite-datamodel-0.1.7/pvsite_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-01-23 17:14:44.000000 pvsite-datamodel-0.1.7/pvsite_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-01-23 17:14:44.000000 pvsite-datamodel-0.1.7/pvsite_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 17:14:44.000000 pvsite-datamodel-0.1.7/pvsite_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-23 17:14:44.000000 pvsite-datamodel-0.1.7/pvsite_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-23 17:14:44.000000 pvsite-datamodel-0.1.7/pvsite_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 17:14:44.124383 pvsite-datamodel-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-01-23 17:14:33.000000 pvsite-datamodel-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 14:25:28.025949 pvsite-datamodel-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-01-26 14:25:28.025949 pvsite-datamodel-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 14:25:28.021949 pvsite-datamodel-0.1.9/pvsite_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 14:25:28.021949 pvsite-datamodel-0.1.9/pvsite_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/read/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/read/latest_forecast_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/read/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/read/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/read/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/sqlmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 14:25:28.021949 pvsite-datamodel-0.1.9/pvsite_datamodel/write/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/write/datetime_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/write/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/write/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/write/upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pvsite_datamodel/write/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 14:25:28.021949 pvsite-datamodel-0.1.9/pvsite_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-01-26 14:25:28.000000 pvsite-datamodel-0.1.9/pvsite_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-01-26 14:25:28.000000 pvsite-datamodel-0.1.9/pvsite_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 14:25:28.000000 pvsite-datamodel-0.1.9/pvsite_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-01-26 14:25:28.000000 pvsite-datamodel-0.1.9/pvsite_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-26 14:25:28.000000 pvsite-datamodel-0.1.9/pvsite_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 14:25:28.025949 pvsite-datamodel-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 14:25:28.021949 pvsite-datamodel-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-01-26 14:25:16.000000 pvsite-datamodel-0.1.9/tests/test_write.py
```

### Comparing `pvsite-datamodel-0.1.7/pvsite_datamodel/connection.py` & `pvsite-datamodel-0.1.9/pvsite_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `pvsite-datamodel-0.1.7/pvsite_datamodel/read/generation.py` & `pvsite-datamodel-0.1.9/pvsite_datamodel/read/generation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,88 @@
 """ Read pv generation functions """
 import logging
-from datetime import datetime, timezone
-from typing import List, Optional, Union
+import uuid
+from datetime import datetime
+from typing import List, Optional
 
-from sqlalchemy import desc
-from sqlalchemy.orm import Session, joinedload
+from pvsite_datamodel.sqlmodels import ClientSQL, DatetimeIntervalSQL, GenerationSQL, SiteSQL
+from sqlalchemy.orm import Session
 
-from pvsite_datamodel.sqlmodels import GenerationSQL, SiteSQL, DatetimeIntervalSQL, ClientSQL
+from .utils import filter_query_by_datetime_interval
 
 logger = logging.getLogger(__name__)
 
 
-def get_pv_generation(
+def get_pv_generation_by_client(
     session: Session,
     start_utc: Optional[datetime] = None,
     end_utc: Optional[datetime] = None,
     client_names: Optional[List[str]] = None,
-) -> Union[List[GenerationSQL]]:
+) -> List[GenerationSQL]:
     """
-    Get the generation data
+    Get the generation data by client
+
     :param session: database session
     :param end_utc: search filters < on 'datetime_utc'. Can be None
     :param start_utc: search filters >= on 'datetime_utc'. Can be None
     :param client_names: optional list of provider names
-    :return: either list of pv yields, or pv systems
+    :return:list of pv yields
     """
 
     # start main query
     query = session.query(GenerationSQL)
     query = query.join(SiteSQL)
     query = query.join(ClientSQL)
     query = query.join(DatetimeIntervalSQL)
 
-    # filter on start time
-    if start_utc is not None:
-        query = query.filter(DatetimeIntervalSQL.start_utc >= start_utc)
-
-    # filter on end time
-    if end_utc is not None:
-        query = query.filter(DatetimeIntervalSQL.end_utc < end_utc)
+    # Filter by time interval
+    query = filter_query_by_datetime_interval(query=query, start_utc=start_utc, end_utc=end_utc)
 
     if client_names is not None:
         query = query.filter(ClientSQL.client_name.in_(client_names))
 
     # order by 'created_utc' desc, so we get the latest one
     query = query.order_by(
         SiteSQL.site_uuid,
         DatetimeIntervalSQL.start_utc,
     )
 
     # get all results
     generations: List[GenerationSQL] = query.all()
 
     return generations
+
+
+def get_pv_generation_by_sites(
+    session: Session,
+    start_utc: Optional[datetime] = None,
+    end_utc: Optional[datetime] = None,
+    site_uuids: Optional[List[uuid.UUID]] = None,
+) -> List[GenerationSQL]:
+    """
+    Get the generation data by site
+
+    :param session: database session
+    :param start_utc: search filters >= on 'datetime_utc'
+    :param end_utc: search fileters < on 'datetime_utc'
+    :param site_uuids: optional list of site uuids
+    :return: list of pv yields
+    """
+
+    # start main query
+    query = session.query(GenerationSQL)
+    query = query.join(SiteSQL)
+    query = query.join(DatetimeIntervalSQL)
+
+    # Filter by time interval
+    query = filter_query_by_datetime_interval(query=query, start_utc=start_utc, end_utc=end_utc)
+
+    if site_uuids is not None:
+        query = query.filter(SiteSQL.site_uuid.in_(site_uuids))
+
+    # Order by 'created_utc' desc
+    query = query.order_by(SiteSQL.site_uuid, DatetimeIntervalSQL.start_utc)
+
+    # get all results
+    generations: List[GenerationSQL] = query.all()
+
+    return generations
```

### Comparing `pvsite-datamodel-0.1.7/pvsite_datamodel/read/site.py` & `pvsite-datamodel-0.1.9/pvsite_datamodel/read/site.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,115 @@
 """
 Functions for reading to pvsite db
 """
 
 import logging
+from typing import List, Optional
 
-from sqlalchemy.orm import Session
 from pvsite_datamodel.sqlmodels import ClientSQL, SiteSQL
+from sqlalchemy.orm import Session
 
 logger = logging.getLogger(__name__)
 
 
-def get_site_from_uuid(session: Session, site_uuid: str):
+def get_site_by_uuid(session: Session, site_uuid: str) -> SiteSQL:
     """
     Get site object from uuid.
 
-    Raise error if site does not exists
+    Raise error if site does not exist
 
     :param session: database sessions
     :param site_uuid: the site uuid
     :return: the site object
     """
     query = session.query(SiteSQL)
     query = query.filter(SiteSQL.site_uuid == site_uuid)
-    existing_site: SiteSQL = query.first()
+    existing_site: Optional[SiteSQL] = query.first()
     if existing_site is None:
         raise KeyError(f"Site uuid {site_uuid} not found in sites table")
 
     return existing_site
 
 
-def get_site(
-    session: Session, client_name: str, client_id: str
-) -> SiteSQL:
+def get_site_by_client_site_id(session: Session, client_name: str, client_site_id: int) -> SiteSQL:
     """
-    Get site from client name and client id
+    Get site from client name and client site id
 
     :param session: database sessions
     :param client_name: client name
-    :param client_id: client id
-    :return: site object
+    :param client_site_id: client's id of site
+    :return: site object, or None
     """
 
-    logger.debug(f'Getting site for {client_name=} and {client_id=}')
+    logger.debug(f"Getting {client_name}'s site {client_site_id}")
 
     # start main query
     query = session.query(SiteSQL)
     query = query.join(ClientSQL)
 
-    # select the correct client id
-    query = query.filter(SiteSQL.client_site_id == client_id)
+    # select the correct client site id
+    query = query.filter(SiteSQL.client_site_id == client_site_id)
 
     # filter on client_name
     query = query.filter(ClientSQL.client_name == client_name)
 
-    # get all results
-    site = query.first()
+    # get first result (should only be one site)
+    site: Optional[SiteSQL] = query.first()
 
     if site is None:
-        raise Exception(f"Could not find site with {client_id=} and {client_name=}")
+        raise Exception(f"Could not find site {client_site_id} from client {client_name}")
 
     return site
 
 
-def get_all_site(
-    session: Session,
+def get_site_by_client_site_name(
+    session: Session, client_name: str, client_site_name: str
 ) -> SiteSQL:
     """
-    Get all sites
+    Get site from client name and client site id
+
+    :param session: database sessions
+    :param client_name: client name
+    :param client_site_name: client's name of site
+    :return: site object, or None
+    """
+
+    logger.debug(f"Getting {client_name}'s site {client_site_name}")
+
+    # start main query
+    query = session.query(SiteSQL)
+    query = query.join(ClientSQL)
+
+    # select the correct client site name
+    query = query.filter(SiteSQL.client_site_name == client_site_name)
+
+    # filter on client_name
+    query = query.filter(ClientSQL.client_name == client_name)
+
+    # get first result (should only be one site)
+    site: Optional[SiteSQL] = query.first()
+
+    if site is None:
+        raise Exception(f"Could not find site {client_site_name} from client {client_name}")
+
+    return site
+
+
+def get_all_sites(session: Session) -> List[SiteSQL]:
+    """
+    Gets all sites from sites table
 
     :param session: database sessions
     :return: site object
     """
 
-    logger.debug(f'Getting all sites')
+    logger.debug("Getting all sites")
 
     # start main query
     query = session.query(SiteSQL)
 
     # get all results
     sites = query.all()
 
-    logger.debug(f'Found {len(sites)} sites')
+    logger.debug(f"Found {len(sites)} sites")
 
     return sites
-
```

### Comparing `pvsite-datamodel-0.1.7/pvsite_datamodel/schema.py` & `pvsite-datamodel-0.1.9/pvsite_datamodel/schema.py`

 * *Files identical despite different names*

### Comparing `pvsite-datamodel-0.1.7/pvsite_datamodel/sqlmodels.py` & `pvsite-datamodel-0.1.9/pvsite_datamodel/sqlmodels.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 SQLAlchemy definition of the pvsite database schema
 """
 
 import uuid
 from datetime import datetime
+from typing import List
 
 import sqlalchemy as sa
+from sqlalchemy import Column, DateTime
 from sqlalchemy.dialects.postgresql import FLOAT, INTEGER, REAL, TIMESTAMP, UUID
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import relationship
 from sqlalchemy.schema import UniqueConstraint
-from sqlalchemy import Column, DateTime
 
 Base = declarative_base()
 
 
 class CreatedMixin:
     """Mixin to add created datetime to model"""
 
@@ -50,17 +51,17 @@
     longitude = sa.Column(FLOAT, nullable=False)
     capacity_kw = sa.Column(REAL, nullable=False)
     updated_utc = sa.Column(TIMESTAMP, nullable=False, default=lambda: datetime.utcnow())
     ml_id = sa.Column(sa.Integer, autoincrement=True, nullable=False, unique=True)
 
     __table_args__ = (UniqueConstraint("client_site_id", client_uuid, name="idx_client"),)
 
-    forecasts = relationship("ForecastSQL")
-    latest_forecast_values = relationship("LatestForecastValueSQL")
-    generation = relationship("GenerationSQL")
+    forecasts: List["ForecastSQL"] = relationship("ForecastSQL")
+    latest_forecast_values: List["LatestForecastValueSQL"] = relationship("LatestForecastValueSQL")
+    generation: List["GenerationSQL"] = relationship("GenerationSQL")
 
 
 class GenerationSQL(Base, CreatedMixin):
     """
     Class representing the generation table.
 
     Each generation row specifies a generated power output over a
@@ -102,15 +103,15 @@
     site_uuid = sa.Column(
         UUID(as_uuid=True), sa.ForeignKey("sites.site_uuid"), nullable=False, default=uuid.uuid4
     )
 
     forecast_version = sa.Column(sa.String(32), nullable=False)
 
     # one (forecasts) to many (forecast_values)
-    forecast_values = relationship("ForecastValueSQL")
+    forecast_values: List["ForecastValueSQL"] = relationship("ForecastValueSQL")
 
 
 class ForecastValueSQL(Base, CreatedMixin):
     """
     Class representing the forecast_values table.
 
     Each forecast_value row is a prediction for the power output
@@ -169,15 +170,15 @@
 
     forecast_uuid = sa.Column(UUID(as_uuid=True), default=uuid.uuid4, nullable=False)
     site_uuid = sa.Column(
         UUID(as_uuid=True), sa.ForeignKey("sites.site_uuid"), nullable=False, default=uuid.uuid4
     )
     forecast_version = sa.Column(sa.String(32), nullable=False)
 
-    latest_forecast = relationship("SiteSQL", back_populates="latest_forecast_values")
+    latest_forecast: SiteSQL = relationship("SiteSQL", back_populates="latest_forecast_values")
 
 
 class ClientSQL(Base, CreatedMixin):
     """
     Class representing the clients table.
 
     Each client row defines a provider of site data
@@ -187,15 +188,15 @@
     """
 
     __tablename__ = "clients"
 
     client_uuid = sa.Column(UUID(as_uuid=True), default=uuid.uuid4, primary_key=True)
     client_name = sa.Column(sa.String(255), nullable=False)
 
-    sites = relationship("SiteSQL")
+    sites: List[SiteSQL] = relationship("SiteSQL")
 
 
 class DatetimeIntervalSQL(Base, CreatedMixin):
     """
     Class representing the datetime_intervals table.
 
     Each datetime_interval row defines a timespan between a start and end time
@@ -206,17 +207,17 @@
 
     __tablename__ = "datetime_intervals"
 
     datetime_interval_uuid = sa.Column(UUID(as_uuid=True), default=uuid.uuid4, primary_key=True)
     start_utc = sa.Column(TIMESTAMP, nullable=False)
     end_utc = sa.Column(TIMESTAMP, nullable=False)
 
-    generation = relationship("GenerationSQL")
-    forecast_values = relationship("ForecastValueSQL")
-    latest_forecast_values = relationship("LatestForecastValueSQL")
+    generation: List[GenerationSQL] = relationship("GenerationSQL")
+    forecast_values: List[ForecastValueSQL] = relationship("ForecastValueSQL")
+    latest_forecast_values: List[LatestForecastValueSQL] = relationship("LatestForecastValueSQL")
 
 
 class StatusSQL(Base, CreatedMixin):
     """
     Class representing the status table:
 
     Each status row defines a message reporting on the status of the
```

### Comparing `pvsite-datamodel-0.1.7/pvsite_datamodel/write/datetime_intervals.py` & `pvsite-datamodel-0.1.9/pvsite_datamodel/write/datetime_intervals.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,52 @@
+"""
+Functions for wiritng datetime intervals
+"""
+
 import datetime as dt
 import uuid
 
-from sqlalchemy import orm as sa_orm
-
-from pvsite_datamodel import sqlmodels
+from pvsite_datamodel.sqlmodels import DatetimeIntervalSQL
 from pvsite_datamodel.write.upsert import upsert
-from pvsite_datamodel.write.utils import WrittenRow, FORECAST_TIMESPAN
+from pvsite_datamodel.write.utils import FORECAST_TIMESPAN, WrittenRow
+from sqlalchemy import orm as sa_orm
 
 
 def get_or_else_create_datetime_interval(
-    session: sa_orm.Session, start_time: dt.datetime, end_time: dt.datetime = None
-) -> tuple[sqlmodels.DatetimeIntervalSQL, list[WrittenRow]]:
+    session: sa_orm.Session, start_time: dt.datetime, end_time: dt.datetime | None = None
+) -> tuple[DatetimeIntervalSQL, list[WrittenRow]]:
     """
     Gets a DatetimeInterval from the DB by start time if it exists, otherwise it creates a new entry
 
     :param session: The SQLAlchemy session used for performing db updates
     :param start_time: The start time of the datetime interval
     :param end_time: The end time of the datetime interval. Optional, defaults to the start_time
     + FORECAST_TIMESPAN
-    :return tuple(sqlmodels.DatetimeIntervalSQL, list[WrittenRow]): A tuple containing the existing
+    :return tuple(DatetimeIntervalSQL, list[WrittenRow]): A tuple containing the existing
     or created DatetimeIntervalSQL object, and a list of WrittenRow objects dictating what was
     written to the DB
     """
 
     # End time defaults to the start time + FORECAST_TIMESPAN timedelta
     if end_time is None:
         end_time = start_time + FORECAST_TIMESPAN
 
     # Check if a datetime interval exists for the input times
-    query = session.query(sqlmodels.DatetimeIntervalSQL)
-    query = query.filter(sqlmodels.DatetimeIntervalSQL.start_utc == start_time)
-    query = query.filter(sqlmodels.DatetimeIntervalSQL.end_utc == end_time)
-    existing_interval: sqlmodels.DatetimeIntervalSQL = query.first()
+    query = session.query(DatetimeIntervalSQL)
+    query = query.filter(DatetimeIntervalSQL.start_utc == start_time)
+    query = query.filter(DatetimeIntervalSQL.end_utc == end_time)
+    existing_interval: DatetimeIntervalSQL = query.first()
 
     # If it does, fetch it's uuid
     if existing_interval is not None:
         return existing_interval, []
 
     # If it doesn't, create a new one
     else:
-        datetime_interval: sqlmodels.DatetimeIntervalSQL = sqlmodels.DatetimeIntervalSQL(
+        datetime_interval: DatetimeIntervalSQL = DatetimeIntervalSQL(
             datetime_interval_uuid=uuid.uuid4(),
             start_utc=start_time,
             end_utc=end_time,
             created_utc=dt.datetime.now(tz=dt.timezone.utc),
         )
-        written_rows = upsert(session, sqlmodels.DatetimeIntervalSQL, [datetime_interval.__dict__])
-        return datetime_interval, written_rows
+        written_rows = upsert(session, DatetimeIntervalSQL, [datetime_interval.__dict__])
+        return datetime_interval, written_rows
```

### Comparing `pvsite-datamodel-0.1.7/pvsite_datamodel/write/forecast.py` & `pvsite-datamodel-0.1.9/pvsite_datamodel/write/forecast.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,22 @@
 """
 
 import datetime as dt
 import logging
 import uuid
 
 import dateutil.parser as dp
-import numpy as np
+import numpy.typing as npt
 import pandas as pd
 import sqlalchemy.orm as sa_orm
-from pvsite_datamodel import  sqlmodels
-
-# Defines the length of time over which a forecast is valid
+from pvsite_datamodel.read.site import get_site_by_uuid
+from pvsite_datamodel.sqlmodels import ForecastSQL, ForecastValueSQL
 from pvsite_datamodel.write.datetime_intervals import get_or_else_create_datetime_interval
 from pvsite_datamodel.write.upsert import upsert
 from pvsite_datamodel.write.utils import WrittenRow
-from pvsite_datamodel.read.site import get_site_from_uuid
 
 
 def insert_forecast_values(
     session: sa_orm.Session, df_forecast_values: pd.DataFrame, forecast_version: str = "0.0.0"
 ) -> list[WrittenRow]:
     """
     Inserts a dataframe of forecast values into the database.
@@ -32,36 +30,36 @@
     :return list[WrittenRow]: list of added rows to DB
     """
 
     # Track rows added to DB
     written_rows: list[WrittenRow] = []
 
     # Loop over all the unique sites that have got forecast values
-    sites: np.ndarray = df_forecast_values["pv_uuid"].unique()
+    sites: npt.ndarray[uuid.UUID] = df_forecast_values["pv_uuid"].unique()
     sql_forecast_values = []
     for site_uuid in sites:
 
         # Check whether the site id exits in the table, otherwise return an error
-        get_site_from_uuid(session=session, site_uuid=site_uuid)
+        get_site_by_uuid(session=session, site_uuid=site_uuid)
 
         # Create a forcast (sequence) for the site, and write it to db
-        forecast: sqlmodels.ForecastSQL = sqlmodels.ForecastSQL(
+        forecast: ForecastSQL = ForecastSQL(
             forecast_uuid=uuid.uuid4(),
             site_uuid=site_uuid,
             created_utc=dt.datetime.now(tz=dt.timezone.utc),
             forecast_version=forecast_version,
         )
-        newly_written_rows = upsert(session, sqlmodels.ForecastSQL, forecast.__dict__)
+        newly_written_rows = upsert(session, ForecastSQL, forecast.__dict__)
         written_rows.extend(newly_written_rows)
 
         # Get all dataframe forecast value entries for current site_uuid
         df_site: pd.DataFrame = df_forecast_values.loc[df_forecast_values["pv_uuid"] == site_uuid]
 
         # Filter the forecasted values by target_time
-        target_times: np.ndarray = df_site["target_datetime_utc"].unique()
+        target_times: npt.ndarray[dt.datetime] = df_site["target_datetime_utc"].unique()
 
         # Print a warning if there are duplicate target_times for this site's forecast
         if len(target_times) != len(df_site):
             logging.warning(
                 f"duplicate target times exist in forecast {forecast.forecast_uuid} "
                 f"for site {site_uuid}"
             )
@@ -79,23 +77,21 @@
             # For each entry with this targettime (there should only be one)
             df_target_entries: pd.DataFrame = df_site.loc[
                 df_site["target_datetime_utc"] == target_time
             ]
 
             # Create a ForecastValueSQL object for each forecast value, and surface as dict
             # TODO there might be quicker ways to do this, like go from pandas straight to a dict
-            sql_forecast_value =  sqlmodels.ForecastValueSQL(
-                    forecast_uuid=forecast.forecast_uuid,
-                    forecast_value_uuid=uuid.uuid4(),
-                    datetime_interval_uuid=datetime_interval.datetime_interval_uuid,
-                    created_utc=dt.datetime.now(tz=dt.timezone.utc),
-                    forecast_generation_kw=df_target_entries.iloc[0]["forecast_kw"],
+            sql_forecast_value = ForecastValueSQL(
+                forecast_uuid=forecast.forecast_uuid,
+                forecast_value_uuid=uuid.uuid4(),
+                datetime_interval_uuid=datetime_interval.datetime_interval_uuid,
+                created_utc=dt.datetime.now(tz=dt.timezone.utc),
+                forecast_generation_kw=df_target_entries.iloc[0]["forecast_kw"],
             ).__dict__
             sql_forecast_values.append(sql_forecast_value)
 
     # Save it to the db
-    newly_added_rows = upsert(session, sqlmodels.ForecastValueSQL, sql_forecast_values)
+    newly_added_rows = upsert(session, ForecastValueSQL, sql_forecast_values)
     written_rows.extend(newly_added_rows)
 
     return written_rows
-
-
```

### Comparing `pvsite-datamodel-0.1.7/pvsite_datamodel/write/generation.py` & `pvsite-datamodel-0.1.9/pvsite_datamodel/write/generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,85 +1,81 @@
 """
 Functions for writing to pvsite db
 """
-
+import datetime as dt
 import logging
 import uuid
 
-import numpy as np
+import numpy.typing as npt
 import pandas as pd
 import sqlalchemy.orm as sa_orm
+from pvsite_datamodel.read.site import get_site_by_uuid
 from pvsite_datamodel.sqlmodels import GenerationSQL
 
 # Defines the length of time over which a forecast is valid
 from pvsite_datamodel.write.datetime_intervals import get_or_else_create_datetime_interval
 from pvsite_datamodel.write.upsert import upsert
 from pvsite_datamodel.write.utils import WrittenRow
-from pvsite_datamodel.read.site import get_site_from_uuid
-
 
 
 def insert_generation_values(
-    session: sa_orm.Session, generation_values_df: pd.DataFrame,
+    session: sa_orm.Session,
+    generation_values_df: pd.DataFrame,
 ) -> list[WrittenRow]:
     """
     Inserts a dataframe of forecast values into the database.
 
     :param session: sqlalchemy session for interacting with the database
     :param generation_values_df: pandas dataframe with columns
     ["start_datetime_utc", "power_kw", "pv_uuid"]
     :return list[WrittenRow]: list of added rows to DB
     """
 
     # Track rows added to DB
     written_rows: list[WrittenRow] = []
 
     # Loop over all the unique sites that have got forecast values
-    site_uuids: np.ndarray = generation_values_df["site_uuid"].unique()
+    site_uuids: npt.ndarray[uuid.UUID] = generation_values_df["site_uuid"].unique()
     generation_sqls = []
     for site_uuid in site_uuids:
 
         # Check whether the site id exits in the table, otherwise return an error
-        get_site_from_uuid(session=session, site_uuid=site_uuid)
+        get_site_by_uuid(session=session, site_uuid=site_uuid)
 
         # Get all dataframe forecast value entries for current site_uuid
-        df_site: pd.DataFrame = generation_values_df.loc[generation_values_df["site_uuid"] == site_uuid]
+        df_site: pd.DataFrame = generation_values_df.loc[
+            generation_values_df["site_uuid"] == site_uuid
+        ]
 
         # Filter the forecasted values by target_time
-        start_datetimes: np.ndarray = df_site["start_datetime_utc"].unique()
+        start_datetimes: npt.ndarray[dt.datetime] = df_site["start_datetime_utc"].unique()
 
         # Print a warning if there are duplicate target_times for this site's forecast
         if len(start_datetimes) != len(df_site):
-            logging.warning(
-                f"duplicate target datetimes "
-                f"for site {site_uuid}"
-            )
+            logging.warning(f"duplicate target datetimes " f"for site {site_uuid}")
 
         # For each target time:
         for start_datetime in start_datetimes:
-
             datetime_interval, newly_added_rows = get_or_else_create_datetime_interval(
                 session=session, start_time=pd.to_datetime(start_datetime)
             )
             written_rows.extend(newly_added_rows)
 
             # For each entry with this target time:
             df_target_entries: pd.DataFrame = df_site.loc[
                 df_site["start_datetime_utc"] == start_datetimes
             ]
 
             # Create a GenerationSQL object for each generation, and surface as dict
             generation = GenerationSQL(
                 site_uuid=site_uuid,
                 generation_uuid=uuid.uuid4(),
-                power_kw=df_target_entries.iloc[0].power_kw,
+                power_kw=df_target_entries.iloc[0]["power_kw"],
                 datetime_interval_uuid=datetime_interval.datetime_interval_uuid,
             ).__dict__
             generation_sqls.append(generation)
 
         # Save it to the db
         newly_added_rows = upsert(session, GenerationSQL, generation_sqls)
         written_rows.extend(newly_added_rows)
 
     return written_rows
-
-
```

### Comparing `pvsite-datamodel-0.1.7/pvsite_datamodel/write/upsert.py` & `pvsite-datamodel-0.1.9/pvsite_datamodel/write/upsert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+"""
+Generic DB rows writer
+"""
+
 import sqlalchemy as sa
+from pvsite_datamodel.sqlmodels import Base
+from pvsite_datamodel.write.utils import WrittenRow
 from sqlalchemy import orm as sa_orm
 from sqlalchemy.dialects import postgresql as sa_psql
 
-from pvsite_datamodel import sqlmodels
-from pvsite_datamodel.write.utils import WrittenRow
-
 
-def upsert(session: sa_orm.Session, table: sqlmodels.Base, rows: list[dict]) -> list[WrittenRow]:
+def upsert(session: sa_orm.Session, table: Base, rows: list[dict]) -> list[WrittenRow]:
     """
     Upsert rows into table
 
     This functions checks the primary keys, and if present, updates the row.
     :param session: sqlalchemy Session
     :param table: the table
     :param rows: the rows we are going to update
@@ -33,8 +36,8 @@
     if not update_dict:
         raise ValueError("insert_or_update resulted in an empty update_dict")
 
     stmt = stmt.on_conflict_do_update(index_elements=primary_key_names, set_=update_dict)
     session.execute(stmt, rows)
     session.commit()
 
-    return [WrittenRow(table=table, pk_value=row[primary_key_names[0]]) for row in rows]
+    return [WrittenRow(table=table, pk_value=row[primary_key_names[0]]) for row in rows]
```

