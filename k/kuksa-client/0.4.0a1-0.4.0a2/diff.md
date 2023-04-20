# Comparing `tmp/kuksa_client-0.4.0a1.tar.gz` & `tmp/kuksa_client-0.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuksa_client-0.4.0a1.tar", last modified: Wed Apr 12 10:05:48 2023, max compression
+gzip compressed data, was "kuksa_client-0.4.0a2.tar", last modified: Thu Apr 20 06:55:42 2023, max compression
```

## Comparing `kuksa_client-0.4.0a1.tar` & `kuksa_client-0.4.0a2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.005578 kuksa_client-0.4.0a1/
--rw-r--r--   0 erik      (1000) erik      (1000)    11357 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)       35 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/MANIFEST.in
--rw-r--r--   0 erik      (1000) erik      (1000)     9640 2023-04-12 10:05:48.005578 kuksa_client-0.4.0a1/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)     8758 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/README.md
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:47.997582 kuksa_client-0.4.0a1/kuksa/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:47.997582 kuksa_client-0.4.0a1/kuksa/val/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa/val/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:47.997582 kuksa_client-0.4.0a1/kuksa/val/v1/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa/val/v1/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     9374 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa/val/v1/types_pb2.py
--rw-r--r--   0 erik      (1000) erik      (1000)      159 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa/val/v1/types_pb2_grpc.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3751 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa/val/v1/val_pb2.py
--rw-r--r--   0 erik      (1000) erik      (1000)     8731 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa/val/v1/val_pb2_grpc.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.001580 kuksa_client-0.4.0a1/kuksa_certificates/
--rw-r--r--   0 erik      (1000) erik      (1000)     1675 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a1/kuksa_certificates/CA.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1342 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/CA.pem
--rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a1/kuksa_certificates/Client.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1334 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/Client.pem
--rw-r--r--   0 erik      (1000) erik      (1000)     2267 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a1/kuksa_certificates/Server.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1334 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/Server.pem
--rw-r--r--   0 erik      (1000) erik      (1000)      114 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/__init__.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)     1398 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/genCerts.sh
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.001580 kuksa_client-0.4.0a1/kuksa_certificates/jwt/
--rw-r--r--   0 erik      (1000) erik      (1000)      151 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/all-read-write.json
--rw-r--r--   0 erik      (1000) erik      (1000)      875 2022-11-01 08:41:15.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/all-read-write.json.token
--rwxr-xr-x   0 erik      (1000) erik      (1000)     1430 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/createToken.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3243 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/jwt.key
--rw-r--r--   0 erik      (1000) erik      (1000)      800 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/jwt.key.pub
--rwxr-xr-x   0 erik      (1000) erik      (1000)      901 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/recreateJWTkeyPair.sh
--rw-r--r--   0 erik      (1000) erik      (1000)       34 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/requirements.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      167 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/single-read.json
--rw-r--r--   0 erik      (1000) erik      (1000)      895 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/single-read.json.token
--rw-r--r--   0 erik      (1000) erik      (1000)      175 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/super-admin.json
--rw-r--r--   0 erik      (1000) erik      (1000)      899 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/super-admin.json.token
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.001580 kuksa_client-0.4.0a1/kuksa_client/
--rw-r--r--   0 erik      (1000) erik      (1000)     3680 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/__init__.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)    22102 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/__main__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1708 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/_metadata.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.005578 kuksa_client-0.4.0a1/kuksa_client/cli_backend/
--rw-r--r--   0 erik      (1000) erik      (1000)     2114 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/cli_backend/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     9739 2023-04-12 07:56:08.000000 kuksa_client-0.4.0a1/kuksa_client/cli_backend/grpc.py
--rw-r--r--   0 erik      (1000) erik      (1000)     9070 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/cli_backend/ws.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.005578 kuksa_client-0.4.0a1/kuksa_client/grpc/
--rw-r--r--   0 erik      (1000) erik      (1000)    36389 2023-04-12 07:56:08.000000 kuksa_client-0.4.0a1/kuksa_client/grpc/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)    15204 2023-04-12 07:56:08.000000 kuksa_client-0.4.0a1/kuksa_client/grpc/aio.py
--rw-r--r--   0 erik      (1000) erik      (1000)      385 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/logging.ini
--rw-r--r--   0 erik      (1000) erik      (1000)      605 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/logo
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.005578 kuksa_client-0.4.0a1/kuksa_client/ws/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/ws/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.001580 kuksa_client-0.4.0a1/kuksa_client.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)     9640 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa_client.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)     1542 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa_client.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa_client.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       60 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa_client.egg-info/entry_points.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      227 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa_client.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       44 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa_client.egg-info/top_level.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      625 2023-04-12 10:04:35.000000 kuksa_client-0.4.0a1/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)     1388 2023-04-12 10:05:48.005578 kuksa_client-0.4.0a1/setup.cfg
--rw-r--r--   0 erik      (1000) erik      (1000)     1168 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/setup.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.005578 kuksa_client-0.4.0a1/tests/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/tests/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2545 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/tests/conftest.py
--rw-r--r--   0 erik      (1000) erik      (1000)    63303 2023-04-12 07:56:08.000000 kuksa_client-0.4.0a1/tests/test_grpc.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.514595 kuksa_client-0.4.0a2/
+-rw-r--r--   0 erik      (1000) erik      (1000)    11357 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)       35 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/MANIFEST.in
+-rw-r--r--   0 erik      (1000) erik      (1000)     9640 2023-04-20 06:55:42.514595 kuksa_client-0.4.0a2/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     8758 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/README.md
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.498603 kuksa_client-0.4.0a2/kuksa/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.498603 kuksa_client-0.4.0a2/kuksa/val/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa/val/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.498603 kuksa_client-0.4.0a2/kuksa/val/v1/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa/val/v1/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     9374 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa/val/v1/types_pb2.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      159 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa/val/v1/types_pb2_grpc.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3751 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa/val/v1/val_pb2.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     8731 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa/val/v1/val_pb2_grpc.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.502601 kuksa_client-0.4.0a2/kuksa_certificates/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1675 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a2/kuksa_certificates/CA.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1342 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_certificates/CA.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a2/kuksa_certificates/Client.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1371 2023-04-19 12:14:28.000000 kuksa_client-0.4.0a2/kuksa_certificates/Client.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)     2267 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_certificates/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a2/kuksa_certificates/Server.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1371 2023-04-19 12:14:28.000000 kuksa_client-0.4.0a2/kuksa_certificates/Server.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)      114 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_certificates/__init__.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     1443 2023-04-19 12:14:28.000000 kuksa_client-0.4.0a2/kuksa_certificates/genCerts.sh
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.502601 kuksa_client-0.4.0a2/kuksa_certificates/jwt/
+-rw-r--r--   0 erik      (1000) erik      (1000)      151 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/all-read-write.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      875 2022-11-01 08:41:15.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/all-read-write.json.token
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     1430 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/createToken.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3243 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/jwt.key
+-rw-r--r--   0 erik      (1000) erik      (1000)      800 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/jwt.key.pub
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      901 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/recreateJWTkeyPair.sh
+-rw-r--r--   0 erik      (1000) erik      (1000)       34 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/requirements.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      167 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/single-read.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      895 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/single-read.json.token
+-rw-r--r--   0 erik      (1000) erik      (1000)      175 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/super-admin.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      899 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/super-admin.json.token
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.502601 kuksa_client-0.4.0a2/kuksa_client/
+-rw-r--r--   0 erik      (1000) erik      (1000)     3929 2023-04-20 06:51:14.000000 kuksa_client-0.4.0a2/kuksa_client/__init__.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)    23519 2023-04-19 12:14:28.000000 kuksa_client-0.4.0a2/kuksa_client/__main__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1708 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_client/_metadata.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.514595 kuksa_client-0.4.0a2/kuksa_client/cli_backend/
+-rw-r--r--   0 erik      (1000) erik      (1000)     2189 2023-04-19 12:14:28.000000 kuksa_client-0.4.0a2/kuksa_client/cli_backend/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    11064 2023-04-20 06:51:14.000000 kuksa_client-0.4.0a2/kuksa_client/cli_backend/grpc.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     9397 2023-04-19 12:14:28.000000 kuksa_client-0.4.0a2/kuksa_client/cli_backend/ws.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.514595 kuksa_client-0.4.0a2/kuksa_client/grpc/
+-rw-r--r--   0 erik      (1000) erik      (1000)    37360 2023-04-20 06:51:14.000000 kuksa_client-0.4.0a2/kuksa_client/grpc/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    16144 2023-04-20 06:51:14.000000 kuksa_client-0.4.0a2/kuksa_client/grpc/aio.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      385 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_client/logging.ini
+-rw-r--r--   0 erik      (1000) erik      (1000)      605 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_client/logo
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.514595 kuksa_client-0.4.0a2/kuksa_client/ws/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_client/ws/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.514595 kuksa_client-0.4.0a2/kuksa_client.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)     9640 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa_client.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     1542 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       60 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa_client.egg-info/entry_points.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      227 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa_client.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       44 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa_client.egg-info/top_level.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      625 2023-04-12 10:04:35.000000 kuksa_client-0.4.0a2/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)     1388 2023-04-20 06:55:42.518593 kuksa_client-0.4.0a2/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)     1168 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/setup.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.514595 kuksa_client-0.4.0a2/tests/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/tests/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2545 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/tests/conftest.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    63303 2023-04-12 07:56:08.000000 kuksa_client-0.4.0a2/tests/test_grpc.py
```

### Comparing `kuksa_client-0.4.0a1/LICENSE` & `kuksa_client-0.4.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/PKG-INFO` & `kuksa_client-0.4.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuksa_client
-Version: 0.4.0a1
+Version: 0.4.0a2
 Summary: kuksa.val python clients and SDK
 Home-page: https://github.com/eclipse/kuksa.val
 Author: Sebastian Schildt, Naresh Nayak, Wenwen Chen
 Author-email: sebastian.schildt@de.bosch.com, naresh.nayak@de.bosch.com, wenwen.chen@de.bosch.com
 Project-URL: Source, https://github.com/eclipse/kuksa.val/tree/master/kuksa-client
 Project-URL: Bug Tracker, https://github.com/eclipse/kuksa.val/issues
 Classifier: Intended Audience :: Developers
