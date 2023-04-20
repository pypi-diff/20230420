# Comparing `tmp/appyter-0.19.8.tar.gz` & `tmp/appyter-0.19.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appyter-0.19.8.tar", last modified: Wed May 11 16:16:24 2022, max compression
+gzip compressed data, was "appyter-0.19.9.tar", last modified: Thu Jun  2 17:14:48 2022, max compression
```

## Comparing `appyter-0.19.8.tar` & `appyter-0.19.9.tar`

### file list

```diff
@@ -1,516 +1,517 @@
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.164750 appyter-0.19.8/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.081417 appyter-0.19.8/.github/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.094750 appyter-0.19.8/.github/workflows/
--rw-r--r--   0 u8sand    (1000) users      (984)      661 2022-04-26 19:20:22.000000 appyter-0.19.8/.github/workflows/deploy-doc-to-ghpages.yml
--rw-r--r--   0 u8sand    (1000) users      (984)       64 2022-04-26 19:20:22.000000 appyter-0.19.8/.gitignore
--rw-r--r--   0 u8sand    (1000) users      (984)    20850 2021-09-29 21:54:05.000000 appyter-0.19.8/LICENSE
--rw-r--r--   0 u8sand    (1000) users      (984)      243 2022-04-26 19:20:22.000000 appyter-0.19.8/MANIFEST.in
--rw-r--r--   0 u8sand    (1000) users      (984)     6685 2022-05-11 16:16:24.164750 appyter-0.19.8/PKG-INFO
--rw-r--r--   0 u8sand    (1000) users      (984)     5958 2022-04-26 19:20:22.000000 appyter-0.19.8/README.md
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.094750 appyter-0.19.8/appyter/
--rw-r--r--   0 u8sand    (1000) users      (984)        6 2022-05-11 16:08:22.000000 appyter-0.19.8/appyter/VERSION
--rw-r--r--   0 u8sand    (1000) users      (984)      276 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)      393 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/__main__.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1305 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/cli.py
--rw-r--r--   0 u8sand    (1000) users      (984)    11535 2022-05-11 16:08:16.000000 appyter-0.19.8/appyter/context.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.098084 appyter-0.19.8/appyter/execspec/
--rw-r--r--   0 u8sand    (1000) users      (984)      127 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/execspec/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)      372 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/execspec/core.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.098084 appyter-0.19.8/appyter/execspec/implementations/
--rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/execspec/implementations/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)     4673 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/execspec/implementations/cavatica.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1719 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/execspec/implementations/dispatch.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2249 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/execspec/implementations/docker.py
--rw-r--r--   0 u8sand    (1000) users      (984)     4329 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/execspec/implementations/kube.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1381 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/execspec/implementations/local.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1138 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/execspec/implementations/subprocess.py
--rw-r--r--   0 u8sand    (1000) users      (984)     5448 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/execspec/implementations/wes.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1825 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/execspec/registry.py
--rw-r--r--   0 u8sand    (1000) users      (984)      792 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/execspec/spec.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.101417 appyter-0.19.8/appyter/ext/
--rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/ext/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1040 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/aiohttp.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.101417 appyter-0.19.8/appyter/ext/asyncio/
--rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-04-25 15:13:20.000000 appyter-0.19.8/appyter/ext/asyncio/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2714 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/asyncio/event_emitter.py
--rw-r--r--   0 u8sand    (1000) users      (984)     3285 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/asyncio/event_loop.py
--rw-r--r--   0 u8sand    (1000) users      (984)     5306 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/asyncio/helpers.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1484 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/asyncio/subprocess.py
--rw-r--r--   0 u8sand    (1000) users      (984)     6656 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/asyncio/test_helpers.py
--rw-r--r--   0 u8sand    (1000) users      (984)      741 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/asyncio/test_subprocess.py
--rw-r--r--   0 u8sand    (1000) users      (984)      817 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/asyncio/try_n_times.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.101417 appyter-0.19.8/appyter/ext/click/
--rw-r--r--   0 u8sand    (1000) users      (984)     1238 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/ext/click/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)      972 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/contextlib.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2260 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/cryptography.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1923 2022-05-11 16:08:16.000000 appyter-0.19.8/appyter/ext/dict.py
--rw-r--r--   0 u8sand    (1000) users      (984)      868 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/drs.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2138 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/emitter.py
--rw-r--r--   0 u8sand    (1000) users      (984)      204 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/exceptions.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2341 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/flask.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.104750 appyter-0.19.8/appyter/ext/fsspec/
--rw-r--r--   0 u8sand    (1000) users      (984)      575 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)     9573 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/chroot.py
--rw-r--r--   0 u8sand    (1000) users      (984)     3450 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/core.py
--rw-r--r--   0 u8sand    (1000) users      (984)     3569 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/drs.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1799 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/fuse.py
--rw-r--r--   0 u8sand    (1000) users      (984)     6090 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/mapperfs.py
--rw-r--r--   0 u8sand    (1000) users      (984)     7526 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/overlayfs.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1933 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/s3fs.py
--rw-r--r--   0 u8sand    (1000) users      (984)    18894 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/sbfs.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1504 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/singleton.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.108084 appyter-0.19.8/appyter/ext/fsspec/spec/
--rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/spec/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1453 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/spec/composable.py
--rw-r--r--   0 u8sand    (1000) users      (984)      589 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/spec/mountable.py
--rw-r--r--   0 u8sand    (1000) users      (984)     4707 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/spec/sync_async.py
--rw-r--r--   0 u8sand    (1000) users      (984)      556 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/storage.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1962 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/test_chroot.py
--rw-r--r--   0 u8sand    (1000) users      (984)     3578 2022-05-11 16:08:16.000000 appyter-0.19.8/appyter/ext/fsspec/test_drs.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1794 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/test_fuse.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1911 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/test_fuseless_mount.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1054 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/test_mapperfs.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2154 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/test_overlayfs.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2599 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/test_pathmap.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1619 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/test_sbfs.py
--rw-r--r--   0 u8sand    (1000) users      (984)      628 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/util.py
--rw-r--r--   0 u8sand    (1000) users      (984)     8710 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/fsspec/writecache.py
--rw-r--r--   0 u8sand    (1000) users      (984)      526 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/functools.py
--rw-r--r--   0 u8sand    (1000) users      (984)      657 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/hashlib.py
--rw-r--r--   0 u8sand    (1000) users      (984)      914 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/importlib.py
--rw-r--r--   0 u8sand    (1000) users      (984)      427 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/io.py
--rw-r--r--   0 u8sand    (1000) users      (984)      581 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/itertools.py
--rw-r--r--   0 u8sand    (1000) users      (984)      378 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/json.py
--rw-r--r--   0 u8sand    (1000) users      (984)       57 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/multiprocessing.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.108084 appyter-0.19.8/appyter/ext/nbclient/
--rw-r--r--   0 u8sand    (1000) users      (984)     4148 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/nbclient/__init__.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.108084 appyter-0.19.8/appyter/ext/pathlib/
--rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/pathlib/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)      434 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/pathlib/assertions.py
--rw-r--r--   0 u8sand    (1000) users      (984)      932 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/pathlib/chroot.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1381 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/pytest.py
--rw-r--r--   0 u8sand    (1000) users      (984)      200 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/re.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.108084 appyter-0.19.8/appyter/ext/socketio/
--rw-r--r--   0 u8sand    (1000) users      (984)      103 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/ext/socketio/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1169 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/socketio/chunked_emit.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1038 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/socketio/client.py
--rw-r--r--   0 u8sand    (1000) users      (984)      502 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/socketio/forwarding.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1567 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/socketio/priority_queued_emit.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1101 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/socketio/server.py
--rw-r--r--   0 u8sand    (1000) users      (984)      238 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/subprocess.py
--rw-r--r--   0 u8sand    (1000) users      (984)      830 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/tempfile.py
--rw-r--r--   0 u8sand    (1000) users      (984)     9328 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/urllib.py
--rw-r--r--   0 u8sand    (1000) users      (984)      284 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/ext/uuid.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.108084 appyter-0.19.8/appyter/ext/watchgod/
--rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/ext/watchgod/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1010 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/ext/watchgod/watcher.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.108084 appyter-0.19.8/appyter/extras/
--rw-r--r--   0 u8sand    (1000) users      (984)      667 2022-04-28 16:42:16.000000 appyter-0.19.8/appyter/extras/__init__.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.111417 appyter-0.19.8/appyter/extras/catalog_integration/
--rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/extras/catalog_integration/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1335 2022-05-11 16:08:16.000000 appyter-0.19.8/appyter/extras/catalog_integration/executor.py
--rw-r--r--   0 u8sand    (1000) users      (984)      721 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/extras/catalog_integration/notebooks.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1973 2022-05-11 15:50:01.000000 appyter-0.19.8/appyter/extras/catalog_integration/request.py
--rw-r--r--   0 u8sand    (1000) users      (984)      896 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/extras/catalog_integration/storage.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1034 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/extras/catalog_integration/uploads.py
--rw-r--r--   0 u8sand    (1000) users      (984)      506 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/extras/catalog_integration/user_config.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2902 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/extras/catalog_integration/userfs.py
--rw-r--r--   0 u8sand    (1000) users      (984)     8490 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/fields.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.111417 appyter-0.19.8/appyter/helpers/
--rw-r--r--   0 u8sand    (1000) users      (984)      180 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/helpers/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)     4215 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/helpers/commandify.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.111417 appyter-0.19.8/appyter/helpers/cookiecutter/
--rw-r--r--   0 u8sand    (1000) users      (984)      391 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/helpers/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.111417 appyter-0.19.8/appyter/helpers/cookiecutter/{{ cookiecutter.project_slug }}/
--rw-r--r--   0 u8sand    (1000) users      (984)      430 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/helpers/cookiecutter/{{ cookiecutter.project_slug }}/README.md
--rw-r--r--   0 u8sand    (1000) users      (984)      719 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/helpers/cookiecutter/{{ cookiecutter.project_slug }}/appyter.json
--rw-r--r--   0 u8sand    (1000) users      (984)      192 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/helpers/cookiecutter/{{ cookiecutter.project_slug }}/requirements.txt
--rw-r--r--   0 u8sand    (1000) users      (984)     1746 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/helpers/cookiecutter/{{ cookiecutter.project_slug }}/{{ cookiecutter.project_slug }}.ipynb
--rw-r--r--   0 u8sand    (1000) users      (984)      829 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/helpers/dockerize.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2045 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/helpers/fetch_and_serve.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1696 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/helpers/init.py
--rw-r--r--   0 u8sand    (1000) users      (984)      820 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/helpers/nbclean.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2223 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/helpers/serve.py
--rw-r--r--   0 u8sand    (1000) users      (984)     4661 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/magic.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.111417 appyter-0.19.8/appyter/orchestration/
--rw-r--r--   0 u8sand    (1000) users      (984)      178 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/orchestration/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)      221 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/orchestration/cli.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.111417 appyter-0.19.8/appyter/orchestration/dispatcher/
--rw-r--r--   0 u8sand    (1000) users      (984)     2638 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/orchestration/dispatcher/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)     3118 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/orchestration/dispatcher/core.py
--rw-r--r--   0 u8sand    (1000) users      (984)       91 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/orchestration/dispatcher/socketio.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.114750 appyter-0.19.8/appyter/parse/
--rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/parse/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)      594 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/parse/nb.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1257 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/parse/nbtemplate.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.114750 appyter-0.19.8/appyter/profiles/
--rw-r--r--   0 u8sand    (1000) users      (984)      817 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/__init__.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.114750 appyter-0.19.8/appyter/profiles/biojupies/
--rw-r--r--   0 u8sand    (1000) users      (984)       72 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/biojupies/__init__.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.114750 appyter-0.19.8/appyter/profiles/biojupies/templates/
--rw-r--r--   0 u8sand    (1000) users      (984)       33 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/biojupies/templates/base.j2
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.114750 appyter-0.19.8/appyter/profiles/biojupies/templates/biojupies/
--rw-r--r--   0 u8sand    (1000) users      (984)      860 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/biojupies/templates/biojupies/base.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      290 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/biojupies/templates/biojupies/form.j2
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.114750 appyter-0.19.8/appyter/profiles/biojupies/templates/fields/
--rw-r--r--   0 u8sand    (1000) users      (984)      962 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/biojupies/templates/fields/BoolField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      630 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/biojupies/templates/fields/ChoiceField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      605 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/biojupies/templates/fields/FloatField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/biojupies/templates/fields/IntField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      656 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/biojupies/templates/fields/MultiChoiceField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/biojupies/templates/fields/SectionField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/biojupies/templates/fields/StringField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/biojupies/templates/fields/TextField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/biojupies/templates/fields/TextListField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       33 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/biojupies/templates/form.j2
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.114750 appyter-0.19.8/appyter/profiles/bootstrap/
--rw-r--r--   0 u8sand    (1000) users      (984)       61 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/bootstrap/__init__.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.084750 appyter-0.19.8/appyter/profiles/bootstrap/static/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.114750 appyter-0.19.8/appyter/profiles/bootstrap/static/css/
--rw-r--r--   0 u8sand    (1000) users      (984)   161994 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/bootstrap/static/css/bootstrap.css
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.084750 appyter-0.19.8/appyter/profiles/bootstrap/static/js/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.084750 appyter-0.19.8/appyter/profiles/bootstrap/static/js/lib/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.114750 appyter-0.19.8/appyter/profiles/bootstrap/static/js/lib/bootstrap/
--rw-r--r--   0 u8sand    (1000) users      (984)    84378 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/bootstrap/static/js/lib/bootstrap/bootstrap.bundle.min.js
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.118084 appyter-0.19.8/appyter/profiles/bootstrap/static/js/lib/select2/
--rw-r--r--   0 u8sand    (1000) users      (984)    70851 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/bootstrap/static/js/lib/select2/select2.min.js
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.118084 appyter-0.19.8/appyter/profiles/bootstrap/templates/
--rw-r--r--   0 u8sand    (1000) users      (984)       33 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/bootstrap/templates/base.j2
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.118084 appyter-0.19.8/appyter/profiles/bootstrap/templates/bootstrap/
--rw-r--r--   0 u8sand    (1000) users      (984)      649 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/bootstrap/templates/bootstrap/base.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      341 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/bootstrap/templates/bootstrap/form.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       33 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/bootstrap/templates/form.j2
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.118084 appyter-0.19.8/appyter/profiles/default/
--rw-r--r--   0 u8sand    (1000) users      (984)      243 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/__init__.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.118084 appyter-0.19.8/appyter/profiles/default/blueprints/
--rw-r--r--   0 u8sand    (1000) users      (984)     2760 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/blueprints/StorageFileField.py
--rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/blueprints/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1448 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/blueprints/locate.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.121417 appyter-0.19.8/appyter/profiles/default/fields/
--rw-r--r--   0 u8sand    (1000) users      (984)     2272 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/fields/AutocompleteField.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1782 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/fields/BoolField.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1374 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/fields/ChoiceField.py
--rw-r--r--   0 u8sand    (1000) users      (984)      901 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/fields/DescriptionField.py
--rw-r--r--   0 u8sand    (1000) users      (984)     4869 2022-04-28 16:45:18.000000 appyter-0.19.8/appyter/profiles/default/fields/FileField.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1515 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/fields/FloatField.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2287 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/fields/IntField.py
--rw-r--r--   0 u8sand    (1000) users      (984)     3658 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/fields/MultiCheckboxField.py
--rw-r--r--   0 u8sand    (1000) users      (984)     3420 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/fields/MultiChoiceField.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1177 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/fields/SectionField.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2102 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/fields/StringField.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1611 2022-05-11 14:44:24.000000 appyter-0.19.8/appyter/profiles/default/fields/TabField.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2326 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/fields/TextField.py
--rw-r--r--   0 u8sand    (1000) users      (984)     4329 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/fields/TextListField.py
--rw-r--r--   0 u8sand    (1000) users      (984)     3944 2022-05-11 14:44:24.000000 appyter-0.19.8/appyter/profiles/default/fields/VariableField.py
--rw-r--r--   0 u8sand    (1000) users      (984)      279 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/fields/__init__.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.121417 appyter-0.19.8/appyter/profiles/default/filters/
--rw-r--r--   0 u8sand    (1000) users      (984)      105 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/filters/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)       75 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/filters/atob.py
--rw-r--r--   0 u8sand    (1000) users      (984)       75 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/filters/btoa.py
--rw-r--r--   0 u8sand    (1000) users      (984)       63 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/filters/fmt.py
--rw-r--r--   0 u8sand    (1000) users      (984)       51 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/filters/join_routes.py
--rw-r--r--   0 u8sand    (1000) users      (984)       52 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/filters/jsonify.py
--rw-r--r--   0 u8sand    (1000) users      (984)      179 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/filters/pyeval.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1080 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/filters/url_for.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.121417 appyter-0.19.8/appyter/profiles/default/templates/
--rw-r--r--   0 u8sand    (1000) users      (984)       31 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/base.j2
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.121417 appyter-0.19.8/appyter/profiles/default/templates/default/
--rw-r--r--   0 u8sand    (1000) users      (984)     1412 2022-05-11 16:08:16.000000 appyter-0.19.8/appyter/profiles/default/templates/default/base.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      483 2022-03-26 22:16:07.000000 appyter-0.19.8/appyter/profiles/default/templates/default/form.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      417 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/templates/default/landing.j2
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.124750 appyter-0.19.8/appyter/profiles/default/templates/fields/
--rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/AutocompleteField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      328 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/BoolField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      462 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/ChoiceField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      149 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/DescriptionField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/FileField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      371 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/FloatField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      964 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/IntField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/MultiCheckboxField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      479 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/MultiChoiceField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       16 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/SectionField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      353 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/StringField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/TabField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      411 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/TextField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      466 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/TextListField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fields/VariableField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       31 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/form.j2
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.124750 appyter-0.19.8/appyter/profiles/default/templates/fragments/
--rw-r--r--   0 u8sand    (1000) users      (984)   221111 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fragments/jupyter.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      107 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fragments/loader.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      203 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/templates/fragments/svelte-field.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       34 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/profiles/default/templates/landing.j2
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.128084 appyter-0.19.8/appyter/profiles/default/templates/production/
--rw-r--r--   0 u8sand    (1000) users      (984)     2574 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/templates/production/Dockerfile.j2
--rw-r--r--   0 u8sand    (1000) users      (984)     6388 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/templates/production/nginx.conf.j2
--rw-r--r--   0 u8sand    (1000) users      (984)     1221 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/profiles/default/templates/production/supervisord.conf.j2
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.128084 appyter-0.19.8/appyter/render/
--rw-r--r--   0 u8sand    (1000) users      (984)      218 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/__init__.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.128084 appyter-0.19.8/appyter/render/flask_app/
--rw-r--r--   0 u8sand    (1000) users      (984)     7285 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/flask_app/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)     3858 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/flask_app/constants.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2049 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/flask_app/core.py
--rw-r--r--   0 u8sand    (1000) users      (984)     4321 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/flask_app/development.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2614 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/flask_app/drs.py
--rw-r--r--   0 u8sand    (1000) users      (984)     3097 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/flask_app/execution.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2214 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/flask_app/export.py
--rw-r--r--   0 u8sand    (1000) users      (984)      386 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/render/flask_app/livereload.py
--rw-r--r--   0 u8sand    (1000) users      (984)     5024 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/flask_app/prepare.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2167 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/flask_app/production.py
--rw-r--r--   0 u8sand    (1000) users      (984)     2410 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/flask_app/room_manager.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1029 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/flask_app/socketio.py
--rw-r--r--   0 u8sand    (1000) users      (984)     3381 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/flask_app/static.py
--rw-r--r--   0 u8sand    (1000) users      (984)     4823 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/flask_app/upload.py
--rw-r--r--   0 u8sand    (1000) users      (984)      355 2022-03-25 22:22:22.000000 appyter-0.19.8/appyter/render/form.py
--rw-r--r--   0 u8sand    (1000) users      (984)     3612 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/nbconstruct.py
--rw-r--r--   0 u8sand    (1000) users      (984)     7300 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/nbexecute.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.131417 appyter-0.19.8/appyter/render/nbinspect/
--rw-r--r--   0 u8sand    (1000) users      (984)      187 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/nbinspect/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)      212 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/nbinspect/cli.py
--rw-r--r--   0 u8sand    (1000) users      (984)     4049 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/nbinspect/cwl.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1707 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/nbinspect/jsonschema.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1392 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/nbinspect/nbtemplate_json.py
--rw-r--r--   0 u8sand    (1000) users      (984)    12378 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/render/nbinspect/openapi.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.131417 appyter-0.19.8/appyter/static/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.088083 appyter-0.19.8/appyter/static/profiles/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.088083 appyter-0.19.8/appyter/static/profiles/biojupies/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.131417 appyter-0.19.8/appyter/static/profiles/biojupies/css/
--rw-r--r--   0 u8sand    (1000) users      (984)    59305 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/css/fontawesome.css
--rw-r--r--   0 u8sand    (1000) users      (984)   160873 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/biojupies/css/index.css
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.131417 appyter-0.19.8/appyter/static/profiles/biojupies/js/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.131417 appyter-0.19.8/appyter/static/profiles/biojupies/js/fields/
--rw-r--r--   0 u8sand    (1000) users      (984)     7545 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/biojupies/js/fields/IntField.js
--rw-r--r--   0 u8sand    (1000) users      (984)    13813 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/biojupies/js/fields/SectionField.js
--rw-r--r--   0 u8sand    (1000) users      (984)     9133 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/biojupies/js/fields/StringField.js
--rw-r--r--   0 u8sand    (1000) users      (984)     8532 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/biojupies/js/fields/TextField.js
--rw-r--r--   0 u8sand    (1000) users      (984)     9326 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/biojupies/js/fields/TextListField.js
--rw-r--r--   0 u8sand    (1000) users      (984)    29461 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/biojupies/js/form.js
--rw-r--r--   0 u8sand    (1000) users      (984)     3038 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/biojupies/js/index.js
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.131417 appyter-0.19.8/appyter/static/profiles/biojupies/js/lib/
--rw-r--r--   0 u8sand    (1000) users      (984)    83862 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/biojupies/js/lib/bootstrap.js
--rw-r--r--   0 u8sand    (1000) users      (984)      237 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/biojupies/js/lib/bootstrap.js.LICENSE.txt
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.141417 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/
--rw-r--r--   0 u8sand    (1000) users      (984)   134294 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-brands-400.eot
--rw-r--r--   0 u8sand    (1000) users      (984)   747927 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-brands-400.svg
--rw-r--r--   0 u8sand    (1000) users      (984)   133988 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-brands-400.ttf
--rw-r--r--   0 u8sand    (1000) users      (984)    89988 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-brands-400.woff
--rw-r--r--   0 u8sand    (1000) users      (984)    76736 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-brands-400.woff2
--rw-r--r--   0 u8sand    (1000) users      (984)    34034 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-regular-400.eot
--rw-r--r--   0 u8sand    (1000) users      (984)   144714 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-regular-400.svg
--rw-r--r--   0 u8sand    (1000) users      (984)    33736 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-regular-400.ttf
--rw-r--r--   0 u8sand    (1000) users      (984)    16276 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-regular-400.woff
--rw-r--r--   0 u8sand    (1000) users      (984)    13224 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-regular-400.woff2
--rw-r--r--   0 u8sand    (1000) users      (984)   203030 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-solid-900.eot
--rw-r--r--   0 u8sand    (1000) users      (984)   918991 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-solid-900.svg
--rw-r--r--   0 u8sand    (1000) users      (984)   202744 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-solid-900.ttf
--rw-r--r--   0 u8sand    (1000) users      (984)   101648 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-solid-900.woff
--rw-r--r--   0 u8sand    (1000) users      (984)    78268 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.088083 appyter-0.19.8/appyter/static/profiles/bootstrap/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.141417 appyter-0.19.8/appyter/static/profiles/bootstrap/css/
--rw-r--r--   0 u8sand    (1000) users      (984)   167619 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/bootstrap/css/index.css
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.141417 appyter-0.19.8/appyter/static/profiles/bootstrap/js/
--rw-r--r--   0 u8sand    (1000) users      (984)     3038 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/bootstrap/js/index.js
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.088083 appyter-0.19.8/appyter/static/profiles/default/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.141417 appyter-0.19.8/appyter/static/profiles/default/css/
--rw-r--r--   0 u8sand    (1000) users      (984)     2443 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/css/index.css
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.141417 appyter-0.19.8/appyter/static/profiles/default/js/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.144750 appyter-0.19.8/appyter/static/profiles/default/js/chunks/
--rw-r--r--   0 u8sand    (1000) users      (984)    35216 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/229.js
--rw-r--r--   0 u8sand    (1000) users      (984)    19816 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/246.js
--rw-r--r--   0 u8sand    (1000) users      (984)      254 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/284.js
--rw-r--r--   0 u8sand    (1000) users      (984)     6501 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/29.js
--rw-r--r--   0 u8sand    (1000) users      (984)    28673 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/316.js
--rw-r--r--   0 u8sand    (1000) users      (984)     2356 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/322.js
--rw-r--r--   0 u8sand    (1000) users      (984)      741 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/494.js
--rw-r--r--   0 u8sand    (1000) users      (984)    21282 2022-05-11 16:08:16.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/58.js
--rw-r--r--   0 u8sand    (1000) users      (984)    36325 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/671.js
--rw-r--r--   0 u8sand    (1000) users      (984)      187 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/671.js.LICENSE.txt
--rw-r--r--   0 u8sand    (1000) users      (984)   147776 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/680.js
--rw-r--r--   0 u8sand    (1000) users      (984)      447 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/704.js
--rw-r--r--   0 u8sand    (1000) users      (984)     1435 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/755.js
--rw-r--r--   0 u8sand    (1000) users      (984)      832 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/798.js
--rw-r--r--   0 u8sand    (1000) users      (984)     4127 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/826.js
--rw-r--r--   0 u8sand    (1000) users      (984)     7405 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/849.js
--rw-r--r--   0 u8sand    (1000) users      (984)    14487 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/chunks/977.js
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.144750 appyter-0.19.8/appyter/static/profiles/default/js/fields/
--rw-r--r--   0 u8sand    (1000) users      (984)    13697 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/fields/AutocompleteField.js
--rw-r--r--   0 u8sand    (1000) users      (984)    20120 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/fields/FileField.js
--rw-r--r--   0 u8sand    (1000) users      (984)     8075 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/fields/MultiCheckboxField.js
--rw-r--r--   0 u8sand    (1000) users      (984)    13458 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/fields/TabField.js
--rw-r--r--   0 u8sand    (1000) users      (984)    11928 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/fields/VariableField.js
--rw-r--r--   0 u8sand    (1000) users      (984)     2957 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/index.js
--rw-r--r--   0 u8sand    (1000) users      (984)    29508 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/landing.js
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.144750 appyter-0.19.8/appyter/static/profiles/default/js/lib/
--rw-r--r--   0 u8sand    (1000) users      (984)    89521 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/lib/jquery.js
--rw-r--r--   0 u8sand    (1000) users      (984)       89 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/lib/jquery.js.LICENSE.txt
--rw-r--r--   0 u8sand    (1000) users      (984)    17656 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/lib/require.js
--rw-r--r--   0 u8sand    (1000) users      (984)      202 2022-05-11 15:20:50.000000 appyter-0.19.8/appyter/static/profiles/default/js/lib/require.js.LICENSE.txt
--rw-r--r--   0 u8sand    (1000) users      (984)      115 2022-04-26 19:20:22.000000 appyter-0.19.8/appyter/static/silent-check-sso.html
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.094750 appyter-0.19.8/appyter.egg-info/
--rw-r--r--   0 u8sand    (1000) users      (984)     6685 2022-05-11 16:16:22.000000 appyter-0.19.8/appyter.egg-info/PKG-INFO
--rw-r--r--   0 u8sand    (1000) users      (984)    16226 2022-05-11 16:16:23.000000 appyter-0.19.8/appyter.egg-info/SOURCES.txt
--rw-r--r--   0 u8sand    (1000) users      (984)        1 2022-05-11 16:16:22.000000 appyter-0.19.8/appyter.egg-info/dependency_links.txt
--rw-r--r--   0 u8sand    (1000) users      (984)       50 2022-05-11 16:16:23.000000 appyter-0.19.8/appyter.egg-info/entry_points.txt
--rw-r--r--   0 u8sand    (1000) users      (984)      459 2022-05-11 16:16:23.000000 appyter-0.19.8/appyter.egg-info/requires.txt
--rw-r--r--   0 u8sand    (1000) users      (984)        8 2022-05-11 16:16:23.000000 appyter-0.19.8/appyter.egg-info/top_level.txt
--rw-r--r--   0 u8sand    (1000) users      (984)       17 2021-05-03 14:23:28.000000 appyter-0.19.8/deps.production.txt
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.148084 appyter-0.19.8/docs/
--rw-r--r--   0 u8sand    (1000) users      (984)       29 2021-05-03 14:23:28.000000 appyter-0.19.8/docs/.gitignore
--rw-r--r--   0 u8sand    (1000) users      (984)      800 2021-05-03 14:23:28.000000 appyter-0.19.8/docs/Makefile
--rw-r--r--   0 u8sand    (1000) users      (984)      799 2021-05-03 14:23:28.000000 appyter-0.19.8/docs/make.bat
--rw-r--r--   0 u8sand    (1000) users      (984)       46 2022-04-26 19:20:22.000000 appyter-0.19.8/docs/requirements.txt
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.148084 appyter-0.19.8/docs/source/
--rw-r--r--   0 u8sand    (1000) users      (984)       13 2021-05-03 14:23:28.000000 appyter-0.19.8/docs/source/.gitignore
--rw-r--r--   0 u8sand    (1000) users      (984)     3539 2022-04-26 19:20:22.000000 appyter-0.19.8/docs/source/conf.py
--rw-r--r--   0 u8sand    (1000) users      (984)      507 2021-05-03 14:23:28.000000 appyter-0.19.8/docs/source/index.rst
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.148084 appyter-0.19.8/example/
--rw-r--r--   0 u8sand    (1000) users      (984)       10 2022-03-16 21:31:07.000000 appyter-0.19.8/example/.dockerignore
--rw-r--r--   0 u8sand    (1000) users      (984)     1501 2022-04-26 19:20:22.000000 appyter-0.19.8/example/Dockerfile
--rw-r--r--   0 u8sand    (1000) users      (984)     1543 2022-04-26 19:20:22.000000 appyter-0.19.8/example/README.md
--rw-r--r--   0 u8sand    (1000) users      (984)     3792 2022-04-26 19:20:22.000000 appyter-0.19.8/example/appyter.cwl
--rw-r--r--   0 u8sand    (1000) users      (984)      651 2022-04-26 19:20:22.000000 appyter-0.19.8/example/appyter.json
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.148084 appyter-0.19.8/example/blueprints/
--rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-02-22 22:19:08.000000 appyter-0.19.8/example/blueprints/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)      153 2022-02-22 22:19:08.000000 appyter-0.19.8/example/blueprints/testblueprint.py
--rw-r--r--   0 u8sand    (1000) users      (984)     1392 2022-04-26 19:20:22.000000 appyter-0.19.8/example/blueprints/testdash.py
--rw-r--r--   0 u8sand    (1000) users      (984)     7973 2022-04-26 19:20:22.000000 appyter-0.19.8/example/example.ipynb
--rw-r--r--   0 u8sand    (1000) users      (984)      854 2022-04-26 19:20:22.000000 appyter-0.19.8/example/example_test.py
--rw-r--r--   0 u8sand    (1000) users      (984)      468 2022-04-26 19:20:22.000000 appyter-0.19.8/example/example_test.sh
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.148084 appyter-0.19.8/example/fields/
--rw-r--r--   0 u8sand    (1000) users      (984)      269 2021-05-03 14:23:28.000000 appyter-0.19.8/example/fields/EmailField.py
--rw-r--r--   0 u8sand    (1000) users      (984)        0 2021-05-03 14:23:28.000000 appyter-0.19.8/example/fields/__init__.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.151417 appyter-0.19.8/example/filters/
--rw-r--r--   0 u8sand    (1000) users      (984)        0 2021-05-03 14:23:28.000000 appyter-0.19.8/example/filters/__init__.py
--rw-r--r--   0 u8sand    (1000) users      (984)      257 2021-05-03 14:23:28.000000 appyter-0.19.8/example/filters/do_op.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.151417 appyter-0.19.8/example/production/
--rw-r--r--   0 u8sand    (1000) users      (984)       72 2021-05-03 14:23:28.000000 appyter-0.19.8/example/production/.env.example
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.151417 appyter-0.19.8/example/production/appyter/
--rw-r--r--   0 u8sand    (1000) users      (984)      802 2021-05-03 14:23:28.000000 appyter-0.19.8/example/production/appyter/Dockerfile
--rw-r--r--   0 u8sand    (1000) users      (984)     1246 2022-04-26 19:20:22.000000 appyter-0.19.8/example/production/docker-compose.yml
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.151417 appyter-0.19.8/example/production/s3/
--rw-r--r--   0 u8sand    (1000) users      (984)      222 2021-05-03 14:23:28.000000 appyter-0.19.8/example/production/s3/Dockerfile
--rw-r--r--   0 u8sand    (1000) users      (984)      429 2021-05-03 14:23:28.000000 appyter-0.19.8/example/production/s3/entrypoint.sh
--rw-r--r--   0 u8sand    (1000) users      (984)       17 2021-05-03 14:23:28.000000 appyter-0.19.8/example/requirements.txt
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.151417 appyter-0.19.8/example/static/
--rw-r--r--   0 u8sand    (1000) users      (984)     7110 2021-05-03 14:23:28.000000 appyter-0.19.8/example/static/GitHub-Mark.png
--rw-r--r--   0 u8sand    (1000) users      (984)       19 2021-05-03 14:23:28.000000 appyter-0.19.8/example/static/test.js
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.151417 appyter-0.19.8/example/templates/
--rw-r--r--   0 u8sand    (1000) users      (984)      424 2022-04-26 19:20:22.000000 appyter-0.19.8/example/templates/base.j2
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.151417 appyter-0.19.8/example/templates/fields/
--rw-r--r--   0 u8sand    (1000) users      (984)      354 2021-05-03 14:23:28.000000 appyter-0.19.8/example/templates/fields/EmailField.j2
--rw-r--r--   0 u8sand    (1000) users      (984)      352 2021-05-03 14:23:28.000000 appyter-0.19.8/example/templates/form.j2
--rw-r--r--   0 u8sand    (1000) users      (984)       42 2021-05-03 14:23:28.000000 appyter-0.19.8/example/test.py
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.151417 appyter-0.19.8/js/
--rw-r--r--   0 u8sand    (1000) users      (984)       12 2021-05-03 14:23:28.000000 appyter-0.19.8/js/.gitignore
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.154750 appyter-0.19.8/js/components/
--rw-r--r--   0 u8sand    (1000) users      (984)      187 2021-05-03 14:23:28.000000 appyter-0.19.8/js/components/Ansi.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      691 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/HTML.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      558 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/Lazy.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      178 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/Loader.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      159 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/Markdown.svelte
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.154750 appyter-0.19.8/js/components/app/
--rw-r--r--   0 u8sand    (1000) users      (984)      129 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/app/Error.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     1137 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/app/SSRField.svelte
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.154750 appyter-0.19.8/js/components/fields/
--rw-r--r--   0 u8sand    (1000) users      (984)      142 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/fields/DescriptionField.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     1166 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/fields/SectionField.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     2022 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/fields/StringField.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     1117 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/fields/TabField.svelte
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.154750 appyter-0.19.8/js/components/jupyter/
--rw-r--r--   0 u8sand    (1000) users      (984)      118 2021-05-03 14:23:28.000000 appyter-0.19.8/js/components/jupyter/Cell.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)       68 2021-05-03 14:23:28.000000 appyter-0.19.8/js/components/jupyter/Cells.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)       42 2021-05-03 14:23:28.000000 appyter-0.19.8/js/components/jupyter/Input.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     2071 2022-04-26 19:25:20.000000 appyter-0.19.8/js/components/jupyter/Notebook.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      860 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/Output.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     1514 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/OutputMimetype.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     1790 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/Outputs.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      578 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/Prompt.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      309 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/Source.svelte
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.158084 appyter-0.19.8/js/components/jupyter/output_mimetype/
--rw-r--r--   0 u8sand    (1000) users      (984)      207 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/output_mimetype/ApplicationJavascript.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      220 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/output_mimetype/ImagePng.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      185 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/output_mimetype/ImageSvgXml.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      200 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/output_mimetype/TextHtml.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      211 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/output_mimetype/TextMarkdown.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      280 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/output_mimetype/TextPlain.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      802 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/output_mimetype/index.js
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.158084 appyter-0.19.8/js/components/jupyter/output_type/
--rw-r--r--   0 u8sand    (1000) users      (984)      186 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/output_type/OutputDisplayData.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      585 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/output_type/OutputError.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      188 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/output_type/OutputExecuteResult.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      233 2022-04-26 19:20:22.000000 appyter-0.19.8/js/components/jupyter/output_type/OutputStream.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      392 2021-09-29 21:54:05.000000 appyter-0.19.8/js/components/jupyter/output_type/index.js
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.091417 appyter-0.19.8/js/extras/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.158084 appyter-0.19.8/js/extras/catalog-integration/
--rw-r--r--   0 u8sand    (1000) users      (984)     4499 2022-05-11 16:08:16.000000 appyter-0.19.8/js/extras/catalog-integration/LaunchSettings.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     1517 2022-04-26 19:20:22.000000 appyter-0.19.8/js/extras/catalog-integration/LocateFileField.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      940 2022-04-26 19:20:22.000000 appyter-0.19.8/js/extras/catalog-integration/TableOfContents.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      678 2022-04-26 19:20:22.000000 appyter-0.19.8/js/extras/catalog-integration/pagehit.js
--rw-r--r--   0 u8sand    (1000) users      (984)     1047 2022-04-26 19:20:22.000000 appyter-0.19.8/js/extras/catalog-integration/report_error.js
--rw-r--r--   0 u8sand    (1000) users      (984)     1450 2022-04-26 19:20:22.000000 appyter-0.19.8/js/extras/catalog-integration/toc.js
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.158084 appyter-0.19.8/js/extras/file-field/
--rw-r--r--   0 u8sand    (1000) users      (984)     3830 2022-04-26 19:20:22.000000 appyter-0.19.8/js/extras/file-field/Storage.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      996 2022-04-26 19:20:22.000000 appyter-0.19.8/js/extras/file-field/URI.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     5978 2022-04-26 19:20:22.000000 appyter-0.19.8/js/extras/file-field/Upload.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      108 2022-04-26 19:20:22.000000 appyter-0.19.8/js/jsconfig.json
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.161417 appyter-0.19.8/js/lib/
--rw-r--r--   0 u8sand    (1000) users      (984)      448 2022-04-26 19:20:22.000000 appyter-0.19.8/js/lib/livereload.js
--rw-r--r--   0 u8sand    (1000) users      (984)     1152 2022-04-26 19:20:22.000000 appyter-0.19.8/js/lib/markdown_it.js
--rw-r--r--   0 u8sand    (1000) users      (984)      206 2022-04-26 19:20:22.000000 appyter-0.19.8/js/lib/socket.js
--rw-r--r--   0 u8sand    (1000) users      (984)      851 2022-04-26 19:20:22.000000 appyter-0.19.8/js/lib/socketio.js
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.161417 appyter-0.19.8/js/lib/stores/
--rw-r--r--   0 u8sand    (1000) users      (984)     2130 2022-04-26 19:20:22.000000 appyter-0.19.8/js/lib/stores/keycloak_auth_store.js
--rw-r--r--   0 u8sand    (1000) users      (984)     2330 2022-04-26 19:20:22.000000 appyter-0.19.8/js/lib/stores/url_hash_store.js
--rw-r--r--   0 u8sand    (1000) users      (984)     1463 2022-04-26 19:20:22.000000 appyter-0.19.8/js/lib/svelte_component_mounter.js
--rw-r--r--   0 u8sand    (1000) users      (984)       53 2022-04-26 19:20:22.000000 appyter-0.19.8/js/lib/webpack_public_path.js
--rw-r--r--   0 u8sand    (1000) users      (984)   338686 2022-04-28 16:42:16.000000 appyter-0.19.8/js/package-lock.json
--rw-r--r--   0 u8sand    (1000) users      (984)     1516 2022-04-28 16:42:16.000000 appyter-0.19.8/js/package.json
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.091417 appyter-0.19.8/js/profiles/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.091417 appyter-0.19.8/js/profiles/biojupies/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.161417 appyter-0.19.8/js/profiles/biojupies/css/
--rw-r--r--   0 u8sand    (1000) users      (984)    11720 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/biojupies/css/index.scss
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.161417 appyter-0.19.8/js/profiles/biojupies/js/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.161417 appyter-0.19.8/js/profiles/biojupies/js/fields/
--rw-r--r--   0 u8sand    (1000) users      (984)     1391 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/biojupies/js/fields/IntField.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     1442 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/biojupies/js/fields/SectionField.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     2016 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/biojupies/js/fields/StringField.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     1893 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/biojupies/js/fields/TextField.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     2144 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/biojupies/js/fields/TextListField.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     3009 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/biojupies/js/form.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)       88 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/biojupies/js/index.js
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.091417 appyter-0.19.8/js/profiles/bootstrap/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.161417 appyter-0.19.8/js/profiles/bootstrap/css/
--rw-r--r--   0 u8sand    (1000) users      (984)      147 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/bootstrap/css/index.scss
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.161417 appyter-0.19.8/js/profiles/bootstrap/js/
--rw-r--r--   0 u8sand    (1000) users      (984)       88 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/bootstrap/js/index.js
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.091417 appyter-0.19.8/js/profiles/default/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.161417 appyter-0.19.8/js/profiles/default/css/
--rw-r--r--   0 u8sand    (1000) users      (984)     1473 2022-04-26 19:30:58.000000 appyter-0.19.8/js/profiles/default/css/index.scss
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.161417 appyter-0.19.8/js/profiles/default/js/
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.164750 appyter-0.19.8/js/profiles/default/js/fields/
--rw-r--r--   0 u8sand    (1000) users      (984)     5208 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/default/js/fields/AutocompleteField.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     1420 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/default/js/fields/FileField.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     1611 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/default/js/fields/MultiCheckboxField.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      488 2022-05-11 14:44:24.000000 appyter-0.19.8/js/profiles/default/js/fields/TabField.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)     1830 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/default/js/fields/VariableField.svelte
--rw-r--r--   0 u8sand    (1000) users      (984)      555 2022-04-26 19:20:22.000000 appyter-0.19.8/js/profiles/default/js/index.js
--rw-r--r--   0 u8sand    (1000) users      (984)    10649 2022-04-28 16:42:16.000000 appyter-0.19.8/js/profiles/default/js/landing.svelte
-drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-05-11 16:16:24.164750 appyter-0.19.8/js/utils/
--rw-r--r--   0 u8sand    (1000) users      (984)      101 2021-05-03 14:23:28.000000 appyter-0.19.8/js/utils/any.js
--rw-r--r--   0 u8sand    (1000) users      (984)      273 2022-04-26 19:20:22.000000 appyter-0.19.8/js/utils/auth_headers.js
--rw-r--r--   0 u8sand    (1000) users      (984)      138 2021-05-03 14:23:28.000000 appyter-0.19.8/js/utils/collapse.js
--rw-r--r--   0 u8sand    (1000) users      (984)      136 2021-09-29 21:54:05.000000 appyter-0.19.8/js/utils/ensure_list.js
--rw-r--r--   0 u8sand    (1000) users      (984)      301 2021-09-29 21:54:05.000000 appyter-0.19.8/js/utils/get_require.js
--rw-r--r--   0 u8sand    (1000) users      (984)      126 2021-05-03 14:23:28.000000 appyter-0.19.8/js/utils/hash.js
--rw-r--r--   0 u8sand    (1000) users      (984)      281 2022-04-26 19:20:22.000000 appyter-0.19.8/js/utils/human_size.js
--rw-r--r--   0 u8sand    (1000) users      (984)       77 2022-04-26 19:20:22.000000 appyter-0.19.8/js/utils/null.js
--rw-r--r--   0 u8sand    (1000) users      (984)      183 2022-04-26 19:20:22.000000 appyter-0.19.8/js/utils/re_full.js
--rw-r--r--   0 u8sand    (1000) users      (984)      115 2022-04-26 19:20:22.000000 appyter-0.19.8/js/utils/silent-check-sso.html
--rw-r--r--   0 u8sand    (1000) users      (984)      156 2021-05-03 14:23:28.000000 appyter-0.19.8/js/utils/slugify.js
--rw-r--r--   0 u8sand    (1000) users      (984)      557 2022-04-26 19:20:22.000000 appyter-0.19.8/js/utils/url_for.js
--rw-r--r--   0 u8sand    (1000) users      (984)      495 2022-04-26 19:20:22.000000 appyter-0.19.8/js/utils/with_timeout.js
--rw-r--r--   0 u8sand    (1000) users      (984)     4407 2022-04-26 19:20:22.000000 appyter-0.19.8/js/webpack.config.js
--rw-r--r--   0 u8sand    (1000) users      (984)       73 2022-04-26 19:20:22.000000 appyter-0.19.8/requirements.production.txt
--rw-r--r--   0 u8sand    (1000) users      (984)      341 2022-04-26 19:20:22.000000 appyter-0.19.8/requirements.txt
--rw-r--r--   0 u8sand    (1000) users      (984)       38 2022-05-11 16:16:24.164750 appyter-0.19.8/setup.cfg
--rw-r--r--   0 u8sand    (1000) users      (984)     1131 2022-04-26 19:20:22.000000 appyter-0.19.8/setup.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.155834 appyter-0.19.9/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.019166 appyter-0.19.9/.github/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.039166 appyter-0.19.9/.github/workflows/
+-rw-r--r--   0 u8sand    (1000) users      (984)      661 2022-04-26 19:20:22.000000 appyter-0.19.9/.github/workflows/deploy-doc-to-ghpages.yml
+-rw-r--r--   0 u8sand    (1000) users      (984)       64 2022-04-26 19:20:22.000000 appyter-0.19.9/.gitignore
+-rw-r--r--   0 u8sand    (1000) users      (984)    20850 2021-09-29 21:54:05.000000 appyter-0.19.9/LICENSE
+-rw-r--r--   0 u8sand    (1000) users      (984)      243 2022-04-26 19:20:22.000000 appyter-0.19.9/MANIFEST.in
+-rw-r--r--   0 u8sand    (1000) users      (984)     6685 2022-06-02 17:14:48.155834 appyter-0.19.9/PKG-INFO
+-rw-r--r--   0 u8sand    (1000) users      (984)     5958 2022-04-26 19:20:22.000000 appyter-0.19.9/README.md
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.042499 appyter-0.19.9/appyter/
+-rw-r--r--   0 u8sand    (1000) users      (984)        6 2022-06-02 17:13:19.000000 appyter-0.19.9/appyter/VERSION
+-rw-r--r--   0 u8sand    (1000) users      (984)      276 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      393 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/__main__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1305 2022-05-31 21:19:00.000000 appyter-0.19.9/appyter/cli.py
+-rw-r--r--   0 u8sand    (1000) users      (984)    11535 2022-05-11 16:08:16.000000 appyter-0.19.9/appyter/context.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.045833 appyter-0.19.9/appyter/execspec/
+-rw-r--r--   0 u8sand    (1000) users      (984)      127 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/execspec/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      372 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/execspec/core.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.049166 appyter-0.19.9/appyter/execspec/implementations/
+-rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/execspec/implementations/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     4673 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/execspec/implementations/cavatica.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1719 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/execspec/implementations/dispatch.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2249 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/execspec/implementations/docker.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     4329 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/execspec/implementations/kube.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1381 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/execspec/implementations/local.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1138 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/execspec/implementations/subprocess.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     5448 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/execspec/implementations/wes.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1825 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/execspec/registry.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      792 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/execspec/spec.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.055833 appyter-0.19.9/appyter/ext/
+-rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/ext/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1040 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/aiohttp.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.055833 appyter-0.19.9/appyter/ext/asyncio/
+-rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-04-25 15:13:20.000000 appyter-0.19.9/appyter/ext/asyncio/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2714 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/asyncio/event_emitter.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     3429 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/ext/asyncio/event_loop.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     5306 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/asyncio/helpers.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1484 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/asyncio/subprocess.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     6656 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/asyncio/test_helpers.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      741 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/asyncio/test_subprocess.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      817 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/asyncio/try_n_times.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.055833 appyter-0.19.9/appyter/ext/click/
+-rw-r--r--   0 u8sand    (1000) users      (984)     1238 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/ext/click/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      972 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/contextlib.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2260 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/cryptography.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1935 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/ext/dict.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      868 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/drs.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2138 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/emitter.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      204 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/exceptions.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2341 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/flask.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.062500 appyter-0.19.9/appyter/ext/fsspec/
+-rw-r--r--   0 u8sand    (1000) users      (984)      575 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     9573 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/chroot.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     3450 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/core.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     3569 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/drs.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1799 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/fuse.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     6090 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/mapperfs.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     7526 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/overlayfs.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1933 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/s3fs.py
+-rw-r--r--   0 u8sand    (1000) users      (984)    18894 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/sbfs.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1504 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/singleton.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.065833 appyter-0.19.9/appyter/ext/fsspec/spec/
+-rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/spec/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1453 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/spec/composable.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      589 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/spec/mountable.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     4707 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/spec/sync_async.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      556 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/storage.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1962 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/test_chroot.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     3578 2022-05-11 16:08:16.000000 appyter-0.19.9/appyter/ext/fsspec/test_drs.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1794 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/test_fuse.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1911 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/test_fuseless_mount.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1054 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/test_mapperfs.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2154 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/test_overlayfs.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2599 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/test_pathmap.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1619 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/test_sbfs.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      628 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/fsspec/util.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     8759 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/ext/fsspec/writecache.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      526 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/functools.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      657 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/hashlib.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      914 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/importlib.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      427 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/io.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      581 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/itertools.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      378 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/json.py
+-rw-r--r--   0 u8sand    (1000) users      (984)       57 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/multiprocessing.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.065833 appyter-0.19.9/appyter/ext/nbclient/
+-rw-r--r--   0 u8sand    (1000) users      (984)     5396 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/ext/nbclient/__init__.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.065833 appyter-0.19.9/appyter/ext/pathlib/
+-rw-r--r--   0 u8sand    (1000) users      (984)      195 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/ext/pathlib/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      434 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/pathlib/assertions.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      932 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/pathlib/chroot.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1381 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/pytest.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      200 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/re.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.065833 appyter-0.19.9/appyter/ext/socketio/
+-rw-r--r--   0 u8sand    (1000) users      (984)      103 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/ext/socketio/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1152 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/ext/socketio/chunked_emit.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1121 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/ext/socketio/client.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      502 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/socketio/forwarding.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1567 2022-05-31 17:09:46.000000 appyter-0.19.9/appyter/ext/socketio/priority_queued_emit.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1184 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/ext/socketio/server.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      238 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/subprocess.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      830 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/tempfile.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     9328 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/urllib.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      284 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/ext/uuid.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.069166 appyter-0.19.9/appyter/ext/watchgod/
+-rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/ext/watchgod/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1010 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/ext/watchgod/watcher.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.069166 appyter-0.19.9/appyter/extras/
+-rw-r--r--   0 u8sand    (1000) users      (984)      667 2022-04-28 16:42:16.000000 appyter-0.19.9/appyter/extras/__init__.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.069166 appyter-0.19.9/appyter/extras/catalog_integration/
+-rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/extras/catalog_integration/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1335 2022-05-11 16:08:16.000000 appyter-0.19.9/appyter/extras/catalog_integration/executor.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      721 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/extras/catalog_integration/notebooks.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1973 2022-05-11 15:50:01.000000 appyter-0.19.9/appyter/extras/catalog_integration/request.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      896 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/extras/catalog_integration/storage.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1034 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/extras/catalog_integration/uploads.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      506 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/extras/catalog_integration/user_config.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2902 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/extras/catalog_integration/userfs.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     8490 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/fields.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.072500 appyter-0.19.9/appyter/helpers/
+-rw-r--r--   0 u8sand    (1000) users      (984)      180 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/helpers/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     4215 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/helpers/commandify.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.072500 appyter-0.19.9/appyter/helpers/cookiecutter/
+-rw-r--r--   0 u8sand    (1000) users      (984)      391 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/helpers/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.072500 appyter-0.19.9/appyter/helpers/cookiecutter/{{ cookiecutter.project_slug }}/
+-rw-r--r--   0 u8sand    (1000) users      (984)      430 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/helpers/cookiecutter/{{ cookiecutter.project_slug }}/README.md
+-rw-r--r--   0 u8sand    (1000) users      (984)      719 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/helpers/cookiecutter/{{ cookiecutter.project_slug }}/appyter.json
+-rw-r--r--   0 u8sand    (1000) users      (984)      192 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/helpers/cookiecutter/{{ cookiecutter.project_slug }}/requirements.txt
+-rw-r--r--   0 u8sand    (1000) users      (984)     1746 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/helpers/cookiecutter/{{ cookiecutter.project_slug }}/{{ cookiecutter.project_slug }}.ipynb
+-rw-r--r--   0 u8sand    (1000) users      (984)      829 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/helpers/dockerize.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2045 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/helpers/fetch_and_serve.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1696 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/helpers/init.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      820 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/helpers/nbclean.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2223 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/helpers/serve.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     4661 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/magic.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.072500 appyter-0.19.9/appyter/orchestration/
+-rw-r--r--   0 u8sand    (1000) users      (984)      178 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/orchestration/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      221 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/orchestration/cli.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.072500 appyter-0.19.9/appyter/orchestration/dispatcher/
+-rw-r--r--   0 u8sand    (1000) users      (984)     2638 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/orchestration/dispatcher/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     3118 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/orchestration/dispatcher/core.py
+-rw-r--r--   0 u8sand    (1000) users      (984)       91 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/orchestration/dispatcher/socketio.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.075833 appyter-0.19.9/appyter/parse/
+-rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/parse/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      594 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/parse/nb.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1257 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/parse/nbtemplate.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.075833 appyter-0.19.9/appyter/profiles/
+-rw-r--r--   0 u8sand    (1000) users      (984)      817 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/__init__.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.075833 appyter-0.19.9/appyter/profiles/biojupies/
+-rw-r--r--   0 u8sand    (1000) users      (984)       72 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/biojupies/__init__.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.075833 appyter-0.19.9/appyter/profiles/biojupies/templates/
+-rw-r--r--   0 u8sand    (1000) users      (984)       33 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/biojupies/templates/base.j2
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.075833 appyter-0.19.9/appyter/profiles/biojupies/templates/biojupies/
+-rw-r--r--   0 u8sand    (1000) users      (984)      860 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/biojupies/templates/biojupies/base.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      290 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/biojupies/templates/biojupies/form.j2
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.079166 appyter-0.19.9/appyter/profiles/biojupies/templates/fields/
+-rw-r--r--   0 u8sand    (1000) users      (984)     1023 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/profiles/biojupies/templates/fields/BoolField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      630 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/biojupies/templates/fields/ChoiceField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      605 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/biojupies/templates/fields/FloatField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/biojupies/templates/fields/IntField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      656 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/biojupies/templates/fields/MultiChoiceField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/biojupies/templates/fields/SectionField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/biojupies/templates/fields/StringField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/biojupies/templates/fields/TextField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/biojupies/templates/fields/TextListField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       33 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/biojupies/templates/form.j2
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.079166 appyter-0.19.9/appyter/profiles/bootstrap/
+-rw-r--r--   0 u8sand    (1000) users      (984)       61 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/bootstrap/__init__.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.022499 appyter-0.19.9/appyter/profiles/bootstrap/static/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.079166 appyter-0.19.9/appyter/profiles/bootstrap/static/css/
+-rw-r--r--   0 u8sand    (1000) users      (984)   161994 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/bootstrap/static/css/bootstrap.css
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.022499 appyter-0.19.9/appyter/profiles/bootstrap/static/js/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.025833 appyter-0.19.9/appyter/profiles/bootstrap/static/js/lib/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.079166 appyter-0.19.9/appyter/profiles/bootstrap/static/js/lib/bootstrap/
+-rw-r--r--   0 u8sand    (1000) users      (984)    84378 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/bootstrap/static/js/lib/bootstrap/bootstrap.bundle.min.js
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.079166 appyter-0.19.9/appyter/profiles/bootstrap/static/js/lib/select2/
+-rw-r--r--   0 u8sand    (1000) users      (984)    70851 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/bootstrap/static/js/lib/select2/select2.min.js
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.079166 appyter-0.19.9/appyter/profiles/bootstrap/templates/
+-rw-r--r--   0 u8sand    (1000) users      (984)       33 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/bootstrap/templates/base.j2
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.079166 appyter-0.19.9/appyter/profiles/bootstrap/templates/bootstrap/
+-rw-r--r--   0 u8sand    (1000) users      (984)      649 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/bootstrap/templates/bootstrap/base.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      341 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/bootstrap/templates/bootstrap/form.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       33 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/bootstrap/templates/form.j2
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.079166 appyter-0.19.9/appyter/profiles/default/
+-rw-r--r--   0 u8sand    (1000) users      (984)      243 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/__init__.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.082500 appyter-0.19.9/appyter/profiles/default/blueprints/
+-rw-r--r--   0 u8sand    (1000) users      (984)     2760 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/blueprints/StorageFileField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/blueprints/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1448 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/blueprints/locate.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.085833 appyter-0.19.9/appyter/profiles/default/fields/
+-rw-r--r--   0 u8sand    (1000) users      (984)     2272 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/fields/AutocompleteField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1967 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/profiles/default/fields/BoolField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1374 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/fields/ChoiceField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      901 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/fields/DescriptionField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     4869 2022-04-28 16:45:18.000000 appyter-0.19.9/appyter/profiles/default/fields/FileField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1515 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/fields/FloatField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2287 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/fields/IntField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     3658 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/fields/MultiCheckboxField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     3420 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/fields/MultiChoiceField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1177 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/fields/SectionField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2102 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/fields/StringField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1611 2022-05-11 14:44:24.000000 appyter-0.19.9/appyter/profiles/default/fields/TabField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2326 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/fields/TextField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     4329 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/fields/TextListField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     3944 2022-05-11 14:44:24.000000 appyter-0.19.9/appyter/profiles/default/fields/VariableField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      279 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/fields/__init__.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.085833 appyter-0.19.9/appyter/profiles/default/filters/
+-rw-r--r--   0 u8sand    (1000) users      (984)      105 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/filters/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)       75 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/filters/atob.py
+-rw-r--r--   0 u8sand    (1000) users      (984)       75 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/filters/btoa.py
+-rw-r--r--   0 u8sand    (1000) users      (984)       63 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/filters/fmt.py
+-rw-r--r--   0 u8sand    (1000) users      (984)       51 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/filters/join_routes.py
+-rw-r--r--   0 u8sand    (1000) users      (984)       52 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/filters/jsonify.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      179 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/filters/pyeval.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1080 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/filters/url_for.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.089166 appyter-0.19.9/appyter/profiles/default/templates/
+-rw-r--r--   0 u8sand    (1000) users      (984)       31 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/base.j2
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.089166 appyter-0.19.9/appyter/profiles/default/templates/default/
+-rw-r--r--   0 u8sand    (1000) users      (984)     1412 2022-05-11 16:08:16.000000 appyter-0.19.9/appyter/profiles/default/templates/default/base.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      483 2022-03-26 22:16:07.000000 appyter-0.19.9/appyter/profiles/default/templates/default/form.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      417 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/templates/default/landing.j2
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.092500 appyter-0.19.9/appyter/profiles/default/templates/fields/
+-rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/AutocompleteField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      328 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/BoolField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      462 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/ChoiceField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      149 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/DescriptionField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/FileField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      371 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/FloatField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      964 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/IntField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/MultiCheckboxField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      479 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/MultiChoiceField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       16 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/SectionField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      353 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/StringField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/TabField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      411 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/TextField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      466 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/TextListField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       41 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fields/VariableField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       31 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/form.j2
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.092500 appyter-0.19.9/appyter/profiles/default/templates/fragments/
+-rw-r--r--   0 u8sand    (1000) users      (984)   221111 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fragments/jupyter.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      107 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fragments/loader.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      203 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/templates/fragments/svelte-field.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       34 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/profiles/default/templates/landing.j2
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.092500 appyter-0.19.9/appyter/profiles/default/templates/production/
+-rw-r--r--   0 u8sand    (1000) users      (984)     2574 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/templates/production/Dockerfile.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)     6540 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/profiles/default/templates/production/nginx.conf.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)     1221 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/profiles/default/templates/production/supervisord.conf.j2
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.095833 appyter-0.19.9/appyter/render/
+-rw-r--r--   0 u8sand    (1000) users      (984)      218 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/__init__.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.095833 appyter-0.19.9/appyter/render/flask_app/
+-rw-r--r--   0 u8sand    (1000) users      (984)     7285 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/flask_app/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     3858 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/flask_app/constants.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2049 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/flask_app/core.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     4327 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/render/flask_app/development.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2614 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/flask_app/drs.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     3097 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/flask_app/execution.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2214 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/flask_app/export.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      386 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/render/flask_app/livereload.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     5024 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/flask_app/prepare.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2167 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/flask_app/production.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     2410 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/flask_app/room_manager.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1029 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/flask_app/socketio.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     3381 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/flask_app/static.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     4823 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/flask_app/upload.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      355 2022-03-25 22:22:22.000000 appyter-0.19.9/appyter/render/form.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     3612 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/nbconstruct.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     7300 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/nbexecute.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.099166 appyter-0.19.9/appyter/render/nbinspect/
+-rw-r--r--   0 u8sand    (1000) users      (984)      187 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/nbinspect/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      212 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/nbinspect/cli.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     4173 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/render/nbinspect/cwl.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1707 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/nbinspect/jsonschema.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1392 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/nbinspect/nbtemplate_json.py
+-rw-r--r--   0 u8sand    (1000) users      (984)    12378 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/render/nbinspect/openapi.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.099166 appyter-0.19.9/appyter/static/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.029166 appyter-0.19.9/appyter/static/profiles/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.029166 appyter-0.19.9/appyter/static/profiles/biojupies/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.099166 appyter-0.19.9/appyter/static/profiles/biojupies/css/
+-rw-r--r--   0 u8sand    (1000) users      (984)    59305 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/css/fontawesome.css
+-rw-r--r--   0 u8sand    (1000) users      (984)   160873 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/biojupies/css/index.css
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.099166 appyter-0.19.9/appyter/static/profiles/biojupies/js/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.102500 appyter-0.19.9/appyter/static/profiles/biojupies/js/fields/
+-rw-r--r--   0 u8sand    (1000) users      (984)     7547 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/static/profiles/biojupies/js/fields/IntField.js
+-rw-r--r--   0 u8sand    (1000) users      (984)    13813 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/biojupies/js/fields/SectionField.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     9133 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/biojupies/js/fields/StringField.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     8532 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/biojupies/js/fields/TextField.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     9326 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/biojupies/js/fields/TextListField.js
+-rw-r--r--   0 u8sand    (1000) users      (984)    29876 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/static/profiles/biojupies/js/form.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     3038 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/biojupies/js/index.js
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.102500 appyter-0.19.9/appyter/static/profiles/biojupies/js/lib/
+-rw-r--r--   0 u8sand    (1000) users      (984)    83862 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/biojupies/js/lib/bootstrap.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      237 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/biojupies/js/lib/bootstrap.js.LICENSE.txt
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.112500 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/
+-rw-r--r--   0 u8sand    (1000) users      (984)   134294 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-brands-400.eot
+-rw-r--r--   0 u8sand    (1000) users      (984)   747927 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-brands-400.svg
+-rw-r--r--   0 u8sand    (1000) users      (984)   133988 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 u8sand    (1000) users      (984)    89988 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-brands-400.woff
+-rw-r--r--   0 u8sand    (1000) users      (984)    76736 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 u8sand    (1000) users      (984)    34034 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-regular-400.eot
+-rw-r--r--   0 u8sand    (1000) users      (984)   144714 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-regular-400.svg
+-rw-r--r--   0 u8sand    (1000) users      (984)    33736 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 u8sand    (1000) users      (984)    16276 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-regular-400.woff
+-rw-r--r--   0 u8sand    (1000) users      (984)    13224 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 u8sand    (1000) users      (984)   203030 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-solid-900.eot
+-rw-r--r--   0 u8sand    (1000) users      (984)   918991 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-solid-900.svg
+-rw-r--r--   0 u8sand    (1000) users      (984)   202744 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 u8sand    (1000) users      (984)   101648 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-solid-900.woff
+-rw-r--r--   0 u8sand    (1000) users      (984)    78268 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.029166 appyter-0.19.9/appyter/static/profiles/bootstrap/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.112500 appyter-0.19.9/appyter/static/profiles/bootstrap/css/
+-rw-r--r--   0 u8sand    (1000) users      (984)   167619 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/bootstrap/css/index.css
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.112500 appyter-0.19.9/appyter/static/profiles/bootstrap/js/
+-rw-r--r--   0 u8sand    (1000) users      (984)     3038 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/bootstrap/js/index.js
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.029166 appyter-0.19.9/appyter/static/profiles/default/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.112500 appyter-0.19.9/appyter/static/profiles/default/css/
+-rw-r--r--   0 u8sand    (1000) users      (984)     2443 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/css/index.css
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.115833 appyter-0.19.9/appyter/static/profiles/default/js/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.119166 appyter-0.19.9/appyter/static/profiles/default/js/chunks/
+-rw-r--r--   0 u8sand    (1000) users      (984)    35216 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/229.js
+-rw-r--r--   0 u8sand    (1000) users      (984)    19860 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/246.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      254 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/284.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     6501 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/29.js
+-rw-r--r--   0 u8sand    (1000) users      (984)    28632 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/316.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     2356 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/322.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      741 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/494.js
+-rw-r--r--   0 u8sand    (1000) users      (984)    21282 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/58.js
+-rw-r--r--   0 u8sand    (1000) users      (984)    36325 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/671.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      187 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/671.js.LICENSE.txt
+-rw-r--r--   0 u8sand    (1000) users      (984)   147776 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/680.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      447 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/704.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     1435 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/755.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      832 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/798.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     4127 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/826.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     7405 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/849.js
+-rw-r--r--   0 u8sand    (1000) users      (984)    14531 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/static/profiles/default/js/chunks/977.js
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.119166 appyter-0.19.9/appyter/static/profiles/default/js/fields/
+-rw-r--r--   0 u8sand    (1000) users      (984)    13749 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/static/profiles/default/js/fields/AutocompleteField.js
+-rw-r--r--   0 u8sand    (1000) users      (984)    20130 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/static/profiles/default/js/fields/FileField.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     8075 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/fields/MultiCheckboxField.js
+-rw-r--r--   0 u8sand    (1000) users      (984)    13458 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/fields/TabField.js
+-rw-r--r--   0 u8sand    (1000) users      (984)    11928 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/fields/VariableField.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     2957 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/index.js
+-rw-r--r--   0 u8sand    (1000) users      (984)    29552 2022-06-02 17:13:11.000000 appyter-0.19.9/appyter/static/profiles/default/js/landing.js
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.122500 appyter-0.19.9/appyter/static/profiles/default/js/lib/
+-rw-r--r--   0 u8sand    (1000) users      (984)    89521 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/lib/jquery.js
+-rw-r--r--   0 u8sand    (1000) users      (984)       89 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/lib/jquery.js.LICENSE.txt
+-rw-r--r--   0 u8sand    (1000) users      (984)    17656 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/lib/require.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      202 2022-06-02 16:08:41.000000 appyter-0.19.9/appyter/static/profiles/default/js/lib/require.js.LICENSE.txt
+-rw-r--r--   0 u8sand    (1000) users      (984)      115 2022-04-26 19:20:22.000000 appyter-0.19.9/appyter/static/silent-check-sso.html
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.045833 appyter-0.19.9/appyter.egg-info/
+-rw-r--r--   0 u8sand    (1000) users      (984)     6685 2022-06-02 17:14:46.000000 appyter-0.19.9/appyter.egg-info/PKG-INFO
+-rw-r--r--   0 u8sand    (1000) users      (984)    16249 2022-06-02 17:14:47.000000 appyter-0.19.9/appyter.egg-info/SOURCES.txt
+-rw-r--r--   0 u8sand    (1000) users      (984)        1 2022-06-02 17:14:46.000000 appyter-0.19.9/appyter.egg-info/dependency_links.txt
+-rw-r--r--   0 u8sand    (1000) users      (984)       50 2022-06-02 17:14:47.000000 appyter-0.19.9/appyter.egg-info/entry_points.txt
+-rw-r--r--   0 u8sand    (1000) users      (984)      459 2022-06-02 17:14:47.000000 appyter-0.19.9/appyter.egg-info/requires.txt
+-rw-r--r--   0 u8sand    (1000) users      (984)        8 2022-06-02 17:14:47.000000 appyter-0.19.9/appyter.egg-info/top_level.txt
+-rw-r--r--   0 u8sand    (1000) users      (984)       17 2021-05-03 14:23:28.000000 appyter-0.19.9/deps.production.txt
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.122500 appyter-0.19.9/docs/
+-rw-r--r--   0 u8sand    (1000) users      (984)       29 2021-05-03 14:23:28.000000 appyter-0.19.9/docs/.gitignore
+-rw-r--r--   0 u8sand    (1000) users      (984)      800 2021-05-03 14:23:28.000000 appyter-0.19.9/docs/Makefile
+-rw-r--r--   0 u8sand    (1000) users      (984)      799 2021-05-03 14:23:28.000000 appyter-0.19.9/docs/make.bat
+-rw-r--r--   0 u8sand    (1000) users      (984)       46 2022-04-26 19:20:22.000000 appyter-0.19.9/docs/requirements.txt
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.122500 appyter-0.19.9/docs/source/
+-rw-r--r--   0 u8sand    (1000) users      (984)       13 2021-05-03 14:23:28.000000 appyter-0.19.9/docs/source/.gitignore
+-rw-r--r--   0 u8sand    (1000) users      (984)     3539 2022-04-26 19:20:22.000000 appyter-0.19.9/docs/source/conf.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      507 2021-05-03 14:23:28.000000 appyter-0.19.9/docs/source/index.rst
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.125833 appyter-0.19.9/example/
+-rw-r--r--   0 u8sand    (1000) users      (984)       10 2022-03-16 21:31:07.000000 appyter-0.19.9/example/.dockerignore
+-rw-r--r--   0 u8sand    (1000) users      (984)     1501 2022-04-26 19:20:22.000000 appyter-0.19.9/example/Dockerfile
+-rw-r--r--   0 u8sand    (1000) users      (984)     1543 2022-04-26 19:20:22.000000 appyter-0.19.9/example/README.md
+-rw-r--r--   0 u8sand    (1000) users      (984)     3792 2022-04-26 19:20:22.000000 appyter-0.19.9/example/appyter.cwl
+-rw-r--r--   0 u8sand    (1000) users      (984)      651 2022-04-26 19:20:22.000000 appyter-0.19.9/example/appyter.json
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.125833 appyter-0.19.9/example/blueprints/
+-rw-r--r--   0 u8sand    (1000) users      (984)        0 2022-02-22 22:19:08.000000 appyter-0.19.9/example/blueprints/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      153 2022-02-22 22:19:08.000000 appyter-0.19.9/example/blueprints/testblueprint.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     1392 2022-04-26 19:20:22.000000 appyter-0.19.9/example/blueprints/testdash.py
+-rw-r--r--   0 u8sand    (1000) users      (984)     3603 2022-06-02 17:13:11.000000 appyter-0.19.9/example/droptest.ipynb
+-rw-r--r--   0 u8sand    (1000) users      (984)     7973 2022-04-26 19:20:22.000000 appyter-0.19.9/example/example.ipynb
+-rw-r--r--   0 u8sand    (1000) users      (984)      854 2022-04-26 19:20:22.000000 appyter-0.19.9/example/example_test.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      468 2022-04-26 19:20:22.000000 appyter-0.19.9/example/example_test.sh
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.125833 appyter-0.19.9/example/fields/
+-rw-r--r--   0 u8sand    (1000) users      (984)      269 2021-05-03 14:23:28.000000 appyter-0.19.9/example/fields/EmailField.py
+-rw-r--r--   0 u8sand    (1000) users      (984)        0 2021-05-03 14:23:28.000000 appyter-0.19.9/example/fields/__init__.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.129167 appyter-0.19.9/example/filters/
+-rw-r--r--   0 u8sand    (1000) users      (984)        0 2021-05-03 14:23:28.000000 appyter-0.19.9/example/filters/__init__.py
+-rw-r--r--   0 u8sand    (1000) users      (984)      257 2021-05-03 14:23:28.000000 appyter-0.19.9/example/filters/do_op.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.129167 appyter-0.19.9/example/production/
+-rw-r--r--   0 u8sand    (1000) users      (984)       72 2021-05-03 14:23:28.000000 appyter-0.19.9/example/production/.env.example
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.129167 appyter-0.19.9/example/production/appyter/
+-rw-r--r--   0 u8sand    (1000) users      (984)      802 2021-05-03 14:23:28.000000 appyter-0.19.9/example/production/appyter/Dockerfile
+-rw-r--r--   0 u8sand    (1000) users      (984)     1246 2022-04-26 19:20:22.000000 appyter-0.19.9/example/production/docker-compose.yml
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.129167 appyter-0.19.9/example/production/s3/
+-rw-r--r--   0 u8sand    (1000) users      (984)      222 2021-05-03 14:23:28.000000 appyter-0.19.9/example/production/s3/Dockerfile
+-rw-r--r--   0 u8sand    (1000) users      (984)      429 2021-05-03 14:23:28.000000 appyter-0.19.9/example/production/s3/entrypoint.sh
+-rw-r--r--   0 u8sand    (1000) users      (984)       17 2021-05-03 14:23:28.000000 appyter-0.19.9/example/requirements.txt
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.129167 appyter-0.19.9/example/static/
+-rw-r--r--   0 u8sand    (1000) users      (984)     7110 2021-05-03 14:23:28.000000 appyter-0.19.9/example/static/GitHub-Mark.png
+-rw-r--r--   0 u8sand    (1000) users      (984)       19 2021-05-03 14:23:28.000000 appyter-0.19.9/example/static/test.js
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.129167 appyter-0.19.9/example/templates/
+-rw-r--r--   0 u8sand    (1000) users      (984)      424 2022-04-26 19:20:22.000000 appyter-0.19.9/example/templates/base.j2
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.129167 appyter-0.19.9/example/templates/fields/
+-rw-r--r--   0 u8sand    (1000) users      (984)      354 2021-05-03 14:23:28.000000 appyter-0.19.9/example/templates/fields/EmailField.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)      352 2021-05-03 14:23:28.000000 appyter-0.19.9/example/templates/form.j2
+-rw-r--r--   0 u8sand    (1000) users      (984)       42 2021-05-03 14:23:28.000000 appyter-0.19.9/example/test.py
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.132500 appyter-0.19.9/js/
+-rw-r--r--   0 u8sand    (1000) users      (984)       12 2021-05-03 14:23:28.000000 appyter-0.19.9/js/.gitignore
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.135833 appyter-0.19.9/js/components/
+-rw-r--r--   0 u8sand    (1000) users      (984)      187 2021-05-03 14:23:28.000000 appyter-0.19.9/js/components/Ansi.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      691 2022-05-31 21:49:23.000000 appyter-0.19.9/js/components/HTML.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      558 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/Lazy.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      178 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/Loader.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      159 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/Markdown.svelte
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.135833 appyter-0.19.9/js/components/app/
+-rw-r--r--   0 u8sand    (1000) users      (984)      129 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/app/Error.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     1137 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/app/SSRField.svelte
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.135833 appyter-0.19.9/js/components/fields/
+-rw-r--r--   0 u8sand    (1000) users      (984)      142 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/fields/DescriptionField.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     1166 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/fields/SectionField.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     2022 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/fields/StringField.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     1117 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/fields/TabField.svelte
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.139167 appyter-0.19.9/js/components/jupyter/
+-rw-r--r--   0 u8sand    (1000) users      (984)      118 2021-05-03 14:23:28.000000 appyter-0.19.9/js/components/jupyter/Cell.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)       68 2021-05-03 14:23:28.000000 appyter-0.19.9/js/components/jupyter/Cells.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)       42 2021-05-03 14:23:28.000000 appyter-0.19.9/js/components/jupyter/Input.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     2071 2022-04-26 19:25:20.000000 appyter-0.19.9/js/components/jupyter/Notebook.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      860 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/Output.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     1514 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/OutputMimetype.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     1773 2022-06-02 17:13:11.000000 appyter-0.19.9/js/components/jupyter/Outputs.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      578 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/Prompt.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      309 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/Source.svelte
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.142500 appyter-0.19.9/js/components/jupyter/output_mimetype/
+-rw-r--r--   0 u8sand    (1000) users      (984)      207 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/output_mimetype/ApplicationJavascript.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      220 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/output_mimetype/ImagePng.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      185 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/output_mimetype/ImageSvgXml.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      200 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/output_mimetype/TextHtml.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      211 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/output_mimetype/TextMarkdown.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      280 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/output_mimetype/TextPlain.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      802 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/output_mimetype/index.js
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.142500 appyter-0.19.9/js/components/jupyter/output_type/
+-rw-r--r--   0 u8sand    (1000) users      (984)      186 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/output_type/OutputDisplayData.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      585 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/output_type/OutputError.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      188 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/output_type/OutputExecuteResult.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      233 2022-04-26 19:20:22.000000 appyter-0.19.9/js/components/jupyter/output_type/OutputStream.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      392 2021-09-29 21:54:05.000000 appyter-0.19.9/js/components/jupyter/output_type/index.js
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.035833 appyter-0.19.9/js/extras/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.145833 appyter-0.19.9/js/extras/catalog-integration/
+-rw-r--r--   0 u8sand    (1000) users      (984)     4499 2022-05-11 16:08:16.000000 appyter-0.19.9/js/extras/catalog-integration/LaunchSettings.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     1517 2022-04-26 19:20:22.000000 appyter-0.19.9/js/extras/catalog-integration/LocateFileField.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      940 2022-04-26 19:20:22.000000 appyter-0.19.9/js/extras/catalog-integration/TableOfContents.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      678 2022-04-26 19:20:22.000000 appyter-0.19.9/js/extras/catalog-integration/pagehit.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     1047 2022-04-26 19:20:22.000000 appyter-0.19.9/js/extras/catalog-integration/report_error.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     1450 2022-04-26 19:20:22.000000 appyter-0.19.9/js/extras/catalog-integration/toc.js
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.145833 appyter-0.19.9/js/extras/file-field/
+-rw-r--r--   0 u8sand    (1000) users      (984)     3830 2022-04-26 19:20:22.000000 appyter-0.19.9/js/extras/file-field/Storage.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      996 2022-04-26 19:20:22.000000 appyter-0.19.9/js/extras/file-field/URI.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     5978 2022-04-26 19:20:22.000000 appyter-0.19.9/js/extras/file-field/Upload.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      108 2022-04-26 19:20:22.000000 appyter-0.19.9/js/jsconfig.json
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.145833 appyter-0.19.9/js/lib/
+-rw-r--r--   0 u8sand    (1000) users      (984)      448 2022-04-26 19:20:22.000000 appyter-0.19.9/js/lib/livereload.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     1152 2022-04-26 19:20:22.000000 appyter-0.19.9/js/lib/markdown_it.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      206 2022-04-26 19:20:22.000000 appyter-0.19.9/js/lib/socket.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      851 2022-04-26 19:20:22.000000 appyter-0.19.9/js/lib/socketio.js
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.145833 appyter-0.19.9/js/lib/stores/
+-rw-r--r--   0 u8sand    (1000) users      (984)     2130 2022-04-26 19:20:22.000000 appyter-0.19.9/js/lib/stores/keycloak_auth_store.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     2412 2022-06-02 17:13:11.000000 appyter-0.19.9/js/lib/stores/url_hash_store.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     1463 2022-04-26 19:20:22.000000 appyter-0.19.9/js/lib/svelte_component_mounter.js
+-rw-r--r--   0 u8sand    (1000) users      (984)       53 2022-04-26 19:20:22.000000 appyter-0.19.9/js/lib/webpack_public_path.js
+-rw-r--r--   0 u8sand    (1000) users      (984)   338686 2022-04-28 16:42:16.000000 appyter-0.19.9/js/package-lock.json
+-rw-r--r--   0 u8sand    (1000) users      (984)     1516 2022-04-28 16:42:16.000000 appyter-0.19.9/js/package.json
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.035833 appyter-0.19.9/js/profiles/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.035833 appyter-0.19.9/js/profiles/biojupies/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.145833 appyter-0.19.9/js/profiles/biojupies/css/
+-rw-r--r--   0 u8sand    (1000) users      (984)    11720 2022-04-26 19:20:22.000000 appyter-0.19.9/js/profiles/biojupies/css/index.scss
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.149167 appyter-0.19.9/js/profiles/biojupies/js/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.149167 appyter-0.19.9/js/profiles/biojupies/js/fields/
+-rw-r--r--   0 u8sand    (1000) users      (984)     1393 2022-06-02 17:13:11.000000 appyter-0.19.9/js/profiles/biojupies/js/fields/IntField.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     1442 2022-04-26 19:20:22.000000 appyter-0.19.9/js/profiles/biojupies/js/fields/SectionField.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     2016 2022-04-26 19:20:22.000000 appyter-0.19.9/js/profiles/biojupies/js/fields/StringField.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     1893 2022-04-26 19:20:22.000000 appyter-0.19.9/js/profiles/biojupies/js/fields/TextField.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     2144 2022-04-26 19:20:22.000000 appyter-0.19.9/js/profiles/biojupies/js/fields/TextListField.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     3955 2022-06-02 17:13:11.000000 appyter-0.19.9/js/profiles/biojupies/js/form.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)       88 2022-04-26 19:20:22.000000 appyter-0.19.9/js/profiles/biojupies/js/index.js
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.035833 appyter-0.19.9/js/profiles/bootstrap/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.149167 appyter-0.19.9/js/profiles/bootstrap/css/
+-rw-r--r--   0 u8sand    (1000) users      (984)      147 2022-04-26 19:20:22.000000 appyter-0.19.9/js/profiles/bootstrap/css/index.scss
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.149167 appyter-0.19.9/js/profiles/bootstrap/js/
+-rw-r--r--   0 u8sand    (1000) users      (984)       88 2022-04-26 19:20:22.000000 appyter-0.19.9/js/profiles/bootstrap/js/index.js
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.039166 appyter-0.19.9/js/profiles/default/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.149167 appyter-0.19.9/js/profiles/default/css/
+-rw-r--r--   0 u8sand    (1000) users      (984)     1473 2022-04-26 19:30:58.000000 appyter-0.19.9/js/profiles/default/css/index.scss
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.149167 appyter-0.19.9/js/profiles/default/js/
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.152500 appyter-0.19.9/js/profiles/default/js/fields/
+-rw-r--r--   0 u8sand    (1000) users      (984)     5275 2022-06-02 17:13:11.000000 appyter-0.19.9/js/profiles/default/js/fields/AutocompleteField.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     1425 2022-06-02 17:13:11.000000 appyter-0.19.9/js/profiles/default/js/fields/FileField.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     1611 2022-04-26 19:20:22.000000 appyter-0.19.9/js/profiles/default/js/fields/MultiCheckboxField.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      488 2022-05-11 14:44:24.000000 appyter-0.19.9/js/profiles/default/js/fields/TabField.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)     1830 2022-04-26 19:20:22.000000 appyter-0.19.9/js/profiles/default/js/fields/VariableField.svelte
+-rw-r--r--   0 u8sand    (1000) users      (984)      555 2022-04-26 19:20:22.000000 appyter-0.19.9/js/profiles/default/js/index.js
+-rw-r--r--   0 u8sand    (1000) users      (984)    10649 2022-05-31 21:16:47.000000 appyter-0.19.9/js/profiles/default/js/landing.svelte
+drwxr-xr-x   0 u8sand    (1000) users      (984)        0 2022-06-02 17:14:48.155834 appyter-0.19.9/js/utils/
+-rw-r--r--   0 u8sand    (1000) users      (984)      101 2021-05-03 14:23:28.000000 appyter-0.19.9/js/utils/any.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      273 2022-04-26 19:20:22.000000 appyter-0.19.9/js/utils/auth_headers.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      138 2021-05-03 14:23:28.000000 appyter-0.19.9/js/utils/collapse.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      136 2021-09-29 21:54:05.000000 appyter-0.19.9/js/utils/ensure_list.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      301 2021-09-29 21:54:05.000000 appyter-0.19.9/js/utils/get_require.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      126 2021-05-03 14:23:28.000000 appyter-0.19.9/js/utils/hash.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      281 2022-04-26 19:20:22.000000 appyter-0.19.9/js/utils/human_size.js
+-rw-r--r--   0 u8sand    (1000) users      (984)       77 2022-04-26 19:20:22.000000 appyter-0.19.9/js/utils/null.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      183 2022-04-26 19:20:22.000000 appyter-0.19.9/js/utils/re_full.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      115 2022-04-26 19:20:22.000000 appyter-0.19.9/js/utils/silent-check-sso.html
+-rw-r--r--   0 u8sand    (1000) users      (984)      156 2021-05-03 14:23:28.000000 appyter-0.19.9/js/utils/slugify.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      557 2022-04-26 19:20:22.000000 appyter-0.19.9/js/utils/url_for.js
+-rw-r--r--   0 u8sand    (1000) users      (984)      495 2022-04-26 19:20:22.000000 appyter-0.19.9/js/utils/with_timeout.js
+-rw-r--r--   0 u8sand    (1000) users      (984)     4407 2022-04-26 19:20:22.000000 appyter-0.19.9/js/webpack.config.js
+-rw-r--r--   0 u8sand    (1000) users      (984)       73 2022-04-26 19:20:22.000000 appyter-0.19.9/requirements.production.txt
+-rw-r--r--   0 u8sand    (1000) users      (984)      341 2022-04-26 19:20:22.000000 appyter-0.19.9/requirements.txt
+-rw-r--r--   0 u8sand    (1000) users      (984)       38 2022-06-02 17:14:48.155834 appyter-0.19.9/setup.cfg
+-rw-r--r--   0 u8sand    (1000) users      (984)     1131 2022-04-26 19:20:22.000000 appyter-0.19.9/setup.py
```

### Comparing `appyter-0.19.8/.github/workflows/deploy-doc-to-ghpages.yml` & `appyter-0.19.9/.github/workflows/deploy-doc-to-ghpages.yml`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/LICENSE` & `appyter-0.19.9/LICENSE`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/PKG-INFO` & `appyter-0.19.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appyter
-Version: 0.19.8
+Version: 0.19.9
 Summary: UNKNOWN
 Home-page: https://github.com/maayanLab/appyter/
 Author: Daniel J. B. Clarke
 Author-email: u8sand@gmail.com
 License: CC-BY-NC-SA-4.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `appyter-0.19.8/README.md` & `appyter-0.19.9/README.md`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/cli.py` & `appyter-0.19.9/appyter/cli.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/context.py` & `appyter-0.19.9/appyter/context.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/execspec/implementations/cavatica.py` & `appyter-0.19.9/appyter/execspec/implementations/cavatica.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/execspec/implementations/dispatch.py` & `appyter-0.19.9/appyter/execspec/implementations/dispatch.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/execspec/implementations/docker.py` & `appyter-0.19.9/appyter/execspec/implementations/docker.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/execspec/implementations/kube.py` & `appyter-0.19.9/appyter/execspec/implementations/kube.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/execspec/implementations/local.py` & `appyter-0.19.9/appyter/execspec/implementations/local.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/execspec/implementations/subprocess.py` & `appyter-0.19.9/appyter/execspec/implementations/subprocess.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/execspec/implementations/wes.py` & `appyter-0.19.9/appyter/execspec/implementations/wes.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/execspec/registry.py` & `appyter-0.19.9/appyter/execspec/registry.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/execspec/spec.py` & `appyter-0.19.9/appyter/execspec/spec.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/aiohttp.py` & `appyter-0.19.9/appyter/ext/aiohttp.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/asyncio/event_emitter.py` & `appyter-0.19.9/appyter/ext/asyncio/event_emitter.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/asyncio/event_loop.py` & `appyter-0.19.9/appyter/ext/asyncio/event_loop.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,20 @@
   - a thread pool executor that sets the event loop in spawned threads
   '''
   global _LOOP
   if _LOOP is not None:
     logger.warning('Event loop already exists')
     return _LOOP
   logger.debug(f"New event loop")
-  loop = asyncio.new_event_loop()
+  try:
+    import uvloop
+    loop = uvloop.new_event_loop()
+  except ImportError:
+    logger.warning('Install uvloop for better performance')
+    loop = asyncio.new_event_loop()
   asyncio.set_event_loop(loop)
   loop_executor = SharedEventLoopThreadPoolExecutor(loop=loop)
   loop.set_default_executor(loop_executor)
   loop_thread = EventLoopThread(loop=loop)
   loop_thread.start()
   _loop_close = loop.close
   def loop_close(*args, **kwargs):
```

### Comparing `appyter-0.19.8/appyter/ext/asyncio/helpers.py` & `appyter-0.19.9/appyter/ext/asyncio/helpers.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/asyncio/subprocess.py` & `appyter-0.19.9/appyter/ext/asyncio/subprocess.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/asyncio/test_helpers.py` & `appyter-0.19.9/appyter/ext/asyncio/test_helpers.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/asyncio/test_subprocess.py` & `appyter-0.19.9/appyter/ext/asyncio/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/asyncio/try_n_times.py` & `appyter-0.19.9/appyter/ext/asyncio/try_n_times.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/click/__init__.py` & `appyter-0.19.9/appyter/ext/click/__init__.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/contextlib.py` & `appyter-0.19.9/appyter/ext/contextlib.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/cryptography.py` & `appyter-0.19.9/appyter/ext/cryptography.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/dict.py` & `appyter-0.19.9/appyter/ext/dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 def dict_filter_none(d):
-  return { k: v for k, v in d.items() if v }
+  return { k: v for k, v in d.items() if v is not None }
 
 def dict_collision_free_update(d, **kwargs):
   for k, v in kwargs.items():
     assert k not in d, 'Collision in update'
     d[k] = v
 
 def dict_flatten(d):
```

### Comparing `appyter-0.19.8/appyter/ext/drs.py` & `appyter-0.19.9/appyter/ext/drs.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/emitter.py` & `appyter-0.19.9/appyter/ext/emitter.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/flask.py` & `appyter-0.19.9/appyter/ext/flask.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/__init__.py` & `appyter-0.19.9/appyter/ext/fsspec/__init__.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/chroot.py` & `appyter-0.19.9/appyter/ext/fsspec/chroot.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/core.py` & `appyter-0.19.9/appyter/ext/fsspec/core.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/drs.py` & `appyter-0.19.9/appyter/ext/fsspec/drs.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/fuse.py` & `appyter-0.19.9/appyter/ext/fsspec/fuse.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/mapperfs.py` & `appyter-0.19.9/appyter/ext/fsspec/mapperfs.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/overlayfs.py` & `appyter-0.19.9/appyter/ext/fsspec/overlayfs.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/s3fs.py` & `appyter-0.19.9/appyter/ext/fsspec/s3fs.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/sbfs.py` & `appyter-0.19.9/appyter/ext/fsspec/sbfs.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/singleton.py` & `appyter-0.19.9/appyter/ext/fsspec/singleton.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/spec/composable.py` & `appyter-0.19.9/appyter/ext/fsspec/spec/composable.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/spec/mountable.py` & `appyter-0.19.9/appyter/ext/fsspec/spec/mountable.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/spec/sync_async.py` & `appyter-0.19.9/appyter/ext/fsspec/spec/sync_async.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/storage.py` & `appyter-0.19.9/appyter/ext/fsspec/storage.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/test_chroot.py` & `appyter-0.19.9/appyter/ext/fsspec/test_chroot.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/test_drs.py` & `appyter-0.19.9/appyter/ext/fsspec/test_drs.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/test_fuse.py` & `appyter-0.19.9/appyter/ext/fsspec/test_fuse.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/test_fuseless_mount.py` & `appyter-0.19.9/appyter/ext/fsspec/test_fuseless_mount.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/test_mapperfs.py` & `appyter-0.19.9/appyter/ext/fsspec/test_mapperfs.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/test_overlayfs.py` & `appyter-0.19.9/appyter/ext/fsspec/test_overlayfs.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/test_pathmap.py` & `appyter-0.19.9/appyter/ext/fsspec/test_pathmap.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/test_sbfs.py` & `appyter-0.19.9/appyter/ext/fsspec/test_sbfs.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/util.py` & `appyter-0.19.9/appyter/ext/fsspec/util.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/fsspec/writecache.py` & `appyter-0.19.9/appyter/ext/fsspec/writecache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import contextlib
 from pathlib import PurePath
 from fsspec import AbstractFileSystem, filesystem
 from appyter.ext.fsspec.spec.mountable import MountableAbstractFileSystem
 from appyter.ext.fsspec.spec.composable import ComposableAbstractFileSystem
+from appyter.ext.pathlib import is_relative_to
 from appyter.ext.tempfile import mktemp
 
 import logging
 logger = logging.getLogger(__name__)
 
 class WriteCacheFileSystem(MountableAbstractFileSystem, ComposableAbstractFileSystem, AbstractFileSystem):
   protocol = 'writecache'
@@ -146,15 +147,15 @@
       raise
     else:
       if recursive:
         p1 = PurePath(path1)
         p2 = PurePath(path2)
         for d in list(self._dir_cache):
           p = PurePath(d)
-          if p.is_relative_to(p1):
+          if is_relative_to(p, p1):
             self._dir_cache.add(str(p2 / p.relative_to(path1)))
 
   def mv(self, path1, path2, recursive=False, maxdepth=None, **kwargs):
     path1 = self.fs.root_marker + path1.lstrip('/')
     path2 = self.fs.root_marker + path2.lstrip('/')
     try:
       self.fs.mv(path1, path2, recursive=recursive, maxdepth=maxdepth, **kwargs)
@@ -162,15 +163,15 @@
       raise
     else:
       if recursive:
         p1 = PurePath(path1)
         p2 = PurePath(path2)
         for d in list(self._dir_cache):
           p = PurePath(d)
-          if p.is_relative_to(p1):
+          if is_relative_to(p, p1):
             self._dir_cache.remove(d)
             self._dir_cache.add(str(p2 / p.relative_to(path1)))
 
   def exists(self, path, **kwargs):
     path = self.fs.root_marker + path.lstrip('/')
     if path in self._local_cache or path in self._dir_cache:
       return True
```

### Comparing `appyter-0.19.8/appyter/ext/functools.py` & `appyter-0.19.9/appyter/ext/functools.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/hashlib.py` & `appyter-0.19.9/appyter/ext/hashlib.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/importlib.py` & `appyter-0.19.9/appyter/ext/importlib.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/itertools.py` & `appyter-0.19.9/appyter/ext/itertools.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/pathlib/chroot.py` & `appyter-0.19.9/appyter/ext/pathlib/chroot.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/pytest.py` & `appyter-0.19.9/appyter/ext/pytest.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/socketio/chunked_emit.py` & `appyter-0.19.9/appyter/ext/socketio/chunked_emit.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class ChunkedEmitMixin:
   ''' A mixin for splitting up large `emit` calls into `chunked` calls of lower priority
   '''
   CHUNK_SIZE = 1<<20 # 1kb
 
   async def emit(self, evt, data, priority=0, **kwargs):
-    chunkable = evt not in {'chunked', 'forward'}
+    chunkable = evt != 'chunked'
     if chunkable:
       serialized = await async_json_dumps(data, sort_keys=True, separators=None, ensure_ascii=True)
       chunkable = len(serialized) > self.CHUNK_SIZE
     #
     if chunkable:
       logger.debug(f"Large packet ({len(serialized)}), chunking...")
       data_hash = str(uuid.uuid4())
```

### Comparing `appyter-0.19.8/appyter/ext/socketio/client.py` & `appyter-0.19.9/appyter/ext/socketio/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 import traceback
 import socketio
 import logging
 logger = logging.getLogger(__name__)
 
 from appyter.ext.socketio.forwarding import ForwardingMixin
 from appyter.ext.socketio.priority_queued_emit import PriorityQueuedEmitMixin
+from appyter.ext.socketio.chunked_emit import ChunkedEmitMixin
 
 class AsyncClient(
+  ChunkedEmitMixin,
   ForwardingMixin,
   PriorityQueuedEmitMixin,
   socketio.AsyncClient,
 ):
   ''' Client with packet forwarding, emit buffering & chunking
    `async with` is necessary for initialization
   '''
```

### Comparing `appyter-0.19.8/appyter/ext/socketio/priority_queued_emit.py` & `appyter-0.19.9/appyter/ext/socketio/priority_queued_emit.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/socketio/server.py` & `appyter-0.19.9/appyter/ext/socketio/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import socketio
 import logging
 logger = logging.getLogger(__name__)
 
 from appyter.ext.socketio.priority_queued_emit import PriorityQueuedEmitMixin
+from appyter.ext.socketio.chunked_emit import ChunkedEmitMixin
 
 class AsyncServer(
+  ChunkedEmitMixin,
   PriorityQueuedEmitMixin,
   socketio.AsyncServer,
 ):
   ''' Server with packet forwarding.
   `async with` is necessary for initialization
   '''
   def __init__(self, *args, **kwargs):
```

### Comparing `appyter-0.19.8/appyter/ext/tempfile.py` & `appyter-0.19.9/appyter/ext/tempfile.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/urllib.py` & `appyter-0.19.9/appyter/ext/urllib.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/ext/watchgod/watcher.py` & `appyter-0.19.9/appyter/ext/watchgod/watcher.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/extras/__init__.py` & `appyter-0.19.9/appyter/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/extras/catalog_integration/executor.py` & `appyter-0.19.9/appyter/extras/catalog_integration/executor.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/extras/catalog_integration/notebooks.py` & `appyter-0.19.9/appyter/extras/catalog_integration/notebooks.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/extras/catalog_integration/request.py` & `appyter-0.19.9/appyter/extras/catalog_integration/request.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/extras/catalog_integration/storage.py` & `appyter-0.19.9/appyter/extras/catalog_integration/storage.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/extras/catalog_integration/uploads.py` & `appyter-0.19.9/appyter/extras/catalog_integration/uploads.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/extras/catalog_integration/userfs.py` & `appyter-0.19.9/appyter/extras/catalog_integration/userfs.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/fields.py` & `appyter-0.19.9/appyter/fields.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/helpers/commandify.py` & `appyter-0.19.9/appyter/helpers/commandify.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/helpers/cookiecutter/{{ cookiecutter.project_slug }}/appyter.json` & `appyter-0.19.9/appyter/helpers/cookiecutter/{{ cookiecutter.project_slug }}/appyter.json`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/helpers/cookiecutter/{{ cookiecutter.project_slug }}/{{ cookiecutter.project_slug }}.ipynb` & `appyter-0.19.9/appyter/helpers/cookiecutter/{{ cookiecutter.project_slug }}/{{ cookiecutter.project_slug }}.ipynb`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/helpers/dockerize.py` & `appyter-0.19.9/appyter/helpers/dockerize.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/helpers/fetch_and_serve.py` & `appyter-0.19.9/appyter/helpers/fetch_and_serve.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/helpers/init.py` & `appyter-0.19.9/appyter/helpers/init.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/helpers/nbclean.py` & `appyter-0.19.9/appyter/helpers/nbclean.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/helpers/serve.py` & `appyter-0.19.9/appyter/helpers/serve.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/magic.py` & `appyter-0.19.9/appyter/magic.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/orchestration/dispatcher/__init__.py` & `appyter-0.19.9/appyter/orchestration/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/orchestration/dispatcher/core.py` & `appyter-0.19.9/appyter/orchestration/dispatcher/core.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/parse/nb.py` & `appyter-0.19.9/appyter/parse/nb.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/parse/nbtemplate.py` & `appyter-0.19.9/appyter/parse/nbtemplate.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/__init__.py` & `appyter-0.19.9/appyter/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/biojupies/templates/biojupies/base.j2` & `appyter-0.19.9/appyter/profiles/biojupies/templates/biojupies/base.j2`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/biojupies/templates/fields/BoolField.j2` & `appyter-0.19.9/appyter/profiles/biojupies/templates/fields/BoolField.j2`

 * *Files 24% similar despite different names*

```diff
@@ -4,13 +4,13 @@
     {%- if this.args.description %}
       <sup data-toggle="tooltip" title="{{ this.args.description }}"><i class="far fa-question-circle"></i></sup>
     {% endif -%}
   </div>
   <div class="col-lg-1 pt-1 pt-lg-0">
     <div class="border-grey rounded d-table mt-lg-1 overflow-hidden my-auto">
       <input type="radio" id="{{ this.args.name }}-yes" name="{{ this.args.name }}" value="yes" class="d-none" {% if this.value %} checked{% endif %}>
-      <label for="{{ this.args.name }}-yes" class="radio-label px-2 py-1 cursor-pointer d-table-cell">Yes</label>
+      <label for="{{ this.args.name }}-yes" class="radio-label px-2 py-1 cursor-pointer d-table-cell">{{ self.args.yes_label or 'Yes' }}</label>
       <input type="radio" id="{{ this.args.name }}-no" name="{{ this.args.name }}" value="no" class="d-none" {% if not this.value %} checked{% endif %}>
-      <label for="{{ this.args.name }}-no" class="radio-label px-2 py-1 cursor-pointer d-table-cell">No</label>
+      <label for="{{ this.args.name }}-no" class="radio-label px-2 py-1 cursor-pointer d-table-cell">{{ self.args.no_label or 'No' }}</label>
     </div>
   </div>
 </div>
```

### Comparing `appyter-0.19.8/appyter/profiles/biojupies/templates/fields/ChoiceField.j2` & `appyter-0.19.9/appyter/profiles/biojupies/templates/fields/ChoiceField.j2`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/biojupies/templates/fields/FloatField.j2` & `appyter-0.19.9/appyter/profiles/biojupies/templates/fields/FloatField.j2`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/biojupies/templates/fields/MultiChoiceField.j2` & `appyter-0.19.9/appyter/profiles/biojupies/templates/fields/MultiChoiceField.j2`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/bootstrap/static/css/bootstrap.css` & `appyter-0.19.9/appyter/profiles/bootstrap/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/bootstrap/static/js/lib/bootstrap/bootstrap.bundle.min.js` & `appyter-0.19.9/appyter/profiles/bootstrap/static/js/lib/bootstrap/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/bootstrap/static/js/lib/select2/select2.min.js` & `appyter-0.19.9/appyter/profiles/bootstrap/static/js/lib/select2/select2.min.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/bootstrap/templates/bootstrap/base.j2` & `appyter-0.19.9/appyter/profiles/bootstrap/templates/bootstrap/base.j2`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/blueprints/StorageFileField.py` & `appyter-0.19.9/appyter/profiles/default/blueprints/StorageFileField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/blueprints/locate.py` & `appyter-0.19.9/appyter/profiles/default/blueprints/locate.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/AutocompleteField.py` & `appyter-0.19.9/appyter/profiles/default/fields/AutocompleteField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/BoolField.py` & `appyter-0.19.9/appyter/profiles/default/fields/BoolField.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import json
 from appyter.fields import Field
 
 class BoolField(Field):
   ''' Represing a true or false value with a checkbox.
 
   :param name: (str) A name that will be used to refer to the object as a variable and in the HTML form.
   :param label: (str) A human readable label for the field for the HTML form
   :param description: (Optional[str]) A long human readable description for the field for the HTML form
   :param required: (Optional[bool]) Whether or not this field is required (defaults to false)
   :param default: (bool) A default value as an example and for use during prototyping
   :param section: (Optional[str]) The name of a SectionField for which to nest this field under, defaults to a root SectionField
