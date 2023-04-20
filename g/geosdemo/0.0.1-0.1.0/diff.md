# Comparing `tmp/geosdemo-0.0.1.tar.gz` & `tmp/geosdemo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geosdemo-0.0.1.tar", last modified: Tue Feb 21 15:36:25 2023, max compression
+gzip compressed data, was "geosdemo-0.1.0.tar", last modified: Thu Apr 20 14:17:51 2023, max compression
```

## Comparing `geosdemo-0.0.1.tar` & `geosdemo-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-21 15:36:25.111713 geosdemo-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-02-21 15:16:55.000000 geosdemo-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-02-21 15:16:55.000000 geosdemo-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1368 2023-02-21 15:36:25.112217 geosdemo-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      588 2023-02-21 15:16:55.000000 geosdemo-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-21 15:36:25.090971 geosdemo-0.0.1/geosdemo/
--rw-rw-rw-   0        0        0      128 2023-02-21 15:16:56.000000 geosdemo-0.0.1/geosdemo/__init__.py
--rw-rw-rw-   0        0        0       20 2023-02-21 15:16:56.000000 geosdemo-0.0.1/geosdemo/geosdemo.py
-drwxrwxrwx   0        0        0        0 2023-02-21 15:36:25.109713 geosdemo-0.0.1/geosdemo.egg-info/
--rw-rw-rw-   0        0        0     1368 2023-02-21 15:36:24.000000 geosdemo-0.0.1/geosdemo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-02-21 15:36:24.000000 geosdemo-0.0.1/geosdemo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-21 15:36:24.000000 geosdemo-0.0.1/geosdemo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-21 15:36:24.000000 geosdemo-0.0.1/geosdemo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-02-21 15:36:24.000000 geosdemo-0.0.1/geosdemo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-02-21 15:16:55.000000 geosdemo-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      416 2023-02-21 15:36:25.119667 geosdemo-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1796 2023-02-21 15:16:55.000000 geosdemo-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:17:51.805172 geosdemo-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 14:17:36.000000 geosdemo-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-20 14:17:36.000000 geosdemo-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-20 14:17:51.805172 geosdemo-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-20 14:17:36.000000 geosdemo-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:17:51.805172 geosdemo-0.1.0/geosdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 14:17:36.000000 geosdemo-0.1.0/geosdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-20 14:17:36.000000 geosdemo-0.1.0/geosdemo/foliumap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-20 14:17:36.000000 geosdemo-0.1.0/geosdemo/geosdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:17:51.805172 geosdemo-0.1.0/geosdemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-20 14:17:51.000000 geosdemo-0.1.0/geosdemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 14:17:51.000000 geosdemo-0.1.0/geosdemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-20 14:17:51.000000 geosdemo-0.1.0/geosdemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:17:51.000000 geosdemo-0.1.0/geosdemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-20 14:17:51.000000 geosdemo-0.1.0/geosdemo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 14:17:51.000000 geosdemo-0.1.0/geosdemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 14:17:36.000000 geosdemo-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-20 14:17:51.805172 geosdemo-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-20 14:17:36.000000 geosdemo-0.1.0/setup.py
```

### Comparing `geosdemo-0.0.1/LICENSE` & `geosdemo-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2023, Qiusheng Wu
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2023, Qiusheng Wu
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `geosdemo-0.0.1/PKG-INFO` & `geosdemo-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-Metadata-Version: 2.1
-Name: geosdemo
-Version: 0.0.1
-Summary: A python package for interactive mapping.
-Home-page: https://github.com/giswqs/geosdemo
-Author: Qiusheng Wu
-Author-email: giswqs@gmail.com
-License: MIT license
-Keywords: geosdemo
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# geosdemo
-
-
-[![image](https://img.shields.io/pypi/v/geosdemo.svg)](https://pypi.python.org/pypi/geosdemo)
-[![image](https://img.shields.io/conda/vn/conda-forge/geosdemo.svg)](https://anaconda.org/conda-forge/geosdemo)
-
-
-**A python package for interactive mapping.**
-
-
--   Free software: MIT license
--   Documentation: https://giswqs.github.io/geosdemo
-    
-
-## Features
-
--   TODO
-
-## Credits
-
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
+Metadata-Version: 2.1
+Name: geosdemo
+Version: 0.1.0
+Summary: A python package for interactive mapping.
+Home-page: https://github.com/giswqs/geosdemo
+Author: Qiusheng Wu
+Author-email: giswqs@gmail.com
+License: MIT license
+Keywords: geosdemo
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# geosdemo
+
+[![image](https://img.shields.io/pypi/v/geosdemo.svg)](https://pypi.python.org/pypi/geosdemo)
+[![image](https://img.shields.io/conda/vn/conda-forge/geosdemo.svg)](https://anaconda.org/conda-forge/geosdemo)
+
+**A python package for interactive mapping.**
+
+-   Free software: MIT license
+-   Documentation: https://geosdemo.gishub.org
+
+## Features
+
+-   TODO
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `geosdemo-0.0.1/geosdemo.egg-info/PKG-INFO` & `geosdemo-0.1.0/geosdemo.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-Metadata-Version: 2.1
-Name: geosdemo
-Version: 0.0.1
-Summary: A python package for interactive mapping.
-Home-page: https://github.com/giswqs/geosdemo
-Author: Qiusheng Wu
-Author-email: giswqs@gmail.com
-License: MIT license
-Keywords: geosdemo
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# geosdemo
-
-
-[![image](https://img.shields.io/pypi/v/geosdemo.svg)](https://pypi.python.org/pypi/geosdemo)
-[![image](https://img.shields.io/conda/vn/conda-forge/geosdemo.svg)](https://anaconda.org/conda-forge/geosdemo)
-
-
-**A python package for interactive mapping.**
-
-
--   Free software: MIT license
--   Documentation: https://giswqs.github.io/geosdemo
-    
-
-## Features
-
--   TODO
-
-## Credits
-
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
+Metadata-Version: 2.1
+Name: geosdemo
+Version: 0.1.0
+Summary: A python package for interactive mapping.
+Home-page: https://github.com/giswqs/geosdemo
+Author: Qiusheng Wu
+Author-email: giswqs@gmail.com
+License: MIT license
+Keywords: geosdemo
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# geosdemo
+
+[![image](https://img.shields.io/pypi/v/geosdemo.svg)](https://pypi.python.org/pypi/geosdemo)
+[![image](https://img.shields.io/conda/vn/conda-forge/geosdemo.svg)](https://anaconda.org/conda-forge/geosdemo)
+
+**A python package for interactive mapping.**
+
+-   Free software: MIT license
+-   Documentation: https://geosdemo.gishub.org
+
+## Features
+
+-   TODO
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `geosdemo-0.0.1/setup.py` & `geosdemo-0.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-import io
-from os import path as op
-from setuptools import setup, find_packages
-
-with open('README.md') as readme_file:
-    readme = readme_file.read()
-
-here = op.abspath(op.dirname(__file__))
-
-# get the dependencies and installs
-with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
-    all_reqs = f.read().split("\n")
-
-install_requires = [x.strip() for x in all_reqs if "git+" not in x]
-dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
-
-requirements = [ ]
-
-setup_requirements = [ ]
-
-test_requirements = [ ]
-
-setup(
-    author="Qiusheng Wu",
-    author_email='giswqs@gmail.com',
-    python_requires='>=3.7',
-    classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-    ],
-    description="A python package for interactive mapping.",
-    install_requires=install_requires,
-    dependency_links=dependency_links,
-    license="MIT license",
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    include_package_data=True,
-    keywords='geosdemo',
-    name='geosdemo',
-    packages=find_packages(include=['geosdemo', 'geosdemo.*']),
-    setup_requires=setup_requirements,
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/giswqs/geosdemo',
-    version='0.0.1',
-    zip_safe=False,
-)
+#!/usr/bin/env python
+
+"""The setup script."""
+
+import io
+from os import path as op
+from setuptools import setup, find_packages
+
+with open('README.md') as readme_file:
+    readme = readme_file.read()
+
+here = op.abspath(op.dirname(__file__))
+
+# get the dependencies and installs
+with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
+    all_reqs = f.read().split("\n")
+
+install_requires = [x.strip() for x in all_reqs if "git+" not in x]
+dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
+
+requirements = [ ]
+
+setup_requirements = [ ]
+
+test_requirements = [ ]
+
+setup(
+    author="Qiusheng Wu",
+    author_email='giswqs@gmail.com',
+    python_requires='>=3.7',
+    classifiers=[
+        'Development Status :: 2 - Pre-Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+    ],
+    description="A python package for interactive mapping.",
+    install_requires=install_requires,
+    dependency_links=dependency_links,
+    license="MIT license",
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    include_package_data=True,
+    keywords='geosdemo',
+    name='geosdemo',
+    packages=find_packages(include=['geosdemo', 'geosdemo.*']),
+    setup_requires=setup_requirements,
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://github.com/giswqs/geosdemo',
+    version='0.1.0',
+    zip_safe=False,
+)
```

