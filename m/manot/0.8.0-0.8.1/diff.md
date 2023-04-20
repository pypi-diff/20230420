# Comparing `tmp/manot-0.8.0.tar.gz` & `tmp/manot-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manot-0.8.0.tar", last modified: Thu Apr 20 08:22:38 2023, max compression
+gzip compressed data, was "manot-0.8.1.tar", last modified: Thu Apr 20 08:49:23 2023, max compression
```

## Comparing `manot-0.8.0.tar` & `manot-0.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-04-20 08:22:38.917274 manot-0.8.0/
--rw-rw-r--   0 armen     (1000) armen     (1000)     1061 2023-02-14 12:07:02.000000 manot-0.8.0/LICENSE
--rw-rw-r--   0 armen     (1000) armen     (1000)     7041 2023-04-20 08:22:38.917274 manot-0.8.0/PKG-INFO
--rw-rw-r--   0 armen     (1000) armen     (1000)     6077 2023-04-20 08:17:39.000000 manot-0.8.0/README.md
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-04-20 08:22:38.917274 manot-0.8.0/manot.egg-info/
--rw-rw-r--   0 armen     (1000) armen     (1000)     7041 2023-04-20 08:22:38.000000 manot-0.8.0/manot.egg-info/PKG-INFO
--rw-rw-r--   0 armen     (1000) armen     (1000)      274 2023-04-20 08:22:38.000000 manot-0.8.0/manot.egg-info/SOURCES.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)        1 2023-04-20 08:22:38.000000 manot-0.8.0/manot.egg-info/dependency_links.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)       59 2023-04-20 08:22:38.000000 manot-0.8.0/manot.egg-info/requires.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)        6 2023-04-20 08:22:38.000000 manot-0.8.0/manot.egg-info/top_level.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)     1074 2023-04-20 08:18:27.000000 manot-0.8.0/pyproject.toml
--rw-rw-r--   0 armen     (1000) armen     (1000)       38 2023-04-20 08:22:38.917274 manot-0.8.0/setup.cfg
--rw-rw-r--   0 armen     (1000) armen     (1000)      816 2023-04-20 08:18:27.000000 manot-0.8.0/setup.py
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-04-20 08:22:38.913274 manot-0.8.0/src/
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-04-20 08:22:38.917274 manot-0.8.0/src/manot/
--rw-rw-r--   0 armen     (1000) armen     (1000)       78 2023-02-14 12:07:02.000000 manot-0.8.0/src/manot/__init__.py
--rw-rw-r--   0 armen     (1000) armen     (1000)     1358 2023-02-14 12:07:02.000000 manot-0.8.0/src/manot/logger.py
--rw-rw-r--   0 armen     (1000) armen     (1000)    11604 2023-04-18 10:27:49.000000 manot-0.8.0/src/manot/manot.py
--rw-rw-r--   0 armen     (1000) armen     (1000)     4890 2023-04-17 14:43:30.000000 manot-0.8.0/src/manot/upload_manager.py
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-04-20 08:49:23.562493 manot-0.8.1/
+-rw-rw-r--   0 armen     (1000) armen     (1000)     1061 2023-02-14 12:07:02.000000 manot-0.8.1/LICENSE
+-rw-rw-r--   0 armen     (1000) armen     (1000)     7099 2023-04-20 08:49:23.562493 manot-0.8.1/PKG-INFO
+-rw-rw-r--   0 armen     (1000) armen     (1000)     6135 2023-04-20 08:48:59.000000 manot-0.8.1/README.md
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-04-20 08:49:23.562493 manot-0.8.1/manot.egg-info/
+-rw-rw-r--   0 armen     (1000) armen     (1000)     7099 2023-04-20 08:49:23.000000 manot-0.8.1/manot.egg-info/PKG-INFO
+-rw-rw-r--   0 armen     (1000) armen     (1000)      274 2023-04-20 08:49:23.000000 manot-0.8.1/manot.egg-info/SOURCES.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)        1 2023-04-20 08:49:23.000000 manot-0.8.1/manot.egg-info/dependency_links.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)       59 2023-04-20 08:49:23.000000 manot-0.8.1/manot.egg-info/requires.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)        6 2023-04-20 08:49:23.000000 manot-0.8.1/manot.egg-info/top_level.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)     1074 2023-04-20 08:49:16.000000 manot-0.8.1/pyproject.toml
+-rw-rw-r--   0 armen     (1000) armen     (1000)       38 2023-04-20 08:49:23.562493 manot-0.8.1/setup.cfg
+-rw-rw-r--   0 armen     (1000) armen     (1000)      816 2023-04-20 08:49:16.000000 manot-0.8.1/setup.py
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-04-20 08:49:23.562493 manot-0.8.1/src/
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-04-20 08:49:23.562493 manot-0.8.1/src/manot/
+-rw-rw-r--   0 armen     (1000) armen     (1000)       78 2023-02-14 12:07:02.000000 manot-0.8.1/src/manot/__init__.py
+-rw-rw-r--   0 armen     (1000) armen     (1000)     1358 2023-02-14 12:07:02.000000 manot-0.8.1/src/manot/logger.py
+-rw-rw-r--   0 armen     (1000) armen     (1000)    11936 2023-04-20 08:48:59.000000 manot-0.8.1/src/manot/manot.py
+-rw-rw-r--   0 armen     (1000) armen     (1000)     4890 2023-04-17 14:43:30.000000 manot-0.8.1/src/manot/upload_manager.py
```

### Comparing `manot-0.8.0/LICENSE` & `manot-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `manot-0.8.0/PKG-INFO` & `manot-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manot
-Version: 0.8.0
+Version: 0.8.1
 Summary: manot AI is a model observability platform to monitor computer vision performance in real-time.
 Home-page: https://www.manot.ai
 Author: manot
 Author-email: manot <engineering@manot.ai>
 License: MIT
 Project-URL: Homepage, https://www.manot.ai
 Project-URL: Documentation, https://api.manot.ai/api-documentation/v1
@@ -48,23 +48,29 @@
 
 ```python
 from manot import manotAI
 
 manot = manotAI("manot_service_url", "token")
 ```
 
+Uploading data for setup
+-------
+
 ```python
 # Upload data to manot manager S3 bucket for Setup. The data should be in YOLO format
 manot.upload_data(dir_path="/path/to/data", process="setup")
 ```
 
+Running setup 
+-------
+
 ```python
