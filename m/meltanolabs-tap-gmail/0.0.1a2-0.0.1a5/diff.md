# Comparing `tmp/meltanolabs_tap_gmail-0.0.1a2.tar.gz` & `tmp/meltanolabs_tap_gmail-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_tap_gmail-0.0.1a2.tar", max compression
+gzip compressed data, was "meltanolabs_tap_gmail-0.0.1a5.tar", max compression
```

## Comparing `meltanolabs_tap_gmail-0.0.1a2.tar` & `meltanolabs_tap_gmail-0.0.1a5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1066 2023-04-20 10:31:51.677962 meltanolabs_tap_gmail-0.0.1a2/LICENSE
--rw-r--r--   0        0        0      974 2023-04-20 10:55:29.343596 meltanolabs_tap_gmail-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 10:31:51.679292 meltanolabs_tap_gmail-0.0.1a2/tap_gmail/__init__.py
--rw-r--r--   0        0        0     1122 2023-04-20 10:31:51.679434 meltanolabs_tap_gmail-0.0.1a2/tap_gmail/auth.py
--rw-r--r--   0        0        0     2051 2023-04-20 10:31:51.679735 meltanolabs_tap_gmail-0.0.1a2/tap_gmail/client.py
--rw-r--r--   0        0        0      261 2023-04-20 10:31:51.680071 meltanolabs_tap_gmail-0.0.1a2/tap_gmail/schemas/message_list.json
--rw-r--r--   0        0        0     4082 2023-04-20 10:31:51.680240 meltanolabs_tap_gmail-0.0.1a2/tap_gmail/schemas/messages.json
--rw-r--r--   0        0        0     1595 2023-04-20 10:31:51.680374 meltanolabs_tap_gmail-0.0.1a2/tap_gmail/streams.py
--rw-r--r--   0        0        0     1830 2023-04-20 10:31:51.680511 meltanolabs_tap_gmail-0.0.1a2/tap_gmail/tap.py
--rw-r--r--   0        0        0       32 2023-04-20 10:31:51.680672 meltanolabs_tap_gmail-0.0.1a2/tap_gmail/tests/__init__.py
--rw-r--r--   0        0        0      645 2023-04-20 10:31:51.680790 meltanolabs_tap_gmail-0.0.1a2/tap_gmail/tests/test_core.py
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 meltanolabs_tap_gmail-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-20 11:20:14.718042 meltanolabs_tap_gmail-0.0.1a5/LICENSE
+-rw-r--r--   0        0        0     2253 2023-04-20 11:20:14.718042 meltanolabs_tap_gmail-0.0.1a5/README.md
+-rw-r--r--   0        0        0      995 2023-04-20 11:20:34.482016 meltanolabs_tap_gmail-0.0.1a5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 11:20:14.718042 meltanolabs_tap_gmail-0.0.1a5/tap_gmail/__init__.py
+-rw-r--r--   0        0        0     1122 2023-04-20 11:20:14.718042 meltanolabs_tap_gmail-0.0.1a5/tap_gmail/auth.py
+-rw-r--r--   0        0        0     2051 2023-04-20 11:20:14.718042 meltanolabs_tap_gmail-0.0.1a5/tap_gmail/client.py
+-rw-r--r--   0        0        0      261 2023-04-20 11:20:14.718042 meltanolabs_tap_gmail-0.0.1a5/tap_gmail/schemas/message_list.json
+-rw-r--r--   0        0        0     4082 2023-04-20 11:20:14.718042 meltanolabs_tap_gmail-0.0.1a5/tap_gmail/schemas/messages.json
+-rw-r--r--   0        0        0     1595 2023-04-20 11:20:14.718042 meltanolabs_tap_gmail-0.0.1a5/tap_gmail/streams.py
+-rw-r--r--   0        0        0     1830 2023-04-20 11:20:14.718042 meltanolabs_tap_gmail-0.0.1a5/tap_gmail/tap.py
+-rw-r--r--   0        0        0       32 2023-04-20 11:20:14.718042 meltanolabs_tap_gmail-0.0.1a5/tap_gmail/tests/__init__.py
+-rw-r--r--   0        0        0      645 2023-04-20 11:20:14.718042 meltanolabs_tap_gmail-0.0.1a5/tap_gmail/tests/test_core.py
+-rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 meltanolabs_tap_gmail-0.0.1a5/PKG-INFO
```

### Comparing `meltanolabs_tap_gmail-0.0.1a2/LICENSE` & `meltanolabs_tap_gmail-0.0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `meltanolabs_tap_gmail-0.0.1a2/pyproject.toml` & `meltanolabs_tap_gmail-0.0.1a5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.poetry]
 name = "meltanolabs-tap-gmail"
-version = "0.0.1-a.2"
+version = "0.0.1-a.5"
 description = "`tap-gmail` is a Singer tap for Gmail, built with the Meltano SDK for Singer Taps."
+readme = "README.md"
 authors = ["Ken Payne"]
 keywords = [
     "ELT",
     "Gmail",
 ]
 license = "Apache 2.0"
 packages = [
```

### Comparing `meltanolabs_tap_gmail-0.0.1a2/tap_gmail/auth.py` & `meltanolabs_tap_gmail-0.0.1a5/tap_gmail/auth.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_tap_gmail-0.0.1a2/tap_gmail/client.py` & `meltanolabs_tap_gmail-0.0.1a5/tap_gmail/client.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_tap_gmail-0.0.1a2/tap_gmail/schemas/messages.json` & `meltanolabs_tap_gmail-0.0.1a5/tap_gmail/schemas/messages.json`

 * *Files identical despite different names*

### Comparing `meltanolabs_tap_gmail-0.0.1a2/tap_gmail/streams.py` & `meltanolabs_tap_gmail-0.0.1a5/tap_gmail/streams.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_tap_gmail-0.0.1a2/tap_gmail/tap.py` & `meltanolabs_tap_gmail-0.0.1a5/tap_gmail/tap.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_tap_gmail-0.0.1a2/tap_gmail/tests/test_core.py` & `meltanolabs_tap_gmail-0.0.1a5/tap_gmail/tests/test_core.py`

 * *Files identical despite different names*

