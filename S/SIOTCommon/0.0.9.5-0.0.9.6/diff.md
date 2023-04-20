# Comparing `tmp/SIOTCommon-0.0.9.5.tar.gz` & `tmp/SIOTCommon-0.0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIOTCommon-0.0.9.5.tar", last modified: Thu Apr 20 13:04:56 2023, max compression
+gzip compressed data, was "SIOTCommon-0.0.9.6.tar", last modified: Thu Apr 20 13:30:11 2023, max compression
```

## Comparing `SIOTCommon-0.0.9.5.tar` & `SIOTCommon-0.0.9.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 13:04:56.442831 SIOTCommon-0.0.9.5/
--rw-rw-rw-   0        0        0      341 2023-04-20 13:04:56.442831 SIOTCommon-0.0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.9.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 13:04:56.421833 SIOTCommon-0.0.9.5/SIOTC/
--rw-rw-rw-   0        0        0     1851 2023-04-19 16:34:13.000000 SIOTCommon-0.0.9.5/SIOTC/DatabaseLayer.py
--rw-rw-rw-   0        0        0     6846 2023-04-19 15:57:38.000000 SIOTCommon-0.0.9.5/SIOTC/Operations.py
--rw-rw-rw-   0        0        0      443 2023-04-12 16:56:02.000000 SIOTCommon-0.0.9.5/SIOTC/__init__.py
--rw-rw-rw-   0        0        0     2650 2023-04-20 13:04:33.000000 SIOTCommon-0.0.9.5/SIOTC/helperhttps.py
-drwxrwxrwx   0        0        0        0 2023-04-20 13:04:56.440834 SIOTCommon-0.0.9.5/SIOTCommon.egg-info/
--rw-rw-rw-   0        0        0      341 2023-04-20 13:04:56.000000 SIOTCommon-0.0.9.5/SIOTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-20 13:04:56.000000 SIOTCommon-0.0.9.5/SIOTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 13:04:56.000000 SIOTCommon-0.0.9.5/SIOTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      636 2023-04-20 13:04:56.000000 SIOTCommon-0.0.9.5/SIOTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 13:04:56.000000 SIOTCommon-0.0.9.5/SIOTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 13:04:56.443831 SIOTCommon-0.0.9.5/setup.cfg
--rw-rw-rw-   0        0        0      583 2023-04-20 13:04:46.000000 SIOTCommon-0.0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 13:30:11.335346 SIOTCommon-0.0.9.6/
+-rw-rw-rw-   0        0        0      341 2023-04-20 13:30:11.334347 SIOTCommon-0.0.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.9.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 13:30:11.312349 SIOTCommon-0.0.9.6/SIOTC/
+-rw-rw-rw-   0        0        0     1843 2023-04-20 13:29:33.000000 SIOTCommon-0.0.9.6/SIOTC/DatabaseLayer.py
+-rw-rw-rw-   0        0        0     7680 2023-04-20 13:23:27.000000 SIOTCommon-0.0.9.6/SIOTC/Operations.py
+-rw-rw-rw-   0        0        0      443 2023-04-12 16:56:02.000000 SIOTCommon-0.0.9.6/SIOTC/__init__.py
+-rw-rw-rw-   0        0        0     2648 2023-04-20 13:27:13.000000 SIOTCommon-0.0.9.6/SIOTC/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-04-20 13:30:11.331364 SIOTCommon-0.0.9.6/SIOTCommon.egg-info/
+-rw-rw-rw-   0        0        0      341 2023-04-20 13:30:11.000000 SIOTCommon-0.0.9.6/SIOTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-20 13:30:11.000000 SIOTCommon-0.0.9.6/SIOTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 13:30:11.000000 SIOTCommon-0.0.9.6/SIOTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      636 2023-04-20 13:30:11.000000 SIOTCommon-0.0.9.6/SIOTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 13:30:11.000000 SIOTCommon-0.0.9.6/SIOTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 13:30:11.335346 SIOTCommon-0.0.9.6/setup.cfg
+-rw-rw-rw-   0        0        0      583 2023-04-20 13:29:57.000000 SIOTCommon-0.0.9.6/setup.py
```

### Comparing `SIOTCommon-0.0.9.5/SIOTC/DatabaseLayer.py` & `SIOTCommon-0.0.9.6/SIOTC/DatabaseLayer.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from sqlalchemy.orm import sessionmaker, scoped_session
 import os
 
 dir_path = '/home/ubuntu/config/'
 filename = 'db_config.txt'
 file_path = os.path.join(dir_path, filename)
 
