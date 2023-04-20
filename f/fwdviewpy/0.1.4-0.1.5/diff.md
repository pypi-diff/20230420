# Comparing `tmp/fwdviewpy-0.1.4.tar.gz` & `tmp/fwdviewpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fwdviewpy-0.1.4.tar", last modified: Tue Apr 18 10:11:18 2023, max compression
+gzip compressed data, was "fwdviewpy-0.1.5.tar", last modified: Thu Apr 20 14:58:21 2023, max compression
```

## Comparing `fwdviewpy-0.1.4.tar` & `fwdviewpy-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 10:11:18.985511 fwdviewpy-0.1.4/
--rw-rw-rw-   0        0        0      623 2023-04-18 10:11:18.978389 fwdviewpy-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 10:11:18.942817 fwdviewpy-0.1.4/fwdviewpy/
--rw-rw-rw-   0        0        0      101 2023-04-18 10:09:30.000000 fwdviewpy-0.1.4/fwdviewpy/__init__.py
--rw-rw-rw-   0        0        0    10482 2023-04-17 15:48:31.000000 fwdviewpy-0.1.4/fwdviewpy/main.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:11:18.975388 fwdviewpy-0.1.4/fwdviewpy.egg-info/
--rw-rw-rw-   0        0        0      623 2023-04-18 10:11:18.000000 fwdviewpy-0.1.4/fwdviewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-04-18 10:11:18.000000 fwdviewpy-0.1.4/fwdviewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 10:11:18.000000 fwdviewpy-0.1.4/fwdviewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 10:11:18.000000 fwdviewpy-0.1.4/fwdviewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-18 10:11:18.000000 fwdviewpy-0.1.4/fwdviewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 10:11:18.985511 fwdviewpy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      830 2023-04-18 10:10:54.000000 fwdviewpy-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:58:21.351387 fwdviewpy-0.1.5/
+-rw-rw-rw-   0        0        0      623 2023-04-20 14:58:21.351387 fwdviewpy-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-20 14:58:21.286531 fwdviewpy-0.1.5/fwdviewpy/
+-rw-rw-rw-   0        0        0      101 2023-04-18 10:09:30.000000 fwdviewpy-0.1.5/fwdviewpy/__init__.py
+-rw-rw-rw-   0        0        0    10707 2023-04-20 14:54:14.000000 fwdviewpy-0.1.5/fwdviewpy/main.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:58:21.344372 fwdviewpy-0.1.5/fwdviewpy.egg-info/
+-rw-rw-rw-   0        0        0      623 2023-04-20 14:58:21.000000 fwdviewpy-0.1.5/fwdviewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-04-20 14:58:21.000000 fwdviewpy-0.1.5/fwdviewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 14:58:21.000000 fwdviewpy-0.1.5/fwdviewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 14:58:21.000000 fwdviewpy-0.1.5/fwdviewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-20 14:58:21.000000 fwdviewpy-0.1.5/fwdviewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 14:58:21.359398 fwdviewpy-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      830 2023-04-18 14:43:43.000000 fwdviewpy-0.1.5/setup.py
```

### Comparing `fwdviewpy-0.1.4/PKG-INFO` & `fwdviewpy-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwdviewpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package developed by FWD View - The Data Transformation Specialists.
 Author: Cameron Bose & Ryan Springett
 Author-email: cameron.bose@fwdview.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `fwdviewpy-0.1.4/fwdviewpy/main.py` & `fwdviewpy-0.1.5/fwdviewpy/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,264 +1,253 @@
 import logging
 import sys
 import requests
-import time
-from datetime import datetime 
+import time 
 import json
 
 class VirtualisationEngineSessionManager:
-
     def __init__(self, address, username, password, major, minor, micro):
-        # SETTING UP LOG FILE
-        logging.basicConfig(filename='VirtualisationEngineSessionManager.log',
-                            level=logging.DEBUG, format='%(asctime)s %(levelname)s:%(message)s', filemode='w')
+        logging.basicConfig(filename='DelphixEngineSessionManager.log',
+                            level=logging.INFO, format='%(asctime)s %(levelname)s:%(message)s', filemode='w')
         logging.info(30 * '=' + '| RUN BEGINS |' + 30 * '=')
-
         self.address = address
         self.username = username
         self.password = password
         self.major = major
         self.minor = minor
         self.micro = micro
 
     def __str__(self):
         return f'Virtualisation Engine Session Manager: {self.address}'
 
-    # POTENTIALLY ADD A REFRESH FUNCTION RATHER THAN USING THE LOGIN TO REFRESH DATA
-
-    def login(self):
+    def _login(self):
         """This function logs into the Virtualisation Engine
         """
-        # establishing session
         session = requests.session()
         session_url = f"http://{self.address}/resources/json/delphix/session"
         data = {
             "type": "APISession",
             "version": {
                 "type": "APIVersion",
                 "major": self.major,
                 "minor": self.minor,
                 "micro": self.micro
             }
         }
         response = session.post(session_url, json=data)
-        print(response.text)
         if response.ok:
-            logging.debug(f"Session established on {self.address}")
+            logging.info(f"Session established on {self.address}")
         else:
             logging.error(f"Session NOT established on {self.address}")
             sys.exit()
-        # this logs in and grabs all information from engine - works as a refresh
         url = f"http://{self.address}/resources/json/delphix/login"
         data = {
             "type": "LoginRequest",
             "username": self.username,
             "password": self.password
         }
-
         response = session.post(url, json=data)
-        print(response.text)
         if response.ok:
-            logging.debug(
+            logging.info(
                 f"login SUCCEEDED - Response: {response.status_code}")
-            # self.datasets = self.get_datasets_info()
-            # self.bookmarks = self.get_bookmarks_info()
-            # self.snapshots = self.get_snapshots_info()
-            # self.sources = self.get_sources_info()
-            # self.replications = self.get_replications_info()
-            # self.environments = self.get_environments_info()
         else:
             logging.error(f"login FAILED - Response: {response.status_code}")
             sys.exit()
         return session
 
     def createBookmark(self, containerName, bookmarkName):
         # Set up the session object
-        containerReference, containerBranch = self.getTemplateBranch(containerName)
+        """ 
+        This method creates a bookmark on the container of the Delphix Engine. 
+
+        Args: 
+            containerName: This is the name of the container to be bookmarked on the Delphix Engine. 
+            bookmarkName: This argument is the name of the bookmark to be made on the containerName.
+        
+        Returns: 
+            This method does not return any value. 
+        """
+        containerReference, containerBranch = self._getTemplateBranch(containerName)
         # Send a POST request to the bookmark endpoint with cookies set from the session
         bookmark_url = f"http://{self.address}/resources/json/delphix/selfservice/bookmark"
         data = {
             "type": "JSBookmarkCreateParameters",
             "bookmark": {
                 "type": "JSBookmark",
                 "name": bookmarkName,
                 "branch": containerBranch
             },
             "timelinePointParameters": {
                 "type": "JSTimelinePointLatestTimeInput",
                 "sourceDataLayout": containerReference
             }
         }
-        session = self.login()
+        session = self._login()
         response = session.post(bookmark_url, json=data)
         action = response.json()['action']
-        self.checkActionLoop(action)
-        # print(response.json())
+        self._checkActionLoop(action)
         session.close()
-        return str(f"Bookmark: {bookmarkName}\nDate and Time: {datetime.now()}\nOutput: {response.json()}\n{'=' * 30}\n")
+        logging.debug(f"Bookmark has been created. \n Bookmark: {bookmarkName} \n Container: {containerName} \n Engine: {self.address}")
 
-    def checkActionLoop(self, action): 
+    def _checkActionLoop(self, action): 
         while True:
-            if self.checkAction(action):
-                print("It has Completed!")
+            if self._checkAction(action):
                 break
-            elif self.checkAction(action) == "FAILED":
-                current_time = datetime.datetime.now()
-                current_time_formatted = current_time.strftime("%Y-%m-%d %H:%M:%S")
-                print("Action has failed, check engine logs.")
-                """ sendEmailAlert(bookmarkName, current_time_formatted, "Virtualisation Engine") """
+            elif self._checkAction(action) == "FAILED":
+                logging.error("Failed to create Bookmark. Please see Engine logs.")
                 sys.exit()
             else:
-                print("Not yet Completed, check again in 30 seconds")
-                time.sleep(30)
+                print("Not yet Completed, check again in 10 seconds")
+                time.sleep(10)
 
-    def checkAction(self, action):
+    def _checkAction(self, action):
         session = self.login()
         action_url = f"http://{self.address}/resources/json/delphix/action"
         APIQuery = session.get(action_url)
         for actions in APIQuery.json()["result"]:
             if actions['reference'] == action:
                 state = actions['state']
-                print(state)
                 if state == "COMPLETED":
                     session.close()
                     return True
                 elif state == "FAILED":
                     state = "FAILED"
                     session.close()
                     return state
                 else:
                     return False
     
-    def getTemplateBranch(self, containerName):
+    def _getTemplateBranch(self, containerName):
         # Log in and obtain the session object
         session = self.login() 
-
-
         # Send a GET request to the selfservice/template endpoint with cookies set from the session
         template_url = f"http://{self.address}/resources/json/delphix/selfservice/container"
         response = session.get(template_url)
-
         # Extract the template reference and active branch from the API response
         container_reference = None
         container_branch = None
         for container in response.json()["result"]:
             if container['name'] == containerName:
                 container_reference = container["reference"]
                 container_branch = container["activeBranch"]
                 break
-
-        print(
-            f"container reference: {container_reference} & Template branch: {container_branch}")
-
-        # Close the session
+        logging.debug(f"container reference: {container_reference} & Template branch: {container_branch}")
         session.close()
-
         return container_reference, container_branch 
     
-class MaskingEngineSessionManager: 
+class MaskingEngineSessionManager(VirtualisationEngineSessionManager): 
     def __init__(self, address, username, password, major, minor, micro): 
-        self.address = address 
-        self.username = username 
-        self.password = password
-        self.major = major 
-        self.minor = minor
-        self.micro = micro 
+        super().__init__(self, address, username, password, major, minor, micro)
 
+    def __str__(self):
+        return f'Masking Engine Session Manager: {self.address}'
     
-    def login(self): 
+    def login(self):
+        """
+        This method logs in to the Delphix Masking Engine. 
+
+        Returns: 
+            This method returns an authentication key used to send API's to the engine. 
+        """ 
         url = f"http://{self.address}/masking/api/v5.1.14/login"
 
         payload = json.dumps({"username": self.username, "password": self.password})
         headers = {'Content-Type': 'application/json'}
         response = requests.request("POST", url, headers=headers, data=payload)
         responseDict = response.json()
         authKey = responseDict['Authorization']
-        print(authKey)
+        logging.info(f"Authentication key established for Masking Engine {self.address}. Key: {authKey}")
         return authKey
     
     def runMaskingJob(self, environment, maskingRule, connectorName):
-        authKey = self.login()
-        envID = self.getEnvironment(authKey, environment)
-        ruleID = self.getJobId(authKey, maskingRule, envID)
-        targetConnectorID = self.getTargetConnectorID(authKey, connectorName, envID)
-        executejob = self.execute_job(authKey, ruleID, targetConnectorID)
-        print(executejob)
-        executionID = self.getExecutionID(authKey, ruleID)
-        jobStatus = self.checkStatus(executionID) 
+        """
+        This method executes pre-configured masking jobs on the masking engine.
+
+        Args: 
+            environment: This is the environent on the Delphix masking engine on which to run the masking job. 
+            maskingRule: This is the ruleset that we want to run on the delphix engine. 
+            connectorName: This is the name of the connector for which connects the masking job to the data. 
         
-        if jobStatus == "SUCCEEDED":
-            print("Moving on to the next step.")
-            return str(f"Masking Job: \nDate and Time: {datetime.now()}\nOutput: {jobStatus}\n{'=' * 30}\n")
+        Returns: 
+            This method does not return any value. 
+        """
+        authKey = self.login()
+        envID = self._getEnvironment(authKey, environment)
+        ruleID = self._getJobId(authKey, maskingRule, envID)
+        targetConnectorID = self._getTargetConnectorID(authKey, connectorName, envID)
+        self._execute_job(authKey, ruleID, targetConnectorID)
+        logging.info(f"Masking job triggered. Job: {maskingRule}")
+        executionID = self._getExecutionID(authKey, ruleID)
+        jobStatus = self._checkStatus(executionID) 
 
+        if jobStatus == "SUCCEEDED":
+            logging.info(f"Masking Successful. Job: {maskingRule}")
         else:
-            current_time = datetime.datetime.now()
-            current_time_formatted = current_time.strftime("%Y-%m-%d %H:%M:%S")
-            print(
-                f"Please check error logs for masking job: {maskingRule} @ {current_time_formatted}")
-
+            logging.error(f"Please check error logs for masking job: {maskingRule}")
             sys.exit()
     
-    def getEnvironment(self, authKey, envName):
-        response = self.getRequest(authKey, "environments")
+    def _getEnvironment(self, authKey, envName):
+        response = self._getRequest(authKey, "environments")
         response = json.loads(response)
         for env in response["responseList"]:
             if env["environmentName"] == envName:
                 envID = env["environmentId"]
         return envID
     
 
-    def getRequest(self, authKey, endPoint):
+    def _getRequest(self, authKey, endPoint):
         url = f"http://{self.address}/masking/api/v5.1.14/{endPoint}"
         payload = {}
         headers = {
             'Authorization': authKey
         }
         response = requests.request("GET", url, headers=headers, data=payload)
-        response = response.text
-        return response
+        return response.text
+
+    def _getExecutionID(self, authKey, jobID):
+        endPoint = f"executions?job_id={jobID}&page_number=1&execution_status=RUNNING"
+        response = self._getRequest(authKey, endPoint)
+        response = json.loads(response)
+        executionID = response['responseList'][0]['executionId']
+        return executionID
 
-    def getJobId(self, authKey, jobName, envID):
+    def _getJobId(self, authKey, jobName, envID):
         endPoint = f"masking-jobs?environment_id={envID}"
-        response = self.getRequest(authKey, endPoint)
+        response = self._getRequest(authKey, endPoint)
         response = json.loads(response)
         for job in response["responseList"]:
             if job["jobName"] == jobName:
                 jobID = job['maskingJobId']
         return jobID
 
-    def getTargetConnectorID(self, authKey, connectorName, environmentId):
-        response = self.getRequest(authKey, "database-connectors")
+    def _getTargetConnectorID(self, authKey, connectorName, environmentId):
+        response = self._getRequest(authKey, "database-connectors")
         response = json.loads(response)
         for connectors in response["responseList"]:
             if connectors["connectorName"] == connectorName and connectors["environmentId"] == environmentId:
                 targetConnectorID = connectors["databaseConnectorId"]
         return targetConnectorID
      
-    def execute_job(self, auth_key, job_id, targetConnectorID):
+    def _execute_job(self, auth_key, job_id, targetConnectorID):
         url = f"http://{self.address}/masking/api/v5.1.14/executions"
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json',
             'Authorization': auth_key
         }
         data = {
             'jobId': job_id, 
             'targetConnectorId': targetConnectorID
         }
         response = requests.post(url, headers=headers, data=json.dumps(data))
-
         return response.text
 
-    def checkStatus(self, executionID):
+    def _checkStatus(self, executionID):
         authKey = self.login()
         while True:
-            status = self.getStatus(authKey, executionID)
+            status = self._getStatus(authKey, executionID)
             if status == "RUNNING":
                 time.sleep(300)
                 print("Job is still running, check again in 5 minutes.")
             else:
                 print(f"Job has finished running. Job Status is: {status}")
-                return status
-                break
-
- 
+                return status
```

### Comparing `fwdviewpy-0.1.4/fwdviewpy.egg-info/PKG-INFO` & `fwdviewpy-0.1.5/fwdviewpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwdviewpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package developed by FWD View - The Data Transformation Specialists.
 Author: Cameron Bose & Ryan Springett
 Author-email: cameron.bose@fwdview.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `fwdviewpy-0.1.4/setup.py` & `fwdviewpy-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fwdviewpy',
-    version='0.1.4',
+    version='0.1.5',
     description='Python package developed by FWD View - The Data Transformation Specialists.',
     long_description='Python package developed by FWD View to aid automation of Delphix actions on both the Virtulaization and Continuous Compliance Delphix engines.',
     packages=find_packages(),
     author='Cameron Bose & Ryan Springett',
     author_email="cameron.bose@fwdview.com",
 
     install_requires=[
```

