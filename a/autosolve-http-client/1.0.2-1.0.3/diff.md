# Comparing `tmp/autosolve-http-client-1.0.2.tar.gz` & `tmp/autosolve-http-client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosolve-http-client-1.0.2.tar", last modified: Sat Apr  8 06:33:40 2023, max compression
+gzip compressed data, was "autosolve-http-client-1.0.3.tar", last modified: Wed Apr 19 23:57:33 2023, max compression
```

## Comparing `autosolve-http-client-1.0.2.tar` & `autosolve-http-client-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 fuzzy      (501) staff       (20)        0 2023-04-08 06:33:40.882551 autosolve-http-client-1.0.2/
--rw-r--r--   0 fuzzy      (501) staff       (20)     1065 2023-04-08 06:06:54.000000 autosolve-http-client-1.0.2/LICENSE
--rw-r--r--   0 fuzzy      (501) staff       (20)      365 2023-04-08 06:33:40.882182 autosolve-http-client-1.0.2/PKG-INFO
--rw-r--r--   0 fuzzy      (501) staff       (20)      139 2023-04-08 06:06:47.000000 autosolve-http-client-1.0.2/README.md
-drwxr-xr-x   0 fuzzy      (501) staff       (20)        0 2023-04-08 06:33:40.879640 autosolve-http-client-1.0.2/autosolve_http_client/
--rw-r--r--   0 fuzzy      (501) staff       (20)     5194 2023-04-02 19:53:04.000000 autosolve-http-client-1.0.2/autosolve_http_client/session.py
-drwxr-xr-x   0 fuzzy      (501) staff       (20)        0 2023-04-08 06:33:40.881821 autosolve-http-client-1.0.2/autosolve_http_client.egg-info/
--rw-r--r--   0 fuzzy      (501) staff       (20)      365 2023-04-08 06:33:40.000000 autosolve-http-client-1.0.2/autosolve_http_client.egg-info/PKG-INFO
--rw-r--r--   0 fuzzy      (501) staff       (20)      283 2023-04-08 06:33:40.000000 autosolve-http-client-1.0.2/autosolve_http_client.egg-info/SOURCES.txt
--rw-r--r--   0 fuzzy      (501) staff       (20)        1 2023-04-08 06:33:40.000000 autosolve-http-client-1.0.2/autosolve_http_client.egg-info/dependency_links.txt
--rw-r--r--   0 fuzzy      (501) staff       (20)        8 2023-04-08 06:33:40.000000 autosolve-http-client-1.0.2/autosolve_http_client.egg-info/requires.txt
--rw-r--r--   0 fuzzy      (501) staff       (20)       22 2023-04-08 06:33:40.000000 autosolve-http-client-1.0.2/autosolve_http_client.egg-info/top_level.txt
--rw-r--r--   0 fuzzy      (501) staff       (20)       38 2023-04-08 06:33:40.882617 autosolve-http-client-1.0.2/setup.cfg
--rw-r--r--   0 fuzzy      (501) staff       (20)      510 2023-04-08 06:33:07.000000 autosolve-http-client-1.0.2/setup.py
+drwxr-xr-x   0 fuzzy      (501) staff       (20)        0 2023-04-19 23:57:33.974494 autosolve-http-client-1.0.3/
+-rw-r--r--   0 fuzzy      (501) staff       (20)     1065 2023-04-08 06:06:54.000000 autosolve-http-client-1.0.3/LICENSE
+-rw-r--r--   0 fuzzy      (501) staff       (20)      365 2023-04-19 23:57:33.974075 autosolve-http-client-1.0.3/PKG-INFO
+-rw-r--r--   0 fuzzy      (501) staff       (20)      139 2023-04-08 06:06:47.000000 autosolve-http-client-1.0.3/README.md
+drwxr-xr-x   0 fuzzy      (501) staff       (20)        0 2023-04-19 23:57:33.958694 autosolve-http-client-1.0.3/autosolve_http_client/
+-rw-r--r--   0 fuzzy      (501) staff       (20)     5610 2023-04-19 23:49:09.000000 autosolve-http-client-1.0.3/autosolve_http_client/session.py
+drwxr-xr-x   0 fuzzy      (501) staff       (20)        0 2023-04-19 23:57:33.972999 autosolve-http-client-1.0.3/autosolve_http_client.egg-info/
+-rw-r--r--   0 fuzzy      (501) staff       (20)      365 2023-04-19 23:57:33.000000 autosolve-http-client-1.0.3/autosolve_http_client.egg-info/PKG-INFO
+-rw-r--r--   0 fuzzy      (501) staff       (20)      283 2023-04-19 23:57:33.000000 autosolve-http-client-1.0.3/autosolve_http_client.egg-info/SOURCES.txt
+-rw-r--r--   0 fuzzy      (501) staff       (20)        1 2023-04-19 23:57:33.000000 autosolve-http-client-1.0.3/autosolve_http_client.egg-info/dependency_links.txt
+-rw-r--r--   0 fuzzy      (501) staff       (20)        8 2023-04-19 23:57:33.000000 autosolve-http-client-1.0.3/autosolve_http_client.egg-info/requires.txt
+-rw-r--r--   0 fuzzy      (501) staff       (20)       22 2023-04-19 23:57:33.000000 autosolve-http-client-1.0.3/autosolve_http_client.egg-info/top_level.txt
+-rw-r--r--   0 fuzzy      (501) staff       (20)       38 2023-04-19 23:57:33.974552 autosolve-http-client-1.0.3/setup.cfg
+-rw-r--r--   0 fuzzy      (501) staff       (20)      510 2023-04-19 23:56:08.000000 autosolve-http-client-1.0.3/setup.py
```

### Comparing `autosolve-http-client-1.0.2/LICENSE` & `autosolve-http-client-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autosolve-http-client-1.0.2/autosolve_http_client/session.py` & `autosolve-http-client-1.0.3/autosolve_http_client/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,36 +33,43 @@
 class Session:
     def __init__(self, api_key):
         self.api_key = api_key
         self.debug = False
         self.auth_lock = Lock()
         self.token_expires_at = 0
         self.token = None
