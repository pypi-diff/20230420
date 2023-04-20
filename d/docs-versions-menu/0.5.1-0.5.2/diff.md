# Comparing `tmp/docs_versions_menu-0.5.1.tar.gz` & `tmp/docs_versions_menu-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docs_versions_menu-0.5.1.tar", last modified: Wed Jan 25 18:44:16 2023, max compression
+gzip compressed data, was "docs_versions_menu-0.5.2.tar", last modified: Thu Apr 20 03:41:35 2023, max compression
```

## Comparing `docs_versions_menu-0.5.1.tar` & `docs_versions_menu-0.5.2.tar`

### file list

```diff
@@ -1,198 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.615817 docs_versions_menu-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (122)      992 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10434 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7980 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      317 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    17274 2023-01-25 18:44:16.615817 docs_versions_menu-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7967 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.603817 docs_versions_menu-0.5.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.603817 docs_versions_menu-0.5.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)    97321 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/_static/docs-versions-menu-screenshot.png
--rw-r--r--   0 runner    (1001) docker     (122)   118716 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/_static/doctr-versions-menu-screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.603817 docs_versions_menu-0.5.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2587 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/_templates/package.rst
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6536 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7739 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/deployment.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6678 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/folderspecs.rst
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7552 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/options.rst
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4872 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/related_software.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4445 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/sphinx_extension.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/templates.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/docs/versions_json.rst
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-01-25 18:44:16.615817 docs_versions_menu-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3111 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.603817 docs_versions_menu-0.5.1/src/
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.603817 docs_versions_menu-0.5.1/src/docs_versions_menu/
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.603817 docs_versions_menu-0.5.1/src/docs_versions_menu/_css/
--rw-r--r--   0 runner    (1001) docker     (122)     4428 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/_css/badge_only.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/src/docs_versions_menu/_fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   165742 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/_fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (122)   444379 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/_fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (122)   165548 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/_fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (122)    98024 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/_fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (122)    77160 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/_fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/src/docs_versions_menu/_script/
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/_script/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/src/docs_versions_menu/_template/
--rw-r--r--   0 runner    (1001) docker     (122)     6150 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/_template/docs-versions-menu.js_t
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/_template/index.html_t
--rw-r--r--   0 runner    (1001) docker     (122)    12384 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2939 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     6806 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/folder_spec.py
--rw-r--r--   0 runner    (1001) docker     (122)     3185 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/groups.py
--rw-r--r--   0 runner    (1001) docker     (122)     5647 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/src/docs_versions_menu/version_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.603817 docs_versions_menu-0.5.1/src/docs_versions_menu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    17274 2023-01-25 18:44:16.000000 docs_versions_menu-0.5.1/src/docs_versions_menu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5171 2023-01-25 18:44:16.000000 docs_versions_menu-0.5.1/src/docs_versions_menu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-25 18:44:16.000000 docs_versions_menu-0.5.1/src/docs_versions_menu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-01-25 18:44:16.000000 docs_versions_menu-0.5.1/src/docs_versions_menu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-25 18:44:16.000000 docs_versions_menu-0.5.1/src/docs_versions_menu.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-01-25 18:44:16.000000 docs_versions_menu-0.5.1/src/docs_versions_menu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-01-25 18:44:16.000000 docs_versions_menu-0.5.1/src/docs_versions_menu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.599817 docs_versions_menu-0.5.1/tests/test_cli/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.595817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_downloads/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_downloads/master/
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_downloads/master/downloads.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_downloads/v0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_downloads/v0.1.0/downloads.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_downloads/v1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_downloads/v1.0.0/downloads.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_index/
--rw-r--r--   0 runner    (1001) docker     (122)      466 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_index/index.html_t
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_index/master/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_index/master/index.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_index/v0.1.0-rc1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_index/v0.1.0-rc1/index.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.595817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/doc-testing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/doc-testing/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/master/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/master/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/testing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/testing/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v0.1.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v0.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v0.2.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0+dev/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0+dev/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0-dev0/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0-dev0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0-post1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0-post1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0-rc1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0-rc1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v1.1.0-rc1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_labels_warnings/v1.1.0-rc1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.599817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_suffix/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_suffix/master/
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_suffix/master/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_suffix/v0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_suffix/v0.1.0/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_suffix/v1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_custom_suffix/v1.0.0/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.599817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_default/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.607817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_default/main/
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_default/main/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_default/v0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_default/v0.1.0/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_default/v1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_default/v1.0.0/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.599817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/doc-testing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/doc-testing/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/master/
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/master/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/testing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/testing/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v0.1.0/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v0.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v0.2.0/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v1.0.0/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v1.0.0+dev/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v1.0.0+dev/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v1.0.0-dev0/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v1.0.0-dev0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v1.0.0-post1/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v1.0.0-post1/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v1.0.0-rc1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v1.0.0-rc1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v1.1.0-rc1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_envvars/v1.1.0-rc1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.599817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/doc-testing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/doc-testing/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/master/
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/master/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/testing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/testing/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v0.1.0/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v0.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v0.2.0/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v1.0.0/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v1.0.0+dev/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v1.0.0+dev/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v1.0.0-dev0/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v1.0.0-dev0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v1.0.0-post1/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v1.0.0-post1/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v1.0.0-rc1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v1.0.0-rc1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v1.1.0-rc1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_many_releases/v1.1.0-rc1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.599817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_default_branch/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_default_branch/mybranch/
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_default_branch/mybranch/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.599817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_default_branch_release/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_default_branch_release/mybranch/
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_default_branch_release/mybranch/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_default_branch_release/v1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_default_branch_release/v1.0.0/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_downloads/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_downloads/doctr-versions-menu.conf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_downloads/master/
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_downloads/master/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_downloads/v0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_downloads/v0.1.0/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_downloads/v1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_downloads/v1.0.0/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.599817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_release/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_release/master/
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_release/master/_downloads
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_release/v1.0.0-rc1/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli/gh_pages_no_release/v1.0.0-rc1/_downloads
--rw-r--r--   0 runner    (1001) docker     (122)    25945 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_docs_versions_menu.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.599817 docs_versions_menu-0.5.1/tests/test_extension/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.599817 docs_versions_menu-0.5.1/tests/test_extension/roots/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_extension/roots/test-basic/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_extension/roots/test-basic/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_extension/roots/test-basic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_extension/roots/test-custom/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_extension/roots/test-custom/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_extension/roots/test-custom/_templates/doctr-versions-menu.js_t
--rw-r--r--   0 runner    (1001) docker     (122)      551 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_extension/roots/test-custom/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_extension/roots/test-custom/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 18:44:16.611817 docs_versions_menu-0.5.1/tests/test_extension/roots/test-rtdtheme/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_extension/roots/test-rtdtheme/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_extension/roots/test-rtdtheme/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (122)     8325 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_folder_spec.py
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-01-25 18:44:04.000000 docs_versions_menu-0.5.1/tests/test_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      992 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10434 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8144 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      317 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    17438 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7967 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.175005 docs_versions_menu-0.5.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.175005 docs_versions_menu-0.5.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)    97321 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/_static/docs-versions-menu-screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (122)   118716 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/_static/doctr-versions-menu-screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.175005 docs_versions_menu-0.5.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2587 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/_templates/package.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6536 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7739 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6678 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/folderspecs.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7552 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/options.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4872 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/related_software.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4445 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/sphinx_extension.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/templates.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/docs/versions_json.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3111 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.175005 docs_versions_menu-0.5.2/src/
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.175005 docs_versions_menu-0.5.2/src/docs_versions_menu/
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.175005 docs_versions_menu-0.5.2/src/docs_versions_menu/_css/
+-rw-r--r--   0 runner    (1001) docker     (122)     4428 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/_css/badge_only.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/src/docs_versions_menu/_fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   165742 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/_fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   444379 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/_fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (122)   165548 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/_fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    98024 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/_fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    77160 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/_fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/src/docs_versions_menu/_script/
+-rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/_script/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/src/docs_versions_menu/_template/
+-rw-r--r--   0 runner    (1001) docker     (122)     6150 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/_template/docs-versions-menu.js_t
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/_template/index.html_t
+-rw-r--r--   0 runner    (1001) docker     (122)    12384 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2939 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6795 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/folder_spec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3159 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/parse_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5517 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/src/docs_versions_menu/version_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.175005 docs_versions_menu-0.5.2/src/docs_versions_menu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    17438 2023-04-20 03:41:35.000000 docs_versions_menu-0.5.2/src/docs_versions_menu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5239 2023-04-20 03:41:35.000000 docs_versions_menu-0.5.2/src/docs_versions_menu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 03:41:35.000000 docs_versions_menu-0.5.2/src/docs_versions_menu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-04-20 03:41:35.000000 docs_versions_menu-0.5.2/src/docs_versions_menu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 03:41:35.000000 docs_versions_menu-0.5.2/src/docs_versions_menu.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-20 03:41:35.000000 docs_versions_menu-0.5.2/src/docs_versions_menu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-20 03:41:35.000000 docs_versions_menu-0.5.2/src/docs_versions_menu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.171005 docs_versions_menu-0.5.2/tests/test_cli/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.167005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_downloads/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_downloads/master/
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_downloads/master/downloads.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_downloads/v0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_downloads/v0.1.0/downloads.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_downloads/v1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_downloads/v1.0.0/downloads.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_index/
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_index/index.html_t
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_index/master/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_index/master/index.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_index/v0.1.0-rc1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_index/v0.1.0-rc1/index.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.167005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/doc-testing/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/doc-testing/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/master/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/master/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/testing/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v0.1.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v0.2.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0+dev/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0+dev/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0-dev0/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0-dev0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0-post1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0-post1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0-rc1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v1.0.0-rc1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v1.1.0-rc1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_labels_warnings/v1.1.0-rc1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.171005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_suffix/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_suffix/master/
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_suffix/master/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_suffix/v0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_suffix/v0.1.0/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_suffix/v1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_custom_suffix/v1.0.0/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.171005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_default/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_default/main/
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_default/main/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_default/v0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_default/v0.1.0/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_default/v1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_default/v1.0.0/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.171005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/doc-testing/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/doc-testing/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/master/
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/master/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/testing/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v0.1.0/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v0.2.0/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v1.0.0/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v1.0.0+dev/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v1.0.0+dev/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.179005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v1.0.0-dev0/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v1.0.0-dev0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v1.0.0-post1/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v1.0.0-post1/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v1.0.0-rc1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v1.0.0-rc1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v1.1.0-rc1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_envvars/v1.1.0-rc1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.171005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/doc-testing/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/doc-testing/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/master/
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/master/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/testing/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v0.1.0/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v0.2.0/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v1.0.0/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v1.0.0+dev/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v1.0.0+dev/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v1.0.0-dev0/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v1.0.0-dev0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v1.0.0-post1/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v1.0.0-post1/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v1.0.0-rc1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v1.0.0-rc1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v1.1.0-rc1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_many_releases/v1.1.0-rc1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.171005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_default_branch/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_default_branch/mybranch/
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_default_branch/mybranch/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.171005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_default_branch_release/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_default_branch_release/mybranch/
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_default_branch_release/mybranch/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_default_branch_release/v1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_default_branch_release/v1.0.0/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_downloads/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_downloads/doctr-versions-menu.conf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_downloads/master/
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_downloads/master/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_downloads/v0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_downloads/v0.1.0/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_downloads/v1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_downloads/v1.0.0/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.171005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_release/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_release/master/
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_release/master/_downloads
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_release/v1.0.0-rc1/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli/gh_pages_no_release/v1.0.0-rc1/_downloads
+-rw-r--r--   0 runner    (1001) docker     (122)    25945 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_docs_versions_menu.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.171005 docs_versions_menu-0.5.2/tests/test_extension/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.171005 docs_versions_menu-0.5.2/tests/test_extension/roots/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_extension/roots/test-basic/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_extension/roots/test-basic/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_extension/roots/test-basic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_extension/roots/test-custom/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_extension/roots/test-custom/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_extension/roots/test-custom/_templates/doctr-versions-menu.js_t
+-rw-r--r--   0 runner    (1001) docker     (122)      551 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_extension/roots/test-custom/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_extension/roots/test-custom/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 03:41:35.183005 docs_versions_menu-0.5.2/tests/test_extension/roots/test-rtdtheme/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_extension/roots/test-rtdtheme/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_extension/roots/test-rtdtheme/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8325 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_folder_spec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-04-20 03:41:24.000000 docs_versions_menu-0.5.2/tests/test_parse_version.py
```

### Comparing `docs_versions_menu-0.5.1/AUTHORS.rst` & `docs_versions_menu-0.5.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/CONTRIBUTING.rst` & `docs_versions_menu-0.5.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/HISTORY.rst` & `docs_versions_menu-0.5.2/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =======
 History
 =======
 
