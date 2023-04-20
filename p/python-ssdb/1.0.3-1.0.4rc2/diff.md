# Comparing `tmp/python_ssdb-1.0.3.tar.gz` & `tmp/python_ssdb-1.0.4rc2-pp39-pypy39_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ssdb-1.0.3.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

