# Comparing `tmp/async_mvg_api-0.1.3.tar.gz` & `tmp/async_mvg_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_mvg_api-0.1.3.tar", max compression
+gzip compressed data, was "async_mvg_api-0.1.4.tar", max compression
```

## Comparing `async_mvg_api-0.1.3.tar` & `async_mvg_api-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35184 2022-12-10 11:36:21.271710 async_mvg_api-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2022-12-03 15:42:09.092422 async_mvg_api-0.1.3/mvg_api/__init__.py
--rw-r--r--   0        0        0        0 2022-11-29 14:00:44.819142 async_mvg_api-0.1.3/mvg_api/api/__init__.py
--rw-r--r--   0        0        0    11269 2022-12-10 11:31:43.416867 async_mvg_api-0.1.3/mvg_api/api/api.py
--rw-r--r--   0        0        0        0 2022-11-29 14:00:22.839034 async_mvg_api-0.1.3/mvg_api/models/__init__.py
--rw-r--r--   0        0        0     4415 2022-12-02 17:15:39.219527 async_mvg_api-0.1.3/mvg_api/models/route.py
--rw-r--r--   0        0        0     1572 2022-12-02 23:40:22.454153 async_mvg_api-0.1.3/mvg_api/models/ticker.py
--rw-r--r--   0        0        0     9098 2022-12-09 23:13:34.029374 async_mvg_api-0.1.3/mvg_api/mvg.py
--rw-r--r--   0        0        0        0 2022-12-02 17:39:31.765071 async_mvg_api-0.1.3/mvg_api/tests/__init__.py
--rw-r--r--   0        0        0     3097 2022-12-10 11:31:55.574048 async_mvg_api-0.1.3/mvg_api/tests/api_tests.py
--rw-r--r--   0        0        0    21657 2022-12-10 11:37:25.131780 async_mvg_api-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1404 2022-12-09 23:56:14.842549 async_mvg_api-0.1.3/README.md
--rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 async_mvg_api-0.1.3/setup.py
--rw-r--r--   0        0        0     1908 1970-01-01 00:00:00.000000 async_mvg_api-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-10 11:36:21.271710 async_mvg_api-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2022-12-03 15:42:09.092422 async_mvg_api-0.1.4/mvg_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-29 14:00:44.819142 async_mvg_api-0.1.4/mvg_api/api/__init__.py
+-rw-r--r--   0        0        0    11269 2022-12-10 11:31:43.416867 async_mvg_api-0.1.4/mvg_api/api/api.py
+-rw-r--r--   0        0        0        0 2022-11-29 14:00:22.839034 async_mvg_api-0.1.4/mvg_api/models/__init__.py
+-rw-r--r--   0        0        0     4415 2022-12-02 17:15:39.219527 async_mvg_api-0.1.4/mvg_api/models/route.py
+-rw-r--r--   0        0        0     1572 2022-12-02 23:40:22.454153 async_mvg_api-0.1.4/mvg_api/models/ticker.py
+-rw-r--r--   0        0        0     9098 2022-12-09 23:13:34.029374 async_mvg_api-0.1.4/mvg_api/mvg.py
+-rw-r--r--   0        0        0        0 2022-12-02 17:39:31.765071 async_mvg_api-0.1.4/mvg_api/tests/__init__.py
+-rw-r--r--   0        0        0     3097 2022-12-10 11:31:55.574048 async_mvg_api-0.1.4/mvg_api/tests/api_tests.py
+-rw-r--r--   0        0        0    21656 2023-04-20 10:15:50.771249 async_mvg_api-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1404 2022-12-09 23:56:14.842549 async_mvg_api-0.1.4/README.md
+-rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 async_mvg_api-0.1.4/setup.py
+-rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 async_mvg_api-0.1.4/PKG-INFO
```

### Comparing `async_mvg_api-0.1.3/LICENSE` & `async_mvg_api-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `async_mvg_api-0.1.3/mvg_api/api/api.py` & `async_mvg_api-0.1.4/mvg_api/api/api.py`

 * *Files identical despite different names*

### Comparing `async_mvg_api-0.1.3/mvg_api/models/route.py` & `async_mvg_api-0.1.4/mvg_api/models/route.py`

 * *Files identical despite different names*

### Comparing `async_mvg_api-0.1.3/mvg_api/models/ticker.py` & `async_mvg_api-0.1.4/mvg_api/models/ticker.py`

 * *Files identical despite different names*

