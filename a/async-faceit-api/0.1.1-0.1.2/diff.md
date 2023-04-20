# Comparing `tmp/async_faceit_api-0.1.1.tar.gz` & `tmp/async_faceit_api-0.1.2.tar.gz`

## Comparing `async_faceit_api-0.1.1.tar` & `async_faceit_api-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.gitattributes
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.readthedocs.yaml
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.idea/.gitignore
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.idea/AsyncFaceitApi.iml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0     9338 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.idea/workspace.xml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/docs/Makefile
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/docs/async_faceit_api.rst
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/docs/conf.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/docs/index.rst
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/docs/make.bat
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/docs/modules.rst
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/docs/requirements.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/src/async_faceit_api/__init__.py
--rw-r--r--   0        0        0    42627 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/src/async_faceit_api/api.py
--rw-r--r--   0        0        0    45723 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/src/async_faceit_api/dataclasses.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/src/async_faceit_api/enums.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/tests/example.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/tests/subclassing.py
--rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/tests/test.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/LICENSE
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/README.md
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/.gitattributes
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/.idea/.gitignore
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/.idea/AsyncFaceitApi.iml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/.idea/misc.xml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/docs/Makefile
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/docs/async_faceit_api.rst
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/docs/conf.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/docs/make.bat
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/docs/modules.rst
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/docs/requirements.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/src/async_faceit_api/__init__.py
+-rw-r--r--   0        0        0    43659 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/src/async_faceit_api/api.py
+-rw-r--r--   0        0        0    45988 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/src/async_faceit_api/dataclasses.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/src/async_faceit_api/enums.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/tests/example.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/tests/subclassing.py
+-rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/tests/test.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/README.md
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 async_faceit_api-0.1.2/PKG-INFO
```

### Comparing `async_faceit_api-0.1.1/.idea/AsyncFaceitApi.iml` & `async_faceit_api-0.1.2/.idea/AsyncFaceitApi.iml`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.1/.idea/workspace.xml` & `async_faceit_api-0.1.2/.idea/workspace.xml`

 * *Files 22% similar despite different names*

#### Comparing `async_faceit_api-0.1.1/.idea/workspace.xml` & `async_faceit_api-0.1.2/.idea/workspace.xml`

```diff
@@ -1,11 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
-    <list default="true" id="7a343e8b-7b6d-4f78-a923-893771613ad2" name="Changes" comment=""/>
+    <list default="true" id="7a343e8b-7b6d-4f78-a923-893771613ad2" name="Changes" comment="">
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/async_faceit_api/api.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/async_faceit_api/api.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/async_faceit_api/dataclasses.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/async_faceit_api/dataclasses.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/async_faceit_api/enums.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/async_faceit_api/enums.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/test.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test.py" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -32,15 +38,15 @@
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent">
     <property name="RunOnceActivity.OpenProjectViewOnStart" value="true"/>
     <property name="RunOnceActivity.ShowReadmeOnStart" value="true"/>
-    <property name="last_opened_file_path" value="$PROJECT_DIR$/../PythonApp"/>
+    <property name="last_opened_file_path" value="$PROJECT_DIR$"/>
     <property name="settings.editor.selected.configurable" value="com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable"/>
   </component>
   <component name="PyDebuggerOptionsProvider">
     <option name="mySaveCallSignatures" value="true"/>
   </component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
```

### Comparing `async_faceit_api-0.1.1/docs/Makefile` & `async_faceit_api-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.1/docs/async_faceit_api.rst` & `async_faceit_api-0.1.2/docs/async_faceit_api.rst`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.1/docs/conf.py` & `async_faceit_api-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.1/docs/make.bat` & `async_faceit_api-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.1/src/async_faceit_api/api.py` & `async_faceit_api-0.1.2/src/async_faceit_api/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,57 @@
+import asyncio
 import datetime
 from typing import Tuple, Any
 from aiohttp import request
+from asyncio import Semaphore
 from .enums import *
 from .dataclasses import *
 
 
 class FaceitAPI:
     """
     See the faceit data-api docs for more information:
     https://developers.faceit.com/docs/tools/data-api
     """
 
-    __BASE_URL: str = 'https://open.faceit.com/data/v4/{}'
+    __BASE_URL = 'https://open.faceit.com/data/v4/{}'
+    __LIMIT_PER_SEC = 100
+    __LIMIT_PER_H = 10_000
 
-    def __init__(self, api_token: str):
+    __sec_semaphore = Semaphore(__LIMIT_PER_SEC)
+    __h_semaphore = Semaphore(__LIMIT_PER_H)
+
+    def __init__(self, api_token: str, rate_limit_behaviour: RateLimitBehaviour = RateLimitBehaviour.WAIT_SOME_SEC):
         self.__header = {
             'accept': 'application/json',
             'Authorization': f'Bearer {api_token}'
         }
+        self.__rate_limit_behaviour = rate_limit_behaviour
 
     async def __make_request(self, method: str, url: str) -> Tuple[int, Any]:
-        async with request(method, url, headers=self.__header) as response:
-            return response.status, await response.json()
-
+        if self.__rate_limit_behaviour == RateLimitBehaviour.NEVER_WAIT and (self.__sec_semaphore.locked() or self.__h_semaphore.locked()):
+            return 429, {}
+        if self.__rate_limit_behaviour == RateLimitBehaviour.WAIT_SOME_SEC and self.__h_semaphore.locked():
+            return 429, {}
+        await self.__sec_semaphore.acquire()
+        await self.__h_semaphore.acquire()
+        try:
+            async with request(method, url, headers=self.__header) as response:
+                return response.status, await response.json()
+        finally:
+            loop = asyncio.get_event_loop()
+            loop.call_later(1, self.__sec_semaphore.release)
+            loop.call_later(3600, self.__h_semaphore.release)
 
     @staticmethod
     async def __create_object(response: Tuple[int, Any], object_class=None) -> Any:
         status, json_response = response
         if not 200 <= status < 300:
