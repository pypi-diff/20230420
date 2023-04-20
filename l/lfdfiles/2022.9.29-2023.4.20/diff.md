# Comparing `tmp/lfdfiles-2022.9.29.tar.gz` & `tmp/lfdfiles-2023.4.20-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfdfiles-2022.9.29.tar", last modified: Thu Sep 29 17:08:41 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

