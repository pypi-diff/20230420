# Comparing `tmp/kmaps-0.0.1.tar.gz` & `tmp/kmaps-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmaps-0.0.1.tar", last modified: Mon Feb 27 15:50:22 2023, max compression
+gzip compressed data, was "kmaps-0.0.4.tar", last modified: Thu Apr 20 14:45:12 2023, max compression
```

## Comparing `kmaps-0.0.1.tar` & `kmaps-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 15:50:22.265502 kmaps-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-02-27 15:45:26.000000 kmaps-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-02-27 15:45:26.000000 kmaps-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1274 2023-02-27 15:50:22.275669 kmaps-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-02-27 15:45:26.000000 kmaps-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-27 15:50:22.252595 kmaps-0.0.1/kmaps/
--rw-rw-rw-   0        0        0      126 2023-02-27 15:45:26.000000 kmaps-0.0.1/kmaps/__init__.py
--rw-rw-rw-   0        0        0       20 2023-02-27 15:45:26.000000 kmaps-0.0.1/kmaps/kmaps.py
-drwxrwxrwx   0        0        0        0 2023-02-27 15:50:22.265502 kmaps-0.0.1/kmaps.egg-info/
--rw-rw-rw-   0        0        0     1274 2023-02-27 15:50:22.000000 kmaps-0.0.1/kmaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-02-27 15:50:22.000000 kmaps-0.0.1/kmaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 15:50:22.000000 kmaps-0.0.1/kmaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 15:50:22.000000 kmaps-0.0.1/kmaps.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-02-27 15:50:22.000000 kmaps-0.0.1/kmaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-02-27 15:45:26.000000 kmaps-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      413 2023-02-27 15:50:22.275669 kmaps-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1748 2023-02-27 15:45:26.000000 kmaps-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:45:12.180660 kmaps-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 14:44:59.000000 kmaps-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-20 14:44:59.000000 kmaps-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-20 14:45:12.180660 kmaps-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-20 14:44:59.000000 kmaps-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:45:12.176660 kmaps-0.0.4/kmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 14:45:00.000000 kmaps-0.0.4/kmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-20 14:45:00.000000 kmaps-0.0.4/kmaps/folium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-04-20 14:45:00.000000 kmaps-0.0.4/kmaps/kmaps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:45:12.176660 kmaps-0.0.4/kmaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-20 14:45:12.000000 kmaps-0.0.4/kmaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 14:45:12.000000 kmaps-0.0.4/kmaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 14:45:12.000000 kmaps-0.0.4/kmaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:45:12.000000 kmaps-0.0.4/kmaps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 14:45:12.000000 kmaps-0.0.4/kmaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 14:45:12.000000 kmaps-0.0.4/kmaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 14:45:00.000000 kmaps-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 14:45:12.180660 kmaps-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-20 14:45:00.000000 kmaps-0.0.4/setup.py
```

### Comparing `kmaps-0.0.1/PKG-INFO` & `kmaps-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1
-Name: kmaps
-Version: 0.0.1
-Summary: TBA
-Home-page: https://github.com/ChangwhaOh/kmaps
-Author: Changwha Oh
-Author-email: coh4@vols.utk.edu
-License: MIT license
-Keywords: kmaps
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
-# kmaps
-
-
-[![image](https://img.shields.io/pypi/v/kmaps.svg)](https://pypi.python.org/pypi/kmaps)
-[![image](https://img.shields.io/conda/vn/conda-forge/kmaps.svg)](https://anaconda.org/conda-forge/kmaps)
-
-
-**TBA**
-
-
--   Free software: MIT license
--   Documentation: https://ChangwhaOh.github.io/kmaps
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
+Name: kmaps
+Version: 0.0.4
+Summary: TBA
+Home-page: https://github.com/ChangwhaOh/kmaps
+Author: Changwha Oh
+Author-email: coh4@vols.utk.edu
+License: MIT license
+Keywords: kmaps
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
+# kmaps
+
+
+[![image](https://img.shields.io/pypi/v/kmaps.svg)](https://pypi.python.org/pypi/kmaps)
+[![image](https://img.shields.io/conda/vn/conda-forge/kmaps.svg)](https://anaconda.org/conda-forge/kmaps)
+
+
+**TBA**
+
+
+-   Free software: MIT license
+-   Documentation: https://ChangwhaOh.github.io/kmaps
+    
+
+## Features
+
+-   kmaps is in development.
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `kmaps-0.0.1/kmaps.egg-info/PKG-INFO` & `kmaps-0.0.4/kmaps.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1
-Name: kmaps
-Version: 0.0.1
-Summary: TBA
-Home-page: https://github.com/ChangwhaOh/kmaps
-Author: Changwha Oh
-Author-email: coh4@vols.utk.edu
-License: MIT license
-Keywords: kmaps
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
-# kmaps
-
-
-[![image](https://img.shields.io/pypi/v/kmaps.svg)](https://pypi.python.org/pypi/kmaps)
-[![image](https://img.shields.io/conda/vn/conda-forge/kmaps.svg)](https://anaconda.org/conda-forge/kmaps)
-
-
-**TBA**
-
-
--   Free software: MIT license
--   Documentation: https://ChangwhaOh.github.io/kmaps
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
+Name: kmaps
+Version: 0.0.4
+Summary: TBA
+Home-page: https://github.com/ChangwhaOh/kmaps
+Author: Changwha Oh
+Author-email: coh4@vols.utk.edu
+License: MIT license
+Keywords: kmaps
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
+# kmaps
+
+
+[![image](https://img.shields.io/pypi/v/kmaps.svg)](https://pypi.python.org/pypi/kmaps)
+[![image](https://img.shields.io/conda/vn/conda-forge/kmaps.svg)](https://anaconda.org/conda-forge/kmaps)
+
+
+**TBA**
+
+
+-   Free software: MIT license
+-   Documentation: https://ChangwhaOh.github.io/kmaps
+    
+
+## Features
+
+-   kmaps is in development.
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `kmaps-0.0.1/setup.py` & `kmaps-0.0.4/setup.py`

 * *Files 22% similar despite different names*

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
-    author="Changwha Oh",
-    author_email='coh4@vols.utk.edu',
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
-    description="TBA",
-    install_requires=install_requires,
-    dependency_links=dependency_links,
-    license="MIT license",
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    include_package_data=True,
-    keywords='kmaps',
-    name='kmaps',
-    packages=find_packages(include=['kmaps', 'kmaps.*']),
-    setup_requires=setup_requirements,
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/ChangwhaOh/kmaps',
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
+    author="Changwha Oh",
+    author_email='coh4@vols.utk.edu',
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
+    description="TBA",
+    install_requires=install_requires,
+    dependency_links=dependency_links,
+    license="MIT license",
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    include_package_data=True,
+    keywords='kmaps',
+    name='kmaps',
+    packages=find_packages(include=['kmaps', 'kmaps.*']),
+    setup_requires=setup_requirements,
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://github.com/ChangwhaOh/kmaps',
+    version='0.0.4',
+    zip_safe=False,
+)
```

