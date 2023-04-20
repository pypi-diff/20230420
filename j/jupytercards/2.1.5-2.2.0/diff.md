# Comparing `tmp/jupytercards-2.1.5.tar.gz` & `tmp/jupytercards-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupytercards-2.1.5.tar", last modified: Wed Apr  5 19:43:52 2023, max compression
+gzip compressed data, was "jupytercards-2.2.0.tar", last modified: Thu Apr 20 17:27:01 2023, max compression
```

## Comparing `jupytercards-2.1.5.tar` & `jupytercards-2.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.1.5/.gitignore
--rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.1.5/LICENSE
--rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.1.5/Markdown-flashcards.ipynb
--rw-r--r--   0        0        0     3763 2022-11-18 02:28:35.734112 jupytercards-2.1.5/README.md
--rw-r--r--   0        0        0    23266 2022-09-09 14:44:12.606945 jupytercards-2.1.5/example.ipynb
--rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.1.5/extractdefinitions.py
--rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.1.5/flashcards.gif
--rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.1.5/google73e9274d2fa18926.html
--rw-r--r--   0        0        0      657 2023-04-05 19:43:13.229475 jupytercards-2.1.5/jupytercards/__init__.py
--rw-r--r--   0        0        0     5980 2022-09-09 14:44:12.608062 jupytercards-2.1.5/jupytercards/dynamic.py
--rw-r--r--   0        0        0     9879 2022-09-09 14:44:12.609234 jupytercards-2.1.5/jupytercards/flashcards.js
--rw-r--r--   0        0        0     4217 2023-04-05 19:40:51.851785 jupytercards-2.1.5/jupytercards/styles.css
--rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.1.5/jupytercards/swiped-events.min.js
--rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.1.5/pyproject.toml
--rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 jupytercards-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.2.0/.gitignore
+-rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.2.0/LICENSE
+-rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.2.0/Markdown-flashcards.ipynb
+-rw-r--r--   0        0        0     3763 2022-11-18 02:28:35.734112 jupytercards-2.2.0/README.md
+-rw-r--r--   0        0        0    23266 2022-09-09 14:44:12.606945 jupytercards-2.2.0/example.ipynb
+-rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.2.0/extractdefinitions.py
+-rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.2.0/flashcards.gif
+-rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.2.0/google73e9274d2fa18926.html
+-rw-r--r--   0        0        0      657 2023-04-20 17:26:35.018537 jupytercards-2.2.0/jupytercards/__init__.py
+-rw-r--r--   0        0        0     6042 2023-04-20 15:22:14.070372 jupytercards-2.2.0/jupytercards/dynamic.py
+-rw-r--r--   0        0        0     9930 2023-04-20 17:13:57.229194 jupytercards-2.2.0/jupytercards/flashcards.js
+-rw-r--r--   0        0        0     4217 2023-04-05 19:40:51.851785 jupytercards-2.2.0/jupytercards/styles.css
+-rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.2.0/jupytercards/swiped-events.min.js
+-rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 jupytercards-2.2.0/PKG-INFO
```

### Comparing `jupytercards-2.1.5/.gitignore` & `jupytercards-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupytercards-2.1.5/LICENSE` & `jupytercards-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercards-2.1.5/Markdown-flashcards.ipynb` & `jupytercards-2.2.0/Markdown-flashcards.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.1.5/README.md` & `jupytercards-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jupytercards-2.1.5/example.ipynb` & `jupytercards-2.2.0/example.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.1.5/extractdefinitions.py` & `jupytercards-2.2.0/extractdefinitions.py`

 * *Files identical despite different names*

### Comparing `jupytercards-2.1.5/flashcards.gif` & `jupytercards-2.2.0/flashcards.gif`

 * *Files identical despite different names*

### Comparing `jupytercards-2.1.5/jupytercards/__init__.py` & `jupytercards-2.2.0/jupytercards/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.1.5'
+__version__ = '2.2.0'
 from .dynamic import display_flashcards, md2json
