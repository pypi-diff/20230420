# Comparing `tmp/flet-0.6.0.dev1322.tar.gz` & `tmp/flet-0.6.0.dev1336.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-0.6.0.dev1322.tar", max compression
+gzip compressed data, was "flet-0.6.0.dev1336.tar", max compression
```

## Comparing `flet-0.6.0.dev1322.tar` & `flet-0.6.0.dev1336.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     2145 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/README.md
--rw-r--r--   0        0        0     1066 2023-04-17 18:18:47.509180 flet-0.6.0.dev1322/pyproject.toml
--rw-r--r--   0        0        0      155 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/__init__.py
--rw-r--r--   0        0        0       72 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/__pyinstaller/__init__.py
--rw-r--r--   0        0        0       20 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/__pyinstaller/config.py
--rw-r--r--   0        0        0      378 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/__pyinstaller/hook-flet.py
--rw-r--r--   0        0        0     2985 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/__pyinstaller/macos_utils.py
--rw-r--r--   0        0        0      187 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
--rw-r--r--   0        0        0       61 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/__pyinstaller/rthooks.dat
--rw-r--r--   0        0        0      562 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/__pyinstaller/utils.py
--rw-r--r--   0        0        0     3636 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/__pyinstaller/win_utils.py
--rw-r--r--   0        0        0     6192 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/async_local_socket_connection.py
--rw-r--r--   0        0        0     7183 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/async_websocket_connection.py
--rw-r--r--   0        0        0     9083 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/auth/authorization.py
--rw-r--r--   0        0        0      128 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/auth/group.py
--rw-r--r--   0        0        0     1499 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/auth/oauth_provider.py
--rw-r--r--   0        0        0      847 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/auth/oauth_token.py
--rw-r--r--   0        0        0      735 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/auth/providers/auth0_oauth_provider.py
--rw-r--r--   0        0        0      840 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/auth/providers/azure_oauth_provider.py
--rw-r--r--   0        0        0     3669 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/auth/providers/github_oauth_provider.py
--rw-r--r--   0        0        0      799 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/auth/providers/google_oauth_provider.py
--rw-r--r--   0        0        0      182 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/auth/user.py
--rw-r--r--   0        0        0     2958 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/cli/cli.py
--rw-r--r--   0        0        0     1953 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/cli/commands/base.py
--rw-r--r--   0        0        0      673 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/cli/commands/options.py
--rw-r--r--   0        0        0     8449 2023-04-17 18:18:07.065538 flet-0.6.0.dev1322/src/flet/cli/commands/pack.py
--rw-r--r--   0        0        0     8885 2023-04-17 18:18:07.069538 flet-0.6.0.dev1322/src/flet/cli/commands/publish.py
--rw-r--r--   0        0        0     6711 2023-04-17 18:18:07.069538 flet-0.6.0.dev1322/src/flet/cli/commands/run.py
--rw-r--r--   0        0        0       52 2023-04-17 18:18:07.069538 flet-0.6.0.dev1322/src/flet/constants.py
--rw-r--r--   0        0        0    21493 2023-04-17 18:18:07.069538 flet-0.6.0.dev1322/src/flet/flet.py
--rw-r--r--   0        0        0       55 2023-04-17 18:18:07.069538 flet-0.6.0.dev1322/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-04-17 18:18:07.069538 flet-0.6.0.dev1322/src/flet/plotly_chart.py
--rw-r--r--   0        0        0    10239 2023-04-17 18:18:07.069538 flet-0.6.0.dev1322/src/flet/pubsub.py
--rw-r--r--   0        0        0     3046 2023-04-17 18:18:07.069538 flet-0.6.0.dev1322/src/flet/reconnecting_websocket.py
--rw-r--r--   0        0        0     1272 2023-04-17 18:18:07.069538 flet-0.6.0.dev1322/src/flet/security.py
--rw-r--r--   0        0        0     6843 2023-04-17 18:18:07.069538 flet-0.6.0.dev1322/src/flet/sync_local_socket_connection.py
--rw-r--r--   0        0        0     5396 2023-04-17 18:18:07.069538 flet-0.6.0.dev1322/src/flet/sync_websocket_connection.py
--rw-r--r--   0        0        0     6955 2023-04-17 18:18:07.069538 flet-0.6.0.dev1322/src/flet/utils.py
--rw-r--r--   0        0        0     1431 2023-04-17 18:18:47.269181 flet-0.6.0.dev1322/src/flet/version.py
--rw-r--r--   0        0        0       32 2023-04-17 18:09:46.000000 flet-0.6.0.dev1322/src/flet/web/.last_build_id
--rw-r--r--   0        0        0      455 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/assets/AssetManifest.json
--rw-r--r--   0        0        0       82 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/assets/FontManifest.json
--rw-r--r--   0        0        0   916508 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/assets/NOTICES
--rw-r--r--   0        0        0  1645184 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/assets/fonts/MaterialIcons-Regular.otf
--rw-r--r--   0        0        0      298 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/assets/packages/window_manager/images/ic_chrome_close.png
--rw-r--r--   0        0        0      271 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/assets/packages/window_manager/images/ic_chrome_maximize.png
--rw-r--r--   0        0        0      166 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/assets/packages/window_manager/images/ic_chrome_minimize.png
--rw-r--r--   0        0        0      366 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/assets/packages/window_manager/images/ic_chrome_unmaximize.png
--rw-r--r--   0        0        0     1028 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/favicon.png
--rw-r--r--   0        0        0    13910 2023-04-17 18:08:29.000000 flet-0.6.0.dev1322/src/flet/web/flutter.js
--rw-r--r--   0        0        0     7836 2023-04-17 18:09:46.000000 flet-0.6.0.dev1322/src/flet/web/flutter_service_worker.js
--rw-r--r--   0        0        0     4699 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/icons/apple-touch-icon-192.png
--rw-r--r--   0        0        0     6622 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/icons/icon-192.png
--rw-r--r--   0        0        0    18666 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/icons/icon-512.png
--rw-r--r--   0        0        0     4128 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/icons/icon-maskable-192.png
--rw-r--r--   0        0        0    11906 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/icons/icon-maskable-512.png
--rw-r--r--   0        0        0    17040 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/icons/loading-animation.png
--rw-r--r--   0        0        0     2972 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/index.html
--rw-r--r--   0        0        0  5302372 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/main.dart.js
--rw-r--r--   0        0        0      789 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/manifest.json
--rw-r--r--   0        0        0     1573 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/python-worker.js
--rw-r--r--   0        0        0      744 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/python.js
--rw-r--r--   0        0        0       92 2023-04-17 18:09:45.000000 flet-0.6.0.dev1322/src/flet/web/version.json
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 flet-0.6.0.dev1322/PKG-INFO
+-rw-r--r--   0        0        0     2145 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/README.md
+-rw-r--r--   0        0        0     1066 2023-04-19 23:41:11.719771 flet-0.6.0.dev1336/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/__init__.py
+-rw-r--r--   0        0        0       72 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0       20 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/__pyinstaller/config.py
+-rw-r--r--   0        0        0      378 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/__pyinstaller/hook-flet.py
+-rw-r--r--   0        0        0     2985 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/__pyinstaller/macos_utils.py
+-rw-r--r--   0        0        0      187 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
+-rw-r--r--   0        0        0       61 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/__pyinstaller/rthooks.dat
+-rw-r--r--   0        0        0      562 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/__pyinstaller/utils.py
+-rw-r--r--   0        0        0     3620 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/__pyinstaller/win_utils.py
+-rw-r--r--   0        0        0     6194 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/async_local_socket_connection.py
+-rw-r--r--   0        0        0     7202 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/async_websocket_connection.py
+-rw-r--r--   0        0        0     9083 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/auth/authorization.py
+-rw-r--r--   0        0        0      128 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/auth/group.py
+-rw-r--r--   0        0        0     1499 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/auth/oauth_provider.py
+-rw-r--r--   0        0        0      847 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/auth/oauth_token.py
+-rw-r--r--   0        0        0      735 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/auth/providers/auth0_oauth_provider.py
+-rw-r--r--   0        0        0      840 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/auth/providers/azure_oauth_provider.py
+-rw-r--r--   0        0        0     3653 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/auth/providers/github_oauth_provider.py
+-rw-r--r--   0        0        0      799 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/auth/providers/google_oauth_provider.py
+-rw-r--r--   0        0        0      182 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/auth/user.py
+-rw-r--r--   0        0        0     2958 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/cli/cli.py
+-rw-r--r--   0        0        0     1953 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/cli/commands/base.py
+-rw-r--r--   0        0        0      673 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/cli/commands/options.py
+-rw-r--r--   0        0        0     8468 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/cli/commands/pack.py
+-rw-r--r--   0        0        0     8907 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/cli/commands/publish.py
+-rw-r--r--   0        0        0     6715 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/cli/commands/run.py
+-rw-r--r--   0        0        0       52 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/constants.py
+-rw-r--r--   0        0        0    21493 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0    10239 2023-04-19 23:40:35.342384 flet-0.6.0.dev1336/src/flet/pubsub.py
+-rw-r--r--   0        0        0     3049 2023-04-19 23:40:35.346384 flet-0.6.0.dev1336/src/flet/reconnecting_websocket.py
+-rw-r--r--   0        0        0     1272 2023-04-19 23:40:35.346384 flet-0.6.0.dev1336/src/flet/security.py
+-rw-r--r--   0        0        0     6819 2023-04-19 23:40:35.346384 flet-0.6.0.dev1336/src/flet/sync_local_socket_connection.py
+-rw-r--r--   0        0        0     5396 2023-04-19 23:40:35.346384 flet-0.6.0.dev1336/src/flet/sync_websocket_connection.py
+-rw-r--r--   0        0        0     6955 2023-04-19 23:40:35.346384 flet-0.6.0.dev1336/src/flet/utils.py
+-rw-r--r--   0        0        0     1431 2023-04-19 23:41:11.503776 flet-0.6.0.dev1336/src/flet/version.py
+-rw-r--r--   0        0        0       32 2023-04-19 23:32:47.000000 flet-0.6.0.dev1336/src/flet/web/.last_build_id
+-rw-r--r--   0        0        0      455 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/assets/AssetManifest.json
+-rw-r--r--   0        0        0       82 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/assets/FontManifest.json
+-rw-r--r--   0        0        0   916508 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/assets/NOTICES
+-rw-r--r--   0        0        0  1645184 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/assets/fonts/MaterialIcons-Regular.otf
+-rw-r--r--   0        0        0      298 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/assets/packages/window_manager/images/ic_chrome_close.png
+-rw-r--r--   0        0        0      271 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/assets/packages/window_manager/images/ic_chrome_maximize.png
+-rw-r--r--   0        0        0      166 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/assets/packages/window_manager/images/ic_chrome_minimize.png
+-rw-r--r--   0        0        0      366 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/assets/packages/window_manager/images/ic_chrome_unmaximize.png
+-rw-r--r--   0        0        0     1028 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/favicon.png
+-rw-r--r--   0        0        0    13910 2023-04-19 23:31:35.000000 flet-0.6.0.dev1336/src/flet/web/flutter.js
+-rw-r--r--   0        0        0     7836 2023-04-19 23:32:47.000000 flet-0.6.0.dev1336/src/flet/web/flutter_service_worker.js
+-rw-r--r--   0        0        0     4699 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/icons/apple-touch-icon-192.png
+-rw-r--r--   0        0        0     6622 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/icons/icon-192.png
+-rw-r--r--   0        0        0    18666 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/icons/icon-512.png
+-rw-r--r--   0        0        0     4128 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/icons/icon-maskable-192.png
+-rw-r--r--   0        0        0    11906 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/icons/icon-maskable-512.png
+-rw-r--r--   0        0        0    17040 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/icons/loading-animation.png
+-rw-r--r--   0        0        0     2972 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/index.html
+-rw-r--r--   0        0        0  5302372 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/main.dart.js
+-rw-r--r--   0        0        0      789 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/manifest.json
+-rw-r--r--   0        0        0     1573 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/python-worker.js
+-rw-r--r--   0        0        0      744 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/python.js
+-rw-r--r--   0        0        0       92 2023-04-19 23:32:46.000000 flet-0.6.0.dev1336/src/flet/web/version.json
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 flet-0.6.0.dev1336/PKG-INFO
```

### Comparing `flet-0.6.0.dev1322/README.md` & `flet-0.6.0.dev1336/README.md`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/pyproject.toml` & `flet-0.6.0.dev1336/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet"
-version = "0.6.0.dev1322"
+version = "0.6.0.dev1336"
 description = "Flet for Python - easily build interactive multi-platform apps in Python"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.6.0.dev1322"
+flet-core = "0.6.0.dev1336"
 python = "^3.7"
 typing-extensions = { version = "^4.4.0", python = "<3.8" }
 websocket-client = "^1.4.2"
 watchdog = "^2.2.1"
 oauthlib = "^3.2.2"
 websockets = "^10.4"
 httpx = "^0.23.3"
```

