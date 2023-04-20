# Comparing `tmp/django_breeze-0.1.5.tar.gz` & `tmp/django_breeze-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_breeze-0.1.5.tar", max compression
+gzip compressed data, was "django_breeze-0.1.6.tar", max compression
```

## Comparing `django_breeze-0.1.5.tar` & `django_breeze-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,42 @@
--rwxr-xr-x   0        0        0        0 2023-04-16 21:20:58.715528 django_breeze-0.1.5/LICENSE.md
--rwxr-xr-x   0        0        0     3055 2023-04-18 19:06:55.231382 django_breeze-0.1.5/README.md
--rwxr-xr-x   0        0        0       61 2023-04-18 13:00:06.368911 django_breeze-0.1.5/django_breeze/__init__.py
--rwxr-xr-x   0        0        0      222 2023-04-18 11:37:34.673551 django_breeze-0.1.5/django_breeze/__main__.py
--rwxr-xr-x   0        0        0      246 2023-04-18 13:00:26.296628 django_breeze-0.1.5/django_breeze/apps.py
--rwxr-xr-x   0        0        0        0 2023-04-17 12:29:24.898719 django_breeze-0.1.5/django_breeze/core/__init__.py
--rwxr-xr-x   0        0        0     4100 2023-04-18 15:20:17.808443 django_breeze-0.1.5/django_breeze/core/management/__init__.py
--rwxr-xr-x   0        0        0      719 2023-04-17 12:34:24.726621 django_breeze-0.1.5/django_breeze/middleware.py
--rwxr-xr-x   0        0        0      232 2023-04-18 13:30:15.928013 django_breeze-0.1.5/django_breeze/scripts/django_breeze.py
--rwxr-xr-x   0        0        0     2673 2023-04-18 17:54:24.394097 django_breeze-0.1.5/django_breeze/settings.py
--rwxr-xr-x   0        0        0      322 2023-04-17 16:02:16.221609 django_breeze-0.1.5/django_breeze/templates/react/.gitignore
--rwxr-xr-x   0        0        0      561 2023-04-17 15:38:34.137680 django_breeze-0.1.5/django_breeze/templates/react/package.json
--rwxr-xr-x   0        0        0       80 2023-04-11 16:36:16.193044 django_breeze-0.1.5/django_breeze/templates/react/postcss.config.js
--rwxr-xr-x   0        0        0      115 2023-04-17 15:55:52.679212 django_breeze-0.1.5/django_breeze/templates/react/src/Layout/SiteLayout.jsx
--rwxr-xr-x   0        0        0     4126 2023-04-11 12:18:56.391967 django_breeze-0.1.5/django_breeze/templates/react/src/assets/react.svg
--rwxr-xr-x   0        0        0       58 2023-04-17 15:26:59.812312 django_breeze-0.1.5/django_breeze/templates/react/src/index.css
--rwxr-xr-x   0        0        0      416 2023-04-17 15:48:56.251208 django_breeze-0.1.5/django_breeze/templates/react/src/index.html
--rwxr-xr-x   0        0        0      544 2023-04-17 15:28:13.267633 django_breeze-0.1.5/django_breeze/templates/react/src/main.jsx
--rwxr-xr-x   0        0        0      143 2023-04-17 15:42:26.503686 django_breeze-0.1.5/django_breeze/templates/react/src/pages/index.jsx
--rwxr-xr-x   0        0        0      174 2023-04-11 16:37:38.133133 django_breeze-0.1.5/django_breeze/templates/react/tailwind.config.js
--rwxr-xr-x   0        0        0      814 2023-04-16 23:40:08.446285 django_breeze-0.1.5/django_breeze/templates/react/vite.config.js
--rwxr-xr-x   0        0        0      322 2023-04-17 16:02:19.154142 django_breeze-0.1.5/django_breeze/templates/react_typescript/.gitignore
--rwxr-xr-x   0        0        0      577 2023-04-17 15:47:44.921698 django_breeze-0.1.5/django_breeze/templates/react_typescript/package.json
--rwxr-xr-x   0        0        0       80 2023-04-11 16:36:16.193044 django_breeze-0.1.5/django_breeze/templates/react_typescript/postcss.config.js
--rwxr-xr-x   0        0        0     1497 2023-04-17 15:44:03.080989 django_breeze-0.1.5/django_breeze/templates/react_typescript/public/vite.svg
--rwxr-xr-x   0        0        0      115 2023-04-17 15:55:31.215573 django_breeze-0.1.5/django_breeze/templates/react_typescript/src/Layout/SiteLayout.tsx
--rwxr-xr-x   0        0        0     4126 2023-04-17 15:44:03.128485 django_breeze-0.1.5/django_breeze/templates/react_typescript/src/assets/react.svg
--rwxr-xr-x   0        0        0       59 2023-04-17 15:51:58.938773 django_breeze-0.1.5/django_breeze/templates/react_typescript/src/index.css
--rwxr-xr-x   0        0        0      417 2023-04-17 15:49:05.983645 django_breeze-0.1.5/django_breeze/templates/react_typescript/src/index.html
--rwxr-xr-x   0        0        0      544 2023-04-17 15:56:37.832534 django_breeze-0.1.5/django_breeze/templates/react_typescript/src/main.tsx
--rwxr-xr-x   0        0        0      143 2023-04-17 15:53:30.284520 django_breeze-0.1.5/django_breeze/templates/react_typescript/src/pages/index.tsx
--rwxr-xr-x   0        0        0       38 2023-04-17 15:44:03.129843 django_breeze-0.1.5/django_breeze/templates/react_typescript/src/vite-env.d.ts
--rwxr-xr-x   0        0        0      174 2023-04-11 16:37:38.133133 django_breeze-0.1.5/django_breeze/templates/react_typescript/tailwind.config.js
--rwxr-xr-x   0        0        0      559 2023-04-17 15:44:03.150638 django_breeze-0.1.5/django_breeze/templates/react_typescript/tsconfig.json
--rwxr-xr-x   0        0        0      184 2023-04-17 15:44:03.151143 django_breeze-0.1.5/django_breeze/templates/react_typescript/tsconfig.node.json
--rwxr-xr-x   0        0        0      814 2023-04-17 15:57:23.467510 django_breeze-0.1.5/django_breeze/templates/react_typescript/vite.config.ts
--rwxr-xr-x   0        0        0      763 2023-04-18 19:09:22.634034 django_breeze-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3848 1970-01-01 00:00:00.000000 django_breeze-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-20 12:19:20.337512 django_breeze-0.1.6/LICENSE.md
+-rw-r--r--   0        0        0     3434 2023-04-20 12:19:20.337512 django_breeze-0.1.6/README.md
+-rw-r--r--   0        0        0       61 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/__init__.py
+-rw-r--r--   0        0        0      222 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/__main__.py
+-rw-r--r--   0        0        0      814 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/apps.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/core/__init__.py
+-rw-r--r--   0        0        0     4100 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/core/management/__init__.py
+-rw-r--r--   0        0        0      719 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/middleware.py
+-rw-r--r--   0        0        0      232 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/scripts/django_breeze.py
+-rw-r--r--   0        0        0     3057 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/settings.py
+-rw-r--r--   0        0        0   129342 2023-04-20 12:19:20.337512 django_breeze-0.1.6/django_breeze/static/django_breeze/django-breeze-logo.jpg
+-rw-r--r--   0        0        0   211529 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/static/django_breeze/django-breeze-logo.png
+-rw-r--r--   0        0        0      322 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/.gitignore
+-rw-r--r--   0        0        0      561 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/package.json
+-rw-r--r--   0        0        0       80 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/postcss.config.js
+-rw-r--r--   0        0        0      115 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/src/Layout/SiteLayout.jsx
+-rw-r--r--   0        0        0     4126 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/src/assets/react.svg
+-rw-r--r--   0        0        0       58 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/src/index.css
+-rw-r--r--   0        0        0      416 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/src/index.html
+-rw-r--r--   0        0        0      544 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/src/main.jsx
+-rw-r--r--   0        0        0      983 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/src/pages/index.jsx
+-rw-r--r--   0        0        0      174 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/tailwind.config.js
+-rw-r--r--   0        0        0      814 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react/vite.config.js
+-rw-r--r--   0        0        0      322 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/.gitignore
+-rw-r--r--   0        0        0      577 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/package.json
+-rw-r--r--   0        0        0       80 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/postcss.config.js
+-rw-r--r--   0        0        0     1497 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/public/vite.svg
+-rw-r--r--   0        0        0      115 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/src/Layout/SiteLayout.tsx
+-rw-r--r--   0        0        0     4126 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/src/assets/react.svg
+-rw-r--r--   0        0        0       59 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/src/index.css
+-rw-r--r--   0        0        0      417 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/src/index.html
+-rw-r--r--   0        0        0      544 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/src/main.tsx
+-rw-r--r--   0        0        0     1024 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/src/pages/index.tsx
+-rw-r--r--   0        0        0       38 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/src/vite-env.d.ts
+-rw-r--r--   0        0        0      174 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/tailwind.config.js
+-rw-r--r--   0        0        0      559 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/tsconfig.json
+-rw-r--r--   0        0        0      184 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/tsconfig.node.json
+-rw-r--r--   0        0        0      814 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/templates/react_typescript/vite.config.ts
+-rw-r--r--   0        0        0      130 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/urls.py
+-rw-r--r--   0        0        0      354 2023-04-20 12:19:20.341512 django_breeze-0.1.6/django_breeze/views.py
+-rw-r--r--   0        0        0      804 2023-04-20 12:19:20.341512 django_breeze-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4267 1970-01-01 00:00:00.000000 django_breeze-0.1.6/PKG-INFO
```

### Comparing `django_breeze-0.1.5/README.md` & `django_breeze-0.1.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+![image](/django_breeze/static/django_breeze/django-breeze-logo.jpg)
+
 # Django Breeze
 
 ## Introduction
 
