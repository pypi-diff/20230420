# Comparing `tmp/pytest-result-sender-0.0.2.tar.gz` & `tmp/pytest_result_sender-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-result-sender-0.0.2.tar", last modified: Mon Apr 17 11:29:45 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