-with open(file_path, 'w') as f:
+with open(file_path, 'r') as f:
     # Write the connection string to the file
-    first_line = f.readline().strip()
+    first_line = f.readline()
 
 def GetSession():
     Base = automap_base()
     engine = create_engine(first_line, echo=True)
     Base.prepare(engine, reflect=True, schema='public')
     session_factory = sessionmaker(bind=engine)
     session = scoped_session(session_factory)
```

### Comparing `SIOTCommon-0.0.9.5/SIOTC/Operations.py` & `SIOTCommon-0.0.9.6/SIOTC/Operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from SIOTC import DatabaseLayer
+from DatabaseLayer import CreateTableObject
 from sqlalchemy.exc import SQLAlchemyError, IntegrityError
 dl = DatabaseLayer
 
 def executeQuery(query_func, *args, **kwargs):
     # Get a database session and the SQLAlchemy Base object
     session, base = dl.GetSession()
     try:
@@ -68,14 +69,31 @@
         newObject = tableModel.insert().values(**newValues)
         session.execute(newObject)
         session.commit()
         # Return success
         return True
     return executeQuery(queryFunc, values)
 
+def GetFromTable(table, id):
+    def queryFunc(session, base, table, id):
+        # Get the table model from the metadata based on the provided table name
+        name = "public." + table
+        tableModel = base.metadata.tables.get(name)
+        # Check if the table exists in the metadata
+        if tableModel is None:
+            return False, 'Error: Table not found'
+        # Ensure that an ID is provided
+        assert id is not None, "Error: No ID provided"
+        # Create a query to get a row with the given ID from the table
+        query = tableModel.select().where(tableModel.c.id == id)
+        # Execute the query and return the result
+        result = session.execute(query)
+        return result.first()
+    return executeQuery(queryFunc, table, id)
+
 def RemoveFromTable(table, id):
     def queryFunc(session, base, table, id):
         # Get the table model from the metadata based on the provided table name
         name = "public." + table
         tableModel = base.metadata.tables.get(name)
         # Check if the table exists in the metadata
         if tableModel is None:
```

### Comparing `SIOTCommon-0.0.9.5/SIOTC/helperhttps.py` & `SIOTCommon-0.0.9.6/SIOTC/helperhttps.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,28 +49,28 @@
         # Get the id from the JWT
         jwt_id = get_jwt_identity()
 
         user = jwt_id
         if not user:
             return jsonify({'message': 'Current user not provided.'}), 401
 
-        user_role = op.GetTable('users').query.filter_by(id=user).first().role.name
+        user_role = op.GetSpecificFromColumnInTable(user, 'role_id', 'users')
 
         if user_role != 'System Administrator':
             return jsonify({'message': 'You do not have permission to access this endpoint.'}), 403
         return fn(*args, **kwargs)
     return wrapper
 
 
 def device_ownership_required(f):
     @wraps(f)
     def wrapper(*args, **kwargs):
         verify_jwt_in_request()
         user = get_jwt_identity()
         if not user:
             return jsonify({'message': 'Current user not provided.'}), 401
-        deviceID = op.GetTable('devices').query.filter_by(id=user).first()
+        deviceID = op.GetSpecificFromColumnInTable(user, 'user_id', 'devices')
 
         if user != deviceID.user_id:
             return jsonify({'message': 'User does not own device.'}), 403
         return f(*args, **kwargs)
     return wrapper
```

### Comparing `SIOTCommon-0.0.9.5/SIOTCommon.egg-info/requires.txt` & `SIOTCommon-0.0.9.6/SIOTCommon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.9.5/setup.py` & `SIOTCommon-0.0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SIOTCommon',
-    version='0.0.9.5',
+    version='0.0.9.6',
     packages=find_packages(),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
```

