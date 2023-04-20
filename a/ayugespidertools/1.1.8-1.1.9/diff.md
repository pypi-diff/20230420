# Comparing `tmp/ayugespidertools-1.1.8.tar.gz` & `tmp/ayugespidertools-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-1.1.8.tar", max compression
+gzip compressed data, was "ayugespidertools-1.1.9.tar", max compression
```

## Comparing `ayugespidertools-1.1.8.tar` & `ayugespidertools-1.1.9.tar`

### file list

```diff
@@ -1,96 +1,115 @@
--rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-1.1.8/LICENSE
--rw-r--r--   0        0        0    13472 2023-04-14 08:11:10.000000 ayugespidertools-1.1.8/README.md
--rw-r--r--   0        0        0      201 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/AyuRequest.py
--rw-r--r--   0        0        0      108 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/AyugeCrawlSpider.py
--rw-r--r--   0        0        0       92 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/AyugeSpider.py
--rw-r--r--   0        0        0     8257 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/DownloaderMiddlewares.py
--rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-1.1.8/ayugespidertools/FormatData.py
--rw-r--r--   0        0        0     7681 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/ImgOperation.py
--rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-1.1.8/ayugespidertools/Items.py
--rw-r--r--   0        0        0      673 2023-02-17 07:53:37.000000 ayugespidertools-1.1.8/ayugespidertools/Middlewares.py
--rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/MongoClient.py
--rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/MysqlClient.py
--rw-r--r--   0        0        0     5475 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/Oss.py
--rw-r--r--   0        0        0      694 2023-02-17 07:53:37.000000 ayugespidertools-1.1.8/ayugespidertools/Pipelines.py
--rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/ProcessManager.py
--rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/RPA.py
--rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/RunJs.py
--rw-r--r--   0        0        0     6924 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/VerificationCode.py
--rw-r--r--   0        0        0      474 2023-02-24 06:05:27.000000 ayugespidertools-1.1.8/ayugespidertools/__init__.py
--rw-r--r--   0        0        0     7227 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0     7109 2023-03-29 02:02:32.428686 ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      685 2023-03-29 02:02:32.466687 ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
--rw-r--r--   0        0        0     2947 2023-03-29 02:02:32.473687 ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
--rw-r--r--   0        0        0     1158 2023-03-29 02:02:32.506687 ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
--rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-1.1.8/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     4072 2023-03-28 09:33:33.000000 ayugespidertools-1.1.8/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      626 2023-03-28 09:33:33.000000 ayugespidertools-1.1.8/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0     3704 2023-04-14 07:32:45.000000 ayugespidertools-1.1.8/ayugespidertools/common/Encryption.py
--rw-r--r--   0        0        0     6622 2023-04-14 08:08:19.000000 ayugespidertools-1.1.8/ayugespidertools/common/Expend.py
--rw-r--r--   0        0        0     3832 2023-04-11 07:28:36.000000 ayugespidertools-1.1.8/ayugespidertools/common/MongoDBPipe.py
--rw-r--r--   0        0        0    11869 2023-04-14 06:07:52.000000 ayugespidertools-1.1.8/ayugespidertools/common/MultiPlexing.py
--rw-r--r--   0        0        0    13474 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/common/MysqlErrorHandle.py
--rw-r--r--   0        0        0    32577 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/common/Params.py
--rw-r--r--   0        0        0     4264 2023-04-11 07:33:08.000000 ayugespidertools-1.1.8/ayugespidertools/common/SpiderDBConf.py
--rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-1.1.8/ayugespidertools/common/SqlFormat.py
--rw-r--r--   0        0        0     1421 2023-04-06 08:21:44.000000 ayugespidertools-1.1.8/ayugespidertools/common/TypeVars.py
--rw-r--r--   0        0        0    11610 2023-04-13 08:18:25.000000 ayugespidertools-1.1.8/ayugespidertools/common/Utils.py
--rw-r--r--   0        0        0     3693 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/common/YiDunGap.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-1.1.8/ayugespidertools/config.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      187 2023-02-17 07:53:37.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0      348 2023-03-29 02:02:28.613683 ayugespidertools-1.1.8/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1557 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1439 2023-03-29 02:02:28.615683 ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     8625 2023-03-29 02:02:28.620683 ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
--rw-r--r--   0        0        0    10545 2023-03-01 02:44:36.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0      970 2023-02-28 02:20:41.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0     1742 2023-04-11 07:50:13.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0     4275 2023-04-11 07:41:24.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/netlib/requestslib.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0     4244 2023-04-11 07:45:40.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2869 2023-04-11 07:45:43.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0    11208 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/proxy/private.py
--rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/download/image.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0     3022 2023-04-10 09:37:05.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0     1356 2023-04-12 02:07:09.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0    13312 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0     2823 2023-04-11 02:54:07.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     1754 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2840 2023-04-06 08:21:44.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3899 2023-04-11 03:05:04.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     6737 2023-04-10 01:20:43.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0     4569 2023-04-13 07:18:00.730130 ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      760 2023-04-13 07:18:02.706131 ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
--rw-r--r--   0        0        0     1213 2023-03-31 08:04:57.033997 ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__pycache__/init.cpython-38.pyc
--rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/.gitignore
--rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0      630 2023-04-06 08:21:44.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      535 2023-03-02 09:20:59.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/common/DataEnum.py.tmpl
--rw-r--r--   0        0        0      282 2023-01-29 07:51:47.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2023-01-29 07:51:47.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     4647 2023-04-14 08:26:26.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-1.1.8/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1654 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     6423 2023-03-14 08:48:24.000000 ayugespidertools-1.1.8/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1950 2023-02-03 02:54:13.000000 ayugespidertools-1.1.8/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-1.1.8/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-1.1.8/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-1.1.8/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0     5953 2023-02-10 19:57:28.000000 ayugespidertools-1.1.8/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     3094 2023-04-12 09:55:12.000000 ayugespidertools-1.1.8/pyproject.toml
--rw-r--r--   0        0        0    15149 1970-01-01 00:00:00.000000 ayugespidertools-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-1.1.9/LICENSE
+-rw-r--r--   0        0        0    13490 2023-04-18 02:43:49.000000 ayugespidertools-1.1.9/README.md
+-rw-r--r--   0        0        0      201 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/AyuRequest.py
+-rw-r--r--   0        0        0      108 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/AyugeCrawlSpider.py
+-rw-r--r--   0        0        0       92 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/AyugeSpider.py
+-rw-r--r--   0        0        0     8203 2023-04-19 06:53:29.000000 ayugespidertools-1.1.9/ayugespidertools/DownloaderMiddlewares.py
+-rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-1.1.9/ayugespidertools/FormatData.py
+-rw-r--r--   0        0        0     7681 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/ImgOperation.py
+-rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-1.1.9/ayugespidertools/Items.py
+-rw-r--r--   0        0        0      673 2023-02-17 07:53:37.000000 ayugespidertools-1.1.9/ayugespidertools/Middlewares.py
+-rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/MongoClient.py
+-rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/MysqlClient.py
+-rw-r--r--   0        0        0     5475 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/Oss.py
+-rw-r--r--   0        0        0      694 2023-02-17 07:53:37.000000 ayugespidertools-1.1.9/ayugespidertools/Pipelines.py
+-rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/ProcessManager.py
+-rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/RPA.py
+-rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/RunJs.py
+-rw-r--r--   0        0        0     6924 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/VerificationCode.py
+-rw-r--r--   0        0        0      474 2023-02-24 06:05:27.000000 ayugespidertools-1.1.9/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-1.1.9/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-18 06:47:49.372425 ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      536 2023-04-17 09:29:59.544907 ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc
+-rw-r--r--   0        0        0      685 2023-03-29 02:02:32.466687 ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
+-rw-r--r--   0        0        0     2914 2023-04-18 06:47:49.395425 ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
+-rw-r--r--   0        0        0     1086 2023-04-19 07:06:38.147286 ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
+-rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-1.1.9/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0     4170 2023-04-18 02:26:28.000000 ayugespidertools-1.1.9/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-1.1.9/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0     3704 2023-04-14 07:32:45.000000 ayugespidertools-1.1.9/ayugespidertools/common/Encryption.py
+-rw-r--r--   0        0        0     6622 2023-04-14 08:08:19.000000 ayugespidertools-1.1.9/ayugespidertools/common/Expend.py
+-rw-r--r--   0        0        0     3847 2023-04-20 03:24:39.000000 ayugespidertools-1.1.9/ayugespidertools/common/MongoDBPipe.py
+-rw-r--r--   0        0        0    11850 2023-04-18 08:38:38.000000 ayugespidertools-1.1.9/ayugespidertools/common/MultiPlexing.py
+-rw-r--r--   0        0        0    13474 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/common/MysqlErrorHandle.py
+-rw-r--r--   0        0        0    32577 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/common/Params.py
+-rw-r--r--   0        0        0     4264 2023-04-18 13:16:46.000000 ayugespidertools-1.1.9/ayugespidertools/common/SpiderDBConf.py
+-rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-1.1.9/ayugespidertools/common/SqlFormat.py
+-rw-r--r--   0        0        0     1514 2023-04-18 06:42:57.000000 ayugespidertools-1.1.9/ayugespidertools/common/TypeVars.py
+-rw-r--r--   0        0        0    10924 2023-04-18 09:04:47.000000 ayugespidertools-1.1.9/ayugespidertools/common/Utils.py
+-rw-r--r--   0        0        0     3693 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/common/YiDunGap.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-1.1.9/ayugespidertools/config.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      187 2023-02-17 07:53:37.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0      348 2023-03-29 02:02:28.613683 ayugespidertools-1.1.9/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1557 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1439 2023-03-29 02:02:28.615683 ayugespidertools-1.1.9/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8625 2023-03-29 02:02:28.620683 ayugespidertools-1.1.9/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
+-rw-r--r--   0        0        0    10545 2023-03-01 02:44:36.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0      970 2023-02-28 02:20:41.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0      813 2023-04-18 08:27:37.369445 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2248 2023-04-18 08:27:37.370445 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc
+-rw-r--r--   0        0        0     1742 2023-04-11 07:50:13.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0     2178 2023-04-18 08:27:37.372445 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc
+-rw-r--r--   0        0        0     4275 2023-04-11 07:41:24.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/netlib/requestslib.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0      175 2023-04-18 08:27:37.372445 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3927 2023-04-18 08:27:37.374445 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc
+-rw-r--r--   0        0        0     3051 2023-04-18 08:27:37.376445 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc
+-rw-r--r--   0        0        0     7802 2023-04-18 08:27:37.381445 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc
+-rw-r--r--   0        0        0     4244 2023-04-11 07:45:40.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2869 2023-04-11 07:45:43.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0    11208 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/private.py
+-rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0      885 2023-04-14 09:46:54.212591 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/download/image.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0      173 2023-04-14 09:46:54.212591 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3093 2023-04-14 09:46:54.213591 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc
+-rw-r--r--   0        0        0     1820 2023-04-14 09:46:54.217591 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc
+-rw-r--r--   0        0        0     3022 2023-04-10 09:37:05.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0     1356 2023-04-12 02:07:09.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0    13398 2023-04-18 06:55:07.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0    11211 2023-04-18 07:50:48.385727 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3005 2023-04-18 06:47:10.331390 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc
+-rw-r--r--   0        0        0      717 2023-04-14 09:46:54.228591 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc
+-rw-r--r--   0        0        0     1998 2023-04-14 09:46:54.228591 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc
+-rw-r--r--   0        0        0     3621 2023-04-18 06:47:10.350390 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc
+-rw-r--r--   0        0        0     2824 2023-04-18 06:45:18.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     1754 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2840 2023-04-06 08:21:44.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3897 2023-04-18 06:44:38.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     6737 2023-04-18 13:17:20.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0     4569 2023-04-18 13:18:47.788335 ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      760 2023-04-13 07:18:02.706131 ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
+-rw-r--r--   0        0        0     1213 2023-03-31 08:04:57.033997 ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__pycache__/init.cpython-38.pyc
+-rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/.gitignore
+-rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/README.md
+-rw-r--r--   0        0        0      627 2023-04-20 06:55:52.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      535 2023-03-02 09:20:59.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/common/DataEnum.py.tmpl
+-rw-r--r--   0        0        0      282 2023-01-29 07:51:47.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     4161 2023-04-19 03:35:24.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0     1654 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     6423 2023-03-14 08:48:24.000000 ayugespidertools-1.1.9/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1950 2023-02-03 02:54:13.000000 ayugespidertools-1.1.9/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-1.1.9/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-1.1.9/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-1.1.9/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-17 09:29:59.415907 ayugespidertools-1.1.9/ayugespidertools/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5360 2023-04-18 06:47:53.532429 ayugespidertools-1.1.9/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc
+-rw-r--r--   0        0        0     5953 2023-04-18 02:22:33.000000 ayugespidertools-1.1.9/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     3136 2023-04-19 07:13:26.000000 ayugespidertools-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0    15160 1970-01-01 00:00:00.000000 ayugespidertools-1.1.9/PKG-INFO
```

### Comparing `ayugespidertools-1.1.8/LICENSE` & `ayugespidertools-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/README.md` & `ayugespidertools-1.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ![ayugespidertools-logo](https://raw.githubusercontent.com/shengchenyang/AyugeSpiderTools/main/artwork/ayugespidertools-logo.png)
 
 [![OSCS Status](https://www.oscs1024.com/platform/badge/AyugeSpiderTools.svg?size=small)](https://www.murphysec.com/accept?code=0ec375759aebea7fd260248910b98806&type=1&from=2)
 ![GitHub](https://img.shields.io/github/license/shengchenyang/AyugeSpiderTools)
-![python](https://img.shields.io/badge/python-3.8%2B-blue)
+![python](https://img.shields.io/badge/python-3.8.1%2B-blue)
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/shengchenyang/AyugeSpiderTools/codeql.yml?branch=main)
 ![Read the Docs](https://img.shields.io/readthedocs/ayugespidertools)
 ![GitHub all releases](https://img.shields.io/github/downloads/shengchenyang/AyugeSpiderTools/total?label=releases%20downloads)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/AyugeSpiderTools?label=pypi%20downloads)
 
 # AyugeSpiderTools 工具说明
 
@@ -24,15 +24,15 @@
 
 > `python 3.8+` 可以直接输入以下命令：
 
 ```shell
 pip install ayugespidertools -i https://pypi.org/simple
 ```
 
-注：本库依赖中的 `pymongo` 版本要在 `3.12.3` 及以下是因为我的 `mongoDB` 的版本为 `3.4`，`pymogo` 官方从 `3.12.3` 以后的版本开始不再支持 `3.6` 版本以下的 `MongoDB` 数据库了，望周知！**你也可以根据 [3.3](#3.3.-Build-Your-Own-Library) 自定义库**
+注：本库依赖中的 `pymongo` 版本要在 `^3.12.3` (即`3.13.0` 及以下) 是因为我的 `mongoDB` 的版本为 `3.4`，`pymogo` 官方从 `3.13.0` 以后的版本开始不再支持 `3.6` 版本以下的 `MongoDB` 数据库了，望周知！**你也可以根据 [3.3](#3.3.-Build-Your-Own-Library) 自定义库**
 
 ## 2. 使用方法
 
 > 项目主要包含两部分：
 >
 
 - 开发场景中的工具库
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/DownloaderMiddlewares.py` & `ayugespidertools-1.1.9/ayugespidertools/DownloaderMiddlewares.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,14 @@
         # parse_result = urllib.parse.urlsplit(request.url)
         # domain = parse_result.hostname
 
         # _timeout = self.download_timeout
         # if aiohttp_meta.get('timeout') is not None:
         #     _timeout = aiohttp_meta.get('timeout')
 
-        spider.slog.debug(f"crawling {request.url}")
         html_content = None
         try:
             # 获取请求头信息
             aiohttp_headers = ToolsForAyu.get_dict_form_scrapy_req_headers(
                 scrapy_headers=request.headers
             )
             aiohttp_headers_args = {"headers": aiohttp_headers}
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/FormatData.py` & `ayugespidertools-1.1.9/ayugespidertools/FormatData.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/ImgOperation.py` & `ayugespidertools-1.1.9/ayugespidertools/ImgOperation.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/Items.py` & `ayugespidertools-1.1.9/ayugespidertools/Items.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/Middlewares.py` & `ayugespidertools-1.1.9/ayugespidertools/Middlewares.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/MongoClient.py` & `ayugespidertools-1.1.9/ayugespidertools/MongoClient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/MysqlClient.py` & `ayugespidertools-1.1.9/ayugespidertools/MysqlClient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/Oss.py` & `ayugespidertools-1.1.9/ayugespidertools/Oss.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/Pipelines.py` & `ayugespidertools-1.1.9/ayugespidertools/Pipelines.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/RPA.py` & `ayugespidertools-1.1.9/ayugespidertools/RPA.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/RunJs.py` & `ayugespidertools-1.1.9/ayugespidertools/RunJs.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/VerificationCode.py` & `ayugespidertools-1.1.9/ayugespidertools/VerificationCode.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc` & `ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc` & `ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Mar 28 09:33:33 2023 UTC, .py size: 4072 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6db4 2264 e80f 0000  U.......m."d....
+00000000: 550d 0d0a 0000 0000 d4ff 3d64 4a10 0000  U.........=dJ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6401 6c0d  m.Z.m.Z...d.d.l.
@@ -31,155 +31,153 @@
 000001e0: 7761 7265 732e 7079 2e74 6d70 6c29 0272  wares.py.tmpl).r
 000001f0: 0c00 0000 7a0b 7275 6e2e 7079 2e74 6d70  ....z.run.py.tmp
 00000200: 6c29 0272 0c00 0000 7a17 636f 6d6d 6f6e  l).r....z.common
 00000210: 2f44 6174 6145 6e75 6d2e 7079 2e74 6d70  /DataEnum.py.tmp
 00000220: 6c7a 052a 2e70 7963 da0b 5f5f 7079 6361  lz.*.pyc..__pyca
 00000230: 6368 655f 5f7a 042e 7376 6e63 0000 0000  che__z..svnc....
 00000240: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00000250: 4000 0000 7334 0000 0065 005a 0164 005a  @...s4...e.Z.d.Z
-00000260: 0264 015a 0364 0164 0264 039c 025a 0464  .d.Z.d.d.d...Z.d
-00000270: 0464 0584 005a 0565 0665 0764 069c 0164  .d...Z.e.e.d...d
-00000280: 0764 0884 0483 015a 0864 0953 0029 0ada  .d.....Z.d.S.)..
-00000290: 0a41 7975 436f 6d6d 616e 6446 5429 02da  .AyuCommandFT)..
-000002a0: 0b4c 4f47 5f45 4e41 424c 4544 da17 5350  .LOG_ENABLED..SP
-000002b0: 4944 4552 5f4c 4f41 4445 525f 5741 524e  IDER_LOADER_WARN
-000002c0: 5f4f 4e4c 5963 0300 0000 0000 0000 0000  _ONLYc..........
-000002d0: 0000 0900 0000 0700 0000 0300 0000 73a4  ..............s.
-000002e0: 0100 0074 007c 0183 0164 016b 0772 1274  ...t.|...d.k.r.t
-000002f0: 0183 0082 017c 0164 0219 0089 0074 007c  .....|.d.....t.|
-00000300: 0183 0164 036b 0272 3474 027c 0164 0419  ...d.k.r4t.|.d..
-00000310: 0083 017d 036e 0c74 027c 0164 0219 0083  ...}.n.t.|.d....
-00000320: 017d 037c 0364 051b 00a0 03a1 0072 6864  .}.|.d.......rhd
-00000330: 047c 005f 0474 0564 067c 03a0 06a1 009b  .|._.t.d.|......
-00000340: 009d 0283 0101 0064 0053 007c 00a0 0788  .......d.S.|....
-00000350: 00a1 0173 7c64 047c 005f 0464 0053 007c  ...s|d.|._.d.S.|
-00000360: 00a0 0874 027c 006a 0983 017c 03a0 06a1  ...t.|.j...|....
-00000370: 00a1 0201 0074 0a7c 0364 071b 007c 0388  .....t.|.d...|..
-00000380: 001b 0083 0201 0074 0b44 005d 347d 0474  .......t.D.]4}.t
-00000390: 027c 0366 0187 0066 0164 0864 0984 087c  .|.f...f.d.d...|
-000003a0: 0444 0083 019e 028e 007d 0574 0c7c 0588  .D.......}.t.|..
-000003b0: 0064 0a74 0d88 0083 0164 0b8d 0401 0071  .d.t.....d.....q
-000003c0: a87c 039b 0064 0c7c 039b 0064 0d9d 047d  .|...d.|...d...}
-000003d0: 0674 027c 0683 01a0 06a1 007d 0774 0e6a  .t.|.......}.t.j
-000003e0: 0f90 0172 2874 0564 0e83 0101 0074 027c  ...r(t.d.....t.|
-000003f0: 0683 017d 0874 02a0 037c 08a1 0190 0172  ...}.t...|.....r
-00000400: 467c 08a0 10a1 0001 006e 1e74 0c7c 067c  F|.......n.t.|.|
-00000410: 0774 0d74 117c 0783 0183 0188 0074 0d88  .t.t.|.......t..
-00000420: 0083 0164 0f8d 0501 0074 0564 1088 009b  ...d.....t.d....
-00000430: 0064 117c 006a 099b 0064 129d 0583 0101  .d.|.j...d......
-00000440: 0074 0564 137c 03a0 06a1 009b 0064 149d  .t.d.|.......d..
-00000450: 0383 0101 0074 0564 1583 0101 0074 0564  .....t.d.....t.d
-00000460: 167c 039b 009d 0283 0101 0074 0564 1783  .|.........t.d..
-00000470: 0101 0074 0564 1883 0101 0074 0564 1983  ...t.d.....t.d..
-00000480: 0101 0064 0053 0029 1a4e 2902 e901 0000  ...d.S.).N).....
-00000490: 00e9 0200 0000 7201 0000 0072 1200 0000  ......r....r....
-000004a0: 7211 0000 0072 0b00 0000 7a24 4572 726f  r....r....z$Erro
-000004b0: 723a 2073 6372 6170 792e 6366 6720 616c  r: scrapy.cfg al
-000004c0: 7265 6164 7920 6578 6973 7473 2069 6e20  ready exists in 
-000004d0: da06 6d6f 6475 6c65 6301 0000 0000 0000  ..modulec.......
-000004e0: 0000 0000 0002 0000 0004 0000 0033 0000  .............3..
-000004f0: 0073 2000 0000 7c00 5d18 7d01 7400 a001  .s ...|.].}.t...
-00000500: 7c01 a101 6a02 8800 6400 8d01 5600 0100  |...j...d...V...
-00000510: 7102 6401 5300 2902 a901 da0c 7072 6f6a  q.d.S.).....proj
-00000520: 6563 745f 6e61 6d65 4e29 03da 0673 7472  ect_nameN)...str
-00000530: 696e 67da 0854 656d 706c 6174 65da 0a73  ing..Template..s
-00000540: 7562 7374 6974 7574 6529 02da 022e 30da  ubstitute)....0.
-00000550: 0173 7214 0000 00a9 00fa 472f 726f 6f74  .sr.......G/root
-00000560: 2f6d 7970 726f 6a2f 4179 7567 6553 7069  /myproj/AyugeSpi
-00000570: 6465 7254 6f6f 6c73 2f61 7975 6765 7370  derTools/ayugesp
-00000580: 6964 6572 746f 6f6c 732f 636f 6d6d 616e  idertools/comman
-00000590: 6473 2f73 7461 7274 7072 6f6a 6563 742e  ds/startproject.
-000005a0: 7079 da09 3c67 656e 6578 7072 3e3e 0000  py..<genexpr>>..
-000005b0: 0073 0400 0000 0402 02ff 7a21 4179 7543  .s........z!AyuC
-000005c0: 6f6d 6d61 6e64 2e72 756e 2e3c 6c6f 6361  ommand.run.<loca
-000005d0: 6c73 3e2e 3c67 656e 6578 7072 3e7a 0324  ls>.<genexpr>z.$
-000005e0: 7079 2903 7215 0000 00da 0270 79da 0b50  py).r......py..P
-000005f0: 726f 6a65 6374 4e61 6d65 fa01 2f7a 0c2f  rojectName../z./
-00000600: 7275 6e2e 7368 2e74 6d70 6c7a 3a49 6e66  run.sh.tmplz:Inf
-00000610: 6f3a 2054 6865 2072 756e 2e73 6820 6669  o: The run.sh fi
-00000620: 6c65 2069 7320 6e6f 206c 6f6e 6765 7220  le is no longer 
-00000630: 6765 6e65 7261 7465 6420 756e 6465 7220  generated under 
-00000640: 7769 6e64 6f77 7329 045a 1370 726f 6a65  windows).Z.proje
-00000650: 6374 5f73 7461 7274 7570 5f64 6972 5a11  ct_startup_dirZ.
-00000660: 5072 6f6a 6563 7453 7461 7274 7570 4469  ProjectStartupDi
-00000670: 7272 1500 0000 721f 0000 007a 144e 6577  rr....r....z.New
-00000680: 2053 6372 6170 7920 7072 6f6a 6563 7420   Scrapy project 
-00000690: 277a 1d27 2c20 7573 696e 6720 7465 6d70  'z.', using temp
-000006a0: 6c61 7465 2064 6972 6563 746f 7279 2027  late directory '
-000006b0: 7a0e 272c 2063 7265 6174 6564 2069 6e3a  z.', created in:
-000006c0: 7a04 2020 2020 da01 0a7a 2559 6f75 2063  z.    ...z%You c
-000006d0: 616e 2073 7461 7274 2079 6f75 7220 6669  an start your fi
-000006e0: 7273 7420 7370 6964 6572 2077 6974 683a  rst spider with:
-000006f0: 7a07 2020 2020 6364 207a 2820 2020 2073  z.    cd z(    s
-00000700: 6372 6170 7920 6765 6e73 7069 6465 7220  crapy genspider 
-00000710: 6578 616d 706c 6520 6578 616d 706c 652e  example example.
-00000720: 636f 6d7a 394f 7220 796f 7520 6361 6e20  comz9Or you can 
-00000730: 7374 6172 7420 796f 7572 2066 6972 7374  start your first
-00000740: 2073 7069 6465 7220 7769 7468 2061 7975   spider with ayu
-00000750: 6765 7370 6964 6572 746f 6f6c 733a 7a32  gespidertools:z2
-00000760: 2020 2020 6179 7567 6573 7069 6465 7274      ayugespidert
-00000770: 6f6f 6c73 2067 656e 7370 6964 6572 2065  ools genspider e
-00000780: 7861 6d70 6c65 2065 7861 6d70 6c65 2e63  xample example.c
-00000790: 6f6d 2912 da03 6c65 6e72 0600 0000 7202  om)...lenr....r.
-000007a0: 0000 00da 0665 7869 7374 73da 0865 7869  .....exists..exi
-000007b0: 7463 6f64 65da 0570 7269 6e74 da07 7265  tcode..print..re
-000007c0: 736f 6c76 655a 0e5f 6973 5f76 616c 6964  solveZ._is_valid
-000007d0: 5f6e 616d 65da 095f 636f 7079 7472 6565  _name.._copytree
-000007e0: da0d 7465 6d70 6c61 7465 735f 6469 7272  ..templates_dirr
-000007f0: 0400 0000 da13 5445 4d50 4c41 5445 535f  ......TEMPLATES_
-00000800: 544f 5f52 454e 4445 5272 0700 0000 7208  TO_RENDERr....r.
-00000810: 0000 0072 0900 0000 da0a 4953 5f57 494e  ...r......IS_WIN
-00000820: 444f 5753 da06 756e 6c69 6e6b da03 7374  DOWS..unlink..st
-00000830: 7229 09da 0473 656c 66da 0461 7267 73da  r)...self..args.
-00000840: 046f 7074 735a 0b70 726f 6a65 6374 5f64  .optsZ.project_d
-00000850: 6972 da05 7061 7468 735a 0774 706c 6669  ir..pathsZ.tplfi
-00000860: 6c65 5a0e 7275 6e5f 7368 656c 6c5f 7061  leZ.run_shell_pa
-00000870: 7468 5a11 7275 6e5f 7368 656c 6c5f 6162  thZ.run_shell_ab
-00000880: 7370 6174 685a 0864 656c 5f66 696c 6572  spathZ.del_filer
-00000890: 1b00 0000 7214 0000 0072 1c00 0000 da03  ....r....r......
-000008a0: 7275 6e25 0000 0073 6800 0000 0001 0c01  run%...sh.......
-000008b0: 0602 0802 0c01 0e02 0c02 0c01 0601 1201  ................
-000008c0: 0402 0a01 0601 0402 1601 1201 0801 0201  ................
-000008d0: 02ff 0202 0a02 02fe 04fe 0607 0201 0201  ................
-000008e0: 0202 0201 06fb 0809 1001 0c02 0801 0801  ................
-000008f0: 0801 0c01 0a03 0201 0201 0201 0a01 0201  ................
-00000900: 06fb 0608 0201 12ff 0404 1401 0801 0e01  ................
-00000910: 0802 0801 7a0e 4179 7543 6f6d 6d61 6e64  ....z.AyuCommand
-00000920: 2e72 756e 2901 da06 7265 7475 726e 6301  .run)...returnc.
-00000930: 0000 0000 0000 0000 0000 0001 0000 0005  ................
-00000940: 0000 0043 0000 0073 1a00 0000 7400 7401  ...C...s....t.t.
-00000950: 7401 7402 6a03 6401 1900 6402 8302 6403  t.t.j.d...d...d.
-00000960: 8302 8301 5300 2904 4e72 0100 0000 da09  ....S.).Nr......
-00000970: 7465 6d70 6c61 7465 73da 0770 726f 6a65  templates..proje
-00000980: 6374 2904 722c 0000 0072 0200 0000 da10  ct).r,...r......
-00000990: 6179 7567 6573 7069 6465 7274 6f6f 6c73  ayugespidertools
-000009a0: da08 5f5f 7061 7468 5f5f 2901 722d 0000  ..__path__).r-..
-000009b0: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-000009c0: 7228 0000 006a 0000 0073 0c00 0000 0003  r(...j...s......
-000009d0: 0201 0201 0e01 02fe 02ff 7a18 4179 7543  ..........z.AyuC
-000009e0: 6f6d 6d61 6e64 2e74 656d 706c 6174 6573  ommand.templates
-000009f0: 5f64 6972 4e29 09da 085f 5f6e 616d 655f  _dirN)...__name_
-00000a00: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000a10: 5f71 7561 6c6e 616d 655f 5fda 1072 6571  _qualname__..req
-00000a20: 7569 7265 735f 7072 6f6a 6563 74da 1064  uires_project..d
-00000a30: 6566 6175 6c74 5f73 6574 7469 6e67 7372  efault_settingsr
-00000a40: 3100 0000 da08 7072 6f70 6572 7479 722c  1.....propertyr,
-00000a50: 0000 0072 2800 0000 721b 0000 0072 1b00  ...r(...r....r..
-00000a60: 0000 721b 0000 0072 1c00 0000 720e 0000  ..r....r....r...
-00000a70: 0021 0000 0073 0a00 0000 0801 0401 0a02  .!...s..........
-00000a80: 0845 0201 720e 0000 0029 1372 1600 0000  .E..r....).r....
-00000a90: da07 7061 7468 6c69 6272 0200 0000 da06  ..pathlibr......
-00000aa0: 7368 7574 696c 7203 0000 0072 0400 0000  shutilr....r....
-00000ab0: 5a1c 7363 7261 7079 2e63 6f6d 6d61 6e64  Z.scrapy.command
-00000ac0: 732e 7374 6172 7470 726f 6a65 6374 7205  s.startprojectr.
-00000ad0: 0000 00da 1173 6372 6170 792e 6578 6365  .....scrapy.exce
-00000ae0: 7074 696f 6e73 7206 0000 00da 1573 6372  ptionsr......scr
-00000af0: 6170 792e 7574 696c 732e 7465 6d70 6c61  apy.utils.templa
-00000b00: 7465 7207 0000 0072 0800 0000 7235 0000  ter....r....r5..
-00000b10: 00da 1e61 7975 6765 7370 6964 6572 746f  ...ayugespiderto
-00000b20: 6f6c 732e 636f 6d6d 6f6e 2e50 6172 616d  ols.common.Param
-00000b30: 7372 0900 0000 7229 0000 005a 0649 474e  sr....r)...Z.IGN
-00000b40: 4f52 4572 0e00 0000 721b 0000 0072 1b00  OREr....r....r..
-00000b50: 0000 721b 0000 0072 1c00 0000 da08 3c6d  ..r....r......<m
-00000b60: 6f64 756c 653e 0100 0000 7314 0000 0008  odule>....s.....
-00000b70: 010c 0110 020c 010c 0110 0208 010c 0304  ................
-00000b80: 110c 03                                  ...
+00000250: 4000 0000 7326 0000 0065 005a 0164 005a  @...s&...e.Z.d.Z
+00000260: 0264 0164 0284 005a 0365 0465 0564 039c  .d.d...Z.e.e.d..
+00000270: 0164 0464 0584 0483 015a 0664 0653 0029  .d.d.....Z.d.S.)
+00000280: 07da 0a41 7975 436f 6d6d 616e 6463 0300  ...AyuCommandc..
+00000290: 0000 0000 0000 0000 0000 0a00 0000 0700  ................
+000002a0: 0000 0300 0000 73c2 0100 0074 007c 0183  ......s....t.|..
+000002b0: 0164 016b 0772 1274 0183 0082 017c 0164  .d.k.r.t.....|.d
+000002c0: 0219 0089 0074 007c 0183 0164 036b 0272  .....t.|...d.k.r
+000002d0: 3864 047d 0374 027c 0164 0519 0083 017d  8d.}.t.|.d.....}
+000002e0: 046e 1064 067d 0374 027c 0164 0219 0083  .n.d.}.t.|.d....
+000002f0: 017d 047c 0464 071b 00a0 03a1 0072 7064  .}.|.d.......rpd
+00000300: 057c 005f 0474 0564 087c 04a0 06a1 009b  .|._.t.d.|......
+00000310: 009d 0283 0101 0064 0053 007c 00a0 0788  .......d.S.|....
+00000320: 00a1 0173 8464 057c 005f 0464 0053 007c  ...s.d.|._.d.S.|
+00000330: 00a0 0874 027c 006a 0983 017c 04a0 06a1  ...t.|.j...|....
+00000340: 00a1 0201 0074 0a7c 0464 091b 007c 0488  .....t.|.d...|..
+00000350: 001b 0083 0201 0074 0b44 005d 347d 0574  .......t.D.]4}.t
+00000360: 027c 0466 0187 0066 0164 0a64 0b84 087c  .|.f...f.d.d...|
+00000370: 0544 0083 019e 028e 007d 0674 0c7c 0688  .D.......}.t.|..
+00000380: 0064 0c74 0d88 0083 0164 0d8d 0401 0071  .d.t.....d.....q
+00000390: b07c 0372 fc7c 049b 0064 0e88 009b 0064  .|.r.|...d.....d
+000003a0: 0f9d 047d 076e 107c 049b 0064 0e7c 049b  ...}.n.|...d.|..
+000003b0: 0064 0f9d 047d 0774 027c 0483 01a0 06a1  .d...}.t.|......
+000003c0: 007d 0874 0e6a 0f90 0172 4674 0564 1083  .}.t.j...rFt.d..
+000003d0: 0101 0074 027c 0783 017d 0974 02a0 037c  ...t.|...}.t...|
+000003e0: 09a1 0190 0172 647c 09a0 10a1 0001 006e  .....rd|.......n
+000003f0: 1e74 0c7c 077c 0874 0d74 117c 0883 0183  .t.|.|.t.t.|....
+00000400: 0188 0074 0d88 0083 0164 118d 0501 0074  ...t.....d.....t
+00000410: 0564 1288 009b 0064 137c 006a 099b 0064  .d.....d.|.j...d
+00000420: 149d 0583 0101 0074 0564 157c 04a0 06a1  .......t.d.|....
+00000430: 009b 0064 169d 0383 0101 0074 0564 1783  ...d.......t.d..
+00000440: 0101 0074 0564 187c 049b 009d 0283 0101  ...t.d.|........
+00000450: 0074 0564 1983 0101 0074 0564 1a83 0101  .t.d.....t.d....
+00000460: 0074 0564 1b83 0101 0064 0053 0029 1c4e  .t.d.....d.S.).N
+00000470: 2902 e901 0000 00e9 0200 0000 7201 0000  )...........r...
+00000480: 0072 1000 0000 5472 0f00 0000 4672 0b00  .r....Tr....Fr..
+00000490: 0000 7a24 4572 726f 723a 2073 6372 6170  ..z$Error: scrap
+000004a0: 792e 6366 6720 616c 7265 6164 7920 6578  y.cfg already ex
+000004b0: 6973 7473 2069 6e20 da06 6d6f 6475 6c65  ists in ..module
+000004c0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000004d0: 0004 0000 0033 0000 0073 2000 0000 7c00  .....3...s ...|.
+000004e0: 5d18 7d01 7400 a001 7c01 a101 6a02 8800  ].}.t...|...j...
+000004f0: 6400 8d01 5600 0100 7102 6401 5300 2902  d...V...q.d.S.).
+00000500: a901 da0c 7072 6f6a 6563 745f 6e61 6d65  ....project_name
+00000510: 4e29 03da 0673 7472 696e 67da 0854 656d  N)...string..Tem
+00000520: 706c 6174 65da 0a73 7562 7374 6974 7574  plate..substitut
+00000530: 6529 02da 022e 30da 0173 7212 0000 00a9  e)....0..sr.....
+00000540: 00fa 472f 726f 6f74 2f6d 7970 726f 6a2f  ..G/root/myproj/
+00000550: 4179 7567 6553 7069 6465 7254 6f6f 6c73  AyugeSpiderTools
+00000560: 2f61 7975 6765 7370 6964 6572 746f 6f6c  /ayugespidertool
+00000570: 732f 636f 6d6d 616e 6473 2f73 7461 7274  s/commands/start
+00000580: 7072 6f6a 6563 742e 7079 da09 3c67 656e  project.py..<gen
+00000590: 6578 7072 3e3d 0000 0073 0400 0000 0402  expr>=...s......
+000005a0: 02ff 7a21 4179 7543 6f6d 6d61 6e64 2e72  ..z!AyuCommand.r
+000005b0: 756e 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  un.<locals>.<gen
+000005c0: 6578 7072 3e7a 0324 7079 2903 7213 0000  expr>z.$py).r...
+000005d0: 00da 0270 79da 0b50 726f 6a65 6374 4e61  ...py..ProjectNa
+000005e0: 6d65 fa01 2f7a 0c2f 7275 6e2e 7368 2e74  me../z./run.sh.t
+000005f0: 6d70 6c7a 3a49 6e66 6f3a 2054 6865 2072  mplz:Info: The r
+00000600: 756e 2e73 6820 6669 6c65 2069 7320 6e6f  un.sh file is no
+00000610: 206c 6f6e 6765 7220 6765 6e65 7261 7465   longer generate
+00000620: 6420 756e 6465 7220 7769 6e64 6f77 7329  d under windows)
+00000630: 045a 1370 726f 6a65 6374 5f73 7461 7274  .Z.project_start
+00000640: 7570 5f64 6972 5a11 5072 6f6a 6563 7453  up_dirZ.ProjectS
+00000650: 7461 7274 7570 4469 7272 1300 0000 721d  tartupDirr....r.
+00000660: 0000 007a 144e 6577 2053 6372 6170 7920  ...z.New Scrapy 
+00000670: 7072 6f6a 6563 7420 277a 1d27 2c20 7573  project 'z.', us
+00000680: 696e 6720 7465 6d70 6c61 7465 2064 6972  ing template dir
+00000690: 6563 746f 7279 2027 7a0e 272c 2063 7265  ectory 'z.', cre
+000006a0: 6174 6564 2069 6e3a 7a04 2020 2020 da01  ated in:z.    ..
+000006b0: 0a7a 2559 6f75 2063 616e 2073 7461 7274  .z%You can start
+000006c0: 2079 6f75 7220 6669 7273 7420 7370 6964   your first spid
+000006d0: 6572 2077 6974 683a 7a07 2020 2020 6364  er with:z.    cd
+000006e0: 207a 2820 2020 2073 6372 6170 7920 6765   z(    scrapy ge
+000006f0: 6e73 7069 6465 7220 6578 616d 706c 6520  nspider example 
+00000700: 6578 616d 706c 652e 636f 6d7a 394f 7220  example.comz9Or 
+00000710: 796f 7520 6361 6e20 7374 6172 7420 796f  you can start yo
+00000720: 7572 2066 6972 7374 2073 7069 6465 7220  ur first spider 
+00000730: 7769 7468 2061 7975 6765 7370 6964 6572  with ayugespider
+00000740: 746f 6f6c 733a 7a32 2020 2020 6179 7567  tools:z2    ayug
+00000750: 6573 7069 6465 7274 6f6f 6c73 2067 656e  espidertools gen
+00000760: 7370 6964 6572 2065 7861 6d70 6c65 2065  spider example e
+00000770: 7861 6d70 6c65 2e63 6f6d 2912 da03 6c65  xample.com)...le
+00000780: 6e72 0600 0000 7202 0000 00da 0665 7869  nr....r......exi
+00000790: 7374 73da 0865 7869 7463 6f64 65da 0570  sts..exitcode..p
+000007a0: 7269 6e74 da07 7265 736f 6c76 655a 0e5f  rint..resolveZ._
+000007b0: 6973 5f76 616c 6964 5f6e 616d 65da 095f  is_valid_name.._
+000007c0: 636f 7079 7472 6565 da0d 7465 6d70 6c61  copytree..templa
+000007d0: 7465 735f 6469 7272 0400 0000 da13 5445  tes_dirr......TE
+000007e0: 4d50 4c41 5445 535f 544f 5f52 454e 4445  MPLATES_TO_RENDE
+000007f0: 5272 0700 0000 7208 0000 0072 0900 0000  Rr....r....r....
+00000800: da0a 4953 5f57 494e 444f 5753 da06 756e  ..IS_WINDOWS..un
+00000810: 6c69 6e6b da03 7374 7229 0ada 0473 656c  link..str)...sel
+00000820: 66da 0461 7267 73da 046f 7074 735a 155f  f..args..optsZ._
+00000830: 6861 735f 7072 6f6a 6563 745f 6469 725f  has_project_dir_
+00000840: 6172 6773 da0b 7072 6f6a 6563 745f 6469  args..project_di
+00000850: 72da 0570 6174 6873 5a07 7470 6c66 696c  r..pathsZ.tplfil
+00000860: 655a 0e72 756e 5f73 6865 6c6c 5f70 6174  eZ.run_shell_pat
+00000870: 685a 1172 756e 5f73 6865 6c6c 5f61 6273  hZ.run_shell_abs
+00000880: 7061 7468 5a08 6465 6c5f 6669 6c65 7219  pathZ.del_filer.
+00000890: 0000 0072 1200 0000 721a 0000 00da 0372  ...r....r......r
+000008a0: 756e 2200 0000 7370 0000 0000 010c 0106  un"...sp........
+000008b0: 0208 020c 0104 010e 0204 010c 020c 0106  ................
+000008c0: 0112 0104 020a 0106 0104 0216 0112 0108  ................
+000008d0: 0102 0102 ff02 020a 0202 fe04 fe06 0702  ................
+000008e0: 0102 0102 0202 0106 fb08 0904 0112 0210  ................
+000008f0: 010c 0208 0108 0108 010c 010a 0302 0102  ................
+00000900: 0102 010a 0102 0106 fb06 0802 0112 ff04  ................
+00000910: 0414 0108 010e 0108 0208 017a 0e41 7975  ...........z.Ayu
+00000920: 436f 6d6d 616e 642e 7275 6e29 01da 0672  Command.run)...r
+00000930: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
+00000940: 0000 0100 0000 0500 0000 4300 0000 731a  ..........C...s.
+00000950: 0000 0074 0074 0174 0174 026a 0364 0119  ...t.t.t.t.j.d..
+00000960: 0064 0283 0264 0383 0283 0153 0029 044e  .d...d.....S.).N
+00000970: 7201 0000 00da 0974 656d 706c 6174 6573  r......templates
+00000980: da07 7072 6f6a 6563 7429 0472 2a00 0000  ..project).r*...
+00000990: 7202 0000 00da 1061 7975 6765 7370 6964  r......ayugespid
+000009a0: 6572 746f 6f6c 73da 085f 5f70 6174 685f  ertools..__path_
+000009b0: 5f29 0172 2b00 0000 7219 0000 0072 1900  _).r+...r....r..
+000009c0: 0000 721a 0000 0072 2600 0000 6c00 0000  ..r....r&...l...
+000009d0: 730c 0000 0000 0302 0102 010e 0102 fe02  s...............
+000009e0: ff7a 1841 7975 436f 6d6d 616e 642e 7465  .z.AyuCommand.te
+000009f0: 6d70 6c61 7465 735f 6469 724e 2907 da08  mplates_dirN)...
+00000a00: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000a10: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000a20: 5f5f 7230 0000 00da 0870 726f 7065 7274  __r0.....propert
+00000a30: 7972 2a00 0000 7226 0000 0072 1900 0000  yr*...r&...r....
+00000a40: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00000a50: 0e00 0000 2100 0000 7306 0000 0008 0108  ....!...s.......
+00000a60: 4a02 0172 0e00 0000 2913 7214 0000 00da  J..r....).r.....
+00000a70: 0770 6174 686c 6962 7202 0000 00da 0673  .pathlibr......s
+00000a80: 6875 7469 6c72 0300 0000 7204 0000 005a  hutilr....r....Z
+00000a90: 1c73 6372 6170 792e 636f 6d6d 616e 6473  .scrapy.commands
+00000aa0: 2e73 7461 7274 7072 6f6a 6563 7472 0500  .startprojectr..
+00000ab0: 0000 da11 7363 7261 7079 2e65 7863 6570  ....scrapy.excep
+00000ac0: 7469 6f6e 7372 0600 0000 da15 7363 7261  tionsr......scra
+00000ad0: 7079 2e75 7469 6c73 2e74 656d 706c 6174  py.utils.templat
+00000ae0: 6572 0700 0000 7208 0000 0072 3400 0000  er....r....r4...
+00000af0: da1e 6179 7567 6573 7069 6465 7274 6f6f  ..ayugespidertoo
+00000b00: 6c73 2e63 6f6d 6d6f 6e2e 5061 7261 6d73  ls.common.Params
+00000b10: 7209 0000 0072 2700 0000 5a06 4947 4e4f  r....r'...Z.IGNO
+00000b20: 5245 720e 0000 0072 1900 0000 7219 0000  REr....r....r...
+00000b30: 0072 1900 0000 721a 0000 00da 083c 6d6f  .r....r......<mo
+00000b40: 6475 6c65 3e01 0000 0073 1400 0000 0801  dule>....s......
+00000b50: 0c01 1002 0c01 0c01 1002 0801 0c03 0411  ................
+00000b60: 0c03                                     ..
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/commands/__pycache__/version.cpython-38.pyc` & `ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/version.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Mar 28 09:33:33 2023 UTC, .py size: 626 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,68 @@
-00000000: 550d 0d0a 0000 0000 6db4 2264 7202 0000  U.......m."dr...
+00000000: 550d 0d0a 0000 0000 6bff 3d64 0c02 0000  U.......k.=d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 6502 8303 5a05 6401  d.d...d.e...Z.d.
 00000060: 5300 2906 e900 0000 004e 2901 da07 436f  S.)......N)...Co
 00000070: 6d6d 616e 6429 01da 0c4e 6f72 6d61 6c43  mmand)...NormalC
 00000080: 6f6e 6669 6763 0000 0000 0000 0000 0000  onfigc..........
