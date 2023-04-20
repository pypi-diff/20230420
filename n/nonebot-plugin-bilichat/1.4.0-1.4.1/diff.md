# Comparing `tmp/nonebot_plugin_bilichat-1.4.0.tar.gz` & `tmp/nonebot_plugin_bilichat-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-1.4.0.tar", last modified: Sat Apr 15 16:01:07 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-1.4.1.tar", last modified: Thu Apr 20 03:15:16 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-1.4.0.tar` & `nonebot_plugin_bilichat-1.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    34523 2023-04-15 16:00:57.754367 nonebot_plugin_bilichat-1.4.0/LICENSE
--rw-r--r--   0        0        0     8253 2023-04-15 16:00:57.754367 nonebot_plugin_bilichat-1.4.0/README.md
--rw-r--r--   0        0        0     7148 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4576 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4592 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      927 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     4534 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0     2854 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0      893 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0       93 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      148 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1045 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5573 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4388 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2342 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-04-15 16:00:57.762367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1764 2023-04-15 16:00:57.766367 nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1344 2023-04-15 16:01:07.538455 nonebot_plugin_bilichat-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     9542 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-20 03:15:06.033037 nonebot_plugin_bilichat-1.4.1/LICENSE
+-rw-r--r--   0        0        0    10989 2023-04-20 03:15:06.033037 nonebot_plugin_bilichat-1.4.1/README.md
+-rw-r--r--   0        0        0     7289 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4611 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4592 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      927 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     4657 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0     2854 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0      893 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0       93 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      148 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-04-20 03:15:06.045037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1045 2023-04-20 03:15:06.045037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5573 2023-04-20 03:15:06.045037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4388 2023-04-20 03:15:06.045037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2342 2023-04-20 03:15:06.045037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-04-20 03:15:06.045037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1764 2023-04-20 03:15:06.045037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1407 2023-04-20 03:15:16.561197 nonebot_plugin_bilichat-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    12278 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.4.1/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-1.4.0/LICENSE` & `nonebot_plugin_bilichat-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/README.md` & `nonebot_plugin_bilichat-1.4.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -28,14 +28,28 @@
     <img src="https://img.shields.io/badge/pdm-managed-blueviolet" alt="pdm-managed">
 </a>
 
 <a href="https://github.com/psf/black">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black">
 </a>
 
+<a href="https://onebot.dev/">
+  <img src="https://img.shields.io/badge/OneBot-v11-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">
+</a>
+<a href="https://onebot.dev/">
+  <img src="https://img.shields.io/badge/OneBot-v12-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">
+</a>
+
+<a href="https://jq.qq.com/?_wv=1027&k=5OFifDh">
+  <img src="https://img.shields.io/badge/QQ%E7%BE%A4-768887710-orange?style=flat-square" alt="QQ Chat Group">
+</a>
+<a href="https://jq.qq.com/?_wv=1027&k=7LWx6q4J">
+  <img src="https://img.shields.io/badge/QQ%E7%BE%A4-720053992-orange?style=flat-square" alt="QQ Chat Group">
+</a>
+
 </div>
 
 ## 📖 介绍
 
 视频链接解析，并根据其内容生成**基本信息**、**词云**和**内容总结**
 
 <details>
@@ -121,23 +135,31 @@
 
 ### 通用配置项
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | bilichat_block              | bool      | False | 是否拦截事件(防止其他插件二次解析) |
 | bilichat_enable_private     | bool      | True  | 是否允许响应私聊 |
-| bilichat_enable_v12_channel | bool      | True  | 是否允许响应频道消息(ob12专属) |
+| bilichat_enable_self        | bool      | False | 是否允许响应自身的消息 |
+| bilichat_enable_v12_channel | bool      | True  | ~~是否允许响应频道消息(ob12专属)~~(暂未实现) |
 | bilichat_enable_unkown_src  | bool      | False | 是否允许响应未知来源的消息 |
 | bilichat_whitelist          | list[str] | []    | **响应**的群聊(频道)名单, 会覆盖黑名单 |
 | bilichat_blacklist          | list[str] | []    | **不响应**的群聊(频道)名单 |
 | bilichat_dynamic_font       | str       | None  | 视频信息及词云图片使用的字体 |
 | bilichat_cd_time            | int       | 120   | 对同一视频的响应冷却时间(防止刷屏) |
 | bilichat_neterror_retry     | int       | 3     | 对部分网络请求错误的尝试次数 |
 | bilichat_use_bcut_asr       | bool      | True  | 是否在**没有字幕时**调用必剪接口生成字幕 |
 
