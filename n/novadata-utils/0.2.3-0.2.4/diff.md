# Comparing `tmp/novadata_utils-0.2.3.tar.gz` & `tmp/novadata_utils-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novadata_utils-0.2.3.tar", last modified: Mon Apr 10 15:15:45 2023, max compression
+gzip compressed data, was "novadata_utils-0.2.4.tar", last modified: Thu Apr 20 10:40:54 2023, max compression
```

## Comparing `novadata_utils-0.2.3.tar` & `novadata_utils-0.2.4.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1066 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/LICENSE
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1019 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/PKG-INFO
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      574 2023-04-10 15:14:28.000000 novadata_utils-0.2.3/README.md
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.377091 novadata_utils-0.2.3/novadata_utils/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       60 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.377091 novadata_utils-0.2.3/novadata_utils/admin/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/admin/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     4353 2023-04-10 14:26:47.000000 novadata_utils-0.2.3/novadata_utils/admin/novadata_model_admin.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      219 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/apps.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.377091 novadata_utils-0.2.3/novadata_utils/auth/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/auth/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      729 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/auth/login_username_email.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.377091 novadata_utils-0.2.3/novadata_utils/forms/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/forms/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/novadata_utils/functions/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      126 2023-04-10 14:20:05.000000 novadata_utils-0.2.3/novadata_utils/functions/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     3573 2023-04-10 14:19:03.000000 novadata_utils-0.2.3/novadata_utils/functions/get_prop.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      416 2023-04-10 14:19:49.000000 novadata_utils-0.2.3/novadata_utils/functions/transform_field.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/novadata_utils/managers/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/managers/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/novadata_utils/middlewares/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/middlewares/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/novadata_utils/migrations/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1232 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/migrations/0001_initial.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/migrations/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/novadata_utils/models/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       76 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/models/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1188 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/models/novadata_model.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/novadata_utils/redirect/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       87 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/redirect/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1130 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/redirect/reverse_lazy_plus.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/novadata_utils/save/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      130 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/save/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1749 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/save/create_logs.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     2152 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/save/get_changes.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/novadata_utils/serializers/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      107 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/serializers/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      880 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/serializers/novadata_model_serializer.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/novadata_utils/signals/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/signals/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/novadata_utils/templatetags/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/templatetags/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/novadata_utils/tests/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/tests/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       58 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/urls.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/novadata_utils/views/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/views/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/novadata_utils/viewsets/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       98 2023-04-04 12:57:52.000000 novadata_utils-0.2.3/novadata_utils/viewsets/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     4830 2023-04-04 13:09:11.000000 novadata_utils-0.2.3/novadata_utils/viewsets/novadata_model_viewset.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-10 15:15:45.377091 novadata_utils-0.2.3/novadata_utils.egg-info/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1019 2023-04-10 15:15:45.000000 novadata_utils-0.2.3/novadata_utils.egg-info/PKG-INFO
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1327 2023-04-10 15:15:45.000000 novadata_utils-0.2.3/novadata_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        1 2023-04-10 15:15:45.000000 novadata_utils-0.2.3/novadata_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      123 2023-04-10 15:15:45.000000 novadata_utils-0.2.3/novadata_utils.egg-info/requires.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       15 2023-04-10 15:15:45.000000 novadata_utils-0.2.3/novadata_utils.egg-info/top_level.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       38 2023-04-10 15:15:45.381091 novadata_utils-0.2.3/setup.cfg
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      878 2023-04-10 15:15:18.000000 novadata_utils-0.2.3/setup.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1066 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/LICENSE
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1018 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/PKG-INFO
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      573 2023-04-16 16:52:43.000000 novadata_utils-0.2.4/README.md
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.994428 novadata_utils-0.2.4/novadata_utils/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       60 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.994428 novadata_utils-0.2.4/novadata_utils/admin/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/admin/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     4353 2023-04-10 14:26:47.000000 novadata_utils-0.2.4/novadata_utils/admin/novadata_model_admin.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      219 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/apps.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.994428 novadata_utils-0.2.4/novadata_utils/auth/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/auth/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      729 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/auth/login_username_email.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.994428 novadata_utils-0.2.4/novadata_utils/forms/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/forms/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.994428 novadata_utils-0.2.4/novadata_utils/functions/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      177 2023-04-16 18:28:57.000000 novadata_utils-0.2.4/novadata_utils/functions/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     2186 2023-04-16 18:28:38.000000 novadata_utils-0.2.4/novadata_utils/functions/get_prop.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     2979 2023-04-16 18:28:07.000000 novadata_utils-0.2.4/novadata_utils/functions/props_dict.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      416 2023-04-10 14:19:49.000000 novadata_utils-0.2.4/novadata_utils/functions/transform_field.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/managers/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/managers/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/middlewares/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/middlewares/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/migrations/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1232 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/migrations/0001_initial.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/migrations/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/models/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       76 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/models/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1188 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/models/novadata_model.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/redirect/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       87 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/redirect/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1130 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/redirect/reverse_lazy_plus.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/save/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      130 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/save/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1749 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/save/create_logs.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     2152 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/save/get_changes.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/serializers/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      107 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/serializers/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1934 2023-04-16 16:54:07.000000 novadata_utils-0.2.4/novadata_utils/serializers/novadata_model_serializer.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/signals/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/signals/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/templatetags/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/templatetags/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/tests/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/tests/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       58 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/urls.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/views/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/views/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/viewsets/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       98 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/viewsets/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     5457 2023-04-16 18:25:27.000000 novadata_utils-0.2.4/novadata_utils/viewsets/novadata_model_viewset.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.994428 novadata_utils-0.2.4/novadata_utils.egg-info/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1018 2023-04-20 10:40:53.000000 novadata_utils-0.2.4/novadata_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1366 2023-04-20 10:40:53.000000 novadata_utils-0.2.4/novadata_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        1 2023-04-20 10:40:53.000000 novadata_utils-0.2.4/novadata_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      123 2023-04-20 10:40:53.000000 novadata_utils-0.2.4/novadata_utils.egg-info/requires.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       15 2023-04-20 10:40:53.000000 novadata_utils-0.2.4/novadata_utils.egg-info/top_level.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       38 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/setup.cfg
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      878 2023-04-20 10:40:48.000000 novadata_utils-0.2.4/setup.py
```

### Comparing `novadata_utils-0.2.3/LICENSE` & `novadata_utils-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.3/PKG-INFO` & `novadata_utils-0.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novadata_utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: novadata utils
 Home-page: https://github.com/TimeNovaData/novadata_utils/
 Author: Flávio Silva
 Author-email: flavio.nogueira.profissional@gmail.com
 License: MIT License
 Project-URL: GitHub, https://github.com/TimeNovaData/novadata_utils/
 Keywords: Django,utils,ndt,novadata,nova data,nova,data
