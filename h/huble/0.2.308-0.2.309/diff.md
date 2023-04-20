# Comparing `tmp/huble-0.2.308.tar.gz` & `tmp/huble-0.2.309.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huble-0.2.308.tar", max compression
+gzip compressed data, was "huble-0.2.309.tar", max compression
```

## Comparing `huble-0.2.308.tar` & `huble-0.2.309.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0        0 2022-09-01 20:06:17.369927 huble-0.2.308/README.md
--rw-r--r--   0        0        0      684 2023-04-20 16:13:56.867479 huble-0.2.308/pyproject.toml
--rw-r--r--   0        0        0      134 2023-02-04 11:17:14.977888 huble-0.2.308/src/huble/__init__.py
--rw-r--r--   0        0        0       26 2023-03-13 11:26:31.526581 huble-0.2.308/src/huble/automl/__init__.py
--rw-r--r--   0        0        0     5320 2023-04-20 15:30:18.998080 huble-0.2.308/src/huble/automl/automl.py
--rw-r--r--   0        0        0       98 2023-02-04 11:17:06.597876 huble-0.2.308/src/huble/connector/__init__.py
--rw-r--r--   0        0        0      587 2023-04-18 10:13:25.574236 huble-0.2.308/src/huble/connector/dataset.py
--rw-r--r--   0        0        0     1547 2023-04-20 15:54:44.569807 huble-0.2.308/src/huble/connector/deployment.py
--rw-r--r--   0        0        0     2188 2023-04-19 12:55:09.325037 huble-0.2.308/src/huble/connector/experiment.py
--rw-r--r--   0        0        0      156 2023-02-01 12:25:17.923451 huble-0.2.308/src/huble/error/__init__.py
--rw-r--r--   0        0        0      524 2023-02-01 07:34:10.430416 huble-0.2.308/src/huble/error/decorators.py
--rw-r--r--   0        0        0      608 2023-02-01 12:25:17.930118 huble-0.2.308/src/huble/error/exceptions.py
--rw-r--r--   0        0        0      447 2023-04-18 09:17:59.948453 huble-0.2.308/src/huble/main.py
--rw-r--r--   0        0        0      118 2023-02-01 12:25:17.910118 huble-0.2.308/src/huble/sklearn/__init__.py
--rw-r--r--   0        0        0       75 2023-01-30 06:53:33.773046 huble-0.2.308/src/huble/sklearn/essentials/__init__.py
--rw-r--r--   0        0        0      933 2023-01-29 09:39:15.224016 huble-0.2.308/src/huble/sklearn/essentials/essentail_params.ts
--rw-r--r--   0        0        0     1257 2023-04-19 08:30:24.640416 huble-0.2.308/src/huble/sklearn/essentials/function.py
--rw-r--r--   0        0        0     1009 2023-04-18 12:36:03.383049 huble-0.2.308/src/huble/sklearn/essentials/handler.py
--rw-r--r--   0        0        0     1246 2023-04-19 12:40:24.580020 huble-0.2.308/src/huble/sklearn/evaluate.py
--rw-r--r--   0        0        0     3499 2023-04-19 08:13:38.386795 huble-0.2.308/src/huble/sklearn/generate.py
--rw-r--r--   0        0        0     1410 2023-02-14 03:58:18.837339 huble-0.2.308/src/huble/sklearn/graph.py
--rw-r--r--   0        0        0       33 2023-02-01 12:25:17.910118 huble-0.2.308/src/huble/sklearn/metrics/__init__.py
--rw-r--r--   0        0        0     4860 2023-02-24 09:49:44.133824 huble-0.2.308/src/huble/sklearn/metrics/metrics.py
--rw-r--r--   0        0        0      570 2023-02-01 12:25:17.916785 huble-0.2.308/src/huble/sklearn/process/__init__.py
--rw-r--r--   0        0        0     6548 2023-02-18 12:25:51.014331 huble-0.2.308/src/huble/sklearn/process/functions.py
--rw-r--r--   0        0        0    11268 2023-02-18 12:25:51.014331 huble-0.2.308/src/huble/sklearn/process/handler.py
--rw-r--r--   0        0        0    21731 2023-02-18 12:25:51.014331 huble-0.2.308/src/huble/sklearn/process/preprocess_params.ts
--rw-r--r--   0        0        0      602 2023-02-01 12:25:17.926785 huble-0.2.308/src/huble/sklearn/train/__init__.py
--rw-r--r--   0        0        0     4944 2023-02-15 04:48:23.675688 huble-0.2.308/src/huble/sklearn/train/functions.py
--rw-r--r--   0        0        0    13409 2023-02-04 12:30:51.391609 huble-0.2.308/src/huble/sklearn/train/handler.py
--rw-r--r--   0        0        0    35186 2023-01-12 16:42:04.986469 huble-0.2.308/src/huble/sklearn/train/model_params.ts
--rw-r--r--   0        0        0      357 2023-04-20 15:31:22.442168 huble-0.2.308/src/huble/util/__init__.py
--rw-r--r--   0        0        0     3792 2023-02-01 12:25:17.993452 huble-0.2.308/src/huble/util/convert_to_reactflow_graph.py
--rw-r--r--   0        0        0     1186 2023-04-20 15:30:18.998080 huble-0.2.308/src/huble/util/data_types.py
--rw-r--r--   0        0        0     1122 2023-04-19 07:48:55.011248 huble-0.2.308/src/huble/util/feature_selection.py
--rw-r--r--   0        0        0     2528 2023-02-14 06:45:35.870429 huble-0.2.308/src/huble/util/inference_pipeline.py
--rw-r--r--   0        0        0     1739 2023-04-20 16:13:52.247421 huble-0.2.308/src/huble/util/preprocess_code.py
--rw-r--r--   0        0        0      502 2023-02-01 12:25:17.946785 huble-0.2.308/src/huble/util/recommend_model.py
--rw-r--r--   0        0        0     1402 2023-04-19 09:09:33.409266 huble-0.2.308/src/huble/util/typed_params.py
--rw-r--r--   0        0        0     2970 2023-04-17 11:56:37.994780 huble-0.2.308/src/huble/util/verify_builder_pipeline.py
--rw-r--r--   0        0        0     4888 2023-02-14 03:58:18.837339 huble-0.2.308/src/huble/util/verify_ml.py
--rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 huble-0.2.308/setup.py
--rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 huble-0.2.308/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-09-01 20:06:17.369927 huble-0.2.309/README.md
+-rw-r--r--   0        0        0      684 2023-04-20 18:20:08.054762 huble-0.2.309/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-02-04 11:17:14.977888 huble-0.2.309/src/huble/__init__.py
+-rw-r--r--   0        0        0       26 2023-03-13 11:26:31.526581 huble-0.2.309/src/huble/automl/__init__.py
+-rw-r--r--   0        0        0     5320 2023-04-20 15:30:18.998080 huble-0.2.309/src/huble/automl/automl.py
+-rw-r--r--   0        0        0       98 2023-02-04 11:17:06.597876 huble-0.2.309/src/huble/connector/__init__.py
+-rw-r--r--   0        0        0      587 2023-04-18 10:13:25.574236 huble-0.2.309/src/huble/connector/dataset.py
+-rw-r--r--   0        0        0     1547 2023-04-20 15:54:44.569807 huble-0.2.309/src/huble/connector/deployment.py
+-rw-r--r--   0        0        0     2275 2023-04-20 18:11:26.223801 huble-0.2.309/src/huble/connector/experiment.py
+-rw-r--r--   0        0        0      156 2023-02-01 12:25:17.923451 huble-0.2.309/src/huble/error/__init__.py
+-rw-r--r--   0        0        0      524 2023-02-01 07:34:10.430416 huble-0.2.309/src/huble/error/decorators.py
+-rw-r--r--   0        0        0      608 2023-02-01 12:25:17.930118 huble-0.2.309/src/huble/error/exceptions.py
+-rw-r--r--   0        0        0      447 2023-04-18 09:17:59.948453 huble-0.2.309/src/huble/main.py
+-rw-r--r--   0        0        0      118 2023-02-01 12:25:17.910118 huble-0.2.309/src/huble/sklearn/__init__.py
+-rw-r--r--   0        0        0       75 2023-01-30 06:53:33.773046 huble-0.2.309/src/huble/sklearn/essentials/__init__.py
+-rw-r--r--   0        0        0      933 2023-01-29 09:39:15.224016 huble-0.2.309/src/huble/sklearn/essentials/essentail_params.ts
+-rw-r--r--   0        0        0     1295 2023-04-20 18:11:26.223801 huble-0.2.309/src/huble/sklearn/essentials/function.py
+-rw-r--r--   0        0        0     1028 2023-04-20 18:11:26.223801 huble-0.2.309/src/huble/sklearn/essentials/handler.py
+-rw-r--r--   0        0        0     1246 2023-04-19 12:40:24.580020 huble-0.2.309/src/huble/sklearn/evaluate.py
+-rw-r--r--   0        0        0     3518 2023-04-20 18:11:26.227134 huble-0.2.309/src/huble/sklearn/generate.py
+-rw-r--r--   0        0        0     1410 2023-02-14 03:58:18.837339 huble-0.2.309/src/huble/sklearn/graph.py
+-rw-r--r--   0        0        0       33 2023-02-01 12:25:17.910118 huble-0.2.309/src/huble/sklearn/metrics/__init__.py
+-rw-r--r--   0        0        0     4860 2023-02-24 09:49:44.133824 huble-0.2.309/src/huble/sklearn/metrics/metrics.py
+-rw-r--r--   0        0        0      570 2023-02-01 12:25:17.916785 huble-0.2.309/src/huble/sklearn/process/__init__.py
+-rw-r--r--   0        0        0     6548 2023-02-18 12:25:51.014331 huble-0.2.309/src/huble/sklearn/process/functions.py
+-rw-r--r--   0        0        0    11268 2023-02-18 12:25:51.014331 huble-0.2.309/src/huble/sklearn/process/handler.py
+-rw-r--r--   0        0        0    21731 2023-02-18 12:25:51.014331 huble-0.2.309/src/huble/sklearn/process/preprocess_params.ts
+-rw-r--r--   0        0        0      602 2023-02-01 12:25:17.926785 huble-0.2.309/src/huble/sklearn/train/__init__.py
+-rw-r--r--   0        0        0     4944 2023-02-15 04:48:23.675688 huble-0.2.309/src/huble/sklearn/train/functions.py
+-rw-r--r--   0        0        0    13409 2023-02-04 12:30:51.391609 huble-0.2.309/src/huble/sklearn/train/handler.py
+-rw-r--r--   0        0        0    35186 2023-01-12 16:42:04.986469 huble-0.2.309/src/huble/sklearn/train/model_params.ts
+-rw-r--r--   0        0        0      357 2023-04-20 15:31:22.442168 huble-0.2.309/src/huble/util/__init__.py
+-rw-r--r--   0        0        0     3792 2023-02-01 12:25:17.993452 huble-0.2.309/src/huble/util/convert_to_reactflow_graph.py
+-rw-r--r--   0        0        0     1186 2023-04-20 15:30:18.998080 huble-0.2.309/src/huble/util/data_types.py
+-rw-r--r--   0        0        0     1157 2023-04-20 18:11:26.227134 huble-0.2.309/src/huble/util/feature_selection.py
+-rw-r--r--   0        0        0     2528 2023-02-14 06:45:35.870429 huble-0.2.309/src/huble/util/inference_pipeline.py
+-rw-r--r--   0        0        0     1739 2023-04-20 16:13:52.247421 huble-0.2.309/src/huble/util/preprocess_code.py
+-rw-r--r--   0        0        0      502 2023-02-01 12:25:17.946785 huble-0.2.309/src/huble/util/recommend_model.py
+-rw-r--r--   0        0        0     1402 2023-04-19 09:09:33.409266 huble-0.2.309/src/huble/util/typed_params.py
+-rw-r--r--   0        0        0     2970 2023-04-17 11:56:37.994780 huble-0.2.309/src/huble/util/verify_builder_pipeline.py
+-rw-r--r--   0        0        0     4888 2023-02-14 03:58:18.837339 huble-0.2.309/src/huble/util/verify_ml.py
+-rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 huble-0.2.309/setup.py
+-rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 huble-0.2.309/PKG-INFO
```

### Comparing `huble-0.2.308/pyproject.toml` & `huble-0.2.309/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huble"
-version = "0.2.308"
+version = "0.2.309"
 description = ""
 authors = ["Rugz007 <rugvedsomwanshi007@gmail.com>"]
 maintainers = [
     "Arjit Agarwal <arjitagarwal123@gmail.com>",
     "Ashmika Gupte <ashmikagupte01@gmail.com>",
 ]
 readme = "README.md"
