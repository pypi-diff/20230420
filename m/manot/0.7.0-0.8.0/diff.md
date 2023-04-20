# Comparing `tmp/manot-0.7.0.tar.gz` & `tmp/manot-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manot-0.7.0.tar", last modified: Mon Mar 13 15:52:06 2023, max compression
+gzip compressed data, was "manot-0.8.0.tar", last modified: Thu Apr 20 08:22:38 2023, max compression
```

## Comparing `manot-0.7.0.tar` & `manot-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kostya     (501) staff       (20)        0 2023-03-13 15:52:06.313663 manot-0.7.0/
--rw-r--r--   0 kostya     (501) staff       (20)     1061 2022-12-19 07:28:46.000000 manot-0.7.0/LICENSE
--rw-r--r--   0 kostya     (501) staff       (20)     6655 2023-03-13 15:52:06.313535 manot-0.7.0/PKG-INFO
--rw-r--r--   0 kostya     (501) staff       (20)     5691 2023-03-13 15:47:14.000000 manot-0.7.0/README.md
-drwxr-xr-x   0 kostya     (501) staff       (20)        0 2023-03-13 15:52:06.312386 manot-0.7.0/manot.egg-info/
--rw-r--r--   0 kostya     (501) staff       (20)     6655 2023-03-13 15:52:06.000000 manot-0.7.0/manot.egg-info/PKG-INFO
--rw-r--r--   0 kostya     (501) staff       (20)      274 2023-03-13 15:52:06.000000 manot-0.7.0/manot.egg-info/SOURCES.txt
--rw-r--r--   0 kostya     (501) staff       (20)        1 2023-03-13 15:52:06.000000 manot-0.7.0/manot.egg-info/dependency_links.txt
--rw-r--r--   0 kostya     (501) staff       (20)       59 2023-03-13 15:52:06.000000 manot-0.7.0/manot.egg-info/requires.txt
--rw-r--r--   0 kostya     (501) staff       (20)        6 2023-03-13 15:52:06.000000 manot-0.7.0/manot.egg-info/top_level.txt
--rw-r--r--   0 kostya     (501) staff       (20)     1074 2023-03-13 15:37:51.000000 manot-0.7.0/pyproject.toml
--rw-r--r--   0 kostya     (501) staff       (20)       38 2023-03-13 15:52:06.313700 manot-0.7.0/setup.cfg
--rw-r--r--   0 kostya     (501) staff       (20)      816 2023-03-13 15:37:51.000000 manot-0.7.0/setup.py
-drwxr-xr-x   0 kostya     (501) staff       (20)        0 2023-03-13 15:52:06.311245 manot-0.7.0/src/
-drwxr-xr-x   0 kostya     (501) staff       (20)        0 2023-03-13 15:52:06.313376 manot-0.7.0/src/manot/
--rw-r--r--   0 kostya     (501) staff       (20)       78 2023-01-30 16:07:05.000000 manot-0.7.0/src/manot/__init__.py
--rw-r--r--   0 kostya     (501) staff       (20)     1358 2023-01-30 16:07:05.000000 manot-0.7.0/src/manot/logger.py
--rw-r--r--   0 kostya     (501) staff       (20)    10044 2023-03-13 15:42:09.000000 manot-0.7.0/src/manot/manot.py
--rw-r--r--   0 kostya     (501) staff       (20)     4890 2023-03-13 15:36:01.000000 manot-0.7.0/src/manot/upload_manager.py
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-04-20 08:22:38.917274 manot-0.8.0/
+-rw-rw-r--   0 armen     (1000) armen     (1000)     1061 2023-02-14 12:07:02.000000 manot-0.8.0/LICENSE
+-rw-rw-r--   0 armen     (1000) armen     (1000)     7041 2023-04-20 08:22:38.917274 manot-0.8.0/PKG-INFO
+-rw-rw-r--   0 armen     (1000) armen     (1000)     6077 2023-04-20 08:17:39.000000 manot-0.8.0/README.md
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-04-20 08:22:38.917274 manot-0.8.0/manot.egg-info/
+-rw-rw-r--   0 armen     (1000) armen     (1000)     7041 2023-04-20 08:22:38.000000 manot-0.8.0/manot.egg-info/PKG-INFO
+-rw-rw-r--   0 armen     (1000) armen     (1000)      274 2023-04-20 08:22:38.000000 manot-0.8.0/manot.egg-info/SOURCES.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)        1 2023-04-20 08:22:38.000000 manot-0.8.0/manot.egg-info/dependency_links.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)       59 2023-04-20 08:22:38.000000 manot-0.8.0/manot.egg-info/requires.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)        6 2023-04-20 08:22:38.000000 manot-0.8.0/manot.egg-info/top_level.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)     1074 2023-04-20 08:18:27.000000 manot-0.8.0/pyproject.toml
+-rw-rw-r--   0 armen     (1000) armen     (1000)       38 2023-04-20 08:22:38.917274 manot-0.8.0/setup.cfg
+-rw-rw-r--   0 armen     (1000) armen     (1000)      816 2023-04-20 08:18:27.000000 manot-0.8.0/setup.py
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-04-20 08:22:38.913274 manot-0.8.0/src/
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-04-20 08:22:38.917274 manot-0.8.0/src/manot/
+-rw-rw-r--   0 armen     (1000) armen     (1000)       78 2023-02-14 12:07:02.000000 manot-0.8.0/src/manot/__init__.py
+-rw-rw-r--   0 armen     (1000) armen     (1000)     1358 2023-02-14 12:07:02.000000 manot-0.8.0/src/manot/logger.py
+-rw-rw-r--   0 armen     (1000) armen     (1000)    11604 2023-04-18 10:27:49.000000 manot-0.8.0/src/manot/manot.py
+-rw-rw-r--   0 armen     (1000) armen     (1000)     4890 2023-04-17 14:43:30.000000 manot-0.8.0/src/manot/upload_manager.py
```

### Comparing `manot-0.7.0/LICENSE` & `manot-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manot-0.7.0/PKG-INFO` & `manot-0.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manot
-Version: 0.7.0
+Version: 0.8.0
 Summary: manot AI is a model observability platform to monitor computer vision performance in real-time.
 Home-page: https://www.manot.ai
 Author: manot
 Author-email: manot <engineering@manot.ai>
 License: MIT
 Project-URL: Homepage, https://www.manot.ai
 Project-URL: Documentation, https://api.manot.ai/api-documentation/v1
