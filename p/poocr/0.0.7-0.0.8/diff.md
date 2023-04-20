# Comparing `tmp/poocr-0.0.7.tar.gz` & `tmp/poocr-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poocr-0.0.7.tar", last modified: Tue Apr 18 16:21:14 2023, max compression
+gzip compressed data, was "poocr-0.0.8.tar", last modified: Thu Apr 20 14:36:10 2023, max compression
```

## Comparing `poocr-0.0.7.tar` & `poocr-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 16:21:14.121553 poocr-0.0.7/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     4115 2023-04-18 16:21:14.121553 poocr-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3594 2023-04-18 15:02:36.000000 poocr-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 16:21:14.078671 poocr-0.0.7/poocr/
--rw-rw-rw-   0        0        0      522 2023-04-18 16:20:50.000000 poocr-0.0.7/poocr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:21:14.103478 poocr-0.0.7/poocr/api/
--rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.0.7/poocr/api/__init__.py
--rw-rw-rw-   0        0        0    20975 2023-01-30 12:39:04.000000 poocr-0.0.7/poocr/api/ocr.py
--rw-rw-rw-   0        0        0     3259 2023-04-18 14:46:51.000000 poocr-0.0.7/poocr/api/ocr2excel.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:21:14.107488 poocr-0.0.7/poocr/core/
--rw-rw-rw-   0        0        0     4071 2023-01-30 12:39:04.000000 poocr-0.0.7/poocr/core/OCR.py
--rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.0.7/poocr/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:21:14.116026 poocr-0.0.7/poocr/lib/
--rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.0.7/poocr/lib/CommonUtils.py
--rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.0.7/poocr/lib/Config.py
--rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.0.7/poocr/lib/Const.py
--rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.0.7/poocr/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:21:14.097426 poocr-0.0.7/poocr.egg-info/
--rw-rw-rw-   0        0        0     4115 2023-04-18 16:21:13.000000 poocr-0.0.7/poocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-04-18 16:21:13.000000 poocr-0.0.7/poocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 16:21:13.000000 poocr-0.0.7/poocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-18 16:20:22.000000 poocr-0.0.7/poocr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-04-18 16:21:13.000000 poocr-0.0.7/poocr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-18 16:21:13.000000 poocr-0.0.7/poocr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      741 2023-04-18 16:21:14.124546 poocr-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:21:14.119027 poocr-0.0.7/tests/
--rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.0.7/tests/__init__.py
--rw-rw-rw-   0        0        0      823 2023-04-16 09:36:45.000000 poocr-0.0.7/tests/test_tencent.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:36:10.607901 poocr-0.0.8/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     4115 2023-04-20 14:36:10.608898 poocr-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3594 2023-04-18 15:02:36.000000 poocr-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 14:36:10.545657 poocr-0.0.8/poocr/
+-rw-rw-rw-   0        0        0      522 2023-04-18 16:20:50.000000 poocr-0.0.8/poocr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:36:10.585176 poocr-0.0.8/poocr/api/
+-rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.0.8/poocr/api/__init__.py
+-rw-rw-rw-   0        0        0    20975 2023-01-30 12:39:04.000000 poocr-0.0.8/poocr/api/ocr.py
+-rw-rw-rw-   0        0        0     3438 2023-04-20 14:35:27.000000 poocr-0.0.8/poocr/api/ocr2excel.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:36:10.589672 poocr-0.0.8/poocr/core/
+-rw-rw-rw-   0        0        0     4071 2023-01-30 12:39:04.000000 poocr-0.0.8/poocr/core/OCR.py
+-rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.0.8/poocr/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:36:10.602898 poocr-0.0.8/poocr/lib/
+-rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.0.8/poocr/lib/CommonUtils.py
+-rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.0.8/poocr/lib/Config.py
+-rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.0.8/poocr/lib/Const.py
+-rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.0.8/poocr/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:36:10.568668 poocr-0.0.8/poocr.egg-info/
+-rw-rw-rw-   0        0        0     4115 2023-04-20 14:36:10.000000 poocr-0.0.8/poocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-04-20 14:36:10.000000 poocr-0.0.8/poocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 14:36:10.000000 poocr-0.0.8/poocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-18 16:20:22.000000 poocr-0.0.8/poocr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-04-20 14:36:10.000000 poocr-0.0.8/poocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 14:36:10.000000 poocr-0.0.8/poocr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      741 2023-04-20 14:36:10.611922 poocr-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:36:10.606896 poocr-0.0.8/tests/
+-rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.0.8/tests/__init__.py
+-rw-rw-rw-   0        0        0      947 2023-04-19 16:14:45.000000 poocr-0.0.8/tests/test_tencent.py
```

### Comparing `poocr-0.0.7/LICENSE` & `poocr-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `poocr-0.0.7/PKG-INFO` & `poocr-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.0.7
+Version: 0.0.8
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.0.7 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.0.8 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
```

