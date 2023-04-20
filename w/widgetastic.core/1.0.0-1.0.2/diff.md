# Comparing `tmp/widgetastic.core-1.0.0.tar.gz` & `tmp/widgetastic.core-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widgetastic.core-1.0.0.tar", last modified: Fri Apr 29 10:09:30 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `widgetastic.core-1.0.0.tar` & `widgetastic.core-1.0.2.tar`

### file list

```diff
@@ -1,75 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 10:09:30.493071 widgetastic.core-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 10:09:30.485071 widgetastic.core-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 10:09:30.485071 widgetastic.core-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4011 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/.github/workflows/test_suite.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3029 2022-04-29 10:09:30.493071 widgetastic.core-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1961 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 10:09:30.485071 widgetastic.core-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    13021 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/docs/advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/docs/basic_usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     6847 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/docs/guidelines.rst
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8476 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/docs/internals.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3176 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1558 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/docs/ouia.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 10:09:30.489071 widgetastic.core-1.0.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/docs/source/widgetastic.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/docs/source/widgetastic.widget.rst
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-04-29 10:09:30.493071 widgetastic.core-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 10:09:30.485071 widgetastic.core-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 10:09:30.489071 widgetastic.core-1.0.0/src/widgetastic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    46123 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/browser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6379 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 10:09:30.489071 widgetastic.core-1.0.0/src/widgetastic/ouia/
--rw-r--r--   0 runner    (1001) docker     (121)     3750 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/ouia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/ouia/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/ouia/input.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/ouia/text.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/types.py
--rw-r--r--   0 runner    (1001) docker     (121)    26515 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 10:09:30.489071 widgetastic.core-1.0.0/src/widgetastic/widget/
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    48883 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/widget/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/widget/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/widget/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     3745 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/widget/input.py
--rw-r--r--   0 runner    (1001) docker     (121)    10250 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/widget/select.py
--rw-r--r--   0 runner    (1001) docker     (121)    49760 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/widget/table.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/widget/text.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/src/widgetastic/xpath.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 10:09:30.489071 widgetastic.core-1.0.0/src/widgetastic.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3029 2022-04-29 10:09:29.000000 widgetastic.core-1.0.0/src/widgetastic.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-04-29 10:09:30.000000 widgetastic.core-1.0.0/src/widgetastic.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-29 10:09:29.000000 widgetastic.core-1.0.0/src/widgetastic.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-04-29 10:09:30.000000 widgetastic.core-1.0.0/src/widgetastic.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-29 10:09:30.000000 widgetastic.core-1.0.0/src/widgetastic.core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 10:09:30.489071 widgetastic.core-1.0.0/testing/
--rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 10:09:30.493071 widgetastic.core-1.0.0/testing/html/
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/html/iframe_page.html
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/html/iframe_page2.html
--rw-r--r--   0 runner    (1001) docker     (121)     9759 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/html/testing_page.html
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/ouia_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)    35566 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/test_basic_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)    11028 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/test_fillable.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/test_log.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/test_ouia.py
--rw-r--r--   0 runner    (1001) docker     (121)     1722 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/test_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/test_version_pick.py
--rw-r--r--   0 runner    (1001) docker     (121)    22893 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/test_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/test_widget_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-04-29 10:09:17.000000 widgetastic.core-1.0.0/testing/test_xpath.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/pytest.ini
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.github/workflows/test_suite.yml
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/Activate.ps1
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/activate
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/activate.csh
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/activate.fish
+-rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/docutils
+-rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/keyring
+-rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/markdown-it
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/normalizer
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/pip
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/pip3
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/pip3.11
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/pkginfo
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/pygmentize
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/python -> /usr/bin/python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/rst2html.py
+-rwxr-xr-x   0        0        0      763 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/rst2html4.py
+-rwxr-xr-x   0        0        0     1108 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/rst2html5.py
+-rwxr-xr-x   0        0        0      840 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/rst2latex.py
+-rwxr-xr-x   0        0        0      663 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/rst2man.py
+-rwxr-xr-x   0        0        0      829 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/rst2odt.py
+-rwxr-xr-x   0        0        0     1767 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0        0        0      648 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0        0        0      684 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/rst2s5.py
+-rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/rst2xetex.py
+-rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/rst2xml.py
+-rwxr-xr-x   0        0        0      717 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/rstpep2html.py
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/twine
+-rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.venv/bin/wheel
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0    13021 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/docs/advanced_usage.rst
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/docs/basic_usage.rst
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/docs/conf.py
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/docs/guidelines.rst
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/docs/index.rst
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/docs/internals.rst
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/docs/intro.rst
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/docs/ouia.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/docs/source/modules.rst
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/docs/source/widgetastic.rst
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/docs/source/widgetastic.widget.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/__init__.py
+-rw-r--r--   0        0        0    46248 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/browser.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/exceptions.py
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/log.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/types.py
+-rw-r--r--   0        0        0    26515 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/utils.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/xpath.py
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/ouia/__init__.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/ouia/checkbox.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/ouia/input.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/ouia/text.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/widget/__init__.py
+-rw-r--r--   0        0        0    48883 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/widget/base.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/widget/checkbox.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/widget/image.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/widget/input.py
+-rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/widget/select.py
+-rw-r--r--   0        0        0    49871 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/widget/table.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/src/widgetastic/widget/text.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/conftest.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/ouia_widgets.py
+-rw-r--r--   0        0        0    35566 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/test_basic_widgets.py
+-rw-r--r--   0        0        0    11028 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/test_browser.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/test_fillable.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/test_log.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/test_ouia.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/test_table.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/test_utils.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/test_version.py
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/test_version_pick.py
+-rw-r--r--   0        0        0    22893 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/test_view.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/test_widget.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/test_widget_descriptor.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/test_xpath.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/html/iframe_page.html
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/html/iframe_page2.html
+-rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/testing/html/testing_page.html
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/.gitignore
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/README.rst
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 widgetastic_core-1.0.2/PKG-INFO
```

