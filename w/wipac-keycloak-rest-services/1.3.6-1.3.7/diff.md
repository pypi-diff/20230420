# Comparing `tmp/wipac-keycloak-rest-services-1.3.6.tar.gz` & `tmp/wipac-keycloak-rest-services-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-keycloak-rest-services-1.3.6.tar", last modified: Wed Feb 22 19:23:48 2023, max compression
+gzip compressed data, was "wipac-keycloak-rest-services-1.3.7.tar", last modified: Thu Apr 20 19:26:38 2023, max compression
```

## Comparing `wipac-keycloak-rest-services-1.3.6.tar` & `wipac-keycloak-rest-services-1.3.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 19:23:48.773623 wipac-keycloak-rest-services-1.3.6/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-02-22 19:23:45.000000 wipac-keycloak-rest-services-1.3.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4044 2023-02-22 19:23:48.773623 wipac-keycloak-rest-services-1.3.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3036 2023-02-22 19:23:45.000000 wipac-keycloak-rest-services-1.3.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 19:23:48.773623 wipac-keycloak-rest-services-1.3.6/krs/
--rw-r--r--   0 root         (0) root         (0)      513 2023-02-22 19:23:46.000000 wipac-keycloak-rest-services-1.3.6/krs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20266 2023-02-22 19:23:45.000000 wipac-keycloak-rest-services-1.3.6/krs/apps.py
--rw-r--r--   0 root         (0) root         (0)    15733 2023-02-22 19:23:45.000000 wipac-keycloak-rest-services-1.3.6/krs/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     2870 2023-02-22 19:23:45.000000 wipac-keycloak-rest-services-1.3.6/krs/email.py
--rw-r--r--   0 root         (0) root         (0)    10971 2023-02-22 19:23:45.000000 wipac-keycloak-rest-services-1.3.6/krs/groups.py
--rw-r--r--   0 root         (0) root         (0)     8766 2023-02-22 19:23:45.000000 wipac-keycloak-rest-services-1.3.6/krs/institutions.py
--rw-r--r--   0 root         (0) root         (0)    22784 2023-02-22 19:23:45.000000 wipac-keycloak-rest-services-1.3.6/krs/ldap.py
--rw-r--r--   0 root         (0) root         (0)     5722 2023-02-22 19:23:45.000000 wipac-keycloak-rest-services-1.3.6/krs/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-02-22 19:23:45.000000 wipac-keycloak-rest-services-1.3.6/krs/token.py
--rw-r--r--   0 root         (0) root         (0)     8841 2023-02-22 19:23:45.000000 wipac-keycloak-rest-services-1.3.6/krs/users.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-02-22 19:23:48.773623 wipac-keycloak-rest-services-1.3.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2023-02-22 19:23:45.000000 wipac-keycloak-rest-services-1.3.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 19:23:48.773623 wipac-keycloak-rest-services-1.3.6/wipac_keycloak_rest_services.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4044 2023-02-22 19:23:48.000000 wipac-keycloak-rest-services-1.3.6/wipac_keycloak_rest_services.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      441 2023-02-22 19:23:48.000000 wipac-keycloak-rest-services-1.3.6/wipac_keycloak_rest_services.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-22 19:23:48.000000 wipac-keycloak-rest-services-1.3.6/wipac_keycloak_rest_services.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      214 2023-02-22 19:23:48.000000 wipac-keycloak-rest-services-1.3.6/wipac_keycloak_rest_services.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-02-22 19:23:48.000000 wipac-keycloak-rest-services-1.3.6/wipac_keycloak_rest_services.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:26:38.581016 wipac-keycloak-rest-services-1.3.7/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-04-20 19:26:34.000000 wipac-keycloak-rest-services-1.3.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-04-20 19:26:38.581016 wipac-keycloak-rest-services-1.3.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-04-20 19:26:34.000000 wipac-keycloak-rest-services-1.3.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:26:38.581016 wipac-keycloak-rest-services-1.3.7/krs/
+-rw-r--r--   0 root         (0) root         (0)      513 2023-04-20 19:26:35.000000 wipac-keycloak-rest-services-1.3.7/krs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20266 2023-04-20 19:26:34.000000 wipac-keycloak-rest-services-1.3.7/krs/apps.py
+-rw-r--r--   0 root         (0) root         (0)    15733 2023-04-20 19:26:34.000000 wipac-keycloak-rest-services-1.3.7/krs/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-04-20 19:26:34.000000 wipac-keycloak-rest-services-1.3.7/krs/email.py
+-rw-r--r--   0 root         (0) root         (0)    10971 2023-04-20 19:26:34.000000 wipac-keycloak-rest-services-1.3.7/krs/groups.py
+-rw-r--r--   0 root         (0) root         (0)     8766 2023-04-20 19:26:34.000000 wipac-keycloak-rest-services-1.3.7/krs/institutions.py
+-rw-r--r--   0 root         (0) root         (0)    22784 2023-04-20 19:26:34.000000 wipac-keycloak-rest-services-1.3.7/krs/ldap.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 19:26:34.000000 wipac-keycloak-rest-services-1.3.7/krs/py.typed
+-rw-r--r--   0 root         (0) root         (0)     5722 2023-04-20 19:26:34.000000 wipac-keycloak-rest-services-1.3.7/krs/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-04-20 19:26:34.000000 wipac-keycloak-rest-services-1.3.7/krs/token.py
+-rw-r--r--   0 root         (0) root         (0)     9060 2023-04-20 19:26:34.000000 wipac-keycloak-rest-services-1.3.7/krs/users.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-04-20 19:26:38.585016 wipac-keycloak-rest-services-1.3.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-20 19:26:34.000000 wipac-keycloak-rest-services-1.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 19:26:38.581016 wipac-keycloak-rest-services-1.3.7/wipac_keycloak_rest_services.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-04-20 19:26:38.000000 wipac-keycloak-rest-services-1.3.7/wipac_keycloak_rest_services.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      454 2023-04-20 19:26:38.000000 wipac-keycloak-rest-services-1.3.7/wipac_keycloak_rest_services.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 19:26:38.000000 wipac-keycloak-rest-services-1.3.7/wipac_keycloak_rest_services.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      200 2023-04-20 19:26:38.000000 wipac-keycloak-rest-services-1.3.7/wipac_keycloak_rest_services.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-20 19:26:38.000000 wipac-keycloak-rest-services-1.3.7/wipac_keycloak_rest_services.egg-info/top_level.txt
```

### Comparing `wipac-keycloak-rest-services-1.3.6/LICENSE` & `wipac-keycloak-rest-services-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.6/PKG-INFO` & `wipac-keycloak-rest-services-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-keycloak-rest-services
-Version: 1.3.6
+Version: 1.3.7
 Summary: Services surrounding KeyCloak, that use the REST API to read/update state
 Home-page: https://github.com/WIPACrepo/keycloak-rest-services
 Download-URL: https://pypi.org/project/wipac-keycloak-rest-services/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_9b_pusek_/tmphnw94r9y_TarContainer/0/2", line 93, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_9b_pusek_/tmphnw94r9y_TarContainer/0/2", line 93, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.3.6
+Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.3.7
 Summary: Services surrounding KeyCloak, that use the REST API to read/update
 state Home-page: https://github.com/WIPACrepo/keycloak-rest-services Download-
 URL: https://pypi.org/project/wipac-keycloak-rest-services/ Author: WIPAC
 Developers Author-email: developers@icecube.wisc.edu License: MIT Project-URL:
 Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues Project-
 URL: Source, https://github.com/WIPACrepo/keycloak-rest-services Keywords:
 keycloak,rest,tools,utilities Classifier: Development Status :: 5 - Production/
```

### Comparing `wipac-keycloak-rest-services-1.3.6/README.md` & `wipac-keycloak-rest-services-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.6/krs/__init__.py` & `wipac-keycloak-rest-services-1.3.7/krs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.3.6"
+__version__ = "1.3.7"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-keycloak-rest-services-1.3.6/krs/apps.py` & `wipac-keycloak-rest-services-1.3.7/krs/apps.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.6/krs/bootstrap.py` & `wipac-keycloak-rest-services-1.3.7/krs/bootstrap.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.6/krs/email.py` & `wipac-keycloak-rest-services-1.3.7/krs/email.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.6/krs/groups.py` & `wipac-keycloak-rest-services-1.3.7/krs/groups.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.6/krs/institutions.py` & `wipac-keycloak-rest-services-1.3.7/krs/institutions.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.6/krs/ldap.py` & `wipac-keycloak-rest-services-1.3.7/krs/ldap.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.6/krs/rabbitmq.py` & `wipac-keycloak-rest-services-1.3.7/krs/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.6/krs/token.py` & `wipac-keycloak-rest-services-1.3.7/krs/token.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.6/krs/users.py` & `wipac-keycloak-rest-services-1.3.7/krs/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 User actions against Keycloak.
 """
 import asyncio
 import logging
 
+import requests.exceptions
+
 from .token import get_rest_client
 
 logger = logging.getLogger('krs.users')
 
 
 def _fix_attributes(user):
     """