+注:
+
+1. 由于 OneBot 协议未规定是否应上报自身事件，因此在不同的场景下能否获取自身事件并不一定，`bilichat_enable_self` 实际能否生效也与之相关
+2. 当 `bilichat_whitelist` 存在时，`bilichat_blacklist` 将会被禁用
+3. `bilichat_dynamic_font` 可填写自定义的字体url，但并不推荐修改
+4. 当使用 `bcut_asr` 接口来生成AI字幕时，根据视频时长和网络情况有可能会识别失败，Bot会提示 `BCut-ASR conversion failed due to network error`。可以通过调高 `bilichat_neterror_retry` 次数或几分钟后重试来尝试重新生成字幕
+
 ### 基础信息配置项
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | bilichat_basic_info          | bool | True | 是否开启视频基本信息 |
 | bilichat_reply_to_basic_info | bool | True | 后续消息是否回复基础信息(关闭则回复发送者的信息) |
 
@@ -145,14 +167,16 @@
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[wordcloud]`
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | bilichat_word_cloud  | bool | True | 是否开启词云功能 |
 
+注：词云功能在 python3.11 中由于 `wordcloud` 包安装失败暂时无法启用，请不要在 3.11 中开启此功能
+
 ### AI视频总结配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[openai,newbing]`
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | bilichat_newbing_cookie      | str       | None               | newbing的cookie文件路径(获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) , 若留空则禁用newbing总结 |
@@ -161,26 +185,28 @@
 | bilichat_openai_token        | str       | None               | openai的apikey, 若留空则禁用openai总结 |
 | bilichat_openai_proxy        | str       | None               | 访问openai或newbing使用的代理地址 |
 | bilichat_openai_model        | str       | gpt-3.5-turbo-0301 | 使用的语言模型名称 |
 | bilichat_openai_token_limit  | int       | 3500               | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
 
 注:
 
-1. 如果同时填写了 `bilichat_openai_token` 和 `bilichat_newbing_cookie`，则会使用 `newbing` 进行总结, 并在 `newbing` 总结失败时使用 `openai` 进行总结
-2. `newbing` 和 `openai` 均有缓存机制，同一视频在**获取到正常的总结内容后**不会重复发送请求，如需刷新请求内容可以手动删除对应视频的缓存文件或整个缓存文件夹
-3. 经测试，目前 `newbing` 至少能总结 12000 字符以上的文本，推测 token 上限应为 `gpt-4-32k-0314` 的 `32200` token，但过长的内容易造成输出内容包含额外内容或总结失败，因此也建议设置一个合理的 token 上限 ~~（反正不要钱，要啥自行车）~~
-4. 由于 `newbing` 限制较大，也不如 `openai` 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
+1. openai 与 newbing 目前均需求科学上网才能使用，国内服务器请务必填写 `bilichat_openai_proxy` 或全局透明代理
+2. 如果同时填写了 `bilichat_openai_token` 和 `bilichat_newbing_cookie`，则会使用 `newbing` 进行总结, 并在 `newbing` 总结失败时使用 `openai` 进行总结
+3. `newbing` 和 `openai` 均有缓存机制，同一视频在**获取到正常的总结内容后**不会重复发送请求，如需刷新请求内容可以手动删除对应视频的缓存文件或整个缓存文件夹
+4. 经测试，目前 `newbing` 至少能总结 12000 字符以上的文本，推测 token 上限应为 `gpt-4-32k-0314` 的 `32200` token，但过长的内容易造成输出内容包含额外内容或总结失败，因此也建议设置一个合理的 token 上限 ~~（反正不要钱，要啥自行车）~~
+5. 由于 `newbing` 限制较大，也不如 `openai` 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
 
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
 ### 指令表
 
 > 正在开发指令相关，请无视这里的模板