@@ -33,15 +33,15 @@
 Using our SDK you can quickly set up your project by defining a few key parameters, including the paths to your data,
 classes and model. Once the project is set up you will be able to use the insight method to extract outliers that manot
 has detected on the new unstructured data that the performance of the model is evaluated on.
 
 Installation
 ------------
 
-Install manot with `pip`:
+Install manot using `pip`:
 
     pip install manot
 
 Example
 -------
 
 This is an example how to start:
@@ -49,17 +49,22 @@
 ```python
 from manot import manotAI
 
 manot = manotAI("manot_service_url", "token")
 ```
 
 ```python
+# Upload data to manot manager S3 bucket for Setup. The data should be in YOLO format
+manot.upload_data(dir_path="/path/to/data", process="setup")
+```
+
+```python
 # Setup process for "local" and "s3" providers
 setup = manot.setup(
-    data_provider="local", # it must be "s3" or "local"
+    data_provider="s3", # it must be "s3" or "local"
     arguments={
             "name": "setup_example",
             "images_path": "/path/to/images",
             "ground_truths_path": "/path/to/ground_truths",
             "detections_path": "/path/to/detections",
             "detections_metadata_format": "xyx2y2",  # it must be one of "xyx2y2", "xywh", or "cxcywh"
             "classes_txt_path": "/path/to/classes.txt",
@@ -92,19 +97,24 @@
 # {"id": setup_id, "name": "setup_example", "status": "started"}
 
 setup_info = manot.get_setup(setup["id"])
 # when setup is successfully finished, then setup_info is {"id": setup_id, "name": "setup_example", "status": "started"}
 ```
 
 ```python
+# Upload data to manot manager S3 bucket to get insights
+manot.upload_data(dir_path="/path/to/data", process="insight")
+```
+
+```python
 insight = manot.insight(
     name="insight_example",
     setup_id=setup["id"],
     data_path="/path/to/data",
-    data_provider="local",  # it must be "s3" or "local"
+    data_provider="s3",  # it must be "s3" or "local"
     percentage="percentage" # percentage of images to be considered insight should be larger than 0 and less or equal than 100
 )
 print(insight)
 # {"id": insight_id, "name": "insight_example", "status": "started"}
 
 insight_info = manot.get_insight(insight["id"])
 # when setup is successfully finished, then insight_info is {"id": insight_id, "name": "setup_example", "status": "started"}
@@ -114,15 +124,16 @@
 scores = manot.get_score(insight['id'])
 #returns list of all processed images graded by their score from 0 to 10 (higher is more impactful image)
 # if the image cannot be assigned a score it will not be showing in the list 
 ```
 
 ```python
 #in case of deeplake please also provide deeplake token 
-manot.visualize_data_set(insight_info['data_set']['id'], deeplake_token)
+manot.visualize_data_set(insight_info['data_set']['id'], deeplake_token,group_similar=True)
+# if group similar is set to True(default) will only return unique images 
 ```
 
 ```python
 # Upload data for Setup or Insights process
 manot.upload_data(dir_path="/path/to/data", process="process_name")
 ```
 For Setup process
