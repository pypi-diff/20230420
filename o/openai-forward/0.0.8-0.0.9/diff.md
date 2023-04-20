# Comparing `tmp/openai_forward-0.0.8.tar.gz` & `tmp/openai_forward-0.0.9.tar.gz`

## Comparing `openai_forward-0.0.8.tar` & `openai_forward-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/__init__.py
--rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/__main__.py
--rwxr-xr-x   0        0        0     5713 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/_base.py
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/app.py
--rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/config.py
--rwxr-xr-x   0        0        0      490 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/openai.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/routers/__init__.py
--rwxr-xr-x   0        0        0      490 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/routers/openai_v1.py
--rwxr-xr-x   0        0        0     2316 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/routers/schemas.py
--rwxr-xr-x   0        0        0    40662 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/web/index.js
--rwxr-xr-x   0        0        0     1876 2020-02-02 00:00:00.000000 openai_forward-0.0.8/.gitignore
--rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.0.8/LICENSE
--rwxr-xr-x   0        0        0     3079 2020-02-02 00:00:00.000000 openai_forward-0.0.8/README.md
--rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 openai_forward-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 openai_forward-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/__init__.py
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/__main__.py
+-rwxr-xr-x   0        0        0     5672 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/_base.py
+-rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/app.py
+-rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/config.py
+-rwxr-xr-x   0        0        0      729 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/openai.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/routers/__init__.py
+-rwxr-xr-x   0        0        0      490 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/routers/openai_v1.py
+-rwxr-xr-x   0        0        0     2316 2020-02-02 00:00:00.000000 openai_forward-0.0.9/openai_forward/routers/schemas.py
+-rwxr-xr-x   0        0        0     1869 2020-02-02 00:00:00.000000 openai_forward-0.0.9/.gitignore
+-rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.0.9/LICENSE
+-rwxr-xr-x   0        0        0     5755 2020-02-02 00:00:00.000000 openai_forward-0.0.9/README.md
+-rwxr-xr-x   0        0        0     1562 2020-02-02 00:00:00.000000 openai_forward-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6942 2020-02-02 00:00:00.000000 openai_forward-0.0.9/PKG-INFO
```

### Comparing `openai_forward-0.0.8/openai_forward/_base.py` & `openai_forward-0.0.9/openai_forward/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import orjson
 from orjson import JSONDecodeError
-from fastapi import Request, Response, HTTPException, status
+from fastapi import Request
 from fastapi.responses import StreamingResponse, RedirectResponse, FileResponse
 from loguru import logger
 import httpx
 from httpx._decoders import LineDecoder
 from starlette.background import BackgroundTask
 import os
 from dotenv import load_dotenv
@@ -55,16 +55,15 @@
         else:
             self.allow_ips.append(ip)
 
     def validate_request_host(self, ip):
         if ip == "*" or ip in self.allow_ips:
             return True
         else:
-            raise HTTPException(status_code=status.HTTP_403_FORBIDDEN,
-                                detail=f"Forbidden, please add {ip=} to `allow_ips`")
+            return False
 
     @staticmethod
     def _parse_iter_line_content(line: str):
         line = line[6:]
         try:
             line_dict = orjson.loads(line)
             return line_dict['choices'][0]['delta']['content']
@@ -128,23 +127,26 @@
         else:
             tmp_headers = {}
 
         headers.pop("host", None)
         # headers.pop("user-agent", None)
         headers.update(tmp_headers)
         if cls.LOG_CHAT:
-            input_info = await request.json()
-            msgs = input_info['messages']
-            cls._current_chat_info.append(
-                {
-                    "model": input_info['model'],
-                    "messages": [{msg['role']: msg['content']} for msg in msgs],
-                }
-            )
-            logger.info(f"{input_info}")
+            try:
+                input_info = await request.json()
+                msgs = input_info['messages']
+                cls._current_chat_info.append(
+                    {
+                        "model": input_info['model'],
+                        "messages": [{msg['role']: msg['content']} for msg in msgs],
+                    }
+                )
+                logger.info(f"{input_info}")
+            except Exception as e:
+                logger.warning(e)
         req = client.build_request(
             request.method, url, headers=headers,
             content=request.stream(),
             timeout=cls.timeout,
         )
         r = await client.send(req, stream=True)
```

### Comparing `openai_forward-0.0.8/openai_forward/app.py` & `openai_forward-0.0.9/openai_forward/app.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.0.8/openai_forward/config.py` & `openai_forward-0.0.9/openai_forward/config.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.0.8/openai_forward/routers/schemas.py` & `openai_forward-0.0.9/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.0.8/.gitignore` & `openai_forward-0.0.9/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 .vscode/
 third-party/
 run.sh
 ssl/
 chat.yaml
 chat_*.yaml
 
-tests/
 Log/
 dist/
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `openai_forward-0.0.8/LICENSE` & `openai_forward-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.0.8/pyproject.toml` & `openai_forward-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "openai_forward"
 description = ""
 authors = [
     { name = "kunyuan", email = "beidongjiedeguang@gmail.com" },
 ]
 requires-python = ">=3.6"
 readme = "README.md"
-keywords = ["openai", "chatgpt", "api forward", "chatbot", "streaming-api", "fastapi", "openai-proxy"]
+keywords = ["openai", "chatgpt", "openai-api", "openai-proxy", "forward", "streaming-api", "fastapi", "python"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3"
 ]
 
 dependencies = [
```

