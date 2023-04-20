# Comparing `tmp/vnpy_binance_pro-2023.4.14.1.tar.gz` & `tmp/vnpy_binance_pro-2023.4.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_binance_pro-2023.4.14.1.tar", last modified: Fri Apr 14 07:31:37 2023, max compression
+gzip compressed data, was "vnpy_binance_pro-2023.4.20.1.tar", last modified: Thu Apr 20 08:47:50 2023, max compression
```

## Comparing `vnpy_binance_pro-2023.4.14.1.tar` & `vnpy_binance_pro-2023.4.20.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-14 07:31:37.638879 vnpy_binance_pro-2023.4.14.1/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1066 2023-04-13 07:25:05.000000 vnpy_binance_pro-2023.4.14.1/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2126 2023-04-14 07:31:37.638978 vnpy_binance_pro-2023.4.14.1/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1165 2023-04-13 10:17:44.000000 vnpy_binance_pro-2023.4.14.1/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1028 2023-04-14 07:31:37.639464 vnpy_binance_pro-2023.4.14.1/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-04-13 07:25:05.000000 vnpy_binance_pro-2023.4.14.1/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-14 07:31:37.635753 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1460 2023-04-13 07:27:31.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    31285 2023-04-13 07:36:35.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/binance_inverse_gateway.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    28895 2023-04-14 04:01:41.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/binance_spot_gateway.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    31615 2023-04-14 05:30:18.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/binance_usdt_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-14 07:31:37.638687 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2126 2023-04-14 07:31:37.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      429 2023-04-14 07:31:37.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-14 07:31:37.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 10:20:10.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-04-14 07:31:37.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       17 2023-04-14 07:31:37.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-20 08:47:50.714898 vnpy_binance_pro-2023.4.20.1/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1066 2023-04-20 08:16:53.000000 vnpy_binance_pro-2023.4.20.1/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2126 2023-04-20 08:47:50.715014 vnpy_binance_pro-2023.4.20.1/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1165 2023-04-20 08:16:53.000000 vnpy_binance_pro-2023.4.20.1/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1028 2023-04-20 08:47:50.715515 vnpy_binance_pro-2023.4.20.1/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-04-20 08:16:53.000000 vnpy_binance_pro-2023.4.20.1/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-20 08:47:50.712715 vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1460 2023-04-20 08:16:53.000000 vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    31285 2023-04-20 08:16:53.000000 vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro/binance_inverse_gateway.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    29023 2023-04-20 08:38:41.000000 vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro/binance_spot_gateway.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    31746 2023-04-20 08:43:26.000000 vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro/binance_usdt_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-20 08:47:50.714573 vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2126 2023-04-20 08:47:50.000000 vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      429 2023-04-20 08:47:50.000000 vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-20 08:47:50.000000 vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-20 08:47:50.000000 vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-04-20 08:47:50.000000 vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       17 2023-04-20 08:47:50.000000 vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro.egg-info/top_level.txt
```

### Comparing `vnpy_binance_pro-2023.4.14.1/LICENSE` & `vnpy_binance_pro-2023.4.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_binance_pro-2023.4.14.1/PKG-INFO` & `vnpy_binance_pro-2023.4.20.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_binance_pro
-Version: 2023.4.14.1
+Version: 2023.4.20.1
 Summary: BINANCE gateway for vn.py quant trading framework.
 Home-page: https://github.com/monk-after-90s/vnpy-binance-pro
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vnpy_binance_pro-2023.4.14.1/README.md` & `vnpy_binance_pro-2023.4.20.1/README.md`

 * *Files identical despite different names*

### Comparing `vnpy_binance_pro-2023.4.14.1/setup.cfg` & `vnpy_binance_pro-2023.4.20.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnpy_binance_pro
-version = 2023.4.14.1
+version = 2023.4.20.1
 url = https://github.com/monk-after-90s/vnpy-binance-pro
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = BINANCE gateway for vn.py quant trading framework.
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/__init__.py` & `vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/binance_inverse_gateway.py` & `vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro/binance_inverse_gateway.py`

 * *Files identical despite different names*

### Comparing `vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/binance_spot_gateway.py` & `vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro/binance_spot_gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,16 +609,18 @@
                 "symbol": req.symbol.upper(),
                 "interval": INTERVAL_VT2BINANCE[req.interval],
                 "limit": limit,
                 "startTime": start_time * 1000,  # 转换成毫秒
             }
 
             if req.end:
-                end_time: int = int(datetime.timestamp(req.end))
-                params["endTime"] = end_time * 1000  # 转换成毫秒
+                interval_seconds = int(TIMEDELTA_MAP[req.interval].total_seconds())
+                end_time: int = int(datetime.timestamp(req.end)) // interval_seconds * interval_seconds
+
+                params["endTime"] = end_time * 1000 - 1  # 转换成毫秒
 
             resp: Response = self.request(
                 "GET",
                 "/api/v3/klines",
                 data={"security": Security.NONE},
                 params=params
             )
```

### Comparing `vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/binance_usdt_gateway.py` & `vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro/binance_usdt_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -679,17 +679,17 @@
                 "interval": INTERVAL_VT2BINANCES[req.interval],
                 "limit": limit
             }
 
             params["startTime"] = start_time * 1000
             path: str = "/fapi/v1/klines"
             if req.end:
-                end_time = int(datetime.timestamp(req.end))
-                params["endTime"] = end_time * 1000  # 转换成毫秒
-
+                interval_seconds = int(TIMEDELTA_MAP[req.interval].total_seconds())
+                end_time: int = int(datetime.timestamp(req.end)) // interval_seconds * interval_seconds
+                params["endTime"] = end_time * 1000 - 1  # 转换成毫秒
             resp: Response = self.request(
                 "GET",
                 path=path,
                 data={"security": Security.NONE},
                 params=params
             )
             # 限速控制
```

### Comparing `vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/PKG-INFO` & `vnpy_binance_pro-2023.4.20.1/vnpy_binance_pro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-binance-pro
-Version: 2023.4.14.1
+Version: 2023.4.20.1
 Summary: BINANCE gateway for vn.py quant trading framework.
 Home-page: https://github.com/monk-after-90s/vnpy-binance-pro
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