-00000090: 0000 0000 0000 0300 0000 4000 0000 7334  ..........@...s4
-000000a0: 0000 0065 005a 0164 005a 0264 0164 0264  ...e.Z.d.Z.d.d.d
-000000b0: 039c 025a 0364 0464 0584 005a 0465 0564  ...Z.d.d...Z.e.d
-000000c0: 069c 0164 0764 0884 045a 0664 0964 0a84  ...d.d...Z.d.d..
-000000d0: 005a 0764 0b53 0029 0cda 0a41 7975 436f  .Z.d.S.)...AyuCo
-000000e0: 6d6d 616e 6446 5429 02da 0b4c 4f47 5f45  mmandFT)...LOG_E
-000000f0: 4e41 424c 4544 da17 5350 4944 4552 5f4c  NABLED..SPIDER_L
-00000100: 4f41 4445 525f 5741 524e 5f4f 4e4c 5963  OADER_WARN_ONLYc
-00000110: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000120: 0100 0000 4300 0000 7304 0000 0064 0153  ....C...s....d.S
-00000130: 0029 024e 7a1e 5072 696e 7420 4179 7567  .).Nz.Print Ayug
-00000140: 6553 7069 6465 7254 6f6f 6c73 2076 6572  eSpiderTools ver
-00000150: 7369 6f6e a900 2901 da04 7365 6c66 7207  sion..)...selfr.
-00000160: 0000 0072 0700 0000 fa42 2f72 6f6f 742f  ...r.....B/root/
-00000170: 6d79 7072 6f6a 2f41 7975 6765 5370 6964  myproj/AyugeSpid
-00000180: 6572 546f 6f6c 732f 6179 7567 6573 7069  erTools/ayugespi
-00000190: 6465 7274 6f6f 6c73 2f63 6f6d 6d61 6e64  dertools/command
-000001a0: 732f 7665 7273 696f 6e2e 7079 da0a 7368  s/version.py..sh
-000001b0: 6f72 745f 6465 7363 0a00 0000 7302 0000  ort_desc....s...
-000001c0: 0000 017a 1541 7975 436f 6d6d 616e 642e  ...z.AyuCommand.
-000001d0: 7368 6f72 745f 6465 7363 2901 da06 7265  short_desc)...re
-000001e0: 7475 726e 6301 0000 0000 0000 0000 0000  turnc...........
-000001f0: 0003 0000 0009 0000 0043 0000 0073 3c00  .........C...s<.
-00000200: 0000 7400 7401 6a02 9b00 6401 9d02 6402  ..t.t.j...d...d.
-00000210: 6403 6404 8d03 8f10 7d01 7403 a004 7c01  d.d.....}.t...|.
-00000220: a101 7d02 5700 3500 5100 5200 5800 7c02  ..}.W.5.Q.R.X.|.
-00000230: 6405 1900 6406 1900 6407 1900 5300 2908  d...d...d...S.).
-00000240: 4e7a 0f2f 7079 7072 6f6a 6563 742e 746f  Nz./pyproject.to
-00000250: 6d6c da01 727a 0575 7466 2d38 2901 da08  ml..rz.utf-8)...
-00000260: 656e 636f 6469 6e67 da04 746f 6f6c 5a06  encoding..toolZ.
-00000270: 706f 6574 7279 da07 7665 7273 696f 6e29  poetry..version)
-00000280: 05da 046f 7065 6e72 0300 0000 da08 524f  ...openr......RO
-00000290: 4f54 5f44 4952 da04 746f 6d6c da04 6c6f  OT_DIR..toml..lo
-000002a0: 6164 2903 7208 0000 00da 0166 da06 636f  ad).r......f..co
-000002b0: 6e66 6967 7207 0000 0072 0700 0000 7209  nfigr....r....r.
-000002c0: 0000 00da 085f 7665 7273 696f 6e0d 0000  ....._version...
-000002d0: 0073 1000 0000 0001 0201 0a00 0200 02ff  .s..............
-000002e0: 0602 0201 1402 7a13 4179 7543 6f6d 6d61  ......z.AyuComma
-000002f0: 6e64 2e5f 7665 7273 696f 6e63 0300 0000  nd._versionc....
-00000300: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00000310: 4300 0000 7316 0000 0074 0064 017c 00a0  C...s....t.d.|..
-00000320: 01a1 009b 009d 0283 0101 0064 0053 0029  ...........d.S.)
-00000330: 024e 7a11 4179 7567 6553 7069 6465 7254  .Nz.AyugeSpiderT
-00000340: 6f6f 6c73 2029 02da 0570 7269 6e74 7216  ools )...printr.
-00000350: 0000 0029 0372 0800 0000 da04 6172 6773  ...).r......args
-00000360: da04 6f70 7473 7207 0000 0072 0700 0000  ..optsr....r....
-00000370: 7209 0000 00da 0372 756e 1500 0000 7302  r......run....s.
-00000380: 0000 0000 017a 0e41 7975 436f 6d6d 616e  .....z.AyuComman
-00000390: 642e 7275 6e4e 2908 da08 5f5f 6e61 6d65  d.runN)...__name
-000003a0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-000003b0: 5f5f 7175 616c 6e61 6d65 5f5f da10 6465  __qualname__..de
-000003c0: 6661 756c 745f 7365 7474 696e 6773 720a  fault_settingsr.
-000003d0: 0000 00da 0373 7472 7216 0000 0072 1a00  .....strr....r..
-000003e0: 0000 7207 0000 0072 0700 0000 7207 0000  ..r....r....r...
-000003f0: 0072 0900 0000 7204 0000 0007 0000 0073  .r....r........s
-00000400: 0800 0000 0801 0a02 0803 0e08 7204 0000  ............r...
-00000410: 0029 0672 1200 0000 5a17 7363 7261 7079  .).r....Z.scrapy
-00000420: 2e63 6f6d 6d61 6e64 732e 7665 7273 696f  .commands.versio
-00000430: 6e72 0200 0000 da17 6179 7567 6573 7069  nr......ayugespi
-00000440: 6465 7274 6f6f 6c73 2e63 6f6e 6669 6772  dertools.configr
-00000450: 0300 0000 7204 0000 0072 0700 0000 7207  ....r....r....r.
-00000460: 0000 0072 0700 0000 7209 0000 00da 083c  ...r....r......<
-00000470: 6d6f 6475 6c65 3e01 0000 0073 0600 0000  module>....s....
-00000480: 0801 0c02 0c03                           ......
+00000090: 0000 0000 0000 0300 0000 4000 0000 732a  ..........@...s*
+000000a0: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
+000000b0: 005a 0365 0464 039c 0164 0464 0584 045a  .Z.e.d...d.d...Z
+000000c0: 0564 0664 0784 005a 0664 0853 0029 09da  .d.d...Z.d.S.)..
+000000d0: 0a41 7975 436f 6d6d 616e 6463 0100 0000  .AyuCommandc....
+000000e0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+000000f0: 4300 0000 7304 0000 0064 0153 0029 024e  C...s....d.S.).N
+00000100: 7a1e 5072 696e 7420 4179 7567 6553 7069  z.Print AyugeSpi
+00000110: 6465 7254 6f6f 6c73 2076 6572 7369 6f6e  derTools version
+00000120: a900 2901 da04 7365 6c66 7205 0000 0072  ..)...selfr....r
+00000130: 0500 0000 fa42 2f72 6f6f 742f 6d79 7072  .....B/root/mypr
+00000140: 6f6a 2f41 7975 6765 5370 6964 6572 546f  oj/AyugeSpiderTo
+00000150: 6f6c 732f 6179 7567 6573 7069 6465 7274  ols/ayugespidert
+00000160: 6f6f 6c73 2f63 6f6d 6d61 6e64 732f 7665  ools/commands/ve
+00000170: 7273 696f 6e2e 7079 da0a 7368 6f72 745f  rsion.py..short_
+00000180: 6465 7363 0800 0000 7302 0000 0000 017a  desc....s......z
+00000190: 1541 7975 436f 6d6d 616e 642e 7368 6f72  .AyuCommand.shor
+000001a0: 745f 6465 7363 2901 da06 7265 7475 726e  t_desc)...return
+000001b0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+000001c0: 0009 0000 0043 0000 0073 3c00 0000 7400  .....C...s<...t.
+000001d0: 7401 6a02 9b00 6401 9d02 6402 6403 6404  t.j...d...d.d.d.
+000001e0: 8d03 8f10 7d01 7403 a004 7c01 a101 7d02  ....}.t...|...}.
+000001f0: 5700 3500 5100 5200 5800 7c02 6405 1900  W.5.Q.R.X.|.d...
+00000200: 6406 1900 6407 1900 5300 2908 4e7a 0f2f  d...d...S.).Nz./
+00000210: 7079 7072 6f6a 6563 742e 746f 6d6c da01  pyproject.toml..
+00000220: 727a 0575 7466 2d38 2901 da08 656e 636f  rz.utf-8)...enco
+00000230: 6469 6e67 da04 746f 6f6c 5a06 706f 6574  ding..toolZ.poet
+00000240: 7279 da07 7665 7273 696f 6e29 05da 046f  ry..version)...o
+00000250: 7065 6e72 0300 0000 da08 524f 4f54 5f44  penr......ROOT_D
+00000260: 4952 da04 746f 6d6c da04 6c6f 6164 2903  IR..toml..load).
+00000270: 7206 0000 00da 0166 da06 636f 6e66 6967  r......f..config
+00000280: 7205 0000 0072 0500 0000 7207 0000 00da  r....r....r.....
+00000290: 085f 7665 7273 696f 6e0b 0000 0073 1000  ._version....s..
+000002a0: 0000 0001 0201 0a00 0200 02ff 0602 0201  ................
+000002b0: 1402 7a13 4179 7543 6f6d 6d61 6e64 2e5f  ..z.AyuCommand._
+000002c0: 7665 7273 696f 6e63 0300 0000 0000 0000  versionc........
+000002d0: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
+000002e0: 7316 0000 0074 0064 017c 00a0 01a1 009b  s....t.d.|......
+000002f0: 009d 0283 0101 0064 0053 0029 024e 7a11  .......d.S.).Nz.
+00000300: 4179 7567 6553 7069 6465 7254 6f6f 6c73  AyugeSpiderTools
+00000310: 2029 02da 0570 7269 6e74 7214 0000 0029   )...printr....)
+00000320: 0372 0600 0000 da04 6172 6773 da04 6f70  .r......args..op
+00000330: 7473 7205 0000 0072 0500 0000 7207 0000  tsr....r....r...
+00000340: 00da 0372 756e 1300 0000 7302 0000 0000  ...run....s.....
+00000350: 017a 0e41 7975 436f 6d6d 616e 642e 7275  .z.AyuCommand.ru
+00000360: 6e4e 2907 da08 5f5f 6e61 6d65 5f5f da0a  nN)...__name__..
+00000370: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000380: 616c 6e61 6d65 5f5f 7208 0000 00da 0373  alname__r......s
+00000390: 7472 7214 0000 0072 1800 0000 7205 0000  trr....r....r...
+000003a0: 0072 0500 0000 7205 0000 0072 0700 0000  .r....r....r....
+000003b0: 7204 0000 0007 0000 0073 0600 0000 0801  r........s......
+000003c0: 0803 0e08 7204 0000 0029 0672 1000 0000  ....r....).r....
+000003d0: 5a17 7363 7261 7079 2e63 6f6d 6d61 6e64  Z.scrapy.command
+000003e0: 732e 7665 7273 696f 6e72 0200 0000 da17  s.versionr......
+000003f0: 6179 7567 6573 7069 6465 7274 6f6f 6c73  ayugespidertools
+00000400: 2e63 6f6e 6669 6772 0300 0000 7204 0000  .configr....r...
+00000410: 0072 0500 0000 7205 0000 0072 0500 0000  .r....r....r....
+00000420: 7207 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000430: 0000 0073 0600 0000 0801 0c02 0c03       ...s..........
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/commands/startproject.py` & `ayugespidertools-1.1.9/ayugespidertools/commands/startproject.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,26 +27,25 @@
     ("${project_name}", "common/DataEnum.py.tmpl"),
 )
 
 IGNORE = ignore_patterns("*.pyc", "__pycache__", ".svn")
 
 
 class AyuCommand(Command):
