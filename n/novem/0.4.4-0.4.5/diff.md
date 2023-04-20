# Comparing `tmp/novem-0.4.4.tar.gz` & `tmp/novem-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novem-0.4.4.tar", max compression
+gzip compressed data, was "novem-0.4.5.tar", max compression
```

## Comparing `novem-0.4.4.tar` & `novem-0.4.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1194 2022-04-03 20:39:39.813737 novem-0.4.4/LICENSE
--rw-r--r--   0        0        0     3976 2022-04-03 20:39:39.814271 novem-0.4.4/README.md
--rw-r--r--   0        0        0      130 2023-03-24 10:52:33.433768 novem-0.4.4/novem/__init__.py
--rw-r--r--   0        0        0      152 2023-03-24 10:52:33.434441 novem-0.4.4/novem/__main__.py
--rw-r--r--   0        0        0     5520 2023-03-24 10:52:33.439534 novem-0.4.4/novem/api_ref.py
--rw-r--r--   0        0        0      252 2023-03-24 10:52:33.440298 novem-0.4.4/novem/applicator.py
--rw-r--r--   0        0        0    12297 2023-03-24 10:52:33.449688 novem-0.4.4/novem/cli/__init__.py
--rw-r--r--   0        0        0     3269 2023-03-24 10:52:33.441977 novem-0.4.4/novem/cli/config.py
--rw-r--r--   0        0        0     2661 2023-03-24 10:52:33.441394 novem-0.4.4/novem/cli/editor.py
--rw-r--r--   0        0        0     8148 2023-03-24 10:52:33.450046 novem-0.4.4/novem/cli/group.py
--rw-r--r--   0        0        0     3213 2023-03-24 10:52:33.450425 novem-0.4.4/novem/cli/invite.py
--rw-r--r--   0        0        0     5812 2023-03-24 10:52:33.443273 novem-0.4.4/novem/cli/mail.py
--rw-r--r--   0        0        0     5556 2023-03-24 10:52:33.444148 novem-0.4.4/novem/cli/plot.py
--rw-r--r--   0        0        0    11982 2023-03-24 10:52:33.450798 novem-0.4.4/novem/cli/setup.py
--rw-r--r--   0        0        0     5309 2023-03-24 10:52:33.451210 novem-0.4.4/novem/cli/vis.py
--rw-r--r--   0        0        0      109 2023-03-24 10:52:33.452008 novem-0.4.4/novem/colors/__init__.py
--rw-r--r--   0        0        0     2033 2023-03-24 10:52:33.452675 novem-0.4.4/novem/colors/colors.py
--rw-r--r--   0        0        0      133 2023-03-24 10:52:33.454768 novem-0.4.4/novem/exceptions/__init__.py
--rw-r--r--   0        0        0      382 2023-03-24 10:52:33.456366 novem-0.4.4/novem/mail.py
--rw-r--r--   0        0        0       66 2023-03-24 10:52:33.457095 novem-0.4.4/novem/table/__init__.py
--rw-r--r--   0        0        0     3437 2023-03-24 10:52:33.457792 novem-0.4.4/novem/table/selector.py
--rw-r--r--   0        0        0     8940 2023-03-24 10:52:33.460116 novem-0.4.4/novem/utils.py
--rw-r--r--   0        0        0       22 2023-03-24 10:52:33.460815 novem-0.4.4/novem/version.py
--rw-r--r--   0        0        0    13852 2023-03-24 10:52:33.475014 novem-0.4.4/novem/vis/__init__.py
--rw-r--r--   0        0        0     3398 2023-03-24 10:52:33.461749 novem-0.4.4/novem/vis/cell.py
--rw-r--r--   0        0        0     1406 2023-03-24 10:52:33.462910 novem-0.4.4/novem/vis/colors.py
--rw-r--r--   0        0        0      915 2023-03-24 10:52:33.467644 novem-0.4.4/novem/vis/files.py
--rw-r--r--   0        0        0     9117 2023-03-24 10:52:33.475367 novem-0.4.4/novem/vis/mail.py
--rw-r--r--   0        0        0    16106 2023-03-24 10:52:33.463622 novem-0.4.4/novem/vis/mail_sections.py
--rw-r--r--   0        0        0     7237 2023-03-24 10:52:33.475730 novem-0.4.4/novem/vis/plot.py
--rw-r--r--   0        0        0     1487 2023-03-24 10:52:33.464795 novem-0.4.4/novem/vis/plot_config.py
--rw-r--r--   0        0        0     1468 2023-03-24 10:52:33.465970 novem-0.4.4/novem/vis/shared.py
--rw-r--r--   0        0        0     1507 2023-03-24 10:52:38.206646 novem-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     5040 2023-03-24 10:55:11.559440 novem-0.4.4/setup.py
--rw-r--r--   0        0        0     4734 2023-03-24 10:55:11.560215 novem-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1194 2022-04-03 20:39:39.813737 novem-0.4.5/LICENSE
+-rw-r--r--   0        0        0     3976 2022-04-03 20:39:39.814271 novem-0.4.5/README.md
+-rw-r--r--   0        0        0      130 2023-04-20 13:01:33.609368 novem-0.4.5/novem/__init__.py
+-rw-r--r--   0        0        0      152 2023-04-20 13:01:33.610085 novem-0.4.5/novem/__main__.py
+-rw-r--r--   0        0        0     5520 2023-04-20 13:01:33.616697 novem-0.4.5/novem/api_ref.py
+-rw-r--r--   0        0        0      252 2023-04-20 13:01:33.617439 novem-0.4.5/novem/applicator.py
+-rw-r--r--   0        0        0    12405 2023-04-20 13:01:33.628293 novem-0.4.5/novem/cli/__init__.py
+-rw-r--r--   0        0        0     3269 2023-04-20 13:01:33.618684 novem-0.4.5/novem/cli/config.py
+-rw-r--r--   0        0        0     2661 2023-04-20 13:01:33.618131 novem-0.4.5/novem/cli/editor.py
+-rw-r--r--   0        0        0     8148 2023-04-20 13:01:33.626755 novem-0.4.5/novem/cli/group.py
+-rw-r--r--   0        0        0     3213 2023-04-20 13:01:33.627165 novem-0.4.5/novem/cli/invite.py
+-rw-r--r--   0        0        0     5812 2023-04-20 13:01:33.619590 novem-0.4.5/novem/cli/mail.py
+-rw-r--r--   0        0        0     5556 2023-04-20 13:01:33.620818 novem-0.4.5/novem/cli/plot.py
+-rw-r--r--   0        0        0    11982 2023-04-20 13:01:33.627520 novem-0.4.5/novem/cli/setup.py
+-rw-r--r--   0        0        0     5309 2023-04-20 13:01:33.627873 novem-0.4.5/novem/cli/vis.py
+-rw-r--r--   0        0        0      109 2023-04-20 13:01:33.628999 novem-0.4.5/novem/colors/__init__.py
+-rw-r--r--   0        0        0     2033 2023-04-20 13:01:33.629617 novem-0.4.5/novem/colors/colors.py
+-rw-r--r--   0        0        0      133 2023-04-20 13:01:33.632073 novem-0.4.5/novem/exceptions/__init__.py
+-rw-r--r--   0        0        0      382 2023-04-20 13:01:33.634329 novem-0.4.5/novem/mail.py
+-rw-r--r--   0        0        0       66 2023-04-20 13:01:33.635059 novem-0.4.5/novem/table/__init__.py
+-rw-r--r--   0        0        0     5814 2023-04-20 13:01:33.637042 novem-0.4.5/novem/table/selector.py
+-rw-r--r--   0        0        0     8940 2023-04-20 13:01:33.637941 novem-0.4.5/novem/utils.py
+-rw-r--r--   0        0        0       22 2023-04-20 13:01:33.638563 novem-0.4.5/novem/version.py
+-rw-r--r--   0        0        0    13852 2023-04-20 13:01:33.649893 novem-0.4.5/novem/vis/__init__.py
+-rw-r--r--   0        0        0     3398 2023-04-20 13:01:33.639782 novem-0.4.5/novem/vis/cell.py
+-rw-r--r--   0        0        0     1406 2023-04-20 13:01:33.640377 novem-0.4.5/novem/vis/colors.py
+-rw-r--r--   0        0        0      915 2023-04-20 13:01:33.642864 novem-0.4.5/novem/vis/files.py
+-rw-r--r--   0        0        0     9117 2023-04-20 13:01:33.650256 novem-0.4.5/novem/vis/mail.py
+-rw-r--r--   0        0        0    16106 2023-04-20 13:01:33.641054 novem-0.4.5/novem/vis/mail_sections.py
+-rw-r--r--   0        0        0     7237 2023-04-20 13:01:33.650592 novem-0.4.5/novem/vis/plot.py
+-rw-r--r--   0        0        0     1487 2023-04-20 13:01:33.641634 novem-0.4.5/novem/vis/plot_config.py
+-rw-r--r--   0        0        0     1468 2023-04-20 13:01:33.642275 novem-0.4.5/novem/vis/shared.py
+-rw-r--r--   0        0        0     1525 2023-04-20 13:01:25.954589 novem-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     5090 2023-04-20 13:04:46.342384 novem-0.4.5/setup.py
+-rw-r--r--   0        0        0     4812 2023-04-20 13:04:46.342891 novem-0.4.5/PKG-INFO
```

### Comparing `novem-0.4.4/LICENSE` & `novem-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/README.md` & `novem-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/api_ref.py` & `novem-0.4.5/novem/api_ref.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/cli/__init__.py` & `novem-0.4.5/novem/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,14 +334,18 @@
 
     #    return
 
     # Gather the provided arguements as an array.
     # (parser:Any, args:Dict[str, str]) = setup(raw_args)
     (parser, args) = setup(raw_args)
 
