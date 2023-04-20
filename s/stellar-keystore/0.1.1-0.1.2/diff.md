# Comparing `tmp/stellar_keystore-0.1.1.tar.gz` & `tmp/stellar_keystore-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellar_keystore-0.1.1.tar", max compression
+gzip compressed data, was "stellar_keystore-0.1.2.tar", max compression
```

## Comparing `stellar_keystore-0.1.1.tar` & `stellar_keystore-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-04-20 08:17:11.649882 stellar_keystore-0.1.1/LICENSE
--rw-r--r--   0        0        0     1942 2023-04-20 08:17:11.649882 stellar_keystore-0.1.1/README.md
--rw-r--r--   0        0        0     1408 2023-04-20 08:17:11.649882 stellar_keystore-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3164 2023-04-20 08:17:11.649882 stellar_keystore-0.1.1/stellar_keystore/__init__.py
--rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 stellar_keystore-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-20 10:37:19.614376 stellar_keystore-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1942 2023-04-20 10:37:19.614376 stellar_keystore-0.1.2/README.md
+-rw-r--r--   0        0        0     1408 2023-04-20 10:37:19.614376 stellar_keystore-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3213 2023-04-20 10:37:19.614376 stellar_keystore-0.1.2/stellar_keystore/__init__.py
+-rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 stellar_keystore-0.1.2/PKG-INFO
```

### Comparing `stellar_keystore-0.1.1/LICENSE` & `stellar_keystore-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stellar_keystore-0.1.1/README.md` & `stellar_keystore-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `stellar_keystore-0.1.1/pyproject.toml` & `stellar_keystore-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stellar-keystore"
-version = "0.1.1"
+version = "0.1.2"
 description = "Tools for handling the encrypted keystore format used to store Stellar keypairs."
 authors = ["overcat <4catcode@gmail.com>"]
 maintainers = ["overcat <4catcode@gmail.com>"]
 homepage = "https://github.com/overcat/stellar-keystore"
 repository = "https://github.com/overcat/stellar-keystore"
 documentation = "https://github.com/overcat/stellar-keystore"
 keywords = [
```

### Comparing `stellar_keystore-0.1.1/stellar_keystore/__init__.py` & `stellar_keystore-0.1.2/stellar_keystore/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import nacl.secret
 from nacl.hashlib import scrypt
 from stellar_sdk import Keypair
 
 __all__ = ["create_keystore", "load_keystore"]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 VERSION = "stellarport-1-20-2018"
 NONCE_SIZE = nacl.secret.SecretBox.NONCE_SIZE
 SALT_SIZE = 32
 DK_LEN = nacl.secret.SecretBox.KEY_SIZE
 SCRYPT_N = 16384
 SCRYPT_R = 8
@@ -42,22 +42,22 @@
     )
     secret_box = nacl.secret.SecretBox(key)
     # In my opinion, it may be better to use keypair.raw_secret_key() as data.
     encrypted_data = bytes(secret_box.encrypt(keypair.secret.encode(), nonce=nonce))
     if not encrypted_data.startswith(nonce):
         raise ValueError("Encryption failed, nonce mismatch.")
 
-    encrypted_data = encrypted_data[len(nonce):]
+    encrypted_data = encrypted_data[len(nonce) :]
     return {
         "version": VERSION,
         "address": keypair.public_key,
         "crypto": {
-            "ciphertext": base64.b64encode(encrypted_data),
-            "nonce": base64.b64encode(nonce),
-            "salt": base64.b64encode(salt),
+            "ciphertext": base64.b64encode(encrypted_data).decode("utf-8"),
+            "nonce": base64.b64encode(nonce).decode("utf-8"),
+            "salt": base64.b64encode(salt).decode("utf-8"),
             "scryptOptions": {
                 "N": SCRYPT_N,
                 "r": SCRYPT_R,
                 "p": SCRYPT_P,
                 "dkLen": DK_LEN,
                 "encoding": ENCODING_FORMAT,
             },
```

### Comparing `stellar_keystore-0.1.1/PKG-INFO` & `stellar_keystore-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellar-keystore
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tools for handling the encrypted keystore format used to store Stellar keypairs.
 Home-page: https://github.com/overcat/stellar-keystore
 License: Apache-2.0
 Keywords: stellar,stellar.org,keystore,keyfile
 Author: overcat
 Author-email: 4catcode@gmail.com
 Maintainer: overcat
```