### Comparing `async_mvg_api-0.1.3/mvg_api/mvg.py` & `async_mvg_api-0.1.4/mvg_api/mvg.py`

 * *Files identical despite different names*

### Comparing `async_mvg_api-0.1.3/mvg_api/tests/api_tests.py` & `async_mvg_api-0.1.4/mvg_api/tests/api_tests.py`

 * *Files identical despite different names*

### Comparing `async_mvg_api-0.1.3/pyproject.toml` & `async_mvg_api-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "async_mvg_api"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Lukas Mahr <lukas@yousuckatprogramming.de>"]
 readme = "README.md"
 packages = [{include = "mvg_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-pydantic = "^1.10.2"
-httpx = "^0.23.1"
-levenshtein = "^0.20.8"
-black = "^22.10.0"
+pydantic = "^1.10.7"
+httpx = "^0.24.0"
+levenshtein = "^0.21.0"
+black = "^23.3.0"
 pylint = "^2.15.7"
 pytest = "^7.2.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `async_mvg_api-0.1.3/README.md` & `async_mvg_api-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `async_mvg_api-0.1.3/setup.py` & `async_mvg_api-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 packages = \
 ['mvg_api', 'mvg_api.api', 'mvg_api.models', 'mvg_api.tests']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['black>=22.10.0,<23.0.0',
- 'httpx>=0.23.1,<0.24.0',
- 'levenshtein>=0.20.8,<0.21.0',
- 'pydantic>=1.10.2,<2.0.0',
+['black>=23.3.0,<24.0.0',
+ 'httpx>=0.24.0,<0.25.0',
+ 'levenshtein>=0.21.0,<0.22.0',
+ 'pydantic>=1.10.7,<2.0.0',
  'pylint>=2.15.7,<3.0.0',
  'pytest>=7.2.0,<8.0.0']
 
 setup_kwargs = {
     'name': 'async-mvg-api',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': '',
     'long_description': '# Unofficial MVG api\n\nAn async and sync wrapper for the MVG endpoints, with data validation over pydantic\n\n# Usage policy of the MVG api\n## ACHTUNG: \nUnsere Systeme dienen der direkten Kundeninteraktion. Die Verarbeitung unserer Inhalte oder Daten durch Dritte erfordert unsere ausdrückliche Zustimmung. Für private, nicht-kommerzielle Zwecke, wird eine gemäßigte Nutzung ohne unsere ausdrückliche Zustimmung geduldet. Jegliche Form von Data-Mining stellt keine gemäßigte Nutzung dar. Wir behalten uns vor, die Duldung grundsätzlich oder in Einzelfällen zu widerrufen. Fragen richten Sie bitte gerne an: redaktion@mvg.de.\n\nIn other words: Private, noncomercial, moderate use of the API is tolerated. They don\'t consider data mining as moderate use.\n\n(Disclaimer: I am not a lawyer, this isn\'t legal advice)\n\n## Installation\npip installation or clone the repository and install the [poetry](https://python-poetry.org/) dependencies\n\n```bash\npip install async-mvg-api\n```\n\nor \n\n```bash\ngit clone https://github.com/Plutokekz/MVG-Api.git\ncd MVG-Api\npoetry install\n```\n## Usage\n\n```python\nfrom mvg_api.mvg import MVG\nmvg = MVG()\nmvg.get_location("Hauptbahnhof")\n```\n\n## Tests\n\n```bash\npoetry run pytest mvg_api/tests/api_tests.py\n```\n\n# Credit\nFor Endpoint Information and Code snippets\n* https://github.com/leftshift/python_mvg_api\n* https://www.mvg.de/\n',
     'author': 'Lukas Mahr',
     'author_email': 'lukas@yousuckatprogramming.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `async_mvg_api-0.1.3/PKG-INFO` & `async_mvg_api-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: async-mvg-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Lukas Mahr
 Author-email: lukas@yousuckatprogramming.de
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: black (>=22.10.0,<23.0.0)
-Requires-Dist: httpx (>=0.23.1,<0.24.0)
-Requires-Dist: levenshtein (>=0.20.8,<0.21.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: black (>=23.3.0,<24.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: levenshtein (>=0.21.0,<0.22.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pylint (>=2.15.7,<3.0.0)
 Requires-Dist: pytest (>=7.2.0,<8.0.0)
 Description-Content-Type: text/markdown
 
 # Unofficial MVG api
 
 An async and sync wrapper for the MVG endpoints, with data validation over pydantic
```

