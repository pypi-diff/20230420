# Comparing `tmp/eis1600-0.8.4.tar.gz` & `tmp/eis1600-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-0.8.4.tar", last modified: Wed Apr 19 08:36:01 2023, max compression
+gzip compressed data, was "eis1600-0.8.5.tar", last modified: Thu Apr 20 10:02:52 2023, max compression
```

## Comparing `eis1600-0.8.4.tar` & `eis1600-0.8.5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:36:01.327223 eis1600-0.8.4/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.8.4/LICENSE
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-19 08:36:01.327223 eis1600-0.8.4/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5895 2023-04-13 08:22:59.000000 eis1600-0.8.4/README.md
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:36:01.323223 eis1600-0.8.4/eis1600/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.8.4/eis1600/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:36:01.323223 eis1600-0.8.4/eis1600/dates/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.8.4/eis1600/dates/Date.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.4/eis1600/dates/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5856 2023-04-06 11:34:18.000000 eis1600-0.8.4/eis1600/dates/date_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.8.4/eis1600/dates/methods.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:36:01.323223 eis1600-0.8.4/eis1600/gazetteers/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4225 2023-04-14 12:34:00.000000 eis1600-0.8.4/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3259 2023-04-12 08:40:27.000000 eis1600-0.8.4/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.8.4/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:36:01.323223 eis1600-0.8.4/eis1600/gazetteers/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.4/eis1600/gazetteers/data/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:36:01.323223 eis1600-0.8.4/eis1600/helper/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-06 10:45:49.000000 eis1600-0.8.4/eis1600/helper/Singleton.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.8.4/eis1600/helper/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.8.4/eis1600/helper/ar_normalization.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:36:01.323223 eis1600-0.8.4/eis1600/helper/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.8.4/eis1600/helper/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      374 2023-04-05 10:09:07.000000 eis1600-0.8.4/eis1600/helper/entity_tags.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1237 2023-04-12 06:44:26.000000 eis1600-0.8.4/eis1600/helper/fix_miu_annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.8.4/eis1600/helper/logging.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      637 2023-04-06 09:28:14.000000 eis1600-0.8.4/eis1600/helper/markdown_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3723 2023-04-14 12:34:00.000000 eis1600-0.8.4/eis1600/helper/markdown_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.8.4/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      370 2023-04-13 08:15:00.000000 eis1600-0.8.4/eis1600/helper/my_json_ecoder.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10796 2023-04-05 11:18:46.000000 eis1600-0.8.4/eis1600/helper/repo.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1425 2023-04-13 08:57:43.000000 eis1600-0.8.4/eis1600/helper/yml_to_json.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:36:01.327223 eis1600-0.8.4/eis1600/markdown/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.8.4/eis1600/markdown/UIDs.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.8.4/eis1600/markdown/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.8.4/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.8.4/eis1600/markdown/insert_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    13026 2023-04-13 10:26:19.000000 eis1600-0.8.4/eis1600/markdown/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.8.4/eis1600/markdown/update_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5284 2023-04-05 08:21:34.000000 eis1600-0.8.4/eis1600/markdown/update_uids_old_process.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:36:01.327223 eis1600-0.8.4/eis1600/miu/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3484 2023-04-12 15:29:30.000000 eis1600-0.8.4/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6622 2023-04-14 12:11:46.000000 eis1600-0.8.4/eis1600/miu/YAMLHandler.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.8.4/eis1600/miu/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2715 2023-02-23 07:39:16.000000 eis1600-0.8.4/eis1600/miu/disassemble_into_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8907 2023-04-12 06:50:23.000000 eis1600-0.8.4/eis1600/miu/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.8.4/eis1600/miu/reassemble_from_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6008 2023-04-17 08:45:53.000000 eis1600-0.8.4/eis1600/miu/yml_handling.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:36:01.327223 eis1600-0.8.4/eis1600/nlp/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.8.4/eis1600/nlp/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.8.4/eis1600/nlp/cameltools.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3672 2023-03-31 11:52:32.000000 eis1600-0.8.4/eis1600/nlp/ner_annotate_mius.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.8.4/eis1600/nlp/utils.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:36:01.327223 eis1600-0.8.4/eis1600/onomastics/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.8.4/eis1600/onomastics/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1201 2023-04-17 07:58:03.000000 eis1600-0.8.4/eis1600/onomastics/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10081 2023-04-17 11:47:02.000000 eis1600-0.8.4/eis1600/onomastics/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.8.4/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:36:01.327223 eis1600-0.8.4/eis1600/processing/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.4/eis1600/processing/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4660 2023-04-12 08:23:03.000000 eis1600-0.8.4/eis1600/processing/postprocessing.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4604 2023-04-14 13:42:02.000000 eis1600-0.8.4/eis1600/processing/preprocessing.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:36:01.327223 eis1600-0.8.4/eis1600/stats/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.8.4/eis1600/stats/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.8.4/eis1600/stats/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.8.4/eis1600/stats/miu_stats.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-19 08:36:01.323223 eis1600-0.8.4/eis1600.egg-info/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-19 08:36:01.000000 eis1600-0.8.4/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1749 2023-04-19 08:36:01.000000 eis1600-0.8.4/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-04-19 08:36:01.000000 eis1600-0.8.4/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      746 2023-04-19 08:36:01.000000 eis1600-0.8.4/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       72 2023-04-19 08:36:01.000000 eis1600-0.8.4/eis1600.egg-info/requires.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-04-19 08:36:01.000000 eis1600-0.8.4/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-04-19 08:36:01.327223 eis1600-0.8.4/setup.cfg
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2253 2023-04-19 08:35:57.000000 eis1600-0.8.4/setup.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.196050 eis1600-0.8.5/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.8.5/LICENSE
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-20 10:02:52.196050 eis1600-0.8.5/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5895 2023-04-13 08:22:59.000000 eis1600-0.8.5/README.md
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.184050 eis1600-0.8.5/eis1600/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.8.5/eis1600/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.188050 eis1600-0.8.5/eis1600/dates/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.8.5/eis1600/dates/Date.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.5/eis1600/dates/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5856 2023-04-06 11:34:18.000000 eis1600-0.8.5/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.8.5/eis1600/dates/methods.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.188050 eis1600-0.8.5/eis1600/gazetteers/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4225 2023-04-14 12:34:00.000000 eis1600-0.8.5/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3259 2023-04-12 08:40:27.000000 eis1600-0.8.5/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.8.5/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.188050 eis1600-0.8.5/eis1600/gazetteers/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.5/eis1600/gazetteers/data/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.192050 eis1600-0.8.5/eis1600/helper/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      712 2023-04-20 08:48:52.000000 eis1600-0.8.5/eis1600/helper/EntityTags.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-06 10:45:49.000000 eis1600-0.8.5/eis1600/helper/Singleton.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.8.5/eis1600/helper/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.8.5/eis1600/helper/ar_normalization.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.192050 eis1600-0.8.5/eis1600/helper/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.8.5/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1237 2023-04-12 06:44:26.000000 eis1600-0.8.5/eis1600/helper/fix_miu_annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.8.5/eis1600/helper/logging.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      637 2023-04-06 09:28:14.000000 eis1600-0.8.5/eis1600/helper/markdown_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3739 2023-04-20 08:46:34.000000 eis1600-0.8.5/eis1600/helper/markdown_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.8.5/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      370 2023-04-19 14:31:23.000000 eis1600-0.8.5/eis1600/helper/my_json_ecoder.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10796 2023-04-05 11:18:46.000000 eis1600-0.8.5/eis1600/helper/repo.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1425 2023-04-20 09:45:05.000000 eis1600-0.8.5/eis1600/helper/yml_to_json.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.192050 eis1600-0.8.5/eis1600/markdown/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.8.5/eis1600/markdown/UIDs.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.8.5/eis1600/markdown/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.8.5/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.8.5/eis1600/markdown/insert_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    13077 2023-04-19 15:21:14.000000 eis1600-0.8.5/eis1600/markdown/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.8.5/eis1600/markdown/update_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5284 2023-04-05 08:21:34.000000 eis1600-0.8.5/eis1600/markdown/update_uids_old_process.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.192050 eis1600-0.8.5/eis1600/miu/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3484 2023-04-12 15:29:30.000000 eis1600-0.8.5/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6164 2023-04-20 09:51:08.000000 eis1600-0.8.5/eis1600/miu/YAMLHandler.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.8.5/eis1600/miu/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2715 2023-02-23 07:39:16.000000 eis1600-0.8.5/eis1600/miu/disassemble_into_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8907 2023-04-12 06:50:23.000000 eis1600-0.8.5/eis1600/miu/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.8.5/eis1600/miu/reassemble_from_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6314 2023-04-20 09:52:40.000000 eis1600-0.8.5/eis1600/miu/yml_handling.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.192050 eis1600-0.8.5/eis1600/nlp/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.8.5/eis1600/nlp/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.8.5/eis1600/nlp/cameltools.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3672 2023-03-31 11:52:32.000000 eis1600-0.8.5/eis1600/nlp/ner_annotate_mius.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.8.5/eis1600/nlp/utils.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.192050 eis1600-0.8.5/eis1600/onomastics/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.8.5/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1410 2023-04-20 10:02:38.000000 eis1600-0.8.5/eis1600/onomastics/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10301 2023-04-20 10:02:38.000000 eis1600-0.8.5/eis1600/onomastics/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.8.5/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.196050 eis1600-0.8.5/eis1600/processing/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.5/eis1600/processing/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4660 2023-04-12 08:23:03.000000 eis1600-0.8.5/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4604 2023-04-14 13:42:02.000000 eis1600-0.8.5/eis1600/processing/preprocessing.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.196050 eis1600-0.8.5/eis1600/stats/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.8.5/eis1600/stats/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.8.5/eis1600/stats/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.8.5/eis1600/stats/miu_stats.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.188050 eis1600-0.8.5/eis1600.egg-info/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-20 10:02:52.000000 eis1600-0.8.5/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1748 2023-04-20 10:02:52.000000 eis1600-0.8.5/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-04-20 10:02:52.000000 eis1600-0.8.5/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      746 2023-04-20 10:02:52.000000 eis1600-0.8.5/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       72 2023-04-20 10:02:52.000000 eis1600-0.8.5/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-04-20 10:02:52.000000 eis1600-0.8.5/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-04-20 10:02:52.196050 eis1600-0.8.5/setup.cfg
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2253 2023-04-20 10:02:38.000000 eis1600-0.8.5/setup.py
```

### Comparing `eis1600-0.8.4/LICENSE` & `eis1600-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/PKG-INFO` & `eis1600-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.8.4
+Version: 0.8.5
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.8.4/README.md` & `eis1600-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/dates/Date.py` & `eis1600-0.8.5/eis1600/dates/Date.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/dates/date_patterns.py` & `eis1600-0.8.5/eis1600/dates/date_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/dates/methods.py` & `eis1600-0.8.5/eis1600/dates/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/gazetteers/Onomastics.py` & `eis1600-0.8.5/eis1600/gazetteers/Onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/gazetteers/Toponyms.py` & `eis1600-0.8.5/eis1600/gazetteers/Toponyms.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/helper/Singleton.py` & `eis1600-0.8.5/eis1600/helper/Singleton.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/helper/ar_normalization.py` & `eis1600-0.8.5/eis1600/helper/ar_normalization.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/helper/fix_miu_annotation.py` & `eis1600-0.8.5/eis1600/helper/fix_miu_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/helper/markdown_methods.py` & `eis1600-0.8.5/eis1600/helper/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/helper/markdown_patterns.py` & `eis1600-0.8.5/eis1600/helper/markdown_patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from eis1600.helper.entity_tags import get_entity_tags
+from eis1600.helper.EntityTags import EntityTags
 
 AR_LETTERS_CHARSET = frozenset(
         u'\u0621\u0622\u0623\u0624\u0625\u0626\u0627'
         u'\u0628\u0629\u062a\u062b\u062c\u062d\u062e'
         u'\u062f\u0630\u0631\u0632\u0633\u0634\u0635'
         u'\u0636\u0637\u0638\u0639\u063a\u0640\u0641'
         u'\u0642\u0643\u0644\u0645\u0646\u0647\u0648'
@@ -45,15 +45,15 @@
 NOR_DIGIT_NOR_AR_STR = r'[^\d\n' + u''.join(AR_LETTERS_CHARSET) + ']+?'
 TAG_AND_TEXT_SAME_LINE = r'([$@]+' + NOR_DIGIT_NOR_AR_STR + r'\d*' + NOR_DIGIT_NOR_AR_STR + r') ?((?:[(\[] ?)?' + AR_STR + r')'
 UID_TAG_AND_TEXT_SAME_LINE_PATTERN = re.compile(
         r'(_ء_#=\d{12}= )' + TAG_AND_TEXT_SAME_LINE)
 MIU_TAG_AND_TEXT_PATTERN = re.compile(r'(' + MIU_UID + r'[$@]+?(?: \d+)?)\n((?:\( ?)?' + AR_STR + r')')
 
 # MIU entity tags
-entity_tags = '|'.join(get_entity_tags())
+entity_tags = '|'.join(EntityTags.instance().get_entity_tags())
 ENTITY_TAGS_PATTERN = re.compile(r'Ü?(?P<entity>' + entity_tags + r')(?P<length>\d{1,2})(?:[A-Z0-9]+)?')
 YEAR_PATTERN = re.compile(r'Ü?Y\d{1,2}(?P<cat>[A-Z])(?P<written>\d{4})(?P<i>I)?Y(?P<real>\d{4})?')
 AGE_PATTERN = re.compile(r'Ü?A\d(?P<cat>[A-Z])(?P<written>\d{2,3})(?P<i>I)?A(?P<real>\d{2,3})?')
 
 # EIS1600 light mARkdown
 HEADING_OR_BIO_PATTERN = re.compile(r'# [|$]+')
 MIU_LIGHT_OR_EIS1600_PATTERN = re.compile(r'#|_ء_#')
```

### Comparing `eis1600-0.8.4/eis1600/helper/miu_random_revisions.py` & `eis1600-0.8.5/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/helper/repo.py` & `eis1600-0.8.5/eis1600/helper/repo.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/helper/yml_to_json.py` & `eis1600-0.8.5/eis1600/helper/yml_to_json.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/markdown/UIDs.py` & `eis1600-0.8.5/eis1600/markdown/UIDs.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-0.8.5/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/markdown/insert_uids.py` & `eis1600-0.8.5/eis1600/markdown/insert_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/markdown/methods.py` & `eis1600-0.8.5/eis1600/markdown/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,15 @@
                 paragraph = paragraph.replace('#', f'_ء_#={uids.get_uid()}=')
                 # Insert a paragraph tag
                 heading_and_text = paragraph.splitlines()
                 if len(heading_and_text) > 1:
                     paragraph = heading_and_text[0] + f'\n\n_ء_={uids.get_uid()}= ::UNDEFINED:: ~\n' + \
                                 heading_and_text[1]
                 text_updated.append(paragraph)
+            # TODO elif paragraph.startswith('::')
             elif '%~%' in paragraph:
                 paragraph = f'_ء_={uids.get_uid()}= ::POETRY:: ~\n' + paragraph
                 text_updated.append(paragraph)
             elif PAGE_TAG_PATTERN.fullmatch(paragraph):
                 page_tag = PAGE_TAG_PATTERN.match(paragraph).group('page_tag')
                 if PAGE_TAG_SPLITTING_PARAGRAPH_PATTERN.search('\n\n'.join([prev_p, paragraph, next_p])):
                     if text_updated:
```

### Comparing `eis1600-0.8.4/eis1600/markdown/update_uids.py` & `eis1600-0.8.5/eis1600/markdown/update_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/markdown/update_uids_old_process.py` & `eis1600-0.8.5/eis1600/markdown/update_uids_old_process.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/miu/HeadingTracker.py` & `eis1600-0.8.5/eis1600/miu/HeadingTracker.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/miu/YAMLHandler.py` & `eis1600-0.8.5/eis1600/miu/YAMLHandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, Optional
 
 from eis1600.helper.markdown_patterns import MIU_HEADER
 from eis1600.miu.HeadingTracker import HeadingTracker
 
 
 class YAMLHandler:
     """A class to take care of the MIU YAML Headers
@@ -51,28 +51,27 @@
             return val
 
     @staticmethod
     def __parse_yml(yml_str: str) -> Dict:
         yml = {}
         level = []
         dict_elem = {}
-        # print(yml_str)
         for line in yml_str.splitlines():
             if not line.startswith('#'):
                 intend = (len(line) - len(line.lstrip())) / 4
                 key_val = line.split(':')
                 key = key_val[0].strip(' -')
                 val = ':'.join(key_val[1:]).strip()
 
                 if intend < len(level):
                     yml[level[0]] = dict_elem
                     dict_elem = {}
                     level.pop()
-                    yml[key] = YAMLHandler.__parse_yml_val(val)
-                elif intend and intend == len(level):
+
+                if intend and intend == len(level):
                     dict_elem[key] = YAMLHandler.__parse_yml_val(val)
                 elif val == '':
                     dict_elem = {}
                     level.append(key)
                 else:
                     yml[key] = YAMLHandler.__parse_yml_val(val)
 
@@ -83,16 +82,15 @@
 
     def __init__(self, yml: Optional[Dict] = None) -> None:
         self.reviewed = 'NOT REVIEWED'
         self.reviewer = None
         self.headings = None
         self.dates_headings = None
         self.dates = None
-        self.onomastics = {}
-        self.nasab_filtered = None
+        self.onomastics = None
         self.category = None
         self.ambigious_toponyms = False
 
         if yml:
             for key, val in yml.items():
                 if key == 'headings':
                     val = HeadingTracker(val)
@@ -120,25 +118,28 @@
         yaml_str = MIU_HEADER + 'Begin#\n\n'
         for key, val in vars(self).items():
             if key == 'category' and val is not None:
                 yaml_str += key + '    : \'' + val + '\'\n'
             elif isinstance(val, dict):
                 yaml_str += key + '    :\n'
                 for key2, val2 in val.items():
-                    yaml_str += '   - ' + key2 + '  : ' + str(val2) + '\n'
+                    yaml_str += '    - ' + key2 + '  : ' + str(val2) + '\n'
             elif val is not None:
                 yaml_str += key + '    : ' + str(val) + '\n'
         yaml_str += '\n' + MIU_HEADER + 'End#\n\n'
 
         return yaml_str
 
     def to_json(self) -> Dict:
         json_dict = {}
         for key, val in vars(self).items():
             if val is not None:
+                #if key == 'dates':
+                #    val = [elem for elem in val if isinstance(elem, (str, int))]
+                #    json_dict[key] = [{'str': d_str, 'num': d_num} for d_str, d_num in val]
                 json_dict[key] = val
         return json_dict
 
     def is_bio(self) -> bool:
         return self.category == '$' or self.category == '$$'
 
     def is_reviewed(self) -> bool:
@@ -154,30 +155,17 @@
     def add_date_headings(self, date: int) -> None:
         if self.dates_headings:
             if date not in self.dates_headings:
                 self.dates_headings.append(date)
         else:
             self.dates_headings = [date]
 
-    def add_nas(self, nas: List[Tuple[int, str]]) -> None:
-        if hasattr(self, 'onomastics') and self.onomastics:
-            self.onomanstics['nas'] = nas
-        else:
-            self.onomastics = {'nas': nas}
-
-    def add_nasab_filtered(self, nasab_filtered: str) -> None:
-        self.nasab_filtered = nasab_filtered
-
     def add_tagged_entities(self, entities_dict: dict) -> None:
         for key, val in entities_dict.items():
-            if key == 'onomastics' and hasattr(self, 'onomastics') and self.onomastics:
-                for key2, val2 in val.items():
-                    self.onomastics[key2] = val2
-            else:
-                self.__setattr__(key, val)
+            self.__setattr__(key, val)
 
     def __setitem__(self, key: str, value: Any) -> None:
         super().__setattr__(key, value)
 
     def __repr__(self) -> str:
         return str(self.__dict__)
```

### Comparing `eis1600-0.8.4/eis1600/miu/disassemble_into_miu_files.py` & `eis1600-0.8.5/eis1600/miu/disassemble_into_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/miu/methods.py` & `eis1600-0.8.5/eis1600/miu/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/miu/reassemble_from_miu_files.py` & `eis1600-0.8.5/eis1600/miu/reassemble_from_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/miu/yml_handling.py` & `eis1600-0.8.5/eis1600/miu/yml_handling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from itertools import combinations
 from typing import Dict, List, Optional, Set, TextIO, Tuple, Union
 
 from eis1600.gazetteers.Toponyms import Toponyms
 from eis1600.helper.markdown_methods import get_yrs_tag_value
-from eis1600.helper.entity_tags import get_entity_tags_df
+from eis1600.helper.EntityTags import EntityTags
 from eis1600.miu.HeadingTracker import HeadingTracker
 from eis1600.miu.YAMLHandler import YAMLHandler
 from eis1600.helper.markdown_patterns import ENTITY_TAGS_PATTERN, MIU_HEADER_PATTERN, NEWLINES_CROWD_PATTERN
 
 
 def create_yml_header(category: str, headings: Optional[HeadingTracker] = None) -> str:
     """Creates a YAML header for the current MIU file and returns it as yamlfied string.
@@ -56,15 +56,15 @@
             text = NEWLINES_CROWD_PATTERN.sub('\n\n', text)
 
     return miu_yml_header, text
 
 
 def add_to_entities_dict(
         entities_dict: Dict, cat: str,
-        entity: Union[str, Tuple[str, Union[int, str]], List[Tuple[str, str]], List[str]],
+        entity: Union[str, Tuple[str, Union[int, str]], List[Tuple[str, str]], List[str], Tuple[int, str]],
         tag: Optional[str] = None
 ) -> None:
     """Add a tagged entity to the respective list in the entities_dict.
 
     :param Dict entities_dict: Dict containing previous tagged entities.
     :param str cat: Category of the entity.
     :param Union[str|int] entity: Entity - might be int if entity is a date, otherwise str.
@@ -94,18 +94,21 @@
 def add_annotated_entities_to_yml(text_with_tags: str, yml_handler: YAMLHandler, filename: str) -> None:
     """Populates YAMLHeader with annotated entities.
 
     :param str text_with_tags: Text with inserted tags of the MIU.
     :param YAMLHandler yml_handler: YAMLHandler of the MIU.
     :param str filename: Filename of the current MIU (used in error msg).
     """
-    entity_tags_df = get_entity_tags_df()
+    # We do not need to differentiate between automated and manual tags
+    text_with_tags = text_with_tags.replace('Ü', '')
+    entity_tags_df = EntityTags.instance().get_entity_tags_df()
     entities_dict = {}
     toponyms_set: Set[str] = set()
     provinces_set: Set[str] = set()
+    nas_counter = 0
 
     m = ENTITY_TAGS_PATTERN.search(text_with_tags)
     while m:
         tag = m.group('entity')
         length = int(m.group('length'))
         entity = ' '.join(text_with_tags[m.end():].split(maxsplit=length)[:length])
 
@@ -113,27 +116,31 @@
         if cat == 'DATE' or cat == 'AGE':
             try:
                 val = get_yrs_tag_value(m.group(0))
                 add_to_entities_dict(entities_dict, cat, (entity, val))
             except ValueError:
                 print(f'Tag is neither year nor age: {m.group(0)}\nCheck: {filename}')
                 return
+        elif cat == 'TOPONYM':
+            tg = Toponyms.instance()
+            place, uri, list_of_uris, list_of_provinces = tg.look_up_entity(entity)
+            if len(list_of_uris) > 1:
+                yml_handler.set_ambigious_toponyms()
+            toponyms_set.update(list_of_uris)
+            provinces_set.update(list_of_provinces)
+            add_to_entities_dict(entities_dict, cat, (place, uri))
+        elif cat == 'ONOMASTIC':
+            if tag.startswith('SHR') and entity.startswith('ب'):
+                entity = entity[1:]
+            elif tag.startswith('NAS'):
+                entity = (nas_counter, entity)
+                nas_counter += 1
+            add_to_entities_dict(entities_dict, cat, entity, tag)
         else:
-            if cat == 'TOPONYM':
-                tg = Toponyms.instance()
-                place, uri, list_of_uris, list_of_provinces = tg.look_up_entity(entity)
-                if len(list_of_uris) > 1:
-                    yml_handler.set_ambigious_toponyms()
-                toponyms_set.update(list_of_uris)
-                provinces_set.update(list_of_provinces)
-                add_to_entities_dict(entities_dict, cat, (place, uri))
-            else:
-                if (tag.startswith('ÜSHR') or tag.startswith('SHR')) and entity.startswith('ب'):
-                    entity = entity[1:]
-                add_to_entities_dict(entities_dict, cat, entity, tag)
+            add_to_entities_dict(entities_dict, cat, entity, tag)
 
         m = ENTITY_TAGS_PATTERN.search(text_with_tags, m.end())
 
     add_to_entities_dict(entities_dict, 'edges_toponym', list(combinations(toponyms_set, 2)))
     add_to_entities_dict(entities_dict, 'province', list(provinces_set))
     add_to_entities_dict(entities_dict, 'edges_province', list(combinations(provinces_set, 2)))
     yml_handler.add_tagged_entities(entities_dict)
```

### Comparing `eis1600-0.8.4/eis1600/nlp/cameltools.py` & `eis1600-0.8.5/eis1600/nlp/cameltools.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/nlp/ner_annotate_mius.py` & `eis1600-0.8.5/eis1600/nlp/ner_annotate_mius.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/nlp/utils.py` & `eis1600-0.8.5/eis1600/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/onomastics/annotation.py` & `eis1600-0.8.5/eis1600/onomastics/annotation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from glob import glob
 from pathlib import Path
 
 import sys
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from functools import partial
 
 from eis1600.helper.logging import setup_logger
@@ -14,21 +15,26 @@
     arg_parser = ArgumentParser(
             prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to annotate onomastic information in gold-standard MIUs.'''
     )
 
     with open('OpenITI_EIS1600_MIUs/gold_standard.txt', 'r', encoding='utf-8') as fh:
         files_txt = fh.read().splitlines()
-    infiles = ['OpenITI_EIS1600_MIUs/training_data/' + file for file in files_txt if Path(
-            'OpenITI_EIS1600_MIUs/training_data/' + file).exists()]
+    # Uncomment to test on training_data
+    # infiles = ['OpenITI_EIS1600_MIUs/training_data/' + file for file in files_txt if Path(
+    #         'OpenITI_EIS1600_MIUs/training_data/' + file).exists()]
+
+    # test on new batch
+    infiles = glob('OpenITI_EIS1600_MIUs/training_data_nasab_ML2/*.EIS1600')
 
     logger_nasab = setup_logger('nasab_unknown', 'OpenITI_EIS1600_MIUs/logs/nasab_unknown.log')
     res = []
     res += p_uimap(partial(nasab_annotation, logger_nasab=logger_nasab), infiles)
 
+    # run serialized (nor parallelized)
     # for file in infiles:
     #     print(file)
     #     res.append(nasab_annotation(file, logger_nasab))
 
     with open('gazetteers/tagged.txt', 'w', encoding='utf-8') as fh:
         fh.write('\n\n'.join(res))
```

### Comparing `eis1600-0.8.4/eis1600/onomastics/methods.py` & `eis1600-0.8.5/eis1600/onomastics/methods.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from eis1600.gazetteers.Onomastics import Onomastics
 from eis1600.gazetteers.Toponyms import Toponyms
 from eis1600.onomastics.re_pattern import ABU, ABI, BANU_BANI, CRF_PATTERN, IBN_IBNA, BN_BNT, SHR_PATTERN, SPELLING, UMM
 from eis1600.processing.preprocessing import get_tokens_and_tags, get_yml_and_miu_df
 from eis1600.processing.postprocessing import reconstruct_miu_text_with_tags, write_updated_miu_to_file
 
 
-def get_nas(text: str, yml_handler: YAMLHandler) -> str:
+def get_nas(text: str) -> str:
     """Add the list of forefathers to the YAMLHeader and return nasab part with tagged NAS and manipulated so it is
     ignored for further onomastic analysis (all elements which refere to ancestors are filtered here).
 
     :param str text: nasab str.
     :param YAMLHandler yml_handler: YAMLHandler of the MIU.
     :return str: nasab str with tagged and manipulated nas elements.
     """
@@ -46,16 +46,14 @@
         last_ancestor = text_mnpld[end + 1:].find(' ')
         if last_ancestor == -1:
             ancestors = BN_BNT.split(text_mnpld[start:])
         else:
             ancestors = BN_BNT.split(text_mnpld[start:end + 1 + last_ancestor])
         if ancestors[0] == '':
             ancestors = ancestors[1:]
-        nas = [(i, txt.replace('_', ' ')) for i, txt in enumerate([a for a in ancestors if not a.startswith('بن')])]
-        yml_handler.add_nas(nas)
         nas_w_tags = ''
         # Insert NAS tags
         for elem in ancestors:
             if not elem.startswith('بن'):
                 num_tokens = len(elem.replace('_', ' ').split())
                 nas_w_tags += ' ÜNAS' + str(max(1, num_tokens))
             nas_w_tags += ' ' + elem
@@ -174,15 +172,17 @@
     :return Series: a series of the same length as the df containing the nasab tags corresponding to the tokens.
     """
     if not yml_handler.is_bio():
         return Series([nan] * len(df))
 
     s_notna = df['TAGS_LISTS'].loc[df['TAGS_LISTS'].notna()].apply(lambda tag_list: ','.join(tag_list))
     try:
-        idx = s_notna.loc[s_notna.str.contains('NASAB')].index[0]
+        # training_data batch uses old NASAB tag, not new ENASAB tag
+        # idx = s_notna.loc[s_notna.str.contains('NASAB')].index[0]
+        idx = s_notna.loc[s_notna.str.contains('ENASAB')].index[0]
     except IndexError:
         print(
                 f'MIU does not have a NASAB tag, most likely the MIU is not a biography but a cross reference. '
                 f'Check:\n{file}'
         )
         return Series([nan] * len(df))
 
@@ -204,15 +204,15 @@
         if count > 0:
             count -= 1
             spl_idcs.append(row[0])
 
     nasab_idx = df.loc[nasab_idx.difference(spl_idcs)].index
     text = ' '.join(df['TOKENS'].loc[nasab_idx])
 
-    text_w_mnpld_nas = get_nas(text, yml_handler)
+    text_w_mnpld_nas = get_nas(text)
     tagged_onomastics = tag_nasab(text_w_mnpld_nas, logger_nasab)
     ar_tokens, tags = get_tokens_and_tags(tagged_onomastics)
     df.loc[nasab_idx, 'NASAB_TAGS'] = tags
 
     if idx != len(df):
         # TODO make NASAB stay on same line
         df.loc[idx - 1, 'NASAB_END'] = 'NASAB'
@@ -220,24 +220,29 @@
     return df['NASAB_TAGS'].to_list()
 
 
 def nasab_annotation(file: str, logger_nasab: Logger) -> str:
     """Only used for onomastic_annotation cmdline script."""
     with open(file, 'r', encoding='utf-8') as miu_file_object:
         yml_handler, df = get_yml_and_miu_df(miu_file_object)
-    if '$' not in df.iloc[0]['SECTIONS'] or '$$$' in df.iloc[0]['SECTIONS'] or not yml_handler.is_reviewed():
-        df['NASAB_TAGS'] = Series([nan] * len(df))
-    else:
-        yml_handler.set_category('$')
-        df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, file, logger_nasab)
+    # Only used if run on training_data batch because this information is missing there
+    # if '$' not in df.iloc[0]['SECTIONS'] or '$$$' in df.iloc[0]['SECTIONS'] or not yml_handler.is_reviewed():
+    #     df['NASAB_TAGS'] = Series([nan] * len(df))
+    # else:
+    #     yml_handler.set_category('$')
+    #     df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, file, logger_nasab)
 