@@ -97,15 +99,19 @@
             'firstName': first_name,
             'lastName': last_name,
             'username': username,
             'enabled': True,
             'attributes': attribs,
         }
 
-        await rest_client.request('POST', '/users', user)
+        try:
+            await rest_client.request('POST', '/users', user)
+        except requests.exceptions.HTTPError as e:
+            logger.error('Keycloak returned HTTP error %r: %r', e.response.status_code, e.response.text)
+            raise
         logger.info(f'user "{username}" created')
     else:
         logger.info(f'user "{username}" already exists')
 
 
 async def modify_user(username, first_name=None, last_name=None, email=None, attribs=None, actions=None, actions_reset=False, rest_client=None):
     """
```

### Comparing `wipac-keycloak-rest-services-1.3.6/setup.cfg` & `wipac-keycloak-rest-services-1.3.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -33,25 +33,25 @@
 	Tracker = https://github.com/WIPACrepo/keycloak-rest-services/issues
 	Source = https://github.com/WIPACrepo/keycloak-rest-services
 
 [semantic_release]
 version_variable = krs/__init__.py:__version__
 upload_to_pypi = True
 patch_without_tag = True
-commit_parser = semantic_release.history.tag_parser
-minor_tag = [minor]
-fix_tag = [fix]
+commit_parser = semantic_release.history.emoji_parser
+major_emoji = [major]
+minor_emoji = [minor]
+patch_emoji = [fix], [patch]
 branch = master
 
 [options]
 install_requires = 
 	aio_pika
 	ldap3
 	motor
-	pyjwt[crypto]
 	requests
 	wipac-dev-tools
 	wipac-rest-tools
 python_requires = >=3.8, <3.12
 packages = find:
 
 [options.extras_require]
```

### Comparing `wipac-keycloak-rest-services-1.3.6/wipac_keycloak_rest_services.egg-info/PKG-INFO` & `wipac-keycloak-rest-services-1.3.7/wipac_keycloak_rest_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-keycloak-rest-services
-Version: 1.3.6
+Version: 1.3.7
 Summary: Services surrounding KeyCloak, that use the REST API to read/update state
 Home-page: https://github.com/WIPACrepo/keycloak-rest-services
 Download-URL: https://pypi.org/project/wipac-keycloak-rest-services/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_9b_pusek_/tmphnw94r9y_TarContainer/0/18", line 93, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_9b_pusek_/tmphnw94r9y_TarContainer/0/18", line 93, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.3.6
+Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.3.7
 Summary: Services surrounding KeyCloak, that use the REST API to read/update
 state Home-page: https://github.com/WIPACrepo/keycloak-rest-services Download-
 URL: https://pypi.org/project/wipac-keycloak-rest-services/ Author: WIPAC
 Developers Author-email: developers@icecube.wisc.edu License: MIT Project-URL:
 Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues Project-
 URL: Source, https://github.com/WIPACrepo/keycloak-rest-services Keywords:
 keycloak,rest,tools,utilities Classifier: Development Status :: 5 - Production/
```

