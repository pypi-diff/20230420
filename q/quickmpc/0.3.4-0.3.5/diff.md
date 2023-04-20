# Comparing `tmp/quickmpc-0.3.4.tar.gz` & `tmp/quickmpc-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-yd53resg/quickmpc-0.3.4.tar", last modified: Mon Apr 17 01:18:10 2023, max compression
+gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-7iswz950/quickmpc-0.3.5.tar", last modified: Thu Apr 20 06:51:19 2023, max compression
```

## Comparing `quickmpc-0.3.4.tar` & `quickmpc-0.3.5.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-17 01:17:45.000000 quickmpc-0.3.4/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-17 01:17:45.000000 quickmpc-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-17 01:17:45.000000 quickmpc-0.3.4/.isort.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-17 01:17:45.000000 quickmpc-0.3.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 01:17:45.000000 quickmpc-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-17 01:17:45.000000 quickmpc-0.3.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-17 01:18:10.000000 quickmpc-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-17 01:17:45.000000 quickmpc-0.3.4/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-04-17 01:17:45.000000 quickmpc-0.3.4/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-17 01:17:45.000000 quickmpc-0.3.4/README-ja.md
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-17 01:17:45.000000 quickmpc-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-17 01:17:45.000000 quickmpc-0.3.4/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 01:17:45.000000 quickmpc-0.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc/
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc/proto/common_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/common_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/common_types/common_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/common_types/common_types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18252 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/qmpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/share.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/utils/if_present.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/utils/make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/utils/overload_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/utils/parse_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/utils/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-17 01:18:10.000000 quickmpc-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 01:17:45.000000 quickmpc-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/tests/unit_tests/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/certificates/server1.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/certificates/server1.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/certificates/server2.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/certificates/server2.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/certificates/server3.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/certificates/server3.pem
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/local_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/tests/unit_tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/bitvector.csv
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/diff_col.csv
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/edge_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/empty.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/none.csv
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/not_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/over_number.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/string_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_over_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_share_recons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_share_sharize.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:19.000000 quickmpc-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-20 06:51:03.000000 quickmpc-0.3.5/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 06:51:03.000000 quickmpc-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-20 06:51:03.000000 quickmpc-0.3.5/.isort.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:19.000000 quickmpc-0.3.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-20 06:51:03.000000 quickmpc-0.3.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 06:51:03.000000 quickmpc-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-20 06:51:03.000000 quickmpc-0.3.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-20 06:51:19.000000 quickmpc-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-20 06:51:03.000000 quickmpc-0.3.5/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-04-20 06:51:03.000000 quickmpc-0.3.5/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-20 06:51:03.000000 quickmpc-0.3.5/README-ja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-20 06:51:03.000000 quickmpc-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-20 06:51:03.000000 quickmpc-0.3.5/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-20 06:51:03.000000 quickmpc-0.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:19.000000 quickmpc-0.3.5/quickmpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 06:51:19.000000 quickmpc-0.3.5/quickmpc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:19.000000 quickmpc-0.3.5/quickmpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/proto/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:19.000000 quickmpc-0.3.5/quickmpc/proto/common_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/proto/common_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/proto/common_types/common_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/proto/common_types/common_types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/proto/libc_to_manage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/proto/libc_to_manage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/proto/libc_to_manage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18252 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/qmpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/share.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:19.000000 quickmpc-0.3.5/quickmpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/utils/if_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/utils/make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/utils/overload_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/utils/parse_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/utils/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-20 06:51:03.000000 quickmpc-0.3.5/quickmpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:19.000000 quickmpc-0.3.5/quickmpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-20 06:51:19.000000 quickmpc-0.3.5/quickmpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-20 06:51:19.000000 quickmpc-0.3.5/quickmpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:51:19.000000 quickmpc-0.3.5/quickmpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 06:51:19.000000 quickmpc-0.3.5/quickmpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 06:51:19.000000 quickmpc-0.3.5/quickmpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 06:51:19.000000 quickmpc-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 06:51:03.000000 quickmpc-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:19.000000 quickmpc-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:19.000000 quickmpc-0.3.5/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:19.000000 quickmpc-0.3.5/tests/unit_tests/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/certificates/server1.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/certificates/server1.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/certificates/server2.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/certificates/server2.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/certificates/server3.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/certificates/server3.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/local_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:51:19.000000 quickmpc-0.3.5/tests/unit_tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_files/bitvector.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_files/diff_col.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_files/edge_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_files/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_files/none.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_files/normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_files/not_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_files/over_number.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_files/string_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_over_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_share_recons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tests/unit_tests/test_share_sharize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-20 06:51:03.000000 quickmpc-0.3.5/tox.ini
```

### Comparing `quickmpc-0.3.4/.vscode/settings.json` & `quickmpc-0.3.5/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/LICENSE` & `quickmpc-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/Pipfile.lock` & `quickmpc-0.3.5/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/README-ja.md` & `quickmpc-0.3.5/README-ja.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/README.md` & `quickmpc-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/mypy.ini` & `quickmpc-0.3.5/mypy.ini`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/quickmpc/README.md` & `quickmpc-0.3.5/quickmpc/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,29 @@
 # QuickMPC-libClient-pyが提供する機能
 
-## QMPC.parse_csv_file
-csvファイルからテーブルデータを読み込んでパースする．
+## QMPC.send_share_from_csv_file
+csvファイルからテーブルデータを読み込みShare化して送信する
 ### Parameters
 - file: `str`
 	- 読み込むファイル名
 
 ### Returns
-- parse_data: `Tuple[List[List[float]], List[str]]`
-	- parse_data[0]: schemaを除くテーブルデータ
-	- parse_data[1]: schema
+- res: `Dict`
+	- res["is_ok"]: `bool`
+		- 送信が成功したかどうか
+	- res["data_id"]: `str`
+		- テーブルデータのID
 
-## QMPC.parse_csv_data
-テーブルデータをパースする．
+## QMPC.send_share_from_csv_data
+テーブルデータをShare化して送信する
 ### Parameters
 - data: `List[List[str]]`
 	- パースするテーブルデータ
 
 ### Returns
-- parse_data: `Tuple[List[List[float]], List[str]]`
-	- parse_data[0]: schemaを除くテーブルデータ
-	- parse_data[1]: schema
-
-## QMPC.send_share
-エンジンにテーブルデータをShare化して送信する
-### Parameters
-- secrets: `List[List[str]]`
-	- 送信するテーブルデータ
-- schema: `List[str]`
-	- テーブルデータのschema
-- matching_column: `int`
-	- 結合する場合に用いる列
-- party_size: `int`
-	- エンジンのParty数
-- piece_size: `int`
-	- 分割データの最大サイズ
-### Returns
 - res: `Dict`
 	- res["is_ok"]: `bool`
 		- 送信が成功したかどうか
 	- res["data_id"]: `str`
 		- テーブルデータのID
 
 ## QMPC.delete_share
@@ -62,16 +46,16 @@
 	- 例えば(["d1", "d2"], [1], [1, 2])であれば，data_idがd1のテーブルデータとd2のテーブルデータをd1の1列目とd2の2列目をopenした値で突合させて横結合する
 - src: `List[int]`
 	- 平均値を計算する列リスト
 ### Returns
 - res: `Dict`
 	- res["is_ok"]: `bool`
 		- 送信が成功したかどうか
-	- res["job_id"]: `str`
-		- 計算スレッドのID
+	- res["job_uuid"]: `str`
+		- 計算スレッドのUUID
 
 ## QMPC.variance
 分散を計算する
 ### Parameters
 - join_order: `Tuple[List[str], List[int], List[int]]`
 	- join_order[0]: data_idのリスト
 	- join_order[1]: テーブルデータの結合方向(1:横(open)，2:縦(open)，3:横(share))
@@ -79,16 +63,16 @@
 	- 例えば(["d1", "d2"], [1], [1, 2])であれば，data_idがd1のテーブルデータとd2のテーブルデータをd1の1列目とd2の2列目をopenした値で突合させて横結合する
 - src: `List[int]`
 	- 分散を計算する列リスト
 ### Returns
 - res: `Dict`
 	- res["is_ok"]: `bool`
 		- 送信が成功したかどうか
-	- res["job_id"]: `str`
-		- 計算スレッドのID
+	- res["job_uuid"]: `str`
+		- 計算スレッドのUUID
 
 ## QMPC.sum
 総和を計算する
 ### Parameters
 - join_order: `Tuple[List[str], List[int], List[int]]`
 	- join_order[0]: data_idのリスト
 	- join_order[1]: テーブルデータの結合方向(1:横(open)，2:縦(open)，3:横(share))
@@ -96,16 +80,16 @@
 	- 例えば(["d1", "d2"], [1], [1, 2])であれば，data_idがd1のテーブルデータとd2のテーブルデータをd1の1列目とd2の2列目をopenした値で突合させて横結合する
 - src: `List[int]`
 	- 総和を計算する列リスト
 ### Returns
 - res: `Dict`
 	- res["is_ok"]: `bool`
 		- 送信が成功したかどうか
-	- res["job_id"]: `str`
-		- 計算スレッドのID
+	- res["job_uuid"]: `str`
+		- 計算スレッドのUUID
 
 ## QMPC.correl
 相関係数を計算する
 ### Parameters
 - join_order: `Tuple[List[str], List[int], List[int]]`
 	- join_order[0]: data_idのリスト
 	- join_order[1]: テーブルデータの結合方向(1:横(open)，2:縦(open)，3:横(share))
@@ -114,16 +98,16 @@
 - inp: `Tuple[List[int], List[int]]`
 	- inp[0]: 相関係数の左列リスト
 	- inp[1]: 相関係数の右列リスト
 ### Returns
 - res: `Dict`
 	- res["is_ok"]: `bool`
 		- 送信が成功したかどうか
-	- res["job_id"]: `str`
-		- 計算スレッドのID
+	- res["job_uuid"]: `str`
+		- 計算スレッドのUUID
 
 ## QMPC.meshcode
 メッシュコードを計算する
 ### Parameters
 - join_order: `Tuple[List[str], List[int], List[int]]`
 	- join_order[0]: data_idのリスト
 	- join_order[1]: テーブルデータの結合方向(1:横(open)，2:縦(open)，3:横(share))
@@ -131,45 +115,46 @@
 	- 例えば(["d1", "d2"], [1], [1, 2])であれば，data_idがd1のテーブルデータとd2のテーブルデータをd1の1列目とd2の2列目をopenした値で突合させて横結合する
 - src: `List[int]`
 	- メッシュコードを計算する列リスト
 ### Returns
 - res: `Dict`
 	- res["is_ok"]: `bool`
 		- 送信が成功したかどうか
-	- res["job_id"]: `str`
-		- 計算スレッドのID
+	- res["job_uuid"]: `str`
+		- 計算スレッドのUUID
 
 ## QMPC.get_join_table
 テーブルを結合する
 ### Parameters
 - join_order: `Tuple[List[str], List[int], List[int]]`
 	- join_order[0]: data_idのリスト
 	- join_order[1]: テーブルデータの結合方向(1:横(open)，2:縦(open)，3:横(share))
 	- join_order[2]: 結合に用いるIDの列リスト
 	- 例えば(["d1", "d2"], [1], [1, 2])であれば，data_idがd1のテーブルデータとd2のテーブルデータをd1の1列目とd2の2列目をopenした値で突合させて横結合する
 ### Returns
 - res: `Dict`
 	- res["is_ok"]: `bool`
 		- 送信が成功したかどうか
-	- res["job_id"]: `str`
-		- 計算スレッドのID
+	- res["job_uuid"]: `str`
+		- 計算スレッドのUUID
 
 ## QMPC.get_computation_result
 計算結果を取得する
 ### Parameters
-- job_id: `str`
-	- 計算スレッドのID
+- job_uuid: `str`
+	- 計算スレッドのUUID
 ### Returns
 - res: `Dict`
 	- res["is_ok"]: `bool`
 		- 送信が成功したかどうか
 	- res["results"]: `List[float]`
 		- 計算結果
 
 ## QMPC.get_data_list
+[deplecated]
 エンジンに保存されているテーブルデータのIDを全て取得する
 ### Parameters
 ### Returns
 - res: `Dict`
 	- res["is_ok"]: `bool`
 		- 送信が成功したかどうか
 	- res["results"]: `List[str]`
```

