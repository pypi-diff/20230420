# Comparing `tmp/etsy3py-0.0.2.tar.gz` & `tmp/etsy3py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etsy3py-0.0.2.tar", last modified: Wed Apr 19 12:40:24 2023, max compression
+gzip compressed data, was "etsy3py-0.0.3.tar", last modified: Thu Apr 20 09:06:34 2023, max compression
```

## Comparing `etsy3py-0.0.2.tar` & `etsy3py-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-19 12:40:24.821848 etsy3py-0.0.2/
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)     1055 2023-04-12 13:00:44.000000 etsy3py-0.0.2/LICENSE.txt
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)     3644 2023-04-19 12:40:24.821504 etsy3py-0.0.2/PKG-INFO
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)     3120 2023-04-19 12:40:19.000000 etsy3py-0.0.2/README.md
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)       38 2023-04-19 12:40:24.821986 etsy3py-0.0.2/setup.cfg
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)      890 2023-04-19 12:40:19.000000 etsy3py-0.0.2/setup.py
-drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-19 12:40:24.815199 etsy3py-0.0.2/src/
-drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-19 12:40:24.818872 etsy3py-0.0.2/src/etsy3py/
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)        0 2023-04-12 12:44:41.000000 etsy3py-0.0.2/src/etsy3py/__init__.py
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)     2493 2023-04-19 12:40:19.000000 etsy3py-0.0.2/src/etsy3py/base_client.py
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)     3205 2023-04-19 08:48:24.000000 etsy3py-0.0.2/src/etsy3py/oauth.py
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)    15320 2023-04-19 12:40:19.000000 etsy3py-0.0.2/src/etsy3py/v3.py
-drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-19 12:40:24.821056 etsy3py-0.0.2/src/etsy3py.egg-info/
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)     3644 2023-04-19 12:40:24.000000 etsy3py-0.0.2/src/etsy3py.egg-info/PKG-INFO
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)      294 2023-04-19 12:40:24.000000 etsy3py-0.0.2/src/etsy3py.egg-info/SOURCES.txt
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)        1 2023-04-19 12:40:24.000000 etsy3py-0.0.2/src/etsy3py.egg-info/dependency_links.txt
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)       32 2023-04-19 12:40:24.000000 etsy3py-0.0.2/src/etsy3py.egg-info/requires.txt
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)        8 2023-04-19 12:40:24.000000 etsy3py-0.0.2/src/etsy3py.egg-info/top_level.txt
+drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-20 09:06:34.169551 etsy3py-0.0.3/
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)     1055 2023-04-12 13:00:44.000000 etsy3py-0.0.3/LICENSE.txt
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)     3658 2023-04-20 09:06:34.169232 etsy3py-0.0.3/PKG-INFO
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)     3098 2023-04-20 09:02:30.000000 etsy3py-0.0.3/README.md
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)       38 2023-04-20 09:06:34.169688 etsy3py-0.0.3/setup.cfg
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)      938 2023-04-20 09:05:40.000000 etsy3py-0.0.3/setup.py
+drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-20 09:06:34.160247 etsy3py-0.0.3/src/
+drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-20 09:06:34.164576 etsy3py-0.0.3/src/etsy3py/
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)        0 2023-04-12 12:44:41.000000 etsy3py-0.0.3/src/etsy3py/__init__.py
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)     2859 2023-04-20 08:55:03.000000 etsy3py-0.0.3/src/etsy3py/base_client.py
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)     3205 2023-04-19 08:48:24.000000 etsy3py-0.0.3/src/etsy3py/oauth.py
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)    26926 2023-04-20 08:55:03.000000 etsy3py-0.0.3/src/etsy3py/v3.py
+drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-20 09:06:34.168763 etsy3py-0.0.3/src/etsy3py.egg-info/
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)     3658 2023-04-20 09:06:34.000000 etsy3py-0.0.3/src/etsy3py.egg-info/PKG-INFO
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)      294 2023-04-20 09:06:34.000000 etsy3py-0.0.3/src/etsy3py.egg-info/SOURCES.txt
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)        1 2023-04-20 09:06:34.000000 etsy3py-0.0.3/src/etsy3py.egg-info/dependency_links.txt
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)       32 2023-04-20 09:06:34.000000 etsy3py-0.0.3/src/etsy3py.egg-info/requires.txt
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)        8 2023-04-20 09:06:34.000000 etsy3py-0.0.3/src/etsy3py.egg-info/top_level.txt
```

### Comparing `etsy3py-0.0.2/LICENSE.txt` & `etsy3py-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etsy3py-0.0.2/PKG-INFO` & `etsy3py-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: etsy3py
-Version: 0.0.2
+Version: 0.0.3
 Summary: ETSY API v3 Client
 Home-page: https://github.com/damhuman/Etsy3Py
