# Comparing `tmp/aprilbox-1.0.0b2.tar.gz` & `tmp/aprilbox-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aprilbox-1.0.0b2.tar", last modified: Wed Apr 19 10:11:51 2023, max compression
+gzip compressed data, was "dist/aprilbox-1.0.0b4.tar", last modified: Thu Apr 20 09:58:13 2023, max compression
```

## Comparing `aprilbox-1.0.0b2.tar` & `aprilbox-1.0.0b4.tar`

### file list

```diff
@@ -1,84 +1,83 @@
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1587 2022-12-22 10:24:41.000000 aprilbox-1.0.0b2/LICENSE.txt
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      963 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/PKG-INFO
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      706 2023-04-19 06:14:13.000000 aprilbox-1.0.0b2/README.md
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      526 2023-04-19 06:33:58.000000 aprilbox-1.0.0b2/aprilbox/__init__.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      314 2023-04-19 06:34:21.000000 aprilbox-1.0.0b2/aprilbox/ai/__init__.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      505 2023-04-19 06:17:32.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/__init__.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/activation/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      320 2023-04-19 09:29:33.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/activation/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2991 2023-04-19 09:29:38.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/activation/acon.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2302 2023-04-19 09:29:44.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/activation/smu.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      424 2023-04-10 06:04:03.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     7552 2023-04-19 09:30:19.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/lstm.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3084 2023-04-19 09:30:19.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/resnet.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4201 2023-04-19 09:30:19.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/unet.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)    10459 2023-04-19 09:30:19.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/vit.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/benchmark/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      328 2023-04-10 06:04:30.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/benchmark/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)    16473 2023-04-19 09:30:19.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/benchmark/scinet.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1509 2023-04-19 07:01:02.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/benchmark/simvp.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      497 2023-04-19 09:30:59.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/__init__.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      426 2023-04-19 09:30:27.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1558 2023-04-19 09:30:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/lka.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     7114 2023-04-19 09:30:50.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/psa.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      852 2023-03-31 08:08:57.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/simple.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3763 2023-04-19 09:30:56.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/split.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1236 2023-04-10 06:05:56.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/cca.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3328 2023-04-19 06:44:54.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/conv.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4526 2023-04-19 06:45:16.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/inception.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4186 2023-04-19 09:31:05.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/block/memory.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      573 2023-04-19 09:31:10.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1172 2023-04-19 09:31:21.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/dice.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4899 2023-04-19 07:02:27.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/efl.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2683 2023-04-19 07:28:33.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/loss.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1506 2023-04-10 05:47:56.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/rmse.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3807 2023-04-17 03:00:51.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/seesaw.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3762 2023-04-19 09:31:21.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/ssim.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1386 2023-04-10 05:58:58.000000 aprilbox-1.0.0b2/aprilbox/ai/dl/loss/ts.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/ml/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      231 2023-04-19 07:03:03.000000 aprilbox-1.0.0b2/aprilbox/ai/ml/__init__.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/ai/tools/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      240 2023-04-19 07:26:53.000000 aprilbox-1.0.0b2/aprilbox/ai/tools/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     7260 2023-04-19 07:29:05.000000 aprilbox-1.0.0b2/aprilbox/ai/tools/base.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2800 2023-04-19 07:27:43.000000 aprilbox-1.0.0b2/aprilbox/ai/tools/config.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2931 2023-04-19 07:33:34.000000 aprilbox-1.0.0b2/aprilbox/ai/tools/weight.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/data/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      332 2023-04-19 09:28:00.000000 aprilbox-1.0.0b2/aprilbox/data/__init__.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/data/met/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      332 2023-04-19 09:27:17.000000 aprilbox-1.0.0b2/aprilbox/data/met/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2578 2023-04-19 09:24:47.000000 aprilbox-1.0.0b2/aprilbox/data/met/constant.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)    11518 2023-04-19 07:45:35.000000 aprilbox-1.0.0b2/aprilbox/data/met/loader.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/data/preprocess/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      235 2023-04-19 09:27:28.000000 aprilbox-1.0.0b2/aprilbox/data/preprocess/__init__.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/eval/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      233 2023-04-19 06:34:40.000000 aprilbox-1.0.0b2/aprilbox/eval/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2379 2023-04-19 09:22:36.000000 aprilbox-1.0.0b2/aprilbox/types.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/utils/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      443 2023-04-19 06:52:00.000000 aprilbox-1.0.0b2/aprilbox/utils/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     6810 2023-04-19 06:48:01.000000 aprilbox-1.0.0b2/aprilbox/utils/interpolate.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/utils/met/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      332 2023-04-19 07:36:09.000000 aprilbox-1.0.0b2/aprilbox/utils/met/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4054 2023-04-19 07:35:45.000000 aprilbox-1.0.0b2/aprilbox/utils/met/distance.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3835 2023-04-19 07:35:45.000000 aprilbox-1.0.0b2/aprilbox/utils/met/factor.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3767 2023-04-19 07:44:00.000000 aprilbox-1.0.0b2/aprilbox/utils/path.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2867 2023-04-19 09:32:01.000000 aprilbox-1.0.0b2/aprilbox/utils/pool.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox/vis/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      287 2023-04-19 06:36:23.000000 aprilbox-1.0.0b2/aprilbox/vis/__init__.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      532 2023-04-19 06:20:56.000000 aprilbox-1.0.0b2/aprilbox/vis/base.py
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1454 2023-04-19 06:37:27.000000 aprilbox-1.0.0b2/aprilbox/vis/precipitation.py
-drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox.egg-info/
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      963 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox.egg-info/PKG-INFO
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1833 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox.egg-info/SOURCES.txt
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)        1 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox.egg-info/dependency_links.txt
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      140 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox.egg-info/requires.txt
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)        9 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/aprilbox.egg-info/top_level.txt
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      423 2023-04-19 10:11:51.000000 aprilbox-1.0.0b2/setup.cfg
--rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      494 2023-04-19 09:46:04.000000 aprilbox-1.0.0b2/setup.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:13.000000 aprilbox-1.0.0b4/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1216 2023-04-20 09:58:13.000000 aprilbox-1.0.0b4/PKG-INFO
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      710 2023-04-19 09:38:51.000000 aprilbox-1.0.0b4/README.md
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      526 2023-04-19 06:33:58.000000 aprilbox-1.0.0b4/aprilbox/__init__.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/ai/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      314 2023-04-19 06:34:21.000000 aprilbox-1.0.0b4/aprilbox/ai/__init__.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      505 2023-04-19 06:17:32.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/__init__.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/activation/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      320 2023-04-19 09:29:33.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/activation/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2991 2023-04-19 09:29:38.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/activation/acon.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2302 2023-04-19 09:29:44.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/activation/smu.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/backbone/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      424 2023-04-10 06:04:03.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/backbone/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     7552 2023-04-19 09:30:19.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/backbone/lstm.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3084 2023-04-19 09:30:19.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/backbone/resnet.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4201 2023-04-19 09:30:19.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/backbone/unet.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)    10459 2023-04-19 09:30:19.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/backbone/vit.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/benchmark/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      328 2023-04-10 06:04:30.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/benchmark/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)    16473 2023-04-19 09:30:19.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/benchmark/scinet.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1509 2023-04-19 07:01:02.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/benchmark/simvp.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/block/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      497 2023-04-19 09:30:59.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/block/__init__.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/block/attention/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      426 2023-04-19 09:30:27.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/block/attention/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1502 2023-04-20 09:36:06.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/block/attention/lka.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     7114 2023-04-19 09:30:50.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/block/attention/psa.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      852 2023-03-31 08:08:57.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/block/attention/simple.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3763 2023-04-19 09:30:56.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/block/attention/split.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1236 2023-04-10 06:05:56.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/block/cca.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3328 2023-04-19 06:44:54.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/block/conv.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4526 2023-04-19 06:45:16.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/block/inception.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4186 2023-04-19 09:31:05.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/block/memory.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/loss/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      524 2023-04-20 09:53:55.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/loss/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1172 2023-04-19 09:31:21.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/loss/dice.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     6349 2023-04-20 09:22:47.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/loss/focal.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3193 2023-04-20 09:34:34.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/loss/loss.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1506 2023-04-10 05:47:56.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/loss/rmse.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3657 2023-04-20 09:29:26.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/loss/seesaw.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3762 2023-04-19 09:31:21.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/loss/ssim.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1390 2023-04-20 09:33:56.000000 aprilbox-1.0.0b4/aprilbox/ai/dl/loss/ts.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/ai/ml/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      231 2023-04-19 07:03:03.000000 aprilbox-1.0.0b4/aprilbox/ai/ml/__init__.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/ai/tools/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      240 2023-04-19 07:26:53.000000 aprilbox-1.0.0b4/aprilbox/ai/tools/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     7312 2023-04-20 09:46:20.000000 aprilbox-1.0.0b4/aprilbox/ai/tools/base.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2807 2023-04-20 09:46:53.000000 aprilbox-1.0.0b4/aprilbox/ai/tools/config.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2931 2023-04-19 07:33:34.000000 aprilbox-1.0.0b4/aprilbox/ai/tools/weight.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/data/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      332 2023-04-19 09:28:00.000000 aprilbox-1.0.0b4/aprilbox/data/__init__.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/data/met/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      332 2023-04-19 09:27:17.000000 aprilbox-1.0.0b4/aprilbox/data/met/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3234 2023-04-19 10:24:20.000000 aprilbox-1.0.0b4/aprilbox/data/met/constant.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)    10830 2023-04-19 10:25:17.000000 aprilbox-1.0.0b4/aprilbox/data/met/loader.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/data/preprocess/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      235 2023-04-19 09:27:28.000000 aprilbox-1.0.0b4/aprilbox/data/preprocess/__init__.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/eval/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      233 2023-04-19 06:34:40.000000 aprilbox-1.0.0b4/aprilbox/eval/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2388 2023-04-20 09:51:46.000000 aprilbox-1.0.0b4/aprilbox/types.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox/utils/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      437 2023-04-20 09:52:57.000000 aprilbox-1.0.0b4/aprilbox/utils/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     6810 2023-04-19 06:48:01.000000 aprilbox-1.0.0b4/aprilbox/utils/interpolate.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:13.000000 aprilbox-1.0.0b4/aprilbox/utils/met/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      332 2023-04-19 07:36:09.000000 aprilbox-1.0.0b4/aprilbox/utils/met/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     4066 2023-04-20 09:50:38.000000 aprilbox-1.0.0b4/aprilbox/utils/met/distance.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3849 2023-04-20 09:51:11.000000 aprilbox-1.0.0b4/aprilbox/utils/met/factor.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     3840 2023-04-20 09:52:40.000000 aprilbox-1.0.0b4/aprilbox/utils/path.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     2867 2023-04-19 09:32:01.000000 aprilbox-1.0.0b4/aprilbox/utils/pool.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:13.000000 aprilbox-1.0.0b4/aprilbox/vis/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      287 2023-04-19 06:36:23.000000 aprilbox-1.0.0b4/aprilbox/vis/__init__.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      532 2023-04-19 06:20:56.000000 aprilbox-1.0.0b4/aprilbox/vis/base.py
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1454 2023-04-19 06:37:27.000000 aprilbox-1.0.0b4/aprilbox/vis/precipitation.py
+drwxrwxr-x   0 fanghao  (100054) fanghao  (100054)        0 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox.egg-info/
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1216 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox.egg-info/PKG-INFO
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)     1823 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)        1 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      166 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox.egg-info/requires.txt
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)        9 2023-04-20 09:58:12.000000 aprilbox-1.0.0b4/aprilbox.egg-info/top_level.txt
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      440 2023-04-20 09:58:13.000000 aprilbox-1.0.0b4/setup.cfg
+-rw-rw-r--   0 fanghao  (100054) fanghao  (100054)      494 2023-04-20 09:38:19.000000 aprilbox-1.0.0b4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `aprilbox-1.0.0b2/PKG-INFO` & `aprilbox-1.0.0b4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 Metadata-Version: 2.1
 Name: aprilbox
-Version: 1.0.0b2
+Version: 1.0.0b4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Fang Linwanghao
 Author-email: fanglwh@outlook.com
 License: BSD-3-Clause
+Description: AprilBox, is a personal development toolkit primarily used for developing and researching 
+        artificial intelligence-related content. It also includes various other tools, 
+        including but not limited to meteorological indicators calculation, verification and evaluation calculation,
+        and common quantitative visualization.
+        
+        # Content
+           * [Install]()
+           * [Document]()
+           * [Usage]()
+           * [License]()
+           * [Support]()
+           * [Developers]()
+        
+        
+        ## [Document]()
+        
+        
+        ## [Install]()
+        
+        
+        ## [Usage]()
+        
+        ## [LICENSE]()
+        
+        This project is licensed under the BSD 3-Clause License - see the [LICENSE](/LICENSE.txt) file for details.
+        
+        ## [Support]()
+        
+        Give a ⭐️ if this project helped you!
+        
+        
+        ## [Developer]()
+        * [Linwanghao, Fang]()
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-AprilBox, is a personal development toolkit primarily used for developing and researching 
-artificial intelligence-related content. It also includes various other tools, 
-including but not limited to meteorological indicators calculation, verification and evaluation calculation,
-and common quantitative visualization.
-
-# Content
-   * [Install]()
-   * [Document]()
-   * [Usage]()
-   * [License]()
-   * [Support]()
-   * [Developers]()
-
-
-## [Document]()
-
-
-## [Install]()
-
-
-## [Usage]()
-
-## [LICENSE]()
-
-This project is licensed under the BSD 3-Clause License - see the [LICENSE](/LICENSE) file for details.
-
-## [Support]()
-
-Give a ⭐️ if this project helped you!
-
-
-## [Developer]()
-* [Linwanghao, Fang]()
-
-
```

