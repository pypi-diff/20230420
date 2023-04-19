# Comparing `tmp/Levenshtein-0.20.9.tar.gz` & `tmp/Levenshtein-0.21.0-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Levenshtein-0.20.9.tar", last modified: Sun Dec 25 17:54:11 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

