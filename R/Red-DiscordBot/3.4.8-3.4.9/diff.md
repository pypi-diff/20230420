# Comparing `tmp/Red-DiscordBot-3.4.8.tar.gz` & `tmp/Red-DiscordBot-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Red-DiscordBot-3.4.8.tar", last modified: Mon Apr  5 23:06:44 2021, max compression
+gzip compressed data, was "Red-DiscordBot-3.4.9.tar", last modified: Tue Apr  6 01:58:16 2021, max compression
```

## Comparing `Red-DiscordBot-3.4.8.tar` & `Red-DiscordBot-3.4.9.tar`

### file list

```diff
@@ -1,1542 +1,1542 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.580521 Red-DiscordBot-3.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)     8007 2021-04-05 23:06:44.580521 Red-DiscordBot-3.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5574 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.296521 Red-DiscordBot-3.4.8/Red_DiscordBot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8007 2021-04-05 23:06:43.000000 Red-DiscordBot-3.4.8/Red_DiscordBot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    55474 2021-04-05 23:06:44.000000 Red-DiscordBot-3.4.8/Red_DiscordBot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-05 23:06:43.000000 Red-DiscordBot-3.4.8/Red_DiscordBot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      167 2021-04-05 23:06:43.000000 Red-DiscordBot-3.4.8/Red_DiscordBot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2371 2021-04-05 23:06:43.000000 Red-DiscordBot-3.4.8/Red_DiscordBot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-05 23:06:43.000000 Red-DiscordBot-3.4.8/Red_DiscordBot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      158 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.296521 Red-DiscordBot-3.4.8/redbot/
--rw-r--r--   0 runner    (1001) docker     (121)     6907 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20979 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.296521 Red-DiscordBot-3.4.8/redbot/cogs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.296521 Red-DiscordBot-3.4.8/redbot/cogs/admin/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17850 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2239 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/announcer.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.304521 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     7741 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)    13395 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)    11178 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     7813 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)    12292 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    12070 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     9685 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)    13045 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     7737 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     5991 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     5945 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    12089 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    12104 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)    12922 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     7806 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     9019 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)     7747 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)    12064 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)    12181 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     8482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     7999 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     6041 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    12036 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)    12142 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)    12552 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)    12313 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     8840 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     7784 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)    15262 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)    11714 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     7824 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     7824 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     9086 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)    12296 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     7906 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     8649 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     9199 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     7758 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     8412 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/zh-TW.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.304521 Red-DiscordBot-3.4.8/redbot/cogs/alias/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15808 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/alias.py
--rw-r--r--   0 runner    (1001) docker     (121)     9024 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/alias_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.308521 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     4480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)     7181 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)     4612 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     4552 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)     4478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     6447 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     4477 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)     6919 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     4476 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4637 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     4430 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     6544 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     4504 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)     6702 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4527 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     4476 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)     4861 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)     6468 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)     6792 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     4577 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     7068 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4621 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     6601 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)     6725 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)     6699 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)     4632 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     4523 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)     8115 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)     4504 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     4563 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     4563 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     4546 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)     6776 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4645 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     4474 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     4872 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     4497 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     4486 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/zh-TW.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.308521 Red-DiscordBot-3.4.8/redbot/cogs/audio/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.312521 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4828 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7750 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/global_db.py
--rw-r--r--   0 runner    (1001) docker     (121)    43091 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)    15482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/local_db.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.316521 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)     3471 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     2553 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     3771 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     2478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)     3827 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3808 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     3728 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)     3645 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     2473 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     3739 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3675 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)     3718 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)     3555 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)     3164 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     2485 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     2524 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)     4499 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)     2505 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     2564 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     2564 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)     3746 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     2646 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     2475 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     2486 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     2498 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     3586 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)     5347 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/persist_queue_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    20084 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/playlist_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)    10506 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/playlist_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7880 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/spotify.py
--rw-r--r--   0 runner    (1001) docker     (121)     3096 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/youtube.py
--rw-r--r--   0 runner    (1001) docker     (121)    25799 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/audio_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)      427 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/audio_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)    20005 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.316521 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/
--rw-r--r--   0 runner    (1001) docker     (121)     5180 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16963 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4323 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/cog_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.320520 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      730 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    63670 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/audioset.py
--rw-r--r--   0 runner    (1001) docker     (121)    41399 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)    16968 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/equalizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9196 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/llset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.328521 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/
--rw-r--r--   0 runner    (1001) docker     (121)   101436 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)   120426 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)   101442 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)   101508 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)   101434 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)   103296 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)   101453 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)   124064 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)   101432 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)   140932 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)   125328 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)   119355 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)   101483 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)   101432 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)   101479 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)   104295 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)   109105 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)   102357 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)   109427 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)   137021 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)   105272 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)   130548 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)   107006 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)   101440 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)   101496 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)   134978 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)   101460 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)   101519 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)   101519 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)   101442 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)   148643 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)   101601 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)   101430 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)   101444 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)   101453 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)   109212 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)     5079 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/localtracks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5327 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (121)    44231 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/player.py
--rw-r--r--   0 runner    (1001) docker     (121)    85502 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/playlists.py
--rw-r--r--   0 runner    (1001) docker     (121)    15902 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.328521 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/
--rw-r--r--   0 runner    (1001) docker     (121)      375 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8492 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/cog.py
--rw-r--r--   0 runner    (1001) docker     (121)    12445 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/dpy.py
--rw-r--r--   0 runner    (1001) docker     (121)    24217 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/lavalink.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.336521 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     3544 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)     4340 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)     3544 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     3616 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)     3542 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     3633 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     3541 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)     4670 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     3540 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4903 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     4827 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)     4650 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3591 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     3540 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)     3552 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)     3561 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)     3563 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     3659 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     4947 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4766 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)     3637 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)     4814 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)     4186 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3548 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     3587 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)     4913 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)     3568 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     3627 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     3627 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     3545 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)     4866 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3709 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     3538 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     3549 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     3561 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     3764 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)     2117 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/red.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.340521 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/
--rw-r--r--   0 runner    (1001) docker     (121)      590 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)      738 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)      590 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)      662 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)      588 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)      668 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)      623 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)      586 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)      636 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)      618 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)      628 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)      637 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)      586 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)      636 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)      584 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)      631 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)      642 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)      629 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)      632 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)      619 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)      775 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)      649 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)      594 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)      633 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)      838 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)      668 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)      673 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)      673 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)      591 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)      617 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)      755 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)      584 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)      595 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)      607 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)      632 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/zh-TW.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.340521 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      345 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5186 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/lavalink.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.348521 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)     2343 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     2237 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     2211 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)     3961 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     2364 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)     2386 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     2261 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     4015 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3772 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)     2507 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)     2272 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)     2238 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     2297 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     2297 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     2215 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)     3942 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     2219 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     2231 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     3395 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)     4532 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/player.py
--rw-r--r--   0 runner    (1001) docker     (121)    13028 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/startup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.348521 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)      734 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7377 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/equalizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    18205 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)     5055 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/local_tracks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.356521 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/
--rw-r--r--   0 runner    (1001) docker     (121)    14317 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)    16530 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)    14317 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)    14389 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)    14315 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    15303 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)    14314 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)    19028 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)    14313 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)    19086 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    18770 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)    17774 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)    14364 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)    14313 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)    14317 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)    14746 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)    14456 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)    14342 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)    17623 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)    18400 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)    15151 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)    19060 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)    14715 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)    14321 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    14360 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)    21591 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)    14341 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)    14400 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)    14400 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)    14318 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)    18840 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)    14482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)    14311 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)    14322 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)    14334 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)    15408 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/zh-TW.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.356521 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.360521 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)      564 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)      554 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)      505 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)      529 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)      472 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)      489 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)      625 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)      486 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)      525 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)      645 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)      506 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)      647 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)      499 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)      488 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)    15064 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)    31151 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/player.py
--rw-r--r--   0 runner    (1001) docker     (121)    30427 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/playlists.py
--rw-r--r--   0 runner    (1001) docker     (121)     6755 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     3446 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.360521 Red-DiscordBot-3.4.8/redbot/cogs/audio/data/
--rw-r--r--   0 runner    (1001) docker     (121)      464 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/data/application.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/equalizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3026 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.364521 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     2296 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)     2378 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)     2296 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     2368 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)     2294 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     2319 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     2293 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)     2578 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)    34835 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    35460 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     3152 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     3221 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)     2471 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     2343 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)     2296 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)     2290 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)     2294 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     2288 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)    34826 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     3023 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)     3398 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)     2311 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     2300 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     2339 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)     3066 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)     2320 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)     3144 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     2290 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     2301 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     2302 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)    14210 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    11716 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/sql_statements.py
--rw-r--r--   0 runner    (1001) docker     (121)     6736 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/audio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.364521 Red-DiscordBot-3.4.8/redbot/cogs/bank/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5063 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/bank.py
--rw-r--r--   0 runner    (1001) docker     (121)      446 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.368521 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)     3452 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)     2375 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     2431 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     3062 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)     3324 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     1864 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     3340 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)     3401 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     2406 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)     2368 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)     2364 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)     2673 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)     3505 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     2363 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     2402 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)     4214 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)     2383 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     2833 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)     3294 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     2524 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/zh-TW.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.372521 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/checks.py
--rw-r--r--   0 runner    (1001) docker     (121)    22491 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.376521 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     6480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)     6663 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)     6480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     6552 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)     6478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     6615 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     6477 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)     6700 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     6476 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3432 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     3391 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    10407 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     6478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)     7425 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     6527 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     6476 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)    10554 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)     6507 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)     6500 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     6472 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     6523 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3423 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    11435 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)     6573 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)     6842 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)     6530 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     6484 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     6647 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)     7981 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)     6504 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     6563 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     6563 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     6630 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)    11605 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     6645 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     6474 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     6485 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     6497 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     6598 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/zh-TW.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.376521 Red-DiscordBot-3.4.8/redbot/cogs/customcom/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32229 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/customcom.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.380521 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     8926 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)    11145 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)     8926 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     8998 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)     8924 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     9906 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     9277 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)    11478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     8922 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     5941 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     5900 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    14659 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     8924 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)    11367 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     8973 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     8922 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)     8983 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)     9154 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)     9200 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     8918 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     9250 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     5932 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    14148 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)     9015 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)     9126 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)     8941 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     8930 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     8969 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)    12300 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)     8950 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     9009 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     9009 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     9129 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)    14351 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     9091 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     8920 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     8931 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     8943 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     9052 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/zh-TW.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.384521 Red-DiscordBot-3.4.8/redbot/cogs/downloader/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/checks.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/converters.py
--rw-r--r--   0 runner    (1001) docker     (121)    71082 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2759 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     6971 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/info_schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     6771 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/installable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/json_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.392521 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/
--rw-r--r--   0 runner    (1001) docker     (121)    24842 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)    29954 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)    24966 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)    24914 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)    24840 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    26182 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)    24839 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)    28018 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)    24838 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     7133 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     6854 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    35392 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    24850 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)    30744 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)    24889 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)    24838 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)    24850 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)    24921 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)    24947 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)    24954 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)    24980 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     6886 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    36977 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)    25446 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)    25162 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)    24978 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)    24846 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    24885 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)    26255 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)    24866 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)    24925 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)    24925 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)    25048 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)    39420 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)    25007 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)    24836 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)    24925 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)    24859 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)    24957 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/log.py
--rw-r--r--   0 runner    (1001) docker     (121)    40810 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/downloader/repo_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.392521 Red-DiscordBot-3.4.8/redbot/cogs/economy/
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      699 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/converters.py
--rw-r--r--   0 runner    (1001) docker     (121)    41423 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/economy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.400521 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/
--rw-r--r--   0 runner    (1001) docker     (121)    16289 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)    18673 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)    16867 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)    16361 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)    16287 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    18130 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)    16286 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)    19364 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)    16285 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     8878 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     8304 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    20496 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    16319 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)    20483 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)    16336 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)    16285 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)    16373 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)    16675 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)    16666 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)    16689 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)    16772 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     8336 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    26589 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)    17523 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)    16896 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)    16672 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)    16293 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    16332 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)    18768 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)    16313 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)    16372 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)    16372 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)    16719 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)    27462 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)    16454 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)    16283 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)    16576 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)    16306 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)    16586 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/zh-TW.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.400521 Red-DiscordBot-3.4.8/redbot/cogs/filter/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19114 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.408521 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     6766 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)     6848 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)     6766 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     6838 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)     6764 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     7478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     6763 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)     7758 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     6762 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     5024 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     4983 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     7712 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     6764 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)     7694 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     6813 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     6762 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)     6809 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)     7109 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)     7093 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     6758 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     7154 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     5015 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    11047 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)     7519 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)     6909 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)     6781 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     6770 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     6809 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)     8155 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)     6790 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     6849 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     6849 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     7084 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)    11199 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     6931 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     6760 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     6771 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     6783 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     6772 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/zh-TW.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.412521 Red-DiscordBot-3.4.8/redbot/cogs/general/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22904 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/general.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.420521 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/
--rw-r--r--   0 runner    (1001) docker     (121)    11095 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)    13226 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)    12063 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)    11167 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)    11093 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    12367 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)    12003 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)    14187 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)    11091 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     6780 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     6186 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    14990 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    13818 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)    15137 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)    11142 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)    11091 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)    13530 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)    11910 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)    11639 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)    11770 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)    11844 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     6218 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    14660 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)    12045 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)    13486 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)    11110 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)    11099 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    11138 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)    14480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)    11677 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)    11178 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)    11178 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)    11618 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)    14952 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)    11260 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)    11089 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)    11574 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)    11112 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)    11817 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/general/locales/zh-TW.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.420521 Red-DiscordBot-3.4.8/redbot/cogs/image/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9620 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/image.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.428521 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     4372 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)     6053 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)     4510 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     4444 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)     4370 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     6281 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     4369 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)     5668 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     4368 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3737 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     3619 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     6452 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     4370 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)     6371 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4419 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     4368 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)     4445 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)     4451 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)     4444 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     4463 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     4449 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3651 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     6086 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)     4709 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)     6395 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)     4387 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4376 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     4415 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)     5101 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)     4396 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     4455 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     4455 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     4445 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)     7481 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4537 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     4366 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     4499 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     4389 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     4451 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/image/locales/zh-TW.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.436521 Red-DiscordBot-3.4.8/redbot/cogs/locales/
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)      564 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)      554 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)      505 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)      529 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)      472 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)      489 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)      625 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)      486 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)      525 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)      645 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)      506 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)      647 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)      499 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)      488 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/locales/zh-TW.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.440521 Red-DiscordBot-3.4.8/redbot/cogs/mod/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      695 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/converters.py
--rw-r--r--   0 runner    (1001) docker     (121)     7497 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/events.py
--rw-r--r--   0 runner    (1001) docker     (121)    37209 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/kickban.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.448521 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/
--rw-r--r--   0 runner    (1001) docker     (121)    26406 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)    30864 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)    26581 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)    26478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)    26404 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    27771 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)    26419 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)    34287 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)    26402 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)    17594 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    17428 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    38370 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    26437 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)    38587 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)    26453 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)    26402 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)    26425 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)    27355 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)    26495 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)    26495 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)    27427 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)    17460 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    41297 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)    26618 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)    26944 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)    26444 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)    26421 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    26449 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)    30523 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)    26438 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)    26489 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)    26489 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)    26567 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)    42719 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)    26571 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)    26405 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)    26496 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)    26423 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)    27228 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)     8227 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/mod.py
--rw-r--r--   0 runner    (1001) docker     (121)    12665 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/names.py
--rw-r--r--   0 runner    (1001) docker     (121)    21427 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/slowmode.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.448521 Red-DiscordBot-3.4.8/redbot/cogs/modlog/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.468521 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     3788 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)     5088 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)     3788 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     3860 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)     3786 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     3984 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     3805 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)     5378 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     3784 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3139 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     3101 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     5281 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     3811 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)     5384 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3835 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     3784 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)     4135 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)     3930 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)     3807 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     3780 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     3959 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3143 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     5243 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)     3805 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)     4045 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)     3825 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3792 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     4773 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)     5765 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)     3812 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     3871 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     3871 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     3924 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)     5283 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     3953 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     3782 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     3817 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     3805 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     3812 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)     9569 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/modlog/modlog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.468521 Red-DiscordBot-3.4.8/redbot/cogs/mutes/
--rw-r--r--   0 runner    (1001) docker     (121)      122 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.476521 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/
--rw-r--r--   0 runner    (1001) docker     (121)    15562 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)    15848 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)    15570 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)    15634 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)    15560 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    15686 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)    15559 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)    16016 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)    15558 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)    18737 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    15587 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)    16203 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)    15609 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)    15558 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)    15570 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)    15677 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)    15577 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)    15560 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)    15665 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)    23818 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)    15567 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)    15813 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)    15621 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)    15566 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    15605 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)    16285 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)    15586 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)    15645 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)    15645 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)    15568 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)    25290 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)    15727 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)    15556 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)    15570 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)    15579 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)    15577 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)    75764 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/mutes.py
--rw-r--r--   0 runner    (1001) docker     (121)     9656 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/mutes/voicemutes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.476521 Red-DiscordBot-3.4.8/redbot/cogs/permissions/
--rw-r--r--   0 runner    (1001) docker     (121)      421 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6217 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.484521 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/
--rw-r--r--   0 runner    (1001) docker     (121)    10161 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)    10272 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)    10161 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)    10233 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)    10159 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    10706 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)    10158 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)    14415 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)    10157 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)    10137 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    10096 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    16846 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    10159 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)    12745 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)    10208 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)    10157 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)    10231 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)    10155 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)    10176 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)    10153 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)    10151 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)    10128 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    16381 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)    10174 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)    11488 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)    10203 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)    10165 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    10204 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)    12613 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)    10185 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)    10244 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)    10244 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)    10162 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)    16944 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)    10326 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)    10155 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)    10166 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)    10178 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)    10167 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)    33084 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/permissions/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.484521 Red-DiscordBot-3.4.8/redbot/cogs/reports/
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.496521 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     5045 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)     5127 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)     5045 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     5117 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)     5043 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     5494 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     5042 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)     6970 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     5041 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4461 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     4420 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     7841 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     5043 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)     6879 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     5092 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     5041 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)     5045 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)     5039 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)     5043 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     5037 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     5035 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4452 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     7657 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)     5155 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)     5188 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)     5060 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     5049 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     5088 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)     7491 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)     5069 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     5128 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     5128 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     5046 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)     7823 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     5210 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     5039 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     5050 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     5062 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     5718 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)    17187 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/reports/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.496521 Red-DiscordBot-3.4.8/redbot/cogs/streams/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      342 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.504521 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/
--rw-r--r--   0 runner    (1001) docker     (121)    11099 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)    12550 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)    11107 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)    11171 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)    11097 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    12871 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)    11096 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)    15180 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)    11095 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     9608 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     9567 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    17439 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    11109 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)    14340 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)    11146 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)    11095 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)    11099 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)    11104 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)    11104 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)    11097 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)    11111 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     9599 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    16714 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)    11099 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)    11262 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)    11114 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)    11103 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    11142 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)    15241 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)    11123 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)    11182 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)    11182 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)    12166 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)    17317 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)    11264 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)    11093 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)    11107 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)    11116 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)    11122 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)    38572 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/streams.py
--rw-r--r--   0 runner    (1001) docker     (121)    21301 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/streams/streamtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.504521 Red-DiscordBot-3.4.8/redbot/cogs/trivia/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      772 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/checks.py
--rw-r--r--   0 runner    (1001) docker     (121)      464 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.292521 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.516521 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/
--rw-r--r--   0 runner    (1001) docker     (121)     7229 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/2015.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    17580 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/2016.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    44095 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/anime.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    39235 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/artandliterature.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     9125 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/boombeach.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6187 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/cars.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6936 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/clashroyale.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    18933 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/computers.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    90845 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/disney.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    38231 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/dota2abilities.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13702 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/dota2items.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5643 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/elements.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    45994 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/entertainment.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    48659 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/finalfantasy.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4605 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/gameofthrones.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    18959 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/games.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    51451 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/general.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6379 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/geography.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    10682 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/greekmyth.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    15869 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/harrypotter.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    94811 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/hockey.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    45064 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/leagueoflegends.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     9154 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/leagueults.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    19203 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/lotr.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6638 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/michaeljackson.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     7116 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/mlb.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    19579 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/nba.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    19720 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/overwatch.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    29304 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/pokemon.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    11284 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/prince.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    53105 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/r6siege.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    10114 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/slogans.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    14630 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/sports.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    21365 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/starwars.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3153 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/uscapitals.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5702 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/usflags.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5701 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/usmap.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3821 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/usstateabbreviations.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    24985 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/warcraft.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    10632 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/whosthatpokemon.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     7051 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/whosthatpokemon2.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     9761 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/whosthatpokemon3.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     7809 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/whosthatpokemon4.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    11522 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/whosthatpokemon5.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5266 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/whosthatpokemon6.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     9871 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/worldcapitals.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    17756 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/worldflags.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    17606 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/worldmap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.524521 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/
--rw-r--r--   0 runner    (1001) docker     (121)    11304 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)    16505 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)    11304 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)    11376 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)    11302 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    11649 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)    11301 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)    16884 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)    11300 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     8361 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     8320 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    16713 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    16256 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)    17083 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)    11351 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)    11300 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)    11304 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)    11298 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)    13570 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)    11296 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)    11294 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     8352 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    16976 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)    11501 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)    11473 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)    11319 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)    11308 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    11347 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)    15246 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)    11328 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)    11387 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)    11387 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)    11305 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)    17784 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)    11469 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)    11298 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)    11339 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)    11321 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)    11310 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/log.py
--rw-r--r--   0 runner    (1001) docker     (121)    12755 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/session.py
--rw-r--r--   0 runner    (1001) docker     (121)    27009 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/trivia/trivia.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.524521 Red-DiscordBot-3.4.8/redbot/cogs/warnings/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5898 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.532521 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/
--rw-r--r--   0 runner    (1001) docker     (121)    10429 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)    10511 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)    10429 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)    10501 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)    10427 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    14491 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)    11617 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)    16209 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)    10425 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     7909 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     7868 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    10821 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    10427 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)    13735 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)    10476 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)    10425 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)    10429 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)    10575 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)    11873 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)    10421 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)    12188 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     7900 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)    15629 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)    10703 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)    10623 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)    10590 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)    10433 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    10472 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)    13296 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)    10453 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)    10512 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)    10512 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)    10430 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)    16038 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)    10594 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)    10423 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)    10434 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)    10446 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)    10435 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)    25232 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/cogs/warnings/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.536521 Red-DiscordBot-3.4.8/redbot/core/
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/_sharedlibdeprecation.py
--rw-r--r--   0 runner    (1001) docker     (121)    28666 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/bank.py
--rw-r--r--   0 runner    (1001) docker     (121)    65658 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/bot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1998 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     9865 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    15401 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/cog_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.540521 Red-DiscordBot-3.4.8/redbot/core/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     6137 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3073 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/_dpy_reimplements.py
--rw-r--r--   0 runner    (1001) docker     (121)    39428 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)    10420 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/context.py
--rw-r--r--   0 runner    (1001) docker     (121)    13770 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    33601 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/help.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.544521 Red-DiscordBot-3.4.8/redbot/core/commands/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     4176 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)     4276 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)     4180 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     4248 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)     4174 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     4493 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     4175 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)     5465 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     4172 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     5853 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     5855 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)     4652 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4223 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     4172 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)     5795 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)     4185 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)     4312 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     4177 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     4191 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     1536 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     5915 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)     4455 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)     6248 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)     4501 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4180 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     4219 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)     5481 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)     4234 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     4259 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     4259 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     5051 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)     6111 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     4341 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     4170 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     4184 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     4193 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     4653 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)    28720 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/commands/requires.py
--rw-r--r--   0 runner    (1001) docker     (121)    46859 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/config.py
--rw-r--r--   0 runner    (1001) docker     (121)   157256 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/core_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     6230 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    12587 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/dev_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.548521 Red-DiscordBot-3.4.8/redbot/core/drivers/
--rw-r--r--   0 runner    (1001) docker     (121)     3389 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18596 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/_mongo.py
--rw-r--r--   0 runner    (1001) docker     (121)    11530 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8516 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.552521 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)      564 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)      554 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)      505 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)      529 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)      472 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)      489 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)      625 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)      486 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)      525 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)      645 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)      506 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)      647 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)      499 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)      488 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)      258 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.552521 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24598 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/ddl.sql
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/drop_ddl.sql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.556521 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)      564 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)      554 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)      505 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)      529 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)      472 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)      489 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)      625 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)      486 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)      525 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)      645 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)      506 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)      647 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)      499 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)      488 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)     8078 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/postgres.py
--rw-r--r--   0 runner    (1001) docker     (121)     2555 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    18120 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     2693 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/generic_casetypes.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/global_checks.py
--rw-r--r--   0 runner    (1001) docker     (121)    10489 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.568521 Red-DiscordBot-3.4.8/redbot/core/locales/
--rw-r--r--   0 runner    (1001) docker     (121)    77441 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)    92063 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)    78588 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)    77513 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)    77439 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    81070 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)    79332 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)   104850 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     4499 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/debugging.po
--rw-r--r--   0 runner    (1001) docker     (121)    77437 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)    42825 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    41567 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)   101014 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)    79388 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)   107504 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)    77488 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)    77437 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)    80102 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)    78466 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)    79751 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)    78488 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)    78744 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)    41752 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)   118204 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)    78749 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)    88474 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)    81160 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)    77800 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)    78159 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)   110897 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)    77558 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)    77524 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)    77524 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)    80520 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)   126819 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)    77606 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)    77440 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)    78018 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)    77458 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)    77545 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)    37928 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/modlog.py
--rw-r--r--   0 runner    (1001) docker     (121)     5980 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/rpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    19557 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/settings_caches.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.568521 Red-DiscordBot-3.4.8/redbot/core/utils/
--rw-r--r--   0 runner    (1001) docker     (121)    17433 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13711 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/_internal_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1986 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/antispam.py
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (121)    15905 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/chat_formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)     3799 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/common_filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1767 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/dbtools.py
--rw-r--r--   0 runner    (1001) docker     (121)      529 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/embed.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.576521 Red-DiscordBot-3.4.8/redbot/core/utils/locales/
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/af-ZA.po
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/ar-SA.po
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/bg-BG.po
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/bs-BA.po
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/ca-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/cs-CZ.po
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/da-DK.po
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/de-DE.po
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/el-GR.po
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/en-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/en-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/es-ES.po
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/fi-FI.po
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/fr-FR.po
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/he-IL.po
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/hi-IN.po
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/hu-HU.po
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/id-ID.po
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/it-IT.po
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/ja-JP.po
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/ko-KR.po
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/lol-US.po
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/nb-NO.po
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/nl-NL.po
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/pl-PL.po
--rw-r--r--   0 runner    (1001) docker     (121)     1387 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/pt-BR.po
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/pt-PT.po
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/ro-RO.po
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/ru-RU.po
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/sk-SK.po
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/sr-CS.po
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/sr-SP.po
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/sv-SE.po
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/tr-TR.po
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/uk-UA.po
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/vi-VN.po
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/zh-CN.po
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/zh-HK.po
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/locales/zh-TW.po
--rw-r--r--   0 runner    (1001) docker     (121)     6760 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/menus.py
--rw-r--r--   0 runner    (1001) docker     (121)     7475 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/mod.py
--rw-r--r--   0 runner    (1001) docker     (121)    32978 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/predicates.py
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/safety.py
--rw-r--r--   0 runner    (1001) docker     (121)     8511 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/core/utils/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5140 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/launcher.py
--rw-r--r--   0 runner    (1001) docker     (121)    14048 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/meta.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.580521 Red-DiscordBot-3.4.8/redbot/pytest/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/pytest/alias.py
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/pytest/cog_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3759 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/pytest/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/pytest/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     6681 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/pytest/downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3740 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/pytest/downloader_testrepo.export
--rw-r--r--   0 runner    (1001) docker     (121)      380 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/pytest/economy.py
--rw-r--r--   0 runner    (1001) docker     (121)      321 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/pytest/mod.py
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/pytest/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)      880 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/pytest/rpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    13843 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.292521 Red-DiscordBot-3.4.8/redbot/vendored/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.292521 Red-DiscordBot-3.4.8/redbot/vendored/discord/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.292521 Red-DiscordBot-3.4.8/redbot/vendored/discord/ext/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 23:06:44.580521 Red-DiscordBot-3.4.8/redbot/vendored/discord/ext/menus/
--rw-r--r--   0 runner    (1001) docker     (121)    40800 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/redbot/vendored/discord/ext/menus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3275 2021-04-05 23:06:44.580521 Red-DiscordBot-3.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-04-05 23:06:34.000000 Red-DiscordBot-3.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.141753 Red-DiscordBot-3.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     8007 2021-04-06 01:58:16.145753 Red-DiscordBot-3.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5574 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.841756 Red-DiscordBot-3.4.9/Red_DiscordBot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8007 2021-04-06 01:58:15.000000 Red-DiscordBot-3.4.9/Red_DiscordBot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    55474 2021-04-06 01:58:15.000000 Red-DiscordBot-3.4.9/Red_DiscordBot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-06 01:58:15.000000 Red-DiscordBot-3.4.9/Red_DiscordBot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2021-04-06 01:58:15.000000 Red-DiscordBot-3.4.9/Red_DiscordBot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2371 2021-04-06 01:58:15.000000 Red-DiscordBot-3.4.9/Red_DiscordBot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-06 01:58:15.000000 Red-DiscordBot-3.4.9/Red_DiscordBot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.845756 Red-DiscordBot-3.4.9/redbot/
+-rw-r--r--   0 runner    (1001) docker     (121)     6907 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20979 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.845756 Red-DiscordBot-3.4.9/redbot/cogs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.845756 Red-DiscordBot-3.4.9/redbot/cogs/admin/
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17850 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2239 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/announcer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.849756 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     7741 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    13395 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11178 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7813 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12292 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12070 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9685 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    13045 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7737 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5991 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5945 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12089 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12104 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12922 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7806 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9019 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7747 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12064 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12181 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7999 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6041 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12036 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12142 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12552 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12313 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8840 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7784 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15262 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11714 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7824 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7824 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9086 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12296 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7906 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8649 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9199 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7758 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8412 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/zh-TW.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.849756 Red-DiscordBot-3.4.9/redbot/cogs/alias/
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15808 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/alias.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9024 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/alias_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.857756 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     4480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7181 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4612 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4552 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6447 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4477 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6919 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4476 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4637 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4430 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6544 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4504 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6702 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4527 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4476 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4861 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6468 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6792 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4577 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7068 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4621 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6601 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6725 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6699 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4632 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4484 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4523 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8115 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4504 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4563 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4563 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4546 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6776 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4645 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4474 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4872 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4497 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4486 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/zh-TW.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.857756 Red-DiscordBot-3.4.9/redbot/cogs/audio/
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.861756 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4828 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7750 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/global_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43091 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/local_db.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.865756 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     2481 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3471 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2481 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2553 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2479 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3771 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3827 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2477 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3808 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3728 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3846 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2477 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2481 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3645 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3751 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2473 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3739 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3675 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3718 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3555 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3164 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2485 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2524 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4499 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2505 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2564 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2564 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3746 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2646 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2475 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2486 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2498 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3586 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5347 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/persist_queue_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20084 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/playlist_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10506 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/playlist_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7880 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/spotify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3096 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25799 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/audio_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/audio_logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20005 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.865756 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     5180 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16963 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/abc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4323 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/cog_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.869756 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    63670 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/audioset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41399 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16968 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/equalizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9196 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/llset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.877756 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)   101436 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)   120426 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101442 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101508 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101434 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)   103296 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101453 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)   124064 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101432 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)   140932 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)   125328 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)   119355 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101483 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101432 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101479 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)   104295 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)   109105 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)   102357 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)   109427 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)   137021 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)   105272 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)   130548 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)   107006 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101440 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101496 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)   134978 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101460 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101519 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101519 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101442 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)   148643 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101601 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101430 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101444 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101453 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)   109212 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5079 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/localtracks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5327 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44231 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/player.py
+-rw-r--r--   0 runner    (1001) docker     (121)    85502 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15902 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.877756 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8492 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/cog.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12445 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/dpy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24217 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/lavalink.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.885756 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     3544 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4340 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3544 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3616 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3542 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3633 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3541 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4670 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3540 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4903 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4827 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4650 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3591 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3540 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3552 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3561 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3563 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3659 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4947 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4766 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3637 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4814 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4186 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3548 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3587 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4913 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3568 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3627 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3627 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3545 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4866 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3709 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3538 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3549 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3561 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3764 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2117 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/red.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.889756 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)      590 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      590 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      649 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)      633 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)      591 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/zh-TW.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.889756 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5186 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/lavalink.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.893756 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     2214 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2343 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2214 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2286 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2212 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2237 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2211 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3961 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2210 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3846 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2364 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2386 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2261 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2210 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2214 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2208 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2212 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2206 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4015 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3772 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2210 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2507 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2272 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2218 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2257 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2489 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2238 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2297 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2297 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2215 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3942 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2379 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2208 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2219 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2231 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3395 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4532 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/player.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13028 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/startup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.897756 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7377 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/equalizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18205 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5055 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/local_tracks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.901756 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)    14317 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16530 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14317 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14389 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14315 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15303 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14314 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    19028 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14313 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    19086 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    18770 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)    17774 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14364 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14313 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14317 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14746 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14456 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14342 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    17623 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    18400 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15151 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    19060 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14715 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14321 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14360 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    21591 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14341 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14400 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14400 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14318 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    18840 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14311 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14322 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14334 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15408 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/zh-TW.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.901756 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.909756 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      529 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)      506 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15064 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1323 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31151 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/player.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30427 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6755 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/queue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3446 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.909756 Red-DiscordBot-3.4.9/redbot/cogs/audio/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/data/application.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1518 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/equalizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3026 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.913756 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     2296 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2378 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2296 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2368 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2294 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2319 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2293 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2578 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2292 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    34835 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    35460 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3152 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3221 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2471 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2343 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2292 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2296 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2290 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2294 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2288 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2286 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    34826 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3023 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2292 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3398 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2311 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2300 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2339 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3066 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2320 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2379 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2379 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2909 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3144 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2290 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2301 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2313 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2302 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14210 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11716 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/sql_statements.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6736 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/audio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.913756 Red-DiscordBot-3.4.9/redbot/cogs/bank/
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5063 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/bank.py
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.921756 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     2359 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3452 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2375 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2431 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2357 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3062 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2356 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3324 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2355 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1864 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1817 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3340 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2373 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3401 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2406 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2355 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2368 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2369 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2364 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2366 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2370 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1855 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3220 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2673 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3505 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2380 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2363 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2402 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4214 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2383 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2442 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2442 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2833 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3294 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2524 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2353 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2370 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2376 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2380 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/zh-TW.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.921756 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22491 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1013 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.929756 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     6480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6663 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6552 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6615 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6477 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6700 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6476 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3432 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3391 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10407 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7425 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6527 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6476 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10554 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6507 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6500 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6472 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6523 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3423 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11435 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6573 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6842 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6530 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6484 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6647 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7981 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6504 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6563 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6563 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6630 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11605 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6645 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6474 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6485 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6497 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6598 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/zh-TW.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.929756 Red-DiscordBot-3.4.9/redbot/cogs/customcom/
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32229 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/customcom.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.937755 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     8926 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11145 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8926 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8998 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8924 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9906 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9277 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8922 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5941 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5900 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14659 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8924 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11367 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8973 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8922 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8983 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9154 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9200 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8918 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9250 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5932 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14148 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9015 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9126 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8941 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8930 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8969 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12300 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8950 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9009 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9009 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9129 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14351 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9091 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8920 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8931 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8943 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9052 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/zh-TW.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.941755 Red-DiscordBot-3.4.9/redbot/cogs/downloader/
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1252 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      706 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/converters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    71082 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2759 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6971 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/info_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6771 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/installable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1354 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/json_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.949755 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)    24842 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    29954 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24966 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24914 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24840 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26182 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24839 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    28018 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24838 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7133 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6854 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    35392 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24850 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)    30744 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24889 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24838 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24850 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24921 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24947 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24954 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24980 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6886 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    36977 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    25446 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    25162 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24978 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24846 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24885 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26255 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24866 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24925 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24925 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    25048 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    39420 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    25007 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24836 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24925 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24859 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    24957 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40810 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/downloader/repo_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.949755 Red-DiscordBot-3.4.9/redbot/cogs/economy/
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      699 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/converters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41423 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/economy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.965755 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)    16289 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    18673 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16867 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16361 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16287 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    18130 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16286 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    19364 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16285 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8878 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8304 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    20496 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16319 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)    20483 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16336 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16285 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16373 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16675 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16666 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16689 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16772 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8336 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26589 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    17523 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16896 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16672 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16293 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16332 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    18768 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16313 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16372 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16372 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16719 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    27462 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16454 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16283 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16576 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16306 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16586 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/zh-TW.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.965755 Red-DiscordBot-3.4.9/redbot/cogs/filter/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19114 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.977755 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     6766 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6848 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6766 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6838 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6764 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6763 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7758 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6762 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5024 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4983 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7712 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6764 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7694 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6813 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6762 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6809 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7109 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7093 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6758 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7154 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5015 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11047 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7519 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6909 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6781 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6770 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6809 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8155 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6790 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6849 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6849 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7084 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11199 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6931 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6760 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6771 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6783 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6772 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/zh-TW.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.977755 Red-DiscordBot-3.4.9/redbot/cogs/general/
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22904 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/general.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.985755 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)    11095 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    13226 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12063 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11167 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11093 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12367 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12003 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14187 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11091 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6780 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6186 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14990 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    13818 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15137 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11142 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11091 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    13530 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11910 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11639 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11770 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11844 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6218 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14660 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12045 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    13486 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11110 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11099 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11138 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11677 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11178 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11178 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11618 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14952 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11260 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11089 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11574 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11112 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11817 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/general/locales/zh-TW.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.985755 Red-DiscordBot-3.4.9/redbot/cogs/image/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9620 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/image.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.997755 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     4372 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6053 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4510 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4444 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4370 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6281 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4369 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5668 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4368 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3737 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3619 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6452 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4370 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6371 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4419 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4368 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4445 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4451 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4444 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4463 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4449 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3651 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6086 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4709 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6395 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4387 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4376 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4415 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5101 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4396 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4455 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4455 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4445 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7481 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4537 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4366 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4499 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4389 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4451 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/image/locales/zh-TW.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.005755 Red-DiscordBot-3.4.9/redbot/cogs/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      529 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)      506 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/locales/zh-TW.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.005755 Red-DiscordBot-3.4.9/redbot/cogs/mod/
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      695 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/abc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      718 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/converters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7497 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37209 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/kickban.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.017755 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)    26406 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    30864 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26581 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26404 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    27771 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26419 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    34287 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26402 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    17594 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    17428 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    38370 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26437 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)    38587 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26453 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26402 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26425 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    27355 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26495 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26495 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    27427 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    17460 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    41297 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26618 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26944 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26444 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26421 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26449 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    30523 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26438 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26489 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26489 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26567 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    42719 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26571 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26405 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26496 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    26423 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    27228 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8227 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/mod.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12665 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/names.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21427 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1275 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/slowmode.py
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.017755 Red-DiscordBot-3.4.9/redbot/cogs/modlog/
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.029754 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     3788 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5088 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3788 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3860 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3786 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3984 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3805 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5378 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3784 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3139 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3101 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5281 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3811 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5384 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3835 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3784 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4135 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3930 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3807 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3780 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3959 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3143 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5243 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3805 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4045 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3825 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3792 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4773 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5765 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3812 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3871 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3871 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3924 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5283 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3953 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3782 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3817 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3805 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3812 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9569 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/modlog/modlog.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.029754 Red-DiscordBot-3.4.9/redbot/cogs/mutes/
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1121 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/abc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1983 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.041754 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)    15562 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15848 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15570 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15634 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15560 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15686 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15559 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16016 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15558 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    18737 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15587 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16203 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15609 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15558 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15570 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15677 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15577 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15560 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15665 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    23818 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15567 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15813 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15621 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15566 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15605 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16285 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15586 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15645 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15645 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15568 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    25290 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15727 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15556 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15570 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15579 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15577 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)    75764 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/mutes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9656 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/mutes/voicemutes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.041754 Red-DiscordBot-3.4.9/redbot/cogs/permissions/
+-rw-r--r--   0 runner    (1001) docker     (121)      421 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6217 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.053754 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)    10161 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10272 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10161 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10233 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10159 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10706 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10158 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14415 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10157 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10137 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10096 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16846 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10159 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12745 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10208 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10157 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10231 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10155 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10176 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10153 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10151 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10128 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16381 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10174 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11488 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10203 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10165 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10204 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12613 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10185 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10244 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10244 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10162 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16944 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10326 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10155 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10166 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10178 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10167 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)    33084 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/permissions/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.053754 Red-DiscordBot-3.4.9/redbot/cogs/reports/
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.057754 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     5045 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5127 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5045 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5117 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5043 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5494 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5042 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6970 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5041 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4461 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4420 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7841 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5043 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6879 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5092 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5041 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5045 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5039 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5043 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5037 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5035 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4452 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7657 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5155 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5188 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5060 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5049 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5088 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7491 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5069 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5128 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5128 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5046 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7823 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5210 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5039 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5050 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5062 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5718 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)    17187 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/reports/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.057754 Red-DiscordBot-3.4.9/redbot/cogs/streams/
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.065754 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)    11099 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12550 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11107 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11171 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11097 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12871 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11096 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15180 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11095 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9608 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9567 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    17439 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11109 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14340 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11146 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11095 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11099 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11104 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11104 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11097 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11111 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9599 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16714 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11099 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11262 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11114 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11103 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11142 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15241 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11123 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11182 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11182 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12166 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    17317 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11264 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11093 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11107 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11116 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11122 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)    38572 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/streams.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21301 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/streams/streamtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.065754 Red-DiscordBot-3.4.9/redbot/cogs/trivia/
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.841756 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.077754 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/
+-rw-r--r--   0 runner    (1001) docker     (121)     7229 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/2015.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    17580 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/2016.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    44095 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/anime.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    39235 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/artandliterature.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     9125 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/boombeach.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6187 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/cars.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6936 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/clashroyale.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    18933 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/computers.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    90845 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/disney.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    38231 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/dota2abilities.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    13702 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/dota2items.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5643 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/elements.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    45994 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/entertainment.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    48659 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/finalfantasy.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     4605 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/gameofthrones.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    18959 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/games.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    51451 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/general.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6379 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/geography.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    10682 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/greekmyth.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    15869 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/harrypotter.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    94811 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/hockey.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    45064 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/leagueoflegends.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     9154 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/leagueults.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    19203 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/lotr.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6638 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/michaeljackson.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     7116 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/mlb.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    19579 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/nba.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    19720 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/overwatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    29304 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/pokemon.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    11284 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/prince.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    53105 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/r6siege.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    10114 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/slogans.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    14630 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/sports.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    21365 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/starwars.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     3153 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/uscapitals.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5702 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/usflags.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5701 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/usmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     3821 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/usstateabbreviations.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    24985 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/warcraft.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    10632 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/whosthatpokemon.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     7051 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/whosthatpokemon2.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     9761 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/whosthatpokemon3.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     7809 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/whosthatpokemon4.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    11522 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/whosthatpokemon5.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5266 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/whosthatpokemon6.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     9871 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/worldcapitals.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    17756 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/worldflags.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    17606 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/worldmap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.081754 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)    11304 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16505 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11304 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11376 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11302 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11649 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11301 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16884 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11300 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8361 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8320 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16713 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16256 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)    17083 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11351 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11300 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11304 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11298 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)    13570 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11296 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11294 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8352 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16976 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11501 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11473 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11319 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11308 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11347 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15246 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11328 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11387 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11387 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11305 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    17784 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11469 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11298 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11339 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11321 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11310 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12755 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/session.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27009 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/trivia/trivia.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.081754 Red-DiscordBot-3.4.9/redbot/cogs/warnings/
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5898 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.089754 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)    10429 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10511 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10429 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10501 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10427 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14491 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11617 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16209 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10425 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7909 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7868 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10821 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10427 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)    13735 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10476 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10425 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10429 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10575 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11873 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10421 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12188 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7900 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15629 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10703 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10623 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10590 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10433 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10472 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    13296 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10453 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10512 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10512 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10430 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)    16038 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10594 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10423 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10434 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10446 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    10435 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)    25232 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/cogs/warnings/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.093754 Red-DiscordBot-3.4.9/redbot/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      983 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/_sharedlibdeprecation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28666 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/bank.py
+-rw-r--r--   0 runner    (1001) docker     (121)    65658 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/bot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1998 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9865 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15401 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/cog_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.097754 Red-DiscordBot-3.4.9/redbot/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     6137 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3073 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/_dpy_reimplements.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39428 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10420 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13770 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/converter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33601 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/help.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.101754 Red-DiscordBot-3.4.9/redbot/core/commands/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     4176 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4276 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4180 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4248 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4174 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4493 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4175 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5465 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4172 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1545 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1504 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5853 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5855 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4652 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4223 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4172 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5795 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4185 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4312 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4177 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4191 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1536 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5915 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4455 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6248 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4501 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4180 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4219 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5481 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4234 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4259 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4259 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     5051 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6111 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4341 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4170 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4184 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4193 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4653 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)    28720 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/commands/requires.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46859 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)   157256 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/core_commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6230 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12587 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/dev_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.105754 Red-DiscordBot-3.4.9/redbot/core/drivers/
+-rw-r--r--   0 runner    (1001) docker     (121)     3389 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18596 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11530 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8516 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.113754 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      529 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)      506 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/log.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.113754 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24598 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/drop_ddl.sql
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.121754 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      529 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)      506 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)     8078 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2555 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18120 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2693 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/generic_casetypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/global_checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10489 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.133753 Red-DiscordBot-3.4.9/redbot/core/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)    77441 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    92063 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    78588 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)    77513 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    77439 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    81070 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)    79332 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)   104850 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     4499 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/debugging.po
+-rw-r--r--   0 runner    (1001) docker     (121)    77437 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    42825 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    41567 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)   101014 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)    79388 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)   107504 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    77488 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    77437 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    80102 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    78466 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)    79751 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    78488 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    78744 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    41752 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)   118204 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)    78749 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    88474 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)    81160 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    77800 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)    78159 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)   110897 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)    77558 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    77524 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)    77524 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)    80520 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)   126819 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)    77606 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)    77440 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    78018 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)    77458 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)    77545 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)    37928 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/modlog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5980 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19557 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/settings_caches.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.133753 Red-DiscordBot-3.4.9/redbot/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)    17433 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13711 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/_internal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1986 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/antispam.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1423 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15905 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/chat_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3799 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/common_filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1767 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/dbtools.py
+-rw-r--r--   0 runner    (1001) docker     (121)      529 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/embed.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.141753 Red-DiscordBot-3.4.9/redbot/core/utils/locales/
+-rw-r--r--   0 runner    (1001) docker     (121)     1312 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/af-ZA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1394 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/ar-SA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1356 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/bg-BG.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1384 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/bs-BA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/ca-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1398 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/cs-CZ.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1309 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/da-DK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1376 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/de-DE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1308 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/el-GR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1533 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/en-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1432 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1376 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/es-ES.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1397 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/fi-FI.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1369 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/fr-FR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1359 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/he-IL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1308 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/hi-IN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1372 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/hu-HU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1323 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/id-ID.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/it-IT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/ja-JP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1320 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/ko-KR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1470 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/lol-US.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1388 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/nb-NO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1372 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/nl-NL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1524 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/pl-PL.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1387 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/pt-BR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1316 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/pt-PT.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1355 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/ro-RO.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/ru-RU.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1405 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/sk-SK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1395 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/sr-CS.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1395 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/sr-SP.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1378 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/sv-SE.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/tr-TR.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1477 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/uk-UA.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1306 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/vi-VN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1356 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/zh-CN.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1329 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/zh-HK.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1360 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/locales/zh-TW.po
+-rw-r--r--   0 runner    (1001) docker     (121)     6760 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/menus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7475 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/mod.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32978 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1540 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/safety.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8511 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/core/utils/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5140 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14048 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/meta.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.141753 Red-DiscordBot-3.4.9/redbot/pytest/
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/pytest/alias.py
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/pytest/cog_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3759 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/pytest/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/pytest/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6681 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/pytest/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3740 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/pytest/downloader_testrepo.export
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/pytest/economy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/pytest/mod.py
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/pytest/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/pytest/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13843 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.841756 Red-DiscordBot-3.4.9/redbot/vendored/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.841756 Red-DiscordBot-3.4.9/redbot/vendored/discord/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:15.841756 Red-DiscordBot-3.4.9/redbot/vendored/discord/ext/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 01:58:16.141753 Red-DiscordBot-3.4.9/redbot/vendored/discord/ext/menus/
+-rw-r--r--   0 runner    (1001) docker     (121)    40800 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/redbot/vendored/discord/ext/menus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3275 2021-04-06 01:58:16.145753 Red-DiscordBot-3.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2021-04-06 01:58:05.000000 Red-DiscordBot-3.4.9/setup.py
```

### Comparing `Red-DiscordBot-3.4.8/PKG-INFO` & `Red-DiscordBot-3.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Red-DiscordBot
-Version: 3.4.8
+Version: 3.4.9
 Summary: A highly customisable Discord bot
 Home-page: https://github.com/Cog-Creators/Red-DiscordBot
 Author: Cog-Creators
 Author-email: cogcreators@gmail.com
 License: GPL-3.0
 Project-URL: Discord Server, https://discord.gg/red
 Project-URL: Documentation, https://docs.discord.red
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Red-DiscordBot Version: 3.4.8 Summary: A highly
+Metadata-Version: 2.1 Name: Red-DiscordBot Version: 3.4.9 Summary: A highly
 customisable Discord bot Home-page: https://github.com/Cog-Creators/Red-
 DiscordBot Author: Cog-Creators Author-email: cogcreators@gmail.com License:
 GPL-3.0 Project-URL: Discord Server, https://discord.gg/red Project-URL:
 Documentation, https://docs.discord.red Project-URL: Donate on Patreon, https:/
 /www.patreon.com/Red_Devs Project-URL: Issue Tracker, https://github.com/Cog-
 Creators/Red-DiscordBot/issues Project-URL: Source Code, https://github.com/
 Cog-Creators/Red-DiscordBot Description:
```

### Comparing `Red-DiscordBot-3.4.8/README.md` & `Red-DiscordBot-3.4.9/README.md`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/Red_DiscordBot.egg-info/PKG-INFO` & `Red-DiscordBot-3.4.9/Red_DiscordBot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Red-DiscordBot
-Version: 3.4.8
+Version: 3.4.9
 Summary: A highly customisable Discord bot
 Home-page: https://github.com/Cog-Creators/Red-DiscordBot
 Author: Cog-Creators
 Author-email: cogcreators@gmail.com
 License: GPL-3.0
 Project-URL: Discord Server, https://discord.gg/red
 Project-URL: Documentation, https://docs.discord.red
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Red-DiscordBot Version: 3.4.8 Summary: A highly
+Metadata-Version: 2.1 Name: Red-DiscordBot Version: 3.4.9 Summary: A highly
 customisable Discord bot Home-page: https://github.com/Cog-Creators/Red-
 DiscordBot Author: Cog-Creators Author-email: cogcreators@gmail.com License:
 GPL-3.0 Project-URL: Discord Server, https://discord.gg/red Project-URL:
 Documentation, https://docs.discord.red Project-URL: Donate on Patreon, https:/
 /www.patreon.com/Red_Devs Project-URL: Issue Tracker, https://github.com/Cog-
 Creators/Red-DiscordBot/issues Project-URL: Source Code, https://github.com/
 Cog-Creators/Red-DiscordBot Description:
```

