# Comparing `tmp/baikal-sdk-1.2.3.tar.gz` & `tmp/baikal-sdk-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baikal-sdk-1.2.3.tar", last modified: Tue Apr 26 12:20:56 2022, max compression
+gzip compressed data, was "dist/baikal-sdk-1.2.4.tar", last modified: Thu Apr 20 11:33:51 2023, max compression
```

## Comparing `baikal-sdk-1.2.3.tar` & `baikal-sdk-1.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 eag        (502) staff       (20)        0 2022-04-26 12:20:56.819212 baikal-sdk-1.2.3/
--rw-r--r--   0 eag        (502) staff       (20)    10174 2019-09-13 10:03:31.000000 baikal-sdk-1.2.3/LICENSE
--rw-r--r--   0 eag        (502) staff       (20)      552 2019-09-13 10:03:31.000000 baikal-sdk-1.2.3/NOTICE
--rw-r--r--   0 eag        (502) staff       (20)     7109 2022-04-26 12:20:56.817936 baikal-sdk-1.2.3/PKG-INFO
--rw-r--r--   0 eag        (502) staff       (20)     6492 2020-08-14 22:02:08.000000 baikal-sdk-1.2.3/README.md
-drwxr-xr-x   0 eag        (502) staff       (20)        0 2022-04-26 12:20:56.803049 baikal-sdk-1.2.3/baikal_sdk.egg-info/
--rw-r--r--   0 eag        (502) staff       (20)     7109 2022-04-26 12:20:52.000000 baikal-sdk-1.2.3/baikal_sdk.egg-info/PKG-INFO
--rw-r--r--   0 eag        (502) staff       (20)      419 2022-04-26 12:20:56.000000 baikal-sdk-1.2.3/baikal_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 eag        (502) staff       (20)        1 2022-04-26 12:20:52.000000 baikal-sdk-1.2.3/baikal_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 eag        (502) staff       (20)        1 2019-09-12 19:36:18.000000 baikal-sdk-1.2.3/baikal_sdk.egg-info/not-zip-safe
--rw-r--r--   0 eag        (502) staff       (20)      158 2022-04-26 12:20:55.000000 baikal-sdk-1.2.3/baikal_sdk.egg-info/requires.txt
--rw-r--r--   0 eag        (502) staff       (20)        8 2022-04-26 12:20:55.000000 baikal-sdk-1.2.3/baikal_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 eag        (502) staff       (20)        0 2022-04-26 12:20:56.808569 baikal-sdk-1.2.3/clients/
--rw-r--r--   0 eag        (502) staff       (20)        0 2019-06-10 08:42:41.000000 baikal-sdk-1.2.3/clients/__init__.py
-drwxr-xr-x   0 eag        (502) staff       (20)        0 2022-04-26 12:20:56.816653 baikal-sdk-1.2.3/clients/aio/
--rw-r--r--   0 eag        (502) staff       (20)        0 2020-07-20 10:04:47.000000 baikal-sdk-1.2.3/clients/aio/__init__.py
--rw-r--r--   0 eag        (502) staff       (20)     1821 2020-07-20 10:04:47.000000 baikal-sdk-1.2.3/clients/aio/aiohttp_client.py
--rw-r--r--   0 eag        (502) staff       (20)     9683 2020-11-19 17:00:42.000000 baikal-sdk-1.2.3/clients/aio/baikal_client.py
--rw-r--r--   0 eag        (502) staff       (20)    12332 2022-04-26 12:13:35.000000 baikal-sdk-1.2.3/clients/baikal_client.py
--rw-r--r--   0 eag        (502) staff       (20)     9115 2019-10-02 08:00:24.000000 baikal-sdk-1.2.3/clients/cache.py
--rw-r--r--   0 eag        (502) staff       (20)      249 2019-10-01 19:56:39.000000 baikal-sdk-1.2.3/clients/exceptions.py
--rw-r--r--   0 eag        (502) staff       (20)      158 2022-04-26 12:17:01.000000 baikal-sdk-1.2.3/requirements.txt
--rw-r--r--   0 eag        (502) staff       (20)       38 2022-04-26 12:20:56.819377 baikal-sdk-1.2.3/setup.cfg
--rw-r--r--   0 eag        (502) staff       (20)     1101 2022-04-26 12:18:00.000000 baikal-sdk-1.2.3/setup.py
+drwxr-xr-x   0 jarf      (1000) jarf      (1000)        0 2023-04-20 11:33:51.000000 baikal-sdk-1.2.4/
+-rw-r--r--   0 jarf      (1000) jarf      (1000)    10174 2023-04-20 10:50:03.000000 baikal-sdk-1.2.4/LICENSE
+-rw-r--r--   0 jarf      (1000) jarf      (1000)      552 2023-04-20 10:50:03.000000 baikal-sdk-1.2.4/NOTICE
+-rw-r--r--   0 jarf      (1000) jarf      (1000)     7127 2023-04-20 11:33:51.000000 baikal-sdk-1.2.4/PKG-INFO
+-rw-r--r--   0 jarf      (1000) jarf      (1000)     6530 2023-04-20 10:50:03.000000 baikal-sdk-1.2.4/README.md
+drwxr-xr-x   0 jarf      (1000) jarf      (1000)        0 2023-04-20 11:33:51.000000 baikal-sdk-1.2.4/baikal_sdk.egg-info/
+-rw-r--r--   0 jarf      (1000) jarf      (1000)     7127 2023-04-20 11:33:51.000000 baikal-sdk-1.2.4/baikal_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 jarf      (1000) jarf      (1000)      419 2023-04-20 11:33:51.000000 baikal-sdk-1.2.4/baikal_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jarf      (1000) jarf      (1000)        1 2023-04-20 11:33:51.000000 baikal-sdk-1.2.4/baikal_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jarf      (1000) jarf      (1000)        1 2023-04-20 11:33:51.000000 baikal-sdk-1.2.4/baikal_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 jarf      (1000) jarf      (1000)      158 2023-04-20 11:33:51.000000 baikal-sdk-1.2.4/baikal_sdk.egg-info/requires.txt
+-rw-r--r--   0 jarf      (1000) jarf      (1000)        8 2023-04-20 11:33:51.000000 baikal-sdk-1.2.4/baikal_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 jarf      (1000) jarf      (1000)        0 2023-04-20 11:33:51.000000 baikal-sdk-1.2.4/clients/
+-rw-r--r--   0 jarf      (1000) jarf      (1000)        0 2023-04-20 10:50:03.000000 baikal-sdk-1.2.4/clients/__init__.py
+drwxr-xr-x   0 jarf      (1000) jarf      (1000)        0 2023-04-20 11:33:51.000000 baikal-sdk-1.2.4/clients/aio/
+-rw-r--r--   0 jarf      (1000) jarf      (1000)        0 2023-04-20 10:50:03.000000 baikal-sdk-1.2.4/clients/aio/__init__.py
+-rw-r--r--   0 jarf      (1000) jarf      (1000)     1821 2023-04-20 10:50:03.000000 baikal-sdk-1.2.4/clients/aio/aiohttp_client.py
+-rw-r--r--   0 jarf      (1000) jarf      (1000)     9683 2023-04-20 10:50:03.000000 baikal-sdk-1.2.4/clients/aio/baikal_client.py
+-rw-r--r--   0 jarf      (1000) jarf      (1000)    12332 2023-04-20 10:50:03.000000 baikal-sdk-1.2.4/clients/baikal_client.py
+-rw-r--r--   0 jarf      (1000) jarf      (1000)     9115 2023-04-20 10:50:03.000000 baikal-sdk-1.2.4/clients/cache.py
+-rw-r--r--   0 jarf      (1000) jarf      (1000)      249 2023-04-20 10:50:03.000000 baikal-sdk-1.2.4/clients/exceptions.py
+-rw-r--r--   0 jarf      (1000) jarf      (1000)      158 2023-04-20 11:16:43.000000 baikal-sdk-1.2.4/requirements.txt
+-rw-r--r--   0 jarf      (1000) jarf      (1000)       38 2023-04-20 11:33:51.000000 baikal-sdk-1.2.4/setup.cfg
+-rw-r--r--   0 jarf      (1000) jarf      (1000)     1101 2023-04-20 11:33:26.000000 baikal-sdk-1.2.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `baikal-sdk-1.2.3/LICENSE` & `baikal-sdk-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `baikal-sdk-1.2.3/NOTICE` & `baikal-sdk-1.2.4/NOTICE`

 * *Files identical despite different names*

### Comparing `baikal-sdk-1.2.3/PKG-INFO` & `baikal-sdk-1.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: baikal-sdk
-Version: 1.2.3
+Version: 1.2.4
 Summary: SDK to generate tokens for the 4th Platform
 Home-page: https://github.com/Telefonica/baikal-sdk/python
 Maintainer: 4th Platform team
 Maintainer-email: 4pf@telefonica.com
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,31 +26,32 @@
 
 ```bash
 pip install baikal-sdk
 ```
 
 ## Usage
 