-    requires_project = False
-    default_settings = {"LOG_ENABLED": False, "SPIDER_LOADER_WARN_ONLY": True}
-
     def run(self, args, opts):
         if len(args) not in (1, 2):
             raise UsageError()
 
         project_name = args[0]
 
         if len(args) == 2:
+            _has_project_dir_args = True
             project_dir = Path(args[1])
         else:
+            _has_project_dir_args = False
             project_dir = Path(args[0])
 
         if (project_dir / "scrapy.cfg").exists():
             self.exitcode = 1
             print(f"Error: scrapy.cfg already exists in {project_dir.resolve()}")
             return
 
@@ -69,16 +68,19 @@
                 project_name=project_name,
                 # 这个 py 就只为了处理模板中 .gitignore 多余的 $py 干扰
                 py="$py",
                 ProjectName=string_camelcase(project_name),
             )
 
         # 添加执行 shell 文件 run.sh 的生成
-        run_shell_path = f"{project_dir}/{project_dir}/run.sh.tmpl"
-        run_shell_abspath = Path(run_shell_path).resolve()
+        if _has_project_dir_args:
+            run_shell_path = f"{project_dir}/{project_name}/run.sh.tmpl"
+        else:
+            run_shell_path = f"{project_dir}/{project_dir}/run.sh.tmpl"
+        run_shell_abspath = Path(project_dir).resolve()
         # 如果是 windows 环境的话，就不生成 shell 文件了，没啥必要
         if Param.IS_WINDOWS:
             print("Info: The run.sh file is no longer generated under windows")
             del_file = Path(run_shell_path)
             if Path.exists(del_file):
                 del_file.unlink()
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/common/Encryption.py` & `ayugespidertools-1.1.9/ayugespidertools/common/Encryption.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/common/Expend.py` & `ayugespidertools-1.1.9/ayugespidertools/common/Expend.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/common/MongoDBPipe.py` & `ayugespidertools-1.1.9/ayugespidertools/common/MongoDBPipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 
 
 class AbstractClass(ABC):
     """
     用于处理 mysql 异常的模板方法类
     """
 