```

### Comparing `manot-0.7.0/README.md` & `manot-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Using our SDK you can quickly set up your project by defining a few key parameters, including the paths to your data,
 classes and model. Once the project is set up you will be able to use the insight method to extract outliers that manot
 has detected on the new unstructured data that the performance of the model is evaluated on.
 
 Installation
 ------------
 
-Install manot with `pip`:
+Install manot using `pip`:
 
     pip install manot
 
 Example
 -------
 
 This is an example how to start:
@@ -25,17 +25,22 @@
 ```python
 from manot import manotAI
 
 manot = manotAI("manot_service_url", "token")
 ```
 
 ```python
+# Upload data to manot manager S3 bucket for Setup. The data should be in YOLO format
+manot.upload_data(dir_path="/path/to/data", process="setup")
+```
+
+```python
 # Setup process for "local" and "s3" providers
 setup = manot.setup(
-    data_provider="local", # it must be "s3" or "local"
+    data_provider="s3", # it must be "s3" or "local"
     arguments={
             "name": "setup_example",
             "images_path": "/path/to/images",
             "ground_truths_path": "/path/to/ground_truths",
             "detections_path": "/path/to/detections",
             "detections_metadata_format": "xyx2y2",  # it must be one of "xyx2y2", "xywh", or "cxcywh"
             "classes_txt_path": "/path/to/classes.txt",
@@ -68,19 +73,24 @@
 # {"id": setup_id, "name": "setup_example", "status": "started"}
 
 setup_info = manot.get_setup(setup["id"])
 # when setup is successfully finished, then setup_info is {"id": setup_id, "name": "setup_example", "status": "started"}
 ```
 
 ```python
+# Upload data to manot manager S3 bucket to get insights
+manot.upload_data(dir_path="/path/to/data", process="insight")
+```
+
+```python
 insight = manot.insight(
     name="insight_example",
     setup_id=setup["id"],
     data_path="/path/to/data",
-    data_provider="local",  # it must be "s3" or "local"
+    data_provider="s3",  # it must be "s3" or "local"
     percentage="percentage" # percentage of images to be considered insight should be larger than 0 and less or equal than 100
 )
 print(insight)
 # {"id": insight_id, "name": "insight_example", "status": "started"}
 
 insight_info = manot.get_insight(insight["id"])
 # when setup is successfully finished, then insight_info is {"id": insight_id, "name": "setup_example", "status": "started"}
@@ -90,15 +100,16 @@
 scores = manot.get_score(insight['id'])
 #returns list of all processed images graded by their score from 0 to 10 (higher is more impactful image)
 # if the image cannot be assigned a score it will not be showing in the list 
 ```
 
 ```python
 #in case of deeplake please also provide deeplake token 
-manot.visualize_data_set(insight_info['data_set']['id'], deeplake_token)
+manot.visualize_data_set(insight_info['data_set']['id'], deeplake_token,group_similar=True)
+# if group similar is set to True(default) will only return unique images 
 ```
 
 ```python
 # Upload data for Setup or Insights process
 manot.upload_data(dir_path="/path/to/data", process="process_name")
 ```
 For Setup process
