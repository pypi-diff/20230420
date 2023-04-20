# Comparing `tmp/django-okta-client-0.1.7.tar.gz` & `tmp/django-okta-client-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-okta-client-0.1.7.tar", last modified: Tue Mar 21 17:38:23 2023, max compression
+gzip compressed data, was "django-okta-client-0.1.8.tar", last modified: Thu Apr 20 16:17:04 2023, max compression
```

## Comparing `django-okta-client-0.1.7.tar` & `django-okta-client-0.1.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 17:38:23.344636 django-okta-client-0.1.7/
--rw-rw-rw-   0        0        0     1349 2023-03-06 15:01:57.000000 django-okta-client-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     1084 2023-03-21 17:38:23.343635 django-okta-client-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2322 2023-03-06 15:01:57.000000 django-okta-client-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-21 17:38:23.314639 django-okta-client-0.1.7/django_okta_client.egg-info/
--rw-rw-rw-   0        0        0     1084 2023-03-21 17:38:23.000000 django-okta-client-0.1.7/django_okta_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-03-21 17:38:23.000000 django-okta-client-0.1.7/django_okta_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 17:38:23.000000 django-okta-client-0.1.7/django_okta_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-03-21 17:38:23.000000 django-okta-client-0.1.7/django_okta_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-21 17:38:23.000000 django-okta-client-0.1.7/django_okta_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-21 17:38:23.332637 django-okta-client-0.1.7/okta_client/
--rw-rw-rw-   0        0        0      169 2023-03-21 17:04:41.000000 django-okta-client-0.1.7/okta_client/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-03-06 22:25:24.000000 django-okta-client-0.1.7/okta_client/admin.py
--rw-rw-rw-   0        0        0      159 2023-03-06 15:01:57.000000 django-okta-client-0.1.7/okta_client/apps.py
--rw-rw-rw-   0        0        0     1513 2023-03-06 15:01:57.000000 django-okta-client-0.1.7/okta_client/managers.py
-drwxrwxrwx   0        0        0        0 2023-03-21 17:38:23.339631 django-okta-client-0.1.7/okta_client/migrations/
--rw-rw-rw-   0        0        0     6432 2023-03-06 15:01:57.000000 django-okta-client-0.1.7/okta_client/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     9555 2023-03-06 15:01:57.000000 django-okta-client-0.1.7/okta_client/migrations/0002_alter_oktauser_options_alter_oktauser_managers_and_more.py
--rw-rw-rw-   0        0        0        0 2023-03-06 15:01:57.000000 django-okta-client-0.1.7/okta_client/migrations/__init__.py
--rw-rw-rw-   0        0        0     7115 2023-03-06 15:01:57.000000 django-okta-client-0.1.7/okta_client/models.py
-drwxrwxrwx   0        0        0        0 2023-03-21 17:38:23.285103 django-okta-client-0.1.7/okta_client/templates/
-drwxrwxrwx   0        0        0        0 2023-03-21 17:38:23.341632 django-okta-client-0.1.7/okta_client/templates/okta-client/
--rw-rw-rw-   0        0        0     4445 2023-03-06 15:01:57.000000 django-okta-client-0.1.7/okta_client/templates/okta-client/index.html
--rw-rw-rw-   0        0        0       63 2023-03-06 15:01:57.000000 django-okta-client-0.1.7/okta_client/tests.py
--rw-rw-rw-   0        0        0      286 2023-03-06 15:01:57.000000 django-okta-client-0.1.7/okta_client/urls.py
--rw-rw-rw-   0        0        0     5216 2023-03-06 15:01:57.000000 django-okta-client-0.1.7/okta_client/views.py
--rw-rw-rw-   0        0        0     1262 2023-03-21 17:38:10.000000 django-okta-client-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-21 17:38:23.345633 django-okta-client-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      208 2023-03-21 17:29:55.000000 django-okta-client-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:17:04.259855 django-okta-client-0.1.8/
+-rw-rw-rw-   0        0        0     1349 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     1084 2023-04-20 16:17:04.258854 django-okta-client-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2322 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 16:17:04.229331 django-okta-client-0.1.8/django_okta_client.egg-info/
+-rw-rw-rw-   0        0        0     1084 2023-04-20 16:17:04.000000 django-okta-client-0.1.8/django_okta_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2023-04-20 16:17:04.000000 django-okta-client-0.1.8/django_okta_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 16:17:04.000000 django-okta-client-0.1.8/django_okta_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-20 16:17:04.000000 django-okta-client-0.1.8/django_okta_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 16:17:04.000000 django-okta-client-0.1.8/django_okta_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 16:17:04.247876 django-okta-client-0.1.8/okta_client/
+-rw-rw-rw-   0        0        0      169 2023-04-20 16:15:09.000000 django-okta-client-0.1.8/okta_client/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-03-06 22:25:24.000000 django-okta-client-0.1.8/okta_client/admin.py
+-rw-rw-rw-   0        0        0      159 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/apps.py
+-rw-rw-rw-   0        0        0     1513 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/managers.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:17:04.254854 django-okta-client-0.1.8/okta_client/migrations/
+-rw-rw-rw-   0        0        0     6432 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     9555 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/migrations/0002_alter_oktauser_options_alter_oktauser_managers_and_more.py
+-rw-rw-rw-   0        0        0        0 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/migrations/__init__.py
+-rw-rw-rw-   0        0        0     7920 2023-04-20 16:05:38.000000 django-okta-client-0.1.8/okta_client/models.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:17:04.200314 django-okta-client-0.1.8/okta_client/templates/
+drwxrwxrwx   0        0        0        0 2023-04-20 16:17:04.256853 django-okta-client-0.1.8/okta_client/templates/okta-client/
+-rw-rw-rw-   0        0        0     4445 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/templates/okta-client/index.html
+-rw-rw-rw-   0        0        0       63 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/tests.py
+-rw-rw-rw-   0        0        0      286 2023-03-06 15:01:57.000000 django-okta-client-0.1.8/okta_client/urls.py
+-rw-rw-rw-   0        0        0     7046 2023-04-20 16:00:25.000000 django-okta-client-0.1.8/okta_client/views.py
+-rw-rw-rw-   0        0        0     1262 2023-03-21 17:38:10.000000 django-okta-client-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 16:17:04.261363 django-okta-client-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      208 2023-03-21 17:29:55.000000 django-okta-client-0.1.8/setup.py
```

### Comparing `django-okta-client-0.1.7/LICENSE` & `django-okta-client-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.7/PKG-INFO` & `django-okta-client-0.1.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-okta-client
-Version: 0.1.7
+Version: 0.1.8
 Summary: Okta client Django app
 Author-email: Irving Leonard <irvingleonard@gmail.com>
 License: BSD 2-Clause "Simplified" License
 Project-URL: homepage, https://github.com/irvingleonard/django-okta-client
 Project-URL: repository, https://github.com/irvingleonard/django-okta-client.git
 Keywords: okta,saml,saml2
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-okta-client-0.1.7/README.md` & `django-okta-client-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.7/django_okta_client.egg-info/PKG-INFO` & `django-okta-client-0.1.8/django_okta_client.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-okta-client
-Version: 0.1.7
+Version: 0.1.8
 Summary: Okta client Django app
 Author-email: Irving Leonard <irvingleonard@gmail.com>
 License: BSD 2-Clause "Simplified" License
 Project-URL: homepage, https://github.com/irvingleonard/django-okta-client
 Project-URL: repository, https://github.com/irvingleonard/django-okta-client.git
 Keywords: okta,saml,saml2
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-okta-client-0.1.7/django_okta_client.egg-info/SOURCES.txt` & `django-okta-client-0.1.8/django_okta_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.7/okta_client/admin.py` & `django-okta-client-0.1.8/okta_client/admin.py`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.7/okta_client/managers.py` & `django-okta-client-0.1.8/okta_client/managers.py`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.7/okta_client/migrations/0001_initial.py` & `django-okta-client-0.1.8/okta_client/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.7/okta_client/migrations/0002_alter_oktauser_options_alter_oktauser_managers_and_more.py` & `django-okta-client-0.1.8/okta_client/migrations/0002_alter_oktauser_options_alter_oktauser_managers_and_more.py`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.7/okta_client/models.py` & `django-okta-client-0.1.8/okta_client/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,27 +60,49 @@
 		verbose_name = _('okta user')
 		verbose_name_plural = _('okta users')
 		abstract = True
 	
 	def __str__(self):
 		return self.login
 	
+	@classmethod
+	def _attributes_from_okta_profile(cls, okta_profile):
+		attributes = {}
+		for field in cls._meta.fields:
+			if hasattr(okta_profile, field.name):
+				okta_attr = getattr(okta_profile, field.name)
+				if (okta_attr is None) or not len(okta_attr):
+					continue
+				if isinstance(field, models.fields.DateTimeField):
+					okta_attr = datetime.datetime.fromisoformat(okta_attr.rstrip('Z'))
+				attributes[field.name] = okta_attr
+		return attributes
+
+	@classmethod
+	def from_okta_profile(cls, okta_profile):
+		return cls(**cls._attributes_from_okta_profile(okta_profile))
+
 	def get_full_name(self):
 		if self.displayName:
 			return self.displayName
 		else:
 			components = ('honorificPrefix', 'firstName', 'middleName', 'lastName', 'honorificSuffix')
 			return ' '.join([getattr(self, component) for component in components if getattr(self, component)])
 
 	def get_short_name(self):
 		if self.nickName:
 			return self.nickName
 		else:
 			return self.firstName
 
+	def update_from_okta_profile(self, okta_profile):
+		for field_name, field_value in self._attributes_from_okta_profile(okta_profile).items():
+			setattr(self, field_name, field_value)
+		return self
+
 
 class OktaUser(AbstractOktaUser):
 	'''Django user model
 	Alternate user model for Django based on Okta profiles.
 	'''
 	
 	class Meta(AbstractOktaUser.Meta):
```

### Comparing `django-okta-client-0.1.7/okta_client/templates/okta-client/index.html` & `django-okta-client-0.1.8/okta_client/templates/okta-client/index.html`

 * *Files identical despite different names*

### Comparing `django-okta-client-0.1.7/pyproject.toml` & `django-okta-client-0.1.8/pyproject.toml`

 * *Files identical despite different names*