-    def _get_collection_name(self, collection_prefix: str, table: str) -> str:
+    def _get_collection_name(self, table: str, collection_prefix: str = "") -> str:
         """
         获取集合名称
         Args:
-            collection_prefix: 集合前缀
             table: item 中的 table 字段
+            collection_prefix: 集合前缀
 
         Returns:
             full_collection_name: 完整的集合名称
         """
         assert isinstance(table, str), "item 中 table 字段不是 str，或未传入 table 参数"
         full_collection_name = f"""{collection_prefix}{table}"""
 
@@ -35,15 +35,15 @@
         ), "集合名不能含空格，请检查 MONGODB_COLLECTION_PREFIX 参数和 item 中的 table 参数"
         return full_collection_name
 
     def template_method(
         self,
         item_dict: ItemAdapter,
         db: Param.PymongoDataBase,
-        collection_prefix: str,
+        collection_prefix: str = "",
     ) -> None:
         """
         模板方法，用于 mongodb 存储场景
         Args:
             item_dict: item ItemAdapter 格式数据，可像字典一样操作
             db: mongodb 数据库连接
             collection_prefix: 集合前缀
@@ -72,15 +72,15 @@
             insert_data = ReuseOperation.get_items_except_keys(
                 dict_conf=item_dict,
                 key_list=["table", "item_mode", "mongo_update_rule"],
             )
 
         # 真实的集合名称为：集合前缀名 + 集合名称
         collection_name = self._get_collection_name(
-            collection_prefix=collection_prefix, table=item_dict["table"]
+            table=item_dict["table"], collection_prefix=collection_prefix
         )
         # 如果没有查重字段时，就直接插入数据（不去重）
         if not item_dict.get("mongo_update_rule"):
             db[collection_name].insert(insert_data)
         else:
             db[collection_name].update(
                 item_dict["mongo_update_rule"], {"$set": insert_data}, True
@@ -110,12 +110,12 @@
         pass
 
 
 def mongodb_pipe(
     abstract_class: AbstractClass,
     item_dict: ItemAdapter,
     db: Param.PymongoDataBase,
-    collection_prefix: str,
+    collection_prefix: str = "",
 ) -> None:
     abstract_class.template_method(
         item_dict=item_dict, db=db, collection_prefix=collection_prefix
     )
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/common/MultiPlexing.py` & `ayugespidertools-1.1.9/ayugespidertools/common/MultiPlexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,29 +165,29 @@
         return all(key in dict_conf for key in key_list)
 
     @classmethod
     def get_items_by_keys(
         cls,
         dict_conf: dict,
         key_list: List[str],
-    ) -> Union[dict, bool]:
+    ) -> dict:
         """
         获取 dict_conf 中的含有 key_list 的 key 的字段
         Args:
             dict_conf: 需要处理的参数
             key_list: 需要取的 key 值列表
 
         Returns:
             1). 取值后的 dict，或不满足请求的 False 值
         """
-        # 参数先要满足最小限定，然后再取出限定的参数值；否则直接返回 False
+        # 参数先要满足最小限定，然后再取出限定的参数值；否则返回空字典
         return (
             {k: dict_conf[k] for k in key_list}
             if cls.is_dict_meet_min_limit(dict_conf=dict_conf, key_list=key_list)
-            else False
+            else {}
         )
 
     @classmethod
     def get_items_except_keys(cls, dict_conf, key_list: List[str]) -> dict:
         """
         获取 dict_conf 中的不含有 key_list 的 key 的字段
         Args:
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/common/MysqlErrorHandle.py` & `ayugespidertools-1.1.9/ayugespidertools/common/MysqlErrorHandle.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/common/Params.py` & `ayugespidertools-1.1.9/ayugespidertools/common/Params.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/common/SpiderDBConf.py` & `ayugespidertools-1.1.9/ayugespidertools/common/SpiderDBConf.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/common/SqlFormat.py` & `ayugespidertools-1.1.9/ayugespidertools/common/SqlFormat.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/common/TypeVars.py` & `ayugespidertools-1.1.9/ayugespidertools/common/TypeVars.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # such as NoneType = type(None), etc.
 from enum import Enum, unique
 from typing import NamedTuple, Optional, TypedDict, TypeVar
 
 __all__ = [
     "TableTemplate",
     "TableEnumTypeVar",
+    "AlterItem",
     "MysqlConfig",
     "MongoDBConfig",
 ]
 
 TableEnumTypeVar = TypeVar("TableEnumTypeVar", bound="TableEnum")
 
 
