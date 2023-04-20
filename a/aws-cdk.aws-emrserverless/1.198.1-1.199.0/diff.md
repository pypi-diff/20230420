# Comparing `tmp/aws-cdk.aws-emrserverless-1.198.1.tar.gz` & `tmp/aws_cdk.aws_emrserverless-1.199.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src451122087/src/packages/@aws-cdk/aws-emrserverless/dist/python/aws-cdk.aws-emrserverless-1.198.1.tar", last modified: Tue Mar 28 21:36:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

