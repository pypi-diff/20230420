# Comparing `tmp/fiduswriter-gitrepo-export-3.11.3.tar.gz` & `tmp/fiduswriter-gitrepo-export-3.11.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/johannes/src/fiduswriter/fiduswriter-gitrepo-export/dist/.tmp-3hn5anu3/fiduswriter-gitrepo-export-3.11.3.tar", last modified: Mon Apr 17 10:47:49 2023, max compression
+gzip compressed data, was "/home/johannes/src/fiduswriter/fiduswriter-gitrepo-export/dist/.tmp-3oqge60h/fiduswriter-gitrepo-export-3.11.4.tar", last modified: Thu Apr 20 12:43:04 2023, max compression
```

## Comparing `fiduswriter-gitrepo-export-3.11.3.tar` & `fiduswriter-gitrepo-export-3.11.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.889304 fiduswriter-gitrepo-export-3.11.3/
--rw-r--r--   0 johannes  (1000) johannes  (1000)    34523 2020-04-02 14:48:36.000000 fiduswriter-gitrepo-export-3.11.3/LICENSE
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      338 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/MANIFEST.in
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2726 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/PKG-INFO
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1857 2023-03-01 06:56:29.000000 fiduswriter-gitrepo-export-3.11.3/README.md
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.869304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.877304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      280 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/admin.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      143 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/apps.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.877304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/helpers/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/helpers/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2509 2023-04-13 22:20:28.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/helpers/github.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2704 2023-04-13 22:39:13.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/helpers/gitlab.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/bg/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.877304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2206 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3539 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/de/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.881304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1800 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3133 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/es/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.881304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1763 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3123 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/fr/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.881304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1784 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3117 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/it/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.881304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1711 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3044 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/pt_BR/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.881304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1755 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3088 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.881304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/migrations/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2586 2023-02-26 06:56:30.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/migrations/0001_initial.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/migrations/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1057 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/models.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    11633 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/books_overview.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2482 2023-02-25 17:01:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_exporters.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5779 2023-04-13 22:39:18.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_processor.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       53 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3325 2023-04-13 22:39:54.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_file.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2149 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_tree.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3058 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_zip_contents.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      183 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      372 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/promise_chain.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2234 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_exporters.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5342 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_processor.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       53 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3303 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/commit.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       76 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1521 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/zip2blobs.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       62 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3024 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/templates.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1403 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/tools.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/plugins/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/plugins/books_overview/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       74 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/plugins/books_overview/gitrepo_export.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      795 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/urls.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6267 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/views.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/fiduswriter_gitrepo_export.egg-info/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2726 2023-04-17 10:47:49.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter_gitrepo_export.egg-info/PKG-INFO
--rw-r--r--   0 johannes  (1000) johannes  (1000)     3004 2023-04-17 10:47:49.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter_gitrepo_export.egg-info/SOURCES.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)        1 2023-04-17 10:47:49.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter_gitrepo_export.egg-info/dependency_links.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)       20 2023-04-17 10:47:49.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter_gitrepo_export.egg-info/top_level.txt
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      914 2023-04-17 10:47:34.000000 fiduswriter-gitrepo-export-3.11.3/pyproject.toml
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       38 2023-04-17 10:47:49.889304 fiduswriter-gitrepo-export-3.11.3/setup.cfg
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1083 2023-03-01 06:58:00.000000 fiduswriter-gitrepo-export-3.11.3/setup.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.408136 fiduswriter-gitrepo-export-3.11.4/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    34523 2020-04-02 14:48:36.000000 fiduswriter-gitrepo-export-3.11.4/LICENSE
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      338 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/MANIFEST.in
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2726 2023-04-20 12:43:04.408136 fiduswriter-gitrepo-export-3.11.4/PKG-INFO
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1857 2023-03-01 06:56:29.000000 fiduswriter-gitrepo-export-3.11.4/README.md
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.396136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.400136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      280 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/admin.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      143 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/apps.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.400136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/helpers/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/helpers/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2610 2023-04-20 12:37:43.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/helpers/github.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2750 2023-04-20 12:37:57.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/helpers/gitlab.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.396136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.396136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/bg/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.400136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2206 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3539 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.396136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/de/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.400136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1800 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3133 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.396136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/es/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.400136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1763 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3123 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.396136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/fr/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.404136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1784 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3117 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.396136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/it/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.404136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1711 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3044 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.396136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/pt_BR/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.404136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1755 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3088 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.404136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/migrations/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2586 2023-02-26 06:56:30.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/migrations/0001_initial.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/migrations/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1057 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/models.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.396136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.396136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.396136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.404136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    11633 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/books_overview.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.404136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2482 2023-02-25 17:01:11.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_exporters.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5779 2023-04-13 22:39:18.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_processor.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       53 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.408136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3325 2023-04-13 22:39:54.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_file.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2149 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_tree.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3058 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_zip_contents.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      183 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      372 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/promise_chain.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.408136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2234 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_exporters.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5342 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_processor.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       53 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.408136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3303 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/commit.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       76 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1521 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/zip2blobs.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       62 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3241 2023-04-20 12:40:31.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/templates.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1403 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/tools.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.396136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/plugins/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.408136 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/plugins/books_overview/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       74 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/plugins/books_overview/gitrepo_export.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      795 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/urls.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6267 2023-04-20 12:39:06.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/views.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-20 12:43:04.408136 fiduswriter-gitrepo-export-3.11.4/fiduswriter_gitrepo_export.egg-info/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2726 2023-04-20 12:43:04.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter_gitrepo_export.egg-info/PKG-INFO
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     3004 2023-04-20 12:43:04.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter_gitrepo_export.egg-info/SOURCES.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        1 2023-04-20 12:43:04.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter_gitrepo_export.egg-info/dependency_links.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       20 2023-04-20 12:43:04.000000 fiduswriter-gitrepo-export-3.11.4/fiduswriter_gitrepo_export.egg-info/top_level.txt
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      914 2023-04-20 12:42:30.000000 fiduswriter-gitrepo-export-3.11.4/pyproject.toml
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       38 2023-04-20 12:43:04.408136 fiduswriter-gitrepo-export-3.11.4/setup.cfg
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1083 2023-03-01 06:58:00.000000 fiduswriter-gitrepo-export-3.11.4/setup.py
```

### Comparing `fiduswriter-gitrepo-export-3.11.3/LICENSE` & `fiduswriter-gitrepo-export-3.11.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/PKG-INFO` & `fiduswriter-gitrepo-export-3.11.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiduswriter-gitrepo-export
-Version: 3.11.3
+Version: 3.11.4
 Summary: A Fidus Writer plugin to allow publishing of books to a Gitlab/Github repository.
 Author-email: Johannes Wilm <johannes@fiduswriter.org>
 License: AGPL-3.0-or-later
 Project-URL: repository, https://www.github.org/fiduswriter/fiduswriter-gitrepo-export
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
```

### Comparing `fiduswriter-gitrepo-export-3.11.3/README.md` & `fiduswriter-gitrepo-export-3.11.4/README.md`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/helpers/github.py` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/helpers/github.py`

 * *Files 12% similar despite different names*

```diff
@@ -65,13 +65,16 @@
         url = f"https://api.github.com/user/repos?page={page}&per_page=100"
         request = Request("GET", url, headers=headers)
         async with AsyncClient(
             timeout=88  # Firefox times out after 90 seconds, so we need to return before that.
         ) as client:
             response = await client.send(request)
         content = json.loads(response.text)
