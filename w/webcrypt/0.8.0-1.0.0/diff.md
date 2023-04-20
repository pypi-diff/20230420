# Comparing `tmp/webcrypt-0.8.0.tar.gz` & `tmp/webcrypt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcrypt-0.8.0.tar", max compression
+gzip compressed data, was "webcrypt-1.0.0.tar", max compression
```

## Comparing `webcrypt-0.8.0.tar` & `webcrypt-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11380 2021-10-25 12:47:57.112731 webcrypt-0.8.0/LICENSE
--rw-r--r--   0        0        0    12505 2022-07-27 17:27:14.454650 webcrypt-0.8.0/README.md
--rw-r--r--   0        0        0     1485 2022-07-27 18:00:50.793350 webcrypt-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      179 2022-07-27 17:59:39.040271 webcrypt-0.8.0/src/webcrypt/__init__.py
--rw-r--r--   0        0        0     8977 2022-04-01 15:50:54.281931 webcrypt-0.8.0/src/webcrypt/convert.py
--rw-r--r--   0        0        0     1488 2021-10-26 19:39:55.806783 webcrypt-0.8.0/src/webcrypt/exceptions.py
--rw-r--r--   0        0        0    24611 2022-01-09 22:14:17.418709 webcrypt-0.8.0/src/webcrypt/jose.py
--rw-r--r--   0        0        0    50351 2022-01-09 22:03:24.247715 webcrypt-0.8.0/src/webcrypt/jwe.py
--rw-r--r--   0        0        0    31221 2022-01-09 22:00:16.027898 webcrypt-0.8.0/src/webcrypt/jws.py
--rw-r--r--   0        0        0    38591 2022-07-27 17:36:25.687109 webcrypt-0.8.0/src/webcrypt/keys.py
--rw-r--r--   0        0        0        0 2021-09-15 18:36:12.217801 webcrypt-0.8.0/src/webcrypt/py.typed
--rw-r--r--   0        0        0    21795 2021-10-26 16:51:52.152041 webcrypt-0.8.0/src/webcrypt/rfc1751.py
--rw-r--r--   0        0        0    13629 2022-07-27 18:02:06.938031 webcrypt-0.8.0/setup.py
--rw-r--r--   0        0        0    13415 2022-07-27 18:02:06.939077 webcrypt-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11380 2021-10-25 12:47:57.000000 webcrypt-1.0.0/LICENSE
+-rw-r--r--   0        0        0    12505 2022-07-27 17:27:14.000000 webcrypt-1.0.0/README.md
+-rw-r--r--   0        0        0     1589 2023-04-20 16:11:01.991519 webcrypt-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      179 2022-07-28 02:11:08.000000 webcrypt-1.0.0/src/webcrypt/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-20 16:11:01.991519 webcrypt-1.0.0/src/webcrypt/cli.py
+-rw-r--r--   0        0        0     8977 2022-04-01 15:50:54.000000 webcrypt-1.0.0/src/webcrypt/convert.py
+-rw-r--r--   0        0        0     1488 2021-10-26 19:39:55.000000 webcrypt-1.0.0/src/webcrypt/exceptions.py
+-rw-r--r--   0        0        0    24611 2022-01-09 22:14:17.000000 webcrypt-1.0.0/src/webcrypt/jose.py
+-rw-r--r--   0        0        0    50351 2022-01-09 22:03:24.000000 webcrypt-1.0.0/src/webcrypt/jwe.py
+-rw-r--r--   0        0        0    31221 2022-01-09 22:00:16.000000 webcrypt-1.0.0/src/webcrypt/jws.py
+-rw-r--r--   0        0        0    38591 2022-07-27 17:36:25.000000 webcrypt-1.0.0/src/webcrypt/keys.py
+-rw-r--r--   0        0        0        0 2021-09-15 18:36:12.000000 webcrypt-1.0.0/src/webcrypt/py.typed
+-rw-r--r--   0        0        0    21795 2021-10-26 16:51:52.000000 webcrypt-1.0.0/src/webcrypt/rfc1751.py
+-rw-r--r--   0        0        0    13556 1970-01-01 00:00:00.000000 webcrypt-1.0.0/PKG-INFO
```

### Comparing `webcrypt-0.8.0/LICENSE` & `webcrypt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `webcrypt-0.8.0/README.md` & `webcrypt-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `webcrypt-0.8.0/pyproject.toml` & `webcrypt-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "webcrypt"
-version = "0.8.0"
+version = "1.0.0"
 description = "High level Constructs for Web App cryptography and JOSE spec implementation"
 license = "Apache-2.0"
 authors = ["mk <mk@plataux.com>"]
 maintainers = []
 readme = "README.md"
 homepage = "https://plataux.com"
 repository = "https://github.com/plataux/webcrypt"
@@ -18,28 +18,32 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent"
 ]
 packages = [
     { include = "webcrypt", from = "src" },
 ]
 
+[tool.poetry.scripts]
+webcrypt = "webcrypt.cli:main"
+
 
 [tool.poetry.dependencies]
-python = "^3.8"
-pydantic = "^1.9"
-cryptography = "^37.0"
+python = ">=3.8,<4"
+pydantic = "^1.10"
+cryptography = "^40.0"
+typer = {extras = ["all"], version = "^0.6.1"}
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0"
 tox = "^3.24"
