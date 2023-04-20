# Comparing `tmp/magnus_extensions-0.2.7.tar.gz` & `tmp/magnus_extensions-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnus_extensions-0.2.7.tar", max compression
+gzip compressed data, was "magnus_extensions-0.2.8.tar", max compression
```

## Comparing `magnus_extensions-0.2.7.tar` & `magnus_extensions-0.2.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-03-21 15:03:11.366295 magnus_extensions-0.2.7/LICENSE
--rw-r--r--   0        0        0     2304 2023-03-21 15:03:11.366295 magnus_extensions-0.2.7/README.md
--rw-r--r--   0        0        0     5339 2023-03-21 15:03:11.374296 magnus_extensions-0.2.7/magnus_extensions/aws.py
--rw-r--r--   0        0        0      718 2023-03-21 15:03:11.374296 magnus_extensions-0.2.7/magnus_extensions/catalog/k8s_pvc/implementation.py
--rw-r--r--   0        0        0     1952 2023-03-21 15:03:11.374296 magnus_extensions-0.2.7/magnus_extensions/catalog/k8s_pvc/integration.py
--rw-r--r--   0        0        0     7820 2023-03-21 15:03:11.374296 magnus_extensions-0.2.7/magnus_extensions/catalog/s3/implementation.py
--rw-r--r--   0        0        0      632 2023-03-21 15:03:11.374296 magnus_extensions-0.2.7/magnus_extensions/catalog/s3/integration.py
--rw-r--r--   0        0        0      598 2023-03-21 15:03:11.374296 magnus_extensions-0.2.7/magnus_extensions/datastore/chunked_k8s_pvc/implementation.py
--rw-r--r--   0        0        0     2020 2023-03-21 15:03:11.374296 magnus_extensions-0.2.7/magnus_extensions/datastore/chunked_k8s_pvc/integration.py
--rw-r--r--   0        0        0     7953 2023-03-21 15:03:11.374296 magnus_extensions-0.2.7/magnus_extensions/datastore/chunked_s3/implementation.py
--rw-r--r--   0        0        0      777 2023-03-21 15:03:11.374296 magnus_extensions-0.2.7/magnus_extensions/datastore/chunked_s3/integration.py
--rw-r--r--   0        0        0    18942 2023-03-21 15:03:11.374296 magnus_extensions-0.2.7/magnus_extensions/datastore/db/implementation.py
--rw-r--r--   0        0        0      818 2023-03-21 15:03:11.374296 magnus_extensions-0.2.7/magnus_extensions/datastore/db/integration.py
--rw-r--r--   0        0        0      562 2023-03-21 15:03:11.374296 magnus_extensions-0.2.7/magnus_extensions/datastore/k8s_pvc/implementation.py
--rw-r--r--   0        0        0     2013 2023-03-21 15:03:11.374296 magnus_extensions-0.2.7/magnus_extensions/datastore/k8s_pvc/integration.py
--rw-r--r--   0        0        0     5037 2023-03-21 15:03:11.378296 magnus_extensions-0.2.7/magnus_extensions/datastore/s3/implementation.py
--rw-r--r--   0        0        0     1868 2023-03-21 15:03:11.378296 magnus_extensions-0.2.7/magnus_extensions/datastore/s3/integration.py
--rw-r--r--   0        0        0    15783 2023-03-21 15:03:11.378296 magnus_extensions-0.2.7/magnus_extensions/executor/argo/implementation.py
--rw-r--r--   0        0        0     1589 2023-03-21 15:03:11.378296 magnus_extensions-0.2.7/magnus_extensions/executor/argo/integration.py
--rw-r--r--   0        0        0     8955 2023-03-21 15:03:11.378296 magnus_extensions-0.2.7/magnus_extensions/executor/k8s_job/implementation.py
--rw-r--r--   0        0        0     2169 2023-03-21 15:03:11.378296 magnus_extensions-0.2.7/magnus_extensions/executor/k8s_job/integration.py
--rw-r--r--   0        0        0    13340 2023-03-21 15:03:11.378296 magnus_extensions-0.2.7/magnus_extensions/executor/kubeflow/implementation.py
--rw-r--r--   0        0        0     1577 2023-03-21 15:03:11.378296 magnus_extensions-0.2.7/magnus_extensions/executor/kubeflow/integration.py
--rw-r--r--   0        0        0     3364 2023-03-21 15:03:11.378296 magnus_extensions-0.2.7/magnus_extensions/experiment_tracker/mlflow/implementation.py
--rw-r--r--   0        0        0       87 2023-03-21 15:03:11.378296 magnus_extensions-0.2.7/magnus_extensions/magnus_extension_template/implementation.py
--rw-r--r--   0        0        0       47 2023-03-21 15:03:11.378296 magnus_extensions-0.2.7/magnus_extensions/magnus_extension_template/integration.py
--rw-r--r--   0        0        0     2623 2023-03-21 15:03:11.378296 magnus_extensions-0.2.7/magnus_extensions/secrets/aws/implementation.py
--rw-r--r--   0        0        0      641 2023-03-21 15:03:11.378296 magnus_extensions-0.2.7/magnus_extensions/secrets/aws/integration.py
--rw-r--r--   0        0        0     4996 2023-03-21 15:03:30.159503 magnus_extensions-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 magnus_extensions-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-20 13:10:43.146381 magnus_extensions-0.2.8/LICENSE
+-rw-r--r--   0        0        0     2304 2023-04-20 13:10:43.146381 magnus_extensions-0.2.8/README.md
+-rw-r--r--   0        0        0     5339 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/aws.py
+-rw-r--r--   0        0        0      718 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/catalog/k8s_pvc/implementation.py
+-rw-r--r--   0        0        0     1952 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/catalog/k8s_pvc/integration.py
+-rw-r--r--   0        0        0     7820 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/catalog/s3/implementation.py
+-rw-r--r--   0        0        0      632 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/catalog/s3/integration.py
+-rw-r--r--   0        0        0      598 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_k8s_pvc/implementation.py
+-rw-r--r--   0        0        0     2020 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_k8s_pvc/integration.py
+-rw-r--r--   0        0        0     7953 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_s3/implementation.py
+-rw-r--r--   0        0        0      777 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_s3/integration.py
+-rw-r--r--   0        0        0    18942 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/db/implementation.py
+-rw-r--r--   0        0        0      818 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/db/integration.py
+-rw-r--r--   0        0        0      562 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/k8s_pvc/implementation.py
+-rw-r--r--   0        0        0     2013 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/k8s_pvc/integration.py
+-rw-r--r--   0        0        0     5037 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/s3/implementation.py
+-rw-r--r--   0        0        0     1868 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/s3/integration.py
+-rw-r--r--   0        0        0    16160 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/executor/argo/implementation.py
+-rw-r--r--   0        0        0     1589 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/executor/argo/integration.py
+-rw-r--r--   0        0        0     9776 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/executor/k8s_job/implementation.py
+-rw-r--r--   0        0        0     2169 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/executor/k8s_job/integration.py
+-rw-r--r--   0        0        0    13340 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/executor/kubeflow/implementation.py
+-rw-r--r--   0        0        0     1577 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/executor/kubeflow/integration.py
+-rw-r--r--   0        0        0     3364 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/experiment_tracker/mlflow/implementation.py
+-rw-r--r--   0        0        0       87 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/magnus_extension_template/implementation.py
+-rw-r--r--   0        0        0       47 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/magnus_extension_template/integration.py
+-rw-r--r--   0        0        0     2623 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/secrets/aws/implementation.py
+-rw-r--r--   0        0        0      641 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/secrets/aws/integration.py
+-rw-r--r--   0        0        0     4996 2023-04-20 13:11:00.795077 magnus_extensions-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 magnus_extensions-0.2.8/PKG-INFO
```

### Comparing `magnus_extensions-0.2.7/LICENSE` & `magnus_extensions-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/README.md` & `magnus_extensions-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/aws.py` & `magnus_extensions-0.2.8/magnus_extensions/aws.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/catalog/k8s_pvc/implementation.py` & `magnus_extensions-0.2.8/magnus_extensions/catalog/k8s_pvc/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/catalog/k8s_pvc/integration.py` & `magnus_extensions-0.2.8/magnus_extensions/catalog/k8s_pvc/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/catalog/s3/implementation.py` & `magnus_extensions-0.2.8/magnus_extensions/catalog/s3/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/catalog/s3/integration.py` & `magnus_extensions-0.2.8/magnus_extensions/catalog/s3/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/datastore/chunked_k8s_pvc/implementation.py` & `magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_k8s_pvc/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/datastore/chunked_k8s_pvc/integration.py` & `magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_k8s_pvc/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/datastore/chunked_s3/implementation.py` & `magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_s3/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/datastore/chunked_s3/integration.py` & `magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_s3/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/datastore/db/implementation.py` & `magnus_extensions-0.2.8/magnus_extensions/datastore/db/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/datastore/db/integration.py` & `magnus_extensions-0.2.8/magnus_extensions/datastore/db/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/datastore/k8s_pvc/implementation.py` & `magnus_extensions-0.2.8/magnus_extensions/datastore/k8s_pvc/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/datastore/k8s_pvc/integration.py` & `magnus_extensions-0.2.8/magnus_extensions/datastore/k8s_pvc/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/datastore/s3/implementation.py` & `magnus_extensions-0.2.8/magnus_extensions/datastore/s3/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/datastore/s3/integration.py` & `magnus_extensions-0.2.8/magnus_extensions/datastore/s3/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/executor/argo/implementation.py` & `magnus_extensions-0.2.8/magnus_extensions/executor/argo/implementation.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,30 +17,25 @@
     secret_name: str
     secret_key: str
 
     def dict(self, *args, **kwargs):
         return {
             "name": self.environment_variable,
             "valueFrom": {
-                "secretKeyRef": {
-                    "name": self.secret_name,
-                    "key": self.secret_key
-                }
-            }
+                "secretKeyRef": {"name": self.secret_name, "key": self.secret_key}
+            },
         }
 
 
 class EnvVar(BaseModel):
     name: str
     value: Any
 
     def dict(self, *args, **kwargs):
