# Comparing `tmp/github_actions_tests_louxsdon-0.1.1.tar.gz` & `tmp/github_actions_tests_louxsdon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_actions_tests_louxsdon-0.1.1.tar", max compression
+gzip compressed data, was "github_actions_tests_louxsdon-0.1.2.tar", max compression
```

## Comparing `github_actions_tests_louxsdon-0.1.1.tar` & `github_actions_tests_louxsdon-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-04-20 11:06:24.666343 github_actions_tests_louxsdon-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-20 11:06:24.670343 github_actions_tests_louxsdon-0.1.1/github_actions/__init__.py
--rw-r--r--   0        0        0      389 2023-04-20 11:06:24.670343 github_actions_tests_louxsdon-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      360 1970-01-01 00:00:00.000000 github_actions_tests_louxsdon-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-20 11:29:20.942130 github_actions_tests_louxsdon-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 11:29:20.946130 github_actions_tests_louxsdon-0.1.2/github_actions/__init__.py
+-rw-r--r--   0        0        0      389 2023-04-20 11:29:20.946130 github_actions_tests_louxsdon-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      360 1970-01-01 00:00:00.000000 github_actions_tests_louxsdon-0.1.2/PKG-INFO
```

