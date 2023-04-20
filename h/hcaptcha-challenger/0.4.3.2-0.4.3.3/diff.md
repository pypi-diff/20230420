# Comparing `tmp/hcaptcha-challenger-0.4.3.2.tar.gz` & `tmp/hcaptcha-challenger-0.4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcaptcha-challenger-0.4.3.2.tar", last modified: Mon Mar 20 13:48:45 2023, max compression
+gzip compressed data, was "hcaptcha-challenger-0.4.3.3.tar", last modified: Thu Apr 20 10:54:49 2023, max compression
```

## Comparing `hcaptcha-challenger-0.4.3.2.tar` & `hcaptcha-challenger-0.4.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 13:48:45.396074 hcaptcha-challenger-0.4.3.2/
--rw-rw-rw-   0        0        0    35823 2022-02-15 09:25:26.000000 hcaptcha-challenger-0.4.3.2/LICENSE
--rw-rw-rw-   0        0        0     2821 2023-03-20 13:48:45.395069 hcaptcha-challenger-0.4.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1799 2023-03-19 10:17:12.000000 hcaptcha-challenger-0.4.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 13:48:45.368961 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/
--rw-rw-rw-   0        0        0     2854 2023-03-20 13:46:36.000000 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-20 13:48:45.381072 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/_scaffold/
--rw-rw-rw-   0        0        0     6814 2023-03-20 13:45:45.000000 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/_scaffold/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-20 13:48:45.391072 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/_solutions/
--rw-rw-rw-   0        0        0      138 2022-10-23 21:40:20.000000 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/_solutions/__init__.py
--rw-rw-rw-   0        0        0    12036 2023-01-28 01:33:00.000000 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/_solutions/kernel.py
--rw-rw-rw-   0        0        0     4937 2022-10-23 21:40:20.000000 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/_solutions/resnet.py
--rw-rw-rw-   0        0        0     5844 2022-10-23 21:40:20.000000 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/_solutions/yolo.py
--rw-rw-rw-   0        0        0    30470 2023-02-02 10:03:47.000000 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/core.py
--rw-rw-rw-   0        0        0     1241 2022-10-23 21:40:20.000000 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-20 13:48:45.379075 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger.egg-info/
--rw-rw-rw-   0        0        0     2821 2023-03-20 13:48:45.000000 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      540 2023-03-20 13:48:45.000000 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 13:48:45.000000 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2023-03-20 13:48:45.000000 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-03-20 13:48:45.000000 hcaptcha-challenger-0.4.3.2/hcaptcha_challenger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-20 13:48:45.396074 hcaptcha-challenger-0.4.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1894 2023-03-20 13:48:08.000000 hcaptcha-challenger-0.4.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 10:54:49.401841 hcaptcha-challenger-0.4.3.3/
+-rw-rw-rw-   0        0        0    35823 2022-02-15 09:25:26.000000 hcaptcha-challenger-0.4.3.3/LICENSE
+-rw-rw-rw-   0        0        0     2821 2023-04-20 10:54:49.400839 hcaptcha-challenger-0.4.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1799 2023-03-19 10:17:12.000000 hcaptcha-challenger-0.4.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 10:54:49.376841 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/
+-rw-rw-rw-   0        0        0     2854 2023-04-20 10:53:15.000000 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 10:54:49.389844 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/_scaffold/
+-rw-rw-rw-   0        0        0     7291 2023-04-20 10:53:15.000000 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/_scaffold/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 10:54:49.397841 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/_solutions/
+-rw-rw-rw-   0        0        0      138 2022-10-23 21:40:20.000000 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/_solutions/__init__.py
+-rw-rw-rw-   0        0        0    12002 2023-04-20 10:53:15.000000 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/_solutions/kernel.py
+-rw-rw-rw-   0        0        0     5000 2023-04-20 10:53:15.000000 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/_solutions/resnet.py
+-rw-rw-rw-   0        0        0     5844 2022-10-23 21:40:20.000000 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/_solutions/yolo.py
+-rw-rw-rw-   0        0        0    30470 2023-04-20 10:27:00.000000 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/core.py
+-rw-rw-rw-   0        0        0     1241 2022-10-23 21:40:20.000000 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-20 10:54:49.387842 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger.egg-info/
+-rw-rw-rw-   0        0        0     2821 2023-04-20 10:54:49.000000 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-04-20 10:54:49.000000 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 10:54:49.000000 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2023-04-20 10:54:49.000000 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-20 10:54:49.000000 hcaptcha-challenger-0.4.3.3/hcaptcha_challenger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 10:54:49.402850 hcaptcha-challenger-0.4.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1894 2023-03-20 13:48:08.000000 hcaptcha-challenger-0.4.3.3/setup.py
```

### Comparing `hcaptcha-challenger-0.4.3.2/LICENSE` & `hcaptcha-challenger-0.4.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hcaptcha-challenger-0.4.3.2/PKG-INFO` & `hcaptcha-challenger-0.4.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcaptcha-challenger
-Version: 0.4.3.2
+Version: 0.4.3.3
 Summary: 🥂 Gracefully face hCaptcha challenge with YOLOv6(ONNX) embedded solution.
 Home-page: https://github.com/QIN2DIM/hcaptcha-challenger
 Author: QIN2DIM
 Author-email: qinse.top@foxmail.com
 Maintainer: QIN2DIM, Bingjie Yan
 Maintainer-email: qinse.top@foxmail.com, bj.yan.pa@qq.com
 License: GNU General Public License v3.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hcaptcha-challenger Version: 0.4.3.2 Summary: ð¥
