# Comparing `tmp/gameyamlspiderandgenerator-1.2.0.tar.gz` & `tmp/gameyamlspiderandgenerator-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.2.0.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.3.0.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.2.0.tar` & `gameyamlspiderandgenerator-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1069 2023-04-14 04:39:09.582935 gameyamlspiderandgenerator-1.2.0/LICENSE
--rwxr-xr-x   0        0        0      809 2023-04-14 04:39:09.583123 gameyamlspiderandgenerator-1.2.0/README.md
--rwxr-xr-x   0        0        0      610 2023-04-14 04:39:09.583410 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0      980 2023-04-14 04:39:09.583612 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      753 2023-04-14 04:39:09.583800 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-04-14 04:39:09.584087 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      194 2023-04-14 04:39:09.584282 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0     2365 2023-04-16 02:41:59.202807 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0       56 2023-04-14 04:39:09.584827 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     2406 2023-04-14 04:39:09.585063 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     6985 2023-04-17 07:30:56.959305 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7561 2023-04-17 06:48:24.156686 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-04-14 04:39:09.585883 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1133 2023-04-17 06:52:34.054978 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1447 2023-04-17 07:29:28.159875 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1908 2023-04-17 06:46:51.090830 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     1944 2023-04-16 02:40:43.137333 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2611 2023-04-16 02:40:42.901945 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      617 2023-04-17 07:35:59.555205 gameyamlspiderandgenerator-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-04-20 06:26:01.842563 gameyamlspiderandgenerator-1.3.0/LICENSE
+-rwxr-xr-x   0        0        0      809 2023-04-20 06:26:01.842841 gameyamlspiderandgenerator-1.3.0/README.md
+-rwxr-xr-x   0        0        0      604 2023-04-20 08:11:44.723735 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0      980 2023-04-20 06:26:01.843615 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      753 2023-04-20 06:26:01.843909 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-04-20 06:26:01.844401 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      194 2023-04-20 06:26:01.844722 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0     2659 2023-04-20 08:17:40.725993 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0       56 2023-04-20 06:26:01.845620 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     2586 2023-04-20 08:13:25.308014 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7013 2023-04-20 07:59:29.061316 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7706 2023-04-20 08:13:03.423899 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-04-20 06:26:01.847280 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1133 2023-04-20 06:26:01.847686 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1459 2023-04-20 08:19:19.429134 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1908 2023-04-20 06:26:01.848348 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     1944 2023-04-20 06:26:01.848713 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2611 2023-04-20 06:26:01.849061 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      639 2023-04-20 08:23:07.635645 gameyamlspiderandgenerator-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.3.0/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.2.0/LICENSE` & `gameyamlspiderandgenerator-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.2.0/README.md` & `gameyamlspiderandgenerator-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import Optional, Callable
+from typing import Optional
 
 from loguru import logger
 
 from .plugin import BasePlugin
 from .util.fgi_yaml import YamlData
 from .util.plugin_manager import pkg
 
 
-def verify(url: str) -> Optional[Callable]:
+def verify(url: str) -> Optional[BasePlugin]:
     verify_list = [
         [
             pkg.plugin[n].verify,
             pkg.plugin[n],
         ]
         for n in pkg.plugin
     ]
     return next((cls for func, cls in verify_list if func(url)), None)
 
 
 def produce_yaml(url: str) -> Optional[YamlData]:
-    ret: Callable = verify(url)
+    ret: BasePlugin = verify(url)
     if ret is None:
         logger.error("URL is invalid")
         return
     return ret(url).to_yaml()
```

### Comparing `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     def __load_hook__(self, data: dict):
         """
         加载钩子
 
         Args:
             data: 钩子数据
         """
