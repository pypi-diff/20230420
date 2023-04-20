# Comparing `tmp/twtvt-2023.4.17.post1.tar.gz` & `tmp/twtvt-2023.4.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twtvt-2023.4.17.post1.tar", max compression
+gzip compressed data, was "twtvt-2023.4.20.tar", max compression
```

## Comparing `twtvt-2023.4.17.post1.tar` & `twtvt-2023.4.20.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1017 2023-04-17 07:34:24.441033 twtvt-2023.4.17.post1/README.md
--rw-r--r--   0        0        0     1465 2023-04-17 07:34:51.005530 twtvt-2023.4.17.post1/pyproject.toml
--rw-r--r--   0        0        0      120 2023-04-17 07:34:24.441033 twtvt-2023.4.17.post1/twtvt/__init__.py
--rw-r--r--   0        0        0      110 2023-04-17 07:34:24.441033 twtvt-2023.4.17.post1/twtvt/__main__.py
--rw-r--r--   0        0        0       41 2023-04-17 07:34:24.441033 twtvt-2023.4.17.post1/twtvt/cli/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-17 07:34:24.441033 twtvt-2023.4.17.post1/twtvt/cli/commands.py
--rw-r--r--   0        0        0       79 2023-04-17 07:34:24.441033 twtvt-2023.4.17.post1/twtvt/main.py
--rw-r--r--   0        0        0        0 2023-04-17 07:34:24.441033 twtvt-2023.4.17.post1/twtvt/tests/__init__.py
--rw-r--r--   0        0        0       47 2023-04-17 07:34:24.441033 twtvt-2023.4.17.post1/twtvt/tests/sample_test.py
--rw-r--r--   0        0        0      238 2023-04-17 07:34:24.441033 twtvt-2023.4.17.post1/twtvt/utils/__init__.py
--rw-r--r--   0        0        0     5159 2023-04-17 07:34:24.441033 twtvt-2023.4.17.post1/twtvt/utils/download_video.py
--rw-r--r--   0        0        0      249 2023-04-17 07:34:24.441033 twtvt-2023.4.17.post1/twtvt/utils/logger.py
--rw-r--r--   0        0        0     1354 2023-04-17 07:34:24.441033 twtvt-2023.4.17.post1/twtvt/utils/monsnode_parser.py
--rw-r--r--   0        0        0     7832 2023-04-17 07:34:24.441033 twtvt-2023.4.17.post1/twtvt/utils/twitter_parser.py
--rw-r--r--   0        0        0      566 2023-04-17 07:34:24.441033 twtvt-2023.4.17.post1/twtvt/utils/uri_validator.py
--rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 twtvt-2023.4.17.post1/PKG-INFO
+-rw-r--r--   0        0        0     1017 2023-04-20 08:27:49.976533 twtvt-2023.4.20/README.md
+-rw-r--r--   0        0        0     1463 2023-04-20 08:28:13.872202 twtvt-2023.4.20/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/__init__.py
+-rw-r--r--   0        0        0      110 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/__main__.py
+-rw-r--r--   0        0        0       41 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/cli/__init__.py
+-rw-r--r--   0        0        0     1357 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/cli/commands.py
+-rw-r--r--   0        0        0       79 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/tests/sample_test.py
+-rw-r--r--   0        0        0      238 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/utils/__init__.py
+-rw-r--r--   0        0        0     6643 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/utils/download_video.py
+-rw-r--r--   0        0        0      327 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/utils/execute_parallel.py
+-rw-r--r--   0        0        0      842 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/utils/istarmap.py
+-rw-r--r--   0        0        0      249 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/utils/logger.py
+-rw-r--r--   0        0        0     1354 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/utils/monsnode_parser.py
+-rw-r--r--   0        0        0     7832 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/utils/twitter_parser.py
+-rw-r--r--   0        0        0      566 2023-04-20 08:27:49.976533 twtvt-2023.4.20/twtvt/utils/uri_validator.py
+-rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 twtvt-2023.4.20/PKG-INFO
```

### Comparing `twtvt-2023.4.17.post1/README.md` & `twtvt-2023.4.20/README.md`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.17.post1/pyproject.toml` & `twtvt-2023.4.20/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "twtvt"
-version = "2023.04.17-1"
+version = "2023.04.20"
 description = ""
 authors = []
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "twtvt"
 
 [tool.pyright]
```

