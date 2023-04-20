# Comparing `tmp/pidgy-2023.1.7.post1.tar.gz` & `tmp/pidgy-2023.4.20.tar.gz`

## Comparing `pidgy-2023.1.7.post1.tar` & `pidgy-2023.4.20.tar`

### file list

```diff
@@ -1,83 +1,94 @@
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/.readthedocs.yml
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/dodo.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/mkdocs.yml
--rw-r--r--   0        0        0    61833 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/pidgy.png
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/sanitize.cfg
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/.binder/postBuild
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/.binder/requirements.txt
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/.github/workflows/pythonpackage.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/.pytest_cache/README.md
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/_templates/lite-demo.html
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/_templates/sbt-sidebar-footer.html
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/_templates/sbt-sidebar-nav.html
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/_templates/sidebar-logo.html
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/docs/environment.yml
--rw-r--r--   0        0        0    12141 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/docs/pidgy_examples.md.ipynb
--rw-r--r--   0        0        0    11026 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/docs/tangle_examples.ipynb
--rw-r--r--   0        0        0     6934 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/docs/test_extras.ipynb
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/docs/coverage/.gitignore
--rw-r--r--   0        0        0    20650 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/docs/coverage/coverage_html.js
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/docs/coverage/favicon_32.png
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/docs/coverage/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/docs/coverage/keybd_open.png
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/docs/coverage/status.json
--rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/docs/coverage/style.css
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyter-lite.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyter_lite_config.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/overrides.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/requirements.txt
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/.eslintignore
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/.eslintrc.js
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/.prettierignore
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/.prettierrc
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/MANIFEST.in
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/README.md
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/install.json
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/package.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/setup.cfg
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/setup.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/tsconfig.json
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/webpack.config.js
--rw-r--r--   0        0        0   225390 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/yarn.lock
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/py_src/jupyterlite_pidgy/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/py_src/jupyterlite_pidgy/_version.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/src/declarations.d.ts
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/src/index.ts
--rw-r--r--   0        0        0     9650 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/src/kernel.ts
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/src/tokens.ts
--rw-r--r--   0        0        0    11006 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/src/worker.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/style/index.js
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/lite/retro/jupyter-lite.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/kernelspec/kernel.json
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/kernelspec/logo-32x32.png
--rw-r--r--   0        0        0    46887 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/kernelspec/logo-64x64.png
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/README.md
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/__init__.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/__main__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/_version.py
--rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/displays.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/environment.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/extras.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/filters.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/kernel.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/loader.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/magics.py
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/pidgy.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/tangle.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/weave.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/ext/mkdocs.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/kernel/__init__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/src/pidgy/kernel/__main__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/LICENSE
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/README.md
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/pyproject.toml
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pidgy-2023.1.7.post1/PKG-INFO
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pidgy-2023.4.20/.readthedocs.yml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pidgy-2023.4.20/conftest.py
+-rw-r--r--   0        0        0     8847 2020-02-02 00:00:00.000000 pidgy-2023.4.20/dodo.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 pidgy-2023.4.20/mkdocs.yml
+-rw-r--r--   0        0        0    51934 2020-02-02 00:00:00.000000 pidgy-2023.4.20/pidgy.png
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pidgy-2023.4.20/sanitize.cfg
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pidgy-2023.4.20/.binder/postBuild
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pidgy-2023.4.20/.binder/requirements.txt
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 pidgy-2023.4.20/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pidgy-2023.4.20/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pidgy-2023.4.20/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pidgy-2023.4.20/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pidgy-2023.4.20/.pytest_cache/README.md
+-rw-r--r--   0        0        0     4562 2020-02-02 00:00:00.000000 pidgy-2023.4.20/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 pidgy-2023.4.20/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pidgy-2023.4.20/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 pidgy-2023.4.20/_templates/lite-demo.html
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pidgy-2023.4.20/_templates/sbt-sidebar-footer.html
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pidgy-2023.4.20/_templates/sbt-sidebar-nav.html
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 pidgy-2023.4.20/_templates/sidebar-logo.html
+-rw-r--r--   0        0        0    15097 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/basics.ipynb
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/hooks.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/index.md
+-rw-r--r--   0        0        0    16599 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/magics.ipynb
+-rw-r--r--   0        0        0     8026 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/mkdocs.ipynb
+-rw-r--r--   0        0        0    51934 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/pidgy.png
+-rw-r--r--   0        0        0    12141 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/pidgy_examples.md.ipynb
+-rw-r--r--   0        0        0    11569 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/reactivity.ipynb
+-rw-r--r--   0        0        0    11026 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/tangle_examples.ipynb
+-rw-r--r--   0        0        0     6934 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/test_extras.ipynb
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/coverage/.gitignore
+-rw-r--r--   0        0        0    20650 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/coverage/coverage_html.js
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/coverage/favicon_32.png
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/coverage/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/coverage/keybd_open.png
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/coverage/status.json
+-rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 pidgy-2023.4.20/docs/coverage/style.css
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyter-lite.json
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyter_lite_config.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/overrides.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/requirements.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/.eslintignore
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/.eslintrc.js
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/.prettierignore
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/.prettierrc
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/MANIFEST.in
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/README.md
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/install.json
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/package.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/setup.cfg
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/setup.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/tsconfig.json
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/webpack.config.js
+-rw-r--r--   0        0        0   232694 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/yarn.lock
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/py_src/jupyterlite_pidgy/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/py_src/jupyterlite_pidgy/_version.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/src/declarations.d.ts
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/src/index.ts
+-rw-r--r--   0        0        0     9594 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/src/kernel.ts
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/src/tokens.ts
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/src/worker.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/jupyterlite-pidgy/style/index.js
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pidgy-2023.4.20/lite/retro/jupyter-lite.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/kernelspec/kernel.json
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/kernelspec/logo-32x32.png
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/kernelspec/logo-64x64.png
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/README.md
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/__init__.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/__main__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/_version.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/current.py
+-rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/displays.py
+-rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/environment.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/extras.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/filters.py
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/inspect.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/kernel.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/loader.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/magics.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/tangle.py
+-rw-r--r--   0        0        0     8537 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/weave.py
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/ext/mkdocs.py
+-rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/ext/templates/ipynb.md.j2
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/help/mermaid.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/help/pidgy.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/kernel/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pidgy-2023.4.20/src/pidgy/kernel/__main__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pidgy-2023.4.20/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pidgy-2023.4.20/LICENSE
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 pidgy-2023.4.20/README.md
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 pidgy-2023.4.20/pyproject.toml
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 pidgy-2023.4.20/PKG-INFO
```

### Comparing `pidgy-2023.1.7.post1/dodo.py` & `pidgy-2023.4.20/dodo.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,28 +29,27 @@
 EXT_SRC_PKG_DATA = json.load(EXT_SRC_PKG.open())
 EXT_DIST_PKG = EXT / "py_src/jupyterlite_pidgy/labextension/package.json"
 EXT_DIST = EXT / "dist"
 EXT_WHL_NAME = f"""jupyterlite_pidgy-{EXT_SRC_PKG_DATA["version"]}-py3-none-any.whl"""
 EXT_WHL = EXT_DIST / EXT_WHL_NAME
 EXT_ICON = EXT / "style/pidgy.png"
 SHA256SUMS = DIST / "SHA256SUMS"
-KERNEL_DATA = HERE / "src/pidgy/kernel/pidgy"
+KERNEL_DATA = HERE / "src/kernelspec"
 KERNEL_ICON = KERNEL_DATA / "logo-64x64.png"
 WHL_PY = [
     p
     for p in [
-        HERE / "setup.py",
+        HERE / "pyproject.toml",
         *Path("src").rglob("*.py"),
     ]
     if p.name != "_version.py"
 ]