### Comparing `quickmpc-0.3.4/quickmpc/proto/common_types/common_types_pb2.py` & `quickmpc-0.3.5/quickmpc/proto/common_types/common_types_pb2.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/quickmpc/proto/common_types/common_types_pb2.pyi` & `quickmpc-0.3.5/quickmpc/proto/common_types/common_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2.py` & `quickmpc-0.3.5/quickmpc/proto/libc_to_manage_pb2.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2.pyi` & `quickmpc-0.3.5/quickmpc/proto/libc_to_manage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2_grpc.py` & `quickmpc-0.3.5/quickmpc/proto/libc_to_manage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2_grpc.pyi` & `quickmpc-0.3.5/quickmpc/proto/libc_to_manage_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/quickmpc/qmpc.py` & `quickmpc-0.3.5/quickmpc/qmpc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from dataclasses import dataclass, field, InitVar
 from typing import Dict, List, Optional, Tuple
 
 from .proto.common_types import common_types_pb2
 from .qmpc_server import QMPCServer
 from .share import Share
-from .utils.parse_csv import (parse, parse_csv, ShareValueType)
+from .utils.parse_csv import (parse, parse_csv)
 from .utils.restore import restore
 
 logger = logging.getLogger(__name__)
 # qmpc.JobStatus でアクセスできるようにエイリアスを設定する
 JobStatus \
     = common_types_pb2.JobStatus
 ComputationMethod \