### Comparing `twtvt-2023.4.17.post1/twtvt/cli/commands.py` & `twtvt-2023.4.20/twtvt/cli/commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,27 +6,32 @@
 from twtvt.utils import download_video
 
 cli_app = Typer()
 
 
 @cli_app.command()
 def twtvt(
-    target_uris: list[str] = typer.Argument(..., help="Video tweet link, target user's likes or media, or file path."),
-    username: Optional[str] = typer.Option(None, help='Your twitter credentials username.'),
-    password: Optional[str] = typer.Option(None, help='Your twitter credentials password.'),
-    cookies_from_browser: Optional[str] = typer.Option(None, help='Browser to get cookies from. '),
-    output: str = typer.Option('.', help='Output path for downloaded videos.'),
-    debug: bool = typer.Option(False, help='Enable debug mode. This disables headless mode of Browser.'),
-    until_link: Optional[str] = typer.Option(
-        None,
-        help="Keeps finding videos until this link is found. None for no limit. Only for user's likes or media.",
-    ),
+        target_uris: list[str] = typer.Argument(
+            ...,
+            help="Video tweet link, target user's likes or media, or file path.",
+        ),
+        username: Optional[str] = typer.Option(None, help='Your twitter credentials username.'),
+        password: Optional[str] = typer.Option(None, help='Your twitter credentials password.'),
+        cookies_from_browser: Optional[str] = typer.Option(None, help='Browser to get cookies from. '),
+        output: str = typer.Option('.', help='Output path for downloaded videos.'),
+        debug: bool = typer.Option(False, help='Enable debug mode. This disables headless mode of Browser.'),
+        until_link: Optional[str] = typer.Option(
+            None,
+            help="Keeps finding videos until this link is found. None for no limit. Only for user's likes or media.",
+        ),
+        parallel: bool = typer.Option(False, help='Download videos in parallel.'),
 ):
     download_video(
         target_uris=target_uris,
         username=username,
         password=password,
         output=output,
         debug=debug,
         cookies_from_browser=cookies_from_browser,
         until_link=until_link,
+        parallel=parallel,
     )
```

### Comparing `twtvt-2023.4.17.post1/twtvt/utils/download_video.py` & `twtvt-2023.4.20/twtvt/utils/download_video.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 import logging
 import time
 from multiprocessing import cpu_count as get_cpu_count
-from typing import Iterable, Optional, Union
+from typing import Any, Iterable, Optional
 
 import yt_dlp
 from playwright.sync_api import sync_playwright
+from rich.progress import Progress
 from tenacity import after_log, before_sleep_log, retry, stop_after_attempt, wait_fixed
 
+from twtvt.utils.execute_parallel import execute_parallel
+
 from .logger import logger
 from .twitter_parser import TwitterParser
 from .uri_validator import URIValidator
 
 
 def download_video(
     target_uris: list[str],
     output: str = '.',
     until_link: Optional[str] = None,
     username: Optional[str] = None,
     password: Optional[str] = None,
     cookies_from_browser: Optional[str] = None,
     debug: bool = False,
+    parallel: bool = False,
 ):
     _validate_target_uris(target_uris=target_uris)
     video_links: tuple[str] = (
         *_extract_from_file_paths(target_uris=target_uris),
         *_extract_from_twitter_links(
             target_uris=target_uris,
             username=username,
             password=password,
             until_link=until_link,
             debug=debug,
         ),
     )
     _backup_links(links=video_links, output=output)
-    _download_videos(video_links=video_links, output=output, cookies_from_browser=cookies_from_browser)
+    if parallel:
+        _download_videos_parallel(video_links=video_links, output=output, cookies_from_browser=cookies_from_browser)
+    else:
+        _download_videos(video_links=video_links, output=output, cookies_from_browser=cookies_from_browser)
 
 
 def _validate_target_uris(target_uris: list[str]):
     for target_uri in target_uris:
         validators = [URIValidator.is_twitter_link, URIValidator.is_monsnode_link, URIValidator.is_file_path]
         if not any(validator(target_uri) for validator in validators):
             raise ValueError(f'Invalid target_uri: {target_uri}')
