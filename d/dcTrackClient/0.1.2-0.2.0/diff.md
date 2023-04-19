# Comparing `tmp/dctrackclient-0.1.2.tar.gz` & `tmp/dctrackclient-0.2.0.tar.gz`

## Comparing `dctrackclient-0.1.2.tar` & `dctrackclient-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 dctrackclient-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 dctrackclient-0.1.2/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.1.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.1.2/LICENSE
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 dctrackclient-0.1.2/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 dctrackclient-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/.github/workflows/doc.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/README.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/PKG-INFO
```

### Comparing `dctrackclient-0.1.2/.github/workflows/python-publish.yml` & `dctrackclient-0.2.0/.github/workflows/python-publish.yml`

 * *Files 13% similar despite different names*

```diff
@@ -26,14 +26,16 @@
       uses: actions/setup-python@v3
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
+    - name: Write documentation
+      run: python .github/workflows/doc.py >> README.md
     - name: Build package
       run: python -m build
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `dctrackclient-0.1.2/src/dcTrackClient/__init__.py` & `dctrackclient-0.2.0/src/dcTrackClient/__init__.py`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.1.2/LICENSE` & `dctrackclient-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.1.2/pyproject.toml` & `dctrackclient-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