-# Setup process for "local" and "s3" providers
+# Setup process for "local","gcs" and "s3" providers
 setup = manot.setup(
-    data_provider="s3", # it must be "s3" or "local"
+    data_provider="s3", # it must be "s3", "gcs" or "local"
     arguments={
             "name": "setup_example",
             "images_path": "/path/to/images",
             "ground_truths_path": "/path/to/ground_truths",
             "detections_path": "/path/to/detections",
             "detections_metadata_format": "xyx2y2",  # it must be one of "xyx2y2", "xywh", or "cxcywh"
             "classes_txt_path": "/path/to/classes.txt",
@@ -92,81 +98,92 @@
             "task": 'task_type', #can be classification or detection, in case of classification you don't have to provide detections_metadata_format
             "weight_name": "yolov5s" # by default, it is None   
         }
 )
 print(setup)
 # {"id": setup_id, "name": "setup_example", "status": "started"}
 
+```
+Get setup by id 
+-------
+
+```python
+
 setup_info = manot.get_setup(setup["id"])
 # when setup is successfully finished, then setup_info is {"id": setup_id, "name": "setup_example", "status": "started"}
 ```
+Upload data to get insights from 
+-------
 
 ```python
 # Upload data to manot manager S3 bucket to get insights
 manot.upload_data(dir_path="/path/to/data", process="insight")
 ```
+Running insight on data in s3, gcs or local machine
+-------
 
 ```python
 insight = manot.insight(
     name="insight_example",
     setup_id=setup["id"],
     data_path="/path/to/data",
-    data_provider="s3",  # it must be "s3" or "local"
+    data_provider="s3",  # it must be "s3", "gcs" or "local"
     percentage="percentage" # percentage of images to be considered insight should be larger than 0 and less or equal than 100
 )
 print(insight)
 # {"id": insight_id, "name": "insight_example", "status": "started"}
 
 insight_info = manot.get_insight(insight["id"])
 # when setup is successfully finished, then insight_info is {"id": insight_id, "name": "setup_example", "status": "started"}
 ```
 
+Running insight on hugging face model and dataset 
+-------
+
+```python
+insight = manot.huggingface_insight(
+    name='manot-huggingface',
+    data_path="huggingface_dataset",
+    model_path="huggingface_model",
+    task="detection",
+    percentage=0.5
+)
+insight_info = manot.get_insight(insight["id"])
+```
+
 ```
 scores = manot.get_score(insight['id'])
 #returns list of all processed images graded by their score from 0 to 10 (higher is more impactful image)
 # if the image cannot be assigned a score it will not be showing in the list 
 ```
 
 ```python
 #in case of deeplake please also provide deeplake token 
 manot.visualize_data_set(insight_info['data_set']['id'], deeplake_token,group_similar=True)
 # if group similar is set to True(default) will only return unique images 
 ```
 
-```python
-# Upload data for Setup or Insights process
-manot.upload_data(dir_path="/path/to/data", process="process_name")
-```
-For Setup process
-- dir_path is directory path, which must contain images, detections, and ground_truths folders and classes.txt file.
-- process must be "setup".
-
-For Insight process
-- dir_path is directory path, which must contain data. Data formats must be ".jpeg", ".jpg", ".png", ".avi", ".gif", ".m4v", ".mkv" or ".mp4".
-- process must be "insight".
-
-
 In case of detection task use this to calculate mAP on your data
 ```python
 manot.calculate_map(
     ground_truths_path="/path/to/ground_truths",
     detections_path="/path/to/detections",
     classes_txt_path="/path/to/classes.txt",
-    data_provider="local",  # it must be "s3" or "local"
+    data_provider="local",  # it must be "s3", "gcs" or "local"
     data_set_id="data_set_id",  # if data_set_id is provided will calculate mAP only on selected data, otherwise will calculate mAP on all the data
 )
 ```
 In case of classification use this to calculate accuracy on your data
 
 ```python
 manot.calculate_accuracy(
     images_path="/path/to/images",
     predictions_path="/path/to/predictions",
     classes_txt_path="/path/to/classes.txt",
-    data_provider="local",  # it must be "s3" or "local"
+    data_provider="local",  # it must be "s3", "gcs" or "local"
     data_set_id="data_set_id",  # if data_set_id is provided will calculate mAP only on selected data, otherwise will calculate mAP on all the data
 )
 ```
 
 Resources
 ---------
```