```

### Comparing `kuksa_client-0.4.0a1/README.md` & `kuksa_client-0.4.0a2/README.md`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa/val/v1/types_pb2.py` & `kuksa_client-0.4.0a2/kuksa/val/v1/types_pb2.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa/val/v1/val_pb2.py` & `kuksa_client-0.4.0a2/kuksa/val/v1/val_pb2.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa/val/v1/val_pb2_grpc.py` & `kuksa_client-0.4.0a2/kuksa/val/v1/val_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_certificates/CA.key` & `kuksa_client-0.4.0a2/kuksa_certificates/CA.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_certificates/CA.pem` & `kuksa_client-0.4.0a2/kuksa_certificates/CA.pem`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_certificates/Client.key` & `kuksa_client-0.4.0a2/kuksa_certificates/Client.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_certificates/README.md` & `kuksa_client-0.4.0a2/kuksa_certificates/README.md`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_certificates/Server.key` & `kuksa_client-0.4.0a2/kuksa_certificates/Server.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_certificates/genCerts.sh` & `kuksa_client-0.4.0a2/kuksa_certificates/genCerts.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/bin/sh
+#!/bin/bash
 
 
 genCAKey() {
     openssl genrsa -out CA.key 2048
 }
 
 
@@ -13,15 +13,15 @@
 
 genKey() {
     openssl genrsa -out $1.key 2048
 }
 
 genCert() {
     openssl req -new -key $1.key -out $1.csr -passin pass:"temp" -subj "/C=CA/ST=Ontario/L=Ottawa/O=Eclipse.org Foundation, Inc./CN=$1/emailAddress=kuksa-dev@eclipse.org"
-    openssl x509 -req -in $1.csr -CA CA.pem -CAkey CA.key -CAcreateserial -days 365 -out $1.pem
+    openssl x509 -req -in $1.csr -extfile <(printf "subjectAltName=DNS:$1") -CA CA.pem -CAkey CA.key -CAcreateserial -days 365 -out $1.pem
     openssl verify -CAfile CA.pem $1.pem
 }
 
 set -e
 # Check if the CA is available, else make CA certificates
 if [ -f "CA.key" ]; then
     echo "Existing CA.key will be used"
```

### Comparing `kuksa_client-0.4.0a1/kuksa_certificates/jwt/all-read-write.json.token` & `kuksa_client-0.4.0a2/kuksa_certificates/jwt/all-read-write.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_certificates/jwt/createToken.py` & `kuksa_client-0.4.0a2/kuksa_certificates/jwt/createToken.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_certificates/jwt/jwt.key` & `kuksa_client-0.4.0a2/kuksa_certificates/jwt/jwt.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_certificates/jwt/jwt.key.pub` & `kuksa_client-0.4.0a2/kuksa_certificates/jwt/jwt.key.pub`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_certificates/jwt/recreateJWTkeyPair.sh` & `kuksa_client-0.4.0a2/kuksa_certificates/jwt/recreateJWTkeyPair.sh`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_certificates/jwt/single-read.json.token` & `kuksa_client-0.4.0a2/kuksa_certificates/jwt/single-read.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_certificates/jwt/super-admin.json.token` & `kuksa_client-0.4.0a2/kuksa_certificates/jwt/super-admin.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_client/__init__.py` & `kuksa_client-0.4.0a2/kuksa_client/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from typing import Iterable
 import uuid
 
 from kuksa_client._metadata import *
 
 from . import cli_backend
 
+
 class KuksaClientThread(threading.Thread):
 
     # Constructor
     def __init__(self, config):
         super().__init__()
 
         self.backend = cli_backend.Backend.from_config(config)
@@ -47,58 +48,64 @@
     def checkConnection(self):
         return self.backend.checkConnection()
 
     def stop(self):
         self.backend.stop()
 
     # Do authorization by passing a jwt token or a token file
-    def authorize(self, token=None, timeout=5):
-        return self.backend.authorize(token, timeout)
+    def authorize(self, token_or_tokenfile: str=None, timeout=5):
+        return self.backend.authorize(token_or_tokenfile, timeout)
 
     # Update VSS Tree Entry
-    def updateVSSTree(self, jsonStr, timeout=5):
+    def updateVSSTree(self, jsonStr: str, timeout=5):
         return self.backend.updateVSSTree(jsonStr, timeout)
 
     # Update Meta Data of a given path
-    def updateMetaData(self, path, jsonStr, timeout=5):
+    def updateMetaData(self, path: str, jsonStr: str, timeout=5):
         return self.backend.updateMetaData(path, jsonStr, timeout)
 
     # Get Meta Data of a given path
-    def getMetaData(self, path, timeout=5):
+    def getMetaData(self, path: str, timeout=5):
         return self.backend.getMetaData(path, timeout)
 
     # Set value to a given path
-    def setValue(self, path, value, attribute="value", timeout=5):
+    def setValue(self, path: str, value, attribute="value", timeout=5):
         return self.backend.setValue(path, value, attribute, timeout)
 
     # Set value of every given path
     def setValues(self, updates: Dict[str, Any], attribute="value", timeout=5):
         return self.backend.setValues(updates, attribute, timeout)
 
     # Get value to a given path
-    def getValue(self, path, attribute="value", timeout=5):
+    def getValue(self, path: str, attribute="value", timeout=5):
         return self.backend.getValue(path, attribute, timeout)
 
     # Get value of every given path
     def getValues(self, paths: Iterable[str], attribute="value", timeout=5):
         return self.backend.getValues(paths, attribute, timeout)
 
     # Subscribe value changes of to a given path.
     # The given callback function will be called then, if the given path is updated:
     #   updateMessage = await webSocket.recv()
     #   callback(updateMessage)
-    def subscribe(self, path, callback, attribute = "value", timeout=5):
+    def subscribe(self, path: str, callback, attribute="value", timeout=5):
         return self.backend.subscribe(path, callback, attribute, timeout)
 
-    def subscribeMultiple(self, paths, callback, attribute = "value", timeout=5):
+    def subscribeMultiple(self, paths: Iterable[str], callback, attribute="value", timeout=5):
         return self.backend.subscribeMultiple(paths, callback, attribute, timeout)
 
     # Unsubscribe value changes of to a given path.
     # The subscription id from the response of the corresponding subscription request will be required
-    def unsubscribe(self, sub_id, timeout=5):
+    def unsubscribe(self, sub_id: int, timeout=5):
         return self.backend.unsubscribe(sub_id, timeout)
 
+    def disconnect(self, timeout=5):
+        return self.backend.disconnect(timeout)
+
+    def connect(self, timeout=5):
+        return self.backend.connect(timeout)
+
     # Thread function: Start the asyncio loop
     def run(self):
         self.loop = asyncio.new_event_loop()
         asyncio.set_event_loop(self.loop)
         self.loop.run_until_complete(self.backend.mainLoop())
```

### Comparing `kuksa_client-0.4.0a1/kuksa_client/__main__.py` & `kuksa_client-0.4.0a2/kuksa_client/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from kuksa_client import _metadata
 
 DEFAULT_SERVER_ADDR = "127.0.0.1"
 DEFAULT_SERVER_PORT = 8090
 DEFAULT_SERVER_PROTOCOL = "ws"
 SUPPORTED_SERVER_PROTOCOLS = ("ws", "grpc")
 
-scriptDir= os.path.dirname(os.path.realpath(__file__))
+scriptDir = os.path.dirname(os.path.realpath(__file__))
 
 
 def assignment_statement(arg):
     path, value = arg.split('=', maxsplit=1)
     return (path, value)
 
 
@@ -70,15 +70,15 @@
                 childVssTree = childVssTree[path]
             elif 'children' in childVssTree and path in childVssTree['children']:
                 childVssTree = childVssTree['children'][path]
             else:
                 # This else-branch is reached when one of the path components is invalid
                 # In that case stop parsing further and return an empty tree
                 # Autocompletion can't help here.
-                childVssTree={}
+                childVssTree = {}
                 break
 
         if 'children' in childVssTree:
             childVssTree = childVssTree['children']
         return childVssTree
 
     def path_completer(self, text, line, begidx, endidx):
@@ -89,39 +89,41 @@
 
             if 'metadata' in tree:
                 self.vssTree = tree['metadata']
 
         self.pathCompletionItems = []
         childTree = self.get_childtree(text)
         prefix = ""
-        seperator="/"
+        seperator = "/"
 
         if "/" in text:
             prefix = text[:text.rfind("/")]+"/"
-        elif  "." in text:
+        elif "." in text:
             prefix = text[:text.rfind(".")]+"."
