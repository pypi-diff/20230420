# Comparing `tmp/mkdocs-glightbox-0.3.2.tar.gz` & `tmp/mkdocs-glightbox-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-glightbox-0.3.2.tar", last modified: Sun Mar 19 10:26:50 2023, max compression
+gzip compressed data, was "mkdocs-glightbox-0.3.3.tar", last modified: Thu Apr 20 14:43:58 2023, max compression
```

## Comparing `mkdocs-glightbox-0.3.2.tar` & `mkdocs-glightbox-0.3.3.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-03-19 10:26:50.670267 mkdocs-glightbox-0.3.2/
--rw-r--r--   0 blueswen   (501) staff       (20)     1065 2022-06-10 06:58:58.000000 mkdocs-glightbox-0.3.2/LICENSE
--rw-r--r--   0 blueswen   (501) staff       (20)       37 2022-07-15 16:30:44.000000 mkdocs-glightbox-0.3.2/MANIFEST.in
--rw-r--r--   0 blueswen   (501) staff       (20)     5252 2023-03-19 10:26:50.670126 mkdocs-glightbox-0.3.2/PKG-INFO
--rw-r--r--   0 blueswen   (501) staff       (20)     4826 2022-11-21 15:45:42.000000 mkdocs-glightbox-0.3.2/README.md
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-03-19 10:26:50.666226 mkdocs-glightbox-0.3.2/mkdocs_glightbox/
--rw-r--r--   0 blueswen   (501) staff       (20)        0 2022-06-12 06:19:32.000000 mkdocs-glightbox-0.3.2/mkdocs_glightbox/__init__.py
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-03-19 10:26:50.668049 mkdocs-glightbox-0.3.2/mkdocs_glightbox/__pycache__/
--rw-r--r--   0 blueswen   (501) staff       (20)      165 2022-11-15 14:31:20.000000 mkdocs-glightbox-0.3.2/mkdocs_glightbox/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 blueswen   (501) staff       (20)     5137 2023-03-19 10:01:50.000000 mkdocs-glightbox-0.3.2/mkdocs_glightbox/__pycache__/plugin.cpython-39.pyc
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-03-19 10:26:50.669095 mkdocs-glightbox-0.3.2/mkdocs_glightbox/glightbox/
--rw-r--r--   0 blueswen   (501) staff       (20)     1096 2022-06-10 06:42:44.000000 mkdocs-glightbox-0.3.2/mkdocs_glightbox/glightbox/LICENSE.md
--rw-r--r--   0 blueswen   (501) staff       (20)    13749 2022-06-07 11:18:17.000000 mkdocs-glightbox-0.3.2/mkdocs_glightbox/glightbox/glightbox.min.css
--rw-r--r--   0 blueswen   (501) staff       (20)    56280 2022-06-07 11:18:23.000000 mkdocs-glightbox-0.3.2/mkdocs_glightbox/glightbox/glightbox.min.js
--rw-r--r--   0 blueswen   (501) staff       (20)     7233 2023-03-19 10:01:43.000000 mkdocs-glightbox-0.3.2/mkdocs_glightbox/plugin.py
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-03-19 10:26:50.667596 mkdocs-glightbox-0.3.2/mkdocs_glightbox.egg-info/
--rw-r--r--   0 blueswen   (501) staff       (20)     5252 2023-03-19 10:26:50.000000 mkdocs-glightbox-0.3.2/mkdocs_glightbox.egg-info/PKG-INFO
--rw-r--r--   0 blueswen   (501) staff       (20)      567 2023-03-19 10:26:50.000000 mkdocs-glightbox-0.3.2/mkdocs_glightbox.egg-info/SOURCES.txt
--rw-r--r--   0 blueswen   (501) staff       (20)        1 2023-03-19 10:26:50.000000 mkdocs-glightbox-0.3.2/mkdocs_glightbox.egg-info/dependency_links.txt
--rw-r--r--   0 blueswen   (501) staff       (20)       69 2023-03-19 10:26:50.000000 mkdocs-glightbox-0.3.2/mkdocs_glightbox.egg-info/entry_points.txt
--rw-r--r--   0 blueswen   (501) staff       (20)       23 2023-03-19 10:26:50.000000 mkdocs-glightbox-0.3.2/mkdocs_glightbox.egg-info/requires.txt
--rw-r--r--   0 blueswen   (501) staff       (20)       17 2023-03-19 10:26:50.000000 mkdocs-glightbox-0.3.2/mkdocs_glightbox.egg-info/top_level.txt
--rw-r--r--   0 blueswen   (501) staff       (20)       38 2023-03-19 10:26:50.670313 mkdocs-glightbox-0.3.2/setup.cfg
--rw-rw-r--   0 blueswen   (501) staff       (20)      865 2023-03-19 10:08:31.000000 mkdocs-glightbox-0.3.2/setup.py
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-20 14:43:58.579763 mkdocs-glightbox-0.3.3/
+-rw-r--r--   0 blueswen   (501) staff       (20)     1065 2022-06-10 06:58:58.000000 mkdocs-glightbox-0.3.3/LICENSE
+-rw-r--r--   0 blueswen   (501) staff       (20)       37 2022-07-15 16:30:44.000000 mkdocs-glightbox-0.3.3/MANIFEST.in
+-rw-r--r--   0 blueswen   (501) staff       (20)     5205 2023-04-20 14:43:58.579565 mkdocs-glightbox-0.3.3/PKG-INFO
+-rw-r--r--   0 blueswen   (501) staff       (20)     4779 2023-04-20 14:30:58.000000 mkdocs-glightbox-0.3.3/README.md
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-20 14:43:58.577083 mkdocs-glightbox-0.3.3/mkdocs_glightbox/
+-rw-r--r--   0 blueswen   (501) staff       (20)        0 2022-06-12 06:19:32.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox/__init__.py
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-20 14:43:58.578438 mkdocs-glightbox-0.3.3/mkdocs_glightbox/__pycache__/
+-rw-r--r--   0 blueswen   (501) staff       (20)      165 2022-11-15 14:31:20.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 blueswen   (501) staff       (20)     6248 2023-04-20 14:34:14.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox/__pycache__/plugin.cpython-39.pyc
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-20 14:43:58.579110 mkdocs-glightbox-0.3.3/mkdocs_glightbox/glightbox/
+-rw-r--r--   0 blueswen   (501) staff       (20)     1096 2022-06-10 06:42:44.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox/glightbox/LICENSE.md
+-rw-r--r--   0 blueswen   (501) staff       (20)    13749 2022-06-07 11:18:17.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox/glightbox/glightbox.min.css
+-rw-r--r--   0 blueswen   (501) staff       (20)    56280 2022-06-07 11:18:23.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox/glightbox/glightbox.min.js
+-rw-r--r--   0 blueswen   (501) staff       (20)     8184 2023-04-20 14:27:45.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox/plugin.py
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2023-04-20 14:43:58.577937 mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/
+-rw-r--r--   0 blueswen   (501) staff       (20)     5205 2023-04-20 14:43:58.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/PKG-INFO
+-rw-r--r--   0 blueswen   (501) staff       (20)      528 2023-04-20 14:43:58.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/SOURCES.txt
+-rw-r--r--   0 blueswen   (501) staff       (20)        1 2023-04-20 14:43:58.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/dependency_links.txt
+-rw-r--r--   0 blueswen   (501) staff       (20)       69 2023-04-20 14:43:58.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/entry_points.txt
+-rw-r--r--   0 blueswen   (501) staff       (20)       17 2023-04-20 14:43:58.000000 mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/top_level.txt
+-rw-r--r--   0 blueswen   (501) staff       (20)       38 2023-04-20 14:43:58.579810 mkdocs-glightbox-0.3.3/setup.cfg
+-rw-rw-r--   0 blueswen   (501) staff       (20)      816 2023-04-20 14:30:38.000000 mkdocs-glightbox-0.3.3/setup.py
```

### Comparing `mkdocs-glightbox-0.3.2/LICENSE` & `mkdocs-glightbox-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.2/PKG-INFO` & `mkdocs-glightbox-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-glightbox
-Version: 0.3.2
+Version: 0.3.3
 Summary: MkDocs plugin supports image lightbox with GLightbox.
 Home-page: https://blueswen.github.io/mkdocs-glightbox
 Author: Blueswen
 Author-email: blueswen.tw@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/Blueswen/mkdocs-glightbox
 Keywords: mkdocs,plugin,lightbox
