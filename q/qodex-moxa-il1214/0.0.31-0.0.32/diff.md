# Comparing `tmp/qodex_moxa_il1214-0.0.31-py3-none-any.whl.zip` & `tmp/qodex_moxa_il1214-0.0.32-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2247 bytes, number of entries: 6
+Zip file size: 2274 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-19 12:26 moxa_contr/__init__.py
--rw-rw-rw-  2.0 fat     2825 b- defN 23-Apr-20 10:17 moxa_contr/main.py
--rw-rw-rw-  2.0 fat      162 b- defN 23-Apr-20 10:17 qodex_moxa_il1214-0.0.31.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 10:17 qodex_moxa_il1214-0.0.31.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-20 10:17 qodex_moxa_il1214-0.0.31.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      492 b- defN 23-Apr-20 10:17 qodex_moxa_il1214-0.0.31.dist-info/RECORD
-6 files, 3582 bytes uncompressed, 1345 bytes compressed:  62.5%
+-rw-rw-rw-  2.0 fat     2798 b- defN 23-Apr-20 10:23 moxa_contr/main.py
+-rw-rw-rw-  2.0 fat      187 b- defN 23-Apr-20 10:23 qodex_moxa_il1214-0.0.32.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 10:23 qodex_moxa_il1214-0.0.32.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-20 10:23 qodex_moxa_il1214-0.0.32.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      492 b- defN 23-Apr-20 10:23 qodex_moxa_il1214-0.0.32.dist-info/RECORD
+6 files, 3580 bytes uncompressed, 1372 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: moxa_contr/__init__.py
 Comment: 
 
 Filename: moxa_contr/main.py
 Comment: 
 
-Filename: qodex_moxa_il1214-0.0.31.dist-info/METADATA
+Filename: qodex_moxa_il1214-0.0.32.dist-info/METADATA
 Comment: 
 
-Filename: qodex_moxa_il1214-0.0.31.dist-info/WHEEL
+Filename: qodex_moxa_il1214-0.0.32.dist-info/WHEEL
 Comment: 
 
-Filename: qodex_moxa_il1214-0.0.31.dist-info/top_level.txt
+Filename: qodex_moxa_il1214-0.0.32.dist-info/top_level.txt
 Comment: 
 
-Filename: qodex_moxa_il1214-0.0.31.dist-info/RECORD
+Filename: qodex_moxa_il1214-0.0.32.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## moxa_contr/main.py

```diff
@@ -1,10 +1,9 @@
 import json
 import time
-
 import requests
 
 
 class MoxaServer:
     schema = "http://"
     api_io = f"/api/slot/0/io"
     api_io_di = f"/api/slot/0/io/di"
@@ -40,22 +39,22 @@
 
 
 class MoxaDevice(MoxaServer):
     index = None
     ip = None
     status_on = 1
     status_off = 0
+    api_relay = f"{super().api_io}/relay/{index}"
+    relay_status_link = f"{api_relay}/relayStatus"
 
     def __init__(self, ip, index, status_on=1, status_off=0):
         super().__init__(ip=ip)
         self.index = index
         self.status_on = status_on
         self.status_off = status_off
-        self.api_relay = f"{self.api_io}/relay/{self.index}"
-        self.relay_status_link = f"{self.api_relay}/relayStatus"
 
     def get_relay_info(self):
         return self.get_info(self.relay_status_link)
 
     def get_di_status(self):
         return self.get_info(f"{self.api_io_di}/{self.index}/diStatus")
```