-
 **Create a client**
+
 ```python
 from clients.baikal_client import OpenIDClient
 
 
 oidc_client = OpenIDClient(
     authserver_endpoint='https://auth.xxx.baikalplatform.com', # authserver endpoint
     client_id='your_oauth_client_id',
     client_secret='your_oauth_client_secret',
     # For using grantUser method (jwt-bearer grant type)
     client_keys=[{ 'key': 'stringWithTheKey', format: 'pem' }],  # optional
     issuer='http://yourserver.com/',  # your jwt issuer id
     private_certs_path='/path/to/certs/directory'  # directory to read certificates/private keys.
 )
 ```
-if you want to use in an asynchronous environment:
+
+If you want to use in an asynchronous environment:
 
 ```python
 from clients.aio.baikal_client import OpenIDClient
 
 
 oidc_client = OpenIDClient(
     authserver_endpoint='https://auth.xxx.baikalplatform.com', # authserver endpoint
@@ -76,15 +76,17 @@
   ['list', 'of', 'scopes'],
   ['list', 'of', 'purposes'],
   authorization_id='46921050-e97c-418b-928c-4158256be92c', # optional
   identifier={'id': 'my-phone-number', 'type': 'phone_number'}, # optional
   full_authserver_response=False # optional (get full response, including expires_in, scopes ...)
 )
 ```
