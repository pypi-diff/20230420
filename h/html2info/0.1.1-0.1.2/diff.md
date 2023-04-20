# Comparing `tmp/html2info-0.1.1.tar.gz` & `tmp/html2info-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2info-0.1.1.tar", last modified: Wed Apr 19 23:29:10 2023, max compression
+gzip compressed data, was "html2info-0.1.2.tar", last modified: Thu Apr 20 20:58:01 2023, max compression
```

## Comparing `html2info-0.1.1.tar` & `html2info-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 23:29:10.717073 html2info-0.1.1/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1515 2023-04-19 23:29:10.717073 html2info-0.1.1/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      780 2023-04-19 23:25:06.000000 html2info-0.1.1/README.md
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 23:29:10.717073 html2info-0.1.1/html2info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 18:56:39.000000 html2info-0.1.1/html2info/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     4779 2023-04-19 22:59:51.000000 html2info-0.1.1/html2info/linkedin.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      190 2023-04-19 19:16:29.000000 html2info-0.1.1/html2info/utils.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 23:29:10.717073 html2info-0.1.1/html2info.egg-info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1515 2023-04-19 23:29:10.000000 html2info-0.1.1/html2info.egg-info/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      260 2023-04-19 23:29:10.000000 html2info-0.1.1/html2info.egg-info/SOURCES.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-04-19 23:29:10.000000 html2info-0.1.1/html2info.egg-info/dependency_links.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       50 2023-04-19 23:29:10.000000 html2info-0.1.1/html2info.egg-info/requires.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       10 2023-04-19 23:29:10.000000 html2info-0.1.1/html2info.egg-info/top_level.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1478 2023-04-19 22:54:36.000000 html2info-0.1.1/pyproject.toml
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-04-19 23:29:10.717073 html2info-0.1.1/setup.cfg
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1360 2023-04-19 23:25:14.000000 html2info-0.1.1/setup.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-20 20:58:01.828477 html2info-0.1.2/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-20 20:58:01.828477 html2info-0.1.2/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5278 2023-04-20 20:54:37.000000 html2info-0.1.2/README.md
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-20 20:58:01.828477 html2info-0.1.2/html2info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 18:56:39.000000 html2info-0.1.2/html2info/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     4720 2023-04-20 20:52:29.000000 html2info-0.1.2/html2info/linkedin.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      190 2023-04-19 19:16:29.000000 html2info-0.1.2/html2info/utils.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-20 20:58:01.828477 html2info-0.1.2/html2info.egg-info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-20 20:58:01.000000 html2info-0.1.2/html2info.egg-info/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      260 2023-04-20 20:58:01.000000 html2info-0.1.2/html2info.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-04-20 20:58:01.000000 html2info-0.1.2/html2info.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       23 2023-04-20 20:58:01.000000 html2info-0.1.2/html2info.egg-info/requires.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       10 2023-04-20 20:58:01.000000 html2info-0.1.2/html2info.egg-info/top_level.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1478 2023-04-19 22:54:36.000000 html2info-0.1.2/pyproject.toml
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-04-20 20:58:01.828477 html2info-0.1.2/setup.cfg
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1360 2023-04-20 20:54:01.000000 html2info-0.1.2/setup.py
```

### Comparing `html2info-0.1.1/html2info/linkedin.py` & `html2info-0.1.2/html2info/linkedin.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,26 +52,25 @@
 
         for item in experience_items:
             title = item.find("span", class_="t-bold")
             company = item.find("span", class_="t-14 t-normal")
             image_link = item.find("img")["src"] if item.find("img") else None
             company_link = item.find("a", class_="optional-action-target-wrapper")["href"]
 
-            date_span = item.find("span", {"class": "t-14 t-normal t-black--light"})
-            dates = date_span.span.text.strip()
+            dates = item.find("span", {"class": "t-14 t-normal t-black--light"})
 
             description = item.find("div", class_="inline-show-more-text")
 
             self.experience += [
                 {
                     "title": title.span.text.strip() if title else None,
                     "company": company.span.text.strip() if company else None,
                     "image_link": image_link.strip() if image_link else None,
                     "company_link": company_link.strip() if company_link else None,
-                    "dates": dates,
+                    "dates": dates.span.text.strip() if dates else None,
                     "description": description.span.text.strip() if description else None,
                 }
             ]
 
     def parse_education(self):
         self.education_list = []
 
@@ -86,31 +85,31 @@
 
             degree_and_major_tags = item.find_all("span", {"class": "t-14 t-normal"})
             if len(degree_and_major_tags) == 0:
                 continue
 
             university_name = item.find("span", {"class": "mr1"})
             degree_and_major = degree_and_major_tags[0].span
+
             # extract the dates
-            date_span = item.find("span", {"class": "t-14 t-normal t-black--light"})
-            dates = date_span.span
+            dates = item.find("span", {"class": "t-14 t-normal t-black--light"})
 
             # extract the link to the university
             university_link = item.find("a")["href"]
 
             # extract the link to the university logo
             image_tag = item.find("img", {"class": "ivm-view-attr__img--centered"})
             image_link = image_tag["src"] if image_tag else None
 
             # add the education details to the list
             self.education_list += [
                 {
                     "university_name": university_name.span.text.strip() if university_name else None,
                     "degree_and_major": degree_and_major.text.strip() if degree_and_major else None,
-                    "dates": dates.text.strip() if degree_and_major else None,
+                    "dates": dates.span.text.strip() if dates else None,
                     "university_link": university_link,
                     "image_link": image_link,
                 }
             ]
 
     def to_dict(self):
         exclude_keys = {"soup"}
```

### Comparing `html2info-0.1.1/pyproject.toml` & `html2info-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `html2info-0.1.1/setup.py` & `html2info-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="html2info",  # Replace with your package name
-    version="0.1.1",  # Replace with your package version
+    version="0.1.2",  # Replace with your package version
     author="Vladimir Iglovikov",  # Replace with your name
     author_email="iglovikov@gmail.com",  # Replace with your email
     description="A package to parse raw HTML and return structured information.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
     classifiers=[
```

