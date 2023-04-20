# Comparing `tmp/invenio-theme-tugraz-4.10.1.tar.gz` & `tmp/invenio-theme-tugraz-4.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-theme-tugraz-4.10.1.tar", last modified: Thu Nov 10 08:22:51 2022, max compression
+gzip compressed data, was "dist/invenio-theme-tugraz-4.11.0.tar", last modified: Thu Apr 20 20:10:30 2023, max compression
```

## Comparing `invenio-theme-tugraz-4.10.1.tar` & `invenio-theme-tugraz-4.11.0.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/.tx/
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/.tx/config
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3082 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3584 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7212 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7465 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10405 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7009 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/footer.scss
--rw-r--r--   0 runner    (1001) docker     (121)     3099 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/header.scss
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/overrides.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/footer.scss
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/theme.scss
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/variables.scss
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/theme.scss
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/communities.less
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/deposit.less
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/
--rw-r--r--   0 runner    (1001) docker     (121)     4513 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (121)    94816 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   269108 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less
--rw-r--r--   0 runner    (1001) docker     (121)     1884 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less
--rw-r--r--   0 runner    (1001) docker     (121)     4594 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/login.less
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/macros.less
--rw-r--r--   0 runner    (1001) docker     (121)     3021 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/record.less
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/search.less
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less
--rw-r--r--   0 runner    (1001) docker     (121)     3202 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/ext.py
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/search.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/extra/
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/extra/orcid.png
--rw-r--r--   0 runner    (1001) docker     (121)     2550 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)    18533 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/Icon_1_v2.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4154 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/TU_Austria_Logo.png
--rw-r--r--   0 runner    (1001) docker     (121)   225210 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/footer.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     3117 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/icon_use.png
--rw-r--r--   0 runner    (1001) docker     (121)    18643 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/inveniordm-tail.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/library_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    23820 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/login_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    97455 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)    16480 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/oea.svg
--rw-r--r--   0 runner    (1001) docker     (121)    38212 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/re3data.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6438 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/tug_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/
--rw-r--r--   0 runner    (1001) docker     (121)     4316 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html
--rw-r--r--   0 runner    (1001) docker     (121)     3814 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html
--rw-r--r--   0 runner    (1001) docker     (121)     3870 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html
--rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/comingsoon.html
--rw-r--r--   0 runner    (1001) docker     (121)     5581 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html
--rw-r--r--   0 runner    (1001) docker     (121)     4480 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html
--rw-r--r--   0 runner    (1001) docker     (121)     6530 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/translations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/translations/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     6979 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)    15973 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (121)    12215 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/views.py
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7212 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4759 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/invenio_theme_tugraz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      660 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 08:22:51.000000 invenio-theme-tugraz-4.10.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-11-10 08:22:42.000000 invenio-theme-tugraz-4.10.1/tests/test_invenio_theme_tugraz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/overrides.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/communities.less
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/deposit.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    94816 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   269108 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/login.less
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/macros.less
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/record.less
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/search.less
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/extra/orcid.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/Icon_1_v2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/TU_Austria_Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   225210 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/footer.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/icon_use.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/inveniordm-tail.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/library_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23820 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/login_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97455 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/oea.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    38212 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/re3data.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/tug_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/comingsoon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/translations/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-04-20 20:10:29.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-04-20 20:10:29.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:10:29.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-20 20:10:29.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:10:29.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 20:10:29.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 20:10:29.000000 invenio-theme-tugraz-4.11.0/invenio_theme_tugraz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:10:30.000000 invenio-theme-tugraz-4.11.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-20 20:10:17.000000 invenio-theme-tugraz-4.11.0/tests/test_invenio_theme_tugraz.py
```

### Comparing `invenio-theme-tugraz-4.10.1/.editorconfig` & `invenio-theme-tugraz-4.11.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/.github/workflows/pypi-publish.yml` & `invenio-theme-tugraz-4.11.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/.github/workflows/tests.yml` & `invenio-theme-tugraz-4.11.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/.tx/config` & `invenio-theme-tugraz-4.11.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/CHANGES.rst` & `invenio-theme-tugraz-4.11.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,19 @@
     invenio-theme-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v4.11.0 (release 2023-04-20)
+
+- global: make dependencies compatible with v11
+
+
 Version v4.10.1 (release 2022-11-10)
 
 - dep: bump in invenio-assets
 
 
 Version v4.10.0 (release 2022-10-13)
```

### Comparing `invenio-theme-tugraz-4.10.1/CONTRIBUTING.rst` & `invenio-theme-tugraz-4.11.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/LICENSE` & `invenio-theme-tugraz-4.11.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/MANIFEST.in` & `invenio-theme-tugraz-4.11.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/PKG-INFO` & `invenio-theme-tugraz-4.11.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme-tugraz
-Version: 4.10.1
+Version: 4.11.0
 Summary: "Invenio module for TUGRAZ theme."
 Home-page: https://github.com/tu-graz-library/invenio-theme-tugraz
 Author: "Graz University of Technology"
 Author-email: mojib.wali@tugraz.at
 License: MIT
 Description: ..
             Copyright (C) 2020-2021 Graz University of Technology.