### Comparing `flet-0.6.0.dev1322/src/flet/__pyinstaller/macos_utils.py` & `flet-0.6.0.dev1336/src/flet/__pyinstaller/macos_utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/__pyinstaller/utils.py` & `flet-0.6.0.dev1336/src/flet/__pyinstaller/utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/__pyinstaller/win_utils.py` & `flet-0.6.0.dev1336/src/flet/__pyinstaller/win_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import tempfile
 import uuid
 from pathlib import Path
 
-import packaging.version as version
+from packaging import version
 import pefile
-import PyInstaller.utils.win32.versioninfo as versioninfo
+from PyInstaller.utils.win32 import versioninfo
 from PyInstaller.building.icon import normalize_icon_type
 from PyInstaller.compat import win32api
 from PyInstaller.utils.win32.icon import IconFile, normalize_icon_type
 
 
 def update_flet_view_icon(exe_path, icon_path):
     print("Updating Flet View icon", exe_path, icon_path)
```

### Comparing `flet-0.6.0.dev1322/src/flet/async_local_socket_connection.py` & `flet-0.6.0.dev1336/src/flet/async_local_socket_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             self.__receive_loop_task = asyncio.create_task(self.__receive_loop(reader))
             self.__send_loop_task = asyncio.create_task(self.__send_loop(writer))
 
     async def __receive_loop(self, reader: asyncio.StreamReader):
         while True:
             try:
                 raw_msglen = await reader.readexactly(4)
