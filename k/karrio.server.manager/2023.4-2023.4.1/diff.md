# Comparing `tmp/karrio.server.manager-2023.4-py3-none-any.whl.zip` & `tmp/karrio.server.manager-2023.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 90055 bytes, number of entries: 89
+Zip file size: 90261 bytes, number of entries: 89
 -rw-rw-r--  2.0 unx       64 b- defN 22-Nov-15 19:21 karrio/server/manager/__init__.py
 -rw-rw-r--  2.0 unx       35 b- defN 22-Nov-15 19:21 karrio/server/manager/admin.py
 -rw-rw-r--  2.0 unx      364 b- defN 22-Nov-15 19:21 karrio/server/manager/apps.py
 -rw-rw-r--  2.0 unx    24605 b- defN 23-Mar-27 07:55 karrio/server/manager/models.py
 -rw-rw-r--  2.0 unx       95 b- defN 22-Nov-15 19:21 karrio/server/manager/router.py
 -rw-rw-r--  2.0 unx     1918 b- defN 22-Nov-15 19:21 karrio/server/manager/signals.py
 -rw-rw-r--  2.0 unx      220 b- defN 22-Nov-15 19:21 karrio/server/manager/urls.py
@@ -78,14 +78,14 @@
 -rw-rw-r--  2.0 unx     3533 b- defN 23-Mar-30 05:44 karrio/server/manager/tests/test_trackers.py
 -rw-rw-r--  2.0 unx      356 b- defN 22-Nov-15 19:21 karrio/server/manager/views/__init__.py
 -rw-rw-r--  2.0 unx     4374 b- defN 23-Mar-03 13:50 karrio/server/manager/views/addresses.py
 -rw-rw-r--  2.0 unx     4516 b- defN 23-Mar-03 13:50 karrio/server/manager/views/customs.py
 -rw-rw-r--  2.0 unx     3906 b- defN 23-Mar-18 11:05 karrio/server/manager/views/documents.py
 -rw-rw-r--  2.0 unx     4347 b- defN 23-Mar-03 13:50 karrio/server/manager/views/parcels.py
 -rw-rw-r--  2.0 unx     5236 b- defN 23-Mar-03 13:50 karrio/server/manager/views/pickups.py
--rw-rw-r--  2.0 unx     9300 b- defN 23-Mar-18 05:05 karrio/server/manager/views/shipments.py
+-rw-rw-r--  2.0 unx     9951 b- defN 23-Apr-20 18:14 karrio/server/manager/views/shipments.py
 -rw-rw-r--  2.0 unx    11160 b- defN 23-Mar-29 20:04 karrio/server/manager/views/trackers.py
--rw-rw-r--  2.0 unx      708 b- defN 23-Apr-18 10:32 karrio.server.manager-2023.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 10:32 karrio.server.manager-2023.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 10:32 karrio.server.manager-2023.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     9813 b- defN 23-Apr-18 10:32 karrio.server.manager-2023.4.dist-info/RECORD
-89 files, 327352 bytes uncompressed, 73605 bytes compressed:  77.5%
+-rw-rw-r--  2.0 unx      710 b- defN 23-Apr-20 18:43 karrio.server.manager-2023.4.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 18:43 karrio.server.manager-2023.4.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-20 18:43 karrio.server.manager-2023.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     9821 b- defN 23-Apr-20 18:43 karrio.server.manager-2023.4.1.dist-info/RECORD
+89 files, 328013 bytes uncompressed, 73795 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -249,20 +249,20 @@
 
 Filename: karrio/server/manager/views/shipments.py
 Comment: 
 
 Filename: karrio/server/manager/views/trackers.py
 Comment: 
 
-Filename: karrio.server.manager-2023.4.dist-info/METADATA
+Filename: karrio.server.manager-2023.4.1.dist-info/METADATA
 Comment: 
 
-Filename: karrio.server.manager-2023.4.dist-info/WHEEL
+Filename: karrio.server.manager-2023.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.server.manager-2023.4.dist-info/top_level.txt
+Filename: karrio.server.manager-2023.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.server.manager-2023.4.dist-info/RECORD
+Filename: karrio.server.manager-2023.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/server/manager/views/shipments.py

