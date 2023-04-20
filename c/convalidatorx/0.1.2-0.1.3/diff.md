# Comparing `tmp/convalidatorx-0.1.2.tar.gz` & `tmp/convalidatorx-0.1.3.win-amd64.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convalidatorx-0.1.2.tar", last modified: Thu Apr 20 06:28:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

