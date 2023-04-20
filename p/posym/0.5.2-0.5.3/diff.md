# Comparing `tmp/posym-0.5.2.tar.gz` & `tmp/posym-0.5.3-cp37-cp37m-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posym-0.5.2.tar", last modified: Fri Apr  7 17:00:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