-        repos += map(githubrepo2repodata, content)
-        if len(content) == 100:
-            page += 1
+        if isinstance(content, list):
+            repos += map(githubrepo2repodata, content)
+            if len(content) == 100:
+                page += 1
+            else:
+                last_page = True
         else:
             last_page = True
     return repos
```

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/helpers/gitlab.py` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/helpers/gitlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,16 @@
 
 
 async def get_repos(gitlab_token):
     # TODO: API documentation unclear on whether pagination is required.
     headers = get_headers(gitlab_token)
     repos = []
     url = f"{GITLAB_BASE_URL}projects?min_access_level=30&simple=true"
-    request = Request("GET", url, headers)
+    request = Request("GET", url, headers=headers)
     async with AsyncClient(
         timeout=88  # Firefox times out after 90 seconds, so we need to return before that.
     ) as client:
         response = await client.send(request)
     content = json.loads(response.text)
-    repos += map(gitlabrepo2repodata, content)
+    if isinstance(content, list):
+        repos += map(gitlabrepo2repodata, content)
     return repos
```

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.mo` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.po` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.mo` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.po` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.mo` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.po` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.mo` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.po` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.mo` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.po` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.po` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/migrations/0001_initial.py` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/models.py` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/models.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/books_overview.js` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/books_overview.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_exporters.js` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_exporters.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_processor.js` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_processor.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_file.js` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_file.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_tree.js` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_tree.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_zip_contents.js` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_zip_contents.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_exporters.js` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_exporters.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_processor.js` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_processor.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/commit.js` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/commit.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/zip2blobs.js` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/zip2blobs.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/templates.js` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/templates.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -23,38 +23,43 @@
 }) => {
     const bookRepo = bookRepos[book.id]
     return `<tr>
         <th>
             <h4 class="fw-tablerow-title">${gettext("Git repository")}</h4>
         </th>
         <td>