-            seperator="."
+            seperator = "."
 
         for key in childTree:
             child = childTree[key]
             if isinstance(child, dict):
                 description = ""
                 nodetype = "unknown"
 
                 if 'description' in child:
                     description = child['description']
 
                 if 'type' in child:
-                    nodetype=child['type'].capitalize()
+                    nodetype = child['type'].capitalize()
 
-                self.pathCompletionItems.append(CompletionItem(prefix + key, nodetype+": "+ description))
+                self.pathCompletionItems.append(CompletionItem(
+                    prefix + key, nodetype+": " + description))
 
                 if 'children' in child:
                     self.pathCompletionItems.append(
-                        CompletionItem(prefix + key+seperator, "Children of branch "+prefix+key),
+                        CompletionItem(prefix + key+seperator,
+                                       "Children of branch "+prefix+key),
                     )
 
         return basic_complete(text, line, begidx, endidx, self.pathCompletionItems)
 
     def subscribeCallback(self, logPath, resp):
         with logPath.open('a', encoding='utf-8') as logFile:
             logFile.write(resp + "\n")
@@ -134,250 +136,295 @@
 
     COMM_SETUP_COMMANDS = "Communication Set-up Commands"
     VSS_COMMANDS = "Kuksa Interaction Commands"
     INFO_COMMANDS = "Info Commands"
 
     ap_getServerAddr = argparse.ArgumentParser()
     ap_connect = argparse.ArgumentParser()
-    ap_connect.add_argument('-i', "--insecure", default=False, action="store_true", help='Connect in insecure mode')
+    ap_connect.add_argument(
+        '-i', "--insecure", default=False, action="store_true", help='Connect in insecure mode')
     ap_disconnect = argparse.ArgumentParser()
     ap_authorize = argparse.ArgumentParser()
     tokenfile_completer_method = functools.partial(Cmd.path_complete,
-        path_filter=lambda path: (os.path.isdir(path) or path.endswith(".token")))
+                                                   path_filter=lambda path: (os.path.isdir(path) or path.endswith(".token")))
     ap_authorize.add_argument(
-        'Token',
+        'token_or_tokenfile',
         help='JWT(or the file storing the token) for authorizing the client.',
-        completer_method=tokenfile_completer_method,
-    )
+        completer_method=tokenfile_completer_method,)
     ap_setServerAddr = argparse.ArgumentParser()
-    ap_setServerAddr.add_argument('IP', help='VISS/gRPC Server IP Address', default=DEFAULT_SERVER_ADDR)
-    ap_setServerAddr.add_argument('Port', type=int, help='VISS/gRPC Server Port', default=DEFAULT_SERVER_PORT)
+    ap_setServerAddr.add_argument(
+        'IP', help='VISS/gRPC Server IP Address', default=DEFAULT_SERVER_ADDR)
+    ap_setServerAddr.add_argument(
+        'Port', type=int, help='VISS/gRPC Server Port', default=DEFAULT_SERVER_PORT)
     ap_setServerAddr.add_argument(
         '-p',
         "--protocol",
         help='VISS/gRPC Server Communication Protocol (ws or grpc)',
         default=DEFAULT_SERVER_PROTOCOL,
     )
 
     ap_setValue = argparse.ArgumentParser()
-    ap_setValue.add_argument("Path", help="Path to be set", completer_method=path_completer)
+    ap_setValue.add_argument(
+        "Path", help="Path to be set", completer_method=path_completer)
     ap_setValue.add_argument("Value", help="Value to be set")
-    ap_setValue.add_argument("-a", "--attribute", help="Attribute to be set", default="value")
+    ap_setValue.add_argument(
+        "-a", "--attribute", help="Attribute to be set", default="value")
 
     ap_setValues = argparse.ArgumentParser()
     ap_setValues.add_argument(
         "Path=Value",
         help="Path and new value this path is to be set with",
         nargs='+',
         type=assignment_statement,
     )
-    ap_setValues.add_argument("-a", "--attribute", help="Attribute to be set", default="value")
+    ap_setValues.add_argument(
+        "-a", "--attribute", help="Attribute to be set", default="value")
 
     ap_getValue = argparse.ArgumentParser()
-    ap_getValue.add_argument("Path", help="Path to be read", completer_method=path_completer)
-    ap_getValue.add_argument("-a", "--attribute", help="Attribute to be get", default="value")
+    ap_getValue.add_argument(
+        "Path", help="Path to be read", completer_method=path_completer)
+    ap_getValue.add_argument(
+        "-a", "--attribute", help="Attribute to be get", default="value")
 
     ap_getValues = argparse.ArgumentParser()
-    ap_getValues.add_argument("Path", help="Path whose value is to be read", nargs='+', completer_method=path_completer)
-    ap_getValues.add_argument("-a", "--attribute", help="Attribute to be get", default="value")
+    ap_getValues.add_argument(
+        "Path", help="Path whose value is to be read", nargs='+', completer_method=path_completer)
+    ap_getValues.add_argument(
+        "-a", "--attribute", help="Attribute to be get", default="value")
 
     ap_setTargetValue = argparse.ArgumentParser()
-    ap_setTargetValue.add_argument("Path", help="Path whose target value to be set", completer_method=path_completer)
+    ap_setTargetValue.add_argument(
+        "Path", help="Path whose target value to be set", completer_method=path_completer)
     ap_setTargetValue.add_argument("Value", help="Value to be set")
 
     ap_setTargetValues = argparse.ArgumentParser()
     ap_setTargetValues.add_argument(
         "Path=Value",
         help="Path and new target value this path is to be set with",
         nargs='+',
         type=assignment_statement,
     )
 
     ap_getTargetValue = argparse.ArgumentParser()
-    ap_getTargetValue.add_argument("Path", help="Path whose target value is to be read", completer_method=path_completer)
+    ap_getTargetValue.add_argument(
+        "Path", help="Path whose target value is to be read", completer_method=path_completer)
 
     ap_getTargetValues = argparse.ArgumentParser()
-    ap_getTargetValues.add_argument("Path", help="Path whose target value is to be read", nargs='+', completer_method=path_completer)
+    ap_getTargetValues.add_argument(
+        "Path", help="Path whose target value is to be read", nargs='+', completer_method=path_completer)
 
     ap_subscribe = argparse.ArgumentParser()
-    ap_subscribe.add_argument("Path", help="Path to subscribe to", completer_method=path_completer)
-    ap_subscribe.add_argument("-a", "--attribute", help="Attribute to subscribe to", default="value")
+    ap_subscribe.add_argument(
+        "Path", help="Path to subscribe to", completer_method=path_completer)
+    ap_subscribe.add_argument(
+        "-a", "--attribute", help="Attribute to subscribe to", default="value")
 
     ap_subscribeMultiple = argparse.ArgumentParser()
-    ap_subscribeMultiple.add_argument("Path", help="Path to subscribe to", nargs='+', completer_method=path_completer)
-    ap_subscribeMultiple.add_argument("-a", "--attribute", help="Attribute to subscribe to", default="value")
+    ap_subscribeMultiple.add_argument(
+        "Path", help="Path to subscribe to", nargs='+', completer_method=path_completer)
+    ap_subscribeMultiple.add_argument(
+        "-a", "--attribute", help="Attribute to subscribe to", default="value")
 
     ap_unsubscribe = argparse.ArgumentParser()
     ap_unsubscribe.add_argument(
         "SubscribeId", help="Corresponding subscription Id", completer_method=subscriptionIdCompleter,
     )
 
     ap_getMetaData = argparse.ArgumentParser()
-    ap_getMetaData.add_argument("Path", help="Path whose metadata is to be read", completer_method=path_completer)
+    ap_getMetaData.add_argument(
+        "Path", help="Path whose metadata is to be read", completer_method=path_completer)
     ap_updateMetaData = argparse.ArgumentParser()
-    ap_updateMetaData.add_argument("Path", help="Path whose MetaData is to update", completer_method=path_completer)
+    ap_updateMetaData.add_argument(
+        "Path", help="Path whose MetaData is to update", completer_method=path_completer)
     ap_updateMetaData.add_argument(
         "Json",
         help="MetaData to update. Note, only attributes can be update, if update children or the whole vss tree, use"
         " `updateVSSTree` instead.",
     )
 
     ap_updateVSSTree = argparse.ArgumentParser()
     jsonfile_completer_method = functools.partial(Cmd.path_complete,
-        path_filter=lambda path: (os.path.isdir(path) or path.endswith(".json")))
-    ap_updateVSSTree.add_argument("Json", help="Json tree to update VSS", completer_method=jsonfile_completer_method)
+                                                  path_filter=lambda path: (os.path.isdir(path) or path.endswith(".json")))
+    ap_updateVSSTree.add_argument(
+        "Json", help="Json tree to update VSS", completer_method=jsonfile_completer_method)
 
     # Constructor
-    def __init__(self, server_ip=None, server_port=None, server_protocol=None, insecure=False):
+    def __init__(self, server_ip=None, server_port=None, server_protocol=None, insecure=False, token_or_tokenfile=None):
         super().__init__(
             persistent_history_file=".vssclient_history", persistent_history_length=100, allow_cli_args=False,
         )
 
         self.prompt = "Test Client> "
         self.max_completion_items = 20
         self.serverIP = server_ip or DEFAULT_SERVER_ADDR
         self.serverPort = server_port or DEFAULT_SERVER_PORT
         self.serverProtocol = server_protocol or DEFAULT_SERVER_PROTOCOL
         self.supportedProtocols = SUPPORTED_SERVER_PROTOCOLS
         self.vssTree = {}
         self.pathCompletionItems = []
         self.subscribeIds = set()
         self.commThread = None
