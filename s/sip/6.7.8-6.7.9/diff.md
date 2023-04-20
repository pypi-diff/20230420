# Comparing `tmp/sip-6.7.8.tar.gz` & `tmp/sip-6.7.9-cp37-abi3-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sip-6.7.8.tar", last modified: Tue Apr  4 15:45:13 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

