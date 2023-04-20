# Comparing `tmp/pyrfc-2.8.0.tar.gz` & `tmp/pyrfc-2.8.1-cp39-cp39-macosx_13_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfc-2.8.0.tar", last modified: Wed Apr 19 12:32:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

