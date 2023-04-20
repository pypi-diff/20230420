# Comparing `tmp/ansys-sphinx-theme-0.9.7.tar.gz` & `tmp/ansys-sphinx-theme-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-sphinx-theme-0.9.7.tar", last modified: Mon Apr 10 08:29:28 2023, max compression
+gzip compressed data, was "ansys-sphinx-theme-0.9.8.tar", last modified: Thu Apr 20 13:32:49 2023, max compression
```

## Comparing `ansys-sphinx-theme-0.9.7.tar` & `ansys-sphinx-theme-0.9.8.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0     1089 2023-04-10 08:29:14.208554 ansys-sphinx-theme-0.9.7/LICENSE
--rw-r--r--   0        0        0     4224 2023-04-10 08:29:14.208554 ansys-sphinx-theme-0.9.7/README.rst
--rw-r--r--   0        0        0     2175 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     3919 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/__init__.py
--rw-r--r--   0        0        0       78 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/examples/__init__.py
--rw-r--r--   0        0        0      726 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/examples/sample_func.py
--rw-r--r--   0        0        0     6335 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/examples/samples.py
--rw-r--r--   0        0        0      755 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/examples/type_hint_example.py
--rw-r--r--   0        0        0      423 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/latex/404.html
--rw-r--r--   0        0        0     2432 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/latex/__init__.py
--rw-r--r--   0        0        0     4523 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/latex/cover.tex
--rw-r--r--   0        0        0      102 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/base.rst
--rw-r--r--   0        0        0      606 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      391 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/announcement_version.html
--rw-r--r--   0        0        0      237 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/breadcrumbs.html
--rw-r--r--   0        0        0     2560 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/search-field.html
--rw-r--r--   0        0        0     1183 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/layout.html
--rw-r--r--   0        0        0      175 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/404.rst
--rw-r--r--   0        0        0      327 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys-favicon.png
--rw-r--r--   0        0        0    45165 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black.jpg
--rw-r--r--   0        0        0    50754 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black_cropped.jpg
--rw-r--r--   0        0        0     4788 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white.pdf
--rw-r--r--   0        0        0     4503 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white_cropped.pdf
--rw-r--r--   0        0        0    19674 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/ansys_sphinx_theme.css
--rw-r--r--   0        0        0     1133 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/breadcrumbs.css
--rw-r--r--   0        0        0     2626 2023-04-10 08:29:14.212554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/meilisearch.css
--rw-r--r--   0        0        0   268588 2023-04-10 08:29:14.216554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Light.ttf
--rw-r--r--   0        0        0   269108 2023-04-10 08:29:14.216554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Regular.ttf
--rw-r--r--   0        0        0   268280 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-SemiBold.ttf
--rw-r--r--   0        0        0      227 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/js/download_target_blank.js
--rw-r--r--   0        0        0       76 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/js/table.js
--rw-r--r--   0        0        0    54761 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0    54600 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-white-cropped.png
--rw-r--r--   0        0        0    54836 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark.png
--rw-r--r--   0        0        0    32456 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark_square.png
--rw-r--r--   0        0        0    54325 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light.png
--rw-r--r--   0        0        0    31713 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light_square.png
--rw-r--r--   0        0        0     1729 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/watermark.pdf
--rw-r--r--   0        0        0      326 2023-04-10 08:29:14.220554 ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/theme.conf
--rw-r--r--   0        0        0     5624 1970-01-01 00:00:00.000000 ansys-sphinx-theme-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/LICENSE
+-rw-r--r--   0        0        0     4224 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/README.rst
+-rw-r--r--   0        0        0     2172 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     4933 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/__init__.py
+-rw-r--r--   0        0        0       78 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/examples/__init__.py
+-rw-r--r--   0        0        0      726 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/examples/sample_func.py
+-rw-r--r--   0        0        0     6335 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/examples/samples.py
+-rw-r--r--   0        0        0      755 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/examples/type_hint_example.py
+-rw-r--r--   0        0        0      423 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/latex/404.html
+-rw-r--r--   0        0        0     2432 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/latex/__init__.py
+-rw-r--r--   0        0        0     4523 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/latex/cover.tex
+-rw-r--r--   0        0        0      102 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0      606 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      391 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/announcement_version.html
+-rw-r--r--   0        0        0      237 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/breadcrumbs.html
+-rw-r--r--   0        0        0     2560 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/search-field.html
+-rw-r--r--   0        0        0      557 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/theme-version.html
+-rw-r--r--   0        0        0     1183 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/layout.html
+-rw-r--r--   0        0        0      175 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/404.rst
+-rw-r--r--   0        0        0      327 2023-04-20 13:32:34.984655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys-favicon.png
+-rw-r--r--   0        0        0    45165 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black.jpg
+-rw-r--r--   0        0        0    50754 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black_cropped.jpg
+-rw-r--r--   0        0        0     4788 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white.pdf
+-rw-r--r--   0        0        0     4503 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white_cropped.pdf
+-rw-r--r--   0        0        0    19674 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/ansys_sphinx_theme.css
+-rw-r--r--   0        0        0     1133 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/breadcrumbs.css
+-rw-r--r--   0        0        0     2626 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/meilisearch.css
+-rw-r--r--   0        0        0   268588 2023-04-20 13:32:34.988655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Light.ttf
+-rw-r--r--   0        0        0   269108 2023-04-20 13:32:34.992655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Regular.ttf
+-rw-r--r--   0        0        0   268280 2023-04-20 13:32:34.992655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-SemiBold.ttf
+-rw-r--r--   0        0        0      227 2023-04-20 13:32:34.992655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/js/download_target_blank.js
+-rw-r--r--   0        0        0       76 2023-04-20 13:32:34.992655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/js/table.js
+-rw-r--r--   0        0        0    54761 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0    54600 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-white-cropped.png
+-rw-r--r--   0        0        0    54836 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark.png
+-rw-r--r--   0        0        0    32456 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark_square.png
+-rw-r--r--   0        0        0    54325 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light.png
+-rw-r--r--   0        0        0    31713 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light_square.png
+-rw-r--r--   0        0        0     1729 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/watermark.pdf
+-rw-r--r--   0        0        0      358 2023-04-20 13:32:34.996655 ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/theme.conf
+-rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 ansys-sphinx-theme-0.9.8/PKG-INFO
```

### Comparing `ansys-sphinx-theme-0.9.7/LICENSE` & `ansys-sphinx-theme-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/README.rst` & `ansys-sphinx-theme-0.9.8/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/pyproject.toml` & `ansys-sphinx-theme-0.9.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,26 +21,26 @@
     "Framework :: Sphinx",
     "Framework :: Sphinx :: Theme",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "Sphinx>=4.2.0,<6",
