# Comparing `tmp/strplus-1.0.2.tar.gz` & `tmp/strplus-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strplus-1.0.2.tar", max compression
+gzip compressed data, was "strplus-1.0.3.tar", max compression
```

## Comparing `strplus-1.0.2.tar` & `strplus-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-1.0.2/LICENSE
--rw-r--r--   0        0        0     2835 2023-04-19 13:50:23.887228 strplus-1.0.2/README.md
--rw-r--r--   0        0        0      876 2023-04-19 13:50:38.307230 strplus-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      161 2023-04-19 13:41:19.627394 strplus-1.0.2/strplus/__init__.py
--rw-r--r--   0        0        0     4243 2023-04-19 13:41:19.627394 strplus-1.0.2/strplus/cases.py
--rw-r--r--   0        0        0      542 2023-04-19 13:41:19.627394 strplus-1.0.2/strplus/functions.py
--rw-r--r--   0        0        0     4231 2023-04-19 13:41:19.627394 strplus-1.0.2/strplus/strplus.py
--rw-r--r--   0        0        0     3491 1970-01-01 00:00:00.000000 strplus-1.0.2/setup.py
--rw-r--r--   0        0        0     3463 1970-01-01 00:00:00.000000 strplus-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2840 2023-04-20 18:44:25.544135 strplus-1.0.3/README.md
+-rw-r--r--   0        0        0     1027 2023-04-20 18:44:25.554135 strplus-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-04-20 18:44:25.554135 strplus-1.0.3/strplus/__init__.py
+-rw-r--r--   0        0        0     4271 2023-04-20 18:45:53.984107 strplus-1.0.3/strplus/cases.py
+-rw-r--r--   0        0        0      722 2023-04-20 18:44:25.554135 strplus-1.0.3/strplus/functions.py
+-rw-r--r--   0        0        0     4316 2023-04-20 18:46:05.964103 strplus-1.0.3/strplus/strplus.py
+-rw-r--r--   0        0        0     3496 1970-01-01 00:00:00.000000 strplus-1.0.3/setup.py
+-rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 strplus-1.0.3/PKG-INFO
```

### Comparing `strplus-1.0.2/LICENSE` & `strplus-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `strplus-1.0.2/README.md` & `strplus-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 ---
 
 <br>
 <br>
 
 <a href="https://github.com/wiseupdata/wiseupdata">
-<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/python.png" width="300" />
+<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/imgs/python.png" width="300" />
 </a>
 
 <h1>
 Python extra functions for strings ❤️
 </h1>
 
 <br>
```

### Comparing `strplus-1.0.2/pyproject.toml` & `strplus-1.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strplus"
-version = "1.0.2"
+version = "1.0.3"
 authors = ["Silvio Liborio <silvio.liborio@wiseupdata.com>"]
 readme = "README.md"
 
 description = "Python extra functions for strings"
 
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -18,20 +18,24 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 ipykernel = "^6.22.0"
-sphinx = "^6.1.3"
-yummy-sphinx-theme = "^0.1.1"
 pytest-cov = "^4.0.0"
 coverage = "^7.2.3"
 black = "^23.3.0"
 isort = "^5.12.0"
-sphinx-material = "^0.0.35"
-pygments = "^2.15.0"
-sphinx-copybutton = "^0.5.2"
+mkdocs = "^1.4.2"
+mkdocstrings = {extras = ["python"], version = "^0.21.2"}
+mkdocs-gen-files = "^0.4.0"
+mkdocs-literate-nav = "^0.6.0"
+mkdocs-section-index = "^0.3.5"
+mkdocs-material = "^9.1.6"
+pypeln = "^0.4.9"
+mkdocs-material-extensions = "^1.1.1"
+mkdocs-jupyter = "^0.24.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `strplus-1.0.2/strplus/cases.py` & `strplus-1.0.3/strplus/cases.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,24 @@
 
     Args:
         text (str): The input string.
 
     Returns:
         str: The PascalCase version of the input string.
 
-    Example:
+    Examples:
         >>> to_pascal('hello_world')
         'HelloWorld'
+        
         >>> to_pascal('CamelCase')
         'CamelCase'
+        
         >>> to_pascal('some-mixed_string With spaces_underscores-and-hyphens')
         'SomeMixedStringWithSpacesUnderscoresAndHyphens'
+        
         >>> to_pascal('123abc')
         '123abc'
     """
     text = text.strip()
 
     if not text:  # If the input string is empty or only whitespace, return an empty string
         return ""
```

### Comparing `strplus-1.0.2/strplus/strplus.py` & `strplus-1.0.3/strplus/strplus.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     This class provides several methods for converting strings to different cases, as well as a method for
     converting a string to a list of words.
 
     All methods that return strings return instances of the Str class, so they can be further manipulated
     with any of the methods provided by this class or by the built-in str class.
 
     Examples:
+    
         >>> my_string = Str('hello_world')
         >>> my_string.to_pascal()
         'HelloWorld'
 
         >>> my_string = Str('this_is-an_example')
         >>> my_string.to_camel()
         'thisIsAnExample'
@@ -65,59 +66,66 @@
     def to_pascal(self):
         """
         Converts a string to PascalCase.
 
         Returns:
             str: The PascalCase version of the input string.
 