```

### Comparing `manot-0.7.0/manot.egg-info/PKG-INFO` & `manot-0.8.0/manot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manot
-Version: 0.7.0
+Version: 0.8.0
 Summary: manot AI is a model observability platform to monitor computer vision performance in real-time.
 Home-page: https://www.manot.ai
 Author: manot
 Author-email: manot <engineering@manot.ai>
 License: MIT
 Project-URL: Homepage, https://www.manot.ai
 Project-URL: Documentation, https://api.manot.ai/api-documentation/v1
@@ -33,15 +33,15 @@
 Using our SDK you can quickly set up your project by defining a few key parameters, including the paths to your data,
 classes and model. Once the project is set up you will be able to use the insight method to extract outliers that manot
 has detected on the new unstructured data that the performance of the model is evaluated on.
 
 Installation
 ------------
 
-Install manot with `pip`:
+Install manot using `pip`:
 
     pip install manot
 
 Example
 -------
 
 This is an example how to start:
@@ -49,17 +49,22 @@
 ```python
 from manot import manotAI
 
 manot = manotAI("manot_service_url", "token")
 ```
 
 ```python
+# Upload data to manot manager S3 bucket for Setup. The data should be in YOLO format
+manot.upload_data(dir_path="/path/to/data", process="setup")
+```
+
+```python
 # Setup process for "local" and "s3" providers
 setup = manot.setup(
-    data_provider="local", # it must be "s3" or "local"
+    data_provider="s3", # it must be "s3" or "local"
     arguments={
             "name": "setup_example",
             "images_path": "/path/to/images",
             "ground_truths_path": "/path/to/ground_truths",
             "detections_path": "/path/to/detections",
             "detections_metadata_format": "xyx2y2",  # it must be one of "xyx2y2", "xywh", or "cxcywh"
             "classes_txt_path": "/path/to/classes.txt",
@@ -92,19 +97,24 @@
 # {"id": setup_id, "name": "setup_example", "status": "started"}
 
 setup_info = manot.get_setup(setup["id"])
 # when setup is successfully finished, then setup_info is {"id": setup_id, "name": "setup_example", "status": "started"}
 ```
 
 ```python
+# Upload data to manot manager S3 bucket to get insights
+manot.upload_data(dir_path="/path/to/data", process="insight")
+```
+
+```python
 insight = manot.insight(
     name="insight_example",
     setup_id=setup["id"],
     data_path="/path/to/data",
-    data_provider="local",  # it must be "s3" or "local"
+    data_provider="s3",  # it must be "s3" or "local"
     percentage="percentage" # percentage of images to be considered insight should be larger than 0 and less or equal than 100
 )
 print(insight)
 # {"id": insight_id, "name": "insight_example", "status": "started"}
 
 insight_info = manot.get_insight(insight["id"])
 # when setup is successfully finished, then insight_info is {"id": insight_id, "name": "setup_example", "status": "started"}
@@ -114,15 +124,16 @@
 scores = manot.get_score(insight['id'])
 #returns list of all processed images graded by their score from 0 to 10 (higher is more impactful image)
 # if the image cannot be assigned a score it will not be showing in the list 
 ```
 
 ```python
 #in case of deeplake please also provide deeplake token 
-manot.visualize_data_set(insight_info['data_set']['id'], deeplake_token)
+manot.visualize_data_set(insight_info['data_set']['id'], deeplake_token,group_similar=True)
+# if group similar is set to True(default) will only return unique images 
 ```
 
 ```python
 # Upload data for Setup or Insights process
 manot.upload_data(dir_path="/path/to/data", process="process_name")
 ```
 For Setup process
