# Comparing `tmp/AnimeCrawler-0.1.0.tar.gz` & `tmp/AnimeCrawler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnimeCrawler-0.1.0.tar", last modified: Mon Apr 17 15:15:14 2023, max compression
+gzip compressed data, was "AnimeCrawler-0.1.1.tar", last modified: Thu Apr 20 12:53:34 2023, max compression
```

## Comparing `AnimeCrawler-0.1.0.tar` & `AnimeCrawler-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 15:15:14.310238 AnimeCrawler-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-04-17 15:15:14.229957 AnimeCrawler-0.1.0/AnimeCrawler/
--rw-rw-rw-   0        0        0      198 2023-04-17 13:33:24.000000 AnimeCrawler-0.1.0/AnimeCrawler/__init__.py
--rw-rw-rw-   0        0        0      115 2023-04-17 14:04:39.000000 AnimeCrawler-0.1.0/AnimeCrawler/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:15:14.248946 AnimeCrawler-0.1.0/AnimeCrawler/command/
--rw-rw-rw-   0        0        0       87 2023-04-17 13:43:55.000000 AnimeCrawler-0.1.0/AnimeCrawler/command/__init__.py
--rw-rw-rw-   0        0        0     1602 2023-04-17 14:38:14.000000 AnimeCrawler-0.1.0/AnimeCrawler/command/run.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:15:14.259940 AnimeCrawler-0.1.0/AnimeCrawler/mhyyy/
--rw-rw-rw-   0        0        0      245 2023-04-17 13:09:32.000000 AnimeCrawler-0.1.0/AnimeCrawler/mhyyy/__init__.py
--rw-rw-rw-   0        0        0     2024 2023-04-17 13:09:52.000000 AnimeCrawler-0.1.0/AnimeCrawler/mhyyy/downloader.py
--rw-rw-rw-   0        0        0     3780 2023-04-17 14:28:08.000000 AnimeCrawler-0.1.0/AnimeCrawler/mhyyy/spider.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:15:14.302186 AnimeCrawler-0.1.0/AnimeCrawler/utils/
--rw-rw-rw-   0        0        0      113 2023-04-17 13:08:48.000000 AnimeCrawler-0.1.0/AnimeCrawler/utils/__init__.py
--rw-rw-rw-   0        0        0      804 2023-04-16 14:41:04.000000 AnimeCrawler-0.1.0/AnimeCrawler/utils/decode.py
--rw-rw-rw-   0        0        0     2030 2023-04-17 11:41:57.000000 AnimeCrawler-0.1.0/AnimeCrawler/utils/file.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:15:14.242949 AnimeCrawler-0.1.0/AnimeCrawler.egg-info/
--rw-rw-rw-   0        0        0     3406 2023-04-17 15:15:13.000000 AnimeCrawler-0.1.0/AnimeCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-04-17 15:15:14.000000 AnimeCrawler-0.1.0/AnimeCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:15:13.000000 AnimeCrawler-0.1.0/AnimeCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 15:15:13.000000 AnimeCrawler-0.1.0/AnimeCrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-17 15:15:13.000000 AnimeCrawler-0.1.0/AnimeCrawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2023-04-15 13:28:24.000000 AnimeCrawler-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3406 2023-04-17 15:15:14.309238 AnimeCrawler-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2989 2023-04-17 15:08:48.000000 AnimeCrawler-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 15:15:14.311236 AnimeCrawler-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      768 2023-04-17 14:50:03.000000 AnimeCrawler-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:53:34.212812 AnimeCrawler-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-04-20 12:53:34.093887 AnimeCrawler-0.1.1/AnimeCrawler/
+-rw-rw-rw-   0        0        0      248 2023-04-18 15:03:38.000000 AnimeCrawler-0.1.1/AnimeCrawler/__init__.py
+-rw-rw-rw-   0        0        0      311 2023-04-19 14:06:47.000000 AnimeCrawler-0.1.1/AnimeCrawler/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:53:34.167838 AnimeCrawler-0.1.1/AnimeCrawler/command/
+-rw-rw-rw-   0        0        0       87 2023-04-17 15:39:52.000000 AnimeCrawler-0.1.1/AnimeCrawler/command/__init__.py
+-rw-rw-rw-   0        0        0     3542 2023-04-20 12:45:39.000000 AnimeCrawler-0.1.1/AnimeCrawler/command/run.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:53:34.194822 AnimeCrawler-0.1.1/AnimeCrawler/mhyyy/
+-rw-rw-rw-   0        0        0      245 2023-04-17 15:39:52.000000 AnimeCrawler-0.1.1/AnimeCrawler/mhyyy/__init__.py
+-rw-rw-rw-   0        0        0     2024 2023-04-17 15:39:52.000000 AnimeCrawler-0.1.1/AnimeCrawler/mhyyy/downloader.py
+-rw-rw-rw-   0        0        0     3846 2023-04-19 13:04:13.000000 AnimeCrawler-0.1.1/AnimeCrawler/mhyyy/spider.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:53:34.205821 AnimeCrawler-0.1.1/AnimeCrawler/utils/
+-rw-rw-rw-   0        0        0      113 2023-04-17 15:39:52.000000 AnimeCrawler-0.1.1/AnimeCrawler/utils/__init__.py
+-rw-rw-rw-   0        0        0      804 2023-04-17 15:39:52.000000 AnimeCrawler-0.1.1/AnimeCrawler/utils/decode.py
+-rw-rw-rw-   0        0        0     2131 2023-04-19 13:15:05.000000 AnimeCrawler-0.1.1/AnimeCrawler/utils/file.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:53:34.147849 AnimeCrawler-0.1.1/AnimeCrawler.egg-info/
+-rw-rw-rw-   0        0        0     3411 2023-04-20 12:53:33.000000 AnimeCrawler-0.1.1/AnimeCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-04-20 12:53:33.000000 AnimeCrawler-0.1.1/AnimeCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 12:53:33.000000 AnimeCrawler-0.1.1/AnimeCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-20 12:53:33.000000 AnimeCrawler-0.1.1/AnimeCrawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-20 12:53:33.000000 AnimeCrawler-0.1.1/AnimeCrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-20 12:53:33.000000 AnimeCrawler-0.1.1/AnimeCrawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2023-04-15 13:28:24.000000 AnimeCrawler-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3411 2023-04-20 12:53:34.208814 AnimeCrawler-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2962 2023-04-20 12:31:36.000000 AnimeCrawler-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 12:53:34.213812 AnimeCrawler-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-04-20 12:52:40.000000 AnimeCrawler-0.1.1/setup.py
```

### Comparing `AnimeCrawler-0.1.0/AnimeCrawler/mhyyy/downloader.py` & `AnimeCrawler-0.1.1/AnimeCrawler/mhyyy/downloader.py`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.1.0/AnimeCrawler/mhyyy/spider.py` & `AnimeCrawler-0.1.1/AnimeCrawler/mhyyy/spider.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,25 +25,26 @@
 
 class AnimeSpider(Spider):
     _base_ts_url = None
     _mixed_m3u8 = None
     headers = {'User-Agent': 'Mozilla/5.0'}
 
     @classmethod
-    def init(cls, anime_title: str, start_urls: str):
+    def init(cls, anime_title: str, start_urls: str, del_ts: bool = False):
         '''初始化爬虫
 
         Args:
             anime_title (str): 动漫标题，用于取文件夹的名称，利于管理动漫
             start_urls (str): 第一页的网址
 
         Returns:
             cls: 为了链式调用返回了cls
         '''
-        cls.start_urls = start_urls
+        cls.start_urls = [start_urls]
+        cls.del_ts = del_ts
         video_path = Path(get_video_path()) / anime_title  # 在项目目录下存储
         cls.PATH = folder_path(video_path)
         return cls
 
     async def _mixed_m3u8_url_parse(self, index_m3u8_url: str, item: AnimeItem) -> None:
         resp = await self.request(index_m3u8_url).fetch()
         text = await resp.text()
@@ -95,12 +96,12 @@
         episodes = item.episodes
         folder_path = self.PATH / f'{episodes}'
         print('\033[0;32;40m写入mixed.m3u8\033[0m')
         await write(folder_path, text, 'mixed', 'm3u8', 'w+')
         urls = self._parse_mixed_m3u8(item)
         await Downloader(urls).download_ts_files(folder_path, episodes)
         self.logger.info(f"正在把第 {episodes} 集的ts文件转码成 mp4")
-        await merge_ts2mp4(folder_path, episodes)
+        await merge_ts2mp4(folder_path, episodes, self.del_ts)
 
 
 if __name__ == '__main__':
     AnimeSpider.init('魔女之旅', ['https://www.mhyyy.com/play/166269-1-1.html']).start()
```

