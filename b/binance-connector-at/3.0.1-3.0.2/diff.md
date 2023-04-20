# Comparing `tmp/binance-connector-at-3.0.1.tar.gz` & `tmp/binance_connector_at-3.0.2-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-connector-at-3.0.1.tar", last modified: Thu Apr 20 03:31:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

