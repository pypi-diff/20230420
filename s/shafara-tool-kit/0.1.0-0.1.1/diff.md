# Comparing `tmp/shafara_tool_kit-0.1.0.tar.gz` & `tmp/shafara_tool_kit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shafara_tool_kit-0.1.0.tar", max compression
+gzip compressed data, was "shafara_tool_kit-0.1.1.tar", max compression
```

## Comparing `shafara_tool_kit-0.1.0.tar` & `shafara_tool_kit-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      337 2023-04-20 11:35:39.292714 shafara_tool_kit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 11:35:39.264722 shafara_tool_kit-0.1.0/README.md
--rw-r--r--   0        0        0       41 2023-04-20 11:42:31.531797 shafara_tool_kit-0.1.0/shafara_tool_kit/__init__.py
--rw-r--r--   0        0        0      108 2023-04-20 11:41:05.406004 shafara_tool_kit-0.1.0/shafara_tool_kit/props.py
--rw-r--r--   0        0        0      348 1970-01-01 00:00:00.000000 shafara_tool_kit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      335 2023-04-20 12:43:31.366573 shafara_tool_kit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 11:35:39.264722 shafara_tool_kit-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 12:39:40.438529 shafara_tool_kit-0.1.1/shafaratoolkit/__init__.py
+-rw-r--r--   0        0        0      108 2023-04-20 11:41:05.406004 shafara_tool_kit-0.1.1/shafaratoolkit/props.py
+-rw-r--r--   0        0        0      392 1970-01-01 00:00:00.000000 shafara_tool_kit-0.1.1/PKG-INFO
```