-        return_value = {
-            "name": self.name
-        }
+        return_value = {"name": self.name}
 
         if self.value:
             return_value["value"] = self.value
 
         return return_value
 
 
@@ -51,18 +46,15 @@
 
 class Limit(BaseModel):
     memory: str
     cpu: str
     gpu: int = 0
 
     def dict(self, *args, **kwargs) -> dict:
-        resource = {
-            "cpu": self.cpu,
-            "memory": self.memory
-        }
+        resource = {"cpu": self.cpu, "memory": self.memory}
         if self.gpu:
             # TODO: This should be via config to allow users to specify the vendor
             resource["nvidia.com/gpu"] = self.gpu
 
         return resource
 
 
@@ -84,57 +76,57 @@
     def dict(self, *args, **kwargs) -> dict:
         return {
             "command": self.command,
             "image": self.image,
             "imagePullPolicy": self.imagePullPolicy,
             "resources": {
                 "limits": self.limits.dict(),
-                "requests": self.requests.dict()
+                "requests": self.requests.dict(),
             },
             "retryStrategy": {"limit": str(self.retry)},
             "env": [e.dict() for e in self.env],
-            "volumeMounts": [v.dict() for v in self.volumeMounts]
+            "volumeMounts": [v.dict() for v in self.volumeMounts],
         }
 
 
 class TaskTemplate(BaseModel):
     name: str
     template: str
