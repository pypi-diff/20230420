# Comparing `tmp/llm4gpt-2023.4.20.14.31.20.tar.gz` & `tmp/llm4gpt-2023.4.20.17.30.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4gpt-2023.4.20.14.31.20.tar", last modified: Thu Apr 20 06:31:20 2023, max compression
+gzip compressed data, was "llm4gpt-2023.4.20.17.30.9.tar", last modified: Thu Apr 20 09:30:09 2023, max compression
```

## Comparing `llm4gpt-2023.4.20.14.31.20.tar` & `llm4gpt-2023.4.20.17.30.9.tar`

### file list

```diff
@@ -1,113 +1,57 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.556660 llm4gpt-2023.4.20.14.31.20/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1206 2023-04-11 04:36:04.000000 llm4gpt-2023.4.20.14.31.20/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1370 2023-04-20 06:31:20.556771 llm4gpt-2023.4.20.14.31.20/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      553 2023-04-11 06:33:00.000000 llm4gpt-2023.4.20.14.31.20/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.532168 llm4gpt-2023.4.20.14.31.20/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      379 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-11 04:38:41.000000 llm4gpt-2023.4.20.14.31.20/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.532708 llm4gpt-2023.4.20.14.31.20/llm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/llm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.533235 llm4gpt-2023.4.20.14.31.20/llm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/llm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/llm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/llm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/llm/llm4gpt.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.533594 llm4gpt-2023.4.20.14.31.20/llm/models/
--rw-r--r--   0 betterme   (501) staff       (20)       29 2023-04-20 06:28:16.000000 llm4gpt-2023.4.20.14.31.20/llm/models/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1400 2023-04-20 06:31:18.000000 llm4gpt-2023.4.20.14.31.20/llm/models/chatglm.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.533722 llm4gpt-2023.4.20.14.31.20/llm/uis/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.20.14.31.20/llm/uis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2926 2023-04-20 06:24:44.000000 llm4gpt-2023.4.20.14.31.20/llm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.534896 llm4gpt-2023.4.20.14.31.20/llm4gpt.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     1370 2023-04-20 06:31:20.000000 llm4gpt-2023.4.20.14.31.20/llm4gpt.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     2191 2023-04-20 06:31:20.000000 llm4gpt-2023.4.20.14.31.20/llm4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 06:31:20.000000 llm4gpt-2023.4.20.14.31.20/llm4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-20 06:31:20.000000 llm4gpt-2023.4.20.14.31.20/llm4gpt.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 06:31:20.000000 llm4gpt-2023.4.20.14.31.20/llm4gpt.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       31 2023-04-20 06:31:20.000000 llm4gpt-2023.4.20.14.31.20/llm4gpt.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-20 06:31:20.000000 llm4gpt-2023.4.20.14.31.20/llm4gpt.egg-info/top_level.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       32 2023-04-13 05:31:18.000000 llm4gpt-2023.4.20.14.31.20/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-20 06:31:20.557096 llm4gpt-2023.4.20.14.31.20/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.20.14.31.20/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.535194 llm4gpt-2023.4.20.14.31.20/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.14.31.20/tox.ini
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.541849 llm4gpt-2023.4.20.14.31.20/wenda/
--rw-r--r--   0 betterme   (501) staff       (20)  2467981 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/20B_tokenizer.json
--rw-r--r--   0 betterme   (501) staff       (20)     3896 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     3638 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/YuanAPI.py
--rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-04-13 04:03:39.000000 llm4gpt-2023.4.20.14.31.20/wenda/conf.yml
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.545139 llm4gpt-2023.4.20.14.31.20/wenda/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)    64678 2023-04-13 02:39:17.000000 llm4gpt-2023.4.20.14.31.20/wenda/imgs/func.png
--rw-r--r--   0 betterme   (501) staff       (20)    97397 2023-04-13 02:39:17.000000 llm4gpt-2023.4.20.14.31.20/wenda/imgs/novel.png
--rw-r--r--   0 betterme   (501) staff       (20)    61231 2023-04-13 02:39:17.000000 llm4gpt-2023.4.20.14.31.20/wenda/imgs/setting.png
--rw-r--r--   0 betterme   (501) staff       (20)    14173 2023-04-13 02:39:17.000000 llm4gpt-2023.4.20.14.31.20/wenda/imgs/setting2.png
--rw-r--r--   0 betterme   (501) staff       (20)   166421 2023-04-13 02:39:17.000000 llm4gpt-2023.4.20.14.31.20/wenda/imgs/wzmx.png
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-13 02:39:17.000000 llm4gpt-2023.4.20.14.31.20/wenda/imgs/zsk-glm.png
--rw-r--r--   0 betterme   (501) staff       (20)   431957 2023-04-13 02:39:17.000000 llm4gpt-2023.4.20.14.31.20/wenda/imgs/zsk-rwkv.png
--rw-r--r--   0 betterme   (501) staff       (20)    72379 2023-04-13 02:39:17.000000 llm4gpt-2023.4.20.14.31.20/wenda/imgs/zsk-test.png
--rw-r--r--   0 betterme   (501) staff       (20)    34523 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/licence
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.547886 llm4gpt-2023.4.20.14.31.20/wenda/plugins/
--rw-r--r--   0 betterme   (501) staff       (20)      991 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/plugins/defineSQL.py
--rw-r--r--   0 betterme   (501) staff       (20)     1470 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/plugins/gen_data_s.py
--rw-r--r--   0 betterme   (501) staff       (20)     2321 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/plugins/gen_data_x.py
--rw-r--r--   0 betterme   (501) staff       (20)     3211 2023-04-12 01:31:21.000000 llm4gpt-2023.4.20.14.31.20/wenda/plugins/llm_glm6b.py
--rw-r--r--   0 betterme   (501) staff       (20)     1043 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/plugins/llm_llama.py
--rw-r--r--   0 betterme   (501) staff       (20)     3446 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/plugins/llm_rwkv.py
--rw-r--r--   0 betterme   (501) staff       (20)     3085 2023-04-13 02:12:33.000000 llm4gpt-2023.4.20.14.31.20/wenda/plugins/settings.py
--rw-r--r--   0 betterme   (501) staff       (20)     1467 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/plugins/zhishiku_bing.py
--rw-r--r--   0 betterme   (501) staff       (20)     1502 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/plugins/zhishiku_bingsite.py
--rw-r--r--   0 betterme   (501) staff       (20)     1540 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/plugins/zhishiku_bingxs.py
--rw-r--r--   0 betterme   (501) staff       (20)     2851 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/plugins/zhishiku_knowledge_graph.py
--rw-r--r--   0 betterme   (501) staff       (20)      622 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/plugins/zhishiku_s.py
--rw-r--r--   0 betterme   (501) staff       (20)      547 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/plugins/zhishiku_wn.py
--rw-r--r--   0 betterme   (501) staff       (20)     1223 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/plugins/zhishiku_x.py
--rw-r--r--   0 betterme   (501) staff       (20)    12288 2023-04-13 04:04:33.000000 llm4gpt-2023.4.20.14.31.20/wenda/record.db
--rw-r--r--   0 betterme   (501) staff       (20)       70 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/requirements-bing.txt
--rw-r--r--   0 betterme   (501) staff       (20)       11 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/requirements-glm6b-lora.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/requirements-rwkv.txt
--rw-r--r--   0 betterme   (501) staff       (20)      100 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/requirements-sy.txt
--rw-r--r--   0 betterme   (501) staff       (20)      168 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/requirements-yy.txt
--rw-r--r--   0 betterme   (501) staff       (20)      176 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/run_GLM6B.sh
--rw-r--r--   0 betterme   (501) staff       (20)      151 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/run_data_processing.sh
--rw-r--r--   0 betterme   (501) staff       (20)      175 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/run_rwkv.sh
--rw-r--r--   0 betterme   (501) staff       (20)     2235 2023-04-12 01:31:21.000000 llm4gpt-2023.4.20.14.31.20/wenda/setting.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.548052 llm4gpt-2023.4.20.14.31.20/wenda/views/
--rw-r--r--   0 betterme   (501) staff       (20)    14365 2023-04-13 02:13:05.000000 llm4gpt-2023.4.20.14.31.20/wenda/views/index.html
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.551735 llm4gpt-2023.4.20.14.31.20/wenda/views/static/
--rw-r--r--   0 betterme   (501) staff       (20)   103012 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/views/static/markdown-it.min.js
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.526439 llm4gpt-2023.4.20.14.31.20/wenda/views/static/mdi_font/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.554175 llm4gpt-2023.4.20.14.31.20/wenda/views/static/mdi_font/css/
--rw-r--r--   0 betterme   (501) staff       (20)   374378 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/views/static/mdi_font/css/materialdesignicons.css
--rw-r--r--   0 betterme   (501) staff       (20)   309937 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/views/static/mdi_font/css/materialdesignicons.min.css
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 06:31:20.555725 llm4gpt-2023.4.20.14.31.20/wenda/views/static/mdi_font/fonts/
--rw-r--r--   0 betterme   (501) staff       (20)   528804 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/views/static/mdi_font/fonts/materialdesignicons-webfont.woff
--rw-r--r--   0 betterme   (501) staff       (20)   366844 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/views/static/mdi_font/fonts/materialdesignicons-webfont.woff2
--rw-r--r--   0 betterme   (501) staff       (20)    94151 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/views/static/vue.js
--rw-r--r--   0 betterme   (501) staff       (20)   536684 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/views/static/vuetify.min.css
--rw-r--r--   0 betterme   (501) staff       (20)   535254 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/views/static/vuetify.min.js
--rw-r--r--   0 betterme   (501) staff       (20)     6957 2023-04-12 01:09:53.000000 llm4gpt-2023.4.20.14.31.20/wenda/wenda.py
--rw-r--r--   0 betterme   (501) staff       (20)      451 2023-04-12 08:29:49.000000 llm4gpt-2023.4.20.14.31.20/wenda/zippp.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.713052 llm4gpt-2023.4.20.17.30.9/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1206 2023-04-11 04:36:04.000000 llm4gpt-2023.4.20.17.30.9/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1369 2023-04-20 09:30:09.713141 llm4gpt-2023.4.20.17.30.9/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      553 2023-04-11 06:33:00.000000 llm4gpt-2023.4.20.17.30.9/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.710512 llm4gpt-2023.4.20.17.30.9/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      379 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-11 04:38:41.000000 llm4gpt-2023.4.20.17.30.9/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.710900 llm4gpt-2023.4.20.17.30.9/llm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/llm/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1497 2023-04-20 07:47:11.000000 llm4gpt-2023.4.20.17.30.9/llm/chatllm.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.711327 llm4gpt-2023.4.20.17.30.9/llm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/llm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/llm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/llm/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.711594 llm4gpt-2023.4.20.17.30.9/llm/kb/
+-rw-r--r--   0 betterme   (501) staff       (20)     1458 2023-04-20 09:28:22.000000 llm4gpt-2023.4.20.17.30.9/llm/kb/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 08:50:43.000000 llm4gpt-2023.4.20.17.30.9/llm/kb/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.711712 llm4gpt-2023.4.20.17.30.9/llm/uis/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.20.17.30.9/llm/uis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2923 2023-04-20 09:28:23.000000 llm4gpt-2023.4.20.17.30.9/llm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.712634 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1369 2023-04-20 09:30:09.000000 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      825 2023-04-20 09:30:09.000000 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 09:30:09.000000 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-20 09:30:09.000000 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 09:30:09.000000 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       31 2023-04-20 09:30:09.000000 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-20 09:30:09.000000 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       32 2023-04-13 05:31:18.000000 llm4gpt-2023.4.20.17.30.9/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-20 09:30:09.713420 llm4gpt-2023.4.20.17.30.9/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.20.17.30.9/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.712903 llm4gpt-2023.4.20.17.30.9/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/tox.ini
```

### Comparing `llm4gpt-2023.4.20.14.31.20/.gitignore` & `llm4gpt-2023.4.20.17.30.9/.gitignore`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.14.31.20/.travis.yml` & `llm4gpt-2023.4.20.17.30.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.14.31.20/CONTRIBUTING.rst` & `llm4gpt-2023.4.20.17.30.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.14.31.20/LICENSE` & `llm4gpt-2023.4.20.17.30.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.14.31.20/Makefile` & `llm4gpt-2023.4.20.17.30.9/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.14.31.20/PKG-INFO` & `llm4gpt-2023.4.20.17.30.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.20.14.31.20
+Version: 2023.4.20.17.30.9
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.20.14.31.20/README.md` & `llm4gpt-2023.4.20.17.30.9/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.14.31.20/README.rst` & `llm4gpt-2023.4.20.17.30.9/README.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.14.31.20/docs/Makefile` & `llm4gpt-2023.4.20.17.30.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.14.31.20/docs/conf.py` & `llm4gpt-2023.4.20.17.30.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.14.31.20/docs/installation.rst` & `llm4gpt-2023.4.20.17.30.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.14.31.20/docs/make.bat` & `llm4gpt-2023.4.20.17.30.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.14.31.20/llm/clis/cli.py` & `llm4gpt-2023.4.20.17.30.9/llm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.14.31.20/llm/utils.py` & `llm4gpt-2023.4.20.17.30.9/llm/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         assert gpu_target < num_gpus
         device_map[f'transformer.layers.{i}'] = gpu_target
         used += 1
 
     return device_map
 
 
-
 def llm_load(model_name_or_path="THUDM/chatglm-6b", device='cpu', device_map: Optional[Dict[str, int]] = None,
              **kwargs):
     tokenizer = AutoTokenizer.from_pretrained(model_name_or_path, trust_remote_code=True)
     model = AutoModel.from_pretrained(model_name_or_path, trust_remote_code=True, **kwargs)
 
     if torch.cuda.is_available() and device.lower().startswith("cuda"):
         # 根据当前设备GPU数量决定是否进行多卡部署
@@ -75,9 +74,7 @@
     return model.eval(), tokenizer
 
 
 if __name__ == '__main__':
     # cuda_empty_cache()
 
     a = llm_load("/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm")
-
-
```

### Comparing `llm4gpt-2023.4.20.14.31.20/llm4gpt.egg-info/PKG-INFO` & `llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.20.14.31.20
+Version: 2023.4.20.17.30.9
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.20.14.31.20/setup.py` & `llm4gpt-2023.4.20.17.30.9/setup.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.14.31.20/tests/test_llm4gpt.py` & `llm4gpt-2023.4.20.17.30.9/tests/test_llm4gpt.py`

 * *Files identical despite different names*

