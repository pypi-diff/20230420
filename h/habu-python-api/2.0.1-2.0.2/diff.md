# Comparing `tmp/habu-python-api-2.0.1.tar.gz` & `tmp/habu-python-api-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/roopakgupta/habu/habu-api/dist/.tmp-yrlaz99p/habu-python-api-2.0.1.tar", last modified: Thu Feb 16 17:37:17 2023, max compression
+gzip compressed data, was "/Users/roopakgupta/habu/habu-api/dist/.tmp-hcdkvtns/habu-python-api-2.0.2.tar", last modified: Thu Apr 20 03:56:18 2023, max compression
```

## Comparing `habu-python-api-2.0.1.tar` & `habu-python-api-2.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-02-16 17:37:17.093599 habu-python-api-2.0.1/
--rw-r--r--   0 roopakgupta   (501) staff       (20)      563 2023-02-16 17:37:17.092731 habu-python-api-2.0.1/PKG-INFO
--rw-r--r--   0 roopakgupta   (501) staff       (20)      145 2021-09-13 19:52:09.000000 habu-python-api-2.0.1/README.md
--rw-r--r--   0 roopakgupta   (501) staff       (20)      133 2021-09-13 19:52:09.000000 habu-python-api-2.0.1/pyproject.toml
--rw-r--r--   0 roopakgupta   (501) staff       (20)       38 2023-02-16 17:37:17.093788 habu-python-api-2.0.1/setup.cfg
--rw-r--r--   0 roopakgupta   (501) staff       (20)      739 2023-02-16 17:33:16.000000 habu-python-api-2.0.1/setup.py
-drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-02-16 17:37:17.081888 habu-python-api-2.0.1/src/
-drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-02-16 17:37:17.087187 habu-python-api-2.0.1/src/habu_api/
--rw-r--r--   0 roopakgupta   (501) staff       (20)        0 2021-09-13 19:52:09.000000 habu-python-api-2.0.1/src/habu_api/__init__.py
--rw-r--r--   0 roopakgupta   (501) staff       (20)     3444 2023-02-16 17:33:16.000000 habu-python-api-2.0.1/src/habu_api/cleanRoom.py
-drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-02-16 17:37:17.091511 habu-python-api-2.0.1/src/habu_python_api.egg-info/
--rw-r--r--   0 roopakgupta   (501) staff       (20)      563 2023-02-16 17:37:17.000000 habu-python-api-2.0.1/src/habu_python_api.egg-info/PKG-INFO
--rw-r--r--   0 roopakgupta   (501) staff       (20)      256 2023-02-16 17:37:17.000000 habu-python-api-2.0.1/src/habu_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 roopakgupta   (501) staff       (20)        1 2023-02-16 17:37:17.000000 habu-python-api-2.0.1/src/habu_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 roopakgupta   (501) staff       (20)        9 2023-02-16 17:37:17.000000 habu-python-api-2.0.1/src/habu_python_api.egg-info/top_level.txt
+drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-04-20 03:56:18.929182 habu-python-api-2.0.2/
+-rw-r--r--   0 roopakgupta   (501) staff       (20)      880 2023-04-20 03:56:18.928636 habu-python-api-2.0.2/PKG-INFO
+-rw-r--r--   0 roopakgupta   (501) staff       (20)      463 2023-02-23 23:56:27.000000 habu-python-api-2.0.2/README.md
+-rw-r--r--   0 roopakgupta   (501) staff       (20)      133 2021-09-13 19:52:09.000000 habu-python-api-2.0.2/pyproject.toml
+-rw-r--r--   0 roopakgupta   (501) staff       (20)       38 2023-04-20 03:56:18.929333 habu-python-api-2.0.2/setup.cfg
+-rw-r--r--   0 roopakgupta   (501) staff       (20)      739 2023-04-20 03:55:36.000000 habu-python-api-2.0.2/setup.py
+drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-04-20 03:56:18.920796 habu-python-api-2.0.2/src/
+drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-04-20 03:56:18.924456 habu-python-api-2.0.2/src/habu_api/
+-rw-r--r--   0 roopakgupta   (501) staff       (20)        0 2021-09-13 19:52:09.000000 habu-python-api-2.0.2/src/habu_api/__init__.py
+-rw-r--r--   0 roopakgupta   (501) staff       (20)     3606 2023-04-20 03:55:36.000000 habu-python-api-2.0.2/src/habu_api/cleanRoom.py
+drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-04-20 03:56:18.927894 habu-python-api-2.0.2/src/habu_python_api.egg-info/
+-rw-r--r--   0 roopakgupta   (501) staff       (20)      880 2023-04-20 03:56:18.000000 habu-python-api-2.0.2/src/habu_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 roopakgupta   (501) staff       (20)      256 2023-04-20 03:56:18.000000 habu-python-api-2.0.2/src/habu_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 roopakgupta   (501) staff       (20)        1 2023-04-20 03:56:18.000000 habu-python-api-2.0.2/src/habu_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 roopakgupta   (501) staff       (20)        9 2023-04-20 03:56:18.000000 habu-python-api-2.0.2/src/habu_python_api.egg-info/top_level.txt
```

### Comparing `habu-python-api-2.0.1/setup.py` & `habu-python-api-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="habu-python-api",
-    version="2.0.1",
+    version="2.0.2",
     author="Habu",
     author_email="support@habu.com",
     description="Habu Python API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deklareddotcom/habu-api",
     project_urls={
```

### Comparing `habu-python-api-2.0.1/src/habu_api/cleanRoom.py` & `habu-python-api-2.0.2/src/habu_api/cleanRoom.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,7 +83,11 @@
     def get_question_runs(self, question_uuid, limit=500, offset=0):
         return self.get("%s/v1/cleanroom-questions/%s/cleanroom-question-runs?limit=%s&offset=%s"
                         % (self.api, question_uuid, limit, offset))
 
     def get_question_run_data(self, run_uuid, limit=500, offset=0):
         return self.get("%s/v1/cleanroom-question-runs/%s/data?limit=%s&offset=%s"
                         % (self.api, run_uuid, limit, offset))
+
+    def get_run_data_count(self, run_uuid):
+        return self.get("%s/v1/cleanroom-question-runs/%s/data/count"
+                        % (self.api, run_uuid))
```

