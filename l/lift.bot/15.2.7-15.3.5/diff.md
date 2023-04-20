# Comparing `tmp/lift.bot-15.2.7.tar.gz` & `tmp/lift.bot-15.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lift.bot-15.2.7.tar", last modified: Thu Apr 20 03:10:17 2023, max compression
+gzip compressed data, was "lift.bot-15.3.5.tar", last modified: Thu Apr 20 03:44:29 2023, max compression
```

## Comparing `lift.bot-15.2.7.tar` & `lift.bot-15.3.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 03:10:17.725858 lift.bot-15.2.7/
--rw-rw-rw-   0        0        0      715 2023-04-20 03:10:17.719858 lift.bot-15.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-20 03:10:17.639918 lift.bot-15.2.7/lift/
--rw-rw-rw-   0        0        0        0 2023-04-20 03:08:06.000000 lift.bot-15.2.7/lift/__init__.py
--rw-rw-rw-   0        0        0    31867 2023-04-20 03:08:04.000000 lift.bot-15.2.7/lift/gradient.py
--rw-rw-rw-   0        0        0     3040 2023-04-20 03:08:03.000000 lift.bot-15.2.7/lift/lft.py
--rw-rw-rw-   0        0        0     1175 2023-04-20 03:08:07.000000 lift.bot-15.2.7/lift/status.py
-drwxrwxrwx   0        0        0        0 2023-04-20 03:10:17.715861 lift.bot-15.2.7/lift.bot.egg-info/
--rw-rw-rw-   0        0        0      715 2023-04-20 03:10:17.000000 lift.bot-15.2.7/lift.bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-20 03:10:17.000000 lift.bot-15.2.7/lift.bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 03:10:17.000000 lift.bot-15.2.7/lift.bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-20 03:10:17.000000 lift.bot-15.2.7/lift.bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-20 03:10:17.000000 lift.bot-15.2.7/lift.bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 03:10:17.726855 lift.bot-15.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-04-20 03:10:09.000000 lift.bot-15.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:44:29.806688 lift.bot-15.3.5/
+-rw-rw-rw-   0        0        0      715 2023-04-20 03:44:29.803693 lift.bot-15.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1403 2023-04-20 03:42:22.000000 lift.bot-15.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 03:44:29.724743 lift.bot-15.3.5/lift/
+-rw-rw-rw-   0        0        0        0 2023-04-20 03:08:06.000000 lift.bot-15.3.5/lift/__init__.py
+-rw-rw-rw-   0        0        0    31867 2023-04-20 03:08:04.000000 lift.bot-15.3.5/lift/gradient.py
+-rw-rw-rw-   0        0        0     3040 2023-04-20 03:08:03.000000 lift.bot-15.3.5/lift/lft.py
+-rw-rw-rw-   0        0        0     1175 2023-04-20 03:08:07.000000 lift.bot-15.3.5/lift/status.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:44:29.797693 lift.bot-15.3.5/lift.bot.egg-info/
+-rw-rw-rw-   0        0        0      715 2023-04-20 03:44:29.000000 lift.bot-15.3.5/lift.bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-04-20 03:44:29.000000 lift.bot-15.3.5/lift.bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 03:44:29.000000 lift.bot-15.3.5/lift.bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-20 03:44:29.000000 lift.bot-15.3.5/lift.bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-20 03:44:29.000000 lift.bot-15.3.5/lift.bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 03:44:29.806688 lift.bot-15.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1155 2023-04-20 03:10:09.000000 lift.bot-15.3.5/setup.py
```

### Comparing `lift.bot-15.2.7/PKG-INFO` & `lift.bot-15.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lift.bot
-Version: 15.2.7
+Version: 15.3.5
 Summary: lift.bot
 Home-page: https://github.com/bytebuildz/liftcord.py-tools/
 Author: .drmr
 Author-email: hi@icey.fr
 License: MIT License
 Keywords: lift
 Classifier: Programming Language :: Python
```

### Comparing `lift.bot-15.2.7/lift/gradient.py` & `lift.bot-15.3.5/lift/gradient.py`

 * *Files identical despite different names*

### Comparing `lift.bot-15.2.7/lift/lft.py` & `lift.bot-15.3.5/lift/lft.py`

 * *Files identical despite different names*

### Comparing `lift.bot-15.2.7/lift/status.py` & `lift.bot-15.3.5/lift/status.py`

 * *Files identical despite different names*

### Comparing `lift.bot-15.2.7/lift.bot.egg-info/PKG-INFO` & `lift.bot-15.3.5/lift.bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lift.bot
-Version: 15.2.7
+Version: 15.3.5
 Summary: lift.bot
 Home-page: https://github.com/bytebuildz/liftcord.py-tools/
 Author: .drmr
 Author-email: hi@icey.fr
 License: MIT License
 Keywords: lift
 Classifier: Programming Language :: Python
```

### Comparing `lift.bot-15.2.7/setup.py` & `lift.bot-15.3.5/setup.py`

 * *Files identical despite different names*