+    "Sphinx>=4.2.0",
     "pydata-sphinx-theme==0.13.3",
     "Jinja2>=3.1.2",
 ]
 
 [project.optional-dependencies]
 doc = [
     "numpydoc==1.5.0",
-    "Sphinx==5.3.0",
-    "sphinx-copybutton==0.5.1",
+    "Sphinx==6.1.3",
+    "sphinx-copybutton==0.5.2",
     "sphinx-notfound-page==0.8.3",
-    "sphinx-design==0.3.0",
+    "sphinx-design==0.4.1",
     "bs4==0.0.1",
     "html5lib==1.1",
     "requests==2.28.2",
     "sphinx-jinja==2.0.2",
 ]
 
 [project.entry-points."sphinx.html_themes"]
```

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/__init__.py` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """This is the ansys-sphinx-theme module."""
 import pathlib
-from typing import Dict
+from typing import Any, Dict
 
+from docutils.nodes import document
 from sphinx.application import Sphinx
 
 from ansys_sphinx_theme.latex import generate_404  # noqa: F401
 
-__version__ = "0.9.7"
+__version__ = "0.9.8"
 
 # Declare the fundamental paths of the theme
 THIS_PATH = pathlib.Path(__file__).parent.resolve()
 THEME_PATH = THIS_PATH / "theme" / "ansys_sphinx_theme"
 STATIC_PATH = THEME_PATH / "static"
 STYLE_PATH = STATIC_PATH / "css"
 JS_PATH = STATIC_PATH / "js"
@@ -80,14 +81,39 @@
     if app.config.html_theme_options.get("switcher"):
         app.config.html_theme_options.setdefault(
             "navbar_end", ["version-switcher", "theme-switcher", "navbar-icon-links"]
         )
     app.config.html_theme_options.setdefault("collapse_navigation", True)
 
 