+0.5.2 (2023-04-19)
+------------------
+
+* Compatibility with ``packaging >= 22.0`` (`#27`_, `#32`_)
+
+
 0.5.1 (2023-01-25)
 ------------------
 
 * Pin ``packaging`` dependency to ``< 22.0`` (`#27`_, `#28`_)
 
 
 0.5.0 (2022-11-17)
@@ -124,8 +130,9 @@
 .. _#9: https://github.com/goerz/docs_versions_menu/issues/9
 .. _#12: https://github.com/goerz/docs_versions_menu/issues/12
 .. _#13: https://github.com/goerz/docs_versions_menu/issues/13
 .. _#15: https://github.com/goerz/docs_versions_menu/issues/15
 .. _#18: https://github.com/goerz/docs_versions_menu/issues/18
 .. _#27: https://github.com/goerz/docs_versions_menu/issues/27
 .. _#28: https://github.com/goerz/docs_versions_menu/issues/28
+.. _#32: https://github.com/goerz/docs_versions_menu/issues/32
 .. _conda-feedstock: https://github.com/conda-forge/docs-versions-menu-feedstock#readme
```

### Comparing `docs_versions_menu-0.5.1/LICENSE` & `docs_versions_menu-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/PKG-INFO` & `docs_versions_menu-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs_versions_menu
-Version: 0.5.1
+Version: 0.5.2
 Summary: A versions menu for Sphinx-based documentation
 Home-page: https://github.com/goerz/docs_versions_menu
 Author: Michael Goerz
 Author-email: mail@michaelgoerz.net
 License: MIT license
 Keywords: Doctr,Sphinx,Github
 Classifier: Development Status :: 4 - Beta
