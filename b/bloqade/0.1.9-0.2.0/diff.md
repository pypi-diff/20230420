# Comparing `tmp/bloqade-0.1.9.tar.gz` & `tmp/bloqade-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloqade-0.1.9.tar", max compression
+gzip compressed data, was "bloqade-0.2.0.tar", last modified: Thu Apr 20 18:42:46 2023, max compression
```

## Comparing `bloqade-0.1.9.tar` & `bloqade-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0    10619 2022-07-30 19:05:47.566955 bloqade-0.1.9/LICENSE
--rw-r--r--   0        0        0        0 2022-07-18 16:04:50.607748 bloqade-0.1.9/README.md
--rw-r--r--   0        0        0      152 2022-07-30 22:27:30.381230 bloqade-0.1.9/bloqade/__init__.py
--rw-r--r--   0        0        0     1070 2022-07-30 22:27:36.222881 bloqade-0.1.9/bloqade/julia.py
--rw-r--r--   0        0        0     1632 2022-07-30 22:45:16.206339 bloqade-0.1.9/bloqade/types.py
--rw-r--r--   0        0        0       22 2022-07-30 23:12:01.637766 bloqade-0.1.9/bloqade/version.py
--rw-r--r--   0        0        0      167 2022-07-18 16:04:50.608211 bloqade-0.1.9/juliapkg.json
--rw-r--r--   0        0        0     1013 2022-07-30 23:12:01.637364 bloqade-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      666 2022-07-30 23:12:20.615319 bloqade-0.1.9/setup.py
--rw-r--r--   0        0        0     1055 2022-07-30 23:12:20.615455 bloqade-0.1.9/PKG-INFO
+drwxr-xr-x   0 roger      (501) staff       (20)        0 2023-04-20 18:42:46.236289 bloqade-0.2.0/
+-rw-r--r--   0 roger      (501) staff       (20)      279 2023-04-20 18:42:46.236177 bloqade-0.2.0/PKG-INFO
+-rw-r--r--   0 roger      (501) staff       (20)       49 2023-04-20 16:44:32.000000 bloqade-0.2.0/README.md
+-rw-r--r--   0 roger      (501) staff       (20)      660 2023-04-20 18:42:43.000000 bloqade-0.2.0/pyproject.toml
+-rw-r--r--   0 roger      (501) staff       (20)       38 2023-04-20 18:42:46.236320 bloqade-0.2.0/setup.cfg
+drwxr-xr-x   0 roger      (501) staff       (20)        0 2023-04-20 18:42:46.235068 bloqade-0.2.0/src/
+drwxr-xr-x   0 roger      (501) staff       (20)        0 2023-04-20 18:42:46.235420 bloqade-0.2.0/src/bloqade/
+-rw-r--r--   0 roger      (501) staff       (20)      129 2023-04-20 18:39:21.000000 bloqade-0.2.0/src/bloqade/__init__.py
+drwxr-xr-x   0 roger      (501) staff       (20)        0 2023-04-20 18:42:46.236008 bloqade-0.2.0/src/bloqade.egg-info/
+-rw-r--r--   0 roger      (501) staff       (20)      279 2023-04-20 18:42:46.000000 bloqade-0.2.0/src/bloqade.egg-info/PKG-INFO
+-rw-r--r--   0 roger      (501) staff       (20)      222 2023-04-20 18:42:46.000000 bloqade-0.2.0/src/bloqade.egg-info/SOURCES.txt
+-rw-r--r--   0 roger      (501) staff       (20)        1 2023-04-20 18:42:46.000000 bloqade-0.2.0/src/bloqade.egg-info/dependency_links.txt
+-rw-r--r--   0 roger      (501) staff       (20)       86 2023-04-20 18:42:46.000000 bloqade-0.2.0/src/bloqade.egg-info/requires.txt
+-rw-r--r--   0 roger      (501) staff       (20)        8 2023-04-20 18:42:46.000000 bloqade-0.2.0/src/bloqade.egg-info/top_level.txt
```