### Comparing `manot-0.8.0/README.md` & `manot-0.8.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -24,23 +24,29 @@
 
 ```python
 from manot import manotAI
 
 manot = manotAI("manot_service_url", "token")
 ```
 
+Uploading data for setup
+-------
+
 ```python
 # Upload data to manot manager S3 bucket for Setup. The data should be in YOLO format
 manot.upload_data(dir_path="/path/to/data", process="setup")
 ```
 
+Running setup 
+-------
+
 ```python
-# Setup process for "local" and "s3" providers
+# Setup process for "local","gcs" and "s3" providers
 setup = manot.setup(
-    data_provider="s3", # it must be "s3" or "local"
+    data_provider="s3", # it must be "s3", "gcs" or "local"
     arguments={
             "name": "setup_example",
             "images_path": "/path/to/images",
             "ground_truths_path": "/path/to/ground_truths",
             "detections_path": "/path/to/detections",
             "detections_metadata_format": "xyx2y2",  # it must be one of "xyx2y2", "xywh", or "cxcywh"
             "classes_txt_path": "/path/to/classes.txt",
@@ -68,81 +74,92 @@
             "task": 'task_type', #can be classification or detection, in case of classification you don't have to provide detections_metadata_format
             "weight_name": "yolov5s" # by default, it is None   
         }
 )
 print(setup)
 # {"id": setup_id, "name": "setup_example", "status": "started"}
 
+```
+Get setup by id 
+-------
+
+```python
+
 setup_info = manot.get_setup(setup["id"])
 # when setup is successfully finished, then setup_info is {"id": setup_id, "name": "setup_example", "status": "started"}
 ```