@@ -191,14 +191,20 @@
 .. _workflow file: https://github.com/goerz/docs_versions_menu/blob/master/.github/workflows/docs.yml
 
 
 =======
 History
 =======
 
+0.5.2 (2023-04-19)
+------------------
+
+* Compatibility with ``packaging >= 22.0`` (`#27`_, `#32`_)
+
+
 0.5.1 (2023-01-25)
 ------------------
 
 * Pin ``packaging`` dependency to ``< 22.0`` (`#27`_, `#28`_)
 
 
 0.5.0 (2022-11-17)
@@ -317,8 +323,9 @@
 .. _#9: https://github.com/goerz/docs_versions_menu/issues/9
 .. _#12: https://github.com/goerz/docs_versions_menu/issues/12
 .. _#13: https://github.com/goerz/docs_versions_menu/issues/13
 .. _#15: https://github.com/goerz/docs_versions_menu/issues/15
 .. _#18: https://github.com/goerz/docs_versions_menu/issues/18
 .. _#27: https://github.com/goerz/docs_versions_menu/issues/27
 .. _#28: https://github.com/goerz/docs_versions_menu/issues/28
+.. _#32: https://github.com/goerz/docs_versions_menu/issues/32
 .. _conda-feedstock: https://github.com/conda-forge/docs-versions-menu-feedstock#readme
