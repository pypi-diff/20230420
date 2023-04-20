# Comparing `tmp/NewsArticlesScraper-0.2.tar.gz` & `tmp/NewsArticlesScraper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewsArticlesScraper-0.2.tar", last modified: Mon Apr 17 15:31:56 2023, max compression
+gzip compressed data, was "NewsArticlesScraper-0.2.1.tar", last modified: Thu Apr 20 12:41:00 2023, max compression
```

## Comparing `NewsArticlesScraper-0.2.tar` & `NewsArticlesScraper-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 15:31:56.670459 NewsArticlesScraper-0.2/
-drwxrwxrwx   0        0        0        0 2023-04-17 15:31:56.660459 NewsArticlesScraper-0.2/NewsArticlesScraper/
--rw-rw-rw-   0        0        0    12860 2023-04-17 15:28:59.000000 NewsArticlesScraper-0.2/NewsArticlesScraper/Scrapers.py
--rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.2/NewsArticlesScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:31:56.668960 NewsArticlesScraper-0.2/NewsArticlesScraper.egg-info/
--rw-rw-rw-   0        0        0      646 2023-04-17 15:31:56.000000 NewsArticlesScraper-0.2/NewsArticlesScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-04-17 15:31:56.000000 NewsArticlesScraper-0.2/NewsArticlesScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:31:56.000000 NewsArticlesScraper-0.2/NewsArticlesScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-17 15:31:56.000000 NewsArticlesScraper-0.2/NewsArticlesScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-17 15:31:56.000000 NewsArticlesScraper-0.2/NewsArticlesScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      646 2023-04-17 15:31:56.669963 NewsArticlesScraper-0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 15:31:56.670959 NewsArticlesScraper-0.2/setup.cfg
--rw-rw-rw-   0        0        0      994 2023-04-17 15:28:59.000000 NewsArticlesScraper-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:41:00.119482 NewsArticlesScraper-0.2.1/
+drwxrwxrwx   0        0        0        0 2023-04-20 12:41:00.095483 NewsArticlesScraper-0.2.1/NewsArticlesScraper/
+-rw-rw-rw-   0        0        0    13762 2023-04-20 12:33:03.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper/Scrapers.py
+-rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper/__init__.py
+-rw-rw-rw-   0        0        0     1138 2023-04-20 12:35:55.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper/test.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:41:00.117980 NewsArticlesScraper-0.2.1/NewsArticlesScraper.egg-info/
+-rw-rw-rw-   0        0        0      648 2023-04-20 12:41:00.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-04-20 12:41:00.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 12:41:00.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-20 12:41:00.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-20 12:41:00.000000 NewsArticlesScraper-0.2.1/NewsArticlesScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      648 2023-04-20 12:41:00.118982 NewsArticlesScraper-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 12:41:00.119482 NewsArticlesScraper-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      996 2023-04-20 12:40:52.000000 NewsArticlesScraper-0.2.1/setup.py
```

### Comparing `NewsArticlesScraper-0.2/NewsArticlesScraper/Scrapers.py` & `NewsArticlesScraper-0.2.1/NewsArticlesScraper/Scrapers.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,28 +98,31 @@
                     if "premium" in clasf:
                         premium = True
                 if not premium:
                     if result["cn:branding"] == "cnbc":
                         if result["cn:type"] not in ["cnbcvideo", "live_story"]:
                             yield scrapy.Request(result["cn:liveURL"], callback=self.parse_article, meta={"time": t})
 
+    def parse_article(self, response):
+        yield self.parse_article_func(response, meta=response.meta)
+
     @staticmethod
-    def parse_article(response):
+    def parse_article_func(response, meta):
         content = "".join(response.css(".ArticleBody-subtitle , .group p").css("::text").getall())
         title = response.css(".ArticleHeader-headline ::text").get()
         if title is None:
             title = response.css(".twoCol .title ::text").get()
         author = response.css(".Author-authorName ::text").get()
         if author is None:
             author = response.css(".source > a ::text").get()