+Metadata-Version: 2.1 Name: hcaptcha-challenger Version: 0.4.3.3 Summary: ð¥
 Gracefully face hCaptcha challenge with YOLOv6(ONNX) embedded solution. Home-
 page: https://github.com/QIN2DIM/hcaptcha-challenger Author: QIN2DIM Author-
 email: qinse.top@foxmail.com Maintainer: QIN2DIM, Bingjie Yan Maintainer-email:
 qinse.top@foxmail.com, bj.yan.pa@qq.com License: GNU General Public License
 v3.0 Keywords: hcaptcha,hcaptcha-challenger,hcaptcha-challenger-
 python,hcaptcha-solver Classifier: Topic :: Scientific/Engineering Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
```

### Comparing `hcaptcha-challenger-0.4.3.2/README.md` & `hcaptcha-challenger-0.4.3.3/README.md`

 * *Files identical despite different names*

### Comparing `hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/__init__.py` & `hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 # Description:
 import os
 import shutil
 import time
 import typing
 from urllib.parse import urlparse
 
-from ._scaffold import init_log, Config, get_challenge_ctx
+from ._scaffold import Config, get_challenge_ctx, init_log
 from ._solutions.kernel import ModelHub
 from ._solutions.kernel import PluggableObjects
-from ._solutions.yolo import YOLO, Prefix
+from ._solutions.yolo import Prefix, YOLO
 from .core import HolyChallenger
 
 __all__ = ["HolyChallenger", "new_challenger", "get_challenge_ctx"]
-__version__ = "0.4.3.2"
+__version__ = "0.4.3.3"
 
 logger = init_log(
     error=os.path.join("datas", "logs", "error.log"),
     runtime=os.path.join("datas", "logs", "runtime.log"),
 )
```

### Comparing `hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/_scaffold/__init__.py` & `hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/_scaffold/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 import logging
 import os
 import sys
 import typing
 import warnings
 
-import undetected_chromedriver as uc
 from loguru import logger
 from selenium.common.exceptions import WebDriverException
+from undetected_chromedriver import Chrome, ChromeOptions
 from webdriver_manager.chrome import ChromeDriverManager, ChromeType
 from webdriver_manager.core.utils import get_browser_version_from_os
 
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 
 
 def init_log(**sink_path):
@@ -128,54 +128,69 @@
 ):
     """
     Challenger drive for handling human-machine challenges.
 
     :param silence: Control headless browser
     :param lang: Restrict the language of hCAPTCHA label.
       See https://github.com/QIN2DIM/hcaptcha-challenger/issues/13
-    :rtype: uc.Chrome
+    :rtype: undetected_chromedriver.Chrome
     """
     # Control headless browser
     # If on Linux, and no X server is available (`DISPLAY` not set), assume
     # headless operation
     silence = (
         True
         if silence is None or ("linux" in sys.platform and "DISPLAY" not in os.environ)
         else silence
     )
 
-    # - Restrict browser startup parameters
-    options = uc.ChromeOptions()
-    options.add_argument("--log-level=3")
-    options.add_argument("--disable-dev-shm-usage")
-
-    # - Restrict the language of hCaptcha label
-    # - Environment variables are valid only in the current process
-    # and do not affect other processes in the operating system
-    os.environ["LANGUAGE"] = "en_US" if lang is None else lang
-    options.add_argument(f"--lang={os.getenv('LANGUAGE')}")
-
-    if silence is True:
-        options.add_argument("--disable-gpu")
-        options.add_argument("--disable-software-rasterizer")
-
     # - Use chromedriver cache to improve application startup speed
     # - Requirement: undetected-chromedriver >= 3.1.5.post2
     logging.getLogger("WDM").setLevel(logging.NOTSET)
     driver_executable_path = ChromeDriverManager().install()
     version_main = get_browser_version_from_os(ChromeType.GOOGLE).split(".")[0]
 
     logger.debug("🎮 Activate challenger context")
     try:
-        return uc.Chrome(
-            options=options,
+        return Chrome(
+            options=createChromeOptions(silence, lang),
             headless=silence,
             driver_executable_path=driver_executable_path,
             **kwargs,
         )
     except WebDriverException:
-        return uc.Chrome(
-            options=options,
+        return Chrome(
+            options=createChromeOptions(silence, lang),
             headless=silence,
             version_main=int(version_main) if version_main.isdigit() else None,
             **kwargs,
         )
+
+
+def createChromeOptions(
+    silence: typing.Optional[bool] = None, lang: typing.Optional[str] = None
+) -> ChromeOptions:
+    """
+    Create ChromeOptions for undetected_chromedriver.Chrome
+
+    :param silence: Control headless browser
+    :param lang: Restrict the language of hCAPTCHA label.
+
+    :rtype: undetected_chromedriver.ChromeOptions
+    """
+
+    # - Restrict browser startup parameters
+    options = ChromeOptions()
+    options.add_argument("--log-level=3")
+    options.add_argument("--disable-dev-shm-usage")
+
+    # - Restrict the language of hCaptcha label
+    # - Environment variables are valid only in the current process
+    # and do not affect other processes in the operating system
+    os.environ["LANGUAGE"] = "en_US" if lang is None else lang
+    options.add_argument(f"--lang={os.getenv('LANGUAGE')}")
+
+    if silence is True:
+        options.add_argument("--disable-gpu")
+        options.add_argument("--disable-software-rasterizer")
+
+    return options
```

### Comparing `hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/_solutions/kernel.py` & `hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/_solutions/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 @dataclass
 class GitHubUpStream:
     username: str
     GITHUB_RELEASE_API = ""
     URL_REMOTE_OBJECTS = ""
 
     def __post_init__(self):
-        self.GITHUB_RELEASE_API = f"https://api.github.com/repos/{self.username}/hcaptcha-challenger/releases"
+        self.GITHUB_RELEASE_API = (
+            f"https://api.github.com/repos/{self.username}/hcaptcha-challenger/releases"
+        )
         self.URL_REMOTE_OBJECTS = f"https://raw.githubusercontent.com/{self.username}/hcaptcha-challenger/main/src/objects.yaml"
 
 
 _hook = GitHubUpStream(username="QIN2DIM")
 
 
 class Memory:
@@ -133,51 +135,52 @@
                     logger.warning(err)
 
     def _offload(self):
         """仅在 Assets._pull 网络请求发起后实现，用于更新本地缓存的内容及时间戳"""
         os.makedirs(self._dir_assets, exist_ok=True)
         for asset_fn in os.listdir(self._dir_assets):
             asset_src = join(self._dir_assets, asset_fn)
-            asset_dst = join(self._dir_assets, f"_{asset_fn}")
+            asset_dst = join(self._dir_assets, f"_{asset_fn.replace('_', '')}")
             shutil.move(asset_src, asset_dst)
         recoded_name = join(self._dir_assets, str(int(time.time())))
         with open(recoded_name, "w", encoding="utf8") as file:
             json.dump(self._fn2assets, file)
 
     def _pull(self, skip_preload: bool = False) -> typing.Optional[typing.Dict[str, dict]]:
-        def request_assets():
-            logger.debug(f"Pulling AssetsObject from {self.GITHUB_RELEASE_API}")
-
-            try:
-                session = requests.session()
-                resp = session.get(self.GITHUB_RELEASE_API, proxies=getproxies(), timeout=3)
-                data = resp.json()[0]
-            except (requests.exceptions.ConnectionError, json.decoder.JSONDecodeError) as err:
-                logger.error(err)
-            except (AttributeError, IndexError, KeyError) as err:
-                logger.error(err)
-            else:
-                if isinstance(data, dict):
-                    assets: typing.List[dict] = data.get(self.NAME_ASSETS, [])
-                    for asset in assets:
-                        self._fn2assets[asset[self.NAME_ASSET_NAME]] = asset
-            finally:
-                self._offload()
-
         if not skip_preload:
             self._preload()
         if not self._fn2assets:
-            request_assets()
+            self._request_assets()
         return self._fn2assets
 
+    def _request_assets(self):
+        logger.debug(f"Pulling AssetsObject from {self.GITHUB_RELEASE_API}")
+
+        try:
+            session = requests.session()
+            resp = session.get(self.GITHUB_RELEASE_API, proxies=getproxies(), timeout=3)
+            data = resp.json()[0]
+        except (requests.exceptions.ConnectionError, json.decoder.JSONDecodeError) as err:
+            logger.error(err)
+        except (AttributeError, IndexError, KeyError) as err:
+            logger.error(err)
+        else:
+            if isinstance(data, dict):
+                assets: typing.List[dict] = data.get(self.NAME_ASSETS, [])
+                for asset in assets:
+                    self._fn2assets[asset[self.NAME_ASSET_NAME]] = asset
+        finally:
+            self._offload()
+
     def _get_asset(self, key: str, oncall_default: typing.Any):
         return self._fn2assets.get(self.fn, {}).get(key, oncall_default)
 
-    def sync(self, force: typing.Optional[bool] = None, **kwargs):
-        raise NotImplementedError
+    def sync(self):
+        self._fn2assets = {}
+        self._request_assets()
 
     @property
     def dir_assets(self):
         return self._dir_assets
 
     def get_node_id(self) -> typing.Optional[str]:
         return self._get_asset(self.NAME_ASSET_NODE_ID, "")
```

### Comparing `hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/_solutions/resnet.py` & `hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/_solutions/resnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 import typing
 import warnings
 
 import cv2
 import numpy as np
 import yaml
+from loguru import logger
 
 from .kernel import ChallengeStyle
 from .kernel import ModelHub
 
 warnings.filterwarnings("ignore", category=UserWarning)
 
 
@@ -47,15 +48,17 @@
         net = self.match_net()
         if net is None:
             _err_prompt = f"""
             The remote network does not exist or the local cache has expired.
             1. Check objects.yaml for typos | model={self.fn};
             2. Restart the program after deleting the local cache | dir={self.assets.dir_assets};
             """
-            raise ResourceWarning(_err_prompt)  # maybe mercy
+            logger.warning(_err_prompt)
+            self.assets.sync()
+            return False
         net.setInput(blob)
         out = net.forward()
         if not np.argmax(out, axis=1)[0]:
             return True
         return False
 
     def solution(self, img_stream, **kwargs) -> bool:
```

### Comparing `hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/_solutions/yolo.py` & `hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/_solutions/yolo.py`

 * *Files identical despite different names*

### Comparing `hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/core.py` & `hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/core.py`

 * *Files identical despite different names*

### Comparing `hcaptcha-challenger-0.4.3.2/hcaptcha_challenger/exceptions.py` & `hcaptcha-challenger-0.4.3.3/hcaptcha_challenger/exceptions.py`

 * *Files identical despite different names*

### Comparing `hcaptcha-challenger-0.4.3.2/hcaptcha_challenger.egg-info/PKG-INFO` & `hcaptcha-challenger-0.4.3.3/hcaptcha_challenger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcaptcha-challenger
-Version: 0.4.3.2
+Version: 0.4.3.3
 Summary: 🥂 Gracefully face hCaptcha challenge with YOLOv6(ONNX) embedded solution.
 Home-page: https://github.com/QIN2DIM/hcaptcha-challenger
 Author: QIN2DIM
 Author-email: qinse.top@foxmail.com
 Maintainer: QIN2DIM, Bingjie Yan
 Maintainer-email: qinse.top@foxmail.com, bj.yan.pa@qq.com
 License: GNU General Public License v3.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hcaptcha-challenger Version: 0.4.3.2 Summary: ð¥
+Metadata-Version: 2.1 Name: hcaptcha-challenger Version: 0.4.3.3 Summary: ð¥
 Gracefully face hCaptcha challenge with YOLOv6(ONNX) embedded solution. Home-
 page: https://github.com/QIN2DIM/hcaptcha-challenger Author: QIN2DIM Author-
 email: qinse.top@foxmail.com Maintainer: QIN2DIM, Bingjie Yan Maintainer-email:
 qinse.top@foxmail.com, bj.yan.pa@qq.com License: GNU General Public License
 v3.0 Keywords: hcaptcha,hcaptcha-challenger,hcaptcha-challenger-
 python,hcaptcha-solver Classifier: Topic :: Scientific/Engineering Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
```

### Comparing `hcaptcha-challenger-0.4.3.2/hcaptcha_challenger.egg-info/SOURCES.txt` & `hcaptcha-challenger-0.4.3.3/hcaptcha_challenger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcaptcha-challenger-0.4.3.2/setup.py` & `hcaptcha-challenger-0.4.3.3/setup.py`

 * *Files identical despite different names*