-            <select class="entryForm" name="book-settings-repository"
-                title="${gettext("Select git repository to export to")}"
-                id="book-settings-repository"
-                ${
+            <div class="fw-select-container">
+                <select class="entry-form dk fw-button fw-light fw-large" name="book-settings-repository"
+                    title="${gettext("Select git repository to export to")}"
+                    id="book-settings-repository"
+                    ${
     book.rights === "read" ?
         "disabled=\"disabled\"" :
         ""
 }
-            >
-            ${
+                >
+                ${
     bookRepo ?
         `<option value="${bookRepo.repo_type}-${bookRepo.repo_id}" selected>${repoName(bookRepo.repo_name, bookRepo.repo_type, userReposMultitype)}</option>
-                    <option value="-0"></option>` :
+                        <option value="-0"></option>` :
         "<option value=\"-0\" selected></option>"
 }
-            ${
+                ${
     Object.entries(userRepos).sort((a, b) => a[1].name > b[1].name ? 1 : -1).map(([key, repo]) =>
         `<option value="${key}">${repoName(repo.name, repo.type, userReposMultitype)}</option>`
     ).join("")
 }
-            </select>
-            <button type="button" class="ui-button ui-widget ui-state-default ui-corner-all ui-button-text-only fw-button fw-dark fw-small reload">
-                ${gettext("Reload")}
-            </button>
+                </select>
+                <div class="fw-select-arrow fa fa-caret-down"></div>
+            </div>
+        </td>
+        <td>
+        <button type="button" class="ui-button ui-widget ui-state-default ui-corner-all ui-button-text-only fw-button fw-dark fw-small reload">
+            ${gettext("Reload")}
+        </button>
         </td>
     </tr>
 
     <tr>
         <th>
             <h4 class="fw-tablerow-title">${gettext("Export EPUB")}</h4>
         </th>
```

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/tools.js` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/tools.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/urls.py` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/urls.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/views.py` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter/gitrepo_export/views.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter_gitrepo_export.egg-info/PKG-INFO` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter_gitrepo_export.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiduswriter-gitrepo-export
-Version: 3.11.3
+Version: 3.11.4
 Summary: A Fidus Writer plugin to allow publishing of books to a Gitlab/Github repository.
 Author-email: Johannes Wilm <johannes@fiduswriter.org>
 License: AGPL-3.0-or-later
 Project-URL: repository, https://www.github.org/fiduswriter/fiduswriter-gitrepo-export
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
```

### Comparing `fiduswriter-gitrepo-export-3.11.3/fiduswriter_gitrepo_export.egg-info/SOURCES.txt` & `fiduswriter-gitrepo-export-3.11.4/fiduswriter_gitrepo_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.3/pyproject.toml` & `fiduswriter-gitrepo-export-3.11.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=65.6.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fiduswriter-gitrepo-export"
 description = "A Fidus Writer plugin to allow publishing of books to a Gitlab/Github repository."
-version = "3.11.3"
+version = "3.11.4"
 readme = "README.md"
 license = {text = "AGPL-3.0-or-later"}
 authors = [
   {email = "johannes@fiduswriter.org", name = "Johannes Wilm"},
 ]
 classifiers=[
   "Environment :: Web Environment",
```

### Comparing `fiduswriter-gitrepo-export-3.11.3/setup.py` & `fiduswriter-gitrepo-export-3.11.4/setup.py`

 * *Files identical despite different names*