-Django Breeze provides a minimal and simple starting point for building a Django application with `Inertia` and `Vite` with minimal or no configuration. Styled with Tailwind CSS.
+Django Breeze provides a minimal and simple starting point for building a Django application with `Inertia` and `Vite.js` with minimal or no configuration. Styled with Tailwind CSS.
 
 Inertia helps build single-page apps, without building an API. Create modern single-page React, Vue, and Svelte apps using classic server-side routing. Works with any backend. Documentation for Inertia can be found on the [Intertia website](https://inertiajs.com/).
 
 ## Installation
 
 Install the following python package via pip
 
@@ -40,20 +42,28 @@
 
 Generate your frontend project files with django-breeze
 
 ### React
 
 ```bash
 django-breeze react
+
+# or with typescript
+
+django-breeze react --typescript
 ```
 
 ### Vue 3
 
 ```bash
 django-breeze vue3
+
+# or with typescript
+
+django-breeze vue3 --typescript
 ```
 
 ## Install node packages
 
 Run this command to install packages for the frontend.
 
 ```zsh
@@ -78,14 +88,18 @@
 
 ```bash
 python manage.py runserver
 ```
 
 Now you're all set!
 
+## Usage
+
+For usage, refer to [inertia-django](https://github.com/inertiajs/inertia-django#usage) for in-depth guidlines.
+
 ## Configurations
 
 Although, djang breeze comes with minimal or no configurations but here are some of the default settings it comes with out of the box.
 
 ### Django Settings
 
 ```python
@@ -94,25 +108,26 @@
  DJANGO_BREEZE = {
         "INERTIA": {
             "LAYOUT": "index.html",
             "SSR_URL": "http://localhost:13714",
             "SSR_ENABLED": False,
         },
         "DJANGO_VITE": {
-            "DEV_MODE": True,
+            "DEV_MODE": True, # vite dev mode, default based on django DEBUG
             "SERVER_PROTOCOL": "http",
             "DEV_SERVER_HOST": "localhost",
             "DEV_SERVER_PORT": 5173,
             "WS_CLIENT_URL": "@vite/client",
-            "ASSETS_PATH": "static/dist",
+            "ASSETS_PATH": "static/dist", # vite build asset path
             "STATIC_URL_PREFIX": "",
         }
 ```
 
 Settings for [Inertia Django](https://github.com/inertiajs/inertia-django) is under `INERTIA` and [Django Vite](https://github.com/MrBin99/django-vite) is `DJANGO_VITE`. You can find more explaination of the settings on their repos
+
 `Note:` All settings are joined with underscore to match how their developers defined them e.g inertia settings is `INERTIA_LAYOUT` and django vite is `DJANGO_VITE_DEV_MODE` which has been done automatically by django breeze so you just use the `DJANGO_BREEZE` settings format in your `settings.py` file.
 
 ## Thank you
 
 A very big thanks to [Inertia.js Team](https://github.com/inertiajs) for [Inertia Django Adaptor](https://github.com/inertiajs/inertia-django), and [MrBin99](https://github.com/MrBin99) for [Django Vite](https://github.com/MrBin99/django-vite).
 
 ## License
```

### Comparing `django_breeze-0.1.5/django_breeze/core/management/__init__.py` & `django_breeze-0.1.6/django_breeze/core/management/__init__.py`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.5/django_breeze/middleware.py` & `django_breeze-0.1.6/django_breeze/middleware.py`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.5/django_breeze/settings.py` & `django_breeze-0.1.6/django_breeze/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     MIDDLEWARES = [
         "inertia.middleware.InertiaMiddleware",
         # "django-breeze.django_breeze.middleware.inertia_share",
     ]
 
     # Django Breeze Default Settings
     DJANGO_BREEZE: dict = {
+        "TEMPLATE_DIR_PATH": Path(BASE_DIR) / "src/",  # path to frontend files
         "INERTIA": {
             "LAYOUT": "index.html",
             "SSR_URL": inertia_settings.INERTIA_SSR_URL,
             "SSR_ENABLED": inertia_settings.INERTIA_SSR_ENABLED,
             "JSON_ENCODER": inertia_settings.INERTIA_JSON_ENCODER,
         },
         "DJANGO_VITE": {
@@ -32,15 +33,15 @@
             "LEGACY_POLYFILLS_MOTIF": "legacy-polyfills",
         },
         "STATIC_ROOT": "static",
         "CSRF_HEADER_NAME": "HTTP_X_XSRF_TOKEN",
         "CSRF_COOKIE_NAME": "XSRF-TOKEN",
     }
 
-    # Merge DJANGO_BREEZE and user-defined settings
+    # Get user defined django breeze settings
     user_settings = getattr(django_settings, "DJANGO_BREEZE", {})
 
     def merge_dicts(*dicts):
         """
         Recursively merges dictionaries.
         """
         result = {}
@@ -48,14 +49,15 @@
             for k, v in d.items():
                 if isinstance(v, dict):
                     result[k] = merge_dicts(result.get(k, {}), v)
                 else:
                     result[k] = v
         return result
 
+    # Merge DJANGO_BREEZE and user-defined settings
     merged_settings = merge_dicts(DJANGO_BREEZE, user_settings)
 
     def key_exist(key) -> bool:
         return (
             hasattr(django_settings, key) and getattr(django_settings, key) is not None
         )
 
@@ -70,11 +72,19 @@
         else:
             if not key_exist(key):
                 settings[key] = value
 
     for key, value in settings.items():
         setattr(django_settings, key, value)
 
-    django_settings.TEMPLATES[0]["DIRS"].append(Path(BASE_DIR) / "src/")
+    TEMPLATE_DIR = Path(getattr(django_settings, "TEMPLATE_DIR_PATH"))
 
+    django_settings.TEMPLATES[0]["DIRS"].append(TEMPLATE_DIR)
+    django_settings.STATICFILES_DIRS.extend(
+        [
+            django_settings.DJANGO_VITE_ASSETS_PATH,
+            TEMPLATE_DIR / "assets",
+            TEMPLATE_DIR / "public",
+        ]
+    )
     for middleware in MIDDLEWARES:
         django_settings.MIDDLEWARE.append(middleware)
```

### Comparing `django_breeze-0.1.5/django_breeze/templates/react/package.json` & `django_breeze-0.1.6/django_breeze/templates/react/package.json`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.5/django_breeze/templates/react/src/assets/react.svg` & `django_breeze-0.1.6/django_breeze/templates/react/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.5/django_breeze/templates/react/src/main.jsx` & `django_breeze-0.1.6/django_breeze/templates/react/src/main.jsx`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.5/django_breeze/templates/react/vite.config.js` & `django_breeze-0.1.6/django_breeze/templates/react/vite.config.js`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.5/django_breeze/templates/react_typescript/package.json` & `django_breeze-0.1.6/django_breeze/templates/react_typescript/package.json`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.5/django_breeze/templates/react_typescript/public/vite.svg` & `django_breeze-0.1.6/django_breeze/templates/react_typescript/public/vite.svg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.5/django_breeze/templates/react_typescript/src/assets/react.svg` & `django_breeze-0.1.6/django_breeze/templates/react_typescript/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.5/django_breeze/templates/react_typescript/src/main.tsx` & `django_breeze-0.1.6/django_breeze/templates/react_typescript/src/main.tsx`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.5/django_breeze/templates/react_typescript/tsconfig.json` & `django_breeze-0.1.6/django_breeze/templates/react_typescript/tsconfig.json`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.5/django_breeze/templates/react_typescript/vite.config.ts` & `django_breeze-0.1.6/django_breeze/templates/react_typescript/vite.config.ts`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.5/pyproject.toml` & `django_breeze-0.1.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "django-breeze"
-version = "0.1.5"
-description = "Django Breeze provides a minimal and simple starting point for building a Django application with Inertia.js Styled with Tailwind CSS."
+version =  "0.1.6"
+description = "Django Breeze provides a minimal and simple starting point for building a Django application with Inertia and Vite with minimal or no configuration. Styled with Tailwind CSS."
 keywords = ["react", "django", "vue", "inertia", "vite"]
 authors = ["louxsdon <louisayivi.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Louxsdon/django-breeze"
 packages = [{include = "django_breeze"}]
```

### Comparing `django_breeze-0.1.5/PKG-INFO` & `django_breeze-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-breeze
-Version: 0.1.5
-Summary: Django Breeze provides a minimal and simple starting point for building a Django application with Inertia.js Styled with Tailwind CSS.
+Version: 0.1.6
+Summary: Django Breeze provides a minimal and simple starting point for building a Django application with Inertia and Vite with minimal or no configuration. Styled with Tailwind CSS.
 Home-page: https://github.com/Louxsdon/django-breeze
 License: MIT
 Keywords: react,django,vue,inertia,vite
 Author: louxsdon
 Author-email: louisayivi.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,19 +13,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django-vite (>=2.0.2,<3.0.0)
 Requires-Dist: inertia-django (>=0.5.2,<0.6.0)
 Project-URL: Repository, https://github.com/Louxsdon/django-breeze
 Description-Content-Type: text/markdown
 
+![image](/django_breeze/static/django_breeze/django-breeze-logo.jpg)
+
 # Django Breeze
 
 ## Introduction
 
-Django Breeze provides a minimal and simple starting point for building a Django application with `Inertia` and `Vite` with minimal or no configuration. Styled with Tailwind CSS.
+Django Breeze provides a minimal and simple starting point for building a Django application with `Inertia` and `Vite.js` with minimal or no configuration. Styled with Tailwind CSS.
 
 Inertia helps build single-page apps, without building an API. Create modern single-page React, Vue, and Svelte apps using classic server-side routing. Works with any backend. Documentation for Inertia can be found on the [Intertia website](https://inertiajs.com/).
 
 ## Installation
 
 Install the following python package via pip
 
@@ -59,20 +61,28 @@
 
 Generate your frontend project files with django-breeze
 
 ### React
 
 ```bash
 django-breeze react
+
+# or with typescript
+
+django-breeze react --typescript
 ```
 
 ### Vue 3
 
 ```bash
 django-breeze vue3
+
+# or with typescript
+
+django-breeze vue3 --typescript
 ```
 
 ## Install node packages
 
 Run this command to install packages for the frontend.
 
 ```zsh
@@ -97,14 +107,18 @@
 
 ```bash
 python manage.py runserver
 ```
 
 Now you're all set!
 
+## Usage
+
+For usage, refer to [inertia-django](https://github.com/inertiajs/inertia-django#usage) for in-depth guidlines.
+
 ## Configurations
 
 Although, djang breeze comes with minimal or no configurations but here are some of the default settings it comes with out of the box.
 
 ### Django Settings
 
 ```python
@@ -113,25 +127,26 @@
  DJANGO_BREEZE = {
         "INERTIA": {
             "LAYOUT": "index.html",
             "SSR_URL": "http://localhost:13714",
             "SSR_ENABLED": False,
         },
         "DJANGO_VITE": {
-            "DEV_MODE": True,
+            "DEV_MODE": True, # vite dev mode, default based on django DEBUG
             "SERVER_PROTOCOL": "http",
             "DEV_SERVER_HOST": "localhost",
             "DEV_SERVER_PORT": 5173,
             "WS_CLIENT_URL": "@vite/client",
-            "ASSETS_PATH": "static/dist",
+            "ASSETS_PATH": "static/dist", # vite build asset path
             "STATIC_URL_PREFIX": "",
         }
 ```
 
 Settings for [Inertia Django](https://github.com/inertiajs/inertia-django) is under `INERTIA` and [Django Vite](https://github.com/MrBin99/django-vite) is `DJANGO_VITE`. You can find more explaination of the settings on their repos
+
 `Note:` All settings are joined with underscore to match how their developers defined them e.g inertia settings is `INERTIA_LAYOUT` and django vite is `DJANGO_VITE_DEV_MODE` which has been done automatically by django breeze so you just use the `DJANGO_BREEZE` settings format in your `settings.py` file.
 
 ## Thank you
 
 A very big thanks to [Inertia.js Team](https://github.com/inertiajs) for [Inertia Django Adaptor](https://github.com/inertiajs/inertia-django), and [MrBin99](https://github.com/MrBin99) for [Django Vite](https://github.com/MrBin99/django-vite).
 
 ## License
```