-pytest = "^6.2"
-pytest-cov = "^3.0"
-mypy = "^0.910"
-sphinx = "^4.2"
-sphinx-rtd-theme = "^1.0"
+pytest = "^7.3"
+pytest-cov = "^4.0"
+mypy = "^1.2"
+sphinx = "^4.4"
+sphinx-rtd-theme = "^1.2"
 recommonmark = "^0.7"
 
 
 [tool.mypy]
 mypy_path = "src"
 check_untyped_defs = true
 disallow_any_generics = true
```

### Comparing `webcrypt-0.8.0/src/webcrypt/convert.py` & `webcrypt-1.0.0/src/webcrypt/convert.py`

 * *Files identical despite different names*

### Comparing `webcrypt-0.8.0/src/webcrypt/exceptions.py` & `webcrypt-1.0.0/src/webcrypt/exceptions.py`

 * *Files identical despite different names*

### Comparing `webcrypt-0.8.0/src/webcrypt/jose.py` & `webcrypt-1.0.0/src/webcrypt/jose.py`

 * *Files identical despite different names*

### Comparing `webcrypt-0.8.0/src/webcrypt/jwe.py` & `webcrypt-1.0.0/src/webcrypt/jwe.py`

 * *Files identical despite different names*

### Comparing `webcrypt-0.8.0/src/webcrypt/jws.py` & `webcrypt-1.0.0/src/webcrypt/jws.py`

 * *Files identical despite different names*

### Comparing `webcrypt-0.8.0/src/webcrypt/keys.py` & `webcrypt-1.0.0/src/webcrypt/keys.py`

 * *Files identical despite different names*

### Comparing `webcrypt-0.8.0/src/webcrypt/rfc1751.py` & `webcrypt-1.0.0/src/webcrypt/rfc1751.py`

 * *Files identical despite different names*

### Comparing `webcrypt-0.8.0/setup.py` & `webcrypt-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,393 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: webcrypt
+Version: 1.0.0
+Summary: High level Constructs for Web App cryptography and JOSE spec implementation
+Home-page: https://plataux.com
+License: Apache-2.0
+Keywords: cryptography,security
+Author: mk
+Author-email: mk@plataux.com
+Requires-Python: >=3.8,<4
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: cryptography (>=40.0,<41.0)
+Requires-Dist: pydantic (>=1.10,<2.0)
+Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
+Project-URL: Repository, https://github.com/plataux/webcrypt
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Webcrypt
 
