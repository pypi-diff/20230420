# Comparing `tmp/ticgithub-0.1.0.tar.gz` & `tmp/ticgithub-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ticgithub-0.1.0.tar", last modified: Tue Feb 28 23:37:21 2023, max compression
+gzip compressed data, was "ticgithub-0.1.1.tar", last modified: Thu Apr 20 13:47:37 2023, max compression
```

## Comparing `ticgithub-0.1.0.tar` & `ticgithub-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:21.643767 ticgithub-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-28 23:37:09.000000 ticgithub-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-28 23:37:09.000000 ticgithub-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-02-28 23:37:21.643767 ticgithub-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-02-28 23:37:09.000000 ticgithub-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-02-28 23:37:21.643767 ticgithub-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-02-28 23:37:09.000000 ticgithub-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:21.643767 ticgithub-0.1.0/ticgithub/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-28 23:37:21.000000 ticgithub-0.1.0/ticgithub/_installed_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:21.643767 ticgithub-0.1.0/ticgithub/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:21.643767 ticgithub-0.1.0/ticgithub/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/data/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/data/templates/email_reply.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/data/templates/unassigned.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/data/templates/unclosed.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:21.643767 ticgithub-0.1.0/ticgithub/data/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/data/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/data/workflows/assignment-to-gmail.yml
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/data/workflows/scheduled_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/inbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/issues.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:21.643767 ticgithub-0.1.0/ticgithub/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/tasks/assignment_to_gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/tasks/emails_to_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/tasks/reminder_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/tasks/unassigned_reminder.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/tasks/unclosed_reminder.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/team.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:21.643767 ticgithub-0.1.0/ticgithub/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/tests/test_something.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:21.643767 ticgithub-0.1.0/ticgithub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/utils/datafiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-02-28 23:37:09.000000 ticgithub-0.1.0/ticgithub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 23:37:21.643767 ticgithub-0.1.0/ticgithub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-02-28 23:37:21.000000 ticgithub-0.1.0/ticgithub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-28 23:37:21.000000 ticgithub-0.1.0/ticgithub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 23:37:21.000000 ticgithub-0.1.0/ticgithub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-28 23:37:21.000000 ticgithub-0.1.0/ticgithub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-28 23:37:21.000000 ticgithub-0.1.0/ticgithub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:37.755353 ticgithub-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 13:47:22.000000 ticgithub-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 13:47:22.000000 ticgithub-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-04-20 13:47:37.755353 ticgithub-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-04-20 13:47:22.000000 ticgithub-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-20 13:47:37.755353 ticgithub-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-20 13:47:22.000000 ticgithub-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:37.755353 ticgithub-0.1.1/ticgithub/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 13:47:37.000000 ticgithub-0.1.1/ticgithub/_installed_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:37.755353 ticgithub-0.1.1/ticgithub/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:37.755353 ticgithub-0.1.1/ticgithub/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/data/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/data/templates/email_reply.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/data/templates/unassigned.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/data/templates/unclosed.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:37.755353 ticgithub-0.1.1/ticgithub/data/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/data/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/data/workflows/assignment-to-gmail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/data/workflows/scheduled_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/inbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/issues.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:37.755353 ticgithub-0.1.1/ticgithub/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/tasks/assignment_to_gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/tasks/emails_to_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/tasks/reminder_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/tasks/unassigned_reminder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/tasks/unclosed_reminder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/team.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:37.755353 ticgithub-0.1.1/ticgithub/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/tests/test_something.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:37.755353 ticgithub-0.1.1/ticgithub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/utils/datafiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-04-20 13:47:22.000000 ticgithub-0.1.1/ticgithub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:47:37.755353 ticgithub-0.1.1/ticgithub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-04-20 13:47:37.000000 ticgithub-0.1.1/ticgithub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 13:47:37.000000 ticgithub-0.1.1/ticgithub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:47:37.000000 ticgithub-0.1.1/ticgithub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 13:47:37.000000 ticgithub-0.1.1/ticgithub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 13:47:37.000000 ticgithub-0.1.1/ticgithub.egg-info/top_level.txt
```

### Comparing `ticgithub-0.1.0/LICENSE` & `ticgithub-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.0/PKG-INFO` & `ticgithub-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ticgithub
-Version: 0.1.0
+Version: 0.1.1
 Summary: Use GitHub as a ticketing system for shared GMail
 Home-page: https://github.com/dwhswenson/ticgithub
 Author: David W.H. Swenson
 Author-email: dwhs@hyperblazer.net
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `ticgithub-0.1.0/README.md` & `ticgithub-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.0/setup.cfg` & `ticgithub-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ticgithub
-version = 0.1.0
+version = 0.1.1
 short_description = Use GitHub as a ticketing system for shared GMail
 description = Use GitHub as a ticketing system for shared GMail
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = David W.H. Swenson
 author_email = dwhs@hyperblazer.net
 license = MIT
```

### Comparing `ticgithub-0.1.0/setup.py` & `ticgithub-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.0/ticgithub/bot.py` & `ticgithub-0.1.1/ticgithub/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.user = user
         self.host = host
         self.secret = secret
         self.port = port
 
     def sendmail(self, email, recipients):
         with smtplib.SMTP_SSL(self.host, self.port) as smtp:
-            smtp.login(user, os.environ.get(self.secret))
+            smtp.login(self.user, os.environ.get(self.secret))
             smtp.sendmail(self.user, recipients, email.as_string())
 
     def __repr__(self):
         return (f"{self.__class__.__name__}('{self.user}:"
                 f"{self.port}")
```

### Comparing `ticgithub-0.1.0/ticgithub/build.py` & `ticgithub-0.1.1/ticgithub/build.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.0/ticgithub/gmail.py` & `ticgithub-0.1.1/ticgithub/gmail.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.0/ticgithub/inbox.py` & `ticgithub-0.1.1/ticgithub/inbox.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.0/ticgithub/issues.py` & `ticgithub-0.1.1/ticgithub/issues.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.0/ticgithub/tasks/assignment_to_gmail.py` & `ticgithub-0.1.1/ticgithub/tasks/assignment_to_gmail.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.0/ticgithub/tasks/emails_to_issues.py` & `ticgithub-0.1.1/ticgithub/tasks/emails_to_issues.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.0/ticgithub/tasks/reminder_task.py` & `ticgithub-0.1.1/ticgithub/tasks/reminder_task.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.0/ticgithub/tasks/task.py` & `ticgithub-0.1.1/ticgithub/tasks/task.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.0/ticgithub/tasks/unassigned_reminder.py` & `ticgithub-0.1.1/ticgithub/tasks/unassigned_reminder.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.0/ticgithub/tasks/unclosed_reminder.py` & `ticgithub-0.1.1/ticgithub/tasks/unclosed_reminder.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.0/ticgithub/version.py` & `ticgithub-0.1.1/ticgithub/version.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.0/ticgithub.egg-info/PKG-INFO` & `ticgithub-0.1.1/ticgithub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ticgithub
-Version: 0.1.0
+Version: 0.1.1
 Summary: Use GitHub as a ticketing system for shared GMail
 Home-page: https://github.com/dwhswenson/ticgithub
 Author: David W.H. Swenson
 Author-email: dwhs@hyperblazer.net
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `ticgithub-0.1.0/ticgithub.egg-info/SOURCES.txt` & `ticgithub-0.1.1/ticgithub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

