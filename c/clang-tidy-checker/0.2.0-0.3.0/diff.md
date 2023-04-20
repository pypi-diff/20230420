# Comparing `tmp/clang_tidy_checker-0.2.0.tar.gz` & `tmp/clang_tidy_checker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clang_tidy_checker-0.2.0.tar", max compression
+gzip compressed data, was "clang_tidy_checker-0.3.0.tar", max compression
```

## Comparing `clang_tidy_checker-0.2.0.tar` & `clang_tidy_checker-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0       75 2023-01-06 11:22:56.325055 clang_tidy_checker-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-01-06 11:22:56.325055 clang_tidy_checker-0.2.0/clang_tidy_checker/__init__.py
--rw-r--r--   0        0        0       94 2023-01-06 11:22:56.325055 clang_tidy_checker-0.2.0/clang_tidy_checker/__main__.py
--rw-r--r--   0        0        0      979 2023-01-06 11:22:56.325055 clang_tidy_checker-0.2.0/clang_tidy_checker/check_files.py
--rw-r--r--   0        0        0     2032 2023-01-06 11:22:56.325055 clang_tidy_checker-0.2.0/clang_tidy_checker/config.py
--rw-r--r--   0        0        0     2010 2023-01-06 11:22:56.325055 clang_tidy_checker-0.2.0/clang_tidy_checker/execute_clang_tidy.py
--rw-r--r--   0        0        0     2499 2023-01-06 11:22:56.325055 clang_tidy_checker-0.2.0/clang_tidy_checker/main.py
--rw-r--r--   0        0        0      602 2023-01-06 11:22:56.325055 clang_tidy_checker-0.2.0/clang_tidy_checker/search_checked_files.py
--rw-r--r--   0        0        0      743 2023-01-06 11:22:56.325055 clang_tidy_checker-0.2.0/clang_tidy_checker/search_clang_tidy.py
--rw-r--r--   0        0        0     1701 2023-01-06 11:22:56.327055 clang_tidy_checker-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 clang_tidy_checker-0.2.0/setup.py
--rw-r--r--   0        0        0     1401 1970-01-01 00:00:00.000000 clang_tidy_checker-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      204 2023-04-20 13:30:00.713326 clang_tidy_checker-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 13:30:00.713326 clang_tidy_checker-0.3.0/clang_tidy_checker/__init__.py
+-rw-r--r--   0        0        0       94 2023-04-20 13:30:00.713326 clang_tidy_checker-0.3.0/clang_tidy_checker/__main__.py
+-rw-r--r--   0        0        0      979 2023-04-20 13:30:00.713326 clang_tidy_checker-0.3.0/clang_tidy_checker/check_files.py
+-rw-r--r--   0        0        0     2032 2023-04-20 13:30:00.713326 clang_tidy_checker-0.3.0/clang_tidy_checker/config.py
+-rw-r--r--   0        0        0     2010 2023-04-20 13:30:00.713326 clang_tidy_checker-0.3.0/clang_tidy_checker/execute_clang_tidy.py
+-rw-r--r--   0        0        0     2499 2023-04-20 13:30:00.713326 clang_tidy_checker-0.3.0/clang_tidy_checker/main.py
+-rw-r--r--   0        0        0      602 2023-04-20 13:30:00.713326 clang_tidy_checker-0.3.0/clang_tidy_checker/search_checked_files.py
+-rw-r--r--   0        0        0      743 2023-04-20 13:30:00.714326 clang_tidy_checker-0.3.0/clang_tidy_checker/search_clang_tidy.py
+-rw-r--r--   0        0        0     1701 2023-04-20 13:30:00.715326 clang_tidy_checker-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 clang_tidy_checker-0.3.0/PKG-INFO
```

### Comparing `clang_tidy_checker-0.2.0/clang_tidy_checker/check_files.py` & `clang_tidy_checker-0.3.0/clang_tidy_checker/check_files.py`

 * *Files identical despite different names*

### Comparing `clang_tidy_checker-0.2.0/clang_tidy_checker/config.py` & `clang_tidy_checker-0.3.0/clang_tidy_checker/config.py`

 * *Files identical despite different names*

### Comparing `clang_tidy_checker-0.2.0/clang_tidy_checker/execute_clang_tidy.py` & `clang_tidy_checker-0.3.0/clang_tidy_checker/execute_clang_tidy.py`

 * *Files identical despite different names*

### Comparing `clang_tidy_checker-0.2.0/clang_tidy_checker/main.py` & `clang_tidy_checker-0.3.0/clang_tidy_checker/main.py`

 * *Files identical despite different names*

### Comparing `clang_tidy_checker-0.2.0/clang_tidy_checker/search_checked_files.py` & `clang_tidy_checker-0.3.0/clang_tidy_checker/search_checked_files.py`

 * *Files identical despite different names*

### Comparing `clang_tidy_checker-0.2.0/clang_tidy_checker/search_clang_tidy.py` & `clang_tidy_checker-0.3.0/clang_tidy_checker/search_clang_tidy.py`

 * *Files identical despite different names*

### Comparing `clang_tidy_checker-0.2.0/pyproject.toml` & `clang_tidy_checker-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 [tool.poetry]
 name = "clang_tidy_checker"
-version = "0.2.0"
+version = "0.3.0"
 description = "Tool to check C / C++ source codes using clang-tidy."
 authors = ["Kenta Kabashima <kenta_program37@hotmail.co.jp>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/MusicScience37Projects/tools/clang-tidy-checker"
 repository = "https://gitlab.com/MusicScience37Projects/tools/clang-tidy-checker.git"
 # documentation = "TODO"
 keywords = ["clang-tidy", "c++"]
 # Classifiers: https://pypi.org/classifiers/
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: C",
     "Programming Language :: C++",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Quality Assurance",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9, <3.12"
+python = ">=3.9,<3.12"
 PyYAML = "^6.0"
 click = "^8.1.3"
 tqdm = "^4.64.0"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^2.20.0"
-Sphinx = "^5.0.2"
-black = "^22.6.0"
+pre-commit = "^3.2.2"
+Sphinx = "^6.1.3"
+black = "^23.3.0"
 doc8 = "^0.11.2"
-pylint = "^2.14.5"
+pylint = "^2.17.2"
 sphinx-autobuild = "^2021.3.14"
-sphinx-rtd-theme = "^1.0.0"
-mypy = "^0.971"
-flake8 = "^4.0.1"
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
+sphinx-rtd-theme = "^1.2.0"
+mypy = "^1.2.0"
+flake8 = "^6.0.0"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
 cmakelang = "^0.6.13"
 pytest-approvaltests = "^0.2.4"
-types-PyYAML = "^6.0.11"
+types-PyYAML = "^6.0.12.9"
 toml = "^0.10.2"
-types-toml = "^0.10.8"
-myst-parser = "^0.18.0"
-pytest-asyncio = "^0.20.3"
+types-toml = "^0.10.8.6"
+myst-parser = "^1.0.0"
+pytest-asyncio = "^0.21.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 clang-tidy-checker = "clang_tidy_checker.main:main"
```