```

### Comparing `manot-0.7.0/pyproject.toml` & `manot-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "manot"
-version = "0.7.0"
+version = "0.8.0"
 authors = [
     { name = "manot", email = "engineering@manot.ai" },
 ]
 license = {text = "MIT"}
 description = "manot AI is a model observability platform to monitor computer vision performance in real-time."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `manot-0.7.0/setup.py` & `manot-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
 setup(
     name='manot',
-    version='0.7.0',
+    version='0.8.0',
     description='The manot SDK is a wrapper on top of our API to make it easier to work with our model performance monitoring system. Using our SDK you can quickly set up your project by defining a few key parameters, including the paths to your data, classes and model. Once the project is set up you will be able to use the insight method to extract outliers that manot has detected on the new unstructured data that the performance of the model is evaluated on.',
     author='manot',
     author_email='engineering@manot.ai',
     url='https://www.manot.ai',
     packages=['manot'],
     package_dir={'manot': 'src/manot'},
     project_urls={
```

### Comparing `manot-0.7.0/src/manot/logger.py` & `manot-0.8.0/src/manot/logger.py`

 * *Files identical despite different names*

### Comparing `manot-0.7.0/src/manot/manot.py` & `manot-0.8.0/src/manot/manot.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,54 @@
             else:
                 log.error(f'There is problem setup process with id {response.json()["id"]}.')
                 return False
 
         log.error(response.text)
         return False
 
+    def huggingface_insight(
+            self,
+            name: str,
+            data_path: str,
+            task: Optional[Literal['classification', 'segmentation', 'detection']] = 'detection',
+            percentage: Optional[float] = None,
+            model_path: Optional[str] = None,
+
+    ) -> Union[bool, dict]:
+
+        url = f"{self.__url}/api/v1/insight/huggingface"
+        data = {
+            "name": name,
+            "data_path": data_path,
+            "model_path": model_path,
+            "task": task,
+            "percentage": percentage
+        }
+        try:
+            response = requests.post(url=url, data=json.dumps(data), headers={"token": self.__token})
+        except Exception:
+            log.error("There is problem with request.")
+            return False
+
+        if response.status_code == 202:
+            log.info("Insight process is being prepared to be started.")
+            progress_result = self.__check_progress(self.get_insight, response.json()["id"])
+            if progress_result:
+                if progress_result['status'] == "finished":
+                    log.info("Insight process has successfully finished.")
+                elif progress_result['status'] == "failure":
+                    log.error(f'There is problem insight process with id {response.json()["id"]}.')
+                return progress_result
+            else:
+                log.error(f'There is problem insight process with id {response.json()["id"]}.')
+                return False
+
+        log.error(response.text)
+        return False
+
     def get_setup(self, setup_id: int) -> Union[bool, None, dict]:
 
         url = f"{self.__url}/api/v1/setup/{setup_id}"
 
         try:
             response = requests.get(url=url)
         except Exception:
@@ -94,15 +134,14 @@
             return False
 
         if response.status_code != 200:
             log.warning("Setup not found.")
             return None
 
         return response.json()
-
     def insight(
             self,
             name: str,
             setup_id: int,
             data_path: Union[str, List[str]],
             data_provider: Literal['s3', 'local', 'deeplake'],
             weight_name: Optional[str] = None,
@@ -139,15 +178,14 @@
                 return progress_result
             else:
                 log.error(f'There is problem insight process with id {response.json()["id"]}.')
                 return False
 
         log.error(response.text)
         return False
-
     def get_insight(self, insight_id: int) -> Union[bool, None, dict]:
 
         url = f"{self.__url}/api/v1/insight/{insight_id}"
 
         try:
             response = requests.get(url=url)
         except Exception:
```

### Comparing `manot-0.7.0/src/manot/upload_manager.py` & `manot-0.8.0/src/manot/upload_manager.py`

 * *Files identical despite different names*

