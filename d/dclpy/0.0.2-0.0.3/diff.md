# Comparing `tmp/dclpy-0.0.2.tar.gz` & `tmp/dclpy-0.0.3-cp39-cp39-manylinux1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dclpy-0.0.2.tar", last modified: Tue Apr  4 22:28:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