+    # Run on new data batch
+    df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, file, logger_nasab)
     yml_handler.unset_reviewed()
 
     reconstructed_miu = reconstruct_miu_text_with_tags(df[['SECTIONS', 'TOKENS', 'NASAB_TAGS']])
 
-    output_path = str(file).replace('training_data', 'training_nasab')
+    # Outpath for training_data batch
+    # output_path = str(file).replace('training_data', 'training_nasab')
+    output_path = str(file)
     with open(output_path, 'w', encoding='utf-8') as out_file_object:
         write_updated_miu_to_file(
                 out_file_object, yml_handler, df[['SECTIONS', 'TOKENS', 'TAGS_LISTS', 'NASAB_TAGS']]
         )
 
     return f'{file}\n' + reconstructed_miu
```

### Comparing `eis1600-0.8.4/eis1600/onomastics/re_pattern.py` & `eis1600-0.8.5/eis1600/onomastics/re_pattern.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/processing/postprocessing.py` & `eis1600-0.8.5/eis1600/processing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/processing/preprocessing.py` & `eis1600-0.8.5/eis1600/processing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/stats/methods.py` & `eis1600-0.8.5/eis1600/stats/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600/stats/miu_stats.py` & `eis1600-0.8.5/eis1600/stats/miu_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/eis1600.egg-info/PKG-INFO` & `eis1600-0.8.5/eis1600.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.8.4
+Version: 0.8.5
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.8.4/eis1600.egg-info/SOURCES.txt` & `eis1600-0.8.5/eis1600.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 eis1600/dates/__init__.py
 eis1600/dates/date_patterns.py
 eis1600/dates/methods.py
 eis1600/gazetteers/Onomastics.py
 eis1600/gazetteers/Toponyms.py
 eis1600/gazetteers/__init__.py
 eis1600/gazetteers/data/__init__.py
+eis1600/helper/EntityTags.py
 eis1600/helper/Singleton.py
 eis1600/helper/__init__.py
 eis1600/helper/ar_normalization.py
-eis1600/helper/entity_tags.py
 eis1600/helper/fix_miu_annotation.py
 eis1600/helper/logging.py
 eis1600/helper/markdown_methods.py
 eis1600/helper/markdown_patterns.py
 eis1600/helper/miu_random_revisions.py
 eis1600/helper/my_json_ecoder.py
 eis1600/helper/repo.py
```

### Comparing `eis1600-0.8.4/eis1600.egg-info/entry_points.txt` & `eis1600-0.8.5/eis1600.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.4/setup.py` & `eis1600-0.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='0.8.4',
+      version='0.8.5',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
```

