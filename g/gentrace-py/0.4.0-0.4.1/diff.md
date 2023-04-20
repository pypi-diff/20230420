# Comparing `tmp/gentrace_py-0.4.0.tar.gz` & `tmp/gentrace_py-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentrace_py-0.4.0.tar", max compression
+gzip compressed data, was "gentrace_py-0.4.1.tar", max compression
```

## Comparing `gentrace_py-0.4.0.tar` & `gentrace_py-0.4.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      980 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/__init__.py
--rw-r--r--   0        0        0    59420 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/api_client.py
--rw-r--r--   0        0        0      215 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/apis/__init__.py
--rw-r--r--   0        0        0      325 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/apis/paths/__init__.py
--rw-r--r--   0        0        0      105 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/apis/paths/pipeline_run.py
--rw-r--r--   0        0        0      459 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/apis/tag_to_api.py
--rw-r--r--   0        0        0      335 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/apis/tags/__init__.py
--rw-r--r--   0        0        0      485 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/apis/tags/ingestion_api.py
--rw-r--r--   0        0        0    15476 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/configuration.py
--rw-r--r--   0        0        0     4444 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/exceptions.py
--rw-r--r--   0        0        0      342 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/__init__.py
--rw-r--r--   0        0        0     5209 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/feedback_request.py
--rw-r--r--   0        0        0     4998 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/feedback_request.pyi
--rw-r--r--   0        0        0     2144 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/feedback_response.py
--rw-r--r--   0        0        0     2121 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/feedback_response.pyi
--rw-r--r--   0        0        0    33338 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/pipeline_run_request.py
--rw-r--r--   0        0        0    32730 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/pipeline_run_request.pyi
--rw-r--r--   0        0        0     2779 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/pipeline_run_response.py
--rw-r--r--   0        0        0     2739 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/pipeline_run_response.pyi
--rw-r--r--   0        0        0      640 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/models/__init__.py
--rw-r--r--   0        0        0      318 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/paths/__init__.py
--rw-r--r--   0        0        0      299 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/paths/pipeline_run/__init__.py
--rw-r--r--   0        0        0    12578 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/paths/pipeline_run/post.py
--rw-r--r--   0        0        0    12355 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/paths/pipeline_run/post.pyi
--rw-r--r--   0        0        0      202 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/__init__.py
--rw-r--r--   0        0        0     3352 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/getters.py
--rw-r--r--   0        0        0      182 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/llms/__init__.py
--rw-r--r--   0        0        0    22046 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/llms/openai.py
--rw-r--r--   0        0        0     3042 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/pipeline.py
--rw-r--r--   0        0        0     6252 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/pipeline_run.py
--rw-r--r--   0        0        0      531 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/step_run.py
--rw-r--r--   0        0        0      695 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/utils.py
--rw-r--r--   0        0        0      219 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/vectorstores/__init__.py
--rw-r--r--   0        0        0    10432 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/vectorstores/pinecone.py
--rw-r--r--   0        0        0    10398 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/rest.py
--rw-r--r--   0        0        0   103185 2023-04-19 22:15:13.688094 gentrace_py-0.4.0/gentrace/schemas.py
--rw-r--r--   0        0        0     1298 2023-04-19 22:15:13.688094 gentrace_py-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      980 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/__init__.py
+-rw-r--r--   0        0        0    59420 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/api_client.py
+-rw-r--r--   0        0        0      215 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/apis/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/apis/paths/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/apis/paths/pipeline_run.py
+-rw-r--r--   0        0        0      459 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/apis/tag_to_api.py
+-rw-r--r--   0        0        0      335 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/apis/tags/__init__.py
+-rw-r--r--   0        0        0      485 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/apis/tags/ingestion_api.py
+-rw-r--r--   0        0        0    15476 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/configuration.py
+-rw-r--r--   0        0        0     4444 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/exceptions.py
+-rw-r--r--   0        0        0      342 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/__init__.py
+-rw-r--r--   0        0        0     5209 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/feedback_request.py
+-rw-r--r--   0        0        0     4998 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/feedback_request.pyi
+-rw-r--r--   0        0        0     2144 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/feedback_response.py
+-rw-r--r--   0        0        0     2121 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/feedback_response.pyi
+-rw-r--r--   0        0        0    33338 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/pipeline_run_request.py
+-rw-r--r--   0        0        0    32730 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/pipeline_run_request.pyi
+-rw-r--r--   0        0        0     2779 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/pipeline_run_response.py
+-rw-r--r--   0        0        0     2739 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/model/pipeline_run_response.pyi
+-rw-r--r--   0        0        0      640 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/models/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/paths/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/paths/pipeline_run/__init__.py
+-rw-r--r--   0        0        0    12578 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/paths/pipeline_run/post.py
+-rw-r--r--   0        0        0    12355 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/paths/pipeline_run/post.pyi
+-rw-r--r--   0        0        0      202 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/__init__.py
+-rw-r--r--   0        0        0     3352 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/getters.py
+-rw-r--r--   0        0        0      182 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/llms/__init__.py
+-rw-r--r--   0        0        0    22973 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/llms/openai.py
+-rw-r--r--   0        0        0     3042 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/pipeline.py
+-rw-r--r--   0        0        0     6318 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/pipeline_run.py
+-rw-r--r--   0        0        0      531 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/step_run.py
+-rw-r--r--   0        0        0      695 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/utils.py
+-rw-r--r--   0        0        0      219 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/vectorstores/__init__.py
+-rw-r--r--   0        0        0    10432 2023-04-20 13:08:25.593953 gentrace_py-0.4.1/gentrace/providers/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    10398 2023-04-20 13:08:25.597952 gentrace_py-0.4.1/gentrace/rest.py
+-rw-r--r--   0        0        0   103185 2023-04-20 13:08:25.597952 gentrace_py-0.4.1/gentrace/schemas.py
+-rw-r--r--   0        0        0     1298 2023-04-20 13:08:25.597952 gentrace_py-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.4.1/PKG-INFO
```

### Comparing `gentrace_py-0.4.0/gentrace/__init__.py` & `gentrace_py-0.4.1/gentrace/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/api_client.py` & `gentrace_py-0.4.1/gentrace/api_client.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/configuration.py` & `gentrace_py-0.4.1/gentrace/configuration.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/exceptions.py` & `gentrace_py-0.4.1/gentrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/model/feedback_request.py` & `gentrace_py-0.4.1/gentrace/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/model/feedback_request.pyi` & `gentrace_py-0.4.1/gentrace/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/model/feedback_response.py` & `gentrace_py-0.4.1/gentrace/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/model/feedback_response.pyi` & `gentrace_py-0.4.1/gentrace/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/model/pipeline_run_request.py` & `gentrace_py-0.4.1/gentrace/model/pipeline_run_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/model/pipeline_run_request.pyi` & `gentrace_py-0.4.1/gentrace/model/pipeline_run_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/model/pipeline_run_response.py` & `gentrace_py-0.4.1/gentrace/model/pipeline_run_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/model/pipeline_run_response.pyi` & `gentrace_py-0.4.1/gentrace/model/pipeline_run_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/models/__init__.py` & `gentrace_py-0.4.1/gentrace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/paths/pipeline_run/post.py` & `gentrace_py-0.4.1/gentrace/paths/pipeline_run/post.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/paths/pipeline_run/post.pyi` & `gentrace_py-0.4.1/gentrace/paths/pipeline_run/post.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/providers/getters.py` & `gentrace_py-0.4.1/gentrace/providers/getters.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/providers/llms/openai.py` & `gentrace_py-0.4.1/gentrace/providers/llms/openai.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+import uuid
 from typing import Dict, Optional
 
 import openai
 import pystache
 
 from gentrace.configuration import Configuration
 from gentrace.providers.pipeline import Pipeline