-Author: Anton Dasyuk, Ali-Abdulla
-Author-email: anton.dasyuk@gmail.com, alexukr1999@gmail.com
+Author: Anton Dasyuk
+Author-email: anton.dasyuk@gmail.com
+Maintainer: Ali-Abdulla Al-Sayed
+Maintainer-email: alexukr1999@gmail.com
 License: MIT
 Keywords: etsy,api,client,etsy v3 api
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Etsy3Py
 Client for Etsy API v3
@@ -21,14 +23,45 @@
 ## Installation
 You can install etsy3py using pip:
 
 ``` python
 pip install etsy3py
 ```
 
+## Requirements
+Python 3.6 or higher.
+
+# Etsy API
+This is a Python client for the Etsy API. 
+The client makes it easy to interact with the Etsy API and perform operations on a user's behalf.
+
+## Usage
+To use the EtsyApi class, you will need to obtain an access token from the Etsy API.
+
+``` python
+from etsy3py.v3 import EtsyApi
+
+access_token = "YOUR_ACCESS_TOKEN"
+client_id = "YOUR_CLIENT_ID"
+
+etsy_api = EtsyApi(access_token=access_token, client_id=client_id)
+
+listing_id = 12345
+listing = etsy_api.get_listing(listing_id)
+```
+
+### Authentication
+The EtsyApi class uses OAuth 2.0 authentication. You will need to obtain an access token from the Etsy API 
+before using the client. You can obtain an access token by following the
+instructions in the Etsy API documentation.
+
+### Rate Limiting
+The Etsy API has a rate limiting policy that limits the number of requests that can be made in a given time period.
+
+
 
 # Authentication step-by-step
 `EtsyOAuthClient` is a Python class that provides an authentication client for the Etsy marketplace API, 
 allowing users to connect to the API using OAuth2 authentication.
 
 ## Usage
 Here is an example of how to use the EtsyOAuthClient to obtain an access token from the Etsy API.
@@ -63,27 +96,27 @@
 ``` python
 authorization_code = 'the_authorization_code'
 access_token = client.fetch_token(authorization_code)
 ```
 
 You can now use the access token to make requests to the Etsy API
 
-## Refresh token
+# Refresh token
 
 The `refresh_token` method of the `EtsyOAuthClient` class requests a new access token from the authorization server using a refresh token.
 
 ### Parameters
 
 `refresh_token` (required): The refresh token used to obtain a new access token.
 
 ### Return Value
 
 The `refresh_token` method returns a dictionary containing the new access token and any additional data returned by the authorization server.
 
-### Example
+## Usage
 
 Replace these with your own values from the Etsy Developer Console
 
 ``` python
 client_id = 'your_client_id'
 client_secret = 'your_client_secret'
 
@@ -92,37 +125,9 @@
 client = EtsyOAuthClient(client_id, client_secret)
 
 # if the access token expires, you can use the refresh token to obtain a new access token and additional data 
 
 new_access_token = client.refresh_token(refresh_token)
 ```
 
-# Etsy API
-This is a Python client for the Etsy API. 
-The client makes it easy to interact with the Etsy API and perform operations on a user's behalf.
-
-### Requirements
-Python 3.6 or higher
-
-## Usage
-To use the EtsyApi class, you will need to obtain an access token from the Etsy API.
-
-``` python
-from etsy3py.v3 import EtsyApi
-
-access_token = "YOUR_ACCESS_TOKEN"
-client_id = "YOUR_CLIENT_ID"
-
-etsy_api = EtsyApi(access_token=access_token, client_id=client_id)
-# you can then call methods on the etsy_api object to interact with the Etsy API.
-```
-
-### Authentication
-The EtsyApi class uses OAuth 2.0 authentication. You will need to obtain an access token from the Etsy API 
-before using the client. You can obtain an access token by following the
-instructions in the Etsy API documentation.
-
-### Rate Limiting
-The Etsy API has a rate limiting policy that limits the number of requests that can be made in a given time period.
-
 #### This package is licensed under the MIT License.