@@ -24,17 +24,15 @@
 
 GLightbox is a pure javascript lightbox library with mobile support.
 
 [Live demo](https://blueswen.github.io/mkdocs-glightbox/) with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).
 
 ## Dependency
 
-1. Python Package
-   1. beautifulsoup4>=4.11.1
-2. GLightbox javascript file and CSS file
+1. GLightbox javascript file and CSS file
    1. GLightbox==3.2.0
 
 ## Usage
 
 1. Install the plugin from PyPI
 
     ```bash
```

### Comparing `mkdocs-glightbox-0.3.2/README.md` & `mkdocs-glightbox-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 
 GLightbox is a pure javascript lightbox library with mobile support.
 
 [Live demo](https://blueswen.github.io/mkdocs-glightbox/) with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).
 
 ## Dependency
 
-1. Python Package
-   1. beautifulsoup4>=4.11.1
-2. GLightbox javascript file and CSS file
+1. GLightbox javascript file and CSS file
    1. GLightbox==3.2.0
 
 ## Usage
 
 1. Install the plugin from PyPI
 
     ```bash
```

### Comparing `mkdocs-glightbox-0.3.2/mkdocs_glightbox/glightbox/LICENSE.md` & `mkdocs-glightbox-0.3.3/mkdocs_glightbox/glightbox/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.2/mkdocs_glightbox/glightbox/glightbox.min.css` & `mkdocs-glightbox-0.3.3/mkdocs_glightbox/glightbox/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.2/mkdocs_glightbox/glightbox/glightbox.min.js` & `mkdocs-glightbox-0.3.3/mkdocs_glightbox/glightbox/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.2/mkdocs_glightbox/plugin.py` & `mkdocs-glightbox-0.3.3/mkdocs_glightbox/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import logging
 import os
+import re
 
-from bs4 import BeautifulSoup
 from mkdocs import utils
 from mkdocs.config import config_options
 from mkdocs.plugins import BasePlugin
 
 log = logging.getLogger(__name__)
 base_path = os.path.dirname(os.path.abspath(__file__))
 
@@ -36,117 +36,142 @@
 
     def on_post_page(self, output, page, config, **kwargs):
         """Add css link tag, javascript script tag, and javascript code to initialize GLightbox"""
         # skip page with meta glightbox is false
         if "glightbox" in page.meta and page.meta.get("glightbox", True) is False:
             return output
 
-        soup = BeautifulSoup(output, "html.parser")
-
-        if soup.head:
-            css_link = soup.new_tag("link")
-            css_link.attrs["href"] = utils.get_relative_url(
-                utils.normalize_url("assets/stylesheets/glightbox.min.css"), page.url
-            )
-            css_link.attrs["rel"] = "stylesheet"
-            soup.head.append(css_link)
-
-            css_patch = soup.new_tag("style")
-            css_patch.string = """
-            html.glightbox-open { overflow: initial; height: 100%; }
-            .gslide-title { margin-top: 0px; user-select: text; }
-            .gslide-desc { color: #666; user-select: text; }
-            .gslide-image img { background: white; }
+        # Define regular expressions for matching the relevant sections of the HTML code
+        head_regex = re.compile(r"<head>(.*?)<\/head>", flags=re.DOTALL)
+        body_regex = re.compile(r"<body(.*?)<\/body>", flags=re.DOTALL)
+
+        # Modify the CSS link
+        css_link = f'<link href="{utils.get_relative_url(utils.normalize_url("assets/stylesheets/glightbox.min.css"), page.url)}" rel="stylesheet"/>'
+        output = head_regex.sub(f"<head>\\1 {css_link}</head>", output)
+
+        # Modify the CSS patch
+        css_patch = """
+        html.glightbox-open { overflow: initial; height: 100%; }
+        .gslide-title { margin-top: 0px; user-select: text; }
+        .gslide-desc { color: #666; user-select: text; }
+        .gslide-image img { background: white; }
+        """
+        if config["theme"].name == "material":
+            css_patch += """
+            .gscrollbar-fixer { padding-right: 15px; }
+            .gdesc-inner { font-size: 0.75rem; }
+            body[data-md-color-scheme="slate"] .gdesc-inner { background: var(--md-default-bg-color);}
+            body[data-md-color-scheme="slate"] .gslide-title { color: var(--md-default-fg-color);}
+            body[data-md-color-scheme="slate"] .gslide-desc { color: var(--md-default-fg-color);}
             """
-            if config["theme"].name == "material":
-                css_patch.string += """
-                .gscrollbar-fixer { padding-right: 15px; }
-                .gdesc-inner { font-size: 0.75rem; }
-                body[data-md-color-scheme="slate"] .gdesc-inner { background: var(--md-default-bg-color);}
-                body[data-md-color-scheme="slate"] .gslide-title { color: var(--md-default-fg-color);}
-                body[data-md-color-scheme="slate"] .gslide-desc { color: var(--md-default-fg-color);}
-                """
-            soup.head.append(css_patch)
-
-            js_script = soup.new_tag("script")
-            js_script.attrs["src"] = utils.get_relative_url(
-                utils.normalize_url("assets/javascripts/glightbox.min.js"), page.url
-            )
-            soup.head.append(js_script)
-
-            js_code = soup.new_tag("script")
-            plugin_config = dict(self.config)
-            lb_config = {
-                k: plugin_config[k]
-                for k in ["touchNavigation", "loop", "zoomable", "draggable"]
-            }
-            lb_config["openEffect"] = plugin_config.get("effect", "zoom")
-            lb_config["closeEffect"] = plugin_config.get("effect", "zoom")
-            lb_config["slideEffect"] = plugin_config.get("slide_effect", "slide")
-            js_code.string = f"const lightbox = GLightbox({json.dumps(lb_config)});"
-            if config["theme"].name == "material" or "navigation.instant" in config[
-                "theme"
-            ]._vars.get("features", []):
-                # support compatible with mkdocs-material Instant loading feature
-                js_code.string = "document$.subscribe(() => {" + js_code.string + "})"
-            soup.body.append(js_code)
+        output = head_regex.sub(f"<head>\\1<style>{css_patch}</style></head>", output)
+
+        # Modify the JS script
+        js_script = f'<script src="{utils.get_relative_url(utils.normalize_url("assets/javascripts/glightbox.min.js"), page.url)}"></script>'
+        output = head_regex.sub(f"<head>\\1 {js_script}</head>", output)
+
+        # Modify the JS code
+        plugin_config = dict(self.config)
+        lb_config = {
+            k: plugin_config[k]
+            for k in ["touchNavigation", "loop", "zoomable", "draggable"]
+        }
+        lb_config["openEffect"] = plugin_config.get("effect", "zoom")
+        lb_config["closeEffect"] = plugin_config.get("effect", "zoom")
+        lb_config["slideEffect"] = plugin_config.get("slide_effect", "slide")
+        js_code = f"const lightbox = GLightbox({json.dumps(lb_config)});"
+        if config["theme"].name == "material" or "navigation.instant" in config[
+            "theme"
+        ]._vars.get("features", []):
+            # support compatible with mkdocs-material Instant loading feature
+            js_code = "document$.subscribe(() => {" + js_code + "})"
+        output = body_regex.sub(f"<body\\1<script>{js_code}</script></body>", output)
 
-        return str(soup)
+        return output
 
     def on_page_content(self, html, page, config, **kwargs):
         """Wrap img tag with anchor tag with glightbox class and attributes from config"""
         # skip page with meta glightbox is false
         if "glightbox" in page.meta and page.meta.get("glightbox", True) is False:
             return html
         plugin_config = {k: dict(self.config)[k] for k in ["width", "height"]}
         # skip emoji img with index as class name from pymdownx.emoji https://facelessuser.github.io/pymdown-extensions/extensions/emoji/
         skip_class = ["emojione", "twemoji", "gemoji"]
         # skip image with off-glb and specific class
         skip_class += ["off-glb"] + self.config["skip_classes"]
-        soup = BeautifulSoup(html, "html.parser")
-        imgs = soup.find_all("img")
-        for img in imgs:
-            if set(skip_class) & set(img.get("class", [])) or img.parent.name == "a":
-                continue
-            a = soup.new_tag("a")
-            a["class"] = "glightbox"
-            a["href"] = img.get("src", "")
-            a["data-type"] = "image"
-            # setting data-width and data-height with plugin options
-            for k, v in plugin_config.items():
-                a[f"data-{k}"] = v
-            slide_options = ["title", "description", "caption-position", "gallery"]
-            for option in slide_options:
-                attr = f"data-{option}"
-                if attr == "data-title":
-                    # alt as title when auto_caption is enabled
-                    if self.config["auto_caption"] or (
-                        "glightbox.auto_caption" in page.meta
-                        and page.meta.get("glightbox.auto_caption", False) is True
-                    ):
-                        val = img.get("data-title", img.get("alt", ""))
-                    else:
-                        val = img.get("data-title", "")
-                elif attr == "data-caption-position":
-                    # plugin option caption_position as default
-                    val = img.get(
-                        "data-caption-position", self.config["caption_position"]
+
+        # Use regex to find image tags that need to be wrapped with anchor tags and image tags already wrapped with anchor tags
+        pattern = re.compile(
+            r"<a\b[^>]*>(?:\s*<[^>]+>\s*)*<img\b[^>]*>(?:\s*<[^>]+>\s*)*</a>|<img(?P<attr>.*?)>"
+        )
+        html = pattern.sub(
+            lambda match: self.wrap_img_with_anchor(
+                match, plugin_config, skip_class, page.meta
+            ),
+            html,
+        )
+
+        return html
+
+    def wrap_img_with_anchor(self, match, plugin_config, skip_class, meta):
+        """Wrap image tags with anchor tags"""
+        a_pattern = re.compile(r"<a(?P<attr>.*?)>")
+        if a_pattern.match(match.group(0)):
+            return match.group(0)
+
+        img_tag = match.group(0)
+        img_attr = match.group("attr")
+        classes = re.findall(r'class="([^"]+)"', img_attr)
+        classes = [c for match in classes for c in match.split()]
+
+        if set(skip_class) & set(classes):
+            return img_tag
+
+        src = re.search(r"src=[\"\']([^\"\']+)", img_attr).group(1)
+        a_tag = f'<a class="glightbox" href="{src}" data-type="image"'
+        # setting data-width and data-height with plugin options
+        for k, v in plugin_config.items():
+            a_tag += f' data-{k}="{v}"'
+        slide_options = [
+            "title",
+            "description",
+            "caption-position",
+            "gallery",
+        ]
+        for option in slide_options:
+            attr = f"data-{option}"
+            if attr == "data-title":
+                val = re.search(r"data-title=[\"\']([^\"\']+)", img_attr)
+                if self.config["auto_caption"] or (
+                    "glightbox.auto_caption" in meta
+                    and meta.get("glightbox.auto_caption", False) is True
+                ):
+                    val = (
+                        val.group(1)
+                        if val
+                        else re.search(r"alt=[\"\']([^\"\']+)", img_attr).group(1)
                     )
                 else:
-                    val = img.get(attr, "")
-
-                # skip val is empty
-                if val != "":
-                    # convert data-caption-position to data-desc-position
-                    if attr == "data-caption-position":
-                        a["data-desc-position"] = val
-                    else:
-                        a[attr] = val
-            img.wrap(a)
-        return str(soup)
+                    val = val.group(1) if val else ""
+            elif attr == "data-caption-position":
+                val = re.search(r"data-caption-position=[\"\']([^\"\']+)", img_attr)
+                val = val.group(1) if val else self.config["caption_position"]
+            else:
+                val = re.search(f"{attr}=[\"']([^\"']+)", img_attr)
+                val = val.group(1) if val else ""
+
+            # skip val is empty
+            if val != "":
+                # convert data-caption-position to data-desc-position
+                if attr == "data-caption-position":
+                    a_tag += f' data-desc-position="{val}"'
+                else:
+                    a_tag += f' {attr}="{val}"'
+        a_tag += f">{img_tag}</a>"
+        return a_tag
 
     def on_post_build(self, config, **kwargs):
         """Copy glightbox"s css and js files to assets directory"""
 
         output_base_path = os.path.join(config["site_dir"], "assets")
         css_path = os.path.join(output_base_path, "stylesheets")
         utils.copy_file(
```

### Comparing `mkdocs-glightbox-0.3.2/mkdocs_glightbox.egg-info/PKG-INFO` & `mkdocs-glightbox-0.3.3/mkdocs_glightbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-glightbox
-Version: 0.3.2
+Version: 0.3.3
 Summary: MkDocs plugin supports image lightbox with GLightbox.
 Home-page: https://blueswen.github.io/mkdocs-glightbox
 Author: Blueswen
 Author-email: blueswen.tw@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/Blueswen/mkdocs-glightbox
 Keywords: mkdocs,plugin,lightbox
@@ -24,17 +24,15 @@
 
 GLightbox is a pure javascript lightbox library with mobile support.
 
 [Live demo](https://blueswen.github.io/mkdocs-glightbox/) with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).
 
 ## Dependency
 
-1. Python Package
-   1. beautifulsoup4>=4.11.1
-2. GLightbox javascript file and CSS file
+1. GLightbox javascript file and CSS file
    1. GLightbox==3.2.0
 
 ## Usage
 
 1. Install the plugin from PyPI
 
     ```bash
```

### Comparing `mkdocs-glightbox-0.3.2/setup.py` & `mkdocs-glightbox-0.3.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mkdocs-glightbox",
-    version="0.3.2",
+    version="0.3.3",
     author="Blueswen",
     author_email="blueswen.tw@gmail.com",
     url="https://blueswen.github.io/mkdocs-glightbox",
     project_urls={
         "Source": "https://github.com/Blueswen/mkdocs-glightbox",
     },
     keywords=["mkdocs", "plugin", "lightbox"],
     packages=find_packages(),
     license="MIT",
     description="MkDocs plugin supports image lightbox with GLightbox.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["beautifulsoup4>=4.11.1"],
     include_package_data=True,
     entry_points={
         "mkdocs.plugins": [
             "glightbox = mkdocs_glightbox.plugin:LightboxPlugin",
         ]
     },
 )
```

