# Comparing `tmp/pywaclient-1.3.3.tar.gz` & `tmp/pywaclient-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywaclient-1.3.3.tar", last modified: Fri Apr  7 16:22:04 2023, max compression
+gzip compressed data, was "dist/pywaclient-1.3.4.tar", last modified: Thu Apr 20 14:55:23 2023, max compression
```

## Comparing `pywaclient-1.3.3.tar` & `pywaclient-1.3.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:22:04.000000 pywaclient-1.3.3/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-07 16:21:50.000000 pywaclient-1.3.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-04-07 16:21:50.000000 pywaclient-1.3.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-04-07 16:21:50.000000 pywaclient-1.3.3/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2208 2023-04-07 16:22:04.000000 pywaclient-1.3.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1759 2023-04-07 16:21:50.000000 pywaclient-1.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:22:04.000000 pywaclient-1.3.3/pywaclient/
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3560 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:22:04.000000 pywaclient-1.3.3/pywaclient/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)     7013 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/articles.py
--rw-rw-rw-   0 root         (0) root         (0)     2242 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/block_templates.py
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/canvas.py
--rw-rw-rw-   0 root         (0) root         (0)     2265 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/categories.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/chronicles.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/histories.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/images.py
--rw-rw-rw-   0 root         (0) root         (0)     5984 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/manuscripts.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/map_marker_types.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/maps.py
--rw-rw-rw-   0 root         (0) root         (0)     3076 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/notebooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1048 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/rpg_system.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/secrets.py
--rw-rw-rw-   0 root         (0) root         (0)      808 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/subscriber_groups.py
--rw-rw-rw-   0 root         (0) root         (0)      794 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/timelines.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/users.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/variables.py
--rw-rw-rw-   0 root         (0) root         (0)    14182 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/endpoints/worlds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:22:04.000000 pywaclient-1.3.3/pywaclient/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)     2777 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/exceptions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:22:04.000000 pywaclient-1.3.3/pywaclient/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6892 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/models/article.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/models/block.py
--rw-rw-rw-   0 root         (0) root         (0)     3532 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/models/category.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/models/entity.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/models/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     5558 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/models/manuscript.py
--rw-rw-rw-   0 root         (0) root         (0)     1640 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/models/secret.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/models/user.py
--rw-rw-rw-   0 root         (0) root         (0)     4012 2023-04-07 16:21:50.000000 pywaclient-1.3.3/pywaclient/models/world.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:22:04.000000 pywaclient-1.3.3/pywaclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2208 2023-04-07 16:22:04.000000 pywaclient-1.3.3/pywaclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2035 2023-04-07 16:22:04.000000 pywaclient-1.3.3/pywaclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 16:22:04.000000 pywaclient-1.3.3/pywaclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-07 16:22:04.000000 pywaclient-1.3.3/pywaclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-07 16:22:04.000000 pywaclient-1.3.3/pywaclient.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-07 16:21:50.000000 pywaclient-1.3.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 16:22:04.000000 pywaclient-1.3.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      833 2023-04-07 16:21:50.000000 pywaclient-1.3.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:22:04.000000 pywaclient-1.3.3/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:22:04.000000 pywaclient-1.3.3/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)     1266 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/data/block.json
--rw-rw-rw-   0 root         (0) root         (0)     2469 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/data/form_schema.json
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/init_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_article_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1638 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_block_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3926 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_block_template_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_block_template_part_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1836 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_canvas_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1855 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_category_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_chronicle_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_history_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_image_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1295 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_manuscript_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_map_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_notebook_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2986 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_parse_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1820 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_rpg_system_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     4154 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_secret_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2556 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_subscriber_group_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_timeline_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_user_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_variable_collection_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1679 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_variable_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     4530 2023-04-07 16:21:50.000000 pywaclient-1.3.3/tests/test_world_endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:55:23.000000 pywaclient-1.3.4/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-20 14:55:07.000000 pywaclient-1.3.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-04-20 14:55:07.000000 pywaclient-1.3.4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-04-20 14:55:07.000000 pywaclient-1.3.4/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-04-20 14:55:23.000000 pywaclient-1.3.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1759 2023-04-20 14:55:07.000000 pywaclient-1.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:55:23.000000 pywaclient-1.3.4/pywaclient/
+-rw-rw-rw-   0 root         (0) root         (0)      605 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3560 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:55:23.000000 pywaclient-1.3.4/pywaclient/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)     7013 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/articles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2242 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/block_templates.py
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/canvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/categories.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/chronicles.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/histories.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/images.py
+-rw-rw-rw-   0 root         (0) root         (0)     6023 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/manuscripts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/map_marker_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/maps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3076 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/notebooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1048 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/rpg_system.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)      808 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/subscriber_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      794 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/timelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/users.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/variables.py
+-rw-rw-rw-   0 root         (0) root         (0)    14182 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/endpoints/worlds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:55:23.000000 pywaclient-1.3.4/pywaclient/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/exceptions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:55:23.000000 pywaclient-1.3.4/pywaclient/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6892 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/models/article.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/models/block.py
+-rw-rw-rw-   0 root         (0) root         (0)     3532 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/models/category.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/models/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/models/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     5558 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/models/manuscript.py
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/models/secret.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/models/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2023-04-20 14:55:07.000000 pywaclient-1.3.4/pywaclient/models/world.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:55:23.000000 pywaclient-1.3.4/pywaclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-04-20 14:55:23.000000 pywaclient-1.3.4/pywaclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-04-20 14:55:23.000000 pywaclient-1.3.4/pywaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 14:55:23.000000 pywaclient-1.3.4/pywaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-20 14:55:23.000000 pywaclient-1.3.4/pywaclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-20 14:55:23.000000 pywaclient-1.3.4/pywaclient.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-20 14:55:07.000000 pywaclient-1.3.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 14:55:23.000000 pywaclient-1.3.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      833 2023-04-20 14:55:07.000000 pywaclient-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:55:23.000000 pywaclient-1.3.4/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:55:23.000000 pywaclient-1.3.4/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/data/block.json
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/data/form_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/init_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_article_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_block_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3926 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_block_template_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_block_template_part_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_canvas_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1855 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_category_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_chronicle_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_history_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_image_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3772 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_manuscript_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_map_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_notebook_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_parse_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1820 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_rpg_system_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     4154 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_secret_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2556 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_subscriber_group_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_timeline_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_user_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_variable_collection_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_variable_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     4530 2023-04-20 14:55:07.000000 pywaclient-1.3.4/tests/test_world_endpoint.py
```

### Comparing `pywaclient-1.3.3/LICENCE` & `pywaclient-1.3.4/LICENCE`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/PKG-INFO` & `pywaclient-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaclient
-Version: 1.3.3
+Version: 1.3.4
 Summary: A small wrapper library around the World Anvil Aragorn API: https://www.worldanvil.com/api/aragorn/documentation.
 Home-page: https://gitlab.com/SoulLink/world-anvil-api-client
 Author: Jonas Waeber
 Author-email: jonaswaeber@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pywaclient-1.3.3/README.md` & `pywaclient-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/__init__.py` & `pywaclient-1.3.4/pywaclient/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/api.py` & `pywaclient-1.3.4/pywaclient/api.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/__init__.py` & `pywaclient-1.3.4/pywaclient/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/articles.py` & `pywaclient-1.3.4/pywaclient/endpoints/articles.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/block_templates.py` & `pywaclient-1.3.4/pywaclient/endpoints/block_templates.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/blocks.py` & `pywaclient-1.3.4/pywaclient/endpoints/blocks.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/canvas.py` & `pywaclient-1.3.4/pywaclient/endpoints/canvas.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/categories.py` & `pywaclient-1.3.4/pywaclient/endpoints/categories.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/chronicles.py` & `pywaclient-1.3.4/pywaclient/endpoints/chronicles.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/histories.py` & `pywaclient-1.3.4/pywaclient/endpoints/histories.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/images.py` & `pywaclient-1.3.4/pywaclient/endpoints/images.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/manuscripts.py` & `pywaclient-1.3.4/pywaclient/endpoints/manuscripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,19 +108,19 @@
 class ManuscriptCrudEndpoint(CrudEndpoint):
 
     def __init__(self, client: 'AragornApiClient'):
         super().__init__(client, 'manuscript')
         self.bookmark = ManuscriptBookmarkCrudEndpoint(client)
         self._path_bookmarks = f'{self.path}/manuscript_bookmarks'
         self.tag = ManuscriptTagCrudEndpoint(client)
-        self._path_tags = 'manuscript_tags'
+        self._path_tags = f'{self.path}/manuscript_tags'
         self.label = ManuscriptLabelCrudEndpoint(client)
-        self._path_labels = 'manuscript_labels'
+        self._path_labels = f'{self.path}/manuscript_labels'
         self.version = ManuscriptVersionCrudEndpoint(client)
-        self._path_versions = 'manuscript_versions'
+        self._path_versions = f'{self.path}/manuscript_versions'
 
     def bookmarks(self, identifier: str) -> Iterable[Dict[str, Any]]:
         """Retrieve an iterable of all the bookmarks on a manuscript.
 
         :param identifier:  Identifier of the manuscript.
         :return:            Iterable dictionary of the entities.
         """
```

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/map_marker_types.py` & `pywaclient-1.3.4/pywaclient/endpoints/map_marker_types.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/maps.py` & `pywaclient-1.3.4/pywaclient/endpoints/maps.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/notebooks.py` & `pywaclient-1.3.4/pywaclient/endpoints/notebooks.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/rpg_system.py` & `pywaclient-1.3.4/pywaclient/endpoints/rpg_system.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/secrets.py` & `pywaclient-1.3.4/pywaclient/endpoints/secrets.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/subscriber_groups.py` & `pywaclient-1.3.4/pywaclient/endpoints/subscriber_groups.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/timelines.py` & `pywaclient-1.3.4/pywaclient/endpoints/timelines.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/users.py` & `pywaclient-1.3.4/pywaclient/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/variables.py` & `pywaclient-1.3.4/pywaclient/endpoints/variables.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/endpoints/worlds.py` & `pywaclient-1.3.4/pywaclient/endpoints/worlds.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/exceptions/__init__.py` & `pywaclient-1.3.4/pywaclient/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/models/article.py` & `pywaclient-1.3.4/pywaclient/models/article.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/models/block.py` & `pywaclient-1.3.4/pywaclient/models/block.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/models/category.py` & `pywaclient-1.3.4/pywaclient/models/category.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/models/entity.py` & `pywaclient-1.3.4/pywaclient/models/entity.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/models/genre.py` & `pywaclient-1.3.4/pywaclient/models/genre.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/models/manuscript.py` & `pywaclient-1.3.4/pywaclient/models/manuscript.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/models/secret.py` & `pywaclient-1.3.4/pywaclient/models/secret.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/models/user.py` & `pywaclient-1.3.4/pywaclient/models/user.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient/models/world.py` & `pywaclient-1.3.4/pywaclient/models/world.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/pywaclient.egg-info/PKG-INFO` & `pywaclient-1.3.4/pywaclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaclient
-Version: 1.3.3
+Version: 1.3.4
 Summary: A small wrapper library around the World Anvil Aragorn API: https://www.worldanvil.com/api/aragorn/documentation.
 Home-page: https://gitlab.com/SoulLink/world-anvil-api-client
 Author: Jonas Waeber
 Author-email: jonaswaeber@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pywaclient-1.3.3/pywaclient.egg-info/SOURCES.txt` & `pywaclient-1.3.4/pywaclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/setup.py` & `pywaclient-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/data/block.json` & `pywaclient-1.3.4/tests/data/block.json`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/data/form_schema.json` & `pywaclient-1.3.4/tests/data/form_schema.json`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/init_client.py` & `pywaclient-1.3.4/tests/init_client.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_article_endpoint.py` & `pywaclient-1.3.4/tests/test_article_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_block_endpoint.py` & `pywaclient-1.3.4/tests/test_block_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_block_template_endpoint.py` & `pywaclient-1.3.4/tests/test_block_template_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_block_template_part_endpoint.py` & `pywaclient-1.3.4/tests/test_block_template_part_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_canvas_endpoint.py` & `pywaclient-1.3.4/tests/test_canvas_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_category_endpoint.py` & `pywaclient-1.3.4/tests/test_category_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_chronicle_endpoint.py` & `pywaclient-1.3.4/tests/test_chronicle_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_history_endpoint.py` & `pywaclient-1.3.4/tests/test_history_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_image_endpoint.py` & `pywaclient-1.3.4/tests/test_image_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_map_endpoint.py` & `pywaclient-1.3.4/tests/test_map_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_notebook_endpoint.py` & `pywaclient-1.3.4/tests/test_notebook_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_parse_response.py` & `pywaclient-1.3.4/tests/test_parse_response.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_rpg_system_endpoint.py` & `pywaclient-1.3.4/tests/test_rpg_system_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_secret_endpoint.py` & `pywaclient-1.3.4/tests/test_secret_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_subscriber_group_endpoint.py` & `pywaclient-1.3.4/tests/test_subscriber_group_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_timeline_endpoint.py` & `pywaclient-1.3.4/tests/test_timeline_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_user_endpoint.py` & `pywaclient-1.3.4/tests/test_user_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_variable_collection_endpoint.py` & `pywaclient-1.3.4/tests/test_variable_collection_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_variable_endpoint.py` & `pywaclient-1.3.4/tests/test_variable_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.3/tests/test_world_endpoint.py` & `pywaclient-1.3.4/tests/test_world_endpoint.py`

 * *Files identical despite different names*

