# Comparing `tmp/ipfskvs-0.0.9.tar.gz` & `tmp/ipfskvs-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfskvs-0.0.9.tar", last modified: Mon Apr 17 20:39:52 2023, max compression
+gzip compressed data, was "ipfskvs-0.1.0.tar", max compression
```

## Comparing `ipfskvs-0.0.9.tar` & `ipfskvs-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,7 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 20:39:52.300344 ipfskvs-0.0.9/
--rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-12 01:55:42.000000 ipfskvs-0.0.9/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)     3243 2023-04-17 20:39:52.300230 ipfskvs-0.0.9/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     1353 2023-04-17 19:42:03.000000 ipfskvs-0.0.9/README.md
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 20:39:52.300101 ipfskvs-0.0.9/ipfskvs.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)     3243 2023-04-17 20:39:52.000000 ipfskvs-0.0.9/ipfskvs.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      195 2023-04-17 20:39:52.000000 ipfskvs-0.0.9/ipfskvs.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 20:39:52.000000 ipfskvs-0.0.9/ipfskvs.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)       50 2023-04-17 20:39:52.000000 ipfskvs-0.0.9/ipfskvs.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 20:39:52.000000 ipfskvs-0.0.9/ipfskvs.egg-info/top_level.txt
--rw-r--r--   0 nate       (501) staff       (20)      638 2023-04-17 20:34:56.000000 ipfskvs-0.0.9/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-17 20:39:52.300377 ipfskvs-0.0.9/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)      886 2023-04-17 20:36:37.000000 ipfskvs-0.0.9/setup.py
+-rw-r--r--   0        0        0     1211 2023-04-12 01:55:42.945987 ipfskvs-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2015 2023-04-20 00:29:03.095803 ipfskvs-0.1.0/README.md
+-rw-r--r--   0        0        0      114 2023-04-19 23:07:57.572749 ipfskvs-0.1.0/ipfskvs/__init__.py
+-rw-r--r--   0        0        0     6386 2023-04-18 01:17:33.926227 ipfskvs-0.1.0/ipfskvs/index.py
+-rw-r--r--   0        0        0     9039 2023-04-19 00:48:11.804274 ipfskvs-0.1.0/ipfskvs/store.py
+-rw-r--r--   0        0        0      434 2023-04-20 00:27:38.616370 ipfskvs-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 ipfskvs-0.1.0/PKG-INFO
```

### Comparing `ipfskvs-0.0.9/LICENSE` & `ipfskvs-0.1.0/LICENSE`

 * *Files identical despite different names*