@@ -96,39 +103,68 @@
 
 def _backup_links(links: tuple[str], output: str):
     with open(f'{output}/links-{int(time.time())}-{len(links)}_videos.txt', 'w') as f:
         f.write('\n'.join(links))
 
 
 def _download_videos(video_links: tuple[str], output: str, cookies_from_browser: Optional[str]):
-    for index, video_link in enumerate(video_links):
-        logger.info(f'Downloading video from {video_link} ({index + 1}/{len(video_links)})')
-        try:
-            _download_video(video_link, output, cookies_from_browser)
-        except Exception as e:
-            logger.error(f'Failed to download video from {video_link}: {e}')
+    with Progress() as progress:
+        video_download_task = progress.add_task('Downloading Videos', total=len(video_links))
+        for index, video_link in enumerate(video_links):
+            progress.update(video_download_task, advance=1)
+            try:
+                _download_video(video_link, output, cookies_from_browser, (index, len(video_links)))
+            except Exception as e:
+                logger.error(f'Failed to download video from {video_link}: {e}')
+
+
+def _download_videos_parallel(video_links: tuple[str], output: str, cookies_from_browser: Optional[str]):
+    args = [(video_link, output, cookies_from_browser) for video_link in video_links]
+
+    with Progress() as progress:
+        video_download_task = progress.add_task('Downloading Videos', total=len(args))
+        for _ in execute_parallel(_download_video, args):
+            progress.update(video_download_task, advance=1)
+            progress.refresh()
 
 
 @retry(
     reraise=True,
     before_sleep=before_sleep_log(logger, logging.DEBUG),
     after=after_log(logger, logging.INFO),
     stop=stop_after_attempt(60),
     wait=wait_fixed(10),
 )
-def _download_video(video_link: str, output: str, cookies_from_browser: Optional[str]):
-    ydl_opts: dict[str, Union[str, bool, int, tuple[Optional[str]]]] = {
+def _download_video(
+    video_link: str,
+    output: str,
+    cookies_from_browser: Optional[str],
+    counters: Optional[tuple[int, int]] = None,
+):
+    nothing_logger = logging.getLogger('nothing')
+    nothing_logger.setLevel(logging.CRITICAL)
+    ydl_opts: dict[str, Any] = {
         'nocheckcertificate': True,
-        'concurrent_fragment_downloads': get_cpu_count(),
-        'outtmpl': f'{output}/%(title).200B.%(upload_date>%Y-%m-%d)s.%(id)s.%(ext)s'
+        'concurrent_fragment_downloads': get_cpu_count() + 1,
+        'outtmpl': f'{output}/%(title).200B.%(upload_date>%Y-%m-%d)s.%(id)s.%(ext)s',
+        'no_warnings': True,
+        'logger': nothing_logger,
     }
     if cookies_from_browser:
         ydl_opts['cookiesfrombrowser'] = (cookies_from_browser, )  # noqa
 
     try:
         with yt_dlp.YoutubeDL(ydl_opts) as ydl:
-            ydl.download([video_link])
+            result: dict[str, str] = ydl.extract_info(video_link, download=True)  # type: ignore
+            if counters:
+                logger.info(
+                    f"[{counters[0]+1}/{counters[1]}] Downloaded video [magenta]{result['title']}[/]",
+                    extra={'markup': True},
+                )
+            else:
+                logger.info(f"Downloaded video [magenta]{result['title']}[/]", extra={'markup': True})
+            return result
     except yt_dlp.utils.DownloadError as e:
         if '429' in str(e):  # Check if the error message contains "Too Many Requests"
             logger.info('Too many requests. Waiting for 5 minutes and retrying...')
             time.sleep(60 * 5)
             raise e  # Raise the exception to retry
```

### Comparing `twtvt-2023.4.17.post1/twtvt/utils/monsnode_parser.py` & `twtvt-2023.4.20/twtvt/utils/monsnode_parser.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.17.post1/twtvt/utils/twitter_parser.py` & `twtvt-2023.4.20/twtvt/utils/twitter_parser.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.17.post1/twtvt/utils/uri_validator.py` & `twtvt-2023.4.20/twtvt/utils/uri_validator.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.17.post1/PKG-INFO` & `twtvt-2023.4.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twtvt
-Version: 2023.4.17.post1
+Version: 2023.4.20
 Summary: 
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
```