+def update_footer_theme(
+    app: Sphinx, pagename: str, templatename: str, context: Dict[str, Any], doctree: document
+) -> None:
+    """Update the version number of the Ansys Sphinx theme in the footer.
+
+    Connect to the Sphinx application instance for rendering the documentation,
+    and add the current version number of the Ansys Sphinx theme to the page context.
+    This allows the theme to update the footer with the current version number.
+
+    Parameters
+    ----------
+    app : ~sphinx.application.Sphinx
+        Application instance for rendering the documentation.
+    pagename : str
+        The name of the current page.
+    templatename : str
+        The name of the template being used.
+    context : dict
+        The context dictionary for the page.
+    doctree : ~docutils.nodes.document
+        The document tree for the page.
+    """
+    context["ansys_sphinx_theme_version"] = __version__
+
+
 def setup(app: Sphinx) -> Dict:
     """Connect to the sphinx theme app.
 
     Parameters
     ----------
     app : ~sphinx.application.Sphinx
         Application instance for rendering the documentation.
@@ -109,14 +135,15 @@
     # Verify that the main CSS file exists
     if not CSS_PATH.exists():
         raise FileNotFoundError(f"Unable to locate ansys-sphinx theme at {CSS_PATH.absolute()}")
     app.add_css_file(str(CSS_PATH.relative_to(STATIC_PATH)))
     app.add_js_file(str(JS_FILE.relative_to(STATIC_PATH)))
     app.add_js_file("https://cdn.datatables.net/1.10.23/js/jquery.dataTables.min.js")
     app.add_css_file("https://cdn.datatables.net/1.10.23/css/jquery.dataTables.min.css")
+    app.connect("html-page-context", update_footer_theme)
     # Add templates for autosummary
     app.config.templates_path.append(str(TEMPLATES_PATH))
 
     return {
         "version": __version__,
         "parallel_read_safe": True,
         "parallel_write_safe": True,
```

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/examples/sample_func.py` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/examples/sample_func.py`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/examples/samples.py` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/examples/samples.py`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/examples/type_hint_example.py` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/examples/type_hint_example.py`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/latex/__init__.py` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/latex/cover.tex` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/latex/cover.tex`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/class.rst` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/search-field.html` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/components/search-field.html`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/layout.html` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black.jpg` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black.jpg`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black_cropped.jpg` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_black_cropped.jpg`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white.pdf` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white.pdf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white_cropped.pdf` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/ansys_logo_white_cropped.pdf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/ansys_sphinx_theme.css` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/ansys_sphinx_theme.css`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/breadcrumbs.css` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/breadcrumbs.css`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/meilisearch.css` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/css/meilisearch.css`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Light.ttf` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Light.ttf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Regular.ttf` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-SemiBold.ttf` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/fonts/SourceSansPro-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-black-cropped.png` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-white-cropped.png` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys-logo-white-cropped.png`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark.png` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark.png`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark_square.png` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_dark_square.png`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light.png` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light.png`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light_square.png` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/pyansys_light_square.png`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/watermark.pdf` & `ansys-sphinx-theme-0.9.8/src/ansys_sphinx_theme/theme/ansys_sphinx_theme/static/watermark.pdf`

 * *Files identical despite different names*

### Comparing `ansys-sphinx-theme-0.9.7/PKG-INFO` & `ansys-sphinx-theme-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: ansys-sphinx-theme
-Version: 0.9.7
+Version: 0.9.8
 Summary: A theme devised by ANSYS, Inc. for Sphinx documentation.
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: Sphinx>=4.2.0,<6
+Requires-Dist: Sphinx>=4.2.0
 Requires-Dist: pydata-sphinx-theme==0.13.3
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
-Requires-Dist: Sphinx==5.3.0 ; extra == "doc"
-Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
+Requires-Dist: Sphinx==6.1.3 ; extra == "doc"
+Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
-Requires-Dist: sphinx-design==0.3.0 ; extra == "doc"
+Requires-Dist: sphinx-design==0.4.1 ; extra == "doc"
 Requires-Dist: bs4==0.0.1 ; extra == "doc"
 Requires-Dist: html5lib==1.1 ; extra == "doc"
 Requires-Dist: requests==2.28.2 ; extra == "doc"
 Requires-Dist: sphinx-jinja==2.0.2 ; extra == "doc"
 Project-URL: Documentation, https://sphinxdocs.ansys.com/
 Project-URL: Home, https://sphinxdocs.ansys.com/
 Project-URL: Source, https://github.com/ansys/ansys-sphinx-theme
```

