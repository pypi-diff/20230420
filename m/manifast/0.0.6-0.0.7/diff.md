# Comparing `tmp/manifast-0.0.6.tar.gz` & `tmp/manifast-0.0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/manifast-0.0.6.tar", last modified: Tue Apr  4 08:39:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