```

### Comparing `etsy3py-0.0.2/README.md` & `etsy3py-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,45 @@
 ## Installation
 You can install etsy3py using pip:
 
 ``` python
 pip install etsy3py
 ```
 
+## Requirements
+Python 3.6 or higher.
+
+# Etsy API
+This is a Python client for the Etsy API. 
+The client makes it easy to interact with the Etsy API and perform operations on a user's behalf.
+
+## Usage
+To use the EtsyApi class, you will need to obtain an access token from the Etsy API.
+
+``` python
+from etsy3py.v3 import EtsyApi
+
+access_token = "YOUR_ACCESS_TOKEN"
+client_id = "YOUR_CLIENT_ID"
+
+etsy_api = EtsyApi(access_token=access_token, client_id=client_id)
+
+listing_id = 12345
+listing = etsy_api.get_listing(listing_id)
+```
+
+### Authentication
+The EtsyApi class uses OAuth 2.0 authentication. You will need to obtain an access token from the Etsy API 
+before using the client. You can obtain an access token by following the
+instructions in the Etsy API documentation.
+
+### Rate Limiting
+The Etsy API has a rate limiting policy that limits the number of requests that can be made in a given time period.
+
+
 
 # Authentication step-by-step
 `EtsyOAuthClient` is a Python class that provides an authentication client for the Etsy marketplace API, 
 allowing users to connect to the API using OAuth2 authentication.
 
 ## Usage
 Here is an example of how to use the EtsyOAuthClient to obtain an access token from the Etsy API.
@@ -46,27 +77,27 @@
 ``` python
 authorization_code = 'the_authorization_code'
 access_token = client.fetch_token(authorization_code)
 ```
 
 You can now use the access token to make requests to the Etsy API
 
-## Refresh token
+# Refresh token
 
 The `refresh_token` method of the `EtsyOAuthClient` class requests a new access token from the authorization server using a refresh token.
 
 ### Parameters
 
 `refresh_token` (required): The refresh token used to obtain a new access token.
 
 ### Return Value
 
 The `refresh_token` method returns a dictionary containing the new access token and any additional data returned by the authorization server.
 
-### Example
+## Usage
 
 Replace these with your own values from the Etsy Developer Console
 
 ``` python
 client_id = 'your_client_id'
 client_secret = 'your_client_secret'
 
@@ -75,36 +106,8 @@
 client = EtsyOAuthClient(client_id, client_secret)
 
 # if the access token expires, you can use the refresh token to obtain a new access token and additional data 
 
 new_access_token = client.refresh_token(refresh_token)
 ```
 
-# Etsy API
-This is a Python client for the Etsy API. 
-The client makes it easy to interact with the Etsy API and perform operations on a user's behalf.
-
-### Requirements
-Python 3.6 or higher
-
-## Usage
-To use the EtsyApi class, you will need to obtain an access token from the Etsy API.
-
-``` python
-from etsy3py.v3 import EtsyApi
-
-access_token = "YOUR_ACCESS_TOKEN"
-client_id = "YOUR_CLIENT_ID"
-
-etsy_api = EtsyApi(access_token=access_token, client_id=client_id)
-# you can then call methods on the etsy_api object to interact with the Etsy API.
-```
-
-### Authentication
-The EtsyApi class uses OAuth 2.0 authentication. You will need to obtain an access token from the Etsy API 
-before using the client. You can obtain an access token by following the
-instructions in the Etsy API documentation.
-
-### Rate Limiting
-The Etsy API has a rate limiting policy that limits the number of requests that can be made in a given time period.
-
 #### This package is licensed under the MIT License.