### Comparing `aprilbox-1.0.0b2/README.md` & `aprilbox-1.0.0b4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ## [Install]()
 
 
 ## [Usage]()
 
 ## [LICENSE]()
 
-This project is licensed under the BSD 3-Clause License - see the [LICENSE](/LICENSE) file for details.
+This project is licensed under the BSD 3-Clause License - see the [LICENSE](/LICENSE.txt) file for details.
 
 ## [Support]()
 
 Give a ⭐️ if this project helped you!
 
 
 ## [Developer]()
```

### Comparing `aprilbox-1.0.0b2/aprilbox/__init__.py` & `aprilbox-1.0.0b4/aprilbox/__init__.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/activation/acon.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/activation/acon.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/activation/smu.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/activation/smu.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/lstm.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/backbone/lstm.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/resnet.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/unet.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/backbone/unet.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/backbone/vit.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/benchmark/scinet.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/benchmark/scinet.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/benchmark/simvp.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/benchmark/simvp.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/lka.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/block/attention/lka.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 
 import torch.nn as nn
 
 
 class LKA(nn.Module):
     """Large Kernel Attention(LKA)
 
-    References:
-        [1]Guo, M. H., Lu, C. Z., Liu, Z. N., Cheng, M. M., & Hu, S. M. (2022). Visual attention network. arXiv preprint arXiv:2202.09741.
+    Notes:
+        Refers to `Visual attention network
+        <https://arxiv.org/abs/2202.09741>
     """
 
     def __init__(self, in_channel: int):
         super(LKA, self).__init__()
 
         self.dw_conv = nn.Conv2d(in_channel, in_channel, kernel_size=5, padding=2, groups=in_channel)
         self.dw_d_conv = nn.Conv2d(in_channel, in_channel, kernel_size=7, stride=1, padding=9, dilation=3, groups=in_channel)