-WHL_MD = [HERE / "readme.md", Path("src/pidgy/readme.md")]
+WHL_MD = [HERE / "README.md", Path("src/pidgy/README.md")]
 WHL_DEPS = [
     HERE / "pyproject.toml",
-    HERE / "setup.cfg",
     *KERNEL_DATA.rglob("*"),
     *WHL_MD,
     *WHL_PY,
 ]
 ALL_PY = [DODO, *WHL_PY]
 ALL_MD = [*WHL_MD]
 ALL_JSON = [
@@ -106,15 +105,15 @@
     """build distributions"""
     yield dict(
         name="pidgy",
         doc="build pidgy distributions",
         file_dep=WHL_DEPS,
         actions=[
             lambda: [shutil.rmtree(DIST) if DIST.is_dir() else None, None][-1],
-            [PY, "setup.py", "sdist"],
+            [PY, "-m", "hatch", "build", "-t", "sdist"],
             [PY, "-m", "pip", "wheel", "-w", DIST, "--no-deps", "."],
             (
                 build_hashfile,
                 [
                     SHA256SUMS,
                     lambda: [*DIST.glob("pidgy*.whl"), *DIST.glob("pidgy*.tar.gz")],
                 ],
@@ -218,18 +217,24 @@
 
         if rc == 0:
             build_hashfile(LITE_PYPI_SHA256SUMS, lambda: [*LITE_PYPI.glob("*py3-none-any.whl")])
             return True
 
         return False
 
+    def _clean():
+        """remove conflicting packages that get patched"""
+        for x in ["tornado", "ipython", "ipykernel", "psutil", "pyzmq"]:
+            for file in LITE_PYPI.glob(F"{x}*.whl"):
+                file.unlink()
+
     yield dict(
         name="wheels",
         file_dep=[SHA256SUMS, LITE_REQS, EXT_WHL],
-        actions=[(doit.tools.create_folder, [LITE / "pypi"]), _wheels],
+        actions=[(doit.tools.create_folder, [LITE / "pypi"]), _wheels, _clean],
     )
 
     def _lite(args, extra_args=None):
         lite_cmd = [PY, "-m", "jupyter", "lite"]
         lite_args = ["--debug", "--LiteBuildConfig.federated_extensions", EXT_WHL]
         extra_args = extra_args or []
         return doit.tools.CmdAction(
```

### Comparing `pidgy-2023.1.7.post1/.github/workflows/publish.yml` & `pidgy-2023.4.20/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/.pytest_cache/v/cache/lastfailed` & `pidgy-2023.4.20/.pytest_cache/v/cache/lastfailed`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8666666666666667%*

 * *Differences: {"'Untitled.ipynb::Cell 0'": 'True',*

 * * "'docs/magics.ipynb::Cell 4'": 'True',*

 * * "'docs/magics.ipynb::Cell 5'": 'True',*

 * * "'docs/reactivity.ipynb::Cell 4'": 'True',*

 * * "'site/run/files/basics.ipynb::Cell 1'": 'True',*

 * * "'site/run/files/basics.ipynb::Cell 2'": 'True',*

 * * "'site/run/files/basics.ipynb::Cell 3'": 'True',*

 * * "'site/run/files/basics.ipynb::Cell 4'": 'True',*

 * * "'site/run/files/basics.ipynb::Cell 5'": 'True',*

 * * "'site/run/files/magics.ipynb::Cell 2'": 'True'}*

```diff
@@ -1,8 +1,9 @@
 {
+    "Untitled.ipynb::Cell 0": true,
     "_build/html/_/files/pidgy_examples.md.ipynb::Cell 0": true,
     "_build/html/_/files/pidgy_examples.md.ipynb::Cell 1": true,
     "_build/html/_/files/pidgy_examples.md.ipynb::Cell 2": true,
     "_build/html/_/files/pidgy_examples.md.ipynb::Cell 4": true,
     "_build/html/_/files/pidgy_examples.md.ipynb::Cell 5": true,
     "_build/html/_/files/tangle_examples.ipynb::Cell 1": true,
     "_build/html/_/files/tangle_examples.ipynb::Cell 10": true,
@@ -41,14 +42,17 @@
     "_build/jupyter_execute/docs/tangle_examples.ipynb::Cell 4": true,
     "_build/jupyter_execute/docs/tangle_examples.ipynb::Cell 5": true,
     "_build/jupyter_execute/docs/tangle_examples.ipynb::Cell 6": true,
     "_build/jupyter_execute/docs/tangle_examples.ipynb::Cell 7": true,
     "_build/jupyter_execute/docs/tangle_examples.ipynb::Cell 8": true,
     "_build/jupyter_execute/docs/tangle_examples.ipynb::Cell 9": true,
     "docs/2022-08-18-.ipynb::Cell 0": true,
+    "docs/magics.ipynb::Cell 4": true,
+    "docs/magics.ipynb::Cell 5": true,
+    "docs/reactivity.ipynb::Cell 4": true,
     "docs/test_extras.ipynb::Cell 6": true,
     "docs/test_suite.py::test_compare[function-docstring-minor-trailing-indent-test7]": true,
     "docs/test_suite.py::test_compare[item0]": true,
     "docs/test_suite.py::test_compare[test-indent-test0]": true,
     "lite/_/_/files/pidgy_examples.md.ipynb::Cell 0": true,
     "lite/_/_/files/pidgy_examples.md.ipynb::Cell 1": true,
     "lite/_/_/files/pidgy_examples.md.ipynb::Cell 2": true,
@@ -59,9 +63,15 @@
     "lite/_/_/files/tangle_examples.ipynb::Cell 2": true,
     "lite/_/_/files/tangle_examples.ipynb::Cell 3": true,
     "lite/_/_/files/tangle_examples.ipynb::Cell 4": true,
     "lite/_/_/files/tangle_examples.ipynb::Cell 5": true,
     "lite/_/_/files/tangle_examples.ipynb::Cell 6": true,
     "lite/_/_/files/tangle_examples.ipynb::Cell 7": true,
     "lite/_/_/files/tangle_examples.ipynb::Cell 8": true,
-    "lite/_/_/files/tangle_examples.ipynb::Cell 9": true
+    "lite/_/_/files/tangle_examples.ipynb::Cell 9": true,
+    "site/run/files/basics.ipynb::Cell 1": true,
+    "site/run/files/basics.ipynb::Cell 2": true,
+    "site/run/files/basics.ipynb::Cell 3": true,
+    "site/run/files/basics.ipynb::Cell 4": true,
+    "site/run/files/basics.ipynb::Cell 5": true,
+    "site/run/files/magics.ipynb::Cell 2": true
 }
```

### Comparing `pidgy-2023.1.7.post1/_templates/lite-demo.html` & `pidgy-2023.4.20/_templates/lite-demo.html`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/docs/pidgy_examples.md.ipynb` & `pidgy-2023.4.20/docs/pidgy_examples.md.ipynb`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/docs/tangle_examples.ipynb` & `pidgy-2023.4.20/docs/tangle_examples.ipynb`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/docs/test_extras.ipynb` & `pidgy-2023.4.20/docs/test_extras.ipynb`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/docs/coverage/coverage_html.js` & `pidgy-2023.4.20/docs/coverage/coverage_html.js`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/docs/coverage/favicon_32.png` & `pidgy-2023.4.20/docs/coverage/favicon_32.png`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/docs/coverage/keybd_closed.png` & `pidgy-2023.4.20/docs/coverage/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/docs/coverage/keybd_open.png` & `pidgy-2023.4.20/docs/coverage/keybd_open.png`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/docs/coverage/style.css` & `pidgy-2023.4.20/docs/coverage/style.css`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/lite/overrides.json` & `pidgy-2023.4.20/lite/overrides.json`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/.eslintrc.js` & `pidgy-2023.4.20/lite/jupyterlite-pidgy/.eslintrc.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -8,14 +8,19 @@
     parser: '@typescript-eslint/parser',
     parserOptions: {
         project: 'tsconfig.json',
         sourceType: 'module'
     },
     plugins: ['@typescript-eslint'],
     rules: {
+        '@typescript-eslint/ban-ts-comment': [
+            'error', {
+                'ts-ignore': 'allow-with-description'
+            },
+        ],
         '@typescript-eslint/naming-convention': [
             'error', {
                 'selector': 'interface',
                 'format': ['PascalCase'],
                 'custom': {
                     'regex': '^I[A-Z]',
                     'match': true
```

### Comparing `pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/README.md` & `pidgy-2023.4.20/lite/jupyterlite-pidgy/README.md`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/package.json` & `pidgy-2023.4.20/lite/jupyterlite-pidgy/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9886363636363636%*

 * *Differences: {"'dependencies'": "{'@jupyterlite/kernel': '^0.1.0-beta.18', '@jupyterlite/pyolite-kernel': "*

 * *                   "'0.1.0-beta.18', '@jupyterlite/server': '^0.1.0-beta.18'}"}*

```diff
@@ -3,17 +3,17 @@
         "email": "deathbeds@users.noreply.github.com",
         "name": "deathbeds"
     },
     "bugs": {
         "url": "https://github.com/deathbeds/pidgy/issues"
     },
     "dependencies": {
-        "@jupyterlite/kernel": "^0.1.0-alpha.20",
-        "@jupyterlite/pyolite-kernel": "0.1.0-alpha.20",
-        "@jupyterlite/server": "^0.1.0-alpha.20"
+        "@jupyterlite/kernel": "^0.1.0-beta.18",
+        "@jupyterlite/pyolite-kernel": "0.1.0-beta.18",
+        "@jupyterlite/server": "^0.1.0-beta.18"
     },
     "description": "A pidgy kernel for JupyterLite",
     "devDependencies": {
         "@jupyterlab/builder": "^3.2.0",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
```

### Comparing `pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/setup.cfg` & `pidgy-2023.4.20/lite/jupyterlite-pidgy/setup.cfg`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/setup.py` & `pidgy-2023.4.20/lite/jupyterlite-pidgy/setup.py`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/tsconfig.json` & `pidgy-2023.4.20/lite/jupyterlite-pidgy/tsconfig.json`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/yarn.lock` & `pidgy-2023.4.20/lite/jupyterlite-pidgy/yarn.lock`

 * *Files 4% similar despite different names*

```diff
@@ -123,267 +123,379 @@
     prettier "~2.1.1"
     process "^0.11.10"
     semver "^7.3.2"
     sort-package-json "~1.44.0"
     typescript "~4.1.3"
     verdaccio "^5.1.1"
 
-"@jupyterlab/coreutils@^5.2.8", "@jupyterlab/coreutils@~5.2.6":
-  version "5.2.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/coreutils/-/coreutils-5.2.8.tgz#8bb3456d0d98450b73e2aa3729bda83d42943a87"
-  integrity sha512-Qto/4ayWIkDnovK/myse2xbcs6MmShtK0MntQCipp+rdIX3T6m6UHPX5AURB9vuJoZmnx57KsejOhuYxJXHBIw==
-  dependencies:
-    "@lumino/coreutils" "^1.5.3"
-    "@lumino/disposable" "^1.4.3"
-    "@lumino/signaling" "^1.4.3"
+"@jupyterlab/coreutils@^5.5.3", "@jupyterlab/coreutils@~5.5.2":
+  version "5.5.3"
+  resolved "https://registry.npmjs.org/@jupyterlab/coreutils/-/coreutils-5.5.3.tgz#3e10a7a94d6c88f10e51cf7b94b76a5d0782a821"
+  integrity sha512-GCAymoQAwscE8MGH7eb366bRxvWawOXKFeyq642SAtl0/xWty8Kem56UfdUdyTCRzxwYW5r1sJuRHBvbTjnvUA==
+  dependencies:
+    "@lumino/coreutils" "^1.11.0"
+    "@lumino/disposable" "^1.10.0"
+    "@lumino/signaling" "^1.10.0"
     minimist "~1.2.0"
     moment "^2.24.0"
     path-browserify "^1.0.0"
     url-parse "~1.5.1"
 
-"@jupyterlab/nbformat@^3.2.8", "@jupyterlab/nbformat@~3.2.6":
-  version "3.2.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.2.8.tgz#5ddabda4cddc64498828b43bb9f01dada4981842"
-  integrity sha512-w73u+8CKSkSBaqyshrfRDyTGRVGpOmJPQFMVJYkymdVoJYlcdNOUJgXp3kp66xvXYxiE94rG3i3thJNospobQw==
-  dependencies:
-    "@lumino/coreutils" "^1.5.3"
-
-"@jupyterlab/observables@^4.2.8", "@jupyterlab/observables@~4.2.6":
-  version "4.2.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/observables/-/observables-4.2.8.tgz#d0a1b2dbb84751cf545c87455f47a2e3200ce8e3"
-  integrity sha512-jHLkhsVj3cA01hCZR3gGYTBiactQGLjFvX4OSGs3P8XQ9P4qIKTNy+hmAmzWtvBTjjTo0FI97yJIA+oDkq+J1Q==
-  dependencies:
-    "@lumino/algorithm" "^1.3.3"
-    "@lumino/coreutils" "^1.5.3"
-    "@lumino/disposable" "^1.4.3"
-    "@lumino/messaging" "^1.4.3"
-    "@lumino/signaling" "^1.4.3"
-
-"@jupyterlab/services@~6.2.6":
-  version "6.2.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/services/-/services-6.2.8.tgz#20537b3b86a2fd1029775c54be84d0a2682ffdb6"
-  integrity sha512-s6WZZe2MpGGiiLU9fp7FGOKjg84STVV8gXcaDO438m/B16/z9J1Si70OEM+XwELqPTgMna13BONfb73Ygipc2A==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.2.8"
-    "@jupyterlab/nbformat" "^3.2.8"
-    "@jupyterlab/observables" "^4.2.8"
-    "@jupyterlab/settingregistry" "^3.2.8"
-    "@jupyterlab/statedb" "^3.2.8"
-    "@lumino/algorithm" "^1.3.3"
-    "@lumino/coreutils" "^1.5.3"
-    "@lumino/disposable" "^1.4.3"
-    "@lumino/polling" "^1.3.3"
-    "@lumino/signaling" "^1.4.3"
+"@jupyterlab/nbformat@^3.5.3", "@jupyterlab/nbformat@~3.5.2":
+  version "3.5.3"
+  resolved "https://registry.npmjs.org/@jupyterlab/nbformat/-/nbformat-3.5.3.tgz#7368770488832fbf359a67677d17cd5adedb777b"
+  integrity sha512-7HIdRXrm5BKrP4P1cT+b34BFiqmEcr5fJyyBW6nIm3DXh9ZNTKhQUN8vGvkL7qTXZFXmdhc//eTSZUPQ3F3JcA==
+  dependencies:
+    "@lumino/coreutils" "^1.11.0"
+
+"@jupyterlab/observables@^4.5.3", "@jupyterlab/observables@~4.5.2":
+  version "4.5.3"
+  resolved "https://registry.npmjs.org/@jupyterlab/observables/-/observables-4.5.3.tgz#2d36e9c65a9e22c362d16b8889f9bf011a3677ae"
+  integrity sha512-WERivf/gr2ZMGCXEiJpgv4AGVG8ovKzdg/tIgzrf72eB4Jq5WXMy4r5GLvM+g3PkiiG8o50C2t/SXcUlvNDTaw==
+  dependencies:
+    "@lumino/algorithm" "^1.9.0"
+    "@lumino/coreutils" "^1.11.0"
+    "@lumino/disposable" "^1.10.0"
+    "@lumino/messaging" "^1.10.0"
+    "@lumino/signaling" "^1.10.0"
+
+"@jupyterlab/services@~6.5.2":
+  version "6.5.3"
+  resolved "https://registry.npmjs.org/@jupyterlab/services/-/services-6.5.3.tgz#b0ecf9d42c7a2261df4cb812e5c6c44b2da44a7e"
+  integrity sha512-9wIVzKeAvgx9J0g9DoG96yauG+HU4/ms28DM+7iS34/akoHSM17czWGGnmKY0Y3MyZ22up7aZelCthP+WiAQxQ==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.5.3"
+    "@jupyterlab/nbformat" "^3.5.3"
+    "@jupyterlab/observables" "^4.5.3"
+    "@jupyterlab/settingregistry" "^3.5.3"
+    "@jupyterlab/statedb" "^3.5.3"
+    "@lumino/algorithm" "^1.9.0"
+    "@lumino/coreutils" "^1.11.0"
+    "@lumino/disposable" "^1.10.0"
+    "@lumino/polling" "^1.9.0"
+    "@lumino/signaling" "^1.10.0"
     node-fetch "^2.6.0"
     ws "^7.4.6"
 
-"@jupyterlab/settingregistry@^3.2.8", "@jupyterlab/settingregistry@~3.2.6":
-  version "3.2.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/settingregistry/-/settingregistry-3.2.8.tgz#03d70b11fa7eedfa017614ad5ba8b226c51385bd"
-  integrity sha512-8YuGSGsmsKwix5EOMkkp62XxujyO02Cr4//W+bCGfqedwB3CxePuwy9ze8zuZJGKJxR4RtSUMsj43nPKmeVV3Q==
-  dependencies:
-    "@jupyterlab/statedb" "^3.2.8"
-    "@lumino/commands" "^1.12.0"
-    "@lumino/coreutils" "^1.5.3"
-    "@lumino/disposable" "^1.4.3"
-    "@lumino/signaling" "^1.4.3"
+"@jupyterlab/settingregistry@^3.5.3", "@jupyterlab/settingregistry@~3.5.2":
+  version "3.5.3"
+  resolved "https://registry.npmjs.org/@jupyterlab/settingregistry/-/settingregistry-3.5.3.tgz#b961bd5829cf1b95df10b00bed0eb7edcf341e8a"
+  integrity sha512-PWkISgGHikSaOEOiPVIDCcnLdiuXAcFdI7ZPLWoaq0v+NykemenQ5+MXOEaEOgf3KUAE8PFAGNr+3indbwFXNw==
+  dependencies:
+    "@jupyterlab/statedb" "^3.5.3"
+    "@lumino/commands" "^1.19.0"
+    "@lumino/coreutils" "^1.11.0"
+    "@lumino/disposable" "^1.10.0"
+    "@lumino/signaling" "^1.10.0"
     ajv "^6.12.3"
     json5 "^2.1.1"
 
-"@jupyterlab/statedb@^3.2.8", "@jupyterlab/statedb@~3.2.6":
-  version "3.2.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/statedb/-/statedb-3.2.8.tgz#c158bff0d4b106bd5e0ef716327d0ee7f78e58a9"
-  integrity sha512-8eaH9jvu2nZOOkUqojuEXRyrDp9qCRoVNlHMiX1v0voro4ldR0ipOPybhbI5BX2kGWEamSCKfVUQqI2+KlOSzQ==
+"@jupyterlab/statedb@^3.5.3", "@jupyterlab/statedb@~3.5.2":
+  version "3.5.3"
+  resolved "https://registry.npmjs.org/@jupyterlab/statedb/-/statedb-3.5.3.tgz#7d8fda70c315400a548eda16a418cd8d701de87a"
+  integrity sha512-QlFLcSzOJUjjwiXjgv5dQVHTRXXBT5+e/kJKVLddi80li/p0hBmKQHP+9e15Ql+i599uyoE6zE7lyMRPHrO98w==
+  dependencies:
+    "@lumino/commands" "^1.19.0"
+    "@lumino/coreutils" "^1.11.0"
+    "@lumino/disposable" "^1.10.0"
+    "@lumino/properties" "^1.8.0"
+    "@lumino/signaling" "^1.10.0"
+
+"@jupyterlite/contents@^0.1.0-beta.18":
+  version "0.1.0-beta.18"
+  resolved "https://registry.yarnpkg.com/@jupyterlite/contents/-/contents-0.1.0-beta.18.tgz#81a802cd05b104c625901421aec662dc81977c4c"
+  integrity sha512-O6iOFD8MwfB3xOa2De1JtIIbdn63dXio40g2XnQlLbH3hPgUeTE2p1Vl9VjTQmULH/e3SjtJAjFpKYgTfkMr0g==
+  dependencies:
+    "@jupyterlab/nbformat" "~3.5.2"
+    "@jupyterlab/services" "~6.5.2"
+    "@jupyterlite/localforage" "^0.1.0-beta.18"
+    "@lumino/coreutils" "^1.12.0"
+    "@types/emscripten" "^1.39.6"
+    localforage "^1.9.0"
+    mime "^3.0.0"
+
+"@jupyterlite/kernel@^0.1.0-beta.18":
+  version "0.1.0-beta.18"
+  resolved "https://registry.yarnpkg.com/@jupyterlite/kernel/-/kernel-0.1.0-beta.18.tgz#5c6051f2f6d00c0b0a38fdcc3148a132402d6be6"
+  integrity sha512-GHZMBee085Z1BYyBIm3tJt2Le1K3WCFZRihG/99Xj0l3gaY8SGGvvUHuMNirFwyjmghXYdfckYafEcZouIAjnQ==
+  dependencies:
+    "@jupyterlab/coreutils" "~5.5.2"
+    "@jupyterlab/observables" "~4.5.2"
+    "@jupyterlab/services" "~6.5.2"
+    "@lumino/coreutils" "^1.12.0"
+    "@lumino/disposable" "^1.10.1"
+    "@lumino/signaling" "^1.10.1"
+    async-mutex "^0.3.1"
+    comlink "^4.3.1"
+    mock-socket "^9.1.0"
+
+"@jupyterlite/localforage@^0.1.0-beta.18":
+  version "0.1.0-beta.18"
+  resolved "https://registry.yarnpkg.com/@jupyterlite/localforage/-/localforage-0.1.0-beta.18.tgz#68d30d43d0fb1642cba87904b413468f7e3b221a"
+  integrity sha512-ukPXjs+thOG86IPoZmHQOBfNj1WfS4BgpRX1els6zL0yWITkpsLAju0LTF9A5Hsu0VdrtNq5KPvhmGShsZmJ7Q==
   dependencies:
-    "@lumino/commands" "^1.12.0"
+    "@jupyterlab/coreutils" "~5.5.2"
     "@lumino/coreutils" "^1.5.3"
-    "@lumino/disposable" "^1.4.3"
-    "@lumino/properties" "^1.2.3"
-    "@lumino/signaling" "^1.4.3"
-
-"@jupyterlite/contents@^0.1.0-alpha.20":
-  version "0.1.0-alpha.20"
-  resolved "https://registry.yarnpkg.com/@jupyterlite/contents/-/contents-0.1.0-alpha.20.tgz#f35b3525b80b6249be702edace374fb5483f0991"
-  integrity sha512-VEcjnagQvvy4ORjMJcomCXQR8R5gMSFdRDfSHCMOBwuGVBZx+wY/d1wVsd7EL9a5NM+OLtFqgyEH/yC/kvHubw==
-  dependencies:
-    "@jupyterlab/nbformat" "~3.2.6"
-    "@jupyterlab/services" "~6.2.6"
-    "@lumino/coreutils" "^1.8.0"
     localforage "^1.9.0"
+    localforage-memoryStorageDriver "^0.9.2"
 
-"@jupyterlite/kernel@^0.1.0-alpha.20":
-  version "0.1.0-alpha.20"
-  resolved "https://registry.yarnpkg.com/@jupyterlite/kernel/-/kernel-0.1.0-alpha.20.tgz#1f549b4be89ed949b5d4ea3f14bfdd96d73e156c"
-  integrity sha512-W3ahBuW+LT0cuyTHBlSpAaAi2KVYeZ2fM3PefHp5cfkKtUlA9FqSMs9pFzSRDU79EvGuWrvhbcYNYM64/czCkw==
-  dependencies:
-    "@jupyterlab/observables" "~4.2.6"
-    "@jupyterlab/services" "~6.2.6"
-    "@lumino/coreutils" "^1.8.0"
-    "@lumino/disposable" "^1.7.0"
-    "@lumino/signaling" "^1.7.0"
-    async-mutex "^0.3.1"
-    mock-socket "^9.0.3"
+"@jupyterlite/pyolite-kernel@0.1.0-beta.18":
+  version "0.1.0-beta.18"
+  resolved "https://registry.yarnpkg.com/@jupyterlite/pyolite-kernel/-/pyolite-kernel-0.1.0-beta.18.tgz#84295e5f05e15b507967acbcc4307f27e288ecc3"
+  integrity sha512-CsUugrlRoD+naCbOYEuhLecL9YgwH6r5TDeVfBHtlBzzP2MR+KPnwHSXbx7WiDVwzRVcG0pFrzGvRs0CQ0Rvrw==
+  dependencies:
+    "@jupyterlite/contents" "^0.1.0-beta.18"
+    "@jupyterlite/kernel" "^0.1.0-beta.18"
+    comlink "^4.3.1"
+
+"@jupyterlite/server@^0.1.0-beta.18":
+  version "0.1.0-beta.18"
+  resolved "https://registry.yarnpkg.com/@jupyterlite/server/-/server-0.1.0-beta.18.tgz#e53cedbb1f0e6c0d9552fbf11054979915002812"
+  integrity sha512-iPJi5PfVYdyqK2b9zb3Yc0VtwBzCCKMecdUT7fmma0fFJdNdYrbQJ8UljoYammPXquV/U5CXqjWPcAwVDwnwWA==
+  dependencies:
+    "@jupyterlab/coreutils" "~5.5.2"
+    "@jupyterlab/nbformat" "~3.5.2"
+    "@jupyterlab/observables" "~4.5.2"
+    "@jupyterlab/services" "~6.5.2"
+    "@jupyterlab/settingregistry" "~3.5.2"
+    "@jupyterlab/statedb" "~3.5.2"
+    "@jupyterlite/contents" "^0.1.0-beta.18"
+    "@jupyterlite/kernel" "^0.1.0-beta.18"
+    "@jupyterlite/session" "^0.1.0-beta.18"
+    "@jupyterlite/settings" "^0.1.0-beta.18"
+    "@jupyterlite/translation" "^0.1.0-beta.18"
+    "@lumino/application" "^1.27.0"
+    "@lumino/coreutils" "^1.12.0"
+    mock-socket "^9.1.0"
+
+"@jupyterlite/session@^0.1.0-beta.18":
+  version "0.1.0-beta.18"
+  resolved "https://registry.yarnpkg.com/@jupyterlite/session/-/session-0.1.0-beta.18.tgz#d178d38d9eb5e199c88cb705df801cf60a647e74"
+  integrity sha512-1ZnYGJRo90YmpcTgVQZUpYp8q4tmntB4l63IcpFJGbF4ciL+1bjZ2JUgWTJAshjHaXxbdFQCqQMfI+zMH+nVQw==
+  dependencies:
+    "@jupyterlab/coreutils" "~5.5.2"
+    "@jupyterlab/services" "~6.5.2"
+    "@jupyterlite/kernel" "^0.1.0-beta.18"
+    "@lumino/algorithm" "^1.9.1"
+    "@lumino/coreutils" "^1.12.0"
 
-"@jupyterlite/pyolite-kernel@0.1.0-alpha.20":
-  version "0.1.0-alpha.20"
-  resolved "https://registry.yarnpkg.com/@jupyterlite/pyolite-kernel/-/pyolite-kernel-0.1.0-alpha.20.tgz#cb7a555ec6b364df29487eb670d337b740b4b384"
-  integrity sha512-9KiY1iQYHhrPYqn/kDDGLZk0u/Mixa30Bz7Rowndy6zbJ2WCIwwv4SMW0Ea82JXD7oLUCecZEEGQdU4GIXH7iw==
-  dependencies:
-    "@jupyterlite/kernel" "^0.1.0-alpha.20"
-
-"@jupyterlite/server@^0.1.0-alpha.20":
-  version "0.1.0-alpha.20"
-  resolved "https://registry.yarnpkg.com/@jupyterlite/server/-/server-0.1.0-alpha.20.tgz#8a0077336c3712ad9332a99b9ac60e1a818f2471"
-  integrity sha512-dx3kHSHhB7AAyKxaDKyn9NG6iO5BXkwbDGBxzX4S7OnhG+dEexKiRSPqvhIWCdginS0UDlhBtUzWIHY5q5Jkyg==
-  dependencies:
-    "@jupyterlab/coreutils" "~5.2.6"
-    "@jupyterlab/nbformat" "~3.2.6"
-    "@jupyterlab/observables" "~4.2.6"
-    "@jupyterlab/services" "~6.2.6"
-    "@jupyterlab/settingregistry" "~3.2.6"
-    "@jupyterlab/statedb" "~3.2.6"
-    "@jupyterlite/contents" "^0.1.0-alpha.20"
-    "@jupyterlite/kernel" "^0.1.0-alpha.20"
-    "@jupyterlite/session" "^0.1.0-alpha.20"
-    "@jupyterlite/settings" "^0.1.0-alpha.20"
-    "@jupyterlite/translation" "^0.1.0-alpha.20"
-    "@lumino/application" "^1.20.0"
-    "@lumino/coreutils" "^1.8.0"
-    mock-socket "^9.0.3"
-
-"@jupyterlite/session@^0.1.0-alpha.20":
-  version "0.1.0-alpha.20"
-  resolved "https://registry.yarnpkg.com/@jupyterlite/session/-/session-0.1.0-alpha.20.tgz#7bc5bdaa43bdfeba1ac20ebb9e83751f329d3670"
-  integrity sha512-LNOpy34Sd9ow3YaXqrZ8Q7B0CMFnoQjn4bSnS0Zi7bZ7nj0MTWelxY4KD4gQNu4pJ7CGAJurpGuC6DQeSdLwDQ==
-  dependencies:
-    "@jupyterlab/services" "~6.2.6"
-    "@jupyterlite/kernel" "^0.1.0-alpha.20"
-    "@lumino/algorithm" "^1.6.0"
-    "@lumino/coreutils" "^1.8.0"
-
-"@jupyterlite/settings@^0.1.0-alpha.20":
-  version "0.1.0-alpha.20"
-  resolved "https://registry.yarnpkg.com/@jupyterlite/settings/-/settings-0.1.0-alpha.20.tgz#1979beddde18e91850c548517680825018038631"
-  integrity sha512-E0ypm+NtQFACbscQHntSmHexmac2SKPK6cZETkCHiAGNp16GyrP8U1VifLN8gWSv8noZI676PiiM+RGBlAeFQA==
-  dependencies:
-    "@jupyterlab/coreutils" "~5.2.6"
-    "@jupyterlab/settingregistry" "~3.2.6"
-    "@lumino/coreutils" "^1.8.0"
+"@jupyterlite/settings@^0.1.0-beta.18":
+  version "0.1.0-beta.18"
+  resolved "https://registry.yarnpkg.com/@jupyterlite/settings/-/settings-0.1.0-beta.18.tgz#165d2dddca265d0f86beaf8e84e61f00026d99ac"
+  integrity sha512-msTXN8auojgjFu2j411Tvp8uyKgjEyr0TSigJ8ndS4mW7zxT4oeN5tMaqwr/wuTjNclfoveRxprDz8T5VXr+Hg==
+  dependencies:
+    "@jupyterlab/coreutils" "~5.5.2"
+    "@jupyterlab/settingregistry" "~3.5.2"
+    "@jupyterlite/localforage" "^0.1.0-beta.18"
+    "@lumino/coreutils" "^1.12.0"
     json5 "^2.2.0"
     localforage "^1.9.0"
 
-"@jupyterlite/translation@^0.1.0-alpha.20":
-  version "0.1.0-alpha.20"
-  resolved "https://registry.yarnpkg.com/@jupyterlite/translation/-/translation-0.1.0-alpha.20.tgz#b08c6b713c10b28cbb2007ae2ed6c48118fd2cb0"
-  integrity sha512-DHuGJ3J+XODdfjaGX3nsYkXq3jpt3AGQmxEPFCkkS0AmmId0cvIsswRFBh1iAIMPakxEW+l+ddac80qtNrfPFg==
+"@jupyterlite/translation@^0.1.0-beta.18":
+  version "0.1.0-beta.18"
+  resolved "https://registry.yarnpkg.com/@jupyterlite/translation/-/translation-0.1.0-beta.18.tgz#8ae58f964c6752b67613833f5e725b4a0a09fb59"
+  integrity sha512-FmTSWwjeM2jaFN7b8a6Pnk6YR5QJwZPZQCSNpWxlowgnT5V9mPtbSukr7iv7VylFWfHVCaihTJtln9+0gdsDqw==
   dependencies:
-    "@jupyterlab/coreutils" "~5.2.6"
-    "@lumino/coreutils" "^1.8.0"
+    "@jupyterlab/coreutils" "~5.5.2"
+    "@lumino/coreutils" "^1.12.0"
 
-"@lumino/algorithm@^1.3.3", "@lumino/algorithm@^1.6.0", "@lumino/algorithm@^1.9.1":
+"@lumino/algorithm@^1.3.3", "@lumino/algorithm@^1.9.1":
   version "1.9.1"
   resolved "https://registry.yarnpkg.com/@lumino/algorithm/-/algorithm-1.9.1.tgz#a870598e031f5ee85e20e77ce7bfffbb0dffd7f5"
   integrity sha512-d0rj7IYRzYj6WbWSrbJbKvrfO4H0NUnXT2yjSWS/sCklpTpSp0IGmndK/X4r6gG+ev5lb5+wBg9ofUDBvoAlAw==
 
-"@lumino/application@^1.16.0", "@lumino/application@^1.20.0":
+"@lumino/algorithm@^1.9.0", "@lumino/algorithm@^1.9.2":
+  version "1.9.2"
+  resolved "https://registry.npmjs.org/@lumino/algorithm/-/algorithm-1.9.2.tgz#b95e6419aed58ff6b863a51bfb4add0f795141d3"
+  integrity sha512-Z06lp/yuhz8CtIir3PNTGnuk7909eXt4ukJsCzChsGuot2l5Fbs96RJ/FOHgwCedaX74CtxPjXHXoszFbUA+4A==
+
+"@lumino/application@^1.16.0":
   version "1.28.1"
   resolved "https://registry.yarnpkg.com/@lumino/application/-/application-1.28.1.tgz#dfefe82ad414f51659e5931e3d07989364d7625e"
   integrity sha512-BRRtWJ3mG2abZ9XwB/olGJWXeJjtflDGB/uW6ZsG53Pfu7ekyXKv0wUcijvW+HM9o3bMR+PwM7ELyXtHKkodig==
   dependencies:
     "@lumino/commands" "^1.20.0"
     "@lumino/coreutils" "^1.12.0"
     "@lumino/widgets" "^1.31.1"
 
+"@lumino/application@^1.27.0":
+  version "1.31.3"
+  resolved "https://registry.npmjs.org/@lumino/application/-/application-1.31.3.tgz#c5a9bc84212a2505be8f5d43516e0603d9100965"
+  integrity sha512-XnsXm5PD9QevJRl/pHJziYmhRKqJYjEOTL6Vh9dtKpPPML57uswOj59Pokxx/yCvym1xRF9iDVvujy3KallRwQ==
+  dependencies:
+    "@lumino/commands" "^1.21.1"
+    "@lumino/coreutils" "^1.12.1"
+    "@lumino/widgets" "^1.37.1"
+
 "@lumino/collections@^1.9.1":
   version "1.9.1"
   resolved "https://registry.yarnpkg.com/@lumino/collections/-/collections-1.9.1.tgz#268f1ec6850d5e131cfc8db232c7e1e106144aa0"
   integrity sha512-5RaRGUY7BJ/1j173sc9DCfiVf70Z0hopRnBV8/AeAaK9bJJRAYjDhlZ9O8xTyouegh6krkOfiDyjl3pwogLrQw==
   dependencies:
     "@lumino/algorithm" "^1.9.1"
 
+"@lumino/collections@^1.9.3":
+  version "1.9.3"
+  resolved "https://registry.npmjs.org/@lumino/collections/-/collections-1.9.3.tgz#370dc2d50aa91371288a4f7376bea5a3191fc5dc"
+  integrity sha512-2i2Wf1xnfTgEgdyKEpqM16bcYRIhUOGCDzaVCEZACVG9R1CgYwOe3zfn71slBQOVSjjRgwYrgLXu4MBpt6YK+g==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+
 "@lumino/commands@^1.12.0", "@lumino/commands@^1.20.0":
   version "1.20.0"
   resolved "https://registry.yarnpkg.com/@lumino/commands/-/commands-1.20.0.tgz#44c797134bb33946141a490c506420bd5f12ce0f"
   integrity sha512-xyrzDIJ9QEbcbRAwmXrjb7A7/E5MDNbnLANKwqmFVNF+4LSnF62obdvY4On3Rify3HmfX0u16Xr9gfoWPX9wLQ==
   dependencies:
     "@lumino/algorithm" "^1.9.1"
     "@lumino/coreutils" "^1.12.0"
     "@lumino/disposable" "^1.10.1"
     "@lumino/domutils" "^1.8.1"
     "@lumino/keyboard" "^1.8.1"
     "@lumino/signaling" "^1.10.1"
     "@lumino/virtualdom" "^1.14.1"
 
-"@lumino/coreutils@^1.12.0", "@lumino/coreutils@^1.5.3", "@lumino/coreutils@^1.8.0":
+"@lumino/commands@^1.19.0", "@lumino/commands@^1.21.1":
+  version "1.21.1"
+  resolved "https://registry.npmjs.org/@lumino/commands/-/commands-1.21.1.tgz#eda8b3cf5ef73b9c8ce93b3b5cf66bb053df2a76"
+  integrity sha512-d1zJmwz5bHU0BM/Rl3tRdZ7/WgXnFB0bM7x7Bf0XDlmX++jnU9k0j3mh6/5JqCGLmIApKCRwVqSaV7jPmSJlcQ==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+    "@lumino/coreutils" "^1.12.1"
+    "@lumino/disposable" "^1.10.4"
+    "@lumino/domutils" "^1.8.2"
+    "@lumino/keyboard" "^1.8.2"
+    "@lumino/signaling" "^1.11.1"
+    "@lumino/virtualdom" "^1.14.3"
+
+"@lumino/coreutils@^1.11.0", "@lumino/coreutils@^1.12.1":
+  version "1.12.1"
+  resolved "https://registry.npmjs.org/@lumino/coreutils/-/coreutils-1.12.1.tgz#79860c9937483ddf6cda87f6c2b9da8eb1a5d768"
+  integrity sha512-JLu3nTHzJk9N8ohZ85u75YxemMrmDzJdNgZztfP7F7T7mxND3YVNCkJG35a6aJ7edu1sIgCjBxOvV+hv27iYvQ==
+
+"@lumino/coreutils@^1.12.0", "@lumino/coreutils@^1.5.3":
   version "1.12.0"
   resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-1.12.0.tgz#fbdef760f736eaf2bd396a5c6fc3a68a4b449b15"
   integrity sha512-DSglh4ylmLi820CNx9soJmDJCpUgymckdWeGWuN0Ash5g60oQvrQDfosVxEhzmNvtvXv45WZEqSBzDP6E5SEmQ==
 
-"@lumino/disposable@^1.10.1", "@lumino/disposable@^1.4.3", "@lumino/disposable@^1.7.0":
+"@lumino/disposable@^1.10.0", "@lumino/disposable@^1.10.4":
+  version "1.10.4"
+  resolved "https://registry.npmjs.org/@lumino/disposable/-/disposable-1.10.4.tgz#73b452044fecf988d7fa73fac9451b1a7f987323"
+  integrity sha512-4ZxyYcyzUS+ZeB2KAH9oAH3w0DUUceiVr+FIZHZ2TAYGWZI/85WlqJtfm0xjwEpCwLLW1TDqJrISuZu3iMmVMA==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+    "@lumino/signaling" "^1.11.1"
+
+"@lumino/disposable@^1.10.1", "@lumino/disposable@^1.4.3":
   version "1.10.1"
   resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-1.10.1.tgz#58fddc619cf89335802d168564b76ff5315d5a84"
   integrity sha512-mZQILc8sVGZC7mJNOGVmehDRO9/u3sIRdjZ+pCYjDgXKcINLd6HoPhZDquKCWiRBfHTL1B3tOHjnBhahBc2N/Q==
   dependencies:
     "@lumino/algorithm" "^1.9.1"
     "@lumino/signaling" "^1.10.1"
 
 "@lumino/domutils@^1.2.3", "@lumino/domutils@^1.8.1":
   version "1.8.1"
   resolved "https://registry.yarnpkg.com/@lumino/domutils/-/domutils-1.8.1.tgz#cf118e4eba90c3bf1e3edf7f19cce8846ec7875c"
   integrity sha512-QUVXwmDMIfcHC3yslhmyGK4HYBKaJ3xX5MTwDrjsSX7J7AZ4jwL4zfsxyF9ntdqEKraoJhLQ6BaUBY+Ur1cnYw==
 
+"@lumino/domutils@^1.8.2":
+  version "1.8.2"
+  resolved "https://registry.npmjs.org/@lumino/domutils/-/domutils-1.8.2.tgz#d15cdbae12bea52852bbc13c4629360f9f05b7f5"
+  integrity sha512-QIpMfkPJrs4GrWBuJf2Sn1fpyVPmvqUUAeD8xAQo8+4V5JAT0vUDLxZ9HijefMgNCi3+Bs8Z3lQwRCrz+cFP1A==
+
 "@lumino/dragdrop@^1.14.0", "@lumino/dragdrop@^1.7.1":
   version "1.14.0"
   resolved "https://registry.yarnpkg.com/@lumino/dragdrop/-/dragdrop-1.14.0.tgz#48baacc190518d0cb563698daa0d5b976d6fe5c3"
   integrity sha512-hO8sgF0BkpihKIP6UZgVJgiOEhz89i7Oxtp9FR9Jqw5alGocxSXt7q3cteMvqpcL6o2/s3CafZNRkVLRXmepNw==
   dependencies:
     "@lumino/coreutils" "^1.12.0"
     "@lumino/disposable" "^1.10.1"
 
+"@lumino/dragdrop@^1.14.4":
+  version "1.14.4"
+  resolved "https://registry.npmjs.org/@lumino/dragdrop/-/dragdrop-1.14.4.tgz#b6ec4cf4f470c17a849e31f299d5a24acdc8c7d3"
+  integrity sha512-IHX2M8Yqs2YsFHHXKSKiYLgv9DEuhyyKoDS85Chg34J9OaPC5ocT0AmNVnpeq9T4A50sg3vdL9mSRCZ0f302Gw==
+  dependencies:
+    "@lumino/coreutils" "^1.12.1"
+    "@lumino/disposable" "^1.10.4"
+
 "@lumino/keyboard@^1.8.1":
   version "1.8.1"
   resolved "https://registry.yarnpkg.com/@lumino/keyboard/-/keyboard-1.8.1.tgz#e7850e2fb973fbb4c6e737ca8d9307f2dc3eb74b"
   integrity sha512-8x0y2ZQtEvOsblpI2gfTgf+gboftusP+5aukKEsgNQtzFl28RezQXEOSVd8iD3K6+Q1MaPQF0OALYP0ASqBjBg==
 
+"@lumino/keyboard@^1.8.2":
+  version "1.8.2"
+  resolved "https://registry.npmjs.org/@lumino/keyboard/-/keyboard-1.8.2.tgz#714dbe671f0718f516d1ec23188b31a9ccd82fb2"
+  integrity sha512-Dy+XqQ1wXbcnuYtjys5A0pAqf4SpAFl9NY6owyIhXAo0Va7w3LYp3jgiP1xAaBAwMuUppiUAfrbjrysZuZ625g==
+
+"@lumino/messaging@^1.10.0", "@lumino/messaging@^1.10.3":
+  version "1.10.3"
+  resolved "https://registry.npmjs.org/@lumino/messaging/-/messaging-1.10.3.tgz#b6227bdfc178a8542571625ecb68063691b6af3c"
+  integrity sha512-F/KOwMCdqvdEG8CYAJcBSadzp6aI7a47Fr60zAKGqZATSRRRV41q53iXU7HjFPqQqQIvdn9Z7J32rBEAyQAzww==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+    "@lumino/collections" "^1.9.3"
+
 "@lumino/messaging@^1.10.1", "@lumino/messaging@^1.4.3":
   version "1.10.1"
   resolved "https://registry.yarnpkg.com/@lumino/messaging/-/messaging-1.10.1.tgz#b29575cca46e2f23b84626b793ec8e2be46a53ba"
   integrity sha512-XZSdt9ih94rdeeLL0cryUw6HHD51D7TP8c+MFf+YRF6VKwOFB9RoajfQWadeqpmH+schTs3EsrFfA9KHduzC7w==
   dependencies:
     "@lumino/algorithm" "^1.9.1"
     "@lumino/collections" "^1.9.1"
 
-"@lumino/polling@^1.3.3":
-  version "1.10.0"
-  resolved "https://registry.yarnpkg.com/@lumino/polling/-/polling-1.10.0.tgz#94a92811edf4c2534c741510b30f500d8c16a395"
-  integrity sha512-ZNXObJQfugnS41Yrlr7yWcFiRK+xAGGOXO08JJ0Mctsg5mT30UEGFVWJY2AjZ6N5aQuLyGed/pMkBzLzrzt8OA==
-  dependencies:
-    "@lumino/coreutils" "^1.12.0"
-    "@lumino/disposable" "^1.10.1"
-    "@lumino/signaling" "^1.10.1"
+"@lumino/polling@^1.9.0":
+  version "1.11.4"
+  resolved "https://registry.npmjs.org/@lumino/polling/-/polling-1.11.4.tgz#ddfe47da5b41af4cfa474898542c099e445c0e6c"
+  integrity sha512-yC7JLssj3mqVK6TsYj7dg4AG0rcsC42YtpoDLtz9yzO84Q5flQUfmjAPQB6oPA6wZOlISs3iasF+uO2w1ls5jg==
+  dependencies:
+    "@lumino/coreutils" "^1.12.1"
+    "@lumino/disposable" "^1.10.4"
+    "@lumino/signaling" "^1.11.1"
 
 "@lumino/properties@^1.2.3", "@lumino/properties@^1.8.1":
   version "1.8.1"
   resolved "https://registry.yarnpkg.com/@lumino/properties/-/properties-1.8.1.tgz#47eb8516e92c987dcb2c404db83a258159efec3d"
   integrity sha512-O+CCcAqP64Di32DUZ4Jqq0DtUyE5RJREN5vbkgGZGu+WauJ/RYoiLDe1ubbAeSaHk71OrS60ZBV7QyC8ZaBVsA==
 
-"@lumino/signaling@^1.10.1", "@lumino/signaling@^1.4.3", "@lumino/signaling@^1.7.0":
+"@lumino/properties@^1.8.0", "@lumino/properties@^1.8.2":
+  version "1.8.2"
+  resolved "https://registry.npmjs.org/@lumino/properties/-/properties-1.8.2.tgz#91131f2ca91a902faa138771eb63341db78fc0fd"
+  integrity sha512-EkjI9Cw8R0U+xC9HxdFSu7X1tz1H1vKu20cGvJ2gU+CXlMB1DvoYJCYxCThByHZ+kURTAap4SE5x8HvKwNPbig==
+
+"@lumino/signaling@^1.10.0", "@lumino/signaling@^1.11.1":
+  version "1.11.1"
+  resolved "https://registry.npmjs.org/@lumino/signaling/-/signaling-1.11.1.tgz#438f447a1b644fd286549804f9851b5aec9679a2"
+  integrity sha512-YCUmgw08VoyMN5KxzqPO3KMx+cwdPv28tAN06C0K7Q/dQf+oufb1XocuhZb5selTrTmmuXeizaYxgLIQGdS1fA==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+    "@lumino/properties" "^1.8.2"
+
+"@lumino/signaling@^1.10.1", "@lumino/signaling@^1.4.3":
   version "1.10.1"
   resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-1.10.1.tgz#c8a1cb5b661b6744ea817c99c758fdc897847c26"
   integrity sha512-GZVbX4cfk/ZqLwkemPD/NwqToaTL/6q7qdLpEhgkiPlaH1S5/V7fDpP7N1uFy4n3BDITId8cpYgH/Ds32Mdp3A==
   dependencies:
     "@lumino/algorithm" "^1.9.1"
 
 "@lumino/virtualdom@^1.14.1", "@lumino/virtualdom@^1.8.0":
   version "1.14.1"
   resolved "https://registry.yarnpkg.com/@lumino/virtualdom/-/virtualdom-1.14.1.tgz#2551b146cbe87c48d23754f370c1331a60c9fe62"
   integrity sha512-imIJd/wtRkoR1onEiG5nxPEaIrf70nn4PgD/56ri3/Lo6AJEX2CusF6iIA27GVB8yl/7CxgTHUnzzCwTFPypcA==
   dependencies:
     "@lumino/algorithm" "^1.9.1"
 
+"@lumino/virtualdom@^1.14.3":
+  version "1.14.3"
+  resolved "https://registry.npmjs.org/@lumino/virtualdom/-/virtualdom-1.14.3.tgz#e490c36ff506d877cf45771d6968e3e26a8919fd"
+  integrity sha512-5joUC1yuxeXbpfbSBm/OR8Mu9HoTo6PDX0RKqzlJ9o97iml7zayFN/ynzcxScKGQAo9iaXOY8uVIvGUT8FnsGw==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+
 "@lumino/widgets@^1.19.0", "@lumino/widgets@^1.31.1":
   version "1.31.1"
   resolved "https://registry.yarnpkg.com/@lumino/widgets/-/widgets-1.31.1.tgz#c9c0b8c7940b412e55369fa277392bf86c6e4136"
   integrity sha512-4RzAMqWwWHa5IiaQaeIbiZdIBm/FOg6ub0w8dG3km0k+zIQyA4LFq2dbB1w6SHT1d06N+L/ebYfgvMFswPENag==
   dependencies:
     "@lumino/algorithm" "^1.9.1"
     "@lumino/commands" "^1.20.0"
@@ -393,14 +505,31 @@
     "@lumino/dragdrop" "^1.14.0"
     "@lumino/keyboard" "^1.8.1"
     "@lumino/messaging" "^1.10.1"
     "@lumino/properties" "^1.8.1"
     "@lumino/signaling" "^1.10.1"
     "@lumino/virtualdom" "^1.14.1"
 
+"@lumino/widgets@^1.37.1":
+  version "1.37.1"
+  resolved "https://registry.npmjs.org/@lumino/widgets/-/widgets-1.37.1.tgz#d7a2398b276e15e60aff4fec58c035d46549a75b"
+  integrity sha512-/whz5B/hL0fjv0bR8JYZ+Emx+CH7HBwXc4TqI9PrrHGm3g6+jRJAyIFGZcQubqkPxxHrRE/VxQgoDKGhINw/Gw==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+    "@lumino/commands" "^1.21.1"
+    "@lumino/coreutils" "^1.12.1"
+    "@lumino/disposable" "^1.10.4"
+    "@lumino/domutils" "^1.8.2"
+    "@lumino/dragdrop" "^1.14.4"
+    "@lumino/keyboard" "^1.8.2"
+    "@lumino/messaging" "^1.10.3"
+    "@lumino/properties" "^1.8.2"
+    "@lumino/signaling" "^1.11.1"
+    "@lumino/virtualdom" "^1.14.3"
+
 "@nodelib/fs.scandir@2.1.5":
   version "2.1.5"
   resolved "https://registry.yarnpkg.com/@nodelib/fs.scandir/-/fs.scandir-2.1.5.tgz#7619c2eb21b25483f6d167548b4cfd5a7488c3d5"
   integrity sha512-vq24Bq3ym5HEQm2NKCr3yXDwjc7vTsEThRDnkp2DK9p1uqLR+DHurm/NOTo0KG7HYHU7eppKZj3MyqYuMBf62g==
   dependencies:
     "@nodelib/fs.stat" "2.0.5"
     run-parallel "^1.1.9"
@@ -442,14 +571,19 @@
 "@szmarczak/http-timer@^1.1.2":
   version "1.1.2"
   resolved "https://registry.yarnpkg.com/@szmarczak/http-timer/-/http-timer-1.1.2.tgz#b1665e2c461a2cd92f4c1bbf50d5454de0d4b421"
   integrity sha512-XIB2XbzHTN6ieIjfIMV9hlVcfPU26s2vafYWQcZHWXHOxiaRZYEDKEwdl129Zyg50+foYV2jCgtrqSA6qNuNSA==
   dependencies:
     defer-to-connect "^1.0.1"
 
+"@types/emscripten@^1.39.6":
+  version "1.39.6"
+  resolved "https://registry.yarnpkg.com/@types/emscripten/-/emscripten-1.39.6.tgz#698b90fe60d44acf93c31064218fbea93fbfd85a"
+  integrity sha512-H90aoynNhhkQP6DRweEjJp5vfUVdIj7tdPLsu7pq89vODD/lcugKfZOsfgwpvM6XUewEp2N5dCg1Uf3Qe55Dcg==
+
 "@types/eslint-scope@^3.7.0":
   version "3.7.3"
   resolved "https://registry.yarnpkg.com/@types/eslint-scope/-/eslint-scope-3.7.3.tgz#125b88504b61e3c8bc6f870882003253005c3224"
   integrity sha512-PB3ldyrcnAicT35TWPs5IcwKD8S333HMaa2VVv4+wdvebJkjWuW/xESoB8IwRcog8HYVYamb1g/R31Qv5Bx03g==
   dependencies:
     "@types/eslint" "*"
     "@types/estree" "*"
@@ -1249,14 +1383,19 @@
 combined-stream@^1.0.6, combined-stream@~1.0.6:
   version "1.0.8"
   resolved "https://registry.yarnpkg.com/combined-stream/-/combined-stream-1.0.8.tgz#c3d45a8b34fd730631a110a8a2520682b31d5a7f"
   integrity sha512-FQN4MRfuJeHf7cBbBMJFXhKSDq+2kAArBlmRBvcvFE5BB1HZKXtSFASDhdlz9zOYwxh8lDdnvmMOe/+5cdoEdg==
   dependencies:
     delayed-stream "~1.0.0"
 
+comlink@^4.3.1:
+  version "4.4.1"
+  resolved "https://registry.yarnpkg.com/comlink/-/comlink-4.4.1.tgz#e568b8e86410b809e8600eb2cf40c189371ef981"
+  integrity sha512-+1dlx0aY5Jo1vHy/tSsIGpSkN4tS9rZSW8FIhG0JH/crs9wwweswIo/POr451r7bZww3hFbPAKnTpimzL/mm4Q==
+
 commander@^2.20.0:
   version "2.20.3"
   resolved "https://registry.yarnpkg.com/commander/-/commander-2.20.3.tgz#fd485e84c03eb4881c20722ba48035e8531aeb33"
   integrity sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==
 
 commander@^7.0.0:
   version "7.2.0"
@@ -2841,21 +2980,26 @@
 json5@^1.0.1:
   version "1.0.1"
   resolved "https://registry.yarnpkg.com/json5/-/json5-1.0.1.tgz#779fb0018604fa854eacbf6252180d83543e3dbe"
   integrity sha512-aKS4WQjPenRxiQsC93MNfjx+nbF4PAdYzmd/1JIj8HYzqfbu86beTuNgXDzPknWk0n0uARlyewZo4s++ES36Ow==
   dependencies:
     minimist "^1.2.0"
 
-json5@^2.1.1, json5@^2.1.2, json5@^2.2.0:
+json5@^2.1.1, json5@^2.1.2:
   version "2.2.0"
   resolved "https://registry.yarnpkg.com/json5/-/json5-2.2.0.tgz#2dfefe720c6ba525d9ebd909950f0515316c89a3"
   integrity sha512-f+8cldu7X/y7RAJurMEJmdoKXGB/X550w2Nr3tTbezL6RwEE/iMcm+tZnXeoZtKuOq6ft8+CqzEkrIgx1fPoQA==
   dependencies:
     minimist "^1.2.5"
 
+json5@^2.2.0:
+  version "2.2.3"
+  resolved "https://registry.npmjs.org/json5/-/json5-2.2.3.tgz#78cd6f1a19bdc12b73db5ad0c61efd66c1e29283"
+  integrity sha512-XmOWe7eyHYH14cLdVPoyg+GOH3rYX++KpzrylJwSW98t3Nk+U8XOl8FWKOgwtzdb8lXGf6zYwDUzeHMWfxasyg==
+
 jsonfile@^6.0.1:
   version "6.1.0"
   resolved "https://registry.yarnpkg.com/jsonfile/-/jsonfile-6.1.0.tgz#bc55b2634793c679ec6403094eb13698a6ec0aae"
   integrity sha512-5dgndWOriYSm5cnYaJNhalLNDKOqFwyDB/rr1E9ZsGciGvKPs8R2xYGCacuf3z6K1YKDz182fd+fY3cn3pMqXQ==
   dependencies:
     universalify "^2.0.0"
   optionalDependencies:
@@ -2993,15 +3137,22 @@
   resolved "https://registry.yarnpkg.com/loader-utils/-/loader-utils-2.0.2.tgz#d6e3b4fb81870721ae4e0868ab11dd638368c129"
   integrity sha512-TM57VeHptv569d/GKh6TAYdzKblwDNiumOdkFnejjD0XwTH87K90w3O7AiJRqdQoXygvi1VQTJTLGhJl7WqA7A==
   dependencies:
     big.js "^5.2.2"
     emojis-list "^3.0.0"
     json5 "^2.1.2"
 
-localforage@^1.9.0:
+localforage-memoryStorageDriver@^0.9.2:
+  version "0.9.2"
+  resolved "https://registry.yarnpkg.com/localforage-memoryStorageDriver/-/localforage-memoryStorageDriver-0.9.2.tgz#2e0f7ff2acb0e9ff5e82c52c9e2eb3d63b998d30"
+  integrity sha512-DRB4BkkW9o5HIetbsuvtcg98GP7J1JBRDyDMJK13hfr9QsNpnMW6UUWmU9c6bcRg99akR1mGZ/ubUV1Ek0fbpg==
+  dependencies:
+    localforage ">=1.4.0"
+
+localforage@>=1.4.0, localforage@^1.9.0:
   version "1.10.0"
   resolved "https://registry.yarnpkg.com/localforage/-/localforage-1.10.0.tgz#5c465dc5f62b2807c3a84c0c6a1b1b3212781dd4"
   integrity sha512-14/H1aX7hzBBmmh7sGPd+AOMkkIrHM3Z1PAyGgZigA1H1p5O5ANnMyWzvpAETtG68/dC4pC0ncy3+PPGzXZHPg==
   dependencies:
     lie "3.1.1"
 
 locate-path@^5.0.0:
@@ -3207,14 +3358,19 @@
   integrity sha512-x0Vn8spI+wuJ1O6S7gnbaQg8Pxh4NNHb7KSINmEWKiPE4RKOplvijn+NkmYmmRgP68mc70j2EbeTFRsrswaQeg==
 
 mime@2.6.0:
   version "2.6.0"
   resolved "https://registry.yarnpkg.com/mime/-/mime-2.6.0.tgz#a2a682a95cd4d0cb1d6257e28f83da7e35800367"
   integrity sha512-USPkMeET31rOMiarsBNIHZKLGgvKc/LrjofAnBlOttf5ajRvqiRA8QsenbcooctK6d6Ts6aqZXBA+XbkKthiQg==
 
+mime@^3.0.0:
+  version "3.0.0"
+  resolved "https://registry.yarnpkg.com/mime/-/mime-3.0.0.tgz#b374550dca3a0c18443b0c950a6a58f1931cf7a7"
+  integrity sha512-jSCU7/VB1loIWBZe14aEYHU/+1UMEHoaO7qxCOVJOw9GgH72VAWppxNcjU+x9a2k3GSIBXNKxXQFqRvvZ7vr3A==
+
 mimic-fn@^2.1.0:
   version "2.1.0"
   resolved "https://registry.yarnpkg.com/mimic-fn/-/mimic-fn-2.1.0.tgz#7ed2c2ccccaf84d3ffcb7a69b57711fc2083401b"
   integrity sha512-OqbOk5oEQeAZ8WXWydlu9HJjz9WVdEIvamMCcXmuqUYjTknH/sqsWvhQ3vgwKFRR1HpjvNBKQ37nbJgYzGqGcg==
 
 mimic-response@^1.0.0, mimic-response@^1.0.1:
   version "1.0.1"
@@ -3286,15 +3442,15 @@
 mkdirp@~0.5.1:
   version "0.5.5"
   resolved "https://registry.yarnpkg.com/mkdirp/-/mkdirp-0.5.5.tgz#d91cefd62d1436ca0f41620e251288d420099def"
   integrity sha512-NKmAlESf6jMGym1++R0Ra7wvhV+wFW63FaSOFPwRahvea0gMUcGUhVeAg/0BC0wiv9ih5NYPB1Wn1UEI1/L+xQ==
   dependencies:
     minimist "^1.2.5"
 
-mock-socket@^9.0.3:
+mock-socket@^9.1.0:
   version "9.1.0"
   resolved "https://registry.yarnpkg.com/mock-socket/-/mock-socket-9.1.0.tgz#583f5984aa5759909c1b0f43676c669060722596"
   integrity sha512-zNsH8h0D7buVMDZ2X1GyFYso9A1X1Co/TDfFs0AIKhSLkJeh381HYESNl/mL6BzmQpNOxZVnNhEDS1OWBrS+cQ==
 
 moment@^2.24.0:
   version "2.29.1"
   resolved "https://registry.yarnpkg.com/moment/-/moment-2.29.1.tgz#b2be769fa31940be9eeea6469c075e35006fa3d3"
```

### Comparing `pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/src/index.ts` & `pidgy-2023.4.20/lite/jupyterlite-pidgy/src/index.ts`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 /**
  * A plugin to register the Pyodide kernel.
  */
 const kernel: JupyterLiteServerPlugin<void> = {
   id: PLUGIN_ID,
   autoStart: true,
+  // @ts-ignore: Types have separate declarations of a private property
   optional: [IKernelSpecs],
   activate: (app: JupyterLiteServer, kernelspecs: IKernelSpecs) => {
     console.log(UPSTREAM_PLUGIN_ID, PYODIDE_CDN_URL, PageConfig, URLExt, kernelspecs);
     // const baseUrl = PageConfig.getBaseUrl();
     const config =
       JSON.parse(PageConfig.getOption('litePluginSettings') || '{}')[
         UPSTREAM_PLUGIN_ID
```

### Comparing `pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/src/kernel.ts` & `pidgy-2023.4.20/lite/jupyterlite-pidgy/src/kernel.ts`

 * *Files 1% similar despite different names*

```diff
@@ -38,17 +38,15 @@
    * @param options The instantiation options for a new PyodideKernel
    */
   protected buildWorkerScript(options: PidgyKernel.IOptions): string[] {
     const { pyodideUrl } = options;
 
     const indexUrl = pyodideUrl.slice(0, pyodideUrl.lastIndexOf('/') + 1);
 
-    const { origin } = window.location;
-
-    const pypi = URLExt.join(origin, PageConfig.getOption('appUrl'), 'build/pypi');
+    const pypi = URLExt.join(PageConfig.getBaseUrl(), 'build/pypi');
 
     const pipliteUrls = [...(options.pipliteUrls || []), URLExt.join(pypi, 'all.json')];
 
     const pipliteWheelUrl = URLExt.join(pypi, PIPLITE_WHEEL);
 
     return [
       // first we need the pyodide initialization scripts...
```

### Comparing `pidgy-2023.1.7.post1/lite/jupyterlite-pidgy/src/worker.ts` & `pidgy-2023.4.20/lite/jupyterlite-pidgy/src/worker.ts`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
   // this is the only use of `loadPackage`, allow `piplite` to handle the rest
   await pyodide.loadPackage(['micropip']);
 
   // get piplite early enough to impact pyolite dependencies
   await pyodide.runPythonAsync(`
     import micropip
-    await micropip.install('${_pipliteWheelUrl}')
+    await micropip.install('${_pipliteWheelUrl}', keep_going=True)
     import piplite.piplite
     piplite.piplite._PIPLITE_DISABLE_PYPI = ${_disablePyPIFallback ? 'True' : 'False'}
     piplite.piplite._PIPLITE_URLS = ${JSON.stringify(_pipliteUrls)}
   `);
 
   // from this point forward, only use piplite
   await pyodide.runPythonAsync(`
```

### Comparing `pidgy-2023.1.7.post1/src/pidgy/README.md` & `pidgy-2023.4.20/src/pidgy/README.md`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/src/pidgy/displays.py` & `pidgy-2023.4.20/src/pidgy/displays.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """Reactive IPython/IPywidgets templates
+
+these displays combine IPython displays with jinja2 environments.
+we export multiple displays to use in different contexts.
+for example, voila prefers HTML ipywidgets based displays to gain interactivity.
 """
 # in this module we try to shield the library imports to make
 # dependencies optional. we always have markdown it and ipython.
 # ipywidgets may be optional
 
 from dataclasses import dataclass, field
 from io import StringIO
 from re import compile
 from IPython.display import DisplayHandle, display, HTML, Markdown
 
 from markdown_it import MarkdownIt
 from asyncio import ensure_future
+from . import get_ipython
 
 URL = compile("^(http[s]|file)://")
 
 
 @dataclass
 class TemplateDisplay:
     """the TemplateDisplays base class that provides the api for displaying and updating templates."""
@@ -28,53 +33,57 @@
     vars: set = field(default_factory=set)
     # this is not used by the base class but may be used by other base classes that render html
     tokens: object = None
     markdown_renderer: object = None
     use_async: bool = True
 
     def _ipython_display_(self):
+        """display the template contents"""
         if self.display_handle is None:
             self.display_handle = DisplayHandle()
 
-        if self.use_async:
+        if self.use_async and get_ipython().weave.reactive:
             self.display_handle.display(self.display_object(self.body))
             ensure_future(self.aupdate())
         else:
+            try:
+                import nest_asyncio
+
+                nest_asyncio.apply()
+            except ModuleNotFoundError:
+                raise ImportError("nest_asyncio is needed to use synchronous rendering.")
             self.display_handle.display(self.display_object(self.render()))
 
     def _is_list_urls(self, x):
         for line in filter(bool, map(str.strip, StringIO(x))):
             if URL.match(line):
                 continue
 
             return False
         return True
 
     async def arender(self):
-        render = await self.template.render_async()
-
-        if self._is_list_urls(render):
-            return self.embed(render)
+        """async template rendering"""
+        output = StringIO()
 
-        return render
+        try:
+            async for part in self.template.generate_async():
+                output.write(part)
+        except BaseException as e:
+            import traceback
+
+            msg = "".join(traceback.format_exception(type(e), e, e.__traceback__))
+            return f"""`````````pytb\n{msg}\n`````````"""
+        return output.getvalue()
 
     def render(self):
-        render = self.template.render()
-        if self.is_list_urls is None:
-            self.is_list_urls = self._is_list_urls(render)
-
-        if self.is_list_urls:
-            return self.embed(render)
-
-        return render
+        """sync template rendering"""
+        return self.template.render()
 
     def display_object(self, object, **kwargs):
-        # metadata = self.get_markdown_metadata()
-        # if metadata:
-        #     kwargs.setdefault("metadata", {"@graph": metadata})
         return self.display_cls(object, **kwargs)
 
     async def aupdate(self):
         # it should be possible to do smarter updates
         if self.display_handle:
             self.display_handle.update(self.display_object(await self.arender()))
 
@@ -152,17 +161,7 @@
     from sys import modules
 
     if "ipywidgets" in modules:
         from ipywidgets import Widget
 
         return isinstance(object, Widget)
     return False
-
-
-def is_widget_type(object):
-    from sys import modules
-
-    if "ipywidgets" in modules:
-        from ipywidgets import Widget
-
-        return issubclass(object, Widget)
-    return False
```

### Comparing `pidgy-2023.1.7.post1/src/pidgy/environment.py` & `pidgy-2023.4.20/src/pidgy/environment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,29 @@
+"""pidgy weaves commonmark markdown into rich, reactive displays."""
+
 from re import compile
 from typing import ChainMap
 
 from IPython import get_ipython
 from jinja2 import Environment, Template, Undefined
 from traitlets import Instance
 
 CELL_MAGIC = compile("^\s*%{2}\S")
 NO_SHOW = compile(r"^\s*\r?\n")
-
-from IPython import get_ipython
-
 URL = compile("^(http[s]|file)://")
 
 
-class Finalizer:
-    def __new__(cls, object):
-        return object
-
-
-class IPythonFinalizer(Finalizer):
-    """a finalizer that extracts content from IPython displays"""
+class IPythonFinalizer:
+    """a finalizer that extracts mimetype data from IPython displays"""
 
     @staticmethod
     def normalize(type, object, metadata) -> str:
         """normalize and object with (mime)type and return a string."""
-
+        # indents can affect the display when mimetypes are
+        # converted to markdown dislays 
         if type == "text/html" or "svg" in type:
             object = get_minified(object)
 
         if type.startswith("image"):
             md = metadata.get(type, {})
             width, height = md.get("width"), md.get("height")
             object = get_decoded(object)
@@ -46,58 +41,60 @@
         key = next(filter(data.__contains__, get_active_types(shell)), str(object))
         if key == "text/plain":
             return str(object)
         return cls.normalize(key, data[key], metadata)
 
 
 class IPythonEnvironment(Environment):
-    def init_filters(self):
-        try:
-            from nbconvert.exporters.templateexporter import default_filters
-
-            self.filters.update(default_filters)
-        except ModuleNotFoundError:
-            pass
+    """a jinja2 environment available in the ipython shell"""
 
+    def init_filters(self):
         from . import filters
 
         self.filters.update(
             (k, v) for k, v in vars(filters).items() if k[0].isalpha() and callable(v)
         )
 
     def __init__(self, *args, **kwargs):
         from jinja2 import ChoiceLoader, DictLoader, FileSystemLoader
 
         kwargs.setdefault("loader", ChoiceLoader([DictLoader({}), FileSystemLoader(".")]))
         kwargs.setdefault("finalize", IPythonFinalizer)
         kwargs.setdefault("undefined", Undefined)
-        kwargs.setdefault("enable_async", True)  # enable this later
+        kwargs.setdefault("enable_async", True)
         super().__init__(*args, **kwargs)
         self.init_filters()
 
 
 class IPythonTemplate(Template):
+    """an ipython shell and namespace aware jinja template"""
     def ns(self, *args, **kwargs):
         import builtins
 
         ns = get_ipython()
         if ns:
             return ChainMap(kwargs, ns.user_ns, vars(builtins))
         return {}
 
     def render(self, *args, **kwargs):
         return super().render(self.ns(*args, **kwargs))
 
     async def render_async(self, *args, **kwargs):
         return await super().render_async(self.ns(*args, **kwargs))
 
+    async def generate_async(self, *args, **kwargs):
+        async for x in super().generate_async(self.ns(*args, **kwargs)):
+            yield x
+
 
 class Undefined(Undefined):
-    def _fail_with_undefined_error(self, *args, **kwargs):
+    def __str__(self, *args, **kwargs):
         # log that the template failed
+        if self._undefined_obj:
+            return f"`{self._undefined_name} of {self._undefined_obj} is undefined`"
         return f"`{self._undefined_name} is undefined`"
 
 
 def get_active_types(shell=None):
     """get the active types in the current IPython shell.
     we ignore latex, but i forget why."""
     shell = shell or get_ipython()
```

### Comparing `pidgy-2023.1.7.post1/src/pidgy/extras.py` & `pidgy-2023.4.20/src/pidgy/extras.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,22 @@
 3. IPython display objects are added to the user namespace
 4. top-level return statement become IPython.display expressions.
 5. it should be easy to copy and paste json for beginners. 
      `true, false and null` are buultins.
 """
 
 import builtins
-from ast import Call, Expr, NodeTransformer, Tuple, parse, copy_location, fix_missing_locations
+from ast import Call, Expr, NodeTransformer, Tuple, parse, copy_location
 from pathlib import Path
 from subprocess import CalledProcessError
 
 import IPython
-from traitlets import CUnicode
-
 from . import get_ipython
 
-builtins.true, builtins.false, builtins.null = True, False, None
-
 
-# happens each execution
 def sys_modules_are_part_of_ns():
     from sys import modules
 
     shell = get_ipython()
     for k in modules:
         if k:
             if k.startswith("_"):
@@ -113,14 +108,15 @@
                 )
             ),
             node,
         )
 
 
 def load_ipython_extension(shell: IPython.InteractiveShell):
+    builtins.true, builtins.false, builtins.null = True, False, None
     shell.events.register("pre_execute", sys_modules_are_part_of_ns)
     ipython_displays_are_part_of_ns(shell)
     shell.ast_transformers.append(ReturnDisplay())
     shell.input_transformers_cleanup.append(shebang_transform)
     shell.register_magic_function(shebang_cell_magic, "cell", "/usr/bin/env")
```

### Comparing `pidgy-2023.1.7.post1/src/pidgy/kernel.py` & `pidgy-2023.4.20/src/pidgy/kernel.py`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/src/pidgy/tangle.py` & `pidgy-2023.4.20/src/pidgy/tangle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """tangle.py provides the Markdown to Python translation model.
 """
-import ast
-import dis
-import types
 from dataclasses import dataclass, field
 from io import StringIO
 from re import MULTILINE, compile
 from urllib.parse import urlparse
 
 from midgy.python import Python
 
+from .current import Execution
 from . import get_cell_id, get_ipython
 
 # an instance of this class is used to transform markdown to valid python
 # in the ipython extension. the python conversion is constrained by being
 # a line for line transformation using indent code blocks (not code fences)
 # as references for translating the markdown to valid python objects.
 
@@ -34,35 +32,28 @@
     set_current_execution(shell)
 
     lines = "".join(lines)
     if IS_MAGIC.match(lines):
         return lines.splitlines(True)
 
     tokens = shell.tangle.parse(lines)
-    if hasattr(shell, "pidgy") and shell.pidgy.current_execution:
-        shell.pidgy.current_execution.tokens = tokens
-    return shell.tangle.render_tokens(tokens, src=lines).splitlines(True)
+    if hasattr(shell, "current_execution"):
+        shell.current_execution.tokens = tokens
 
-
-@dataclass
-class Execution:
-    id: str
-    tokens: list = None
-    py: str = None
-    nodes: ast.AST = None
-    bytecode: types.CodeType = None
-    instructions: list[dis.Instruction] = None
+    shell.current_execution.py = shell.tangle.render_tokens(tokens, src=lines)
+    return shell.current_execution.py.splitlines(True)
 
 
 @dataclass
 class IPython(Python):
     """a markdown to python transpiler meant o be used in IPython"""
 
     parent: object = field(default_factory=get_ipython)
     last_tokens: list = None
+    env: dict = field(default_factory=dict)
     URL_PROTOCOLS = "file", "http", "https"
     VALID_URL_LIST_TOKENS = {
         "paragraph_open",
         "paragraph_close",
         "bullet_list_open",
         "bullet_list_close",
         "list_item_open",
@@ -85,28 +76,43 @@
                 else:
                     continue
                 break
             break
         else:
             return urls
 
+    def parse(self, src):
+        """parse a cell and add information to the current execution."""
+        get_ipython().current_execution.md_env = env = dict()
+        tokens = super().parse(src, env)
+        refs, dups = env.get("references"), env.get("duplicates_refs")
+        if refs:
+            self.env.setdefault("references", refs).update(refs)
+        if dups:
+            self.env.setdefault("duplicates_refs", [])
+            self.extend(dups)
+        return tokens
+
+
+def _add_tangle_trait(shell):
+    if not shell.has_trait("tangle"):
+        from traitlets import Instance
 
-def load_ipython_extension(shell):
-    from traitlets import Instance
+        shell.add_traits(tangle=Instance(IPython, ()))
+    from . import current
 
-    def tangle(line, cell):
-        print(shell.tangle.render(cell))
+    current.load_ipython_extension(shell)
 
-    def parse(line, cell):
-        print(shell.tangle.parse(cell))
 
-    shell.add_traits(tangle=Instance(IPython, ()))
+def load_ipython_extension(shell):
+
+    _add_tangle_trait(shell)
     shell.input_transformer_manager.cleanup_transforms.insert(0, pidgy_render_lines)
-    shell.register_magic_function(tangle, "cell")
-    shell.register_magic_function(parse, "cell")
 
 
 def unload_ipython_extension(shell):
+    from . import current
+
     try:
         shell.input_transformer_manager.cleanup_transforms.remove(pidgy_render_lines)
     except ValueError:
         pass
```

### Comparing `pidgy-2023.1.7.post1/src/pidgy/weave.py` & `pidgy-2023.4.20/src/pidgy/weave.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from collections import defaultdict
-from dataclasses import dataclass, field
-from io import StringIO
 from re import compile
-from typing import ChainMap
-from asyncio import ensure_future, gather
+from asyncio import ensure_future
 
-from jinja2 import Environment, Template
 from jinja2.meta import find_undeclared_variables
 from markdown_it import MarkdownIt
 from traitlets import Bool, Dict, Instance, Type, HasTraits, observe, Enum
 
 from .displays import IPythonMarkdown, TemplateDisplay, is_widget
 from .environment import IPythonTemplate
 from . import get_ipython
 
 CELL_MAGIC = compile("^\s*%{2}\S")
 NO_SHOW = compile(r"^\s*\r?\n")
 
 URL = compile("^(http[s]|file)://")
+REFS = compile("\!?(\[.*\])?(\[(?P<a>[^\[]+)\])")
 
 
 class Weave(HasTraits):
+    enabled = Bool(True).tag(config=True)
     displays = Dict()
     shell = Instance("IPython.InteractiveShell", ())
     prior = Dict()  # prior value to compare against when reacting to updates
     template_type = Enum(["markdown", "html", "widget"]).tag(config=True)
     template_cls = Type(IPythonMarkdown, TemplateDisplay)
     markdown_renderer = Instance(MarkdownIt, args=())
     reactive = Bool(True).tag(config=True)
@@ -51,24 +49,65 @@
             template=template,
             vars=self.get_template_vars(body),
             markdown_renderer=self.markdown_renderer,
             use_async=self.use_async,
         )
 
     def filter_meta_tokens(self, body):
-        if self.shell.pidgy.current_execution:
-            for token in self.shell.pidgy.current_execution.tokens:
+        if self.shell.has_trait("current_execution") and self.shell.current_execution.tokens:
+            for token in self.shell.current_execution.tokens:
                 if token.type in {"front_matter", "shebang"}:
                     continue
                 break
             return "".join(body.splitlines(1)[token.map[0] :])
         return body
 
+    def _append_references(self, body):
+        # we can't reuse markdown references across cells without
+        # intervention. this function builds a body of references
+        # that might be undefined in the markdown block, but
+        # defined in a prior cell.
+
+        from markdown_it.common.utils import normalizeReference
+
+        defs = ""
+        for t in self.shell.current_execution.tokens:
+            if t.type == "definition":
+                defs += f"* [{t.meta['label']}]\n"
+                continue
+            break
+        else:
+            return "\n" * 3 + defs
+
+        extras = {}
+
+        all = self.shell.tangle.env.get("references", {})
+        this = self.shell.current_execution.md_env.get("references", {})
+        for m in REFS.finditer(body):
+            r = normalizeReference(m.group("a"))
+            if r in extras:
+                continue
+            if r in this:
+                continue
+            if r in all:
+                ref = all[r]
+                extra = f"[{r}]: " + ref["href"]
+                if ref.get("title"):
+                    extra += f' "{ref["title"]}"'
+                extra += "\n"
+                extras[r] = extra
+
+        if extras:
+            return "\n" * 3 + "\n".join(extras.values())
+        return ""
+
     def weave_cell(self, body):
         body = self.filter_meta_tokens(body)
+        if self.shell.tangle.env.get("references"):
+            body += self._append_references(body)
         template = self.shell.environment.from_string(body, None, IPythonTemplate)
         vars = find_undeclared_variables(self.shell.environment.parse(body))
         return self.template_cls(
             body=body, template=template, vars=vars, markdown_renderer=self.markdown_renderer
         )
 
     def get_value(self, key, raw=True):
@@ -109,78 +148,118 @@
 
                 for display in displays:
                     value.observe(display.observe, "value")
 
         for old in olds:
             old.close()
 
+    def weave(self, body):
+        id = self.get_id()
+        self.displays[id] = self.weave_cell(body)
+        return self.displays[id]
+
     def post_run_cell(self, result):
         from IPython.display import display, Markdown
 
+        if not self.enabled:
+            return
+
         id = self.get_id()
         if result.error_in_exec or result.error_before_exec:
             pass  # don't do anything when there are errors
-        elif NO_SHOW.match(result.info.raw_cell):
-            display(Markdown(f"<div hidden>\n\n{result.info.raw_cell}\n\n</div>"))
         elif CELL_MAGIC.match(result.info.raw_cell):
             pass
+        elif NO_SHOW.match(result.info.raw_cell):
+            display(Markdown(f"<div hidden>\n\n{result.info.raw_cell}\n\n</div>"))
         else:
-            self.displays[id] = self.weave_cell(result.info.raw_cell)
-            display(self.displays[id])
-            return
+            return display(self.weave(result.info.raw_cell))
 
         self.displays.pop(id, None)
 
-    def pre_execute(self):
-        metadata = self.shell.kernel.get_parent().get("metadata", {})
+    def del_displays(self, metadata):
         for id in metadata.get("deletedCells", []):
+            # clear and deleted displays
             if id in self.displays:
                 del self.displays[id]
 
+    def pre_execute(self):
+        if not self.enabled:
+            return
+
+        metadata = self.shell.kernel.get_parent().get("metadata", {})
+        self.del_displays(metadata)
+
         vars = set()
         for id, disp in self.displays.items():
             if disp.vars:
                 vars.update(disp.vars)
+        # collect the state of any reactive or tracked variables before execution
         self.prior.update(zip(vars, map(self.get_value, vars)))
 
-    def post_execute(self):
-        if self.reactive:
+    def post_execute(self, force=False):
+        if force or (self.enabled and self.reactive):
             changed = set()
 
             for k, v in self.prior.items():
                 y = self.get_value(k)
                 if y is not v:
                     changed.add(k)
 
-            for disp in self.displays.values():
-                if changed.intersection(disp.vars):
-                    ensure_future(disp.aupdate())
-
             if self.reactive:
-                self.link_widgets()
+                for disp in self.displays.values():
+                    if changed.intersection(disp.vars):
+                        ensure_future(disp.aupdate())
 
-    def update_displays(self):
-        self.post_execute()
+            self.link_widgets()
 
+    def update(self):
+        self.post_execute(True)
 
-def load_ipython_extension(shell):
-    from .environment import load_ipython_extension
 
-    load_ipython_extension(shell)
+def _add_weave_trait(shell):
+    from . import environment
+
+    environment.load_ipython_extension(shell)
+
     if not shell.has_trait("weave"):
         shell.add_traits(
             weave=Instance(
                 Weave, kw=dict(shell=shell, markdown_renderer=shell.tangle.parser), allow_none=True
-            )
+            ).tag(config=True)
         )
+
+
+def _add_interactivity(shell):
     shell.events.register("pre_execute", shell.weave.pre_execute)
-    shell.events.register("post_run_cell", shell.weave.post_run_cell)
     shell.events.register("post_execute", shell.weave.post_execute)
 
 
+def _rm_interactivity(shell):
+    for e in ["pre_execute", "post_run_cell", "post_execute"]:
+        try:
+            shell.events.unregister(e, getattr(shell.weave, e))
+        except ValueError:
+            pass
+
+
+def load_ipython_extension(shell):
+    _add_weave_trait(shell)
+    _add_interactivity(shell)
+    shell.events.register("post_run_cell", shell.weave.post_run_cell)
+
+    if is_voila():
+        from .displays import IPyWidgetsHtml
+
+        # when voila runs a pidgy application we use the ipywidgets template
+        shell.weave.template_cls = IPyWidgetsHtml
+
+
 def unload_ipython_extension(shell):
     if shell.has_trait("weave"):
-        for e in ["pre_execute", "post_run_cell", "post_execute"]:
-            try:
-                shell.events.unregister(e, getattr(shell.weave, e))
-            except ValueError:
-                pass
+        _rm_interactivity(shell)
+
+
+def is_voila():
+    """determine if voila is running from the environment variables."""
+    from os import environ
+
+    return any(x for x in environ if "voila" in x.lower())
```

### Comparing `pidgy-2023.1.7.post1/.gitignore` & `pidgy-2023.4.20/.gitignore`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/LICENSE` & `pidgy-2023.4.20/LICENSE`

 * *Files identical despite different names*

### Comparing `pidgy-2023.1.7.post1/pyproject.toml` & `pidgy-2023.4.20/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -12,23 +12,45 @@
   "Development Status :: 4 - Beta",
   "Natural Language :: English",
   "Framework :: IPython",
   "Framework :: Jupyter",
   "Programming Language :: Python",
   "License :: OSI Approved :: BSD License",
 ]
-dependencies = ["midgy", "jinja2"]
+dependencies = ["midgy", "jinja2", "IPython", "importnb"]
 dynamic = ["version"] # uses hatch-vcs
 
 [project.optional-dependencies]
-interactive = ["IPython"]
-docs = ["mkdocs-material", "mkdocs-jupyter", "ruamel.yaml", "mkdocs-macros-plugin", "IPython"]
+docs = ["mkdocs-material", "ruamel.yaml", "nbconvert", "mkdocstrings[python]"]
+lite = [
+  "doit",
+  "jupyterlite",
+  "jupyterlab-webrtc-docprovider",
+  "jupyterlab-deck",
+  "jupyter-videochat",
+  "jupyterlab-fonts",
+  "jupyterlab_execute_time",
+  "jupyterlab-recents",
+  "jupyterlab-markup",
+  "matplotlib",
+  "ipympl",
+  "cairosvg",
+  "pillow",
+  "pandas",
+  "retrolab",
+  "pyyaml",
+  "depfinder",
+  "requests_cache",
+  "ipywidgets",
+  "hatch",
+  "pkginfo"
+]
 
 [project.entry-points."mkdocs.plugins"]
-pidgy = "pidgy.ext.mkdocs:PidgyPlugin"
+pidgy = "pidgy.ext.mkdocs:Notebooks"
 
 [project.scripts]
 pidgy = "pidgy.__main__:main"
 
 [project.urls]
 Documentation = "https://github.com/deathbeds/pidgy#readme"
 Issues = "https://github.com/deathbeds/pidgy/issues"
@@ -47,46 +69,54 @@
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/pidgy/_version.py"
 
 # test matrix
 [tool.hatch.envs.test]
+description = "pidgy tests"
 dependencies = ["pytest", "pytest-cov", "nbval", "pandas", "ipywidgets", "matplotlib"]
 
 [tool.hatch.envs.test.scripts]
 cov = "pytest"
 
 [tool.pytest.ini_options]
-addopts = "-pno:warnings -p no:importnb --ignore lite --cov pidgy --cov-report term --cov-report html --current-env --nbval --sanitize-with sanitize.cfg "
+addopts = "-pno:warnings -p no:importnb --ignore lite --cov pidgy --cov-report term --cov-report html --nbval-current-env --nbval --nbval-sanitize-with sanitize.cfg"
 
 [tool.coverage.report]
 omit = ["docs/*"]
 
 [tool.coverage.html]
 directory = "docs/coverage"
 
-
 # documentation
 [tool.hatch.envs.docs]
 features = ["docs"]
 
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build"
 serve = "mkdocs serve"
 
+[tool.hatch.envs.format.scripts]
+code = """
+isort .
+black .
+"""
+
+[tool.hatch.envs.lite]
+description = "build jupyterlite"
+features = ["lite"]
+python = "3.10"
+
+[tool.hatch.envs.lite.scripts]
+build = """doit lite"""
+
 # formatting cause linting sucks
 [tool.isort]
 profile = "black"
 
 [tool.black]
 line_length = 100
 
 [tool.hatch.envs.format]
 skip-install = true
-dependencies = ["black", "isort"]
-
-[tool.hatch.envs.format.scripts]
-code = """
-isort .
-black .
-"""
+dependencies = ["black", "isort"]
```