### Comparing `AnimeCrawler-0.1.0/AnimeCrawler/utils/decode.py` & `AnimeCrawler-0.1.1/AnimeCrawler/utils/decode.py`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.1.0/AnimeCrawler/utils/file.py` & `AnimeCrawler-0.1.1/AnimeCrawler/utils/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,19 +55,22 @@
         Defaults to 'a'.
     '''
     folder = folder_path(path)
     async with aiofiles.open(folder / f'{title}.{suffix}', mode) as fp:
         await fp.write(text)
 
 
-async def merge_ts2mp4(folder_path: Path, episodes: int = None):
+async def merge_ts2mp4(folder_path: Path, episodes: int = None, del_ts: bool = False):
     '''将ts文件合并成mp4
 
     Args:
         folder_path (Path): 文件夹路径，里面应有ts文件
         episodes (int): 动漫集数. Defaults to None.
     '''
+    print(del_ts)
     for file_path in folder_path.iterdir():
         if file_path.suffix == '.ts':
             with open(file_path, 'rb') as f1:
                 with open(folder_path / f"第{episodes}集.mp4", 'ab') as f2:
                     f2.write(f1.read())
+            if del_ts:
+                file_path.unlink()
```

### Comparing `AnimeCrawler-0.1.0/AnimeCrawler.egg-info/PKG-INFO` & `AnimeCrawler-0.1.1/AnimeCrawler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: AnimeCrawler
-Version: 0.1.0
-Summary: test
+Version: 0.1.1
+Summary: 一个可免费下载动漫的爬虫
 Home-page: https://github.com/Senvlin/AnimeCrawler
 Author: Senvlin
 Author-email: 2994515402@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -22,15 +22,15 @@
 <p align="center">网络原因，把我拒之门外</p>
 
 <p align="center">惆怅万分，决定用爬虫改变现状</p>
 
 <p align="center">离线播放，享受流畅的观看体验</p>
 
 
-这是一款基于 <code>[**Ruia**](https://github.com/howie6879/ruia)</code> 轻量级框架、在Windows平台下专门爬取免费动漫的爬虫，底层使用<code>aiohttp</code>库，使用异步模式，大幅增加爬取及下载速度。可**离线播放**各大动漫，支持命令行输入，立志成为最实用，最轻量的动漫管理及下载助手
+这是一款在Windows平台下基于轻量级框架<code>[**Ruia**](https://github.com/howie6879/ruia)</code>、专门爬取免费动漫的爬虫，底层使用<code>aiohttp</code>库，使用异步模式，大幅增加爬取及下载速度。可**离线播放**各大动漫，支持**命令行输入**，立志成为最实用，最轻量的动漫管理及下载助手
 
 ## ❓如何使用
 1. 首先来到[这里](https://www.python.org/downloads)下载Python解释器, 要求Python3.8及以上版本，安装即可
 2. 然后，打开命令提示符，输入 <code>pip install AnimeCrawler</code>
 3. 其次，来到[这个网站](https://www.mhyyy.com/),搜索您喜欢的动漫，点击播放页，将第一页的url复制一下
 4. 最后，打开命令提示符，输入 <code>python -m AnimeCrawler "动漫名称" "url"</code> 回车就可以下载啦
     - 输入 <code>python -m AnimeCrawler -h</code> 会有详细的说明
@@ -45,17 +45,16 @@
 
 > 有的时候在dev分支中，您的需求如一些bug（或feature）已解决（或已被实现），请确认后再提交Issue
 
 ## 📝TODO
 
 - [x] 下载多集动漫
 - [x] 支持命令行工具
-- [ ] 支持动漫检索
+- [ ] 支持检索动漫
 - [ ] 可更换下载源
-- [ ] 支持命令行输入
 - [ ] 支持上传网盘
 - [ ] <span style="text-decoration: line-through">甚至是GUI</span>
 
 ## 🧱从源码搭建
 1. 点击[这里](https://github.com/Senvlin/AnimeCrawler/releases)找到最新版本，下载源码
 2. 转到项目目录，使用 <code>pip install -r requirement.txt</code> 安装依赖库
 3. 随后使用 <code>python -m AnimeCrawler "动漫名称" "url"</code> 或打开 <code>AnimeCrawler\mhyyy\spider.py</code>运行即可
```

### Comparing `AnimeCrawler-0.1.0/LICENSE` & `AnimeCrawler-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.1.0/PKG-INFO` & `AnimeCrawler-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: AnimeCrawler
-Version: 0.1.0
-Summary: test
+Version: 0.1.1
+Summary: 一个可免费下载动漫的爬虫
 Home-page: https://github.com/Senvlin/AnimeCrawler
 Author: Senvlin
 Author-email: 2994515402@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -22,15 +22,15 @@
 <p align="center">网络原因，把我拒之门外</p>
 
 <p align="center">惆怅万分，决定用爬虫改变现状</p>
 
 <p align="center">离线播放，享受流畅的观看体验</p>
 
 
-这是一款基于 <code>[**Ruia**](https://github.com/howie6879/ruia)</code> 轻量级框架、在Windows平台下专门爬取免费动漫的爬虫，底层使用<code>aiohttp</code>库，使用异步模式，大幅增加爬取及下载速度。可**离线播放**各大动漫，支持命令行输入，立志成为最实用，最轻量的动漫管理及下载助手
+这是一款在Windows平台下基于轻量级框架<code>[**Ruia**](https://github.com/howie6879/ruia)</code>、专门爬取免费动漫的爬虫，底层使用<code>aiohttp</code>库，使用异步模式，大幅增加爬取及下载速度。可**离线播放**各大动漫，支持**命令行输入**，立志成为最实用，最轻量的动漫管理及下载助手
 
 ## ❓如何使用
 1. 首先来到[这里](https://www.python.org/downloads)下载Python解释器, 要求Python3.8及以上版本，安装即可
 2. 然后，打开命令提示符，输入 <code>pip install AnimeCrawler</code>
 3. 其次，来到[这个网站](https://www.mhyyy.com/),搜索您喜欢的动漫，点击播放页，将第一页的url复制一下
 4. 最后，打开命令提示符，输入 <code>python -m AnimeCrawler "动漫名称" "url"</code> 回车就可以下载啦
     - 输入 <code>python -m AnimeCrawler -h</code> 会有详细的说明
@@ -45,17 +45,16 @@
 
 > 有的时候在dev分支中，您的需求如一些bug（或feature）已解决（或已被实现），请确认后再提交Issue
 
 ## 📝TODO
 
 - [x] 下载多集动漫
 - [x] 支持命令行工具
-- [ ] 支持动漫检索
+- [ ] 支持检索动漫
 - [ ] 可更换下载源
-- [ ] 支持命令行输入
 - [ ] 支持上传网盘
 - [ ] <span style="text-decoration: line-through">甚至是GUI</span>
 
 ## 🧱从源码搭建
 1. 点击[这里](https://github.com/Senvlin/AnimeCrawler/releases)找到最新版本，下载源码
 2. 转到项目目录，使用 <code>pip install -r requirement.txt</code> 安装依赖库
 3. 随后使用 <code>python -m AnimeCrawler "动漫名称" "url"</code> 或打开 <code>AnimeCrawler\mhyyy\spider.py</code>运行即可
```

### Comparing `AnimeCrawler-0.1.0/README.md` & `AnimeCrawler-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 <p align="center">网络原因，把我拒之门外</p>
 
 <p align="center">惆怅万分，决定用爬虫改变现状</p>
 
 <p align="center">离线播放，享受流畅的观看体验</p>
 
 
-这是一款基于 <code>[**Ruia**](https://github.com/howie6879/ruia)</code> 轻量级框架、在Windows平台下专门爬取免费动漫的爬虫，底层使用<code>aiohttp</code>库，使用异步模式，大幅增加爬取及下载速度。可**离线播放**各大动漫，支持命令行输入，立志成为最实用，最轻量的动漫管理及下载助手
+这是一款在Windows平台下基于轻量级框架<code>[**Ruia**](https://github.com/howie6879/ruia)</code>、专门爬取免费动漫的爬虫，底层使用<code>aiohttp</code>库，使用异步模式，大幅增加爬取及下载速度。可**离线播放**各大动漫，支持**命令行输入**，立志成为最实用，最轻量的动漫管理及下载助手
 
 ## ❓如何使用
 1. 首先来到[这里](https://www.python.org/downloads)下载Python解释器, 要求Python3.8及以上版本，安装即可
 2. 然后，打开命令提示符，输入 <code>pip install AnimeCrawler</code>
 3. 其次，来到[这个网站](https://www.mhyyy.com/),搜索您喜欢的动漫，点击播放页，将第一页的url复制一下
 4. 最后，打开命令提示符，输入 <code>python -m AnimeCrawler "动漫名称" "url"</code> 回车就可以下载啦
     - 输入 <code>python -m AnimeCrawler -h</code> 会有详细的说明
@@ -31,17 +31,16 @@
 
 > 有的时候在dev分支中，您的需求如一些bug（或feature）已解决（或已被实现），请确认后再提交Issue
 
 ## 📝TODO
 
 - [x] 下载多集动漫
 - [x] 支持命令行工具
-- [ ] 支持动漫检索
+- [ ] 支持检索动漫
 - [ ] 可更换下载源
-- [ ] 支持命令行输入
 - [ ] 支持上传网盘
 - [ ] <span style="text-decoration: line-through">甚至是GUI</span>
 
 ## 🧱从源码搭建
 1. 点击[这里](https://github.com/Senvlin/AnimeCrawler/releases)找到最新版本，下载源码
 2. 转到项目目录，使用 <code>pip install -r requirement.txt</code> 安装依赖库
 3. 随后使用 <code>python -m AnimeCrawler "动漫名称" "url"</code> 或打开 <code>AnimeCrawler\mhyyy\spider.py</code>运行即可
```

### Comparing `AnimeCrawler-0.1.0/setup.py` & `AnimeCrawler-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AnimeCrawler",
-    version="v0.1.0",
+    version="v0.1.1",
     author="Senvlin",
     author_email="2994515402@qq.com",
-    description="test",
+    description="一个可免费下载动漫的爬虫",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Senvlin/AnimeCrawler",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'ruia==0.8.5',
-        'tqdm==4.65.0',
-        'aiofiles==23.1.0',
+        'ruia',
+        'tqdm',
+        'aiofiles',
     ],
+    entry_points={
+        'console_scripts': [
+            'animecrawler = AnimeCrawler.command.run:main',
+        ],
+    },
     python_requires='>=3.8',
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

