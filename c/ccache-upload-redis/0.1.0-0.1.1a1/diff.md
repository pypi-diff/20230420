# Comparing `tmp/ccache_upload_redis-0.1.0.tar.gz` & `tmp/ccache_upload_redis-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccache_upload_redis-0.1.0.tar", max compression
+gzip compressed data, was "ccache_upload_redis-0.1.1a1.tar", max compression
```

## Comparing `ccache_upload_redis-0.1.0.tar` & `ccache_upload_redis-0.1.1a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1097 2023-04-19 04:58:00.966726 ccache_upload_redis-0.1.0/LICENSE
--rw-r--r--   0        0        0     3170 2023-04-19 06:56:45.848803 ccache_upload_redis-0.1.0/README.md
--rwxr-xr-x   0        0        0     2244 2023-04-19 05:04:49.867881 ccache_upload_redis-0.1.0/ccache-download-redis
--rwxr-xr-x   0        0        0    10254 2023-04-19 06:30:07.099422 ccache_upload_redis-0.1.0/ccache-performance
--rwxr-xr-x   0        0        0     2532 2023-04-19 07:05:13.780841 ccache_upload_redis-0.1.0/ccache-upload-redis
--rw-r--r--   0        0        0      696 2023-04-19 21:20:46.645195 ccache_upload_redis-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 ccache_upload_redis-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-04-19 04:58:00.966726 ccache_upload_redis-0.1.1a1/LICENSE
+-rw-r--r--   0        0        0     3170 2023-04-19 06:56:45.848803 ccache_upload_redis-0.1.1a1/README.md
+-rwxr-xr-x   0        0        0     2244 2023-04-19 05:04:49.867881 ccache_upload_redis-0.1.1a1/ccache-download-redis
+-rwxr-xr-x   0        0        0    10254 2023-04-19 06:30:07.099422 ccache_upload_redis-0.1.1a1/ccache-performance
+-rwxr-xr-x   0        0        0     2532 2023-04-19 07:05:13.780841 ccache_upload_redis-0.1.1a1/ccache-upload-redis
+-rw-r--r--   0        0        0     1045 2023-04-19 23:13:25.120012 ccache_upload_redis-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0     4155 1970-01-01 00:00:00.000000 ccache_upload_redis-0.1.1a1/PKG-INFO
```

### Comparing `ccache_upload_redis-0.1.0/LICENSE` & `ccache_upload_redis-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.0/README.md` & `ccache_upload_redis-0.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.0/ccache-download-redis` & `ccache_upload_redis-0.1.1a1/ccache-download-redis`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.0/ccache-performance` & `ccache_upload_redis-0.1.1a1/ccache-performance`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.0/ccache-upload-redis` & `ccache_upload_redis-0.1.1a1/ccache-upload-redis`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.0/pyproject.toml` & `ccache_upload_redis-0.1.1a1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 [tool.poetry]
 #name = "ccache-download-upload-redis"
 name = "ccache_upload_redis"
-version = "0.1.0"
+version = "0.1.1a1"
 description = "A script to downloads the contents of the local ccache cache from a Redis remote storage."
 authors = ["berlin4apk <83521068+berlin4apk@users.noreply.github.com>"]
+repository = "https://github.com/berlin4apk/action-ccache-download-upload-redis"
+keywords = ["ccache", "redis", "upload", "download"]
 readme = "README.md"
+license = "GPL-3.0-or-later"
 packages = [
     { include = "ccache-upload-redis" },
     { include = "ccache-download-redis" },
     { include = "ccache-performance" },
 ]
 
+[tool.poetry.scripts]
+#ccache-upload-redis_cli = 'ccache-upload-redis.console:run'
+ccache-upload-redis = 'ccache-upload-redis.console:run'
+my_package_cli = 'my_package.console:run'
+
+
 [tool.poetry.dependencies]
 python = "^3.9"
 progress-bar = "^8"
 humanize = "^4.6.0"
 progress = "^1.6"
 redis = "^4.5.4"
 
 [tool.poetry.group.dev.dependencies]
 shiv = "^1.0.3"
 
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ccache_upload_redis-0.1.0/PKG-INFO` & `ccache_upload_redis-0.1.1a1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: ccache-upload-redis
-Version: 0.1.0
+Version: 0.1.1a1
 Summary: A script to downloads the contents of the local ccache cache from a Redis remote storage.
+Home-page: https://github.com/berlin4apk/action-ccache-download-upload-redis
+License: GPL-3.0-or-later
+Keywords: ccache,redis,upload,download
 Author: berlin4apk
 Author-email: 83521068+berlin4apk@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: humanize (>=4.6.0,<5.0.0)
 Requires-Dist: progress (>=1.6,<2.0)
 Requires-Dist: progress-bar (>=8,<9)
 Requires-Dist: redis (>=4.5.4,<5.0.0)
+Project-URL: Repository, https://github.com/berlin4apk/action-ccache-download-upload-redis
 Description-Content-Type: text/markdown
 
 # ccache-upload-redis / ccache-download-redis GitHub Action
 
 An GitHub Action for using ccache-upload-redis / ccache-download-redis
 to uploads / downloads the contents of the local ccache cache from a Redis remote storage.
```

