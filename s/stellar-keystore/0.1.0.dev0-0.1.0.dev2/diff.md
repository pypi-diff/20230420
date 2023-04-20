# Comparing `tmp/stellar-keystore-0.1.0.dev0.tar.gz` & `tmp/stellar_keystore-0.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellar-keystore-0.1.0.dev0.tar", max compression
+gzip compressed data, was "stellar_keystore-0.1.0.dev2.tar", max compression
```

## Comparing `stellar-keystore-0.1.0.dev0.tar` & `stellar_keystore-0.1.0.dev2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-04-20 07:15:09.656571 stellar-keystore-0.1.0.dev0/LICENSE
--rw-r--r--   0        0        0     1942 2023-04-20 07:33:42.071880 stellar-keystore-0.1.0.dev0/README.md
--rw-r--r--   0        0        0     1413 2023-04-20 07:28:04.235109 stellar-keystore-0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     3018 2023-04-20 07:34:02.678419 stellar-keystore-0.1.0.dev0/stellar_keystore/__init__.py
--rw-r--r--   0        0        0     2764 2023-04-20 07:36:02.409292 stellar-keystore-0.1.0.dev0/setup.py
--rw-r--r--   0        0        0     3523 2023-04-20 07:36:02.409475 stellar-keystore-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-20 08:00:10.026725 stellar_keystore-0.1.0.dev2/LICENSE
+-rw-r--r--   0        0        0     1942 2023-04-20 08:00:10.026725 stellar_keystore-0.1.0.dev2/README.md
+-rw-r--r--   0        0        0     1413 2023-04-20 08:00:10.026725 stellar_keystore-0.1.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     3025 2023-04-20 08:00:10.026725 stellar_keystore-0.1.0.dev2/stellar_keystore/__init__.py
+-rw-r--r--   0        0        0     3574 1970-01-01 00:00:00.000000 stellar_keystore-0.1.0.dev2/PKG-INFO
```

### Comparing `stellar-keystore-0.1.0.dev0/LICENSE` & `stellar_keystore-0.1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `stellar-keystore-0.1.0.dev0/README.md` & `stellar_keystore-0.1.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `stellar-keystore-0.1.0.dev0/pyproject.toml` & `stellar_keystore-0.1.0.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stellar-keystore"
-version = "0.1.0.dev0"
+version = "0.1.0.dev2"
 description = "Tools for handling the encrypted keystore format used to store Stellar keypairs."
 authors = ["overcat <4catcode@gmail.com>"]
 maintainers = ["overcat <4catcode@gmail.com>"]
 homepage = "https://github.com/overcat/stellar-keystore"
 repository = "https://github.com/overcat/stellar-keystore"
 documentation = "https://github.com/overcat/stellar-keystore"
 keywords = [
```

### Comparing `stellar-keystore-0.1.0.dev0/stellar_keystore/__init__.py` & `stellar_keystore-0.1.0.dev2/stellar_keystore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         n=SCRYPT_N,
         r=SCRYPT_R,
         p=SCRYPT_P,
         dklen=DK_LEN,
     )
     secret_box = nacl.secret.SecretBox(key)
     # In my opinion, it may be better to use keypair.raw_secret_key() as data.
-    encrypted_data = secret_box.encrypt(keypair.secret.encode(), nonce=nonce)
+    encrypted_data = bytes(secret_box.encrypt(keypair.secret.encode(), nonce=nonce))
     if not encrypted_data.startswith(nonce):
         raise ValueError("Encryption failed, nonce mismatch.")
 
     encrypted_data = encrypted_data[len(nonce) :]
     return {
         "version": VERSION,
         "address": keypair.public_key,
```

### Comparing `stellar-keystore-0.1.0.dev0/PKG-INFO` & `stellar_keystore-0.1.0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellar-keystore
-Version: 0.1.0.dev0
+Version: 0.1.0.dev2
 Summary: Tools for handling the encrypted keystore format used to store Stellar keypairs.
 Home-page: https://github.com/overcat/stellar-keystore
 License: Apache-2.0
 Keywords: stellar,stellar.org,keystore,keyfile
 Author: overcat
 Author-email: 4catcode@gmail.com
 Maintainer: overcat
@@ -13,19 +13,20 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: PyNaCl (>=1.5.0,<2.0.0)
 Requires-Dist: stellar-sdk (>=8.0.0,<9.0.0)
 Project-URL: Bug Tracker, https://github.com/overcat/stellar-keystore/issues
```

