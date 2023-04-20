# Comparing `tmp/soil-0.9.7.tar.gz` & `tmp/soil-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/soil-0.9.7.tar", last modified: Mon Oct  9 12:43:52 2017, max compression
+gzip compressed data, was "soil-1.0.0rc1.tar", last modified: Thu Apr 20 16:05:38 2023, max compression
```

## Comparing `soil-0.9.7.tar` & `soil-1.0.0rc1.tar`

### file list

```diff
@@ -1,96 +1,98 @@
-drwxr-xr-x   0 jfernando  (1000) jfernando  (1000)        0 2017-10-09 12:43:52.000000 soil-0.9.7/
-drwxr-xr-x   0 jfernando  (1000) jfernando  (1000)        0 2017-10-09 12:43:52.000000 soil-0.9.7/soil.egg-info/
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)       45 2017-10-09 12:43:51.000000 soil-0.9.7/soil.egg-info/entry_points.txt
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)        1 2017-10-09 12:43:51.000000 soil-0.9.7/soil.egg-info/dependency_links.txt
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)       45 2017-10-09 12:43:51.000000 soil-0.9.7/soil.egg-info/requires.txt
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)        5 2017-10-09 12:43:51.000000 soil-0.9.7/soil.egg-info/top_level.txt
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     3267 2017-10-09 12:43:52.000000 soil-0.9.7/soil.egg-info/SOURCES.txt
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)      839 2017-10-09 12:43:51.000000 soil-0.9.7/soil.egg-info/PKG-INFO
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)       84 2017-07-03 16:16:47.000000 soil-0.9.7/MANIFEST.in
-drwxr-xr-x   0 jfernando  (1000) jfernando  (1000)        0 2017-10-09 12:43:52.000000 soil-0.9.7/soil/
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1349 2017-10-09 12:43:47.000000 soil-0.9.7/soil/__init__.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     6499 2017-10-09 09:19:52.000000 soil-0.9.7/soil/environment.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1569 2017-10-09 09:21:10.000000 soil-0.9.7/soil/utils.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)       24 2017-07-03 16:16:47.000000 soil-0.9.7/soil/settings.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     6712 2017-10-09 12:35:25.000000 soil-0.9.7/soil/environment.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     8370 2017-10-09 09:19:52.000000 soil-0.9.7/soil/simulation.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)      431 2017-10-09 09:19:51.000000 soil-0.9.7/soil/__init__.pyc
-drwxr-xr-x   0 jfernando  (1000) jfernando  (1000)        0 2017-10-09 12:43:52.000000 soil-0.9.7/soil/__pycache__/
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1454 2017-10-09 12:43:51.000000 soil-0.9.7/soil/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     7415 2017-10-09 09:35:07.000000 soil-0.9.7/soil/__pycache__/simulation.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)      950 2017-07-03 10:42:16.000000 soil-0.9.7/soil/__pycache__/analysis.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)      112 2017-10-09 12:32:42.000000 soil-0.9.7/soil/__pycache__/settings.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1892 2017-10-09 09:21:59.000000 soil-0.9.7/soil/__pycache__/utils.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1900 2017-10-09 12:31:16.000000 soil-0.9.7/soil/__pycache__/utils.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     8067 2017-10-09 12:31:16.000000 soil-0.9.7/soil/__pycache__/simulation.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)      129 2017-07-03 16:17:39.000000 soil-0.9.7/soil/__pycache__/settings.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1258 2017-10-09 12:32:42.000000 soil-0.9.7/soil/__pycache__/__main__.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     5602 2017-10-09 12:37:37.000000 soil-0.9.7/soil/__pycache__/environment.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1553 2017-10-09 09:21:58.000000 soil-0.9.7/soil/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     6129 2017-10-09 09:21:59.000000 soil-0.9.7/soil/__pycache__/environment.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     8040 2017-10-09 09:21:59.000000 soil-0.9.7/soil/__pycache__/simulation.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1738 2017-10-09 09:35:07.000000 soil-0.9.7/soil/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     6160 2017-10-09 12:35:27.000000 soil-0.9.7/soil/__pycache__/environment.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)      112 2017-10-09 09:21:59.000000 soil-0.9.7/soil/__pycache__/settings.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1559 2017-10-09 12:31:15.000000 soil-0.9.7/soil/__pycache__/__init__.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1252 2017-10-09 09:21:59.000000 soil-0.9.7/soil/__pycache__/__main__.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)      103 2017-10-09 09:19:52.000000 soil-0.9.7/soil/settings.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1130 2017-10-09 09:10:43.000000 soil-0.9.7/soil/__main__.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     8744 2017-10-09 09:21:10.000000 soil-0.9.7/soil/simulation.py
-drwxr-xr-x   0 jfernando  (1000) jfernando  (1000)        0 2017-10-09 12:43:52.000000 soil-0.9.7/soil/agents/
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     2839 2017-10-09 09:19:51.000000 soil-0.9.7/soil/agents/SISaModel.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     4745 2017-10-09 09:21:10.000000 soil-0.9.7/soil/agents/__init__.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1016 2017-07-03 16:16:47.000000 soil-0.9.7/soil/agents/CounterModel.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1481 2017-10-09 09:19:51.000000 soil-0.9.7/soil/agents/CounterModel.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     6117 2017-10-09 09:19:51.000000 soil-0.9.7/soil/agents/__init__.pyc
-drwxr-xr-x   0 jfernando  (1000) jfernando  (1000)        0 2017-10-09 12:43:52.000000 soil-0.9.7/soil/agents/__pycache__/
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     5201 2017-10-09 09:35:07.000000 soil-0.9.7/soil/agents/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1401 2017-10-09 09:21:58.000000 soil-0.9.7/soil/agents/__pycache__/CounterModel.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1348 2017-10-09 09:21:58.000000 soil-0.9.7/soil/agents/__pycache__/BassModel.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1285 2017-07-03 16:17:39.000000 soil-0.9.7/soil/agents/__pycache__/BassModel.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)      915 2017-07-03 16:17:39.000000 soil-0.9.7/soil/agents/__pycache__/DrawingAgent.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1320 2017-07-03 16:17:39.000000 soil-0.9.7/soil/agents/__pycache__/CounterModel.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     6997 2017-10-09 12:31:15.000000 soil-0.9.7/soil/agents/__pycache__/ModelM2.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     2738 2017-10-09 09:30:26.000000 soil-0.9.7/soil/agents/__pycache__/SISaModel.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     3999 2017-07-02 12:29:55.000000 soil-0.9.7/soil/agents/__pycache__/BaseBehaviour.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1401 2017-10-09 12:31:15.000000 soil-0.9.7/soil/agents/__pycache__/CounterModel.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1626 2017-10-09 09:21:58.000000 soil-0.9.7/soil/agents/__pycache__/IndependentCascadeModel.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     2741 2017-10-09 12:31:15.000000 soil-0.9.7/soil/agents/__pycache__/SISaModel.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1534 2017-07-03 16:17:39.000000 soil-0.9.7/soil/agents/__pycache__/IndependentCascadeModel.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1629 2017-10-09 12:31:15.000000 soil-0.9.7/soil/agents/__pycache__/IndependentCascadeModel.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1351 2017-10-09 12:31:15.000000 soil-0.9.7/soil/agents/__pycache__/BassModel.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)      980 2017-10-09 09:21:58.000000 soil-0.9.7/soil/agents/__pycache__/DrawingAgent.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)      460 2017-06-20 15:00:40.000000 soil-0.9.7/soil/agents/__pycache__/models.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     5595 2017-10-09 09:21:58.000000 soil-0.9.7/soil/agents/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)      980 2017-10-09 12:31:15.000000 soil-0.9.7/soil/agents/__pycache__/DrawingAgent.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     2537 2017-10-09 09:35:07.000000 soil-0.9.7/soil/agents/__pycache__/SISaModel.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     2958 2017-07-03 16:17:39.000000 soil-0.9.7/soil/agents/__pycache__/BigMarketModel.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     3031 2017-10-09 09:21:58.000000 soil-0.9.7/soil/agents/__pycache__/SentimentCorrelationModel.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     5622 2017-10-09 12:31:15.000000 soil-0.9.7/soil/agents/__pycache__/__init__.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     3190 2017-10-09 09:21:58.000000 soil-0.9.7/soil/agents/__pycache__/BigMarketModel.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     3214 2017-10-09 12:31:15.000000 soil-0.9.7/soil/agents/__pycache__/BigMarketModel.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     3049 2017-10-09 12:31:15.000000 soil-0.9.7/soil/agents/__pycache__/SentimentCorrelationModel.cpython-34.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     2763 2017-07-03 16:17:39.000000 soil-0.9.7/soil/agents/__pycache__/SentimentCorrelationModel.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     6274 2017-07-03 16:17:39.000000 soil-0.9.7/soil/agents/__pycache__/ModelM2.cpython-36.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     6928 2017-10-09 09:21:58.000000 soil-0.9.7/soil/agents/__pycache__/ModelM2.cpython-35.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)      493 2017-07-03 16:16:47.000000 soil-0.9.7/soil/agents/DrawingAgent.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     7061 2017-10-09 09:19:51.000000 soil-0.9.7/soil/agents/ModelM2.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1436 2017-10-09 09:19:51.000000 soil-0.9.7/soil/agents/BassModel.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     3974 2017-10-09 09:30:20.000000 soil-0.9.7/soil/agents/SISaModel.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1754 2017-10-09 09:19:51.000000 soil-0.9.7/soil/agents/IndependentCascadeModel.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     4486 2017-07-03 16:16:47.000000 soil-0.9.7/soil/agents/BigMarketModel.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1153 2017-07-03 16:16:47.000000 soil-0.9.7/soil/agents/BassModel.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     3227 2017-10-09 09:19:51.000000 soil-0.9.7/soil/agents/SentimentCorrelationModel.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     4209 2017-07-03 16:16:47.000000 soil-0.9.7/soil/agents/SentimentCorrelationModel.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     3368 2017-10-09 09:19:51.000000 soil-0.9.7/soil/agents/BigMarketModel.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1623 2017-07-03 16:16:47.000000 soil-0.9.7/soil/agents/IndependentCascadeModel.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1102 2017-10-09 09:19:51.000000 soil-0.9.7/soil/agents/DrawingAgent.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)    10490 2017-07-03 16:16:47.000000 soil-0.9.7/soil/agents/ModelM2.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)      818 2017-07-03 16:16:47.000000 soil-0.9.7/soil/analysis.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     2239 2017-10-09 09:19:52.000000 soil-0.9.7/soil/utils.pyc
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1797 2017-10-09 09:36:50.000000 soil-0.9.7/setup.py
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)        0 2017-07-03 16:16:47.000000 soil-0.9.7/test-requirements.txt
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)       38 2017-10-09 12:43:52.000000 soil-0.9.7/setup.cfg
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)     1354 2017-07-03 16:41:34.000000 soil-0.9.7/README.md
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)       45 2017-10-09 09:21:03.000000 soil-0.9.7/requirements.txt
--rw-r--r--   0 jfernando  (1000) jfernando  (1000)      839 2017-10-09 12:43:52.000000 soil-0.9.7/PKG-INFO
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.760715 soil-1.0.0rc1/
+-rw-r--r--   0 j         (1000) j         (1000)    11412 2018-12-07 19:26:39.000000 soil-1.0.0rc1/LICENSE
+-rw-r--r--   0 j         (1000) j         (1000)      163 2020-03-11 15:11:50.000000 soil-1.0.0rc1/MANIFEST.in
+-rw-rw-r--   0 j         (1000) j         (1000)     5741 2023-04-20 16:05:38.760715 soil-1.0.0rc1/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)     4660 2023-04-20 15:35:04.000000 soil-1.0.0rc1/README.md
+-rw-rw-r--   0 j         (1000) j         (1000)      166 2023-04-14 21:22:05.000000 soil-1.0.0rc1/requirements.txt
+-rw-r--r--   0 j         (1000) j         (1000)      191 2023-04-20 16:05:38.760715 soil-1.0.0rc1/setup.cfg
+-rw-rw-r--   0 j         (1000) j         (1000)     2188 2023-04-20 16:05:16.000000 soil-1.0.0rc1/setup.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.748715 soil-1.0.0rc1/soil/
+-rw-rw-r--   0 j         (1000) j         (1000)      365 2023-03-23 13:48:55.000000 soil-1.0.0rc1/soil/.VERSION.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-14 19:48:55.000000 soil-1.0.0rc1/soil/.__init__.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    13297 2023-03-23 13:34:51.000000 soil-1.0.0rc1/soil/.analysis.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    14451 2023-04-14 21:44:41.000000 soil-1.0.0rc1/soil/.environment.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     2588 2023-04-14 20:43:29.000000 soil-1.0.0rc1/soil/.exporters.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     1110 2023-04-14 21:29:51.000000 soil-1.0.0rc1/soil/.serialization.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    15937 2023-04-16 19:59:22.000000 soil-1.0.0rc1/soil/.simulation.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     5011 2023-03-23 13:48:01.000000 soil-1.0.0rc1/soil/.stats.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    19083 2023-04-16 21:07:22.000000 soil-1.0.0rc1/soil/.time.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      330 2023-04-14 19:49:37.000000 soil-1.0.0rc1/soil/.utils.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-04 13:46:42.000000 soil-1.0.0rc1/soil/.visualization.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)        8 2023-04-20 16:02:50.000000 soil-1.0.0rc1/soil/VERSION
+-rw-rw-r--   0 j         (1000) j         (1000)     7923 2023-04-19 23:43:19.000000 soil-1.0.0rc1/soil/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      107 2023-04-14 18:17:58.000000 soil-1.0.0rc1/soil/__main__.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.748715 soil-1.0.0rc1/soil/agents/
+-rw-rw-r--   0 j         (1000) j         (1000)     1422 2023-04-16 20:19:36.000000 soil-1.0.0rc1/soil/agents/.__init__.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     5970 2023-04-14 19:52:27.000000 soil-1.0.0rc1/soil/agents/.fsm.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      734 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/agents/BassModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1171 2023-04-14 18:19:58.000000 soil-1.0.0rc1/soil/agents/CounterModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)      731 2023-04-17 13:43:11.000000 soil-1.0.0rc1/soil/agents/Geo.py
+-rw-rw-r--   0 j         (1000) j         (1000)      766 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/agents/IndependentCascadeModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3385 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/agents/SISaModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)    19495 2023-04-17 13:33:41.000000 soil-1.0.0rc1/soil/agents/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2365 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/agents/evented.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4493 2023-04-17 14:27:57.000000 soil-1.0.0rc1/soil/agents/fsm.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3409 2023-04-17 13:51:14.000000 soil-1.0.0rc1/soil/agents/network_agents.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2196 2023-04-20 11:27:08.000000 soil-1.0.0rc1/soil/analysis.py
+-rw-rw-r--   0 j         (1000) j         (1000)       36 2023-04-13 16:06:35.000000 soil-1.0.0rc1/soil/config.py
+-rw-rw-r--   0 j         (1000) j         (1000)      843 2023-04-18 16:33:54.000000 soil-1.0.0rc1/soil/datacollection.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7217 2023-04-14 15:59:02.000000 soil-1.0.0rc1/soil/debugging.py
+-rw-rw-r--   0 j         (1000) j         (1000)      168 2023-04-14 11:40:15.000000 soil-1.0.0rc1/soil/decorators.py
+-rw-rw-r--   0 j         (1000) j         (1000)    15254 2023-04-20 09:19:00.000000 soil-1.0.0rc1/soil/environment.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1092 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/events.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9141 2023-04-20 11:22:12.000000 soil-1.0.0rc1/soil/exporters.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2149 2023-04-09 02:16:08.000000 soil-1.0.0rc1/soil/network.py
+-rw-rw-r--   0 j         (1000) j         (1000)      739 2023-04-08 22:41:17.000000 soil-1.0.0rc1/soil/parameters.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7687 2023-04-14 21:29:51.000000 soil-1.0.0rc1/soil/serialization.py
+-rw-r--r--   0 j         (1000) j         (1000)       24 2018-12-07 19:26:39.000000 soil-1.0.0rc1/soil/settings.py
+-rw-rw-r--   0 j         (1000) j         (1000)    13830 2023-04-20 14:51:30.000000 soil-1.0.0rc1/soil/simulation.py
+-rw-rw-r--   0 j         (1000) j         (1000)     6099 2023-04-17 22:07:07.000000 soil-1.0.0rc1/soil/time.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4381 2023-04-17 21:29:17.000000 soil-1.0.0rc1/soil/utils.py
+-rw-rw-r--   0 j         (1000) j         (1000)      476 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/version.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.748715 soil-1.0.0rc1/soil/web/
+-rw-r--r--   0 j         (1000) j         (1000)       41 2018-12-08 17:08:24.000000 soil-1.0.0rc1/soil/web/.gitignore
+-rw-r--r--   0 j         (1000) j         (1000)     2984 2018-12-08 17:08:24.000000 soil-1.0.0rc1/soil/web/README.md
+-rw-rw-r--   0 j         (1000) j         (1000)    11272 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/web/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)       59 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/web/__main__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      575 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/web/config.yml
+-rw-rw-r--   0 j         (1000) j         (1000)     1073 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/web/run.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.740715 soil-1.0.0rc1/soil/web/static/
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.748715 soil-1.0.0rc1/soil/web/static/css/
+-rw-r--r--   0 j         (1000) j         (1000)     7157 2018-12-08 17:08:24.000000 soil-1.0.0rc1/soil/web/static/css/main.css
+-rw-r--r--   0 j         (1000) j         (1000)     1107 2018-12-08 17:08:24.000000 soil-1.0.0rc1/soil/web/static/css/timeline.css
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.748715 soil-1.0.0rc1/soil/web/static/img/
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.752715 soil-1.0.0rc1/soil/web/static/img/background/
+-rw-r--r--   0 j         (1000) j         (1000)  1167302 2018-12-08 17:08:24.000000 soil-1.0.0rc1/soil/web/static/img/background/map.png
+-rw-r--r--   0 j         (1000) j         (1000)  8340070 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/background/map_4800x2860.jpg
+-rw-r--r--   0 j         (1000) j         (1000)    18053 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/logo_gsi.svg
+-rw-r--r--   0 j         (1000) j         (1000)   103744 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/logo_soil.png
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.760715 soil-1.0.0rc1/soil/web/static/img/svg/
+-rw-r--r--   0 j         (1000) j         (1000)      462 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/svg/home.svg
+-rw-r--r--   0 j         (1000) j         (1000)      812 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/svg/person.svg
+-rw-r--r--   0 j         (1000) j         (1000)      697 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/svg/plus.svg
+-rw-r--r--   0 j         (1000) j         (1000)      992 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/svg/target.svg
+-rw-r--r--   0 j         (1000) j         (1000)     1561 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/svg/time.svg
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.760715 soil-1.0.0rc1/soil/web/static/js/
+-rwxr-xr-x   0 j         (1000) j         (1000)    16528 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/js/socket.js
+-rw-r--r--   0 j         (1000) j         (1000)     5040 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/js/template.js
+-rw-r--r--   0 j         (1000) j         (1000)    12269 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/js/timeline.js
+-rw-r--r--   0 j         (1000) j         (1000)    21818 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/js/visualization.js
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.760715 soil-1.0.0rc1/soil/web/templates/
+-rw-r--r--   0 j         (1000) j         (1000)    16450 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/templates/index.html
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.748715 soil-1.0.0rc1/soil.egg-info/
+-rw-r--r--   0 j         (1000) j         (1000)     5741 2023-04-20 16:05:38.000000 soil-1.0.0rc1/soil.egg-info/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)     2046 2023-04-20 16:05:38.000000 soil-1.0.0rc1/soil.egg-info/SOURCES.txt
+-rw-r--r--   0 j         (1000) j         (1000)        1 2023-04-20 16:05:38.000000 soil-1.0.0rc1/soil.egg-info/dependency_links.txt
+-rw-r--r--   0 j         (1000) j         (1000)       78 2023-04-20 16:05:38.000000 soil-1.0.0rc1/soil.egg-info/entry_points.txt
+-rw-r--r--   0 j         (1000) j         (1000)      257 2023-04-20 16:05:38.000000 soil-1.0.0rc1/soil.egg-info/requires.txt
+-rw-r--r--   0 j         (1000) j         (1000)        5 2023-04-20 16:05:38.000000 soil-1.0.0rc1/soil.egg-info/top_level.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       43 2023-03-23 16:42:54.000000 soil-1.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.760715 soil-1.0.0rc1/tests/
+-rw-rw-r--   0 j         (1000) j         (1000)     5920 2023-04-17 17:50:01.000000 soil-1.0.0rc1/tests/test_agents.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2336 2023-04-19 17:02:06.000000 soil-1.0.0rc1/tests/test_config.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2450 2023-04-19 17:02:06.000000 soil-1.0.0rc1/tests/test_examples.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3756 2023-04-20 11:00:16.000000 soil-1.0.0rc1/tests/test_exporters.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7709 2023-04-19 22:29:46.000000 soil-1.0.0rc1/tests/test_main.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1940 2023-03-23 16:42:54.000000 soil-1.0.0rc1/tests/test_mesa.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3133 2023-04-14 11:36:16.000000 soil-1.0.0rc1/tests/test_network.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2092 2023-04-17 17:32:50.000000 soil-1.0.0rc1/tests/test_time.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `soil-0.9.7/soil/environment.py` & `soil-1.0.0rc1/tests/test_agents.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,189 +1,177 @@
-import os
-import csv
-import weakref
-from random import random
-from copy import deepcopy
-
-import networkx as nx
-import nxsim
-
-
-class SoilEnvironment(nxsim.NetworkEnvironment):
-
-    def __init__(self, name=None,
-                 network_agents=None,
-                 environment_agents=None,
-                 states=None,
-                 default_state=None,
-                 interval=1,
-                 *args, **kwargs):
-        self.name = name or 'UnnamedEnvironment'
-        self.states = deepcopy(states) or {}
-        self.default_state = deepcopy(default_state) or {}
-        super().__init__(*args, **kwargs)
-        self._env_agents = {}
-        self._history = {}
-        self.interval = interval
-        self.logger = None
-        # Add environment agents first, so their events get
-        # executed before network agents
-        self.environment_agents = environment_agents or []
-        self.network_agents = network_agents or []
-        self.process(self.save_state())
-
-    @property
-    def agents(self):
-        yield from self.environment_agents
-        yield from self.network_agents
-
-    @property
-    def environment_agents(self):
-        for ref in self._env_agents.values():
-            yield ref()
-
-    @environment_agents.setter
-    def environment_agents(self, environment_agents):
-        # Set up environmental agent
-        self._env_agents = {}
-        for item in environment_agents:
-            kwargs = deepcopy(item)
-            atype = kwargs.pop('agent_type')
-            kwargs['agent_id'] = kwargs.get('agent_id', atype.__name__)
-            kwargs['state'] = kwargs.get('state', {})
-            a = atype(environment=self, **kwargs)
-            self._env_agents[a.id] = weakref.ref(a)
-
-    @property
-    def network_agents(self):
-        for i in self.G.nodes():
-            node = self.G.node[i]
-            if 'agent' in node:
-                yield node['agent']
-
-    @network_agents.setter
-    def network_agents(self, network_agents):
-        for ix in self.G.nodes():
-            i = ix
-            node = self.G.node[i]
-            v = random()
-            found = False
-            for d in network_agents:
-                threshold = d['threshold']
-                if v >= threshold[0] and v < threshold[1]:
-                    agent = d['agent_type']
-                    state = None
-                    if 'state' in d:
-                        state = deepcopy(d['state'])
-                    else:
-                        try:
-                            state = self.states[i]
-                        except (IndexError, KeyError):
-                            state = deepcopy(self.default_state)
-                    node['agent'] = agent(environment=self,
-                                          agent_id=i,
-                                          state=state)
-                    found = True
-                    break
-            assert found
-
-    def run(self, *args, **kwargs):
-        self._save_state()
-        super().run(*args, **kwargs)
-        self._save_state()
-
-    def _save_state(self):
-        for agent in self.agents:
-            agent.save_state()
-        self._history[self.now] = deepcopy(self.environment_params)
-
-    def save_state(self):
-        while True:
-            ev = self.event()
-            ev._ok = True
-            # Schedule the event with minimum priority so
-            # that it executes after all agents are done
-            self.schedule(ev, -1, self.interval)
-            yield ev
-            self._save_state()
-
-    def __getitem__(self, key):
-        return self.environment_params[key]
-
-    def __setitem__(self, key, value):
-        self.environment_params[key] = value
-
-    def get_path(self, dir_path=None):
-        dir_path = dir_path or self.sim().dir_path
-        if not os.path.exists(dir_path):
-            os.makedirs(dir_path)
-        return dir_path
-
-    def get_agent(self, agent_id):
-        return self.G.node[agent_id]['agent']
-
-    def get_agents(self):
-        return list(self.agents)
-
-    def dump_csv(self, dir_path=None):
-        csv_name = os.path.join(self.get_path(dir_path),
-                                '{}.environment.csv'.format(self.name))
-
-        with open(csv_name, 'w') as f:
-            cr = csv.writer(f)
-            cr.writerow(('agent_id', 'tstep', 'attribute', 'value'))
-            for i in self.history_to_tuples():
-                cr.writerow(i)
-
-    def dump_gexf(self, dir_path=None):
-        G = self.history_to_graph()
-        graph_path = os.path.join(self.get_path(dir_path),
-                                  self.name+".gexf")
-        nx.write_gexf(G, graph_path, version="1.2draft")
-
-    def history_to_tuples(self):
-        for tstep, state in self._history.items():
-            for attribute, value in state.items():
-                yield ('env', tstep, attribute, value)
-        for agent in self.agents:
-            for tstep, state in agent._history.items():
-                for attribute, value in state.items():
-                    yield (agent.id, tstep, attribute, value)
-
-    def history_to_graph(self):
-        G = nx.Graph(self.G)
-
-        for agent in self.agents:
-
-            attributes = {'agent': str(agent.__class__)}
-            lastattributes = {}
-            spells = []
-            lastvisible = False
-            laststep = None
-            for t_step, state in reversed(list(agent._history.items())):
-                for attribute, value in state.items():
-                    if attribute == 'visible':
-                        nowvisible = state[attribute]
-                        if nowvisible and not lastvisible:
-                            laststep = t_step
-                        if not nowvisible and lastvisible:
-                            spells.append((laststep, t_step))
+from unittest import TestCase
+import pytest
 
-                        lastvisible = nowvisible
-                    else:
-                        if attribute not in lastattributes or lastattributes[attribute][0] != value:
-                            laststep = lastattributes.get(attribute,
-                                                          (None, None))[1]
-                            value = (state[attribute], t_step, laststep)
-                            key = 'attr_' + attribute
-                            if key not in attributes:
-                                attributes[key] = list()
-                            attributes[key].append(value)
-                            lastattributes[attribute] = (state[attribute], t_step)
-            if lastvisible:
-                spells.append((laststep, None))
-            if spells:
-                G.add_node(agent.id, spells=spells, **attributes)
-            else:
-                G.add_node(agent.id, **attributes)
+from soil import agents, environment
+from soil import time as stime
 
-        return G
+
+class Dead(agents.FSM):
+    @agents.default_state
+    @agents.state
+    def only(self):
+        return self.die()
+
+
+class TestAgents(TestCase):
+    def test_die_returns_infinity(self):
+        """The last step of a dead agent should return time.INFINITY"""
+        d = Dead(unique_id=0, model=environment.Environment())
+        ret = d.step()
+        assert ret == stime.NEVER
+
+    def test_die_raises_exception(self):
+        """A dead agent should raise an exception if it is stepped after death"""
+        d = Dead(unique_id=0, model=environment.Environment())
+        assert d.alive
+        d.step()
+        assert not d.alive
+        with pytest.raises(stime.DeadAgent):
+            d.step()
+
+    def test_agent_generator(self):
+        """
+        The step function of an agent could be a generator. In that case, the state of the
+        agent will be resumed after every call to step.
+        """
+        a = 0
+
+        class Gen(agents.BaseAgent):
+            def step(self):
+                nonlocal a
+                for i in range(5):
+                    yield
+                    a += 1
+
+        e = environment.Environment()
+        g = Gen(model=e, unique_id=e.next_id())
+        e.schedule.add(g)
+
+        for i in range(5):
+            e.step()
+            assert a == i
+
+    def test_state_decorator(self):
+        class MyAgent(agents.FSM):
+            run = 0
+
+            @agents.state("original", default=True)
+            def root(self):
+                self.run += 1
+                return self.other
+
+            @agents.state
+            def other(self):
+                self.run += 1
+
+        e = environment.Environment()
+        a = e.add_agent(MyAgent)
+        e.step()
+        assert a.run == 1
+        a.step()
+        print("DONE")
+
+    def test_broadcast(self):
+        """
+        An agent should be able to broadcast messages to every other agent, AND each receiver should be able
+        to process it
+        """
+
+        class BCast(agents.Evented):
+            pings_received = 0
+
+            def step(self):
+                print(self.model.broadcast)
+                try:
+                    self.model.broadcast("PING")
+                except Exception as ex:
+                    print(ex)
+                while True:
+                    self.check_messages()
+                    yield
+
+            def on_receive(self, msg, sender=None):
+                self.pings_received += 1
+
+        e = environment.EventedEnvironment()
+
+        for i in range(10):
+            e.add_agent(agent_class=BCast)
+        e.step()
+        pings_received = lambda: [a.pings_received for a in e.agents]
+        assert sorted(pings_received()) == list(range(1, 11))
+        e.step()
+        assert all(x == 10 for x in pings_received())
+
+    def test_ask_messages(self):
+        """
+        An agent should be able to ask another agent, and wait for a response.
+        """
+
+        # There are two agents, they try to send pings
+        # This is arguably a very contrived example.
+        # There should be a delay of one step between agent 0 and 1
+        # On the first step:
+        #   Agent 0 sends a PING, but blocks before a PONG
+        #   Agent 1 detects the PING, responds with a PONG, and blocks after its own PING
+        # After that step, every agent can both receive (there are pending messages) and send.
+        # In each step, for each agent, one message is sent, and another one is received
+        # (although not necessarily in that order).
+
+        # Results depend on ordering (agents are normally shuffled)
+        # so we force the timedactivation not to be shuffled
+
+        pings = []
+        pongs = []
+        responses = []
+
+        class Ping(agents.EventedAgent):
+            def step(self):
+                target_id = (self.unique_id + 1) % self.count_agents()
+                target = self.model.agents[target_id]
+                print("starting")
+                while True:
+                    if pongs or not pings:  # First agent, or anyone after that
+                        pings.append(self.now)
+                        response = yield target.ask("PING")
+                        responses.append(response)
+                    else:
+                        print("NOT sending ping")
+                    print("Checking msgs")
+                    # Do not block if we have already received a PING
+                    if not self.check_messages():
+                        yield self.received()
+                print("done")
+
+            def on_receive(self, msg, sender=None):
+                if msg == "PING":
+                    pongs.append(self.now)
+                    return "PONG"
+                raise Exception("This should never happen")
+
+        e = environment.EventedEnvironment(schedule_class=stime.OrderedTimedActivation)
+        for i in range(2):
+            e.add_agent(agent_class=Ping)
+        assert e.now == 0
+
+        for i in range(5):
+            e.step()
+            time = i + 1
+            assert e.now == time
+            assert len(pings) == 2 * time
+            assert len(pongs) == (2 * time) - 1
+            # Every step between 0 and t appears twice
+            assert sum(pings) == sum(range(time)) * 2
+            # It is the same as pings, without the leading 0
+            assert sum(pongs) == sum(range(time)) * 2
+
+    def test_agent_filter(self):
+        e = environment.Environment()
+        e.add_agent(agent_class=agents.BaseAgent)
+        e.add_agent(agent_class=agents.Evented)
+        base = list(e.agents(agent_class=agents.BaseAgent))
+        assert len(base) == 2
+        ev = list(e.agents(agent_class=agents.Evented))
+        assert len(ev) == 1
+        assert ev[0].unique_id == 1
+        null = list(e.agents(unique_ids=[0, 1], agent_class=agents.NetworkAgent))
+        assert not null
```