```

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/psa.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/block/attention/psa.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/simple.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/block/attention/simple.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/block/attention/split.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/block/attention/split.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/block/cca.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/block/cca.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/block/conv.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/block/conv.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/block/inception.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/block/inception.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/block/memory.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/block/memory.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/loss/dice.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/loss/dice.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/loss/loss.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/loss/loss.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 __all__ = ["BaseLoss", "GeneralizedCrossEntropyLoss"]
 
 from abc import ABC
 from typing import Optional
 
+import torch
 from torch import nn, Tensor
 
 
 class BaseLoss(nn.Module):
     """
 
     Args:
@@ -77,8 +78,20 @@
                  ignore_index: int = -1
                  ) -> None:
         BaseLoss.__init__(self,
                           name=name,
                           reduction=reduction,
                           loss_weight=loss_weight)
         self.activation_type = activation_type
-        self.ignore_index = ignore_index
+        self.ignore_index = ignore_index
+
+    @staticmethod
+    def flatten(x: Tensor, dim: int = 1) -> Tensor:
+        if x.dim() > 2:
+            # shape like B * Num_class * ...
+            return torch.flatten(torch.flatten(x, start_dim=dim + 1, end_dim=-1).permute(0, 2, 1), start_dim=0, end_dim=1)
+        elif x.dim() == 2:
+            # shape like N * Num_class
+            return x
+        else:
+            # shape is not supported
+            raise ValueError("CrossEntropyLoss is expected input N-dims input.")
```

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/loss/rmse.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/loss/rmse.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/loss/seesaw.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/loss/seesaw.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 from torch import Tensor
 import torch.nn.functional as F
 
 from .loss import GeneralizedCrossEntropyLoss
 
 
 class SeesawLoss(GeneralizedCrossEntropyLoss):
