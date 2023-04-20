# Comparing `tmp/channels_yroom-0.0.1.tar.gz` & `tmp/channels_yroom-0.0.2.tar.gz`

## Comparing `channels_yroom-0.0.1.tar` & `channels_yroom-0.0.2.tar`

### file list

```diff
@@ -1,59 +1,56 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/.DS_Store
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/admin.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/apps.py
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/channel.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/conf.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/consumer.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/models.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/storage.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/utils.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/worker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/management/commands/__init__.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/management/commands/yroom.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/channels_yroom/migrations/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/.dockerignore
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/Dockerfile
--rw-r--r--   0        0        0   147456 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/db.sqlite3
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/docker-compose.yml
--rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/manage.py
--rw-r--r--   0        0        0    75131 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/package-lock.json
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/package.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/requirements.txt
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/vite.config.js
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/frontend/.DS_Store
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/frontend/main.js
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/frontend/prosemirror.js
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/frontend/schema.js
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/frontend/style.css
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab/admin.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab/apps.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab/consumers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab/models.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab/routing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab/tests.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab/urls.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab/views.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab/migrations/__init__.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab/templates/textcollab/index.html
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab/templates/textcollab/room.html
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab_project/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab_project/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab_project/asgi.py
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab_project/settings.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab_project/urls.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/example/textcollab_project/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/tests/test_consumer.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/LICENSE
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/README.md
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 channels_yroom-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/.dockerignore
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/Dockerfile
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/docker-compose.yml
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/admin.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/apps.py
+-rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/channel.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/conf.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/consumer.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/models.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/storage.py
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/utils.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/worker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/management/commands/__init__.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/management/commands/yroom.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/migrations/__init__.py
+-rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/manage.py
+-rw-r--r--   0        0        0    75131 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/package-lock.json
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/package.json
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/requirements.txt
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/vite.config.js
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/frontend/main.js
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/frontend/prosemirror.js
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/frontend/schema.js
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/frontend/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/admin.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/apps.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/consumers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/models.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/routing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/tests.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/urls.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/views.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/migrations/__init__.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/templates/textcollab/index.html
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/templates/textcollab/room.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab_project/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab_project/asgi.py
+-rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab_project/settings.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab_project/urls.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab_project/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/tests/test_consumer.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/README.md
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/PKG-INFO
```

### Comparing `channels_yroom-0.0.1/channels_yroom/consumer.py` & `channels_yroom-0.0.2/channels_yroom/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import random
 import logging
