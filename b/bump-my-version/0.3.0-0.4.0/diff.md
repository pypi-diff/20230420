# Comparing `tmp/bump-my-version-0.3.0.tar.gz` & `tmp/bump-my-version-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bump-my-version-0.3.0.tar", last modified: Mon Apr 17 13:59:51 2023, max compression
+gzip compressed data, was "bump-my-version-0.4.0.tar", last modified: Thu Apr 20 19:42:48 2023, max compression
```

## Comparing `bump-my-version-0.3.0.tar` & `bump-my-version-0.4.0.tar`

### file list

```diff
@@ -1,69 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.689983 bump-my-version-0.3.0/bump_my_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-17 13:59:51.000000 bump-my-version-0.3.0/bump_my_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-17 13:59:51.000000 bump-my-version-0.3.0/bump_my_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:59:51.000000 bump-my-version-0.3.0/bump_my_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 13:59:51.000000 bump-my-version-0.3.0/bump_my_version.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:59:51.000000 bump-my-version-0.3.0/bump_my_version.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-17 13:59:51.000000 bump-my-version-0.3.0/bump_my_version.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 13:59:51.000000 bump-my-version-0.3.0/bump_my_version.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.689983 bump-my-version-0.3.0/bumpversion/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/bumpversion/version_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/prod.in
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/prod.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/basic_cfg.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/basic_cfg.toml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/basic_cfg_expected.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/tests/fixtures/glob/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/tests/fixtures/glob/directory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/glob/directory/file3.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/glob/file1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/glob/file2.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/glob/not-text.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:59:51.693983 bump-my-version-0.3.0/tests/fixtures/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/interpolation/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/interpolation/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/fixtures/interpolation/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-04-17 13:59:32.000000 bump-my-version-0.3.0/tests/test_version_part.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.114294 bump-my-version-0.4.0/bump_my_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-20 19:42:48.000000 bump-my-version-0.4.0/bump_my_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-20 19:42:48.000000 bump-my-version-0.4.0/bump_my_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:42:48.000000 bump-my-version-0.4.0/bump_my_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 19:42:48.000000 bump-my-version-0.4.0/bump_my_version.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-20 19:42:48.000000 bump-my-version-0.4.0/bump_my_version.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-20 19:42:48.000000 bump-my-version-0.4.0/bump_my_version.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.114294 bump-my-version-0.4.0/bumpversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/version_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/basic_cfg.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/basic_cfg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/basic_cfg_expected.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/tests/fixtures/glob/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/tests/fixtures/glob/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/glob/directory/file3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/glob/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/glob/file2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/glob/not-text.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/tests/fixtures/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/interpolation/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/interpolation/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/interpolation/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_version_part.py
```

### Comparing `bump-my-version-0.3.0/CHANGELOG.md` & `bump-my-version-0.4.0/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,62 @@
 # Changelog
 