+    # let's add traceback back in
+    if "debug" in args and args["debug"]:
+        del sys.tracebacklimit
+
     if len(raw_args) == 0:
         print_short(parser)
         return
 
     if args and args["version"]:
         print(f"novem {__version__}")
         return
```

### Comparing `novem-0.4.4/novem/cli/config.py` & `novem-0.4.5/novem/cli/config.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/cli/editor.py` & `novem-0.4.5/novem/cli/editor.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/cli/group.py` & `novem-0.4.5/novem/cli/group.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/cli/invite.py` & `novem-0.4.5/novem/cli/invite.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/cli/mail.py` & `novem-0.4.5/novem/cli/mail.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/cli/plot.py` & `novem-0.4.5/novem/cli/plot.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/cli/setup.py` & `novem-0.4.5/novem/cli/setup.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/cli/vis.py` & `novem-0.4.5/novem/cli/vis.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/colors/colors.py` & `novem-0.4.5/novem/colors/colors.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/utils.py` & `novem-0.4.5/novem/utils.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/vis/__init__.py` & `novem-0.4.5/novem/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/vis/cell.py` & `novem-0.4.5/novem/vis/cell.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/vis/colors.py` & `novem-0.4.5/novem/vis/colors.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/vis/files.py` & `novem-0.4.5/novem/vis/files.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/vis/mail.py` & `novem-0.4.5/novem/vis/mail.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/vis/mail_sections.py` & `novem-0.4.5/novem/vis/mail_sections.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/vis/plot.py` & `novem-0.4.5/novem/vis/plot.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/vis/plot_config.py` & `novem-0.4.5/novem/vis/plot_config.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/novem/vis/shared.py` & `novem-0.4.5/novem/vis/shared.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.4/pyproject.toml` & `novem-0.4.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "novem"
-version = "0.4.4"
+version = "0.4.5"
 description = "python library for the novem.no data visualisation platform"
 authors = ["Sondov Engen <sondov@novem.no>"]
 homepage = "https://novem.no"
 repository = "https://github.com/novem-no/novem"
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.26.0"
 pyreadline3 = "^3.4.1"
 colorama = "^0.4.6"
 urllib3 = "^1.26.15"
