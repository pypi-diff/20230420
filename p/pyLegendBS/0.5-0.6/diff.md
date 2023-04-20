# Comparing `tmp/pyLegendBS-0.5.tar.gz` & `tmp/pyLegendBS-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLegendBS-0.5.tar", last modified: Tue Apr  4 09:12:45 2023, max compression
+gzip compressed data, was "pyLegendBS-0.6.tar", last modified: Thu Apr 20 06:37:45 2023, max compression
```

## Comparing `pyLegendBS-0.5.tar` & `pyLegendBS-0.6.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 09:12:45.416273 pyLegendBS-0.5/
--rw-rw-rw-   0        0        0    35149 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-04 09:12:44.936265 pyLegendBS-0.5/LegendBS/
--rw-rw-rw-   0        0        0        1 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LegendBS/__init__.py
--rw-rw-rw-   0        0        0      543 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LegendBS/banall.py
--rw-rw-rw-   0        0        0     2536 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LegendBS/birthday.py
--rw-rw-rw-   0        0        0        1 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LegendBS/botspam.py
--rw-rw-rw-   0        0        0      369 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LegendBS/error.py
--rw-rw-rw-   0        0        0      390 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LegendBS/get_time.py
--rw-rw-rw-   0        0        0     2081 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LegendBS/get_user.py
--rw-rw-rw-   0        0        0     1705 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LegendBS/love.py
--rw-rw-rw-   0        0        0     3094 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LegendBS/porn.py
--rw-rw-rw-   0        0        0    33658 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LegendBS/raid.py
--rw-rw-rw-   0        0        0      911 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LegendBS/start.py
--rw-rw-rw-   0        0        0      198 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LegendBS/start_bot.py
--rw-rw-rw-   0        0        0        1 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LegendBS/start_help.py
--rw-rw-rw-   0        0        0    17800 2023-04-04 08:48:45.000000 pyLegendBS-0.5/LegendBS/yup.py
--rw-rw-rw-   0        0        0     1156 2023-04-04 09:12:45.373267 pyLegendBS-0.5/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-04-04 08:48:45.000000 pyLegendBS-0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 09:12:45.369271 pyLegendBS-0.5/pyLegendBS.egg-info/
--rw-rw-rw-   0        0        0     1156 2023-04-04 09:12:44.000000 pyLegendBS-0.5/pyLegendBS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-04-04 09:12:44.000000 pyLegendBS-0.5/pyLegendBS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 09:12:44.000000 pyLegendBS-0.5/pyLegendBS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-04 09:12:44.000000 pyLegendBS-0.5/pyLegendBS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-04 09:12:44.000000 pyLegendBS-0.5/pyLegendBS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 09:12:45.490274 pyLegendBS-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1413 2023-04-04 08:58:16.000000 pyLegendBS-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:37:45.610034 pyLegendBS-0.6/
+-rw-rw-rw-   0        0        0    35149 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-20 06:37:45.482025 pyLegendBS-0.6/LegendBS/
+-rw-rw-rw-   0        0        0        1 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/__init__.py
+-rw-rw-rw-   0        0        0      794 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/banall.py
+-rw-rw-rw-   0        0        0     2536 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/birthday.py
+-rw-rw-rw-   0        0        0        1 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/botspam.py
+-rw-rw-rw-   0        0        0      369 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/error.py
+-rw-rw-rw-   0        0        0      390 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/get_time.py
+-rw-rw-rw-   0        0        0     2081 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/get_user.py
+-rw-rw-rw-   0        0        0     1705 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/love.py
+-rw-rw-rw-   0        0        0     3094 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/porn.py
+-rw-rw-rw-   0        0        0    33658 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/raid.py
+-rw-rw-rw-   0        0        0      911 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/start.py
+-rw-rw-rw-   0        0        0      216 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/start_bot.py
+-rw-rw-rw-   0        0        0        1 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/start_help.py
+-rw-rw-rw-   0        0        0     3518 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/startup.py
+-rw-rw-rw-   0        0        0    17800 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/yup.py
+-rw-rw-rw-   0        0        0     1156 2023-04-20 06:37:45.601031 pyLegendBS-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-04-20 04:51:14.000000 pyLegendBS-0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 06:37:45.598034 pyLegendBS-0.6/pyLegendBS.egg-info/
+-rw-rw-rw-   0        0        0     1156 2023-04-20 06:37:45.000000 pyLegendBS-0.6/pyLegendBS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2023-04-20 06:37:45.000000 pyLegendBS-0.6/pyLegendBS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 06:37:45.000000 pyLegendBS-0.6/pyLegendBS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 06:37:45.000000 pyLegendBS-0.6/pyLegendBS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 06:37:45.000000 pyLegendBS-0.6/pyLegendBS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 06:37:45.610034 pyLegendBS-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1413 2023-04-20 04:51:14.000000 pyLegendBS-0.6/setup.py
```

### Comparing `pyLegendBS-0.5/LICENSE` & `pyLegendBS-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.5/LegendBS/banall.py` & `pyLegendBS-0.6/LegendBS/banall.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 async def start_banall(Legend, message):
-   chat = message.chat
-   x = Legend.send_message(chat.id, "Hey it's Legend Bot Spam")
-   done = 0
-   failed = 0
-   async for u in Legend.get_chat_members(chat.id):
-      user = u.user
-      try:
-         await Legend.ban_chat_member(chat.id, user.id)
-         done += 1
-      except Exception as err:
-         print(f"Legend Bot Spam- [INFO]: {str(err)}")
-         failed += 1
-   await x.delete()
-   await Legend.send_message(chat.id, f"Members Banned ✓ \n\n Banned {done} users\n failed {failed}")
+    chat = message.chat
+    a = await Legend.get_chat_member(chat.id, 'me')
+    if a.status == "administrator":
+        x = await Legend.send_message(chat.id, "Hey it's Legend Bot Spam")
+        done = 0
+        failed = 0
+        async for u in Legend.get_chat_members(chat.id):
+            user = u.user
+            try:
+                await Legend.ban_chat_member(chat.id, user.id)
+                done += 1
+            except Exception as err:
+                print(f"Legend Bot Spam- [INFO]: {str(err)}")
+                failed += 1
+        await x.delete()
+        await Legend.send_message(chat.id, f"Members Banned ✓ \n\n Banned {done} users\n failed {failed}")
+    else:
+        await Legend.send_message(chat.id, "Promote me to admin😭")
```

### Comparing `pyLegendBS-0.5/LegendBS/birthday.py` & `pyLegendBS-0.6/LegendBS/birthday.py`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.5/LegendBS/get_user.py` & `pyLegendBS-0.6/LegendBS/get_user.py`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.5/LegendBS/love.py` & `pyLegendBS-0.6/LegendBS/love.py`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.5/LegendBS/porn.py` & `pyLegendBS-0.6/LegendBS/porn.py`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.5/LegendBS/raid.py` & `pyLegendBS-0.6/LegendBS/raid.py`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.5/LegendBS/start.py` & `pyLegendBS-0.6/LegendBS/start.py`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.5/LegendBS/yup.py` & `pyLegendBS-0.6/LegendBS/yup.py`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.5/PKG-INFO` & `pyLegendBS-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLegendBS
-Version: 0.5
+Version: 0.6
 Summary: This is a simple package which is used in Bot Spam
 Home-page: https://github.com/LEGEND-AI/pyLegendBS
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyLegendBS,LegendBS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyLegendBS-0.5/pyLegendBS.egg-info/PKG-INFO` & `pyLegendBS-0.6/pyLegendBS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLegendBS
-Version: 0.5
+Version: 0.6
 Summary: This is a simple package which is used in Bot Spam
 Home-page: https://github.com/LEGEND-AI/pyLegendBS
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyLegendBS,LegendBS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyLegendBS-0.5/setup.py` & `pyLegendBS-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     sys.stderr.write( "Warning: Could not open README.md due %s\n" % error )
     
 
 setup(
     name="pyLegendBS",
     author="LegendBoy",
     author_email="krishna045jaiswal@gmail.com",
-    version="0.5",
+    version="0.6",
     description="This is a simple package which is used in Bot Spam",
     long_description = readme_contents,
     long_description_content_type="text/markdown",
     url="https://github.com/LEGEND-AI/pyLegendBS",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     include_package_data=True,
```