-        yield {
+        return {
             "title": title,
             "author_name": author,
             "body": content,
-            "time": response.meta["time"],
+            "time": meta["time"],
             "url": response.url,
             "origin": "c",
         }
 
 
 class NYTSpider(scrapy.Spider):
     """Spider to scrape NYT articles.
@@ -195,25 +198,39 @@
             else:
                 try:
                     url = article["related_urls"][0]["url"]
                 except (TypeError, IndexError):
                     url = article["url"]
             yield scrapy.Request(url=url, callback=self.parse_article, meta={"time": pub_date})
 
+    def parse_article(self, response):
+        yield self.parse_article_func(response, meta=response.meta)
+
     @staticmethod
-    def parse_article(response):
-        content = "".join(response.css(".StoryBodyCompanionColumn > div > p ::text").getall())
+    def parse_article_func(response, meta):
+        title = response.css("div h1 ::text").get()
+        if title is None:
+            title = ""
         author_name = response.css(".last-byline ::text").get()
+        if author_name is None:
+            author_name = response.css(".e1jsehar0 ::text").get()
         if author_name is not None:
             author_name = re.sub("[Bb]y.", "", author_name)
-        yield {
-            "title": response.css("div h1 ::text").get(),
+        else:
+            author_name = ""
+        content = "".join(response.css(".StoryBodyCompanionColumn > div > p ::text").getall())
+        if content == "":
+            content = "".join(response.css(".g-caption ::text").getall())
+        if content == "":
+            content = "".join(response.css(".g-body ::text").getall())
+        return {
+            "title": title,
             "author_name": author_name,
             "body": content,
-            "time": response.meta["time"],
+            "time": meta["time"],
             "url": response.url,
             "origin": "n",
         }
 
 
 class TheGuardianSpider(scrapy.Spider):
     """Spider to scrape The Guardian articles.
@@ -264,16 +281,19 @@
     def parse_api(self, response):
         data = response.json()["response"]
         articles = data["results"]
         for article in articles:
             yield scrapy.Request(url=article["webUrl"], callback=self.parse_article,
                                  meta={"time": article["webPublicationDate"]})
 
+    def parse_article(self, response):
+        yield self.parse_article_func(response, response.meta)
+
     @staticmethod
-    def parse_article(response):
+    def parse_article_func(response, meta):
         title = response.css(".dcr-y70mar ::text").get()
         if title is None:
             title = response.css(".dcr-1kwg2vo ::text").get()
         if title is None:
             title = response.css(".dcr-18ogzt ::text").get()
         if title is None:
             title = response.css(".dcr-1ttbui0 ::text").get()
@@ -289,15 +309,20 @@
             author_name = response.css(".dcr-8gsycy a ::text").get()
         if author_name is None:
             author_name = ""
 
         body = " ".join(response.css(".dcr-n6w1lc ::text").getall())
         if body == "":
             body = " ".join(response.css("#maincontent p ::text").getall())
-        yield {
+        return {
             "title": title,
             "author_name": author_name,
             "body": body,
-            "time": response.meta["time"],
+            "time": meta["time"],
             "url": response.url,
             "origin": "g"
         }
+
+
+parse_cnbc = CNBCSpider.parse_article_func
+parse_nyt = NYTSpider.parse_article_func
+parse_guardian = TheGuardianSpider.parse_article_func
```

### Comparing `NewsArticlesScraper-0.2/NewsArticlesScraper.egg-info/PKG-INFO` & `NewsArticlesScraper-0.2.1/NewsArticlesScraper.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2
+Version: 0.2.1
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2/PKG-INFO` & `NewsArticlesScraper-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2
+Version: 0.2.1
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2/setup.py` & `NewsArticlesScraper-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2'
+VERSION = '0.2.1'
 DESCRIPTION = 'Scraping news articles'
 LONG_DESCRIPTION = 'A package that allows you to scrape news articles from various news sites via scrapy.'
 
 # Setting up
 setup(
     name="NewsArticlesScraper",
     version=VERSION,
```