@@ -26,15 +26,15 @@
 pip install novadata-utils
 ```
 
 Settings.py:
 ```python
 INSTALLED_APPS = [
     ...
-    'django-admin-list-filter-dropdown',
+    'django_admin_listfilter_dropdown',
     'django_object_actions',
     'import_export',
     'novadata_utils',
     'rest_framework',
     ...
 ]
```

### Comparing `novadata_utils-0.2.3/README.md` & `novadata_utils-0.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 pip install novadata-utils
 ```
 
 Settings.py:
 ```python
 INSTALLED_APPS = [
     ...
-    'django-admin-list-filter-dropdown',
+    'django_admin_listfilter_dropdown',
     'django_object_actions',
     'import_export',
     'novadata_utils',
     'rest_framework',
     ...
 ]
```

### Comparing `novadata_utils-0.2.3/novadata_utils/admin/novadata_model_admin.py` & `novadata_utils-0.2.4/novadata_utils/admin/novadata_model_admin.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.3/novadata_utils/auth/login_username_email.py` & `novadata_utils-0.2.4/novadata_utils/auth/login_username_email.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.3/novadata_utils/migrations/0001_initial.py` & `novadata_utils-0.2.4/novadata_utils/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.3/novadata_utils/models/novadata_model.py` & `novadata_utils-0.2.4/novadata_utils/models/novadata_model.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.3/novadata_utils/redirect/reverse_lazy_plus.py` & `novadata_utils-0.2.4/novadata_utils/redirect/reverse_lazy_plus.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.3/novadata_utils/save/create_logs.py` & `novadata_utils-0.2.4/novadata_utils/save/create_logs.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.3/novadata_utils/save/get_changes.py` & `novadata_utils-0.2.4/novadata_utils/save/get_changes.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.3/novadata_utils/viewsets/novadata_model_viewset.py` & `novadata_utils-0.2.4/novadata_utils/viewsets/novadata_model_viewset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django_filters.rest_framework import DjangoFilterBackend
 from rest_framework import filters, status, viewsets
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 
-from novadata_utils.functions import get_prop
+from novadata_utils.functions import get_prop, props_dict
 
 
 class NovadataModelViewSet(viewsets.ModelViewSet):
     permission_classes = [
         IsAuthenticated,
     ]
 
@@ -19,53 +19,68 @@
 
     filterset_fields: list = None
 
     ordering_fields: list = None
 
     search_fields: list = None
 
-    auto_search_fields: bool = False
+    auto_search_fields: bool = True
 
     relation_fields = [
         "OneToOneField",
         "ForeignKey",
     ]
 
     def get_filterset_fields(self):
         """Retorna os campos de filtro."""
         model = self.serializer_class().Meta.model