@@ -58,14 +58,19 @@
             invenio-theme-tugraz is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version v4.11.0 (release 2023-04-20)
+        
+        - global: make dependencies compatible with v11
+        
+        
         Version v4.10.1 (release 2022-11-10)
         
         - dep: bump in invenio-assets
         
         
         Version v4.10.0 (release 2022-10-13)
```

### Comparing `invenio-theme-tugraz-4.10.1/README.rst` & `invenio-theme-tugraz-4.11.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/docs/Makefile` & `invenio-theme-tugraz-4.11.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/docs/conf.py` & `invenio-theme-tugraz-4.11.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/docs/index.rst` & `invenio-theme-tugraz-4.11.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/docs/make.bat` & `invenio-theme-tugraz-4.11.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/footer.scss` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/footer.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/header.scss` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/header.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/overrides.scss` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/overrides.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/footer.scss` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/footer.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/search.less` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/search.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/config.py` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/config.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/ext.py` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/search.py` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/search.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/extra/orcid.png` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/extra/orcid.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/favicon.ico` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/Icon_1_v2.svg` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/Icon_1_v2.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/TU_Austria_Logo.png` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/TU_Austria_Logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/footer.jpg` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/footer.jpg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/icon_use.png` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/icon_use.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/inveniordm-tail.svg` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/inveniordm-tail.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/library_logo.png` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/library_logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/login_logo.png` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/login_logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/logo.svg` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/oea.svg` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/oea.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/re3data.svg` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/re3data.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/static/images/tug_logo.png` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/static/images/tug_logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: \n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid ""
 "\n"
 "                  Uploaded on %(date)s\n"
 "                  "
 msgstr ""
 "\n"
```

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/translations/messages.pot` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/views.py` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/views.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz/webpack.py` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz.egg-info/PKG-INFO` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme-tugraz
-Version: 4.10.1
+Version: 4.11.0
 Summary: "Invenio module for TUGRAZ theme."
 Home-page: https://github.com/tu-graz-library/invenio-theme-tugraz
 Author: "Graz University of Technology"
 Author-email: mojib.wali@tugraz.at
 License: MIT
 Description: ..
             Copyright (C) 2020-2021 Graz University of Technology.
@@ -58,14 +58,19 @@
             invenio-theme-tugraz is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version v4.11.0 (release 2023-04-20)
+        
+        - global: make dependencies compatible with v11
+        
+        
         Version v4.10.1 (release 2022-11-10)
         
         - dep: bump in invenio-assets
         
         
         Version v4.10.0 (release 2022-10-13)
```

### Comparing `invenio-theme-tugraz-4.10.1/invenio_theme_tugraz.egg-info/SOURCES.txt` & `invenio-theme-tugraz-4.11.0/invenio_theme_tugraz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/requirements-devel.txt` & `invenio-theme-tugraz-4.11.0/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/run-tests.sh` & `invenio-theme-tugraz-4.11.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/setup.cfg` & `invenio-theme-tugraz-4.11.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -24,26 +24,25 @@
 
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.8
 zip_safe = False
 install_requires = 
-	Flask-BabelEx>=0.9.4
-	Flask-WebpackExt>=1.0.0
-	invenio-assets>=1.3.0,<1.4.0
+	flask-babel>=2,<3
+	invenio-assets>=2.0.0,<3.0.0
 	invenio-i18n>=1.3.1,<1.4.0
 	invenio_config_tugraz>=0.10.0,<0.11.0
 
 [options.extras_require]
 tests = 
-	pytest-black>=0.3.0,<0.3.10
+	pytest-black>=0.3.0
 	Sphinx>=4.5.0
-	pytest-invenio>=1.4.7
-	invenio-app>=1.3.0,<2.0.0
+	pytest-invenio>=2.1.0,<3.0.0
+	invenio-app>=1.3.4,<1.4.0
 opensearch2 = 
 	invenio-search[opensearch2]>=2.1.0,<3.0.0
 
 [options.entry_points]
 invenio_base.apps = 
 	invenio_theme_tugraz = invenio_theme_tugraz:InvenioThemeTugraz
 invenio_base.blueprints =
```

### Comparing `invenio-theme-tugraz-4.10.1/tests/conftest.py` & `invenio-theme-tugraz-4.11.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.10.1/tests/test_invenio_theme_tugraz.py` & `invenio-theme-tugraz-4.11.0/tests/test_invenio_theme_tugraz.py`

 * *Files identical despite different names*