### Comparing `widgetastic.core-1.0.0/.github/workflows/deploy.yml` & `widgetastic_core-1.0.2/.github/workflows/deploy.yml`

 * *Files 17% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         uses: actions/setup-python@v2
         with:
           python-version: '3.8'
           architecture: 'x64'
 
       - name: Build Package and Check
         run: |
-          python -m pip install --upgrade setuptools wheel twine
-          python setup.py sdist bdist_wheel
-          python -m twine check dist/*
+          pip install -U wheel twine
+          pip wheel --no-deps -w dist .
+          twine check dist/*
 
       - name: Deploy to PyPi
         uses: pypa/gh-action-pypi-publish@v1.4.1
         with:
           user: __token__
           password: ${{ secrets.pypi_wt_core }}
```

### Comparing `widgetastic.core-1.0.0/.github/workflows/test_suite.yml` & `widgetastic_core-1.0.2/.github/workflows/test_suite.yml`

 * *Files 15% similar despite different names*

```diff
@@ -5,47 +5,27 @@
   pull_request:
     types: ["opened", "synchronize", "reopened"]
   schedule:
     # Run every Friday at 23:59 UTC
     - cron: 59 23 * * 5
 
 jobs:
-  codechecks:
-    name: 📃 Code quality [pre-commit]
-    runs-on: ubuntu-20.04
-
-    steps:
-      - name: Checkout
-        uses: actions/checkout@v3
-
-      - name: Setup Python
-        uses: actions/setup-python@v3
-        with:
-          python-version: "3.8"
-          architecture: "x64"
-
-      - name: Pre Commit Checks
-        uses: pre-commit/action@v2.0.0
-
-      - name: Analysis (git diff)
-        if: failure()
-        run: git diff
 
   tests:
     # Run unit tests on different version of python and browser
     name: 🐍 Python-${{ matrix.python-version }}-${{ matrix.browser }}
     runs-on: ubuntu-20.04
     strategy:
       matrix:
         browser: [chrome, firefox]
         python-version: ["3.8", "3.9", "3.10"]
 
     steps:
       - name: Pull selenium-standalone:latest
-        run: podman pull quay.io/redhatqe/selenium-standalone:ff_91.8.0esr_chrome_101.0.4951.41
+        run: podman pull quay.io/redhatqe/selenium-standalone:latest
 
       - name: Pull docker.io/library/nginx:alpine
         run: podman pull docker.io/library/nginx:alpine
 
       - name: Checkout
         uses: actions/checkout@v3
 
@@ -55,15 +35,14 @@
           python-version: ${{ matrix.python-version }}
 
       - name: UnitTest - Python-${{ matrix.python-version }}-${{ matrix.browser }}
         env:
           BROWSER: ${{ matrix.browser }}
           XDG_RUNTIME_DIR: ${{ github.workspace }}
         run: |
-          pip install -U setuptools wheel
           pip install -e .[test]
           mkdir -p ${XDG_RUNTIME_DIR}/podman
           podman system service --time=0 unix://${XDG_RUNTIME_DIR}/podman/podman.sock &
           pytest -n 3
 
       - name: Upload coverage to Codecov
         uses: codecov/codecov-action@v1.0.13
@@ -82,15 +61,15 @@
       - name: Setup Python
         uses: actions/setup-python@v3
         with:
           python-version: "3.8"
 
       - name: Install Deps
         run: |
-          pip install -U pip setuptools wheel
+          pip install -U pip wheel
           pip install .[docs]
 
       - name: Build Docs
         run: sphinx-build -b html -d build/sphinx-doctrees docs build/htmldocs
 
       - name: Archive Docs
         uses: actions/upload-artifact@v2
@@ -114,17 +93,15 @@
         uses: actions/setup-python@v3
         with:
           python-version: "3.8"
           architecture: "x64"
 
       - name: Development setup on ${{ matrix.os }}
         run: |
-          python -m pip install pip --upgrade
           pip install -e .[dev]
-          python -c "import pkg_resources; print(pkg_resources.get_distribution('widgetastic.core').version)"
           python -c "from widgetastic.widget import Widget, Browser"
 
   package:
     name: ⚙️ Build & Verify Package
     runs-on: ubuntu-latest
 
     steps:
@@ -135,12 +112,11 @@
         uses: actions/setup-python@v3
         with:
           python-version: "3.8"
           architecture: "x64"
 
       - name: Build and verify with twine
         run: |
-          python -m pip install pip --upgrade
-          pip install twine setuptools wheel --upgrade
-          python setup.py sdist bdist_wheel
+          pip install wheel twine
+          pip wheel --no-deps -w dist .
           ls -l dist
-          python -m twine check dist/*
+          twine check dist/*
```

### Comparing `widgetastic.core-1.0.0/.gitignore` & `widgetastic_core-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/.pre-commit-config.yaml` & `widgetastic_core-1.0.2/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/asottile/reorder_python_imports
-    rev: v3.0.1
+    rev: v3.1.0
     hooks:
       - id: reorder-python-imports
         language_version: python3
         args:
           - --application-directories=.:src
   - repo: https://github.com/psf/black
     rev: 22.3.0
@@ -16,27 +16,27 @@
   - repo: https://github.com/PyCQA/flake8
     rev: 4.0.1
     hooks:
       - id: flake8
         language_version: python3
         args:
           - --max-line-length=100
-          - --ignore=W503,E203
+          - --ignore=E128,E811,W503,W504,E203
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: trailing-whitespace
         language_version: python3
       - id: end-of-file-fixer
         language_version: python3
       - id: debug-statements
         language_version: python3
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.32.0
+    rev: v2.32.1
     hooks:
       - id: pyupgrade
         language_version: python3
         args: [--py3-plus, --py38-plus]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.942
+    rev: v0.960
     hooks:
       - id: mypy
```

### Comparing `widgetastic.core-1.0.0/LICENSE` & `widgetastic_core-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/README.rst` & `widgetastic_core-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/docs/Makefile` & `widgetastic_core-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/docs/advanced_usage.rst` & `widgetastic_core-1.0.2/docs/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/docs/basic_usage.rst` & `widgetastic_core-1.0.2/docs/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/docs/conf.py` & `widgetastic_core-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/docs/guidelines.rst` & `widgetastic_core-1.0.2/docs/guidelines.rst`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/docs/internals.rst` & `widgetastic_core-1.0.2/docs/internals.rst`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/docs/intro.rst` & `widgetastic_core-1.0.2/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/docs/ouia.rst` & `widgetastic_core-1.0.2/docs/ouia.rst`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/docs/source/widgetastic.rst` & `widgetastic_core-1.0.2/docs/source/widgetastic.rst`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/docs/source/widgetastic.widget.rst` & `widgetastic_core-1.0.2/docs/source/widgetastic.widget.rst`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/setup.cfg` & `widgetastic_core-1.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,60 @@
-[metadata]
-name = widgetastic.core
-author = Milan Falesnik
-author_email = mfalesni@redhat.com
-maintainer = Dmitrii Misharov
-maintainer_email = misharov@redhat.com
-description = Making testing of UIs fantastic
-long_description = file: README.rst
-license = Apache license
-url = https://github.com/RedHatQE/widgetastic.core
-classifiers = 
-	License :: OSI Approved :: Apache Software License
-	Programming Language :: Python
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: Implementation :: CPython
-	Programming Language :: Python :: Implementation :: PyPy
-	Topic :: Software Development :: Libraries :: Python Modules
-	Topic :: Software Development :: Quality Assurance
-	Topic :: Software Development :: Testing
-
-[options]
-python_requires = >= 3.8
-install_requires = 
-	anytree
-	cached_property
-	pytest
-	selenium >= 4.0.0
-	selenium-smart-locator
-	typing_extensions
-	wait_for
-setup_requires = setuptools_scm
-package_dir = 
-	=src
-packages = find:
-
-[options.extras_require]
-test = 
-	podman
-	pytest
-	pytest-xdist
-	pytest-cov
-dev = 
-	podman
-	pre-commit
-	pytest
-	pytest-xdist
-	pytest-cov
-docs = 
-	sphinx
-
-[options.packages.find]
-where = src
-
-[flake8]
-max-line-length = 100
-ignore = E128,E811,W503,W504,E203
-
-[egg_info]
-tag_build = 
-tag_date = 0
+[project]
+classifiers = [
+  "License :: OSI Approved :: Apache Software License",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
+  "Topic :: Software Development :: Libraries :: Python Modules",
+  "Topic :: Software Development :: Quality Assurance",
+  "Topic :: Software Development :: Testing",
+]
+description = "Making testing of UIs fantastic."
+dynamic = ["version"]
+keywords = ["widgetastic", "selenium"]
+license = {file = "LICENSE"}
+maintainers = [{name = "Dmitrii Misharov", email = "misharov@redhat.com"}]
+name = "widgetastic.core"
+readme = "README.rst"
+requires-python = ">=3.8"
+
+dependencies = [
+  "anytree",
+  "cached_property",
+  "selenium >= 4.0.0",
+  "selenium-smart-locator",
+  "typing_extensions",
+  "wait_for",
+]
+
+[project.optional-dependencies]
+dev = [
+  "podman",
+  "pre-commit",
+  "pytest",
+  "pytest-xdist",
+  "pytest-cov",
+]
+docs = ["sphinx"]
+test = [
+  "podman",
+  "pytest",
+  "pytest-xdist",
+  "pytest-cov",
+]
+
+[project.urls]
+repository = "https://github.com/RedHatQE/widgetastic.core"
+
+[build-system]
+build-backend = "hatchling.build"
+requires = ["hatchling", "hatch-vcs"]
 
+[tool.hatch.build.targets.wheel]
+packages = ["src/widgetastic"]
+
+[tool.hatch.version]
+source = "vcs"
```

### Comparing `widgetastic.core-1.0.0/src/widgetastic/browser.py` & `widgetastic_core-1.0.2/src/widgetastic/browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -839,19 +839,20 @@
             el.send_keys(Keys.SPACE, Keys.BACK_SPACE)
         self.plugin.after_keyboard_input(el, None)
         return result
 
     def is_selected(self, *args, **kwargs) -> bool:
         return self.element(*args, **kwargs).is_selected()
 
-    def send_keys(self, text: str, locator: LocatorAlias, *args, **kwargs) -> None:
+    def send_keys(self, text: str, locator: LocatorAlias, sensitive=False, *args, **kwargs) -> None:
         """Sends keys to the element. Detects the file inputs automatically.
 
         Args:
             text: Text to be inserted to the element.
+            sensitive: Bool, If is set to True do not log sensitive data.
             *args: See :py:meth:`elements`
             **kwargs: See :py:meth:`elements`
         """
         text = str(text) or ""
         file_intercept = False
         # If the element is input type file, we will need to use the file detector
         if self.tag(locator, *args, **kwargs) == "input":
@@ -860,15 +861,15 @@
                 file_intercept = True
         try:
             if file_intercept:
                 # If we detected a file upload field, let's use the file detector.
                 self.selenium.file_detector = LocalFileDetector()
             el = self.move_to_element(locator, *args, **kwargs)
             self.plugin.before_keyboard_input(el, text)
-            self.logger.debug("send_keys %r to %r", text, locator)
+            self.logger.debug("send_keys %r to %r", "*" * len(text) if sensitive else text, locator)
             result = el.send_keys(text)
             if Keys.ENTER not in text:
                 try:
                     self.plugin.after_keyboard_input(el, text)
                 except StaleElementReferenceException:
                     pass
             else:
```

### Comparing `widgetastic.core-1.0.0/src/widgetastic/exceptions.py` & `widgetastic_core-1.0.2/src/widgetastic/exceptions.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/src/widgetastic/log.py` & `widgetastic_core-1.0.2/src/widgetastic/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,22 +39,24 @@
 
 class PrependParentsAdapter(logging.LoggerAdapter):
     """This class ensures the path to the widget is represented in the log records."""
 
     def process(
         self, msg: str, kwargs: MutableMapping[str, Any]
     ) -> Tuple[str, MutableMapping[str, Any]]:
+        assert self.extra is not None  # python 3.10+ type check
         widget_path = cast(str, self.extra["widget_path"])
         # Sanitizing %->%% for formatter working properly
         return (
             "[{}]: {}".format(widget_path.replace("%", "%%"), msg),
             kwargs,
         )
 
     def __repr__(self) -> str:
+        assert self.extra is not None  # python 3.10+ type check
         return "{}({!r}, {!r})".format(type(self).__name__, self.logger, self.extra["widget_path"])
 
 
 def create_widget_logger(
     widget_path: str, logger: Optional[logging.Logger] = None
 ) -> PrependParentsAdapter:
     """Create a logger that prepends the ``widget_path`` to the log records.
```

### Comparing `widgetastic.core-1.0.0/src/widgetastic/ouia/__init__.py` & `widgetastic_core-1.0.2/src/widgetastic/ouia/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         ".//*[@data-ouia-component-type={@component_type}{@component_id_suffix}]"
     )
     browser: Browser
 
     def _set_attrs(
         self,
         component_type: str,
-        component_id: Optional[str] = None,
+        component_id: str = "",
     ) -> None:
         self.component_type = quote(component_type)
         self.component_id = quote(component_id)
         component_id = f" and @data-ouia-component-id={quote(component_id)}" if component_id else ""
         self.component_id_suffix = component_id
         self.locator = self.ROOT.locator
 
@@ -100,15 +100,15 @@
     """
 
     OUIA_COMPONENT_TYPE: str
 
     def __init__(
         self,
         parent: ViewParent,
-        component_id: Optional[str] = None,
+        component_id: str = "",
         logger: Optional[Logger] = None,
         component_type: Optional[str] = None,
     ) -> None:
         self._set_attrs(
             component_type=component_type or self.OUIA_COMPONENT_TYPE or type(self).__name__,
             component_id=component_id,
         )
```

### Comparing `widgetastic.core-1.0.0/src/widgetastic/ouia/checkbox.py` & `widgetastic_core-1.0.2/src/widgetastic/ouia/checkbox.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/src/widgetastic/ouia/input.py` & `widgetastic_core-1.0.2/src/widgetastic/ouia/input.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/src/widgetastic/types.py` & `widgetastic_core-1.0.2/src/widgetastic/types.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/src/widgetastic/utils.py` & `widgetastic_core-1.0.2/src/widgetastic/utils.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/src/widgetastic/widget/__init__.py` & `widgetastic_core-1.0.2/src/widgetastic/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/src/widgetastic/widget/base.py` & `widgetastic_core-1.0.2/src/widgetastic/widget/base.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/src/widgetastic/widget/checkbox.py` & `widgetastic_core-1.0.2/src/widgetastic/widget/checkbox.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/src/widgetastic/widget/image.py` & `widgetastic_core-1.0.2/src/widgetastic/widget/image.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/src/widgetastic/widget/input.py` & `widgetastic_core-1.0.2/src/widgetastic/widget/input.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,22 +50,27 @@
     @property
     def value(self):
         return self.browser.get_attribute("value", self)
 
     def read(self):
         return self.value
 
-    def fill(self, value):
+    def fill(self, value, sensitive=False):
+        """Fill TextInput widget with value
+        Args:
+           value: Text to be filled into the input.
+           sensitive: Bool, If is set to True do not log sensitive data.
+        """
         current_value = self.value
         if value == current_value:
             return False
         # Clear and type everything
         self.browser.click(self)
         self.browser.clear(self)
-        self.browser.send_keys(value, self)
+        self.browser.send_keys(value, self, sensitive)
         return True
 
 
 class FileInput(BaseInput):
     """This represents the file input.
 
     Args:
```

### Comparing `widgetastic.core-1.0.0/src/widgetastic/widget/select.py` & `widgetastic_core-1.0.2/src/widgetastic/widget/select.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/src/widgetastic/widget/table.py` & `widgetastic_core-1.0.2/src/widgetastic/widget/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,14 +404,22 @@
     HEADER_IN_ROWS = "./tbody/tr[1]/th"
     HEADERS = "./thead/tr/th|./tr/th|./thead/tr/td" + "|" + HEADER_IN_ROWS
 
     ROOT = ParametrizedLocator("{@locator}")
 
     Row = TableRow
 
+    _CACHED_PROPERTIES = [
+        "headers",
+        "attributized_headers",
+        "header_index_mapping",
+        "index_header_mapping",
+        "assoc_column_position",
+    ]
+
     def __init__(
         self,
         parent,
         locator,
         column_widgets=None,
         assoc_column=None,
         rows_ignore_top=None,
@@ -441,14 +449,18 @@
         return self._table_tree
 
     @property
     def table_tree(self):
         if self.has_rowcolspan:
             return self._get_table_tree()
 
+    @table_tree.deleter
+    def table_tree(self):
+        self._table_tree = None
+
     @cached_property
     def resolver(self):
         return TableResolver()
 
     @cached_property
     def caption(self):
         try:
@@ -481,26 +493,20 @@
         max_index = self.row_count
         if (-nindex) > max_index:
             raise IndexError(f"Negative index {nindex} wanted but we only have {max_index} rows")
         return max_index + nindex
 
     def clear_cache(self):
         """Clear all cached properties."""
-        for item in [
-            "headers",
-            "attributized_headers",
-            "header_index_mapping",
-            "index_header_mapping",
-            "assoc_column_position",
-            "table_tree",
-        ]:
+        for item in self._CACHED_PROPERTIES:
             try:
                 delattr(self, item)
             except AttributeError:
                 pass
+        del self.table_tree
 
     @cached_property
     def headers(self):
         result = []
         for header in self.browser.elements(self.HEADERS, parent=self):
             result.append(self.browser.text(header).strip() or None)
```

### Comparing `widgetastic.core-1.0.0/src/widgetastic/xpath.py` & `widgetastic_core-1.0.2/src/widgetastic/xpath.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/testing/conftest.py` & `widgetastic_core-1.0.2/testing/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 @pytest.fixture(scope="session")
 def selenium_url(worker_id, podman, pod):
     """Yields a command executor URL for selenium, and a port mapped for the test page to run on"""
     # use the worker id number from gw# to create hosts on loopback
     last_oktet = 1 if worker_id == "master" else int(worker_id.lstrip("gw")) + 1
     localhost_for_worker = f"127.0.0.{last_oktet}"
     container = podman.containers.create(
-        image="quay.io/redhatqe/selenium-standalone:ff_91.8.0esr_chrome_101.0.4951.41",
+        image="quay.io/redhatqe/selenium-standalone:latest",
         pod=pod.id,
         remove=True,
         name=f"selenium_{worker_id}",
     )
     container.start()
     yield f"http://{localhost_for_worker}:4444"
     container.remove(force=True)
```

### Comparing `widgetastic.core-1.0.0/testing/html/iframe_page.html` & `widgetastic_core-1.0.2/testing/html/iframe_page.html`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/testing/html/testing_page.html` & `widgetastic_core-1.0.2/testing/html/testing_page.html`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/testing/ouia_widgets.py` & `widgetastic_core-1.0.2/testing/ouia_widgets.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/testing/test_basic_widgets.py` & `widgetastic_core-1.0.2/testing/test_basic_widgets.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/testing/test_browser.py` & `widgetastic_core-1.0.2/testing/test_browser.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/testing/test_log.py` & `widgetastic_core-1.0.2/testing/test_log.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/testing/test_ouia.py` & `widgetastic_core-1.0.2/testing/test_ouia.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,7 +53,17 @@
     assert not testing_view.button.is_safe
     assert testing_view.select.is_safe
 
 
 def test_select(testing_view):
     testing_view.select.choose("first_option")
     testing_view.select.choose("second_option")
+
+
+def test_widget_without_id(browser):
+    class TestView(OUIAGenericView):
+        OUIA_COMPONENT_TYPE = "TestView"
+        button = Button()
+
+    view = TestView(browser)
+    assert view.is_displayed
+    assert view.button.locator == './/*[@data-ouia-component-type="PF/Button"]'
```

### Comparing `widgetastic.core-1.0.0/testing/test_utils.py` & `widgetastic_core-1.0.2/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/testing/test_version.py` & `widgetastic_core-1.0.2/testing/test_version.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/testing/test_version_pick.py` & `widgetastic_core-1.0.2/testing/test_version_pick.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/testing/test_view.py` & `widgetastic_core-1.0.2/testing/test_view.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/testing/test_widget.py` & `widgetastic_core-1.0.2/testing/test_widget.py`

 * *Files identical despite different names*

### Comparing `widgetastic.core-1.0.0/testing/test_widget_descriptor.py` & `widgetastic_core-1.0.2/testing/test_widget_descriptor.py`

 * *Files identical despite different names*