@@ -31,138 +31,138 @@
     def __post_init__(self, endpoints: List[str],
                       token: str):
         logger.info(f"[QuickMPC server IP]={endpoints}")
         object.__setattr__(self, "_QMPC__qmpc_server", QMPCServer(
             endpoints, token))
         object.__setattr__(self, "_QMPC__party_size", len(endpoints))
 
-    def parse_csv_file(self,
-                       filename: str,
-                       matching_column: Optional[int] = 1) \
-            -> Tuple[List[List[ShareValueType]], List[Schema]]:
-        logger.info("parse_csv_file. "
-                    f"[filename]='{filename}'")
-        return parse_csv(filename, matching_column)
-
-    def parse_csv_data(self,
-                       data: List[List[str]],
-                       matching_column: Optional[int] = 1) \
-            -> Tuple[List[List[ShareValueType]], List[Schema]]:
-        logger.info("parse_csv_data. "
-                    f"[data size]={len(data)}x{len(data[0])}")
-        return parse(data, matching_column)
-
-    def send_share(self, secrets: List, schema: List[Schema],
-                   matching_column: int = 1,
-                   piece_size: int = 1_000_000) -> Dict:
-        logger.info("send_share request. "
+    def send_share_from_csv_file(self,
+                                 filename: str,
+                                 matching_column: int = 1,
+                                 piece_size: int = 1_000_000) -> Dict:
+        secrets, schema = parse_csv(filename, matching_column)
+        logger.info("send_share_from_csv_file. "
+                    f"[filename]='{filename}'"
+                    f"[matching ID name]={schema[matching_column-1]}")
+        return self.__qmpc_server.send_share(
+            secrets, schema, matching_column, piece_size)
+
+    def send_share_from_csv_data(self,
+                                 data: List[List[str]],
+                                 matching_column: int = 1,
+                                 piece_size: int = 1_000_000) -> Dict:
+        secrets, schema = parse(data, matching_column)
+        logger.info("send_share_from_csv_data. "
                     f"[secrets size]={len(secrets)}x{len(secrets[0])} "
                     f"[matching ID name]={schema[matching_column-1]}")
         return self.__qmpc_server.send_share(
             secrets, schema, matching_column, piece_size)
 
     def delete_share(self, data_ids: List[str]) -> Dict:
         logger.info("delete_share request. "
                     f"[delete id list]={data_ids}")
         return self.__qmpc_server.delete_share(data_ids)
 
-    def mean(self, join_order: Tuple[List, List, List],
+    def mean(self, join_order: Tuple[List[str], List[int], List[int]],
              src: List) -> Dict:
         logger.info("mean request. "
                     f"[data_id list]={join_order[0]} "
                     f"[join method]={join_order[1]} "
                     f"[matching ID columns]={join_order[2]} "
                     f"[src columns]={src}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_MEAN"),
             join_order, (src, []))
 
-    def variance(self, join_order: Tuple[List, List, List],
+    def variance(self, join_order: Tuple[List[str], List[int], List[int]],
                  src: List) -> Dict:
         logger.info("variance request. "
                     f"[data_id list]={join_order[0]} "
                     f"[join method]={join_order[1]} "
                     f"[matching ID columns]={join_order[2]} "
                     f"[src columns]={src}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_VARIANCE"),
             join_order, (src, []))
 
-    def sum(self, join_order: Tuple[List, List, List], src: List) -> Dict:
+    def sum(self, join_order: Tuple[List[str], List[int], List[int]],
+            src: List) -> Dict:
         logger.info("sum request. "
                     f"[data_id list]={join_order[0]} "
                     f"[join method]={join_order[1]} "
                     f"[matching ID columns]={join_order[2]} "
                     f"[src columns]={src}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_SUM"),
             join_order, (src, []))
 