-    dependencies: List[str] = []
+    depends: List[str] = []
+
+    def dict(self, *args, **kwargs) -> dict:
+        return {
+            "name": self.name,
+            "template": self.template,
+            "depends": " || ".join(self.depends),
+        }
 
 
 class ContainerTemplate(BaseModel):
     name: str
     container: Container
 
 
 class DagTemplate(BaseModel):
     name: str = "magnus-dag"
     tasks: List[TaskTemplate] = []
 
     def dict(self, *args, **kwargs):
         return {
             "name": self.name,
-            "dag": {
-                "tasks": [task.dict() for task in self.tasks]
-            }
+            "dag": {"tasks": [task.dict() for task in self.tasks]},
         }
 
 
 class Volume(BaseModel):
     name: str
     claim: str
 
     def dict(self, *args, **kwargs) -> dict:
-        return {
-            "name": self.name,
-            "persistentVolumeClaim": {
-                "claimName": self.claim
-            }
-        }
+        return {"name": self.name, "persistentVolumeClaim": {"claimName": self.claim}}
 
 
 class Spec(BaseModel):
     entrypoint: str = "magnus-dag"
     templates: Union[DagTemplate, ContainerTemplate] = []
     serviceAccountName: str = "pipeline-runner"
     arguments: List[EnvVar] = []
@@ -142,50 +134,49 @@
 
     def dict(self, *args, **kwargs):
         return {
             "entrypoint": self.entrypoint,
             "volumes": [v.dict() for v in self.volumes],
             "templates": [template.dict() for template in self.templates],
             "serviceAccountName": self.serviceAccountName,
-            "arguments": {
-                "parameters": [env.dict() for env in self.arguments]
-            }
+            "arguments": {"parameters": [env.dict() for env in self.arguments]},
         }
 
 
 class WorkSpec(BaseModel):
     apiVersion: str = "argoproj.io/v1alpha1"
     kind: str = "Workflow"
     metadata: dict = {"generateName": "magnus-dag-"}
     spec: Optional[Spec]
 
 
 class ArgoExecutor(BaseExecutor):
-
     service_name = "argo"
     run_id_placeholder = "{{workflow.parameters.run_id}}"
 
     class Config(BaseExecutor.Config):
         docker_image: str
-        output_file: str = 'pipeline.yaml'
+        output_file: str = "pipeline.yaml"
         cpu_limit: str = "250m"
         memory_limit: str = "1G"
         cpu_request: str = ""
         memory_request: str = ""
         gpu_limit: int = 0
         enable_caching: bool = False
         image_pull_policy: str = "Always"
         secrets_from_k8s: dict = {}  # EnvVar=SecretName:Key
         persistent_volumes: dict = {}  # volume-name:mount_path
 
     def __init__(self, config: dict = None):
         super().__init__(config)
         self.persistent_volumes = {}
 