-packages = \
-['webcrypt']
+Webcrypt is a collection of Python3 tools and constructs that aim to simplify the implementation
+of all sorts of high-level cryptographic functionality commonly needed in the 
+development of modern, distributed, and security-focused web applications.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['cryptography>=37.0,<38.0', 'pydantic>=1.9,<2.0']
-
-setup_kwargs = {
-    'name': 'webcrypt',
-    'version': '0.8.0',
-    'description': 'High level Constructs for Web App cryptography and JOSE spec implementation',
-    'long_description': '# Webcrypt\n\nWebcrypt is a collection of Python3 tools and constructs that aim to simplify the implementation\nof all sorts of high-level cryptographic functionality commonly needed in the \ndevelopment of modern, distributed, and security-focused web applications.\n\nAt its core, Webcrypt relies entirely and **only** on the Python Library ``cryptography`` for all \ncryptographic operations, and acts as a thin wrapper around this library\'s primitives to provide \na high level API that is easier to use in the context of business software development.\n\nThis project borrows ideas from, and is inspired by other Python libraries including:\n\n* ``pycryptodome``\n* ``python-jose``\n\n``pip install "git+https://github.com/plataux/webcrypt@v0.6.1"``\n\n## Project Goals\n\n* Provide all the essential cryptographic tools:\n  * That can be used directly: encryption/decryption, signing/verification\n  * upon which higher level business protocols can be established (for example, nesting of JWTs)\n* Implement most of the essential aspects of JOSE spec to maximize interoperability with other frameworks\n* optimize for Production use:\n  * Focusing on Performance (by caching and reusing validated cryptographic constructs as much as possible)\n  * Focusing on Security (apply thorough validation steps when handling external signatures and other external entities)\n* Promote secure practices:\n  * wherever applicable, rejecting algorithms of insufficient strengths or known vulnerabilities\n  * Defaults to algorithms / key lengths that are reasonably secure and reasonably fast\n  * Make it easier to create new keys, and retire old ones\n\n## Current Features\n\n* Support for most of the JWS signature algorithms: https://datatracker.ietf.org/doc/html/rfc7518#section-3.1:\n  * All HMAC algorithms: ``HS256``, ``HS384``, ``HS512``\n  * All RSA algorithms: ``RS256``, ``RS384``, ``RS512`` and ``PS256``, ``PS384``, ``PS512``\n  * All Elliptic Curve Algorithms: ``ES256``, ``ES384``, ``ES512``\n  * Leaving out only ``none`` algorithm for JWT signatures\n\n* Support for all the JWE Encryption and Key Wrapping Algorithms https://datatracker.ietf.org/doc/html/rfc7518#section-4.1:\n  * All content encryption algorithms: ``A128GCM``, ``A192GCM``, ``A256GCM``, ``A128CBC-HS256``, ``A192CBC-HS384``, ``A256CBC-HS512``\n  * direct ``dir`` encryption using any of the Encryption Algorithms defined by the standard\n  * AES key wrapping of a newly, randomly Generated CEK: ``A128KW``, ``A192KW`` and ``A256KW``\n  * AES-GCM encryption of a newly, randomly generated CEK: ``A128GCMKW``, ``A192GCMKW`` and ``A256GCMKW``\n  * Password-Based Encryption algorithms: ``PBES2-HS256+A128KW``, ``PBES2-HS384+A192KW``, ``PBES2-HS512+A256KW``\n  * RSA key wrapping of CEKs: ``RSA1_5``, ``RSA-OAEP`` and ``RSA-OAEP-256``\n  * ECDH-ES key derivation for direct use, or wrapping of a CEK: ``ECDH-ES``, ``ECDH-ES+A128KW``, ``ECDH-ES+A192KW``, ``ECDH-ES+A256KW``\n\n* Simple API to export and import key sets (JWKS), and public JWKS from Private JWKS\n* Using ``Pydantic`` to validate, serialize and deserialize JWT Tokens \n\n\n## Usage\n\n### JWS Signing and Verification\n\n#### Default Creation and usage of JWS Signing Objects\n\nSign and retrieve byte payloads to and from unicode JWTs. The ``verify`` method will raise\nmany kinds of ``TokenException`` if the JWT is fabricated, corrupted or tampered with in any way\n```python\nfrom webcrypt.jws import JWS\n\n# Creates a new signing key with algorithm ES256 by default - it is fast, and can be verified by clients\nsigner = JWS()\n\npayload = b\'Byte Data to be signed and verified\'\n\ntoken: str = signer.sign(payload)\n\nprint(token)\n# will produce something like this\n# eyJhbGciOiJFUzI1NiIsImt0eSI6IkVDIiwia2lkIjoiZWFjNTgyMWMtZDQ3Yi00ZTA4LWEwMTMtOWQxOWUzNmNkNGRkIn0.\n# RGF0YSB0byBiZSBzaWduZWQgYW5kIHZlcmlmaWVk.tvQcT6S33H9auuGqNyYm_VHsA8I0Bw6NaLGi6plJCwmnr9oKXS78lZYI\n# 9ndlju6dnNXdP3nCAxZuyR9I0vxS-A\n\ndecoded_payload = signer.verify(token)\n\nassert payload == decoded_payload\n```\n\n#### Creation and usage of other JWS algorithms\nThe ``Algorithm`` Enum in the JWS class contains all Algorithms defined by the JOSE spec.\nThe following is an example of newly created signature keys:\n\n* All newly created RSA keys are 2048 bits (minimal recommended, and faster than 3072 and 4096 bit key sizes)\n* All newly created HMAC and EC keys match the length of the Hashing Algorithm used\n```python\nfrom webcrypt.jws import JWS\n\nk1 = JWS(JWS.Algorithm.RS512) # new RSA 2048 bit key with SHA512 hashing and PKCS1v15 Padding\nk2 = JWS(JWS.Algorithm.PS384) # new RSA 2048 bit with SHA384 hashing and PSS Padding\nk3 = JWS(JWS.Algorithm.HS256) # new HMAC signing key with SHA256 Hashing\nk4 = JWS(JWS.Algorithm.ES512) # new Elliptic Curve P-521 (SECP521R1) key, with SHA512 Hashing\n```\n\n#### Loading Existing Keys\n\nJWS Signing keys can be loaded from existing keys in various formats:\n\n* PEM formats\n* ``cryptography`` key objects\n* JWK (JSON Web Key) JSON Format\n\n##### From PEM\n```python\nfrom webcrypt.jws import JWS\n\n# This is a P-256 Curve EC key\nprivkey_pem = """-----BEGIN PRIVATE KEY-----\nMIGHAgEAMBMGByqGSM49AgEGCCqGSM49AwEHBG0wawIBAQQg2/Hi1u+D8HYixWoY\nCl0uQnq9KscIlSw5N2sGJJaWcv+hRANCAASmX7fu++yJAxOCUODmf9ZX14zU0IXb\ndXn5a9lL4Dswt/LLzVAo2DQQWe9nviYx0xb2txYXbtssaqEDUPeKAklF\n-----END PRIVATE KEY-----\n"""\n\n# Since this is a P-256 curve key, a The JWS Algorithm ES256 MUST be used, as per the JOSE spec\n# This key can sign, and verify\nec_jws = JWS.from_pem(privkey_pem,algorithm=JWS.Algorithm.ES256)\n\n\n# this is a 3072 RSA Public Key - can only verify JWTs, but cannot be used to sign\npubkey_pem="""-----BEGIN PUBLIC KEY-----\nMIIBojANBgkqhkiG9w0BAQEFAAOCAY8AMIIBigKCAYEAqBALJZGWr4zAvQsnj8e5\nxIX5KA74Nel7+Q8RR9HW80y+5t2pGpQuObX7WvuXhrkCFGgWxqvaIu7Z9XsxYAv/\nI4waVtoYOjUVH4w4aDI+SpOe8duiF5nAxpiaHp5h4ubDjQcipzsJyp3QQS7qqUAf\nwwNRwJQcYrdchJrFO9AQ/Wg7Actd7O8Ijhh0mSXID/hEVanBwrRuAq8GwQfDSv1Q\nMXNzC9k6ZlecKkUD2aRpTHPUbjbTZcGfPBnACdih2QMkQ+8XvOfIQqKuCM/MDVmD\nqbmQG6t/Bbsxa32cGBXVGmb+JW+e1TnQCF9i5xnOwKj6F08NVCzWaub8+heQeUJX\ngwpdVeejQS9w1q+eO5Ts6EGxOvnTbEs2WboRP7Hi8y1NE7PlKmOCHRQrdWdTaqTH\nj/BXR2V9LT0nNwC2/SnpDtqz9lbFJSvEKpLp4h7BDBuhnjfw6kywyRYaM5Q3HvHM\niiiRP4MeERT4cYKkGiV+GtpjzKqRqYpkDSzcueTNRUhlAgMBAAE=\n-----END PUBLIC KEY-----\n"""\n\n# all JWS RSA Algorithms are applicable with this (or any other) RSA keys (of size 2048 bits or larger)\nrsa_verifier = JWS.from_pem(pubkey_pem,JWS.Algorithm.PS512)\n\n# based on the above parameters, this key can verify signatures by the corresponding Private Key\n# With the specified PS512 JWS Algorithm\n```\n\n##### From cryptography objects\n```python\nfrom webcrypt.jws import JWS\nfrom cryptography.hazmat.primitives.asymmetric import rsa\n\n# assuming this is an existing 4096 bit RSA Private key\nprivkey = rsa.generate_private_key(public_exponent=65537,key_size=1024*4)\n\n# The corresponding Public key to be shared with partners, clients and other third parties\npubkey = privkey.public_key()\n\ndata = b\'Some data to be signed and verified\'\n\n# Uses SHA384 and PKCS1v15 Padding. Can be used to sign and verify\npriv_jwk = JWS(algorithm=JWS.Algorithm.RS384, key_obj=privkey)\n\ntoken = priv_jwk.sign(data)\n\n#######################\n# Somewhere else, construct the JWS object with the public key, and the agreed upon algorithm\n\n# cannot sign, but can verify signatures\npub_jwk = JWS(algorithm=JWS.Algorithm.RS384,key_obj=pubkey)\n\nsigned_data = pub_jwk.verify(token)\nassert signed_data == data\n```\n\n\n##### Exporting and Importing JWK JSON objects\n\nThis is the preferred and easiest method to store, and restore JWK objects, since it includes\nthe private and/or the public key components, as well as the algorithm and the intended usage of the key\n\n```python\nprivkey_jwk="""\n{\n  "use": "sig",\n  "kid": "23b5973e-7257-4fbc-944b-3f79e01da799",\n  "kty": "EC",\n  "alg": "ES384",\n  "key_ops": [\n    "sign",\n    "verify"\n  ],\n  "crv": "P-384",\n  "x": "xcICJQvPvomxkue8ZOE9AsKSSlGwYhEOBpscwdpiFK4jzkh2zGvaq1Ek5wY1BkxU",\n  "y": "Q6VVuYPTlVvZLZYTbtOoxfNUD3kqJs4ZEqQ6mt5cxfOHCc0mGqrGGcnhAZ95YKZ0",\n  "d": "mhKUB-5-leY-XBciNcSRFDEeUJuA4h6rzwaDoxyCeNkTLtauElWoWsRvN8Xu9rIh"\n}\n"""\n\nfrom webcrypt.jws import JWS\nimport json\n\n# can sign and verify\nsigner = JWS.from_jwk(json.loads(privkey_jwk))\n\n# export public components\npublic_jwk = signer.public_jwk()\n\n# which looks something like this:\npubkey_jwk = """{\n  "use": "sig",\n  "kid": "23b5973e-7257-4fbc-944b-3f79e01da799",\n  "kty": "EC",\n  "alg": "ES384",\n  "key_ops": [\n    "verify"\n  ],\n  "crv": "P-384",\n  "x": "xcICJQvPvomxkue8ZOE9AsKSSlGwYhEOBpscwdpiFK4jzkh2zGvaq1Ek5wY1BkxU",\n  "y": "Q6VVuYPTlVvZLZYTbtOoxfNUD3kqJs4ZEqQ6mt5cxfOHCc0mGqrGGcnhAZ95YKZ0"\n}"""\n\n# can verify, but cannot sign\nverifier = JWS.from_jwk(json.loads(pubkey_jwk))\n\n```\n\n### JWE Key Wrapping and Encryption\n\nMost JWE Algorithm involve using a private key to directly encrypt, or to wrap\na newly created CEK (Content Encryption Key)\n\n#### JWE private AES keys for direct ``dir`` encryption:\n\n```python\nfrom webcrypt.jwe import JWE\nimport json\n\n# generate a new 192-bit key used directly in content Encryption\njwk1 = JWE(algorithm=JWE.Algorithm.DIR, encryption=JWE.Encryption.A192GCM)\n\n# generate a new 256-bit key used directly in content Encryption + HMAC Authentication\njwk2 = JWE(algorithm=JWE.Algorithm.DIR, encryption=JWE.Encryption.A128CBC_HS256)\n\n# export jwk1:\nprint(json.dumps(jwk1.to_jwk(),indent=4))\n\n# will look like this:\nprivkey = """{\n    "use": "enc",\n    "kid": "be29da9a-3a89-4839-a664-68de669f145a",\n    "kty": "oct",\n    "alg": "dir",\n    "enc": "A128GCM",\n    "key_ops": [\n        "encrypt",\n        "decrypt"\n    ],\n    "k": "L35wm0tFTg12nKcZviyv1Q"\n}\n"""\n\njwk_reloaded = JWE.from_jwk(json.loads(privkey))\n\ndata = b\'Some byte data to be encrypted then decrypted\'\n\ntoken = jwk_reloaded.encrypt(data,compress=True) # option to compress the data\n\ndata_decrypted = jwk_reloaded.decrypt(token)\n\nassert data_decrypted == data\n\n```\n\n\n#### JWE Key-wrapping Algorithms:\n\n```python\nfrom webcrypt.jwe import JWE\nimport json\n\n# Generate a 192-bit private key to wrap a 256-bit CEK for encrypting and decrypting data\njwk1 = JWE(algorithm=JWE.Algorithm.A192KW, encryption=JWE.Encryption.A256GCM)\n\n# Generate a 256-bit private key to encrypt and wrap a 512-bit key for Encryption + Authentication\njwk2 = JWE(algorithm=JWE.Algorithm.A256GCMKW, encryption=JWE.Encryption.A256CBC_HS512)\n\n# Generate a 128-bit private key to wrap a 192-bit CEK for encrypting and decrypting data\njwk3 = JWE(algorithm=JWE.Algorithm.A128KW, encryption=JWE.Encryption.A192GCM)\n\nprint(json.dumps(jwk2.to_jwk(),indent=4))\n\n# will produce something like this:\n\njwk_json = """{\n    "use": "enc",\n    "kid": "f47a54c3-85d8-46b8-a9cb-8a1b5f47eddb",\n    "kty": "oct",\n    "alg": "A256GCMKW",\n    "enc": "A256CBC-HS512",\n    "key_ops": [\n        "wrapKey",\n        "unwrapKey"\n    ],\n    "k": "dkcM5Fnj7oYN4r4NGs7RMVxSX1jcT9gwvoRgxXJ4um8"\n}\n\n"""\n\n# which can later be reloaded for encryption / decryption operations\njwe_key = JWE.from_jwk(json.loads(jwk_json))\n```\n\n\n#### JWE RSA Key-wrapping Algorithms\n\n```python\nfrom webcrypt.jwe import JWE\n\n# Examples of all RSA Algorithms, with different CEK sizes\n\njwe1 = JWE(algorithm=JWE.Algorithm.RSA_OAEP_256, encryption=JWE.Encryption.A192GCM)\njwe2 = JWE(algorithm=JWE.Algorithm.RSA_OAEP, encryption=JWE.Encryption.A128CBC_HS256)\njwe3 = JWE(algorithm=JWE.Algorithm.RSA1_5, encryption=JWE.Encryption.A256GCM)\n\n\n# Load a Public JWE key from the JWK of a private one\npub_jwe = JWE.from_jwk(jwe1.public_jwk())\n\ndata = b\'Byte data to be encrypted and decrypted\'\n\n# encrypt data, and wrap the CEK\ntoken = pub_jwe.encrypt(data)\n\n# Raises an Error, a public key cannot decrypt the CEK!\npub_jwe.decrypt(token)\n\n# only the corresponding private key can unwrap the CEK and decrypt the data\ndata_decrypted = jwe1.decrypt(token)\n\nassert data_decrypted == data\n```\n\n\n#### JWE PBE (Passphrase based Encryption) Algorithms\n\n```python\nfrom webcrypt.jwe import JWE\nimport json\n\n# Generate a 192-bit private key to wrap a 384-bit key for Authentication + Encryption\njwk = JWE(algorithm=JWE.Algorithm.PBES2_HS384_A192KW,\n          encryption=JWE.Encryption.A256GCM,\n          key="I love python")\n\ndata = b\'Some secret data\'\n\ntoken = jwk.encrypt(data)\n\nprint(json.dumps(JWE.decode_header(token), indent=4))\n\n# the Token header will look something like this, including the alg, enc and\n# the PBE salt and iteration count (p2s and p2c)\nheader="""{\n    "alg": "PBES2-HS384+A192KW",\n    "enc": "A256GCM",\n    "kid": "08842033-5f83-477b-9be3-c91ab6e7635c",\n    "p2s": "7jByuyCgOWc4aEfkoAJ0VQ",\n    "p2c": 1644\n}"""\n```\n',
-    'author': 'mk',
-    'author_email': 'mk@plataux.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://plataux.com',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+At its core, Webcrypt relies entirely and **only** on the Python Library ``cryptography`` for all 
+cryptographic operations, and acts as a thin wrapper around this library's primitives to provide 
+a high level API that is easier to use in the context of business software development.
+
+This project borrows ideas from, and is inspired by other Python libraries including:
+
+* ``pycryptodome``
+* ``python-jose``
+
+``pip install "git+https://github.com/plataux/webcrypt@v0.6.1"``
+
+## Project Goals
+
+* Provide all the essential cryptographic tools:
+  * That can be used directly: encryption/decryption, signing/verification
+  * upon which higher level business protocols can be established (for example, nesting of JWTs)
+* Implement most of the essential aspects of JOSE spec to maximize interoperability with other frameworks
+* optimize for Production use:
+  * Focusing on Performance (by caching and reusing validated cryptographic constructs as much as possible)
+  * Focusing on Security (apply thorough validation steps when handling external signatures and other external entities)
+* Promote secure practices:
+  * wherever applicable, rejecting algorithms of insufficient strengths or known vulnerabilities
+  * Defaults to algorithms / key lengths that are reasonably secure and reasonably fast
+  * Make it easier to create new keys, and retire old ones
+
+## Current Features
+
+* Support for most of the JWS signature algorithms: https://datatracker.ietf.org/doc/html/rfc7518#section-3.1:
+  * All HMAC algorithms: ``HS256``, ``HS384``, ``HS512``
+  * All RSA algorithms: ``RS256``, ``RS384``, ``RS512`` and ``PS256``, ``PS384``, ``PS512``
+  * All Elliptic Curve Algorithms: ``ES256``, ``ES384``, ``ES512``
+  * Leaving out only ``none`` algorithm for JWT signatures
+
+* Support for all the JWE Encryption and Key Wrapping Algorithms https://datatracker.ietf.org/doc/html/rfc7518#section-4.1:
+  * All content encryption algorithms: ``A128GCM``, ``A192GCM``, ``A256GCM``, ``A128CBC-HS256``, ``A192CBC-HS384``, ``A256CBC-HS512``
+  * direct ``dir`` encryption using any of the Encryption Algorithms defined by the standard
+  * AES key wrapping of a newly, randomly Generated CEK: ``A128KW``, ``A192KW`` and ``A256KW``
+  * AES-GCM encryption of a newly, randomly generated CEK: ``A128GCMKW``, ``A192GCMKW`` and ``A256GCMKW``
+  * Password-Based Encryption algorithms: ``PBES2-HS256+A128KW``, ``PBES2-HS384+A192KW``, ``PBES2-HS512+A256KW``
+  * RSA key wrapping of CEKs: ``RSA1_5``, ``RSA-OAEP`` and ``RSA-OAEP-256``
+  * ECDH-ES key derivation for direct use, or wrapping of a CEK: ``ECDH-ES``, ``ECDH-ES+A128KW``, ``ECDH-ES+A192KW``, ``ECDH-ES+A256KW``
+
+* Simple API to export and import key sets (JWKS), and public JWKS from Private JWKS
+* Using ``Pydantic`` to validate, serialize and deserialize JWT Tokens 
+
+
+## Usage
+
+### JWS Signing and Verification
+
+#### Default Creation and usage of JWS Signing Objects
+
+Sign and retrieve byte payloads to and from unicode JWTs. The ``verify`` method will raise
+many kinds of ``TokenException`` if the JWT is fabricated, corrupted or tampered with in any way
+```python
+from webcrypt.jws import JWS
+
+# Creates a new signing key with algorithm ES256 by default - it is fast, and can be verified by clients
+signer = JWS()
+
+payload = b'Byte Data to be signed and verified'
+
+token: str = signer.sign(payload)
+
+print(token)
+# will produce something like this
+# eyJhbGciOiJFUzI1NiIsImt0eSI6IkVDIiwia2lkIjoiZWFjNTgyMWMtZDQ3Yi00ZTA4LWEwMTMtOWQxOWUzNmNkNGRkIn0.
+# RGF0YSB0byBiZSBzaWduZWQgYW5kIHZlcmlmaWVk.tvQcT6S33H9auuGqNyYm_VHsA8I0Bw6NaLGi6plJCwmnr9oKXS78lZYI
+# 9ndlju6dnNXdP3nCAxZuyR9I0vxS-A
+
+decoded_payload = signer.verify(token)
+
+assert payload == decoded_payload
+```
+
+#### Creation and usage of other JWS algorithms
+The ``Algorithm`` Enum in the JWS class contains all Algorithms defined by the JOSE spec.
+The following is an example of newly created signature keys:
+
+* All newly created RSA keys are 2048 bits (minimal recommended, and faster than 3072 and 4096 bit key sizes)
+* All newly created HMAC and EC keys match the length of the Hashing Algorithm used
+```python
+from webcrypt.jws import JWS
+
+k1 = JWS(JWS.Algorithm.RS512) # new RSA 2048 bit key with SHA512 hashing and PKCS1v15 Padding
+k2 = JWS(JWS.Algorithm.PS384) # new RSA 2048 bit with SHA384 hashing and PSS Padding
+k3 = JWS(JWS.Algorithm.HS256) # new HMAC signing key with SHA256 Hashing
+k4 = JWS(JWS.Algorithm.ES512) # new Elliptic Curve P-521 (SECP521R1) key, with SHA512 Hashing
+```
+
+#### Loading Existing Keys
+
+JWS Signing keys can be loaded from existing keys in various formats:
+
+* PEM formats
+* ``cryptography`` key objects
+* JWK (JSON Web Key) JSON Format
+
+##### From PEM
+```python
+from webcrypt.jws import JWS
+
+# This is a P-256 Curve EC key
+privkey_pem = """-----BEGIN PRIVATE KEY-----
+MIGHAgEAMBMGByqGSM49AgEGCCqGSM49AwEHBG0wawIBAQQg2/Hi1u+D8HYixWoY
+Cl0uQnq9KscIlSw5N2sGJJaWcv+hRANCAASmX7fu++yJAxOCUODmf9ZX14zU0IXb
+dXn5a9lL4Dswt/LLzVAo2DQQWe9nviYx0xb2txYXbtssaqEDUPeKAklF
+-----END PRIVATE KEY-----
+"""
+
+# Since this is a P-256 curve key, a The JWS Algorithm ES256 MUST be used, as per the JOSE spec
+# This key can sign, and verify
+ec_jws = JWS.from_pem(privkey_pem,algorithm=JWS.Algorithm.ES256)
+
+
+# this is a 3072 RSA Public Key - can only verify JWTs, but cannot be used to sign
+pubkey_pem="""-----BEGIN PUBLIC KEY-----
+MIIBojANBgkqhkiG9w0BAQEFAAOCAY8AMIIBigKCAYEAqBALJZGWr4zAvQsnj8e5
+xIX5KA74Nel7+Q8RR9HW80y+5t2pGpQuObX7WvuXhrkCFGgWxqvaIu7Z9XsxYAv/
+I4waVtoYOjUVH4w4aDI+SpOe8duiF5nAxpiaHp5h4ubDjQcipzsJyp3QQS7qqUAf
+wwNRwJQcYrdchJrFO9AQ/Wg7Actd7O8Ijhh0mSXID/hEVanBwrRuAq8GwQfDSv1Q
+MXNzC9k6ZlecKkUD2aRpTHPUbjbTZcGfPBnACdih2QMkQ+8XvOfIQqKuCM/MDVmD
+qbmQG6t/Bbsxa32cGBXVGmb+JW+e1TnQCF9i5xnOwKj6F08NVCzWaub8+heQeUJX
+gwpdVeejQS9w1q+eO5Ts6EGxOvnTbEs2WboRP7Hi8y1NE7PlKmOCHRQrdWdTaqTH
+j/BXR2V9LT0nNwC2/SnpDtqz9lbFJSvEKpLp4h7BDBuhnjfw6kywyRYaM5Q3HvHM
+iiiRP4MeERT4cYKkGiV+GtpjzKqRqYpkDSzcueTNRUhlAgMBAAE=
+-----END PUBLIC KEY-----
+"""
+
+# all JWS RSA Algorithms are applicable with this (or any other) RSA keys (of size 2048 bits or larger)
+rsa_verifier = JWS.from_pem(pubkey_pem,JWS.Algorithm.PS512)
+
+# based on the above parameters, this key can verify signatures by the corresponding Private Key
+# With the specified PS512 JWS Algorithm
+```
+
+##### From cryptography objects
+```python
+from webcrypt.jws import JWS
+from cryptography.hazmat.primitives.asymmetric import rsa
+
+# assuming this is an existing 4096 bit RSA Private key
+privkey = rsa.generate_private_key(public_exponent=65537,key_size=1024*4)
+
+# The corresponding Public key to be shared with partners, clients and other third parties
+pubkey = privkey.public_key()
+
+data = b'Some data to be signed and verified'
+
+# Uses SHA384 and PKCS1v15 Padding. Can be used to sign and verify
+priv_jwk = JWS(algorithm=JWS.Algorithm.RS384, key_obj=privkey)
+
+token = priv_jwk.sign(data)
+
+#######################
+# Somewhere else, construct the JWS object with the public key, and the agreed upon algorithm
+
+# cannot sign, but can verify signatures
+pub_jwk = JWS(algorithm=JWS.Algorithm.RS384,key_obj=pubkey)
+
+signed_data = pub_jwk.verify(token)
+assert signed_data == data
+```
+
+
+##### Exporting and Importing JWK JSON objects
+
+This is the preferred and easiest method to store, and restore JWK objects, since it includes
+the private and/or the public key components, as well as the algorithm and the intended usage of the key
+
+```python
+privkey_jwk="""
+{
+  "use": "sig",
+  "kid": "23b5973e-7257-4fbc-944b-3f79e01da799",
+  "kty": "EC",
+  "alg": "ES384",
+  "key_ops": [
+    "sign",
+    "verify"
+  ],
+  "crv": "P-384",
+  "x": "xcICJQvPvomxkue8ZOE9AsKSSlGwYhEOBpscwdpiFK4jzkh2zGvaq1Ek5wY1BkxU",
+  "y": "Q6VVuYPTlVvZLZYTbtOoxfNUD3kqJs4ZEqQ6mt5cxfOHCc0mGqrGGcnhAZ95YKZ0",
+  "d": "mhKUB-5-leY-XBciNcSRFDEeUJuA4h6rzwaDoxyCeNkTLtauElWoWsRvN8Xu9rIh"
+}
+"""
+
+from webcrypt.jws import JWS
+import json
+
+# can sign and verify
+signer = JWS.from_jwk(json.loads(privkey_jwk))
+
+# export public components
+public_jwk = signer.public_jwk()
+
+# which looks something like this:
+pubkey_jwk = """{
+  "use": "sig",
+  "kid": "23b5973e-7257-4fbc-944b-3f79e01da799",
+  "kty": "EC",
+  "alg": "ES384",
+  "key_ops": [
+    "verify"
+  ],
+  "crv": "P-384",
+  "x": "xcICJQvPvomxkue8ZOE9AsKSSlGwYhEOBpscwdpiFK4jzkh2zGvaq1Ek5wY1BkxU",
+  "y": "Q6VVuYPTlVvZLZYTbtOoxfNUD3kqJs4ZEqQ6mt5cxfOHCc0mGqrGGcnhAZ95YKZ0"
+}"""
+
+# can verify, but cannot sign
+verifier = JWS.from_jwk(json.loads(pubkey_jwk))
+
+```
+
+### JWE Key Wrapping and Encryption
+
+Most JWE Algorithm involve using a private key to directly encrypt, or to wrap
+a newly created CEK (Content Encryption Key)
+
+#### JWE private AES keys for direct ``dir`` encryption:
+
+```python
+from webcrypt.jwe import JWE
+import json
+
+# generate a new 192-bit key used directly in content Encryption
+jwk1 = JWE(algorithm=JWE.Algorithm.DIR, encryption=JWE.Encryption.A192GCM)
+
+# generate a new 256-bit key used directly in content Encryption + HMAC Authentication
+jwk2 = JWE(algorithm=JWE.Algorithm.DIR, encryption=JWE.Encryption.A128CBC_HS256)
+
+# export jwk1:
+print(json.dumps(jwk1.to_jwk(),indent=4))
+
+# will look like this:
+privkey = """{
+    "use": "enc",
+    "kid": "be29da9a-3a89-4839-a664-68de669f145a",
+    "kty": "oct",
+    "alg": "dir",
+    "enc": "A128GCM",
+    "key_ops": [
+        "encrypt",
+        "decrypt"
+    ],
+    "k": "L35wm0tFTg12nKcZviyv1Q"
 }
+"""
+
+jwk_reloaded = JWE.from_jwk(json.loads(privkey))
+
+data = b'Some byte data to be encrypted then decrypted'
+
+token = jwk_reloaded.encrypt(data,compress=True) # option to compress the data
+
+data_decrypted = jwk_reloaded.decrypt(token)
+
+assert data_decrypted == data
+
+```
+
+
+#### JWE Key-wrapping Algorithms:
+
+```python
+from webcrypt.jwe import JWE
+import json
+
+# Generate a 192-bit private key to wrap a 256-bit CEK for encrypting and decrypting data
+jwk1 = JWE(algorithm=JWE.Algorithm.A192KW, encryption=JWE.Encryption.A256GCM)
+
+# Generate a 256-bit private key to encrypt and wrap a 512-bit key for Encryption + Authentication
+jwk2 = JWE(algorithm=JWE.Algorithm.A256GCMKW, encryption=JWE.Encryption.A256CBC_HS512)
+
+# Generate a 128-bit private key to wrap a 192-bit CEK for encrypting and decrypting data
+jwk3 = JWE(algorithm=JWE.Algorithm.A128KW, encryption=JWE.Encryption.A192GCM)
+
+print(json.dumps(jwk2.to_jwk(),indent=4))
+
+# will produce something like this:
+
+jwk_json = """{
+    "use": "enc",
+    "kid": "f47a54c3-85d8-46b8-a9cb-8a1b5f47eddb",
+    "kty": "oct",
+    "alg": "A256GCMKW",
+    "enc": "A256CBC-HS512",
+    "key_ops": [
+        "wrapKey",
+        "unwrapKey"
+    ],
+    "k": "dkcM5Fnj7oYN4r4NGs7RMVxSX1jcT9gwvoRgxXJ4um8"
+}
+
+"""
+
+# which can later be reloaded for encryption / decryption operations
+jwe_key = JWE.from_jwk(json.loads(jwk_json))
+```
+
+
+#### JWE RSA Key-wrapping Algorithms
+
+```python
+from webcrypt.jwe import JWE
+
+# Examples of all RSA Algorithms, with different CEK sizes
+
+jwe1 = JWE(algorithm=JWE.Algorithm.RSA_OAEP_256, encryption=JWE.Encryption.A192GCM)
+jwe2 = JWE(algorithm=JWE.Algorithm.RSA_OAEP, encryption=JWE.Encryption.A128CBC_HS256)
+jwe3 = JWE(algorithm=JWE.Algorithm.RSA1_5, encryption=JWE.Encryption.A256GCM)
+
+
+# Load a Public JWE key from the JWK of a private one
+pub_jwe = JWE.from_jwk(jwe1.public_jwk())
+
+data = b'Byte data to be encrypted and decrypted'
+
+# encrypt data, and wrap the CEK
+token = pub_jwe.encrypt(data)
+
+# Raises an Error, a public key cannot decrypt the CEK!
+pub_jwe.decrypt(token)
+
+# only the corresponding private key can unwrap the CEK and decrypt the data
+data_decrypted = jwe1.decrypt(token)
+
+assert data_decrypted == data
+```
+
+
+#### JWE PBE (Passphrase based Encryption) Algorithms
+
+```python
+from webcrypt.jwe import JWE
+import json
+
+# Generate a 192-bit private key to wrap a 384-bit key for Authentication + Encryption
+jwk = JWE(algorithm=JWE.Algorithm.PBES2_HS384_A192KW,
+          encryption=JWE.Encryption.A256GCM,
+          key="I love python")
+
+data = b'Some secret data'
+
+token = jwk.encrypt(data)
+
+print(json.dumps(JWE.decode_header(token), indent=4))
 
+# the Token header will look something like this, including the alg, enc and
+# the PBE salt and iteration count (p2s and p2c)
+header="""{
+    "alg": "PBES2-HS384+A192KW",
+    "enc": "A256GCM",
+    "kid": "08842033-5f83-477b-9be3-c91ab6e7635c",
+    "p2s": "7jByuyCgOWc4aEfkoAJ0VQ",
+    "p2c": 1644
+}"""
+```
 
-setup(**setup_kwargs)
```