```

### Comparing `etsy3py-0.0.2/setup.py` & `etsy3py-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,28 +4,30 @@
     long_description = fh.read()
 
 setup(
     name='etsy3py',
     description='ETSY API v3 Client',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
-    author="Anton Dasyuk, Ali-Abdulla",
-    author_email='anton.dasyuk@gmail.com, alexukr1999@gmail.com',
+    author="Anton Dasyuk",
+    author_email='anton.dasyuk@gmail.com',
+    maintainer="Ali-Abdulla Al-Sayed",
+    maintainer_email="alexukr1999@gmail.com",
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/damhuman/Etsy3Py',
     keywords=['etsy', 'api', 'client', 'etsy v3 api'],
     install_requires=[
         'requests',
         'requests-oauthlib',
         'mypy',
     ],
     python_requires='>=3.6',
     classifiers=[
         "Programming Language :: Python :: 3",
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
     ]
 
 )
```

### Comparing `etsy3py-0.0.2/src/etsy3py/base_client.py` & `etsy3py-0.0.3/src/etsy3py/base_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,68 @@
-from typing import Type
-
 import requests
 from requests.auth import HTTPBasicAuth
 from requests import Request, Session
 
 
 class BaseApiClient:
     base_url = "https://openapi.etsy.com"
-    __token_type = None
-    __token = None
-    __client_id = None
-    session = Session()
- 
+
+    def __init__(self, token: str = None, client_id: str = None, token_type: str = None) -> None:
+        self.__token_type = token_type
+        self.__token = token
+        self.__client_id = client_id
+        self.session = Session()
+
     def _make_request(self,
                       path: str,
                       custom_base: str = None,
                       method: str = 'GET',
                       headers: dict = None,
                       data: dict = None,
                       params: dict = None,
-                      auth_type: str = 'token') -> Type[requests.Response]:
+                      auth_type: str = 'token') -> requests.Response:
 
         if not headers:
             headers = {}
- 
+
         request_url = f"{custom_base if custom_base else self.base_url}{path}"
- 
+
         auth = None
         if auth_type == 'basic':
             auth = HTTPBasicAuth(1, 1)
         if auth_type == 'token':
             headers['Authorization'] = f'{self.__token_type} {self.__token}'
             headers['x-api-key'] = f'{self.__client_id}'
- 
+
         request = Request(method=method,
                           url=request_url,
                           headers=headers,
                           data=data,
                           params=params,
                           auth=auth).prepare()
         response = self.session.send(request)
         return response
- 
+
     def _post(self, path: str, data: dict = None, headers: dict = None,
-              auth_type: str = 'none') -> Type[requests.Response]:
+              auth_type: str = 'none') -> requests.Response:
         return self._make_request(path=path, method='POST', data=data,
                                   headers=headers, auth_type=auth_type)
- 
+
     def _get(self, path: str, params: dict = None, headers: dict = None,
-             auth_type: str = 'none') -> Type[requests.Response]:
+             auth_type: str = 'none') -> requests.Response:
         return self._make_request(path=path, method='GET', params=params,
                                   headers=headers, auth_type=auth_type)
 
+    def _patch(self, path: str, data: dict = None, headers: dict = None,
+               auth_type: str = 'none') -> requests.Response:
+        return self._make_request(path=path, method='PATCH', data=data,
+                                  headers=headers, auth_type=auth_type)
+
     def _put(self, path: str, data: dict = None, headers: dict = None,
-             auth_type: str = 'none') -> Type[requests.Response]:
+             auth_type: str = 'none') -> requests.Response:
         return self._make_request(path=path, method='PUT', data=data,
                                   headers=headers, auth_type=auth_type)
 
     def _delete(self, path: str, params: dict = None, headers: dict = None,
-                auth_type: str = 'none') -> Type[requests.Response]:
+                auth_type: str = 'none') -> requests.Response:
         return self._make_request(path=path, method='DELETE', params=params,
                                   headers=headers, auth_type=auth_type)
```

### Comparing `etsy3py-0.0.2/src/etsy3py/oauth.py` & `etsy3py-0.0.3/src/etsy3py/oauth.py`

 * *Files identical despite different names*

### Comparing `etsy3py-0.0.2/src/etsy3py.egg-info/PKG-INFO` & `etsy3py-0.0.3/src/etsy3py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: etsy3py
-Version: 0.0.2
+Version: 0.0.3
 Summary: ETSY API v3 Client
 Home-page: https://github.com/damhuman/Etsy3Py