```diff
@@ -7,14 +7,15 @@
 from rest_framework.response import Response
 from rest_framework.pagination import LimitOffsetPagination
 from django_filters.rest_framework import DjangoFilterBackend
 from django_downloadview import VirtualDownloadView
 from django.core.files.base import ContentFile
 from django.urls import path, re_path
 
+import karrio.lib as lib
 from karrio.server.core.views.api import GenericAPIView, APIView
 from karrio.server.core.filters import ShipmentFilters
 from karrio.server.manager.router import router
 from karrio.server.manager.serializers import (
     process_dictionaries_mutations,
     fetch_shipment_rates,
     PaginatedResult,
@@ -256,31 +257,50 @@
         self,
         request: Request,
         pk: str,
         doc: str = "label",
         format: str = "pdf",
         **kwargs,
     ):
-        """
-        Retrieve a shipment label.
-        """
-        shipment = models.Shipment.objects.get(pk=pk, label__isnull=False)
-        query_params = request.GET.dict()
+        """Retrieve a shipment label."""
+        self.shipment = models.Shipment.objects.get(pk=pk, label__isnull=False)
+        self.document = getattr(self.shipment, doc, None)
+        self.name = f"{doc}_{self.shipment.tracking_number}.{format}"
 
-        self.document = getattr(shipment, doc, None)
-        self.name = f"{doc}_{shipment.tracking_number}.{format}"
-        self.attachment = query_params.get("download", False)
+        query_params = request.GET.dict()
+        self.preview = "preview" in query_params
+        self.attachment = "download" in query_params
 
         response = super(ShipmentDocs, self).get(request, pk, doc, format, **kwargs)
         response["X-Frame-Options"] = "ALLOWALL"
         return response
 
     def get_file(self):
         content = base64.b64decode(self.document or "")
         buffer = io.BytesIO()
+
+        if self.preview and "ZPL" in self.shipment.label_type or "":
+            width, height, dpmm = (4, 6, 8)
+
+            if "8" in self.shipment.label_type:
+                width, height, dpmm = (8, 4, 12)
+
+            _label = lib.failsafe(
+                lambda: lib.zpl_to_pdf(
+                    self.document,
+                    width,
+                    height,
+                    dpmm=dpmm,
+                )
+            )
+
+            if _label is not None:
+                content = base64.b64decode(_label)
+                self.name = self.name.replace("zpl", "pdf")
+
         buffer.write(content)
 
         return ContentFile(buffer.getvalue(), name=self.name)
 
 
 router.urls.append(path("shipments", ShipmentList.as_view(), name="shipment-list"))
 router.urls.append(
```

## Comparing `karrio.server.manager-2023.4.dist-info/METADATA` & `karrio.server.manager-2023.4.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.server.manager
-Version: 2023.4
+Version: 2023.4.1
 Summary: Multi-carrier shipping API Shipments manager module
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `karrio.server.manager-2023.4.dist-info/RECORD` & `karrio.server.manager-2023.4.1.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -77,13 +77,13 @@
 karrio/server/manager/tests/test_trackers.py,sha256=QddPAHw4YD0zcq7Mkkz2Wb8dFPl0iQVkQCHtTddpPw0,3533
 karrio/server/manager/views/__init__.py,sha256=On5tX6Bfy-XOdnix9ZWyVY4TSHU0Fx1RYs9sRN2P5Zk,356
 karrio/server/manager/views/addresses.py,sha256=NWz7MP_yiUFEY_NCxUtqBrjh5P1XuPE6flQI23UpDKM,4374
 karrio/server/manager/views/customs.py,sha256=YBp9Thtj7ICfE3CtOU3WHDXypo2buiJBS81Frs3XypY,4516
 karrio/server/manager/views/documents.py,sha256=2DcYLtctG-xKdHgDzJbWJ0WCx-2kO3yGD8u0F5Y3Czk,3906
 karrio/server/manager/views/parcels.py,sha256=ZPEc2OHNB4d29WxL4qVsjycau5KMQx174PjGExR3PUI,4347
 karrio/server/manager/views/pickups.py,sha256=gOHSgkcHQLEwB3kaZrI0x5-WdkGKui3KxiyXiXcO8Ps,5236
-karrio/server/manager/views/shipments.py,sha256=O8puMJTGdD2w0COkz6ZKIts8terUSkOAs74cO4jOIMg,9300
+karrio/server/manager/views/shipments.py,sha256=g_-WmFMGhFmdVS9-3eEWrueRm1bGfe48jKXdupCvntA,9951
 karrio/server/manager/views/trackers.py,sha256=5NpXTmj448M6UP1yIHvk-V2rcGYF8ZTkMGc-bp4sPYU,11160
-karrio.server.manager-2023.4.dist-info/METADATA,sha256=rH_Z3Fd1EqkLfXymaZ8_66BFzbH0mBw1bJerE3otX0w,708
-karrio.server.manager-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.server.manager-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.server.manager-2023.4.dist-info/RECORD,,
+karrio.server.manager-2023.4.1.dist-info/METADATA,sha256=SmS9muf_KnPKK25F9fJBHZk5ro8f4iVgYWGZjva-u_A,710
+karrio.server.manager-2023.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.server.manager-2023.4.1.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.server.manager-2023.4.1.dist-info/RECORD,,
```