```

### Comparing `docs_versions_menu-0.5.1/README.rst` & `docs_versions_menu-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/docs/_static/docs-versions-menu-screenshot.png` & `docs_versions_menu-0.5.2/docs/_static/docs-versions-menu-screenshot.png`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/docs/_static/doctr-versions-menu-screenshot.png` & `docs_versions_menu-0.5.2/docs/_static/doctr-versions-menu-screenshot.png`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/docs/_templates/module.rst` & `docs_versions_menu-0.5.2/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/docs/_templates/package.rst` & `docs_versions_menu-0.5.2/docs/_templates/package.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/docs/conf.py` & `docs_versions_menu-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/docs/deployment.rst` & `docs_versions_menu-0.5.2/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/docs/folderspecs.rst` & `docs_versions_menu-0.5.2/docs/folderspecs.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/docs/options.rst` & `docs_versions_menu-0.5.2/docs/options.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/docs/related_software.rst` & `docs_versions_menu-0.5.2/docs/related_software.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/docs/sphinx_extension.rst` & `docs_versions_menu-0.5.2/docs/sphinx_extension.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/docs/templates.rst` & `docs_versions_menu-0.5.2/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/docs/versions_json.rst` & `docs_versions_menu-0.5.2/docs/versions_json.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/setup.cfg` & `docs_versions_menu-0.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/setup.py` & `docs_versions_menu-0.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 except OSError:
     history = ''
 
 # requirements for use
 requirements = [
     'click >= 6.7',
     'jinja2',
-    'packaging < 22.0',
+    'packaging',
     'pyparsing >= 2.0.2',
     'setuptools',
     'sphinx',
 ]
 
 # requirements for development (testing, generating docs)
 dev_requirements = [
-    'black',
+    'black < 23.0',
     'coverage',
     'coveralls',
     'flake8',
     'gitpython',
     'ipython',
     'isort',
     'pdbpp',
```

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu/__init__.py` & `docs_versions_menu-0.5.2/src/docs_versions_menu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Docs Versions Menu.
 
 This package does not define a public API: it publicly provides only a Sphinx
 extension and a command line program.
 """
 
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 
 # All members whose name does not start with an underscore must be listed
 # either in __all__ or in __private__
 __all__ = []
 __private__ = ['setup']
 
 from . import cli, ext
```

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu/_css/badge_only.css` & `docs_versions_menu-0.5.2/src/docs_versions_menu/_css/badge_only.css`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu/_fonts/fontawesome-webfont.eot` & `docs_versions_menu-0.5.2/src/docs_versions_menu/_fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu/_fonts/fontawesome-webfont.svg` & `docs_versions_menu-0.5.2/src/docs_versions_menu/_fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu/_fonts/fontawesome-webfont.ttf` & `docs_versions_menu-0.5.2/src/docs_versions_menu/_fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu/_fonts/fontawesome-webfont.woff` & `docs_versions_menu-0.5.2/src/docs_versions_menu/_fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu/_fonts/fontawesome-webfont.woff2` & `docs_versions_menu-0.5.2/src/docs_versions_menu/_fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu/_script/versions.py` & `docs_versions_menu-0.5.2/src/docs_versions_menu/_script/versions.py`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu/_template/docs-versions-menu.js_t` & `docs_versions_menu-0.5.2/src/docs_versions_menu/_template/docs-versions-menu.js_t`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu/cli.py` & `docs_versions_menu-0.5.2/src/docs_versions_menu/cli.py`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu/ext.py` & `docs_versions_menu-0.5.2/src/docs_versions_menu/ext.py`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu/folder_spec.py` & `docs_versions_menu-0.5.2/src/docs_versions_menu/folder_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Parser for folder specifications."""
 from collections import OrderedDict
 from functools import partial
 
-from packaging.version import parse as parse_version
 from pyparsing import (
     Forward,
     Group,
     Literal,
     Optional,
     ParseException,
     Word,
     ZeroOrMore,
     alphanums,
     delimitedList,
     nums,
     oneOf,
 )
 
+from .parse_version import parse_version
+
 
 def _parse_folder_spec(spec, groups, sort_key):
     """Parse the folder specification into a nested list.
 
     Args:
         spec (str): folder specification
         groups (dict): map of group name to list of folders in group
```

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu/groups.py` & `docs_versions_menu-0.5.2/src/docs_versions_menu/groups.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Classification of folders into groups according to :pep:`440`."""
-from packaging.version import LegacyVersion
-from packaging.version import parse as parse_version
+
+from .parse_version import NonVersionFolderName, parse_version
 
 
 def get_groups(folders, default_branches=None):
     """Sort the given folder names into groups.
 
     Args:
         folders (list[str]): List of folder names, corresponding to git branch
@@ -47,15 +47,15 @@
         'releases': set(),
         'default-branch': set(),
     }
     for folder in folders:
         version = parse_version(folder)
         if folder in default_branches:
             groups['default-branch'].add(folder)
