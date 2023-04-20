# Comparing `tmp/jinja2-arrow-0.1.1.tar.gz` & `tmp/jinja2-arrow-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2-arrow-0.1.1.tar", last modified: Sun Apr 16 08:54:06 2023, max compression
+gzip compressed data, was "jinja2-arrow-0.1.2.tar", last modified: Thu Apr 20 10:08:10 2023, max compression
```

## Comparing `jinja2-arrow-0.1.1.tar` & `jinja2-arrow-0.1.2.tar`

### file list

```diff
@@ -1,3 +1,4 @@
--rw-r--r--   0        0        0       45 2023-04-16 08:32:09.829609 jinja2-arrow-0.1.1/README.md
--rw-r--r--   0        0        0      351 2023-04-16 08:53:38.154533 jinja2-arrow-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      240 1970-01-01 00:00:00.000000 jinja2-arrow-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       45 2023-04-16 08:32:09.829609 jinja2-arrow-0.1.2/README.md
+-rw-r--r--   0        0        0      852 2023-04-20 10:05:39.692340 jinja2-arrow-0.1.2/jinja2_arrow/__init__.py
+-rw-r--r--   0        0        0      787 2023-04-20 10:04:46.112409 jinja2-arrow-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      240 1970-01-01 00:00:00.000000 jinja2-arrow-0.1.2/PKG-INFO
```