-            except:
+            except Exception:
                 return None
 
             if not raw_msglen:
                 return None
             msglen = struct.unpack(">I", raw_msglen)[0]
 
             data = await reader.readexactly(msglen)
@@ -89,16 +89,16 @@
         while True:
             message = await self.__send_queue.get()
             try:
                 data = message.encode("utf-8")
                 msg = struct.pack(">I", len(data)) + data
                 writer.write(msg)
                 # await writer.drain()
-                logger.debug("sent to TCP: {}".format(len(msg)))
-            except:
+                logger.debug(f"sent to TCP: {len(msg)}")
+            except Exception:
                 # re-enqueue the message to repeat it when re-connected
                 self.__send_queue.put_nowait(message)
                 raise
 
     async def __on_message(self, data: str):
         logger.debug(f"_on_message: {data}")
         msg_dict = json.loads(data)
@@ -124,15 +124,15 @@
         elif msg.action == ClientActions.UPDATE_CONTROL_PROPS:
             if self.__on_event is not None:
                 asyncio.create_task(
                     self.__on_event(self._create_update_control_props_handler_arg(msg))
                 )
         else:
             # it's something else
-            raise Exception('Unknown message "{}": {}'.format(msg.action, msg.payload))
+            raise Exception(f'Unknown message "{msg.action}": {msg.payload}')
 
     async def send_command_async(self, session_id: str, command: Command):
         result, message = self._process_command(command)
         if message:
             await self.__send(message)
         return PageCommandResponsePayload(result=result, error="")