-to use asynchronously (e.g. with aiohttp):
+
+to use it asynchronously (e.g. with aiohttp):
+
 ```python
 access_token = await oidc_client.async_grant_user(
   'userSUB',
   ['list', 'of', 'scopes'],
   ['list', 'of', 'purposes'],
   authorization_id='46921050-e97c-418b-928c-4158256be92c', # optional
   identifier={'id': 'my-phone-number', 'type': 'phone_number'} # optional
@@ -95,46 +97,48 @@
 ```python
 access_token = oidc_client.grant_client(
   scopes=['list', 'of', 'scopes'] #optional
   purposes=['list', 'of', 'purposes'] #optional
 )
 ```
 
-The upper methods can be called in an asynchronous environment using await:
+The methods can be called asynchronously using await:
 
-```
-access_token = await oidc_client.xxxx
+```python
+access_token = await oidc_client.async_grant_client(...)
 ```
 
-
 **Introspect access_token**
+
 ```python
 payload = oidc_client.introspect(access_token)
 assert 'scope-sep-string' in payload['scope']
 ```
 
 The upper methods can be called in an asynchronous environment using await:
 
-```
-access_token = await oidc_client.xxxx
+```python
+access_token = await oidc_client.async_introspect(...)
 ```
 
 **Expose your public keys in a server route to use with a `jwt-bearer`**
 
 If you have configured your issuer in the authserver to read from an endpoint,
 you should expose your public keys in an accessible route.
 
 ```python
 oid_client.get_jwk_set()
 ```
+
 This will output the public part of your keys to be directly exposed in JWK format (required by authserver and any OIDC server).
 
 ## Configuration
 
 The `OpenIDClient` configuration will be read from environment if ommited
+
 ```inc
 export BAIKAL_AUTHSERVER_ENDPOINT='https://auth.xxx.baikalplatform.com'
 export BAIKAL_CLIENT_ID='your_oauth_client_id'
 export BAIKAL_CLIENT_SECRET='your_oauth_client_secret'
 export BAIKAL_ISSUER='http://yourserver.com/'
 export BAIKAL_PRIVATE_CERTS_PATH='/path/to/certs/directory'
 ```
@@ -158,15 +162,15 @@
     headers={
         'X-Correlator': '1234-5678-9012-3456-7890'
     },
     timeout=30
 )
 ```
 