### Comparing `Red-DiscordBot-3.4.8/Red_DiscordBot.egg-info/SOURCES.txt` & `Red-DiscordBot-3.4.9/Red_DiscordBot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/Red_DiscordBot.egg-info/requires.txt` & `Red-DiscordBot-3.4.9/Red_DiscordBot.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 attrs==20.3.0
 Babel==2.9.0
 chardet==3.0.4
 click==7.1.2
 colorama==0.4.4
 commonmark==0.9.1
 contextlib2==0.6.0.post1
-discord.py==1.7.0
+discord.py==1.7.1
 fuzzywuzzy==0.18.0
 idna==2.10
 Markdown==3.3.3
 multidict==5.1.0
 PyNaCl==1.3.0
 Pygments==2.7.4
 python-dateutil==2.8.1
```

### Comparing `Red-DiscordBot-3.4.8/redbot/__init__.py` & `Red-DiscordBot-3.4.9/redbot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
             import uvloop as _uvloop
         except ImportError:
             pass
         else:
             _asyncio.set_event_loop_policy(_uvloop.EventLoopPolicy())
 
 
-__version__ = "3.4.8"
+__version__ = "3.4.9"
 version_info = VersionInfo.from_str(__version__)
 
 # Filter fuzzywuzzy slow sequence matcher warning
 _warnings.filterwarnings("ignore", module=r"fuzzywuzzy.*")
 # Show DeprecationWarning
 _warnings.filterwarnings("default", category=DeprecationWarning)