-    def correl(self, join_order: Tuple[List, List, List],
-               inp: Tuple[List, List]) -> Dict:
+    def correl(self, join_order: Tuple[List[str], List[int], List[int]],
+               inp: Tuple[List[int], List[int]]) -> Dict:
         logger.info("correl request. "
                     f"[data_id list]={join_order[0]} "
                     f"[join method]={join_order[1]} "
                     f"[matching ID columns]={join_order[2]} "
                     f"[src columns]={inp[0]}"
                     f"[target columns]={inp[1]}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_CORREL"),
             join_order, inp)
 
-    def meshcode(self, join_order: Tuple[List, List, List],
+    def meshcode(self, join_order: Tuple[List[str], List[int], List[int]],
                  src: List) -> Dict:
         logger.info("meshcode request. "
                     f"[data_id list]={join_order[0]} "
                     f"[join method]={join_order[1]} "
                     f"[matching ID columns]={join_order[2]} "
                     f"[src columns]={src}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_MESH_CODE"),
             join_order, (src, []))
 
-    def get_join_table(self, join_order: Tuple[List, List, List]) -> Dict:
+    def get_join_table(self,
+                       join_order: Tuple[List[str], List[int], List[int]]) \
+            -> Dict:
         logger.info("get_join_table request. "
                     f"[data_id list]={join_order[0]} "
                     f"[join method]={join_order[1]} "
                     f"[matching ID columns]={join_order[2]}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_JOIN_TABLE"),
             join_order, (join_order[2], []))
 