+        from gameyamlspiderandgenerator.util.plugin_manager import pkg
+        pkg.__init__()
+        for i in pkg.hook.values():
+            return i(self.get_name()).setup(data)
 
     @abc.abstractmethod
     def get_name(self) -> str:
         """
         获取游戏名称
 
         Returns:
```

### Comparing `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import itertools
 import re
 from contextlib import suppress
 from json import loads
-from re import match, sub
 from bs4 import BeautifulSoup
 from html2text import html2text
 from langcodes import find
 
 from ._base import BasePlugin
 from ..util.fgi import fgi_dict
 from ..util.fgi_yaml import YamlData, pss_dedent
@@ -18,14 +16,15 @@
 
     @staticmethod
     def remove_query(s: str):
         s = re.sub(r"\?t=\d{6,12}", "", s)
         return s.replace("![]", "![img]")
 
     def __init__(self, link: str) -> None:
+        self.link = link
         self.data_html = get_text(link)
         self.soup = BeautifulSoup(self.data_html, "html.parser")
         self.data = [
             ii
             for ii in [
                 loads(i.text)
                 for i in self.soup.find_all(
@@ -57,15 +56,15 @@
         temp = self.soup.select_one("div.columns > div.right_col.column > div.screenshot_list").select('a')
         return [i.attrs['href'] for i in temp]
 
     def get_desc(self):
         return pss_dedent(self.remove_query(html2text(
             str(self.soup.select_one("div.formatted_description.user_formatted")),
             bodywidth=0,
-        )).replace("\n"*4, "\n").strip())
+        )).replace("\n" * 4, "\n").strip())
 
     def get_platforms(self):
         repl = {
             "Windows": "windows",
             "macOS": "macos",
             "Linux": "linux",
             "Android": "android",
@@ -111,15 +110,17 @@
         return list(set(ret))
 
     def get_langs(self) -> list[str]:
         temp = self.more_info["Languages"] if "Languages" in self.more_info else ["English"]
         return list(set(find(i).language for i in temp))
 
     def get_links(self) -> list[dict]:
-        link = [i.attrs["href"] for i in self.soup.select_one("div.left_col.column > div.formatted_description.user_formatted").select("a[href]")]
+        link = [i.attrs["href"] for i in self.soup.select_one("div.left_col.column > "
+                                                              "div.formatted_description.user_formatted").select("a["
+                                                                                                                 "href]")]
         data = [{"url": i, "processed": False} for i in list(set(link))]
         processed_data = []
         for i in data:
             for p in fgi_dict:
                 if re.match(p["match"], i["url"]):
                     processed_data.append(
                         {
@@ -127,53 +128,48 @@
                             "uri": re.sub(p["match"], p["replace"], i["url"]),
                         }
                     )
                     i["processed"] = True
         for i in data:
             if not i["processed"]:
                 processed_data.append({"name": ".website", "uri": i["url"]})
+        processed_data.append({"name": ".itchio", "uri": self.link})
         return processed_data
 
     def get_more_info(self):
         d = {}
         for i in range(1, 18):
             with suppress(Exception):
                 cache = self.soup.select_one(
                     f"div.info_panel_wrapper > div > table > tbody > tr:nth-child({str(i)})"
                 )
                 temp = [i.get_text() for i in list(cache.children)]
                 d[temp[0]] = temp[1:][0].split(",")
         return d
 
-    def __load_hook__(self, data: dict):
-        from gameyamlspiderandgenerator.util.plugin_manager import pkg
-
-        temp = data.copy()
-        for _ in pkg["hook"].values():
-            temp = pkg["hook"].Search(self.get_name()).setup(temp)
-        return temp
 
     def to_yaml(self) -> YamlData:
         ret = {
             "name": self.get_name(),
             "brief-description": self.get_brief_desc(),
             "description": self.get_desc(),
             "description-format": "markdown",
             "authors": self.get_authors(),
             "tags": {
                 "type": self.get_type_tag(),
                 "lang": self.get_langs(),
                 "platform": self.get_platforms(),
+                "publish": [".itchio"],
                 "misc": self.get_misc_tags(),
             },
             "links": self.get_links(),
             "thumbnail": self.get_thumbnail(),
             "screenshots": self.get_screenshots()  # + self.get_video(),
         }
-        return YamlData(ret)
+        return YamlData(self.__load_hook__(ret))
 
     def get_type_tag(self):
         repl = {
             "Visual Novel": "visual-nove",
             "Real time strategy": "Real time strategy",
             "Strategy": "strategy",
             "Casual": "casual",
```

### Comparing `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,21 +44,22 @@
             "description": self.get_desc(),
             "description-format": "markdown",
             "authors": self.get_authors(),
             "tags": {
                 "type": self.get_type_tag(),
                 "lang": self.get_langs(),
                 "platform": self.get_platforms(),
+                "publish": ["steam"],
                 "misc": self.get_misc_tags(),
             },
             "links": self.get_links(),
             "thumbnail": self.get_thumbnail(),
             "screenshots": self.get_screenshots() + self.get_video(),  # type: ignore
         }
-        return YamlData(ret)
+        return YamlData(self.__load_hook__(ret))
 
     def get_langs(self) -> list[str]:
         temp = self.data[str(self.id)]["data"]["supported_languages"].split(",")
         return list({find(i).language for i in temp})
 
     def get_desc(self):
         return pss_dedent(
@@ -112,16 +113,16 @@
         }
 
         ret = []
         for i, value in repl.items():
             ret.extend(value for ii in self.tag if i in ii)
         return list(set(ret))
 
-    def get_tags(self) -> list[dict]:
-        pass
+    def get_tags(self) -> list[str]:
+        return self.tag
 
     def get_misc_tags(self):
         repl = {
             "3D": "3d",
             "Pixel": "pixel-art",
             "Multiplayer": "multiplayer",
             "PvP": "pvp",
@@ -210,13 +211,14 @@
                             "uri": re.sub(p["match"], p["replace"], i["url"]),
                         }
                     )
                     i["processed"] = True
         for i in data:
             if not i["processed"]:
                 processed_data.append({"name": ".website", "uri": i["url"]})
+        processed_data.append({"name": ".steam", "uri": f'steam:{self.id}'})
         return processed_data
 
     def get_thumbnail(self):
         return self.remove_query(
             self.soup.body.find("img", {"class": "game_header_image_full"}).attrs["src"]
         )
```

### Comparing `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/config.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/fgi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 fgi_dict = [
     {
-        "match": "^https://www.youtube.com/@?([^/]+)/?",
+        "match": "^https://www.youtube.com/(?!watch\?v=)(@?.+)",
         "prefix": ".youtube",
         "replace": "youtube:@\\g<1>",
     },
     {
         "match": "^https://www.youtube.com/channel/(.+[^/])",
         "prefix": ".youtube",
         "replace": "youtube:\\g<1>",
@@ -21,25 +21,25 @@
     },
     {
         "match": "^https://discord.gg/(.+)",
         "prefix": ".discord",
         "replace": "discord:\\g<1>",
     },
     {
-        "match": "https://www.facebook.com/(.+)/",
+        "match": "^https://www.facebook.com/(.+)/",
         "prefix": ".facebook",
         "replace": "facebook:\\g<1>",
     },
     {
-        "match": "https://www.furaffinity.net/user/(.+)/",
+        "match": "^https://www.furaffinity.net/user/(.+)/",
         "prefix": ".furaffinity",
         "replace": "furaffinity:\\g<1>",
     },
     {
-        "match": "(https://weibo.com/.+)",
+        "match": "(https://weibo.com/u/.+)",
         "prefix": ".weibo",
         "replace": "\\g<1>",
     },
 ]
 default_config = {'api': {'apple': 'a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90',
                           'google-play': 'a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90'},
                   'gitToken': 'your token',
```

### Comparing `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.2.0/pyproject.toml` & `gameyamlspiderandgenerator-1.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.2.0"
+version = "1.3.0"
 description = ""
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -18,14 +18,15 @@
 pillow = "^9.4.0"
 pygithub = "^1.57"
 requests = "^2.28.2"
 ruamel-base = "^1.0.0"
 loguru = "^0.6.0"
 pyyaml = "^6.0"
 pysocks = "^1.7.1"
+marisa-trie = "0.7.8"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `gameyamlspiderandgenerator-1.2.0/PKG-INFO` & `gameyamlspiderandgenerator-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.2.0
+Version: 1.3.0
 Summary: 
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.1,<2.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: marisa-trie (==0.7.8)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: pygithub (>=1.57,<2.0)
 Requires-Dist: pysocks (>=1.7.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: ruamel-base (>=1.0.0,<2.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
```