+## 0.4.0 (2023-04-20)
+[Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.3.0...0.4.0)
+
+### Fixes
+
+- Fixed pre-commit hook for dependency checking. [3d5c253](https://github.com/callowayproject/bump-my-version/commit/3d5c2533333112577c43cfe84d2091b1b60564b0)
+    
+- Fixed installing test dependencies. [c1034eb](https://github.com/callowayproject/bump-my-version/commit/c1034ebb0ae08ef140d8d36b345deb8c5f7b33dd)
+    
+- Fixed dependency spec. [4782745](https://github.com/callowayproject/bump-my-version/commit/47827452afa41906fb8cb108e4ab61e1b9aa908d)
+    
+- Fixed missing python in pypi test. [e5ed27d](https://github.com/callowayproject/bump-my-version/commit/e5ed27dee7850a011ac50a063ad055c1bed613d7)
+    
+- Fixed some CI issues. [d4b03d7](https://github.com/callowayproject/bump-my-version/commit/d4b03d7c0d8dacc4f8c726b208763071202e76c5)
+    
+- Fixed vague commit and tagging info. [4fb5158](https://github.com/callowayproject/bump-my-version/commit/4fb515851f3ddf78916c624db86c0b3e1869293b)
+    
+  - If commit is configured false, it will report that it will not commit
+
+  - If commit is configured false, tagging is disabled and it reports that
+
+  - If tagging is configured false, it will report it is not tagging
+- Fixes test package. [7c12072](https://github.com/callowayproject/bump-my-version/commit/7c12072b11938385ec81c5e9cd285d91ac1c00d7)
+    
+  - The build-and-inspect action didn't save the dist packages
+### New
+
+- Added tests for logging branches. [f8f0278](https://github.com/callowayproject/bump-my-version/commit/f8f027846349df4c66377c2cf4cc6903cd1f9bf7)
+    
+- Added path restrictions on release-hints. [e1af658](https://github.com/callowayproject/bump-my-version/commit/e1af65865e16f93441bb07e82800df469232b253)
+    
+- Added test build to CI. [8738f3f](https://github.com/callowayproject/bump-my-version/commit/8738f3f58b8c940ec44ecc8559192b75b45ccbac)
+    
+- Added doc files to table of contents. [49858c0](https://github.com/callowayproject/bump-my-version/commit/49858c0fef25f167f221e4c00070492f48f47070)
+    
+### Other
+
+- Completely migrated setuptools to use pyproject.toml. [f10f8b2](https://github.com/callowayproject/bump-my-version/commit/f10f8b25303c503753b33b434a344600c94409ee)
+    
+- [pre-commit.ci] pre-commit autoupdate. [d626f7d](https://github.com/callowayproject/bump-my-version/commit/d626f7d6240bfae07ab5a6795df222bdbf48d985)
+    
+  **updates:** - https://github.com/python/black → https://github.com/psf/black
+
+### Updates
+
+- Removed pre-commit dependency hook. [ac6cdd0](https://github.com/callowayproject/bump-my-version/commit/ac6cdd03e5260d319146ea0d93cc093496e79a19)
+    
+- Changed the version serialization. [c529452](https://github.com/callowayproject/bump-my-version/commit/c529452b043e8ab1b5711065c1ef96d73030978b)
+    
+  - can bump "dev" to get a development release
+- Updated formatting documentation. [8006f3e](https://github.com/callowayproject/bump-my-version/commit/8006f3efc749a2b8ad21fd365da4d29ebf81cc3b)
+    
+
 ## 0.3.0 (2023-04-17)
 [Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.2.0...0.3.0)
 
 ### Fixes
 
 - Fixed bug in SCMInfo setup. [e8fddc9](https://github.com/callowayproject/bump-my-version/commit/e8fddc99ec5f4632f097790ca6b851d8854e09bd)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bump-my-version-0.3.0/CODE_OF_CONDUCT.md` & `bump-my-version-0.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/CONTRIBUTING.md` & `bump-my-version-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/LICENSE` & `bump-my-version-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/PKG-INFO` & `bump-my-version-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.3.0
+Version: 0.4.0
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,14 +45,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: System :: Software Distribution
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 # Bump My Version
 
 [![image](https://img.shields.io/pypi/v/bump-my-version.svg)](https://pypi.org/project/bump-my-version/)
 [![image](https://img.shields.io/pypi/l/bump-my-version.svg)](https://pypi.org/project/bump-my-version/)
```

### Comparing `bump-my-version-0.3.0/README.md` & `bump-my-version-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/bump_my_version.egg-info/PKG-INFO` & `bump-my-version-0.4.0/bump_my_version.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.3.0
+Version: 0.4.0
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,14 +45,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: System :: Software Distribution
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 # Bump My Version
 
 [![image](https://img.shields.io/pypi/v/bump-my-version.svg)](https://pypi.org/project/bump-my-version/)
 [![image](https://img.shields.io/pypi/l/bump-my-version.svg)](https://pypi.org/project/bump-my-version/)
```

### Comparing `bump-my-version-0.3.0/bump_my_version.egg-info/SOURCES.txt` & `bump-my-version-0.4.0/bump_my_version.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-requirements.txt
 setup.cfg
 setup.py
 bump_my_version.egg-info/PKG-INFO
 bump_my_version.egg-info/SOURCES.txt
 bump_my_version.egg-info/dependency_links.txt
 bump_my_version.egg-info/entry_points.txt
-bump_my_version.egg-info/not-zip-safe
 bump_my_version.egg-info/requires.txt
 bump_my_version.egg-info/top_level.txt
 bumpversion/__init__.py
 bumpversion/__main__.py
 bumpversion/aliases.py
 bumpversion/autocast.py
 bumpversion/bump.py
@@ -25,22 +23,14 @@
 bumpversion/exceptions.py
 bumpversion/files.py
 bumpversion/functions.py
 bumpversion/logging.py
 bumpversion/scm.py
 bumpversion/utils.py
 bumpversion/version_part.py
-requirements/dev.in
-requirements/dev.txt
-requirements/docs.in
-requirements/docs.txt
-requirements/prod.in
-requirements/prod.txt
-requirements/test.in
-requirements/test.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_autocast.py
 tests/test_bump.py
 tests/test_cli.py
 tests/test_config.py
 tests/test_files.py
```

### Comparing `bump-my-version-0.3.0/bumpversion/aliases.py` & `bump-my-version-0.4.0/bumpversion/aliases.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/bumpversion/autocast.py` & `bump-my-version-0.4.0/bumpversion/autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/bumpversion/bump.py` & `bump-my-version-0.4.0/bumpversion/bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/bumpversion/cli.py` & `bump-my-version-0.4.0/bumpversion/cli.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/bumpversion/config.py` & `bump-my-version-0.4.0/bumpversion/config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/bumpversion/exceptions.py` & `bump-my-version-0.4.0/bumpversion/exceptions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/bumpversion/files.py` & `bump-my-version-0.4.0/bumpversion/files.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/bumpversion/functions.py` & `bump-my-version-0.4.0/bumpversion/functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/bumpversion/logging.py` & `bump-my-version-0.4.0/bumpversion/logging.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/bumpversion/scm.py` & `bump-my-version-0.4.0/bumpversion/scm.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         env = os.environ.copy()
         env["HGENCODING"] = "utf-8"
         env["BUMPVERSION_CURRENT_VERSION"] = current_version
         env["BUMPVERSION_NEW_VERSION"] = new_version
 
         try:
             subprocess.run([*cls._COMMIT_COMMAND, f.name, *extra_args], env=env, capture_output=True, check=True)
-        except subprocess.CalledProcessError as exc:
+        except subprocess.CalledProcessError as exc:  # pragma: no-coverage
             err_msg = f"Failed to run {exc.cmd}: return code {exc.returncode}, output: {exc.output}"
             logger.exception(err_msg)
             raise exc
         finally:
             os.unlink(f.name)
 
     @classmethod
@@ -102,15 +102,21 @@
         context: MutableMapping,
         extra_args: Optional[List[str]] = None,
         dry_run: bool = False,
     ) -> None:
         """Commit the files to the source code management system."""
         if not cls.is_usable():
             logger.error("SCM tool '%s' is unusable, unable to commit.", cls.__name__)
-        do_commit = config.commit and not dry_run
+            return
+
+        if not config.commit:
+            logger.info("Would not commit")
+            return
+
+        do_commit = not dry_run
         logger.info(
             "%s %s commit",
             "Preparing" if do_commit else "Would prepare",
             cls.__name__,
         )
         for path in files:
             logger.info(
@@ -142,17 +148,24 @@
     @classmethod
     def tag_in_scm(cls, config: "Config", context: MutableMapping, dry_run: bool = False) -> None:
         """Tag the current commit in the source code management system."""
         sign_tags = config.sign_tags
         tag_name = config.tag_name.format(**context)
         tag_message = config.tag_message.format(**context)
         existing_tags = cls.get_all_tags()
-        do_tag = config.tag and not dry_run
+        if not config.commit:
+            logger.info("Would not tag since we are not committing")
+            return
+        if not config.tag:
+            logger.info("Would not tag")
+            return
+
+        do_tag = not dry_run
 
-        if tag_name in existing_tags and config.tag:
+        if tag_name in existing_tags:
             logger.warning("Tag '%s' already exists. Will not tag.", tag_name)
             return
 
         logger.info(
             "%s '%s' %s in %s and %s",
             "Tagging" if do_tag else "Would tag",
             tag_name,
```

### Comparing `bump-my-version-0.3.0/bumpversion/utils.py` & `bump-my-version-0.4.0/bumpversion/utils.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/bumpversion/version_part.py` & `bump-my-version-0.4.0/bumpversion/version_part.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/pyproject.toml` & `bump-my-version-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -32,23 +32,58 @@
     "Topic :: System :: Software Distribution",
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["bumpversion", "version", "release"]
 dynamic = ["version"]
+dependencies = [
+    "click",
+    "pydantic",
+    "rich-click",
+    "rich",
+    "tomlkit",
+]
 
 [project.urls]
 homepage = "https://github.com/callowayproject/bump-my-version"
 repository = "https://github.com/callowayproject/bump-my-version.git"
 documentation = "https://callowayproject.github.io/bump-my-version/"
 
+[project.optional-dependencies]
+dev = [
+    "git-fame>=1.12.2",
+    "generate-changelog>=0.7.6",
+    "pip-tools",
+    "pre-commit",
+]
+docs = [
+    "ghp-import",
+    "linkify-it-py",
+    "myst-parser",
+    "furo",
+    "Sphinx>=4.3.0",
+    "sphinx-autodoc-typehints",
+    "sphinx-click",
+    "sphinx-copybutton",
+]
+test = [
+    "coverage",
+    "pre-commit",
+    "pytest-cov",
+    "pytest",
+    "pytest-mock",
+]
+
 [tool.setuptools.dynamic]
 version = {attr = "bumpversion.__version__"}
 
+[tool.setuptools.packages.find]
+exclude = ["example*", "tests*", "docs*", "build"]
+
 [tool.coverage.run]
 branch = true
 omit = ["**/test_*.py", "**/__main__.py", "**/aliases.py"]
 
 [tool.coverage.report]
 omit = [
     "*site-packages*",
@@ -166,27 +201,30 @@
 [tool.ruff.isort]
 order-by-type = true
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.bumpversion]
-current_version = "0.3.0"
+current_version = "0.4.0"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "{new_version}"
 allow_dirty = true
-parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.dev(?P<dev>\\d+))?"
+parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.(?P<dev>dev\\d+))?"
 serialize = [
-    "{major}.{minor}.{patch}.dev{dev}",
+    "{major}.{minor}.{patch}.{dev}{distance_to_latest_tag}",
     "{major}.{minor}.{patch}"
 ]
 message = "Version updated from {current_version} to {new_version}"
 
+[tool.bumpversion.parts.dev]
+values = ["release", "dev"]
+
 [[tool.bumpversion.files]]
 filename = "bumpversion/__init__.py"
 
 [[tool.bumpversion.files]]
 filename = "CHANGELOG.md"
 search = "Unreleased"
```

### Comparing `bump-my-version-0.3.0/tests/conftest.py` & `bump-my-version-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/tests/fixtures/basic_cfg.cfg` & `bump-my-version-0.4.0/tests/fixtures/basic_cfg.cfg`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/tests/fixtures/basic_cfg.toml` & `bump-my-version-0.4.0/tests/fixtures/basic_cfg.toml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/tests/fixtures/basic_cfg_expected.json` & `bump-my-version-0.4.0/tests/fixtures/basic_cfg_expected.json`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/tests/test_autocast.py` & `bump-my-version-0.4.0/tests/test_autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/tests/test_bump.py` & `bump-my-version-0.4.0/tests/test_bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/tests/test_cli.py` & `bump-my-version-0.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/tests/test_config.py` & `bump-my-version-0.4.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/tests/test_files.py` & `bump-my-version-0.4.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/tests/test_functions.py` & `bump-my-version-0.4.0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.3.0/tests/test_scm.py` & `bump-my-version-0.4.0/tests/test_scm.py`

 * *Files 22% similar despite different names*

```diff
@@ -139,7 +139,71 @@
         # Assert
         tag_info = scm_class.latest_tag_info("v*")
         if scm_command == "git":
             assert tag_info.commit_sha is not None
             assert tag_info.distance_to_latest_tag == 0
         assert tag_info.current_version == "30.1.0"
         assert tag_info.dirty is False
+
+
+# write tests for no-commit, no-tag and dry-run
+@pytest.mark.parametrize(
+    ["repo", "scm_command", "scm_class"],
+    [
+        param("git_repo", "git", scm.Git, id="git"),
+        param("hg_repo", "hg", scm.Mercurial, id="hg"),
+    ],
+)
+@pytest.mark.parametrize(
+    ["commit", "tag", "dry_run", "should_commit", "should_tag"],
+    [
+        param(True, True, True, False, False, id="dry-run-stops-commit-and-tag"),
+        param(True, False, False, True, False, id="commit-no-tag"),
+        param(False, True, False, False, False, id="no-commit-stops-tag"),
+    ],
+)
+def test_commit_tag_dry_run_interactions(
+    repo: str,
+    scm_command: str,
+    scm_class: scm.SourceCodeManager,
+    commit: bool,
+    tag: bool,
+    dry_run: bool,
+    should_commit: bool,
+    should_tag: bool,
+    caplog: LogCaptureFixture,
+    request,
+):
+    """Combinations of commit, tag, dry-run and should produce the expected results."""
+    # Arrange
+    repo_path: Path = request.getfixturevalue(repo)
+    version_path = repo_path / "VERSION"
+    version_path.write_text("30.0.3")
+
+    overrides = {"current_version": "30.0.3", "commit": commit, "tag": tag, "files": [{"filename": str(version_path)}]}
+    context = {
+        "current_version": "30.0.3",
+        "new_version": "30.1.0",
+    }
+    with inside_dir(repo_path):
+        conf, version_config, current_version = get_config_data(overrides)
+        subprocess.run([scm_command, "add", "VERSION"], check=True, capture_output=True)
+        subprocess.run([scm_command, "commit", "-m", "initial commit"], check=True, capture_output=True)
+        version_path.write_text("30.1.0")
+        # Act
+        scm_class.commit_to_scm(files=[version_path], config=conf, context=context, dry_run=dry_run)
+        scm_class.tag_in_scm(config=conf, context=context, dry_run=dry_run)
+
+        # Assert
+        if commit and dry_run:
+            assert "Would commit" in caplog.text
+        elif should_commit:
+            assert "Committing " in caplog.text
+        else:
+            assert "Would not commit" in caplog.text
+
+        if tag and dry_run:
+            assert "Would tag" in caplog.text
+        elif should_tag:
+            assert "Tagging " in caplog.text
+        else:
+            assert "Would not tag" in caplog.text
```

### Comparing `bump-my-version-0.3.0/tests/test_version_part.py` & `bump-my-version-0.4.0/tests/test_version_part.py`

 * *Files identical despite different names*