```

### Comparing `flet-0.6.0.dev1322/src/flet/async_websocket_connection.py` & `flet-0.6.0.dev1336/src/flet/async_websocket_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                 logger.error(f"{name} threw {exception}")
                 failed = True
         for task in pending:
             task.cancel()
 
         # re-connect if one of tasks failed
         if failed:
-            logger.debug(f"Re-connecting to Flet server in 1 second")
+            logger.debug("Re-connecting to Flet server in 1 second")
             await asyncio.sleep(self.__CONNECT_TIMEOUT)
             await self.connect()
 
     async def __on_ws_message(self, data):
         logger.debug(f"_on_message: {data}")
         msg_dict = json.loads(data)
         msg = Message(**msg_dict)
@@ -144,15 +144,15 @@
             await self.__on_ws_message(message)
 
     async def __send_loop(self):
         while True:
             message = await self.__send_queue.get()
             try:
                 await self.__ws.send(message)
-            except:
+            except Exception:
                 # re-enqueue the message to repeat it when re-connected
                 self.__send_queue.put_nowait(message)
                 raise
 
     async def send_command_async(self, session_id: str, command: Command):
         assert self.page_name is not None
         payload = PageCommandRequestPayload(self.page_name, session_id, command)
@@ -191,9 +191,9 @@
         if self.__receive_loop_task:
             self.__receive_loop_task.cancel()
         if self.__send_loop_task:
             self.__send_loop_task.cancel()
         if self.__ws:
             try:
                 await self.__ws.close()
-            except:
+            except Exception:
                 pass  # do nothing
```

### Comparing `flet-0.6.0.dev1322/src/flet/auth/authorization.py` & `flet-0.6.0.dev1336/src/flet/auth/authorization.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,36 +113,36 @@
             "POST", self.provider.token_endpoint, content=data, headers=headers
         )
 
     def __fetch_user_and_groups(self):
         assert self.__token is not None
         if self.fetch_user:
             self.user = self.provider._fetch_user(self.__token.access_token)
-            if self.user == None and self.provider.user_endpoint != None:
-                if self.provider.user_id_fn == None:
+            if self.user is None and self.provider.user_endpoint is not None:
+                if self.provider.user_id_fn is None:
                     raise Exception(
                         "user_id_fn must be specified too if user_endpoint is not None"
                     )
                 self.user = self.__get_user()
-            if self.fetch_groups and self.user != None:
+            if self.fetch_groups and self.user is not None:
                 self.user.groups = self.provider._fetch_groups(
                     self.__token.access_token
                 )
 
     async def __fetch_user_and_groups_async(self):
         assert self.__token is not None
         if self.fetch_user:
             self.user = await self.provider._fetch_user_async(self.__token.access_token)