### Comparing `soil-0.9.7/soil/agents/__init__.py` & `soil-1.0.0rc1/soil/agents/fsm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,166 +1,148 @@
-# networkStatus = {}  # Dict that will contain the status of every agent in the network
-# sentimentCorrelationNodeArray = []
-# for x in range(0, settings.network_params["number_of_nodes"]):
-#     sentimentCorrelationNodeArray.append({'id': x})
-# Initialize agent states. Let's assume everyone is normal.
-    
-
-import nxsim
-from collections import OrderedDict
-from copy import deepcopy
-import json
-
-from functools import wraps
-
-
-agent_types = {}
-
-
-class MetaAgent(type):
-    def __init__(cls, name, bases, nmspc):
-        super(MetaAgent, cls).__init__(name, bases, nmspc)
-        agent_types[name] = cls
-
-
-class BaseAgent(nxsim.BaseAgent, metaclass=MetaAgent):
-    """
-    A special simpy BaseAgent that keeps track of its state history.
-    """
-
-    def __init__(self, *args, **kwargs):
-        self._history = OrderedDict()
-        self._neighbors = None
-        super().__init__(*args, **kwargs)
-
-    def __getitem__(self, key):
-        if isinstance(key, tuple):
-            k, t_step = key
-            if k is not None:
-                if t_step is not None:
-                    return self._history[t_step][k]
-                else:
-                    return {tt: tv.get(k, None) for tt, tv in self._history.items()}
-            else:
-                return self._history[t_step]
-        return self.state[key]
-
-    def __setitem__(self, key, value):
-        self.state[key] = value
-
-    def save_state(self):
-        self._history[self.now] = deepcopy(self.state)
-
-    @property
-    def now(self):
-        try:
-            return self.env.now
-        except AttributeError:
-            # No environment
-            return None
-
-    def run(self):
-        while True:
-            res = self.step()
-            yield res or self.env.timeout(self.env.interval)
-
-    def step(self):
-        pass
+from . import MetaAgent, BaseAgent
+from ..time import Delta
 