-If you are using the library with a 4th Platform development environment, you can accept self-signed certs setting this environment variable:
+If you are using the library against a Telefónica Kernel development environment, you can accept self-signed certs setting this environment variable:
 
 ```
 export BAIKAL_VERIFY_CERTS=False  # Accept self signed certs for authserver communication (not used in token validation)
 ```
 
 ### Configure asynchronous connections
 
@@ -179,31 +183,31 @@
 
 It's not needed to have private keys generated from a secured authority. For oauth2 verify you can use self-generated keys. Here it's included some tips.
 
 If you want to generate different keys (in JWK format) for development purpose you can use https://mkjwk.org/.
 
 ### Generate a RSA private key (with SHA 256 hash, RS256) (using openssl)
 
-````bash
+````sh
 openssl genrsa -des3 -out private-rsa-protected.pem 2048
 ````
 
 This will produce a private rsa key of 2048 bits protected with a password, in order to remove the password and use directly the private key in the library you can run this:
 
-```bash
+```sh
 openssl rsa -in private-rsa-protected.pem -out private-rsa.pem
 # rm private-rsa-protected.pem
 
 ```
 
 Another option (single line) is to use this command:
-```bash
+
+```sh
 openssl genpkey -out rsakey.pem -algorithm RSA -pkeyopt rsa_keygen_bits:2048
 ```
 
 The private-rsa.pem can be used with the library to generate assertions and to expose the public key part as stated before. Just place the pem in your directory and point the sdk private_certs_path to it.
 The public key is automatically generated in JWK as you can check in the expose your public keys section.
 
-It's not recommended to use rsa keys bigger than 2048 (e.g 4096) as the computational cost is not worth. It's better to have a keys rotation policy every given time (e.g. a week). It's also not recommended
-to use keys of 1024 length as it can be cracked.
-
-
+It's not recommended to use rsa keys bigger than 2048 (e.g 4096) as the computational cost is not worth.
+It's better to have a keys rotation policy every given time (e.g. a week).
+It's also not recommended to use keys of 1024 length as it can be cracked.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `baikal-sdk-1.2.3/README.md` & `baikal-sdk-1.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,31 +9,32 @@
 
 ```bash
 pip install baikal-sdk
 ```
 
 ## Usage
 
-
 **Create a client**
+
 ```python
 from clients.baikal_client import OpenIDClient
 
 
 oidc_client = OpenIDClient(
     authserver_endpoint='https://auth.xxx.baikalplatform.com', # authserver endpoint
     client_id='your_oauth_client_id',
     client_secret='your_oauth_client_secret',
     # For using grantUser method (jwt-bearer grant type)
     client_keys=[{ 'key': 'stringWithTheKey', format: 'pem' }],  # optional
     issuer='http://yourserver.com/',  # your jwt issuer id
     private_certs_path='/path/to/certs/directory'  # directory to read certificates/private keys.
 )
 ```
-if you want to use in an asynchronous environment:
+
+If you want to use in an asynchronous environment:
 
 ```python
 from clients.aio.baikal_client import OpenIDClient
 
 
 oidc_client = OpenIDClient(
     authserver_endpoint='https://auth.xxx.baikalplatform.com', # authserver endpoint
@@ -58,15 +59,17 @@
   ['list', 'of', 'scopes'],
   ['list', 'of', 'purposes'],
   authorization_id='46921050-e97c-418b-928c-4158256be92c', # optional
   identifier={'id': 'my-phone-number', 'type': 'phone_number'}, # optional
   full_authserver_response=False # optional (get full response, including expires_in, scopes ...)
 )
 ```