-            if self.user == None and self.provider.user_endpoint != None:
-                if self.provider.user_id_fn == None:
+            if self.user is None and self.provider.user_endpoint is not None:
+                if self.provider.user_id_fn is None:
                     raise Exception(
                         "user_id_fn must be specified too if user_endpoint is not None"
                     )
                 self.user = await self.__get_user_async()
-            if self.fetch_groups and self.user != None:
+            if self.fetch_groups and self.user is not None:
                 self.user.groups = await self.provider._fetch_groups_async(
                     self.__token.access_token
                 )
 
     def __convert_token(self, t: OAuth2Token):
         return OAuthToken(
             access_token=t["access_token"],
@@ -191,15 +191,15 @@
         )
 
     def __complete_refresh_token_request(self, refresh_resp):
         refresh_resp.raise_for_status()
         assert self.__token is not None
         client = WebApplicationClient(self.provider.client_id)
         t = client.parse_request_body_response(refresh_resp.text)
-        if t.get("refresh_token") == None:
+        if t.get("refresh_token") is None:
             t["refresh_token"] = self.__token.refresh_token
         self.__token = self.__convert_token(t)
 
     def __get_user(self):
         user_req = self.__get_user_request()
         with httpx.Client() as client:
             user_resp = client.send(user_req)
@@ -211,20 +211,20 @@
             user_resp = await client.send(user_req)
             return self.__complete_user_request(user_resp)
 
     def __get_user_request(self):
         assert self.token is not None
         assert self.provider.user_endpoint is not None
         headers = self.__get_default_headers()
-        headers["Authorization"] = "Bearer {}".format(self.token.access_token)
+        headers["Authorization"] = f"Bearer {self.token.access_token}"
         return httpx.Request("GET", self.provider.user_endpoint, headers=headers)
 
     def __complete_user_request(self, user_resp):
         user_resp.raise_for_status()
         assert self.provider.user_id_fn is not None
         uj = json.loads(user_resp.text)
         return User(uj, str(self.provider.user_id_fn(uj)))
 
     def __get_default_headers(self):
         return {
-            "User-Agent": "Flet/{}".format(version),
+            "User-Agent": f"Flet/{version}",
         }
```

### Comparing `flet-0.6.0.dev1322/src/flet/auth/oauth_provider.py` & `flet-0.6.0.dev1336/src/flet/auth/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/auth/oauth_token.py` & `flet-0.6.0.dev1336/src/flet/auth/oauth_token.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/auth/providers/auth0_oauth_provider.py` & `flet-0.6.0.dev1336/src/flet/auth/providers/auth0_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/auth/providers/azure_oauth_provider.py` & `flet-0.6.0.dev1336/src/flet/auth/providers/azure_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/auth/providers/github_oauth_provider.py` & `flet-0.6.0.dev1336/src/flet/auth/providers/github_oauth_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,10 +89,10 @@
             if e["primary"]:
                 uj["email"] = e["email"]
                 break
         return User(uj, id=str(uj["id"]))
 
     def __get_client_headers(self, access_token):
         return {
-            "Authorization": "Bearer {}".format(access_token),
-            "User-Agent": "Flet/{}".format(version),
+            "Authorization": f"Bearer {access_token}",
+            "User-Agent": f"Flet/{version}",
         }
```

### Comparing `flet-0.6.0.dev1322/src/flet/auth/providers/google_oauth_provider.py` & `flet-0.6.0.dev1336/src/flet/auth/providers/google_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/cli/cli.py` & `flet-0.6.0.dev1336/src/flet/cli/cli.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/cli/commands/base.py` & `flet-0.6.0.dev1336/src/flet/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/cli/commands/options.py` & `flet-0.6.0.dev1336/src/flet/cli/commands/options.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/cli/commands/pack.py` & `flet-0.6.0.dev1336/src/flet/cli/commands/pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import os
+import sys
 import shutil
 from pathlib import Path
 
 import flet.__pyinstaller.config as hook_config
 from flet.cli.commands.base import BaseCommand
 from flet.utils import is_macos, is_windows
 
@@ -122,15 +123,15 @@
                     for hidden_import_item in hidden_import_arr:
                         pyi_args.extend(["--hidden-import", hidden_import_item])
             if options.bundle_id:
                 pyi_args.extend(["--osx-bundle-identifier", options.bundle_id])
             if options.onedir:
                 if is_macos():
                     print("--onedir options is not supported on macOS.")
-                    exit(1)
+                    sys.exit(1)
                 pyi_args.append("--onedir")
             else:
                 pyi_args.append("--onefile")
 
             # copy "bin"
             hook_config.temp_bin_dir = copy_flet_bin()
 
