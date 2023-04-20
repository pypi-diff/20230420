# Comparing `tmp/django-mails-2.4.tar.gz` & `tmp/django-mails-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mails-2.4.tar", last modified: Wed Apr 12 12:44:14 2023, max compression
+gzip compressed data, was "django-mails-2.5.tar", last modified: Thu Apr 20 07:52:20 2023, max compression
```

## Comparing `django-mails-2.4.tar` & `django-mails-2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-04-12 12:44:14.470213 django-mails-2.4/
--rw-rw-r--   0 manish    (1000) manish    (1000)     1076 2023-03-27 11:54:46.000000 django-mails-2.4/LICENSE
--rw-rw-r--   0 manish    (1000) manish    (1000)     2125 2023-04-12 12:44:14.470213 django-mails-2.4/PKG-INFO
--rw-rw-r--   0 manish    (1000) manish    (1000)     1312 2023-04-11 13:09:28.000000 django-mails-2.4/README.md
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-04-12 12:44:14.470213 django-mails-2.4/django_mails.egg-info/
--rw-rw-r--   0 manish    (1000) manish    (1000)     2125 2023-04-12 12:44:14.000000 django-mails-2.4/django_mails.egg-info/PKG-INFO
--rw-rw-r--   0 manish    (1000) manish    (1000)      457 2023-04-12 12:44:14.000000 django-mails-2.4/django_mails.egg-info/SOURCES.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)        1 2023-04-12 12:44:14.000000 django-mails-2.4/django_mails.egg-info/dependency_links.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)       97 2023-04-12 12:44:14.000000 django-mails-2.4/django_mails.egg-info/requires.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)       14 2023-04-12 12:44:14.000000 django-mails-2.4/django_mails.egg-info/top_level.txt
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-04-12 12:44:14.470213 django-mails-2.4/email_service/
--rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:30:19.000000 django-mails-2.4/email_service/__init__.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      339 2023-04-11 12:57:14.000000 django-mails-2.4/email_service/admin.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      157 2023-04-11 12:56:41.000000 django-mails-2.4/email_service/apps.py
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-04-12 12:44:14.470213 django-mails-2.4/email_service/migrations/
--rw-rw-r--   0 manish    (1000) manish    (1000)     3361 2023-03-24 11:13:02.000000 django-mails-2.4/email_service/migrations/0001_initial.py
--rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:30:19.000000 django-mails-2.4/email_service/migrations/__init__.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     2734 2023-03-27 07:58:51.000000 django-mails-2.4/email_service/models.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     2568 2023-04-11 12:57:15.000000 django-mails-2.4/email_service/tests.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     3082 2023-04-12 12:44:05.000000 django-mails-2.4/email_service/utils.py
--rw-rw-r--   0 manish    (1000) manish    (1000)       63 2023-03-24 10:30:19.000000 django-mails-2.4/email_service/views.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      966 2023-04-12 12:44:14.470213 django-mails-2.4/setup.cfg
--rw-rw-r--   0 manish    (1000) manish    (1000)       36 2023-03-28 03:53:50.000000 django-mails-2.4/setup.py
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-04-20 07:52:20.953899 django-mails-2.5/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     1076 2023-03-27 11:54:46.000000 django-mails-2.5/LICENSE
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2125 2023-04-20 07:52:20.953899 django-mails-2.5/PKG-INFO
+-rw-rw-r--   0 manish    (1000) manish    (1000)     1312 2023-04-11 13:09:28.000000 django-mails-2.5/README.md
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-04-20 07:52:20.953899 django-mails-2.5/django_mails.egg-info/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2125 2023-04-20 07:52:20.000000 django-mails-2.5/django_mails.egg-info/PKG-INFO
+-rw-rw-r--   0 manish    (1000) manish    (1000)      457 2023-04-20 07:52:20.000000 django-mails-2.5/django_mails.egg-info/SOURCES.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)        1 2023-04-20 07:52:20.000000 django-mails-2.5/django_mails.egg-info/dependency_links.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)       97 2023-04-20 07:52:20.000000 django-mails-2.5/django_mails.egg-info/requires.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)       14 2023-04-20 07:52:20.000000 django-mails-2.5/django_mails.egg-info/top_level.txt
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-04-20 07:52:20.953899 django-mails-2.5/email_service/
+-rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:30:19.000000 django-mails-2.5/email_service/__init__.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      339 2023-04-11 12:57:14.000000 django-mails-2.5/email_service/admin.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      157 2023-04-11 12:56:41.000000 django-mails-2.5/email_service/apps.py
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-04-20 07:52:20.953899 django-mails-2.5/email_service/migrations/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     3361 2023-03-24 11:13:02.000000 django-mails-2.5/email_service/migrations/0001_initial.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:30:19.000000 django-mails-2.5/email_service/migrations/__init__.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2734 2023-03-27 07:58:51.000000 django-mails-2.5/email_service/models.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2568 2023-04-11 12:57:15.000000 django-mails-2.5/email_service/tests.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     3261 2023-04-20 04:50:41.000000 django-mails-2.5/email_service/utils.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)       63 2023-03-24 10:30:19.000000 django-mails-2.5/email_service/views.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      966 2023-04-20 07:52:20.953899 django-mails-2.5/setup.cfg
+-rw-rw-r--   0 manish    (1000) manish    (1000)       36 2023-03-28 03:53:50.000000 django-mails-2.5/setup.py
```

### Comparing `django-mails-2.4/LICENSE` & `django-mails-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mails-2.4/PKG-INFO` & `django-mails-2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mails
-Version: 2.4
+Version: 2.5
 Summary: A Django Library to Send Simple/HTML Emails
 Home-page: https://www.example.com/
 Author: Harsh
 Author-email: harsh@hashtrust.in
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 4.1
```

### Comparing `django-mails-2.4/README.md` & `django-mails-2.5/README.md`

 * *Files identical despite different names*

### Comparing `django-mails-2.4/django_mails.egg-info/PKG-INFO` & `django-mails-2.5/django_mails.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mails
-Version: 2.4
+Version: 2.5
 Summary: A Django Library to Send Simple/HTML Emails
 Home-page: https://www.example.com/
 Author: Harsh
 Author-email: harsh@hashtrust.in
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 4.1
```

### Comparing `django-mails-2.4/email_service/migrations/0001_initial.py` & `django-mails-2.5/email_service/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mails-2.4/email_service/models.py` & `django-mails-2.5/email_service/models.py`

 * *Files identical despite different names*

### Comparing `django-mails-2.4/email_service/tests.py` & `django-mails-2.5/email_service/tests.py`

 * *Files identical despite different names*

### Comparing `django-mails-2.4/email_service/utils.py` & `django-mails-2.5/email_service/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     recipient: List[str] | str,
     path: str | None = None,
     template: any = None,
     template_prefix: str | None = None,
     context: Dict = {},
     subject: str | None = None,
     body: str | None = None,
+    attachement: any = None,
+    attachement_name : str | None = None
 ) -> None:
     from email_service.models import Email
 
     if not recipient or len(recipient) == 0:
         logger.error(
             "Please provide at least one recipient."
         )
@@ -67,14 +69,16 @@
             template=template,
         )
         text_content = html2text.HTML2Text().handle(html_content)
         msg = EmailMultiAlternatives(
             subject or email_subject, text_content, from_email, to, bcc=[bcc_email]
         )
         msg.attach_alternative(html_content, "text/html")
+        if attachement:
+            msg.attach(attachement_name,attachement.read(),attachement.content_type)
         msg.send()
         return "Email Sent Successfully."
     except Exception as ex:
         logger.exception(
             f"""Caught exception {ex} while sending email with params:
             path-{path} template-{template_prefix}, recipient-{recipient},
             context-{context}, subject-{subject}, body-{body}"""
```

### Comparing `django-mails-2.4/setup.cfg` & `django-mails-2.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-mails
-version = 2.4
+version = 2.5
 description = A Django Library to Send Simple/HTML Emails
 readme = "README.md"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.example.com/
 author = Harsh
 author_email = harsh@hashtrust.in
```

