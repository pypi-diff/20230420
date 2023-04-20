# Comparing `tmp/chatgpt-proxy-0.2.3.tar.gz` & `tmp/chatgpt-proxy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-proxy-0.2.3.tar", last modified: Wed Apr 19 16:33:13 2023, max compression
+gzip compressed data, was "chatgpt-proxy-0.2.4.tar", last modified: Wed Apr 19 17:37:39 2023, max compression
```

## Comparing `chatgpt-proxy-0.2.3.tar` & `chatgpt-proxy-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:33:13.687107 chatgpt-proxy-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-19 16:33:02.000000 chatgpt-proxy-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-19 16:33:13.687107 chatgpt-proxy-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-19 16:33:02.000000 chatgpt-proxy-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:33:13.683107 chatgpt-proxy-0.2.3/chatgpt_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 16:33:02.000000 chatgpt-proxy-0.2.3/chatgpt_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-19 16:33:02.000000 chatgpt-proxy-0.2.3/chatgpt_proxy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-04-19 16:33:02.000000 chatgpt-proxy-0.2.3/chatgpt_proxy/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:33:13.687107 chatgpt-proxy-0.2.3/chatgpt_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-19 16:33:13.000000 chatgpt-proxy-0.2.3/chatgpt_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-19 16:33:13.000000 chatgpt-proxy-0.2.3/chatgpt_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:33:13.000000 chatgpt-proxy-0.2.3/chatgpt_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 16:33:13.000000 chatgpt-proxy-0.2.3/chatgpt_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 16:33:13.000000 chatgpt-proxy-0.2.3/chatgpt_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-19 16:33:02.000000 chatgpt-proxy-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:33:13.687107 chatgpt-proxy-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:37:39.691112 chatgpt-proxy-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-19 17:37:28.000000 chatgpt-proxy-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-19 17:37:39.691112 chatgpt-proxy-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-19 17:37:28.000000 chatgpt-proxy-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:37:39.691112 chatgpt-proxy-0.2.4/chatgpt_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 17:37:28.000000 chatgpt-proxy-0.2.4/chatgpt_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-19 17:37:28.000000 chatgpt-proxy-0.2.4/chatgpt_proxy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-04-19 17:37:28.000000 chatgpt-proxy-0.2.4/chatgpt_proxy/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:37:39.691112 chatgpt-proxy-0.2.4/chatgpt_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-19 17:37:39.000000 chatgpt-proxy-0.2.4/chatgpt_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-19 17:37:39.000000 chatgpt-proxy-0.2.4/chatgpt_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:37:39.000000 chatgpt-proxy-0.2.4/chatgpt_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 17:37:39.000000 chatgpt-proxy-0.2.4/chatgpt_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 17:37:39.000000 chatgpt-proxy-0.2.4/chatgpt_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-19 17:37:28.000000 chatgpt-proxy-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 17:37:39.691112 chatgpt-proxy-0.2.4/setup.cfg
```

### Comparing `chatgpt-proxy-0.2.3/LICENSE` & `chatgpt-proxy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-proxy-0.2.3/PKG-INFO` & `chatgpt-proxy-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-proxy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Reverse proxy for OpenAI chatgpt website API
 Author: 18870
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chatgpt-proxy-0.2.3/README.md` & `chatgpt-proxy-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt-proxy-0.2.3/chatgpt_proxy/__main__.py` & `chatgpt-proxy-0.2.4/chatgpt_proxy/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,17 @@
     handlers=[logging.StreamHandler()],
 )
 
 logger = logging.getLogger(__name__)
 
 
 class Settings(BaseSettings):
-    cf_clearance: str = None
-    user_agent: str = None
+    cf_clearance: str = ""
+    user_agent: str = ""
+    puid: str = ""
 
     access_token: str = None
     host: str = "127.0.0.1"
     port: int = 7800
     trust: bool = Field(default=False, env="proxy_trust_client")
     mod_access_token: str = None
 
@@ -32,14 +33,15 @@
 
 
 if __name__ == "__main__":
     env = Settings()
     proxy = WebChatGPTProxy(
         cf_clearance=env.cf_clearance,
         user_agent=env.user_agent,
+        puid=env.puid,
         access_token=env.access_token,
         trust=env.trust,
     )
 
     @asynccontextmanager
     async def lifespan(app: FastAPI):
         asyncio.create_task(proxy._refresh_task())
```

### Comparing `chatgpt-proxy-0.2.3/chatgpt_proxy/proxy.py` & `chatgpt-proxy-0.2.4/chatgpt_proxy/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,16 +110,16 @@
 
 
 class WebChatGPTProxy(ReverseProxy):
     def __init__(
         self,
         cf_clearance: str,
         user_agent: str,
+        puid: str,
         access_token: Optional[str] = None,
-        puid: Optional[str] = None,
         trust: bool = False,
     ) -> None:
         """
         :param cf_clearance: from `cf_clearance` cookie
         :param user_agent: from `user-agent` header
         :param access_token: from openai `access_token`
                              obtained from here https://chat.openai.com/api/auth/session
```

### Comparing `chatgpt-proxy-0.2.3/chatgpt_proxy.egg-info/PKG-INFO` & `chatgpt-proxy-0.2.4/chatgpt_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-proxy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Reverse proxy for OpenAI chatgpt website API
 Author: 18870
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