+            if status == 429:
+                return FaceitApiRateLimitError(**json_response)
             return FaceitApiError(**json_response, status_code=status)
         if object_class is not None:
             return object_class(**json_response)
         return json_response
 
     @staticmethod
     async def __create_collection(response: Tuple[int, Any], object_class, collection_class=Collection) -> Any:
```

### Comparing `async_faceit_api-0.1.1/src/async_faceit_api/dataclasses.py` & `async_faceit_api-0.1.2/src/async_faceit_api/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 class FaceitApiError(FaceitApiResponse):
     def __init__(self, message: str = 'Bad Request', status_code: int = 400, **kwargs):
         super().__init__(False, **kwargs)
         self.message = message
         self.status_code = status_code
 
 
+class FaceitApiRateLimitError(FaceitApiResponse):
+    def __init__(self, message: str = 'Too many requests', status_code: int = 429, **kwargs):
+        super().__init__(False, **kwargs)
+        self.message = message
+        self.status_code = status_code
+
+
 class Assets(FaceitApiResponse):
     def __init__(self,
                  cover: str = None,
                  featured_img_l: str = None,
                  featured_img_m: str = None,
                  featured_img_s: str = None,
                  flag_img_icon: str = None,
```

### Comparing `async_faceit_api-0.1.1/src/async_faceit_api/enums.py` & `async_faceit_api-0.1.2/src/async_faceit_api/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from enum import Enum
 
 
+class RateLimitBehaviour(Enum):
+    NEVER_WAIT = 0
+    ALWAYS_WAIT = 1
+    WAIT_SOME_SEC = 2
+
+
 class Expansion(Enum):
     NONE = ''
     ORGANIZER = 'organizer'
     GAME = 'game'
 
 
 class MatchType(Enum):
```

### Comparing `async_faceit_api-0.1.1/tests/subclassing.py` & `async_faceit_api-0.1.2/tests/subclassing.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.1/tests/test.py` & `async_faceit_api-0.1.2/tests/test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import asyncio
 
 from src.async_faceit_api import FaceitAPI
 from dotenv import load_dotenv
-from src.async_faceit_api.enums import Game, Region
+from src.async_faceit_api.enums import Game, Region, RateLimitBehaviour
 
 load_dotenv()
 
 
 async def test_championship(api: FaceitAPI):
     game_id = Game.CS_GO
     championship_id = "3c5121c0-ac3a-4a99-9788-20ee262fca7f"
@@ -161,29 +161,43 @@
         print("error tournament_brackets(tournament_id)")
     if not await api.tournament_matches(tournament_id):
         print("error tournament_matches(tournament_id)")
     if not await api.tournament_teams(tournament_id):
         print("error tournament_teams(tournament_id)")
 
 
+async def test_rate_limit(api: FaceitAPI):
+    match_id = "1-506ad3d0-7266-4d43-8cfc-fdbbac077027"
+    requests = [api.match_stats(match_id) for i in [0]*101]
+    results = await asyncio.gather(*requests)
+    result = [bool(r) for r in results]
+    print(result)
+    print(len(result))
+    if all(result):
+        print("error test_rate_limit")
+
+
+
+
 async def test_task():
-    api = FaceitAPI(os.getenv('faceit_api_key'))
+    api = FaceitAPI(os.getenv('faceit_api_key'), RateLimitBehaviour.WAIT_SOME_SEC)
 
     await asyncio.gather(
-        test_championship(api),
-        test_games(api),
-        test_hub(api),
-        test_leaderboards(api),
-        test_match(api),
-        test_organizer(api),
-        test_player(api),
-        test_ranking(api),
-        test_search(api),
-        test_teams(api),
-        test_tournament(api)
+        # test_championship(api),
+        # test_games(api),
+        # test_hub(api),
+        # test_leaderboards(api),
+        # test_match(api),
+        # test_organizer(api),
+        # test_player(api),
+        # test_ranking(api),
+        # test_search(api),
+        # test_teams(api),
+        # test_tournament(api),
+        test_rate_limit(api),
     )
 
 
 if __name__ == "__main__":
     loop = asyncio.new_event_loop()
     loop.run_until_complete(test_task())
     loop.close()
```

### Comparing `async_faceit_api-0.1.1/.gitignore` & `async_faceit_api-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.1/LICENSE` & `async_faceit_api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.1/README.md` & `async_faceit_api-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.1/pyproject.toml` & `async_faceit_api-0.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "async_faceit_api"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Stuart", email="stuart.the.yellow.one@gmail.com" },
 ]
 description = "Async wrapper for the faceit API for csgo"
 documentation = "https://async-faceit-api.readthedocs.io/en/latest/index.html"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 dependencies = [
   'aiohttp < 3.8.3',
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `async_faceit_api-0.1.1/PKG-INFO` & `async_faceit_api-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: async_faceit_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: Async wrapper for the faceit API for csgo
 Project-URL: Homepage, https://github.com/StuartTheYellowOne/async_faceit_api
 Project-URL: Bug Tracker, https://github.com/StuartTheYellowOne/async_faceit_api/issues
 Author-email: Stuart <stuart.the.yellow.one@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Requires-Dist: aiohttp<3.8.3
 Description-Content-Type: text/markdown
 
 # Async faceit API
 
 Async wrapper for the faceit API for csgo.
```

