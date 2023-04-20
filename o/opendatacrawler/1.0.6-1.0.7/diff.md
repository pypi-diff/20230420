# Comparing `tmp/opendatacrawler-1.0.6.tar.gz` & `tmp/opendatacrawler-1.0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendatacrawler-1.0.6.tar", last modified: Thu Apr 20 15:17:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