+> 指令设计方案征集中，如果有什么想要实现的功能可以在issue中提出
 
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | 指令1 | 主人 | 否 | 私聊 | 指令说明 |
 | 指令2 | 群员 | 是 | 群聊 | 指令说明 |
 
 ## 🙏 感谢
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
     # nonebot-plugin-bilichat _â¨ å¤åè½çBç«è§é¢è§£æå·¥å· â¨_
 [license] [PyPI_-_Downloads] [pypi] [python] [pdm-managed] [Code_style:_black]
+               [onebot] [onebot] [QQ_Chat_Group] [QQ_Chat_Group]
 ## ð ä»ç»
 è§é¢é¾æ¥è§£æï¼å¹¶æ ¹æ®å¶åå®¹çæ**åºæ¬ä¿¡æ¯**ã**è¯äº**å**åå®¹æ»ç»**
 ææºç«¯è§å¾ ![](docs/mobile.png)   åºæ¬ä¿¡æ¯ ![](docs/basic.png)
 è¯äº ![](docs/wordcloud.png)   è§é¢æ»ç» ```markdown ## æ»ç»
 é«éç¬¬äºä»£éªé¾7+çå·¥ç¨æºï¼æ¥æå°ç§¯çµ4nmå·¥èºï¼CPUè§æ ¼åéªé¾8+ä¸æ¨¡ä¸æ ·ï¼GPUè§æ ¼ä¸æ¯æ°çAdreno
 700æ¶æï¼æ§è½è¡¨ç°åºä¼ï¼è½ææ²çº¿ç¨éäº8+ï¼ä½ä¸­ä½é¢æ®µè½ææ°´å¹³ç¸åï¼ç»ç«¯æºä»·æ ¼å¦æè½åå°1500-
 2000åï¼ç«äºåè¿æ¯å¾è¶³çã ## è¦ç¹ - ð»
@@ -27,32 +28,44 @@
 nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
 é¨åè¿½å åå¥ plugins = ["nonebot_plugin_bilichat"]  ## âï¸ éç½® å¨
 nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®,
 éç½®åä¸º**éå¿é¡»é¡¹** ### éç¨éç½®é¡¹ | éç½®é¡¹ | ç±»å |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | bilichat_block | bool |
 False | æ¯å¦æ¦æªäºä»¶(é²æ­¢å¶ä»æä»¶äºæ¬¡è§£æ) | |
 bilichat_enable_private | bool | True | æ¯å¦åè®¸ååºç§è | |
-bilichat_enable_v12_channel | bool | True | æ¯å¦åè®¸ååºé¢éæ¶æ¯
-(ob12ä¸å±) | | bilichat_enable_unkown_src | bool | False |
+bilichat_enable_self | bool | False | æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | |
+bilichat_enable_v12_channel | bool | True | ~~æ¯å¦åè®¸ååºé¢éæ¶æ¯
+(ob12ä¸å±)~~(ææªå®ç°) | | bilichat_enable_unkown_src | bool | False |
 æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist | list[str] | []
 | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | | bilichat_blacklist
 | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
 (é²æ­¢å·å±) | | bilichat_neterror_retry | int | 3 |
 å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | | bilichat_use_bcut_asr | bool |
-True | æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | ###
+True | æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | æ³¨: 1.
+ç±äº OneBot
+åè®®æªè§å®æ¯å¦åºä¸æ¥èªèº«äºä»¶ï¼å æ­¤å¨ä¸åçåºæ¯ä¸è½å¦è·åèªèº«äºä»¶å¹¶ä¸ä¸å®ï¼`bilichat_enable_self`
+å®éè½å¦çæä¹ä¸ä¹ç¸å³ 2. å½ `bilichat_whitelist`
+å­å¨æ¶ï¼`bilichat_blacklist` å°ä¼è¢«ç¦ç¨ 3. `bilichat_dynamic_font`
+å¯å¡«åèªå®ä¹çå­ä½urlï¼ä½å¹¶ä¸æ¨èä¿®æ¹ 4. å½ä½¿ç¨ `bcut_asr`
+æ¥å£æ¥çæAIå­å¹æ¶ï¼æ ¹æ®è§é¢æ¶é¿åç½ç»æåµæå¯è½ä¼è¯å«å¤±è´¥ï¼Botä¼æç¤º
+`BCut-ASR conversion failed due to network error`ãå¯ä»¥éè¿è°é«
+`bilichat_neterror_retry`
+æ¬¡æ°æå åéåéè¯æ¥å°è¯éæ°çæå­å¹ ###
 åºç¡ä¿¡æ¯éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:---
 -:|:----:|:----:| | bilichat_basic_info | bool | True |
 æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_reply_to_basic_info | bool | True |
 åç»­æ¶æ¯æ¯å¦åå¤åºç¡ä¿¡æ¯(å³é­ååå¤åéèçä¿¡æ¯) | ###
 è¯äºéç½®é¡¹ å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-
 bilichat[wordcloud]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:---
 -:|:----:|:----:| | bilichat_word_cloud | bool | True |
-æ¯å¦å¼å¯è¯äºåè½ | ### AIè§é¢æ»ç»éç½®é¡¹
+æ¯å¦å¼å¯è¯äºåè½ | æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº
+`wordcloud` åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11
+ä¸­å¼å¯æ­¤åè½ ### AIè§é¢æ»ç»éç½®é¡¹
 å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat
 [openai,newbing]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:
 ----:|:----:| | bilichat_newbing_cookie | str | None |
 newbingçcookieæä»¶è·¯å¾(è·åæ¹å¼åè[è¿é](https://github.com/
 acheong08/EdgeGPT#getting-authentication-required)å[è¿é](https://
 github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) ,
 è¥çç©ºåç¦ç¨newbingæ»ç» | | bilichat_newbing_token_limit | int | 0 |
@@ -60,30 +73,34 @@
 | bool | True | æ¯å¦å¯¹newbingçè¿åå¼è¿è¡é¢å¤ç,
 ä»¥å»é¤å¶ä¸­ä¸æ³è¦çåå®¹ | | bilichat_openai_token | str | None |
 openaiçapikey, è¥çç©ºåç¦ç¨openaiæ»ç» | | bilichat_openai_proxy | str
 | None | è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model
 | str | gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
 bilichat_openai_token_limit | int | 3500 | è¯·æ±çææ¬éä¸é,
 è®¡ç®æ¹å¼å¯åè[tiktoken](https://github.com/openai/tiktoken) | æ³¨: 1.
-å¦æåæ¶å¡«åäº `bilichat_openai_token` å
-`bilichat_newbing_cookie`ï¼åä¼ä½¿ç¨ `newbing` è¿è¡æ»ç», å¹¶å¨
-`newbing` æ»ç»å¤±è´¥æ¶ä½¿ç¨ `openai` è¿è¡æ»ç» 2. `newbing` å `openai`
+openai ä¸ newbing
+ç®ååéæ±ç§å­¦ä¸ç½æè½ä½¿ç¨ï¼å½åæå¡å¨è¯·å¡å¿å¡«å
+`bilichat_openai_proxy` æå¨å±éæä»£ç 2. å¦æåæ¶å¡«åäº
+`bilichat_openai_token` å `bilichat_newbing_cookie`ï¼åä¼ä½¿ç¨ `newbing`
+è¿è¡æ»ç», å¹¶å¨ `newbing` æ»ç»å¤±è´¥æ¶ä½¿ç¨ `openai` è¿è¡æ»ç» 3.
+`newbing` å `openai`
 åæç¼å­æºå¶ï¼åä¸è§é¢å¨**è·åå°æ­£å¸¸çæ»ç»åå®¹å**ä¸ä¼éå¤åéè¯·æ±ï¼å¦éå·æ°è¯·æ±åå®¹å¯ä»¥æå¨å é¤å¯¹åºè§é¢çç¼å­æä»¶ææ´ä¸ªç¼å­æä»¶å¤¹
-3. ç»æµè¯ï¼ç®å `newbing` è³å°è½æ»ç» 12000
+4. ç»æµè¯ï¼ç®å `newbing` è³å°è½æ»ç» 12000
 å­ç¬¦ä»¥ä¸çææ¬ï¼æ¨æµ token ä¸éåºä¸º `gpt-4-32k-0314` ç `32200`
 tokenï¼ä½è¿é¿çåå®¹æé æè¾åºåå®¹åå«é¢å¤åå®¹ææ»ç»å¤±è´¥ï¼å æ­¤ä¹å»ºè®®è®¾ç½®ä¸ä¸ªåçç
-token ä¸é ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 4. ç±äº `newbing`
+token ä¸é ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 5. ç±äº `newbing`
 éå¶è¾å¤§ï¼ä¹ä¸å¦ `openai`
 å¬è¯ï¼ä¸éè¦èç½æ¥è¯¢èµæï¼å æ­¤ä½¿ç¨ä½éªå¹¶ä¸å¦ chatgpt
 ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ ## ð ä½¿ç¨ ç´æ¥åéè§é¢
 (ä¸æ )é¾æ¥å³å¯ ### æä»¤è¡¨ >
-æ­£å¨å¼åæä»¤ç¸å³ï¼è¯·æ è§è¿éçæ¨¡æ¿ | æä»¤ | æé | éè¦@
-| èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | æä»¤1 | ä¸»äºº |
-å¦ | ç§è | æä»¤è¯´æ | | æä»¤2 | ç¾¤å | æ¯ | ç¾¤è | æä»¤è¯´æ
-| ## ð æè°¢ å¨æ­¤æè°¢ä»¥ä¸å¼åè
+æ­£å¨å¼åæä»¤ç¸å³ï¼è¯·æ è§è¿éçæ¨¡æ¿ >
+æä»¤è®¾è®¡æ¹æ¡å¾éä¸­ï¼å¦ææä»ä¹æ³è¦å®ç°çåè½å¯ä»¥å¨issueä¸­æåº
+| æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:
+----:| | æä»¤1 | ä¸»äºº | å¦ | ç§è | æä»¤è¯´æ | | æä»¤2 | ç¾¤å |
+æ¯ | ç¾¤è | æä»¤è¯´æ | ## ð æè°¢ å¨æ­¤æè°¢ä»¥ä¸å¼åè
 (é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT](https://github.com/JimmyLv/
 BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-collect](https://github.com/
 SocialSisterYi/bilibili-API-collect) æå§æ¶éçåç§ BiliBili Api
 åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ - [BBot-Graia](https://github.com/djkcyl/
 BBot-Graia) åè½æ¥æº ~~(æ ç æ èª å·±)~~ - [ABot-Graia](https://
 github.com/djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [nonebot-
 plugin-template](https://github.com/A-kirami/nonebot-plugin-template):
```

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,24 +44,26 @@
         "author": "djkcyl & Well404",
         "version": __version__,
         "priority": 1,
     },
 )
 
 