-        if isinstance(version, LegacyVersion):
+        if isinstance(version, NonVersionFolderName):
             groups['branches'].add(folder)
         else:
             groups['releases'].add(folder)
             is_final = True
             if version.local is not None:
                 groups['local-releases'].add(folder)
                 is_final = False
```

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu/version_data.py` & `docs_versions_menu-0.5.2/src/docs_versions_menu/version_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 """Implementation of the versions-data collection."""
 import logging
 import re
 from pathlib import Path
 
 import jinja2
-from packaging.version import parse as parse_version
 
 from .folder_spec import resolve_folder_spec
 from .groups import get_groups
 
 
 def get_version_data(
     *,
-    sort_key=None,
     suffix_latest,
     default_branch_spec,
     versions_spec,
     latest_spec,
     warnings,
     label_specs,
     downloads_file=None
 ):
     """Get the versions data, to be serialized to json."""
     logger = logging.getLogger(__name__)
-    if sort_key is None:
-        sort_key = parse_version
 
     folders = sorted(
         [
             str(f)
             for f in Path().iterdir()
             if (
                 f.is_dir()
```

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu.egg-info/PKG-INFO` & `docs_versions_menu-0.5.2/src/docs_versions_menu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs-versions-menu
-Version: 0.5.1
+Version: 0.5.2
 Summary: A versions menu for Sphinx-based documentation
 Home-page: https://github.com/goerz/docs_versions_menu
 Author: Michael Goerz
 Author-email: mail@michaelgoerz.net
 License: MIT license
 Keywords: Doctr,Sphinx,Github
 Classifier: Development Status :: 4 - Beta