-    def to_json(self):
-        return json.dumps(self._history)
+from functools import partial, wraps
+import inspect
 
 
-class NetworkAgent(BaseAgent, nxsim.BaseNetworkAgent):
-
-    def count_agents(self, state_id=None, limit_neighbors=False):
-        if limit_neighbors:
-            agents = self.global_topology.neighbors(self.id)
-        else:
-            agents = self.global_topology.nodes()
-        count = 0
-        for agent in agents:
-            if state_id and state_id != self.global_topology.node[agent]['agent'].state['id']:
-                continue
-            count += 1
-        return count
-
-    def count_neighboring_agents(self, state_id=None):
-        return self.count_agents(state_id, limit_neighbors=True)
-
-
-def state(func):
-
-    @wraps(func)
-    def func_wrapper(self):
-        when = None
-        next_state = func(self)
-        try:
-            next_state, when = next_state
-        except TypeError:
-            pass
-        if next_state:
-            try:
-                self.state['id'] = next_state.id
-            except AttributeError:
-                raise NotImplemented('State id %s is not valid.' % next_state)
-        return when
-
-    func_wrapper.id = func.__name__
-    func_wrapper.is_default = False
-    return func_wrapper
+def state(name=None, default=False):
+    def decorator(func, name=None):
+        """
+        A state function should return either a state id, or a tuple (state_id, when)
+        The default value for state_id is the current state id.
+        The default value for when is the interval defined in the environment.
+        """
+        if inspect.isgeneratorfunction(func):
+            orig_func = func
+
+            @wraps(func)
+            def func(self):
+                while True:
+                    if not self._coroutine:
+                        self._coroutine = orig_func(self)
+
+                    try:
+                        if self._last_except:
+                            n = self._coroutine.throw(self._last_except)
+                        else:
+                            n = self._coroutine.send(self._last_return)
+                        if n:
+                            return None, n
+                        return n
+                    except StopIteration as ex:
+                        self._coroutine = None
+                        next_state = ex.value
+                        if next_state is not None:
+                            self._set_state(next_state)
+                        return next_state
+                    finally:
+                        self._last_return = None
+                        self._last_except = None
+
+        func.id = name or func.__name__
+        func.is_default = default
+        return func
+
+    if callable(name):
+        return decorator(name)
+    else:
+        return partial(decorator, name=name)
 
 
 def default_state(func):
     func.is_default = True
     return func
 
 
 class MetaFSM(MetaAgent):