-to use asynchronously (e.g. with aiohttp):
+
+to use it asynchronously (e.g. with aiohttp):
+
 ```python
 access_token = await oidc_client.async_grant_user(
   'userSUB',
   ['list', 'of', 'scopes'],
   ['list', 'of', 'purposes'],
   authorization_id='46921050-e97c-418b-928c-4158256be92c', # optional
   identifier={'id': 'my-phone-number', 'type': 'phone_number'} # optional
@@ -77,46 +80,48 @@
 ```python
 access_token = oidc_client.grant_client(
   scopes=['list', 'of', 'scopes'] #optional
   purposes=['list', 'of', 'purposes'] #optional
 )
 ```
 
-The upper methods can be called in an asynchronous environment using await:
+The methods can be called asynchronously using await:
 
+```python
+access_token = await oidc_client.async_grant_client(...)
 ```
-access_token = await oidc_client.xxxx
-```
-
 
 **Introspect access_token**
+
 ```python
 payload = oidc_client.introspect(access_token)
 assert 'scope-sep-string' in payload['scope']
 ```
 
 The upper methods can be called in an asynchronous environment using await:
 
-```
-access_token = await oidc_client.xxxx
+```python
+access_token = await oidc_client.async_introspect(...)
 ```
 
 **Expose your public keys in a server route to use with a `jwt-bearer`**
 
 If you have configured your issuer in the authserver to read from an endpoint,
 you should expose your public keys in an accessible route.
 
 ```python
 oid_client.get_jwk_set()
 ```
+
 This will output the public part of your keys to be directly exposed in JWK format (required by authserver and any OIDC server).
 
 ## Configuration
 
 The `OpenIDClient` configuration will be read from environment if ommited
+
 ```inc
 export BAIKAL_AUTHSERVER_ENDPOINT='https://auth.xxx.baikalplatform.com'
 export BAIKAL_CLIENT_ID='your_oauth_client_id'
 export BAIKAL_CLIENT_SECRET='your_oauth_client_secret'
 export BAIKAL_ISSUER='http://yourserver.com/'
 export BAIKAL_PRIVATE_CERTS_PATH='/path/to/certs/directory'
 ```
@@ -140,15 +145,15 @@
     headers={
         'X-Correlator': '1234-5678-9012-3456-7890'
     },
     timeout=30
 )
 ```
 
-If you are using the library with a 4th Platform development environment, you can accept self-signed certs setting this environment variable:
+If you are using the library against a Telefónica Kernel development environment, you can accept self-signed certs setting this environment variable:
 
 ```
 export BAIKAL_VERIFY_CERTS=False  # Accept self signed certs for authserver communication (not used in token validation)
 ```
 
 ### Configure asynchronous connections
 
@@ -161,29 +166,31 @@
 
 It's not needed to have private keys generated from a secured authority. For oauth2 verify you can use self-generated keys. Here it's included some tips.
 
 If you want to generate different keys (in JWK format) for development purpose you can use https://mkjwk.org/.
 
 ### Generate a RSA private key (with SHA 256 hash, RS256) (using openssl)
 
-````bash
+````sh
 openssl genrsa -des3 -out private-rsa-protected.pem 2048
 ````
 
 This will produce a private rsa key of 2048 bits protected with a password, in order to remove the password and use directly the private key in the library you can run this:
 
-```bash
+```sh
 openssl rsa -in private-rsa-protected.pem -out private-rsa.pem
 # rm private-rsa-protected.pem
 
 ```
 
 Another option (single line) is to use this command:
-```bash
+
+```sh
 openssl genpkey -out rsakey.pem -algorithm RSA -pkeyopt rsa_keygen_bits:2048
 ```
 
 The private-rsa.pem can be used with the library to generate assertions and to expose the public key part as stated before. Just place the pem in your directory and point the sdk private_certs_path to it.
 The public key is automatically generated in JWK as you can check in the expose your public keys section.
 