@@ -191,14 +191,20 @@
 .. _workflow file: https://github.com/goerz/docs_versions_menu/blob/master/.github/workflows/docs.yml
 
 
 =======
 History
 =======
 
+0.5.2 (2023-04-19)
+------------------
+
+* Compatibility with ``packaging >= 22.0`` (`#27`_, `#32`_)
+
+
 0.5.1 (2023-01-25)
 ------------------
 
 * Pin ``packaging`` dependency to ``< 22.0`` (`#27`_, `#28`_)
 
 
 0.5.0 (2022-11-17)
@@ -317,8 +323,9 @@
 .. _#9: https://github.com/goerz/docs_versions_menu/issues/9
 .. _#12: https://github.com/goerz/docs_versions_menu/issues/12
 .. _#13: https://github.com/goerz/docs_versions_menu/issues/13
 .. _#15: https://github.com/goerz/docs_versions_menu/issues/15
 .. _#18: https://github.com/goerz/docs_versions_menu/issues/18
 .. _#27: https://github.com/goerz/docs_versions_menu/issues/27
 .. _#28: https://github.com/goerz/docs_versions_menu/issues/28
+.. _#32: https://github.com/goerz/docs_versions_menu/issues/32
 .. _conda-feedstock: https://github.com/conda-forge/docs-versions-menu-feedstock#readme
```

### Comparing `docs_versions_menu-0.5.1/src/docs_versions_menu.egg-info/SOURCES.txt` & `docs_versions_menu-0.5.2/src/docs_versions_menu.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 docs/_templates/package.rst
 src/conftest.py
 src/docs_versions_menu/__init__.py
 src/docs_versions_menu/cli.py
 src/docs_versions_menu/ext.py
 src/docs_versions_menu/folder_spec.py
 src/docs_versions_menu/groups.py
+src/docs_versions_menu/parse_version.py
 src/docs_versions_menu/version_data.py
 src/docs_versions_menu.egg-info/PKG-INFO
 src/docs_versions_menu.egg-info/SOURCES.txt
 src/docs_versions_menu.egg-info/dependency_links.txt
 src/docs_versions_menu.egg-info/entry_points.txt
 src/docs_versions_menu.egg-info/not-zip-safe
 src/docs_versions_menu.egg-info/requires.txt
@@ -48,14 +49,15 @@
 src/docs_versions_menu/_template/index.html_t
 tests/conftest.py
 tests/test_cli.py
 tests/test_docs_versions_menu.py
 tests/test_extension.py
 tests/test_folder_spec.py
 tests/test_groups.py
+tests/test_parse_version.py
 tests/test_cli/gh_pages_custom_downloads/master/downloads.md
 tests/test_cli/gh_pages_custom_downloads/v0.1.0/downloads.md
 tests/test_cli/gh_pages_custom_downloads/v1.0.0/downloads.md
 tests/test_cli/gh_pages_custom_index/index.html_t
 tests/test_cli/gh_pages_custom_index/master/index.html
 tests/test_cli/gh_pages_custom_index/v0.1.0-rc1/index.html
 tests/test_cli/gh_pages_custom_labels_warnings/doc-testing/.gitignore
```

### Comparing `docs_versions_menu-0.5.1/tests/test_cli.py` & `docs_versions_menu-0.5.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/tests/test_extension/roots/test-basic/index.rst` & `docs_versions_menu-0.5.2/tests/test_extension/roots/test-basic/index.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/tests/test_extension/roots/test-custom/conf.py` & `docs_versions_menu-0.5.2/tests/test_extension/roots/test-custom/conf.py`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/tests/test_extension/roots/test-custom/index.rst` & `docs_versions_menu-0.5.2/tests/test_extension/roots/test-custom/index.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/tests/test_extension/roots/test-rtdtheme/index.rst` & `docs_versions_menu-0.5.2/tests/test_extension/roots/test-rtdtheme/index.rst`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/tests/test_extension.py` & `docs_versions_menu-0.5.2/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/tests/test_folder_spec.py` & `docs_versions_menu-0.5.2/tests/test_folder_spec.py`

 * *Files identical despite different names*

### Comparing `docs_versions_menu-0.5.1/tests/test_groups.py` & `docs_versions_menu-0.5.2/tests/test_groups.py`

 * *Files identical despite different names*

