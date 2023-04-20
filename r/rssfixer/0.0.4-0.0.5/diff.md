# Comparing `tmp/rssfixer-0.0.4.tar.gz` & `tmp/rssfixer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssfixer-0.0.4.tar", last modified: Mon Apr 17 11:06:55 2023, max compression
+gzip compressed data, was "rssfixer-0.0.5.tar", last modified: Thu Apr 20 06:40:54 2023, max compression
```

## Comparing `rssfixer-0.0.4.tar` & `rssfixer-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-17 11:06:55.796680 rssfixer-0.0.4/
--rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-17 09:42:15.000000 rssfixer-0.0.4/LICENSE
--rw-r--r--   0 reuteras   (501) staff       (20)     2914 2023-04-17 11:06:55.796526 rssfixer-0.0.4/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)     2371 2023-04-17 10:59:11.000000 rssfixer-0.0.4/README.md
--rw-r--r--   0 reuteras   (501) staff       (20)      799 2023-04-17 10:56:57.000000 rssfixer-0.0.4/pyproject.toml
--rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-17 11:06:55.796734 rssfixer-0.0.4/setup.cfg
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-17 11:06:55.793836 rssfixer-0.0.4/src/
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-17 11:06:55.795142 rssfixer-0.0.4/src/rssfixer/
--rw-r--r--   0 reuteras   (501) staff       (20)       60 2023-04-17 09:42:15.000000 rssfixer-0.0.4/src/rssfixer/__init__.py
--rw-r--r--   0 reuteras   (501) staff       (20)     5296 2023-04-17 10:54:49.000000 rssfixer-0.0.4/src/rssfixer/rss.py
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-17 11:06:55.796319 rssfixer-0.0.4/src/rssfixer.egg-info/
--rw-r--r--   0 reuteras   (501) staff       (20)     2914 2023-04-17 11:06:55.000000 rssfixer-0.0.4/src/rssfixer.egg-info/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)      295 2023-04-17 11:06:55.000000 rssfixer-0.0.4/src/rssfixer.egg-info/SOURCES.txt
--rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-17 11:06:55.000000 rssfixer-0.0.4/src/rssfixer.egg-info/dependency_links.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-17 11:06:55.000000 rssfixer-0.0.4/src/rssfixer.egg-info/entry_points.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       58 2023-04-17 11:06:55.000000 rssfixer-0.0.4/src/rssfixer.egg-info/requires.txt
--rw-r--r--   0 reuteras   (501) staff       (20)        9 2023-04-17 11:06:55.000000 rssfixer-0.0.4/src/rssfixer.egg-info/top_level.txt
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 06:40:54.906153 rssfixer-0.0.5/
+-rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-17 09:42:15.000000 rssfixer-0.0.5/LICENSE
+-rw-r--r--   0 reuteras   (501) staff       (20)     4627 2023-04-20 06:40:54.906033 rssfixer-0.0.5/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)     4084 2023-04-20 06:30:06.000000 rssfixer-0.0.5/README.md
+-rw-r--r--   0 reuteras   (501) staff       (20)      813 2023-04-19 11:00:15.000000 rssfixer-0.0.5/pyproject.toml
+-rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-20 06:40:54.906196 rssfixer-0.0.5/setup.cfg
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 06:40:54.903735 rssfixer-0.0.5/src/
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 06:40:54.904843 rssfixer-0.0.5/src/rssfixer/
+-rw-r--r--   0 reuteras   (501) staff       (20)       61 2023-04-18 04:00:23.000000 rssfixer-0.0.5/src/rssfixer/__init__.py
+-rw-r--r--   0 reuteras   (501) staff       (20)     8946 2023-04-20 06:29:30.000000 rssfixer-0.0.5/src/rssfixer/rss.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 06:40:54.905617 rssfixer-0.0.5/src/rssfixer.egg-info/
+-rw-r--r--   0 reuteras   (501) staff       (20)     4627 2023-04-20 06:40:54.000000 rssfixer-0.0.5/src/rssfixer.egg-info/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)      317 2023-04-20 06:40:54.000000 rssfixer-0.0.5/src/rssfixer.egg-info/SOURCES.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-20 06:40:54.000000 rssfixer-0.0.5/src/rssfixer.egg-info/dependency_links.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-20 06:40:54.000000 rssfixer-0.0.5/src/rssfixer.egg-info/entry_points.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       65 2023-04-20 06:40:54.000000 rssfixer-0.0.5/src/rssfixer.egg-info/requires.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-20 06:40:54.000000 rssfixer-0.0.5/src/rssfixer.egg-info/top_level.txt
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 06:40:54.905735 rssfixer-0.0.5/src/tests/
+-rw-r--r--   0 reuteras   (501) staff       (20)     2341 2023-04-18 10:59:41.000000 rssfixer-0.0.5/src/tests/test_rss.py
```

### Comparing `rssfixer-0.0.4/LICENSE` & `rssfixer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rssfixer-0.0.4/PKG-INFO` & `rssfixer-0.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # rssfixer
 