+  :param yes_label: (Optional[str]) The text instead of "Yes"
+  :param no_label: (Optional[str]) The text instead of "No"
   :param value: (INTERNAL Any) The raw value of the field (from the form for instance)
   :param \**kwargs: Additional keyword arguments used by other fields
   '''
   def __init__(self, **kwargs):
     super().__init__(**kwargs)
 
   @property
@@ -33,15 +34,15 @@
 
   def to_jsonschema(self):
     return dict(super().to_jsonschema(), type='boolean')
 
   def to_cwl(self):
     schema = super().to_cwl()
     schema['type'] = 'boolean'
-    schema['inputBinding']['prefix'] = f"--{self.args['name']}"
+    schema['inputBinding']['prefix'] = f"--{self.args['name']}="
+    schema['inputBinding']['valueFrom'] = '${ if (self) { return "true"; } else { return "false"; } }'
     return schema
 
   def to_click(self):
     args, kwargs = super().to_click()
     kwargs['type'] = bool
-    kwargs['is_flag'] = True
     return args, kwargs
```

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/ChoiceField.py` & `appyter-0.19.9/appyter/profiles/default/fields/ChoiceField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/DescriptionField.py` & `appyter-0.19.9/appyter/profiles/default/fields/DescriptionField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/FileField.py` & `appyter-0.19.9/appyter/profiles/default/fields/FileField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/FloatField.py` & `appyter-0.19.9/appyter/profiles/default/fields/FloatField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/IntField.py` & `appyter-0.19.9/appyter/profiles/default/fields/IntField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/MultiCheckboxField.py` & `appyter-0.19.9/appyter/profiles/default/fields/MultiCheckboxField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/MultiChoiceField.py` & `appyter-0.19.9/appyter/profiles/default/fields/MultiChoiceField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/SectionField.py` & `appyter-0.19.9/appyter/profiles/default/fields/SectionField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/StringField.py` & `appyter-0.19.9/appyter/profiles/default/fields/StringField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/TabField.py` & `appyter-0.19.9/appyter/profiles/default/fields/TabField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/TextField.py` & `appyter-0.19.9/appyter/profiles/default/fields/TextField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/TextListField.py` & `appyter-0.19.9/appyter/profiles/default/fields/TextListField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/fields/VariableField.py` & `appyter-0.19.9/appyter/profiles/default/fields/VariableField.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/filters/url_for.py` & `appyter-0.19.9/appyter/profiles/default/filters/url_for.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/templates/default/base.j2` & `appyter-0.19.9/appyter/profiles/default/templates/default/base.j2`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/templates/fields/IntField.j2` & `appyter-0.19.9/appyter/profiles/default/templates/fields/IntField.j2`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/templates/fragments/jupyter.j2` & `appyter-0.19.9/appyter/profiles/default/templates/fragments/jupyter.j2`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/templates/production/Dockerfile.j2` & `appyter-0.19.9/appyter/profiles/default/templates/production/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/profiles/default/templates/production/nginx.conf.j2` & `appyter-0.19.9/appyter/profiles/default/templates/production/nginx.conf.j2`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,28 @@
       {% else %}
       proxy_set_header Host $http_host;
       proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
       {%- endif %}
       {%- if ws %}
       proxy_http_version 1.1;
       proxy_set_header Upgrade $http_upgrade;
-      proxy_set_header Connection "Upgrade";
+      proxy_set_header Connection $connection_upgrade;
       proxy_read_timeout 900s;
       proxy_send_timeout 900s;
       proxy_connect_timeout 900s;
       {%- endif %}
       proxy_pass {{ remote }};
       {%- if cache %}
       proxy_cache {{ cache }};
       proxy_cache_revalidate on;
       proxy_cache_use_stale error timeout http_500 http_502 http_503 http_504;
       proxy_cache_lock on;
       {%- endif %}
+      proxy_buffers 512 256M;
+      proxy_buffer_size 256M;
 {%- endmacro -%}
 
 pid {{ str(_tmp_dir/'nginx.pid') }};
 worker_processes 1;
 daemon off;
 
 events {
@@ -83,14 +85,19 @@
   }
   map $http_x_forwarded_host $proxied_host {
     default $http_x_forwarded_host;
     ''      $http_host;
   }
   {%- endif %}
 
+  map $http_upgrade $connection_upgrade {
+    default Upgrade;
+    '' close;
+  }
+
   server {
     listen {{ _config.PORT }};
     server_name {{ _config.HOST }};
     include /etc/nginx/mime.types;
     charset utf-8;
     sendfile on;
     keepalive_timeout 0;
```

### Comparing `appyter-0.19.8/appyter/profiles/default/templates/production/supervisord.conf.j2` & `appyter-0.19.9/appyter/profiles/default/templates/production/supervisord.conf.j2`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/flask_app/__init__.py` & `appyter-0.19.9/appyter/render/flask_app/__init__.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/flask_app/constants.py` & `appyter-0.19.9/appyter/render/flask_app/constants.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/flask_app/core.py` & `appyter-0.19.9/appyter/render/flask_app/core.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/flask_app/development.py` & `appyter-0.19.9/appyter/render/flask_app/development.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   import sys
   import asyncio
   return await asyncio.create_subprocess_exec(
     sys.executable, '-u', '-m', 'appyter',
     f"--socket={config['HOST']}:{config['PORT']}",
     stdout=sys.stdout,
     stderr=sys.stderr,
-    env=os.environ,
+    env=dict(os.environ),
   )
 
 async def app_runner(emitter, config):
   import asyncio
   from appyter.ext.subprocess import interrupt
   state_lock = asyncio.Lock()
   state = dict(proc=await run_app(config))
```

### Comparing `appyter-0.19.8/appyter/render/flask_app/drs.py` & `appyter-0.19.9/appyter/render/flask_app/drs.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/flask_app/execution.py` & `appyter-0.19.9/appyter/render/flask_app/execution.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/flask_app/export.py` & `appyter-0.19.9/appyter/render/flask_app/export.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/flask_app/prepare.py` & `appyter-0.19.9/appyter/render/flask_app/prepare.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/flask_app/production.py` & `appyter-0.19.9/appyter/render/flask_app/production.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/flask_app/room_manager.py` & `appyter-0.19.9/appyter/render/flask_app/room_manager.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/flask_app/socketio.py` & `appyter-0.19.9/appyter/render/flask_app/socketio.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/flask_app/static.py` & `appyter-0.19.9/appyter/render/flask_app/static.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/flask_app/upload.py` & `appyter-0.19.9/appyter/render/flask_app/upload.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/nbconstruct.py` & `appyter-0.19.9/appyter/render/nbconstruct.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/nbexecute.py` & `appyter-0.19.9/appyter/render/nbexecute.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/nbinspect/cwl.py` & `appyter-0.19.9/appyter/render/nbinspect/cwl.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 def render_cwl_from_nbtemplate(env, nb, ipynb=None, cwd=None, info=None):
   ''' Render a cwl representing the relevant Fields throughout the notebook.
   '''
   fields = list(parse_fields_from_nbtemplate(env, nb, deep=True))
   schema = {
     'cwlVersion': 'v1.2',
     'class': 'CommandLineTool',
+    'requirements': [
+        {'class': 'InlineJavascriptRequirement'},
+        {'class': 'LoadListingRequirement'},
+    ],
   }
   # potentially extract info from appyter embedded metadata if not provided
   if info is None and 'appyter' in nb.metadata and 'info' in nb.metadata['appyter']:
     info = nb.metadata['appyter']['info']
   if info is not None:
     schema.update({
       'id': f"appyter-{info['name'].lower()}",
```

### Comparing `appyter-0.19.8/appyter/render/nbinspect/jsonschema.py` & `appyter-0.19.9/appyter/render/nbinspect/jsonschema.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/nbinspect/nbtemplate_json.py` & `appyter-0.19.9/appyter/render/nbinspect/nbtemplate_json.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/render/nbinspect/openapi.py` & `appyter-0.19.9/appyter/render/nbinspect/openapi.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/css/fontawesome.css` & `appyter-0.19.9/appyter/static/profiles/biojupies/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/css/index.css` & `appyter-0.19.9/appyter/static/profiles/biojupies/css/index.css`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/js/fields/IntField.js` & `appyter-0.19.9/appyter/static/profiles/biojupies/js/fields/IntField.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -349,15 +349,15 @@
                     let o, {
                             args: i
                         } = e,
                         r = !0;
                     return t.$$set = t => {
                         "args" in t && n(0, i = t.args)
                     }, t.$$.update = () => {
-                        3 & t.$$.dirty && void 0 !== i && void 0 === o && n(1, o = i.default), 3 & t.$$.dirty && void 0 !== o && void 0 !== i && n(2, r = (0 | o) === o && (B(i.min) || (0 | o) >= i.min) && (B(i.max) || (0 | o) <= i.max))
+                        3 & t.$$.dirty && void 0 !== i && void 0 === o && n(1, o = 0 | i.default), 3 & t.$$.dirty && void 0 !== o && void 0 !== i && n(2, r = (0 | o) === o && (B(i.min) || (0 | o) >= i.min) && (B(i.max) || (0 | o) <= i.max))
                     }, [i, o, r, function() {
                         o = b(this.value), n(1, o), n(0, i)
                     }]
                 }
                 var J = class extends class {
                     $destroy() {
                         N(this, 1), this.$destroy = n
```

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/js/fields/SectionField.js` & `appyter-0.19.9/appyter/static/profiles/biojupies/js/fields/SectionField.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/js/fields/StringField.js` & `appyter-0.19.9/appyter/static/profiles/biojupies/js/fields/StringField.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/js/fields/TextField.js` & `appyter-0.19.9/appyter/static/profiles/biojupies/js/fields/TextField.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/js/fields/TextListField.js` & `appyter-0.19.9/appyter/static/profiles/biojupies/js/fields/TextListField.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/js/form.js` & `appyter-0.19.9/appyter/static/profiles/biojupies/js/form.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -67,22 +67,22 @@
                     function i(t, n, e) {
                         let o, {
                                 classes: i = ""
                             } = n,
                             {
                                 data: c = ""
                             } = n,
-                            u = {};
+                            s = {};
                         return t.$$set = t => {
                             "classes" in t && e(0, i = t.classes), "data" in t && e(1, c = t.data)
                         }, t.$$.update = () => {
                             4 & t.$$.dirty && o && o.querySelectorAll("script").forEach((t => {
                                 "application/json" !== t.type && function(t) {
-                                    if (void 0 === u[t]) {
-                                        u[t] = !0;
+                                    if (void 0 === s[t]) {
+                                        s[t] = !0;
                                         try {
                                             new Function(t)()
                                         } catch (t) {
                                             ! function({
                                                 nb: t,
                                                 type: n,
                                                 error: e
@@ -126,20 +126,20 @@
                         constructor(t) {
                             super(), (0, r.S1n)(this, t, i, o, r.N8, {
                                 classes: 0,
                                 data: 1
                             })
                         }
                     }
-                    var u = c,
-                        s = e(1782);
+                    var s = c,
+                        u = e(1782);
 
                     function a(t) {
                         let n, e;
-                        return n = new u({
+                        return n = new s({
                             props: {
                                 classes: "ssr",
                                 data: t[0]
                             }
                         }), {
                             c() {
                                 (0, r.YCL)(n.$$.fragment)
@@ -161,15 +161,15 @@
                                 (0, r.vpE)(n, t)
                             }
                         }
                     }
 
                     function l(t) {
                         let n, e, o;
-                        return e = new s.Z({}), {
+                        return e = new u.Z({}), {
                             c() {
                                 n = (0, r.bGB)("div"), (0, r.YCL)(e.$$.fragment), (0, r.Ljt)(n, "class", "text-center")
                             },
                             m(t, i) {
                                 (0, r.$Tr)(t, n, i), (0, r.yef)(e, n, null), o = !0
                             },
                             p: r.ZTd,
@@ -184,40 +184,40 @@
                             }
                         }
                     }
 
                     function f(t) {
                         let n, e, o, i;
                         const c = [l, a],
-                            u = [];
+                            s = [];
 
-                        function s(t, n) {
+                        function u(t, n) {
                             return void 0 === t[0] ? 0 : 1
                         }
-                        return n = s(t), e = u[n] = c[n](t), {
+                        return n = u(t), e = s[n] = c[n](t), {
                             c() {
                                 e.c(), o = (0, r.cSb)()
                             },
                             m(t, e) {
-                                u[n].m(t, e), (0, r.$Tr)(t, o, e), i = !0
+                                s[n].m(t, e), (0, r.$Tr)(t, o, e), i = !0
                             },
                             p(t, [i]) {
                                 let a = n;
-                                n = s(t), n === a ? u[n].p(t, i) : ((0, r.dvw)(), (0, r.etI)(u[a], 1, 1, (() => {
-                                    u[a] = null
-                                })), (0, r.gbL)(), e = u[n], e ? e.p(t, i) : (e = u[n] = c[n](t), e.c()), (0, r.Ui)(e, 1), e.m(o.parentNode, o))
+                                n = u(t), n === a ? s[n].p(t, i) : ((0, r.dvw)(), (0, r.etI)(s[a], 1, 1, (() => {
+                                    s[a] = null
+                                })), (0, r.gbL)(), e = s[n], e ? e.p(t, i) : (e = s[n] = c[n](t), e.c()), (0, r.Ui)(e, 1), e.m(o.parentNode, o))
                             },
                             i(t) {
                                 i || ((0, r.Ui)(e), i = !0)
                             },
                             o(t) {
                                 (0, r.etI)(e), i = !1
                             },
                             d(t) {
-                                u[n].d(t), t && (0, r.ogt)(o)
+                                s[n].d(t), t && (0, r.ogt)(o)
                             }
                         }
                     }
 
                     function d(t, n, e) {
                         let r, {
                                 field: o
@@ -333,45 +333,45 @@
                             }
                         }
                     }
 
                     function v(t) {
                         let n, e, o, i;
                         const c = [t[2]];
-                        let u = {};
-                        for (let t = 0; t < c.length; t += 1) u = (0, r.f0i)(u, c[t]);
+                        let s = {};
+                        for (let t = 0; t < c.length; t += 1) s = (0, r.f0i)(s, c[t]);
                         n = new m({
-                            props: u
+                            props: s
                         });
-                        let s = void 0 !== t[2].error && y(t);
+                        let u = void 0 !== t[2].error && y(t);
                         return {
                             c() {
-                                (0, r.YCL)(n.$$.fragment), e = (0, r.DhX)(), s && s.c(), o = (0, r.cSb)()
+                                (0, r.YCL)(n.$$.fragment), e = (0, r.DhX)(), u && u.c(), o = (0, r.cSb)()
                             },
                             m(t, c) {
-                                (0, r.yef)(n, t, c), (0, r.$Tr)(t, e, c), s && s.m(t, c), (0, r.$Tr)(t, o, c), i = !0
+                                (0, r.yef)(n, t, c), (0, r.$Tr)(t, e, c), u && u.m(t, c), (0, r.$Tr)(t, o, c), i = !0
                             },
                             p(t, e) {
                                 const i = 1 & e ? (0, r.LoY)(c, [(0, r.gCg)(t[2])]) : {};
-                                n.$set(i), void 0 !== t[2].error ? s ? s.p(t, e) : (s = y(t), s.c(), s.m(o.parentNode, o)) : s && (s.d(1), s = null)
+                                n.$set(i), void 0 !== t[2].error ? u ? u.p(t, e) : (u = y(t), u.c(), u.m(o.parentNode, o)) : u && (u.d(1), u = null)
                             },
                             i(t) {
                                 i || ((0, r.Ui)(n.$$.fragment, t), i = !0)
                             },
                             o(t) {
                                 (0, r.etI)(n.$$.fragment, t), i = !1
                             },
                             d(t) {
-                                (0, r.vpE)(n, t), t && (0, r.ogt)(e), s && s.d(t), t && (0, r.ogt)(o)
+                                (0, r.vpE)(n, t), t && (0, r.ogt)(e), u && u.d(t), t && (0, r.ogt)(o)
                             }
                         }
                     }
 
                     function w(t) {
-                        let n, e, o, i, c, u, s, a, l, f, d, p, m, y, w, L, j = t[1].title + "";
+                        let n, e, o, i, c, s, u, a, l, f, d, p, m, y, w, L, j = t[1].title + "";
 
                         function T(t, n) {
                             return t[1].img ? h : t[1].icon ? $ : void 0
                         }
                         let I = T(t),
                             _ = I && I(t),
                             k = t[1].subtitle && b(t),
@@ -379,25 +379,25 @@
                             C = [];
                         for (let n = 0; n < x.length; n += 1) C[n] = v(g(t, x, n));
                         const S = t => (0, r.etI)(C[t], 1, 1, (() => {
                             C[t] = null
                         }));
                         return {
                             c() {
-                                n = (0, r.bGB)("div"), e = (0, r.bGB)("div"), o = (0, r.bGB)("div"), i = (0, r.bGB)("div"), c = (0, r.bGB)("div"), _ && _.c(), u = (0, r.DhX)(), s = (0, r.bGB)("div"), a = (0, r.bGB)("div"), l = (0, r.fLW)(j), f = (0, r.DhX)(), k && k.c(), p = (0, r.DhX)(), m = (0, r.bGB)("div"), y = (0, r.bGB)("div");
+                                n = (0, r.bGB)("div"), e = (0, r.bGB)("div"), o = (0, r.bGB)("div"), i = (0, r.bGB)("div"), c = (0, r.bGB)("div"), _ && _.c(), s = (0, r.DhX)(), u = (0, r.bGB)("div"), a = (0, r.bGB)("div"), l = (0, r.fLW)(j), f = (0, r.DhX)(), k && k.c(), p = (0, r.DhX)(), m = (0, r.bGB)("div"), y = (0, r.bGB)("div");
                                 for (let t = 0; t < C.length; t += 1) C[t].c();
-                                (0, r.Ljt)(c, "class", "d-table-cell align-middle card-icon px-3 py-3 text-center"), (0, r.Ljt)(a, "class", "very-small regular pb-2 pr-5"), (0, r.Ljt)(s, "class", "d-table-cell align-middle"), (0, r.Ljt)(i, "class", "d-table w-100 py-2 px-2 py-md-0 px-md-0"), (0, r.Ljt)(o, "class", "mt-3 mb-0 w-100 border-custom rounded bg-lightgrey"), (0, r.Ljt)(o, "data-toggle", "collapse"), (0, r.Ljt)(o, "data-target", d = "#" + t[1].name), (0, r.Ljt)(y, "class", "pt-3"), (0, r.Ljt)(m, "id", w = t[1].name), (0, r.Ljt)(m, "class", "border-grey mx-2 border-top-0 rounded-bottom tiny collapse show"), (0, r.Ljt)(e, "class", "col-sm-12"), (0, r.Ljt)(n, "class", "row")
+                                (0, r.Ljt)(c, "class", "d-table-cell align-middle card-icon px-3 py-3 text-center"), (0, r.Ljt)(a, "class", "very-small regular pb-2 pr-5"), (0, r.Ljt)(u, "class", "d-table-cell align-middle"), (0, r.Ljt)(i, "class", "d-table w-100 py-2 px-2 py-md-0 px-md-0"), (0, r.Ljt)(o, "class", "mt-3 mb-0 w-100 border-custom rounded bg-lightgrey"), (0, r.Ljt)(o, "data-toggle", "collapse"), (0, r.Ljt)(o, "data-target", d = "#" + t[1].name), (0, r.Ljt)(y, "class", "pt-3"), (0, r.Ljt)(m, "id", w = t[1].name), (0, r.Ljt)(m, "class", "border-grey mx-2 border-top-0 rounded-bottom tiny collapse show"), (0, r.Ljt)(e, "class", "col-sm-12"), (0, r.Ljt)(n, "class", "row")
                             },
                             m(t, d) {
-                                (0, r.$Tr)(t, n, d), (0, r.R3I)(n, e), (0, r.R3I)(e, o), (0, r.R3I)(o, i), (0, r.R3I)(i, c), _ && _.m(c, null), (0, r.R3I)(i, u), (0, r.R3I)(i, s), (0, r.R3I)(s, a), (0, r.R3I)(a, l), (0, r.R3I)(s, f), k && k.m(s, null), (0, r.R3I)(e, p), (0, r.R3I)(e, m), (0, r.R3I)(m, y);
+                                (0, r.$Tr)(t, n, d), (0, r.R3I)(n, e), (0, r.R3I)(e, o), (0, r.R3I)(o, i), (0, r.R3I)(i, c), _ && _.m(c, null), (0, r.R3I)(i, s), (0, r.R3I)(i, u), (0, r.R3I)(u, a), (0, r.R3I)(a, l), (0, r.R3I)(u, f), k && k.m(u, null), (0, r.R3I)(e, p), (0, r.R3I)(e, m), (0, r.R3I)(m, y);
                                 for (let t = 0; t < C.length; t += 1) C[t].m(y, null);
                                 L = !0
                             },
                             p(t, [n]) {
-                                if (I === (I = T(t)) && _ ? _.p(t, n) : (_ && _.d(1), _ = I && I(t), _ && (_.c(), _.m(c, null))), (!L || 2 & n) && j !== (j = t[1].title + "") && (0, r.rTO)(l, j), t[1].subtitle ? k ? k.p(t, n) : (k = b(t), k.c(), k.m(s, null)) : k && (k.d(1), k = null), (!L || 2 & n && d !== (d = "#" + t[1].name)) && (0, r.Ljt)(o, "data-target", d), 1 & n) {
+                                if (I === (I = T(t)) && _ ? _.p(t, n) : (_ && _.d(1), _ = I && I(t), _ && (_.c(), _.m(c, null))), (!L || 2 & n) && j !== (j = t[1].title + "") && (0, r.rTO)(l, j), t[1].subtitle ? k ? k.p(t, n) : (k = b(t), k.c(), k.m(u, null)) : k && (k.d(1), k = null), (!L || 2 & n && d !== (d = "#" + t[1].name)) && (0, r.Ljt)(o, "data-target", d), 1 & n) {
                                     let e;
                                     for (x = t[0], e = 0; e < x.length; e += 1) {
                                         const o = g(t, x, e);
                                         C[e] ? (C[e].p(o, n), (0, r.Ui)(C[e], 1)) : (C[e] = v(o), C[e].c(), (0, r.Ui)(C[e], 1), C[e].m(y, null))
                                     }
                                     for ((0, r.dvw)(), e = x.length; e < C.length; e += 1) S(e);
                                     (0, r.gbL)()
@@ -521,15 +521,15 @@
                         }; {
                             const [e, r] = [t.slice(0, n), t.slice(n + 1)];
                             return {
                                 path: e,
                                 params: function(t) {
                                     return "" === t ? {} : t.split("&").map((t => t.split("=").map(decodeURIComponent))).reduce(((t, [n, e]) => ({
                                         ...t,
-                                        [n]: e
+                                        [n]: void 0 === e || e
                                     })), {})
                                 }(r)
                             }
                         }
                     }
 
                     function i() {
@@ -541,16 +541,16 @@
                             params: n,
                             server: e
                         } = {
                             ...o(i()),
                             server: o(`${window.location.pathname}${window.location.search}`)
                         }, {
                             subscribe: c,
-                            update: u,
-                            set: s
+                            update: s,
+                            set: u
                         } = (0, r.fZ)({
                             path: t,
                             params: n,
                             server: e
                         });
                         let a = t;
                         return c((({
@@ -559,33 +559,33 @@
                             server: e
                         }) => {
                             const r = function({
                                 path: t,
                                 params: n
                             }) {
                                 const e = function(t) {
-                                    return Object.keys(t).filter((n => void 0 !== t[n] && "" !== t[n])).map((n => [n, t[n]].map(encodeURIComponent).join("="))).join("&")
+                                    return Object.keys(t).filter((n => void 0 !== t[n] && "" !== t[n])).map((n => !0 === t[n] ? encodeURIComponent(n) : [n, t[n]].map(encodeURIComponent).join("="))).join("&")
                                 }(n);
                                 return "" === e ? t : `${t}?${e}`
                             }({
                                 path: t,
                                 params: n
                             });
                             if (t !== a) window.location.hash = r, a = t;
                             else {
                                 const t = `${window.location.origin}${window.location.pathname}${window.location.search}`;
                                 history.replaceState(void 0, void 0, "" !== r ? `${t}#${r}` : t)
                             }
-                        })), window.addEventListener("hashchange", (() => s({
+                        })), window.addEventListener("hashchange", (() => u({
                             ...o(i()),
                             initServer: e
                         }))), {
                             subscribe: c,
-                            update: u,
-                            set: s
+                            update: s,
+                            set: u
                         }
                     }();
                     n.Z = c
                 },
                 8826: function(t, n, e) {
                     function r() {}
 
@@ -598,19 +598,19 @@
                         return t()
                     }
 
                     function c() {
                         return Object.create(null)
                     }
 
-                    function u(t) {
+                    function s(t) {
                         t.forEach(i)
                     }
 
-                    function s(t) {
+                    function u(t) {
                         return "function" == typeof t
                     }
 
                     function a(t, n) {
                         return t != t ? n == n : t !== n || t && "object" == typeof t || "function" == typeof t
                     }
                     let l;
@@ -707,15 +707,15 @@
                         R3I: function() {
                             return w
                         },
                         RMB: function() {
                             return T
                         },
                         S1n: function() {
-                            return ut
+                            return st
                         },
                         Ui: function() {
                             return tt
                         },
                         VHj: function() {
                             return B
                         },
@@ -749,15 +749,15 @@
                         f0i: function() {
                             return o
                         },
                         fLW: function() {
                             return _
                         },
                         f_C: function() {
-                            return st
+                            return ut
                         },
                         gCg: function() {
                             return rt
                         },
                         gbL: function() {
                             return Q
                         },
@@ -862,60 +862,60 @@
                     }
                     new Map;
                     const N = [],
                         A = [],
                         Y = [],
                         P = [],
                         D = Promise.resolve();
-                    let M = !1;
+                    let F = !1;
 
-                    function X(t) {
+                    function M(t) {
                         Y.push(t)
                     }
-                    const F = new Set;
+                    const X = new Set;
                     let H = 0;
 
                     function q() {
                         const t = y;
                         do {
                             for (; H < N.length;) {
                                 const t = N[H];
                                 H++, G(t), z(t.$$)
                             }
                             for (G(null), N.length = 0, H = 0; A.length;) A.pop()();
                             for (let t = 0; t < Y.length; t += 1) {
                                 const n = Y[t];
-                                F.has(n) || (F.add(n), n())
+                                X.has(n) || (X.add(n), n())
                             }
                             Y.length = 0
                         } while (N.length);
                         for (; P.length;) P.pop()();
-                        M = !1, F.clear(), G(t)
+                        F = !1, X.clear(), G(t)
                     }
 
                     function z(t) {
                         if (null !== t.fragment) {
-                            t.update(), u(t.before_update);
+                            t.update(), s(t.before_update);
                             const n = t.dirty;
-                            t.dirty = [-1], t.fragment && t.fragment.p(t.ctx, n), t.after_update.forEach(X)
+                            t.dirty = [-1], t.fragment && t.fragment.p(t.ctx, n), t.after_update.forEach(M)
                         }
                     }
                     const V = new Set;
                     let J, W;
 
                     function K() {
                         J = {
                             r: 0,
                             c: [],
                             p: J
                         }
                     }
 
                     function Q() {
-                        J.r || u(J.c), J = J.p
+                        J.r || s(J.c), J = J.p
                     }
 
                     function tt(t, n) {
                         t && t.i && (V.delete(t), t.i(n))
                     }
 
                     function nt(t, n, e, r) {
@@ -932,19 +932,19 @@
                             r = {},
                             o = {
                                 $$scope: 1
                             };
                         let i = t.length;
                         for (; i--;) {
                             const c = t[i],
-                                u = n[i];
-                            if (u) {
-                                for (const t in c) t in u || (r[t] = 1);
-                                for (const t in u) o[t] || (e[t] = u[t], o[t] = 1);
-                                t[i] = u
+                                s = n[i];
+                            if (s) {
+                                for (const t in c) t in s || (r[t] = 1);
+                                for (const t in s) o[t] || (e[t] = s[t], o[t] = 1);
+                                t[i] = s
                             } else
                                 for (const t in c) o[t] = 1
                         }
                         for (const t in r) t in e || (e[t] = void 0);
                         return e
                     }
 
@@ -959,32 +959,32 @@
                     function it(t, n, e, r) {
                         const {
                             fragment: o,
                             on_mount: c,
                             on_destroy: a,
                             after_update: l
                         } = t.$$;
-                        o && o.m(n, e), r || X((() => {
-                            const n = c.map(i).filter(s);
-                            a ? a.push(...n) : u(n), t.$$.on_mount = []
-                        })), l.forEach(X)
+                        o && o.m(n, e), r || M((() => {
+                            const n = c.map(i).filter(u);
+                            a ? a.push(...n) : s(n), t.$$.on_mount = []
+                        })), l.forEach(M)
                     }
 
                     function ct(t, n) {
                         const e = t.$$;
-                        null !== e.fragment && (u(e.on_destroy), e.fragment && e.fragment.d(n), e.on_destroy = e.fragment = null, e.ctx = [])
+                        null !== e.fragment && (s(e.on_destroy), e.fragment && e.fragment.d(n), e.on_destroy = e.fragment = null, e.ctx = [])
                     }
 
-                    function ut(t, n, e, o, i, s, a, l = [-1]) {
+                    function st(t, n, e, o, i, u, a, l = [-1]) {
                         const f = y;
                         G(t);
                         const d = t.$$ = {
                             fragment: null,
                             ctx: null,
-                            props: s,
+                            props: u,
                             update: r,
                             not_equal: i,
                             bound: c(),
                             on_mount: [],
                             on_destroy: [],
                             on_disconnect: [],
                             before_update: [],
@@ -996,17 +996,17 @@
                             root: n.target || f.$$.root
                         };
                         a && a(d.root);
                         let p = !1;
                         if (d.ctx = e ? e(t, n.props || {}, ((n, e, ...r) => {
                                 const o = r.length ? r[0] : e;
                                 return d.ctx && i(d.ctx[n], d.ctx[n] = o) && (!d.skip_bound && d.bound[n] && d.bound[n](o), p && function(t, n) {
-                                    -1 === t.$$.dirty[0] && (N.push(t), M || (M = !0, D.then(q)), t.$$.dirty.fill(0)), t.$$.dirty[n / 31 | 0] |= 1 << n % 31
+                                    -1 === t.$$.dirty[0] && (N.push(t), F || (F = !0, D.then(q)), t.$$.dirty.fill(0)), t.$$.dirty[n / 31 | 0] |= 1 << n % 31
                                 }(t, n)), e
-                            })) : [], d.update(), p = !0, u(d.before_update), d.fragment = !!o && o(d.ctx), n.target) {
+                            })) : [], d.update(), p = !0, s(d.before_update), d.fragment = !!o && o(d.ctx), n.target) {
                             if (n.hydrate) {
                                 v = !0;
                                 const t = function(t) {
                                     return Array.from(t.childNodes)
                                 }(n.target);
                                 d.fragment && d.fragment.l(t), t.forEach(j)
                             } else d.fragment && d.fragment.c();
@@ -1020,37 +1020,37 @@
                                 mode: "open"
                             })
                         }
                         connectedCallback() {
                             const {
                                 on_mount: t
                             } = this.$$;
-                            this.$$.on_disconnect = t.map(i).filter(s);
+                            this.$$.on_disconnect = t.map(i).filter(u);
                             for (const t in this.$$.slotted) this.appendChild(this.$$.slotted[t])
                         }
                         attributeChangedCallback(t, n, e) {
                             this[t] = e
                         }
                         disconnectedCallback() {
-                            u(this.$$.on_disconnect)
+                            s(this.$$.on_disconnect)
                         }
                         $destroy() {
                             ct(this, 1), this.$destroy = r
                         }
                         $on(t, n) {
                             const e = this.$$.callbacks[t] || (this.$$.callbacks[t] = []);
                             return e.push(n), () => {
                                 const t = e.indexOf(n); - 1 !== t && e.splice(t, 1)
                             }
                         }
                         $set(t) {
                             this.$$set && !d(t) && (this.$$.skip_bound = !0, this.$$set(t), this.$$.skip_bound = !1)
                         }
                     });
-                    class st {
+                    class ut {
                         $destroy() {
                             ct(this, 1), this.$destroy = r
                         }
                         $on(t, n) {
                             const e = this.$$.callbacks[t] || (this.$$.callbacks[t] = []);
                             return e.push(n), () => {
                                 const t = e.indexOf(n); - 1 !== t && e.splice(t, 1)
@@ -1085,18 +1085,18 @@
                             }
                         }
                         return {
                             set: c,
                             update: function(n) {
                                 c(n(t))
                             },
-                            subscribe: function(o, u = r.ZTd) {
-                                const s = [o, u];
-                                return i.add(s), 1 === i.size && (e = n(c) || r.ZTd), o(t), () => {
-                                    i.delete(s), 0 === i.size && (e(), e = null)
+                            subscribe: function(o, s = r.ZTd) {
+                                const u = [o, s];
+                                return i.add(u), 1 === i.size && (e = n(c) || r.ZTd), o(t), () => {
+                                    i.delete(u), 0 === i.size && (e(), e = null)
                                 }
                             }
                         }
                     }
                 },
                 6043: function(t, n, e) {
                     async function r(t) {
@@ -1162,36 +1162,36 @@
                     if ("object" == typeof window) return window
                 }
             }(), o.o = function(t, n) {
                 return Object.prototype.hasOwnProperty.call(t, n)
             }, t = {}, n = "appyter-js:", o.l = function(e, r, i, c) {
                 if (t[e]) t[e].push(r);
                 else {
-                    var u, s;
+                    var s, u;
                     if (void 0 !== i)
                         for (var a = document.getElementsByTagName("script"), l = 0; l < a.length; l++) {
                             var f = a[l];
                             if (f.getAttribute("src") == e || f.getAttribute("data-webpack") == n + i) {
-                                u = f;
+                                s = f;
                                 break
                             }
                         }
-                    u || (s = !0, (u = document.createElement("script")).charset = "utf-8", u.timeout = 120, o.nc && u.setAttribute("nonce", o.nc), u.setAttribute("data-webpack", n + i), u.src = e), t[e] = [r];
+                    s || (u = !0, (s = document.createElement("script")).charset = "utf-8", s.timeout = 120, o.nc && s.setAttribute("nonce", o.nc), s.setAttribute("data-webpack", n + i), s.src = e), t[e] = [r];
                     var d = function(n, r) {
-                            u.onerror = u.onload = null, clearTimeout(p);
+                            s.onerror = s.onload = null, clearTimeout(p);
                             var o = t[e];
-                            if (delete t[e], u.parentNode && u.parentNode.removeChild(u), o && o.forEach((function(t) {
+                            if (delete t[e], s.parentNode && s.parentNode.removeChild(s), o && o.forEach((function(t) {
                                     return t(r)
                                 })), n) return n(r)
                         },
                         p = setTimeout(d.bind(null, void 0, {
                             type: "timeout",
-                            target: u
+                            target: s
                         }), 12e4);
-                    u.onerror = d.bind(null, u.onerror), u.onload = d.bind(null, u.onload), s && document.head.appendChild(u)
+                    s.onerror = d.bind(null, s.onerror), s.onload = d.bind(null, s.onload), u && document.head.appendChild(s)
                 }
             }, o.r = function(t) {
                 "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(t, Symbol.toStringTag, {
                     value: "Module"
                 }), Object.defineProperty(t, "__esModule", {
                     value: !0
                 })
@@ -1208,46 +1208,46 @@
                         if (r) e.push(r[2]);
                         else {
                             var i = new Promise((function(e, o) {
                                 r = t[n] = [e, o]
                             }));
                             e.push(r[2] = i);
                             var c = o.p + o.u(n),
-                                u = new Error;
+                                s = new Error;
                             o.l(c, (function(e) {
                                 if (o.o(t, n) && (0 !== (r = t[n]) && (t[n] = void 0), r)) {
                                     var i = e && ("load" === e.type ? "missing" : e.type),
                                         c = e && e.target && e.target.src;
-                                    u.message = "Loading chunk " + n + " failed.\n(" + i + ": " + c + ")", u.name = "ChunkLoadError", u.type = i, u.request = c, r[1](u)
+                                    s.message = "Loading chunk " + n + " failed.\n(" + i + ": " + c + ")", s.name = "ChunkLoadError", s.type = i, s.request = c, r[1](s)
                                 }
                             }), "chunk-" + n, n)
                         }
                 };
                 var n = function(n, e) {
                         var r, i, c = e[0],
-                            u = e[1],
-                            s = e[2],
+                            s = e[1],
+                            u = e[2],
                             a = 0;
                         if (c.some((function(n) {
                                 return 0 !== t[n]
                             }))) {
-                            for (r in u) o.o(u, r) && (o.m[r] = u[r]);
-                            s && s(o)
+                            for (r in s) o.o(s, r) && (o.m[r] = s[r]);
+                            u && u(o)
                         }
                         for (n && n(e); a < c.length; a++) i = c[a], o.o(t, i) && t[i] && t[i][0](), t[i] = 0
                     },
                     e = self.webpackChunkappyter_js = self.webpackChunkappyter_js || [];
                 e.forEach(n.bind(null, 0)), e.push = n.bind(null, e.push.bind(e))
             }();
         var i = {};
         return o.p = `${window._config.STATIC}/`,
             function() {
                 o.r(i), o.d(i, {
                     default: function() {
-                        return C
+                        return S
                     }
                 });
                 var t = o(8826),
                     n = o(3608),
                     e = o(1782),
                     r = o(7909);
 
@@ -1269,78 +1269,78 @@
                         },
                         d(n) {
                             (0, t.vpE)(r, n)
                         }
                     }
                 }
 
-                function u(n) {
+                function s(n) {
                     let e, r, o, i;
-                    const c = [a, s],
-                        u = [];
+                    const c = [a, u],
+                        s = [];
 
                     function l(t, n) {
                         return t[1] ? 0 : 1
                     }
-                    return e = l(n), r = u[e] = c[e](n), {
+                    return e = l(n), r = s[e] = c[e](n), {
                         c() {
                             r.c(), o = (0, t.cSb)()
                         },
                         m(n, r) {
-                            u[e].m(n, r), (0, t.$Tr)(n, o, r), i = !0
+                            s[e].m(n, r), (0, t.$Tr)(n, o, r), i = !0
                         },
                         p(n, i) {
-                            let s = e;
-                            e = l(n), e === s ? u[e].p(n, i) : ((0, t.dvw)(), (0, t.etI)(u[s], 1, 1, (() => {
-                                u[s] = null
-                            })), (0, t.gbL)(), r = u[e], r ? r.p(n, i) : (r = u[e] = c[e](n), r.c()), (0, t.Ui)(r, 1), r.m(o.parentNode, o))
+                            let u = e;
+                            e = l(n), e === u ? s[e].p(n, i) : ((0, t.dvw)(), (0, t.etI)(s[u], 1, 1, (() => {
+                                s[u] = null
+                            })), (0, t.gbL)(), r = s[e], r ? r.p(n, i) : (r = s[e] = c[e](n), r.c()), (0, t.Ui)(r, 1), r.m(o.parentNode, o))
                         },
                         i(n) {
                             i || ((0, t.Ui)(r), i = !0)
                         },
                         o(n) {
                             (0, t.etI)(r), i = !1
                         },
                         d(n) {
-                            u[e].d(n), n && (0, t.ogt)(o)
+                            s[e].d(n), n && (0, t.ogt)(o)
                         }
                     }
                 }
 
-                function s(n) {
+                function u(n) {
                     let e, r, o;
                     const i = [n[0]];
                     var c = n[2];
 
-                    function u(n) {
+                    function s(n) {
                         let e = {};
                         for (let n = 0; n < i.length; n += 1) e = (0, t.f0i)(e, i[n]);
                         return {
                             props: e
                         }
                     }
-                    return c && (e = new c(u())), {
+                    return c && (e = new c(s())), {
                         c() {
                             e && (0, t.YCL)(e.$$.fragment), r = (0, t.cSb)()
                         },
                         m(n, i) {
                             e && (0, t.yef)(e, n, i), (0, t.$Tr)(n, r, i), o = !0
                         },
                         p(n, o) {
-                            const s = 1 & o ? (0, t.LoY)(i, [(0, t.gCg)(n[0])]) : {};
+                            const u = 1 & o ? (0, t.LoY)(i, [(0, t.gCg)(n[0])]) : {};
                             if (c !== (c = n[2])) {
                                 if (e) {
                                     (0, t.dvw)();
                                     const n = e;
                                     (0, t.etI)(n.$$.fragment, 1, 0, (() => {
                                         (0, t.vpE)(n, 1)
                                     })), (0, t.gbL)()
                                 }
-                                c ? (e = new c(u()), (0, t.YCL)(e.$$.fragment), (0, t.Ui)(e.$$.fragment, 1), (0, t.yef)(e, r.parentNode, r)) : e = null
-                            } else c && e.$set(s)
+                                c ? (e = new c(s()), (0, t.YCL)(e.$$.fragment), (0, t.Ui)(e.$$.fragment, 1), (0, t.yef)(e, r.parentNode, r)) : e = null
+                            } else c && e.$set(u)
                         },
                         i(n) {
                             o || (e && (0, t.Ui)(e.$$.fragment, n), o = !0)
                         },
                         o(n) {
                             e && (0, t.etI)(e.$$.fragment, n), o = !1
                         },
@@ -1351,50 +1351,50 @@
                 }
 
                 function a(n) {
                     let e, r, o;
                     const i = [n[0]];
                     var c = n[2];
 
-                    function u(n) {
+                    function s(n) {
                         let e = {
                             $$slots: {
                                 default: [l]
                             },
                             $$scope: {
                                 ctx: n
                             }
                         };
                         for (let n = 0; n < i.length; n += 1) e = (0, t.f0i)(e, i[n]);
                         return {
                             props: e
                         }
                     }
-                    return c && (e = new c(u(n))), {
+                    return c && (e = new c(s(n))), {
                         c() {
                             e && (0, t.YCL)(e.$$.fragment), r = (0, t.cSb)()
                         },
                         m(n, i) {
                             e && (0, t.yef)(e, n, i), (0, t.$Tr)(n, r, i), o = !0
                         },
                         p(n, o) {
-                            const s = 1 & o ? (0, t.LoY)(i, [(0, t.gCg)(n[0])]) : {};
-                            if (32 & o && (s.$$scope = {
+                            const u = 1 & o ? (0, t.LoY)(i, [(0, t.gCg)(n[0])]) : {};
+                            if (32 & o && (u.$$scope = {
                                     dirty: o,
                                     ctx: n
                                 }), c !== (c = n[2])) {
                                 if (e) {
                                     (0, t.dvw)();
                                     const n = e;
                                     (0, t.etI)(n.$$.fragment, 1, 0, (() => {
                                         (0, t.vpE)(n, 1)
                                     })), (0, t.gbL)()
                                 }
-                                c ? (e = new c(u(n)), (0, t.YCL)(e.$$.fragment), (0, t.Ui)(e.$$.fragment, 1), (0, t.yef)(e, r.parentNode, r)) : e = null
-                            } else c && e.$set(s)
+                                c ? (e = new c(s(n)), (0, t.YCL)(e.$$.fragment), (0, t.Ui)(e.$$.fragment, 1), (0, t.yef)(e, r.parentNode, r)) : e = null
+                            } else c && e.$set(u)
                         },
                         i(n) {
                             o || (e && (0, t.Ui)(e.$$.fragment, n), o = !0)
                         },
                         o(n) {
                             e && (0, t.etI)(e.$$.fragment, n), o = !1
                         },
@@ -1428,32 +1428,32 @@
                             o && o.d(t)
                         }
                     }
                 }
 
                 function f(n) {
                     let e, r, o, i;
-                    const s = [u, c],
+                    const u = [s, c],
                         a = [];
 
                     function l(t, n) {
                         return void 0 !== t[2] ? 0 : 1
                     }
-                    return e = l(n), r = a[e] = s[e](n), {
+                    return e = l(n), r = a[e] = u[e](n), {
                         c() {
                             r.c(), o = (0, t.cSb)()
                         },
                         m(n, r) {
                             a[e].m(n, r), (0, t.$Tr)(n, o, r), i = !0
                         },
                         p(n, [i]) {
                             let c = e;
                             e = l(n), e === c ? a[e].p(n, i) : ((0, t.dvw)(), (0, t.etI)(a[c], 1, 1, (() => {
                                 a[c] = null
-                            })), (0, t.gbL)(), r = a[e], r ? r.p(n, i) : (r = a[e] = s[e](n), r.c()), (0, t.Ui)(r, 1), r.m(o.parentNode, o))
+                            })), (0, t.gbL)(), r = a[e], r ? r.p(n, i) : (r = a[e] = u[e](n), r.c()), (0, t.Ui)(r, 1), r.m(o.parentNode, o))
                         },
                         i(n) {
                             i || ((0, t.Ui)(r), i = !0)
                         },
                         o(n) {
                             (0, t.etI)(r), i = !1
                         },
@@ -1465,127 +1465,128 @@
 
                 function d(n, e, r) {
                     let o, {
                             $$slots: i = {},
                             $$scope: c
                         } = e,
                         {
-                            module: u
+                            module: s
                         } = e,
                         {
-                            props: s = {}
+                            props: u = {}
                         } = e,
                         {
                             children: a = !1
                         } = e;
-                    return (0, t.H3E)((() => u().then((({
+                    return (0, t.H3E)((() => s().then((({
                         default: t
                     }) => r(2, o = t))).catch((t => console.error(t))))), n.$$set = t => {
-                        "module" in t && r(3, u = t.module), "props" in t && r(0, s = t.props), "children" in t && r(1, a = t.children), "$$scope" in t && r(5, c = t.$$scope)
-                    }, [s, a, o, u, i, c]
+                        "module" in t && r(3, s = t.module), "props" in t && r(0, u = t.props), "children" in t && r(1, a = t.children), "$$scope" in t && r(5, c = t.$$scope)
+                    }, [u, a, o, s, i, c]
                 }
                 class p extends t.f_C {
                     constructor(n) {
                         super(), (0, t.S1n)(this, n, d, f, t.N8, {
                             module: 3,
                             props: 0,
                             children: 1
                         })
                     }
                 }
                 var m = p;
-                var g = o(6043);
+                var g = o(6043),
+                    $ = o(9666);
 
-                function $(t, n, e) {
+                function h(t, n, e) {
                     const r = t.slice();
-                    return r[9] = n[e], r
+                    return r[11] = n[e], r
                 }
 
-                function h(e) {
+                function b(e) {
                     let r, o;
                     return r = new n.default({
                         props: {
                             args: {
                                 name: "_primary",
                                 section: null,
                                 title: "Appyter",
                                 subtitle: "Customize your notebook",
                                 icon: "cogs"
                             },
-                            fields: e[3].map(e[5])
+                            fields: e[3].map(e[6])
                         }
                     }), {
                         c() {
                             (0, t.YCL)(r.$$.fragment)
                         },
                         m(n, e) {
                             (0, t.yef)(r, n, e), o = !0
                         },
                         p(t, n) {
                             const e = {};
-                            10 & n && (e.fields = t[3].map(t[5])), r.$set(e)
+                            10 & n && (e.fields = t[3].map(t[6])), r.$set(e)
                         },
                         i(n) {
                             o || ((0, t.Ui)(r.$$.fragment, n), o = !0)
                         },
                         o(n) {
                             (0, t.etI)(r.$$.fragment, n), o = !1
                         },
                         d(n) {
                             (0, t.vpE)(r, n)
                         }
                     }
                 }
 
-                function b(e) {
+                function y(e) {
                     let r, o;
 
                     function i(...t) {
-                        return e[6](e[9], ...t)
+                        return e[7](e[11], ...t)
                     }
                     return r = new n.default({
                         props: {
-                            args: e[9].args,
-                            fields: e[0].filter(i).map(e[7])
+                            args: e[11].args,
+                            fields: e[0].filter(i).map(e[8])
                         }
                     }), {
                         c() {
                             (0, t.YCL)(r.$$.fragment)
                         },
                         m(n, e) {
                             (0, t.yef)(r, n, e), o = !0
                         },
                         p(t, n) {
                             e = t;
                             const o = {};
-                            1 & n && (o.args = e[9].args), 3 & n && (o.fields = e[0].filter(i).map(e[7])), r.$set(o)
+                            1 & n && (o.args = e[11].args), 3 & n && (o.fields = e[0].filter(i).map(e[8])), r.$set(o)
                         },
                         i(n) {
                             o || ((0, t.Ui)(r.$$.fragment, n), o = !0)
                         },
                         o(n) {
                             (0, t.etI)(r.$$.fragment, n), o = !1
                         },
                         d(n) {
                             (0, t.vpE)(r, n)
                         }
                     }
                 }
 
-                function y(n) {
-                    let e, r, o = "SectionField" === n[9].field && b(n);
+                function v(n) {
+                    let e, r, o = "SectionField" === n[11].field && y(n);
                     return {
                         c() {
                             o && o.c(), e = (0, t.cSb)()
                         },
                         m(n, i) {
                             o && o.m(n, i), (0, t.$Tr)(n, e, i), r = !0
                         },
                         p(n, r) {
-                            "SectionField" === n[9].field ? o ? (o.p(n, r), 1 & r && (0, t.Ui)(o, 1)) : (o = b(n), o.c(), (0, t.Ui)(o, 1), o.m(e.parentNode, e)) : o && ((0, t.dvw)(), (0, t.etI)(o, 1, 1, (() => {
+                            "SectionField" === n[11].field ? o ? (o.p(n, r), 1 & r && (0, t.Ui)(o, 1)) : (o = y(n), o.c(), (0, t.Ui)(o, 1), o.m(e.parentNode, e)) : o && ((0, t.dvw)(), (0, t.etI)(o, 1, 1, (() => {
                                 o = null
                             })), (0, t.gbL)())
                         },
                         i(n) {
                             r || ((0, t.Ui)(o), r = !0)
                         },
                         o(n) {
@@ -1593,15 +1594,15 @@
                         },
                         d(n) {
                             o && o.d(n), n && (0, t.ogt)(e)
                         }
                     }
                 }
 
-                function v(n) {
+                function w(n) {
                     let e, r, o = n[1].message + "";
                     return {
                         c() {
                             e = (0, t.bGB)("div"), r = (0, t.fLW)(o), (0, t.Ljt)(e, "class", "col-sm-12 alert alert-danger")
                         },
                         m(n, o) {
                             (0, t.$Tr)(n, e, o), (0, t.R3I)(e, r)
@@ -1611,15 +1612,15 @@
                         },
                         d(n) {
                             n && (0, t.ogt)(e)
                         }
                     }
                 }
 
-                function w(n) {
+                function L(n) {
                     let e;
                     return {
                         c() {
                             e = (0, t.bGB)("input"), (0, t.Ljt)(e, "class", "btn navigate white border-custom bg-blue nodecoration"), (0, t.Ljt)(e, "type", "submit"), e.value = "Submit"
                         },
                         m(n, r) {
                             (0, t.$Tr)(n, e, r)
@@ -1628,15 +1629,15 @@
                         o: t.ZTd,
                         d(n) {
                             n && (0, t.ogt)(e)
                         }
                     }
                 }
 
-                function L(n) {
+                function j(n) {
                     let r, o;
                     return r = new e.Z({}), {
                         c() {
                             (0, t.YCL)(r.$$.fragment)
                         },
                         m(n, e) {
                             (0, t.yef)(r, n, e), o = !0
@@ -1649,28 +1650,28 @@
                         },
                         d(n) {
                             (0, t.vpE)(r, n)
                         }
                     }
                 }
 
-                function j(n) {
-                    let e, r, o, i, c, u, s, a, l, f, d, p, g, b, j = -1 !== window._config.EXTRAS.indexOf("catalog-integration"),
-                        T = n[3].length > 0 && h(n),
-                        k = n[0].filter(I),
+                function T(n) {
+                    let e, r, o, i, c, s, u, a, l, f, d, p, g, $, y = -1 !== window._config.EXTRAS.indexOf("catalog-integration"),
+                        T = n[3].length > 0 && b(n),
+                        I = n[0].filter(_),
                         x = [];
-                    for (let t = 0; t < k.length; t += 1) x[t] = y($(n, k, t));
+                    for (let t = 0; t < I.length; t += 1) x[t] = v(h(n, I, t));
                     const C = n => (0, t.etI)(x[n], 1, 1, (() => {
                         x[n] = null
                     }));
-                    let S = j && function(n) {
+                    let S = y && function(n) {
                             let e, r;
                             return e = new m({
                                 props: {
-                                    module: _
+                                    module: k
                                 }
                             }), {
                                 c() {
                                     (0, t.YCL)(e.$$.fragment)
                                 },
                                 m(n, o) {
                                     (0, t.yef)(e, n, o), r = !0
@@ -1682,140 +1683,158 @@
                                     (0, t.etI)(e.$$.fragment, n), r = !1
                                 },
                                 d(n) {
                                     (0, t.vpE)(e, n)
                                 }
                             }
                         }(),
-                        E = void 0 !== n[1] && "FieldConstraintException" !== n[1].cls && v(n);
-                    const U = [L, w],
+                        E = void 0 !== n[1] && "FieldConstraintException" !== n[1].cls && w(n);
+                    const U = [j, L],
                         R = [];
 
                     function O(t, n) {
                         return t[2] ? 0 : 1
                     }
                     return f = O(n), d = R[f] = U[f](n), {
                         c() {
                             e = (0, t.bGB)("form"), T && T.c(), r = (0, t.DhX)();
                             for (let t = 0; t < x.length; t += 1) x[t].c();
-                            o = (0, t.DhX)(), S && S.c(), i = (0, t.DhX)(), c = (0, t.bGB)("div"), u = (0, t.bGB)("div"), u.textContent = " ", s = (0, t.DhX)(), E && E.c(), a = (0, t.DhX)(), l = (0, t.bGB)("div"), d.c(), (0, t.Ljt)(u, "class", "col-sm-12"), (0, t.Ljt)(l, "class", "col-sm-12 text-center"), (0, t.Ljt)(c, "class", "row"), (0, t.Ljt)(e, "method", "POST"), (0, t.Ljt)(e, "enctype", "multipart/form-data"), (0, t.Ljt)(e, "action", "#")
+                            o = (0, t.DhX)(), S && S.c(), i = (0, t.DhX)(), c = (0, t.bGB)("div"), s = (0, t.bGB)("div"), s.textContent = " ", u = (0, t.DhX)(), E && E.c(), a = (0, t.DhX)(), l = (0, t.bGB)("div"), d.c(), (0, t.Ljt)(s, "class", "col-sm-12"), (0, t.Ljt)(l, "class", "col-sm-12 text-center"), (0, t.Ljt)(c, "class", "row"), (0, t.Ljt)(e, "method", "POST"), (0, t.Ljt)(e, "enctype", "multipart/form-data"), (0, t.Ljt)(e, "action", "#")
                         },
                         m(d, m) {
                             (0, t.$Tr)(d, e, m), T && T.m(e, null), (0, t.R3I)(e, r);
                             for (let t = 0; t < x.length; t += 1) x[t].m(e, null);
-                            (0, t.R3I)(e, o), S && S.m(e, null), (0, t.R3I)(e, i), (0, t.R3I)(e, c), (0, t.R3I)(c, u), (0, t.R3I)(c, s), E && E.m(c, null), (0, t.R3I)(c, a), (0, t.R3I)(c, l), R[f].m(l, null), p = !0, g || (b = (0, t.oLt)(e, "submit", (0, t.AT7)(n[4])), g = !0)
+                            (0, t.R3I)(e, o), S && S.m(e, null), (0, t.R3I)(e, i), (0, t.R3I)(e, c), (0, t.R3I)(c, s), (0, t.R3I)(c, u), E && E.m(c, null), (0, t.R3I)(c, a), (0, t.R3I)(c, l), R[f].m(l, null), p = !0, g || ($ = (0, t.oLt)(e, "submit", (0, t.AT7)(n[9])), g = !0)
                         },
                         p(n, [i]) {
-                            if (n[3].length > 0 ? T ? (T.p(n, i), 8 & i && (0, t.Ui)(T, 1)) : (T = h(n), T.c(), (0, t.Ui)(T, 1), T.m(e, r)) : T && ((0, t.dvw)(), (0, t.etI)(T, 1, 1, (() => {
+                            if (n[3].length > 0 ? T ? (T.p(n, i), 8 & i && (0, t.Ui)(T, 1)) : (T = b(n), T.c(), (0, t.Ui)(T, 1), T.m(e, r)) : T && ((0, t.dvw)(), (0, t.etI)(T, 1, 1, (() => {
                                     T = null
                                 })), (0, t.gbL)()), 3 & i) {
                                 let r;
-                                for (k = n[0].filter(I), r = 0; r < k.length; r += 1) {
-                                    const c = $(n, k, r);
-                                    x[r] ? (x[r].p(c, i), (0, t.Ui)(x[r], 1)) : (x[r] = y(c), x[r].c(), (0, t.Ui)(x[r], 1), x[r].m(e, o))
+                                for (I = n[0].filter(_), r = 0; r < I.length; r += 1) {
+                                    const c = h(n, I, r);
+                                    x[r] ? (x[r].p(c, i), (0, t.Ui)(x[r], 1)) : (x[r] = v(c), x[r].c(), (0, t.Ui)(x[r], 1), x[r].m(e, o))
                                 }
-                                for ((0, t.dvw)(), r = k.length; r < x.length; r += 1) C(r);
+                                for ((0, t.dvw)(), r = I.length; r < x.length; r += 1) C(r);
                                 (0, t.gbL)()
                             }
-                            void 0 !== n[1] && "FieldConstraintException" !== n[1].cls ? E ? E.p(n, i) : (E = v(n), E.c(), E.m(c, a)) : E && (E.d(1), E = null);
-                            let u = f;
-                            f = O(n), f !== u && ((0, t.dvw)(), (0, t.etI)(R[u], 1, 1, (() => {
-                                R[u] = null
+                            void 0 !== n[1] && "FieldConstraintException" !== n[1].cls ? E ? E.p(n, i) : (E = w(n), E.c(), E.m(c, a)) : E && (E.d(1), E = null);
+                            let s = f;
+                            f = O(n), f !== s && ((0, t.dvw)(), (0, t.etI)(R[s], 1, 1, (() => {
+                                R[s] = null
                             })), (0, t.gbL)(), d = R[f], d || (d = R[f] = U[f](n), d.c()), (0, t.Ui)(d, 1), d.m(l, null))
                         },
                         i(n) {
                             if (!p) {
                                 (0, t.Ui)(T);
-                                for (let n = 0; n < k.length; n += 1)(0, t.Ui)(x[n]);
+                                for (let n = 0; n < I.length; n += 1)(0, t.Ui)(x[n]);
                                 (0, t.Ui)(S), (0, t.Ui)(d), p = !0
                             }
                         },
                         o(n) {
                             (0, t.etI)(T), x = x.filter(Boolean);
                             for (let n = 0; n < x.length; n += 1)(0, t.etI)(x[n]);
                             (0, t.etI)(S), (0, t.etI)(d), p = !1
                         },
                         d(n) {
-                            n && (0, t.ogt)(e), T && T.d(), (0, t.RMB)(x, n), S && S.d(), E && E.d(), R[f].d(), g = !1, b()
+                            n && (0, t.ogt)(e), T && T.d(), (0, t.RMB)(x, n), S && S.d(), E && E.d(), R[f].d(), g = !1, $()
                         }
                     }
                 }
 
-                function T(t, n) {
+                function I(t, n) {
                     return void 0 !== n && "FieldConstraintException" === n.cls && t.args.name === n.field_name && (t.error = n), t
                 }
-                const I = t => "section" === t.type,
-                    _ = () => o.e(58).then(o.bind(o, 9058));
+                const _ = t => "section" === t.type,
+                    k = () => o.e(58).then(o.bind(o, 9058));
 
-                function k(n, e, o) {
-                    let i;
-                    (0, t.FIv)(n, r.Z, (t => o(8, i = t)));
-                    let c, u, {
-                            fields: s = []
+                function x(n, e, o) {
+                    let i, c;
+                    (0, t.FIv)(n, $.Z, (t => o(5, i = t))), (0, t.FIv)(n, r.Z, (t => o(10, c = t)));
+                    let s, u, {
+                            fields: a = []
                         } = e,
-                        a = !1;
-                    return n.$$set = t => {
-                        "fields" in t && o(0, s = t.fields)
-                    }, n.$$.update = () => {
-                        1 & n.$$.dirty && o(3, u = s.filter((t => "section" !== t.type && !t.args.section))), 2 & n.$$.dirty && c && console.error(c)
-                    }, [s, c, a, u, async function(t) {
+                        l = !1;
+                    async function f(t) {
                         try {
-                            o(2, a = !0);
-                            const n = new FormData(t.target),
-                                e = await fetch(window.location.href, {
-                                    method: "POST",
-                                    headers: {
-                                        Accept: "application/json",
-                                        ...await (0, g.Z)(i)
-                                    },
-                                    body: n
-                                });
-                            if (406 === e.status) {
+                            o(2, l = !0);
+                            const n = await fetch(window.location.href, {
+                                method: "POST",
+                                headers: {
+                                    Accept: "application/json",
+                                    ...await (0, g.Z)(c)
+                                },
+                                body: t
+                            });
+                            if (406 === n.status) {
                                 const {
                                     error: t
-                                } = await e.json();
-                                o(1, c = t)
+                                } = await n.json();
+                                o(1, s = t)
                             } else {
                                 const {
                                     _id: t,
-                                    _storage: n,
+                                    _storage: e,
                                     _executor: r
-                                } = await e.json();
-                                o(1, c = void 0), window.location.href = function(t) {
+                                } = await n.json();
+                                o(1, s = void 0), window.location.href = function(t) {
                                     let {
                                         path: n,
                                         params: e
                                     } = t || {};
                                     null == n && (n = "");
                                     const r = function(t) {
                                         return void 0 === t ? "" : Object.keys(t).filter((n => void 0 !== t[n] && "" !== t[n])).map((n => [n, t[n]].map(encodeURIComponent).join("="))).join("&")
                                     }(e);
                                     return "" === r ? n : `${n}?${r}`
                                 }({
                                     path: `${window._config.ORIGIN}/${t}/`,
                                     params: {
-                                        storage: n,
+                                        storage: e,
                                         executor: r
                                     }
                                 })
                             }
                         } catch (t) {
-                            o(1, c = {
+                            o(1, s = {
                                 cls: "FrontendException",
                                 message: t.toString()
                             })
                         } finally {
-                            o(2, a = !1)
+                            o(2, l = !1)
+                        }
+                    }
+                    return n.$$set = t => {
+                        "fields" in t && o(0, a = t.fields)
+                    }, n.$$.update = () => {
+                        if (1 & n.$$.dirty && o(3, u = a.filter((t => "section" !== t.type && !t.args.section))), 2 & n.$$.dirty && s && console.error(s), 33 & n.$$.dirty && a && i.params) {
+                            const t = {
+                                    ...i.params
+                                },
+                                n = function(t) {
+                                    const n = {};
+                                    for (const e in t) {
+                                        const r = /^args\.(.+)$/.exec(e);
+                                        null !== r && (n[r[1]] = t[e])
+                                    }
+                                    return n
+                                }(t);
+                            for (const t of a) t.args.name in n && (t.args.default = n[t.args.name]);
+                            if (!0 === t.submit) {
+                                const t = new FormData;
+                                for (const e in n) t.append(e, n[e]);
+                                f(t)
+                            }
                         }
-                    }, t => T(t, c), (t, n) => n.args.section === t.args.name, t => T(t, c)]
+                    }, [a, s, l, u, f, i, t => I(t, s), (t, n) => n.args.section === t.args.name, t => I(t, s), t => f(new FormData(t.target))]
                 }
-                class x extends t.f_C {
+                class C extends t.f_C {
                     constructor(n) {
-                        super(), (0, t.S1n)(this, n, k, j, t.N8, {
+                        super(), (0, t.S1n)(this, n, x, T, t.N8, {
                             fields: 0
                         })
                     }
                 }
-                var C = x
+                var S = C
             }(), i
     }()
 }));
```

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/js/index.js` & `appyter-0.19.9/appyter/static/profiles/biojupies/js/index.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/js/lib/bootstrap.js` & `appyter-0.19.9/appyter/static/profiles/biojupies/js/lib/bootstrap.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-brands-400.eot` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-brands-400.svg` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-brands-400.ttf` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-brands-400.woff` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-brands-400.woff2` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-regular-400.eot` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-regular-400.svg` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-regular-400.ttf` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-regular-400.woff` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-regular-400.woff2` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-solid-900.eot` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-solid-900.svg` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-solid-900.ttf` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-solid-900.woff` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/biojupies/webfonts/fa-solid-900.woff2` & `appyter-0.19.9/appyter/static/profiles/biojupies/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/bootstrap/css/index.css` & `appyter-0.19.9/appyter/static/profiles/bootstrap/css/index.css`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/bootstrap/js/index.js` & `appyter-0.19.9/appyter/static/profiles/bootstrap/js/index.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/css/index.css` & `appyter-0.19.9/appyter/static/profiles/default/css/index.css`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/chunks/229.js` & `appyter-0.19.9/appyter/static/profiles/default/js/chunks/229.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/chunks/246.js` & `appyter-0.19.9/appyter/static/profiles/default/js/chunks/246.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -311,15 +311,15 @@
                     },
                     d(t) {
                         t && (0, o.ogt)(e)
                     }
                 }
             }
 
-            function x(t) {
+            function R(t) {
                 let e, n = "file" === t[12].type && I(t);
                 return {
                     c() {
                         n && n.c(), e = (0, o.cSb)()
                     },
                     m(t, c) {
                         n && n.m(t, c), (0, o.$Tr)(t, e, c)
@@ -329,15 +329,15 @@
                     },
                     d(t) {
                         n && n.d(t), t && (0, o.ogt)(e)
                     }
                 }
             }
 
-            function R(t) {
+            function x(t) {
                 let e, n;
                 return e = new l.Z({}), {
                     c() {
                         (0, o.YCL)(e.$$.fragment)
                     },
                     m(t, c) {
                         (0, o.yef)(e, t, c), n = !0
@@ -458,15 +458,15 @@
                     },
                     d(t) {
                         t && (0, o.ogt)(e)
                     }
                 }
             }
 
-            function D(t) {
+            function U(t) {
                 let e, n = "file" === t[12].type && G(t);
                 return {
                     c() {
                         n && n.c(), e = (0, o.cSb)()
                     },
                     m(t, c) {
                         n && n.m(t, c), (0, o.$Tr)(t, e, c)
@@ -476,61 +476,61 @@
                     },
                     d(t) {
                         n && n.d(t), t && (0, o.ogt)(e)
                     }
                 }
             }
 
-            function U(t) {
-                let e, n, c, l, r, m, $, L, I, T, k, B, G, z, Z, U, X, C, S, W, O, N, M, _, E, Y, F, H, P, V, A, q, J, K, Q = t[0].label + "",
+            function C(t) {
+                let e, n, c, l, r, m, $, L, I, T, k, B, G, z, Z, C, D, X, S, W, O, N, M, _, E, Y, F, H, P, V, A, q, J, K, Q = t[0].label + "",
                     tt = t[0].description && p(t),
                     et = t[5] !== t[2] && g(),
                     nt = t[3][t[2]] || [],
                     ot = [];
                 for (let e = 0; e < nt.length; e += 1) ot[e] = h(f(t, nt, e));
                 let ct = t[3][t[2]] || [],
                     lt = [];
                 for (let e = 0; e < ct.length; e += 1) lt[e] = b(d(t, ct, e));
                 let rt = t[5] !== t[2] && y(t),
                     it = t[3][t[2]] || [],
                     at = [];
                 for (let e = 0; e < it.length; e += 1) at[e] = w(u(t, it, e));
                 let st = t[3][t[2]] || [],
                     ut = [];
-                for (let e = 0; e < st.length; e += 1) ut[e] = x(s(t, st, e));
-                let dt = t[4] && R(),
+                for (let e = 0; e < st.length; e += 1) ut[e] = R(s(t, st, e));
+                let dt = t[4] && x(),
                     ft = t[5] !== t[2] && v(),
                     pt = t[3][t[2]] || [],
                     gt = [];
                 for (let e = 0; e < pt.length; e += 1) gt[e] = j(a(t, pt, e));
                 let mt = t[3][t[2]] || [],
                     ht = [];
-                for (let e = 0; e < mt.length; e += 1) ht[e] = D(i(t, mt, e));
+                for (let e = 0; e < mt.length; e += 1) ht[e] = U(i(t, mt, e));
                 return {
                     c() {
                         e = (0, o.bGB)("div"), n = (0, o.bGB)("div"), c = (0, o.fLW)(Q), l = (0, o.DhX)(), tt && tt.c(), r = (0, o.fLW)(":"), m = (0, o.DhX)(), $ = (0, o.bGB)("div"), L = (0, o.bGB)("div"), I = (0, o.bGB)("div"), et && et.c(), T = (0, o.DhX)(), k = (0, o.bGB)("span"), k.innerHTML = '<i class="far fa-folder-open"></i>', B = (0, o.DhX)();
                         for (let t = 0; t < ot.length; t += 1) ot[t].c();
                         G = (0, o.DhX)();
                         for (let t = 0; t < lt.length; t += 1) lt[t].c();
-                        z = (0, o.DhX)(), Z = (0, o.bGB)("div"), rt && rt.c(), U = (0, o.DhX)(), X = (0, o.bGB)("button"), C = (0, o.fLW)(". "), S = (0, o.fLW)(t[2]), W = (0, o.DhX)();
+                        z = (0, o.DhX)(), Z = (0, o.bGB)("div"), rt && rt.c(), C = (0, o.DhX)(), D = (0, o.bGB)("button"), X = (0, o.fLW)(". "), S = (0, o.fLW)(t[2]), W = (0, o.DhX)();
                         for (let t = 0; t < at.length; t += 1) at[t].c();
                         O = (0, o.DhX)();
                         for (let t = 0; t < ut.length; t += 1) ut[t].c();
                         N = (0, o.DhX)(), dt && dt.c(), M = (0, o.DhX)(), _ = (0, o.bGB)("div"), ft && ft.c(), E = (0, o.DhX)(), Y = (0, o.bGB)("span"), Y.textContent = " ", F = (0, o.DhX)();
                         for (let t = 0; t < gt.length; t += 1) gt[t].c();
                         H = (0, o.DhX)();
                         for (let t = 0; t < ht.length; t += 1) ht[t].c();
-                        P = (0, o.DhX)(), V = (0, o.bGB)("input"), (0, o.Ljt)(n, "class", "col-lg-3 bold text-lg-right my-auto"), (0, o.czc)(I, "display", "flex"), (0, o.czc)(I, "flex-direction", "column"), (0, o.czc)(I, "align-items", "center"), (0, o.czc)(I, "padding-right", "5px"), (0, o.Ljt)(X, "type", "button"), (0, o.Ljt)(X, "class", "text-btn"), (0, o.czc)(Z, "display", "flex"), (0, o.czc)(Z, "flex-direction", "column"), (0, o.czc)(Z, "align-items", "start"), (0, o.czc)(Z, "white-space", "nowrap"), (0, o.czc)(Z, "overflow-x", "auto"), (0, o.czc)(Z, "flex", "1 1 auto"), (0, o.czc)(_, "display", "flex"), (0, o.czc)(_, "flex-direction", "column"), (0, o.czc)(_, "align-items", "start"), (0, o.czc)(_, "padding-left", "5px"), (0, o.czc)(L, "display", "flex"), (0, o.czc)(L, "flex-direction", "row"), (0, o.czc)(L, "max-height", "500px"), (0, o.czc)(L, "overflow-x", "hidden"), (0, o.czc)(L, "overflow-y", "auto"), (0, o.Ljt)(L, "class", "pl-0"), (0, o.Ljt)(V, "type", "text"), (0, o.czc)(V, "display", "none"), (0, o.Ljt)(V, "name", A = t[0].name), (0, o.Ljt)($, "class", "col-lg-6 pt-2 pt-lg-0"), (0, o.Ljt)(e, "class", "row px-4 px-lg-3 pb-4")
+                        P = (0, o.DhX)(), V = (0, o.bGB)("input"), (0, o.Ljt)(n, "class", "col-lg-3 bold text-lg-right my-auto"), (0, o.czc)(I, "display", "flex"), (0, o.czc)(I, "flex-direction", "column"), (0, o.czc)(I, "align-items", "center"), (0, o.czc)(I, "padding-right", "5px"), (0, o.Ljt)(D, "type", "button"), (0, o.Ljt)(D, "class", "text-btn"), (0, o.czc)(Z, "display", "flex"), (0, o.czc)(Z, "flex-direction", "column"), (0, o.czc)(Z, "align-items", "start"), (0, o.czc)(Z, "white-space", "nowrap"), (0, o.czc)(Z, "overflow-x", "auto"), (0, o.czc)(Z, "flex", "1 1 auto"), (0, o.czc)(_, "display", "flex"), (0, o.czc)(_, "flex-direction", "column"), (0, o.czc)(_, "align-items", "start"), (0, o.czc)(_, "padding-left", "5px"), (0, o.czc)(L, "display", "flex"), (0, o.czc)(L, "flex-direction", "row"), (0, o.czc)(L, "max-height", "500px"), (0, o.czc)(L, "overflow-x", "hidden"), (0, o.czc)(L, "overflow-y", "auto"), (0, o.Ljt)(L, "class", "pl-0"), (0, o.Ljt)(V, "type", "text"), (0, o.czc)(V, "display", "none"), (0, o.Ljt)(V, "name", A = t[0].name), (0, o.Ljt)($, "class", "col-lg-6 pt-2 pt-lg-0"), (0, o.Ljt)(e, "class", "row px-4 px-lg-3 pb-4")
                     },
                     m(i, a) {
                         (0, o.$Tr)(i, e, a), (0, o.R3I)(e, n), (0, o.R3I)(n, c), (0, o.R3I)(n, l), tt && tt.m(n, null), (0, o.R3I)(n, r), (0, o.R3I)(e, m), (0, o.R3I)(e, $), (0, o.R3I)($, L), (0, o.R3I)(L, I), et && et.m(I, null), (0, o.R3I)(I, T), (0, o.R3I)(I, k), (0, o.R3I)(I, B);
                         for (let t = 0; t < ot.length; t += 1) ot[t].m(I, null);
                         (0, o.R3I)(I, G);
                         for (let t = 0; t < lt.length; t += 1) lt[t].m(I, null);
-                        (0, o.R3I)(L, z), (0, o.R3I)(L, Z), rt && rt.m(Z, null), (0, o.R3I)(Z, U), (0, o.R3I)(Z, X), (0, o.R3I)(X, C), (0, o.R3I)(X, S), (0, o.R3I)(Z, W);
+                        (0, o.R3I)(L, z), (0, o.R3I)(L, Z), rt && rt.m(Z, null), (0, o.R3I)(Z, C), (0, o.R3I)(Z, D), (0, o.R3I)(D, X), (0, o.R3I)(D, S), (0, o.R3I)(Z, W);
                         for (let t = 0; t < at.length; t += 1) at[t].m(Z, null);
                         (0, o.R3I)(Z, O);
                         for (let t = 0; t < ut.length; t += 1) ut[t].m(Z, null);
                         (0, o.R3I)(Z, N), dt && dt.m(Z, null), (0, o.R3I)(L, M), (0, o.R3I)(L, _), ft && ft.m(_, null), (0, o.R3I)(_, E), (0, o.R3I)(_, Y), (0, o.R3I)(_, F);
                         for (let t = 0; t < gt.length; t += 1) gt[t].m(_, null);
                         (0, o.R3I)(_, H);
                         for (let t = 0; t < ht.length; t += 1) ht[t].m(_, null);
@@ -551,48 +551,48 @@
                             for (ct = t[3][t[2]] || [], n = 0; n < ct.length; n += 1) {
                                 const o = d(t, ct, n);
                                 lt[n] ? lt[n].p(o, e) : (lt[n] = b(o), lt[n].c(), lt[n].m(I, null))
                             }
                             for (; n < lt.length; n += 1) lt[n].d(1);
                             lt.length = ct.length
                         }
-                        if (t[5] !== t[2] ? rt ? rt.p(t, e) : (rt = y(t), rt.c(), rt.m(Z, U)) : rt && (rt.d(1), rt = null), (!q || 4 & e) && (0, o.rTO)(S, t[2]), 12 & e) {
+                        if (t[5] !== t[2] ? rt ? rt.p(t, e) : (rt = y(t), rt.c(), rt.m(Z, C)) : rt && (rt.d(1), rt = null), (!q || 4 & e) && (0, o.rTO)(S, t[2]), 12 & e) {
                             let n;
                             for (it = t[3][t[2]] || [], n = 0; n < it.length; n += 1) {
                                 const o = u(t, it, n);
                                 at[n] ? at[n].p(o, e) : (at[n] = w(o), at[n].c(), at[n].m(Z, O))
                             }
                             for (; n < at.length; n += 1) at[n].d(1);
                             at.length = it.length
                         }
                         if (14 & e) {
                             let n;
                             for (st = t[3][t[2]] || [], n = 0; n < st.length; n += 1) {
                                 const o = s(t, st, n);
-                                ut[n] ? ut[n].p(o, e) : (ut[n] = x(o), ut[n].c(), ut[n].m(Z, N))
+                                ut[n] ? ut[n].p(o, e) : (ut[n] = R(o), ut[n].c(), ut[n].m(Z, N))
                             }
                             for (; n < ut.length; n += 1) ut[n].d(1);
                             ut.length = st.length
                         }
-                        if (t[4] ? dt ? 16 & e && (0, o.Ui)(dt, 1) : (dt = R(), dt.c(), (0, o.Ui)(dt, 1), dt.m(Z, null)) : dt && ((0, o.dvw)(), (0, o.etI)(dt, 1, 1, (() => {
+                        if (t[4] ? dt ? 16 & e && (0, o.Ui)(dt, 1) : (dt = x(), dt.c(), (0, o.Ui)(dt, 1), dt.m(Z, null)) : dt && ((0, o.dvw)(), (0, o.etI)(dt, 1, 1, (() => {
                                 dt = null
                             })), (0, o.gbL)()), t[5] !== t[2] ? ft || (ft = v(), ft.c(), ft.m(_, E)) : ft && (ft.d(1), ft = null), 12 & e) {
                             let n;
                             for (pt = t[3][t[2]] || [], n = 0; n < pt.length; n += 1) {
                                 const o = a(t, pt, n);
                                 gt[n] ? gt[n].p(o, e) : (gt[n] = j(o), gt[n].c(), gt[n].m(_, H))
                             }
                             for (; n < gt.length; n += 1) gt[n].d(1);
                             gt.length = pt.length
                         }
                         if (14 & e) {
                             let n;
                             for (mt = t[3][t[2]] || [], n = 0; n < mt.length; n += 1) {
                                 const o = i(t, mt, n);
-                                ht[n] ? ht[n].p(o, e) : (ht[n] = D(o), ht[n].c(), ht[n].m(_, null))
+                                ht[n] ? ht[n].p(o, e) : (ht[n] = U(o), ht[n].c(), ht[n].m(_, null))
                             }
                             for (; n < ht.length; n += 1) ht[n].d(1);
                             ht.length = mt.length
                         }(!q || 1 & e && A !== (A = t[0].name)) && (0, o.Ljt)(V, "name", A), 1 & e && V.value !== t[0].value && (0, o.BmG)(V, t[0].value)
                     },
                     i(t) {
                         q || ((0, o.Ui)(dt), q = !0)
@@ -602,15 +602,15 @@
                     },
                     d(t) {
                         t && (0, o.ogt)(e), tt && tt.d(), et && et.d(), (0, o.RMB)(ot, t), (0, o.RMB)(lt, t), rt && rt.d(), (0, o.RMB)(at, t), (0, o.RMB)(ut, t), dt && dt.d(), ft && ft.d(), (0, o.RMB)(gt, t), (0, o.RMB)(ht, t), J = !1, K()
                     }
                 }
             }
 
-            function X(t, e, n) {
+            function D(t, e, n) {
                 let l;
                 (0, o.FIv)(t, c.Z, (t => n(7, l = t)));
                 let {
                     args: r
                 } = e, {
                     backend: i = "StorageFileField"
                 } = e, a = r.value || r.default || "", s = !1, u = "", d = "", f = {};
@@ -638,23 +638,23 @@
                     n(2, u = t.name)
                 }, t => {
                     n(1, a = t.name)
                 }, function() {
                     r.value = this.value, n(0, r), n(1, a)
                 }]
             }
-            class C extends o.f_C {
+            class X extends o.f_C {
                 constructor(t) {
-                    super(), (0, o.S1n)(this, t, X, U, o.N8, {
+                    super(), (0, o.S1n)(this, t, D, C, o.N8, {
                         args: 0,
                         backend: 6
                     })
                 }
             }
-            var S = C,
+            var S = X,
                 W = n(3798);
 
             function O(t) {
                 let e, n, c, l, r, i, a, s;
                 const u = [E, _, M],
                     d = [];
 
@@ -943,15 +943,15 @@
                 }; {
                     const [n, o] = [t.slice(0, e), t.slice(e + 1)];
                     return {
                         path: n,
                         params: function(t) {
                             return "" === t ? {} : t.split("&").map((t => t.split("=").map(decodeURIComponent))).reduce(((t, [e, n]) => ({
                                 ...t,
-                                [e]: n
+                                [e]: void 0 === n || n
                             })), {})
                         }(o)
                     }
                 }
             }
 
             function l() {
@@ -981,15 +981,15 @@
                     server: n
                 }) => {
                     const o = function({
                         path: t,
                         params: e
                     }) {
                         const n = function(t) {
-                            return Object.keys(t).filter((e => void 0 !== t[e] && "" !== t[e])).map((e => [e, t[e]].map(encodeURIComponent).join("="))).join("&")
+                            return Object.keys(t).filter((e => void 0 !== t[e] && "" !== t[e])).map((e => !0 === t[e] ? encodeURIComponent(e) : [e, t[e]].map(encodeURIComponent).join("="))).join("&")
                         }(e);
                         return "" === n ? t : `${t}?${n}`
                     }({
                         path: t,
                         params: e
                     });
                     if (t !== s) window.location.hash = o, s = t;
```

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/chunks/29.js` & `appyter-0.19.9/appyter/static/profiles/default/js/chunks/29.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/chunks/316.js` & `appyter-0.19.9/appyter/static/profiles/default/js/chunks/316.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -537,17 +537,17 @@
             class O extends r.f_C {
                 constructor(t) {
                     super(), (0, r.S1n)(this, t, D, R, r.N8, {
                         data: 0
                     })
                 }
             }
-            var X = O;
+            var H = O;
 
-            function H(t) {
+            function X(t) {
                 let e, n;
                 return e = new N({
                     props: {
                         classes: "output_svg",
                         data: B(t[0])
                     }
                 }), {
@@ -579,15 +579,15 @@
                 } = e;
                 return t.$$set = t => {
                     "data" in t && n(0, r = t.data)
                 }, [r]
             }
             class W extends r.f_C {
                 constructor(t) {
-                    super(), (0, r.S1n)(this, t, M, H, r.N8, {
+                    super(), (0, r.S1n)(this, t, M, X, r.N8, {
                         data: 0
                     })
                 }
             }
             var A = W;
 
             function V(t) {
@@ -795,15 +795,15 @@
                     super(), (0, r.S1n)(this, t, ct, it, r.N8, {
                         data: 1
                     })
                 }
             }
             const lt = {
                     "image/svg+xml": A,
-                    "image/png": X,
+                    "image/png": H,
                     "text/html": q,
                     "application/javascript": k,
                     "text/markdown": K,
                     "text/plain": ut
                 },
                 dt = {
                     "application/vnd.bokehjs_load.v0+json": !0,
@@ -1309,15 +1309,15 @@
                     },
                     d(t) {
                         t && (0, r.ogt)(n), e && (0, r.vpE)(e, t)
                     }
                 }
             }
 
-            function Xt(t) {
+            function Ht(t) {
                 let e, n, a = t[0] && Rt(t);
                 return {
                     c() {
                         a && a.c(), e = (0, r.cSb)()
                     },
                     m(t, o) {
                         a && a.m(t, o), (0, r.$Tr)(t, e, o), n = !0
@@ -1335,15 +1335,15 @@
                     },
                     d(t) {
                         a && a.d(t), t && (0, r.ogt)(e)
                     }
                 }
             }
 
-            function Ht(t, e, n) {
+            function Xt(t, e, n) {
                 let {
                     data: r
                 } = e;
                 return t.$$set = t => {
                     "data" in t && n(0, r = t.data)
                 }, [r, function() {
                     const t = {
@@ -1355,138 +1355,137 @@
                         }
                     };
                     return j(t), JSON.stringify(t)
                 }]
             }
             class Mt extends r.f_C {
                 constructor(t) {
-                    super(), (0, r.S1n)(this, t, Ht, Xt, r.N8, {
+                    super(), (0, r.S1n)(this, t, Xt, Ht, r.N8, {
                         data: 0
                     })
                 }
             }
             var Wt = Mt,
                 At = n(1782);
 
             function Vt(t, e, n) {
                 const r = t.slice();
                 return r[4] = e[n], r
             }
 
-            function Jt(t) {
-                let e, n, a, o, s, i;
-                return n = new L({
+            function Jt(t, e) {
+                let n, a, o, s, i, c;
+                return a = new L({
                     props: {
-                        index: t[1] + "-loader",
+                        index: e[1] + "-" + e[4].index,
                         prompt_type: "output"
                     }
-                }), s = new At.Z({}), {
+                }), i = new Wt({
+                    props: {
+                        data: e[4]
+                    }
+                }), {
+                    key: t,
+                    first: null,
                     c() {
-                        e = (0, r.bGB)("div"), (0, r.YCL)(n.$$.fragment), a = (0, r.DhX)(), o = (0, r.bGB)("div"), (0, r.YCL)(s.$$.fragment), (0, r.Ljt)(o, "class", "output_subarea"), (0, r.Ljt)(e, "class", "output_area")
+                        n = (0, r.bGB)("div"), (0, r.YCL)(a.$$.fragment), o = (0, r.DhX)(), s = (0, r.bGB)("div"), (0, r.YCL)(i.$$.fragment), (0, r.Ljt)(s, "class", "output_subarea"), (0, r.Ljt)(n, "class", "output_area"), this.first = n
                     },
-                    m(t, c) {
-                        (0, r.$Tr)(t, e, c), (0, r.yef)(n, e, null), (0, r.R3I)(e, a), (0, r.R3I)(e, o), (0, r.yef)(s, o, null), i = !0
+                    m(t, e) {
+                        (0, r.$Tr)(t, n, e), (0, r.yef)(a, n, null), (0, r.R3I)(n, o), (0, r.R3I)(n, s), (0, r.yef)(i, s, null), c = !0
                     },
-                    p(t, e) {
+                    p(t, n) {
+                        e = t;
                         const r = {};
-                        2 & e && (r.index = t[1] + "-loader"), n.$set(r)
+                        3 & n && (r.index = e[1] + "-" + e[4].index), a.$set(r);
+                        const o = {};
+                        1 & n && (o.data = e[4]), i.$set(o)
                     },
                     i(t) {
-                        i || ((0, r.Ui)(n.$$.fragment, t), (0, r.Ui)(s.$$.fragment, t), i = !0)
+                        c || ((0, r.Ui)(a.$$.fragment, t), (0, r.Ui)(i.$$.fragment, t), c = !0)
                     },
                     o(t) {
-                        (0, r.etI)(n.$$.fragment, t), (0, r.etI)(s.$$.fragment, t), i = !1
+                        (0, r.etI)(a.$$.fragment, t), (0, r.etI)(i.$$.fragment, t), c = !1
                     },
                     d(t) {
-                        t && (0, r.ogt)(e), (0, r.vpE)(n), (0, r.vpE)(s)
+                        t && (0, r.ogt)(n), (0, r.vpE)(a), (0, r.vpE)(i)
                     }
                 }
             }
 
-            function zt(t, e) {
-                let n, a, o, s, i, c, u;
-                return a = new L({
+            function zt(t) {
+                let e, n, a, o, s, i;
+                return n = new L({
                     props: {
-                        index: e[1] + "-" + e[4].index,
+                        index: t[1] + "-loader",
                         prompt_type: "output"
                     }
-                }), i = new Wt({
-                    props: {
-                        data: e[4]
-                    }
-                }), {
-                    key: t,
-                    first: null,
+                }), s = new At.Z({}), {
                     c() {
-                        n = (0, r.bGB)("div"), (0, r.YCL)(a.$$.fragment), o = (0, r.DhX)(), s = (0, r.bGB)("div"), (0, r.YCL)(i.$$.fragment), c = (0, r.DhX)(), (0, r.Ljt)(s, "class", "output_subarea"), (0, r.Ljt)(n, "class", "output_area"), this.first = n
+                        e = (0, r.bGB)("div"), (0, r.YCL)(n.$$.fragment), a = (0, r.DhX)(), o = (0, r.bGB)("div"), (0, r.YCL)(s.$$.fragment), (0, r.Ljt)(o, "class", "output_subarea"), (0, r.Ljt)(e, "class", "output_area")
                     },
-                    m(t, e) {
-                        (0, r.$Tr)(t, n, e), (0, r.yef)(a, n, null), (0, r.R3I)(n, o), (0, r.R3I)(n, s), (0, r.yef)(i, s, null), (0, r.R3I)(n, c), u = !0
+                    m(t, c) {
+                        (0, r.$Tr)(t, e, c), (0, r.yef)(n, e, null), (0, r.R3I)(e, a), (0, r.R3I)(e, o), (0, r.yef)(s, o, null), i = !0
                     },
-                    p(t, n) {
-                        e = t;
+                    p(t, e) {
                         const r = {};
-                        3 & n && (r.index = e[1] + "-" + e[4].index), a.$set(r);
-                        const o = {};
-                        1 & n && (o.data = e[4]), i.$set(o)
+                        2 & e && (r.index = t[1] + "-loader"), n.$set(r)
                     },
                     i(t) {
-                        u || ((0, r.Ui)(a.$$.fragment, t), (0, r.Ui)(i.$$.fragment, t), u = !0)
+                        i || ((0, r.Ui)(n.$$.fragment, t), (0, r.Ui)(s.$$.fragment, t), i = !0)
                     },
                     o(t) {
-                        (0, r.etI)(a.$$.fragment, t), (0, r.etI)(i.$$.fragment, t), u = !1
+                        (0, r.etI)(n.$$.fragment, t), (0, r.etI)(s.$$.fragment, t), i = !1
                     },
                     d(t) {
-                        t && (0, r.ogt)(n), (0, r.vpE)(a), (0, r.vpE)(i)
+                        t && (0, r.ogt)(e), (0, r.vpE)(n), (0, r.vpE)(s)
                     }
                 }
             }
 
             function qt(t) {
                 let e, n, a, o, s = [],
                     i = new Map,
-                    c = t[1] === t[2] && Jt(t),
-                    u = [...t[3](t[0])];
-                const l = t => t[4].index;
-                for (let e = 0; e < u.length; e += 1) {
-                    let n = Vt(t, u, e),
-                        r = l(n);
-                    i.set(r, s[e] = zt(r, n))
+                    c = [...t[3](t[0])];
+                const u = t => t[4].index;
+                for (let e = 0; e < c.length; e += 1) {
+                    let n = Vt(t, c, e),
+                        r = u(n);
+                    i.set(r, s[e] = Jt(r, n))
                 }
+                let l = t[1] === t[2] && zt(t);
                 return {
                     c() {
-                        e = (0, r.bGB)("div"), n = (0, r.bGB)("div"), c && c.c(), a = (0, r.DhX)();
+                        e = (0, r.bGB)("div"), n = (0, r.bGB)("div");
                         for (let t = 0; t < s.length; t += 1) s[t].c();
-                        (0, r.Ljt)(n, "class", "output"), (0, r.Ljt)(e, "class", "output_wrapper")
+                        a = (0, r.DhX)(), l && l.c(), (0, r.Ljt)(n, "class", "output"), (0, r.Ljt)(e, "class", "output_wrapper")
                     },
                     m(t, i) {
-                        (0, r.$Tr)(t, e, i), (0, r.R3I)(e, n), c && c.m(n, null), (0, r.R3I)(n, a);
+                        (0, r.$Tr)(t, e, i), (0, r.R3I)(e, n);
                         for (let t = 0; t < s.length; t += 1) s[t].m(n, null);
-                        o = !0
+                        (0, r.R3I)(n, a), l && l.m(n, null), o = !0
                     },
                     p(t, [e]) {
-                        t[1] === t[2] ? c ? (c.p(t, e), 6 & e && (0, r.Ui)(c, 1)) : (c = Jt(t), c.c(), (0, r.Ui)(c, 1), c.m(n, a)) : c && ((0, r.dvw)(), (0, r.etI)(c, 1, 1, (() => {
-                            c = null
-                        })), (0, r.gbL)()), 11 & e && (u = [...t[3](t[0])], (0, r.dvw)(), s = (0, r.GQg)(s, e, l, 1, t, u, i, n, r.cly, zt, null, Vt), (0, r.gbL)())
+                        11 & e && (c = [...t[3](t[0])], (0, r.dvw)(), s = (0, r.GQg)(s, e, u, 1, t, c, i, n, r.cly, Jt, a, Vt), (0, r.gbL)()), t[1] === t[2] ? l ? (l.p(t, e), 6 & e && (0, r.Ui)(l, 1)) : (l = zt(t), l.c(), (0, r.Ui)(l, 1), l.m(n, null)) : l && ((0, r.dvw)(), (0, r.etI)(l, 1, 1, (() => {
+                            l = null
+                        })), (0, r.gbL)())
                     },
                     i(t) {
                         if (!o) {
-                            (0, r.Ui)(c);
-                            for (let t = 0; t < u.length; t += 1)(0, r.Ui)(s[t]);
-                            o = !0
+                            for (let t = 0; t < c.length; t += 1)(0, r.Ui)(s[t]);
+                            (0, r.Ui)(l), o = !0
                         }
                     },
                     o(t) {
-                        (0, r.etI)(c);
                         for (let t = 0; t < s.length; t += 1)(0, r.etI)(s[t]);
-                        o = !1
+                        (0, r.etI)(l), o = !1
                     },
                     d(t) {
-                        t && (0, r.ogt)(e), c && c.d();
-                        for (let t = 0; t < s.length; t += 1) s[t].d()
+                        t && (0, r.ogt)(e);
+                        for (let t = 0; t < s.length; t += 1) s[t].d();
+                        l && l.d()
                     }
                 }
             }
 
             function Ft(t, e, n) {
                 let {
                     data: r = []
@@ -1513,18 +1512,15 @@
                                 const t = B(r.text, "\n");
                                 t.startsWith("\r") ? n[r.name].text = t : n[r.name].text += t
                             }
                     else yield {
                         ...r,
                         index: e++
                     };
-                    for (const t in n) n[t].text = n[t].text.replace(/^\r/, "").replace(/(\r?\n)+$/, ""), n[t].text && (yield {
-                        ...n[t],
-                        index: e++
-                    })
+                    for (const t in n) n[t].text = n[t].text.replace(/^\r/, "").replace(/(\r?\n)+$/, ""), n[t].text && (yield n[t])
                 }]
             }
             class Pt extends r.f_C {
                 constructor(t) {
                     super(), (0, r.S1n)(this, t, Ft, qt, r.N8, {
                         data: 0,
                         index: 1,
```

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/chunks/322.js` & `appyter-0.19.9/appyter/static/profiles/default/js/chunks/322.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/chunks/494.js` & `appyter-0.19.9/appyter/static/profiles/default/js/chunks/494.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/chunks/58.js` & `appyter-0.19.9/appyter/static/profiles/default/js/chunks/58.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/chunks/671.js` & `appyter-0.19.9/appyter/static/profiles/default/js/chunks/671.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/chunks/680.js` & `appyter-0.19.9/appyter/static/profiles/default/js/chunks/680.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/chunks/755.js` & `appyter-0.19.9/appyter/static/profiles/default/js/chunks/755.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/chunks/798.js` & `appyter-0.19.9/appyter/static/profiles/default/js/chunks/798.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/chunks/826.js` & `appyter-0.19.9/appyter/static/profiles/default/js/chunks/826.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/chunks/849.js` & `appyter-0.19.9/appyter/static/profiles/default/js/chunks/849.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/chunks/977.js` & `appyter-0.19.9/appyter/static/profiles/default/js/chunks/977.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -460,15 +460,15 @@
                 }; {
                     const [n, r] = [e.slice(0, t), e.slice(t + 1)];
                     return {
                         path: n,
                         params: function(e) {
                             return "" === e ? {} : e.split("&").map((e => e.split("=").map(decodeURIComponent))).reduce(((e, [t, n]) => ({
                                 ...e,
-                                [t]: n
+                                [t]: void 0 === n || n
                             })), {})
                         }(r)
                     }
                 }
             }
 
             function a() {
@@ -498,15 +498,15 @@
                     server: n
                 }) => {
                     const r = function({
                         path: e,
                         params: t
                     }) {
                         const n = function(e) {
-                            return Object.keys(e).filter((t => void 0 !== e[t] && "" !== e[t])).map((t => [t, e[t]].map(encodeURIComponent).join("="))).join("&")
+                            return Object.keys(e).filter((t => void 0 !== e[t] && "" !== e[t])).map((t => !0 === e[t] ? encodeURIComponent(t) : [t, e[t]].map(encodeURIComponent).join("="))).join("&")
                         }(t);
                         return "" === n ? e : `${e}?${n}`
                     }({
                         path: e,
                         params: t
                     });
                     if (e !== c) window.location.hash = r, c = e;
```

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/fields/AutocompleteField.js` & `appyter-0.19.9/appyter/static/profiles/default/js/fields/AutocompleteField.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -643,48 +643,47 @@
                 function dt(t) {
                     const e = {};
                     for (const n of t) e[n] = !0;
                     return e
                 }
 
                 function ft(t, e, n) {
-                    let o, r, l, i, {
-                            args: c
+                    let o, r, l, i, c, {
+                            args: s
                         } = e,
-                        s = c.default,
                         u = -1;
                     var d;
                     return d = async () => {
                             try {
-                                if (void 0 !== c.file_path) {
-                                    const t = await fetch(c.file_path),
+                                if (void 0 !== s.file_path) {
+                                    const t = await fetch(s.file_path),
                                         e = await t.json();
                                     if ("object" != typeof e) throw new Error("Unrecognized type for downloaded file");
-                                    Array.isArray(e) ? n(2, l = dt(e)) : (console.warn("Legacy mode... please use an array"), n(2, l = dt(e[Object.keys(e)[0]])))
+                                    Array.isArray(e) ? n(2, i = dt(e)) : (console.warn("Legacy mode... please use an array"), n(2, i = dt(e[Object.keys(e)[0]])))
                                 } else {
-                                    if (void 0 === c.choices) throw new Error("No autocomplete item source");
-                                    if ("object" != typeof c.choices) throw new Error("Unrecognized type for choices");
-                                    Array.isArray(c.choices) ? n(2, l = dt(c.choices)) : n(2, l = c.choices)
+                                    if (void 0 === s.choices) throw new Error("No autocomplete item source");
+                                    if ("object" != typeof s.choices) throw new Error("Unrecognized type for choices");
+                                    Array.isArray(s.choices) ? n(2, i = dt(s.choices)) : n(2, i = s.choices)
                                 }
                             } catch (t) {
                                 n(4, r = "Failed to load autocomplete items"), console.error(t)
                             }
                         },
                         function() {
                             if (!a) throw new Error("Function called outside component initialization");
                             return a
                         }().$$.on_mount.push(d), t.$$set = t => {
-                            "args" in t && n(0, c = t.args)
+                            "args" in t && n(0, s = t.args)
                         }, t.$$.update = () => {
-                            6 & t.$$.dirty && void 0 !== l && (n(6, i = Object.keys(l).filter((t => t.toLowerCase().substr(0, s.length) === s.toLowerCase() && t !== s)).slice(0, 7)), n(5, u = -1))
-                        }, [c, s, l, o, r, u, i, function() {
-                            s = this.value, n(1, s)
+                            3 & t.$$.dirty && void 0 !== s && void 0 === l && n(1, l = s.default), 6 & t.$$.dirty && void 0 !== i && (n(6, c = Object.keys(i).filter((t => t.toLowerCase().substr(0, l.length) === l.toLowerCase() && t !== l)).slice(0, 7)), n(5, u = -1))
+                        }, [s, l, i, o, r, u, c, function() {
+                            l = this.value, n(1, l), n(0, s)
                         }, () => n(3, o = !0), () => n(3, o = !1), t => {
-                            "ArrowUp" === t.key ? (t.preventDefault(), n(5, u = Math.max(-1, u - 1))) : "ArrowDown" === t.key ? (t.preventDefault(), n(5, u = Math.min(i.length - 1, u + 1))) : "Enter" === t.key && (t.preventDefault(), u >= 0 && n(1, s = i[u]), n(5, u = -1))
-                        }, t => n(1, s = t), t => n(1, s = c.examples[t])]
+                            "ArrowUp" === t.key ? (t.preventDefault(), n(5, u = Math.max(-1, u - 1))) : "ArrowDown" === t.key ? (t.preventDefault(), n(5, u = Math.min(c.length - 1, u + 1))) : "Enter" === t.key && (t.preventDefault(), u >= 0 && n(1, l = c[u]), n(5, u = -1))
+                        }, t => n(1, l = t), t => n(1, l = s.examples[t])]
                 }
                 var pt = class extends J {
                     constructor(t) {
                         super(), G(this, t, ft, ut, c, {
                             args: 0
                         }, W)
                     }
```

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/fields/FileField.js` & `appyter-0.19.9/appyter/static/profiles/default/js/fields/FileField.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -34,30 +34,30 @@
                                 (0, o.vpE)(n, t)
                             }
                         }
                     }
 
                     function u(t) {
                         let n, e, r, i;
-                        const c = [l, s],
+                        const c = [f, s],
                             u = [];
 
-                        function f(t, n) {
+                        function l(t, n) {
                             return t[1] ? 0 : 1
                         }
-                        return n = f(t), e = u[n] = c[n](t), {
+                        return n = l(t), e = u[n] = c[n](t), {
                             c() {
                                 e.c(), r = (0, o.cSb)()
                             },
                             m(t, e) {
                                 u[n].m(t, e), (0, o.$Tr)(t, r, e), i = !0
                             },
                             p(t, i) {
                                 let s = n;
-                                n = f(t), n === s ? u[n].p(t, i) : ((0, o.dvw)(), (0, o.etI)(u[s], 1, 1, (() => {
+                                n = l(t), n === s ? u[n].p(t, i) : ((0, o.dvw)(), (0, o.etI)(u[s], 1, 1, (() => {
                                     u[s] = null
                                 })), (0, o.gbL)(), e = u[n], e ? e.p(t, i) : (e = u[n] = c[n](t), e.c()), (0, o.Ui)(e, 1), e.m(r.parentNode, r))
                             },
                             i(t) {
                                 i || ((0, o.Ui)(e), i = !0)
                             },
                             o(t) {
@@ -109,23 +109,23 @@
                             },
                             d(t) {
                                 t && (0, o.ogt)(e), n && (0, o.vpE)(n, t)
                             }
                         }
                     }
 
-                    function l(t) {
+                    function f(t) {
                         let n, e, r;
                         const i = [t[0]];
                         var c = t[2];
 
                         function u(t) {
                             let n = {
                                 $$slots: {
-                                    default: [f]
+                                    default: [l]
                                 },
                                 $$scope: {
                                     ctx: t
                                 }
                             };
                             for (let t = 0; t < i.length; t += 1) n = (0, o.f0i)(n, i[t]);
                             return {
@@ -163,15 +163,15 @@
                             },
                             d(t) {
                                 t && (0, o.ogt)(e), n && (0, o.vpE)(n, t)
                             }
                         }
                     }
 
-                    function f(t) {
+                    function l(t) {
                         let n;
                         const e = t[4].default,
                             r = (0, o.nuO)(e, t, t[5], null);
                         return {
                             c() {
                                 r && r.c()
                             },
@@ -192,40 +192,40 @@
                             }
                         }
                     }
 
                     function a(t) {
                         let n, e, r, i;
                         const s = [u, c],
-                            l = [];
+                            f = [];
 
-                        function f(t, n) {
+                        function l(t, n) {
                             return void 0 !== t[2] ? 0 : 1
                         }
-                        return n = f(t), e = l[n] = s[n](t), {
+                        return n = l(t), e = f[n] = s[n](t), {
                             c() {
                                 e.c(), r = (0, o.cSb)()
                             },
                             m(t, e) {
-                                l[n].m(t, e), (0, o.$Tr)(t, r, e), i = !0
+                                f[n].m(t, e), (0, o.$Tr)(t, r, e), i = !0
                             },
                             p(t, [i]) {
                                 let c = n;
-                                n = f(t), n === c ? l[n].p(t, i) : ((0, o.dvw)(), (0, o.etI)(l[c], 1, 1, (() => {
-                                    l[c] = null
-                                })), (0, o.gbL)(), e = l[n], e ? e.p(t, i) : (e = l[n] = s[n](t), e.c()), (0, o.Ui)(e, 1), e.m(r.parentNode, r))
+                                n = l(t), n === c ? f[n].p(t, i) : ((0, o.dvw)(), (0, o.etI)(f[c], 1, 1, (() => {
+                                    f[c] = null
+                                })), (0, o.gbL)(), e = f[n], e ? e.p(t, i) : (e = f[n] = s[n](t), e.c()), (0, o.Ui)(e, 1), e.m(r.parentNode, r))
                             },
                             i(t) {
                                 i || ((0, o.Ui)(e), i = !0)
                             },
                             o(t) {
                                 (0, o.etI)(e), i = !1
                             },
                             d(t) {
-                                l[n].d(t), t && (0, o.ogt)(r)
+                                f[n].d(t), t && (0, o.ogt)(r)
                             }
                         }
                     }
 
                     function d(t, n, e) {
                         let o, {
                                 $$slots: i = {},
@@ -234,21 +234,21 @@
                             {
                                 module: u
                             } = n,
                             {
                                 props: s = {}
                             } = n,
                             {
-                                children: l = !1
+                                children: f = !1
                             } = n;
                         return (0, r.H3)((() => u().then((({
                             default: t
                         }) => e(2, o = t))).catch((t => console.error(t))))), t.$$set = t => {
-                            "module" in t && e(3, u = t.module), "props" in t && e(0, s = t.props), "children" in t && e(1, l = t.children), "$$scope" in t && e(5, c = t.$$scope)
-                        }, [s, l, o, u, i, c]
+                            "module" in t && e(3, u = t.module), "props" in t && e(0, s = t.props), "children" in t && e(1, f = t.children), "$$scope" in t && e(5, c = t.$$scope)
+                        }, [s, f, o, u, i, c]
                     }
                     class p extends o.f_C {
                         constructor(t) {
                             super(), (0, o.S1n)(this, t, d, a, o.N8, {
                                 module: 3,
                                 props: 0,
                                 children: 1
@@ -312,19 +312,19 @@
                         t.forEach(i)
                     }
 
                     function s(t) {
                         return "function" == typeof t
                     }
 
-                    function l(t, n) {
+                    function f(t, n) {
                         return t != t ? n == n : t !== n || t && "object" == typeof t || "function" == typeof t
                     }
 
-                    function f(t) {
+                    function l(t) {
                         return 0 === Object.keys(t).length
                     }
 
                     function a(t, n, e) {
                         t.$$.on_destroy.push(function(t, ...n) {
                             if (null == t) return o;
                             const e = t.subscribe(...n);
@@ -393,30 +393,30 @@
                         Ljt: function() {
                             return O
                         },
                         LoY: function() {
                             return nt
                         },
                         N8: function() {
-                            return l
+                            return f
                         },
                         R3I: function() {
                             return v
                         },
                         RMB: function() {
                             return w
                         },
                         S1n: function() {
                             return ut
                         },
                         Ui: function() {
                             return Q
                         },
                         VHj: function() {
-                            return S
+                            return R
                         },
                         VOJ: function() {
                             return m
                         },
                         VnY: function() {
                             return G
                         },
@@ -432,15 +432,15 @@
                         bGB: function() {
                             return x
                         },
                         cSb: function() {
                             return T
                         },
                         czc: function() {
-                            return U
+                            return S
                         },
                         dvw: function() {
                             return J
                         },
                         etI: function() {
                             return tt
                         },
@@ -551,23 +551,23 @@
                         n = "" + n, t.wholeText !== n && (t.data = n)
                     }
 
                     function E(t, n) {
                         t.value = null == n ? "" : n
                     }
 
-                    function U(t, n, e, o) {
+                    function S(t, n, e, o) {
                         null === e ? t.style.removeProperty(n) : t.style.setProperty(n, e, o ? "important" : "")
                     }
 
-                    function S(t, n, e) {
+                    function R(t, n, e) {
                         t.classList[e ? "add" : "remove"](n)
                     }
 
-                    function R(t) {
+                    function U(t) {
                         h = t
                     }
 
                     function N(t) {
                         (function() {
                             if (!h) throw new Error("Function called outside component initialization");
                             return h
@@ -592,25 +592,25 @@
                     let X = 0;
 
                     function q() {
                         const t = h;
                         do {
                             for (; X < B.length;) {
                                 const t = B[X];
-                                X++, R(t), V(t.$$)
+                                X++, U(t), V(t.$$)
                             }
-                            for (R(null), B.length = 0, X = 0; G.length;) G.pop()();
+                            for (U(null), B.length = 0, X = 0; G.length;) G.pop()();
                             for (let t = 0; t < A.length; t += 1) {
                                 const n = A[t];
                                 H.has(n) || (H.add(n), n())
                             }
                             A.length = 0
                         } while (B.length);
                         for (; Y.length;) Y.pop()();
-                        M = !1, H.clear(), R(t)
+                        M = !1, H.clear(), U(t)
                     }
 
                     function V(t) {
                         if (null !== t.fragment) {
                             t.update(), u(t.before_update);
                             const n = t.dirty;
                             t.dirty = [-1], t.fragment && t.fragment.p(t.ctx, n), t.after_update.forEach(Z)
@@ -678,50 +678,50 @@
                         t && t.c()
                     }
 
                     function it(t, n, e, o) {
                         const {
                             fragment: r,
                             on_mount: c,
-                            on_destroy: l,
-                            after_update: f
+                            on_destroy: f,
+                            after_update: l
                         } = t.$$;
                         r && r.m(n, e), o || Z((() => {
                             const n = c.map(i).filter(s);
-                            l ? l.push(...n) : u(n), t.$$.on_mount = []
-                        })), f.forEach(Z)
+                            f ? f.push(...n) : u(n), t.$$.on_mount = []
+                        })), l.forEach(Z)
                     }
 
                     function ct(t, n) {
                         const e = t.$$;
                         null !== e.fragment && (u(e.on_destroy), e.fragment && e.fragment.d(n), e.on_destroy = e.fragment = null, e.ctx = [])
                     }
 
-                    function ut(t, n, e, r, i, s, l, f = [-1]) {
+                    function ut(t, n, e, r, i, s, f, l = [-1]) {
                         const a = h;
-                        R(t);
+                        U(t);
                         const d = t.$$ = {
                             fragment: null,
                             ctx: null,
                             props: s,
                             update: o,
                             not_equal: i,
                             bound: c(),
                             on_mount: [],
                             on_destroy: [],
                             on_disconnect: [],
                             before_update: [],
                             after_update: [],
                             context: new Map(n.context || (a ? a.$$.context : [])),
                             callbacks: c(),
-                            dirty: f,
+                            dirty: l,
                             skip_bound: !1,
                             root: n.target || a.$$.root
                         };
-                        l && l(d.root);
+                        f && f(d.root);
                         let p = !1;
                         if (d.ctx = e ? e(t, n.props || {}, ((n, e, ...o) => {
                                 const r = o.length ? o[0] : e;
                                 return d.ctx && i(d.ctx[n], d.ctx[n] = r) && (!d.skip_bound && d.bound[n] && d.bound[n](r), p && function(t, n) {
                                     -1 === t.$$.dirty[0] && (B.push(t), M || (M = !0, P.then(q)), t.$$.dirty.fill(0)), t.$$.dirty[n / 31 | 0] |= 1 << n % 31
                                 }(t, n)), e
                             })) : [], d.update(), p = !0, u(d.before_update), d.fragment = !!r && r(d.ctx), n.target) {
@@ -730,15 +730,15 @@
                                 const t = function(t) {
                                     return Array.from(t.childNodes)
                                 }(n.target);
                                 d.fragment && d.fragment.l(t), t.forEach(L)
                             } else d.fragment && d.fragment.c();
                             n.intro && Q(t.$$.fragment), it(t, n.target, n.anchor, n.customElement), b = !1, q()
                         }
-                        R(a)
+                        U(a)
                     }
                     "undefined" != typeof window ? window : "undefined" != typeof globalThis ? globalThis : global, new Set(["allowfullscreen", "allowpaymentrequest", "async", "autofocus", "autoplay", "checked", "controls", "default", "defer", "disabled", "formnovalidate", "hidden", "ismap", "loop", "multiple", "muted", "nomodule", "novalidate", "open", "playsinline", "readonly", "required", "reversed", "selected"]), "function" == typeof HTMLElement && (W = class extends HTMLElement {
                         constructor() {
                             super(), this.attachShadow({
                                 mode: "open"
                             })
                         }
@@ -761,29 +761,29 @@
                         $on(t, n) {
                             const e = this.$$.callbacks[t] || (this.$$.callbacks[t] = []);
                             return e.push(n), () => {
                                 const t = e.indexOf(n); - 1 !== t && e.splice(t, 1)
                             }
                         }
                         $set(t) {
-                            this.$$set && !f(t) && (this.$$.skip_bound = !0, this.$$set(t), this.$$.skip_bound = !1)
+                            this.$$set && !l(t) && (this.$$.skip_bound = !0, this.$$set(t), this.$$.skip_bound = !1)
                         }
                     });
                     class st {
                         $destroy() {
                             ct(this, 1), this.$destroy = o
                         }
                         $on(t, n) {
                             const e = this.$$.callbacks[t] || (this.$$.callbacks[t] = []);
                             return e.push(n), () => {
                                 const t = e.indexOf(n); - 1 !== t && e.splice(t, 1)
                             }
                         }
                         $set(t) {
-                            this.$$set && !f(t) && (this.$$.skip_bound = !0, this.$$set(t), this.$$.skip_bound = !1)
+                            this.$$set && !l(t) && (this.$$.skip_bound = !0, this.$$set(t), this.$$.skip_bound = !1)
                         }
                     }
                 }
             },
             i = {};
 
         function c(t) {
@@ -838,16 +838,16 @@
             }(), c.o = function(t, n) {
                 return Object.prototype.hasOwnProperty.call(t, n)
             }, e = {}, o = "appyter-js:", c.l = function(t, n, r, i) {
                 if (e[t]) e[t].push(n);
                 else {
                     var u, s;
                     if (void 0 !== r)
-                        for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                            var a = l[f];
+                        for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
+                            var a = f[l];
                             if (a.getAttribute("src") == t || a.getAttribute("data-webpack") == o + r) {
                                 u = a;
                                 break
                             }
                         }
                     u || (s = !0, (u = document.createElement("script")).charset = "utf-8", u.timeout = 120, c.nc && u.setAttribute("nonce", c.nc), u.setAttribute("data-webpack", o + r), u.src = t), e[t] = [n];
                     var d = function(n, o) {
@@ -895,22 +895,22 @@
                             }), "chunk-" + n, n)
                         }
                 };
                 var n = function(n, e) {
                         var o, r, i = e[0],
                             u = e[1],
                             s = e[2],
-                            l = 0;
+                            f = 0;
                         if (i.some((function(n) {
                                 return 0 !== t[n]
                             }))) {
                             for (o in u) c.o(u, o) && (c.m[o] = u[o]);
                             s && s(c)
                         }
-                        for (n && n(e); l < i.length; l++) r = i[l], c.o(t, r) && t[r] && t[r][0](), t[r] = 0
+                        for (n && n(e); f < i.length; f++) r = i[f], c.o(t, r) && t[r] && t[r][0](), t[r] = 0
                     },
                     e = self.webpackChunkappyter_js = self.webpackChunkappyter_js || [];
                 e.forEach(n.bind(null, 0)), e.push = n.bind(null, e.push.bind(e))
             }();
         var u = {};
         return c.p = `${window._config.STATIC}/`,
             function() {
@@ -947,56 +947,56 @@
                         d(n) {
                             n && (0, t.ogt)(e), n && (0, t.ogt)(i)
                         }
                     }
                 }
 
                 function i(n) {
-                    let e, o, r, i, c, u, s, l = n[4] + "";
+                    let e, o, r, i, c, u, s, f = n[4] + "";
 
-                    function f() {
+                    function l() {
                         return n[3](n[4])
                     }
                     return {
                         c() {
-                            e = (0, t.bGB)("button"), o = (0, t.fLW)(l), r = (0, t.DhX)(), (0, t.Ljt)(e, "type", "button"), (0, t.Ljt)(e, "class", i = "nav-link" + (n[0].value === n[4] ? " active" : "")), (0, t.Ljt)(e, "aria-controls", c = "tab-content-" + n[0].name + "-" + n[4]), (0, t.Ljt)(e, "role", "tab")
+                            e = (0, t.bGB)("button"), o = (0, t.fLW)(f), r = (0, t.DhX)(), (0, t.Ljt)(e, "type", "button"), (0, t.Ljt)(e, "class", i = "nav-link" + (n[0].value === n[4] ? " active" : "")), (0, t.Ljt)(e, "aria-controls", c = "tab-content-" + n[0].name + "-" + n[4]), (0, t.Ljt)(e, "role", "tab")
                         },
                         m(n, i) {
-                            (0, t.$Tr)(n, e, i), (0, t.R3I)(e, o), (0, t.R3I)(e, r), u || (s = (0, t.oLt)(e, "click", f), u = !0)
+                            (0, t.$Tr)(n, e, i), (0, t.R3I)(e, o), (0, t.R3I)(e, r), u || (s = (0, t.oLt)(e, "click", l), u = !0)
                         },
                         p(r, u) {
-                            n = r, 1 & u && l !== (l = n[4] + "") && (0, t.rTO)(o, l), 1 & u && i !== (i = "nav-link" + (n[0].value === n[4] ? " active" : "")) && (0, t.Ljt)(e, "class", i), 1 & u && c !== (c = "tab-content-" + n[0].name + "-" + n[4]) && (0, t.Ljt)(e, "aria-controls", c)
+                            n = r, 1 & u && f !== (f = n[4] + "") && (0, t.rTO)(o, f), 1 & u && i !== (i = "nav-link" + (n[0].value === n[4] ? " active" : "")) && (0, t.Ljt)(e, "class", i), 1 & u && c !== (c = "tab-content-" + n[0].name + "-" + n[4]) && (0, t.Ljt)(e, "aria-controls", c)
                         },
                         d(n) {
                             n && (0, t.ogt)(e), u = !1, s()
                         }
                     }
                 }
 
                 function s(c) {
-                    let u, s, l, f, a, d, p, $, g, m, h, b, v, y = c[0].label + "",
+                    let u, s, f, l, a, d, p, $, g, m, h, b, v, y = c[0].label + "",
                         j = c[0].description && r(c),
                         L = Array.isArray(c[0].choices) ? c[0].choices : Object.keys(c[0].choices),
                         w = [];
                     for (let t = 0; t < L.length; t += 1) w[t] = i(o(c, L, t));
                     const x = c[2].default,
                         _ = (0, t.nuO)(x, c, c[1], e);
                     return {
                         c() {
-                            u = (0, t.bGB)("div"), s = (0, t.bGB)("div"), l = (0, t.fLW)(y), f = (0, t.DhX)(), j && j.c(), a = (0, t.fLW)(":"), d = (0, t.DhX)(), p = (0, t.bGB)("div"), $ = (0, t.bGB)("div");
+                            u = (0, t.bGB)("div"), s = (0, t.bGB)("div"), f = (0, t.fLW)(y), l = (0, t.DhX)(), j && j.c(), a = (0, t.fLW)(":"), d = (0, t.DhX)(), p = (0, t.bGB)("div"), $ = (0, t.bGB)("div");
                             for (let t = 0; t < w.length; t += 1) w[t].c();
                             g = (0, t.DhX)(), m = (0, t.bGB)("div"), h = (0, t.bGB)("div"), b = (0, t.bGB)("div"), _ && _.c(), (0, t.Ljt)(s, "class", "col-lg-2 bold text-lg-right my-auto"), (0, t.Ljt)($, "class", "nav flex-column nav-pills nav-justified"), (0, t.Ljt)($, "aria-orientation", "vertical"), (0, t.Ljt)($, "role", "tablist"), (0, t.Ljt)(p, "class", "col-lg-2 pt-2 pt-lg-0"), (0, t.Ljt)(b, "class", "tab-pane show active"), (0, t.Ljt)(b, "role", "tabpanel"), (0, t.Ljt)(h, "class", "tab-content"), (0, t.Ljt)(m, "class", "col-lg-8 pt-2 pt-lg-0"), (0, t.Ljt)(u, "class", "row px-4 px-lg-3 pb-4")
                         },
                         m(n, e) {
-                            (0, t.$Tr)(n, u, e), (0, t.R3I)(u, s), (0, t.R3I)(s, l), (0, t.R3I)(s, f), j && j.m(s, null), (0, t.R3I)(s, a), (0, t.R3I)(u, d), (0, t.R3I)(u, p), (0, t.R3I)(p, $);
+                            (0, t.$Tr)(n, u, e), (0, t.R3I)(u, s), (0, t.R3I)(s, f), (0, t.R3I)(s, l), j && j.m(s, null), (0, t.R3I)(s, a), (0, t.R3I)(u, d), (0, t.R3I)(u, p), (0, t.R3I)(p, $);
                             for (let t = 0; t < w.length; t += 1) w[t].m($, null);
                             (0, t.R3I)(u, g), (0, t.R3I)(u, m), (0, t.R3I)(m, h), (0, t.R3I)(h, b), _ && _.m(b, null), v = !0
                         },
                         p(c, [u]) {
-                            if ((!v || 1 & u) && y !== (y = c[0].label + "") && (0, t.rTO)(l, y), c[0].description ? j ? j.p(c, u) : (j = r(c), j.c(), j.m(s, a)) : j && (j.d(1), j = null), 1 & u) {
+                            if ((!v || 1 & u) && y !== (y = c[0].label + "") && (0, t.rTO)(f, y), c[0].description ? j ? j.p(c, u) : (j = r(c), j.c(), j.m(s, a)) : j && (j.d(1), j = null), 1 & u) {
                                 let t;
                                 for (L = Array.isArray(c[0].choices) ? c[0].choices : Object.keys(c[0].choices), t = 0; t < L.length; t += 1) {
                                     const n = o(c, L, t);
                                     w[t] ? w[t].p(n, u) : (w[t] = i(n), w[t].c(), w[t].m($, null))
                                 }
                                 for (; t < w.length; t += 1) w[t].d(1);
                                 w.length = L.length
@@ -1011,33 +1011,33 @@
                         },
                         d(n) {
                             n && (0, t.ogt)(u), j && j.d(), (0, t.RMB)(w, n), _ && _.d(n)
                         }
                     }
                 }
 
-                function l(t, n, e) {
+                function f(t, n, e) {
                     let {
                         $$slots: o = {},
                         $$scope: r
                     } = n, {
                         args: i
                     } = n;
                     return t.$$set = t => {
                         "args" in t && e(0, i = t.args), "$$scope" in t && e(1, r = t.$$scope)
                     }, [i, r, o, t => e(0, i.value = t, i)]
                 }
-                class f extends t.f_C {
+                class l extends t.f_C {
                     constructor(n) {
-                        super(), (0, t.S1n)(this, n, l, s, t.N8, {
+                        super(), (0, t.S1n)(this, n, f, s, t.N8, {
                             args: 0
                         })
                     }
                 }
-                var a = f,
+                var a = l,
                     d = c(966);
 
                 function p(n) {
                     let e, o;
                     return e = new d.Z({
                         props: {
                             module: y,
@@ -1118,15 +1118,15 @@
                     let e, o;
                     return e = new d.Z({
                         props: {
                             module: b,
                             props: {
                                 args: {
                                     ...n[0],
-                                    label: "Upload"
+                                    label: "Choose file"
                                 }
                             }
                         }
                     }), {
                         c() {
                             (0, t.YCL)(e.$$.fragment)
                         },
@@ -1134,15 +1134,15 @@
                             (0, t.yef)(e, n, r), o = !0
                         },
                         p(t, n) {
                             const o = {};
                             1 & n && (o.props = {
                                 args: {
                                     ...t[0],
-                                    label: "Upload"
+                                    label: "Choose file"
                                 }
                             }), e.$set(o)
                         },
                         i(n) {
                             o || ((0, t.Ui)(e.$$.fragment, n), o = !0)
                         },
                         o(n) {
@@ -1155,27 +1155,27 @@
                 }
 
                 function m(n) {
                     let e, o, r, i, c;
                     const u = [g, $, p],
                         s = [];
 
-                    function l(t, n) {
+                    function f(t, n) {
                         return 16 & n && (e = null), "Upload" === t[4] ? 0 : (null == e && (e = !(!window._config.EXTRAS.includes("catalog-integration") || "Locate" !== t[4])), e ? 1 : "Passthrough" === t[4] ? 2 : -1)
                     }
-                    return ~(o = l(n, -1)) && (r = s[o] = u[o](n)), {
+                    return ~(o = f(n, -1)) && (r = s[o] = u[o](n)), {
                         c() {
                             r && r.c(), i = (0, t.cSb)()
                         },
                         m(n, e) {
                             ~o && s[o].m(n, e), (0, t.$Tr)(n, i, e), c = !0
                         },
                         p(n, e) {
                             let c = o;
-                            o = l(n, e), o === c ? ~o && s[o].p(n, e) : (r && ((0, t.dvw)(), (0, t.etI)(s[c], 1, 1, (() => {
+                            o = f(n, e), o === c ? ~o && s[o].p(n, e) : (r && ((0, t.dvw)(), (0, t.etI)(s[c], 1, 1, (() => {
                                 s[c] = null
                             })), (0, t.gbL)()), ~o ? (r = s[o], r ? r.p(n, e) : (r = s[o] = u[o](n), r.c()), (0, t.Ui)(r, 1), r.m(i.parentNode, i)) : r = null)
                         },
                         i(n) {
                             c || ((0, t.Ui)(r), c = !0)
                         },
                         o(n) {
```

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/fields/MultiCheckboxField.js` & `appyter-0.19.9/appyter/static/profiles/default/js/fields/MultiCheckboxField.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/fields/TabField.js` & `appyter-0.19.9/appyter/static/profiles/default/js/fields/TabField.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/fields/VariableField.js` & `appyter-0.19.9/appyter/static/profiles/default/js/fields/VariableField.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/index.js` & `appyter-0.19.9/appyter/static/profiles/default/js/index.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/landing.js` & `appyter-0.19.9/appyter/static/profiles/default/js/landing.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1036,15 +1036,15 @@
                     }; {
                         const [e, o] = [t.slice(0, n), t.slice(n + 1)];
                         return {
                             path: e,
                             params: function(t) {
                                 return "" === t ? {} : t.split("&").map((t => t.split("=").map(decodeURIComponent))).reduce(((t, [n, e]) => ({
                                     ...t,
-                                    [n]: e
+                                    [n]: void 0 === e || e
                                 })), {})
                             }(o)
                         }
                     }
                 }
 
                 function a() {
@@ -1074,15 +1074,15 @@
                         server: e
                     }) => {
                         const o = function({
                             path: t,
                             params: n
                         }) {
                             const e = function(t) {
-                                return Object.keys(t).filter((n => void 0 !== t[n] && "" !== t[n])).map((n => [n, t[n]].map(encodeURIComponent).join("="))).join("&")
+                                return Object.keys(t).filter((n => void 0 !== t[n] && "" !== t[n])).map((n => !0 === t[n] ? encodeURIComponent(n) : [n, t[n]].map(encodeURIComponent).join("="))).join("&")
                             }(n);
                             return "" === e ? t : `${t}?${e}`
                         }({
                             path: t,
                             params: n
                         });
                         if (t !== u) window.location.hash = o, u = t;
```

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/lib/jquery.js` & `appyter-0.19.9/appyter/static/profiles/default/js/lib/jquery.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter/static/profiles/default/js/lib/require.js` & `appyter-0.19.9/appyter/static/profiles/default/js/lib/require.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/appyter.egg-info/PKG-INFO` & `appyter-0.19.9/appyter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appyter
-Version: 0.19.8
+Version: 0.19.9
 Summary: UNKNOWN
 Home-page: https://github.com/maayanLab/appyter/
 Author: Daniel J. B. Clarke
 Author-email: u8sand@gmail.com
 License: CC-BY-NC-SA-4.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `appyter-0.19.8/appyter.egg-info/SOURCES.txt` & `appyter-0.19.9/appyter.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -297,14 +297,15 @@
 docs/source/conf.py
 docs/source/index.rst
 example/.dockerignore
 example/Dockerfile
 example/README.md
 example/appyter.cwl
 example/appyter.json
+example/droptest.ipynb
 example/example.ipynb
 example/example_test.py
 example/example_test.sh
 example/requirements.txt
 example/test.py
 example/blueprints/__init__.py
 example/blueprints/testblueprint.py
```

### Comparing `appyter-0.19.8/docs/Makefile` & `appyter-0.19.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/docs/make.bat` & `appyter-0.19.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/docs/source/conf.py` & `appyter-0.19.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/example/Dockerfile` & `appyter-0.19.9/example/Dockerfile`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/example/README.md` & `appyter-0.19.9/example/README.md`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/example/appyter.cwl` & `appyter-0.19.9/example/appyter.cwl`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/example/appyter.json` & `appyter-0.19.9/example/appyter.json`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/example/blueprints/testdash.py` & `appyter-0.19.9/example/blueprints/testdash.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/example/example.ipynb` & `appyter-0.19.9/example/example.ipynb`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/example/example_test.py` & `appyter-0.19.9/example/example_test.py`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/example/production/appyter/Dockerfile` & `appyter-0.19.9/example/production/appyter/Dockerfile`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/example/production/docker-compose.yml` & `appyter-0.19.9/example/production/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/example/static/GitHub-Mark.png` & `appyter-0.19.9/example/static/GitHub-Mark.png`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/components/HTML.svelte` & `appyter-0.19.9/js/components/HTML.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/components/Lazy.svelte` & `appyter-0.19.9/js/components/Lazy.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/components/app/SSRField.svelte` & `appyter-0.19.9/js/components/app/SSRField.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/components/fields/SectionField.svelte` & `appyter-0.19.9/js/components/fields/SectionField.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/components/fields/StringField.svelte` & `appyter-0.19.9/js/components/fields/StringField.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/components/fields/TabField.svelte` & `appyter-0.19.9/js/components/fields/TabField.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/components/jupyter/Notebook.svelte` & `appyter-0.19.9/js/components/jupyter/Notebook.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/components/jupyter/Output.svelte` & `appyter-0.19.9/js/components/jupyter/Output.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/components/jupyter/OutputMimetype.svelte` & `appyter-0.19.9/js/components/jupyter/OutputMimetype.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/components/jupyter/Outputs.svelte` & `appyter-0.19.9/js/components/jupyter/Outputs.svelte`

 * *Files 4% similar despite different names*

```diff
@@ -24,39 +24,39 @@
       } else {
         yield {...output, index: i++}
       }
     }
     for (const stream in streams) {
       streams[stream].text = streams[stream].text.replace(/^\r/, '').replace(/(\r?\n)+$/, '')
       if (streams[stream].text) {
-        yield {...streams[stream], index: i++}
+        yield streams[stream]
       }
     }
   }
 </script>
 
 <div class="output_wrapper">
   <div class="output">
-    {#if index === loading}
+    {#each [...reduce_output_streams(data)] as output (output.index)}
       <div class="output_area">
         <Prompt
-          index="{index}-loader"
+          index="{index}-{output.index}"
           prompt_type="output"
         />
         <div class="output_subarea">
-          <Loader />
+          <Output data={output} />
         </div>
       </div>
-    {/if}
-    {#each [...reduce_output_streams(data)] as output (output.index)}
+    {/each}
+    {#if index === loading}
       <div class="output_area">
         <Prompt
-          index="{index}-{output.index}"
+          index="{index}-loader"
           prompt_type="output"
         />
         <div class="output_subarea">
-          <Output data={output} />
+          <Loader />
         </div>
       </div>
-    {/each}
+    {/if}
   </div>
 </div>
```

#### html2text {}

```diff
@@ -1,3 +1,3 @@
-{#if index === loading}
-{/if} {#each [...reduce_output_streams(data)] as output (output.index)}
-{/each}
+{#each [...reduce_output_streams(data)] as output (output.index)}
+{/each} {#if index === loading}
+{/if}
```

### Comparing `appyter-0.19.8/js/components/jupyter/Prompt.svelte` & `appyter-0.19.9/js/components/jupyter/Prompt.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/components/jupyter/output_mimetype/index.js` & `appyter-0.19.9/js/components/jupyter/output_mimetype/index.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/components/jupyter/output_type/OutputError.svelte` & `appyter-0.19.9/js/components/jupyter/output_type/OutputError.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/extras/catalog-integration/LaunchSettings.svelte` & `appyter-0.19.9/js/extras/catalog-integration/LaunchSettings.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/extras/catalog-integration/LocateFileField.svelte` & `appyter-0.19.9/js/extras/catalog-integration/LocateFileField.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/extras/catalog-integration/TableOfContents.svelte` & `appyter-0.19.9/js/extras/catalog-integration/TableOfContents.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/extras/catalog-integration/pagehit.js` & `appyter-0.19.9/js/extras/catalog-integration/pagehit.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/extras/catalog-integration/report_error.js` & `appyter-0.19.9/js/extras/catalog-integration/report_error.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/extras/catalog-integration/toc.js` & `appyter-0.19.9/js/extras/catalog-integration/toc.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/extras/file-field/Storage.svelte` & `appyter-0.19.9/js/extras/file-field/Storage.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/extras/file-field/URI.svelte` & `appyter-0.19.9/js/extras/file-field/URI.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/extras/file-field/Upload.svelte` & `appyter-0.19.9/js/extras/file-field/Upload.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/lib/markdown_it.js` & `appyter-0.19.9/js/lib/markdown_it.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/lib/socketio.js` & `appyter-0.19.9/js/lib/socketio.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/lib/stores/keycloak_auth_store.js` & `appyter-0.19.9/js/lib/stores/keycloak_auth_store.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/lib/stores/url_hash_store.js` & `appyter-0.19.9/js/lib/stores/url_hash_store.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -5,22 +5,22 @@
 function params_parse(params_encoded) {
     if (params_encoded === '') return {}
     return params_encoded
         .split('&')
         .map(param_pair => param_pair.split('=').map(decodeURIComponent))
         .reduce((params, [key, value]) => ({
             ...params,
-            [key]: value
+            [key]: value !== undefined ? value : true
         }), {})
 }
 
 function params_stringify(params) {
     return Object.keys(params)
         .filter(param => params[param] !== undefined && params[param] !== '')
-        .map((param) => [param, params[param]].map(encodeURIComponent).join('='))
+        .map((param) => params[param] === true ? encodeURIComponent(param) : [param, params[param]].map(encodeURIComponent).join('='))
         .join('&')
 }
 
 function fragment_parse(hash_encoded) {
     // if (!hash_encoded.startsWith('/')) hash_encoded = `/${hash_encoded}`
     const q = hash_encoded.indexOf('?')
     if (q === -1) {
```

### Comparing `appyter-0.19.8/js/lib/svelte_component_mounter.js` & `appyter-0.19.9/js/lib/svelte_component_mounter.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/package-lock.json` & `appyter-0.19.9/js/package-lock.json`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/package.json` & `appyter-0.19.9/js/package.json`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/profiles/biojupies/css/index.scss` & `appyter-0.19.9/js/profiles/biojupies/css/index.scss`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/profiles/biojupies/js/fields/IntField.svelte` & `appyter-0.19.9/js/profiles/biojupies/js/fields/IntField.svelte`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <script>
   import is_null from '@/utils/null'
 
   export let args
 
   let value
   $: if (args !== undefined && value === undefined) {
-    value = args.default
+    value = args.default|0
   }
 
   let valid = true
   $: if (value !== undefined && args !== undefined) {
     valid =
       (value|0) === value
       && (is_null(args.min) || ((value|0) >= args.min))
```

### Comparing `appyter-0.19.8/js/profiles/biojupies/js/fields/SectionField.svelte` & `appyter-0.19.9/js/profiles/biojupies/js/fields/SectionField.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/profiles/biojupies/js/fields/StringField.svelte` & `appyter-0.19.9/js/profiles/biojupies/js/fields/StringField.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/profiles/biojupies/js/fields/TextField.svelte` & `appyter-0.19.9/js/profiles/biojupies/js/fields/TextField.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/profiles/biojupies/js/fields/TextListField.svelte` & `appyter-0.19.9/js/profiles/biojupies/js/fields/TextListField.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/profiles/default/css/index.scss` & `appyter-0.19.9/js/profiles/default/css/index.scss`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/profiles/default/js/fields/AutocompleteField.svelte` & `appyter-0.19.9/js/profiles/default/js/fields/AutocompleteField.svelte`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 <script>
   import { onMount } from 'svelte'
   import Loader from '@/components/Loader.svelte'
 
   export let args
   let focused
   let error
-  let value = args.default
+  let value
   let items
   let current_focus = -1
   let relevant_items
-  
+
+  $: if (args !== undefined && value === undefined) {
+    value = args.default
+  }
+
   $: if (items !== undefined) {
     relevant_items = Object.keys(items)
       .filter(item => item.toLowerCase().substr(0, value.length) === value.toLowerCase() && item !== value)
       .slice(0, 7)
     current_focus = -1
   }
```

### Comparing `appyter-0.19.8/js/profiles/default/js/fields/FileField.svelte` & `appyter-0.19.9/js/profiles/default/js/fields/FileField.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 <TabField bind:args={tabArgs} let:tab={tab}>
   {#if tab === 'Upload'}
     <Lazy
       module={() => import('@/extras/file-field/Upload.svelte')}
       props={{
         args: {
           ...args,
-          label: 'Upload',
+          label: 'Choose file',
         }
       }}
     />
   {:else if window._config.EXTRAS.includes('catalog-integration') && tab === 'Locate'}
     <Lazy
       module={() => import('@/extras/catalog-integration/LocateFileField.svelte')}
       props={{ args }}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
   {#if tab === 'Upload'}
 > import('@/extras/file-field/Upload.svelte')} props={{ args: { ...args, label:
-'Upload', } }} /> {:else if window._config.EXTRAS.includes('catalog-
+'Choose file', } }} /> {:else if window._config.EXTRAS.includes('catalog-
 integration') && tab === 'Locate'}
 > import('@/extras/catalog-integration/LocateFileField.svelte')} props={{ args
 }} /> {:else if tab === 'Passthrough'}
 > import('@/extras/file-field/URI.svelte')} props={{ args: { name: args.name,
 label: 'Uniform Resource Identifier', description: 'One of several supported
 identifiers for accessing your file', examples: Object.keys(args.examples ||
 {}).reduce((agg, example) => (example.indexOf('://') !== -1) ? { ...agg,
```

### Comparing `appyter-0.19.8/js/profiles/default/js/fields/MultiCheckboxField.svelte` & `appyter-0.19.9/js/profiles/default/js/fields/MultiCheckboxField.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/profiles/default/js/fields/VariableField.svelte` & `appyter-0.19.9/js/profiles/default/js/fields/VariableField.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/profiles/default/js/index.js` & `appyter-0.19.9/js/profiles/default/js/index.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/profiles/default/js/landing.svelte` & `appyter-0.19.9/js/profiles/default/js/landing.svelte`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/utils/url_for.js` & `appyter-0.19.9/js/utils/url_for.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/js/webpack.config.js` & `appyter-0.19.9/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `appyter-0.19.8/setup.py` & `appyter-0.19.9/setup.py`

 * *Files identical despite different names*