-    def __init__(cls, name, bases, nmspc):
-        super(MetaFSM, cls).__init__(name, bases, nmspc)
+    def __new__(mcls, name, bases, namespace):
         states = {}
         # Re-use states from inherited classes
         default_state = None
         for i in bases:
             if isinstance(i, MetaFSM):
-                for state_id, state in i.states.items():
+                for state_id, state in i._states.items():
                     if state.is_default:
                         default_state = state
                     states[state_id] = state
 
         # Add new states
-        for name, func in nmspc.items():
-            if hasattr(func, 'id'):
+        for attr, func in namespace.items():
+            if hasattr(func, "id"):
                 if func.is_default:
                     default_state = func
                 states[func.id] = func
-        cls.default_state = default_state
-        cls.states = states
+
+        namespace.update(
+            {
+                "_default_state": default_state,
+                "_states": states,
+            }
+        )
+
+        return super(MetaFSM, mcls).__new__(
+            mcls=mcls, name=name, bases=bases, namespace=namespace
+        )
 
 
 class FSM(BaseAgent, metaclass=MetaFSM):
-    def __init__(self, *args, **kwargs):
-        super(FSM, self).__init__(*args, **kwargs)
-        if 'id' not in self.state:
-            self.state['id'] = self.default_state.id
+    def __init__(self, init=True, **kwargs):
+        super().__init__(**kwargs, init=False)
+        if not hasattr(self, "state_id"):
+            if not self._default_state:
+                raise ValueError(
+                    "No default state specified for {}".format(self.unique_id)
+                )
+            self.state_id = self._default_state.id
+
+        self._coroutine = None
+        self.default_interval = Delta(self.model.interval)
+        self._set_state(self.state_id)
+        if init:
+            self.init()
+
+    @classmethod
+    def states(cls):
+        return list(cls._states.keys())
 
     def step(self):
