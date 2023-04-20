# Comparing `tmp/newsdash-0.1.0.tar.gz` & `tmp/newsdash-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newsdash-0.1.0.tar", max compression
+gzip compressed data, was "newsdash-0.1.1.tar", max compression
```

## Comparing `newsdash-0.1.0.tar` & `newsdash-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-04-07 11:07:34.064591 newsdash-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2963 2023-04-07 11:07:04.424617 newsdash-0.1.0/README.md
--rw-r--r--   0        0        0       52 2023-04-07 11:03:56.200781 newsdash-0.1.0/newsdash/__init__.py
--rw-r--r--   0        0        0    15402 2023-04-07 11:04:57.824728 newsdash-0.1.0/newsdash/client.py
--rw-r--r--   0        0        0     1394 2023-04-07 11:05:47.004685 newsdash-0.1.0/newsdash/exceptions.py
--rw-r--r--   0        0        0     1270 2023-04-07 11:05:24.676704 newsdash-0.1.0/newsdash/http.py
--rw-r--r--   0        0        0      687 2023-04-07 11:07:51.440576 newsdash-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3815 2023-04-07 11:28:23.889955 newsdash-0.1.0/setup.py
--rw-r--r--   0        0        0     3712 2023-04-07 11:28:23.892195 newsdash-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3153 2023-04-20 14:19:12.303323 newsdash-0.1.1/README.md
+-rw-r--r--   0        0        0       76 2023-04-20 14:19:12.307323 newsdash-0.1.1/newsdash/__init__.py
+-rw-r--r--   0        0        0    22992 2023-04-20 14:19:12.307323 newsdash-0.1.1/newsdash/client.py
+-rw-r--r--   0        0        0     1394 2023-04-20 14:19:12.307323 newsdash-0.1.1/newsdash/exceptions.py
+-rw-r--r--   0        0        0     2715 2023-04-20 14:19:12.307323 newsdash-0.1.1/newsdash/http.py
+-rw-r--r--   0        0        0      928 2023-04-20 14:19:12.307323 newsdash-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4209 1970-01-01 00:00:00.000000 newsdash-0.1.1/PKG-INFO
```

### Comparing `newsdash-0.1.0/README.md` & `newsdash-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 ![NewsDash](./readme-assets/poster.jpg)
 # NewsDash