```

### Comparing `huble-0.2.308/src/huble/automl/automl.py` & `huble-0.2.309/src/huble/automl/automl.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/connector/dataset.py` & `huble-0.2.309/src/huble/connector/dataset.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/connector/deployment.py` & `huble-0.2.309/src/huble/connector/deployment.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/connector/experiment.py` & `huble-0.2.309/src/huble/connector/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,21 +35,22 @@
             task_type = project["taskType"]
             modelURL = response["modelURL"]
             input_format = response["inputFormat"]
         except:
             raise Exception("Invalid Experiment ID")
         return graph, task_type, target_column, modelURL, input_format
 
-    def upload_metrics(self, metrics, input_format, feature_importance_dict):
+    def upload_metrics(self, metrics, input_format, feature_importance_dict, selected_features):
         requests.put(
             f"http://localhost:8000/experiments/results/{self.experiment_id}",
             data={
                 "metrics": json.dumps(metrics),
                 "input_format": json.dumps(input_format),
                 "feature_importance": json.dumps(feature_importance_dict),
+                "selected_features": json.dumps(selected_features),
             },
         )
 
     def upload_model(self, file_name):
         try:
             with open(file_name, "rb") as data:
                 print("Uploading model...")
```

### Comparing `huble-0.2.308/src/huble/error/decorators.py` & `huble-0.2.309/src/huble/error/decorators.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/error/exceptions.py` & `huble-0.2.309/src/huble/error/exceptions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/sklearn/essentials/essentail_params.ts` & `huble-0.2.309/src/huble/sklearn/essentials/essentail_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/sklearn/essentials/function.py` & `huble-0.2.309/src/huble/sklearn/essentials/function.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # @function_error_handling("train_test_split")
 def train_test_split(**params):
     data = params["data"]
     target = params["target_column"]
     model = params["model"]
     X = data.drop([target], axis=1)
     data_dict = get_dataframe_types(X)
