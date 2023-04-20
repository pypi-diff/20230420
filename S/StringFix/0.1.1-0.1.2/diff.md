# Comparing `tmp/StringFix-0.1.1.tar.gz` & `tmp/StringFix-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StringFix-0.1.1.tar", last modified: Thu Apr 20 03:15:07 2023, max compression
+gzip compressed data, was "StringFix-0.1.2.tar", last modified: Thu Apr 20 03:27:17 2023, max compression
```

## Comparing `StringFix-0.1.1.tar` & `StringFix-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-20 03:15:07.219614 StringFix-0.1.1/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-04-20 03:05:32.000000 StringFix-0.1.1/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-04-20 03:05:32.000000 StringFix-0.1.1/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      676 2023-04-20 03:15:07.219614 StringFix-0.1.1/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      111 2023-04-20 03:05:32.000000 StringFix-0.1.1/README.md
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-20 03:15:07.219614 StringFix-0.1.1/StringFix.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      676 2023-04-20 03:15:07.000000 StringFix-0.1.1/StringFix.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      262 2023-04-20 03:15:07.000000 StringFix-0.1.1/StringFix.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-04-20 03:15:07.000000 StringFix-0.1.1/StringFix.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-04-20 03:07:46.000000 StringFix-0.1.1/StringFix.egg-info/not-zip-safe
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-04-20 03:15:07.000000 StringFix-0.1.1/StringFix.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-04-20 03:15:07.000000 StringFix-0.1.1/StringFix.egg-info/top_level.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-04-20 03:15:07.219614 StringFix-0.1.1/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     2669 2023-04-20 03:15:02.000000 StringFix-0.1.1/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-20 03:15:07.219614 StringFix-0.1.1/tests/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      100 2023-04-20 03:05:32.000000 StringFix-0.1.1/tests/__init__.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-20 03:27:17.246083 StringFix-0.1.2/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-04-20 03:05:32.000000 StringFix-0.1.2/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-04-20 03:25:54.000000 StringFix-0.1.2/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      676 2023-04-20 03:27:17.246083 StringFix-0.1.2/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      111 2023-04-20 03:25:54.000000 StringFix-0.1.2/README.md
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-20 03:27:17.246083 StringFix-0.1.2/StringFix.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      676 2023-04-20 03:27:17.000000 StringFix-0.1.2/StringFix.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      262 2023-04-20 03:27:17.000000 StringFix-0.1.2/StringFix.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-04-20 03:27:17.000000 StringFix-0.1.2/StringFix.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-04-20 03:27:17.000000 StringFix-0.1.2/StringFix.egg-info/not-zip-safe
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-04-20 03:27:17.000000 StringFix-0.1.2/StringFix.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-04-20 03:27:17.000000 StringFix-0.1.2/StringFix.egg-info/top_level.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-04-20 03:27:17.246083 StringFix-0.1.2/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     2669 2023-04-20 03:27:06.000000 StringFix-0.1.2/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-20 03:27:17.246083 StringFix-0.1.2/tests/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      100 2023-04-20 03:05:32.000000 StringFix-0.1.2/tests/__init__.py
```

### Comparing `StringFix-0.1.1/LICENSE` & `StringFix-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `StringFix-0.1.1/PKG-INFO` & `StringFix-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StringFix
-Version: 0.1.1
+Version: 0.1.2
 Summary: Annotation guided transcriptome assembly program.
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Joongho Lee, Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi StringFix
 Classifier: Programming Language :: Python :: 3
```

### Comparing `StringFix-0.1.1/StringFix.egg-info/PKG-INFO` & `StringFix-0.1.2/StringFix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StringFix
-Version: 0.1.1
+Version: 0.1.2
 Summary: Annotation guided transcriptome assembly program.
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Joongho Lee, Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi StringFix
 Classifier: Programming Language :: Python :: 3
```

### Comparing `StringFix-0.1.1/setup.py` & `StringFix-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     # 배포할 패키지의 이름을 적어줍니다. setup.py파일을 가지는 폴더 이름과 동일하게 합니다.
     name                = 'StringFix',
     # 배포할 패키지의 버전을 적어줍니다. 첫 등록이므로 0.1 또는 0.0.1을 사용합니다.
-    version             = '0.1.1',
+    version             = '0.1.2',
     # 배포할 패키지에 대한 설명을 작성합니다.
     description         = 'Annotation guided transcriptome assembly program.',
     # 배포하는 사람의 이름을 작성합니다.
     author              = 'Joongho Lee, Seokhyun Yoon',
     # 배포하는 사람의 메일주소를 작성합니다.
     author_email        = 'syoon@dku.edu',
     # 배포하는 패키지의 url을 적어줍니다. 보통 github 링크를 적습니다.
```