```

### Comparing `jupytercards-2.1.5/jupytercards/dynamic.py` & `jupytercards-2.2.0/jupytercards/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from IPython.core.display import display,  HTML, Javascript
 import string
 import random
 import json
 import urllib.request
 import pkg_resources
 
-def display_flashcards(ref, keyControl = True):
+def display_flashcards(ref, keyControl = True, grabFocus=False):
 
     resource_package = __name__
     styles = "<style>\n"
     css = pkg_resources.resource_string(resource_package, "styles.css")
     styles += css.decode("utf-8")
     styles += "\n</style>"
 
@@ -77,33 +77,33 @@
         raise Exception("First argument must be list (JSON), URL, or file ref")
 
     loadData += ''';
     '''
     
     if static:
         loadData += f'''
-        createCards("{div_id}", "{keyControl}");
+        createCards("{div_id}", "{keyControl}", "{grabFocus}");
         '''
 
         print()
     else:
         loadData += f'''
 
         {{
         const jmscontroller = new AbortController();
         const signal = jmscontroller.signal;
 
         setTimeout(() => jmscontroller.abort(), 5000);
 
         fetch("{url}", {{signal}})
         .then(response => response.json())
-        .then(json => createCards("{div_id}", "{keyControl}"))
+        .then(json => createCards("{div_id}", "{keyControl}", "{grabFocus}"))
         .catch(err => {{
         console.log("Fetch error or timeout");
-        createCards("{div_id}", "{keyControl}");
+        createCards("{div_id}", "{keyControl}", "{grabFocus}");
         }});
         }}
         '''
         #loadData+=url+script_end
 
 
     #print(loadData)
```

### Comparing `jupytercards-2.1.5/jupytercards/flashcards.js` & `jupytercards-2.2.0/jupytercards/flashcards.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -37,14 +37,15 @@
     return mystring;
 }
 
 window.flipCard = function flipCard(ths) {
     console.log(ths);
     console.log(ths.id);
     ths.classList.toggle("flip");
+    ths.focus();
     var next = document.getElementById(ths.id + '-next');
     next.style.pointerEvents = 'none';
     /* ths.blur(); */
     next.classList.add('flipped');
     if (typeof MathJax != 'undefined') {
         var version = MathJax.version;
         console.log('MathJax version', version);
@@ -236,15 +237,15 @@
 
 }
 
 
 
 
 
-function createCards(id, keyControl) {
+function createCards(id, keyControl, grabFocus) {
     console.log(id);
 
     var mydiv = document.getElementById(id);
     /*mydiv.onclick = window.flipCard(mydiv);*/
     /*
     mydiv.addEventListener('click', function(){window.flipCard(mydiv);}, false);
     mydiv.addEventListener('keydown', function(event){window.checkKey(mydiv,event);}, true);
@@ -322,11 +323,12 @@
         // Don't show next if no other cards!
         next.style.pointerEvents = 'none';
         next.classList.add('hide');
     } else {
         next.innerHTML = "Next >";
     }
 
-    mydiv.focus();
+    if (grabFocus)
+        mydiv.focus();
 
     return flipper;
 }
```

### Comparing `jupytercards-2.1.5/jupytercards/styles.css` & `jupytercards-2.2.0/jupytercards/styles.css`

 * *Files identical despite different names*

### Comparing `jupytercards-2.1.5/jupytercards/swiped-events.min.js` & `jupytercards-2.2.0/jupytercards/swiped-events.min.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.1.5/PKG-INFO` & `jupytercards-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupytercards
-Version: 2.1.5
+Version: 2.2.0
 Summary: Module to display dynamic quizzes in Jupyter notebooks and Jupyter Books. Uses JavaScript to provide
 Home-page: https://github.com/jmshea/jupytercards
 Author: John M. Shea
 Author-email: jshea@ieee.org
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```