-async def _bili_check(event: Union[V11_ME, V12_ME], state: T_State):
-    if isinstance(event, (V11_PME, V12_PME)):
+async def _bili_check(bot: Union[V11_Bot, V12_Bot], event: Union[V11_ME, V12_ME], state: T_State):
+    if str(event.get_user_id()) == str(bot.self_id):
+        return plugin_config.bilichat_enable_self
+    elif isinstance(event, (V11_PME, V12_PME)):
         state["_uid_"] = event.user_id
         return plugin_config.bilichat_enable_private
     elif isinstance(event, (V11_GME, V12_GME)):
         state["_uid_"] = event.group_id
         return plugin_config.verify_permission(event.group_id)
-    elif isinstance(event, V12_CME):
-        state["_uid_"] = event.channel_id
-        return plugin_config.bilichat_enable_v12_channel
+    # elif isinstance(event, V12_CME):
+    #     state["_uid_"] = event.channel_id
+    #     return plugin_config.bilichat_enable_v12_channel
     else:
         state["_uid_"] = "unkown"
         return plugin_config.bilichat_enable_unkown_src
 
 
 bili = on_regex(
     r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})",
```

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib.util
+import json
 import sys
-from typing import Literal, Optional, List, Union
 from pathlib import Path
-import json
+from typing import List, Literal, Optional, Union
 
 from nonebot import get_driver
 from nonebot.log import logger
 from pydantic import BaseModel, validator
 
 # get package version
 if sys.version_info < (3, 10):
@@ -20,23 +20,24 @@
     __version__ = None
 
 
 class Config(BaseModel):
     # general
     bilichat_block: bool = False
     bilichat_enable_private: bool = True
+    bilichat_enable_self: bool = False
     bilichat_enable_v12_channel: bool = True
     bilichat_enable_unkown_src: bool = False
     bilichat_whitelist: List[str] = []
     bilichat_blacklist: List[str] = []
     bilichat_dynamic_font: Optional[str]
     bilichat_cd_time: int = 120
     bilichat_neterror_retry = 3
     nickname: List[str] = ["awesome-nonebot"]
-    
+
     # basic info
     bilichat_basic_info: bool = True
     bilichat_reply_to_basic_info: bool = True
 
     # both WC and AI
     bilichat_use_bcut_asr: bool = True
```

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,29 +74,33 @@
     # check video cd
     if not check_cd(f"{aid}_{uid}"):
         logger.warning(f"Duplicate video {aid}. Skip the video parsing process")
         return (None, None, None)
     # generate video information
     try:
         b23_url = await get_b23_url(f"https://www.bilibili.com/video/{bvid}")