-    """
-    Implementation of seesaw loss.
-    Refers to `Seesaw Loss for Long-Tailed Instance Segmentation (CVPR 2021)
-    <https://arxiv.org/abs/2008.10032>
+    """Implementation of seesaw loss.
+
+    Notes:
+        Refers to `Seesaw Loss for Long-Tailed Instance Segmentation (CVPR 2021)
+        <https://arxiv.org/abs/2008.10032>
 
     Args:
         num_classes: The number of classes. Default: ``1000``.
         p: The ``p`` in the mitigation factor. Default: ``0.8``.
         q: The ``q`` in the compensation factor. Default: ``2.0``.
         eps: The min divisor to smooth the computation of compensation factor. Default: ``1e-2``.
         name: Name of the loss function. Default: ``See_saw_loss``.
@@ -60,18 +61,15 @@
         # cumulative samples for each category
         self.register_buffer("accumulated", torch.zeros(self.num_classes, dtype=torch.float))
 
     def forward(self, input: Tensor, target: Tensor, **kwargs) -> Tensor:
         if self.accumulated.device != input.device:
             self.accumulated = self.accumulated.cuda(input.device)
 
-        if input.dim() > 3:
-            input = torch.flatten(torch.flatten(input, start_dim=2, end_dim=-1).permute(0, 2, 1), start_dim=0, end_dim=-2)
-        else:
-            input = torch.flatten(input, start_dim=0, end_dim=-2)
+        input = self.flatten(input)
         target = torch.flatten(target)
         # accumulate the samples for each category
         for cls in range(self.num_classes):
             self.accumulated[cls] += torch.sum(target == cls)
 
         one_hot_target = F.one_hot(target, self.num_classes)
         seesaw_weights = input.new_ones(one_hot_target.size())
@@ -90,9 +88,9 @@
             self_scores = scores[torch.arange(0, len(scores)).to(scores.device).long(), target.long()]
             score_matrix = scores / self_scores[:, None].clamp(min=self.eps)
             index = (score_matrix > 1.0).float()
             compensation_factor = score_matrix.pow(self.q) * index + (1 - index)
             seesaw_weights = seesaw_weights * compensation_factor
 
         input = input + (seesaw_weights.log() * (1 - one_hot_target))
-        loss = F.cross_entropy(input, target, reduction="none")
+        loss = F.cross_entropy(input, target, ignore_index=self.ignore_index, reduction="none")
         return self._reduce(loss)
```

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/loss/ssim.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/loss/ssim.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/dl/loss/ts.py` & `aprilbox-1.0.0b4/aprilbox/ai/dl/loss/ts.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 ----------------------------------
 Author     : April
 Contact    : fanglwh@outlook.com
 """
 
 __all__ = ["TSLoss"]
 
+
 import torch
 from torch import Tensor
 
 from .loss import BaseLoss
 
+
 class TSLoss(BaseLoss):
     """
 
     Args:
         threshold: The threshold for classify. Default: ``0.1``.
         name: Name of the loss function. Default: ``TSLoss``.
         loss_weight: Loss weight.  Default: ``1.0``.
