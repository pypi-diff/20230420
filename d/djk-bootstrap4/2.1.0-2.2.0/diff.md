# Comparing `tmp/djk-bootstrap4-2.1.0.tar.gz` & `tmp/djk_bootstrap4-2.2.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djk-bootstrap4-2.1.0.tar", last modified: Fri Jun 17 20:37:31 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