-        data = (await binfo_image_create(video_info, b23_url)) if plugin_config.bilichat_basic_info else "IMG_RENDER_DISABLED"
+        data = (
+            (await binfo_image_create(video_info, b23_url))
+            if plugin_config.bilichat_basic_info
+            else "IMG_RENDER_DISABLED"
+        )
         logger.debug(f"Video parsing complete - aid:{aid} cid:{cid} title:{title}")
         return (b23_url, data, {"aid": aid, "cid": cid, "title": title})
     except TimeoutException:
         logger.warning("Video parsing API call timeout")
         return (f"{bili_number} 视频信息生成超时，请稍后再试。", None, None)
     except Exception as e:  # noqa
         capture_exception()
         logger.exception(f"Video parsing API call error: {e}")
         return (f"视频解析 API 调用出错：{e}", None, None)
 
 
 async def get_video_cache(info: Dict):
-    # get subtitle
     cache = Cache.get(f'av{info["aid"]}')
+    # cache file not exists
     if not cache:
         logger.debug(f'cache of av{info["aid"]} not exists, create cache')
         cache = Cache.create(
             id=f'av{info["aid"]}',
             title=info["title"],
             episodes={
                 str(info["cid"]): Episode(
@@ -104,19 +108,21 @@
                     content=await get_subtitle(int(info["aid"]), int(info["cid"])),
                     jieba=None,
                     openai=None,
                     newbing=None,
                 )
             },
         )
+    # cache file exists but cid not found
     elif str(info["cid"]) not in cache.episodes.keys():
         logger.debug(f'cache of av{info["aid"]} exists, but cid{info["cid"]} not found, appending cache')
         cache.episodes[str(info["cid"])] = Episode(
             title=None,
             content=await get_subtitle(int(info["aid"]), int(info["cid"])),
             jieba=None,
             openai=None,
             newbing=None,
         )
+    # cache file exists
     else:
         logger.debug(f'cache of av{info["aid"]} exists, use cache')
     return cache
```

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.0/pyproject.toml` & `nonebot_plugin_bilichat-1.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "black>=23.3.0",
     "nonebot-plugin-all4one>=0.1.0a2",
     "nonebot2[fastapi,websockets]>=2.0.0rc4",
 ]
+test = [
+    "nonebug>=0.3.2",
+    "pytest-asyncio>=0.21.0",
+]
 
 [tool.black]
 line-length = 120
 target-version = [
     "py38",
     "py39",
     "py310",
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "1.4.0"
+version = "1.4.1"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