### Comparing `poocr-0.0.7/README.md` & `poocr-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `poocr-0.0.7/poocr/__init__.py` & `poocr-0.0.8/poocr/__init__.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.7/poocr/api/ocr.py` & `poocr-0.0.8/poocr/api/ocr.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.7/poocr/api/ocr2excel.py` & `poocr-0.0.8/poocr/api/ocr2excel.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,35 +40,38 @@
     else:  # 指定了，但不是xlsx或者xls结束
         raise BaseException(
             f'输出结果名：output_excel参数，必须以xls或者xlsx结尾，您的输入:{output_excel}有误，请修改后重新运行')
     res_df = []  # 装全部识别的结果
     for vat_img in simple_progress(vat_img_files):
         try:
             api_res = VatInvoiceOCR(img_path=str(vat_img), img_url=img_url, configPath=configPath)
+
+            api_res_json = json.loads(str(api_res))
+            VatInvoiceInfos = api_res_json['VatInvoiceInfos']
+            dict_pandas = {}  # 存放一行数据
+            # 读返回值的第一个key
+            for VatInvoiceInfo in VatInvoiceInfos:
+                dict_pandas[VatInvoiceInfo['Name']] = VatInvoiceInfo['Value']
+            # 读返回值的第二个key
+            Items = api_res_json['Items']
+            for Item in Items:
+                dict_pandas.update(Item)
+                res_df.append(pd.DataFrame(dict_pandas, index=[0]))
         except:
             continue
-        api_res_json = json.loads(str(api_res))
-        VatInvoiceInfos = api_res_json['VatInvoiceInfos']
-        dict_pandas = {}  # 存放一行数据
-        # 读返回值的第一个key
-        for VatInvoiceInfo in VatInvoiceInfos:
-            dict_pandas[VatInvoiceInfo['Name']] = VatInvoiceInfo['Value']
-        # 读返回值的第二个key
-        Items = api_res_json['Items']
-        for Item in Items:
-            dict_pandas.update(Item)
-            res_df.append(pd.DataFrame(dict_pandas, index=[0]))
     # 整理全部识别结果
-    res_excel = res_df[0]
-    for index, line_df in enumerate(res_df):
-        if index == 0:
-            continue
-        res_excel = res_excel._append(line_df)
-    pd.DataFrame(res_excel).to_excel(str(abs_output_excel))  # 写入Excel
-
+    if len(res_df)>0:
+        res_excel = res_df[0]
+        for index, line_df in enumerate(res_df):
+            if index == 0:
+                continue
+            res_excel = res_excel._append(line_df)
+        pd.DataFrame(res_excel).to_excel(str(abs_output_excel))  # 写入Excel
+    else:
+        print(f'该文件夹下，没有任何符合条件的发票图片')
 
 def TrainTicketOCR2Excel(input_path: str, output_excel: str = r'./TrainTicketOCR2Excel.xlsx', img_url: str = None,
                          configPath: str = None) -> None:
     ticket_list = []
     ticket_files = get_files(input_path)
     for ticket in simple_progress(ticket_files):
         ticket_info = poocr.ocr.TrainTicketOCR(img_path=ticket, img_url=img_url, configPath=configPath)
```

### Comparing `poocr-0.0.7/poocr/core/OCR.py` & `poocr-0.0.8/poocr/core/OCR.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.7/poocr/lib/CommonUtils.py` & `poocr-0.0.8/poocr/lib/CommonUtils.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.7/poocr/lib/Config.py` & `poocr-0.0.8/poocr/lib/Config.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.7/poocr/lib/Const.py` & `poocr-0.0.8/poocr/lib/Const.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.7/poocr.egg-info/PKG-INFO` & `poocr-0.0.8/poocr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.0.7
+Version: 0.0.8
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.0.7 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.0.8 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
```

### Comparing `poocr-0.0.7/setup.cfg` & `poocr-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f6f 6372 0d0a 7665 7273 696f   = poocr..versio
-00000020: 6e20 3d20 302e 302e 370d 0a64 6573 6372  n = 0.0.7..descr
+00000020: 6e20 3d20 302e 302e 380d 0a64 6573 6372  n = 0.0.8..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f6f 6372 0d0a 6c6f 6e67  tall poocr..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `poocr-0.0.7/tests/test_tencent.py` & `poocr-0.0.8/tests/test_tencent.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,9 +15,13 @@
             img_path=r'C:\Users\Lenovo\Desktop\temp\正面.jpg')
         print(res)
 
     def test_VatInvoiceOCR2Excel(self):
         VatInvoiceOCR2Excel(intput_path=r'C:\Users\Lenovo\Desktop\temp\Snipaste_2023-04-09_22-23-48.png',
                             output_excel=r'./VatInvoiceOCR2Excel.xlsx',
                             configPath=r'./poocr-config.toml')
+
     def test_TrainTicketOCR2Excel(self):
-        TrainTicketOCR2Excel(input_path='', output_excel='',configPath='fdasf')
+        TrainTicketOCR2Excel(input_path='', output_excel='', configPath='fdasf')
+
+    def test_BizLicenseOCR(self):
+        poocr.ocr.BizLicenseOCR(img_path=r'd://test//营业执照的照片.jpg')
```

