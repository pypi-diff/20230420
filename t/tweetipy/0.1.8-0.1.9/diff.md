# Comparing `tmp/tweetipy-0.1.8.tar.gz` & `tmp/tweetipy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweetipy-0.1.8.tar", max compression
+gzip compressed data, was "tweetipy-0.1.9.tar", max compression
```

## Comparing `tweetipy-0.1.8.tar` & `tweetipy-0.1.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1098 2022-09-17 17:37:12.090904 tweetipy-0.1.8/LICENSE
--rw-r--r--   0        0        0      512 2023-04-02 16:20:33.841125 tweetipy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4071 2023-04-02 16:14:56.215614 tweetipy-0.1.8/README.md
--rw-r--r--   0        0        0       26 2022-09-17 23:54:16.165847 tweetipy-0.1.8/tweetipy/__init__.py
--rw-r--r--   0        0        0       34 2023-04-01 23:45:07.117713 tweetipy-0.1.8/tweetipy/enums/expansions/__init__.py
--rw-r--r--   0        0        0      517 2023-04-02 00:27:15.262117 tweetipy-0.1.8/tweetipy/enums/expansions/Tweet.py
--rw-r--r--   0        0        0      161 2023-04-02 11:18:20.684883 tweetipy-0.1.8/tweetipy/enums/fields/__init__.py
--rw-r--r--   0        0        0       31 2023-04-02 11:17:58.922146 tweetipy-0.1.8/tweetipy/enums/fields/_media/__init__.py
--rw-r--r--   0        0        0      668 2023-04-02 00:30:57.221532 tweetipy-0.1.8/tweetipy/enums/fields/_media/main.py
--rw-r--r--   0        0        0       31 2023-04-01 23:49:41.147532 tweetipy-0.1.8/tweetipy/enums/fields/_place/__init__.py
--rw-r--r--   0        0        0      461 2023-04-02 00:31:04.895415 tweetipy-0.1.8/tweetipy/enums/fields/_place/main.py
--rw-r--r--   0        0        0       30 2023-04-01 23:55:17.006929 tweetipy-0.1.8/tweetipy/enums/fields/_poll/__init__.py
--rw-r--r--   0        0        0      409 2023-04-02 00:31:15.279172 tweetipy-0.1.8/tweetipy/enums/fields/_poll/main.py
--rw-r--r--   0        0        0       31 2023-04-01 23:55:20.447402 tweetipy-0.1.8/tweetipy/enums/fields/_tweet/__init__.py
--rw-r--r--   0        0        0      772 2023-04-02 00:31:23.863655 tweetipy-0.1.8/tweetipy/enums/fields/_tweet/main.py
--rw-r--r--   0        0        0       30 2023-04-01 23:56:40.641144 tweetipy-0.1.8/tweetipy/enums/fields/_user/__init__.py
--rw-r--r--   0        0        0      495 2023-04-02 00:31:31.262805 tweetipy-0.1.8/tweetipy/enums/fields/_user/main.py
--rw-r--r--   0        0        0       66 2022-09-17 14:29:20.230309 tweetipy-0.1.8/tweetipy/handlers/__init__.py
--rw-r--r--   0        0        0     7908 2023-04-01 22:29:38.883834 tweetipy-0.1.8/tweetipy/handlers/Media.py
--rw-r--r--   0        0        0     7663 2023-04-02 15:57:15.482196 tweetipy-0.1.8/tweetipy/handlers/Tweets.py
--rw-r--r--   0        0        0       38 2023-03-13 01:39:28.787724 tweetipy-0.1.8/tweetipy/helpers/__init__.py
--rw-r--r--   0        0        0     5631 2023-04-01 22:25:13.802414 tweetipy-0.1.8/tweetipy/helpers/API.py
--rw-r--r--   0        0        0       66 2023-03-13 23:35:29.952472 tweetipy-0.1.8/tweetipy/helpers/QueryBuilder/__init__.py
--rw-r--r--   0        0        0    13424 2023-03-14 01:18:47.749709 tweetipy-0.1.8/tweetipy/helpers/QueryBuilder/alt.py
--rw-r--r--   0        0        0     1320 2023-03-13 23:35:29.952472 tweetipy-0.1.8/tweetipy/helpers/QueryBuilder/lang.py
--rw-r--r--   0        0        0    12590 2023-04-02 16:17:10.760650 tweetipy-0.1.8/tweetipy/helpers/QueryBuilder/main.py
--rw-r--r--   0        0        0     1229 2023-04-02 14:27:40.843425 tweetipy-0.1.8/tweetipy/main.py
--rw-r--r--   0        0        0      355 2023-04-02 14:51:33.732005 tweetipy-0.1.8/tweetipy/types/__init__.py
--rw-r--r--   0        0        0       32 2023-04-02 15:17:04.210497 tweetipy-0.1.8/tweetipy/types/_attachments/__init__.py
--rw-r--r--   0        0        0      185 2023-04-02 15:08:45.863386 tweetipy-0.1.8/tweetipy/types/_attachments/_main.py
--rw-r--r--   0        0        0      197 2023-04-02 01:35:14.342413 tweetipy-0.1.8/tweetipy/types/_geo.py
--rw-r--r--   0        0        0       29 2023-04-02 14:42:17.075906 tweetipy-0.1.8/tweetipy/types/_includes/__init__.py
--rw-r--r--   0        0        0      738 2023-04-02 12:16:49.202345 tweetipy-0.1.8/tweetipy/types/_includes/_main.py
--rw-r--r--   0        0        0      462 2023-04-02 11:44:09.769400 tweetipy-0.1.8/tweetipy/types/_media_to_upload.py
--rw-r--r--   0        0        0       26 2023-04-02 14:28:44.236306 tweetipy-0.1.8/tweetipy/types/_place/__init__.py
--rw-r--r--   0        0        0      512 2023-04-02 14:35:29.118786 tweetipy-0.1.8/tweetipy/types/_place/_main.py
--rw-r--r--   0        0        0       26 2023-04-02 14:29:57.722659 tweetipy-0.1.8/tweetipy/types/_scope/__init__.py
--rw-r--r--   0        0        0     1969 2022-09-17 10:29:15.378004 tweetipy-0.1.8/tweetipy/types/_scope/_main.py
--rw-r--r--   0        0        0       96 2023-04-02 14:26:13.667886 tweetipy-0.1.8/tweetipy/types/context_annotation/__init__.py
--rw-r--r--   0        0        0      341 2023-04-02 14:25:11.649078 tweetipy-0.1.8/tweetipy/types/context_annotation/_domain.py
--rw-r--r--   0        0        0      341 2023-04-02 14:25:24.160937 tweetipy-0.1.8/tweetipy/types/context_annotation/_entity.py
--rw-r--r--   0        0        0      561 2023-04-02 14:26:28.501341 tweetipy-0.1.8/tweetipy/types/context_annotation/_main.py
--rw-r--r--   0        0        0       57 2023-04-02 14:20:05.997465 tweetipy-0.1.8/tweetipy/types/media/__init__.py
--rw-r--r--   0        0        0     1608 2023-04-02 12:45:42.581787 tweetipy-0.1.8/tweetipy/types/media/_main.py
--rw-r--r--   0        0        0      216 2023-04-02 12:06:48.497607 tweetipy-0.1.8/tweetipy/types/media/_variant.py
--rw-r--r--   0        0        0      156 2023-04-02 12:03:51.127432 tweetipy-0.1.8/tweetipy/types/media/metrics/__init__.py
--rw-r--r--   0        0        0      475 2023-04-02 12:00:40.634847 tweetipy-0.1.8/tweetipy/types/media/metrics/_nonpublic.py
--rw-r--r--   0        0        0      535 2023-04-02 12:02:17.780912 tweetipy-0.1.8/tweetipy/types/media/metrics/_organic.py
--rw-r--r--   0        0        0      536 2023-04-02 12:03:31.271923 tweetipy-0.1.8/tweetipy/types/media/metrics/_promoted.py
--rw-r--r--   0        0        0      119 2023-04-02 12:03:25.424954 tweetipy-0.1.8/tweetipy/types/media/metrics/_public.py
--rw-r--r--   0        0        0       52 2023-04-02 14:51:26.644091 tweetipy-0.1.8/tweetipy/types/poll/__init__.py
--rw-r--r--   0        0        0     1199 2023-04-02 15:20:46.667135 tweetipy-0.1.8/tweetipy/types/poll/_main.py
--rw-r--r--   0        0        0      284 2023-04-02 14:54:14.014717 tweetipy-0.1.8/tweetipy/types/poll/_option.py
--rw-r--r--   0        0        0       64 2023-04-02 14:35:20.696777 tweetipy-0.1.8/tweetipy/types/tweet/__init__.py
--rw-r--r--   0        0        0     3854 2023-04-02 15:23:08.040030 tweetipy-0.1.8/tweetipy/types/tweet/_main.py
--rw-r--r--   0        0        0      980 2023-04-02 14:41:54.012498 tweetipy-0.1.8/tweetipy/types/tweet/_reply_config.py
--rw-r--r--   0        0        0       36 2023-04-02 14:18:41.831364 tweetipy-0.1.8/tweetipy/types/tweet/metrics/__init__.py
--rw-r--r--   0        0        0      843 2023-04-02 14:18:25.170773 tweetipy-0.1.8/tweetipy/types/tweet/metrics/_public.py
--rw-r--r--   0        0        0       25 2023-04-02 14:23:08.018606 tweetipy-0.1.8/tweetipy/types/user/__init__.py
--rw-r--r--   0        0        0      965 2023-04-02 14:23:04.007030 tweetipy-0.1.8/tweetipy/types/user/_main.py
--rw-r--r--   0        0        0       36 2023-04-02 14:22:29.131572 tweetipy-0.1.8/tweetipy/types/user/metrics/__init__.py
--rw-r--r--   0        0        0      744 2023-04-02 14:22:18.984358 tweetipy-0.1.8/tweetipy/types/user/metrics/_public.py
--rw-r--r--   0        0        0     5560 1970-01-01 00:00:00.000000 tweetipy-0.1.8/setup.py
--rw-r--r--   0        0        0     4652 1970-01-01 00:00:00.000000 tweetipy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1098 2022-09-17 17:37:12.090904 tweetipy-0.1.9/LICENSE
+-rw-r--r--   0        0        0      513 2023-04-20 00:08:26.514906 tweetipy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4071 2023-04-02 16:14:56.215614 tweetipy-0.1.9/README.md
+-rw-r--r--   0        0        0       26 2023-04-03 11:48:23.509389 tweetipy-0.1.9/tweetipy/__init__.py
+-rw-r--r--   0        0        0       34 2023-04-01 23:45:07.117713 tweetipy-0.1.9/tweetipy/enums/expansions/__init__.py
+-rw-r--r--   0        0        0      517 2023-04-02 00:27:15.262117 tweetipy-0.1.9/tweetipy/enums/expansions/Tweet.py
+-rw-r--r--   0        0        0      161 2023-04-02 11:18:20.684883 tweetipy-0.1.9/tweetipy/enums/fields/__init__.py
+-rw-r--r--   0        0        0       31 2023-04-02 11:17:58.922146 tweetipy-0.1.9/tweetipy/enums/fields/_media/__init__.py
+-rw-r--r--   0        0        0      668 2023-04-02 00:30:57.221532 tweetipy-0.1.9/tweetipy/enums/fields/_media/main.py
+-rw-r--r--   0        0        0       31 2023-04-01 23:49:41.147532 tweetipy-0.1.9/tweetipy/enums/fields/_place/__init__.py
+-rw-r--r--   0        0        0      461 2023-04-02 00:31:04.895415 tweetipy-0.1.9/tweetipy/enums/fields/_place/main.py
+-rw-r--r--   0        0        0       30 2023-04-01 23:55:17.006929 tweetipy-0.1.9/tweetipy/enums/fields/_poll/__init__.py
+-rw-r--r--   0        0        0      409 2023-04-02 00:31:15.279172 tweetipy-0.1.9/tweetipy/enums/fields/_poll/main.py
+-rw-r--r--   0        0        0       31 2023-04-01 23:55:20.447402 tweetipy-0.1.9/tweetipy/enums/fields/_tweet/__init__.py
+-rw-r--r--   0        0        0      772 2023-04-02 00:31:23.863655 tweetipy-0.1.9/tweetipy/enums/fields/_tweet/main.py
+-rw-r--r--   0        0        0       30 2023-04-01 23:56:40.641144 tweetipy-0.1.9/tweetipy/enums/fields/_user/__init__.py
+-rw-r--r--   0        0        0      495 2023-04-02 00:31:31.262805 tweetipy-0.1.9/tweetipy/enums/fields/_user/main.py
+-rw-r--r--   0        0        0       66 2022-09-17 14:29:20.230309 tweetipy-0.1.9/tweetipy/handlers/__init__.py
+-rw-r--r--   0        0        0     7915 2023-04-03 10:34:58.079728 tweetipy-0.1.9/tweetipy/handlers/Media.py
+-rw-r--r--   0        0        0     7691 2023-04-20 00:04:03.157192 tweetipy-0.1.9/tweetipy/handlers/Tweets.py
+-rw-r--r--   0        0        0       38 2023-03-13 01:39:28.787724 tweetipy-0.1.9/tweetipy/helpers/__init__.py
+-rw-r--r--   0        0        0     5636 2023-04-03 10:23:13.325791 tweetipy-0.1.9/tweetipy/helpers/API.py
+-rw-r--r--   0        0        0       66 2023-03-13 23:35:29.952472 tweetipy-0.1.9/tweetipy/helpers/QueryBuilder/__init__.py
+-rw-r--r--   0        0        0    13424 2023-03-14 01:18:47.749709 tweetipy-0.1.9/tweetipy/helpers/QueryBuilder/alt.py
+-rw-r--r--   0        0        0     1320 2023-03-13 23:35:29.952472 tweetipy-0.1.9/tweetipy/helpers/QueryBuilder/lang.py
+-rw-r--r--   0        0        0    12686 2023-04-19 16:31:11.221122 tweetipy-0.1.9/tweetipy/helpers/QueryBuilder/main.py
+-rw-r--r--   0        0        0     1229 2023-04-03 10:18:29.129999 tweetipy-0.1.9/tweetipy/main.py
+-rw-r--r--   0        0        0      355 2023-04-02 14:51:33.732005 tweetipy-0.1.9/tweetipy/types/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-02 15:17:04.210497 tweetipy-0.1.9/tweetipy/types/_attachments/__init__.py
+-rw-r--r--   0        0        0      185 2023-04-02 15:08:45.863386 tweetipy-0.1.9/tweetipy/types/_attachments/_main.py
+-rw-r--r--   0        0        0      197 2023-04-02 01:35:14.342413 tweetipy-0.1.9/tweetipy/types/_geo.py
+-rw-r--r--   0        0        0       29 2023-04-02 14:42:17.075906 tweetipy-0.1.9/tweetipy/types/_includes/__init__.py
+-rw-r--r--   0        0        0      738 2023-04-02 12:16:49.202345 tweetipy-0.1.9/tweetipy/types/_includes/_main.py
+-rw-r--r--   0        0        0      462 2023-04-02 11:44:09.769400 tweetipy-0.1.9/tweetipy/types/_media_to_upload.py
+-rw-r--r--   0        0        0       26 2023-04-02 14:28:44.236306 tweetipy-0.1.9/tweetipy/types/_place/__init__.py
+-rw-r--r--   0        0        0      512 2023-04-02 14:35:29.118786 tweetipy-0.1.9/tweetipy/types/_place/_main.py
+-rw-r--r--   0        0        0       26 2023-04-02 14:29:57.722659 tweetipy-0.1.9/tweetipy/types/_scope/__init__.py
+-rw-r--r--   0        0        0     1969 2022-09-17 10:29:15.378004 tweetipy-0.1.9/tweetipy/types/_scope/_main.py
+-rw-r--r--   0        0        0       96 2023-04-02 14:26:13.667886 tweetipy-0.1.9/tweetipy/types/context_annotation/__init__.py
+-rw-r--r--   0        0        0      341 2023-04-02 14:25:11.649078 tweetipy-0.1.9/tweetipy/types/context_annotation/_domain.py
+-rw-r--r--   0        0        0      341 2023-04-02 14:25:24.160937 tweetipy-0.1.9/tweetipy/types/context_annotation/_entity.py
+-rw-r--r--   0        0        0      561 2023-04-02 14:26:28.501341 tweetipy-0.1.9/tweetipy/types/context_annotation/_main.py
+-rw-r--r--   0        0        0       57 2023-04-02 14:20:05.997465 tweetipy-0.1.9/tweetipy/types/media/__init__.py
+-rw-r--r--   0        0        0     1608 2023-04-02 12:45:42.581787 tweetipy-0.1.9/tweetipy/types/media/_main.py
+-rw-r--r--   0        0        0      216 2023-04-02 12:06:48.497607 tweetipy-0.1.9/tweetipy/types/media/_variant.py
+-rw-r--r--   0        0        0      156 2023-04-02 12:03:51.127432 tweetipy-0.1.9/tweetipy/types/media/metrics/__init__.py
+-rw-r--r--   0        0        0      475 2023-04-02 12:00:40.634847 tweetipy-0.1.9/tweetipy/types/media/metrics/_nonpublic.py
+-rw-r--r--   0        0        0      535 2023-04-02 12:02:17.780912 tweetipy-0.1.9/tweetipy/types/media/metrics/_organic.py
+-rw-r--r--   0        0        0      536 2023-04-02 12:03:31.271923 tweetipy-0.1.9/tweetipy/types/media/metrics/_promoted.py
+-rw-r--r--   0        0        0      162 2023-04-19 23:59:49.226010 tweetipy-0.1.9/tweetipy/types/media/metrics/_public.py
+-rw-r--r--   0        0        0       52 2023-04-02 14:51:26.644091 tweetipy-0.1.9/tweetipy/types/poll/__init__.py
+-rw-r--r--   0        0        0     1199 2023-04-02 15:20:46.667135 tweetipy-0.1.9/tweetipy/types/poll/_main.py
+-rw-r--r--   0        0        0      284 2023-04-02 14:54:14.014717 tweetipy-0.1.9/tweetipy/types/poll/_option.py
+-rw-r--r--   0        0        0       64 2023-04-02 14:35:20.696777 tweetipy-0.1.9/tweetipy/types/tweet/__init__.py
+-rw-r--r--   0        0        0     3854 2023-04-03 10:27:18.808640 tweetipy-0.1.9/tweetipy/types/tweet/_main.py
+-rw-r--r--   0        0        0     1036 2023-04-19 23:57:03.948225 tweetipy-0.1.9/tweetipy/types/tweet/_reply_config.py
+-rw-r--r--   0        0        0       36 2023-04-02 14:18:41.831364 tweetipy-0.1.9/tweetipy/types/tweet/metrics/__init__.py
+-rw-r--r--   0        0        0      843 2023-04-02 14:18:25.170773 tweetipy-0.1.9/tweetipy/types/tweet/metrics/_public.py
+-rw-r--r--   0        0        0       25 2023-04-02 14:23:08.018606 tweetipy-0.1.9/tweetipy/types/user/__init__.py
+-rw-r--r--   0        0        0      965 2023-04-02 14:23:04.007030 tweetipy-0.1.9/tweetipy/types/user/_main.py
+-rw-r--r--   0        0        0       36 2023-04-02 14:22:29.131572 tweetipy-0.1.9/tweetipy/types/user/metrics/__init__.py
+-rw-r--r--   0        0        0      744 2023-04-02 14:22:18.984358 tweetipy-0.1.9/tweetipy/types/user/metrics/_public.py
+-rw-r--r--   0        0        0     5561 1970-01-01 00:00:00.000000 tweetipy-0.1.9/setup.py
+-rw-r--r--   0        0        0     4552 1970-01-01 00:00:00.000000 tweetipy-0.1.9/PKG-INFO
```

### Comparing `tweetipy-0.1.8/LICENSE` & `tweetipy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/pyproject.toml` & `tweetipy-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "tweetipy"
-version = "0.1.8"
+version = "0.1.9"
 description = "A simple \"type hinted\" Python client for interacting with Twitter's API."
 authors = ["Federico Giancarelli <hello@federicogiancarelli.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omirete/tweetipy"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.11"
 requests = "^2.28.1"
 requests-oauthlib = "^1.3.1"
 segno = "^1.5.2"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `tweetipy-0.1.8/README.md` & `tweetipy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/enums/expansions/Tweet.py` & `tweetipy-0.1.9/tweetipy/enums/expansions/Tweet.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/enums/fields/_media/main.py` & `tweetipy-0.1.9/tweetipy/enums/fields/_media/main.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/enums/fields/_tweet/main.py` & `tweetipy-0.1.9/tweetipy/enums/fields/_tweet/main.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/handlers/Media.py` & `tweetipy-0.1.9/tweetipy/handlers/Media.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             endpoint,
             params=params
         )
         try:
             print(r.status_code)
             return _MediaUpload_INIT_Response(**r.json())
         except:
-            r.raise_for_status()
+            return r.raise_for_status()
     
     def _chunk_upload_APPEND(self, media_id: str, segment_index: int, media_bytes: bytes = None, media_data: bytes = None) -> bool:
         """
         HTTP 2XX will be returned with an empty response body on successful
         upload.
         """
         if (media_bytes != None) + (media_data != None) != 1:
```

### Comparing `tweetipy-0.1.8/tweetipy/handlers/Tweets.py` & `tweetipy-0.1.9/tweetipy/handlers/Tweets.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
         body = {
             "media": media.json() if media != None else None,
             "poll": poll.json() if poll != None else None,
             "quote_tweet_id": quote_tweet_id,
             "direct_message_deep_link": direct_message_deep_link,
             "for_super_followers_only": for_super_followers_only,
-            "reply": reply_config if in_reply_to_tweet_id != None else None,
+            "reply": reply_config.json() if in_reply_to_tweet_id != None else None,
             "reply_settings": reply_settings,
             "text": text,
         }
 
         # Remove unused params -------------------------------------------------
         clean_body = {}
         for key, val in body.items():
@@ -65,15 +65,15 @@
 
         r = self.API.post(url=endpoint, json=body)
         if r.status_code == 201:
             tweet_raw = r.json()["data"]
             return Tweet(**tweet_raw)
         else:
             print(r.text)
-            r.raise_for_status()
+            return r.raise_for_status()
     
     def search(
         self,
         query: Union[str, QueryStr],
         max_results: int = 10,
         sort_order: Literal["recency", "relevancy"] = "recency",
         start_time_iso: str = None,
@@ -113,15 +113,15 @@
                 raw_tweets = r_json["data"]
                 tweets = [Tweet(**t) for t in raw_tweets]
                 return tweets
             else:
                 return []
         else:
             print(r.text)
-            r.raise_for_status()
+            return r.raise_for_status()
 
     def getOne(
         self,
         id: str,
         include_media_fields: list[MediaFields] = [],
         include_place_fields: list[PlaceFields] = [PlaceFields.country, PlaceFields.full_name, PlaceFields.place_type],
         include_poll_fields: list[PollFields] = [],
@@ -171,8 +171,8 @@
                 try:
                     tweet_raw['includes'] = res_json["includes"]
                 except KeyError as e:
                     raise Exception(f'There was an error downloading the requested expansions. See details: {e}')
             return Tweet(**tweet_raw)
         else:
             print(r.text)
-            r.raise_for_status()
+            return r.raise_for_status()
```

### Comparing `tweetipy-0.1.8/tweetipy/helpers/API.py` & `tweetipy-0.1.9/tweetipy/helpers/API.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
             return OAuth1(
                 client_key=self.oauth_consumer_key,
                 client_secret=self.oauth_consumer_secret,
                 resource_owner_key=access_token,
                 resource_owner_secret=access_token_secret)
 
-    def __init__(self, oauth_consumer_key: str, oauth_consumer_secret: str, oauth_token: str = None, oauth_token_secret: str = None, session_path: PathLike = None) -> None:
+    def __init__(self, oauth_consumer_key: str, oauth_consumer_secret: str, oauth_token: str = None, oauth_token_secret: str = None, session_path: PathLike[str] = None) -> None:
         self.oauth_consumer_key = oauth_consumer_key
         self.oauth_consumer_secret = oauth_consumer_secret
         self.oauth_token = oauth_token
         self.oauth_token_secret = oauth_token_secret
         self.session_path = session_path if session_path != None else 'session.json'
         self.oauth = self.authorize()
```

### Comparing `tweetipy-0.1.8/tweetipy/helpers/QueryBuilder/alt.py` & `tweetipy-0.1.9/tweetipy/helpers/QueryBuilder/alt.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/helpers/QueryBuilder/lang.py` & `tweetipy-0.1.9/tweetipy/helpers/QueryBuilder/lang.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/helpers/QueryBuilder/main.py` & `tweetipy-0.1.9/tweetipy/helpers/QueryBuilder/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,17 @@
     def with_any_keyword(self, keywords: list[str]) -> QueryStr:
         """
         Will filter for tweets containing at least one of the keywords provided.
         """
         return self._return(f'({" OR ".join(keywords)})')
 
     def with_exact_string(self, string: str) -> QueryStr:
+        """
+        Will filter for tweets containing the exact string provided.
+        """
         return self._return(f'"{string}"')
 
     @property
     def has(self):
         """
         Filter for tweets that have media, links, geolocation data, etc.
         """
```

### Comparing `tweetipy-0.1.8/tweetipy/main.py` & `tweetipy-0.1.9/tweetipy/main.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/types/_includes/_main.py` & `tweetipy-0.1.9/tweetipy/types/_includes/_main.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/types/_place/_main.py` & `tweetipy-0.1.9/tweetipy/types/_place/_main.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/types/_scope/_main.py` & `tweetipy-0.1.9/tweetipy/types/_scope/_main.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/types/context_annotation/_main.py` & `tweetipy-0.1.9/tweetipy/types/context_annotation/_main.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/types/media/_main.py` & `tweetipy-0.1.9/tweetipy/types/media/_main.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/types/media/metrics/_organic.py` & `tweetipy-0.1.9/tweetipy/types/media/metrics/_organic.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/types/media/metrics/_promoted.py` & `tweetipy-0.1.9/tweetipy/types/media/metrics/_promoted.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/types/poll/_main.py` & `tweetipy-0.1.9/tweetipy/types/poll/_main.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/types/tweet/_main.py` & `tweetipy-0.1.9/tweetipy/types/tweet/_main.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/types/tweet/_reply_config.py` & `tweetipy-0.1.9/tweetipy/types/tweet/_reply_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from typing import Union
+
+
 class ReplyConfig():
-    def __init__(self, exclude_reply_user_ids: list[str], in_reply_to_tweet_id: str) -> None:
+    def __init__(self, exclude_reply_user_ids: Union[list[str], None], in_reply_to_tweet_id: Union[str, None]) -> None:
         """
         - exclude_reply_user_ids: A list of User IDs to be excluded from the
         reply Tweet thus removing a user from a thread.
         - in_reply_to_tweet_id: Tweet ID of the Tweet being replied to. Please
         note thatTweet ID of the Tweet being replied to. Please note that
         `in_reply_to_tweet_id` needs to be in the request if
         `exclude_reply_user_ids` is present.
```

### Comparing `tweetipy-0.1.8/tweetipy/types/tweet/metrics/_public.py` & `tweetipy-0.1.9/tweetipy/types/tweet/metrics/_public.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/types/user/_main.py` & `tweetipy-0.1.9/tweetipy/types/user/_main.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/tweetipy/types/user/metrics/_public.py` & `tweetipy-0.1.9/tweetipy/types/user/metrics/_public.py`

 * *Files identical despite different names*

### Comparing `tweetipy-0.1.8/setup.py` & `tweetipy-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 install_requires = \
 ['requests-oauthlib>=1.3.1,<2.0.0',
  'requests>=2.28.1,<3.0.0',
  'segno>=1.5.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'tweetipy',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'A simple "type hinted" Python client for interacting with Twitter\'s API.',
     'long_description': '# Tweetipy\nA simple type hinted Python client for interacting with Twitter\'s API.\n\n```\npip -m install tweetipy\n```\n\nTo use it, setup a developer account under [developer.twitter.com](https://developer.twitter.com/).\n\nAfter that, create an app from the [developer dashboard](https://developer.twitter.com/en/portal/dashboard) and generate the needed tokens ("API Key and Secret").\n\nPlease note that the library does not yet implement the full Twitter API, but rather only some endpoints that are interesting for my projects. Also, although it is already working, please be aware that this library is still in early development phase and thus breaking changes might occur. In other words, don\'t rely on it for production just yet.\n\nIn any case, feel free to use it for your own projects. Do create issues if anything weird pops up. Pull requests and feature requests are welcome!\n\n# Examples\n\n### Posting a tweet\n```python\nfrom tweetipy import Tweetipy\n\n# Initialize client\nttpy = Tweetipy(\n    \'YOUR_TWITTER_API_KEY\',\n    \'YOUR_TWITTER_API_KEY_SECRET\')\n\n# Post tweet to Twitter\ntweet = ttpy.tweets.write("I\'m using Twitter API!")\n\n# See the uploaded tweet! :)\nprint(tweet)\n```\n\n### Posting a tweet with media\n```python\nfrom tweetipy import Tweetipy\nfrom tweetipy.types import MediaToUpload\n\nttpy = Tweetipy(\n    \'YOUR_TWITTER_API_KEY\',\n    \'YOUR_TWITTER_API_KEY_SECRET\')\n\n# First upload the media to Twitter.\nwith open(\'dog.jpeg\', \'rb\') as pic:\n    uploaded_media = ttpy.media.upload(\n        media_bytes=pic.read(),\n        media_type="image/jpeg")\n\n# Then post a tweet, adding the media_id as a parameter.\nttpy.tweets.write(\n    "This tweet contains some media.",\n    media=MediaToUpload([uploaded_media.media_id_string]))\n```\n\n### Searching tweets\n```python\nfrom tweetipy import Tweetipy\n\n# Initialize the client\nttpy = Tweetipy(\n    \'YOUR_TWITTER_API_KEY\',\n    \'YOUR_TWITTER_API_KEY_SECRET\')\n\n# Treat the \'query\' argument as you would a search box.\nsearch_results = ttpy.tweets.search(query=\'space separated keywords\')\n\n\n# See results 🤩\nfor tweet in search_results:\n    print(tweet)\n```\n\n### Doing advanced searches - Single condition\n```python\nfrom tweetipy import Tweetipy\nfrom tweetipy.helpers import QueryBuilder\n\n# Initialize the client\nttpy = Tweetipy(\n    \'YOUR_TWITTER_API_KEY\',\n    \'YOUR_TWITTER_API_KEY_SECRET\')\n\n# The query builder is your friend :)\nt = QueryBuilder()\n\n# Define the search criteria using the query builder.\nsearch_results = ttpy.tweets.search(\n    query=t.from_user(\'Randogs8\'),\n    sort_order=\'recency\'\n)\n\n# See results 🤩\nfor tweet in search_results:\n    print(tweet)\n```\n\n### Doing advanced searches - Multiple conditions (AND)\n```python\nfrom tweetipy import Tweetipy\nfrom tweetipy.helpers import QueryBuilder\n\n# Initialize the client\nttpy = Tweetipy(\n    \'YOUR_TWITTER_API_KEY\',\n    \'YOUR_TWITTER_API_KEY_SECRET\')\n\n# The query builder is your friend :)\nt = QueryBuilder()\n\n# Use the \'and\' operator (&) to define alternative criteria.\n# The query builder will do some background work for you so this works as\n# expected. 😎\nsearch_results = ttpy.tweets.search(\n    query=t.with_all_keywords([\'dogs\', \'love\']) & t.has.media,\n    sort_order=\'relevancy\'\n)\n\n# See the results 🤩\nfor tweet in search_results:\n    print(tweet)\n```\n\n### Doing advanced searches - Multiple conditions (OR)\n```python\nfrom tweetipy import Tweetipy\nfrom tweetipy.helpers import QueryBuilder\n\n# Initialize the client\nttpy = Tweetipy(\n    \'YOUR_TWITTER_API_KEY\',\n    \'YOUR_TWITTER_API_KEY_SECRET\')\n\n# The query builder is your friend :)\nt = QueryBuilder()\n\n# Use the pipe operator (|) to define alternative criteria.\n# The query builder will do some background work for you so this works as\n# expected. 😎\nsearch_results = ttpy.tweets.search(\n    query=t.from_user(\'Randogs8\') | t.from_user(\'cooldogfacts\'),\n    sort_order=\'recency\'\n)\n\n# See the results 🤩\nfor tweet in search_results:\n    print(tweet)\n```\n',
     'author': 'Federico Giancarelli',
     'author_email': 'hello@federicogiancarelli.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/omirete/tweetipy',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.11,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `tweetipy-0.1.8/PKG-INFO` & `tweetipy-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: tweetipy
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple "type hinted" Python client for interacting with Twitter's API.
 Home-page: https://github.com/omirete/tweetipy
 License: MIT
 Author: Federico Giancarelli
 Author-email: hello@federicogiancarelli.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
 Requires-Dist: segno (>=1.5.2,<2.0.0)
 Project-URL: Repository, https://github.com/omirete/tweetipy
 Description-Content-Type: text/markdown
 
 # Tweetipy
```

