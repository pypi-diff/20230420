# Comparing `tmp/nonebot_plugin_ping-1.5.4.tar.gz` & `tmp/nonebot_plugin_ping-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ping-1.5.4.tar", last modified: Fri Feb  3 08:33:30 2023, max compression
+gzip compressed data, was "nonebot_plugin_ping-1.6.4.tar", last modified: Thu Apr 20 00:01:38 2023, max compression
```

## Comparing `nonebot_plugin_ping-1.5.4.tar` & `nonebot_plugin_ping-1.6.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-02-03 08:33:30.577775 nonebot_plugin_ping-1.5.4/
--rw-rw-rw-   0        0        0     1088 2022-12-24 04:11:04.000000 nonebot_plugin_ping-1.5.4/LICENSE
--rw-rw-rw-   0        0        0     1659 2023-02-03 08:33:30.577775 nonebot_plugin_ping-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-01-27 09:02:09.000000 nonebot_plugin_ping-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-02-03 08:33:30.560429 nonebot_plugin_ping-1.5.4/nonebot_plugin_ping/
--rw-rw-rw-   0        0        0     3869 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.5.4/nonebot_plugin_ping/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-03 08:33:30.566939 nonebot_plugin_ping-1.5.4/nonebot_plugin_ping.egg-info/
--rw-rw-rw-   0        0        0     1659 2023-02-03 08:33:30.000000 nonebot_plugin_ping-1.5.4/nonebot_plugin_ping.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-02-03 08:33:30.000000 nonebot_plugin_ping-1.5.4/nonebot_plugin_ping.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-03 08:33:30.000000 nonebot_plugin_ping-1.5.4/nonebot_plugin_ping.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-02-03 08:33:30.000000 nonebot_plugin_ping-1.5.4/nonebot_plugin_ping.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-02-03 08:33:30.000000 nonebot_plugin_ping-1.5.4/nonebot_plugin_ping.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-03 08:33:30.577775 nonebot_plugin_ping-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0     3944 2023-02-03 08:24:56.000000 nonebot_plugin_ping-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 00:01:38.354305 nonebot_plugin_ping-1.6.4/
+-rw-rw-rw-   0        0        0     1088 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.6.4/LICENSE
+-rw-rw-rw-   0        0        0     1659 2023-04-20 00:01:38.349371 nonebot_plugin_ping-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.6.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 00:01:38.339242 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping/
+-rw-rw-rw-   0        0        0     4392 2023-04-19 23:48:09.000000 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 00:01:38.349371 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping.egg-info/
+-rw-rw-rw-   0        0        0     1659 2023-04-20 00:01:38.000000 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-04-20 00:01:38.000000 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 00:01:38.000000 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-20 00:01:38.000000 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-20 00:01:38.000000 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 00:01:38.354305 nonebot_plugin_ping-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     3944 2023-04-19 23:59:42.000000 nonebot_plugin_ping-1.6.4/setup.py
```

### Comparing `nonebot_plugin_ping-1.5.4/LICENSE` & `nonebot_plugin_ping-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ping-1.5.4/PKG-INFO` & `nonebot_plugin_ping-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_ping
-Version: 1.5.4
+Version: 1.6.4
 Summary: ping
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_ping-1.5.4/README.md` & `nonebot_plugin_ping-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ping-1.5.4/nonebot_plugin_ping/__init__.py` & `nonebot_plugin_ping-1.6.4/nonebot_plugin_ping/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,66 +1,68 @@
-from nonebot.plugin.on import on_command
+﻿from nonebot.plugin.on import on_command
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 from nonebot.params import CommandArg
 from httpx import AsyncClient
 import nonebot
 import asyncio
 import platform
 
 try:
     model: int = nonebot.get_driver().config.ping
 except:
     model: int = 1
 
+from .httpcat import httpcat_msgs
+
 
 
 """PING网址"""
 ping = on_command('ping', aliases={'Ping'}, priority=60, block=True)
 @ping.handle()
 async def _(msg: Message = CommandArg()):
     url = msg.extract_plain_text().strip()
+
     if model == 1:
