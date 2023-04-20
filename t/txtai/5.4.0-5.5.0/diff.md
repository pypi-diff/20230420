# Comparing `tmp/txtai-5.4.0.tar.gz` & `tmp/txtai-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/txtai-5.4.0.tar", last modified: Mon Mar  6 15:08:35 2023, max compression
+gzip compressed data, was "dist/txtai-5.5.0.tar", last modified: Thu Apr 20 14:38:40 2023, max compression
```

## Comparing `txtai-5.4.0.tar` & `txtai-5.5.0.tar`

### file list

```diff
@@ -1,189 +1,192 @@
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    30249 2023-03-06 15:08:35.000000 txtai-5.4.0/PKG-INFO
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    27684 2023-03-03 18:41:46.000000 txtai-5.4.0/README.md
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       38 2023-03-06 15:08:35.000000 txtai-5.4.0/setup.cfg
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3325 2023-02-07 02:19:29.000000 txtai-5.4.0/setup.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      269 2023-02-07 02:19:37.000000 txtai-5.4.0/src/python/txtai/__init__.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/ann/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      148 2021-02-26 23:19:14.000000 txtai-5.4.0/src/python/txtai/ann/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1886 2022-12-16 18:47:06.000000 txtai-5.4.0/src/python/txtai/ann/annoy.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3024 2022-09-12 14:07:23.000000 txtai-5.4.0/src/python/txtai/ann/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1287 2022-09-20 16:18:14.000000 txtai-5.4.0/src/python/txtai/ann/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3926 2023-02-17 00:05:12.000000 txtai-5.4.0/src/python/txtai/ann/faiss.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3170 2022-09-12 14:07:23.000000 txtai-5.4.0/src/python/txtai/ann/hnsw.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/api/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      393 2021-11-28 02:00:12.000000 txtai-5.4.0/src/python/txtai/api/__init__.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2013 2022-03-24 13:11:27.000000 txtai-5.4.0/src/python/txtai/api/application.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3163 2023-02-06 00:08:29.000000 txtai-5.4.0/src/python/txtai/api/base.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     6714 2021-12-23 01:22:00.000000 txtai-5.4.0/src/python/txtai/api/cluster.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      369 2021-04-09 22:58:59.000000 txtai-5.4.0/src/python/txtai/api/extension.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      634 2022-09-20 17:18:44.000000 txtai-5.4.0/src/python/txtai/api/factory.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/api/routers/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      357 2022-01-25 18:17:11.000000 txtai-5.4.0/src/python/txtai/api/routers/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      676 2021-11-28 01:58:41.000000 txtai-5.4.0/src/python/txtai/api/routers/caption.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4195 2023-02-05 23:47:39.000000 txtai-5.4.0/src/python/txtai/api/routers/embeddings.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      742 2022-01-25 19:18:17.000000 txtai-5.4.0/src/python/txtai/api/routers/entity.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      593 2023-02-05 00:39:29.000000 txtai-5.4.0/src/python/txtai/api/routers/extractor.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1147 2021-11-21 13:21:34.000000 txtai-5.4.0/src/python/txtai/api/routers/labels.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      778 2021-11-27 15:50:59.000000 txtai-5.4.0/src/python/txtai/api/routers/objects.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      704 2021-11-21 13:21:34.000000 txtai-5.4.0/src/python/txtai/api/routers/segmentation.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1145 2021-11-28 01:39:37.000000 txtai-5.4.0/src/python/txtai/api/routers/similarity.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1123 2021-11-21 13:21:34.000000 txtai-5.4.0/src/python/txtai/api/routers/summary.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      738 2023-03-01 15:20:34.000000 txtai-5.4.0/src/python/txtai/api/routers/tabular.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      717 2021-11-21 13:21:34.000000 txtai-5.4.0/src/python/txtai/api/routers/textractor.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      730 2021-11-21 13:21:34.000000 txtai-5.4.0/src/python/txtai/api/routers/transcription.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1207 2021-11-21 13:21:34.000000 txtai-5.4.0/src/python/txtai/api/routers/translation.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      528 2021-11-27 01:15:11.000000 txtai-5.4.0/src/python/txtai/api/routers/workflow.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/app/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       66 2022-03-01 18:21:41.000000 txtai-5.4.0/src/python/txtai/app/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    20951 2023-03-02 22:24:19.000000 txtai-5.4.0/src/python/txtai/app/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/archive/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      160 2023-02-19 13:31:37.000000 txtai-5.4.0/src/python/txtai/archive/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2840 2023-02-19 18:17:59.000000 txtai-5.4.0/src/python/txtai/archive/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1029 2023-02-19 18:17:27.000000 txtai-5.4.0/src/python/txtai/archive/compress.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      429 2023-02-19 18:15:28.000000 txtai-5.4.0/src/python/txtai/archive/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1272 2023-02-19 00:23:52.000000 txtai-5.4.0/src/python/txtai/archive/tar.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      778 2023-02-19 18:58:42.000000 txtai-5.4.0/src/python/txtai/archive/zip.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/cloud/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      148 2023-02-17 13:35:20.000000 txtai-5.4.0/src/python/txtai/cloud/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2424 2023-02-19 18:45:23.000000 txtai-5.4.0/src/python/txtai/cloud/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1544 2023-02-19 13:30:19.000000 txtai-5.4.0/src/python/txtai/cloud/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3649 2023-03-03 17:46:20.000000 txtai-5.4.0/src/python/txtai/cloud/hub.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2983 2023-02-19 00:21:57.000000 txtai-5.4.0/src/python/txtai/cloud/storage.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/console/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       51 2022-03-29 00:05:18.000000 txtai-5.4.0/src/python/txtai/console/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      274 2022-03-29 16:55:55.000000 txtai-5.4.0/src/python/txtai/console/__main__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6590 2023-02-19 19:08:09.000000 txtai-5.4.0/src/python/txtai/console/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/data/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      190 2023-01-01 14:12:39.000000 txtai-5.4.0/src/python/txtai/data/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3958 2023-01-09 14:39:56.000000 txtai-5.4.0/src/python/txtai/data/base.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1198 2022-11-26 00:37:43.000000 txtai-5.4.0/src/python/txtai/data/labels.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4599 2022-04-16 12:34:51.000000 txtai-5.4.0/src/python/txtai/data/questions.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1336 2022-04-11 19:50:27.000000 txtai-5.4.0/src/python/txtai/data/sequences.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1883 2023-01-09 15:33:33.000000 txtai-5.4.0/src/python/txtai/data/texts.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      579 2022-12-04 18:56:16.000000 txtai-5.4.0/src/python/txtai/data/tokens.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/database/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      159 2021-12-22 11:44:55.000000 txtai-5.4.0/src/python/txtai/database/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8081 2023-03-01 15:04:31.000000 txtai-5.4.0/src/python/txtai/database/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/database/encoder/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      153 2021-12-22 11:16:40.000000 txtai-5.4.0/src/python/txtai/database/encoder/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      719 2022-05-27 12:13:14.000000 txtai-5.4.0/src/python/txtai/database/encoder/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1001 2022-09-20 17:06:23.000000 txtai-5.4.0/src/python/txtai/database/encoder/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      904 2022-02-09 11:29:07.000000 txtai-5.4.0/src/python/txtai/database/encoder/image.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      428 2022-07-21 19:55:46.000000 txtai-5.4.0/src/python/txtai/database/encoder/pickle.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1324 2022-09-20 16:17:28.000000 txtai-5.4.0/src/python/txtai/database/factory.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/database/sql/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      146 2022-03-01 13:12:16.000000 txtai-5.4.0/src/python/txtai/database/sql/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5315 2021-12-26 16:01:02.000000 txtai-5.4.0/src/python/txtai/database/sql/aggregate.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6198 2023-01-09 21:32:56.000000 txtai-5.4.0/src/python/txtai/database/sql/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    13762 2022-11-19 16:44:34.000000 txtai-5.4.0/src/python/txtai/database/sql/expression.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8869 2022-11-19 15:44:37.000000 txtai-5.4.0/src/python/txtai/database/sql/token.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    16900 2022-11-18 19:55:16.000000 txtai-5.4.0/src/python/txtai/database/sqlite.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/embeddings/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      283 2023-03-02 21:46:33.000000 txtai-5.4.0/src/python/txtai/embeddings/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    24388 2023-03-02 21:46:33.000000 txtai-5.4.0/src/python/txtai/embeddings/base.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1882 2022-07-21 19:57:10.000000 txtai-5.4.0/src/python/txtai/embeddings/documents.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4142 2022-03-30 19:35:55.000000 txtai-5.4.0/src/python/txtai/embeddings/explain.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3654 2022-09-14 15:13:58.000000 txtai-5.4.0/src/python/txtai/embeddings/functions.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1783 2022-04-18 19:57:38.000000 txtai-5.4.0/src/python/txtai/embeddings/query.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2709 2022-12-12 13:51:32.000000 txtai-5.4.0/src/python/txtai/embeddings/reducer.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6767 2022-12-12 16:52:20.000000 txtai-5.4.0/src/python/txtai/embeddings/search.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1145 2023-03-02 22:24:02.000000 txtai-5.4.0/src/python/txtai/embeddings/terms.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4956 2022-09-14 15:17:14.000000 txtai-5.4.0/src/python/txtai/embeddings/transform.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/graph/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      139 2022-09-03 13:13:44.000000 txtai-5.4.0/src/python/txtai/graph/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    14771 2023-02-19 19:01:48.000000 txtai-5.4.0/src/python/txtai/graph/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1133 2022-09-20 16:16:49.000000 txtai-5.4.0/src/python/txtai/graph/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4994 2022-09-14 15:17:14.000000 txtai-5.4.0/src/python/txtai/graph/networkx.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4595 2022-09-30 13:52:22.000000 txtai-5.4.0/src/python/txtai/graph/topics.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/models/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      195 2023-01-31 14:10:56.000000 txtai-5.4.0/src/python/txtai/models/__init__.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4424 2022-10-19 19:11:48.000000 txtai-5.4.0/src/python/txtai/models/models.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3508 2023-02-19 19:01:48.000000 txtai-5.4.0/src/python/txtai/models/onnx.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3747 2023-01-28 02:01:25.000000 txtai-5.4.0/src/python/txtai/models/pooling.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1384 2022-10-27 19:39:43.000000 txtai-5.4.0/src/python/txtai/models/registry.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4590 2023-01-31 14:13:50.000000 txtai-5.4.0/src/python/txtai/models/tokendetection.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/pipeline/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      307 2021-11-28 01:42:36.000000 txtai-5.4.0/src/python/txtai/pipeline/__init__.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/pipeline/audio/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      103 2022-11-29 16:35:29.000000 txtai-5.4.0/src/python/txtai/pipeline/audio/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3761 2023-02-18 15:39:14.000000 txtai-5.4.0/src/python/txtai/pipeline/audio/texttospeech.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6548 2022-12-03 12:49:26.000000 txtai-5.4.0/src/python/txtai/pipeline/audio/transcription.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      536 2022-12-02 16:07:11.000000 txtai-5.4.0/src/python/txtai/pipeline/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/pipeline/data/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      161 2021-11-18 20:49:26.000000 txtai-5.4.0/src/python/txtai/pipeline/data/__init__.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3399 2021-11-22 21:19:44.000000 txtai-5.4.0/src/python/txtai/pipeline/data/segmentation.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4093 2023-03-01 15:20:17.000000 txtai-5.4.0/src/python/txtai/pipeline/data/tabular.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2182 2022-03-24 17:06:47.000000 txtai-5.4.0/src/python/txtai/pipeline/data/textractor.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1632 2021-11-18 20:09:32.000000 txtai-5.4.0/src/python/txtai/pipeline/data/tokenizer.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1782 2022-09-20 16:19:32.000000 txtai-5.4.0/src/python/txtai/pipeline/factory.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3687 2022-12-02 16:06:16.000000 txtai-5.4.0/src/python/txtai/pipeline/hfmodel.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2299 2022-10-17 13:20:55.000000 txtai-5.4.0/src/python/txtai/pipeline/hfpipeline.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/pipeline/image/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      114 2022-03-04 16:47:13.000000 txtai-5.4.0/src/python/txtai/pipeline/image/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1503 2022-10-16 13:16:42.000000 txtai-5.4.0/src/python/txtai/pipeline/image/caption.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2546 2022-03-07 14:33:13.000000 txtai-5.4.0/src/python/txtai/pipeline/image/imagehash.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2706 2022-01-25 18:50:43.000000 txtai-5.4.0/src/python/txtai/pipeline/image/objects.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      189 2021-11-19 14:42:33.000000 txtai-5.4.0/src/python/txtai/pipeline/nop.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1058 2022-10-17 13:21:17.000000 txtai-5.4.0/src/python/txtai/pipeline/tensors.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/pipeline/text/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      348 2023-01-31 14:01:28.000000 txtai-5.4.0/src/python/txtai/pipeline/text/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2599 2023-02-19 19:08:49.000000 txtai-5.4.0/src/python/txtai/pipeline/text/crossencoder.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2519 2022-01-27 11:33:22.000000 txtai-5.4.0/src/python/txtai/pipeline/text/entity.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    16163 2023-03-02 22:24:19.000000 txtai-5.4.0/src/python/txtai/pipeline/text/extractor.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1768 2023-01-30 19:10:28.000000 txtai-5.4.0/src/python/txtai/pipeline/text/generator.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     5308 2022-10-25 15:49:15.000000 txtai-5.4.0/src/python/txtai/pipeline/text/labels.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1397 2021-11-29 23:27:03.000000 txtai-5.4.0/src/python/txtai/pipeline/text/questions.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      213 2023-01-31 14:00:05.000000 txtai-5.4.0/src/python/txtai/pipeline/text/sequences.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2237 2022-10-25 17:47:04.000000 txtai-5.4.0/src/python/txtai/pipeline/text/similarity.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2816 2022-11-18 18:40:05.000000 txtai-5.4.0/src/python/txtai/pipeline/text/summary.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8669 2023-02-12 12:27:17.000000 txtai-5.4.0/src/python/txtai/pipeline/text/translation.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/pipeline/train/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      110 2021-11-18 20:49:46.000000 txtai-5.4.0/src/python/txtai/pipeline/train/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5438 2022-10-19 20:33:27.000000 txtai-5.4.0/src/python/txtai/pipeline/train/hfonnx.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8164 2023-02-17 02:35:33.000000 txtai-5.4.0/src/python/txtai/pipeline/train/hftrainer.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1847 2021-11-18 20:18:27.000000 txtai-5.4.0/src/python/txtai/pipeline/train/mlonnx.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/scoring/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      131 2021-02-26 23:19:24.000000 txtai-5.4.0/src/python/txtai/scoring/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9258 2022-12-28 00:02:56.000000 txtai-5.4.0/src/python/txtai/scoring/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      668 2022-10-04 13:39:24.000000 txtai-5.4.0/src/python/txtai/scoring/bm25.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      875 2022-09-12 14:13:51.000000 txtai-5.4.0/src/python/txtai/scoring/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      593 2022-10-04 13:39:24.000000 txtai-5.4.0/src/python/txtai/scoring/sif.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/util/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       56 2022-11-01 17:14:15.000000 txtai-5.4.0/src/python/txtai/util/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      565 2022-09-20 17:08:45.000000 txtai-5.4.0/src/python/txtai/util/resolver.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/vectors/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      201 2022-05-12 15:49:17.000000 txtai-5.4.0/src/python/txtai/vectors/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5114 2023-02-19 18:06:08.000000 txtai-5.4.0/src/python/txtai/vectors/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      781 2022-12-12 14:03:21.000000 txtai-5.4.0/src/python/txtai/vectors/external.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1759 2022-05-12 13:38:48.000000 txtai-5.4.0/src/python/txtai/vectors/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1940 2023-02-19 18:06:08.000000 txtai-5.4.0/src/python/txtai/vectors/transformers.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6572 2023-03-02 21:45:59.000000 txtai-5.4.0/src/python/txtai/vectors/words.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/workflow/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      139 2021-11-29 23:29:08.000000 txtai-5.4.0/src/python/txtai/workflow/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5256 2023-03-02 22:31:06.000000 txtai-5.4.0/src/python/txtai/workflow/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2845 2021-12-05 00:26:44.000000 txtai-5.4.0/src/python/txtai/workflow/execute.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      754 2022-01-28 20:48:47.000000 txtai-5.4.0/src/python/txtai/workflow/factory.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai/workflow/task/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      409 2023-03-02 22:31:06.000000 txtai-5.4.0/src/python/txtai/workflow/task/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    14712 2023-03-02 22:31:06.000000 txtai-5.4.0/src/python/txtai/workflow/task/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      492 2022-02-01 02:31:47.000000 txtai-5.4.0/src/python/txtai/workflow/task/console.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1567 2022-02-01 21:55:52.000000 txtai-5.4.0/src/python/txtai/workflow/task/export.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2200 2023-03-02 22:27:53.000000 txtai-5.4.0/src/python/txtai/workflow/task/factory.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      560 2022-01-10 15:07:33.000000 txtai-5.4.0/src/python/txtai/workflow/task/file.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      732 2022-09-11 23:47:05.000000 txtai-5.4.0/src/python/txtai/workflow/task/image.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1265 2021-11-29 23:29:08.000000 txtai-5.4.0/src/python/txtai/workflow/task/retrieve.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3038 2022-02-09 21:00:35.000000 txtai-5.4.0/src/python/txtai/workflow/task/service.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2985 2022-10-12 14:46:21.000000 txtai-5.4.0/src/python/txtai/workflow/task/storage.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3511 2023-03-02 22:34:44.000000 txtai-5.4.0/src/python/txtai/workflow/task/template.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      346 2022-01-21 00:01:04.000000 txtai-5.4.0/src/python/txtai/workflow/task/url.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      232 2021-11-26 17:08:18.000000 txtai-5.4.0/src/python/txtai/workflow/task/workflow.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai.egg-info/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    30249 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai.egg-info/PKG-INFO
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5950 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai.egg-info/SOURCES.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        1 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai.egg-info/dependency_links.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2026 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai.egg-info/requires.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        6 2023-03-06 15:08:35.000000 txtai-5.4.0/src/python/txtai.egg-info/top_level.txt
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    30293 2023-04-20 14:38:40.000000 txtai-5.5.0/PKG-INFO
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    27709 2023-04-18 21:57:55.000000 txtai-5.5.0/README.md
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       38 2023-04-20 14:38:40.000000 txtai-5.5.0/setup.cfg
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3353 2023-04-17 19:47:20.000000 txtai-5.5.0/setup.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      269 2023-03-06 16:30:04.000000 txtai-5.5.0/src/python/txtai/__init__.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/ann/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      148 2021-02-26 23:19:14.000000 txtai-5.5.0/src/python/txtai/ann/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1886 2022-12-16 18:47:06.000000 txtai-5.5.0/src/python/txtai/ann/annoy.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3193 2023-04-20 13:57:16.000000 txtai-5.5.0/src/python/txtai/ann/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1287 2022-09-20 16:18:14.000000 txtai-5.5.0/src/python/txtai/ann/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3926 2023-02-17 00:05:12.000000 txtai-5.5.0/src/python/txtai/ann/faiss.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3170 2022-09-12 14:07:23.000000 txtai-5.5.0/src/python/txtai/ann/hnsw.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/api/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      393 2021-11-28 02:00:12.000000 txtai-5.5.0/src/python/txtai/api/__init__.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2013 2022-03-24 13:11:27.000000 txtai-5.5.0/src/python/txtai/api/application.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3163 2023-02-06 00:08:29.000000 txtai-5.5.0/src/python/txtai/api/base.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     6714 2021-12-23 01:22:00.000000 txtai-5.5.0/src/python/txtai/api/cluster.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      369 2021-04-09 22:58:59.000000 txtai-5.5.0/src/python/txtai/api/extension.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      634 2022-09-20 17:18:44.000000 txtai-5.5.0/src/python/txtai/api/factory.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/api/routers/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      357 2022-01-25 18:17:11.000000 txtai-5.5.0/src/python/txtai/api/routers/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      676 2023-03-21 17:12:03.000000 txtai-5.5.0/src/python/txtai/api/routers/caption.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4195 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/embeddings.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      742 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/entity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      593 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/extractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1147 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/labels.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      778 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/objects.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      704 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/segmentation.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1145 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/similarity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1123 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/summary.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      738 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/tabular.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      717 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/textractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      730 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/transcription.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1207 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/translation.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      528 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/workflow.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/app/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       66 2022-03-01 18:21:41.000000 txtai-5.5.0/src/python/txtai/app/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    21429 2023-04-17 13:39:45.000000 txtai-5.5.0/src/python/txtai/app/base.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/archive/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      160 2023-02-19 13:31:37.000000 txtai-5.5.0/src/python/txtai/archive/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2840 2023-02-19 18:17:59.000000 txtai-5.5.0/src/python/txtai/archive/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1029 2023-02-19 18:17:27.000000 txtai-5.5.0/src/python/txtai/archive/compress.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      429 2023-02-19 18:15:28.000000 txtai-5.5.0/src/python/txtai/archive/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1272 2023-02-19 00:23:52.000000 txtai-5.5.0/src/python/txtai/archive/tar.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      778 2023-02-19 18:58:42.000000 txtai-5.5.0/src/python/txtai/archive/zip.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/cloud/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      148 2023-02-17 13:35:20.000000 txtai-5.5.0/src/python/txtai/cloud/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2424 2023-02-19 18:45:23.000000 txtai-5.5.0/src/python/txtai/cloud/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1544 2023-02-19 13:30:19.000000 txtai-5.5.0/src/python/txtai/cloud/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3649 2023-03-03 17:46:20.000000 txtai-5.5.0/src/python/txtai/cloud/hub.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2983 2023-02-19 00:21:57.000000 txtai-5.5.0/src/python/txtai/cloud/storage.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/console/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       51 2022-03-29 00:05:18.000000 txtai-5.5.0/src/python/txtai/console/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      274 2022-03-29 16:55:55.000000 txtai-5.5.0/src/python/txtai/console/__main__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6590 2023-02-19 19:08:09.000000 txtai-5.5.0/src/python/txtai/console/base.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/data/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      190 2023-01-01 14:12:39.000000 txtai-5.5.0/src/python/txtai/data/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3958 2023-01-09 14:39:56.000000 txtai-5.5.0/src/python/txtai/data/base.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1198 2022-11-26 00:37:43.000000 txtai-5.5.0/src/python/txtai/data/labels.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4599 2022-04-16 12:34:51.000000 txtai-5.5.0/src/python/txtai/data/questions.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1336 2022-04-11 19:50:27.000000 txtai-5.5.0/src/python/txtai/data/sequences.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1883 2023-01-09 15:33:33.000000 txtai-5.5.0/src/python/txtai/data/texts.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      579 2022-12-04 18:56:16.000000 txtai-5.5.0/src/python/txtai/data/tokens.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/database/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      213 2023-04-18 15:03:48.000000 txtai-5.5.0/src/python/txtai/database/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8179 2023-04-20 11:23:56.000000 txtai-5.5.0/src/python/txtai/database/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1982 2023-04-18 22:29:58.000000 txtai-5.5.0/src/python/txtai/database/duckdb.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/database/encoder/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      153 2021-12-22 11:16:40.000000 txtai-5.5.0/src/python/txtai/database/encoder/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      719 2022-05-27 12:13:14.000000 txtai-5.5.0/src/python/txtai/database/encoder/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1001 2022-09-20 17:06:23.000000 txtai-5.5.0/src/python/txtai/database/encoder/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      904 2022-02-09 11:29:07.000000 txtai-5.5.0/src/python/txtai/database/encoder/image.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      428 2022-07-21 19:55:46.000000 txtai-5.5.0/src/python/txtai/database/encoder/pickle.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1423 2023-04-20 11:15:45.000000 txtai-5.5.0/src/python/txtai/database/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    16339 2023-04-18 21:23:20.000000 txtai-5.5.0/src/python/txtai/database/filedb.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/database/sql/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      146 2022-03-01 13:12:16.000000 txtai-5.5.0/src/python/txtai/database/sql/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5315 2021-12-26 16:01:02.000000 txtai-5.5.0/src/python/txtai/database/sql/aggregate.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6198 2023-01-09 21:32:56.000000 txtai-5.5.0/src/python/txtai/database/sql/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    13762 2022-11-19 16:44:34.000000 txtai-5.5.0/src/python/txtai/database/sql/expression.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8869 2022-11-19 15:44:37.000000 txtai-5.5.0/src/python/txtai/database/sql/token.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1390 2023-04-18 21:21:53.000000 txtai-5.5.0/src/python/txtai/database/sqlite.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/embeddings/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      283 2023-03-02 21:46:33.000000 txtai-5.5.0/src/python/txtai/embeddings/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    24711 2023-03-10 18:45:22.000000 txtai-5.5.0/src/python/txtai/embeddings/base.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1882 2022-07-21 19:57:10.000000 txtai-5.5.0/src/python/txtai/embeddings/documents.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4142 2022-03-30 19:35:55.000000 txtai-5.5.0/src/python/txtai/embeddings/explain.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4329 2023-03-10 18:14:43.000000 txtai-5.5.0/src/python/txtai/embeddings/functions.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1783 2022-04-18 19:57:38.000000 txtai-5.5.0/src/python/txtai/embeddings/query.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2709 2022-12-12 13:51:32.000000 txtai-5.5.0/src/python/txtai/embeddings/reducer.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6767 2022-12-12 16:52:20.000000 txtai-5.5.0/src/python/txtai/embeddings/search.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1145 2023-03-02 22:24:02.000000 txtai-5.5.0/src/python/txtai/embeddings/terms.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4956 2023-03-09 16:16:39.000000 txtai-5.5.0/src/python/txtai/embeddings/transform.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/graph/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      139 2022-09-03 13:13:44.000000 txtai-5.5.0/src/python/txtai/graph/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    15350 2023-04-20 13:59:43.000000 txtai-5.5.0/src/python/txtai/graph/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1133 2022-09-20 16:16:49.000000 txtai-5.5.0/src/python/txtai/graph/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4994 2023-03-09 16:25:39.000000 txtai-5.5.0/src/python/txtai/graph/networkx.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4595 2022-09-30 13:52:22.000000 txtai-5.5.0/src/python/txtai/graph/topics.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/models/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      195 2023-01-31 14:10:56.000000 txtai-5.5.0/src/python/txtai/models/__init__.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4424 2022-10-19 19:11:48.000000 txtai-5.5.0/src/python/txtai/models/models.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3508 2023-02-19 19:01:48.000000 txtai-5.5.0/src/python/txtai/models/onnx.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3747 2023-01-28 02:01:25.000000 txtai-5.5.0/src/python/txtai/models/pooling.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1384 2022-10-27 19:39:43.000000 txtai-5.5.0/src/python/txtai/models/registry.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4659 2023-04-14 21:23:31.000000 txtai-5.5.0/src/python/txtai/models/tokendetection.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/pipeline/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      307 2021-11-28 01:42:36.000000 txtai-5.5.0/src/python/txtai/pipeline/__init__.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/pipeline/audio/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      103 2022-11-29 16:35:29.000000 txtai-5.5.0/src/python/txtai/pipeline/audio/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3823 2023-03-11 15:52:28.000000 txtai-5.5.0/src/python/txtai/pipeline/audio/texttospeech.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6548 2022-12-03 12:49:26.000000 txtai-5.5.0/src/python/txtai/pipeline/audio/transcription.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      536 2022-12-02 16:07:11.000000 txtai-5.5.0/src/python/txtai/pipeline/base.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/pipeline/data/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      161 2021-11-18 20:49:26.000000 txtai-5.5.0/src/python/txtai/pipeline/data/__init__.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3399 2021-11-22 21:19:44.000000 txtai-5.5.0/src/python/txtai/pipeline/data/segmentation.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4093 2023-03-01 15:20:17.000000 txtai-5.5.0/src/python/txtai/pipeline/data/tabular.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2182 2022-03-24 17:06:47.000000 txtai-5.5.0/src/python/txtai/pipeline/data/textractor.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1632 2021-11-18 20:09:32.000000 txtai-5.5.0/src/python/txtai/pipeline/data/tokenizer.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1782 2022-09-20 16:19:32.000000 txtai-5.5.0/src/python/txtai/pipeline/factory.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3687 2022-12-02 16:06:16.000000 txtai-5.5.0/src/python/txtai/pipeline/hfmodel.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2299 2022-10-17 13:20:55.000000 txtai-5.5.0/src/python/txtai/pipeline/hfpipeline.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/pipeline/image/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      114 2022-03-04 16:47:13.000000 txtai-5.5.0/src/python/txtai/pipeline/image/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1503 2022-10-16 13:16:42.000000 txtai-5.5.0/src/python/txtai/pipeline/image/caption.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2546 2022-03-07 14:33:13.000000 txtai-5.5.0/src/python/txtai/pipeline/image/imagehash.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2706 2022-01-25 18:50:43.000000 txtai-5.5.0/src/python/txtai/pipeline/image/objects.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      189 2021-11-19 14:42:33.000000 txtai-5.5.0/src/python/txtai/pipeline/nop.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1058 2022-10-17 13:21:17.000000 txtai-5.5.0/src/python/txtai/pipeline/tensors.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/pipeline/text/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      348 2023-01-31 14:01:28.000000 txtai-5.5.0/src/python/txtai/pipeline/text/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2599 2023-02-19 19:08:49.000000 txtai-5.5.0/src/python/txtai/pipeline/text/crossencoder.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2519 2022-01-27 11:33:22.000000 txtai-5.5.0/src/python/txtai/pipeline/text/entity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    16184 2023-03-29 19:46:04.000000 txtai-5.5.0/src/python/txtai/pipeline/text/extractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2048 2023-04-14 21:51:28.000000 txtai-5.5.0/src/python/txtai/pipeline/text/generator.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     5308 2022-10-25 15:49:15.000000 txtai-5.5.0/src/python/txtai/pipeline/text/labels.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1397 2021-11-29 23:27:03.000000 txtai-5.5.0/src/python/txtai/pipeline/text/questions.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      213 2023-01-31 14:00:05.000000 txtai-5.5.0/src/python/txtai/pipeline/text/sequences.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2237 2022-10-25 17:47:04.000000 txtai-5.5.0/src/python/txtai/pipeline/text/similarity.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2816 2022-11-18 18:40:05.000000 txtai-5.5.0/src/python/txtai/pipeline/text/summary.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9333 2023-03-11 15:52:58.000000 txtai-5.5.0/src/python/txtai/pipeline/text/translation.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/pipeline/train/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      110 2021-11-18 20:49:46.000000 txtai-5.5.0/src/python/txtai/pipeline/train/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5438 2022-10-19 20:33:27.000000 txtai-5.5.0/src/python/txtai/pipeline/train/hfonnx.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8164 2023-02-17 02:35:33.000000 txtai-5.5.0/src/python/txtai/pipeline/train/hftrainer.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1991 2023-03-10 21:59:48.000000 txtai-5.5.0/src/python/txtai/pipeline/train/mlonnx.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/scoring/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      131 2021-02-26 23:19:24.000000 txtai-5.5.0/src/python/txtai/scoring/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9258 2022-12-28 00:02:56.000000 txtai-5.5.0/src/python/txtai/scoring/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      668 2022-10-04 13:39:24.000000 txtai-5.5.0/src/python/txtai/scoring/bm25.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      875 2022-09-12 14:13:51.000000 txtai-5.5.0/src/python/txtai/scoring/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      593 2022-10-04 13:39:24.000000 txtai-5.5.0/src/python/txtai/scoring/sif.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/util/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       56 2022-11-01 17:14:15.000000 txtai-5.5.0/src/python/txtai/util/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      565 2022-09-20 17:08:45.000000 txtai-5.5.0/src/python/txtai/util/resolver.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/vectors/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      201 2022-05-12 15:49:17.000000 txtai-5.5.0/src/python/txtai/vectors/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5174 2023-04-20 14:01:08.000000 txtai-5.5.0/src/python/txtai/vectors/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      781 2022-12-12 14:03:21.000000 txtai-5.5.0/src/python/txtai/vectors/external.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1759 2022-05-12 13:38:48.000000 txtai-5.5.0/src/python/txtai/vectors/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1940 2023-02-19 18:06:08.000000 txtai-5.5.0/src/python/txtai/vectors/transformers.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6572 2023-03-02 21:45:59.000000 txtai-5.5.0/src/python/txtai/vectors/words.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/workflow/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      139 2023-03-21 22:13:38.000000 txtai-5.5.0/src/python/txtai/workflow/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5486 2023-04-14 21:51:47.000000 txtai-5.5.0/src/python/txtai/workflow/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2845 2021-12-05 00:26:44.000000 txtai-5.5.0/src/python/txtai/workflow/execute.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      965 2023-04-14 21:51:47.000000 txtai-5.5.0/src/python/txtai/workflow/factory.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/workflow/task/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      440 2023-04-14 21:51:47.000000 txtai-5.5.0/src/python/txtai/workflow/task/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    14712 2023-03-11 17:31:41.000000 txtai-5.5.0/src/python/txtai/workflow/task/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      492 2022-02-01 02:31:47.000000 txtai-5.5.0/src/python/txtai/workflow/task/console.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1567 2022-02-01 21:55:52.000000 txtai-5.5.0/src/python/txtai/workflow/task/export.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2200 2023-03-02 22:27:53.000000 txtai-5.5.0/src/python/txtai/workflow/task/factory.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      560 2022-01-10 15:07:33.000000 txtai-5.5.0/src/python/txtai/workflow/task/file.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      732 2022-09-11 23:47:05.000000 txtai-5.5.0/src/python/txtai/workflow/task/image.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1265 2021-11-29 23:29:08.000000 txtai-5.5.0/src/python/txtai/workflow/task/retrieve.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3038 2022-02-09 21:00:35.000000 txtai-5.5.0/src/python/txtai/workflow/task/service.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2985 2022-10-12 14:46:21.000000 txtai-5.5.0/src/python/txtai/workflow/task/storage.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      935 2023-04-17 14:31:28.000000 txtai-5.5.0/src/python/txtai/workflow/task/stream.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3511 2023-03-02 22:34:44.000000 txtai-5.5.0/src/python/txtai/workflow/task/template.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      346 2022-01-21 00:01:04.000000 txtai-5.5.0/src/python/txtai/workflow/task/url.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      232 2021-11-26 17:08:18.000000 txtai-5.5.0/src/python/txtai/workflow/task/workflow.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai.egg-info/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    30293 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai.egg-info/PKG-INFO
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6063 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai.egg-info/SOURCES.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        1 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai.egg-info/dependency_links.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2054 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai.egg-info/requires.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        6 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai.egg-info/top_level.txt
```

### Comparing `txtai-5.4.0/PKG-INFO` & `txtai-5.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: txtai
-Version: 5.4.0
-Summary: Build AI-powered semantic search applications
+Version: 5.5.0
+Summary: Semantic search and workflows powered by language models
 Home-page: https://github.com/neuml/txtai
 Author: NeuML
 License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/neuml/txtai
 Project-URL: Issue Tracker, https://github.com/neuml/txtai/issues
 Project-URL: Source Code, https://github.com/neuml/txtai
 Description: <p align="center">
             <img src="https://raw.githubusercontent.com/neuml/txtai/master/logo.png"/>
         </p>
         
         <h3 align="center">