-        self.filterset_fields = get_prop(
+        list_filterset_fields = get_prop(
             model,
             "filterset_fields",
-            str=False,
+            annotate_type=True,
         )
 
-        return self.filterset_fields
+        dict_filterset_fields = {}
+        for filterset_field in list_filterset_fields:
+            name = filterset_field["name"]
+            type = filterset_field["type"]
+
+            sub_props = props_dict.get(type, [])
+            dict_filterset_fields[name] = sub_props
+
+        return dict_filterset_fields
 
     def get_ordering_fields(self):
         """Retorna os campos de ordenação."""
         model = self.serializer_class().Meta.model
-        self.ordering_fields = get_prop(
+        ordering_fields = get_prop(
             model,
             "ordering_fields",
-            str=False,
         )
 
-        return self.ordering_fields
+        return ordering_fields
 
     def get_search_fields(self):
         """Retorna os campos de busca."""
         model = self.serializer_class().Meta.model
-        self.search_fields = get_prop(
+        list_search_fields = get_prop(
             model,
             "search_fields",
-            str=False,
+            annotate_type=True,
         )
 
-        return self.search_fields
+        dict_search_fields = {}
+        for search_field in list_search_fields:
+            name = search_field["name"]
+            type = search_field["type"]
+
+            sub_props = props_dict.get(type, [])
+            dict_search_fields[name] = sub_props
+
+        return dict_search_fields
 
     def get_fk_fields(self):
         """Retorna os campos de relacionamento."""
         model = self.serializer_class().Meta.model
         fields = model._meta.get_fields()
         fk_fields = [
             (field.name, field.remote_field.model)
@@ -94,15 +109,17 @@
     def create(self, request, *args, **kwargs):
         """Realiza o create de um objeto."""
         serializer = self.get_serializer(data=self.get_data(request))
         serializer.is_valid(raise_exception=True)
         self.perform_create(serializer)
         headers = self.get_success_headers(serializer.data)
         return Response(
-            serializer.data, status=status.HTTP_201_CREATED, headers=headers
+            serializer.data,
+            status=status.HTTP_201_CREATED,
+            headers=headers,
         )
 
     def update(self, request, *args, **kwargs):
         """Realiza o update de um objeto."""
         partial = kwargs.pop("partial", False)
         instance = self.get_object()
         data = self.get_data(request)
@@ -147,14 +164,14 @@
 
         return Response(serializer.data)
 
     def __init__(self, **kwargs) -> None:
         """Método para executarmos ações ao iniciar a classe."""
         super().__init__(**kwargs)
         if not self.filterset_fields:
-            self.get_filterset_fields()
+            self.filterset_fields = self.get_filterset_fields()
 
         if not self.ordering_fields:
-            self.get_ordering_fields()
+            self.ordering_fields = self.get_ordering_fields()
 
         if self.auto_search_fields and not self.search_fields:
-            self.get_search_fields()
+            self.search_fields = self.get_search_fields()
```

### Comparing `novadata_utils-0.2.3/novadata_utils.egg-info/PKG-INFO` & `novadata_utils-0.2.4/novadata_utils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novadata-utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: novadata utils
 Home-page: https://github.com/TimeNovaData/novadata_utils/
 Author: Flávio Silva
 Author-email: flavio.nogueira.profissional@gmail.com
 License: MIT License
 Project-URL: GitHub, https://github.com/TimeNovaData/novadata_utils/
 Keywords: Django,utils,ndt,novadata,nova data,nova,data
@@ -26,15 +26,15 @@
 pip install novadata-utils
 ```
 
 Settings.py:
 ```python
 INSTALLED_APPS = [
     ...
-    'django-admin-list-filter-dropdown',
+    'django_admin_listfilter_dropdown',
     'django_object_actions',
     'import_export',
     'novadata_utils',
     'rest_framework',
     ...
 ]
```

### Comparing `novadata_utils-0.2.3/novadata_utils.egg-info/SOURCES.txt` & `novadata_utils-0.2.4/novadata_utils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 novadata_utils/admin/__init__.py
 novadata_utils/admin/novadata_model_admin.py
 novadata_utils/auth/__init__.py
 novadata_utils/auth/login_username_email.py
 novadata_utils/forms/__init__.py
 novadata_utils/functions/__init__.py
 novadata_utils/functions/get_prop.py
+novadata_utils/functions/props_dict.py
 novadata_utils/functions/transform_field.py
 novadata_utils/managers/__init__.py
 novadata_utils/middlewares/__init__.py
 novadata_utils/migrations/0001_initial.py
 novadata_utils/migrations/__init__.py
 novadata_utils/models/__init__.py
 novadata_utils/models/novadata_model.py
```

### Comparing `novadata_utils-0.2.3/setup.py` & `novadata_utils-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     readme = fh.read()
 
 setup(
     name="novadata_utils",
-    version="0.2.3",
+    version="0.2.4",
     url="https://github.com/TimeNovaData/novadata_utils/",
     license="MIT License",
     author="Flávio Silva",
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email="flavio.nogueira.profissional@gmail.com",
     keywords="Django, utils, ndt, novadata, nova data, nova, data",
```