@@ -29,24 +30,26 @@
             for key, value in config.items():
                 setattr(openai, key, value)
 
     def set_pipeline_run(self, pipeline_run):
         self.pipeline_run = pipeline_run
 
 
-def create_step_run(
+def create_completion_step_run(
     cls,
     pipeline_id: str,
     gentrace_config: Configuration,
     start_time,
     end_time,
     base_completion_options,
     prompt_template,
     prompt_inputs,
     completion,
+    pipeline_run_id: Optional[str] = None,
+    stream=False,
 ):
     elapsed_time = int((end_time - start_time) * 1000)
 
     user = base_completion_options.get("user")
     suffix = base_completion_options.get("suffix")
     partial_model_params = {
         k: v for k, v in base_completion_options.items() if k not in ["user", "suffix"]
@@ -67,14 +70,15 @@
             id=pipeline_id,
             api_key=gentrace_config.access_token,
             host=gentrace_config.host,
         )
 
         pipeline_run = PipelineRun(
             pipeline=pipeline,
+            id=pipeline_run_id,
         )
 
     if pipeline_run:
         pipeline_run.add_step_run(
             OpenAICreateCompletionStepRun(
                 elapsed_time,
                 to_date_string(start_time),
@@ -83,19 +87,21 @@
                 {**partial_model_params, "promptTemplate": prompt_template},
                 completion,
             )
         )
 
         if is_self_contained:
             submit_result = pipeline_run.submit()
-            completion.pipeline_run_id = (
-                submit_result["pipelineRunId"]
-                if "pipelineRunId" in submit_result
-                else None
-            )
+
+            if not stream:
+                completion.pipeline_run_id = (
+                    submit_result["pipelineRunId"]
+                    if "pipelineRunId" in submit_result
+                    else None
+                )
 
 
 def create_stream_response(stream_list):
     final_response_string = ""
     for value in stream_list:
         if "choices" in value and value["choices"]:
             first_choice = value["choices"][0]
@@ -128,15 +134,15 @@
 
 
 def intercept_completion(original_fn, gentrace_config: Configuration):
     @classmethod
     def wrapper(cls, *args, **kwargs):
         prompt_template = kwargs.get("prompt_template")
         prompt_inputs = kwargs.get("prompt_inputs")
-        pipeline_id = kwargs.get("pipeline_id")
+        pipeline_id = kwargs.pop("pipeline_id", None)
         stream = kwargs.get("stream")
         base_completion_options = {
             k: v
             for k, v in kwargs.items()
             if k not in ["prompt_template", "prompt_inputs"]
         }
 
@@ -157,70 +163,80 @@
                 **base_completion_options,
                 "prompt": rendered_prompt,
             }
 
             start_time = time.time()
             completion = original_fn(**new_completion_options)
 