```

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/tools/base.py` & `aprilbox-1.0.0b4/aprilbox/ai/tools/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,49 +13,57 @@
 __all__ = ["BaseDataLoader", "BaseExp"]
 
 from abc import ABCMeta, abstractmethod
 from datetime import datetime, timedelta
 import logging
 from pathlib import Path
 import re
-from typing import Union, Tuple, List, Optional
+from typing import Union, Optional, Tuple
 
 import numpy as np
 import pandas as pd
 import torch
 from torch import nn, Tensor
 from torch.utils.data import Dataset as TorchDataset
 
+from .config import NetConfig
+
 
 class BaseDataLoader(TorchDataset, metaclass=ABCMeta):
-    """
+    """ Base data loader for network.
 
     Args:
         samples: The list of the samples.
         mode: default `train`, Optional in `train`, `test` and `eval`. The mode of the DataLoader.
     """
 
-    def __init__(self, samples: Union[list, np.ndarray, pd.DataFrame],
-                 mode: str = "train") -> None:
+    def __init__(self,
+                 samples: Union[list, np.ndarray, pd.DataFrame],
+                 mode: str = "train"
+                 ) -> None:
         super(BaseDataLoader, self).__init__()
         self.samples = samples
         if mode in ["train", "test", "eval"]:
             self.mode = mode
         else:
             raise ValueError(f"Unexpected input of the \"mode\": {mode}, please check it!")
 
     @abstractmethod
-    def __getitem__(self, index: int):
+    def __getitem__(self,
+                    index: int):
         pass
 
     def __len__(self) -> int:
         return len(self.samples)
 
     @staticmethod
-    def merge_file(time: datetime, lead_time: Union[timedelta, None], file: str) -> str:
+    def merge_file(time: datetime,
+                   lead_time: Optional[timedelta],
+                   file: str
+                   ) -> str:
         """ Merge the file with time and lead time.
 
         The time is report time while the lead time is not None. On the contrary, the time is live time while the lead
         time is None.
 
         Args:
             time: The report time or the live time
@@ -73,38 +81,31 @@
             file_split_1 = time.strftime("_".join(file.split("_")[:-1]))
             file_split_2 = (time + lead_time).strftime(file.split("_")[-1])
             file = file_split_1 + "_" + file_split_2
             return file
 
 
 class BaseExp(metaclass=ABCMeta):
-    """ The base class of experiment.
-
-    Attributes:
-        net(nn.Module): The neural network
-        optimizer(Union[None, torch.optim.Optimizer]): The optimizer of the neural network
-        cost_func(dict): The cost functions for training
-        config(NetConfig): The configurations of the neural network
-        net_dir(str): The directory of the pretrained neural network or the saving
-        log_dir(str): The directory of the logs.
-        logger(logging.Logger): The logger for the neural network
+    """ Base experiment.
 
     Args:
         net: The optimizer of the neural network
         cost_func: The cost functions for training
         config: The configurations of the neural network
         net_dir: The directory of the pretrained neural network or the saving
         log_dir: The directory of the logger
     """
 
-    def __init__(self, net: nn.Module,
+    def __init__(self,
+                 net: nn.Module,
                  cost_func: dict,
                  config: NetConfig = NetConfig,
                  net_dir: str = "./model/",
-                 log_dir: str = "./logs/") -> None:
+                 log_dir: str = "./logs/"
+                 ) -> None:
         self.net = net
         self.name = self.net.__name__
         self.optimizer = None
         self.cost_func = cost_func
         self.config = config
         self.net_dir = Path(net_dir)
         self.net_dir.mkdir(parents=True, exist_ok=True)
@@ -124,39 +125,41 @@
         while log_path.exists():
             log_path = log_path.parent.joinpath(f"logs_{i}.log")
             i += 1
         logger.addHandler(logging.FileHandler(str(log_path), mode="w"))
         logger.setLevel(level=logging.INFO)
         return logger
 
-    def calc_loss(self, truth: torch.Tensor,
-                  test: torch.Tensor,
-                  keys: list = None):
+    def calc_loss(self,
+                  target: torch.Tensor,
+                  input: torch.Tensor,
+                  keys: list = None
+                  ) -> Tuple[dict, Tensor]:
         """Calculate loss for training.
 
         Args:
-            truth:
-            test:
-            keys:
-
-        Returns:
-
+            target: the target, which is label value.
+            input: the result from neural network.
+            keys: keys of cost function.
         """
         if keys is None:
             keys = self.cost_func.keys()
 
-        loss_item, loss = dict(), 0
+        loss_item, loss = dict(), torch.Tensor(0)
         for key, func in self.cost_func.items():
             if key in keys:
-                tmp = func[0](input=test, target=truth)
+                tmp = func[0](input=input, target=target)
                 loss += tmp * func[1]
                 loss_item[key] = tmp
         return loss_item, loss
 
-    def load_net(self, reload: bool = False, idx: Optional[int] = None) -> int:
+    def load_net(self,
+                 reload: bool = False,
+                 idx: Optional[int] = None
+                 ) -> int:
         """ Load the neural network
 
         Args:
             reload: default ``False``. Whether reload the neural network parameters, or not.
             idx:  default ``None``. The ID of the pretrained neural network
 
         Returns:
@@ -181,26 +184,30 @@
                 point, idx = _load(self.net_dir)
             self.logger.info("-" * 15 + f">Reload No.{idx:03d} epoch network...")
             self.net.load_state_dict(point["model_states"])
         else:
             self.logger.info("-" * 15 + ">Initiating new network...")
             idx = 0
             point = dict()
+        # todo: change into DistributedDataParallel
         self.net = nn.DataParallel(self.net, device_ids=self.config.DEVICES_IDS)
         _parameters = [p for p in self.net.parameters() if p.requires_grad]
         self.optimizer = torch.optim.Adam(self.net.parameters(), lr=self.config.LR, weight_decay=1e-5)
         if reload:
             self.optimizer.load_state_dict(point["optimizer_states"])
         self.logger.info(f">>>{datetime.now().strftime('%Y-%m-%d %H:%M:%S')} | Net has been loaded!\n")
         return idx
 
-    def save_net(self, epoch: int, **kwargs) -> None:
+    def save_net(self,
+                 epoch: int,
+                 **kwargs
+                 ) -> None:
         """Saving states of the neural network
 
         Args:
-            epoch:
+            epoch: epoch number of training.
 
         """
         path = self.net_dir.joinpath(f"model_{epoch:03d}.pkl")
         # Saving states of the network.
         torch.save(dict(epoch=epoch, **kwargs), path)
         self.logger.info(f">>>{datetime.now().strftime('%Y-%m-%d %H:%M:%S')} | save path: {path}\n")
```

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/tools/config.py` & `aprilbox-1.0.0b4/aprilbox/ai/tools/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 ----------------------------------
 Author     : April
 Contact    : fanglwh@outlook.com
 """
 
 __all__ = ["NetConfig"]
 
-from typing import Union, List
+from typing import Union, List, Tuple
 
 
-def Singleton(cls):
+def singleton(cls):
     _instance = {}
 
     def _singleton(*args, **kwargs):
         if cls not in _instance:
             _instance[cls] = cls(*args, **kwargs)
         return _instance[cls]
 
     return _singleton
 
 
-@Singleton
+@singleton
 class NetConfig(object):
     """The basic configuration for the neural network.
 
     Args:
         batch: The batch size of the input data.
         devices_ids: The ids of the GPU devices.
         shape: The shape of the input data.