@@ -217,8 +218,8 @@
             if hook_config.temp_bin_dir is not None and os.path.exists(
                 hook_config.temp_bin_dir
             ):
                 print("Deleting temp directory:", hook_config.temp_bin_dir)
                 shutil.rmtree(hook_config.temp_bin_dir, ignore_errors=True)
         except ImportError as e:
             print("Please install PyInstaller module to use flet pack command:", e)
-            exit(1)
+            sys.exit(1)
```

### Comparing `flet-0.6.0.dev1322/src/flet/cli/commands/publish.py` & `flet-0.6.0.dev1336/src/flet/cli/commands/publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import json
 import os
+import sys
 import re
 import shutil
 import tarfile
 import tempfile
 from distutils.dir_util import copy_tree
 from pathlib import Path
 
@@ -93,15 +94,15 @@
         # script path
         script_path = options.script
         if not os.path.isabs(script_path):
             script_path = str(Path(os.getcwd()).joinpath(script_path).resolve())
 
         if not Path(script_path).exists():
             print(f"File not found: {script_path}")
-            exit(1)
+            sys.exit(1)
 
         script_dir = os.path.dirname(script_path)
 
         # delete "dist" directory
         dist_dir = options.distpath
         if dist_dir:
             if not os.path.isabs(dist_dir):
@@ -114,27 +115,27 @@
             shutil.rmtree(dist_dir, ignore_errors=True)
         Path(dist_dir).mkdir(parents=True, exist_ok=True)
 
         # copy "web"
         web_path = get_package_web_dir()
         if not os.path.exists(web_path):
             print("Flet module does not contain 'web' directory.")
-            exit(1)
+            sys.exit(1)
         copy_tree(web_path, dist_dir)
 
         # copy assets
         assets_dir = options.assets_dir
         if assets_dir and not Path(assets_dir).is_absolute():
             assets_dir = str(
                 Path(os.path.dirname(script_path)).joinpath(assets_dir).resolve()
             )
         if assets_dir:
             if not os.path.exists(assets_dir):
                 print("Assets dir not found:", assets_dir)
-                exit(1)
+                sys.exit(1)
             copy_tree(assets_dir, dist_dir)
 
         # create "./dist/requirements.txt" if not exist
         # add flet-pyodide=={version} to dist/requirements.txt
         reqs_path = os.path.join(script_dir, reqs_filename)
 
         # add required dependencies
@@ -149,15 +150,15 @@
 
         pyodide_dep_found = False
         for dep in deps:
             if re.search("(^flet-pyodide$)|(^flet-pyodide[^a-z0-9-]+)", dep):
                 pyodide_dep_found = True
                 break
         if not pyodide_dep_found:
-            deps.append(f"flet-pyodide")
+            deps.append("flet-pyodide")
 
         temp_reqs_txt = Path(tempfile.gettempdir()).joinpath(random_string(10))
         with open(temp_reqs_txt, "w") as f:
             f.writelines(dep + "\n" for dep in deps)
 
         # pack all files in script's directory to dist/app.tar.gz
         app_tar_gz_path = os.path.join(dist_dir, app_tar_gz_filename)
```

### Comparing `flet-0.6.0.dev1322/src/flet/cli/commands/run.py` & `flet-0.6.0.dev1336/src/flet/cli/commands/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         # print("RUN COMMAND", options)
         script_path = options.script
         if not os.path.isabs(options.script):
             script_path = str(Path(os.getcwd()).joinpath(options.script).resolve())
 
         if not Path(script_path).exists():
             print(f"File not found: {script_path}")
-            exit(1)
+            sys.exit(1)
 
         script_dir = os.path.dirname(script_path)
 
         port = options.port
         if port is None and is_windows():
             port = get_free_tcp_port()
```

### Comparing `flet-0.6.0.dev1322/src/flet/flet.py` & `flet-0.6.0.dev1336/src/flet/flet.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
 def close_flet_view(pid_file):
     if pid_file is not None and os.path.exists(pid_file):
         try:
             with open(pid_file) as f:
                 fvp_pid = int(f.read())
             logger.debug(f"Flet View process {fvp_pid}")
             os.kill(fvp_pid, signal.SIGKILL)
