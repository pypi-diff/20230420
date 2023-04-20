# Comparing `tmp/gridtools-cpp-2.2.3.tar.gz` & `tmp/gridtools_cpp-2.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridtools-cpp-2.2.3.tar", last modified: Wed Feb 15 08:57:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