-        api = f'https://api.gmit.vip/Api/Ping?format=json&ip={url}'
+        api = f'https://v.api.aa1.cn/api/api-ping/ping.php?url={url}'
         message = await api_ping(api)
     elif model == 2:
         message = await cmd_ping(url)
     else:
         message = "PING 配置项填写有误, 联系 SUPPERUSER 检查!"
+
     await ping.finish(message)
 
+
 async def api_ping(api):
     async with AsyncClient() as client:
         res = (await client.get(api)).json()
-        if res["code"] == 200:
-            url = (res["info"]["request"]["query"]["ip"])
-            ip = (res["data"]["ip"])
-            max = (res["data"]["ping_max"])
-            min = (res["data"]["ping_min"])
-            avg = (res["data"]["ping_avg"])
-            place = (res["data"]["location"])
-            res = f"域名: {url}\nIP: {ip}\n最大延迟: {max}\n最小延迟: {min}\n平均延迟: {avg}\n服务器归属地: {place}"
-            return res
-        elif res["code"] == 400:
-            res = (res["msg"])
+        try:
+            url = (res["host"])
+            ip = (res["ip"])
+            max = (res["ping_time_max"])
+            min = (res["ping_time_min"])
+            place = (res["location"])
+            res = f"域名: {url}\nIP: {ip}\n最大延迟: {max}\n最小延迟: {min}\n服务器归属地: {place}"
             return res
-        else:
+        except Exception:
             return "寄"
 
 async def cmd_ping(url):
     # 获取系统信息, Windows 请求默认 4 次, Linux 请求默认不会停止.
     sys = platform.system()
     # 由于不同系统参数不同, 这里做一下判断.
     if sys == "Windows":
         url = f"ping {url} -n 4"
     elif sys == "Linux":
         # Ubuntu 系统是 -c , 其它发行版未测试.
         url = f"ping {url} -c 4"
     else:
         # 其它系统未测试.
         url = f"ping {url}"
+    
     p = await asyncio.subprocess.create_subprocess_shell(url, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.PIPE)
     stdout, stderr = await p.communicate()
     try:
         result = (stdout or stderr).decode('gb2312')
     except Exception:
         result = str(stdout or stderr)
     result = result.strip()
@@ -99,7 +101,24 @@
             regtime = (res["data"]["create_date"])
             exptime = (res["data"]["expire_date"])
             dnsserver = (res["data"]["nameserver"])
             status = (res["data"]["status"])
             updatetime = (res["data"]["update_date"])
             res = f"请求域名: {url}\n注册商: {reg}\n邮箱: {email}\n注册时间: {regtime}\n过期时间: {exptime}\nDNS服务器: {dnsserver}\n域名状态: {status}\n更新时间: {updatetime}"
             return res
+
+
+
+http_cat = on_command('http_cat', aliases={'httpcat','http猫'}, priority=5, block=True)
+@http_cat.handle()
+async def _handle(code: Message = CommandArg()):
+    url = "https://httpcats.com/{}.jpg".format(code)
+    msgs = await httpcat_msgs('http://www.httpstatus.cn/{}'.format(code))  
+    await http_cat.finish(msgs + MessageSegment.image(file=url, cache=False), at_sender=True)
+#httpx异步 await httpcat_msg(code)
+async def httpcat_msg(code):
+    msgs = await httpcat_msgs('http://www.httpstatus.cn/{}'.format(code))
+    return msgs
+#url同步 httpcat_pic(code)
+def httpcat_pic(code):
+    url = "https://httpcats.com/{}.jpg".format(code)
+    return str(url)
```

### Comparing `nonebot_plugin_ping-1.5.4/nonebot_plugin_ping.egg-info/PKG-INFO` & `nonebot_plugin_ping-1.6.4/nonebot_plugin_ping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ping
-Version: 1.5.4
+Version: 1.6.4
 Summary: ping
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_ping-1.5.4/setup.py` & `nonebot_plugin_ping-1.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'nonebot_plugin_ping'
 DESCRIPTION = 'ping'
 URL = 'https://github.com/zhulinyv/nonebot_plugin_ping'
 EMAIL = 'zhulinyv2005@outlook.com'
 AUTHOR = '(๑•小丫头片子•๑)'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.5.4'
+VERSION = '1.6.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'nonebot2', 'nonebot-adapter-onebot', 'httpx',
 ]
 
 # What packages are optional?
```

