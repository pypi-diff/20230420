# Comparing `tmp/anyon-3.1.20-cp311-cp311-win_amd64.whl.zip` & `tmp/anyon-3.1.22-cp311-cp311-macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 366753 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     1080 b- defN 23-Apr-19 04:10 anyon-3.1.20.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1193 b- defN 23-Apr-19 04:10 anyon-3.1.20.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Apr-19 04:10 anyon-3.1.20.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-19 04:10 anyon-3.1.20.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      381 b- defN 23-Apr-19 04:10 anyon-3.1.20.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20480 b- defN 23-Apr-19 04:10 anyon/__init__.pyd
--rw-rw-rw-  2.0 fat    78336 b- defN 23-Apr-19 04:10 anyon/loader.pyd
--rw-rw-rw-  2.0 fat    99840 b- defN 23-Apr-19 04:10 anyon/remote.pyd
--rw-rw-rw-  2.0 fat   180736 b- defN 23-Apr-19 04:10 anyon/server.pyd
--rw-rw-rw-  2.0 fat    20992 b- defN 23-Apr-19 04:10 anyon/stage/__init__.pyd
--rw-rw-rw-  2.0 fat    92672 b- defN 23-Apr-19 04:10 anyon/stage/calculator.pyd
--rw-rw-rw-  2.0 fat   134144 b- defN 23-Apr-19 04:10 anyon/stage/compiler.pyd
--rw-rw-rw-  2.0 fat    61952 b- defN 23-Apr-19 04:10 anyon/stage/demodulator.pyd
--rw-rw-rw-  2.0 fat   114176 b- defN 23-Apr-19 04:10 anyon/stage/device.pyd
-14 files, 806085 bytes uncompressed, 364981 bytes compressed:  54.7%
+Zip file size: 854347 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1059 b- defN 23-Apr-20 02:24 anyon-3.1.22.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1142 b- defN 23-Apr-20 02:24 anyon-3.1.22.dist-info/METADATA
+-rw-r--r--  2.0 unx      115 b- defN 23-Apr-20 02:24 anyon-3.1.22.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-20 02:24 anyon-3.1.22.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      381 b- defN 23-Apr-20 02:24 anyon-3.1.22.dist-info/RECORD
+-rwxr-xr-x  2.0 unx   121984 b- defN 23-Apr-20 02:23 anyon/__init__.so
+-rwxr-xr-x  2.0 unx   288798 b- defN 23-Apr-20 02:24 anyon/loader.so
+-rwxr-xr-x  2.0 unx   360478 b- defN 23-Apr-20 02:23 anyon/remote.so
+-rwxr-xr-x  2.0 unx   605166 b- defN 23-Apr-20 02:23 anyon/server.so
+-rwxr-xr-x  2.0 unx   122256 b- defN 23-Apr-20 02:24 anyon/stage/__init__.so
+-rwxr-xr-x  2.0 unx   324082 b- defN 23-Apr-20 02:24 anyon/stage/calculator.so
+-rwxr-xr-x  2.0 unx   470688 b- defN 23-Apr-20 02:24 anyon/stage/compiler.so
+-rwxr-xr-x  2.0 unx   236611 b- defN 23-Apr-20 02:24 anyon/stage/demodulator.so
+-rwxr-xr-x  2.0 unx   392334 b- defN 23-Apr-20 02:24 anyon/stage/device.so
+14 files, 2925095 bytes uncompressed, 852593 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -1,43 +1,43 @@
-Filename: anyon-3.1.20.dist-info/LICENSE
+Filename: anyon-3.1.22.dist-info/LICENSE
 Comment: 
 
-Filename: anyon-3.1.20.dist-info/METADATA
+Filename: anyon-3.1.22.dist-info/METADATA
 Comment: 
 
-Filename: anyon-3.1.20.dist-info/WHEEL
+Filename: anyon-3.1.22.dist-info/WHEEL
 Comment: 
 
-Filename: anyon-3.1.20.dist-info/top_level.txt
+Filename: anyon-3.1.22.dist-info/top_level.txt
 Comment: 
 
-Filename: anyon-3.1.20.dist-info/RECORD
+Filename: anyon-3.1.22.dist-info/RECORD
 Comment: 
 
-Filename: anyon/__init__.pyd
+Filename: anyon/__init__.so
 Comment: 
 
-Filename: anyon/loader.pyd
+Filename: anyon/loader.so
 Comment: 
 
-Filename: anyon/remote.pyd
+Filename: anyon/remote.so
 Comment: 
 
-Filename: anyon/server.pyd
+Filename: anyon/server.so
 Comment: 
 
-Filename: anyon/stage/__init__.pyd
+Filename: anyon/stage/__init__.so
 Comment: 
 
-Filename: anyon/stage/calculator.pyd
+Filename: anyon/stage/calculator.so
 Comment: 
 
-Filename: anyon/stage/compiler.pyd
+Filename: anyon/stage/compiler.so
 Comment: 
 
-Filename: anyon/stage/demodulator.pyd
+Filename: anyon/stage/demodulator.so
 Comment: 
 
-Filename: anyon/stage/device.pyd
+Filename: anyon/stage/device.so
 Comment: 
 
 Zip file comment:
```

## Comparing `anyon-3.1.20.dist-info/METADATA` & `anyon-3.1.22.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-Metadata-Version: 2.1
-Name: anyon
-Version: 3.1.20
-Summary: Dream It Possible!
-Home-page: https://gitee.com/
-Author: YL Feng
-Author-email: fengyulong@pku.edu.cn
-License: MIT
-Project-URL: source, https://gitee.com
-Keywords: Hello,World!
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy (>=1.20.0)
-Requires-Dist: axion (>=3.2.20)
-Requires-Dist: srpc (>=4.2.7)
-Requires-Dist: zee (>=0.0.2)
-Requires-Dist: requests (>=2.28.0)
-
-#### 介绍
-
-
-#### 软件架构
-
-
-#### 安装教程
-
-
-#### 使用说明
-
-
-#### 参与贡献
-
-
-#### 特技
-
-
-
-
-
+Metadata-Version: 2.1
+Name: anyon
+Version: 3.1.22
+Summary: Dream It Possible!
+Home-page: https://gitee.com/
+Author: YL Feng
+Author-email: fengyulong@pku.edu.cn
+License: MIT
+Project-URL: source, https://gitee.com
+Keywords: Hello,World!
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.10.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy (>=1.20.0)
+Requires-Dist: axion (>=3.2.20)
+Requires-Dist: srpc (>=4.2.7)
+Requires-Dist: zee (>=0.0.2)
+Requires-Dist: requests (>=2.28.0)
+
+#### 介绍
+
+
+#### 软件架构
+
+
+#### 安装教程
+
+
+#### 使用说明
+
+
+#### 参与贡献
+
+
+#### 特技
+
+
+
+
+
```