+import random
 from typing import Optional
 
 from channels.generic.websocket import AsyncWebsocketConsumer
 
 from .conf import settings
 from .utils import (
     YroomChannelMessage,
@@ -19,17 +19,14 @@
     def get_room_group_name(self) -> str:
         return "yroom_default"
 
     def get_connection_id(self) -> int:
         return random.getrandbits(64)
 
     async def connect(self) -> None:
-        # import ipdb
-
-        # ipdb.set_trace()
         await self.join_room()
 
     async def join_room(self) -> None:
         # Join room group
         self.room_group_name = self.get_room_group_name()
         self.conn_id = self.get_connection_id()
```

### Comparing `channels_yroom-0.0.1/channels_yroom/models.py` & `channels_yroom-0.0.2/channels_yroom/models.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.1/channels_yroom/storage.py` & `channels_yroom-0.0.2/channels_yroom/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Protocol, Optional
-
-from django.utils.module_loading import import_string
+from typing import Optional, Protocol
 
 from asgiref.sync import sync_to_async
+from django.utils.module_loading import import_string
 
-from .models import YDocUpdate
 from .conf import settings
+from .models import YDocUpdate
 
 
 class YDocStorage(Protocol):
     async def get_snapshot(self, name: str) -> Optional[bytes]:
         ...
 
     async def save_snapshot(self, name: str, data: bytes) -> None:
```

### Comparing `channels_yroom-0.0.1/channels_yroom/worker.py` & `channels_yroom-0.0.2/channels_yroom/worker.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.1/channels_yroom/management/commands/yroom.py` & `channels_yroom-0.0.2/channels_yroom/management/commands/yroom.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 
-from django.core.management import BaseCommand, CommandError
-
 from channels import DEFAULT_CHANNEL_LAYER
 from channels.layers import get_channel_layer
 from channels.routing import get_default_application
+from django.core.management import BaseCommand, CommandError
 
 from ...conf import settings
 from ...worker import YroomWorker
 
 logger = logging.getLogger("django.channels.worker")
```

### Comparing `channels_yroom-0.0.1/channels_yroom/migrations/0001_initial.py` & `channels_yroom-0.0.2/channels_yroom/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.1/example/docker-compose.yml` & `channels_yroom-0.0.2/docker-compose.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 version: '3'
 
 x-app-defaults:
   &app_defaults
   build: .
-  command: uvicorn textcollab_project.asgi:application
+  init: true
   links:
-    - db
     - broker
   environment:
-    - DATABASE_URL=://postgres@db/postgres
+    - REDIS_HOST=broker
   depends_on:
-    - db
     - broker
 
 services:
   db:
-    image: postgres:15.2
+    image: postgres:15
     volumes:
-      - postgres-data:/var/lib/postgresql/data/
+      - postgres_data:/var/lib/postgresql/data/
+    environment:
+      - "POSTGRES_HOST_AUTH_METHOD=trust"
+      - "DJANGO_DEBUG=0"
   broker:
     image: redis:5
     volumes:
       - "redis-data:/data"
   app:
     <<: *app_defaults
-    command: uvicorn textcollab_project.asgi:application
+    command: "uvicorn --host 0.0.0.0 textcollab_project.asgi:application"
     ports:
-      - "8000:8000"
+      - "127.0.0.1:8000:8000"
+    expose:
+      - 8000
   worker:
     <<: *app_defaults
-    command: python manage.py yroom
+    command: "python manage.py yroom"
 
 volumes:
-  postgres-data: {}
   redis-data: {}
+  postgres_data: {}
```

### Comparing `channels_yroom-0.0.1/example/manage.py` & `channels_yroom-0.0.2/example/manage.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.1/example/package-lock.json` & `channels_yroom-0.0.2/example/package-lock.json`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.1/example/frontend/schema.js` & `channels_yroom-0.0.2/example/frontend/schema.js`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.1/example/textcollab/migrations/0001_initial.py` & `channels_yroom-0.0.2/example/textcollab/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.1/example/textcollab/templates/textcollab/index.html` & `channels_yroom-0.0.2/example/textcollab/templates/textcollab/index.html`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.1/example/textcollab_project/asgi.py` & `channels_yroom-0.0.2/example/textcollab_project/asgi.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.1/example/textcollab_project/settings.py` & `channels_yroom-0.0.2/example/textcollab_project/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,30 +6,34 @@
 For more information on this file, see
 https://docs.djangoproject.com/en/4.1/topics/settings/
 
 For the full list of settings and their values, see
 https://docs.djangoproject.com/en/4.1/ref/settings/
 """
 
+import os
 from pathlib import Path
 
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 BASE_DIR = Path(__file__).resolve().parent.parent
 
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/4.1/howto/deployment/checklist/
 
 # SECURITY WARNING: keep the secret key used in production secret!
-SECRET_KEY = "django-insecure-3w!ssf@!mc=*tqk_dkqv%mt&*+pw)4=)e4_=lc6uni3i#2x_$6"
+SECRET_KEY = os.environ.get(
+    "DJANGO_SECRET_KEY",
+    "django-insecure-3w!ssf@!mc=*tqk_dkqv%mt&*+pw)4=)e4_=lc6uni3i#2x_$6",
+)
 
 # SECURITY WARNING: don't run with debug turned on in production!
-DEBUG = True
+DEBUG = bool(int(os.environ.get("DJANGO_DEBUG", 1)))
 DJANGO_VITE_DEV_MODE = DEBUG
-ALLOWED_HOSTS = []
+ALLOWED_HOSTS = ["*"]
 
 
 # Application definition
 
 INSTALLED_APPS = [
     "channels",
     "channels_yroom",
@@ -41,14 +45,15 @@
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.staticfiles",
 ]
 
 MIDDLEWARE = [
     "django.middleware.security.SecurityMiddleware",
+    "whitenoise.middleware.WhiteNoiseMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.middleware.clickjacking.XFrameOptionsMiddleware",
 ]
@@ -74,28 +79,41 @@
 WSGI_APPLICATION = "textcollab_project.wsgi.application"
 ASGI_APPLICATION = "textcollab_project.asgi.application"
 
 CHANNEL_LAYERS = {
     "default": {
         "BACKEND": "channels_redis.core.RedisChannelLayer",
         "CONFIG": {
-            "hosts": [("127.0.0.1", 6379)],
+            "hosts": [(os.environ.get("REDIS_HOST", "127.0.0.1"), 6379)],
         },
     },
 }
 
 # Database
 # https://docs.djangoproject.com/en/4.1/ref/settings/#databases
 
-DATABASES = {
-    "default": {
-        "ENGINE": "django.db.backends.sqlite3",
-        "NAME": BASE_DIR / "db.sqlite3",
+
+if DEBUG:
+    DATABASES = {
+        "default": {
+            "ENGINE": "django.db.backends.sqlite3",
+            "NAME": BASE_DIR / "db.sqlite3",
+        }
+    }
+else:
+    DATABASES = {
+        "default": {
+            "ENGINE": "django.db.backends.postgresql",
+            "NAME": "postgres",
+            "USER": "postgres",
+            "PASSWORD": "postgres",
+            "HOST": "db",  # set in docker-compose.yml
+            "PORT": 5432,  # default postgres port
+        }
     }
-}
 
 
 # Password validation
 # https://docs.djangoproject.com/en/4.1/ref/settings/#auth-password-validators
 
 AUTH_PASSWORD_VALIDATORS = [
     {
@@ -130,14 +148,16 @@
 
 STATIC_URL = "static/"
 
 DJANGO_VITE_ASSETS_PATH = BASE_DIR / "build"
 DJANGO_VITE_DEV_SERVER_PORT = 5173
 
 STATICFILES_DIRS = [DJANGO_VITE_ASSETS_PATH]
+STATIC_ROOT = BASE_DIR / "public"
+STATICFILES_STORAGE = "whitenoise.storage.CompressedManifestStaticFilesStorage"
 
 # Default primary key field type
 # https://docs.djangoproject.com/en/4.1/ref/settings/#default-auto-field
 
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 
 
@@ -151,27 +171,22 @@
     "filters": {"require_debug_false": {"()": "django.utils.log.RequireDebugFalse"}},
     "formatters": {
         "verbose": {
             "format": "%(levelname)s %(asctime)s %(module)s %(process)d %(thread)d %(message)s"
         },
     },
     "handlers": {
-        "mail_admins": {
-            "level": "ERROR",
-            "filters": ["require_debug_false"],
-            "class": "django.utils.log.AdminEmailHandler",
-        },
         "console": {
             "level": "DEBUG",
             "class": "logging.StreamHandler",
         },
     },
     "loggers": {
         "django.request": {
-            "handlers": ["mail_admins"],
+            "handlers": ["console"],
             "level": "ERROR",
             "propagate": True,
         },
         "django.db.backends": {
             "level": "ERROR",
             "handlers": ["console"],
             "propagate": False,
```

### Comparing `channels_yroom-0.0.1/example/textcollab_project/urls.py` & `channels_yroom-0.0.2/example/textcollab_project/urls.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.1/tests/conftest.py` & `channels_yroom-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.1/tests/test_consumer.py` & `channels_yroom-0.0.2/tests/test_consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import pytest
-
 from asgiref.testing import ApplicationCommunicator
 from channels.layers import get_channel_layer
 from channels.testing import WebsocketCommunicator
 
-from channels_yroom.consumer import YroomConsumer
-from channels_yroom.conf import settings
 from channels_yroom.channel import YRoomChannelConsumer
+from channels_yroom.conf import settings
+from channels_yroom.consumer import YroomConsumer
 from channels_yroom.models import YDocUpdate
 
 
 async def forward_to_yroom_worker(channel_layer, worker_communicator):
     # Receive message on yroom channel layer...
     message = await channel_layer.receive(settings.YROOM_CHANNEL_NAME)
     # ... and give it to worker consumer
```

### Comparing `channels_yroom-0.0.1/LICENSE` & `channels_yroom-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.1/README.md` & `channels_yroom-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Channels-Yroom
 
-Django Channels Websocket consumer and worker for the Yjs network protocol
-
-`channels-yroom` implements the network protocol for Yjs doc synchronization and awareness updates and makes them available as a Django Channels Websocket consumer and worker.
+`channels-yroom` is a Django Channels WebSocket consumer and worker for synchronizing Yjs clients. It implements the network protocol for Yjs doc synchronization and awareness updates and makes them available as Django Channels WebSocket consumer and worker.
 
 ## Get started
 
-1. Add `channels` and `channels_yroom` to `INSTALLED_APPS` in your settings.
+1. Install:
+
+    `pip install channels-yroom`
 
-2. Set up your websocket consumer.
+2. Add `channels` and `channels_yroom` to `INSTALLED_APPS` in your settings.
 
-   These can be quite simple
+3. Set up your WebSocket consumer in `consumers.py`.
 
    ```python
 
     from channels_yroom.consumer import YroomConsumer
 
     class TextCollaborationConsumer(YroomConsumer):
         def get_room_group_name(self) -> str:
@@ -23,25 +23,24 @@
             """
             room_name = self.scope["url_route"]["kwargs"]["room_name"]
             return "textcollab_%s" % room_name
 
         async def connect(self) -> None:
             """
             Optional: perform some sort of authentication
-            Call .join_room() to connect client to document
             """
             user = self.scope["user"]
             if not user.is_staff:
                 await self.close()
                 return
 
             await super().connect()
     ```
 
-3. Hook your websocket patterns in your `asgi.py` and add a `"channel"` protocol router for the `"yroom"` channel name:
+4. Hook your WebSocket patterns in your `asgi.py` and add a `"channel"` protocol router for the `"yroom"` channel name:
 
     ```python
     # ...
     application = ProtocolTypeRouter(
         {
             "http": get_asgi_application(),
             "websocket": AllowedHostsOriginValidator(
@@ -52,24 +51,38 @@
                     "yroom": YRoomChannelConsumer.as_asgi(),
                 }
             ),
         }
     )
     ```
 
-4. In addition to your webserver with websockets support (e.g. daphne or uvicorn), you need to run a [channels worker](https://channels.readthedocs.io/en/stable/topics/worker.html). You can run the `yroom` worker implementation that supports graceful shutdown:
+5. In addition to your webserver with WebSockets support (e.g. daphne or uvicorn), you need to run a [channels worker](https://channels.readthedocs.io/en/stable/topics/worker.html). You can run the `yroom` worker implementation that supports graceful shutdown:
 
     ```sh
     python manage.py yroom
     ```
 
 
+## Showcase: text collaboration example
+
+The `example` folder contains a simple project that uses `y-prosemirror` to allow for realtime collaboration on rich text.
+
+Run the included Docker compose file to check it out:
+
+```sh
+docker compose up
+# Then visit localhost:8000
+```
+
+
 ## How it works
 
-Yjs clients connect via Websocket to a Channels Websocket Consumer which can perform e.g. authentication and then forwards messages via channel layer to a central worker. This worker runs in a separate process and keeps a Yjs document + awareness information for each 'room', processes synchronization and awareness updates and sends responses (single and broadcast to room) to the Websocket consumers.
+Yjs clients connect via WebSockets to a Channels WebSocket Consumer which can perform e.g. authentication and then forwards messages via channel layer to a central worker. This worker runs in a separate process and keeps a Yjs document + awareness information for each 'room', processes synchronization and awareness updates and sends responses (single and broadcast to room) to the WebSocket consumers.
+
+Under the hood, this project uses [`yroom`](https://github.com/stefanw/yroom/) which is high-level Python binding to a Yjs synchronization and awareness implementation in Rust based on the [official Yjs Rust port](https://github.com/y-crdt).
 
 
 ### Example flow
 
 ```mermaid
 sequenceDiagram
     participant Alice
```

### Comparing `channels_yroom-0.0.1/pyproject.toml` & `channels_yroom-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "channels-yroom"
 description = 'Yjs sync protocol server for Django channels'
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Stefan Wehrmeyer", email = "mail@stefanwehrmeyer.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
@@ -27,48 +26,72 @@
   "Django >= 3.2",
   "channels >= 4.0",
   "yroom >= 0.0.2",
   "django-appconf",
 ]
 dynamic = ["version"]
 
-[project.optional-dependencies]
-test = [
+[tool.hatch.envs.test]
+dependencies = [
   "async-timeout",
-  "pytest",
+  "daphne",
   "pytest-asyncio",
   "pytest-cov",
   "pytest-django",
-  "daphne",
+  "pytest",
+]
+
+[tool.hatch.envs.lint]
+skip-install = true
+detached = true
+dependencies = [
+  "black",
+  "isort",
+  "flake8",
+  "Flake8-pyproject",
+]
+
+[tool.hatch.envs.lint.scripts]
+check = [
+  "flake8 channels_yroom tests",
+  "black --check --diff channels_yroom tests",
+  "isort --check-only --diff channels_yroom tests",
 ]
 
 [project.urls]
 Documentation = "https://github.com/stefanw/channels-yroom#readme"
 Issues = "https://github.com/stefanw/channels-yroom/issues"
 Source = "https://github.com/stefanw/channels-yroom"
 
 [tool.hatch.version]
 path = "channels_yroom/__about__.py"
 
 [tool.hatch.build.targets.wheel]
 packages = ["channels_yroom"]
 
-[tool.hatch.envs.default.scripts]
-cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=channels_yroom --cov=tests {args}"
-no-cov = "cov --no-cov {args}"
+[tool.hatch.envs.test.scripts]
+test = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=channels_yroom --cov=tests {args}"
+no-cov = "test --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
-python = ["37", "38", "39", "310", "311"]
+python = ["3.8", "3.9", "3.10", "3.11"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "channels_yroom/__about__.py",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[tool.flake8]
+extend-ignore = ['E203']
+max-line-length = 88
+
+[tool.isort]
+profile = 'black'
```

### Comparing `channels_yroom-0.0.1/PKG-INFO` & `channels_yroom-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,45 @@
 Metadata-Version: 2.1
 Name: channels-yroom
-Version: 0.0.1
+Version: 0.0.2
 Summary: Yjs sync protocol server for Django channels
 Project-URL: Documentation, https://github.com/stefanw/channels-yroom#readme
 Project-URL: Issues, https://github.com/stefanw/channels-yroom/issues
 Project-URL: Source, https://github.com/stefanw/channels-yroom
 Author-email: Stefan Wehrmeyer <mail@stefanwehrmeyer.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: channels>=4.0
 Requires-Dist: django-appconf
 Requires-Dist: django>=3.2
 Requires-Dist: yroom>=0.0.2
-Provides-Extra: test
-Requires-Dist: async-timeout; extra == 'test'
-Requires-Dist: daphne; extra == 'test'
-Requires-Dist: pytest; extra == 'test'
-Requires-Dist: pytest-asyncio; extra == 'test'
-Requires-Dist: pytest-cov; extra == 'test'
-Requires-Dist: pytest-django; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Channels-Yroom
 
-Django Channels Websocket consumer and worker for the Yjs network protocol
-
-`channels-yroom` implements the network protocol for Yjs doc synchronization and awareness updates and makes them available as a Django Channels Websocket consumer and worker.
+`channels-yroom` is a Django Channels WebSocket consumer and worker for synchronizing Yjs clients. It implements the network protocol for Yjs doc synchronization and awareness updates and makes them available as Django Channels WebSocket consumer and worker.
 
 ## Get started
 
-1. Add `channels` and `channels_yroom` to `INSTALLED_APPS` in your settings.
+1. Install:
+
+    `pip install channels-yroom`
 
-2. Set up your websocket consumer.
+2. Add `channels` and `channels_yroom` to `INSTALLED_APPS` in your settings.
 
-   These can be quite simple
+3. Set up your WebSocket consumer in `consumers.py`.
 
    ```python
 
     from channels_yroom.consumer import YroomConsumer
 
     class TextCollaborationConsumer(YroomConsumer):
         def get_room_group_name(self) -> str:
@@ -56,25 +48,24 @@
             """
             room_name = self.scope["url_route"]["kwargs"]["room_name"]
             return "textcollab_%s" % room_name
 
         async def connect(self) -> None:
             """
             Optional: perform some sort of authentication
-            Call .join_room() to connect client to document
             """
             user = self.scope["user"]
             if not user.is_staff:
                 await self.close()
                 return
 
             await super().connect()
     ```
 
-3. Hook your websocket patterns in your `asgi.py` and add a `"channel"` protocol router for the `"yroom"` channel name:
+4. Hook your WebSocket patterns in your `asgi.py` and add a `"channel"` protocol router for the `"yroom"` channel name:
 
     ```python
     # ...
     application = ProtocolTypeRouter(
         {
             "http": get_asgi_application(),
             "websocket": AllowedHostsOriginValidator(
@@ -85,24 +76,38 @@
                     "yroom": YRoomChannelConsumer.as_asgi(),
                 }
             ),
         }
     )
     ```
 
-4. In addition to your webserver with websockets support (e.g. daphne or uvicorn), you need to run a [channels worker](https://channels.readthedocs.io/en/stable/topics/worker.html). You can run the `yroom` worker implementation that supports graceful shutdown:
+5. In addition to your webserver with WebSockets support (e.g. daphne or uvicorn), you need to run a [channels worker](https://channels.readthedocs.io/en/stable/topics/worker.html). You can run the `yroom` worker implementation that supports graceful shutdown:
 
     ```sh
     python manage.py yroom
     ```
 
 
+## Showcase: text collaboration example
+
+The `example` folder contains a simple project that uses `y-prosemirror` to allow for realtime collaboration on rich text.
+
+Run the included Docker compose file to check it out:
+
+```sh
+docker compose up
+# Then visit localhost:8000
+```
+
+
 ## How it works
 
-Yjs clients connect via Websocket to a Channels Websocket Consumer which can perform e.g. authentication and then forwards messages via channel layer to a central worker. This worker runs in a separate process and keeps a Yjs document + awareness information for each 'room', processes synchronization and awareness updates and sends responses (single and broadcast to room) to the Websocket consumers.
+Yjs clients connect via WebSockets to a Channels WebSocket Consumer which can perform e.g. authentication and then forwards messages via channel layer to a central worker. This worker runs in a separate process and keeps a Yjs document + awareness information for each 'room', processes synchronization and awareness updates and sends responses (single and broadcast to room) to the WebSocket consumers.
+
+Under the hood, this project uses [`yroom`](https://github.com/stefanw/yroom/) which is high-level Python binding to a Yjs synchronization and awareness implementation in Rust based on the [official Yjs Rust port](https://github.com/y-crdt).
 
 
 ### Example flow
 
 ```mermaid
 sequenceDiagram
     participant Alice
```