+Upload data to get insights from 
+-------
 
 ```python
 # Upload data to manot manager S3 bucket to get insights
 manot.upload_data(dir_path="/path/to/data", process="insight")
 ```
+Running insight on data in s3, gcs or local machine
+-------
 
 ```python
 insight = manot.insight(
     name="insight_example",
     setup_id=setup["id"],
     data_path="/path/to/data",
-    data_provider="s3",  # it must be "s3" or "local"
+    data_provider="s3",  # it must be "s3", "gcs" or "local"
     percentage="percentage" # percentage of images to be considered insight should be larger than 0 and less or equal than 100
 )
 print(insight)
 # {"id": insight_id, "name": "insight_example", "status": "started"}
 
 insight_info = manot.get_insight(insight["id"])
 # when setup is successfully finished, then insight_info is {"id": insight_id, "name": "setup_example", "status": "started"}
 ```
 
+Running insight on hugging face model and dataset 
+-------
+
+```python
+insight = manot.huggingface_insight(
+    name='manot-huggingface',
+    data_path="huggingface_dataset",
+    model_path="huggingface_model",
+    task="detection",
+    percentage=0.5
+)
+insight_info = manot.get_insight(insight["id"])
+```
+
 ```
 scores = manot.get_score(insight['id'])
 #returns list of all processed images graded by their score from 0 to 10 (higher is more impactful image)
 # if the image cannot be assigned a score it will not be showing in the list 
 ```
 
 ```python
 #in case of deeplake please also provide deeplake token 
 manot.visualize_data_set(insight_info['data_set']['id'], deeplake_token,group_similar=True)
 # if group similar is set to True(default) will only return unique images 
 ```
 
-```python
-# Upload data for Setup or Insights process
-manot.upload_data(dir_path="/path/to/data", process="process_name")
-```
-For Setup process
-- dir_path is directory path, which must contain images, detections, and ground_truths folders and classes.txt file.
-- process must be "setup".
-
-For Insight process
-- dir_path is directory path, which must contain data. Data formats must be ".jpeg", ".jpg", ".png", ".avi", ".gif", ".m4v", ".mkv" or ".mp4".
-- process must be "insight".
-
-
 In case of detection task use this to calculate mAP on your data
 ```python
 manot.calculate_map(
     ground_truths_path="/path/to/ground_truths",
     detections_path="/path/to/detections",
     classes_txt_path="/path/to/classes.txt",
-    data_provider="local",  # it must be "s3" or "local"
+    data_provider="local",  # it must be "s3", "gcs" or "local"
     data_set_id="data_set_id",  # if data_set_id is provided will calculate mAP only on selected data, otherwise will calculate mAP on all the data
 )
 ```
 In case of classification use this to calculate accuracy on your data
 
 ```python
 manot.calculate_accuracy(
     images_path="/path/to/images",
     predictions_path="/path/to/predictions",
     classes_txt_path="/path/to/classes.txt",
-    data_provider="local",  # it must be "s3" or "local"
+    data_provider="local",  # it must be "s3", "gcs" or "local"
     data_set_id="data_set_id",  # if data_set_id is provided will calculate mAP only on selected data, otherwise will calculate mAP on all the data
 )
 ```
 
 Resources
 ---------
```

### Comparing `manot-0.8.0/manot.egg-info/PKG-INFO` & `manot-0.8.1/manot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manot
-Version: 0.8.0
+Version: 0.8.1
 Summary: manot AI is a model observability platform to monitor computer vision performance in real-time.
 Home-page: https://www.manot.ai
 Author: manot
 Author-email: manot <engineering@manot.ai>
 License: MIT
 Project-URL: Homepage, https://www.manot.ai
 Project-URL: Documentation, https://api.manot.ai/api-documentation/v1
@@ -48,23 +48,29 @@
 
 ```python
 from manot import manotAI
 
 manot = manotAI("manot_service_url", "token")
 ```
 
