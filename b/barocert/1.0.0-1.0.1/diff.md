# Comparing `tmp/barocert-1.0.0-py3-none-any.whl.zip` & `tmp/barocert-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6812 bytes, number of entries: 8
--rw-r--r--  2.0 unx      340 b- defN 23-Apr-20 05:49 barocert/__init__.py
+Zip file size: 6807 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      340 b- defN 23-Apr-20 07:38 barocert/__init__.py
 -rw-r--r--  2.0 unx      441 b- defN 23-Apr-20 05:49 barocert/base.py
--rw-r--r--  2.0 unx    25674 b- defN 23-Apr-20 05:49 barocert/kakaocertService.py
--rw-r--r--  2.0 unx     1063 b- defN 23-Apr-20 06:06 barocert-1.0.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1021 b- defN 23-Apr-20 06:06 barocert-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 06:06 barocert-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-20 06:06 barocert-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      627 b- defN 23-Apr-20 06:06 barocert-1.0.0.dist-info/RECORD
-8 files, 29267 bytes uncompressed, 5720 bytes compressed:  80.5%
+-rw-r--r--  2.0 unx    25676 b- defN 23-Apr-20 07:38 barocert/kakaocertService.py
+-rw-r--r--  2.0 unx     1063 b- defN 23-Apr-20 07:38 barocert-1.0.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1021 b- defN 23-Apr-20 07:38 barocert-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 07:38 barocert-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-20 07:38 barocert-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      627 b- defN 23-Apr-20 07:38 barocert-1.0.1.dist-info/RECORD
+8 files, 29269 bytes uncompressed, 5715 bytes compressed:  80.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: barocert/base.py
 Comment: 
 
 Filename: barocert/kakaocertService.py
 Comment: 
 
-Filename: barocert-1.0.0.dist-info/LICENSE.md
+Filename: barocert-1.0.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: barocert-1.0.0.dist-info/METADATA
+Filename: barocert-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: barocert-1.0.0.dist-info/WHEEL
+Filename: barocert-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: barocert-1.0.0.dist-info/top_level.txt
+Filename: barocert-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: barocert-1.0.0.dist-info/RECORD
+Filename: barocert-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## barocert/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 Version = __version__  # for backward compatibility
 __all__ = ["BarocertException",
            "KakaoCMS",
            "KakaoIdentity",
            "KakaoSign",
            "KakaoMultiSign",
            "KakaoMultiSignTokens",
```

## barocert/kakaocertService.py

```diff
@@ -294,15 +294,15 @@
             raise BarocertException(-99999999, "원문 유형이 입력되지 않았습니다.")
         
         postData = self._stringtify(sign)
 
         return self._httppost('/KAKAO/Sign/' + clientCode, postData)
 
     # 전자서명 상태확인(단건)
-    def getSignState(self, clientCode, receiptId):
+    def getSignStatus(self, clientCode, receiptId):
 
         if clientCode == None or clientCode == "":
             raise BarocertException(-99999999, "이용기관코드가 입력되지 않았습니다.")
         if False == clientCode.isdigit():
             raise BarocertException(-99999999, "이용기관코드는 숫자만 입력할 수 있습니다.")
         if 12 != len(clientCode):
             raise BarocertException(-99999999, "이용기관코드는 12자 입니다.")
@@ -370,15 +370,15 @@
             raise BarocertException(-99999999, "원문 유형이 입력되지 않았습니다.")
 
         postData = self._stringtify(multiSign)
 
         return self._httppost('/KAKAO/MultiSign/' + clientCode, postData)
 
     # 전자서명 상태확인(복수)	
-    def getMultiSignState(self, clientCode, receiptId):
+    def getMultiSignStatus(self, clientCode, receiptId):
 
         if clientCode == None or clientCode == "":
             raise BarocertException(-99999999, "이용기관코드가 입력되지 않았습니다.")
         if False == clientCode.isdigit():
             raise BarocertException(-99999999, "이용기관코드는 숫자만 입력할 수 있습니다.")
         if 12 != len(clientCode):
             raise BarocertException(-99999999, "이용기관코드는 12자 입니다.")
```

## Comparing `barocert-1.0.0.dist-info/LICENSE.md` & `barocert-1.0.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `barocert-1.0.0.dist-info/METADATA` & `barocert-1.0.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: barocert
-Version: 1.0.0
+Version: 1.0.1
 Summary: barocert API SDK Library
 Home-page: https://github.com/barocert/barocert.py
 Author: linkhub dev
 Author-email: dev@linkhubcorp.com
 License: MIT
-Download-URL: https://github.com/barocert/barocert.py/archive/1.0.0.tar.gz
+Download-URL: https://github.com/barocert/barocert.py/archive/1.0.1.tar.gz
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Classifier: Programming Language :: Python :: 2
```

## Comparing `barocert-1.0.0.dist-info/RECORD` & `barocert-1.0.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-barocert/__init__.py,sha256=iFwQ74DMcyilWS1rIVl4nT5yOc0S97NZkHp04Z8RavI,340
+barocert/__init__.py,sha256=3PdVxuAhYMQ1dZk0Vrnjdxu9apepbCPcb91G2ng4ck8,340
 barocert/base.py,sha256=n6NNgtfuMRKayr6vbifvtBfS3J35_nUe2hn-4A2vj0c,441
-barocert/kakaocertService.py,sha256=Y-ZBJ2s-lIMDwrxsoQF1znPpRoMsOjK01KhbOcsyFxA,25674
-barocert-1.0.0.dist-info/LICENSE.md,sha256=FgvZ7zQW0iu6hPMI_pW3dGC34UR54H9pu9mZFHZCRwY,1063
-barocert-1.0.0.dist-info/METADATA,sha256=-06FKiT2OcMin3Yru2bqywX4Q57wRkLXcUxdcjVL9oo,1021
-barocert-1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-barocert-1.0.0.dist-info/top_level.txt,sha256=mu-ftFIfC4GdiuUrj0ySBS3huVW01oxR5_95sWWFoWA,9
-barocert-1.0.0.dist-info/RECORD,,
+barocert/kakaocertService.py,sha256=7XJTuGtZfUq-X2ZzqMm6zSxQXzVMlHKAoDvZo73zx_A,25676
+barocert-1.0.1.dist-info/LICENSE.md,sha256=FgvZ7zQW0iu6hPMI_pW3dGC34UR54H9pu9mZFHZCRwY,1063
+barocert-1.0.1.dist-info/METADATA,sha256=zxNd4Uh99TGr0A4QDudxCQQgEH__5fDtIcTuu2T5CeQ,1021
+barocert-1.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+barocert-1.0.1.dist-info/top_level.txt,sha256=mu-ftFIfC4GdiuUrj0ySBS3huVW01oxR5_95sWWFoWA,9
+barocert-1.0.1.dist-info/RECORD,,
```