-    def get_computation_result(self, job_id: str,
+    def get_computation_result(self, job_uuid: str,
                                path: Optional[str] = None) -> Dict:
         logger.info("get_computation_result request. "
-                    f"[job_id]={job_id} "
+                    f"[job_uuid]={job_uuid} "
                     f"[path]={path}")
-        return self.__qmpc_server.get_computation_result(job_id, path)
+        return self.__qmpc_server.get_computation_result(job_uuid, path)
 
     def get_data_list(self) \
             -> Dict:
         logger.info("get_data_list request.")
         return self.__qmpc_server.get_data_list()
 
     def demo_sharize(self, secrets: List) -> Dict:
         logger.info("demo_sharize request. "
                     f"[secrets size]={len(secrets)}x{len(secrets[0])}")
         share = Share.sharize(secrets, self.__party_size)
         return {'is_ok': True, 'results': share}
 
-    def get_elapsed_time(self, job_id: str) -> Dict:
+    def get_elapsed_time(self, job_uuid: str) -> Dict:
         logger.info("get_elapsed_time request. "
-                    f"[job_id]={job_id}")
-        return self.__qmpc_server.get_elapsed_time(job_id)
+                    f"[job_uuid]={job_uuid}")
+        return self.__qmpc_server.get_elapsed_time(job_uuid)
 
