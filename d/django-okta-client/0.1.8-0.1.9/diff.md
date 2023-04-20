# Comparing `tmp/django-okta-client-0.1.8.tar.gz` & `tmp/django-okta-client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-okta-client-0.1.8.tar", last modified: Thu Apr 20 16:17:04 2023, max compression
+gzip compressed data, was "django-okta-client-0.1.9.tar", last modified: Thu Apr 20 19:55:46 2023, max compression
```

## Comparing `django-okta-client-0.1.8.tar` & `django-okta-client-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 16:17:04.259855 django-okta-client-0.1.8/
--rw-rw-rw-   0        0        0     1349 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1084 2023-04-20 16:17:04.258854 django-okta-client-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2322 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 16:17:04.229331 django-okta-client-0.1.8/django_okta_client.egg-info/
--rw-rw-rw-   0        0        0     1084 2023-04-20 16:17:04.000000 django-okta-client-0.1.8/django_okta_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-04-20 16:17:04.000000 django-okta-client-0.1.8/django_okta_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 16:17:04.000000 django-okta-client-0.1.8/django_okta_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-20 16:17:04.000000 django-okta-client-0.1.8/django_okta_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-20 16:17:04.000000 django-okta-client-0.1.8/django_okta_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 16:17:04.247876 django-okta-client-0.1.8/okta_client/
--rw-rw-rw-   0        0        0      169 2023-04-20 16:15:09.000000 django-okta-client-0.1.8/okta_client/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-03-06 22:25:24.000000 django-okta-client-0.1.8/okta_client/admin.py
--rw-rw-rw-   0        0        0      159 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/apps.py
--rw-rw-rw-   0        0        0     1513 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/managers.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:17:04.254854 django-okta-client-0.1.8/okta_client/migrations/
--rw-rw-rw-   0        0        0     6432 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     9555 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/migrations/0002_alter_oktauser_options_alter_oktauser_managers_and_more.py
--rw-rw-rw-   0        0        0        0 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/migrations/__init__.py
--rw-rw-rw-   0        0        0     7920 2023-04-20 16:05:38.000000 django-okta-client-0.1.8/okta_client/models.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:17:04.200314 django-okta-client-0.1.8/okta_client/templates/
-drwxrwxrwx   0        0        0        0 2023-04-20 16:17:04.256853 django-okta-client-0.1.8/okta_client/templates/okta-client/
--rw-rw-rw-   0        0        0     4445 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/templates/okta-client/index.html
--rw-rw-rw-   0        0        0       63 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/tests.py
--rw-rw-rw-   0        0        0      286 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/urls.py
--rw-rw-rw-   0        0        0     7046 2023-04-20 16:00:25.000000 django-okta-client-0.1.8/okta_client/views.py
--rw-rw-rw-   0        0        0     1262 2023-03-21 17:38:10.000000 django-okta-client-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 16:17:04.261363 django-okta-client-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      208 2023-03-21 17:29:55.000000 django-okta-client-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:55:46.266538 django-okta-client-0.1.9/
+-rw-rw-rw-   0        0        0     1349 2023-03-06 15:01:57.000000 django-okta-client-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1084 2023-04-20 19:55:46.265537 django-okta-client-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2322 2023-03-06 15:01:57.000000 django-okta-client-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 19:55:46.235980 django-okta-client-0.1.9/django_okta_client.egg-info/
+-rw-rw-rw-   0        0        0     1084 2023-04-20 19:55:46.000000 django-okta-client-0.1.9/django_okta_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2023-04-20 19:55:46.000000 django-okta-client-0.1.9/django_okta_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 19:55:46.000000 django-okta-client-0.1.9/django_okta_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-20 19:55:46.000000 django-okta-client-0.1.9/django_okta_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 19:55:46.000000 django-okta-client-0.1.9/django_okta_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 19:55:46.252997 django-okta-client-0.1.9/okta_client/
+-rw-rw-rw-   0        0        0      169 2023-04-20 19:51:26.000000 django-okta-client-0.1.9/okta_client/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-03-06 22:25:24.000000 django-okta-client-0.1.9/okta_client/admin.py
+-rw-rw-rw-   0        0        0      159 2023-03-06 15:01:57.000000 django-okta-client-0.1.9/okta_client/apps.py
+-rw-rw-rw-   0        0        0     1513 2023-03-06 15:01:57.000000 django-okta-client-0.1.9/okta_client/managers.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:55:46.260524 django-okta-client-0.1.9/okta_client/migrations/
+-rw-rw-rw-   0        0        0     6432 2023-03-06 15:01:57.000000 django-okta-client-0.1.9/okta_client/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     9555 2023-03-06 15:01:57.000000 django-okta-client-0.1.9/okta_client/migrations/0002_alter_oktauser_options_alter_oktauser_managers_and_more.py
+-rw-rw-rw-   0        0        0        0 2023-03-06 15:01:57.000000 django-okta-client-0.1.9/okta_client/migrations/__init__.py
+-rw-rw-rw-   0        0        0     7920 2023-04-20 16:05:38.000000 django-okta-client-0.1.9/okta_client/models.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:55:46.196978 django-okta-client-0.1.9/okta_client/templates/
+drwxrwxrwx   0        0        0        0 2023-04-20 19:55:46.262545 django-okta-client-0.1.9/okta_client/templates/okta-client/
+-rw-rw-rw-   0        0        0     4445 2023-03-06 15:01:57.000000 django-okta-client-0.1.9/okta_client/templates/okta-client/index.html
+-rw-rw-rw-   0        0        0       63 2023-03-06 15:01:57.000000 django-okta-client-0.1.9/okta_client/tests.py
+-rw-rw-rw-   0        0        0      286 2023-03-06 15:01:57.000000 django-okta-client-0.1.9/okta_client/urls.py
+-rw-rw-rw-   0        0        0     7674 2023-04-20 19:53:35.000000 django-okta-client-0.1.9/okta_client/views.py
+-rw-rw-rw-   0        0        0     1262 2023-03-21 17:38:10.000000 django-okta-client-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 19:55:46.266538 django-okta-client-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      208 2023-03-21 17:29:55.000000 django-okta-client-0.1.9/setup.py
```

### Comparing `django-okta-client-0.1.8/LICENSE` & `django-okta-client-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.8/PKG-INFO` & `django-okta-client-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-okta-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Okta client Django app
 Author-email: Irving Leonard <irvingleonard@gmail.com>
 License: BSD 2-Clause "Simplified" License
 Project-URL: homepage, https://github.com/irvingleonard/django-okta-client
 Project-URL: repository, https://github.com/irvingleonard/django-okta-client.git
 Keywords: okta,saml,saml2
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-okta-client-0.1.8/README.md` & `django-okta-client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.8/django_okta_client.egg-info/PKG-INFO` & `django-okta-client-0.1.9/django_okta_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-okta-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Okta client Django app
 Author-email: Irving Leonard <irvingleonard@gmail.com>
 License: BSD 2-Clause "Simplified" License
 Project-URL: homepage, https://github.com/irvingleonard/django-okta-client
 Project-URL: repository, https://github.com/irvingleonard/django-okta-client.git
 Keywords: okta,saml,saml2
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-okta-client-0.1.8/django_okta_client.egg-info/SOURCES.txt` & `django-okta-client-0.1.9/django_okta_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.8/okta_client/admin.py` & `django-okta-client-0.1.9/okta_client/admin.py`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.8/okta_client/managers.py` & `django-okta-client-0.1.9/okta_client/managers.py`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.8/okta_client/migrations/0001_initial.py` & `django-okta-client-0.1.9/okta_client/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.8/okta_client/migrations/0002_alter_oktauser_options_alter_oktauser_managers_and_more.py` & `django-okta-client-0.1.9/okta_client/migrations/0002_alter_oktauser_options_alter_oktauser_managers_and_more.py`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.8/okta_client/models.py` & `django-okta-client-0.1.9/okta_client/models.py`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.8/okta_client/templates/okta-client/index.html` & `django-okta-client-0.1.9/okta_client/templates/okta-client/index.html`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.8/okta_client/views.py` & `django-okta-client-0.1.9/okta_client/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,17 +82,18 @@
 	'''Okta Event Hook endpoint
 	Follow Okta's way to do Okta Event Hooks, for your convenience.
 	
 	Your class based view, the one that inherits this mixin, should implement an *okta_"type_of_event"* method for each event type that this view will handle where "type_of_event" will be the event type reported by okta with the dots replaced by underscores. Ex: okta_user_session_start
 	
 	There's also the option to implement a fallback "okta_event" method that will be used if no specific method exists for an event type.
 	
-	All these methods should expect 2 parameters:
+	All these methods should expect 3 parameters:
 	- request: is the Django request object provided to the view
-	- event is the already parsed event that should be processed in this iteration
+	- event: is the already parsed event that should be processed in this iteration
+	- event_targets: is the list of targets in the event as a dictionary keyd by type (an error will be raised if overlapping types). It could be "None" if no targets are present on the event object.
 	
 	Ref: https://developer.okta.com/docs/concepts/event-hooks/
 	'''
 	
 	def get(self, request):
 		'''HTTP GET
 		Only used to confirm that it follows Okta's convention.
@@ -105,18 +106,26 @@
 		Regular Event Hook handling.
 		'''
 		
 		request_body = json.loads(request.body)
 		not_implemented = False
 		for event in request_body['data']['events']:
 			method_name = 'okta_' + event['eventType'].replace('.', '_')
+			if ('target' in event) and (event['target'] is not None):
+				event_targets = {}
+				for target in event['target']:
+					if target['type'] in event_targets:
+						raise RuntimeError('Okta event with overlapping targets: {}'.format(event['uuid']))
+					event_targets[target['type']] = {key : value for key, value in target.items() if key not in ['type']}
+			else:
+				event_targets = None
 			if hasattr(self, method_name):
-				getattr(self, method_name)(request, event)
+				getattr(self, method_name)(request, event, event_targets)
 			elif hasattr(self, 'okta_event'):
-				getattr(self, 'okta_event')(request, event)
+				getattr(self, 'okta_event')(request, event, event_targets)
 			else:
 				not_implemented = True
 				LOGGER.warning('Okta event support not implemented: %s', event['eventType'])
 
 		if not_implemented:
 			return HttpResponse(status = 501)
 		else:
```

### Comparing `django-okta-client-0.1.8/pyproject.toml` & `django-okta-client-0.1.9/pyproject.toml`

 * *Files identical despite different names*