+            is_self_contained = not cls.pipeline_run and pipeline_id
+            if is_self_contained:
+                pipeline_run_id = str(uuid.uuid4())
+
             def profiled_completion():
                 modified_response = []
                 for value in completion:
+                    if value and is_self_contained:
+                        value["pipeline_run_id"] = pipeline_run_id
                     modified_response.append(value)
                     yield value
 
                 end_time = time.time()
 
                 full_response = create_stream_response(modified_response)
 
-                create_step_run(
+                create_completion_step_run(
                     cls,
                     pipeline_id,
                     gentrace_config,
                     start_time,
                     end_time,
                     base_completion_options,
                     prompt_template,
                     prompt_inputs,
                     full_response,
+                    pipeline_run_id if is_self_contained else None,
+                    stream,
                 )
 
             return profiled_completion()
 
         rendered_prompt = pystache.render(prompt_template, prompt_inputs)
 
         new_completion_options = {**base_completion_options, "prompt": rendered_prompt}
 
         start_time = time.time()
         completion = original_fn(**new_completion_options)
 
         end_time = time.time()
 
-        create_step_run(
+        create_completion_step_run(
             cls,
             pipeline_id,
             gentrace_config,
             start_time,
             end_time,
             base_completion_options,
             prompt_template,
             prompt_inputs,
             completion,
+            None,
+            stream,
         )
 
         return completion
 
     return wrapper
 
 
 def intercept_completion_async(original_fn, gentrace_config: Configuration):
     @classmethod
     async def wrapper(cls, *args, **kwargs):
         prompt_template = kwargs.get("prompt_template")
         prompt_inputs = kwargs.get("prompt_inputs")
-        pipeline_id = kwargs.get("pipeline_id")
+        pipeline_id = kwargs.pop("pipeline_id", None)
         stream = kwargs.get("stream")
         base_completion_options = {
             k: v
             for k, v in kwargs.items()
             if k not in ["prompt_template", "prompt_inputs"]
         }
 
@@ -241,124 +257,131 @@
                 **base_completion_options,
                 "prompt": rendered_prompt,
             }
 
             start_time = time.time()
             completion = await original_fn(**new_completion_options)
 
+            is_self_contained = not cls.pipeline_run and pipeline_id
+            if is_self_contained:
+                pipeline_run_id = str(uuid.uuid4())
+
             async def profiled_completion():
                 modified_response = []
                 async for value in completion:
+                    if value and is_self_contained:
+                        value["pipeline_run_id"] = pipeline_run_id
                     modified_response.append(value)
                     yield value
 
                 end_time = time.time()
 
                 full_response = create_stream_response(modified_response)
 
-                create_step_run(
+                create_completion_step_run(
                     cls,
                     pipeline_id,
                     gentrace_config,
                     start_time,
                     end_time,
                     base_completion_options,
                     prompt_template,
                     prompt_inputs,
                     full_response,
+                    pipeline_run_id if is_self_contained else None,
+                    stream,
                 )
 
             return profiled_completion()
 
         rendered_prompt = pystache.render(prompt_template, prompt_inputs)
 
         new_completion_options = {**base_completion_options, "prompt": rendered_prompt}
 
         start_time = time.time()
         completion = await original_fn(**new_completion_options)
         end_time = time.time()
 
-        create_step_run(
+        create_completion_step_run(
             cls,
             pipeline_id,
             gentrace_config,
             start_time,
             end_time,
             base_completion_options,
             prompt_template,
             prompt_inputs,
             completion,
+            None,
+            stream,
         )
         return completion
 
     return wrapper
 
 
 def intercept_chat_completion(original_fn, gentrace_config: Configuration):
     @classmethod
     def wrapper(cls, *args, **kwargs):
         messages = kwargs.get("messages")
         user = kwargs.get("user")
-        pipeline_id = kwargs.get("pipeline_id")
+        pipeline_id = kwargs.pop("pipeline_id", None)
         stream = kwargs.get("stream")
 
         model_params = {
             k: v for k, v in kwargs.items() if k not in ["messages", "user"]
         }
 
         if stream:
             start_time = time.time()
             completion = original_fn(**kwargs)
 
+            is_self_contained = not cls.pipeline_run and pipeline_id
+            if is_self_contained:
+                pipeline_run_id = str(uuid.uuid4())
+
             def profiled_completion():
                 modified_response = []
                 for value in completion:
+                    if value and is_self_contained:
+                        value["pipeline_run_id"] = pipeline_run_id
                     modified_response.append(value)
                     yield value
 
                 end_time = time.time()
 
                 elapsed_time = int((end_time - start_time) * 1000)
 
                 pipeline_run = cls.pipeline_run
 
                 full_response = create_stream_response(modified_response)
 
-                is_self_contained = not pipeline_run and pipeline_id
-
                 if is_self_contained:
                     pipeline = Pipeline(
                         id=pipeline_id,
                         api_key=gentrace_config.access_token,
                         host=gentrace_config.host,
                     )
 
-                    pipeline_run = PipelineRun(
-                        pipeline=pipeline,
-                    )
+                    pipeline_run = PipelineRun(pipeline=pipeline, id=pipeline_run_id)
 
                 if pipeline_run:
                     pipeline_run.add_step_run(
                         OpenAICreateChatCompletionStepRun(
                             elapsed_time,
                             to_date_string(start_time),
                             to_date_string(end_time),
                             {"messages": messages, "user": user},
                             model_params,
                             full_response,
                         )
                     )
 
                     if is_self_contained:
-                        submit_result = pipeline_run.submit()
-                        completion.pipeline_run_id = (
-                            submit_result["pipelineRunId"]
-                            if "pipelineRunId" in submit_result
-                            else None
-                        )
+                        pipeline_run.submit()
 
             return profiled_completion()
 
         start_time = time.time()
         completion = original_fn(**kwargs)
 
         end_time = time.time()
@@ -406,49 +429,53 @@
 
 def intercept_chat_completion_async(original_fn, gentrace_config: Configuration):
     @classmethod
     async def wrapper(cls, *args, **kwargs):
         messages = kwargs.get("messages")
         user = kwargs.get("user")
         stream = kwargs.get("stream")
-        pipeline_id = kwargs.get("pipeline_id")
+        pipeline_id = kwargs.pop("pipeline_id", None)
         model_params = {
             k: v for k, v in kwargs.items() if k not in ["messages", "user"]
         }
 
         start_time = time.time()
         completion = await original_fn(**kwargs)
 
         if stream:
+            is_self_contained = not cls.pipeline_run and pipeline_id
+            if is_self_contained:
+                pipeline_run_id = str(uuid.uuid4())
 
             async def profiled_completion():
                 modified_response = []
                 async for value in completion:
+                    if value and is_self_contained:
+                        value["pipeline_run_id"] = pipeline_run_id
                     modified_response.append(value)
                     yield value
 
                 end_time = time.time()
 
                 full_response = create_stream_response(modified_response)
 
                 elapsed_time = int((end_time - start_time) * 1000)
 
                 pipeline_run = cls.pipeline_run
 
-                is_self_contained = not pipeline_run and pipeline_id
-
                 if is_self_contained:
                     pipeline = Pipeline(
                         id=pipeline_id,
                         api_key=gentrace_config.access_token,
                         host=gentrace_config.host,
                     )
 
                     pipeline_run = PipelineRun(
                         pipeline=pipeline,
+                        id=pipeline_run_id,
                     )
 
                 if pipeline_run:
                     pipeline_run.add_step_run(
                         OpenAICreateChatCompletionStepRun(
                             elapsed_time,
                             to_date_string(start_time),
@@ -456,20 +483,15 @@
                             {"messages": messages, "user": user},
                             model_params,
                             full_response,
                         )
                     )
 
                     if is_self_contained:
-                        submit_result = pipeline_run.submit()
-                        completion.pipeline_run_id = (
-                            submit_result["pipelineRunId"]
-                            if "pipelineRunId" in submit_result
-                            else None
-                        )
+                        pipeline_run.submit()
 
             return profiled_completion()
 
         end_time = time.time()
 
         elapsed_time = int((end_time - start_time) * 1000)
 
@@ -512,15 +534,15 @@
     return wrapper
 
 
 def intercept_embedding(original_fn, gentrace_config: Configuration):
     @classmethod
     def wrapper(cls, *args, **kwargs):
         model = kwargs.get("model")
-        pipeline_id = kwargs.get("pipeline_id")
+        pipeline_id = kwargs.pop("pipeline_id", None)
         input_params = {k: v for k, v in kwargs.items() if k not in ["model"]}
 
         start_time = time.time()
         completion = original_fn(**kwargs)
         end_time = time.time()
 
         elapsed_time = int((end_time - start_time) * 1000)
@@ -564,27 +586,25 @@
     return wrapper
 
 
 def intercept_embedding_async(original_fn, gentrace_config: Configuration):
     @classmethod
     async def wrapper(cls, *args, **kwargs):
         model = kwargs.get("model")
-        pipeline_id = kwargs.get("pipeline_id")
+        pipeline_id = kwargs.pop("pipeline_id", None)
         input_params = {k: v for k, v in kwargs.items() if k not in ["model"]}
 
         start_time = time.time()
         completion = await original_fn(**kwargs)
         end_time = time.time()
 
         elapsed_time = int((end_time - start_time) * 1000)
 
         pipeline_run = cls.pipeline_run if hasattr(cls, "pipeline_run") else None
 
-        print("pipeline_run", pipeline_run)
-
         is_self_contained = not pipeline_run and pipeline_id
 
         if is_self_contained:
             pipeline = Pipeline(
                 id=pipeline_id,
                 api_key=gentrace_config.access_token,
                 host=gentrace_config.host,
```

### Comparing `gentrace_py-0.4.0/gentrace/providers/pipeline.py` & `gentrace_py-0.4.1/gentrace/providers/pipeline.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/providers/pipeline_run.py` & `gentrace_py-0.4.1/gentrace/providers/pipeline_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import concurrent
 import copy
 import inspect
 import threading
 import uuid
-from typing import Dict, List, cast
+from typing import Dict, List, Optional, cast
 
 from gentrace.api_client import ApiClient
 from gentrace.apis.tags.ingestion_api import IngestionApi
 from gentrace.configuration import Configuration
 from gentrace.providers.pipeline import Pipeline
 from gentrace.providers.step_run import StepRun
 from gentrace.providers.utils import pipeline_run_post_background
@@ -33,16 +33,17 @@
     if _pipeline_tasks:
         # Wait for all tasks to complete
         concurrent.futures.wait(_pipeline_tasks)
         _pipeline_tasks.clear()
 
 
 class PipelineRun:
-    def __init__(self, pipeline):
+    def __init__(self, pipeline, id: Optional[str] = None):
         self.pipeline: Pipeline = pipeline
+        self.pipeline_run_id: str = id or str(uuid.uuid4())
         self.step_runs: List[StepRun] = []
 
     def get_pipeline(self):
         return self.pipeline
 
     def get_openai(self):
         if "openai" in self.pipeline.pipeline_handlers:
@@ -143,35 +144,33 @@
                 "elapsedTime": step_run.elapsed_time,
                 "startTime": step_run.start_time,
                 "endTime": step_run.end_time,
             }
             for step_run in self.step_runs
         ]
 
-        pipeline_run_id = str(uuid.uuid4())
-
         if not wait_for_server:
             fire_and_forget(
                 pipeline_run_post_background(
                     ingestion_api,
                     {
-                        "id": pipeline_run_id,
+                        "id": self.pipeline_run_id,
                         "name": self.pipeline.id,
                         "stepRuns": step_runs_data,
                     },
                 )
             )
 
-            return {"pipelineRunId": pipeline_run_id}
+            return {"pipelineRunId": self.pipeline_run_id}
 
         if wait_for_server:
             try:
                 pipeline_post_response = ingestion_api.pipeline_run_post(
                     {
-                        "id": pipeline_run_id,
+                        "id": self.pipeline_run_id,
                         "name": self.pipeline.id,
                         "stepRuns": step_runs_data,
                     }
                 )
                 return {
                     "pipelineRunId": pipeline_post_response.body.get_item_oapg(
                         "pipelineRunId"
```

### Comparing `gentrace_py-0.4.0/gentrace/providers/step_run.py` & `gentrace_py-0.4.1/gentrace/providers/step_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/providers/utils.py` & `gentrace_py-0.4.1/gentrace/providers/utils.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/providers/vectorstores/pinecone.py` & `gentrace_py-0.4.1/gentrace/providers/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/rest.py` & `gentrace_py-0.4.1/gentrace/rest.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/gentrace/schemas.py` & `gentrace_py-0.4.1/gentrace/schemas.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.4.0/pyproject.toml` & `gentrace_py-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Python SDK for the Gentrace API"
 license = "MIT"
 name = "gentrace-py"
 packages = [
   {include = "gentrace"},
 ]
 repository = "https://github.com/gentrace/gentrace-python"
-version = "0.4.0"
+version = "0.4.1"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 frozendict = "^2.3.7"
 pydantic = ">=1.10.2"
 pystache = "^0.6.0"
 python = ">=3.8.1,<4.0"
```

### Comparing `gentrace_py-0.4.0/PKG-INFO` & `gentrace_py-0.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentrace-py
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python SDK for the Gentrace API
 Home-page: https://github.com/gentrace/gentrace-python
 License: MIT
 Author: Gentrace
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

