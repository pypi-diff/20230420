# Comparing `tmp/python_keycloak_async-2.16.0.post7.tar.gz` & `tmp/python_keycloak_async-2.16.0.post8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_keycloak_async-2.16.0.post7.tar", max compression
+gzip compressed data, was "python_keycloak_async-2.16.0.post8.tar", max compression
```

## Comparing `python_keycloak_async-2.16.0.post7.tar` & `python_keycloak_async-2.16.0.post8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     5559 2023-04-20 06:46:13.713909 python_keycloak_async-2.16.0.post7/CHANGELOG.md
--rw-r--r--   0        0        0     3192 2023-04-20 06:46:13.713909 python_keycloak_async-2.16.0.post7/CONTRIBUTING.md
--rw-r--r--   0        0        0     1111 2023-04-20 06:46:13.713909 python_keycloak_async-2.16.0.post7/LICENSE
--rw-r--r--   0        0        0    15646 2023-04-20 06:46:13.713909 python_keycloak_async-2.16.0.post7/README.md
--rw-r--r--   0        0        0     2428 2023-04-20 06:46:32.197875 python_keycloak_async-2.16.0.post7/pyproject.toml
--rw-r--r--   0        0        0     2381 2023-04-20 06:46:13.713909 python_keycloak_async-2.16.0.post7/src/keycloak/__init__.py
--rw-r--r--   0        0        0     1197 2023-04-20 06:46:13.713909 python_keycloak_async-2.16.0.post7/src/keycloak/_version.py
--rw-r--r--   0        0        0     3748 2023-04-20 06:46:13.713909 python_keycloak_async-2.16.0.post7/src/keycloak/authorization/__init__.py
--rw-r--r--   0        0        0     4421 2023-04-20 06:46:13.713909 python_keycloak_async-2.16.0.post7/src/keycloak/authorization/permission.py
--rw-r--r--   0        0        0     5252 2023-04-20 06:46:13.713909 python_keycloak_async-2.16.0.post7/src/keycloak/authorization/policy.py
--rw-r--r--   0        0        0     2306 2023-04-20 06:46:13.713909 python_keycloak_async-2.16.0.post7/src/keycloak/authorization/role.py
--rw-r--r--   0        0        0     9292 2023-04-20 06:46:13.713909 python_keycloak_async-2.16.0.post7/src/keycloak/connection.py
--rw-r--r--   0        0        0     5469 2023-04-20 06:46:13.713909 python_keycloak_async-2.16.0.post7/src/keycloak/exceptions.py
--rw-r--r--   0        0        0   150157 2023-04-20 06:46:13.717909 python_keycloak_async-2.16.0.post7/src/keycloak/keycloak_admin.py
--rw-r--r--   0        0        0    25578 2023-04-20 06:46:13.717909 python_keycloak_async-2.16.0.post7/src/keycloak/keycloak_openid.py
--rw-r--r--   0        0        0    15826 2023-04-20 06:46:13.717909 python_keycloak_async-2.16.0.post7/src/keycloak/keycloak_uma.py
--rw-r--r--   0        0        0    12915 2023-04-20 06:46:13.717909 python_keycloak_async-2.16.0.post7/src/keycloak/openid_connection.py
--rw-r--r--   0        0        0     8755 2023-04-20 06:46:13.717909 python_keycloak_async-2.16.0.post7/src/keycloak/uma_permissions.py
--rw-r--r--   0        0        0    11715 2023-04-20 06:46:13.717909 python_keycloak_async-2.16.0.post7/src/keycloak/urls_patterns.py
--rw-r--r--   0        0        0    17449 1970-01-01 00:00:00.000000 python_keycloak_async-2.16.0.post7/PKG-INFO
+-rw-r--r--   0        0        0     5559 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/CHANGELOG.md
+-rw-r--r--   0        0        0     3192 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1111 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/LICENSE
+-rw-r--r--   0        0        0    15646 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/README.md
+-rw-r--r--   0        0        0     2428 2023-04-20 06:50:28.320121 python_keycloak_async-2.16.0.post8/pyproject.toml
+-rw-r--r--   0        0        0     2381 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/__init__.py
+-rw-r--r--   0        0        0     1197 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/_version.py
+-rw-r--r--   0        0        0     3748 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/authorization/__init__.py
+-rw-r--r--   0        0        0     4421 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/authorization/permission.py
+-rw-r--r--   0        0        0     5252 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/authorization/policy.py
+-rw-r--r--   0        0        0     2306 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/authorization/role.py
+-rw-r--r--   0        0        0     9292 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/connection.py
+-rw-r--r--   0        0        0     5469 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/exceptions.py
+-rw-r--r--   0        0        0   150157 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/keycloak_admin.py
+-rw-r--r--   0        0        0    25578 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/keycloak_openid.py
+-rw-r--r--   0        0        0    15826 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/keycloak_uma.py
+-rw-r--r--   0        0        0    12915 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/openid_connection.py
+-rw-r--r--   0        0        0     8755 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/uma_permissions.py
+-rw-r--r--   0        0        0    11715 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/urls_patterns.py
+-rw-r--r--   0        0        0    17449 1970-01-01 00:00:00.000000 python_keycloak_async-2.16.0.post8/PKG-INFO
```

### Comparing `python_keycloak_async-2.16.0.post7/CHANGELOG.md` & `python_keycloak_async-2.16.0.post8/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/CONTRIBUTING.md` & `python_keycloak_async-2.16.0.post8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/LICENSE` & `python_keycloak_async-2.16.0.post8/LICENSE`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/README.md` & `python_keycloak_async-2.16.0.post8/README.md`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/pyproject.toml` & `python_keycloak_async-2.16.0.post8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-keycloak-async"
-version = "v2.16.0-7"
+version = "v2.16.0-8"
 description = "python-keycloak-async is a Python package providing access to the Keycloak API."
 license = "MIT"
 readme = "README.md"
 keywords = [ "keycloak", "asyncio", "openid", "oidc" ]
 authors = [
     "Quang Phan <quangpq.uit@gmail.com>",
     "Marcos Pereira <marcospereira.mpj@gmail.com>",
```

### Comparing `python_keycloak_async-2.16.0.post7/src/keycloak/__init__.py` & `python_keycloak_async-2.16.0.post8/src/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/src/keycloak/_version.py` & `python_keycloak_async-2.16.0.post8/src/keycloak/_version.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/src/keycloak/authorization/__init__.py` & `python_keycloak_async-2.16.0.post8/src/keycloak/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/src/keycloak/authorization/permission.py` & `python_keycloak_async-2.16.0.post8/src/keycloak/authorization/permission.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/src/keycloak/authorization/policy.py` & `python_keycloak_async-2.16.0.post8/src/keycloak/authorization/policy.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/src/keycloak/authorization/role.py` & `python_keycloak_async-2.16.0.post8/src/keycloak/authorization/role.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/src/keycloak/connection.py` & `python_keycloak_async-2.16.0.post8/src/keycloak/connection.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/src/keycloak/exceptions.py` & `python_keycloak_async-2.16.0.post8/src/keycloak/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/src/keycloak/keycloak_admin.py` & `python_keycloak_async-2.16.0.post8/src/keycloak/keycloak_admin.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/src/keycloak/keycloak_openid.py` & `python_keycloak_async-2.16.0.post8/src/keycloak/keycloak_openid.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/src/keycloak/keycloak_uma.py` & `python_keycloak_async-2.16.0.post8/src/keycloak/keycloak_uma.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/src/keycloak/openid_connection.py` & `python_keycloak_async-2.16.0.post8/src/keycloak/openid_connection.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/src/keycloak/uma_permissions.py` & `python_keycloak_async-2.16.0.post8/src/keycloak/uma_permissions.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/src/keycloak/urls_patterns.py` & `python_keycloak_async-2.16.0.post8/src/keycloak/urls_patterns.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post7/PKG-INFO` & `python_keycloak_async-2.16.0.post8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-keycloak-async
-Version: 2.16.0.post7
+Version: 2.16.0.post8
 Summary: python-keycloak-async is a Python package providing access to the Keycloak API.
 License: MIT
 Keywords: keycloak,asyncio,openid,oidc
 Author: Quang Phan
 Author-email: quangpq.uit@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