-        except:
+        except Exception:
             pass
         finally:
             os.remove(pid_file)
 
 
 def __connect_internal_sync(
     page_name,
@@ -430,15 +430,15 @@
     else:
         # check if flet.exe is in PATH (flet developer mode)
         fletd_path = which(fletd_exe)
         if not fletd_path:
             # download flet from GitHub (python module developer mode)
             fletd_path = __download_fletd()
         else:
-            logger.info(f"Flet Server found in PATH")
+            logger.info("Flet Server found in PATH")
 
     fletd_env = {**os.environ}
 
     if upload_dir:
         if not Path(upload_dir).is_absolute():
             upload_dir = str(
                 Path(get_current_script_dir()).joinpath(upload_dir).resolve()
@@ -460,15 +460,15 @@
     if route_url_strategy is not None:
         logger.info(f"Route URL strategy configured: {route_url_strategy}")
         fletd_env["FLET_ROUTE_URL_STRATEGY"] = route_url_strategy
 
     web_root_dir = get_package_web_dir()
 
     if not os.path.exists(web_root_dir):
-        raise Exception("Web root path not found: {}".format(web_root_dir))
+        raise Exception(f"Web root path not found: {web_root_dir}")
 
     args = [fletd_path, "--content-dir", web_root_dir, "--port", str(port)]
 
     env_assets_dir = os.getenv("FLET_ASSETS_PATH")
     if env_assets_dir:
         assets_dir = env_assets_dir
 
@@ -536,15 +536,15 @@
                     Path(get_current_script_dir()).joinpath(assets_dir).resolve()
                 )
         logger.info(f"Assets path configured: {assets_dir}")
     return assets_dir
 
 
 def __locate_and_unpack_flet_view(page_url, assets_dir, hidden):
-    logger.info(f"Starting Flet View app...")
+    logger.info("Starting Flet View app...")
 
     args = []
 
     # pid file - Flet client writes its process ID to this file
     pid_file = str(Path(tempfile.gettempdir()).joinpath(random_string(20)))
 
     if is_windows():
```

### Comparing `flet-0.6.0.dev1322/src/flet/pubsub.py` & `flet-0.6.0.dev1336/src/flet/pubsub.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/reconnecting_websocket.py` & `flet-0.6.0.dev1336/src/flet/reconnecting_websocket.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,18 +61,18 @@
             self.default_timeout = websocket.getdefaulttimeout()
             websocket.setdefaulttimeout(
                 _LOCAL_CONNECT_TIMEOUT_SEC
                 if is_localhost_url(self._url)
                 else _REMOTE_CONNECT_TIMEOUT_SEC
             )
             r = self.wsapp.run_forever()
-            logger.debug(f"Exited run_forever()")
+            logger.debug("Exited run_forever()")
             websocket.setdefaulttimeout(self.default_timeout)
             self.connected.clear()
-            if r != True:
+            if r is not True:
                 return
 
             if self.retry == 0 and self._on_failed_connect_handler is not None:
                 th = threading.Thread(
                     target=self._on_failed_connect_handler, args=(), daemon=True
                 )
                 th.start()
```

### Comparing `flet-0.6.0.dev1322/src/flet/security.py` & `flet-0.6.0.dev1336/src/flet/security.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/sync_local_socket_connection.py` & `flet-0.6.0.dev1336/src/flet/sync_local_socket_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                     target=self.__on_event,
                     args=(self, self._create_update_control_props_handler_arg(msg)),
                     daemon=True,
                 )
                 th.start()
         else:
             # it's something else
-            raise Exception('Unknown message "{}": {}'.format(msg.action, msg.payload))
+            raise Exception(f'Unknown message "{msg.action}": {msg.payload}')
 
     def send_command(self, session_id: str, command: Command):
         result, message = self._process_command(command)
         if message:
             self.__send(message)
         return PageCommandResponsePayload(result=result, error="")
 
@@ -160,34 +160,34 @@
         self.__send_msg(self.__connection, j.encode("utf-8"))
 
     def __send_msg(self, sock, msg):
         # Prefix each message with a 4-byte length (network byte order)
         msg = struct.pack(">I", len(msg)) + msg
         try:
             sock.sendall(msg)
-            logger.debug("Sent: {}".format(len(msg)))
+            logger.debug(f"Sent: {len(msg)}")
         except Exception as e:
-            logger.debug("Error sending a message over a socket: {}".format(e))
+            logger.debug(f"Error sending a message over a socket: {e}")
 
     def __recv_msg(self, sock):
         # Read message length and unpack it into an integer
         raw_msglen = self.__recvall(sock, 4)
         if not raw_msglen:
             return None
         msglen = struct.unpack(">I", raw_msglen)[0]
-        logger.debug("Message size: {}".format(msglen))
+        logger.debug(f"Message size: {msglen}")
         # Read the message data
         return self.__recvall(sock, msglen)
 
     def __recvall(self, sock, n):
         # Helper function to recv n bytes or return None if EOF is hit
         data = bytearray()
         while len(data) < n:
             try:
                 packet = sock.recv(n - len(data))
-            except:
+            except Exception:
                 return None
             # print("packet received:", len(packet))
             if not packet:
                 return None
             data.extend(packet)
         return data