-    def restore(self, job_id: str, path: str):
+    def restore(self, job_uuid: str, path: str):
         logger.info("restore request. "
-                    f"[job_id]={job_id} "
+                    f"[job_uuid]={job_uuid} "
                     f"[path]={path}")
-        return restore(job_id, path, self.__party_size)
+        return restore(job_uuid, path, self.__party_size)
 
-    def get_job_error_info(self, job_id: str) -> Dict:
+    def get_job_error_info(self, job_uuid: str) -> Dict:
         logger.info("get_job_error_info request. "
-                    f"[job_id]={job_id}")
-        return self.__qmpc_server.get_job_error_info(job_id)
+                    f"[job_uuid]={job_uuid}")
+        return self.__qmpc_server.get_job_error_info(job_uuid)
 
     @staticmethod
     def set_log_level(level: int):
         logger.setLevel(level)
```

### Comparing `quickmpc-0.3.4/quickmpc/qmpc_server.py` & `quickmpc-0.3.5/quickmpc/qmpc_server.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/quickmpc/share.py` & `quickmpc-0.3.5/quickmpc/share.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/quickmpc/utils/make_pieces.py` & `quickmpc-0.3.5/quickmpc/utils/make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/quickmpc/utils/overload_tools.py` & `quickmpc-0.3.5/quickmpc/utils/overload_tools.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/quickmpc/utils/parse_csv.py` & `quickmpc-0.3.5/quickmpc/utils/parse_csv.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/quickmpc/utils/random.py` & `quickmpc-0.3.5/quickmpc/utils/random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/quickmpc/utils/restore.py` & `quickmpc-0.3.5/quickmpc/utils/restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/quickmpc.egg-info/SOURCES.txt` & `quickmpc-0.3.5/quickmpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/certificates/server1.key` & `quickmpc-0.3.5/tests/unit_tests/certificates/server1.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/certificates/server1.pem` & `quickmpc-0.3.5/tests/unit_tests/certificates/server1.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/certificates/server2.key` & `quickmpc-0.3.5/tests/unit_tests/certificates/server2.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/certificates/server2.pem` & `quickmpc-0.3.5/tests/unit_tests/certificates/server2.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/certificates/server3.key` & `quickmpc-0.3.5/tests/unit_tests/certificates/server3.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/certificates/server3.pem` & `quickmpc-0.3.5/tests/unit_tests/certificates/server3.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/conftest.py` & `quickmpc-0.3.5/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/local_server.py` & `quickmpc-0.3.5/tests/unit_tests/local_server.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/test_files/edge_data.csv` & `quickmpc-0.3.5/tests/unit_tests/test_files/edge_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/test_files/string_data.csv` & `quickmpc-0.3.5/tests/unit_tests/test_files/string_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/test_make_pieces.py` & `quickmpc-0.3.5/tests/unit_tests/test_make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/test_over_load.py` & `quickmpc-0.3.5/tests/unit_tests/test_over_load.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/test_parse.py` & `quickmpc-0.3.5/tests/unit_tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/test_qmpc.py` & `quickmpc-0.3.5/tests/unit_tests/test_qmpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/test_random.py` & `quickmpc-0.3.5/tests/unit_tests/test_random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/test_restore.py` & `quickmpc-0.3.5/tests/unit_tests/test_restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/test_share_recons.py` & `quickmpc-0.3.5/tests/unit_tests/test_share_recons.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.4/tests/unit_tests/test_share_sharize.py` & `quickmpc-0.3.5/tests/unit_tests/test_share_sharize.py`

 * *Files identical despite different names*