-Author: Anton Dasyuk, Ali-Abdulla
-Author-email: anton.dasyuk@gmail.com, alexukr1999@gmail.com
+Author: Anton Dasyuk
+Author-email: anton.dasyuk@gmail.com
+Maintainer: Ali-Abdulla Al-Sayed
+Maintainer-email: alexukr1999@gmail.com
 License: MIT
 Keywords: etsy,api,client,etsy v3 api
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Etsy3Py
 Client for Etsy API v3
@@ -21,14 +23,45 @@
 ## Installation
 You can install etsy3py using pip:
 
 ``` python
 pip install etsy3py
 ```
 
+## Requirements
+Python 3.6 or higher.
+
+# Etsy API
+This is a Python client for the Etsy API. 
+The client makes it easy to interact with the Etsy API and perform operations on a user's behalf.
+
+## Usage
+To use the EtsyApi class, you will need to obtain an access token from the Etsy API.
+
+``` python
+from etsy3py.v3 import EtsyApi
+
+access_token = "YOUR_ACCESS_TOKEN"
+client_id = "YOUR_CLIENT_ID"
+
+etsy_api = EtsyApi(access_token=access_token, client_id=client_id)
+
+listing_id = 12345
+listing = etsy_api.get_listing(listing_id)
+```
+
+### Authentication
+The EtsyApi class uses OAuth 2.0 authentication. You will need to obtain an access token from the Etsy API 
+before using the client. You can obtain an access token by following the
+instructions in the Etsy API documentation.
+
+### Rate Limiting
+The Etsy API has a rate limiting policy that limits the number of requests that can be made in a given time period.
+
+
 
 # Authentication step-by-step
 `EtsyOAuthClient` is a Python class that provides an authentication client for the Etsy marketplace API, 
 allowing users to connect to the API using OAuth2 authentication.
 
 ## Usage
 Here is an example of how to use the EtsyOAuthClient to obtain an access token from the Etsy API.
@@ -63,27 +96,27 @@
 ``` python
 authorization_code = 'the_authorization_code'
 access_token = client.fetch_token(authorization_code)
 ```
 
 You can now use the access token to make requests to the Etsy API
 
-## Refresh token
+# Refresh token
 
 The `refresh_token` method of the `EtsyOAuthClient` class requests a new access token from the authorization server using a refresh token.
 
 ### Parameters
 
 `refresh_token` (required): The refresh token used to obtain a new access token.
 
 ### Return Value
 
 The `refresh_token` method returns a dictionary containing the new access token and any additional data returned by the authorization server.
 
-### Example
+## Usage
 
 Replace these with your own values from the Etsy Developer Console
 
 ``` python
 client_id = 'your_client_id'
 client_secret = 'your_client_secret'
 
@@ -92,37 +125,9 @@
 client = EtsyOAuthClient(client_id, client_secret)
 
 # if the access token expires, you can use the refresh token to obtain a new access token and additional data 
 
 new_access_token = client.refresh_token(refresh_token)
 ```
 
-# Etsy API
-This is a Python client for the Etsy API. 
-The client makes it easy to interact with the Etsy API and perform operations on a user's behalf.
-
-### Requirements
-Python 3.6 or higher
-
-## Usage
-To use the EtsyApi class, you will need to obtain an access token from the Etsy API.
-
-``` python
-from etsy3py.v3 import EtsyApi
-
-access_token = "YOUR_ACCESS_TOKEN"
-client_id = "YOUR_CLIENT_ID"
-
-etsy_api = EtsyApi(access_token=access_token, client_id=client_id)
-# you can then call methods on the etsy_api object to interact with the Etsy API.
-```
-
-### Authentication
-The EtsyApi class uses OAuth 2.0 authentication. You will need to obtain an access token from the Etsy API 
-before using the client. You can obtain an access token by following the
-instructions in the Etsy API documentation.
-
-### Rate Limiting
-The Etsy API has a rate limiting policy that limits the number of requests that can be made in a given time period.
-
 #### This package is licensed under the MIT License.
```