```

### Comparing `flet-0.6.0.dev1322/src/flet/sync_websocket_connection.py` & `flet-0.6.0.dev1336/src/flet/sync_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/utils.py` & `flet-0.6.0.dev1336/src/flet/utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/version.py` & `flet-0.6.0.dev1336/src/flet/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess as sp
 from pathlib import Path
 
 import flet
 from flet.utils import is_windows, which
 
 # this value will be replaced by CI
-version = "0.6.0.dev1322"
+version = "0.6.0.dev1336"
 
 
 def update_version():
     """Return the current version or default."""
     working = Path().absolute()
     os.chdir(Path(flet.__file__).absolute().parent)
     in_repo = which("git.exe" if is_windows() else "git") and sp.run(
```

### Comparing `flet-0.6.0.dev1322/src/flet/web/assets/NOTICES` & `flet-0.6.0.dev1336/src/flet/web/assets/NOTICES`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/web/assets/fonts/MaterialIcons-Regular.otf` & `flet-0.6.0.dev1336/src/flet/web/assets/fonts/MaterialIcons-Regular.otf`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/web/favicon.png` & `flet-0.6.0.dev1336/src/flet/web/favicon.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/web/flutter.js` & `flet-0.6.0.dev1336/src/flet/web/flutter.js`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/web/flutter_service_worker.js` & `flet-0.6.0.dev1336/src/flet/web/flutter_service_worker.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -24,16 +24,16 @@
     "icons/icon-512.png": "06b219f171b5a1af6dd8299ea1e116f2",
     "python.js": "9eee2c1773af78bc45ee89ca2ac5724f",
     "canvaskit/canvaskit.wasm": "3de12d898ec208a5f31362cc00f09b9e",
     "canvaskit/canvaskit.js": "97937cb4c2c2073c968525a3e08c86a3",
     "canvaskit/profiling/canvaskit.wasm": "371bc4e204443b0d5e774d64a046eb99",
     "canvaskit/profiling/canvaskit.js": "c21852696bc1cc82e8894d851c01921a",
     "python-worker.js": "b961f261b9ad85e06369e83fd2e33bb7",
-    "index.html": "a7193220d3e40d8746f3037f9037c74a",
-    "/": "a7193220d3e40d8746f3037f9037c74a"
+    "index.html": "23c96877653fbdbd659ec88b5073dd92",
+    "/": "23c96877653fbdbd659ec88b5073dd92"
 };
 
 // The application shell files that are downloaded before a service worker can
 // start.
 const CORE = [
     "main.dart.js",
     "index.html",
```

### Comparing `flet-0.6.0.dev1322/src/flet/web/icons/apple-touch-icon-192.png` & `flet-0.6.0.dev1336/src/flet/web/icons/apple-touch-icon-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/web/icons/icon-192.png` & `flet-0.6.0.dev1336/src/flet/web/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/web/icons/icon-512.png` & `flet-0.6.0.dev1336/src/flet/web/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/web/icons/icon-maskable-192.png` & `flet-0.6.0.dev1336/src/flet/web/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/web/icons/icon-maskable-512.png` & `flet-0.6.0.dev1336/src/flet/web/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/web/icons/loading-animation.png` & `flet-0.6.0.dev1336/src/flet/web/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/web/index.html` & `flet-0.6.0.dev1336/src/flet/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
   <!-- flutterWebRenderer -->
 
   <!-- pyodideCode -->
 
   <script>
     // The value below is injected by flutter build, do not touch.
-    var serviceWorkerVersion = '3001560998';
+    var serviceWorkerVersion = '3501097438';
   </script>
   <!-- This script adds the flutter initialization JS code -->
   <script src="flutter.js" defer></script>
 </head>
 
 <body>
   <div id="loading">
```

### Comparing `flet-0.6.0.dev1322/src/flet/web/main.dart.js` & `flet-0.6.0.dev1336/src/flet/web/main.dart.js`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/web/manifest.json` & `flet-0.6.0.dev1336/src/flet/web/manifest.json`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/web/python-worker.js` & `flet-0.6.0.dev1336/src/flet/web/python-worker.js`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/src/flet/web/python.js` & `flet-0.6.0.dev1336/src/flet/web/python.js`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1322/PKG-INFO` & `flet-0.6.0.dev1336/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flet
-Version: 0.6.0.dev1322
+Version: 0.6.0.dev1336
 Summary: Flet for Python - easily build interactive multi-platform apps in Python
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.6.0.dev1322)
+Requires-Dist: flet-core (==0.6.0.dev1336)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.8"
 Requires-Dist: watchdog (>=2.2.1,<3.0.0)
 Requires-Dist: websocket-client (>=1.4.2,<2.0.0)
 Requires-Dist: websockets (>=10.4,<11.0)
```

