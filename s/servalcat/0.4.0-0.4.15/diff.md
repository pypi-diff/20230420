# Comparing `tmp/servalcat-0.4.0.tar.gz` & `tmp/servalcat-0.4.15-cp38-cp38-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servalcat-0.4.0.tar", last modified: Tue Mar  7 00:06:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