+Uploading data for setup
+-------
+
 ```python
 # Upload data to manot manager S3 bucket for Setup. The data should be in YOLO format
 manot.upload_data(dir_path="/path/to/data", process="setup")
 ```
 
+Running setup 
+-------
+
 ```python
-# Setup process for "local" and "s3" providers
+# Setup process for "local","gcs" and "s3" providers
 setup = manot.setup(
-    data_provider="s3", # it must be "s3" or "local"
+    data_provider="s3", # it must be "s3", "gcs" or "local"
     arguments={
             "name": "setup_example",
             "images_path": "/path/to/images",
             "ground_truths_path": "/path/to/ground_truths",
             "detections_path": "/path/to/detections",
             "detections_metadata_format": "xyx2y2",  # it must be one of "xyx2y2", "xywh", or "cxcywh"
             "classes_txt_path": "/path/to/classes.txt",
@@ -92,81 +98,92 @@
             "task": 'task_type', #can be classification or detection, in case of classification you don't have to provide detections_metadata_format
             "weight_name": "yolov5s" # by default, it is None   
         }
 )
 print(setup)
 # {"id": setup_id, "name": "setup_example", "status": "started"}
 
+```
+Get setup by id 
+-------
+
+```python
+
 setup_info = manot.get_setup(setup["id"])
 # when setup is successfully finished, then setup_info is {"id": setup_id, "name": "setup_example", "status": "started"}
 ```
+Upload data to get insights from 
+-------
 
 ```python
 # Upload data to manot manager S3 bucket to get insights
 manot.upload_data(dir_path="/path/to/data", process="insight")
 ```
+Running insight on data in s3, gcs or local machine
+-------
 
 ```python
 insight = manot.insight(
     name="insight_example",
     setup_id=setup["id"],
     data_path="/path/to/data",
-    data_provider="s3",  # it must be "s3" or "local"
+    data_provider="s3",  # it must be "s3", "gcs" or "local"
     percentage="percentage" # percentage of images to be considered insight should be larger than 0 and less or equal than 100
 )
 print(insight)
 # {"id": insight_id, "name": "insight_example", "status": "started"}
 
 insight_info = manot.get_insight(insight["id"])
 # when setup is successfully finished, then insight_info is {"id": insight_id, "name": "setup_example", "status": "started"}
 ```
 
+Running insight on hugging face model and dataset 
+-------
+
+```python
+insight = manot.huggingface_insight(
+    name='manot-huggingface',
+    data_path="huggingface_dataset",
+    model_path="huggingface_model",
+    task="detection",
+    percentage=0.5
+)
+insight_info = manot.get_insight(insight["id"])
+```
+
 ```
 scores = manot.get_score(insight['id'])
 #returns list of all processed images graded by their score from 0 to 10 (higher is more impactful image)
 # if the image cannot be assigned a score it will not be showing in the list 
 ```
 
 ```python
 #in case of deeplake please also provide deeplake token 
 manot.visualize_data_set(insight_info['data_set']['id'], deeplake_token,group_similar=True)
 # if group similar is set to True(default) will only return unique images 
 ```
 
-```python
-# Upload data for Setup or Insights process
-manot.upload_data(dir_path="/path/to/data", process="process_name")
-```
-For Setup process
-- dir_path is directory path, which must contain images, detections, and ground_truths folders and classes.txt file.
-- process must be "setup".
-
-For Insight process
-- dir_path is directory path, which must contain data. Data formats must be ".jpeg", ".jpg", ".png", ".avi", ".gif", ".m4v", ".mkv" or ".mp4".
-- process must be "insight".
-
-
 In case of detection task use this to calculate mAP on your data
 ```python
 manot.calculate_map(
     ground_truths_path="/path/to/ground_truths",
     detections_path="/path/to/detections",
     classes_txt_path="/path/to/classes.txt",
-    data_provider="local",  # it must be "s3" or "local"
+    data_provider="local",  # it must be "s3", "gcs" or "local"
     data_set_id="data_set_id",  # if data_set_id is provided will calculate mAP only on selected data, otherwise will calculate mAP on all the data
 )
 ```
 In case of classification use this to calculate accuracy on your data
 
 ```python
 manot.calculate_accuracy(
     images_path="/path/to/images",
     predictions_path="/path/to/predictions",
     classes_txt_path="/path/to/classes.txt",
-    data_provider="local",  # it must be "s3" or "local"
+    data_provider="local",  # it must be "s3", "gcs" or "local"
     data_set_id="data_set_id",  # if data_set_id is provided will calculate mAP only on selected data, otherwise will calculate mAP on all the data
 )
 ```
 
 Resources
 ---------