-        Example:
+        Examples:
+        
             >>> my_string = Str('hello_world')
             >>> my_string.to_pascal()
             'HelloWorld'
+            
             >>> my_string = Str('some-mixed_string With spaces_underscores-and-hyphens')
             >>> my_string.to_pascal()
             'SomeMixedStringWithSpacesUnderscoresAndHyphens'
+            
         """
         return Str(to_pascal(self))
 
     def to_camel(self):
         """Converts a string from any case to CamelCase.
 
         Returns:
             str: The converted string in CamelCase.
 
         Examples:
+        
             >>> my_string = Str('this_is-an_example')
             >>> my_string.to_camel()
             'thisIsAnExample'
 
             >>> my_string = Str('This is a test!')
             >>> my_string.to_camel()
             'thisIsATest'
+            
         """
         return Str(to_camel(self))
 
     def to_snake(self):
         """Converts a string to snake_case.
 
         Returns:
             str: The string converted to snake_case.
 
         Examples:
+        
             >>> my_string = Str("HelloWorld")
             >>> my_string.snake("HelloWorld")
             'hello_world'
 
             >>> my_string = Str("  AnotherString!  ")
             >>> my_string.to_snake()
             'another_string'
 
             >>>  my_string = Str("hello-world")
             >>> my_string.to_snake()
             'hello_world'
+            
         """
         return Str(to_snake(self))
 
     def to_list(self):
         return [Str(word) for word in to_list(self)]
```

### Comparing `strplus-1.0.2/setup.py` & `strplus-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['strplus']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'strplus',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': 'Python extra functions for strings',
-    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi](https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://pepy.tech/project/strplus)\n[![versions](https://img.shields.io/pypi/pyversions/strplus.svg)](https://github.com/wiseupdata/strplus)\n\n\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n- Simple use! \n\n<br>\n\n### Simple use example 😍\n```\n>>> my_string = Str(\'Cast_this_string_TO_Pascal\')\n>>> my_string.pascal\n\'CastThisStringToPascal\'\n\n>>> my_string = Str(\'CastMeUseLikeANormalFunction\')\n>>> my_string.snake\n\'cast_me_use_like_a_normal_function\'\n\n```\n<br>\n\n* [More Examples !](https://github.com/wiseupdata/strplus/blob/main/examples/examples_01.ipynb)\n* [Documentations examples](https://wiseupdata.github.io/strplus/index.html)! \n\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
+    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi](https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://pepy.tech/project/strplus)\n[![versions](https://img.shields.io/pypi/pyversions/strplus.svg)](https://github.com/wiseupdata/strplus)\n\n\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/imgs/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n- Simple use! \n\n<br>\n\n### Simple use example 😍\n```\n>>> my_string = Str(\'Cast_this_string_TO_Pascal\')\n>>> my_string.pascal\n\'CastThisStringToPascal\'\n\n>>> my_string = Str(\'CastMeUseLikeANormalFunction\')\n>>> my_string.snake\n\'cast_me_use_like_a_normal_function\'\n\n```\n<br>\n\n* [More Examples !](https://github.com/wiseupdata/strplus/blob/main/examples/examples_01.ipynb)\n* [Documentations examples](https://wiseupdata.github.io/strplus/index.html)! \n\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
     'author': 'Silvio Liborio',
     'author_email': 'silvio.liborio@wiseupdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['strplus']
 package_data = \ {'': ['*']} setup_kwargs = { 'name': 'strplus', 'version':
-'1.0.2', 'description': 'Python extra functions for strings',
+'1.0.3', 'description': 'Python extra functions for strings',
 'long_description': '\n_[Wise_Up_Data\'s_Instagram]_\n \n\n_[wise_Up_Data\'s
 Discord]\n\n\n_[wise_Up_Data_|_Twitter]\n\n\n_[wise_Up_Data\'s_LinkedIN]\n\n\n!
 [visitors](https://visitor-badge.glitch.me/
 badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n!
 [license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi]
 (https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/
 pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://
```

### Comparing `strplus-1.0.2/PKG-INFO` & `strplus-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strplus
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python extra functions for strings
 Author: Silvio Liborio
 Author-email: silvio.liborio@wiseupdata.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,15 +38,15 @@
 
 ---
 
 <br>
 <br>
 
 <a href="https://github.com/wiseupdata/wiseupdata">
-<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/python.png" width="300" />
+<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/imgs/python.png" width="300" />
 </a>
 
 <h1>
 Python extra functions for strings ❤️
 </h1>
 
 <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: strplus Version: 1.0.2 Summary: Python extra
+Metadata-Version: 2.1 Name: strplus Version: 1.0.3 Summary: Python extra
 functions for strings Author: Silvio Liborio Author-email:
 silvio.liborio@wiseupdata.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
```