-        if 'id' in self.state:
-            next_state = self.state['id']
-        elif self.default_state:
-            next_state = self.default_state.id
-        else:
-            raise Exception('{} has no valid state id or default state'.format(self))
-        if next_state not in self.states:
-            raise Exception('{} is not a valid id for {}'.format(next_state, self))
-        self.states[next_state](self)
-
-
-from .BassModel import *
-from .BigMarketModel import *
-from .IndependentCascadeModel import *
-from .ModelM2 import *
-from .SentimentCorrelationModel import *
-from .SISaModel import *
-from .CounterModel import *
-from .DrawingAgent import *
+        self.debug(f"Agent {self.unique_id} @ state {self.state_id}")
+
+        self._check_alive()
+        next_state = self._states[self.state_id](self)
+
+        when = None
+        try:
+            next_state, *when = next_state
+            if not when:
+                when = None
+            elif len(when) == 1:
+                when = when[0]
+            else:
+                raise ValueError(
+                    "Too many values returned. Only state (and time) allowed"
+                )
+        except TypeError:
+            pass
+
+        if next_state is not None:
+            self._set_state(next_state)
+
+        return when or self.default_interval
+
+    def _set_state(self, state, when=None):
+        if hasattr(state, "id"):
+            state = state.id
+        if state not in self._states:
+            raise ValueError("{} is not a valid state".format(state))
+        self.state_id = state
+        if when is not None:
+            self.model.schedule.add(self, when=when)
+        return state
+
+    def die(self, *args, **kwargs):
+        return self.dead, super().die(*args, **kwargs)
+
+    @state
+    def dead(self):
+        return self.die()
```