```

### Comparing `manot-0.8.0/pyproject.toml` & `manot-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "manot"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
     { name = "manot", email = "engineering@manot.ai" },
 ]
 license = {text = "MIT"}
 description = "manot AI is a model observability platform to monitor computer vision performance in real-time."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `manot-0.8.0/setup.py` & `manot-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
 setup(
     name='manot',
-    version='0.8.0',
+    version='0.8.1',
     description='The manot SDK is a wrapper on top of our API to make it easier to work with our model performance monitoring system. Using our SDK you can quickly set up your project by defining a few key parameters, including the paths to your data, classes and model. Once the project is set up you will be able to use the insight method to extract outliers that manot has detected on the new unstructured data that the performance of the model is evaluated on.',
     author='manot',
     author_email='engineering@manot.ai',
     url='https://www.manot.ai',
     packages=['manot'],
     package_dir={'manot': 'src/manot'},
     project_urls={
```

### Comparing `manot-0.8.0/src/manot/logger.py` & `manot-0.8.1/src/manot/logger.py`

 * *Files identical despite different names*

### Comparing `manot-0.8.0/src/manot/manot.py` & `manot-0.8.1/src/manot/manot.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,32 +79,53 @@
             else:
                 log.error(f'There is problem setup process with id {response.json()["id"]}.')
                 return False
 
         log.error(response.text)
         return False
 