-A small tool to generate an [RSS][rss] feed from some [Wordpress][wor] blogs that for some reason don't generate their own feeds.
+[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
+![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)
+[![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)
+
+A small tool to generate an [RSS][rss] feed from some [WordPress][wor] blogs that for some reason don't generate their own feeds. This tool uses [BeautifulSoup][bso] to parse the HTML and [feedgen][fge] to generate the feed.
 
 ## Installation
 
 ```bash
-pip install rssfixer
+python3 -m venv venv
+source venv/bin/activate
+python3 -m pip install rssfixer
 ```
 
 ## Example
 
 Format for storing the links varies but I'll try and add more formats as I find them.
 
 ### List
@@ -35,15 +41,15 @@
 $ rssfixer --title nccgroup https://research.nccgroup.com/
 RSS feed created: rss_feed.xml
 ```
 
 You can specify a filename and silence output:
 
 ```bash
-$ rssfixer --title nccgroup --output nccgroup.xml --quiet https://research.nccgroup.com/
+rssfixer --title nccgroup --output nccgroup.xml --quiet https://research.nccgroup.com/
 ```
 
 The resulting file is available [here][exa] as an example.
 
 Most times you would run the script from crontab to have an updated feed. Here is an example with a venv in _/home/user/src/rssfixer_.
 
 ```bash
@@ -56,38 +62,57 @@
 
 ```bash
 rssfixer --json --quiet --output truesec.xml https://www.truesec.com/hub/blog
 ```
 
 ### Usage
 
-```bash
-usage: rssfixer [-h] [--json] [--json-entries JSON_ENTRIES] [--json-url JSON_URL] [--json-title JSON_TITLE] [--json-description JSON_DESCRIPTION] [--output OUTPUT]
-                [--title TITLE] [-q]
+```Text
+usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html] [--html-entries HTML_ENTRIES] [--html-url HTML_URL] [--html-title HTML_TITLE]
+                [--html-title-class HTML_TITLE_CLASS] [--html-description HTML_DESCRIPTION] [--html-description-class HTML_DESCRIPTION_CLASS] [--json] [--json-entries JSON_ENTRIES]
+                [--json-url JSON_URL] [--json-title JSON_TITLE] [--json-description JSON_DESCRIPTION] [--output OUTPUT] [--title TITLE] [-q] [--list]
                 url
 
-Generate RSS feed for blog that don't publish a feed
+Generate RSS feed for blog that don't publish a feed. Default is to find links in a simple <ul>-list. Options are available to find links in other HTML elements or JSON strings.
 
 positional arguments:
   url                   URL for the blog
 
 options:
   -h, --help            show this help message and exit
+  --version             show program's version number and exit
+  --atom                Generate Atom feed
+  --base-url BASE_URL   Base URL for the blog
+  --html                Find entries in HTML
+  --html-entries HTML_ENTRIES
+                        HTML selector for entries
+  --html-url HTML_URL   HTML selector for URL
+  --html-title HTML_TITLE
+                        HTML selector for title
+  --html-title-class HTML_TITLE_CLASS
+                        Flag to specify title class (regex)
+  --html-description HTML_DESCRIPTION
+                        HTML selector for description
+  --html-description-class HTML_DESCRIPTION_CLASS
+                        Flag to specify description class (regex)
   --json                Find entries in JSON
   --json-entries JSON_ENTRIES
                         JSON key for entries (default: 'entries')
   --json-url JSON_URL   JSON key for URL (default: 'url')
   --json-title JSON_TITLE
-                        JSON key for title (default: 'title')
+                        JSON key for title
   --json-description JSON_DESCRIPTION
-                        JSON key for description (default: 'preamble')
-  --output OUTPUT       Name of the output file (default: "rss_feed.xml")
+                        JSON key for description
+  --output OUTPUT       Name of the output file
   --title TITLE         Title of the RSS feed (default: "My RSS Feed")
   -q, --quiet           Suppress output
+  --list                Find entries in HTML <ul>-list (default)
 ```
 
 
+  [bso]: https://www.crummy.com/software/BeautifulSoup/
   [exa]: https://github.com/reuteras/rssfixer/blob/main/example/nccgroup.xml
+  [fge]: https://feedgen.kiesow.be/ 
   [ncc]: https://research.nccgroup.com/
   [rss]: https://www.rssboard.org/
   [tru]: https://www.truesec.com/hub/blog
   [wor]: https://wordpress.org/
```

### Comparing `rssfixer-0.0.4/pyproject.toml` & `rssfixer-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rssfixer"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Peter Reuterås", email="peter@reuteras.net" },
 ]
 description = "Generate RSS feed for Wordpress blog without it."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -22,14 +22,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project.optional-dependencies]
 dev = [
     "build",
+    "pytest",
     "pylint",
     "twine",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/reuteras/rssfixer"
 "Bug Tracker" = "https://github.com/reuteras/rssfixer/issues"
```

### Comparing `rssfixer-0.0.4/src/rssfixer.egg-info/PKG-INFO` & `rssfixer-0.0.5/src/rssfixer.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # rssfixer
 
-A small tool to generate an [RSS][rss] feed from some [Wordpress][wor] blogs that for some reason don't generate their own feeds.
+[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
+![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)
+[![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)
+
+A small tool to generate an [RSS][rss] feed from some [WordPress][wor] blogs that for some reason don't generate their own feeds. This tool uses [BeautifulSoup][bso] to parse the HTML and [feedgen][fge] to generate the feed.
 
 ## Installation
 
 ```bash
-pip install rssfixer
+python3 -m venv venv
+source venv/bin/activate
+python3 -m pip install rssfixer
 ```
 
 ## Example
 
 Format for storing the links varies but I'll try and add more formats as I find them.
 
 ### List
@@ -35,15 +41,15 @@
 $ rssfixer --title nccgroup https://research.nccgroup.com/
 RSS feed created: rss_feed.xml
 ```
 
 You can specify a filename and silence output:
 
 ```bash
-$ rssfixer --title nccgroup --output nccgroup.xml --quiet https://research.nccgroup.com/
+rssfixer --title nccgroup --output nccgroup.xml --quiet https://research.nccgroup.com/
 ```
 
 The resulting file is available [here][exa] as an example.
 
 Most times you would run the script from crontab to have an updated feed. Here is an example with a venv in _/home/user/src/rssfixer_.
 
 ```bash
@@ -56,38 +62,57 @@
 
 ```bash
 rssfixer --json --quiet --output truesec.xml https://www.truesec.com/hub/blog
 ```
 
 ### Usage
 
-```bash
-usage: rssfixer [-h] [--json] [--json-entries JSON_ENTRIES] [--json-url JSON_URL] [--json-title JSON_TITLE] [--json-description JSON_DESCRIPTION] [--output OUTPUT]
-                [--title TITLE] [-q]
+```Text
+usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html] [--html-entries HTML_ENTRIES] [--html-url HTML_URL] [--html-title HTML_TITLE]
+                [--html-title-class HTML_TITLE_CLASS] [--html-description HTML_DESCRIPTION] [--html-description-class HTML_DESCRIPTION_CLASS] [--json] [--json-entries JSON_ENTRIES]
+                [--json-url JSON_URL] [--json-title JSON_TITLE] [--json-description JSON_DESCRIPTION] [--output OUTPUT] [--title TITLE] [-q] [--list]
                 url
 
-Generate RSS feed for blog that don't publish a feed
+Generate RSS feed for blog that don't publish a feed. Default is to find links in a simple <ul>-list. Options are available to find links in other HTML elements or JSON strings.
 
 positional arguments:
   url                   URL for the blog
 
 options:
   -h, --help            show this help message and exit
+  --version             show program's version number and exit
+  --atom                Generate Atom feed
+  --base-url BASE_URL   Base URL for the blog
+  --html                Find entries in HTML
+  --html-entries HTML_ENTRIES
+                        HTML selector for entries
+  --html-url HTML_URL   HTML selector for URL
+  --html-title HTML_TITLE
+                        HTML selector for title
+  --html-title-class HTML_TITLE_CLASS
+                        Flag to specify title class (regex)
+  --html-description HTML_DESCRIPTION
+                        HTML selector for description
+  --html-description-class HTML_DESCRIPTION_CLASS
+                        Flag to specify description class (regex)
   --json                Find entries in JSON
   --json-entries JSON_ENTRIES
                         JSON key for entries (default: 'entries')
   --json-url JSON_URL   JSON key for URL (default: 'url')
   --json-title JSON_TITLE
-                        JSON key for title (default: 'title')
+                        JSON key for title
   --json-description JSON_DESCRIPTION
-                        JSON key for description (default: 'preamble')
-  --output OUTPUT       Name of the output file (default: "rss_feed.xml")
+                        JSON key for description
+  --output OUTPUT       Name of the output file
   --title TITLE         Title of the RSS feed (default: "My RSS Feed")
   -q, --quiet           Suppress output
+  --list                Find entries in HTML <ul>-list (default)
 ```
 
 
+  [bso]: https://www.crummy.com/software/BeautifulSoup/
   [exa]: https://github.com/reuteras/rssfixer/blob/main/example/nccgroup.xml
+  [fge]: https://feedgen.kiesow.be/ 
   [ncc]: https://research.nccgroup.com/
   [rss]: https://www.rssboard.org/
   [tru]: https://www.truesec.com/hub/blog
   [wor]: https://wordpress.org/
```