-It's not recommended to use rsa keys bigger than 2048 (e.g 4096) as the computational cost is not worth. It's better to have a keys rotation policy every given time (e.g. a week). It's also not recommended
-to use keys of 1024 length as it can be cracked.
+It's not recommended to use rsa keys bigger than 2048 (e.g 4096) as the computational cost is not worth.
+It's better to have a keys rotation policy every given time (e.g. a week).
+It's also not recommended to use keys of 1024 length as it can be cracked.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `baikal-sdk-1.2.3/baikal_sdk.egg-info/PKG-INFO` & `baikal-sdk-1.2.4/baikal_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: baikal-sdk
-Version: 1.2.3
+Version: 1.2.4
 Summary: SDK to generate tokens for the 4th Platform
 Home-page: https://github.com/Telefonica/baikal-sdk/python
 Maintainer: 4th Platform team
 Maintainer-email: 4pf@telefonica.com
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,31 +26,32 @@
 
 ```bash
 pip install baikal-sdk
 ```
 
 ## Usage
 
-
 **Create a client**
+
 ```python
 from clients.baikal_client import OpenIDClient
 
 
 oidc_client = OpenIDClient(
     authserver_endpoint='https://auth.xxx.baikalplatform.com', # authserver endpoint
     client_id='your_oauth_client_id',
     client_secret='your_oauth_client_secret',
     # For using grantUser method (jwt-bearer grant type)
     client_keys=[{ 'key': 'stringWithTheKey', format: 'pem' }],  # optional
     issuer='http://yourserver.com/',  # your jwt issuer id
     private_certs_path='/path/to/certs/directory'  # directory to read certificates/private keys.
 )
 ```
-if you want to use in an asynchronous environment:
+
+If you want to use in an asynchronous environment:
 
 ```python
 from clients.aio.baikal_client import OpenIDClient
 
 
 oidc_client = OpenIDClient(
     authserver_endpoint='https://auth.xxx.baikalplatform.com', # authserver endpoint
@@ -76,15 +76,17 @@
   ['list', 'of', 'scopes'],
   ['list', 'of', 'purposes'],
   authorization_id='46921050-e97c-418b-928c-4158256be92c', # optional
   identifier={'id': 'my-phone-number', 'type': 'phone_number'}, # optional
   full_authserver_response=False # optional (get full response, including expires_in, scopes ...)
 )
 ```
-to use asynchronously (e.g. with aiohttp):
+
+to use it asynchronously (e.g. with aiohttp):
+
 ```python
 access_token = await oidc_client.async_grant_user(
   'userSUB',
   ['list', 'of', 'scopes'],
   ['list', 'of', 'purposes'],
   authorization_id='46921050-e97c-418b-928c-4158256be92c', # optional
   identifier={'id': 'my-phone-number', 'type': 'phone_number'} # optional
@@ -95,46 +97,48 @@
 ```python
 access_token = oidc_client.grant_client(
   scopes=['list', 'of', 'scopes'] #optional
   purposes=['list', 'of', 'purposes'] #optional
 )
 ```
 
-The upper methods can be called in an asynchronous environment using await:
+The methods can be called asynchronously using await:
 
-```
-access_token = await oidc_client.xxxx
+```python
+access_token = await oidc_client.async_grant_client(...)
 ```
 
-
 **Introspect access_token**
+
 ```python
 payload = oidc_client.introspect(access_token)
 assert 'scope-sep-string' in payload['scope']
 ```
 
 The upper methods can be called in an asynchronous environment using await:
 