-    data = select_features(data, target)
+    data, selected_features = select_features(data, target)
     train_dataset, test_dataset = sklearn_tts(data, test_size=params["parameters"]["test_size"], random_state=42)
-    return train_dataset, test_dataset, data_dict
+    return train_dataset, test_dataset, data_dict, selected_features
 
 
 # @function_error_handling("train_model")
 def train_model(**params):
     task_type = params["task_type"]
     data = params["data"]
     model = params["model"]
```

### Comparing `huble-0.2.308/src/huble/sklearn/essentials/handler.py` & `huble-0.2.309/src/huble/sklearn/essentials/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,11 +10,11 @@
         }
         return essentials[function_name](params=params, task_type=task_type, target_column=target_column,id=id)
 
     def __train_test_split(self, params, target_column, **kwargs):
         parameters = {
             "test_size": params["test_size"],
         }
-        return f"training_dataset, test_dataset, input_format = huble.sklearn.train_test_split(data=data,parameters={parameters}, target_column='{target_column}', model=model)"
+        return f"training_dataset, test_dataset, input_format, selected_features = huble.sklearn.train_test_split(data=data,parameters={parameters}, target_column='{target_column}', model=model)"
 
     def __train_model(self, params, task_type, target_column,id, **kwargs):
         return f"Model, filename = huble.sklearn.train_model(data=training_dataset, model=model, column='{target_column}', task_type='{task_type}',id='{id}')"