+pandas = "^2.0.0"
+numpy = "^1.24.2"
 
 [tool.poetry.scripts]
 novem = 'novem.cli:run_cli'
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.0"
 pytest-cov = "^3.0.0"
@@ -26,15 +28,14 @@
 black = {version = "^22.3.0", allow-prereleases = true}
 mypy = "^0.930"
 pydantic = "^1.8.2"
 isort = "^5.10.1"
 requests-mock = "^1.9.3"
 types-requests = "^2.27.7"
 pyfakefs = "^4.5.5"
-pandas = "^1.5.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
```

### Comparing `novem-0.4.4/setup.py` & `novem-0.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,26 @@
  'novem.vis']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['colorama>=0.4.6,<0.5.0',
+ 'numpy>=1.24.2,<2.0.0',
+ 'pandas>=2.0.0,<3.0.0',
  'pyreadline3>=3.4.1,<4.0.0',
  'requests>=2.26.0,<3.0.0',
  'urllib3>=1.26.15,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['novem = novem.cli:run_cli']}
 
 setup_kwargs = {
     'name': 'novem',
-    'version': '0.4.4',
+    'version': '0.4.5',
     'description': 'python library for the novem.no data visualisation platform',
     'long_description': '\n# novem - data visualisation for coders\n\nA wrapper library for the novem.no data visualisation platform. Create charts,\ndocuments e-mails and dashboards through one simple api.\n\n**NB:** novem is currently in closed alpha, if you want to try it out please\nreach out to hello@novem.no\n\n\n## Exampels\n\nCreate a linechart from a dataframe using pandas data reader\n\n```python\nfrom pandas_datareader import data\nfrom novem import Plot\n\nline = Plot("aapl_price_hist", type="line", name="Apple price history")\n\n# Only get the adjusted close.\naapl = data.DataReader("AAPL",\n                       start="2015-1-1",\n                       end="2021-12-31",\n                       data_source="yahoo")["Adj Close"]\n\n# send data to the plot\naapl.pipe(line)\n\n# url to view plot\nprint(line.url)\n```\n\n\n## Getting started\nTo get started with novem you\'ll have to register an account, currently this\ncan be done by reaching out to the novem developers on hello@novem.no.\n\nOnce you have a username and password you can setup your environment using:\n```bash\n  python -m novem --init\n```\n\nIn additon to invoking the novem module as shown above, the novem package also\nincludes an extensive command-line interface (cli). Check out CLI.md in this\nrepostiory or [novem.no](https://novem.no) for more details.\n\n\n\n## Creating a plot\nNovem represents plots as a Plot class that can be imported from the main novem\npackage `from novem import Plot`.\n\nThe plot class takes a single mandatory positional argument, the name of the\nplot.\n * If the plot name is new, the instantiation of the class will create the plot.\n * If the plot name already exist, then the new object will operate on the\n   existing plot.\n\nIn addition to the name, there are two broad categories of options for a\nplot, data and config:\n * The **data** contains the actual information to visualise (usually in the form\n   of numeric csv)\n * **Config**, which contains information about the visual such as:\n   * Type (bar, line, donut, map etc)\n   * Titles/captions/names/colors/legends/axis etc\n\n\nThere are two ways to interact with the plots, one can either supply all\nthe neccessary options as named arguments when creating the plot, or use the\nproperty accessors to modfity them one by one (this is more helpful when working\nwith the plot in an interactive way). Below is an example of the two\napproaches.\n\n```python\nfrom novem import Plot\n\n# everything in the constructor\nbarchart = Plot(<name>, \\\n  type="bar", \\\n  title="barchart title", \\\n  caption = "caption"\n)\n\n# property approach\nbarchart = Plot("plot_name")\nbarchart.type = "bar"\nbarchart.title = "barchart title"\nbarchart.caption = "caption"\n```\n\nIn addition to setting individual properties, the plot object is also callable.\nThis means that the resulting plot can be used as a function, either by being\nprovided data as an argument, or used as part of a pipe chain.\n\n```python\nfrom novem import Plot\nimport pandas as pd\nimport numpy as np\n\n# construct some random sample data\ndf = pd.DataFrame(np.random.randn(100, 4), columns=list("ABCD")).cumsum()\n\nline = Plot("new_line", type="line")\n\n# alternative one, setting data explicitly to a csv string\nline.data = df.to_csv()\n\n# or let the plot invoke the to_csv\nline.data = df\n\n# alternative two, calling Plot with a csv string\nline(df.to_csv())\n\n# alternative three calling the Plot with an object that has a to_csv function\nline(df)\n\n# or\ndf.pipe(line)\n\n```\n\n\n**NB:** All novem plot operations are live.\nThis means that as soon as you write to or modify any aspects of the plot\nobject, those changes are reflected on the novem server and anyone watching\nthe plot in real time.\n\n\n\n## Contribution and development\nThe novem python library and platform is under active development, contributions\nor issues are most welcome.\n\nFor guidelines on how to contribute, please check out the CONTRIBUTING.md file\nin this repository.\n\n\n## LICENSE\nThis python library is licensed under the MIT license, see the LICENSE file for\ndetails\n',
     'author': 'Sondov Engen',
     'author_email': 'sondov@novem.no',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://novem.no',
```

### Comparing `novem-0.4.4/PKG-INFO` & `novem-0.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: novem
-Version: 0.4.4
+Version: 0.4.5
 Summary: python library for the novem.no data visualisation platform
 Home-page: https://novem.no
 License: MIT
 Author: Sondov Engen
 Author-email: sondov@novem.no
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
 Project-URL: Repository, https://github.com/novem-no/novem
 Description-Content-Type: text/markdown
```

