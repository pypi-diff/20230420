# Comparing `tmp/django-mapper-1.1.6.tar.gz` & `tmp/django-mapper-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mapper-1.1.6.tar", last modified: Thu Apr 20 06:49:29 2023, max compression
+gzip compressed data, was "django-mapper-1.1.7.tar", last modified: Thu Apr 20 07:15:56 2023, max compression
```

## Comparing `django-mapper-1.1.6.tar` & `django-mapper-1.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-20 06:49:29.014880 django-mapper-1.1.6/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-20 06:49:29.010880 django-mapper-1.1.6/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.6/README.md
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-20 06:49:29.010880 django-mapper-1.1.6/django_mapper/
--rw-r--r--   0 shubham   (1000) shubham   (1000)       30 2023-04-18 05:43:41.000000 django-mapper-1.1.6/django_mapper/__init__.py
--rw-r--r--   0 shubham   (1000) shubham   (1000)     4789 2023-04-20 06:48:50.000000 django-mapper-1.1.6/django_mapper/mapper.py
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-20 06:49:29.010880 django-mapper-1.1.6/django_mapper.egg-info/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-20 06:49:28.000000 django-mapper-1.1.6/django_mapper.egg-info/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-20 06:49:28.000000 django-mapper-1.1.6/django_mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-20 06:49:28.000000 django-mapper-1.1.6/django_mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-20 06:49:28.000000 django-mapper-1.1.6/django_mapper.egg-info/requires.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-20 06:49:28.000000 django-mapper-1.1.6/django_mapper.egg-info/top_level.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-20 06:49:29.014880 django-mapper-1.1.6/setup.cfg
--rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-20 06:48:57.000000 django-mapper-1.1.6/setup.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-20 07:15:56.633073 django-mapper-1.1.7/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-20 07:15:56.633073 django-mapper-1.1.7/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.7/README.md
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-20 07:15:56.633073 django-mapper-1.1.7/django_mapper/
+-rw-r--r--   0 shubham   (1000) shubham   (1000)       30 2023-04-18 05:43:41.000000 django-mapper-1.1.7/django_mapper/__init__.py
+-rw-r--r--   0 shubham   (1000) shubham   (1000)     4788 2023-04-20 07:08:54.000000 django-mapper-1.1.7/django_mapper/mapper.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-20 07:15:56.633073 django-mapper-1.1.7/django_mapper.egg-info/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-20 07:15:56.000000 django-mapper-1.1.7/django_mapper.egg-info/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-20 07:15:56.000000 django-mapper-1.1.7/django_mapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-20 07:15:56.000000 django-mapper-1.1.7/django_mapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-20 07:15:56.000000 django-mapper-1.1.7/django_mapper.egg-info/requires.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-20 07:15:56.000000 django-mapper-1.1.7/django_mapper.egg-info/top_level.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-20 07:15:56.633073 django-mapper-1.1.7/setup.cfg
+-rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-20 07:13:01.000000 django-mapper-1.1.7/setup.py
```

### Comparing `django-mapper-1.1.6/PKG-INFO` & `django-mapper-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.6
+Version: 1.1.7
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.6/django_mapper/mapper.py` & `django-mapper-1.1.7/django_mapper/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,14 @@
                 instance_kwargs[key] = value
         
         instance_kwargs.update(default_values)
         instance = model.objects.create(**instance_kwargs)
 
         save_again =  False
         for m2m_field in m2m_fields:
-            getattr(instance, m2m_field).add(**m2m_fields[m2m_field])
+            getattr(instance, m2m_field).add(*m2m_fields[m2m_field])
             save_again = True
 
         if save_again:
             instance.save()
 
         return instance
```

### Comparing `django-mapper-1.1.6/django_mapper.egg-info/PKG-INFO` & `django-mapper-1.1.7/django_mapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.6
+Version: 1.1.7
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.6/setup.py` & `django-mapper-1.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-mapper',
-    version='1.1.6',
+    version='1.1.7',
     description='A utility class for mapping data between Django models',
     author='Shubham Vashisht',
     author_email='shubhvas95@gmail.com',
     url='https://github.com/shubh95/django-mapper',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