-        for i, (volume_name, mount_path) in enumerate(self.config.persistent_volumes.items()):
+        for i, (volume_name, mount_path) in enumerate(
+            self.config.persistent_volumes.items()
+        ):
             self.persistent_volumes[f"executor-{i}"] = (volume_name, mount_path)
 
     def prepare_for_graph_execution(self):
         """
         This method would be called prior to calling execute_graph.
         Perform any steps required before doing the graph execution.
 
@@ -226,152 +217,184 @@
 
         integration.validate(self, self.experiment_tracker)
         integration.configure_for_execution(self, self.experiment_tracker)
 
         self._set_up_run_log(exists_ok=True)
 
     def execute_node(self, node: BaseNode, map_variable: dict = None, **kwargs):
-        step_log = self.run_log_store.create_step_log(node.name, node._get_step_log_name(map_variable))
+        step_log = self.run_log_store.create_step_log(
+            node.name, node._get_step_log_name(map_variable)
+        )
 
         self.add_code_identities(node=node, step_log=step_log)
 
         step_log.step_type = node.node_type
         step_log.status = defaults.PROCESSING
         self.run_log_store.add_step_log(step_log, self.run_id)
 
         super()._execute_node(node, map_variable=map_variable, **kwargs)
 
         # Implicit fail
         if self.dag:
             # functions and notebooks do not have dags
-            _, next_node_name = self._get_status_and_next_node_name(node, self.dag, map_variable=map_variable)
+            _, next_node_name = self._get_status_and_next_node_name(
+                node, self.dag, map_variable=map_variable
+            )
             if next_node_name:
                 # Terminal nodes do not have next node name
                 next_node = self.dag.get_node_by_name(next_node_name)
 
                 if next_node.node_type == defaults.FAIL:
                     self.execute_node(next_node, map_variable=map_variable)
 
-        step_log = self.run_log_store.get_step_log(node._get_step_log_name(map_variable), self.run_id)
+        step_log = self.run_log_store.get_step_log(
+            node._get_step_log_name(map_variable), self.run_id
+        )
         if step_log.status == defaults.FAIL:
-            raise Exception(f'Step {node.name} failed')
+            raise Exception(f"Step {node.name} failed")
 
     def get_parameters(self):
         parameters = utils.get_user_set_parameters()
         if self.parameters_file:
             parameters.update(utils.load_yaml(self.parameters_file))
         return parameters
 
     def get_clean_name(self, node_name: str):
         return node_name.replace(" ", "-")
 
-    def create_container_template(self, working_on: BaseNode, command: str, add_parameters: bool = False):
+    def create_container_template(
+        self, working_on: BaseNode, command: str, add_parameters: bool = False
+    ):
         command = shlex.split(command)
-        mode_config = self._resolve_node_config(working_on)
+        mode_config = self._resolve_executor_config(working_on)
         secrets = mode_config.get("secrets_from_k8s", {})
 
-        docker_image = mode_config['docker_image']
-        cpu_limit = mode_config.get('cpu_limit', self.config.cpu_limit)
-        memory_limit = mode_config.get('memory_limit', self.config.memory_limit)
-
-        cpu_request = mode_config.get('cpu_request', self.config.cpu_request) or cpu_limit
-        memory_request = mode_config.get('memory_request', self.config.memory_request) or memory_limit
+        docker_image = mode_config["docker_image"]
+        cpu_limit = mode_config.get("cpu_limit", self.config.cpu_limit)
+        memory_limit = mode_config.get("memory_limit", self.config.memory_limit)
+
+        cpu_request = (
+            mode_config.get("cpu_request", self.config.cpu_request) or cpu_limit
+        )
+        memory_request = (
+            mode_config.get("memory_request", self.config.memory_request)
+            or memory_limit
+        )
 
-        gpu_limit = mode_config.get('gpu_limit', self.config.gpu_limit)
+        gpu_limit = mode_config.get("gpu_limit", self.config.gpu_limit)
 
         request = Request(memory=memory_request, cpu=cpu_request)
         limits = Limit(memory=memory_limit, cpu=cpu_limit, gpu=gpu_limit)
 
-        image_pull_policy = mode_config.get("image_pull_policy", self.config.image_pull_policy)
-
-        container = Container(command=command, image=docker_image, limits=limits, requests=request,
-                              imagePullPolicy=image_pull_policy, retry=working_on._get_max_attempts())
+        image_pull_policy = mode_config.get(
+            "image_pull_policy", self.config.image_pull_policy
+        )
+
+        container = Container(
+            command=command,
+            image=docker_image,
+            limits=limits,
+            requests=request,
+            imagePullPolicy=image_pull_policy,
+            retry=working_on._get_max_attempts(),
+        )
         for secret_env, k8_secret in secrets.items():
             try:
-                secret_name, key = k8_secret.split(':')
+                secret_name, key = k8_secret.split(":")
             except Exception as _e:
-                msg = (
-                    "K8's secret should be of format EnvVar=SecretName:Key"
-                )
+                msg = "K8's secret should be of format EnvVar=SecretName:Key"
                 raise Exception(msg) from _e
-            secret = SecretEnvVar(environment_variable=secret_env, secret_name=secret_name, secret_key=key)
+            secret = SecretEnvVar(
+                environment_variable=secret_env, secret_name=secret_name, secret_key=key
+            )
             container.env.append(secret)
 
-        if add_parameters or working_on.name == self.dag.start_at:  # short circuit when forcing to add parameters
+        if (
+            add_parameters or working_on.name == self.dag.start_at
+        ):  # short circuit when forcing to add parameters
             for key, _ in self.get_parameters().items():
                 # Get the value from work flow parameters for dynamic behavior
-                env_var = EnvVar(name=defaults.PARAMETER_PREFIX + key, value="{{workflow.parameters." + key + "}}")
+                env_var = EnvVar(
+                    name=defaults.PARAMETER_PREFIX + key,
+                    value="{{workflow.parameters." + key + "}}",
+                )
                 container.env.append(env_var)
 
         visited_claims = {}
         for volume_name, claim in self.persistent_volumes.items():
             claim_name, mount_path = claim
 
             # If the volume is already mounted, we cannot mount it again.
             if claim_name in visited_claims:
-                msg = (
-                    "The same persistent volume claim has already been used in the pipeline by another service"
-                )
+                msg = "The same persistent volume claim has already been used in the pipeline by another service"
                 raise Exception(msg)
             visited_claims[claim_name] = claim_name
 
-            container.volumeMounts.append(VolumeMount(name=volume_name, mountPath=mount_path))
-
-        container_template = ContainerTemplate(name=self.get_clean_name(working_on.name), container=container)
+            container.volumeMounts.append(
+                VolumeMount(name=volume_name, mountPath=mount_path)
+            )
+
+        container_template = ContainerTemplate(
+            name=self.get_clean_name(working_on.name), container=container
+        )
 
         return container_template
 
     def get_templates(self, dag):
         current_node = dag.start_at
         previous_node = None
 
         container_templates = {}
         task_templates = {}
         while True:
             working_on = dag.get_node_by_name(current_node)
             if working_on.is_composite:
-                raise NotImplementedError('Composite nodes are not yet implemented')
+                raise NotImplementedError("Composite nodes are not yet implemented")
 
             if previous_node == current_node:
-                raise Exception('Potentially running in a infinite loop')
+                raise Exception("Potentially running in a infinite loop")
 
-            command = utils.get_node_execution_command(self, working_on,
-                                                       over_write_run_id=self.run_id_placeholder)
-            container_template = self.create_container_template(working_on=working_on, command=command)
+            command = utils.get_node_execution_command(
+                self, working_on, over_write_run_id=self.run_id_placeholder
+            )
+            container_template = self.create_container_template(
+                working_on=working_on, command=command
+            )
 
             if current_node not in container_templates:
                 container_templates[current_node] = container_template
 
             clean_name = self.get_clean_name(working_on.name)
             task_template = TaskTemplate(name=clean_name, template=clean_name)
             if previous_node:
-                task_template.dependencies.append(self.get_clean_name(previous_node))
+                task_template.depends.append(
+                    f"{self.get_clean_name(previous_node)}.Succeeded"
+                )
 
             task_templates[current_node] = task_template
 
             previous_node = current_node
 
-            if working_on.node_type in ['success', 'fail']:
+            if working_on.node_type in ["success", "fail"]:
                 break
 
             current_node = working_on._get_next_node()
 
-        return [template for k, template in container_templates.items()], \
-            [template for k, template in task_templates.items()]
+        return [template for _, template in container_templates.items()], [
+            template for _, template in task_templates.items()
+        ]
 
     def add_volumes_to_specification(self, specification: Spec):
         visited_claims = {}
         for volume_name, claim in self.persistent_volumes.items():
             claim_name, mount_path = claim
 
             # If the volume is already mounted, we cannot mount it again.
             if claim_name in visited_claims:
-                msg = (
-                    "The same persistent volume claim has already been used in the pipeline by another service"
-                )
+                msg = "The same persistent volume claim has already been used in the pipeline by another service"
                 raise Exception(msg)
             visited_claims[claim_name] = claim_name
             specification.volumes.append(Volume(name=volume_name, claim=claim_name))
 
     def execute_graph(self, dag: Graph, map_variable: dict = None, **kwargs):
         workspec = WorkSpec()
         specification = Spec()
@@ -389,15 +412,15 @@
         self.add_volumes_to_specification(specification)
 
         container_templates, task_templates = self.get_templates(dag=dag)
         specification.templates.extend(container_templates)
         dag_template = DagTemplate(tasks=task_templates)
         specification.templates.extend([dag_template])
         yaml = YAML()
-        with open(self.config.output_file, 'w') as f:
+        with open(self.config.output_file, "w") as f:
             yaml.dump(workspec.dict(), f)
 
     def execute_job(self, node: BaseNode):
         workspec = WorkSpec()
         specification = Spec()
         workspec.spec = specification
 
@@ -408,33 +431,39 @@
 
         run_id_var = EnvVar(name="run_id", value="{{workflow.uid}}")
         specification.arguments.append(run_id_var)
 
         # Add volumes to specification
         self.add_volumes_to_specification(specification)
 
-        command = utils.get_job_execution_command(self, node, over_write_run_id=self.run_id_placeholder)
-        container_template = self.create_container_template(working_on=node, command=command, add_parameters=True)
+        command = utils.get_job_execution_command(
+            self, node, over_write_run_id=self.run_id_placeholder
+        )
+        container_template = self.create_container_template(
+            working_on=node, command=command, add_parameters=True
+        )
 
         clean_name = self.get_clean_name(node.name)
         task_template = TaskTemplate(name=clean_name, template=clean_name)
 
         specification.templates.extend([container_template])
         dag_template = DagTemplate(tasks=[task_template])
         specification.templates.extend([dag_template])
         yaml = YAML()
-        with open(self.config.output_file, 'w') as f:
+        with open(self.config.output_file, "w") as f:
             yaml.dump(workspec.dict(), f)
 
-    def send_return_code(self, stage='traversal'):
+    def send_return_code(self, stage="traversal"):
         """
         Convenience function used by pipeline to send return code to the caller of the cli
 
         Raises:
             Exception: If the pipeline execution failed
         """
-        if stage != 'traversal':  # traversal does no actual execution, so return code is pointless
+        if (
+            stage != "traversal"
+        ):  # traversal does no actual execution, so return code is pointless
             run_id = self.run_id
 
             run_log = self.run_log_store.get_run_log_by_id(run_id=run_id, full=False)
             if run_log.status == defaults.FAIL:
-                raise Exception('Pipeline execution failed')
+                raise Exception("Pipeline execution failed")
```

### Comparing `magnus_extensions-0.2.7/magnus_extensions/executor/argo/integration.py` & `magnus_extensions-0.2.8/magnus_extensions/executor/argo/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/executor/k8s_job/implementation.py` & `magnus_extensions-0.2.8/magnus_extensions/executor/k8s_job/implementation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-
 import logging
 import shlex
 from typing import Dict, List
 
 from magnus import defaults, integration, utils
 from magnus.executor import BaseExecutor
 from magnus.graph import Graph
 from magnus.nodes import BaseNode
+from pydantic import BaseModel
 from ruamel.yaml import YAML
 
 logger = logging.getLogger(defaults.NAME)
 
 try:
     from kubernetes import client
     from kubernetes import config as k8s_config
     from kubernetes.client import (V1EnvVar, V1EnvVarSource,
                                    V1PersistentVolumeClaimVolumeSource,
                                    V1SecretKeySelector)
 except ImportError as _e:
-    msg = (
-        "Kubernetes Dependencies have not been installed!!"
-    )
+    msg = "Kubernetes Dependencies have not been installed!!"
     raise Exception(msg) from _e
 
 
-class K8sJobExecutor(BaseExecutor):
+class Toleration(BaseModel):
+    effect: str
+    key: str
+    operator: str
+    value: str
 
+
+class K8sJobExecutor(BaseExecutor):
     service_name = "k8s-job"
 
     class Config(BaseExecutor.Config):
         config_path: str
         docker_image: str
         namespace: str = "default"
         cpu_limit: str = "250m"
@@ -39,14 +43,16 @@
         cpu_request: str = ""
         memory_request: str = ""
         active_deadline_seconds: int = 60 * 60 * 2  # 2 hours
         ttl_seconds_after_finished: int = 60  #  1 minute
         image_pull_policy: str = "Always"
         secrets_from_k8s: dict = {}  # EnvVar=SecretName:Key
         persistent_volumes: dict = {}  # volume-name:mount_path
+        node_selector: Dict[str, str] = {}
+        tolerations: List[Toleration] = []
         labels: Dict[str, str] = {}
 
     def __init__(self, config: dict = None):
         super().__init__(config)
         self.persistent_volumes = {}
 
         for i, (claim, mount_path) in enumerate(self.config.persistent_volumes.items()):
@@ -98,125 +104,166 @@
         self._set_up_run_log(exists_ok=True)
 
     @property
     def _client(self):
         k8s_config.load_kube_config(config_file=self.config.config_path)
         return client
 
+    @property
+    def tolerations(self):
+        return [toleration.dict() for toleration in self.config.tolerations]
+
     def execute_job(self, node: BaseNode):
         command = utils.get_job_execution_command(self, node)
-        logger.info(f'Triggering a kubernetes job with : {command}')
+        logger.info(f"Triggering a kubernetes job with : {command}")
 
-        self.config.labels['job_name'] = self.run_id
+        self.config.labels["job_name"] = self.run_id
 
         k8s_batch = self._client.BatchV1Api()
 
         cpu_limit = self.config.cpu_limit
         memory_limit = self.config.memory_limit
 
         cpu_request = self.config.cpu_request or cpu_limit
         memory_request = self.config.memory_request or memory_limit
 
         gpu_limit = str(self.config.gpu_limit)  # Should be something like nvidia -etc
 
-        limits = {"cpu": cpu_limit, "memory": memory_limit, self.config.gpu_vendor: gpu_limit}
+        limits = {
+            "cpu": cpu_limit,
+            "memory": memory_limit,
+            self.config.gpu_vendor: gpu_limit,
+        }
         requests = {"cpu": cpu_request, "memory": memory_request}
         resources = {"limits": limits, "requests": requests}
 
         environment_variables = []
         for secret_env, k8_secret in self.config.secrets_from_k8s.items():
             try:
-                secret_name, key = k8_secret.split(':')
+                secret_name, key = k8_secret.split(":")
             except Exception as _e:
-                msg = (
-                    "K8's secret should be of format EnvVar=SecretName:Key"
-                )
+                msg = "K8's secret should be of format EnvVar=SecretName:Key"
                 raise Exception(msg) from _e
-            secret_as_env = V1EnvVar(name=secret_env, value_from=V1EnvVarSource(
-                secret_key_ref=V1SecretKeySelector(name=secret_name, key=key)))
+            secret_as_env = V1EnvVar(
+                name=secret_env,
+                value_from=V1EnvVarSource(
+                    secret_key_ref=V1SecretKeySelector(name=secret_name, key=key)
+                ),
+            )
             environment_variables.append(secret_as_env)
 
         overridden_params = utils.get_user_set_parameters()
         # The parameters present in the environment override the parameters present in the parameters file
         # The values are coerced to be strings, hopefully they will be fine on the other side.
         for k, v in overridden_params.items():
-            environment_variables.append(V1EnvVar(name=defaults.PARAMETER_PREFIX+k, value=str(v)))
+            environment_variables.append(
+                V1EnvVar(name=defaults.PARAMETER_PREFIX + k, value=str(v))
+            )
 
         pod_volumes = []
         volume_mounts = []
         for claim_name, (claim, mount_path) in self.persistent_volumes.items():
-            pod_volumes.append(self._client.V1Volume(
-                name=claim_name, persistent_volume_claim=V1PersistentVolumeClaimVolumeSource(claim_name=claim)))
-            volume_mounts.append(self._client.V1VolumeMount(name=claim_name, mount_path=mount_path))
+            pod_volumes.append(
+                self._client.V1Volume(
+                    name=claim_name,
+                    persistent_volume_claim=V1PersistentVolumeClaimVolumeSource(
+                        claim_name=claim
+                    ),
+                )
+            )
+            volume_mounts.append(
+                self._client.V1VolumeMount(name=claim_name, mount_path=mount_path)
+            )
 
         base_container = self._client.V1Container(
             name=self.run_id,
             image=self.config.docker_image,
             command=shlex.split(command),
             resources=resources,
             env=environment_variables,
             image_pull_policy="Always",
-            volume_mounts=volume_mounts or None
+            volume_mounts=volume_mounts or None,
         )
 
-        pod_spec = self._client.V1PodSpec(volumes=pod_volumes or None,
-                                          restart_policy='Never',
-                                          containers=[base_container])
+        pod_spec = self._client.V1PodSpec(
+            volumes=pod_volumes or None,
+            restart_policy="Never",
+            containers=[base_container],
+            node_selector=self.config.node_selector,
+            tolerations=self.tolerations,
+        )
 
-        pod_template = self._client.V1PodTemplateSpec(metadata=client.V1ObjectMeta(
-            labels=self.config.labels, annotations={"sidecar.istio.io/inject": "false"}), spec=pod_spec)
+        pod_template = self._client.V1PodTemplateSpec(
+            metadata=client.V1ObjectMeta(
+                labels=self.config.labels,
+                annotations={"sidecar.istio.io/inject": "false"},
+            ),
+            spec=pod_spec,
+        )
 
-        job_spec = client.V1JobSpec(template=pod_template, backoff_limit=2,
-                                    ttl_seconds_after_finished=self.config.ttl_seconds_after_finished)
+        job_spec = client.V1JobSpec(
+            template=pod_template,
+            backoff_limit=2,
+            ttl_seconds_after_finished=self.config.ttl_seconds_after_finished,
+        )
         job_spec.active_deadline_seconds = self.config.active_deadline_seconds
 
         job = client.V1Job(
-            api_version='batch/v1',
-            kind='Job',
+            api_version="batch/v1",
+            kind="Job",
             metadata=client.V1ObjectMeta(name=self.run_id),
-            spec=job_spec)
+            spec=job_spec,
+        )
 
-        logger.debug(f'Submitting kubernetes job: {job}')
+        logger.debug(f"Submitting kubernetes job: {job}")
 
         try:
             response = k8s_batch.create_namespaced_job(
-                body=job, namespace=self.config.namespace, _preload_content=False, pretty=True)
-            print(f'Kubernetes job {self.run_id} created')
-            logger.debug(f'Kubernetes job response: {response}')
+                body=job,
+                namespace=self.config.namespace,
+                _preload_content=False,
+                pretty=True,
+            )
+            print(f"Kubernetes job {self.run_id} created")
+            logger.debug(f"Kubernetes job response: {response}")
         except Exception as e:
             logger.exception(e)
             raise
 
     def execute_node(self, node: BaseNode, map_variable: dict = None, **kwargs):
-        step_log = self.run_log_store.create_step_log(node.name, node._get_step_log_name(map_variable))
+        step_log = self.run_log_store.create_step_log(
+            node.name, node._get_step_log_name(map_variable)
+        )
 
         self.add_code_identities(node=node, step_log=step_log)
 
         step_log.step_type = node.node_type
         step_log.status = defaults.PROCESSING
         self.run_log_store.add_step_log(step_log, self.run_id)
 
         super()._execute_node(node, map_variable=map_variable, **kwargs)
 
-        step_log = self.run_log_store.get_step_log(node._get_step_log_name(map_variable), self.run_id)
+        step_log = self.run_log_store.get_step_log(
+            node._get_step_log_name(map_variable), self.run_id
+        )
         if step_log.status == defaults.FAIL:
-            raise Exception(f'Step {node.name} failed')
+            raise Exception(f"Step {node.name} failed")
 
     def execute_graph(self, dag: Graph, map_variable: dict = None, **kwargs):
-        msg = (
-            "This executor is not supported to execute any graphs but only jobs (functions or notebooks)"
-        )
+        msg = "This executor is not supported to execute any graphs but only jobs (functions or notebooks)"
         raise NotImplementedError(msg)
 
-    def send_return_code(self, stage='traversal'):
+    def send_return_code(self, stage="traversal"):
         """
         Convenience function used by pipeline to send return code to the caller of the cli
 
         Raises:
             Exception: If the pipeline execution failed
         """
-        if stage != 'traversal':  # traversal does no actual execution, so return code is pointless
+        if (
+            stage != "traversal"
+        ):  # traversal does no actual execution, so return code is pointless
             run_id = self.run_id
 
             run_log = self.run_log_store.get_run_log_by_id(run_id=run_id, full=False)
             if run_log.status == defaults.FAIL:
-                raise Exception('Pipeline execution failed')
+                raise Exception("Pipeline execution failed")
```

### Comparing `magnus_extensions-0.2.7/magnus_extensions/executor/k8s_job/integration.py` & `magnus_extensions-0.2.8/magnus_extensions/executor/k8s_job/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/executor/kubeflow/implementation.py` & `magnus_extensions-0.2.8/magnus_extensions/executor/kubeflow/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/executor/kubeflow/integration.py` & `magnus_extensions-0.2.8/magnus_extensions/executor/kubeflow/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/experiment_tracker/mlflow/implementation.py` & `magnus_extensions-0.2.8/magnus_extensions/experiment_tracker/mlflow/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/secrets/aws/implementation.py` & `magnus_extensions-0.2.8/magnus_extensions/secrets/aws/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/magnus_extensions/secrets/aws/integration.py` & `magnus_extensions-0.2.8/magnus_extensions/secrets/aws/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.7/pyproject.toml` & `magnus_extensions-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnus_extensions"
-version = "0.2.7"
+version = "0.2.8"
 description = "Extensions to Magnus core"
 authors = ["Vijay Vammi <mesanthu@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "magnus_extensions"}]
 
 [tool.poetry.dependencies]
```

### Comparing `magnus_extensions-0.2.7/PKG-INFO` & `magnus_extensions-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnus-extensions
-Version: 0.2.7
+Version: 0.2.8
 Summary: Extensions to Magnus core
 License: Apache-2.0
 Author: Vijay Vammi
 Author-email: mesanthu@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