-    def huggingface_insight(
+    def get_setup(self, setup_id: int) -> Union[bool, None, dict]:
+
+        url = f"{self.__url}/api/v1/setup/{setup_id}"
+
+        try:
+            response = requests.get(url=url)
+        except Exception:
+            log.error("There is problem with request.")
+            return False
+
+        if response.status_code != 200:
+            log.warning("Setup not found.")
+            return None
+
+        return response.json()
+
+    def insight(
             self,
             name: str,
-            data_path: str,
-            task: Optional[Literal['classification', 'segmentation', 'detection']] = 'detection',
-            percentage: Optional[float] = None,
-            model_path: Optional[str] = None,
-
+            setup_id: int,
+            data_path: Union[str, List[str]],
+            data_provider: Literal['s3', 'local', 'deeplake'],
+            weight_name: Optional[str] = None,
+            deeplake_token: Optional[str] = None,
+            percentage: Optional[float] = None
     ) -> Union[bool, dict]:
 
-        url = f"{self.__url}/api/v1/insight/huggingface"
+        url = f"{self.__url}/api/v1/insight/"
         data = {
             "name": name,
+            "setup_id": setup_id,
             "data_path": data_path,
-            "model_path": model_path,
-            "task": task,
+            "data_provider": data_provider,
+            "deeplake_token": deeplake_token,
             "percentage": percentage
         }
+        if weight_name:
+            data["weight_name"] = weight_name
+
         try:
             response = requests.post(url=url, data=json.dumps(data), headers={"token": self.__token})
         except Exception:
             log.error("There is problem with request.")
             return False
 
         if response.status_code == 202:
@@ -119,52 +140,33 @@
             else:
                 log.error(f'There is problem insight process with id {response.json()["id"]}.')
                 return False
 
         log.error(response.text)
         return False
 
-    def get_setup(self, setup_id: int) -> Union[bool, None, dict]:
-
-        url = f"{self.__url}/api/v1/setup/{setup_id}"
-
-        try:
-            response = requests.get(url=url)
-        except Exception:
-            log.error("There is problem with request.")
-            return False
-
-        if response.status_code != 200:
-            log.warning("Setup not found.")
-            return None
-
-        return response.json()
-    def insight(
+    def huggingface_insight(
             self,
             name: str,
-            setup_id: int,
-            data_path: Union[str, List[str]],
-            data_provider: Literal['s3', 'local', 'deeplake'],
-            weight_name: Optional[str] = None,
-            deeplake_token: Optional[str] = None,
-            percentage: Optional[float] = None
+            data_path: str,
+            task: Optional[Literal['classification', 'segmentation', 'detection']] = 'detection',
+            percentage: Optional[float] = None,
+            model_path: Optional[str] = None,
+
+
     ) -> Union[bool, dict]:
 
-        url = f"{self.__url}/api/v1/insight/"
+        url = f"{self.__url}/api/v1/insight/huggingface"
         data = {
             "name": name,
-            "setup_id": setup_id,
             "data_path": data_path,
-            "data_provider": data_provider,
-            "deeplake_token": deeplake_token,
+            "model_path": model_path,
+            "task": task,
             "percentage": percentage
         }
-        if weight_name:
-            data["weight_name"] = weight_name
-
         try:
             response = requests.post(url=url, data=json.dumps(data), headers={"token": self.__token})
         except Exception:
             log.error("There is problem with request.")
             return False
 
         if response.status_code == 202:
@@ -178,14 +180,15 @@
                 return progress_result
             else:
                 log.error(f'There is problem insight process with id {response.json()["id"]}.')
                 return False
 
         log.error(response.text)
         return False
+
     def get_insight(self, insight_id: int) -> Union[bool, None, dict]:
 
         url = f"{self.__url}/api/v1/insight/{insight_id}"
 
         try:
             response = requests.get(url=url)
         except Exception:
@@ -194,15 +197,22 @@
 
         if response.status_code != 200:
             log.warning("Insight not found.")
             return None
 
         return response.json()
 
-    def visualize_data_set(self, data_set_id: int, deeplake_token: str = None, group_similar=True):
+    def visualize_data_set(
+            self,
+            data_set_id: int,
+            deeplake_token: str = None,
+            group_similar=True,
+            with_inference: Optional[bool] = False,
+            huggingface_model: Optional[str] = None
+    ):
         url = f"{self.__url}/api/v1/data_set/{data_set_id}?deeplake_token={deeplake_token}&group_similar={group_similar}"
 
         try:
             response = requests.get(url=url).json()
         except Exception:
             log.error("There is problem with request.")
             return False
@@ -210,15 +220,15 @@
         if not response:
             log.warning("Data Set not found.")
             return None
 
         images = response['data_set_images']
         images_urls = []
         for file in images:
-            images_urls.append(self.__process(file['id'], deeplake_token))
+            images_urls.append(self.__process(file['id'], deeplake_token, with_inference, huggingface_model))
         return ipyplot.plot_images(images_urls, img_width=200, show_url=False, max_images=len(images_urls))
 
     def upload_data(self, dir_path: str, process: Literal["setup", "insight"]):
 
         upload_manager = UploadManager(directory=dir_path, url=self.__url, token=self.__token)
         if process == "setup":
             return upload_manager.upload_setup_data()
@@ -297,16 +307,17 @@
             return False
 
         if response.status_code != 200:
             log.warning(response.json()['message'])
             return None
         return response.json()
 
-    def __process(self, image_id: int, deeplake_token: str = None):
-        url = f"{self.__url}/api/v1/image/{image_id}?deeplake_token={deeplake_token}"
+    def __process(self, image_id: int, deeplake_token: str = None, with_inference=False,huggingface_model=None):
+
+        url = f"{self.__url}/api/v1/image/{image_id}?deeplake_token={deeplake_token}&with_inference={with_inference}&huggingface_model={huggingface_model}&time={time.time()}"
         return url
 
     def __check_progress(self, process_method, id):
         progress = 0
         progress_bar = tqdm(desc="Progress", total=100)
         while progress < 100:
             result = process_method(id)
```

### Comparing `manot-0.8.0/src/manot/upload_manager.py` & `manot-0.8.1/src/manot/upload_manager.py`

 * *Files identical despite different names*