-**note**:This is a WIP library, please report bugs if you find one
 [![Python 3.9-3.11](https://img.shields.io/badge/Python-3.9--3.11-blue.svg)]()
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![GitHub stars](https://img.shields.io/github/stars/NaviTheCoderboi/NewsDash.svg)](https://github.com/NaviTheCoderboi/NewsDash)
 ![GitHub last commit](https://img.shields.io/github/last-commit/NaviTheCoderboi/NewsDash.svg)
+[![PyPI version](https://badge.fury.io/py/newsdash.svg)](https://badge.fury.io/py/newsdash)
 
 ***
 NewsDash is a fast and reliable Python wrapper for the News API that simplifies accessing the latest news articles from around the world. 📰
 ***
 Made by: NaviTheCoderboi
 ***
-# Features
+
+---
+
+!!! note "Note"
+    This is a WIP library, please report bugs if you find one
+
+---
+
+## Features
 
 - **Fast performance:** This API wrapper is designed to be fast and efficient, allowing users to retrieve news articles quickly and easily.
 - **Reliable functionality:** The wrapper uses best practices to ensure reliable functionality and accuracy in retrieving news articles from the API.
 - **Easy-to-use interface:** The API wrapper has an intuitive interface that makes it easy for developers to interact with the API and retrieve news articles without having to worry about the details of the underlying protocol.
 - **Built with aiohttp:** The wrapper is built using the popular aiohttp library, which provides high-performance asynchronous HTTP client/server for asyncio and Python. This means the wrapper takes advantage of the latest and greatest in async programming techniques to provide fast and efficient performance.
 - **Customizable functionality:** The wrapper has a range of customization options, allowing developers to tailor their use of the API to their specific needs.
 - **Flexible data handling:** The wrapper is designed to handle a wide variety of data formats, allowing developers to work with the data in the way that best suits their needs.
 - **Well-documented:** The wrapper has clear and comprehensive documentation, making it easy for developers to get up and running quickly and troubleshoot any issues that may arise.
-# Installation
+## Installation
 ```bash
 python -m pip install newsdash
 ```
-# Examples
+## Examples
 - with client
 ```python
 from newsdash import NewsDash
 import asyncio
 
 cl = NewsDash("your_api_key")
 async def get_news():
@@ -46,11 +54,12 @@
 
 async def main():
   async with NewsDash("api_key") as nd:
     print(await nd.get_everything(query="apple"))
 
 asyncio.run(main())
 ```
-# Important urls
+## Important urls
 - [NewsApi](https://newsapi.org)
 - [NewsDash repository](https://github.com/NaviTheCoderboi/NewsDash)
-- [NewsDash pypi](https://pypi.org/project/NewsDash)
+- [NewsDash pypi](https://pypi.org/project/NewsDash)
+- [NewsDash documentation](https://NaviTheCoderboi.github.io/NewsDash)
```

### Comparing `newsdash-0.1.0/newsdash/exceptions.py` & `newsdash-0.1.1/newsdash/exceptions.py`

 * *Files identical despite different names*

### Comparing `newsdash-0.1.0/pyproject.toml` & `newsdash-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 [tool.poetry]
 name = "newsdash"
-version = "0.1.0"
+version = "0.1.1"
 description = "NewsDash is a fast and reliable Python wrapper for the News API that simplifies accessing the latest news articles from around the world."
 license = "MIT"
 authors = ["NaviTheCoderboi <navindersingh568@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/NaviTheCoderboi/NewsDash"
+documentation = "https://NaviTheCoderboi.github.io/NewsDash"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha"
 ]
 packages = [
     { include = "newsdash" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8.4"
 loguru = "^0.6.0"
+mkdocs = "^1.4.2"
+mkdocstrings = {extras = ["python"], version = "^0.21.2"}
+mkdocs-material = "^9.1.6"
+pygments = "^2.15.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `newsdash-0.1.0/setup.py` & `newsdash-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,89 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['newsdash']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp>=3.8.4,<4.0.0', 'loguru>=0.6.0,<0.7.0']
-
-setup_kwargs = {
-    'name': 'newsdash',
-    'version': '0.1.0',
-    'description': 'NewsDash is a fast and reliable Python wrapper for the News API that simplifies accessing the latest news articles from around the world.',
-    'long_description': '![NewsDash](./readme-assets/poster.jpg)\n# NewsDash\n**note**:This is a WIP library, please report bugs if you find one\n[![Python 3.9-3.11](https://img.shields.io/badge/Python-3.9--3.11-blue.svg)]()\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![GitHub stars](https://img.shields.io/github/stars/NaviTheCoderboi/NewsDash.svg)](https://github.com/NaviTheCoderboi/NewsDash)\n![GitHub last commit](https://img.shields.io/github/last-commit/NaviTheCoderboi/NewsDash.svg)\n\n***\nNewsDash is a fast and reliable Python wrapper for the News API that simplifies accessing the latest news articles from around the world. 📰\n***\nMade by: NaviTheCoderboi\n***\n# Features\n\n- **Fast performance:** This API wrapper is designed to be fast and efficient, allowing users to retrieve news articles quickly and easily.\n- **Reliable functionality:** The wrapper uses best practices to ensure reliable functionality and accuracy in retrieving news articles from the API.\n- **Easy-to-use interface:** The API wrapper has an intuitive interface that makes it easy for developers to interact with the API and retrieve news articles without having to worry about the details of the underlying protocol.\n- **Built with aiohttp:** The wrapper is built using the popular aiohttp library, which provides high-performance asynchronous HTTP client/server for asyncio and Python. This means the wrapper takes advantage of the latest and greatest in async programming techniques to provide fast and efficient performance.\n- **Customizable functionality:** The wrapper has a range of customization options, allowing developers to tailor their use of the API to their specific needs.\n- **Flexible data handling:** The wrapper is designed to handle a wide variety of data formats, allowing developers to work with the data in the way that best suits their needs.\n- **Well-documented:** The wrapper has clear and comprehensive documentation, making it easy for developers to get up and running quickly and troubleshoot any issues that may arise.\n# Installation\n```bash\npython -m pip install newsdash\n```\n# Examples\n- with client\n```python\nfrom newsdash import NewsDash\nimport asyncio\n\ncl = NewsDash("your_api_key")\nasync def get_news():\n  print(await cl.get_everything(query="tech",pageSize=5))\n  print(await cl.get_top_headlines(query="Microsoft"))\n  print(await cl.get_sources(country="in",language="en"))\n\nasyncio.run(get_news())\n```\n- with async context manager\n```python\nfrom newsdash import NewsDash\nimport asyncio\n\nasync def main():\n  async with NewsDash("api_key") as nd:\n    print(await nd.get_everything(query="apple"))\n\nasyncio.run(main())\n```\n# Important urls\n- [NewsApi](https://newsapi.org)\n- [NewsDash repository](https://github.com/NaviTheCoderboi/NewsDash)\n- [NewsDash pypi](https://pypi.org/project/NewsDash)',
-    'author': 'NaviTheCoderboi',
-    'author_email': 'navindersingh568@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/NaviTheCoderboi/NewsDash',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: newsdash
+Version: 0.1.1
+Summary: NewsDash is a fast and reliable Python wrapper for the News API that simplifies accessing the latest news articles from around the world.
+Home-page: https://github.com/NaviTheCoderboi/NewsDash
+License: MIT
+Author: NaviTheCoderboi
+Author-email: navindersingh568@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: mkdocs (>=1.4.2,<2.0.0)
+Requires-Dist: mkdocs-material (>=9.1.6,<10.0.0)
+Requires-Dist: mkdocstrings[python] (>=0.21.2,<0.22.0)
+Requires-Dist: pygments (>=2.15.0,<3.0.0)
+Project-URL: Documentation, https://NaviTheCoderboi.github.io/NewsDash
+Project-URL: Repository, https://github.com/NaviTheCoderboi/NewsDash
+Description-Content-Type: text/markdown
+
+![NewsDash](./readme-assets/poster.jpg)
+# NewsDash
+[![Python 3.9-3.11](https://img.shields.io/badge/Python-3.9--3.11-blue.svg)]()
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![GitHub stars](https://img.shields.io/github/stars/NaviTheCoderboi/NewsDash.svg)](https://github.com/NaviTheCoderboi/NewsDash)
+![GitHub last commit](https://img.shields.io/github/last-commit/NaviTheCoderboi/NewsDash.svg)
+[![PyPI version](https://badge.fury.io/py/newsdash.svg)](https://badge.fury.io/py/newsdash)
+
+***
+NewsDash is a fast and reliable Python wrapper for the News API that simplifies accessing the latest news articles from around the world. 📰
+***
+Made by: NaviTheCoderboi
+***
+
+---
+
+!!! note "Note"
+    This is a WIP library, please report bugs if you find one
+
+---
+
+## Features
+
+- **Fast performance:** This API wrapper is designed to be fast and efficient, allowing users to retrieve news articles quickly and easily.
+- **Reliable functionality:** The wrapper uses best practices to ensure reliable functionality and accuracy in retrieving news articles from the API.
+- **Easy-to-use interface:** The API wrapper has an intuitive interface that makes it easy for developers to interact with the API and retrieve news articles without having to worry about the details of the underlying protocol.
+- **Built with aiohttp:** The wrapper is built using the popular aiohttp library, which provides high-performance asynchronous HTTP client/server for asyncio and Python. This means the wrapper takes advantage of the latest and greatest in async programming techniques to provide fast and efficient performance.
+- **Customizable functionality:** The wrapper has a range of customization options, allowing developers to tailor their use of the API to their specific needs.
+- **Flexible data handling:** The wrapper is designed to handle a wide variety of data formats, allowing developers to work with the data in the way that best suits their needs.
+- **Well-documented:** The wrapper has clear and comprehensive documentation, making it easy for developers to get up and running quickly and troubleshoot any issues that may arise.
+## Installation
+```bash
+python -m pip install newsdash
+```
+## Examples
+- with client
+```python
+from newsdash import NewsDash
+import asyncio
+
+cl = NewsDash("your_api_key")
+async def get_news():
+  print(await cl.get_everything(query="tech",pageSize=5))
+  print(await cl.get_top_headlines(query="Microsoft"))
+  print(await cl.get_sources(country="in",language="en"))
+
+asyncio.run(get_news())
+```
+- with async context manager
+```python
+from newsdash import NewsDash
+import asyncio
+
+async def main():
+  async with NewsDash("api_key") as nd:
+    print(await nd.get_everything(query="apple"))
+
+asyncio.run(main())
+```
+## Important urls
+- [NewsApi](https://newsapi.org)
+- [NewsDash repository](https://github.com/NaviTheCoderboi/NewsDash)
+- [NewsDash pypi](https://pypi.org/project/NewsDash)
+- [NewsDash documentation](https://NaviTheCoderboi.github.io/NewsDash)
```