-```
-access_token = await oidc_client.xxxx
+```python
+access_token = await oidc_client.async_introspect(...)
 ```
 
 **Expose your public keys in a server route to use with a `jwt-bearer`**
 
 If you have configured your issuer in the authserver to read from an endpoint,
 you should expose your public keys in an accessible route.
 
 ```python
 oid_client.get_jwk_set()
 ```
+
 This will output the public part of your keys to be directly exposed in JWK format (required by authserver and any OIDC server).
 
 ## Configuration
 
 The `OpenIDClient` configuration will be read from environment if ommited
+
 ```inc
 export BAIKAL_AUTHSERVER_ENDPOINT='https://auth.xxx.baikalplatform.com'
 export BAIKAL_CLIENT_ID='your_oauth_client_id'
 export BAIKAL_CLIENT_SECRET='your_oauth_client_secret'
 export BAIKAL_ISSUER='http://yourserver.com/'
 export BAIKAL_PRIVATE_CERTS_PATH='/path/to/certs/directory'
 ```
@@ -158,15 +162,15 @@
     headers={
         'X-Correlator': '1234-5678-9012-3456-7890'
     },
     timeout=30
 )
 ```
 
-If you are using the library with a 4th Platform development environment, you can accept self-signed certs setting this environment variable:
+If you are using the library against a Telefónica Kernel development environment, you can accept self-signed certs setting this environment variable:
 
 ```
 export BAIKAL_VERIFY_CERTS=False  # Accept self signed certs for authserver communication (not used in token validation)
 ```
 
 ### Configure asynchronous connections
 
@@ -179,31 +183,31 @@
 
 It's not needed to have private keys generated from a secured authority. For oauth2 verify you can use self-generated keys. Here it's included some tips.
 
 If you want to generate different keys (in JWK format) for development purpose you can use https://mkjwk.org/.
 
 ### Generate a RSA private key (with SHA 256 hash, RS256) (using openssl)
 
-````bash
+````sh
 openssl genrsa -des3 -out private-rsa-protected.pem 2048
 ````
 
 This will produce a private rsa key of 2048 bits protected with a password, in order to remove the password and use directly the private key in the library you can run this:
 
-```bash
+```sh
 openssl rsa -in private-rsa-protected.pem -out private-rsa.pem
 # rm private-rsa-protected.pem
 
 ```
 
 Another option (single line) is to use this command:
-```bash
+
+```sh
 openssl genpkey -out rsakey.pem -algorithm RSA -pkeyopt rsa_keygen_bits:2048
 ```
 
 The private-rsa.pem can be used with the library to generate assertions and to expose the public key part as stated before. Just place the pem in your directory and point the sdk private_certs_path to it.
 The public key is automatically generated in JWK as you can check in the expose your public keys section.
 
-It's not recommended to use rsa keys bigger than 2048 (e.g 4096) as the computational cost is not worth. It's better to have a keys rotation policy every given time (e.g. a week). It's also not recommended
-to use keys of 1024 length as it can be cracked.
-
-
+It's not recommended to use rsa keys bigger than 2048 (e.g 4096) as the computational cost is not worth.
+It's better to have a keys rotation policy every given time (e.g. a week).
+It's also not recommended to use keys of 1024 length as it can be cracked.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `baikal-sdk-1.2.3/clients/aio/aiohttp_client.py` & `baikal-sdk-1.2.4/clients/aio/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `baikal-sdk-1.2.3/clients/aio/baikal_client.py` & `baikal-sdk-1.2.4/clients/aio/baikal_client.py`

 * *Files identical despite different names*

### Comparing `baikal-sdk-1.2.3/clients/baikal_client.py` & `baikal-sdk-1.2.4/clients/baikal_client.py`

 * *Files identical despite different names*

### Comparing `baikal-sdk-1.2.3/clients/cache.py` & `baikal-sdk-1.2.4/clients/cache.py`

 * *Files identical despite different names*

### Comparing `baikal-sdk-1.2.3/setup.py` & `baikal-sdk-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     requirements = req_file.read().splitlines()
 
 with open(os.path.join(os.getcwd(), 'README.md')) as readme:
     long_description = readme.read()
 
 setup(
     name='baikal-sdk',
-    version='1.2.3',
+    version='1.2.4',
     license='Apache 2.0',
     maintainer='4th Platform team',
     maintainer_email='4pf@telefonica.com',
     url='https://github.com/Telefonica/baikal-sdk/python',
     packages=['clients', 'clients.aio'],
     description='SDK to generate tokens for the 4th Platform',
     long_description=long_description,
```

