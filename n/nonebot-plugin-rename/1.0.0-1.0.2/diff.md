# Comparing `tmp/nonebot_plugin_rename-1.0.0.tar.gz` & `tmp/nonebot_plugin_rename-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rename-1.0.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_rename-1.0.2.tar", max compression
```

## Comparing `nonebot_plugin_rename-1.0.0.tar` & `nonebot_plugin_rename-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1066 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/LICENSE
--rw-r--r--   0        0        0     4710 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/README.md
--rw-r--r--   0        0        0      361 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/__init__.py
--rw-r--r--   0        0        0      244 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/card/__init__.py
--rw-r--r--   0        0        0      789 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/card/gaokao_time.py
--rw-r--r--   0        0        0      885 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/card/genshin_time.py
--rw-r--r--   0        0        0      676 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/card/get_times.py
--rw-r--r--   0        0        0      894 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/card/hot_search.py
--rw-r--r--   0        0        0      408 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/card/message.py
--rw-r--r--   0        0        0      435 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/card/one_word.py
--rw-r--r--   0        0        0      603 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/card/status.py
--rw-r--r--   0        0        0      252 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/config.py
--rw-r--r--   0        0        0     7139 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/main.py
--rw-r--r--   0        0        0      154 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/utils/__init__.py
--rw-r--r--   0        0        0      465 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/utils/card_choice.py
--rw-r--r--   0        0        0      906 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/utils/card_name.py
--rw-r--r--   0        0        0     1465 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/utils/draw.py
--rw-r--r--   0        0        0      423 2023-04-19 03:25:20.618178 nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/utils/my_yaml.py
--rw-r--r--   0        0        0      644 2023-04-19 03:25:20.622178 nonebot_plugin_rename-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5575 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4789 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/README.md
+-rw-r--r--   0        0        0      363 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/card/__init__.py
+-rw-r--r--   0        0        0      789 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/card/gaokao_time.py
+-rw-r--r--   0        0        0      885 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/card/genshin_time.py
+-rw-r--r--   0        0        0      689 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/card/get_times.py
+-rw-r--r--   0        0        0      925 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/card/hot_search.py
+-rw-r--r--   0        0        0      408 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/card/message.py
+-rw-r--r--   0        0        0      466 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/card/one_word.py
+-rw-r--r--   0        0        0      603 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/card/status.py
+-rw-r--r--   0        0        0      252 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/config.py
+-rw-r--r--   0        0        0     7117 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/main.py
+-rw-r--r--   0        0        0      151 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/utils/__init__.py
+-rw-r--r--   0        0        0      478 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/utils/card_choice.py
+-rw-r--r--   0        0        0      867 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/utils/card_name.py
+-rw-r--r--   0        0        0     1407 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/utils/draw.py
+-rw-r--r--   0        0        0      423 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/utils/my_yaml.py
+-rw-r--r--   0        0        0      644 2023-04-20 17:41:09.768737 nonebot_plugin_rename-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5654 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_rename-1.0.0/LICENSE` & `nonebot_plugin_rename-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.0.0/README.md` & `nonebot_plugin_rename-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 <div align="center">
 
 # nonebot-plugin-rename
 
 _✨ 通过定时任务更改bot所在群自己的群名片,内置了几种常见的群名片并且初步支持了多bot,欢迎**pr**新的群名片! ✨_
 
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/forchannot/nonebot-plugin-rename.svg" alt="license">
+<a href="https://raw.githubusercontent.com/nonebot/nonebot2/master/LICENSE">
+    <img src="https://img.shields.io/github/license/forchannot/nonebot_plugin_rename" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-rename">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-rename.svg" alt="pypi">
 </a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<img src="https://img.shields.io/badge/python-3.8+-yellow.svg" alt="python">
 
 </div>
 
 <!-- TOC -->
 * [nonebot-plugin-rename](#nonebot-plugin-rename)
   * [📖简介](#简介)
   * [🔐许可](#许可)
@@ -137,14 +137,16 @@
 
 **PS:由于本人代码比较烂,很多方法实现都比较复杂,所以对pr不是很友好,如果有更好的方法欢迎pr并指正**
 
 **群名片的生成代码**在/card/文件夹内,每种群名片(或者每类)对应一个文件
 
 当新增一个新的群名片样式时,需要在**以下几个地方**进行修改相应代码使得其生效
 
-* `/utils/card_name.py`内的`name_of_card`和`card_name_list`两个变量按照格式新增你的文件名和对应的描述
+* 在`/card/__init__.py`内导入你的包
+* 在`/utils/card_name.py`内的`card_list`按照格式新增你的文件名和对应的描述以及导包
+
 
 ## 🔥鸣谢
 
 [**自动化插件**的群名片修改js版](https://github.com/Nwflower/auto-plugin/tree/master/model/autoGroupName)
 
 [**小派蒙**的获取系统信息](https://github.com/CMHopeSunshine/LittlePaimon/blob/Bot/LittlePaimon/utils/status.py)
```

#### html2text {}

```diff
@@ -49,13 +49,13 @@
 -- ç³»ç»åå­åcpuä¿¡æ¯
 -- Botæ¶åæ¶æ¯æ±æ»
  ## ð§PRéç¥ **PS:
 ç±äºæ¬äººä»£ç æ¯è¾ç,å¾å¤æ¹æ³å®ç°é½æ¯è¾å¤æ,æä»¥å¯¹prä¸æ¯å¾åå¥½,å¦æææ´å¥½çæ¹æ³æ¬¢è¿prå¹¶ææ­£**
 **ç¾¤åçççæä»£ç **å¨/card/æä»¶å¤¹å,æ¯ç§ç¾¤åç
 (æèæ¯ç±»)å¯¹åºä¸ä¸ªæä»¶
 å½æ°å¢ä¸ä¸ªæ°çç¾¤åçæ ·å¼æ¶,éè¦å¨**ä»¥ä¸å ä¸ªå°æ¹**è¿è¡ä¿®æ¹ç¸åºä»£ç ä½¿å¾å¶çæ
-* `/utils/
-card_name.py`åç`name_of_card`å`card_name_list`ä¸¤ä¸ªåéæç§æ ¼å¼æ°å¢ä½ çæä»¶ååå¯¹åºçæè¿°
+* å¨`/card/__init__.py`åå¯¼å¥ä½ çå * å¨`/utils/
+card_name.py`åç`card_list`æç§æ ¼å¼æ°å¢ä½ çæä»¶ååå¯¹åºçæè¿°ä»¥åå¯¼å
 ## ð¥é¸£è°¢ [**èªå¨åæä»¶**çç¾¤åçä¿®æ¹jsç](https://github.com/
 Nwflower/auto-plugin/tree/master/model/autoGroupName)
 [**å°æ´¾è**çè·åç³»ç»ä¿¡æ¯](https://github.com/CMHopeSunshine/
 LittlePaimon/blob/Bot/LittlePaimon/utils/status.py)
```

### Comparing `nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/card/gaokao_time.py` & `nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/card/gaokao_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/card/genshin_time.py` & `nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/card/genshin_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/card/get_times.py` & `nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/card/get_times.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     BigHourType = ["正", "初"]
     # BigMinName = ["零", "一", "二", "三", "四"]
     hour = now.hour
     # minutes = now.minute
     return f"现在是长安{BigHourName[(hour + 1) // 2]}{BigHourType[hour % 2]}"
 
 
-def now_time():
+def now_time() -> str:
     now = datetime.datetime.now()
     hour = now.hour
-    minutes = now.minute
+    # minutes = now.minute
     if hour < 10:
         hour = f"0{hour}"
-    if minutes < 10:
-        minutes = f"0{minutes}"
+    # if minutes < 10:
+    #     minutes = f"0{minutes}"
     return f"现在是北京时间{hour}点"
```

### Comparing `nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/card/hot_search.py` & `nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/card/hot_search.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Description: 获取热搜
 
 import random
 import httpx
 
 from nonebot import logger
+from typing import Optional
 
 URL = {
     "1": "https://tenapi.cn/v2/bilihot/",  # B站
     "2": "https://tenapi.cn/v2/weibohot",  # 微博
     "3": "https://tenapi.cn/v2/douyinhot",  # 抖音
     "4": "https://tenapi.cn/v2/baiduhot/",  # 百度
     "5": "https://tenapi.cn/v2/zhihuhot",  # 知乎
     "6": "https://tenapi.cn/v2/toutiaohot",  # 今日头条
 }
 
 
-async def hot(num: int) -> str | None:
+async def hot(num: int) -> Optional[str]:
     async with httpx.AsyncClient(follow_redirects=True) as client:
         try:
             res = await client.get(URL[str(num)])
             if res.status_code != 200:
                 return "热搜api失效"
             data = res.json()["data"]
             result = random.choice(data)["name"]
```

### Comparing `nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/card/status.py` & `nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/card/status.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/main.py` & `nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,63 +12,63 @@
     ActionFailed,
 )
 from nonebot.drivers import Driver
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 
 from .config import Config
-from .utils import *
+from .utils import choice_card, generate_card_image, card_list, read_yaml, write_yaml
 
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 
 driver: Driver = get_driver()
 env_config = Config.parse_obj(get_driver().config.dict())
 hour, minute = env_config.set_group_card_hour, env_config.set_group_card_minute
 if driver.config.nickname:
     NICKNAME = env_config.self_name if env_config.self_name else list(driver.config.nickname)[0]
 else:
     NICKNAME = env_config.self_name if env_config.self_name else "bot"
 yml_file = Path.cwd() / "data" / "group_card"
-
+permissions = SUPERUSER | GROUP_ADMIN | GROUP_OWNER
 
 group_card = on_command(
     "设置群名片",
     aliases={"更改群名片", "修改群名片"},
-    permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
+    permission=permissions,
     priority=13,
-    block=False,
+    block=True,
 )
 view_pic = on_command(
     "查看群名片列表",
     aliases={"查看所有群名片", "群名片列表"},
-    permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
+    permission=permissions,
     priority=14,
-    block=False,
+    block=True,
 )
 view_card = on_command(
     "查看当前群名片",
     aliases={"当前群名片"},
-    permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
+    permission=permissions,
     priority=14,
-    block=False,
+    block=True,
 )
 set_card_now = on_command(
     "立即更改群名片",
     aliases={"立即设置群名片", "立即修改群名片"},
-    permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
+    permission=permissions,
     priority=10,
-    block=False,
+    block=True,
 )
 del_group_card = on_command(
     "删除群名片",
     aliases={"删除本群群名片"},
-    permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
+    permission=permissions,
     priority=10,
-    block=False,
+    block=True,
 )
 
 
 # on_command "设置群名片"
 @group_card.handle()
 async def get_group_card(bot: Bot, event: GroupMessageEvent):
     # 解析参数
@@ -77,15 +77,15 @@
     if not group_nicknames:
         await group_card.finish("请输入你想要设置的群名片序号")
     group_id = str(event.group_id)
     bot_id = bot.self_id
     # 读取群名片数据
     group_data = read_yaml(yml_file / "group_card.yaml") or {}
     group_nicknames_valid = not any(
-        int(gn) > len(name_of_card) for gn in group_nicknames
+        int(gn) > len(card_list) for gn in group_nicknames
     )  # 判断用户输入的群名片序号是否有效
     # 更新群名片数据
     if group_nicknames_valid:
         group_data.setdefault(bot_id, {})
         group_data[bot_id].setdefault(group_id, {})
         group_data[bot_id][group_id] = group_nicknames
         write_yaml(yml_file / "group_card.yaml", group_data)
```

### Comparing `nonebot_plugin_rename-1.0.0/nonebot_plugin_rename/utils/draw.py` & `nonebot_plugin_rename-1.0.2/nonebot_plugin_rename/utils/draw.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import base64
 from io import BytesIO
 
 from PIL import Image, ImageDraw, ImageFont
-from .card_name import card_name_list as card_list
+
+from .card_name import card_list
 
 
 def generate_card_image(
     font_path: str = "simhei.ttf",
     font_size: int = 20,
     title_left: str = "群名片序号",
     title_right: str = "群名片描述",
@@ -19,18 +19,17 @@
     draw = ImageDraw.Draw(img)
     # 绘制标题和分割线
     draw.text((50, 10), title_left, font=font, fill="black")
     draw.line((200, 0, 200, len(card_list) * 50 + 50), fill="black")
     draw.text((220, 10), title_right, font=font, fill="black")
     draw.line((0, 50, 800, 50), fill="black")
     # 遍历列表，获取内容并绘制到图片上
-    for i, content in enumerate(card_list):
-        if content[0] and content[1]:
-            draw.text((95, i * 50 + 65), content[0], font=font, fill="black")
+    for i in range(len(card_list)):
+        if card_list[str(i + 1)][0]:
+            draw.text((95, i * 50 + 65), str(i+1), font=font, fill="black")
             draw.line((200, i * 50 + 50, 200, (i + 1) * 50 + 50), fill="black")
-            draw.text((220, i * 50 + 65), content[1], font=font, fill="black")
-            # 绘制分割线
+            draw.text((220, i * 50 + 65), card_list[str(i + 1)][0], font=font, fill="black")
             draw.line((0, (i + 1) * 50 + 50, 800, (i + 1) * 50 + 50), fill="black")
     # 返回base64编码后的图片字符串
     img_buffer = BytesIO()
     img.save(img_buffer, format="PNG")
     return img_buffer.getvalue()
```

### Comparing `nonebot_plugin_rename-1.0.0/pyproject.toml` & `nonebot_plugin_rename-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-rename"
-version = "1.0.0"
+version = "1.0.2"
 description = "更改qq机器人的群名片，内置多种有趣名片"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_rename"}]
 
 [[tool.poetry.source]]
```

### Comparing `nonebot_plugin_rename-1.0.0/PKG-INFO` & `nonebot_plugin_rename-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rename
-Version: 1.0.0
+Version: 1.0.2
 Summary: 更改qq机器人的群名片，内置多种有趣名片
 License: GPL-3.0
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -28,21 +28,21 @@
 
 <div align="center">
 
 # nonebot-plugin-rename
 
 _✨ 通过定时任务更改bot所在群自己的群名片,内置了几种常见的群名片并且初步支持了多bot,欢迎**pr**新的群名片! ✨_
 
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/forchannot/nonebot-plugin-rename.svg" alt="license">
+<a href="https://raw.githubusercontent.com/nonebot/nonebot2/master/LICENSE">
+    <img src="https://img.shields.io/github/license/forchannot/nonebot_plugin_rename" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-rename">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-rename.svg" alt="pypi">
 </a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<img src="https://img.shields.io/badge/python-3.8+-yellow.svg" alt="python">
 
 </div>
 
 <!-- TOC -->
 * [nonebot-plugin-rename](#nonebot-plugin-rename)
   * [📖简介](#简介)
   * [🔐许可](#许可)
@@ -159,15 +159,17 @@
 
 **PS:由于本人代码比较烂,很多方法实现都比较复杂,所以对pr不是很友好,如果有更好的方法欢迎pr并指正**
 
 **群名片的生成代码**在/card/文件夹内,每种群名片(或者每类)对应一个文件
 
 当新增一个新的群名片样式时,需要在**以下几个地方**进行修改相应代码使得其生效
 
-* `/utils/card_name.py`内的`name_of_card`和`card_name_list`两个变量按照格式新增你的文件名和对应的描述
+* 在`/card/__init__.py`内导入你的包
+* 在`/utils/card_name.py`内的`card_list`按照格式新增你的文件名和对应的描述以及导包
+
 
 ## 🔥鸣谢
 
 [**自动化插件**的群名片修改js版](https://github.com/Nwflower/auto-plugin/tree/master/model/autoGroupName)
 
 [**小派蒙**的获取系统信息](https://github.com/CMHopeSunshine/LittlePaimon/blob/Bot/LittlePaimon/utils/status.py)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.0.2 Summary:
 æ´æ¹qqæºå¨äººçç¾¤åçï¼åç½®å¤ç§æè¶£åç License: GPL-3.0
 Author: forchannot Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: httpx (>=0.24.0,<0.25.0) Requires-
@@ -61,13 +61,13 @@
 -- ç³»ç»åå­åcpuä¿¡æ¯
 -- Botæ¶åæ¶æ¯æ±æ»
  ## ð§PRéç¥ **PS:
 ç±äºæ¬äººä»£ç æ¯è¾ç,å¾å¤æ¹æ³å®ç°é½æ¯è¾å¤æ,æä»¥å¯¹prä¸æ¯å¾åå¥½,å¦æææ´å¥½çæ¹æ³æ¬¢è¿prå¹¶ææ­£**
 **ç¾¤åçççæä»£ç **å¨/card/æä»¶å¤¹å,æ¯ç§ç¾¤åç
 (æèæ¯ç±»)å¯¹åºä¸ä¸ªæä»¶
 å½æ°å¢ä¸ä¸ªæ°çç¾¤åçæ ·å¼æ¶,éè¦å¨**ä»¥ä¸å ä¸ªå°æ¹**è¿è¡ä¿®æ¹ç¸åºä»£ç ä½¿å¾å¶çæ
-* `/utils/
-card_name.py`åç`name_of_card`å`card_name_list`ä¸¤ä¸ªåéæç§æ ¼å¼æ°å¢ä½ çæä»¶ååå¯¹åºçæè¿°
+* å¨`/card/__init__.py`åå¯¼å¥ä½ çå * å¨`/utils/
+card_name.py`åç`card_list`æç§æ ¼å¼æ°å¢ä½ çæä»¶ååå¯¹åºçæè¿°ä»¥åå¯¼å
 ## ð¥é¸£è°¢ [**èªå¨åæä»¶**çç¾¤åçä¿®æ¹jsç](https://github.com/
 Nwflower/auto-plugin/tree/master/model/autoGroupName)
 [**å°æ´¾è**çè·åç³»ç»ä¿¡æ¯](https://github.com/CMHopeSunshine/
 LittlePaimon/blob/Bot/LittlePaimon/utils/status.py)
```

