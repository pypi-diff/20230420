# Comparing `tmp/notebook-logger-0.1.2.tar.gz` & `tmp/notebook-logger-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\notebook-logger-0.1.2.tar", last modified: Fri Apr 14 18:58:46 2023, max compression
+gzip compressed data, was "dist\notebook-logger-0.1.3.tar", last modified: Wed Apr 19 22:29:38 2023, max compression
```

## Comparing `notebook-logger-0.1.2.tar` & `notebook-logger-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 18:58:46.000000 notebook-logger-0.1.2/
--rw-rw-rw-   0        0        0    11558 2023-04-12 20:57:02.000000 notebook-logger-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      777 2023-04-14 18:58:46.000000 notebook-logger-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-14 18:56:58.000000 notebook-logger-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 18:58:46.000000 notebook-logger-0.1.2/notebook_logger/
--rw-rw-rw-   0        0        0       34 2023-04-12 21:08:00.000000 notebook-logger-0.1.2/notebook_logger/__init__.py
--rw-rw-rw-   0        0        0      611 2023-04-14 18:57:05.000000 notebook-logger-0.1.2/notebook_logger/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:58:46.000000 notebook-logger-0.1.2/notebook_logger.egg-info/
--rw-rw-rw-   0        0        0      777 2023-04-14 18:58:46.000000 notebook-logger-0.1.2/notebook_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-04-14 18:58:46.000000 notebook-logger-0.1.2/notebook_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 18:58:46.000000 notebook-logger-0.1.2/notebook_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-14 18:58:46.000000 notebook-logger-0.1.2/notebook_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-14 18:58:46.000000 notebook-logger-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      571 2023-04-14 18:56:44.000000 notebook-logger-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 22:29:38.000000 notebook-logger-0.1.3/
+-rw-rw-rw-   0        0        0    11558 2023-04-12 20:57:02.000000 notebook-logger-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      818 2023-04-19 22:29:38.000000 notebook-logger-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-19 22:26:49.000000 notebook-logger-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 22:29:38.000000 notebook-logger-0.1.3/notebook_logger/
+-rw-rw-rw-   0        0        0       34 2023-04-12 21:08:00.000000 notebook-logger-0.1.3/notebook_logger/__init__.py
+-rw-rw-rw-   0        0        0      608 2023-04-19 22:26:30.000000 notebook-logger-0.1.3/notebook_logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-19 22:29:38.000000 notebook-logger-0.1.3/notebook_logger.egg-info/
+-rw-rw-rw-   0        0        0      818 2023-04-19 22:29:38.000000 notebook-logger-0.1.3/notebook_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-04-19 22:29:38.000000 notebook-logger-0.1.3/notebook_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 22:29:38.000000 notebook-logger-0.1.3/notebook_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-19 22:29:38.000000 notebook-logger-0.1.3/notebook_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-19 22:29:38.000000 notebook-logger-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      698 2023-04-19 22:29:30.000000 notebook-logger-0.1.3/setup.py
```

### Comparing `notebook-logger-0.1.2/LICENSE` & `notebook-logger-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook-logger-0.1.2/notebook_logger/logger.py` & `notebook-logger-0.1.3/notebook_logger/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 class SimpleLogger:
 
     def __init__(self, filepath='notebook_msg.log', is_print=True):
         self.is_print = is_print
         logging.basicConfig(
             filename=filepath,
-            level=logging.INFO,
+            level=logging.WARN,
             format='%(asctime)s.%(msecs)03d || %(message)s',
             datefmt='%m/%d/%Y %H:%M:%S',
         )
 
     def set_print(self, is_print=True):
         self.is_print = is_print
 
-    def log(self, message, is_print=True):
+    def log(self, message, is_print=None):
         if (is_print) or (is_print is None and self.is_print):
-            is_print(message)
-        logging.info(message)
+            print(message)
+        logging.warn(message)
```

### Comparing `notebook-logger-0.1.2/setup.py` & `notebook-logger-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import setuptools
 
+with open('README.md', encoding='utf-8') as f:
+    long_description = f.read()
+
 setuptools.setup(
     name='notebook-logger',
-    version='0.1.2',
+    version='0.1.3',
     license='Apache-2.0',
     author='Daniel Lee',
     author_email='rootuser.kr@gmail.com',
     description='Simple logger for jupyter notebook user',
-    long_description=open('README.md').read(),
+    long_description=long_description,
     url='https://github.com/asulikeit/notebook-logger',
+    long_description_content_type='text/markdown',
     packages=['notebook_logger'],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent'
     ]
 )
```