```

### Comparing `aprilbox-1.0.0b2/aprilbox/ai/tools/weight.py` & `aprilbox-1.0.0b4/aprilbox/ai/tools/weight.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/data/met/loader.py` & `aprilbox-1.0.0b4/aprilbox/data/met/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 Author     : April
 Contact    : fanglwh@outlook.com
 """
 
 __all__ = ["Extend", "DataReader"]
 
 
-import glob
 from pathlib import Path
-import re
 from typing import Optional, Union
 
 from netCDF4 import Dataset
 import numpy as np
+import pandas as pd
 import pygrib
 
+from .constant import GRIB2DICT
+from ...types import _NUMBER
+
 
 class Extend(object):
     """ The extend information of location.
 
     Includes `slon`, `elon`, `slat`, elat`, `error` and `plev`.
 
     Attributes:
@@ -41,15 +43,15 @@
         elat: end latitude.
         slon: start longitude.
         elon: end longitude.
         error: Default ``0.05``.The error of the coordination.
         plev: Default ``None``.The height of pressure height.
     """
 
-    def __init__(self, slat: U_FIN, elat: U_FIN, slon: U_FIN, elon: U_FIN, error: float = 0.05,
+    def __init__(self, slat: _NUMBER, elat: _NUMBER, slon: _NUMBER, elon: _NUMBER, error: float = 0.05,
                  plev: Union[list, float, int, None] = None):
         self._slat = slat
         self._elat = elat
         self._slon = slon
         self._elon = elon
         self._error = error
         self._plev = plev
@@ -86,28 +88,16 @@
             raise ValueError(f'>>>Expected "plev" is the U_FIN or list, but got {self._plev}!')
 
 
 class DataReader(object):
     """ Reader of grid data.
 
     Read the data from key words like :obj:`path`, :obj:`vnames`, :obj:`extent` and so on.
-
-    Attributes:
-        GRIBDICT(dict): The default dictionary of grib2 for selecting variables.
     """
-
-    GRIBDICT = dict(PRE_1h=dict(parameterName="Total precipitation"),
-                    rain=dict(parameterName="Total precipitation", level=0, stepType="instant"),
-                    tp=dict(parameterName="Total precipitation", level=0, stepType="accum"),
-                    tem=dict(parameterName="Temperature", level=2, stepType="instant"),
-                    sp=dict(parameterName="Pressure", level=0, stepType="instant"),
-                    rhu=dict(parameterName="Relative humidity", level=2, stepType="instant"),
-                    u=dict(parameterName="u-component of wind", level=10, stepType="instant"),
-                    v=dict(parameterName="v-component of wind", level=10, stepType="instant"),
-                    )
+    GRIBDICT = GRIB2DICT
 
     @classmethod
     def load(cls, path: str or Path, vnames: list, extend: dict, acc: int = 2, gribdict: Optional[dict] = None,
              name_lat: str = "Lat", name_lon: str = "Lon", surface: bool = True, name_height: str = "Plev") -> dict:
         """ Load grid data.
 
         Read data within key words including path, vnames, locational extend, accuracy, and so on.
@@ -140,15 +130,16 @@
 
         error = pow(10, -1 * acc) / 2
         assert isinstance(extend, dict), ValueError("请输入经纬度落区！")
         extend = Extend(error=error, **extend)
 
         # 若基类GRIB2字典表不包含提取变量的关键信息，则传入更新
         if isinstance(gribdict, dict):
-            cls.GRIBDICT.update(gribdict)
+            for key, value in gribdict.items():
+                setattr(cls.GRIBDICT, key, value)
 
         # 选择格点数据读取方式
         ext = p.suffix.lower()
         if ext == ".nc":
             return cls.load_nc(path, vnames, extend=extend, name_lat=name_lat, name_lon=name_lon, surface=surface,
                                name_height=name_height)
         elif ext in [".grb2", ".bin"]:
@@ -216,15 +207,15 @@
 
         if not surface:
             # todo GRIB2 格式数据暂不支持3-D 格点读取
             raise NotImplementedError(f"Loading upar GRIB2 data have not implemented yet!")
         cntr = dict()
         with pygrib.open(str(path)) as messages:
             for vname in vnames:
-                message = messages.select(**cls.GRIBDICT[vname])
+                message = messages.select(**getattr(cls.GRIBDICT, vname))
                 if len(message) == 1:
                     message = message[0]
                 elif len(message) > 1:
                     message = message[0]
                     Warning(f">>> GRIB DATA have more than one message of {vname}!!!")
                 else:
                     Warning(f">>> GRIB DATA have no one message of {vname}!!!")
```