-            <p>Build AI-powered semantic search applications</p>
+            <p>Semantic search and workflows powered by language models</p>
         </h3>
         
         <p align="center">
             <a href="https://github.com/neuml/txtai/releases">
                 <img src="https://img.shields.io/github/release/neuml/txtai.svg?style=flat&color=success" alt="Version"/>
             </a>
             <a href="https://github.com/neuml/txtai">
@@ -35,80 +35,81 @@
             <a href="https://coveralls.io/github/neuml/txtai?branch=master">
                 <img src="https://img.shields.io/coverallsCoverage/github/neuml/txtai" alt="Coverage Status">
             </a>
         </p>
         
         -------------------------------------------------------------------------------------------------------------------------------------------------------
         
-        txtai executes machine-learning workflows to transform data and build AI-powered semantic search applications.
+        txtai is an open-source platform for semantic search and workflows powered by language models.
         
         ![demo](https://raw.githubusercontent.com/neuml/txtai/master/demo.gif)
         
-        Traditional search systems use keywords to find data. Semantic search applications have an understanding of natural language and identify results that have the same meaning, not necessarily the same keywords.
+        Traditional search systems use keywords to find data. Semantic search has an understanding of natural language and identifies results that have the same meaning, not necessarily the same keywords.
         
         ![search](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/search.png#gh-light-mode-only)
         
-        Backed by state-of-the-art machine learning models, data is transformed into vector representations for search (also known as embeddings). Innovation is happening at a rapid pace, models can understand concepts in documents, audio, images and video.
+        txtai builds embeddings databases, which are a union of vector indexes and relational databases. This enables similarity search with SQL. Embeddings databases can stand on their own and/or serve as a powerful knowledge source for large language model (LLM) prompts.
+        
+        Semantic workflows connect language models together to build intelligent applications.
+        
+        ![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-light-mode-only)
+        
+        Integrate vector search, conversational search, automatic summarization, transcription, translation and more.
         
         Summary of txtai features:
         
-        - 🔎 Large-scale similarity search with multiple index backends ([Faiss](https://github.com/facebookresearch/faiss), [Annoy](https://github.com/spotify/annoy), [Hnswlib](https://github.com/nmslib/hnswlib)) and support for external vector databases
-        - 📄 Create embeddings for text snippets, documents, audio, images and video
-        - 💡 Machine-learning pipelines that run question-answering, labeling, transcription, translation, summarization, LLM prompts and more
-        - ↪️️ Workflows to join pipelines together and aggregate business logic. txtai processes can be microservices or full-fledged indexing workflows.
+        - 🔎 Similarity search with SQL, object storage, topic modeling, graph analysis, multiple vector index backends ([Faiss](https://github.com/facebookresearch/faiss), [Annoy](https://github.com/spotify/annoy), [Hnswlib](https://github.com/nmslib/hnswlib)) and support for external vector databases
+        - 📄 Create embeddings for text, documents, audio, images and video
+        - 💡 Pipelines powered by language models that run question-answering, labeling, transcription, translation, summarization, LLM prompts and more
+        - ↪️️ Workflows to join pipelines together and aggregate business logic. txtai processes can be simple microservices or multi-model workflows.
         - ⚙️ Build with Python or YAML. API bindings available for [JavaScript](https://github.com/neuml/txtai.js), [Java](https://github.com/neuml/txtai.java), [Rust](https://github.com/neuml/txtai.rs) and [Go](https://github.com/neuml/txtai.go).
         - ☁️ Cloud-native architecture that scales out with container orchestration systems (e.g. Kubernetes)
         
-        Applications range from similarity search to NLP-driven data extractions that generate structured data. Semantic workflows transform and find data driven by user intent.
-        
-        ![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-light-mode-only)
-        
         The following applications are powered by txtai.
         
         ![apps](https://raw.githubusercontent.com/neuml/txtai/master/apps.jpg)
         
         | Application  | Description  |
         |:----------|:-------------|
+        | [txtchat](https://github.com/neuml/txtchat) | Conversational search and workflows for all |
         | [paperai](https://github.com/neuml/paperai) | Semantic search and workflows for medical/scientific papers |
         | [codequestion](https://github.com/neuml/codequestion) | Semantic search for developers |
         | [tldrstory](https://github.com/neuml/tldrstory) | Semantic search for headlines and story text |
-        | [neuspo](https://neuspo.com) | Fact-driven, real-time sports event and news site |
         
         txtai is built with Python 3.7+, [Hugging Face Transformers](https://github.com/huggingface/transformers), [Sentence Transformers](https://github.com/UKPLab/sentence-transformers) and [FastAPI](https://github.com/tiangolo/fastapi)
         
         ## Why txtai?
         
         ![why](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/why.png#gh-light-mode-only)
         
-        In addition to traditional search systems, a growing number of semantic search solutions are available, so why txtai?
+        In addition to traditional search systems, a growing number of language model backed solutions are available, so why txtai?
         
         - Up and running in minutes with [pip](https://neuml.github.io/txtai/install/) or [Docker](https://neuml.github.io/txtai/cloud/)
         ```python
         # Get started in a couple lines
         from txtai.embeddings import Embeddings
         
         embeddings = Embeddings({"path": "sentence-transformers/all-MiniLM-L6-v2"})
         embeddings.index([(0, "Correct", None), (1, "Not what we hoped", None)])
         embeddings.search("positive", 1)
         #[(0, 0.2986203730106354)]
         ```
-        - Build applications in your programming language of choice via the API
+        - Built-in API makes it easy to develop applications using your programming language of choice
         ```yaml
         # app.yml
         embeddings:
             path: sentence-transformers/all-MiniLM-L6-v2
         ```
         ```bash
         CONFIG=app.yml uvicorn "txtai.api:app"
         curl -X GET "http://localhost:8000/search?query=positive"
         ```
-        - Connect machine learning models together to build intelligent data processing workflows
-        - Works with both small and big data - scale when needed
-        - Supports micromodels all the way up to large language models (LLMs)
-        - Low footprint - install additional dependencies when you need them
+        - Run local - no need to ship data off to disparate remote services
+        - Work with micromodels all the way up to large language models (LLMs)
+        - Low footprint - install additional dependencies and scale up when needed
         - [Learn by example](#examples) - notebooks cover all available functionality
         
         ## Installation
         
         ![install](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/install.png#gh-light-mode-only)
         
         The easiest way to install is via pip and PyPI
@@ -150,15 +151,15 @@
         | [Semantic Graphs](https://github.com/neuml/txtai/blob/master/examples/38_Introducing_the_Semantic_Graph.ipynb) | Explore topics, data connectivity and run network analysis| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/38_Introducing_the_Semantic_Graph.ipynb) |
         | [Topic Modeling with BM25](https://github.com/neuml/txtai/blob/master/examples/39_Classic_Topic_Modeling_with_BM25.ipynb) | Topic modeling backed by a BM25 index | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/39_Classic_Topic_Modeling_with_BM25.ipynb) |
         | [Prompt-driven search with LLMs](https://github.com/neuml/txtai/blob/master/examples/42_Prompt_driven_search_with_LLMs.ipynb) | Embeddings-guided and Prompt-driven search with Large Language Models (LLMs) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/42_Prompt_driven_search_with_LLMs.ipynb) |
         | [Embeddings in the Cloud](https://github.com/neuml/txtai/blob/master/examples/43_Embeddings_in_the_Cloud.ipynb) | Load and use an embeddings index from the Hugging Face Hub | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/43_Embeddings_in_the_Cloud.ipynb) |
         
         ### Pipelines
         
-        Transform data with NLP-backed pipelines.
+        Transform data with language model backed pipelines.
         
         | Notebook  | Description  |       |
         |:----------|:-------------|------:|
         | [Extractive QA with txtai](https://github.com/neuml/txtai/blob/master/examples/05_Extractive_QA_with_txtai.ipynb) | Introduction to extractive question-answering with txtai | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/05_Extractive_QA_with_txtai.ipynb) |
         | [Extractive QA with Elasticsearch](https://github.com/neuml/txtai/blob/master/examples/06_Extractive_QA_with_Elasticsearch.ipynb) | Run extractive question-answering queries with Elasticsearch | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/06_Extractive_QA_with_Elasticsearch.ipynb) |
         | [Extractive QA to build structured data](https://github.com/neuml/txtai/blob/master/examples/20_Extractive_QA_to_build_structured_data.ipynb) | Build structured datasets using extractive question-answering | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/20_Extractive_QA_to_build_structured_data.ipynb) |
         | [Apply labels with zero shot classification](https://github.com/neuml/txtai/blob/master/examples/07_Apply_labels_with_zero_shot_classification.ipynb) | Use zero shot learning for labeling, classification and topic modeling | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/07_Apply_labels_with_zero_shot_classification.ipynb) |
@@ -217,19 +218,19 @@
         
         [Full documentation on txtai](https://neuml.github.io/txtai) including configuration settings for pipelines, workflows, indexing and the API.
         
         ## Further Reading
         
         ![further](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/further.png)
         
-        - [Introducing txtai, AI-powered semantic search built on Transformers](https://medium.com/neuml/introducing-txtai-an-ai-powered-search-engine-built-on-transformers-37674be252ec)
+        - [Introducing txtai, semantic search and workflows built on Transformers](https://medium.com/neuml/introducing-txtai-an-ai-powered-search-engine-built-on-transformers-37674be252ec)
         - [Tutorial series on Hashnode](https://neuml.hashnode.dev/series/txtai-tutorial) | [dev.to](https://dev.to/neuml/tutorial-series-on-txtai-ibg)
         - [What's new in txtai 5.0](https://medium.com/neuml/whats-new-in-txtai-5-0-e5c75a13b101) | [4.0](https://medium.com/neuml/whats-new-in-txtai-4-0-bbc3a65c3d1c)
         - [Getting started with semantic search](https://medium.com/neuml/getting-started-with-semantic-search-a9fd9d8a48cf) | [workflows](https://medium.com/neuml/getting-started-with-semantic-workflows-2fefda6165d9)
-        - [Run machine-learning workflows to transform data and build AI-powered semantic search applications with txtai](https://medium.com/neuml/run-machine-learning-workflows-to-transform-data-and-build-ai-powered-text-indices-with-txtai-43d769b566a7)
+        - [Run workflows to transform data and build semantic search applications with txtai](https://medium.com/neuml/run-machine-learning-workflows-to-transform-data-and-build-ai-powered-text-indices-with-txtai-43d769b566a7)
         - [Semantic search on the cheap](https://medium.com/neuml/semantic-search-on-the-cheap-55940c0fcdab)
         - [Serverless vector search with txtai](https://medium.com/neuml/serverless-vector-search-with-txtai-96f6163ab972)
         - [Insights from the txtai console](https://medium.com/neuml/insights-from-the-txtai-console-d307c28e149e)
         - [The big and small of txtai](https://medium.com/neuml/the-big-and-small-of-txtai-4ca405c1b82)
         
         ## Contributing
```

#### html2text {}

```diff
@@ -1,73 +1,74 @@
-Metadata-Version: 2.1 Name: txtai Version: 5.4.0 Summary: Build AI-powered
-semantic search applications Home-page: https://github.com/neuml/txtai Author:
-NeuML License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0 Project-
-URL: Documentation, https://github.com/neuml/txtai Project-URL: Issue Tracker,
-https://github.com/neuml/txtai/issues Project-URL: Source Code, https://
-github.com/neuml/txtai Description:
+Metadata-Version: 2.1 Name: txtai Version: 5.5.0 Summary: Semantic search and
+workflows powered by language models Home-page: https://github.com/neuml/txtai
+Author: NeuML License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0
+Project-URL: Documentation, https://github.com/neuml/txtai Project-URL: Issue
+Tracker, https://github.com/neuml/txtai/issues Project-URL: Source Code, https:
+//github.com/neuml/txtai Description:
         [https://raw.githubusercontent.com/neuml/txtai/master/logo.png]
-            **** Build AI-powered semantic search applications ****
+      **** Semantic search and workflows powered by language models ****
   [Version] [GitHub_last_commit] [GitHub_issues] [Join_Slack] [Build_Status]
                                [Coverage_Status]
 -------------------------------------------------------------------------------
 ------------------------------------------------------------------------ txtai
-executes machine-learning workflows to transform data and build AI-powered
-semantic search applications. ![demo](https://raw.githubusercontent.com/neuml/
-txtai/master/demo.gif) Traditional search systems use keywords to find data.
-Semantic search applications have an understanding of natural language and
-identify results that have the same meaning, not necessarily the same keywords.
-![search](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/
-search.png#gh-light-mode-only) Backed by state-of-the-art machine learning
-models, data is transformed into vector representations for search (also known
-as embeddings). Innovation is happening at a rapid pace, models can understand
-concepts in documents, audio, images and video. Summary of txtai features: -
-ð Large-scale similarity search with multiple index backends ([Faiss](https:
-//github.com/facebookresearch/faiss), [Annoy](https://github.com/spotify/
-annoy), [Hnswlib](https://github.com/nmslib/hnswlib)) and support for external
-vector databases - ð Create embeddings for text snippets, documents, audio,
-images and video - ð¡ Machine-learning pipelines that run question-answering,
-labeling, transcription, translation, summarization, LLM prompts and more -
-âªï¸ï¸ Workflows to join pipelines together and aggregate business logic.
-txtai processes can be microservices or full-fledged indexing workflows. -
-âï¸ Build with Python or YAML. API bindings available for [JavaScript]
-(https://github.com/neuml/txtai.js), [Java](https://github.com/neuml/
-txtai.java), [Rust](https://github.com/neuml/txtai.rs) and [Go](https://
-github.com/neuml/txtai.go). - âï¸ Cloud-native architecture that scales out
-with container orchestration systems (e.g. Kubernetes) Applications range from
-similarity search to NLP-driven data extractions that generate structured data.
-Semantic workflows transform and find data driven by user intent. ![flows]
+is an open-source platform for semantic search and workflows powered by
+language models. ![demo](https://raw.githubusercontent.com/neuml/txtai/master/
+demo.gif) Traditional search systems use keywords to find data. Semantic search
+has an understanding of natural language and identifies results that have the
+same meaning, not necessarily the same keywords. ![search](https://
+raw.githubusercontent.com/neuml/txtai/master/docs/images/search.png#gh-light-
+mode-only) txtai builds embeddings databases, which are a union of vector
+indexes and relational databases. This enables similarity search with SQL.
+Embeddings databases can stand on their own and/or serve as a powerful
+knowledge source for large language model (LLM) prompts. Semantic workflows
+connect language models together to build intelligent applications. ![flows]
 (https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-
-light-mode-only) The following applications are powered by txtai. ![apps]
-(https://raw.githubusercontent.com/neuml/txtai/master/apps.jpg) | Application |
-Description | |:----------|:-------------| | [paperai](https://github.com/
-neuml/paperai) | Semantic search and workflows for medical/scientific papers |
-| [codequestion](https://github.com/neuml/codequestion) | Semantic search for
-developers | | [tldrstory](https://github.com/neuml/tldrstory) | Semantic
-search for headlines and story text | | [neuspo](https://neuspo.com) | Fact-
-driven, real-time sports event and news site | txtai is built with Python 3.7+,
-[Hugging Face Transformers](https://github.com/huggingface/transformers),
-[Sentence Transformers](https://github.com/UKPLab/sentence-transformers) and
-[FastAPI](https://github.com/tiangolo/fastapi) ## Why txtai? ![why](https://
-raw.githubusercontent.com/neuml/txtai/master/docs/images/why.png#gh-light-mode-
-only) In addition to traditional search systems, a growing number of semantic
-search solutions are available, so why txtai? - Up and running in minutes with
-[pip](https://neuml.github.io/txtai/install/) or [Docker](https://
-neuml.github.io/txtai/cloud/) ```python # Get started in a couple lines from
-txtai.embeddings import Embeddings embeddings = Embeddings({"path": "sentence-
-transformers/all-MiniLM-L6-v2"}) embeddings.index([(0, "Correct", None), (1,
-"Not what we hoped", None)]) embeddings.search("positive", 1) #[(0,
-0.2986203730106354)] ``` - Build applications in your programming language of
-choice via the API ```yaml # app.yml embeddings: path: sentence-transformers/
+light-mode-only) Integrate vector search, conversational search, automatic
+summarization, transcription, translation and more. Summary of txtai features:
+- ð Similarity search with SQL, object storage, topic modeling, graph
+analysis, multiple vector index backends ([Faiss](https://github.com/
+facebookresearch/faiss), [Annoy](https://github.com/spotify/annoy), [Hnswlib]
+(https://github.com/nmslib/hnswlib)) and support for external vector databases
+- ð Create embeddings for text, documents, audio, images and video - ð¡
+Pipelines powered by language models that run question-answering, labeling,
+transcription, translation, summarization, LLM prompts and more - âªï¸ï¸
+Workflows to join pipelines together and aggregate business logic. txtai
+processes can be simple microservices or multi-model workflows. - âï¸ Build
+with Python or YAML. API bindings available for [JavaScript](https://
+github.com/neuml/txtai.js), [Java](https://github.com/neuml/txtai.java), [Rust]
+(https://github.com/neuml/txtai.rs) and [Go](https://github.com/neuml/
+txtai.go). - âï¸ Cloud-native architecture that scales out with container
+orchestration systems (e.g. Kubernetes) The following applications are powered
+by txtai. ![apps](https://raw.githubusercontent.com/neuml/txtai/master/
+apps.jpg) | Application | Description | |:----------|:-------------| |
+[txtchat](https://github.com/neuml/txtchat) | Conversational search and
+workflows for all | | [paperai](https://github.com/neuml/paperai) | Semantic
+search and workflows for medical/scientific papers | | [codequestion](https://
+github.com/neuml/codequestion) | Semantic search for developers | | [tldrstory]
+(https://github.com/neuml/tldrstory) | Semantic search for headlines and story
+text | txtai is built with Python 3.7+, [Hugging Face Transformers](https://
+github.com/huggingface/transformers), [Sentence Transformers](https://
+github.com/UKPLab/sentence-transformers) and [FastAPI](https://github.com/
+tiangolo/fastapi) ## Why txtai? ![why](https://raw.githubusercontent.com/neuml/
+txtai/master/docs/images/why.png#gh-light-mode-only) In addition to traditional
+search systems, a growing number of language model backed solutions are
+available, so why txtai? - Up and running in minutes with [pip](https://
+neuml.github.io/txtai/install/) or [Docker](https://neuml.github.io/txtai/
+cloud/) ```python # Get started in a couple lines from txtai.embeddings import
+Embeddings embeddings = Embeddings({"path": "sentence-transformers/all-MiniLM-
+L6-v2"}) embeddings.index([(0, "Correct", None), (1, "Not what we hoped",
+None)]) embeddings.search("positive", 1) #[(0, 0.2986203730106354)] ``` -
+Built-in API makes it easy to develop applications using your programming
+language of choice ```yaml # app.yml embeddings: path: sentence-transformers/
 all-MiniLM-L6-v2 ``` ```bash CONFIG=app.yml uvicorn "txtai.api:app" curl -X GET
-"http://localhost:8000/search?query=positive" ``` - Connect machine learning
-models together to build intelligent data processing workflows - Works with
-both small and big data - scale when needed - Supports micromodels all the way
-up to large language models (LLMs) - Low footprint - install additional
-dependencies when you need them - [Learn by example](#examples) - notebooks
-cover all available functionality ## Installation ![install](https://
+"http://localhost:8000/search?query=positive" ``` - Run local - no need to ship
+data off to disparate remote services - Work with micromodels all the way up to
+large language models (LLMs) - Low footprint - install additional dependencies
+and scale up when needed - [Learn by example](#examples) - notebooks cover all
+available functionality ## Installation ![install](https://
 raw.githubusercontent.com/neuml/txtai/master/docs/images/install.png#gh-light-
 mode-only) The easiest way to install is via pip and PyPI ``` pip install txtai
 ``` Python 3.7+ is supported. Using a Python [virtual environment](https://
 docs.python.org/3/library/venv.html) is recommended. See the detailed [install
 instructions](https://neuml.github.io/txtai/install) for more information
 covering [optional dependencies](https://neuml.github.io/txtai/install/
 #optional-dependencies), [environment specific prerequisites](https://
@@ -165,18 +166,18 @@
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/neuml/txtai/blob/master/examples/
 42_Prompt_driven_search_with_LLMs.ipynb) | | [Embeddings in the Cloud](https://
 github.com/neuml/txtai/blob/master/examples/43_Embeddings_in_the_Cloud.ipynb) |
 Load and use an embeddings index from the Hugging Face Hub | [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/neuml/txtai/blob/master/examples/
-43_Embeddings_in_the_Cloud.ipynb) | ### Pipelines Transform data with NLP-
-backed pipelines. | Notebook | Description | | |:----------|:-------------|----
---:| | [Extractive QA with txtai](https://github.com/neuml/txtai/blob/master/
-examples/05_Extractive_QA_with_txtai.ipynb) | Introduction to extractive
+43_Embeddings_in_the_Cloud.ipynb) | ### Pipelines Transform data with language
+model backed pipelines. | Notebook | Description | | |:----------|:------------
+-|------:| | [Extractive QA with txtai](https://github.com/neuml/txtai/blob/
+master/examples/05_Extractive_QA_with_txtai.ipynb) | Introduction to extractive
 question-answering with txtai | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/neuml/txtai/blob/master/examples/
 05_Extractive_QA_with_txtai.ipynb) | | [Extractive QA with Elasticsearch]
 (https://github.com/neuml/txtai/blob/master/examples/
 06_Extractive_QA_with_Elasticsearch.ipynb) | Run extractive question-answering
 queries with Elasticsearch | [![Open In Colab](https://
@@ -338,29 +339,29 @@
 examples/workflows.py) | Build and execute txtai workflows. Connect
 summarization, text extraction, transcription, translation and similarity
 search pipelines together to run unified workflows. |[ð¤](https://hf.co/
 spaces/NeuML/txtai)| ## Documentation [Full documentation on txtai](https://
 neuml.github.io/txtai) including configuration settings for pipelines,
 workflows, indexing and the API. ## Further Reading ![further](https://
 raw.githubusercontent.com/neuml/txtai/master/docs/images/further.png) -
-[Introducing txtai, AI-powered semantic search built on Transformers](https://
-medium.com/neuml/introducing-txtai-an-ai-powered-search-engine-built-on-
+[Introducing txtai, semantic search and workflows built on Transformers](https:
+//medium.com/neuml/introducing-txtai-an-ai-powered-search-engine-built-on-
 transformers-37674be252ec) - [Tutorial series on Hashnode](https://
 neuml.hashnode.dev/series/txtai-tutorial) | [dev.to](https://dev.to/neuml/
 tutorial-series-on-txtai-ibg) - [What's new in txtai 5.0](https://medium.com/
 neuml/whats-new-in-txtai-5-0-e5c75a13b101) | [4.0](https://medium.com/neuml/
 whats-new-in-txtai-4-0-bbc3a65c3d1c) - [Getting started with semantic search]
 (https://medium.com/neuml/getting-started-with-semantic-search-a9fd9d8a48cf) |
 [workflows](https://medium.com/neuml/getting-started-with-semantic-workflows-
-2fefda6165d9) - [Run machine-learning workflows to transform data and build AI-
-powered semantic search applications with txtai](https://medium.com/neuml/run-
-machine-learning-workflows-to-transform-data-and-build-ai-powered-text-indices-
-with-txtai-43d769b566a7) - [Semantic search on the cheap](https://medium.com/
-neuml/semantic-search-on-the-cheap-55940c0fcdab) - [Serverless vector search
-with txtai](https://medium.com/neuml/serverless-vector-search-with-txtai-
+2fefda6165d9) - [Run workflows to transform data and build semantic search
+applications with txtai](https://medium.com/neuml/run-machine-learning-
+workflows-to-transform-data-and-build-ai-powered-text-indices-with-txtai-
+43d769b566a7) - [Semantic search on the cheap](https://medium.com/neuml/
+semantic-search-on-the-cheap-55940c0fcdab) - [Serverless vector search with
+txtai](https://medium.com/neuml/serverless-vector-search-with-txtai-
 96f6163ab972) - [Insights from the txtai console](https://medium.com/neuml/
 insights-from-the-txtai-console-d307c28e149e) - [The big and small of txtai]
 (https://medium.com/neuml/the-big-and-small-of-txtai-4ca405c1b82) ##
 Contributing For those who would like to contribute to txtai, please see [this
 guide](https://github.com/neuml/.github/blob/master/CONTRIBUTING.md). Keywords:
 search embedding machine-learning nlp Platform: UNKNOWN Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
```

### Comparing `txtai-5.4.0/README.md` & `txtai-5.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <p align="center">
     <img src="https://raw.githubusercontent.com/neuml/txtai/master/logo.png"/>
 </p>
 
 <h3 align="center">
-    <p>Build AI-powered semantic search applications</p>
+    <p>Semantic search and workflows powered by language models</p>
 </h3>
 
 <p align="center">
     <a href="https://github.com/neuml/txtai/releases">
         <img src="https://img.shields.io/github/release/neuml/txtai.svg?style=flat&color=success" alt="Version"/>
     </a>
     <a href="https://github.com/neuml/txtai">
@@ -25,83 +25,84 @@
     <a href="https://coveralls.io/github/neuml/txtai?branch=master">
         <img src="https://img.shields.io/coverallsCoverage/github/neuml/txtai" alt="Coverage Status">
     </a>
 </p>
 
 -------------------------------------------------------------------------------------------------------------------------------------------------------
 
-txtai executes machine-learning workflows to transform data and build AI-powered semantic search applications.
+txtai is an open-source platform for semantic search and workflows powered by language models.
 
 ![demo](https://raw.githubusercontent.com/neuml/txtai/master/demo.gif)
 
-Traditional search systems use keywords to find data. Semantic search applications have an understanding of natural language and identify results that have the same meaning, not necessarily the same keywords.
+Traditional search systems use keywords to find data. Semantic search has an understanding of natural language and identifies results that have the same meaning, not necessarily the same keywords.
 
 ![search](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/search.png#gh-light-mode-only)
 ![search](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/search-dark.png#gh-dark-mode-only)
 
-Backed by state-of-the-art machine learning models, data is transformed into vector representations for search (also known as embeddings). Innovation is happening at a rapid pace, models can understand concepts in documents, audio, images and video.
+txtai builds embeddings databases, which are a union of vector indexes and relational databases. This enables similarity search with SQL. Embeddings databases can stand on their own and/or serve as a powerful knowledge source for large language model (LLM) prompts.
+
+Semantic workflows connect language models together to build intelligent applications.
+
+![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-light-mode-only)
+![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows-dark.png#gh-dark-mode-only)
+
+Integrate vector search, conversational search, automatic summarization, transcription, translation and more.
 
 Summary of txtai features:
 
-- 🔎 Large-scale similarity search with multiple index backends ([Faiss](https://github.com/facebookresearch/faiss), [Annoy](https://github.com/spotify/annoy), [Hnswlib](https://github.com/nmslib/hnswlib)) and support for external vector databases
-- 📄 Create embeddings for text snippets, documents, audio, images and video
-- 💡 Machine-learning pipelines that run question-answering, labeling, transcription, translation, summarization, LLM prompts and more
-- ↪️️ Workflows to join pipelines together and aggregate business logic. txtai processes can be microservices or full-fledged indexing workflows.
+- 🔎 Similarity search with SQL, object storage, topic modeling, graph analysis, multiple vector index backends ([Faiss](https://github.com/facebookresearch/faiss), [Annoy](https://github.com/spotify/annoy), [Hnswlib](https://github.com/nmslib/hnswlib)) and support for external vector databases
+- 📄 Create embeddings for text, documents, audio, images and video
+- 💡 Pipelines powered by language models that run question-answering, labeling, transcription, translation, summarization, LLM prompts and more
+- ↪️️ Workflows to join pipelines together and aggregate business logic. txtai processes can be simple microservices or multi-model workflows.
 - ⚙️ Build with Python or YAML. API bindings available for [JavaScript](https://github.com/neuml/txtai.js), [Java](https://github.com/neuml/txtai.java), [Rust](https://github.com/neuml/txtai.rs) and [Go](https://github.com/neuml/txtai.go).
 - ☁️ Cloud-native architecture that scales out with container orchestration systems (e.g. Kubernetes)
 
-Applications range from similarity search to NLP-driven data extractions that generate structured data. Semantic workflows transform and find data driven by user intent.
-
-![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-light-mode-only)
-![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows-dark.png#gh-dark-mode-only)
-
 The following applications are powered by txtai.
 
 ![apps](https://raw.githubusercontent.com/neuml/txtai/master/apps.jpg)
 
 | Application  | Description  |
 |:----------|:-------------|
+| [txtchat](https://github.com/neuml/txtchat) | Conversational search and workflows for all |
 | [paperai](https://github.com/neuml/paperai) | Semantic search and workflows for medical/scientific papers |
 | [codequestion](https://github.com/neuml/codequestion) | Semantic search for developers |
 | [tldrstory](https://github.com/neuml/tldrstory) | Semantic search for headlines and story text |
-| [neuspo](https://neuspo.com) | Fact-driven, real-time sports event and news site |
 
 txtai is built with Python 3.7+, [Hugging Face Transformers](https://github.com/huggingface/transformers), [Sentence Transformers](https://github.com/UKPLab/sentence-transformers) and [FastAPI](https://github.com/tiangolo/fastapi)
 
 ## Why txtai?
 
 ![why](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/why.png#gh-light-mode-only)
 ![why](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/why-dark.png#gh-dark-mode-only)
 
-In addition to traditional search systems, a growing number of semantic search solutions are available, so why txtai?
+In addition to traditional search systems, a growing number of language model backed solutions are available, so why txtai?
 
 - Up and running in minutes with [pip](https://neuml.github.io/txtai/install/) or [Docker](https://neuml.github.io/txtai/cloud/)
 ```python
 # Get started in a couple lines
 from txtai.embeddings import Embeddings
 
 embeddings = Embeddings({"path": "sentence-transformers/all-MiniLM-L6-v2"})
 embeddings.index([(0, "Correct", None), (1, "Not what we hoped", None)])
 embeddings.search("positive", 1)
 #[(0, 0.2986203730106354)]
 ```
-- Build applications in your programming language of choice via the API
+- Built-in API makes it easy to develop applications using your programming language of choice
 ```yaml
 # app.yml
 embeddings:
     path: sentence-transformers/all-MiniLM-L6-v2
 ```
 ```bash
 CONFIG=app.yml uvicorn "txtai.api:app"
 curl -X GET "http://localhost:8000/search?query=positive"
 ```
-- Connect machine learning models together to build intelligent data processing workflows
-- Works with both small and big data - scale when needed
-- Supports micromodels all the way up to large language models (LLMs)
-- Low footprint - install additional dependencies when you need them
+- Run local - no need to ship data off to disparate remote services
+- Work with micromodels all the way up to large language models (LLMs)
+- Low footprint - install additional dependencies and scale up when needed
 - [Learn by example](#examples) - notebooks cover all available functionality
 
 ## Installation
 
 ![install](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/install.png#gh-light-mode-only)
 ![install](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/install-dark.png#gh-dark-mode-only)
 
@@ -145,15 +146,15 @@
 | [Semantic Graphs](https://github.com/neuml/txtai/blob/master/examples/38_Introducing_the_Semantic_Graph.ipynb) | Explore topics, data connectivity and run network analysis| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/38_Introducing_the_Semantic_Graph.ipynb) |
 | [Topic Modeling with BM25](https://github.com/neuml/txtai/blob/master/examples/39_Classic_Topic_Modeling_with_BM25.ipynb) | Topic modeling backed by a BM25 index | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/39_Classic_Topic_Modeling_with_BM25.ipynb) |
 | [Prompt-driven search with LLMs](https://github.com/neuml/txtai/blob/master/examples/42_Prompt_driven_search_with_LLMs.ipynb) | Embeddings-guided and Prompt-driven search with Large Language Models (LLMs) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/42_Prompt_driven_search_with_LLMs.ipynb) |
 | [Embeddings in the Cloud](https://github.com/neuml/txtai/blob/master/examples/43_Embeddings_in_the_Cloud.ipynb) | Load and use an embeddings index from the Hugging Face Hub | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/43_Embeddings_in_the_Cloud.ipynb) |
 
 ### Pipelines
 
-Transform data with NLP-backed pipelines.
+Transform data with language model backed pipelines.
 
 | Notebook  | Description  |       |
 |:----------|:-------------|------:|
 | [Extractive QA with txtai](https://github.com/neuml/txtai/blob/master/examples/05_Extractive_QA_with_txtai.ipynb) | Introduction to extractive question-answering with txtai | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/05_Extractive_QA_with_txtai.ipynb) |
 | [Extractive QA with Elasticsearch](https://github.com/neuml/txtai/blob/master/examples/06_Extractive_QA_with_Elasticsearch.ipynb) | Run extractive question-answering queries with Elasticsearch | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/06_Extractive_QA_with_Elasticsearch.ipynb) |
 | [Extractive QA to build structured data](https://github.com/neuml/txtai/blob/master/examples/20_Extractive_QA_to_build_structured_data.ipynb) | Build structured datasets using extractive question-answering | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/20_Extractive_QA_to_build_structured_data.ipynb) |
 | [Apply labels with zero shot classification](https://github.com/neuml/txtai/blob/master/examples/07_Apply_labels_with_zero_shot_classification.ipynb) | Use zero shot learning for labeling, classification and topic modeling | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/07_Apply_labels_with_zero_shot_classification.ipynb) |
@@ -212,19 +213,19 @@
 
 [Full documentation on txtai](https://neuml.github.io/txtai) including configuration settings for pipelines, workflows, indexing and the API.
 
 ## Further Reading
 
 ![further](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/further.png)
 
-- [Introducing txtai, AI-powered semantic search built on Transformers](https://medium.com/neuml/introducing-txtai-an-ai-powered-search-engine-built-on-transformers-37674be252ec)
+- [Introducing txtai, semantic search and workflows built on Transformers](https://medium.com/neuml/introducing-txtai-an-ai-powered-search-engine-built-on-transformers-37674be252ec)
 - [Tutorial series on Hashnode](https://neuml.hashnode.dev/series/txtai-tutorial) | [dev.to](https://dev.to/neuml/tutorial-series-on-txtai-ibg)
 - [What's new in txtai 5.0](https://medium.com/neuml/whats-new-in-txtai-5-0-e5c75a13b101) | [4.0](https://medium.com/neuml/whats-new-in-txtai-4-0-bbc3a65c3d1c)
 - [Getting started with semantic search](https://medium.com/neuml/getting-started-with-semantic-search-a9fd9d8a48cf) | [workflows](https://medium.com/neuml/getting-started-with-semantic-workflows-2fefda6165d9)
-- [Run machine-learning workflows to transform data and build AI-powered semantic search applications with txtai](https://medium.com/neuml/run-machine-learning-workflows-to-transform-data-and-build-ai-powered-text-indices-with-txtai-43d769b566a7)
+- [Run workflows to transform data and build semantic search applications with txtai](https://medium.com/neuml/run-machine-learning-workflows-to-transform-data-and-build-ai-powered-text-indices-with-txtai-43d769b566a7)
 - [Semantic search on the cheap](https://medium.com/neuml/semantic-search-on-the-cheap-55940c0fcdab)
 - [Serverless vector search with txtai](https://medium.com/neuml/serverless-vector-search-with-txtai-96f6163ab972)
 - [Insights from the txtai console](https://medium.com/neuml/insights-from-the-txtai-console-d307c28e149e)
 - [The big and small of txtai](https://medium.com/neuml/the-big-and-small-of-txtai-4ca405c1b82)
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,70 +1,71 @@
         [https://raw.githubusercontent.com/neuml/txtai/master/logo.png]
-            **** Build AI-powered semantic search applications ****
+      **** Semantic search and workflows powered by language models ****
   [Version] [GitHub_last_commit] [GitHub_issues] [Join_Slack] [Build_Status]
                                [Coverage_Status]
 -------------------------------------------------------------------------------
 ------------------------------------------------------------------------ txtai
-executes machine-learning workflows to transform data and build AI-powered
-semantic search applications. ![demo](https://raw.githubusercontent.com/neuml/
-txtai/master/demo.gif) Traditional search systems use keywords to find data.
-Semantic search applications have an understanding of natural language and
-identify results that have the same meaning, not necessarily the same keywords.
-![search](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/
-search.png#gh-light-mode-only) ![search](https://raw.githubusercontent.com/
-neuml/txtai/master/docs/images/search-dark.png#gh-dark-mode-only) Backed by
-state-of-the-art machine learning models, data is transformed into vector
-representations for search (also known as embeddings). Innovation is happening
-at a rapid pace, models can understand concepts in documents, audio, images and
-video. Summary of txtai features: - ð Large-scale similarity search with
-multiple index backends ([Faiss](https://github.com/facebookresearch/faiss),
-[Annoy](https://github.com/spotify/annoy), [Hnswlib](https://github.com/nmslib/
-hnswlib)) and support for external vector databases - ð Create embeddings
-for text snippets, documents, audio, images and video - ð¡ Machine-learning
-pipelines that run question-answering, labeling, transcription, translation,
-summarization, LLM prompts and more - âªï¸ï¸ Workflows to join pipelines
-together and aggregate business logic. txtai processes can be microservices or
-full-fledged indexing workflows. - âï¸ Build with Python or YAML. API
-bindings available for [JavaScript](https://github.com/neuml/txtai.js), [Java]
-(https://github.com/neuml/txtai.java), [Rust](https://github.com/neuml/
-txtai.rs) and [Go](https://github.com/neuml/txtai.go). - âï¸ Cloud-native
-architecture that scales out with container orchestration systems (e.g.
-Kubernetes) Applications range from similarity search to NLP-driven data
-extractions that generate structured data. Semantic workflows transform and
-find data driven by user intent. ![flows](https://raw.githubusercontent.com/
-neuml/txtai/master/docs/images/flows.png#gh-light-mode-only) ![flows](https://
+is an open-source platform for semantic search and workflows powered by
+language models. ![demo](https://raw.githubusercontent.com/neuml/txtai/master/
+demo.gif) Traditional search systems use keywords to find data. Semantic search
+has an understanding of natural language and identifies results that have the
+same meaning, not necessarily the same keywords. ![search](https://
+raw.githubusercontent.com/neuml/txtai/master/docs/images/search.png#gh-light-
+mode-only) ![search](https://raw.githubusercontent.com/neuml/txtai/master/docs/
+images/search-dark.png#gh-dark-mode-only) txtai builds embeddings databases,
+which are a union of vector indexes and relational databases. This enables
+similarity search with SQL. Embeddings databases can stand on their own and/or
+serve as a powerful knowledge source for large language model (LLM) prompts.
+Semantic workflows connect language models together to build intelligent
+applications. ![flows](https://raw.githubusercontent.com/neuml/txtai/master/
+docs/images/flows.png#gh-light-mode-only) ![flows](https://
 raw.githubusercontent.com/neuml/txtai/master/docs/images/flows-dark.png#gh-
-dark-mode-only) The following applications are powered by txtai. ![apps](https:
-//raw.githubusercontent.com/neuml/txtai/master/apps.jpg) | Application |
-Description | |:----------|:-------------| | [paperai](https://github.com/
-neuml/paperai) | Semantic search and workflows for medical/scientific papers |
-| [codequestion](https://github.com/neuml/codequestion) | Semantic search for
-developers | | [tldrstory](https://github.com/neuml/tldrstory) | Semantic
-search for headlines and story text | | [neuspo](https://neuspo.com) | Fact-
-driven, real-time sports event and news site | txtai is built with Python 3.7+,
-[Hugging Face Transformers](https://github.com/huggingface/transformers),
-[Sentence Transformers](https://github.com/UKPLab/sentence-transformers) and
-[FastAPI](https://github.com/tiangolo/fastapi) ## Why txtai? ![why](https://
-raw.githubusercontent.com/neuml/txtai/master/docs/images/why.png#gh-light-mode-
-only) ![why](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/
-why-dark.png#gh-dark-mode-only) In addition to traditional search systems, a
-growing number of semantic search solutions are available, so why txtai? - Up
-and running in minutes with [pip](https://neuml.github.io/txtai/install/) or
-[Docker](https://neuml.github.io/txtai/cloud/) ```python # Get started in a
-couple lines from txtai.embeddings import Embeddings embeddings = Embeddings(
-{"path": "sentence-transformers/all-MiniLM-L6-v2"}) embeddings.index([(0,
-"Correct", None), (1, "Not what we hoped", None)]) embeddings.search
-("positive", 1) #[(0, 0.2986203730106354)] ``` - Build applications in your
-programming language of choice via the API ```yaml # app.yml embeddings: path:
+dark-mode-only) Integrate vector search, conversational search, automatic
+summarization, transcription, translation and more. Summary of txtai features:
+- ð Similarity search with SQL, object storage, topic modeling, graph
+analysis, multiple vector index backends ([Faiss](https://github.com/
+facebookresearch/faiss), [Annoy](https://github.com/spotify/annoy), [Hnswlib]
+(https://github.com/nmslib/hnswlib)) and support for external vector databases
+- ð Create embeddings for text, documents, audio, images and video - ð¡
+Pipelines powered by language models that run question-answering, labeling,
+transcription, translation, summarization, LLM prompts and more - âªï¸ï¸
+Workflows to join pipelines together and aggregate business logic. txtai
+processes can be simple microservices or multi-model workflows. - âï¸ Build
+with Python or YAML. API bindings available for [JavaScript](https://
+github.com/neuml/txtai.js), [Java](https://github.com/neuml/txtai.java), [Rust]
+(https://github.com/neuml/txtai.rs) and [Go](https://github.com/neuml/
+txtai.go). - âï¸ Cloud-native architecture that scales out with container
+orchestration systems (e.g. Kubernetes) The following applications are powered
+by txtai. ![apps](https://raw.githubusercontent.com/neuml/txtai/master/
+apps.jpg) | Application | Description | |:----------|:-------------| |
+[txtchat](https://github.com/neuml/txtchat) | Conversational search and
+workflows for all | | [paperai](https://github.com/neuml/paperai) | Semantic
+search and workflows for medical/scientific papers | | [codequestion](https://
+github.com/neuml/codequestion) | Semantic search for developers | | [tldrstory]
+(https://github.com/neuml/tldrstory) | Semantic search for headlines and story
+text | txtai is built with Python 3.7+, [Hugging Face Transformers](https://
+github.com/huggingface/transformers), [Sentence Transformers](https://
+github.com/UKPLab/sentence-transformers) and [FastAPI](https://github.com/
+tiangolo/fastapi) ## Why txtai? ![why](https://raw.githubusercontent.com/neuml/
+txtai/master/docs/images/why.png#gh-light-mode-only) ![why](https://
+raw.githubusercontent.com/neuml/txtai/master/docs/images/why-dark.png#gh-dark-
+mode-only) In addition to traditional search systems, a growing number of
+language model backed solutions are available, so why txtai? - Up and running
+in minutes with [pip](https://neuml.github.io/txtai/install/) or [Docker]
+(https://neuml.github.io/txtai/cloud/) ```python # Get started in a couple
+lines from txtai.embeddings import Embeddings embeddings = Embeddings({"path":
+"sentence-transformers/all-MiniLM-L6-v2"}) embeddings.index([(0, "Correct",
+None), (1, "Not what we hoped", None)]) embeddings.search("positive", 1) #[(0,
+0.2986203730106354)] ``` - Built-in API makes it easy to develop applications
+using your programming language of choice ```yaml # app.yml embeddings: path:
 sentence-transformers/all-MiniLM-L6-v2 ``` ```bash CONFIG=app.yml uvicorn
 "txtai.api:app" curl -X GET "http://localhost:8000/search?query=positive" ``` -
-Connect machine learning models together to build intelligent data processing
-workflows - Works with both small and big data - scale when needed - Supports
+Run local - no need to ship data off to disparate remote services - Work with
 micromodels all the way up to large language models (LLMs) - Low footprint -
-install additional dependencies when you need them - [Learn by example]
+install additional dependencies and scale up when needed - [Learn by example]
 (#examples) - notebooks cover all available functionality ## Installation !
 [install](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/
 install.png#gh-light-mode-only) ![install](https://raw.githubusercontent.com/
 neuml/txtai/master/docs/images/install-dark.png#gh-dark-mode-only) The easiest
 way to install is via pip and PyPI ``` pip install txtai ``` Python 3.7+ is
 supported. Using a Python [virtual environment](https://docs.python.org/3/
 library/venv.html) is recommended. See the detailed [install instructions]
@@ -166,18 +167,18 @@
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/neuml/txtai/blob/master/examples/
 42_Prompt_driven_search_with_LLMs.ipynb) | | [Embeddings in the Cloud](https://
 github.com/neuml/txtai/blob/master/examples/43_Embeddings_in_the_Cloud.ipynb) |
 Load and use an embeddings index from the Hugging Face Hub | [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/neuml/txtai/blob/master/examples/
-43_Embeddings_in_the_Cloud.ipynb) | ### Pipelines Transform data with NLP-
-backed pipelines. | Notebook | Description | | |:----------|:-------------|----
---:| | [Extractive QA with txtai](https://github.com/neuml/txtai/blob/master/
-examples/05_Extractive_QA_with_txtai.ipynb) | Introduction to extractive
+43_Embeddings_in_the_Cloud.ipynb) | ### Pipelines Transform data with language
+model backed pipelines. | Notebook | Description | | |:----------|:------------
+-|------:| | [Extractive QA with txtai](https://github.com/neuml/txtai/blob/
+master/examples/05_Extractive_QA_with_txtai.ipynb) | Introduction to extractive
 question-answering with txtai | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/neuml/txtai/blob/master/examples/
 05_Extractive_QA_with_txtai.ipynb) | | [Extractive QA with Elasticsearch]
 (https://github.com/neuml/txtai/blob/master/examples/
 06_Extractive_QA_with_Elasticsearch.ipynb) | Run extractive question-answering
 queries with Elasticsearch | [![Open In Colab](https://
@@ -339,27 +340,27 @@
 examples/workflows.py) | Build and execute txtai workflows. Connect
 summarization, text extraction, transcription, translation and similarity
 search pipelines together to run unified workflows. |[ð¤](https://hf.co/
 spaces/NeuML/txtai)| ## Documentation [Full documentation on txtai](https://
 neuml.github.io/txtai) including configuration settings for pipelines,
 workflows, indexing and the API. ## Further Reading ![further](https://
 raw.githubusercontent.com/neuml/txtai/master/docs/images/further.png) -
-[Introducing txtai, AI-powered semantic search built on Transformers](https://
-medium.com/neuml/introducing-txtai-an-ai-powered-search-engine-built-on-
+[Introducing txtai, semantic search and workflows built on Transformers](https:
+//medium.com/neuml/introducing-txtai-an-ai-powered-search-engine-built-on-
 transformers-37674be252ec) - [Tutorial series on Hashnode](https://
 neuml.hashnode.dev/series/txtai-tutorial) | [dev.to](https://dev.to/neuml/
 tutorial-series-on-txtai-ibg) - [What's new in txtai 5.0](https://medium.com/
 neuml/whats-new-in-txtai-5-0-e5c75a13b101) | [4.0](https://medium.com/neuml/
 whats-new-in-txtai-4-0-bbc3a65c3d1c) - [Getting started with semantic search]
 (https://medium.com/neuml/getting-started-with-semantic-search-a9fd9d8a48cf) |
 [workflows](https://medium.com/neuml/getting-started-with-semantic-workflows-
-2fefda6165d9) - [Run machine-learning workflows to transform data and build AI-
-powered semantic search applications with txtai](https://medium.com/neuml/run-
-machine-learning-workflows-to-transform-data-and-build-ai-powered-text-indices-
-with-txtai-43d769b566a7) - [Semantic search on the cheap](https://medium.com/
-neuml/semantic-search-on-the-cheap-55940c0fcdab) - [Serverless vector search
-with txtai](https://medium.com/neuml/serverless-vector-search-with-txtai-
+2fefda6165d9) - [Run workflows to transform data and build semantic search
+applications with txtai](https://medium.com/neuml/run-machine-learning-
+workflows-to-transform-data-and-build-ai-powered-text-indices-with-txtai-
+43d769b566a7) - [Semantic search on the cheap](https://medium.com/neuml/
+semantic-search-on-the-cheap-55940c0fcdab) - [Serverless vector search with
+txtai](https://medium.com/neuml/serverless-vector-search-with-txtai-
 96f6163ab972) - [Insights from the txtai console](https://medium.com/neuml/
 insights-from-the-txtai-console-d307c28e149e) - [The big and small of txtai]
 (https://medium.com/neuml/the-big-and-small-of-txtai-4ca405c1b82) ##
 Contributing For those who would like to contribute to txtai, please see [this
 guide](https://github.com/neuml/.github/blob/master/CONTRIBUTING.md).
```

### Comparing `txtai-5.4.0/setup.py` & `txtai-5.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "uvicorn>=0.12.1",
 ]
 
 extras["cloud"] = ["apache-libcloud>=3.3.1"]
 
 extras["console"] = ["rich>=12.0.1"]
 
-extras["database"] = ["pillow>=7.1.2"]
+extras["database"] = ["duckdb>=0.7.1", "pillow>=7.1.2"]
 
 extras["graph"] = ["networkx>=2.6.3", "python-louvain>=0.16"]
 
 extras["model"] = ["onnx>=1.11.0", "onnxruntime>=1.11.0"]
 
 extras["pipeline-audio"] = ["onnx>=1.11.0", "onnxruntime>=1.11.0", "soundfile>=0.10.3.post1", "scipy>=1.4.1", "ttstokenizer>=1.0.0"]
 
@@ -73,17 +73,17 @@
     + extras["pipeline"]
     + extras["similarity"]
     + extras["workflow"]
 )
 
 setup(
     name="txtai",
-    version="5.4.0",
+    version="5.5.0",
     author="NeuML",
-    description="Build AI-powered semantic search applications",
+    description="Semantic search and workflows powered by language models",
     long_description=DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/neuml/txtai",
     project_urls={
         "Documentation": "https://github.com/neuml/txtai",
         "Issue Tracker": "https://github.com/neuml/txtai/issues",
         "Source Code": "https://github.com/neuml/txtai",
```

### Comparing `txtai-5.4.0/src/python/txtai/ann/annoy.py` & `txtai-5.5.0/src/python/txtai/ann/annoy.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/ann/base.py` & `txtai-5.5.0/src/python/txtai/ann/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import platform
 
 from .. import __version__
 
 
 class ANN:
     """
-    Base class for ANN instances.
+    Base class for ANN instances. This class builds vector indexes to support similarity search.
+    The built-in ANN backends store ids and vectors. Content storage is supported via database instances.
     """
 
     def __init__(self, config):
         """
         Creates a new ANN.
 
         Args:
```

### Comparing `txtai-5.4.0/src/python/txtai/ann/factory.py` & `txtai-5.5.0/src/python/txtai/ann/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/ann/faiss.py` & `txtai-5.5.0/src/python/txtai/ann/faiss.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/ann/hnsw.py` & `txtai-5.5.0/src/python/txtai/ann/hnsw.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/application.py` & `txtai-5.5.0/src/python/txtai/api/application.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/base.py` & `txtai-5.5.0/src/python/txtai/api/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/cluster.py` & `txtai-5.5.0/src/python/txtai/api/cluster.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/factory.py` & `txtai-5.5.0/src/python/txtai/api/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/routers/caption.py` & `txtai-5.5.0/src/python/txtai/api/routers/caption.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/routers/embeddings.py` & `txtai-5.5.0/src/python/txtai/api/routers/embeddings.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/routers/entity.py` & `txtai-5.5.0/src/python/txtai/api/routers/entity.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/routers/extractor.py` & `txtai-5.5.0/src/python/txtai/api/routers/extractor.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/routers/labels.py` & `txtai-5.5.0/src/python/txtai/api/routers/labels.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/routers/objects.py` & `txtai-5.5.0/src/python/txtai/api/routers/objects.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/routers/segmentation.py` & `txtai-5.5.0/src/python/txtai/api/routers/segmentation.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/routers/similarity.py` & `txtai-5.5.0/src/python/txtai/api/routers/similarity.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/routers/summary.py` & `txtai-5.5.0/src/python/txtai/api/routers/summary.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/routers/tabular.py` & `txtai-5.5.0/src/python/txtai/api/routers/tabular.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/routers/textractor.py` & `txtai-5.5.0/src/python/txtai/api/routers/textractor.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/routers/transcription.py` & `txtai-5.5.0/src/python/txtai/api/routers/transcription.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/routers/translation.py` & `txtai-5.5.0/src/python/txtai/api/routers/translation.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/api/routers/workflow.py` & `txtai-5.5.0/src/python/txtai/api/routers/workflow.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/app/base.py` & `txtai-5.5.0/src/python/txtai/app/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,18 @@
             for workflow, config in self.config["workflow"].items():
                 # Create copy of config
                 config = config.copy()
 
                 # Resolve callable functions
                 config["tasks"] = [self.resolve(task) for task in config["tasks"]]
 
+                # Resolve stream functions
+                if "stream" in config:
+                    config["stream"] = self.resolve(config["stream"])
+
                 # Get scheduler config
                 schedule = config.pop("schedule", None)
 
                 # Create workflow
                 self.workflows[workflow] = WorkflowFactory.create(config, workflow)
 
                 # Schedule job if necessary
@@ -636,16 +640,20 @@
             name: workflow name
             elements: elements to process
 
         Returns:
             processed elements
         """
 
-        # Convert lists to tuples
-        elements = [tuple(element) if isinstance(element, list) else element for element in elements]
+        if hasattr(elements, "__len__") and hasattr(elements, "__getitem__"):
+            # Convert to tuples and return as a list since input is sized
+            elements = [tuple(element) if isinstance(element, list) else element for element in elements]
+        else:
+            # Convert to tuples and return as a generator since input is not sized
+            elements = (tuple(element) if isinstance(element, list) else element for element in elements)
 
         # Execute workflow
         return self.workflows[name](elements)
 
     def wait(self):
         """
         Closes threadpool and waits for completion.
```

### Comparing `txtai-5.4.0/src/python/txtai/archive/base.py` & `txtai-5.5.0/src/python/txtai/archive/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/archive/compress.py` & `txtai-5.5.0/src/python/txtai/archive/compress.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/archive/tar.py` & `txtai-5.5.0/src/python/txtai/archive/tar.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/archive/zip.py` & `txtai-5.5.0/src/python/txtai/archive/zip.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/cloud/base.py` & `txtai-5.5.0/src/python/txtai/cloud/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/cloud/factory.py` & `txtai-5.5.0/src/python/txtai/cloud/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/cloud/hub.py` & `txtai-5.5.0/src/python/txtai/cloud/hub.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/cloud/storage.py` & `txtai-5.5.0/src/python/txtai/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/console/base.py` & `txtai-5.5.0/src/python/txtai/console/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/data/base.py` & `txtai-5.5.0/src/python/txtai/data/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/data/labels.py` & `txtai-5.5.0/src/python/txtai/data/labels.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/data/questions.py` & `txtai-5.5.0/src/python/txtai/data/questions.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/data/sequences.py` & `txtai-5.5.0/src/python/txtai/data/sequences.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/data/texts.py` & `txtai-5.5.0/src/python/txtai/data/texts.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/data/tokens.py` & `txtai-5.5.0/src/python/txtai/data/tokens.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/database/base.py` & `txtai-5.5.0/src/python/txtai/database/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 # Logging configuration
 logger = logging.getLogger(__name__)
 
 
 class Database:
     """
-    Base class for database instances. This class encapsulates a document-oriented database
-    used for storing key-value content stored as dicts.
+    Base class for database instances. This class encapsulates a content database used for
+    storing field content as dicts and objects. The database instance works in conjuction
+    with a vector index to execute SQL-driven similarity search.
     """
 
     def __init__(self, config):
         """
         Creates a new Database.
 
         Args:
```

### Comparing `txtai-5.4.0/src/python/txtai/database/encoder/base.py` & `txtai-5.5.0/src/python/txtai/database/encoder/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/database/encoder/factory.py` & `txtai-5.5.0/src/python/txtai/database/encoder/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/database/encoder/image.py` & `txtai-5.5.0/src/python/txtai/database/encoder/image.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/database/factory.py` & `txtai-5.5.0/src/python/txtai/database/factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Factory module
 """
 
 from ..util import Resolver
 
+from .duckdb import DuckDB
 from .sqlite import SQLite
 
 
 class DatabaseFactory:
     """
     Methods to create document databases.
     """
@@ -31,15 +32,17 @@
         content = config.get("content")
 
         # Standardize content name
         if content is True:
             content = "sqlite"
 
         # Create document database instance
-        if content == "sqlite":
+        if content == "duckdb":
+            database = DuckDB(config)
+        elif content == "sqlite":
             database = SQLite(config)
         elif content:
             database = DatabaseFactory.resolve(content, config)
 
         # Store config back
         config["content"] = content
```

### Comparing `txtai-5.4.0/src/python/txtai/database/sql/aggregate.py` & `txtai-5.5.0/src/python/txtai/database/sql/aggregate.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/database/sql/base.py` & `txtai-5.5.0/src/python/txtai/database/sql/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/database/sql/expression.py` & `txtai-5.5.0/src/python/txtai/database/sql/expression.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/database/sql/token.py` & `txtai-5.5.0/src/python/txtai/database/sql/token.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/database/sqlite.py` & `txtai-5.5.0/src/python/txtai/database/filedb.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
-SQLite module
+FileDB module
 """
 
 import datetime
 import json
-import os
-import sqlite3
 
 from .base import Database
 
 
-class SQLite(Database):
+# pylint: disable=R0904
+class FileDB(Database):
     """
-    Document database backed by SQLite.
+    Base file database class.
     """
 
     # Temporary table for working with id batches
     CREATE_BATCH = """
         CREATE TEMP TABLE IF NOT EXISTS batch (
             indexid INTEGER,
             id TEXT,
@@ -45,28 +44,28 @@
             id TEXT PRIMARY KEY,
             data JSON,
             tags TEXT,
             entry DATETIME
         )
     """
 
-    INSERT_DOCUMENT = "REPLACE INTO documents VALUES (?, ?, ?, ?)"
+    INSERT_DOCUMENT = "INSERT OR REPLACE INTO documents VALUES (?, ?, ?, ?)"
     DELETE_DOCUMENTS = "DELETE FROM documents WHERE id IN (SELECT id FROM batch)"
 
     # Objects - stores binary content
     CREATE_OBJECTS = """
         CREATE TABLE IF NOT EXISTS objects (
             id TEXT PRIMARY KEY,
             object BLOB,
             tags TEXT,
             entry DATETIME
         )
     """
 
-    INSERT_OBJECT = "REPLACE INTO objects VALUES (?, ?, ?, ?)"
+    INSERT_OBJECT = "INSERT OR REPLACE INTO objects VALUES (?, ?, ?, ?)"
     DELETE_OBJECTS = "DELETE FROM objects WHERE id IN (SELECT id FROM batch)"
 
     # Sections - stores section text
     CREATE_SECTIONS = """
         CREATE TABLE IF NOT EXISTS %s (
             indexid INTEGER PRIMARY KEY,
             id TEXT,
@@ -105,23 +104,23 @@
 
         Args:
             config: database configuration parameters
         """
 
         super().__init__(config)
 
-        # SQLite connection handle
+        # Database connection handle
         self.connection = None
         self.cursor = None
         self.path = None
 
     def load(self, path):
         # Load an existing database. Thread locking must be handled externally.
-        self.connection = sqlite3.connect(path, check_same_thread=False)
-        self.cursor = self.connection.cursor()
+        self.connection = self.connect(path)
+        self.cursor = self.getcursor()
         self.path = path
 
         # Register custom functions
         self.addfunctions()
 
     def insert(self, documents, index=0):
         # Initialize connection if not open
@@ -153,46 +152,46 @@
 
     def delete(self, ids):
         if self.connection:
             # Batch ids
             self.batch(ids=ids)
 
             # Delete all documents, objects and sections by id
-            self.cursor.execute(SQLite.DELETE_DOCUMENTS)
-            self.cursor.execute(SQLite.DELETE_OBJECTS)
-            self.cursor.execute(SQLite.DELETE_SECTIONS)
+            self.cursor.execute(FileDB.DELETE_DOCUMENTS)
+            self.cursor.execute(FileDB.DELETE_OBJECTS)
+            self.cursor.execute(FileDB.DELETE_SECTIONS)
 
     def reindex(self, columns=None):
         if self.connection:
             # Working table name
             name = "rebuild"
 
             # Resolve and build column strings if provided
             select = "text"
             if columns:
                 select = "|| ' ' ||".join([self.resolve(c) for c in columns])
 
             # Create new table to hold reordered sections
-            self.cursor.execute(SQLite.CREATE_SECTIONS % name)
+            self.cursor.execute(FileDB.CREATE_SECTIONS % name)
 
             # Copy data over
-            self.cursor.execute(SQLite.COPY_SECTIONS % (name, select))
+            self.cursor.execute(FileDB.COPY_SECTIONS % (name, select))
 
             # Stream new results
-            self.cursor.execute(SQLite.STREAM_SECTIONS % name)
-            for uid, text, obj, tags in self.cursor:
+            self.cursor.execute(FileDB.STREAM_SECTIONS % name)
+            for uid, text, obj, tags in self.rows():
                 if not text and self.encoder and obj:
                     yield (uid, self.encoder.decode(obj), tags)
                 else:
                     yield (uid, text, tags)
 
             # Swap as new table
-            self.cursor.execute(SQLite.DROP_SECTIONS)
-            self.cursor.execute(SQLite.RENAME_SECTIONS % name)
-            self.cursor.execute(SQLite.CREATE_SECTIONS_INDEX)
+            self.cursor.execute(FileDB.DROP_SECTIONS)
+            self.cursor.execute(FileDB.RENAME_SECTIONS % name)
+            self.cursor.execute(FileDB.CREATE_SECTIONS_INDEX)
 
     def save(self, path):
         # Temporary database
         if not self.path:
             # Save temporary database
             self.connection.commit()
 
@@ -200,15 +199,15 @@
             connection = self.copy(path)
 
             # Close temporary database
             self.connection.close()
 
             # Point connection to new connection
             self.connection = connection
-            self.cursor = self.connection.cursor()
+            self.cursor = self.getcursor()
             self.path = path
 
             # Register custom functions
             self.addfunctions()
 
         # Paths are equal, commit changes
         elif self.path == path:
@@ -222,15 +221,15 @@
         # Close connection
         if self.connection:
             self.connection.close()
 
     def ids(self, ids):
         # Batch ids and run query
         self.batch(ids=ids)
-        self.cursor.execute(SQLite.SELECT_IDS)
+        self.cursor.execute(FileDB.SELECT_IDS)
 
         # Format and return results
         return self.cursor.fetchall()
 
     def resolve(self, name, alias=None):
         # Standard column names
         sections = ["indexid", "id", "tags", "entry"]
@@ -258,38 +257,38 @@
             return f"s.{name}"
 
         # Standard columns - no prefixes
         if name.lower() in noprefix:
             return name
 
         # Other columns come from documents.data JSON
-        return f'json_extract(data, "$.{name}")'
+        return f"json_extract(data, '$.{name}')"
 
     def embed(self, similarity, batch):
         # Load similarity results id batch
         self.batch(indexids=[i for i, _ in similarity[batch]], batch=batch)
 
         # Average and load all similarity scores with first batch
         if not batch:
             self.scores(similarity)
 
         # Return ids clause placeholder
-        return SQLite.IDS_CLAUSE % batch
+        return FileDB.IDS_CLAUSE % batch
 
     # pylint: disable=R0912
     def query(self, query, limit):
         # Extract query components
         select = query.get("select", self.defaults())
         where = query.get("where")
         groupby, having = query.get("groupby"), query.get("having")
         orderby, qlimit, offset = query.get("orderby"), query.get("limit"), query.get("offset")
         similarity = query.get("similar")
 
         # Build query text
-        query = SQLite.TABLE_CLAUSE % select
+        query = FileDB.TABLE_CLAUSE % select
         if where is not None:
             query += f" WHERE {where}"
         if groupby is not None:
             query += f" GROUP BY {groupby}"
         if having is not None:
             query += f" HAVING {having}"
         if orderby is not None:
@@ -315,15 +314,15 @@
         self.execute(self.cursor.execute, query)
 
         # Retrieve column list from query
         columns = [c[0] for c in self.cursor.description]
 
         # Map results and return
         results = []
-        for row in self.cursor:
+        for row in self.rows():
             result = {}
 
             # Copy columns to result. In cases with duplicate column names, find one with a value
             for x, column in enumerate(columns):
                 if column not in result or result[column] is None:
                     # Decode object
                     if self.encoder and column == "object":
@@ -331,46 +330,32 @@
                     else:
                         result[column] = row[x]
 
             results.append(result)
 
         return results
 
-    def addfunctions(self):
-        """
-        Adds custom functions in current connection.
-        """
-
-        if self.connection and self.functions:
-            # Enable callback tracebacks to show user-defined function errors
-            sqlite3.enable_callback_tracebacks(True)
-
-            for name, argcount, fn in self.functions:
-                self.connection.create_function(name, argcount, fn)
-
     def initialize(self):
         """
         Creates connection and initial database schema if no connection exists.
         """
 
         if not self.connection:
-            name = "sections"
-
             # Create temporary database. Thread locking must be handled externally.
-            self.connection = sqlite3.connect("", check_same_thread=False)
-            self.cursor = self.connection.cursor()
+            self.connection = self.connect()
+            self.cursor = self.getcursor()
 
             # Register custom functions
             self.addfunctions()
 
             # Create initial schema and indices
-            self.cursor.execute(SQLite.CREATE_DOCUMENTS)
-            self.cursor.execute(SQLite.CREATE_OBJECTS)
-            self.cursor.execute(SQLite.CREATE_SECTIONS % name)
-            self.cursor.execute(SQLite.CREATE_SECTIONS_INDEX)
+            self.cursor.execute(FileDB.CREATE_DOCUMENTS)
+            self.cursor.execute(FileDB.CREATE_OBJECTS)
+            self.cursor.execute(FileDB.CREATE_SECTIONS % "sections")
+            self.cursor.execute(FileDB.CREATE_SECTIONS_INDEX)
 
     def insertdocument(self, uid, document, tags, entry):
         """
         Inserts a document.
 
         Args:
             uid: unique id
@@ -386,15 +371,15 @@
         document = document.copy()
 
         # Get and remove object field from document
         obj = document.pop("object") if "object" in document else None
 
         # Insert document as JSON
         if document:
-            self.cursor.execute(SQLite.INSERT_DOCUMENT, [uid, json.dumps(document, allow_nan=False), tags, entry])
+            self.cursor.execute(FileDB.INSERT_DOCUMENT, [uid, json.dumps(document, allow_nan=False), tags, entry])
 
         # Get value of text field
         text = document.get("text")
 
         # If both text and object are set, insert object as it won't otherwise be used
         if text and obj:
             self.insertobject(uid, obj, tags, entry)
@@ -411,60 +396,30 @@
             obj: input object
             tags: object tags
             entry: generated entry date
         """
 
         # If object support is enabled, save object
         if self.encoder:
-            self.cursor.execute(SQLite.INSERT_OBJECT, [uid, self.encoder.encode(obj), tags, entry])
+            self.cursor.execute(FileDB.INSERT_OBJECT, [uid, self.encoder.encode(obj), tags, entry])
 
     def insertsection(self, index, uid, text, tags, entry):
         """
         Inserts a section.
 
         Args:
             index: index id
             uid: unique id
             text: section text
             tags: section tags
             entry: generated entry date
         """
 
         # Save text section
-        self.cursor.execute(SQLite.INSERT_SECTION, [index, uid, text, tags, entry])
-
-    def copy(self, path):
-        """
-        Copies the current database into path. This method will use the backup API if the current connection has no uncommitted changes.
-        Otherwise, iterdump is used, as the backup call will hang for an uncommitted connection.
-
-        Args:
-            path: path to write database
-
-        Returns:
-            new connection with data copied over
-        """
-
-        # Delete existing file, if necessary
-        if os.path.exists(path):
-            os.remove(path)
-
-        # Create database. Thread locking must be handled externally.
-        connection = sqlite3.connect(path, check_same_thread=False)
-
-        if self.connection.in_transaction:
-            # The backup call will hang if there are uncommitted changes, need to copy over
-            # with iterdump (which is much slower)
-            for sql in self.connection.iterdump():
-                connection.execute(sql)
-        else:
-            # Database is up to date, can do a more efficient copy with SQLite C API
-            self.connection.backup(connection)
-
-        return connection
+        self.cursor.execute(FileDB.INSERT_SECTION, [index, uid, text, tags, entry])
 
     def defaults(self):
         """
         Returns a list of default columns when there is no select clause.
 
         Returns:
             list of default columns
@@ -479,43 +434,99 @@
         Args:
             indexids: list of indexids
             ids: list of ids
             batch: batch index, used when statement has multiple subselects
         """
 
         # Create or Replace temporary batch table
-        self.cursor.execute(SQLite.CREATE_BATCH)
+        self.cursor.execute(FileDB.CREATE_BATCH)
 
         # Delete batch when batch id is empty or for batch 0
         if not batch:
-            self.cursor.execute(SQLite.DELETE_BATCH)
+            self.cursor.execute(FileDB.DELETE_BATCH)
 
         if indexids:
-            self.cursor.executemany(SQLite.INSERT_BATCH_INDEXID, [(i, batch) for i in indexids])
+            self.cursor.executemany(FileDB.INSERT_BATCH_INDEXID, [(i, batch) for i in indexids])
         if ids:
-            self.cursor.executemany(SQLite.INSERT_BATCH_ID, [(str(uid), batch) for uid in ids])
+            self.cursor.executemany(FileDB.INSERT_BATCH_ID, [(str(uid), batch) for uid in ids])
 
     def scores(self, similarity):
         """
         Loads a batch of similarity scores to a temporary table for efficient query processing.
 
         Args:
             similarity: similarity results as [(indexid, score)]
         """
 
         # Create or Replace temporary scores table
-        self.cursor.execute(SQLite.CREATE_SCORES)
+        self.cursor.execute(FileDB.CREATE_SCORES)
 
         # Delete scores
-        self.cursor.execute(SQLite.DELETE_SCORES)
+        self.cursor.execute(FileDB.DELETE_SCORES)
 
         if similarity:
             # Average scores per id, needed for multiple similar() clauses
             scores = {}
             for s in similarity:
                 for i, score in s:
                     if i not in scores:
                         scores[i] = []
                     scores[i].append(score)
 
             # Average scores by id
-            self.cursor.executemany(SQLite.INSERT_SCORE, [(i, sum(s) / len(s)) for i, s in scores.items()])
+            self.cursor.executemany(FileDB.INSERT_SCORE, [(i, sum(s) / len(s)) for i, s in scores.items()])
+
+    def connect(self, path=None):
+        """
+        Creates a new database connection.
+
+        Args:
+            path: path to database file
+
+        Returns:
+            connection
+        """
+
+        raise NotImplementedError
+
+    def getcursor(self):
+        """
+        Opens a cursor for current connection.
+
+        Returns:
+            cursor
+        """
+
+        raise NotImplementedError
+
+    def rows(self):
+        """
+        Returns current cursor row iterator for last executed query.
+
+        Args:
+            cursor: cursor
+
+        Returns:
+            iterable collection of rows
+        """
+
+        raise NotImplementedError
+
+    def addfunctions(self):
+        """
+        Adds custom functions in current connection.
+        """
+
+        raise NotImplementedError
+
+    def copy(self, path):
+        """
+        Copies the current database into path.
+
+        Args:
+            path: path to write database
+
+        Returns:
+            new connection with data copied over
+        """
+
+        raise NotImplementedError
```

### Comparing `txtai-5.4.0/src/python/txtai/embeddings/base.py` & `txtai-5.5.0/src/python/txtai/embeddings/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 
         # Approximate nearest neighbor index
         self.ann = None
 
         # Document database
         self.database = None
 
+        # Resolvable functions
+        self.functions = None
+
         # Graph network
         self.graph = None
 
         # Query model
         self.query = None
 
         # Index archive
@@ -147,16 +150,16 @@
         appended to the index, existing data is updated. If the index doesn't exist,
         this method runs a standard index operation.
 
         Args:
             documents: list of (id, data, tags)
         """
 
-        # Run standard insert if index doesn't exist
-        if not self.ann:
+        # Run standard insert if index doesn't exist or it has no records
+        if not self.count():
             self.index(documents)
             return
 
         # Create transform action
         transform = Transform(self, Action.UPSERT)
 
         with tempfile.NamedTemporaryFile(mode="wb", suffix=".npy") as buffer:
@@ -175,15 +178,15 @@
 
                 # Save indexids-ids mapping for indexes with no database
                 if not self.database:
                     self.config["ids"] = self.config["ids"] + ids
 
         # Graph upsert, if necessary
         if self.graph:
-            self.graph.upsert(Search(self, True))
+            self.graph.upsert(Search(self, True), self.batchsimilarity)
 
     def delete(self, ids):
         """
         Deletes from an embeddings index. Returns list of ids deleted.
 
         Args:
             ids: list of ids to delete
@@ -248,14 +251,18 @@
             config["content"] = self.config["content"]
             if "objects" in self.config:
                 config["objects"] = self.config["objects"]
 
             # Reset configuration
             self.configure(config)
 
+            # Reset function references
+            if self.functions:
+                self.functions.reset()
+
             # Reindex
             if function:
                 self.index(function(self.database.reindex(columns)), True)
             else:
                 self.index(self.database.reindex(columns), True)
 
     def transform(self, document):
@@ -575,15 +582,15 @@
 
         self.config, self.reducer, self.scoring, self.model = None, None, None, None
         self.ann, self.graph, self.query, self.archive = None, None, None, None
 
         # Close database connection if open
         if self.database:
             self.database.close()
-            self.database = None
+            self.database, self.functions = None, None
 
     def info(self):
         """
         Prints the current embeddings index configuration.
         """
 
         # Copy and edit config
@@ -757,17 +764,18 @@
 
         # Free existing database resources
         if self.database:
             self.database.close()
 
         config = self.config.copy()
 
-        # Resolve callable functions
-        if "functions" in config:
-            config["functions"] = Functions(self)(config)
+        # Create references to callable functions
+        self.functions = Functions(self) if "functions" in config else None
+        if self.functions:
+            config["functions"] = self.functions(config)
 
         # Create database from config and return
         return DatabaseFactory.create(config)
 
     def creategraph(self):
         """
         Creates a graph from config.
```

### Comparing `txtai-5.4.0/src/python/txtai/embeddings/documents.py` & `txtai-5.5.0/src/python/txtai/embeddings/documents.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/embeddings/explain.py` & `txtai-5.5.0/src/python/txtai/embeddings/explain.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/embeddings/functions.py` & `txtai-5.5.0/src/python/txtai/embeddings/functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,37 +16,52 @@
 
         Args:
             embeddings: embeddings instance
         """
 
         self.embeddings = embeddings
 
+        # Handle to all reference objects
+        self.references = None
+
     def __call__(self, config):
         """
         Resolves a list of functions to function references.
 
         Args:
             config: configuration
 
         Returns:
             list of function references
         """
 
+        # Initialize stored references array
+        self.references = []
+
         # Resolve callable functions
         functions = []
         for fn in config["functions"]:
             if isinstance(fn, dict):
                 fn = fn.copy()
                 fn["function"] = self.function(fn["function"])
             else:
                 fn = self.function(fn)
             functions.append(fn)
 
         return functions
 
+    def reset(self):
+        """
+        Clears all resolved references.
+        """
+
+        if self.references:
+            for reference in self.references:
+                reference.reset()
+
     def function(self, function):
         """
         Resolves function configuration. If function is a string, it's split on '.' and each part
         is separately resolved to an object, attribute or function. Each part is resolved upon the
         first invocation of the function. Otherwise, the input is returned.
 
         Args:
@@ -57,20 +72,22 @@
         """
 
         if isinstance(function, str):
             parts = function.split(".")
 
             if hasattr(self.embeddings, parts[0]):
                 m = Reference(self.embeddings, parts[0])
+                self.references.append(m)
             else:
                 module = ".".join(parts[:-1])
                 m = __import__(module)
 
             for comp in parts[1:]:
                 m = Reference(m, comp)
+                self.references.append(m)
 
             return m
 
         return function
 
 
 class Reference:
@@ -88,14 +105,17 @@
             attribute: attribute name
         """
 
         # Object handle and attribute
         self.obj = obj
         self.attribute = attribute
 
+        # Keep a handle to the original inputs
+        self.inputs = (obj, attribute)
+
         # True if the object and attribute have been resolved
         self.resolved = False
 
         # True if the attribute is a function
         self.function = None
 
     def __call__(self, *args):
@@ -121,7 +141,15 @@
 
         # Determine if attribute is a function
         if self.function is None:
             self.function = isinstance(attribute, (FunctionType, MethodType)) or (hasattr(attribute, "__call__") and args)
 
         # If attribute is a function, execute and return, otherwise return attribute
         return attribute(*args) if self.function else attribute
+
+    def reset(self):
+        """
+        Clears resolved references.
+        """
+
+        self.obj, self.attribute = self.inputs
+        self.resolved = False
```

### Comparing `txtai-5.4.0/src/python/txtai/embeddings/query.py` & `txtai-5.5.0/src/python/txtai/embeddings/query.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/embeddings/reducer.py` & `txtai-5.5.0/src/python/txtai/embeddings/reducer.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/embeddings/search.py` & `txtai-5.5.0/src/python/txtai/embeddings/search.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/embeddings/terms.py` & `txtai-5.5.0/src/python/txtai/embeddings/terms.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/embeddings/transform.py` & `txtai-5.5.0/src/python/txtai/embeddings/transform.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/graph/base.py` & `txtai-5.5.0/src/python/txtai/graph/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 from .topics import Topics
 
 
 # pylint: disable=R0904
 class Graph:
     """
-    Base class for Graph instances.
+    Base class for Graph instances. This class builds graph networks. Supports topic modeling
+    and relationship traversal.
     """
 
     def __init__(self, config):
         """
         Creates a new Graph.
 
         Args:
@@ -373,16 +374,21 @@
 
         for uid in ids:
             # Remove existing node, if it exists
             if self.hasnode(uid):
                 # Delete from topics
                 topic = self.attribute(uid, "topic")
                 if topic and self.topics:
+                    # Delete id from topic
                     self.topics[topic].remove(uid)
 
+                    # Also delete topic, if it's empty
+                    if not self.topics[topic]:
+                        self.topics.pop(topic)
+
                 # Delete node
                 self.removenode(uid)
 
     def index(self, search, similarity):
         """
         Build relationships between graph nodes using a score-based search function.
 
@@ -394,31 +400,36 @@
         # Add node edges
         self.addedges(self.scan(), search)
 
         # Label categories/topics
         if "topics" in self.config:
             self.addtopics(similarity)
 
-    def upsert(self, search):
+    def upsert(self, search, similarity=None):
         """
         Adds relationships for new graph nodes using a score-based search function.
 
         Args:
             search: batch search function - takes a list of queries and returns lists of (id, scores) to use as edge weights
+            similarity: batch similarity function - takes a list of text and labels and returns best matches
         """
 
         # Detect if topics processing is enabled
         hastopics = "topics" in self.config
 
         # Add node edges using new/updated nodes, set updated flag for topic processing, if necessary
         self.addedges(self.scan(attribute="data"), search, {"updated": True} if hastopics else None)
 
         # Infer topics with topics of connected nodes
         if hastopics:
-            self.infertopics()
+            # Infer topics if there is at least one topic, otherwise rebuild
+            if self.topics:
+                self.infertopics()
+            else:
+                self.addtopics(similarity)
 
     def addedges(self, nodes, search, attributes=None):
         """
         Adds edges for a list of nodes using a score-based search function.
 
         Args:
             nodes: list of nodes
```

### Comparing `txtai-5.4.0/src/python/txtai/graph/factory.py` & `txtai-5.5.0/src/python/txtai/graph/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/graph/networkx.py` & `txtai-5.5.0/src/python/txtai/graph/networkx.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/graph/topics.py` & `txtai-5.5.0/src/python/txtai/graph/topics.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/models/models.py` & `txtai-5.5.0/src/python/txtai/models/models.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/models/onnx.py` & `txtai-5.5.0/src/python/txtai/models/onnx.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/models/pooling.py` & `txtai-5.5.0/src/python/txtai/models/pooling.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/models/registry.py` & `txtai-5.5.0/src/python/txtai/models/registry.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/models/tokendetection.py` & `txtai-5.5.0/src/python/txtai/models/tokendetection.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,25 +94,26 @@
         inputs = {"attention_mask": attention_mask} if self.dattention else {}
         doutputs = self.discriminator(dinputs, labels=dlabels, token_type_ids=token_type_ids, **inputs)
 
         # Compute combined loss
         loss = goutputs[0] + self.weight * doutputs[0]
         return loss, goutputs[1], doutputs[1], dlabels
 
-    def save_pretrained(self, output, state_dict=None):
+    def save_pretrained(self, output, state_dict=None, **kwargs):
         """
         Saves current model to output directory.
 
         Args:
             output: output directory
             state_dict: model state
+            kwargs: additional keyword arguments
         """
 
         # Save combined model to support training from checkpoints
-        super().save_pretrained(output, state_dict)
+        super().save_pretrained(output, state_dict, **kwargs)
 
         # Save generator tokenizer and model
         gpath = os.path.join(output, "generator")
         self.tokenizer.save_pretrained(gpath)
         self.generator.save_pretrained(gpath)
 
         # Save discriminator tokenizer and model
```

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/audio/texttospeech.py` & `txtai-5.5.0/src/python/txtai/pipeline/audio/texttospeech.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,29 @@
 
 
 class TextToSpeech(Pipeline):
     """
     Generates speech from text
     """
 
-    def __init__(self, path="neuml/ljspeech-jets-onnx", maxtokens=512):
+    def __init__(self, path=None, maxtokens=512):
         """
         Creates a new TextToSpeech pipeline.
 
         Args:
             path: optional Hugging Face model hub id
             maxtokens: maximum number of tokens model can process, defaults to 512
         """
 
         if not TTS:
             raise ImportError('TextToSpeech pipeline is not available - install "pipeline" extra to enable')
 
+        # Default path
+        path = path if path else "neuml/ljspeech-jets-onnx"
+
         # Get path to model and config
         config = hf_hub_download(path, filename="config.yaml")
         model = hf_hub_download(path, filename="model.onnx")
 
         # Read yaml config
         with open(config, "r", encoding="utf-8") as f:
             config = yaml.safe_load(f)
```

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/audio/transcription.py` & `txtai-5.5.0/src/python/txtai/pipeline/audio/transcription.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/base.py` & `txtai-5.5.0/src/python/txtai/pipeline/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/data/segmentation.py` & `txtai-5.5.0/src/python/txtai/pipeline/data/segmentation.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/data/tabular.py` & `txtai-5.5.0/src/python/txtai/pipeline/data/tabular.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/data/textractor.py` & `txtai-5.5.0/src/python/txtai/pipeline/data/textractor.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/data/tokenizer.py` & `txtai-5.5.0/src/python/txtai/pipeline/data/tokenizer.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/factory.py` & `txtai-5.5.0/src/python/txtai/pipeline/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/hfmodel.py` & `txtai-5.5.0/src/python/txtai/pipeline/hfmodel.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/hfpipeline.py` & `txtai-5.5.0/src/python/txtai/pipeline/hfpipeline.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/image/caption.py` & `txtai-5.5.0/src/python/txtai/pipeline/image/caption.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/image/imagehash.py` & `txtai-5.5.0/src/python/txtai/pipeline/image/imagehash.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/image/objects.py` & `txtai-5.5.0/src/python/txtai/pipeline/image/objects.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/tensors.py` & `txtai-5.5.0/src/python/txtai/pipeline/tensors.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/text/crossencoder.py` & `txtai-5.5.0/src/python/txtai/pipeline/text/crossencoder.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/text/entity.py` & `txtai-5.5.0/src/python/txtai/pipeline/text/entity.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/text/extractor.py` & `txtai-5.5.0/src/python/txtai/pipeline/text/extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             list of answers matching input format (tuple or dict) containing fields as specified by output format
         """
 
         # Save original queue format
         inputs = queue
 
         # Convert dictionary inputs to tuples
-        if isinstance(queue[0], dict):
+        if queue and isinstance(queue[0], dict):
             # Convert dict to tuple
             queue = [tuple(row.get(x) for x in ["name", "query", "question", "snippet"]) for row in queue]
 
         # Rank texts by similarity for each query
         results = self.query([query for _, query, _, _ in queue], texts)
 
         # Build question-context pairs
@@ -362,15 +362,15 @@
             return [answer for _, answer in answers]
 
         # Resolve id reference for each answer
         if self.output == "reference":
             answers = self.reference(queries, answers, topns)
 
         # Ensure output format matches input format
-        if isinstance(inputs[0], dict):
+        if inputs and isinstance(inputs[0], dict):
             # Add name if input queue had name field
             fields = ["name", "answer", "reference"] if "name" in inputs[0] else [None, "answer", "reference"]
             answers = [{fields[x]: column for x, column in enumerate(row) if fields[x]} for row in answers]
 
         return answers
 
     def reference(self, queries, answers, topns):
```

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/text/generator.py` & `txtai-5.5.0/src/python/txtai/pipeline/text/generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,61 +9,67 @@
     """
     Generate text with a causal language model.
     """
 
     def __init__(self, path=None, quantize=False, gpu=True, model=None):
         super().__init__(self.task(), path, quantize, gpu, model)
 
-    def __call__(self, text, prefix=None, maxlength=512, workers=0):
+    def __call__(self, text, prefix=None, maxlength=512, workers=0, **kwargs):
         """
         Generates text using input text
 
         Args:
             text: text|list
             prefix: optional prefix to prepend to text elements
             maxlength: maximum sequence length
             workers: number of concurrent workers to use for processing data, defaults to None
+            kwargs: additional generation keyword arguments
 
         Returns:
             generated text
         """
 
         # List of texts
         texts = text if isinstance(text, list) else [text]
 
         # Add prefix, if necessary
         if prefix:
             texts = [f"{prefix}{x}" for x in texts]
 
         # Run pipeline
-        results = self.pipeline(texts, max_length=maxlength, num_workers=workers)
+        results = self.pipeline(texts, max_length=maxlength, num_workers=workers, **kwargs)
 
         # Get generated text
-        results = [self.clean(x) for x in results]
+        results = [self.clean(texts[x], result) for x, result in enumerate(results)]
 
         return results[0] if isinstance(text, str) else results
 
-    def clean(self, result):
+    def clean(self, prompt, result):
         """
         Applies a series of rules to clean generated text.
 
         Args:
+            prompt: original input prompt
             result: input result
 
         Returns:
             clean text
         """
 
         # Extract output from list, if necessary
         result = result[0] if isinstance(result, list) else result
 
         # Get generated text field
         text = result["generated_text"]
 
-        return text.replace("$=", "<=")
+        # Replace input prompt
+        text = text.replace(prompt, "")
+
+        # Apply text cleaning rules
+        return text.replace("$=", "<=").strip()
 
     def task(self):
         """
         Get the pipeline task name.
 
         Returns:
             pipeline task name
```

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/text/labels.py` & `txtai-5.5.0/src/python/txtai/pipeline/text/labels.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/text/questions.py` & `txtai-5.5.0/src/python/txtai/pipeline/text/questions.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/text/similarity.py` & `txtai-5.5.0/src/python/txtai/pipeline/text/similarity.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/text/summary.py` & `txtai-5.5.0/src/python/txtai/pipeline/text/summary.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/text/translation.py` & `txtai-5.5.0/src/python/txtai/pipeline/text/translation.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,30 +22,31 @@
     """
     Translates text from source language into target language.
     """
 
     # Default language detection model
     DEFAULT_LANG_DETECT = "https://dl.fbaipublicfiles.com/fasttext/supervised-models/lid.176.ftz"
 
-    def __init__(self, path="facebook/m2m100_418M", quantize=False, gpu=True, batch=64, langdetect=DEFAULT_LANG_DETECT, findmodels=True):
+    def __init__(self, path=None, quantize=False, gpu=True, batch=64, langdetect=None, findmodels=True):
         """
         Constructs a new language translation pipeline.
 
         Args:
             path: optional path to model, accepts Hugging Face model hub id or local path,
                   uses default model for task if not provided
             quantize: if model should be quantized, defaults to False
             gpu: True/False if GPU should be enabled, also supports a GPU device id
             batch: batch size used to incrementally process content
-            langdetect: path to language detection model, uses a default path if not provided
+            langdetect: set a custom language detection function, method must take a list of strings and return
+                        language codes for each, uses default language detector if not provided
             findmodels: True/False if the Hugging Face Hub will be searched for source-target translation models
         """
 
         # Call parent constructor
-        super().__init__(path, quantize, gpu, batch)
+        super().__init__(path if path else "facebook/m2m100_418M", quantize, gpu, batch)
 
         # Language detection
         self.detector = None
         self.langdetect = langdetect
         self.findmodels = findmodels
 
         # Language models
@@ -121,23 +122,44 @@
         Args:
             texts: list of text
 
         Returns:
             list of languages
         """
 
-        if not FASTTEXT:
-            raise ImportError('Language detection is not available - install "pipeline" extra to enable')
+        # Default detector
+        if not self.langdetect or isinstance(self.langdetect, str):
+            return self.defaultdetect(texts)
+
+        # Call external language detector
+        return self.langdetect(texts)
+
+    def defaultdetect(self, texts):
+        """
+        Default fasttext language detection model.
+
+        Args:
+            texts: list of text
+
+        Returns:
+            list of languages
+        """
 
         if not self.detector:
+            if not FASTTEXT:
+                raise ImportError('Language detection is not available - install "pipeline" extra to enable')
+
             # Suppress unnecessary warning
             fasttext.FastText.eprint = lambda x: None
 
+            # Get model path
+            path = self.langdetect if self.langdetect else Translation.DEFAULT_LANG_DETECT
+
             # Load language detection model
-            path = cached_download(self.langdetect, legacy_cache_layout=True)
+            path = cached_download(path, legacy_cache_layout=True)
             self.detector = fasttext.load_model(path)
 
         # Transform texts to format expected by language detection model
         texts = [x.lower().replace("\n", " ").replace("\r\n", " ") for x in texts]
 
         return [x[0].split("__")[-1] for x in self.detector.predict(texts)[0]]
```

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/train/hfonnx.py` & `txtai-5.5.0/src/python/txtai/pipeline/train/hfonnx.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/train/hftrainer.py` & `txtai-5.5.0/src/python/txtai/pipeline/train/hftrainer.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/pipeline/train/mlonnx.py` & `txtai-5.5.0/src/python/txtai/pipeline/train/mlonnx.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,12 +47,16 @@
 
         # Prune model graph down to only output probabilities
         model = select_model_inputs_outputs(model, outputs="probabilities")
 
         # pylint: disable=E1101
         # Rename output to logits for consistency with other models
         model.graph.output[0].name = "logits"
-        model.graph.node[0].output[0] = "logits"
+
+        # Find probabilities output node and rename to logits
+        for node in model.graph.node:
+            if node.output[0] == "probabilities":
+                node.output[0] = "logits"
 
         # Save model to specified output path or return bytes
         model = save_onnx_model(model, output)
         return output if output else model
```

### Comparing `txtai-5.4.0/src/python/txtai/scoring/base.py` & `txtai-5.5.0/src/python/txtai/scoring/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/scoring/bm25.py` & `txtai-5.5.0/src/python/txtai/scoring/bm25.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/scoring/factory.py` & `txtai-5.5.0/src/python/txtai/scoring/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/scoring/sif.py` & `txtai-5.5.0/src/python/txtai/scoring/sif.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/util/resolver.py` & `txtai-5.5.0/src/python/txtai/util/resolver.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/vectors/base.py` & `txtai-5.5.0/src/python/txtai/vectors/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 
 from .. import __pickle__
 
 
 class Vectors:
     """
-    Base class for sentence embeddings/vector models.
+    Base class for sentence embeddings/vector models. Vector models transform input content into numeric vectors.
     """
 
     def __init__(self, config, scoring):
         # Store parameters
         self.config = config
         self.scoring = scoring
```

### Comparing `txtai-5.4.0/src/python/txtai/vectors/external.py` & `txtai-5.5.0/src/python/txtai/vectors/external.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/vectors/factory.py` & `txtai-5.5.0/src/python/txtai/vectors/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/vectors/transformers.py` & `txtai-5.5.0/src/python/txtai/vectors/transformers.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/vectors/words.py` & `txtai-5.5.0/src/python/txtai/vectors/words.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/workflow/base.py` & `txtai-5.5.0/src/python/txtai/workflow/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,29 +23,31 @@
 
 
 class Workflow:
     """
     Base class for all workflows.
     """
 
-    def __init__(self, tasks, batch=100, workers=None, name=None):
+    def __init__(self, tasks, batch=100, workers=None, name=None, stream=None):
         """
         Creates a new workflow. Workflows are lists of tasks to execute.
 
         Args:
             tasks: list of workflow tasks
             batch: how many items to process at a time, defaults to 100
             workers: number of concurrent workers
             name: workflow name
+            stream: workflow stream processor
         """
 
         self.tasks = tasks
         self.batch = batch
         self.workers = workers
         self.name = name
+        self.stream = stream
 
         # Set default number of executor workers to max number of actions in a task
         self.workers = max(len(task.action) for task in self.tasks) if not self.workers else self.workers
 
     def __call__(self, elements):
         """
         Executes a workflow for input elements. This method returns a generator that yields transformed
@@ -59,14 +61,17 @@
         """
 
         # Create execute instance for this run
         with Execute(self.workers) as executor:
             # Run task initializers
             self.initialize()
 
+            # Process elements with stream processor, if available
+            elements = self.stream(elements) if self.stream else elements
+
             # Process elements in batches
             for batch in self.chunk(elements):
                 yield from self.process(batch, executor)
 
             # Run task finalizers
             self.finalize()
```

### Comparing `txtai-5.4.0/src/python/txtai/workflow/execute.py` & `txtai-5.5.0/src/python/txtai/workflow/execute.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/workflow/factory.py` & `txtai-5.5.0/src/python/txtai/workflow/factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,9 +28,15 @@
         tasks = []
         for tconfig in config["tasks"]:
             task = tconfig.pop("task") if "task" in tconfig else ""
             tasks.append(TaskFactory.create(tconfig, task))
 
         config["tasks"] = tasks
 
+        if "stream" in config:
+            sconfig = config["stream"]
+            task = sconfig.pop("task") if "task" in sconfig else "stream"
+
+            config["stream"] = TaskFactory.create(sconfig, task)
+
         # Create workflow
         return Workflow(**config, name=name)
```

### Comparing `txtai-5.4.0/src/python/txtai/workflow/task/base.py` & `txtai-5.5.0/src/python/txtai/workflow/task/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/workflow/task/export.py` & `txtai-5.5.0/src/python/txtai/workflow/task/export.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/workflow/task/factory.py` & `txtai-5.5.0/src/python/txtai/workflow/task/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/workflow/task/file.py` & `txtai-5.5.0/src/python/txtai/workflow/task/file.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/workflow/task/image.py` & `txtai-5.5.0/src/python/txtai/workflow/task/image.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/workflow/task/retrieve.py` & `txtai-5.5.0/src/python/txtai/workflow/task/retrieve.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/workflow/task/service.py` & `txtai-5.5.0/src/python/txtai/workflow/task/service.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/workflow/task/storage.py` & `txtai-5.5.0/src/python/txtai/workflow/task/storage.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai/workflow/task/template.py` & `txtai-5.5.0/src/python/txtai/workflow/task/template.py`

 * *Files identical despite different names*

### Comparing `txtai-5.4.0/src/python/txtai.egg-info/PKG-INFO` & `txtai-5.5.0/src/python/txtai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: txtai
-Version: 5.4.0
-Summary: Build AI-powered semantic search applications
+Version: 5.5.0
+Summary: Semantic search and workflows powered by language models
 Home-page: https://github.com/neuml/txtai
 Author: NeuML
 License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/neuml/txtai
 Project-URL: Issue Tracker, https://github.com/neuml/txtai/issues
 Project-URL: Source Code, https://github.com/neuml/txtai
 Description: <p align="center">
             <img src="https://raw.githubusercontent.com/neuml/txtai/master/logo.png"/>
         </p>
         
         <h3 align="center">
-            <p>Build AI-powered semantic search applications</p>
+            <p>Semantic search and workflows powered by language models</p>
         </h3>
         
         <p align="center">
             <a href="https://github.com/neuml/txtai/releases">
                 <img src="https://img.shields.io/github/release/neuml/txtai.svg?style=flat&color=success" alt="Version"/>
             </a>
             <a href="https://github.com/neuml/txtai">
@@ -35,80 +35,81 @@
             <a href="https://coveralls.io/github/neuml/txtai?branch=master">
                 <img src="https://img.shields.io/coverallsCoverage/github/neuml/txtai" alt="Coverage Status">
             </a>
         </p>
         
         -------------------------------------------------------------------------------------------------------------------------------------------------------
         
-        txtai executes machine-learning workflows to transform data and build AI-powered semantic search applications.
+        txtai is an open-source platform for semantic search and workflows powered by language models.
         
         ![demo](https://raw.githubusercontent.com/neuml/txtai/master/demo.gif)
         
-        Traditional search systems use keywords to find data. Semantic search applications have an understanding of natural language and identify results that have the same meaning, not necessarily the same keywords.
+        Traditional search systems use keywords to find data. Semantic search has an understanding of natural language and identifies results that have the same meaning, not necessarily the same keywords.
         
         ![search](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/search.png#gh-light-mode-only)
         
-        Backed by state-of-the-art machine learning models, data is transformed into vector representations for search (also known as embeddings). Innovation is happening at a rapid pace, models can understand concepts in documents, audio, images and video.
+        txtai builds embeddings databases, which are a union of vector indexes and relational databases. This enables similarity search with SQL. Embeddings databases can stand on their own and/or serve as a powerful knowledge source for large language model (LLM) prompts.
+        
+        Semantic workflows connect language models together to build intelligent applications.
+        
+        ![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-light-mode-only)
+        
+        Integrate vector search, conversational search, automatic summarization, transcription, translation and more.
         
         Summary of txtai features:
         
-        - 🔎 Large-scale similarity search with multiple index backends ([Faiss](https://github.com/facebookresearch/faiss), [Annoy](https://github.com/spotify/annoy), [Hnswlib](https://github.com/nmslib/hnswlib)) and support for external vector databases
-        - 📄 Create embeddings for text snippets, documents, audio, images and video
-        - 💡 Machine-learning pipelines that run question-answering, labeling, transcription, translation, summarization, LLM prompts and more
-        - ↪️️ Workflows to join pipelines together and aggregate business logic. txtai processes can be microservices or full-fledged indexing workflows.
+        - 🔎 Similarity search with SQL, object storage, topic modeling, graph analysis, multiple vector index backends ([Faiss](https://github.com/facebookresearch/faiss), [Annoy](https://github.com/spotify/annoy), [Hnswlib](https://github.com/nmslib/hnswlib)) and support for external vector databases
+        - 📄 Create embeddings for text, documents, audio, images and video
+        - 💡 Pipelines powered by language models that run question-answering, labeling, transcription, translation, summarization, LLM prompts and more
+        - ↪️️ Workflows to join pipelines together and aggregate business logic. txtai processes can be simple microservices or multi-model workflows.
         - ⚙️ Build with Python or YAML. API bindings available for [JavaScript](https://github.com/neuml/txtai.js), [Java](https://github.com/neuml/txtai.java), [Rust](https://github.com/neuml/txtai.rs) and [Go](https://github.com/neuml/txtai.go).
         - ☁️ Cloud-native architecture that scales out with container orchestration systems (e.g. Kubernetes)
         
-        Applications range from similarity search to NLP-driven data extractions that generate structured data. Semantic workflows transform and find data driven by user intent.
-        
-        ![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-light-mode-only)
-        
         The following applications are powered by txtai.
         
         ![apps](https://raw.githubusercontent.com/neuml/txtai/master/apps.jpg)
         
         | Application  | Description  |
         |:----------|:-------------|
+        | [txtchat](https://github.com/neuml/txtchat) | Conversational search and workflows for all |
         | [paperai](https://github.com/neuml/paperai) | Semantic search and workflows for medical/scientific papers |
         | [codequestion](https://github.com/neuml/codequestion) | Semantic search for developers |
         | [tldrstory](https://github.com/neuml/tldrstory) | Semantic search for headlines and story text |
-        | [neuspo](https://neuspo.com) | Fact-driven, real-time sports event and news site |
         
         txtai is built with Python 3.7+, [Hugging Face Transformers](https://github.com/huggingface/transformers), [Sentence Transformers](https://github.com/UKPLab/sentence-transformers) and [FastAPI](https://github.com/tiangolo/fastapi)
         
         ## Why txtai?
         
         ![why](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/why.png#gh-light-mode-only)
         
-        In addition to traditional search systems, a growing number of semantic search solutions are available, so why txtai?
+        In addition to traditional search systems, a growing number of language model backed solutions are available, so why txtai?
         
         - Up and running in minutes with [pip](https://neuml.github.io/txtai/install/) or [Docker](https://neuml.github.io/txtai/cloud/)
         ```python
         # Get started in a couple lines
         from txtai.embeddings import Embeddings
         
         embeddings = Embeddings({"path": "sentence-transformers/all-MiniLM-L6-v2"})
         embeddings.index([(0, "Correct", None), (1, "Not what we hoped", None)])
         embeddings.search("positive", 1)
         #[(0, 0.2986203730106354)]
         ```
-        - Build applications in your programming language of choice via the API
+        - Built-in API makes it easy to develop applications using your programming language of choice
         ```yaml
         # app.yml
         embeddings:
             path: sentence-transformers/all-MiniLM-L6-v2
         ```
         ```bash
         CONFIG=app.yml uvicorn "txtai.api:app"
         curl -X GET "http://localhost:8000/search?query=positive"
         ```
-        - Connect machine learning models together to build intelligent data processing workflows
-        - Works with both small and big data - scale when needed
-        - Supports micromodels all the way up to large language models (LLMs)
-        - Low footprint - install additional dependencies when you need them
+        - Run local - no need to ship data off to disparate remote services
+        - Work with micromodels all the way up to large language models (LLMs)
+        - Low footprint - install additional dependencies and scale up when needed
         - [Learn by example](#examples) - notebooks cover all available functionality
         
         ## Installation
         
         ![install](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/install.png#gh-light-mode-only)
         
         The easiest way to install is via pip and PyPI
@@ -150,15 +151,15 @@
         | [Semantic Graphs](https://github.com/neuml/txtai/blob/master/examples/38_Introducing_the_Semantic_Graph.ipynb) | Explore topics, data connectivity and run network analysis| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/38_Introducing_the_Semantic_Graph.ipynb) |
         | [Topic Modeling with BM25](https://github.com/neuml/txtai/blob/master/examples/39_Classic_Topic_Modeling_with_BM25.ipynb) | Topic modeling backed by a BM25 index | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/39_Classic_Topic_Modeling_with_BM25.ipynb) |
         | [Prompt-driven search with LLMs](https://github.com/neuml/txtai/blob/master/examples/42_Prompt_driven_search_with_LLMs.ipynb) | Embeddings-guided and Prompt-driven search with Large Language Models (LLMs) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/42_Prompt_driven_search_with_LLMs.ipynb) |
         | [Embeddings in the Cloud](https://github.com/neuml/txtai/blob/master/examples/43_Embeddings_in_the_Cloud.ipynb) | Load and use an embeddings index from the Hugging Face Hub | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/43_Embeddings_in_the_Cloud.ipynb) |
         
         ### Pipelines
         
-        Transform data with NLP-backed pipelines.
+        Transform data with language model backed pipelines.
         
         | Notebook  | Description  |       |
         |:----------|:-------------|------:|
         | [Extractive QA with txtai](https://github.com/neuml/txtai/blob/master/examples/05_Extractive_QA_with_txtai.ipynb) | Introduction to extractive question-answering with txtai | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/05_Extractive_QA_with_txtai.ipynb) |
         | [Extractive QA with Elasticsearch](https://github.com/neuml/txtai/blob/master/examples/06_Extractive_QA_with_Elasticsearch.ipynb) | Run extractive question-answering queries with Elasticsearch | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/06_Extractive_QA_with_Elasticsearch.ipynb) |
         | [Extractive QA to build structured data](https://github.com/neuml/txtai/blob/master/examples/20_Extractive_QA_to_build_structured_data.ipynb) | Build structured datasets using extractive question-answering | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/20_Extractive_QA_to_build_structured_data.ipynb) |
         | [Apply labels with zero shot classification](https://github.com/neuml/txtai/blob/master/examples/07_Apply_labels_with_zero_shot_classification.ipynb) | Use zero shot learning for labeling, classification and topic modeling | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/07_Apply_labels_with_zero_shot_classification.ipynb) |
@@ -217,19 +218,19 @@
         
         [Full documentation on txtai](https://neuml.github.io/txtai) including configuration settings for pipelines, workflows, indexing and the API.
         
         ## Further Reading
         
         ![further](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/further.png)
         
-        - [Introducing txtai, AI-powered semantic search built on Transformers](https://medium.com/neuml/introducing-txtai-an-ai-powered-search-engine-built-on-transformers-37674be252ec)
+        - [Introducing txtai, semantic search and workflows built on Transformers](https://medium.com/neuml/introducing-txtai-an-ai-powered-search-engine-built-on-transformers-37674be252ec)
         - [Tutorial series on Hashnode](https://neuml.hashnode.dev/series/txtai-tutorial) | [dev.to](https://dev.to/neuml/tutorial-series-on-txtai-ibg)
         - [What's new in txtai 5.0](https://medium.com/neuml/whats-new-in-txtai-5-0-e5c75a13b101) | [4.0](https://medium.com/neuml/whats-new-in-txtai-4-0-bbc3a65c3d1c)
         - [Getting started with semantic search](https://medium.com/neuml/getting-started-with-semantic-search-a9fd9d8a48cf) | [workflows](https://medium.com/neuml/getting-started-with-semantic-workflows-2fefda6165d9)
-        - [Run machine-learning workflows to transform data and build AI-powered semantic search applications with txtai](https://medium.com/neuml/run-machine-learning-workflows-to-transform-data-and-build-ai-powered-text-indices-with-txtai-43d769b566a7)
+        - [Run workflows to transform data and build semantic search applications with txtai](https://medium.com/neuml/run-machine-learning-workflows-to-transform-data-and-build-ai-powered-text-indices-with-txtai-43d769b566a7)
         - [Semantic search on the cheap](https://medium.com/neuml/semantic-search-on-the-cheap-55940c0fcdab)
         - [Serverless vector search with txtai](https://medium.com/neuml/serverless-vector-search-with-txtai-96f6163ab972)
         - [Insights from the txtai console](https://medium.com/neuml/insights-from-the-txtai-console-d307c28e149e)
         - [The big and small of txtai](https://medium.com/neuml/the-big-and-small-of-txtai-4ca405c1b82)
         
         ## Contributing
```

#### html2text {}

```diff
@@ -1,73 +1,74 @@
-Metadata-Version: 2.1 Name: txtai Version: 5.4.0 Summary: Build AI-powered
-semantic search applications Home-page: https://github.com/neuml/txtai Author:
-NeuML License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0 Project-
-URL: Documentation, https://github.com/neuml/txtai Project-URL: Issue Tracker,
-https://github.com/neuml/txtai/issues Project-URL: Source Code, https://
-github.com/neuml/txtai Description:
+Metadata-Version: 2.1 Name: txtai Version: 5.5.0 Summary: Semantic search and
+workflows powered by language models Home-page: https://github.com/neuml/txtai
+Author: NeuML License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0
+Project-URL: Documentation, https://github.com/neuml/txtai Project-URL: Issue
+Tracker, https://github.com/neuml/txtai/issues Project-URL: Source Code, https:
+//github.com/neuml/txtai Description:
         [https://raw.githubusercontent.com/neuml/txtai/master/logo.png]
-            **** Build AI-powered semantic search applications ****
+      **** Semantic search and workflows powered by language models ****
   [Version] [GitHub_last_commit] [GitHub_issues] [Join_Slack] [Build_Status]
                                [Coverage_Status]
 -------------------------------------------------------------------------------
 ------------------------------------------------------------------------ txtai
-executes machine-learning workflows to transform data and build AI-powered
-semantic search applications. ![demo](https://raw.githubusercontent.com/neuml/
-txtai/master/demo.gif) Traditional search systems use keywords to find data.
-Semantic search applications have an understanding of natural language and
-identify results that have the same meaning, not necessarily the same keywords.
-![search](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/
-search.png#gh-light-mode-only) Backed by state-of-the-art machine learning
-models, data is transformed into vector representations for search (also known
-as embeddings). Innovation is happening at a rapid pace, models can understand
-concepts in documents, audio, images and video. Summary of txtai features: -
-ð Large-scale similarity search with multiple index backends ([Faiss](https:
-//github.com/facebookresearch/faiss), [Annoy](https://github.com/spotify/
-annoy), [Hnswlib](https://github.com/nmslib/hnswlib)) and support for external
-vector databases - ð Create embeddings for text snippets, documents, audio,
-images and video - ð¡ Machine-learning pipelines that run question-answering,
-labeling, transcription, translation, summarization, LLM prompts and more -
-âªï¸ï¸ Workflows to join pipelines together and aggregate business logic.
-txtai processes can be microservices or full-fledged indexing workflows. -
-âï¸ Build with Python or YAML. API bindings available for [JavaScript]
-(https://github.com/neuml/txtai.js), [Java](https://github.com/neuml/
-txtai.java), [Rust](https://github.com/neuml/txtai.rs) and [Go](https://
-github.com/neuml/txtai.go). - âï¸ Cloud-native architecture that scales out
-with container orchestration systems (e.g. Kubernetes) Applications range from
-similarity search to NLP-driven data extractions that generate structured data.
-Semantic workflows transform and find data driven by user intent. ![flows]
+is an open-source platform for semantic search and workflows powered by
+language models. ![demo](https://raw.githubusercontent.com/neuml/txtai/master/
+demo.gif) Traditional search systems use keywords to find data. Semantic search
+has an understanding of natural language and identifies results that have the
+same meaning, not necessarily the same keywords. ![search](https://
+raw.githubusercontent.com/neuml/txtai/master/docs/images/search.png#gh-light-
+mode-only) txtai builds embeddings databases, which are a union of vector
+indexes and relational databases. This enables similarity search with SQL.
+Embeddings databases can stand on their own and/or serve as a powerful
+knowledge source for large language model (LLM) prompts. Semantic workflows
+connect language models together to build intelligent applications. ![flows]
 (https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-
-light-mode-only) The following applications are powered by txtai. ![apps]
-(https://raw.githubusercontent.com/neuml/txtai/master/apps.jpg) | Application |
-Description | |:----------|:-------------| | [paperai](https://github.com/
-neuml/paperai) | Semantic search and workflows for medical/scientific papers |
-| [codequestion](https://github.com/neuml/codequestion) | Semantic search for
-developers | | [tldrstory](https://github.com/neuml/tldrstory) | Semantic
-search for headlines and story text | | [neuspo](https://neuspo.com) | Fact-
-driven, real-time sports event and news site | txtai is built with Python 3.7+,
-[Hugging Face Transformers](https://github.com/huggingface/transformers),
-[Sentence Transformers](https://github.com/UKPLab/sentence-transformers) and
-[FastAPI](https://github.com/tiangolo/fastapi) ## Why txtai? ![why](https://
-raw.githubusercontent.com/neuml/txtai/master/docs/images/why.png#gh-light-mode-
-only) In addition to traditional search systems, a growing number of semantic
-search solutions are available, so why txtai? - Up and running in minutes with
-[pip](https://neuml.github.io/txtai/install/) or [Docker](https://
-neuml.github.io/txtai/cloud/) ```python # Get started in a couple lines from
-txtai.embeddings import Embeddings embeddings = Embeddings({"path": "sentence-
-transformers/all-MiniLM-L6-v2"}) embeddings.index([(0, "Correct", None), (1,
-"Not what we hoped", None)]) embeddings.search("positive", 1) #[(0,
-0.2986203730106354)] ``` - Build applications in your programming language of
-choice via the API ```yaml # app.yml embeddings: path: sentence-transformers/
+light-mode-only) Integrate vector search, conversational search, automatic
+summarization, transcription, translation and more. Summary of txtai features:
+- ð Similarity search with SQL, object storage, topic modeling, graph
+analysis, multiple vector index backends ([Faiss](https://github.com/
+facebookresearch/faiss), [Annoy](https://github.com/spotify/annoy), [Hnswlib]
+(https://github.com/nmslib/hnswlib)) and support for external vector databases
+- ð Create embeddings for text, documents, audio, images and video - ð¡
+Pipelines powered by language models that run question-answering, labeling,
+transcription, translation, summarization, LLM prompts and more - âªï¸ï¸
+Workflows to join pipelines together and aggregate business logic. txtai
+processes can be simple microservices or multi-model workflows. - âï¸ Build
+with Python or YAML. API bindings available for [JavaScript](https://
+github.com/neuml/txtai.js), [Java](https://github.com/neuml/txtai.java), [Rust]
+(https://github.com/neuml/txtai.rs) and [Go](https://github.com/neuml/
+txtai.go). - âï¸ Cloud-native architecture that scales out with container
+orchestration systems (e.g. Kubernetes) The following applications are powered
+by txtai. ![apps](https://raw.githubusercontent.com/neuml/txtai/master/
+apps.jpg) | Application | Description | |:----------|:-------------| |
+[txtchat](https://github.com/neuml/txtchat) | Conversational search and
+workflows for all | | [paperai](https://github.com/neuml/paperai) | Semantic
+search and workflows for medical/scientific papers | | [codequestion](https://
+github.com/neuml/codequestion) | Semantic search for developers | | [tldrstory]
+(https://github.com/neuml/tldrstory) | Semantic search for headlines and story
+text | txtai is built with Python 3.7+, [Hugging Face Transformers](https://
+github.com/huggingface/transformers), [Sentence Transformers](https://
+github.com/UKPLab/sentence-transformers) and [FastAPI](https://github.com/
+tiangolo/fastapi) ## Why txtai? ![why](https://raw.githubusercontent.com/neuml/
+txtai/master/docs/images/why.png#gh-light-mode-only) In addition to traditional
+search systems, a growing number of language model backed solutions are
+available, so why txtai? - Up and running in minutes with [pip](https://
+neuml.github.io/txtai/install/) or [Docker](https://neuml.github.io/txtai/
+cloud/) ```python # Get started in a couple lines from txtai.embeddings import
+Embeddings embeddings = Embeddings({"path": "sentence-transformers/all-MiniLM-
+L6-v2"}) embeddings.index([(0, "Correct", None), (1, "Not what we hoped",
+None)]) embeddings.search("positive", 1) #[(0, 0.2986203730106354)] ``` -
+Built-in API makes it easy to develop applications using your programming
+language of choice ```yaml # app.yml embeddings: path: sentence-transformers/
 all-MiniLM-L6-v2 ``` ```bash CONFIG=app.yml uvicorn "txtai.api:app" curl -X GET
-"http://localhost:8000/search?query=positive" ``` - Connect machine learning
-models together to build intelligent data processing workflows - Works with
-both small and big data - scale when needed - Supports micromodels all the way
-up to large language models (LLMs) - Low footprint - install additional
-dependencies when you need them - [Learn by example](#examples) - notebooks
-cover all available functionality ## Installation ![install](https://
+"http://localhost:8000/search?query=positive" ``` - Run local - no need to ship
+data off to disparate remote services - Work with micromodels all the way up to
+large language models (LLMs) - Low footprint - install additional dependencies
+and scale up when needed - [Learn by example](#examples) - notebooks cover all
+available functionality ## Installation ![install](https://
 raw.githubusercontent.com/neuml/txtai/master/docs/images/install.png#gh-light-
 mode-only) The easiest way to install is via pip and PyPI ``` pip install txtai
 ``` Python 3.7+ is supported. Using a Python [virtual environment](https://
 docs.python.org/3/library/venv.html) is recommended. See the detailed [install
 instructions](https://neuml.github.io/txtai/install) for more information
 covering [optional dependencies](https://neuml.github.io/txtai/install/
 #optional-dependencies), [environment specific prerequisites](https://
@@ -165,18 +166,18 @@
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/neuml/txtai/blob/master/examples/
 42_Prompt_driven_search_with_LLMs.ipynb) | | [Embeddings in the Cloud](https://
 github.com/neuml/txtai/blob/master/examples/43_Embeddings_in_the_Cloud.ipynb) |
 Load and use an embeddings index from the Hugging Face Hub | [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/neuml/txtai/blob/master/examples/
-43_Embeddings_in_the_Cloud.ipynb) | ### Pipelines Transform data with NLP-
-backed pipelines. | Notebook | Description | | |:----------|:-------------|----
---:| | [Extractive QA with txtai](https://github.com/neuml/txtai/blob/master/
-examples/05_Extractive_QA_with_txtai.ipynb) | Introduction to extractive
+43_Embeddings_in_the_Cloud.ipynb) | ### Pipelines Transform data with language
+model backed pipelines. | Notebook | Description | | |:----------|:------------
+-|------:| | [Extractive QA with txtai](https://github.com/neuml/txtai/blob/
+master/examples/05_Extractive_QA_with_txtai.ipynb) | Introduction to extractive
 question-answering with txtai | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/neuml/txtai/blob/master/examples/
 05_Extractive_QA_with_txtai.ipynb) | | [Extractive QA with Elasticsearch]
 (https://github.com/neuml/txtai/blob/master/examples/
 06_Extractive_QA_with_Elasticsearch.ipynb) | Run extractive question-answering
 queries with Elasticsearch | [![Open In Colab](https://
@@ -338,29 +339,29 @@
 examples/workflows.py) | Build and execute txtai workflows. Connect
 summarization, text extraction, transcription, translation and similarity
 search pipelines together to run unified workflows. |[ð¤](https://hf.co/
 spaces/NeuML/txtai)| ## Documentation [Full documentation on txtai](https://
 neuml.github.io/txtai) including configuration settings for pipelines,
 workflows, indexing and the API. ## Further Reading ![further](https://
 raw.githubusercontent.com/neuml/txtai/master/docs/images/further.png) -
-[Introducing txtai, AI-powered semantic search built on Transformers](https://
-medium.com/neuml/introducing-txtai-an-ai-powered-search-engine-built-on-
+[Introducing txtai, semantic search and workflows built on Transformers](https:
+//medium.com/neuml/introducing-txtai-an-ai-powered-search-engine-built-on-
 transformers-37674be252ec) - [Tutorial series on Hashnode](https://
 neuml.hashnode.dev/series/txtai-tutorial) | [dev.to](https://dev.to/neuml/
 tutorial-series-on-txtai-ibg) - [What's new in txtai 5.0](https://medium.com/
 neuml/whats-new-in-txtai-5-0-e5c75a13b101) | [4.0](https://medium.com/neuml/
 whats-new-in-txtai-4-0-bbc3a65c3d1c) - [Getting started with semantic search]
 (https://medium.com/neuml/getting-started-with-semantic-search-a9fd9d8a48cf) |
 [workflows](https://medium.com/neuml/getting-started-with-semantic-workflows-
-2fefda6165d9) - [Run machine-learning workflows to transform data and build AI-
-powered semantic search applications with txtai](https://medium.com/neuml/run-
-machine-learning-workflows-to-transform-data-and-build-ai-powered-text-indices-
-with-txtai-43d769b566a7) - [Semantic search on the cheap](https://medium.com/
-neuml/semantic-search-on-the-cheap-55940c0fcdab) - [Serverless vector search
-with txtai](https://medium.com/neuml/serverless-vector-search-with-txtai-
+2fefda6165d9) - [Run workflows to transform data and build semantic search
+applications with txtai](https://medium.com/neuml/run-machine-learning-
+workflows-to-transform-data-and-build-ai-powered-text-indices-with-txtai-
+43d769b566a7) - [Semantic search on the cheap](https://medium.com/neuml/
+semantic-search-on-the-cheap-55940c0fcdab) - [Serverless vector search with
+txtai](https://medium.com/neuml/serverless-vector-search-with-txtai-
 96f6163ab972) - [Insights from the txtai console](https://medium.com/neuml/
 insights-from-the-txtai-console-d307c28e149e) - [The big and small of txtai]
 (https://medium.com/neuml/the-big-and-small-of-txtai-4ca405c1b82) ##
 Contributing For those who would like to contribute to txtai, please see [this
 guide](https://github.com/neuml/.github/blob/master/CONTRIBUTING.md). Keywords:
 search embedding machine-learning nlp Platform: UNKNOWN Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
```

### Comparing `txtai-5.4.0/src/python/txtai.egg-info/SOURCES.txt` & `txtai-5.5.0/src/python/txtai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,17 @@
 src/python/txtai/data/labels.py
 src/python/txtai/data/questions.py
 src/python/txtai/data/sequences.py
 src/python/txtai/data/texts.py
 src/python/txtai/data/tokens.py
 src/python/txtai/database/__init__.py
 src/python/txtai/database/base.py
+src/python/txtai/database/duckdb.py
 src/python/txtai/database/factory.py
+src/python/txtai/database/filedb.py
 src/python/txtai/database/sqlite.py
 src/python/txtai/database/encoder/__init__.py
 src/python/txtai/database/encoder/base.py
 src/python/txtai/database/encoder/factory.py
 src/python/txtai/database/encoder/image.py
 src/python/txtai/database/encoder/pickle.py
 src/python/txtai/database/sql/__init__.py
@@ -148,10 +150,11 @@
 src/python/txtai/workflow/task/export.py
 src/python/txtai/workflow/task/factory.py
 src/python/txtai/workflow/task/file.py
 src/python/txtai/workflow/task/image.py
 src/python/txtai/workflow/task/retrieve.py
 src/python/txtai/workflow/task/service.py
 src/python/txtai/workflow/task/storage.py
+src/python/txtai/workflow/task/stream.py
 src/python/txtai/workflow/task/template.py
 src/python/txtai/workflow/task/url.py
 src/python/txtai/workflow/task/workflow.py
```

### Comparing `txtai-5.4.0/src/python/txtai.egg-info/requires.txt` & `txtai-5.5.0/src/python/txtai.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 [all]
 aiohttp>=3.8.1
 fastapi>=0.61.1
 uvicorn>=0.12.1
 apache-libcloud>=3.3.1
 rich>=12.0.1
+duckdb>=0.7.1
 pillow>=7.1.2
 networkx>=2.6.3
 python-louvain>=0.16
 onnx>=1.11.0
 onnxruntime>=1.11.0
 onnx>=1.11.0
 onnxruntime>=1.11.0
@@ -54,14 +55,15 @@
 [cloud]
 apache-libcloud>=3.3.1
 
 [console]
 rich>=12.0.1
 
 [database]
+duckdb>=0.7.1
 pillow>=7.1.2
 
 [dev]
 black
 coverage
 coveralls
 httpx
```