+        self.token_or_tokenfile = token_or_tokenfile
+        self.insecure = insecure
 
         print("Welcome to Kuksa Client version " + str(_metadata.__version__))
         print()
         with (pathlib.Path(scriptDir) / 'logo').open('r', encoding='utf-8') as f:
             print(f.read())
         print("Default tokens directory: " + self.getDefaultTokenDir())
 
         print()
-        self.connect(insecure)
+        self.connect()
 
     @with_category(COMM_SETUP_COMMANDS)
     @with_argparser(ap_authorize)
     def do_authorize(self, args):
         """Authorize the client to interact with the server"""
+        if args.token_or_tokenfile is not None:
+            self.token_or_tokenfile = args.token_or_tokenfile
         if self.checkConnection():
-            resp = self.commThread.authorize(args.Token)
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+            resp = self.commThread.authorize(self.token_or_tokenfile)
+            print(highlight(resp, lexers.JsonLexer(),
+                    formatters.TerminalFormatter()))
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_setValue)
     def do_setValue(self, args):
         """Set the value of a path"""
         if self.checkConnection():
-            resp = self.commThread.setValue(args.Path, args.Value, args.attribute)
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+            resp = self.commThread.setValue(
+                args.Path, args.Value, args.attribute)
+            print(highlight(resp, lexers.JsonLexer(),
+                  formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_setValues)
     def do_setValues(self, args):
         """Set the value of given paths"""
         if self.checkConnection():
-            resp = self.commThread.setValues(dict(getattr(args, 'Path=Value')), args.attribute)
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+            resp = self.commThread.setValues(
+                dict(getattr(args, 'Path=Value')), args.attribute)
+            print(highlight(resp, lexers.JsonLexer(),
+                  formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_setTargetValue)
     def do_setTargetValue(self, args):
         """Set the target value of a path"""
         if self.checkConnection():
-            resp = self.commThread.setValue(args.Path, args.Value, "targetValue")
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+            resp = self.commThread.setValue(
+                args.Path, args.Value, "targetValue")
+            print(highlight(resp, lexers.JsonLexer(),
+                  formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_setTargetValues)
     def do_setTargetValues(self, args):
         """Set the target value of given paths"""
         if self.checkConnection():
-            resp = self.commThread.setValues(dict(getattr(args, 'Path=Value')), "targetValue")
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+            resp = self.commThread.setValues(
+                dict(getattr(args, 'Path=Value')), "targetValue")
+            print(highlight(resp, lexers.JsonLexer(),
+                  formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_getValue)
     def do_getValue(self, args):
         """Get the value of a path"""
         if self.checkConnection():
             resp = self.commThread.getValue(args.Path, args.attribute)
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+            print(highlight(resp, lexers.JsonLexer(),
+                  formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_getValues)
     def do_getValues(self, args):
         """Get the value of given paths"""
         if self.checkConnection():
             resp = self.commThread.getValues(args.Path, args.attribute)
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+            print(highlight(resp, lexers.JsonLexer(),
+                  formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_getTargetValue)
     def do_getTargetValue(self, args):
         """Get the value of a path"""
         if self.checkConnection():
             resp = self.commThread.getValue(args.Path, "targetValue")
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+            print(highlight(resp, lexers.JsonLexer(),
+                  formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_getTargetValues)
     def do_getTargetValues(self, args):
         """Get the value of given paths"""
         if self.checkConnection():
             resp = self.commThread.getValues(args.Path, "targetValue")
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+            print(highlight(resp, lexers.JsonLexer(),
+                  formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_subscribe)
     def do_subscribe(self, args):
         """Subscribe the value of a path"""
         if self.checkConnection():
 
-            logPath = pathlib.Path.cwd() / f"log_{args.Path.replace('/', '.')}_{args.attribute}_{str(time.time())}"
+            logPath = pathlib.Path.cwd() / \
+                f"log_{args.Path.replace('/', '.')}_{args.attribute}_{str(time.time())}"
             callback = functools.partial(self.subscribeCallback, logPath)
-            resp = self.commThread.subscribe(args.Path, callback, args.attribute)
-            resJson =  json.loads(resp)
+            resp = self.commThread.subscribe(
+                args.Path, callback, args.attribute)
+            resJson = json.loads(resp)
             if "subscriptionId" in resJson:
                 self.subscribeIds.add(resJson["subscriptionId"])
                 logPath.touch()
                 print(f"Subscription log available at {logPath}")
-                print(f"Execute tail -f {logPath} on another Terminal instance")
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+                print(
+                    f"Execute tail -f {logPath} on another Terminal instance")
+            print(highlight(resp, lexers.JsonLexer(),
+                  formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_subscribeMultiple)
     def do_subscribeMultiple(self, args):
         """Subscribe to updates of given paths"""
         if self.checkConnection():
-            logPath = pathlib.Path.cwd() / f"subscribeMultiple_{args.attribute}_{str(time.time())}.log"
+            logPath = pathlib.Path.cwd() / \
+                f"subscribeMultiple_{args.attribute}_{str(time.time())}.log"
             callback = functools.partial(self.subscribeCallback, logPath)
-            resp = self.commThread.subscribeMultiple(args.Path, callback, args.attribute)
-            resJson =  json.loads(resp)
+            resp = self.commThread.subscribeMultiple(
+                args.Path, callback, args.attribute)
+            resJson = json.loads(resp)
             if "subscriptionId" in resJson:
                 self.subscribeIds.add(resJson["subscriptionId"])
                 logPath.touch()
                 print(f"Subscription log available at {logPath}")
-                print(f"Execute tail -f {logPath} on another Terminal instance")
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+                print(
+                    f"Execute tail -f {logPath} on another Terminal instance")
+            print(highlight(resp, lexers.JsonLexer(),
+                  formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_unsubscribe)
     def do_unsubscribe(self, args):
         """Unsubscribe an existing subscription"""
         if self.checkConnection():
             resp = self.commThread.unsubscribe(args.SubscribeId)
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+            print(highlight(resp, lexers.JsonLexer(),
+                  formatters.TerminalFormatter()))
             self.subscribeIds.discard(args.SubscribeId)
             self.pathCompletionItems = []
 
     def stop(self):
         if self.commThread is not None:
             self.commThread.stop()
             self.commThread.join()
@@ -389,107 +436,114 @@
         return "{}"
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_updateVSSTree)
     def do_updateVSSTree(self, args):
         """Update VSS Tree Entry"""
         if self.checkConnection():
-            resp =  self.commThread.updateVSSTree(args.Json)
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+            resp = self.commThread.updateVSSTree(args.Json)
+            print(highlight(resp, lexers.JsonLexer(),
+                  formatters.TerminalFormatter()))
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_updateMetaData)
     def do_updateMetaData(self, args):
         """Update MetaData of a given path"""
         if self.checkConnection():
-            resp =  self.commThread.updateMetaData(args.Path, args.Json)
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+            resp = self.commThread.updateMetaData(args.Path, args.Json)
+            print(highlight(resp, lexers.JsonLexer(),
+                  formatters.TerminalFormatter()))
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_getMetaData)
     def do_getMetaData(self, args):
         """Get MetaData of the path"""
         resp = self.getMetaData(args.Path)
         print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
-
     @with_category(COMM_SETUP_COMMANDS)
     @with_argparser(ap_disconnect)
     def do_disconnect(self, _args):
         """Disconnect from the VISS/gRPC Server"""
         if hasattr(self, "commThread"):
             if self.commThread is not None:
                 self.commThread.stop()
                 self.commThread = None
 
     def checkConnection(self):
         if self.commThread is None or not self.commThread.checkConnection():
             self.connect()
         return self.commThread.checkConnection()
 
-    def connect(self, insecure=False):
+    def connect(self):
         """Connect to the VISS/gRPC Server"""
         if hasattr(self, "commThread"):
             if self.commThread is not None:
                 self.commThread.stop()
                 self.commThread = None
-        config = {'ip':self.serverIP,
-        'port': self.serverPort,
-        'insecure' : insecure,
-        'protocol': self.serverProtocol
-        }
+        config = {'ip': self.serverIP,
+                  'port': self.serverPort,
+                  'insecure': self.insecure,
+                  'protocol': self.serverProtocol,
+                  'token_or_tokenfile': self.token_or_tokenfile,
+                  }
         self.commThread = KuksaClientThread(config)
         self.commThread.start()
 
         waitForConnection = threading.Condition()
         waitForConnection.acquire()
         waitForConnection.wait_for(self.commThread.checkConnection, timeout=1)
         waitForConnection.release()
 
         if self.commThread.checkConnection():
             pass
         else:
-            print("Error: Websocket could not be connected or the gRPC channel could not be created.")
+            print(
+                "Error: Websocket could not be connected or the gRPC channel could not be created.")
             self.commThread.stop()
             self.commThread = None
 
     @with_category(COMM_SETUP_COMMANDS)
     @with_argparser(ap_connect)
     def do_connect(self, args):
-        self.connect(args.insecure)
+        self.insecure = args.insecure
+        self.connect()
 
     @with_category(COMM_SETUP_COMMANDS)
     @with_argparser(ap_setServerAddr)
     def do_setServerAddress(self, args):
         """Sets the IP Address for the VISS/gRPC Server"""
         try:
             self.serverIP = args.IP
             self.serverPort = args.Port
             if args.protocol not in self.supportedProtocols:
                 raise ValueError
             self.serverProtocol = args.protocol
-            print("Setting Server Address to " + args.IP + ":" + str(args.Port) + " with protocol " + args.protocol)
+            print("Setting Server Address to " + args.IP + ":" +
+                  str(args.Port) + " with protocol " + args.protocol)
         except ValueError:
-            print("Error: Please give a valid server Address/Protocol. Only ws and grpc are supported.")
+            print(
+                "Error: Please give a valid server Address/Protocol. Only ws and grpc are supported.")
 
     @with_category(COMM_SETUP_COMMANDS)
     @with_argparser(ap_getServerAddr)
     def do_getServerAddress(self, _args):
         """Gets the IP Address for the VISS/gRPC Server"""
         if hasattr(self, "serverIP") and hasattr(self, "serverPort"):
             print(self.serverIP + ":" + str(self.serverPort))
         else:
             print("Server IP not set!!")
 
     def getDefaultTokenDir(self):
         try:
             return os.path.join(kuksa_certificates.__certificate_dir__, "jwt")
         except AttributeError:
-            guessTokenDir = os.path.join(scriptDir, "../kuksa_certificates/jwt")
+            guessTokenDir = os.path.join(
+                scriptDir, "../kuksa_certificates/jwt")
             if os.path.isdir(guessTokenDir):
                 return guessTokenDir
             return "Unknown"
 
     @with_category(INFO_COMMANDS)
     def do_info(self, _args):
         """Show summary info of the client"""
@@ -508,33 +562,43 @@
     def do_printTokenDir(self, _args):
         """Show default token directory"""
         print(self.getDefaultTokenDir())
 # pylint: enable=too-many-public-methods
 # pylint: enable=too-many-instance-attributes
 
 # Main Function
+
+
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument('--ip', help="VISS/gRPC Server IP Address", default=DEFAULT_SERVER_ADDR)
-    parser.add_argument('--port', type=int, help="VISS/gRPC Server Port", default=DEFAULT_SERVER_PORT)
+    parser.add_argument(
+        '--ip', help="VISS/gRPC Server IP Address", default=DEFAULT_SERVER_ADDR)
+    parser.add_argument(
+        '--port', type=int, help="VISS/gRPC Server Port", default=DEFAULT_SERVER_PORT)
     parser.add_argument(
         '--protocol',
         help="VISS/gRPC Server Communication Protocol",
         choices=SUPPORTED_SERVER_PROTOCOLS,
         default=DEFAULT_SERVER_PROTOCOL,
     )
-    parser.add_argument('--insecure', default=False, action='store_true', help='Connect in insecure mode')
+    parser.add_argument('--insecure', default=False,
+                        action='store_true', help='Connect in insecure mode')
     parser.add_argument(
         '--logging-config', default=os.path.join(scriptDir, 'logging.ini'), help="Path to logging configuration file",
     )
+    parser.add_argument(
+        '--token_or_tokenfile', default=None, help="JWT token or path to a JWT token file (.token)",
+    )
     args = parser.parse_args()
 
     logging.config.fileConfig(args.logging_config)
-    clientApp = TestClient(args.ip, args.port, args.protocol, args.insecure)
+    clientApp = TestClient(args.ip, args.port, args.protocol,
+                           args.insecure, args.token_or_tokenfile)
     try:
         # We exit the loop when the user types "quit" or hits Ctrl-D.
         clientApp.cmdloop()
     finally:
         clientApp.stop()
 
-if __name__=="__main__":
+
+if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `kuksa_client-0.4.0a1/kuksa_client/_metadata.py` & `kuksa_client-0.4.0a2/kuksa_client/_metadata.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_client/cli_backend/__init__.py` & `kuksa_client-0.4.0a2/kuksa_client/cli_backend/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,27 +16,32 @@
 # SPDX-License-Identifier: Apache-2.0
 ########################################################################
 
 import pathlib
 
 import kuksa_certificates
 
+
 class Backend:
     def __init__(self, config):
         self.serverIP = config.get('ip', "127.0.0.1")
         self.serverPort = config.get('port', 8090)
         try:
             self.insecure = config.getboolean('insecure', False)
         except AttributeError:
             self.insecure = config.get('insecure', False)
         self.default_cert_path = pathlib.Path(kuksa_certificates.__path__[0])
-        self.cacertificate = config.get('cacertificate', str(self.default_cert_path / 'CA.pem'))
-        self.certificate = config.get('certificate', str(self.default_cert_path / 'Client.pem'))
-        self.keyfile = config.get('key', str(self.default_cert_path / 'Client.key'))
-        self.tokenfile = config.get('token', str(self.default_cert_path / 'jwt/all-read-write.json.token'))
+        self.cacertificate = config.get(
+            'cacertificate', str(self.default_cert_path / 'CA.pem'))
+        self.certificate = config.get('certificate', str(
+            self.default_cert_path / 'Client.pem'))
+        self.keyfile = config.get('key', str(
+            self.default_cert_path / 'Client.key'))
+        self.token_or_tokenfile = config.get('token_or_tokenfile', str(
+            self.default_cert_path / 'jwt/all-read-write.json.token'))
 
     @staticmethod
     def from_config(config):
         protocol = config.get('protocol', 'ws')
 
         # pylint: disable=cyclic-import,import-outside-toplevel
         if protocol == 'ws':
```

### Comparing `kuksa_client-0.4.0a1/kuksa_client/cli_backend/grpc.py` & `kuksa_client-0.4.0a2/kuksa_client/cli_backend/grpc.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import pathlib
 import queue
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterable
 import uuid
+import os
 
 from kuksa_client import cli_backend
 import kuksa_client.grpc
 import kuksa_client.grpc.aio
 from kuksa_client.grpc import EntryUpdate
 
 
@@ -41,14 +42,23 @@
 
 class Backend(cli_backend.Backend):
     def __init__(self, config):
         super().__init__(config)
         self.cacertificate = pathlib.Path(self.cacertificate)
         self.keyfile = pathlib.Path(self.keyfile)
         self.certificate = pathlib.Path(self.certificate)
+        if self.token_or_tokenfile is not None:
+            if os.path.isfile(self.token_or_tokenfile):
+                self.token_or_tokenfile = pathlib.Path(self.token_or_tokenfile)
+                self.token = self.token_or_tokenfile.expanduser(
+                ).read_text(encoding='utf-8').rstrip('\n')
+            else:
+                self.token = str(self.token_or_tokenfile)
+        else:
+            self.token = ""
         self.grpcConnected = False
 
         self.sendMsgQueue = queue.Queue()
         self.run = False
 
         self.AttrDict = {
             "value": (kuksa_client.grpc.Field.VALUE, kuksa_client.grpc.View.CURRENT_VALUE),
@@ -60,40 +70,41 @@
     def checkConnection(self):
         if self.grpcConnected:
             return True
         return False
 
     # Function to stop the communication
     def stop(self):
+        self.disconnect()
         self.run = False
         print("gRPC channel disconnected.")
 
     # Function to implement fetching of metadata
-    def getMetaData(self, path, timeout=5):
+    def getMetaData(self, path: str, timeout=5):
         return self.getValue(path, "metadata", timeout)
 
-    def updateMetaData(self, path, jsonStr, timeout=5):
+    def updateMetaData(self, path: str, jsonStr, timeout=5):
         return self.setValue(path, jsonStr, "metadata", timeout)
 
     # Function to implement get
-    def getValue(self, path, attribute="value", timeout=5):
+    def getValue(self, path: str, attribute="value", timeout=5):
         return self.getValues((path,), attribute, timeout)
 
-    def getValues(self, paths, attribute="value", timeout=5):
+    def getValues(self, paths: Iterable[str], attribute="value", timeout=5):
         if attribute in self.AttrDict:
             field, view = self.AttrDict[attribute]
             entries = [kuksa_client.grpc.EntryRequest(
                 path=path, view=view, fields=(field,)) for path in paths]
             requestArgs = {'entries': entries}
             return self._sendReceiveMsg(("get", requestArgs), timeout)
 
         return json.dumps({"error": "Invalid Attribute"})
 
     # Function to implement set
-    def setValue(self, path, value, attribute="value", timeout=5):
+    def setValue(self, path: str, value, attribute="value", timeout=5):
         return self.setValues({path: value}, attribute, timeout)
 
     def setValues(self, updates: Dict[str, Any], attribute="value", timeout=5):
         if attribute in self.AttrDict:
             field, _ = self.AttrDict[attribute]
             entry_updates = []
             for path, value in updates.items():
@@ -117,51 +128,64 @@
                 entry_updates.append(kuksa_client.grpc.EntryUpdate(
                     entry=entry, fields=(field,)))
             requestArgs = {'updates': entry_updates}
             return self._sendReceiveMsg(("set", requestArgs), timeout)
         return json.dumps({"error": "Invalid Attribute"})
 
     # Function for authorization
-    def authorize(self, tokenfile=None, timeout=5):
-        if tokenfile is None:
-            tokenfile = self.tokenfile
-        tokenfile = pathlib.Path(tokenfile)
+    def authorize(self, token_or_tokenfile:str =None, timeout=5):
+        if token_or_tokenfile is None:
+            token_or_tokenfile = self.token_or_tokenfile
+        if os.path.isfile(token_or_tokenfile):
+            token_or_tokenfile = pathlib.Path(token_or_tokenfile)
+            token = token_or_tokenfile.expanduser().read_text(encoding='utf-8').rstrip('\n')
+        else:
+            token = token_or_tokenfile
         requestArgs = {
-            'token': tokenfile.expanduser().read_text(encoding='utf-8').rstrip('\n')}
+            'token': token
+        }
 
         return self._sendReceiveMsg(("authorize", requestArgs), timeout)
 
     # Subscribe value changes of to a given path.
     # The given callback function will be called then, if the given path is updated.
-    def subscribe(self, path, callback, attribute="value", timeout=5):
+    def subscribe(self, path: str, callback, attribute="value", timeout=5):
         return self.subscribeMultiple((path,), callback, attribute, timeout)
 
-    def subscribeMultiple(self, paths, callback, attribute="value", timeout=5):
+    def subscribeMultiple(self, paths: Iterable[str], callback, attribute="value", timeout=5):
         if attribute in self.AttrDict:
             field, view = self.AttrDict[attribute]
             entries = [kuksa_client.grpc.SubscribeEntry(
                 path=path, view=view, fields=(field,)) for path in paths]
             requestArgs = {
                 'entries': entries,
                 'callback': callback_wrapper(callback),
             }
             return self._sendReceiveMsg(("subscribe", requestArgs), timeout)
 
         return json.dumps({"error": "Invalid Attribute"})
 
     # Unsubscribe value changes of to a given path.
     # The subscription id from the response of the corresponding subscription request will be required
-    def unsubscribe(self, sub_id, timeout=5):
+    def unsubscribe(self, sub_id: int, timeout=5):
         try:
             sub_id = uuid.UUID(sub_id)
         except ValueError as exc:
             return json.dumps({"error": str(exc)})
         requestArgs = {'subscription_id': sub_id}
         return self._sendReceiveMsg(("unsubscribe", requestArgs), timeout)
 
+    def connect(self, timeout=5):
+        requestArgs = {}
+        return self._sendReceiveMsg(("connect", requestArgs), timeout)
+
+    def disconnect(self, timeout=5):
+        requestArgs = {}
+        return self._sendReceiveMsg(("disconnect", requestArgs), timeout)
+
     def _sendReceiveMsg(self, req, timeout):
         (call, requestArgs) = req
         recvQueue = queue.Queue(maxsize=1)
         self.sendMsgQueue.put((call, requestArgs, recvQueue))
         try:
             resp, error = recvQueue.get(timeout=timeout)
             if error:
@@ -171,42 +195,47 @@
             else:
                 respJson = "OK"
         except queue.Empty:
             respJson = json.dumps({"error": "Timeout"})
         return respJson
 
     # Async function to handle the gRPC calls
-    async def _grpcHandler(self, vss_client):
+    async def _grpcHandler(self, vss_client: kuksa_client.grpc.aio.VSSClient):
         self.grpcConnected = True
         self.run = True
         subscriber_manager = kuksa_client.grpc.aio.SubscriberManager(
             vss_client)
         while self.run:
             try:
                 (call, requestArgs, responseQueue) = self.sendMsgQueue.get_nowait()
             except queue.Empty:
                 await asyncio.sleep(0.01)
                 continue
             try:
                 if call == "get":
                     resp = await vss_client.get(**requestArgs)
-                    resp = [entry.to_dict() for entry in resp]
-                    resp = resp[0] if len(resp) == 1 else resp
+                    if resp is not None:
+                        resp = [entry.to_dict() for entry in resp]
+                        resp = resp[0] if len(resp) == 1 else resp
                 elif call == "set":
                     resp = await vss_client.set(**requestArgs)
                 elif call == "authorize":
                     resp = await vss_client.authorize(str(requestArgs["token"]))
                 elif call == "subscribe":
                     callback = requestArgs.pop('callback')
                     subscriber_response_stream = vss_client.subscribe(
                         **requestArgs)
                     resp = await subscriber_manager.add_subscriber(subscriber_response_stream, callback)
                     resp = {"subscriptionId": str(resp)}
                 elif call == "unsubscribe":
                     resp = await subscriber_manager.remove_subscriber(**requestArgs)
+                elif call == "connect":
+                    resp = await vss_client.connect()
+                elif call == "disconnect":
+                    resp = await vss_client.disconnect()
                 else:
                     raise Exception("Not Implemented.")
 
                 responseQueue.put((resp, None))
             except kuksa_client.grpc.VSSClientError as exc:
                 responseQueue.put((None, exc.to_dict()))
             except ValueError as exc:
@@ -214,20 +243,22 @@
                     (None, {"error": "ValueError in casting the value."}))
 
         self.grpcConnected = False
 
     # Main loop for handling gRPC communication
     async def mainLoop(self):
         if self.insecure:
-            async with kuksa_client.grpc.aio.VSSClient(self.serverIP, self.serverPort) as vss_client:
+
+            async with kuksa_client.grpc.aio.VSSClient(self.serverIP, self.serverPort, token=self.token) as vss_client:
                 print("gRPC channel connected.")
                 await self._grpcHandler(vss_client)
         else:
             async with kuksa_client.grpc.aio.VSSClient(
                 self.serverIP,
                 self.serverPort,
                 root_certificates=self.cacertificate,
                 private_key=self.keyfile,
                 certificate_chain=self.certificate,
+                token=self.token
             ) as vss_client:
                 print("Secure gRPC channel connected.")
                 await self._grpcHandler(vss_client)
```

### Comparing `kuksa_client-0.4.0a1/kuksa_client/cli_backend/ws.py` & `kuksa_client-0.4.0a2/kuksa_client/cli_backend/ws.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import time
 import uuid
 
 import websockets
 
 from kuksa_client import cli_backend
 
+
 class Backend(cli_backend.Backend):
     def __init__(self, config):
         super().__init__(config)
         self.wsConnected = False
 
         self.subscriptionCallbacks = {}
         self.sendMsgQueue = queue.Queue()
@@ -49,15 +50,16 @@
                 try:
                     self.recvMsgQueues[resJson["requestId"]].put(message)
                 finally:
                     del self.recvMsgQueues[resJson["requestId"]]
             else:
                 if "subscriptionId" in resJson and resJson["subscriptionId"] in self.subscriptionCallbacks:
                     try:
-                        self.subscriptionCallbacks[resJson["subscriptionId"]](message)
+                        self.subscriptionCallbacks[resJson["subscriptionId"]](
+                            message)
                     except Exception as e:  # pylint: disable=broad-except
                         print(e)
 
     async def _sender_handler(self, webSocket):
         while self.run:
             try:
                 req = self.sendMsgQueue.get_nowait()
@@ -95,72 +97,77 @@
                 sent = True
             except queue.Full:
                 time.sleep(0.01)
 
         # Wait on the receive queue
         try:
             res = recvQueue.get(timeout=timeout)
-            resJson =  json.loads(res)
+            resJson = json.loads(res)
             if "requestId" in res and str(req["requestId"]) == str(resJson["requestId"]):
                 return json.dumps(resJson, indent=2)
         except queue.Empty:
-            req["error"] =  "timeout"
+            req["error"] = "timeout"
             return json.dumps(req, indent=2)
 
     # Function to stop the communication
     def stop(self):
         self.wsConnected = False
         self.run = False
         print("Server disconnected.")
 
-    # Function to authorize against the kuksa.val server
-    def authorize(self, tokenfile=None, timeout=2):
-        if tokenfile is None:
-            tokenfile = self.tokenfile
-        tokenfile = pathlib.Path(tokenfile)
-        token = tokenfile.expanduser().read_text(encoding='utf-8')
+    def disconnect(self):
+        self.stop()
 
+    # Function to authorize against the kuksa.val server
+    def authorize(self, token_or_tokenfile=None, timeout=2):
+        if token_or_tokenfile is None:
+            token_or_tokenfile = self.token_or_tokenfile
+        if os.path.isfile(token_or_tokenfile):
+            token_or_tokenfile = pathlib.Path(token_or_tokenfile)
+            token = token_or_tokenfile.expanduser().read_text(encoding='utf-8')
+        else:
+            token = token_or_tokenfile
         req = {}
-        req["action"]= "authorize"
+        req["action"] = "authorize"
         req["tokens"] = token
         return self._sendReceiveMsg(req, timeout)
 
     # Update VSS Tree Entry
     def updateVSSTree(self, jsonStr, timeout=5):
         req = {}
-        req["action"]= "updateVSSTree"
+        req["action"] = "updateVSSTree"
         if os.path.isfile(jsonStr):
             with open(jsonStr, "r", encoding="utf-8") as f:
                 req["metadata"] = json.load(f)
         else:
             req["metadata"] = json.loads(jsonStr)
         return self._sendReceiveMsg(req, timeout)
 
    # Update Meta Data of a given path
     def updateMetaData(self, path, jsonStr, timeout=5):
         req = {}
-        req["action"]= "updateMetaData"
+        req["action"] = "updateMetaData"
         req["path"] = path
         req["metadata"] = json.loads(jsonStr)
         return self._sendReceiveMsg(req, timeout)
 
     # Get Meta Data of a given path
     def getMetaData(self, path, timeout=5):
         """Get MetaData of the parameter"""
         req = {}
-        req["action"]= "getMetaData"
+        req["action"] = "getMetaData"
         req["path"] = path
         return self._sendReceiveMsg(req, timeout)
 
     # Set value to a given path
     def setValue(self, path, value, attribute="value", timeout=5):
         if 'nan' == value:
             return json.dumps({"error": path + " has an invalid value " + str(value)}, indent=2)
         req = {}
-        req["action"]= "set"
+        req["action"] = "set"
         req["path"] = path
         req["attribute"] = attribute
         try:
             jsonValue = json.loads(value)
             if isinstance(jsonValue, list):
                 req[attribute] = []
                 for v in jsonValue:
@@ -182,28 +189,28 @@
 
     # Subscribe value changes of to a given path.
     # The given callback function will be called then, if the given path is updated:
     #   updateMessage = await webSocket.recv()
     #   callback(updateMessage)
     def subscribe(self, path, callback, attribute="value", timeout=5):
         req = {}
-        req["action"]= "subscribe"
+        req["action"] = "subscribe"
         req["path"] = path
         req["attribute"] = attribute
         res = self._sendReceiveMsg(req, timeout)
-        resJson =  json.loads(res)
+        resJson = json.loads(res)
         if "subscriptionId" in resJson:
             self.subscriptionCallbacks[resJson["subscriptionId"]] = callback
         return res
 
     # Unsubscribe value changes of to a given path.
     # The subscription id from the response of the corresponding subscription request will be required
     def unsubscribe(self, subId, timeout=5):
         req = {}
-        req["action"]= "unsubscribe"
+        req["action"] = "unsubscribe"
         req["subscriptionId"] = subId
 
         res = {}
         # Check if the subscription subId exists
         if subId in self.subscriptionCallbacks:
             # No matter what happens, remove the callback
             del self.subscriptionCallbacks[subId]
@@ -218,19 +225,19 @@
 
         return res
 
     # Function to check connection
     def checkConnection(self):
         return self.wsConnected
 
-    # Main loop for handling websocket communication
-    async def mainLoop(self):
+    async def connect(self):
         if not self.insecure:
             context = ssl.create_default_context()
-            context.load_cert_chain(certfile=self.certificate, keyfile=self.keyfile)
+            context.load_cert_chain(
+                certfile=self.certificate, keyfile=self.keyfile)
             context.load_verify_locations(cafile=self.cacertificate)
             # Certificates in ../kuksa_certificates does not contain the IP address used for
             # connection to server so hostname check must be disabled
             context.check_hostname = False
             try:
                 print("connect to wss://"+self.serverIP+":"+str(self.serverPort))
                 async with websockets.connect("wss://"+self.serverIP+":"+str(self.serverPort), ssl=context) as ws:
@@ -242,7 +249,11 @@
             try:
                 print("connect to ws://"+self.serverIP+":"+str(self.serverPort))
                 async with websockets.connect("ws://"+self.serverIP+":"+str(self.serverPort)) as ws:
                     print("Websocket connected.")
                     await self._msgHandler(ws)
             except OSError as e:
                 print("Disconnected!! " + str(e))
+
+    # Main loop for handling websocket communication
+    async def mainLoop(self):
+        await self.connect()
```

### Comparing `kuksa_client-0.4.0a1/kuksa_client/grpc/__init__.py` & `kuksa_client-0.4.0a2/kuksa_client/grpc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -474,23 +474,24 @@
         self,
         host: str,
         port: int,
         token: str = None,
         root_certificates: Optional[Path] = None,
         private_key: Optional[Path] = None,
         certificate_chain: Optional[Path] = None,
-        *,
         ensure_startup_connection: bool = True,
+        connected: bool = False,
     ):
         self.authorization_header = self.get_authorization_header(token)
         self.target_host = f'{host}:{port}'
         self.root_certificates = root_certificates
         self.private_key = private_key
         self.certificate_chain = certificate_chain
         self.ensure_startup_connection = ensure_startup_connection
+        self.connected = connected
         self.client_stub = None
 
     def _load_creds(self) -> Optional[grpc.ChannelCredentials]:
         if all((self.root_certificates, self.private_key, self.certificate_chain)):
             root_certificates = self.root_certificates.read_bytes()
             private_key = self.private_key.read_bytes()
             certificate_chain = self.certificate_chain.read_bytes()
@@ -566,16 +567,16 @@
         else:
             error = {}
         if response.errors:
             errors = [json_format.MessageToDict(
                 err, preserving_proto_field_name=True) for err in response.errors]
         else:
             errors = []
-        if (error and error['code'] != http.HTTPStatus.OK) or any(
-            sub_error['error']['code'] != http.HTTPStatus.OK for sub_error in errors
+        if (error and error['code'] is not http.HTTPStatus.OK) or any(
+            sub_error['error']['code'] is not http.HTTPStatus.OK for sub_error in errors
         ):
             raise VSSClientError(error, errors)
 
     def get_authorization_header(self, token: str):
         if token is None:
             return None
         return "Bearer " + token
@@ -595,36 +596,48 @@
 class VSSClient(BaseVSSClient):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.channel = None
         self.exit_stack = contextlib.ExitStack()
 
     def __enter__(self):
+        self.connect()
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.disconnect()
+
+    def check_connected(func):
+        def wrapper(self, *args, **kwargs):
+            if self.connected:
+                return func(self, *args, **kwargs)
+            else:
+                logger.info(
+                    "Disconnected from server! Try connect.")
+        return wrapper
+
+    def connect(self, target_host=None):
         creds = self._load_creds()
+        if target_host is None:
+            target_host = self.target_host
         if creds is not None:
-            channel = grpc.secure_channel(self.target_host, creds)
+            channel = grpc.secure_channel(target_host, creds)
         else:
-            channel = grpc.insecure_channel(self.target_host)
+            channel = grpc.insecure_channel(target_host)
         self.channel = self.exit_stack.enter_context(channel)
         self.client_stub = val_pb2_grpc.VALStub(self.channel)
-        if self.authorization_header is None:
-            logger.debug(
-                "Can not ensure startup connection without token to authorize")
+        self.connected = True
         if self.ensure_startup_connection:
-            try:
-                info = self.get_server_info()
-                logger.debug("Connected to server: %s", info)
-            except:
-                logger.debug("Connection could not be ensured")
-        return self
+            logger.debug("Connected to server: %s", self.get_server_info())
 
-    def __exit__(self, exc_type, exc_value, traceback):
+    def disconnect(self):
         self.exit_stack.close()
         self.client_stub = None
         self.channel = None
+        self.connected = False
 
     def get_current_values(self, paths: Iterable[str], **rpc_kwargs) -> Dict[str, Datapoint]:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         Example:
@@ -778,30 +791,32 @@
         for updates in self.subscribe(
             entries=(SubscribeEntry(path, View.METADATA, (Field(field.value),))
                      for path in paths),
             **rpc_kwargs,
         ):
             yield {update.entry.path: update.entry.metadata for update in updates}
 
-    def get(self, *, entries: Iterable[EntryRequest], **rpc_kwargs) -> List[DataEntry]:
+    @check_connected
+    def get(self, entries: Iterable[EntryRequest], **rpc_kwargs) -> List[DataEntry]:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
         rpc_kwargs["metadata"] = self.generate_metadata_header(
             rpc_kwargs.get("metadata"))
         req = self._prepare_get_request(entries)
         try:
             resp = self.client_stub.Get(req, **rpc_kwargs)
         except RpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
         return self._process_get_response(resp)
 
-    def set(self, *, updates: Collection[EntryUpdate], **rpc_kwargs) -> None:
+    @check_connected
+    def set(self, updates: Collection[EntryUpdate], **rpc_kwargs) -> None:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
         rpc_kwargs["metadata"] = self.generate_metadata_header(
             rpc_kwargs.get("metadata"))
@@ -814,60 +829,78 @@
         req = self._prepare_set_request(updates, paths_with_required_type)
         try:
             resp = self.client_stub.Set(req, **rpc_kwargs)
         except RpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
         self._process_set_response(resp)
 
-    def subscribe(self, *, entries: Iterable[SubscribeEntry], **rpc_kwargs) -> Iterator[List[EntryUpdate]]:
+    # needs to be handled differently
+    def subscribe(self, entries: Iterable[SubscribeEntry], **rpc_kwargs) -> Iterator[List[EntryUpdate]]:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
-        rpc_kwargs["metadata"] = self.generate_metadata_header(
-            rpc_kwargs.get("metadata"))
-        req = self._prepare_subscribe_request(entries)
-        resp_stream = self.client_stub.Subscribe(req, **rpc_kwargs)
-        try:
-            for resp in resp_stream:
-                logger.debug("%s: %s", type(resp).__name__, resp)
-                yield [EntryUpdate.from_message(update) for update in resp.updates]
-        except RpcError as exc:
-            raise VSSClientError.from_grpc_error(exc) from exc
 
-    def authorize(self, *, token: str, **rpc_kwargs) -> str:
+        if self.connected:
+            rpc_kwargs["metadata"] = self.generate_metadata_header(
+                rpc_kwargs.get("metadata"))
+            req = self._prepare_subscribe_request(entries)
+            resp_stream = self.client_stub.Subscribe(req, **rpc_kwargs)
+            try:
+                for resp in resp_stream:
+                    logger.debug("%s: %s", type(resp).__name__, resp)
+                    yield [EntryUpdate.from_message(update) for update in resp.updates]
+            except RpcError as exc:
+                raise VSSClientError.from_grpc_error(exc) from exc
+        else:
+            logger.info("Disconnected from server! Try connect.")
+
+    @check_connected
+    def authorize(self, token: str, **rpc_kwargs) -> str:
+        """
+        Parameters:
+            rpc_kwargs
+                grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
+            token
+                string containing the actual token
+        """
         rpc_kwargs["metadata"] = self.generate_metadata_header(
             metadata=rpc_kwargs.get("metadata"), header=self.get_authorization_header(token))
         req = val_pb2.GetServerInfoRequest()
         try:
             resp = self.client_stub.GetServerInfo(req, **rpc_kwargs)
         except RpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
         logger.debug("%s: %s", type(resp).__name__, resp)
         self.authorization_header = self.get_authorization_header(token)
         return "Authenticated"
 
+    @check_connected
     def get_server_info(self, **rpc_kwargs) -> ServerInfo:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
         rpc_kwargs["metadata"] = self.generate_metadata_header(
             metadata=rpc_kwargs.get("metadata"))
         req = val_pb2.GetServerInfoRequest()
         logger.debug("%s: %s", type(req).__name__, req)
         try:
             resp = self.client_stub.GetServerInfo(req, **rpc_kwargs)
+            logger.debug("%s: %s", type(resp).__name__, resp)
+            return ServerInfo.from_message(resp)
         except RpcError as exc:
-            raise VSSClientError.from_grpc_error(exc) from exc
-        logger.debug("%s: %s", type(resp).__name__, resp)
-
-        return ServerInfo.from_message(resp)
+            if exc.code() == grpc.StatusCode.UNAUTHENTICATED:
+                logger.info("Unauthenticated channel started")
+            else:
+                raise VSSClientError.from_grpc_error(exc) from exc
+        return None
+        
 
     def get_value_types(self, paths: Collection[str], **rpc_kwargs) -> Dict[str, DataType]:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         req = self._prepare_get_request(entries)
```

### Comparing `kuksa_client-0.4.0a1/kuksa_client/grpc/aio.py` & `kuksa_client-0.4.0a2/kuksa_client/grpc/aio.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,36 +53,48 @@
 class VSSClient(BaseVSSClient):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.channel = None
         self.exit_stack = contextlib.AsyncExitStack()
 
     async def __aenter__(self):
+        await self.connect()
+        return self
+
+    async def __aexit__(self, exc_type, exc_value, traceback):
+        await self.disconnect()
+
+    async def connect(self, target_host=None):
         creds = self._load_creds()
+        if target_host is None:
+            target_host = self.target_host
         if creds is not None:
-            channel = grpc.aio.secure_channel(self.target_host, creds)
+            channel = grpc.aio.secure_channel(target_host, creds)
         else:
-            channel = grpc.aio.insecure_channel(self.target_host)
+            channel = grpc.aio.insecure_channel(target_host)
         self.channel = await self.exit_stack.enter_async_context(channel)
         self.client_stub = val_pb2_grpc.VALStub(self.channel)
-        if self.authorization_header is None:
-            logger.debug(
-                "Can not ensure startup connection without token to authorize")
+        self.connected = True
         if self.ensure_startup_connection:
-            try:
-                info = await self.get_server_info()
-                logger.debug("Connected to server: %s", info)
-            except:
-                logger.debug("Connection could not be ensured")
-        return self
+            logger.debug("Connected to server: %s", await self.get_server_info())
 
-    async def __aexit__(self, exc_type, exc_value, traceback):
+    async def disconnect(self):
         await self.exit_stack.aclose()
         self.client_stub = None
         self.channel = None
+        self.connected = False
+
+    def check_connected_async(func):
+        async def wrapper(self, *args, **kwargs):
+            if self.connected:
+                return await func(self, *args, **kwargs)
+            else:
+                logger.info(
+                    "Disconnected from server! Try cli command connect.")
+        return wrapper
 
     async def get_current_values(self, paths: Iterable[str], **rpc_kwargs) -> Dict[str, Datapoint]:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         Example:
@@ -240,30 +252,32 @@
         async for updates in self.subscribe(
             entries=(SubscribeEntry(path, View.METADATA, (Field(field.value),))
                      for path in paths),
             **rpc_kwargs,
         ):
             yield {update.entry.path: update.entry.metadata for update in updates}
 
-    async def get(self, *, entries: Iterable[EntryRequest], **rpc_kwargs) -> List[DataEntry]:
+    @check_connected_async
+    async def get(self, entries: Iterable[EntryRequest], **rpc_kwargs) -> List[DataEntry]:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
         rpc_kwargs["metadata"] = self.generate_metadata_header(
             rpc_kwargs.get("metadata"))
         req = self._prepare_get_request(entries)
         try:
             resp = await self.client_stub.Get(req, **rpc_kwargs)
         except AioRpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
         return self._process_get_response(resp)
 
-    async def set(self, *, updates: Collection[EntryUpdate], **rpc_kwargs) -> None:
+    @check_connected_async
+    async def set(self, updates: Collection[EntryUpdate], **rpc_kwargs) -> None:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
         rpc_kwargs["metadata"] = self.generate_metadata_header(
             rpc_kwargs.get("metadata"))
@@ -275,63 +289,78 @@
         req = self._prepare_set_request(updates, paths_with_required_type)
         try:
             resp = await self.client_stub.Set(req, **rpc_kwargs)
         except AioRpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
         self._process_set_response(resp)
 
-    async def subscribe(self, *,
+    async def subscribe(self,
                         entries: Iterable[SubscribeEntry],
                         **rpc_kwargs,
                         ) -> AsyncIterator[List[EntryUpdate]]:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
-        rpc_kwargs["metadata"] = self.generate_metadata_header(
-            rpc_kwargs.get("metadata"))
-        req = self._prepare_subscribe_request(entries)
-        resp_stream = self.client_stub.Subscribe(req, **rpc_kwargs)
-        try:
-            async for resp in resp_stream:
-                logger.debug("%s: %s", type(resp).__name__, resp)
-                yield [EntryUpdate.from_message(update) for update in resp.updates]
-        except AioRpcError as exc:
-            raise VSSClientError.from_grpc_error(exc) from exc
+        if self.connected:
+            rpc_kwargs["metadata"] = self.generate_metadata_header(
+                rpc_kwargs.get("metadata"))
+            req = self._prepare_subscribe_request(entries)
+            resp_stream = self.client_stub.Subscribe(req, **rpc_kwargs)
+            try:
+                async for resp in resp_stream:
+                    logger.debug("%s: %s", type(resp).__name__, resp)
+                    yield [EntryUpdate.from_message(update) for update in resp.updates]
+            except AioRpcError as exc:
+                raise VSSClientError.from_grpc_error(exc) from exc
+        else:
+            logger.info("Disconnected from server! Try connect.")
 
+    @check_connected_async
     async def authorize(self, token: str, **rpc_kwargs) -> str:
+        """
+        Parameters:
+            rpc_kwargs
+                grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
+            token
+                string containing the actual token
+        """
         rpc_kwargs["metadata"] = self.generate_metadata_header(
             metadata=rpc_kwargs.get("metadata"), header=self.get_authorization_header(token))
         req = val_pb2.GetServerInfoRequest()
         try:
             resp = await self.client_stub.GetServerInfo(req, **rpc_kwargs)
         except AioRpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
         logger.debug("%s: %s", type(resp).__name__, resp)
         self.authorization_header = self.get_authorization_header(token)
         return "Authenticated"
 
+    @check_connected_async
     async def get_server_info(self, **rpc_kwargs) -> ServerInfo:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
         rpc_kwargs["metadata"] = self.generate_metadata_header(
             metadata=rpc_kwargs.get("metadata"))
         req = val_pb2.GetServerInfoRequest()
         logger.debug("%s: %s", type(req).__name__, req)
         try:
             resp = await self.client_stub.GetServerInfo(req, **rpc_kwargs)
+            logger.debug("%s: %s", type(resp).__name__, resp)
+            return ServerInfo.from_message(resp)
         except AioRpcError as exc:
-            raise VSSClientError.from_grpc_error(exc) from exc
-        logger.debug("%s: %s", type(resp).__name__, resp)
-
-        return ServerInfo.from_message(resp)
+            if exc.code() == grpc.StatusCode.UNAUTHENTICATED:
+                logger.info("Unauthenticated channel started")
+            else: 
+                raise VSSClientError.from_grpc_error(exc) from exc
+        return None
 
     async def get_value_types(self, paths: Collection[str], **rpc_kwargs) -> Dict[str, DataType]:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
```

### Comparing `kuksa_client-0.4.0a1/kuksa_client/logo` & `kuksa_client-0.4.0a2/kuksa_client/logo`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/kuksa_client.egg-info/PKG-INFO` & `kuksa_client-0.4.0a2/kuksa_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuksa-client
-Version: 0.4.0a1
+Version: 0.4.0a2
 Summary: kuksa.val python clients and SDK
 Home-page: https://github.com/eclipse/kuksa.val
 Author: Sebastian Schildt, Naresh Nayak, Wenwen Chen
 Author-email: sebastian.schildt@de.bosch.com, naresh.nayak@de.bosch.com, wenwen.chen@de.bosch.com
 Project-URL: Source, https://github.com/eclipse/kuksa.val/tree/master/kuksa-client
 Project-URL: Bug Tracker, https://github.com/eclipse/kuksa.val/issues
 Classifier: Intended Audience :: Developers
```

### Comparing `kuksa_client-0.4.0a1/kuksa_client.egg-info/SOURCES.txt` & `kuksa_client-0.4.0a2/kuksa_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/pyproject.toml` & `kuksa_client-0.4.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/setup.cfg` & `kuksa_client-0.4.0a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/setup.py` & `kuksa_client-0.4.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/tests/conftest.py` & `kuksa_client-0.4.0a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a1/tests/test_grpc.py` & `kuksa_client-0.4.0a2/tests/test_grpc.py`

 * *Files identical despite different names*