@@ -49,7 +50,12 @@
 class MongoDBConfig(NamedTuple):
     host: str
     port: int
     user: str
     password: str
     database: Optional[str] = None
     authsource: Optional[str] = None
+
+
+class AlterItem(NamedTuple):
+    new_item: dict
+    notes_dic: dict
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/common/Utils.py` & `ayugespidertools-1.1.9/ayugespidertools/common/Utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,45 +17,24 @@
 from ayugespidertools.config import logger
 from ayugespidertools.FormatData import DataHandle
 
 __all__ = [
     "ToolsForAyu",
 ]
 
-ConsulFormatStr = Literal["JSON", "HCL", "YAML", "XML"]
+ConsulFormatStr = Literal["json", "hcl", "yaml", "xml"]
 ConsulConfNameStr = Literal["MONGODB", "MYSQL"]
 
 
 class ToolsForAyu(object):
     """
     这里用于存放框架所依赖的方法
     """
 
     @classmethod
-    def consul_get_all_group(cls, host: str, port: int, token: str) -> list:
-        """
-        获取 consul 的所有 group 信息
-        Args:
-            host: host
-            port: port
-            token: 请求 consul 所需要的 token 值
-
-        Returns:
-            1). consul 的所有 group 信息
-        """
-        curr_consul_headers = copy.deepcopy(Param.consul_headers)
-        curr_consul_headers["X-Consul-Token"] = token
-        r = requests.get(
-            url=f"http://{host}:{port}/v1/kv/?keys&dc=dc1&separator=%2F",
-            headers=curr_consul_headers,
-            verify=False,
-        )
-        return r.json()
-
-    @classmethod
     def get_kvs_detail_by_consul(
         cls,
         url: str,
         token: Optional[str] = None,
     ) -> str:
         """
         获取 consul 的 key_values 的详细信息
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/common/YiDunGap.py` & `ayugespidertools-1.1.9/ayugespidertools/common/YiDunGap.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-1.1.9/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc` & `ayugespidertools-1.1.9/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/http/request/form.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/http/request/form.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/netlib/requestslib.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/netlib/requestslib.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/middlewares/proxy/private.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/private.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/__init__.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/download/file.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/download/file.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/download/image.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/download/image.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mongo/fantasy.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/fantasy.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mongo/twisted.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/twisted.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pymysql
 from retrying import retry
 
 from ayugespidertools.common.Expend import MysqlPipeEnhanceMixin
 from ayugespidertools.common.MultiPlexing import ReuseOperation
 from ayugespidertools.common.MysqlErrorHandle import Synchronize, deal_mysql_err
 from ayugespidertools.common.Params import Param
-from ayugespidertools.common.TypeVars import MysqlConfig, TableEnumTypeVar
+from ayugespidertools.common.TypeVars import AlterItem, MysqlConfig, TableEnumTypeVar
 from ayugespidertools.common.Utils import ToolsForAyu
 
 # 将 pymysql 中 Data truncated for column 警告类型置为 Error，其他警告忽略
 warnings.filterwarnings(
     "error", category=pymysql.Warning, message=".*Data truncated for column.*"
 )
 
@@ -90,19 +90,19 @@
 
         # 最终的数据表名不能含有空格
         assert (
             " " not in full_table_name
         ), "数据表名不能含空格，请检查 MYSQL_TABLE_PREFIX 参数和 item 中的 table 参数"
         return full_table_name
 
-    def get_new_item(self, item):
+    def get_new_item(self, item) -> AlterItem:
         """
         重新整合 item
         Args:
-            item: scrapy yield 的 item 信息
+            item: scrapy item
 
         Returns:
             1). 整合后的 item
         """
         new_item = {}
         notes_dic = {}
         # 如果是 ayugespidertools.Items 中的各个自封装类型时
@@ -133,39 +133,40 @@
             save_data_item = ReuseOperation.get_items_except_keys(
                 dict_conf=item, key_list=["table", "item_mode"]
             )
             for key, value in save_data_item.items():
                 new_item[key] = value
                 notes_dic[key] = key
 
-        return {"new_item": new_item, "notes_dic": notes_dic}
+        return AlterItem(new_item=new_item, notes_dic=notes_dic)
 
     def process_item(self, item, spider):
         item_dict = ToolsForAyu.convert_items_to_dict(item)
         # 先查看存储场景是否匹配
         if item_dict["item_mode"] == "Mysql":
             self.insert_item(
-                self.get_new_item(item_dict), self.get_table_name(item_dict["table"])
+                alter_item=self.get_new_item(item_dict),
+                table=self.get_table_name(item_dict["table"]),
             )
         return item
 
-    def insert_item(self, item_o, table):
+    def insert_item(self, alter_item: AlterItem, table: str):
         """
         通用插入数据，将 item 数据存入 Mysql 中，item 中的 key 需要跟 Mysql 数据中的字段名称一致
         Args:
-            item_o: item
+            alter_item: 经过转变后的 item
             table: 数据库表名
 
         Returns:
             None
         """
-        if not (new_item := item_o.get("new_item")):
+        if not (new_item := alter_item.new_item):
             return
 
-        note_dic = item_o.get("notes_dic")
+        note_dic = alter_item.notes_dic
         sql = self._get_sql_by_item(table=table, item=new_item)
 
         try:
             if self.cursor.execute(sql, tuple(new_item.values()) * 2):
                 self.conn.commit()
 
         except Exception as e:
@@ -181,15 +182,15 @@
                 collate=self.collate,
                 database=self.mysql_conf.database,
                 table=table,
                 table_prefix=self.table_prefix,
                 table_enum=self.table_enum,
                 note_dic=note_dic,
             )
-            return self.insert_item(item_o, table)
+            return self.insert_item(alter_item, table)
 
     def close_spider(self, spider):
         # 是否记录程序采集的基本信息到 Mysql 中，只有打开 record_log_to_mysql 配置才会收集和存储相关的统计信息
         if self.record_log_to_mysql:
             log_info = self._get_log_by_spider(
                 spider=spider, crawl_time=self.crawl_time
             )
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/asynced.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/asynced.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,19 @@
         self.tasks.append(task)
         return item
 
     async def insert_item(self, item, spider):
         async with self.pool.acquire() as aiomysql_conn:
             async with aiomysql_conn.cursor() as aiomysql_cursor:
                 item_dict = ToolsForAyu.convert_items_to_dict(item)
-                item_o = super(AsyncMysqlPipeline, self).get_new_item(item_dict)
+                alter_item = super(AsyncMysqlPipeline, self).get_new_item(item_dict)
                 table = super(AsyncMysqlPipeline, self).get_table_name(
                     item_dict["table"]
                 )
-                new_item = item_o.get("new_item")
+                new_item = alter_item.new_item
                 keys = f"""`{"`, `".join(new_item.keys())}`"""
                 values = ", ".join(["%s"] * len(new_item))
                 update = ",".join([f" `{key}` = %s" for key in new_item])
                 sql = f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
 
                 await aiomysql_cursor.execute(sql, tuple(new_item.values()) * 2)
                 await aiomysql_conn.commit()
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/turbo.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/turbo.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/pipelines/mysql/twisted.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/twisted.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,21 +58,21 @@
         # 先查看存储场景是否匹配
         if item_dict["item_mode"] == "Mysql":
             query = self.dbpool.runInteraction(self.db_insert, item_dict)
             query.addErrback(self.handle_error, item)
         return item
 
     def db_insert(self, cursor, item):
-        item_o = super(AyuTwistedMysqlPipeline, self).get_new_item(item)
+        alter_item = super(AyuTwistedMysqlPipeline, self).get_new_item(item)
         table = super(AyuTwistedMysqlPipeline, self).get_table_name(item["table"])
 
-        if not (new_item := item_o.get("new_item")):
+        if not (new_item := alter_item.new_item):
             return
 
-        note_dic = item_o.get("notes_dic")
+        note_dic = alter_item.notes_dic
         sql = self._get_sql_by_item(table=table, item=new_item)
 
         try:
             cursor.execute(sql, tuple(new_item.values()) * 2)
 
         except Exception as e:
             self.slog.warning(f":{e}")
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__init__.py` & `ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Apr 10 01:20:43 2023 UTC, .py size: 6737 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6b64 3364 511a 0000  U.......kd3dQ...
+00000000: 550d 0d0a 0000 0000 6098 3e64 511a 0000  U.......`.>dQ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6400 6406 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -87,44 +87,44 @@
 00000560: 890a 2020 2020 46e9 0300 0000 e9ff ffff  ..    F.........
 00000570: ffda 0364 6576 2905 da0e 524f 424f 5453  ...dev)...ROBOTS
 00000580: 5458 545f 4f42 4559 5a15 5445 4c4e 4554  TXT_OBEYZ.TELNET
 00000590: 434f 4e53 4f4c 455f 454e 4142 4c45 44da  CONSOLE_ENABLED.
 000005a0: 0b52 4554 5259 5f54 494d 4553 da0e 4445  .RETRY_TIMES..DE
 000005b0: 5054 485f 5052 494f 5249 5459 da03 454e  PTH_PRIORITY..EN
 000005c0: 56da 0544 4542 5547 e914 0000 00da 0474  V..DEBUG.......t
-000005d0: 6573 744e 2909 5a09 4c4f 475f 4c45 5645  estN).Z.LOG_LEVE
+000005d0: 6573 744e 2909 da09 4c4f 475f 4c45 5645  estN)...LOG_LEVE
 000005e0: 4c72 2200 0000 5a10 444f 574e 4c4f 4144  Lr"...Z.DOWNLOAD
 000005f0: 5f54 494d 454f 5554 7223 0000 005a 1052  _TIMEOUTr#...Z.R
 00000600: 4544 4952 4543 545f 454e 4142 4c45 4472  EDIRECT_ENABLEDr
 00000610: 2400 0000 7225 0000 00da 0944 4154 415f  $...r%.....DATA_
-00000620: 454e 554d 5a13 5245 434f 5244 5f4c 4f47  ENUMZ.RECORD_LOG
+00000620: 454e 554d da13 5245 434f 5244 5f4c 4f47  ENUM..RECORD_LOG
 00000630: 5f54 4f5f 4d59 5351 4cda 0545 5252 4f52  _TO_MYSQL..ERROR
 00000640: da04 7072 6f64 7a08 2559 2d25 6d2d 2564  ..prodz.%Y-%m-%d
 00000650: da06 636f 6d6d 6f6e da00 6302 0000 0000  ..common..c.....
 00000660: 0000 0000 0000 0003 0000 0003 0000 000b  ................
 00000670: 0000 0073 1800 0000 7400 7401 7c00 8302  ...s....t.t.|...
 00000680: 6a02 7c01 6601 7c02 8e01 0100 6401 5300  j.|.f.|.....d.S.
 00000690: 2902 753d 0000 000a 2020 2020 2020 2020  ).u=....        
 000006a0: e5ae 9ee7 8eb0 e689 80e7 bba7 e689 bfe7  ................
 000006b0: b1bb e79a 8420 6162 7374 7261 6374 20e6  ..... abstract .
 000006c0: 96b9 e6b3 9520 7061 7273 650a 2020 2020  ..... parse.    
 000006d0: 2020 2020 4e29 03da 0573 7570 6572 7209      N)...superr.
 000006e0: 0000 00da 0570 6172 7365 2903 720c 0000  .....parse).r...
 000006f0: 00da 0872 6573 706f 6e73 6572 1800 0000  ...responser....
 00000700: a901 da09 5f5f 636c 6173 735f 5f72 0e00  ....__class__r..
-00000710: 0000 720f 0000 0072 2f00 0000 6400 0000  ..r....r/...d...
+00000710: 0000 720f 0000 0072 3100 0000 6400 0000  ..r....r1...d...
 00000720: 7302 0000 0000 047a 0f41 7975 5370 6964  s......z.AyuSpid
 00000730: 6572 2e70 6172 7365 6301 0000 0000 0000  er.parsec.......
 00000740: 0000 0000 0003 0000 0003 0000 000f 0000  ................
 00000750: 0073 1c00 0000 7400 7401 7c00 8302 6a02  .s....t.t.|...j.
 00000760: 7c01 7c02 8e01 0100 6400 7c00 5f03 6400  |.|.....d.|._.d.
-00000770: 5300 2901 4e29 0472 2e00 0000 7209 0000  S.).N).r....r...
+00000770: 5300 2901 4e29 0472 3000 0000 7209 0000  S.).N).r0...r...
 00000780: 0072 1000 0000 da0c 6d79 7371 6c5f 656e  .r......mysql_en
 00000790: 6769 6e65 2903 720c 0000 0072 1700 0000  gine).r....r....
-000007a0: 7218 0000 0072 3100 0000 720e 0000 0072  r....r1...r....r
+000007a0: 7218 0000 0072 3300 0000 720e 0000 0072  r....r3...r....r
 000007b0: 0f00 0000 7210 0000 006a 0000 0073 0400  ....r....j...s..
 000007c0: 0000 0001 1201 7a12 4179 7553 7069 6465  ......z.AyuSpide
 000007d0: 722e 5f5f 696e 6974 5f5f 6301 0000 0000  r.__init__c.....
 000007e0: 0000 0000 0000 0003 0000 0004 0000 0003  ................
 000007f0: 0000 0073 4c00 0000 7c00 6a00 6a01 a002  ...sL...|.j.j...
 00000800: 6401 a101 7d01 7c00 6a00 6a01 a002 6402  d...}.|.j.j...d.
 00000810: 6403 a102 7d02 7403 7c02 7404 8302 7330  d...}.t.|.t...s0
@@ -159,39 +159,39 @@
 000009e0: 5552 555f 454e 4142 4c45 4454 7529 0000  URU_ENABLEDTu)..
 000009f0: 006c 6f67 7572 755f 656e 6162 6c65 6420  .loguru_enabled 
 00000a00: e58f 82e6 95b0 e6a0 bce5 bc8f e99c 80e8  ................
 00000a10: a681 e4b8 ba20 626f 6f6c 4e29 09da 0763  ..... boolN)...c
 00000a20: 7261 776c 6572 da08 7365 7474 696e 6773  rawler..settings
 00000a30: da03 6765 74da 0a69 7369 6e73 7461 6e63  ..get..isinstanc
 00000a40: 65da 0462 6f6f 6cda 0e41 7373 6572 7469  e..bool..Asserti
-00000a50: 6f6e 4572 726f 7272 0800 0000 722e 0000  onErrorr....r...
+00000a50: 6f6e 4572 726f 7272 0800 0000 7230 0000  onErrorr....r0..
 00000a60: 0072 0900 0000 2903 720c 0000 005a 0f6c  .r....).r....Z.l
 00000a70: 6f67 7572 755f 636f 6e66 5f74 6d70 5a0e  oguru_conf_tmpZ.
-00000a80: 6c6f 6775 7275 5f65 6e61 626c 6564 7231  loguru_enabledr1
+00000a80: 6c6f 6775 7275 5f65 6e61 626c 6564 7233  loguru_enabledr3
 00000a90: 0000 0072 0e00 0000 720f 0000 00da 0473  ...r....r......s
 00000aa0: 6c6f 676e 0000 0073 0c00 0000 000a 0e02  logn...s........
 00000ab0: 1001 1203 0402 0804 7a0e 4179 7553 7069  ........z.AyuSpi
 00000ac0: 6465 722e 736c 6f67 6302 0000 0000 0000  der.slogc.......
 00000ad0: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
 00000ae0: 0073 5e00 0000 7400 7c00 6401 6400 8303  .s^...t.|.d.d...
 00000af0: 7d02 7400 7c00 6402 6403 8303 7d03 7400  }.t.|.d.d...}.t.
 00000b00: 7c00 6404 7c03 9b00 6405 9d03 6900 8303  |.d.|...d...i...
 00000b10: 7d04 7c02 7238 7c02 7c04 6406 3c00 7c01  }.|.r8|.|.d.<.|.
 00000b20: 6a01 7c04 6407 6408 8d02 0100 7c01 6a01  j.|.d.d.....|.j.
 00000b30: 7c00 6a02 7052 6900 6409 6408 8d02 0100  |.j.pRi.d.d.....
 00000b40: 6400 5300 290a 4eda 1163 7573 746f 6d5f  d.S.).N..custom_
 00000b50: 7461 626c 655f 656e 756d da0d 7365 7474  table_enum..sett
-00000b60: 696e 6773 5f74 7970 6572 2c00 0000 5a07  ings_typer,...Z.
+00000b60: 696e 6773 5f74 7970 6572 2e00 0000 5a07  ings_typer....Z.
 00000b70: 6375 7374 6f6d 5fda 095f 7365 7474 696e  custom_.._settin
-00000b80: 6773 7229 0000 005a 0770 726f 6a65 6374  gsr)...Z.project
+00000b80: 6773 722a 0000 00da 0770 726f 6a65 6374  gsr*.....project
 00000b90: 2901 da08 7072 696f 7269 7479 da06 7370  )...priority..sp
 00000ba0: 6964 6572 2903 da07 6765 7461 7474 72da  ider)...getattr.
 00000bb0: 0773 6574 6469 6374 da0f 6375 7374 6f6d  .setdict..custom
 00000bc0: 5f73 6574 7469 6e67 7329 0572 1600 0000  _settings).r....
-00000bd0: 7235 0000 0072 3b00 0000 723c 0000 005a  r5...r;...r<...Z
+00000bd0: 7237 0000 0072 3d00 0000 723e 0000 005a  r7...r=...r>...Z
 00000be0: 0e69 6e6e 6572 5f73 6574 7469 6e67 7372  .inner_settingsr
 00000bf0: 0e00 0000 720e 0000 0072 0f00 0000 da0f  ....r....r......
 00000c00: 7570 6461 7465 5f73 6574 7469 6e67 7386  update_settings.
 00000c10: 0000 0073 0e00 0000 0002 0c02 0c02 1402  ...s............
 00000c20: 0401 0804 0e01 7a19 4179 7553 7069 6465  ......z.AyuSpide
 00000c30: 722e 7570 6461 7465 5f73 6574 7469 6e67  r.update_setting
 00000c40: 7363 0200 0000 0000 0000 0000 0000 0900  sc..............
@@ -208,71 +208,71 @@
 00000cf0: 139b 0064 087c 066a 149b 0064 097c 066a  ...d.|.j...d.|.j
 00000d00: 159b 009d 0c7d 0774 167c 0764 0a8d 016a  .....}.t.|.d...j
 00000d10: 177c 045f 1874 0a74 1983 006a 0c7c 016a  .|._.t.t...j.|.j
 00000d20: 097c 0564 038d 0283 0104 007d 0872 e27c  .|.d.......}.r.|
 00000d30: 046a 04a0 0d64 0ba1 0101 007c 087c 045f  .j...d.....|.|._
 00000d40: 1a7c 0453 0029 0c4e 7516 0000 0073 6574  .|.S.).Nu....set
 00000d50: 7469 6e67 735f 7479 7065 20e9 858d e7bd  tings_type .....
-00000d60: ae3a 2029 0172 3500 0000 2902 7235 0000  .: ).r5...).r5..
+00000d60: ae3a 2029 0172 3700 0000 2902 7237 0000  .: ).r7...).r7..
 00000d70: 005a 0b63 6f6e 7375 6c5f 636f 6e66 7524  .Z.consul_confu$
 00000d80: 0000 00e9 a1b9 e79b aee4 b8ad e985 8de7  ................
 00000d90: bdae e4ba 8620 6d79 7371 6c5f 636f 6e66  ..... mysql_conf
 00000da0: 20e4 bfa1 e681 af7a 106d 7973 716c 2b70   ......z.mysql+p
 00000db0: 796d 7973 716c 3a2f 2ffa 013a fa01 40fa  ymysql://..:..@.
 00000dc0: 012f 7a09 3f63 6861 7273 6574 3d29 0172  ./z.?charset=).r
 00000dd0: 0d00 0000 7526 0000 00e9 a1b9 e79b aee4  ....u&..........
 00000de0: b8ad e985 8de7 bdae e4ba 8620 6d6f 6e67  ........... mong
 00000df0: 6f64 625f 636f 6e66 20e4 bfa1 e681 af29  odb_conf ......)
-00000e00: 1b72 2e00 0000 7209 0000 00da 0c66 726f  .r....r......fro
+00000e00: 1b72 3000 0000 7209 0000 00da 0c66 726f  .r0...r......fro
 00000e10: 6d5f 6372 6177 6c65 72da 0573 7461 7473  m_crawler..stats
-00000e20: 723a 0000 00da 0564 6562 7567 723c 0000  r:.....debugr<..
+00000e20: 723c 0000 00da 0564 6562 7567 723e 0000  r<.....debugr>..
 00000e30: 0072 0400 0000 5a0f 6765 745f 636f 6e73  .r....Z.get_cons
-00000e40: 756c 5f63 6f6e 6672 3500 0000 7207 0000  ul_confr5...r...
+00000e40: 756c 5f63 6f6e 6672 3700 0000 7207 0000  ul_confr7...r...
 00000e50: 0072 0600 0000 5a0e 6372 6561 7465 5f70  .r....Z.create_p
 00000e60: 726f 6475 6374 da04 696e 666f da0a 6d79  roduct..info..my
 00000e70: 7371 6c5f 636f 6e66 da14 6d79 7371 6c5f  sql_conf..mysql_
 00000e80: 656e 6769 6e65 5f65 6e61 626c 6564 da04  engine_enabled..
 00000e90: 7573 6572 da08 7061 7373 776f 7264 da04  user..password..
 00000ea0: 686f 7374 da04 706f 7274 da08 6461 7461  host..port..data
 00000eb0: 6261 7365 da07 6368 6172 7365 7472 0a00  base..charsetr..
-00000ec0: 0000 720b 0000 0072 3300 0000 7205 0000  ..r....r3...r...
+00000ec0: 0000 720b 0000 0072 3500 0000 7205 0000  ..r....r5...r...
 00000ed0: 00da 0c6d 6f6e 676f 6462 5f63 6f6e 6629  ...mongodb_conf)
-00000ee0: 0972 1600 0000 7234 0000 0072 1700 0000  .r....r4...r....
-00000ef0: 7218 0000 0072 3f00 0000 5a0c 5f63 6f6e  r....r?...Z._con
-00000f00: 7375 6c5f 636f 6e66 724b 0000 005a 096d  sul_confrK...Z.m
-00000f10: 7973 716c 5f75 726c 7253 0000 0072 3100  ysql_urlrS...r1.
-00000f20: 0000 720e 0000 0072 0f00 0000 7247 0000  ..r....r....rG..
+00000ee0: 0972 1600 0000 7236 0000 0072 1700 0000  .r....r6...r....
+00000ef0: 7218 0000 0072 4200 0000 5a0c 5f63 6f6e  r....rB...Z._con
+00000f00: 7375 6c5f 636f 6e66 724e 0000 005a 096d  sul_confrN...Z.m
+00000f10: 7973 716c 5f75 726c 7256 0000 0072 3300  ysql_urlrV...r3.
+00000f20: 0000 720e 0000 0072 0f00 0000 724a 0000  ..r....r....rJ..
 00000f30: 0096 0000 0073 3200 0000 0002 1801 0803  .....s2.........
 00000f40: 1402 0e02 0201 0601 0400 02ff 04ff 0805  ................
 00000f50: 0c01 0601 0602 32ff 0206 0e03 0201 0601  ......2.........
 00000f60: 0400 02ff 04ff 0805 0c01 0601 7a16 4179  ............z.Ay
 00000f70: 7553 7069 6465 722e 6672 6f6d 5f63 7261  uSpider.from_cra
 00000f80: 776c 6572 2917 7219 0000 0072 1a00 0000  wler).r....r....
 00000f90: 721b 0000 0072 1c00 0000 5a16 6375 7374  r....r....Z.cust
 00000fa0: 6f6d 5f63 6f6d 6d6f 6e5f 7365 7474 696e  om_common_settin
 00000fb0: 6773 5a15 6375 7374 6f6d 5f64 6562 7567  gsZ.custom_debug
 00000fc0: 5f73 6574 7469 6e67 735a 1763 7573 746f  _settingsZ.custo
 00000fd0: 6d5f 7072 6f64 7563 745f 7365 7474 696e  m_product_settin
 00000fe0: 6773 da04 7469 6d65 da08 7374 7266 7469  gs..time..strfti
 00000ff0: 6d65 da09 6c6f 6361 6c74 696d 655a 0b53  me..localtimeZ.S
-00001000: 5049 4445 525f 5449 4d45 723c 0000 005a  PIDER_TIMEr<...Z
+00001000: 5049 4445 525f 5449 4d45 723e 0000 005a  PIDER_TIMEr>...Z
 00001010: 0f70 726f 6a65 6374 5f63 6f6e 7465 6e74  .project_content
-00001020: 723b 0000 0072 4c00 0000 722f 0000 0072  r;...rL...r/...r
-00001030: 1000 0000 da08 7072 6f70 6572 7479 723a  ......propertyr:
+00001020: 723d 0000 0072 4f00 0000 7231 0000 0072  r=...rO...r1...r
+00001030: 1000 0000 da08 7072 6f70 6572 7479 723c  ......propertyr<
 00001040: 0000 00da 0b63 6c61 7373 6d65 7468 6f64  .....classmethod
-00001050: 7243 0000 0072 4700 0000 da0d 5f5f 636c  rC...rG.....__cl
+00001050: 7246 0000 0072 4a00 0000 da0d 5f5f 636c  rF...rJ.....__cl
 00001060: 6173 7363 656c 6c5f 5f72 0e00 0000 720e  asscell__r....r.
-00001070: 0000 0072 3100 0000 720f 0000 0072 0900  ...r1...r....r..
+00001070: 0000 0072 3300 0000 720f 0000 0072 0900  ...r3...r....r..
 00001080: 0000 2900 0000 7350 0000 0008 0104 0602  ..)...sP........
 00001090: 0102 0102 0102 0102 fb06 0b02 0102 0202  ................
 000010a0: 0202 0202 0202 0202 0202 0202 ef06 1602  ................
 000010b0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
 000010c0: f706 0d10 0204 0204 0204 0204 020c 060c  ................
 000010d0: 0402 010e 1702 010a 0f02 0129 1172 1d00  ...........).r..
-000010e0: 0000 7254 0000 00da 0e73 6372 6170 792e  ..rT.....scrapy.
+000010e0: 0000 7257 0000 00da 0e73 6372 6170 792e  ..rW.....scrapy.
 000010f0: 7370 6964 6572 7372 0200 0000 5a0a 7371  spidersr....Z.sq
 00001100: 6c61 6c63 6865 6d79 7203 0000 005a 2461  lalchemyr....Z$a
 00001110: 7975 6765 7370 6964 6572 746f 6f6c 732e  yugespidertools.
 00001120: 636f 6d6d 6f6e 2e4d 756c 7469 506c 6578  common.MultiPlex
 00001130: 696e 6772 0400 0000 5a24 6179 7567 6573  ingr....Z$ayuges
 00001140: 7069 6465 7274 6f6f 6c73 2e63 6f6d 6d6f  pidertools.commo
 00001150: 6e2e 5370 6964 6572 4442 436f 6e66 7205  n.SpiderDBConfr.
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc` & `ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/scraper/spiders/__pycache__/init.cpython-38.pyc` & `ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__pycache__/init.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/templates/project/.gitignore` & `ayugespidertools-1.1.9/ayugespidertools/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/templates/project/module/VIT/.conf` & `ayugespidertools-1.1.9/ayugespidertools/templates/project/module/VIT/.conf`

 * *Files 1% similar despite different names*

```diff
@@ -6,35 +6,35 @@
 00000050: 6d62 340d 0a0d 0a5b 4d4f 4e47 4f44 425d  mb4....[MONGODB]
 00000060: 0d0a 484f 5354 3d2a 2a2a 0d0a 504f 5254  ..HOST=***..PORT
 00000070: 3d32 3730 3137 0d0a 4441 5441 4241 5345  =27017..DATABASE
 00000080: 3d2a 2a2a 0d0a 4155 5448 534f 5552 4345  =***..AUTHSOURCE
 00000090: 3d2a 2a2a 0d0a 5553 4552 3d2a 2a2a 0d0a  =***..USER=***..
 000000a0: 5041 5353 574f 5244 3d2a 2a2a 0d0a 0d0a  PASSWORD=***....
 000000b0: 5b43 4f4e 5355 4c5d 0d0a 544f 4b45 4e3d  [CONSUL]..TOKEN=
-000000c0: 2a2a 2a0d 0a55 524c 3d68 7474 703a 2f2f  ***..URL=http://
-000000d0: 686f 7374 3a70 6f72 742f 7631 2f6b 762f  host:port/v1/kv/
-000000e0: 2e2e 2e3f 6463 3d64 6331 0d0a 464f 524d  ...?dc=dc1..FORM
-000000f0: 4154 3d6a 736f 6e0d 0a0d 0a5b 4b44 4c5f  AT=json....[KDL_
-00000100: 4459 4e41 4d49 435f 5052 4f58 595d 0d0a  DYNAMIC_PROXY]..
-00000110: 5052 4f58 595f 5552 4c3d 6f36 3638 2e6b  PROXY_URL=o668.k
-00000120: 646c 7470 732e 636f 6d3a 3135 3831 380d  dltps.com:15818.
-00000130: 0a55 5345 524e 414d 453d 2a2a 2a0d 0a50  .USERNAME=***..P
-00000140: 4153 5357 4f52 443d 2a2a 2a0d 0a0d 0a5b  ASSWORD=***....[
-00000150: 4b44 4c5f 4558 434c 5553 4956 455f 5052  KDL_EXCLUSIVE_PR
-00000160: 4f58 595d 0d0a 5052 4f58 595f 5552 4c3d  OXY]..PROXY_URL=
-00000170: 6874 7470 3a2f 2f6b 7073 2e6b 646c 6170  http://kps.kdlap
-00000180: 692e 636f 6d2f 6170 692f 6765 746b 7073  i.com/api/getkps
-00000190: 3f6f 7264 6572 6964 3d2a 2a2a 266e 756d  ?orderid=***&num
-000001a0: 3d31 3030 2666 6f72 6d61 743d 6a73 6f6e  =100&format=json
-000001b0: 0d0a 5553 4552 4e41 4d45 3d2a 2a2a 0d0a  ..USERNAME=***..
-000001c0: 5041 5353 574f 5244 3d2a 2a2a 0d0a 5052  PASSWORD=***..PR
-000001d0: 4f58 595f 494e 4445 583d 310d 0a0d 0a5b  OXY_INDEX=1....[
-000001e0: 414c 495f 4f53 535d 0d0a 4f73 7341 6363  ALI_OSS]..OssAcc
-000001f0: 6573 734b 6579 4964 3d4c 5441 2a2a 2a2a  essKeyId=LTA****
-00000200: 2a2a 0d0a 4f73 7341 6363 6573 734b 6579  **..OssAccessKey
-00000210: 5365 6372 6574 3d2a 2a2a 2a2a 2a0d 0a45  Secret=******..E
-00000220: 6e64 706f 696e 743d 6874 7470 733a 2f2f  ndpoint=https://
-00000230: 6f73 732d 636e 2d2a 2a2a 2a2a 2a2e 616c  oss-cn-******.al
-00000240: 6979 756e 6373 2e63 6f6d 0d0a 4578 616d  iyuncs.com..Exam
-00000250: 706c 6562 7563 6b65 743d 2a2a 2a2a 2a2a  plebucket=******
-00000260: 0d0a 4f70 6572 6174 6544 6f63 3d2a 2a2a  ..OperateDoc=***
-00000270: 2a2a 2a2a 0d0a                           ****..
+000000c0: 0d0a 5552 4c3d 6874 7470 3a2f 2f68 6f73  ..URL=http://hos
+000000d0: 743a 706f 7274 2f76 312f 6b76 2f2e 2e2e  t:port/v1/kv/...
+000000e0: 3f64 633d 6463 310d 0a46 4f52 4d41 543d  ?dc=dc1..FORMAT=
+000000f0: 6a73 6f6e 0d0a 0d0a 5b4b 444c 5f44 594e  json....[KDL_DYN
+00000100: 414d 4943 5f50 524f 5859 5d0d 0a50 524f  AMIC_PROXY]..PRO
+00000110: 5859 5f55 524c 3d6f 3636 382e 6b64 6c74  XY_URL=o668.kdlt
+00000120: 7073 2e63 6f6d 3a31 3538 3138 0d0a 5553  ps.com:15818..US
+00000130: 4552 4e41 4d45 3d2a 2a2a 0d0a 5041 5353  ERNAME=***..PASS
+00000140: 574f 5244 3d2a 2a2a 0d0a 0d0a 5b4b 444c  WORD=***....[KDL
+00000150: 5f45 5843 4c55 5349 5645 5f50 524f 5859  _EXCLUSIVE_PROXY
+00000160: 5d0d 0a50 524f 5859 5f55 524c 3d68 7474  ]..PROXY_URL=htt
+00000170: 703a 2f2f 6b70 732e 6b64 6c61 7069 2e63  p://kps.kdlapi.c
+00000180: 6f6d 2f61 7069 2f67 6574 6b70 733f 6f72  om/api/getkps?or
+00000190: 6465 7269 643d 2a2a 2a26 6e75 6d3d 3130  derid=***&num=10
+000001a0: 3026 666f 726d 6174 3d6a 736f 6e0d 0a55  0&format=json..U
+000001b0: 5345 524e 414d 453d 2a2a 2a0d 0a50 4153  SERNAME=***..PAS
+000001c0: 5357 4f52 443d 2a2a 2a0d 0a50 524f 5859  SWORD=***..PROXY
+000001d0: 5f49 4e44 4558 3d31 0d0a 0d0a 5b41 4c49  _INDEX=1....[ALI
+000001e0: 5f4f 5353 5d0d 0a4f 7373 4163 6365 7373  _OSS]..OssAccess
+000001f0: 4b65 7949 643d 4c54 412a 2a2a 2a2a 2a0d  KeyId=LTA******.
+00000200: 0a4f 7373 4163 6365 7373 4b65 7953 6563  .OssAccessKeySec
+00000210: 7265 743d 2a2a 2a2a 2a2a 0d0a 456e 6470  ret=******..Endp
+00000220: 6f69 6e74 3d68 7474 7073 3a2f 2f6f 7373  oint=https://oss
+00000230: 2d63 6e2d 2a2a 2a2a 2a2a 2e61 6c69 7975  -cn-******.aliyu
+00000240: 6e63 732e 636f 6d0d 0a45 7861 6d70 6c65  ncs.com..Example
+00000250: 6275 636b 6574 3d2a 2a2a 2a2a 2a0d 0a4f  bucket=******..O
+00000260: 7065 7261 7465 446f 633d 2a2a 2a2a 2a2a  perateDoc=******
+00000270: 2a0d 0a                                  *..
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/templates/project/module/common/DataEnum.py.tmpl` & `ayugespidertools-1.1.9/ayugespidertools/templates/project/module/common/DataEnum.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-1.1.9/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/templates/project/module/settings.py.tmpl` & `ayugespidertools-1.1.9/ayugespidertools/templates/project/module/settings.py.tmpl`

 * *Files 8% similar despite different names*

```diff
@@ -62,22 +62,17 @@
     "USER": config_parser.get("MONGODB", "USER", fallback="admin"),
     "PASSWORD": config_parser.get("MONGODB", "PASSWORD", fallback=None),
     "DATABASE": config_parser.get("MONGODB", "DATABASE", fallback=None),
 }
 
 # consul 应用管理的连接配置
 CONSUL_CONFIG = {
-    "HOST": config_parser.get("CONSUL", "HOST", fallback=None),
-    "PORT": config_parser.getint("CONSUL", "PORT", fallback=8500),
-    # 此 token 值只需要只读权限即可，只用于取配置值
     "TOKEN": config_parser.get("CONSUL", "TOKEN", fallback=None),
-    # 这个是应用管理中心最终的 key 值，如果不设置此值会默认设置值为中程序中的 ENV 值
-    "KEY_VALUES": config_parser.get("CONSUL", "KEY_VALUES", fallback=None),
-    # 这个是此配置在应用管理中心所属的 group，默认为空(按需配置，如果不需要直接不配置此值或配置为空皆可)
-    "GROUP": config_parser.get("CONSUL", "GROUP", fallback=None),
+    "URL": config_parser.get("CONSUL", "URL", fallback=None),
+    "FORMAT": config_parser.get("CONSUL", "FORMAT", fallback="json"),
 }
 
 # 动态隧道代理（快代理版本）
 DYNAMIC_PROXY_CONFIG = {
     "PROXY_URL": config_parser.get("KDL_DYNAMIC_PROXY", "PROXY_URL", fallback=None),
     "USERNAME": config_parser.get("KDL_DYNAMIC_PROXY", "USERNAME", fallback=None),
     "PASSWORD": config_parser.get("KDL_DYNAMIC_PROXY", "PASSWORD", fallback=None),
```

### Comparing `ayugespidertools-1.1.8/ayugespidertools/templates/spiders/async.tmpl` & `ayugespidertools-1.1.9/ayugespidertools/templates/spiders/async.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/templates/spiders/basic.tmpl` & `ayugespidertools-1.1.9/ayugespidertools/templates/spiders/basic.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/templates/spiders/crawl.tmpl` & `ayugespidertools-1.1.9/ayugespidertools/templates/spiders/crawl.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-1.1.9/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-1.1.9/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/ayugespidertools/utils/cmdline.py` & `ayugespidertools-1.1.9/ayugespidertools/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.8/pyproject.toml` & `ayugespidertools-1.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AyugeSpiderTools"
-version = "1.1.8"
+version = "1.1.9"
 description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。"
 authors = ["ayuge <ayugesheng@gmail.com>"]
 maintainers = ["ayuge <ayugesheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ayugespidertools"}]
 repository = "https://github.com/shengchenyang/AyugeSpiderTools"
 documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
@@ -18,15 +18,15 @@
 PyMySQL = "^1.0.2"
 environs = "^9.5.0"
 loguru = "^0.6.0"
 numpy = "1.24.2"
 PyExecJS = "^1.5.1"
 requests = "^2.28.1"
 Pillow = "^9.2.0"
-Scrapy = "^2.8.0"
+Scrapy = "2.8.0"
 pandas = "^1.5.0"
 WorkWeixinRobot = "^1.0.1"
 retrying = "^1.3.3"
 SQLAlchemy = "^1.4.41"
 DBUtils = "^3.0.2"
 itemadapter = "^0.7.0"
 aiohttp = "^3.8.3"
@@ -49,28 +49,29 @@
 black = "^23.1.0"
 isort = "^5.12.0"
 sphinx-rtd-theme = "^1.2.0"
 recommonmark = "^0.7.1"
 coverage = "^7.2.2"
 tox = "^4.4.8"
 flake8 = "^6.0.0"
+testfixtures = "^7.1.0"
 
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple"
 
 [tool.pytest.ini_options]
 xfail_strict = true
 python_files = "test_*.py __init__.py"
 python_classes = "Test*"
 testpaths = [
     "tests",
 ]
 norecursedirs = ["dist", "build", "docs", "examples"]
-addopts = "--assert=plain --doctest-modules"
+addopts = "--assert=plain --doctest-modules --reactor=asyncio"
 filterwarnings = [
     "ignore::DeprecationWarning",
     "ignore:scrapy.downloadermiddlewares.decompression is deprecated",
     "ignore:Module scrapy.utils.reqser is deprecated",
     "ignore:typing.re is deprecated",
     "ignore:typing.io is deprecated"
 ]
```

### Comparing `ayugespidertools-1.1.8/PKG-INFO` & `ayugespidertools-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayugespidertools
-Version: 1.1.8
+Version: 1.1.9
 Summary: scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。
 Home-page: https://www.ayuge.top/mkdocs-material/
 Keywords: crawler,scraping,twisted,aiohttp,asyncio,scrapy,aiomysql,mmh3
 Author: ayuge
 Author-email: ayugesheng@gmail.com
 Maintainer: ayuge
 Maintainer-email: ayugesheng@gmail.com
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: DBUtils (>=3.0.2,<4.0.0)
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
 Requires-Dist: PyExecJS (>=1.5.1,<2.0.0)
 Requires-Dist: PyMySQL (>=1.0.2,<2.0.0)
 Requires-Dist: SQLAlchemy (>=1.4.41,<2.0.0)
-Requires-Dist: Scrapy (>=2.8.0,<3.0.0)
+Requires-Dist: Scrapy (==2.8.0)
 Requires-Dist: WorkWeixinRobot (>=1.0.1,<2.0.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiomysql (>=0.1.1,<0.2.0)
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: environs (>=9.5.0,<10.0.0)
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
 Requires-Dist: itemadapter (>=0.7.0,<0.8.0)
@@ -42,15 +42,15 @@
 Project-URL: Repository, https://github.com/shengchenyang/AyugeSpiderTools
 Description-Content-Type: text/markdown
 
 ![ayugespidertools-logo](https://raw.githubusercontent.com/shengchenyang/AyugeSpiderTools/main/artwork/ayugespidertools-logo.png)
 
 [![OSCS Status](https://www.oscs1024.com/platform/badge/AyugeSpiderTools.svg?size=small)](https://www.murphysec.com/accept?code=0ec375759aebea7fd260248910b98806&type=1&from=2)
 ![GitHub](https://img.shields.io/github/license/shengchenyang/AyugeSpiderTools)
-![python](https://img.shields.io/badge/python-3.8%2B-blue)
+![python](https://img.shields.io/badge/python-3.8.1%2B-blue)
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/shengchenyang/AyugeSpiderTools/codeql.yml?branch=main)
 ![Read the Docs](https://img.shields.io/readthedocs/ayugespidertools)
 ![GitHub all releases](https://img.shields.io/github/downloads/shengchenyang/AyugeSpiderTools/total?label=releases%20downloads)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/AyugeSpiderTools?label=pypi%20downloads)
 
 # AyugeSpiderTools 工具说明
 
@@ -68,15 +68,15 @@
 
 > `python 3.8+` 可以直接输入以下命令：
 
 ```shell
 pip install ayugespidertools -i https://pypi.org/simple
 ```
 
-注：本库依赖中的 `pymongo` 版本要在 `3.12.3` 及以下是因为我的 `mongoDB` 的版本为 `3.4`，`pymogo` 官方从 `3.12.3` 以后的版本开始不再支持 `3.6` 版本以下的 `MongoDB` 数据库了，望周知！**你也可以根据 [3.3](#3.3.-Build-Your-Own-Library) 自定义库**
+注：本库依赖中的 `pymongo` 版本要在 `^3.12.3` (即`3.13.0` 及以下) 是因为我的 `mongoDB` 的版本为 `3.4`，`pymogo` 官方从 `3.13.0` 以后的版本开始不再支持 `3.6` 版本以下的 `MongoDB` 数据库了，望周知！**你也可以根据 [3.3](#3.3.-Build-Your-Own-Library) 自定义库**
 
 ## 2. 使用方法
 
 > 项目主要包含两部分：
 >
 
 - 开发场景中的工具库
```