```

### Comparing `huble-0.2.308/src/huble/sklearn/evaluate.py` & `huble-0.2.309/src/huble/sklearn/evaluate.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/sklearn/generate.py` & `huble-0.2.309/src/huble/sklearn/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,10 +78,10 @@
                     # TODO: make changes for clustering
                     f"\tmetrics, feature_importance_dict = huble.sklearn.evaluate_model(model=Model, training_dataset=training_dataset, test_dataset=test_dataset, target_column= '{target_column}', task_type='{task_type}' )"
                 )
                 f.write("\n")
             elif steps_list[i] == "primary_dataset":
                 # TODO: Add support for other datasets
                 f.write(f"\tdata = Dataset('{node['data']['url']}').dataframe\n")
-        f.write("\texperiment.upload_metrics(metrics,input_format,feature_importance_dict)")
+        f.write("\texperiment.upload_metrics(metrics,input_format,feature_importance_dict, selected_features)")
         f.write("\n\tprint(\"Uploading model...\")")
         f.write("\n\texperiment.upload_model(filename)")
```

### Comparing `huble-0.2.308/src/huble/sklearn/graph.py` & `huble-0.2.309/src/huble/sklearn/graph.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/sklearn/metrics/metrics.py` & `huble-0.2.309/src/huble/sklearn/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/sklearn/process/__init__.py` & `huble-0.2.309/src/huble/sklearn/process/__init__.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/sklearn/process/functions.py` & `huble-0.2.309/src/huble/sklearn/process/functions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/sklearn/process/handler.py` & `huble-0.2.309/src/huble/sklearn/process/handler.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/sklearn/process/preprocess_params.ts` & `huble-0.2.309/src/huble/sklearn/process/preprocess_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/sklearn/train/__init__.py` & `huble-0.2.309/src/huble/sklearn/train/__init__.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/sklearn/train/functions.py` & `huble-0.2.309/src/huble/sklearn/train/functions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/sklearn/train/handler.py` & `huble-0.2.309/src/huble/sklearn/train/handler.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/sklearn/train/model_params.ts` & `huble-0.2.309/src/huble/sklearn/train/model_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/util/convert_to_reactflow_graph.py` & `huble-0.2.309/src/huble/util/convert_to_reactflow_graph.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/util/data_types.py` & `huble-0.2.309/src/huble/util/data_types.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/util/feature_selection.py` & `huble-0.2.309/src/huble/util/feature_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
     sfm.fit(X, y)
     selected_features_mask = sfm.get_support()
     selected_features_names = X.columns[selected_features_mask]
 
     selected_data = data[selected_features_names.union([target_column])]
 