### Comparing `aprilbox-1.0.0b2/aprilbox/types.py` & `aprilbox-1.0.0b4/aprilbox/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 Contact    : fanglwh@outlook.com
 """
 
 __all__ = ["_NUMBER", "_NNUMBER",
            "_TNN", "_TII",
 
            "ndarray", "Optional", "Union", "Tuple",
-           "NetConfig",
            "ContingencyTable", "Property"]
 
-
+from collections import namedtuple
 from typing import Optional, Union, Tuple
 
 from numpy import ndarray
 
 
 _NNUMBER = Union[None, ndarray, float, int]
 _NUMBER = Union[ndarray, float, int]
```

### Comparing `aprilbox-1.0.0b2/aprilbox/utils/interpolate.py` & `aprilbox-1.0.0b4/aprilbox/utils/interpolate.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/utils/met/distance.py` & `aprilbox-1.0.0b4/aprilbox/utils/met/distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 Author     : April
 Contact    : fanglwh@outlook.com
 """
 
 __all__ = ["Distance"]
 
 import numpy as np
-from ...types import Tuple, _NUMBER
+
+from ...data import ER
+from ...types import _NUMBER
+
 
 class Distance(object):
     @classmethod
     def euclidean(cls, x1: _NUMBER, y1: _NUMBER, x2: _NUMBER, y2: _NUMBER) -> _NUMBER:
         """Calculate Euclidean distance.
 
         :math:`Distance = \\sqrt{(x_1 - x_2)^2 + (y_1 - y_2)^2}`
@@ -50,15 +53,15 @@
         """
         # degree to radians
         lon1, lon2 = np.deg2rad(lon1), np.deg2rad(lon2)
         lat1, lat2 = np.deg2rad(lat1), np.deg2rad(lat2)
         # calculate distance
         part1 = np.sin((lat2 - lat1) / 2) ** 2
         part2 = np.cos(lat1) * np.cos(lat2) * np.sin((lon2 - lon1) / 2) ** 2
-        return 2.0 * Constant.ER * np.arcsin((part1 + part2) ** 0.5)
+        return 2.0 * ER * np.arcsin((part1 + part2) ** 0.5)
 
     @classmethod
     def vincenty(cls, lon1: _NUMBER, lat1: _NUMBER, lon2: _NUMBER, lat2: _NUMBER,
                  item: int) -> _NUMBER:
         """Calculate Vincenty distance.
 
         :math: `Distance = `
```

### Comparing `aprilbox-1.0.0b2/aprilbox/utils/met/factor.py` & `aprilbox-1.0.0b4/aprilbox/utils/met/factor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 Author     : April
 Contact    : fanglwh@outlook.com
 """
 
 __all__ = ["Factors"]
 
 import numpy as np
+
+from ...data import KELVIN
 from ...types import Tuple, _NUMBER
 
 
 class Factors(object):
     @classmethod
     def saturation_vapor_pressure(cls, temperature: _NUMBER) -> _NUMBER:
         """Calculate the saturation water vapor (partial) pressure.
@@ -27,15 +29,15 @@
             temperature: Air temperature
 
         Returns:
             saturation vapor pressure
         """
         # Converted from original in terms of C to use kelvin. Using raw absolute values of C in
         # a formula plays havoc with units support.
-        return 6.112 * np.exp(17.67 * (temperature - Constant.ZEROK) / (temperature - Constant.ZEROK + 243.5))
+        return 6.112 * np.exp(17.67 * (temperature - KELVIN) / (temperature - KELVIN + 243.5))
 
     @classmethod
     def rhu_from_dpt(cls, tmp: _NUMBER, dpt: _NUMBER) -> _NUMBER:
         """Calculate the relative humidity.
 
         Uses temperature and dewpoint to calculate relative humidity as the ratio of vapor
         pressure to saturation vapor pressures.
```

### Comparing `aprilbox-1.0.0b2/aprilbox/utils/path.py` & `aprilbox-1.0.0b4/aprilbox/utils/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 Author     : April
 Contact    : fanglwh@outlook.com
 """
 
 __all__ = ["PathCather"]
 
 from datetime import datetime, timedelta
+import glob
 from pathlib import Path
+import re
 from typing import Optional
 
 
 class PathCather(object):
 
     @classmethod
     def catch(cls, time: datetime, lead_time: Optional[timedelta], file: str) -> str:
@@ -31,22 +33,23 @@
         Returns:
             The path of file
 
         Exampls:
 
 
             >>> from datetime import datetime, timedelta
