# Comparing `tmp/StringFix-0.0.9.tar.gz` & `tmp/StringFix-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\StringFix-0.0.9.tar", last modified: Tue Jul 27 13:05:36 2021, max compression
+gzip compressed data, was "StringFix-0.1.0.tar", last modified: Thu Apr 20 03:07:46 2023, max compression
```

## Comparing `StringFix-0.0.9.tar` & `StringFix-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2021-07-27 13:05:36.000000 StringFix-0.0.9/
--rw-rw-rw-   0        0        0    35821 2021-06-22 10:02:23.000000 StringFix-0.0.9/LICENSE
--rw-rw-rw-   0        0        0       60 2021-06-22 10:07:07.000000 StringFix-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1283 2021-07-27 13:05:36.000000 StringFix-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      606 2021-07-21 11:03:04.000000 StringFix-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2021-07-27 13:05:36.000000 StringFix-0.0.9/StringFix/
--rw-rw-rw-   0        0        0      187 2021-06-22 10:24:38.000000 StringFix-0.0.9/StringFix/__init__.py
--rw-rw-rw-   0        0        0   597137 2021-07-27 09:39:45.000000 StringFix-0.0.9/StringFix/stringfix_core.py
-drwxrwxrwx   0        0        0        0 2021-07-27 13:05:36.000000 StringFix-0.0.9/StringFix.egg-info/
--rw-rw-rw-   0        0        0     1283 2021-07-27 13:05:36.000000 StringFix-0.0.9/StringFix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2021-07-27 13:05:36.000000 StringFix-0.0.9/StringFix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-27 13:05:36.000000 StringFix-0.0.9/StringFix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2021-07-21 16:15:05.000000 StringFix-0.0.9/StringFix.egg-info/desktop.ini
--rw-rw-rw-   0        0        0        2 2021-07-21 16:14:58.000000 StringFix-0.0.9/StringFix.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       27 2021-07-27 13:05:36.000000 StringFix-0.0.9/StringFix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-07-27 13:05:36.000000 StringFix-0.0.9/StringFix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2021-07-27 13:05:36.000000 StringFix-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     2715 2021-07-27 13:05:21.000000 StringFix-0.0.9/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-20 03:07:46.554294 StringFix-0.1.0/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-04-20 03:05:32.000000 StringFix-0.1.0/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-04-20 03:05:32.000000 StringFix-0.1.0/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      676 2023-04-20 03:07:46.558294 StringFix-0.1.0/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      111 2023-04-20 03:05:32.000000 StringFix-0.1.0/README.md
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-20 03:07:46.554294 StringFix-0.1.0/StringFix.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      676 2023-04-20 03:07:46.000000 StringFix-0.1.0/StringFix.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      262 2023-04-20 03:07:46.000000 StringFix-0.1.0/StringFix.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-04-20 03:07:46.000000 StringFix-0.1.0/StringFix.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-04-20 03:07:46.000000 StringFix-0.1.0/StringFix.egg-info/not-zip-safe
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       43 2023-04-20 03:07:46.000000 StringFix-0.1.0/StringFix.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-04-20 03:07:46.000000 StringFix-0.1.0/StringFix.egg-info/top_level.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-04-20 03:07:46.558294 StringFix-0.1.0/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     2688 2023-04-20 03:05:32.000000 StringFix-0.1.0/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-04-20 03:07:46.554294 StringFix-0.1.0/tests/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      100 2023-04-20 03:05:32.000000 StringFix-0.1.0/tests/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `StringFix-0.0.9/LICENSE` & `StringFix-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `StringFix-0.0.9/setup.py` & `StringFix-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from setuptools import setup, find_packages
 
 setup(
     # 배포할 패키지의 이름을 적어줍니다. setup.py파일을 가지는 폴더 이름과 동일하게 합니다.
     name                = 'StringFix',
     # 배포할 패키지의 버전을 적어줍니다. 첫 등록이므로 0.1 또는 0.0.1을 사용합니다.
-    version             = '0.0.9',
+    version             = '0.1.0',
     # 배포할 패키지에 대한 설명을 작성합니다.
-    description         = 'A reference-based proteome assmebler for RNA-seq reads',
+    description         = 'Annotation guided transcriptome assembly program.',
     # 배포하는 사람의 이름을 작성합니다.
-    author              = 'Seokhyun Yoon',
+    author              = 'Joongho Lee, Seokhyun Yoon',
     # 배포하는 사람의 메일주소를 작성합니다.
     author_email        = 'syoon@dku.edu',
     # 배포하는 패키지의 url을 적어줍니다. 보통 github 링크를 적습니다.
-    # url                 = 'https://github.com/combio-dku/',
+    url                 = 'https://github.com/combio-dku',
     # 배포하는 패키지의 다운로드 url을 적어줍니다.
-    # download_url        = 'https://github.com/combio-dku/',
+    download_url        = 'https://github.com/combio-dku',
     # 해당 패키지를 사용하기 위해 필요한 패키지를 적어줍니다. ex. install_requires= ['numpy', 'django']
     # 여기에 적어준 패키지는 현재 패키지를 install할때 함께 install됩니다.
-    install_requires    =  ['numpy', 'scipy', 'pandas', 'sklearn'],
+    install_requires    =  ['numpy', 'scipy', 'pandas', 'sklearn', 'multiprocessing'],
     # 등록하고자 하는 패키지를 적는 곳입니다.
     # 우리는 find_packages 라이브러리를 이용하기 때문에 아래와 같이 적어줍니다.
     # 만약 제외하고자 하는 파일이 있다면 exclude에 적어줍니다.
     packages            = find_packages(exclude = []),
-    long_description=open('README.md').read(), 
     # 패키지의 키워드를 적습니다.
     keywords            = ['pypi StringFix'],
     # 해당 패키지를 사용하기 위해 필요한 파이썬 버전을 적습니다.
     python_requires     = '>=3',
     # 파이썬 파일이 아닌 다른 파일을 포함시키고 싶다면 package_data에 포함시켜야 합니다.
     package_data        = {},
     # 위의 package_data에 대한 설정을 하였다면 zip_safe설정도 해주어야 합니다.
```