-    return selected_data
+    return selected_data, selected_features_names.to_list()
```

### Comparing `huble-0.2.308/src/huble/util/inference_pipeline.py` & `huble-0.2.309/src/huble/util/inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/util/preprocess_code.py` & `huble-0.2.309/src/huble/util/preprocess_code.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/util/typed_params.py` & `huble-0.2.309/src/huble/util/typed_params.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/util/verify_builder_pipeline.py` & `huble-0.2.309/src/huble/util/verify_builder_pipeline.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/src/huble/util/verify_ml.py` & `huble-0.2.309/src/huble/util/verify_ml.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.308/setup.py` & `huble-0.2.309/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'pandas>=1.3.5,<2.0.0',
  'pydantic>=1.10.4,<2.0.0',
  'scikit-learn==1.1.2',
  'scipy>=1.7.0,<1.8.0']
 
 setup_kwargs = {
     'name': 'huble',
-    'version': '0.2.308',
+    'version': '0.2.309',
     'description': '',
     'long_description': '',
     'author': 'Rugz007',
     'author_email': 'rugvedsomwanshi007@gmail.com',
     'maintainer': 'Arjit Agarwal',
     'maintainer_email': 'arjitagarwal123@gmail.com',
     'url': 'None',
```

### Comparing `huble-0.2.308/PKG-INFO` & `huble-0.2.309/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huble
-Version: 0.2.308
+Version: 0.2.309
 Summary: 
 Author: Rugz007
 Author-email: rugvedsomwanshi007@gmail.com
 Maintainer: Arjit Agarwal
 Maintainer-email: arjitagarwal123@gmail.com
 Requires-Python: >=3.8.1,<3.10
 Classifier: Programming Language :: Python :: 3
```