```

### Comparing `Red-DiscordBot-3.4.8/redbot/__main__.py` & `Red-DiscordBot-3.4.9/redbot/__main__.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/admin.py` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/admin.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/announcer.py` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/announcer.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/converters.py` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/converters.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/admin/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/admin/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/alias.py` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/alias.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/alias_entry.py` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/alias_entry.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/alias/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/alias/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/api_utils.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/api_utils.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/global_db.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/global_db.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/interface.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/interface.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/local_db.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/local_db.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/persist_queue_wrapper.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/persist_queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/playlist_interface.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/playlist_interface.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/playlist_wrapper.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/playlist_wrapper.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/spotify.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/spotify.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/apis/youtube.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/apis/youtube.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/audio_dataclasses.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/audio_dataclasses.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/converters.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/converters.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/__init__.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/abc.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/abc.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/cog_utils.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/cog_utils.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/__init__.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/audioset.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/audioset.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/controller.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/controller.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/equalizer.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/equalizer.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/llset.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/llset.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/localtracks.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/localtracks.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/miscellaneous.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/player.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/player.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/playlists.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/playlists.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/commands/queue.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/commands/queue.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/cog.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/cog.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/dpy.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/dpy.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/lavalink.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/lavalink.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/events/red.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/events/red.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/lavalink.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/lavalink.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/player.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/player.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/tasks/startup.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/tasks/startup.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/__init__.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/equalizer.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/equalizer.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/formatting.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/formatting.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/local_tracks.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/local_tracks.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/menus/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/menus/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/miscellaneous.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/parsers.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/parsers.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/player.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/player.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/playlists.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/playlists.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/queue.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/queue.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/core/utilities/validation.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/core/utilities/validation.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/equalizer.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/equalizer.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/errors.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/errors.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/manager.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/manager.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/sql_statements.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/sql_statements.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/audio/utils.py` & `Red-DiscordBot-3.4.9/redbot/cogs/audio/utils.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/bank.py` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/bank.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/bank/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/bank/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/cleanup.py` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/cleanup.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/converters.py` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/converters.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/cleanup/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/cleanup/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/customcom.py` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/customcom.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/customcom/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/customcom/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/checks.py` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/checks.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/converters.py` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/converters.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/downloader.py` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/errors.py` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/errors.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/info_schemas.py` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/info_schemas.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/installable.py` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/installable.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/json_mixins.py` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/json_mixins.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/downloader/repo_manager.py` & `Red-DiscordBot-3.4.9/redbot/cogs/downloader/repo_manager.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/converters.py` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/converters.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/economy.py` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/economy.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/economy/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/economy/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/filter.py` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/filter.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/filter/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/filter/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/general.py` & `Red-DiscordBot-3.4.9/redbot/cogs/general/general.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/general/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/general/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/image.py` & `Red-DiscordBot-3.4.9/redbot/cogs/image/image.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/image/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/image/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/abc.py` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/abc.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/converters.py` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/converters.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/events.py` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/events.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/kickban.py` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/kickban.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/mod.py` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/mod.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/names.py` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/names.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/settings.py` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/settings.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mod/slowmode.py` & `Red-DiscordBot-3.4.9/redbot/cogs/mod/slowmode.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/modlog/modlog.py` & `Red-DiscordBot-3.4.9/redbot/cogs/modlog/modlog.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/abc.py` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/abc.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/converters.py` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/converters.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/mutes.py` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/mutes.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/mutes/voicemutes.py` & `Red-DiscordBot-3.4.9/redbot/cogs/mutes/voicemutes.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/converters.py` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/converters.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/permissions/permissions.py` & `Red-DiscordBot-3.4.9/redbot/cogs/permissions/permissions.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/reports/reports.py` & `Red-DiscordBot-3.4.9/redbot/cogs/reports/reports.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/streams.py` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/streams.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/streams/streamtypes.py` & `Red-DiscordBot-3.4.9/redbot/cogs/streams/streamtypes.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/checks.py` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/checks.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/2015.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/2015.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/2016.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/2016.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/anime.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/anime.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/artandliterature.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/artandliterature.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/boombeach.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/boombeach.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/cars.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/cars.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/clashroyale.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/clashroyale.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/computers.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/computers.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/disney.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/disney.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/dota2abilities.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/dota2abilities.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/dota2items.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/dota2items.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/elements.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/elements.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/entertainment.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/entertainment.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/finalfantasy.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/finalfantasy.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/gameofthrones.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/gameofthrones.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/games.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/games.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/general.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/general.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/geography.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/geography.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/greekmyth.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/greekmyth.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/harrypotter.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/harrypotter.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/hockey.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/hockey.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/leagueoflegends.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/leagueoflegends.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/leagueults.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/leagueults.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/lotr.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/lotr.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/michaeljackson.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/michaeljackson.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/mlb.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/mlb.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/nba.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/nba.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/overwatch.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/overwatch.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/pokemon.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/pokemon.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/prince.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/prince.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/r6siege.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/r6siege.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/slogans.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/slogans.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/sports.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/sports.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/starwars.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/starwars.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/uscapitals.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/uscapitals.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/usflags.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/usflags.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/usmap.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/usmap.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/usstateabbreviations.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/usstateabbreviations.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/warcraft.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/warcraft.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/whosthatpokemon.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/whosthatpokemon.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/whosthatpokemon2.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/whosthatpokemon2.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/whosthatpokemon3.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/whosthatpokemon3.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/whosthatpokemon4.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/whosthatpokemon4.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/whosthatpokemon5.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/whosthatpokemon5.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/whosthatpokemon6.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/whosthatpokemon6.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/worldcapitals.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/worldcapitals.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/worldflags.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/worldflags.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/data/lists/worldmap.yaml` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/data/lists/worldmap.yaml`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/session.py` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/session.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/trivia/trivia.py` & `Red-DiscordBot-3.4.9/redbot/cogs/trivia/trivia.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/helpers.py` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/helpers.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/cogs/warnings/warnings.py` & `Red-DiscordBot-3.4.9/redbot/cogs/warnings/warnings.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/_sharedlibdeprecation.py` & `Red-DiscordBot-3.4.9/redbot/core/_sharedlibdeprecation.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/bank.py` & `Red-DiscordBot-3.4.9/redbot/core/bank.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/bot.py` & `Red-DiscordBot-3.4.9/redbot/core/bot.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/checks.py` & `Red-DiscordBot-3.4.9/redbot/core/checks.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/cli.py` & `Red-DiscordBot-3.4.9/redbot/core/cli.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/cog_manager.py` & `Red-DiscordBot-3.4.9/redbot/core/cog_manager.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/__init__.py` & `Red-DiscordBot-3.4.9/redbot/core/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/_dpy_reimplements.py` & `Red-DiscordBot-3.4.9/redbot/core/commands/_dpy_reimplements.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/commands.py` & `Red-DiscordBot-3.4.9/redbot/core/commands/commands.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/context.py` & `Red-DiscordBot-3.4.9/redbot/core/commands/context.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/converter.py` & `Red-DiscordBot-3.4.9/redbot/core/commands/converter.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/errors.py` & `Red-DiscordBot-3.4.9/redbot/core/commands/errors.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/help.py` & `Red-DiscordBot-3.4.9/redbot/core/commands/help.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/core/commands/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/commands/requires.py` & `Red-DiscordBot-3.4.9/redbot/core/commands/requires.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/config.py` & `Red-DiscordBot-3.4.9/redbot/core/config.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/core_commands.py` & `Red-DiscordBot-3.4.9/redbot/core/core_commands.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/data_manager.py` & `Red-DiscordBot-3.4.9/redbot/core/data_manager.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/dev_commands.py` & `Red-DiscordBot-3.4.9/redbot/core/dev_commands.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/__init__.py` & `Red-DiscordBot-3.4.9/redbot/core/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/_mongo.py` & `Red-DiscordBot-3.4.9/redbot/core/drivers/_mongo.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/base.py` & `Red-DiscordBot-3.4.9/redbot/core/drivers/base.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/json.py` & `Red-DiscordBot-3.4.9/redbot/core/drivers/json.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/ddl.sql` & `Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/ddl.sql`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/drivers/postgres/postgres.py` & `Red-DiscordBot-3.4.9/redbot/core/drivers/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/errors.py` & `Red-DiscordBot-3.4.9/redbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/events.py` & `Red-DiscordBot-3.4.9/redbot/core/events.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/generic_casetypes.py` & `Red-DiscordBot-3.4.9/redbot/core/generic_casetypes.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/i18n.py` & `Red-DiscordBot-3.4.9/redbot/core/i18n.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/debugging.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/debugging.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/core/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/modlog.py` & `Red-DiscordBot-3.4.9/redbot/core/modlog.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/rpc.py` & `Red-DiscordBot-3.4.9/redbot/core/rpc.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/settings_caches.py` & `Red-DiscordBot-3.4.9/redbot/core/settings_caches.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/__init__.py` & `Red-DiscordBot-3.4.9/redbot/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/_internal_utils.py` & `Red-DiscordBot-3.4.9/redbot/core/utils/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/antispam.py` & `Red-DiscordBot-3.4.9/redbot/core/utils/antispam.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/caching.py` & `Red-DiscordBot-3.4.9/redbot/core/utils/caching.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/chat_formatting.py` & `Red-DiscordBot-3.4.9/redbot/core/utils/chat_formatting.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/common_filters.py` & `Red-DiscordBot-3.4.9/redbot/core/utils/common_filters.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/dbtools.py` & `Red-DiscordBot-3.4.9/redbot/core/utils/dbtools.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/embed.py` & `Red-DiscordBot-3.4.9/redbot/core/utils/embed.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/af-ZA.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/af-ZA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/ar-SA.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/ar-SA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/bg-BG.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/bg-BG.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/bs-BA.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/bs-BA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/ca-ES.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/ca-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/cs-CZ.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/cs-CZ.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/da-DK.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/da-DK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/de-DE.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/de-DE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/el-GR.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/el-GR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/en-PT.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/en-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/en-US.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/en-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/es-ES.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/es-ES.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/fi-FI.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/fi-FI.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/fr-FR.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/fr-FR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/he-IL.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/he-IL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/hi-IN.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/hi-IN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/hu-HU.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/hu-HU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/id-ID.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/id-ID.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/it-IT.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/it-IT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/ja-JP.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/ja-JP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/ko-KR.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/ko-KR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/lol-US.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/lol-US.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/nb-NO.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/nb-NO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/nl-NL.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/nl-NL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/pl-PL.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/pl-PL.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/pt-BR.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/pt-BR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/pt-PT.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/pt-PT.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/ro-RO.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/ro-RO.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/ru-RU.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/ru-RU.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/sk-SK.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/sk-SK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/sr-CS.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/sr-CS.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/sr-SP.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/sr-SP.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/sv-SE.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/sv-SE.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/tr-TR.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/tr-TR.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/uk-UA.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/uk-UA.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/vi-VN.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/vi-VN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/zh-CN.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/zh-CN.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/zh-HK.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/zh-HK.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/locales/zh-TW.po` & `Red-DiscordBot-3.4.9/redbot/core/utils/locales/zh-TW.po`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/menus.py` & `Red-DiscordBot-3.4.9/redbot/core/utils/menus.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/mod.py` & `Red-DiscordBot-3.4.9/redbot/core/utils/mod.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/predicates.py` & `Red-DiscordBot-3.4.9/redbot/core/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/safety.py` & `Red-DiscordBot-3.4.9/redbot/core/utils/safety.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/core/utils/tunnel.py` & `Red-DiscordBot-3.4.9/redbot/core/utils/tunnel.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/launcher.py` & `Red-DiscordBot-3.4.9/redbot/launcher.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/logging.py` & `Red-DiscordBot-3.4.9/redbot/logging.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/pytest/core.py` & `Red-DiscordBot-3.4.9/redbot/pytest/core.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/pytest/downloader.py` & `Red-DiscordBot-3.4.9/redbot/pytest/downloader.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/pytest/downloader_testrepo.export` & `Red-DiscordBot-3.4.9/redbot/pytest/downloader_testrepo.export`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/pytest/rpc.py` & `Red-DiscordBot-3.4.9/redbot/pytest/rpc.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/setup.py` & `Red-DiscordBot-3.4.9/redbot/setup.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/redbot/vendored/discord/ext/menus/__init__.py` & `Red-DiscordBot-3.4.9/redbot/vendored/discord/ext/menus/__init__.py`

 * *Files identical despite different names*

### Comparing `Red-DiscordBot-3.4.8/setup.cfg` & `Red-DiscordBot-3.4.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 	attrs==20.3.0
 	Babel==2.9.0
 	chardet==3.0.4
 	click==7.1.2
 	colorama==0.4.4
 	commonmark==0.9.1
 	contextlib2==0.6.0.post1
-	discord.py==1.7.0
+	discord.py==1.7.1
 	distro==1.5.0; sys_platform == "linux"
 	fuzzywuzzy==0.18.0
 	idna==2.10
 	Markdown==3.3.3
 	multidict==5.1.0
 	PyNaCl==1.3.0
 	Pygments==2.7.4
```

