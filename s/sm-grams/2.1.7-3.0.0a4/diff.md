# Comparing `tmp/sm_grams-2.1.7.tar.gz` & `tmp/sm_grams-3.0.0a4-cp39-cp39-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sm_grams-2.1.7.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

