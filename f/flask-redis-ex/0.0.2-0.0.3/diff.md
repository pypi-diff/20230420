# Comparing `tmp/flask_redis_ex-0.0.2-py3-none-any.whl.zip` & `tmp/flask_redis_ex-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 1698 bytes, number of entries: 5
--rw-rw-r--  2.0 unx      434 b- defN 23-Apr-19 15:00 flask_redis_ex/__init__.py
--rw-rw-r--  2.0 unx      570 b- defN 23-Apr-19 15:10 flask_redis_ex-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 15:10 flask_redis_ex-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-19 15:10 flask_redis_ex-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      407 b- defN 23-Apr-19 15:10 flask_redis_ex-0.0.2.dist-info/RECORD
-5 files, 1518 bytes uncompressed, 932 bytes compressed:  38.6%
+Zip file size: 2581 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx      499 b- defN 23-Apr-19 23:52 flask_redis_ex/__init__.py
+-rw-rw-r--  2.0 unx     1086 b- defN 23-Apr-20 00:58 flask_redis_ex-0.0.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      604 b- defN 23-Apr-20 00:58 flask_redis_ex-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 00:58 flask_redis_ex-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-20 00:58 flask_redis_ex-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      502 b- defN 23-Apr-20 00:58 flask_redis_ex-0.0.3.dist-info/RECORD
+6 files, 2798 bytes uncompressed, 1663 bytes compressed:  40.6%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
 Filename: flask_redis_ex/__init__.py
 Comment: 
 
-Filename: flask_redis_ex-0.0.2.dist-info/METADATA
+Filename: flask_redis_ex-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: flask_redis_ex-0.0.2.dist-info/WHEEL
+Filename: flask_redis_ex-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: flask_redis_ex-0.0.2.dist-info/top_level.txt
+Filename: flask_redis_ex-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: flask_redis_ex-0.0.2.dist-info/RECORD
+Filename: flask_redis_ex-0.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: flask_redis_ex-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flask_redis_ex/__init__.py

```diff
@@ -1,13 +1,18 @@
 from flask import current_app
 from werkzeug.local import LocalProxy
 
 import redis
 
+
 def _get_client():
-    if not hasattr(current_app, 'redis_client') or current_app.redis_client is None:
+    key = "redis_client"
+    if key not in current_app.extensions:
         config = current_app.config
         redis_url = config.get("REDIS_URL")
-        current_app.redis_client = redis.from_url(redis_url)
-    return getattr(current_app, 'redis_client', None)
+        if redis_url is None:
+            raise RuntimeError("REDIS_URL is not configured")
+        current_app.extensions[key] = redis.from_url(redis_url)
+    return current_app.extensions[key]
+
 
-redis_client: redis.Redis = LocalProxy(_get_client)
+redis_client: redis.Redis = LocalProxy(_get_client)
```