+        self.pending_tasks = set({})
         self.tasks = {}
         self.tasks_lock = Lock()
         self.tasks_fetch_at = 0
 
     def enable_debug(self):
         self.debug = True
 
     def disable_debug(self):
         self.debug = False
 
     def solve(self, task_req, timeout):
         if self.__send(task_req, tasksCreateUrl):
-            return self.__wait_for_task(task_req["taskId"], timeout)
+            task_id = task_req["taskId"]
+            self.pending_tasks.add(task_id)
+            return self.__wait_for_task(task_id, timeout)
         else:
             return None
 
     def cancel_many_tasks(self, task_ids):
         cancel_req = {"taskIds": task_ids}
+        for task_id in task_ids:
+            if task_id in self.pending_tasks:
+                self.pending_tasks.remove(task_id)
         return self.__send(cancel_req, tasksCancelUrl)
 
     def cancel_all_tasks(self):
         cancel_req = {}
+        self.pending_tasks.clear()
         return self.__send(cancel_req, tasksCancelUrl)
 
     def __send(self, obj, url):
         body = json.dumps(obj)
         resp = self.__do('POST', url, body)
         if resp is None or not is_status_2xx(resp.status):
             return False
@@ -99,31 +106,33 @@
             raise Exception("failed to get auth token")
         data = json.loads(resp.data.decode('utf-8'))
         self.token = data["token"]
         self.token_expires_at = data['expiresAt']
         self.__log("new auth token is generated with expires_at: " + str(self.token_expires_at))
 
     def __wait_for_task(self, task_id, timeout):
-        start_time = time.time()
+        created_at = round(time.time())
         time.sleep(5)
+        start_time = time.time()
         delay = 5
-        while True:
+        while task_id in self.pending_tasks:
             try:
                 delay = self.__fetch_tasks()
                 if task_id in self.tasks:
                     task_resp = self.tasks[task_id]
                     self.tasks[task_id] = None
                     return task_resp
             except Exception as e:
                 self.__log("failed to fetch tasks: " + str(e))
             if time.time() - start_time > timeout:
                 if not self.cancel_many_tasks([task_id]):
                     self.__log("failed to cancel task: " + task_id)
-                return None
+                break
             time.sleep(delay)
+        return {"taskId": task_id, "createdAt": created_at, "status": Cancelled}
 
     def __fetch_tasks(self):
         self.tasks_lock.acquire()
         next_fetch_delay = 5
         try:
             if self.tasks_fetch_at <= time.time():
                 resp = self.__do('GET', tasksUrl, None)
```

