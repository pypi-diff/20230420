# Comparing `tmp/django-mapper-1.1.4.tar.gz` & `tmp/django-mapper-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mapper-1.1.4.tar", last modified: Wed Apr 19 08:00:25 2023, max compression
+gzip compressed data, was "django-mapper-1.1.5.tar", last modified: Thu Apr 20 04:23:53 2023, max compression
```

## Comparing `django-mapper-1.1.4.tar` & `django-mapper-1.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-19 08:00:25.461548 django-mapper-1.1.4/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-19 08:00:25.461548 django-mapper-1.1.4/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.4/README.md
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-19 08:00:25.457548 django-mapper-1.1.4/django_mapper/
--rw-r--r--   0 shubham   (1000) shubham   (1000)       30 2023-04-18 05:43:41.000000 django-mapper-1.1.4/django_mapper/__init__.py
--rw-r--r--   0 shubham   (1000) shubham   (1000)     4532 2023-04-19 07:59:30.000000 django-mapper-1.1.4/django_mapper/mapper.py
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-19 08:00:25.461548 django-mapper-1.1.4/django_mapper.egg-info/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-19 08:00:25.000000 django-mapper-1.1.4/django_mapper.egg-info/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-19 08:00:25.000000 django-mapper-1.1.4/django_mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-19 08:00:25.000000 django-mapper-1.1.4/django_mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-19 08:00:25.000000 django-mapper-1.1.4/django_mapper.egg-info/requires.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-19 08:00:25.000000 django-mapper-1.1.4/django_mapper.egg-info/top_level.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-19 08:00:25.461548 django-mapper-1.1.4/setup.cfg
--rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-19 07:59:46.000000 django-mapper-1.1.4/setup.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-20 04:23:53.912669 django-mapper-1.1.5/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-20 04:23:53.912669 django-mapper-1.1.5/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.5/README.md
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-20 04:23:53.912669 django-mapper-1.1.5/django_mapper/
+-rw-r--r--   0 shubham   (1000) shubham   (1000)       30 2023-04-18 05:43:41.000000 django-mapper-1.1.5/django_mapper/__init__.py
+-rw-r--r--   0 shubham   (1000) shubham   (1000)     4713 2023-04-20 04:23:33.000000 django-mapper-1.1.5/django_mapper/mapper.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-20 04:23:53.912669 django-mapper-1.1.5/django_mapper.egg-info/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-20 04:23:53.000000 django-mapper-1.1.5/django_mapper.egg-info/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-20 04:23:53.000000 django-mapper-1.1.5/django_mapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-20 04:23:53.000000 django-mapper-1.1.5/django_mapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-20 04:23:53.000000 django-mapper-1.1.5/django_mapper.egg-info/requires.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-20 04:23:53.000000 django-mapper-1.1.5/django_mapper.egg-info/top_level.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-20 04:23:53.912669 django-mapper-1.1.5/setup.cfg
+-rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-20 04:17:10.000000 django-mapper-1.1.5/setup.py
```

### Comparing `django-mapper-1.1.4/PKG-INFO` & `django-mapper-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.4
+Version: 1.1.5
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.4/django_mapper/mapper.py` & `django-mapper-1.1.5/django_mapper/mapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class DataMapper:
     def __init__(self, config, target_model=None, enable_logging=False):
         self.config = config
         self.target_model = target_model
         self.enable_logging = enable_logging
         self.logger = logging.getLogger(__name__)
     
-    def map_data(self, data):
+    def map_data(self, data, default_values={}):
         mapped_data = {}
         for mapping in self.config:
             to_field = mapping.get('to_field')
             
             from_field = mapping.get('from_field')
             default_value = mapping.get('default_value')
 
@@ -34,16 +34,19 @@
 
             elif compute_method:
                 value = compute_method(data)
                 mapped_data = self.set_value(mapped_data, to_field, value)
             else:
                 raise ValueError("from_field or compute_method should be provided")
 
+        if default_values:
+            mapped_data.update(default_values)
+
         if self.target_model:
-            instance = self.create_instance(self.target_model, mapped_data)
+            instance = self.create_instance(self.target_model, mapped_data, default_values=default_values)
             self.logger.info(f"Created instance of {self.target_model.__name__}")
             return instance
         else:
             return mapped_data
     
     def get_value(self, data, field, mapper=None):
         current_data = data
@@ -60,29 +63,29 @@
                 m2m_mapper = DataMapper(self.config, target_model=self.target_model, enable_logging=self.enable_logging)
             elif isinstance(mapper, dict):
                 m2m_mapper = DataMapper(self.config, enable_logging=self.enable_logging)
             else:
                 m2m_mapper = mapper
             
             for m2m_instance in unserialized_data:
-                serialized_instance = m2m_mapper.map_data(m2m_instance)
+                serialized_instance = m2m_mapper.map_data(m2m_instance, )
                 current_data.append(serialized_instance)
 
         return current_data
     
     def set_value(self, data, field, value):
         fields = field.split('__')
         for f in fields[:-1]:
             if f not in data:
                 data[f] = {}
             data = data[f]
         data[fields[-1]] = value
         return data
     
-    def create_instance(self, model, data):
+    def create_instance(self, model, data, default_values={}):
         instance_kwargs = {}
         m2m_fields = {}
         for key, value in data.items():
             if isinstance(value, dict):
                 field = model._meta.get_field(key)
                 related_model = field.related_model
 
@@ -101,18 +104,19 @@
                         m2m_fields[key].append(single_value)
                     else:
                         m2m_fields[key] = [single_value]
 
             else:
                 instance_kwargs[key] = value
         
+        instance_kwargs.update(default_values)
         instance = model.objects.create(**instance_kwargs)
 
         save_again =  False
         for m2m_field in m2m_fields:
             getattr(instance, m2m_field).add(**m2m_fields[m2m_field])
             save_again = True
 
         if save_again:
             instance.save()
-            
+
         return instance
```

### Comparing `django-mapper-1.1.4/django_mapper.egg-info/PKG-INFO` & `django-mapper-1.1.5/django_mapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.4
+Version: 1.1.5
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.4/setup.py` & `django-mapper-1.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-mapper',
-    version='1.1.4',
+    version='1.1.5',
     description='A utility class for mapping data between Django models',
     author='Shubham Vashisht',
     author_email='shubhvas95@gmail.com',
     url='https://github.com/shubh95/django-mapper',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