+            >>> from aprilbox import PathCather
             >>> tag_time = datetime(year=2022, month=7, day=2, hour=4)   # 目标时间
             >>> file1 = "/mnt/PRESKY/data/cmadata/NAFP/CMPAS_GRIB/%Y/%Y%m/%Y%m%d/*%Y%m%d%H.GRB2"
             >>> file2 = "~/product/FCST/SZW_1000M/F_RADA_FCST_03H_DL/%Y%m%d/F_RADA_FCST_03H_DL_SZW_1000M_%Y%m%d%H%M_%Y%m%d%H%M.nc"
 
             >>> # 抓取实况时间为 2022年7月2日5时，文件路径规则为file1的实况数据
-            >>>path1 = DataReader.catch(time=tag_time + timedelta(hours=1), lead_time=None, file=file1)
+            >>>path1 = PathCather.catch(time=tag_time + timedelta(hours=1), lead_time=None, file=file1)
             >>> # 抓取起报时间为2022年7月2日4时，预报时间为2022年7月2日5时（预报时效为1小时），文件路径规则为file2的预报产品数据
-            >>> path2 = DataReader.catch(time=tag_time, lead_time=timedelta(hours=1), file=file2)
+            >>> path2 = PathCather.catch(time=tag_time, lead_time=timedelta(hours=1), file=file2)
         """
         if file.count("*") > 0:
             # 模糊匹配
             if file.count("%Y") + file.count("%m") + file.count("%d") > 0:
                 assert lead_time is None, TypeError(f"{datetime.now()}\n ftime is exists!")
                 file = time.strftime(file)
             path = glob.glob(time.strftime(file))
```

### Comparing `aprilbox-1.0.0b2/aprilbox/utils/pool.py` & `aprilbox-1.0.0b4/aprilbox/utils/pool.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/vis/base.py` & `aprilbox-1.0.0b4/aprilbox/vis/base.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox/vis/precipitation.py` & `aprilbox-1.0.0b4/aprilbox/vis/precipitation.py`

 * *Files identical despite different names*

### Comparing `aprilbox-1.0.0b2/aprilbox.egg-info/PKG-INFO` & `aprilbox-1.0.0b4/aprilbox.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 Metadata-Version: 2.1
 Name: aprilbox
-Version: 1.0.0b2
+Version: 1.0.0b4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Fang Linwanghao
 Author-email: fanglwh@outlook.com
 License: BSD-3-Clause
+Description: AprilBox, is a personal development toolkit primarily used for developing and researching 
+        artificial intelligence-related content. It also includes various other tools, 
+        including but not limited to meteorological indicators calculation, verification and evaluation calculation,
+        and common quantitative visualization.
+        
+        # Content
+           * [Install]()
+           * [Document]()
+           * [Usage]()
+           * [License]()
+           * [Support]()
+           * [Developers]()
+        
+        
+        ## [Document]()
+        
+        
+        ## [Install]()
+        
+        
+        ## [Usage]()
+        
+        ## [LICENSE]()
+        
+        This project is licensed under the BSD 3-Clause License - see the [LICENSE](/LICENSE.txt) file for details.
+        
+        ## [Support]()
+        
+        Give a ⭐️ if this project helped you!
+        
+        
+        ## [Developer]()
+        * [Linwanghao, Fang]()
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-AprilBox, is a personal development toolkit primarily used for developing and researching 
-artificial intelligence-related content. It also includes various other tools, 
-including but not limited to meteorological indicators calculation, verification and evaluation calculation,
-and common quantitative visualization.
-
-# Content
-   * [Install]()
-   * [Document]()
-   * [Usage]()
-   * [License]()
-   * [Support]()
-   * [Developers]()
-
-
-## [Document]()
-
-
-## [Install]()
-
-
-## [Usage]()
-
-## [LICENSE]()
-
-This project is licensed under the BSD 3-Clause License - see the [LICENSE](/LICENSE) file for details.
-
-## [Support]()
-
-Give a ⭐️ if this project helped you!
-
-
-## [Developer]()
-* [Linwanghao, Fang]()
-
-
```

### Comparing `aprilbox-1.0.0b2/aprilbox.egg-info/SOURCES.txt` & `aprilbox-1.0.0b4/aprilbox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE.txt
 README.md
 setup.cfg
 setup.py
 aprilbox/__init__.py
 aprilbox/types.py
 aprilbox.egg-info/PKG-INFO
 aprilbox.egg-info/SOURCES.txt
@@ -30,15 +29,15 @@
 aprilbox/ai/dl/block/attention/__init__.py
 aprilbox/ai/dl/block/attention/lka.py
 aprilbox/ai/dl/block/attention/psa.py
 aprilbox/ai/dl/block/attention/simple.py
 aprilbox/ai/dl/block/attention/split.py
 aprilbox/ai/dl/loss/__init__.py
 aprilbox/ai/dl/loss/dice.py
-aprilbox/ai/dl/loss/efl.py
+aprilbox/ai/dl/loss/focal.py
 aprilbox/ai/dl/loss/loss.py
 aprilbox/ai/dl/loss/rmse.py
 aprilbox/ai/dl/loss/seesaw.py
 aprilbox/ai/dl/loss/ssim.py
 aprilbox/ai/dl/loss/ts.py
 aprilbox/ai/ml/__init__.py
 aprilbox/ai/tools/__init__.py
```

