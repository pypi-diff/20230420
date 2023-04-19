# Comparing `tmp/shiny_mdc-1.4.0.tar.gz` & `tmp/shiny_mdc-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiny_mdc-1.4.0.tar", max compression
+gzip compressed data, was "shiny_mdc-1.4.1.tar", max compression
```

## Comparing `shiny_mdc-1.4.0.tar` & `shiny_mdc-1.4.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     3330 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/LICENSE
--rw-r--r--   0        0        0       78 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/README.md
--rw-r--r--   0        0        0     2297 2023-04-19 06:08:04.539123 shiny_mdc-1.4.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/__init__.py
--rw-r--r--   0        0        0     1061 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/_latexmk.py
--rw-r--r--   0        0        0     1867 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/_liquid.py
--rw-r--r--   0        0        0     4643 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/_pandoc.py
--rw-r--r--   0        0        0     4936 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/_templates.py
--rw-r--r--   0        0        0       64 2023-04-19 06:08:04.539123 shiny_mdc-1.4.0/shinymdc/_version.py
--rw-r--r--   0        0        0      337 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/dynamic/addappendices.tex
--rw-r--r--   0        0        0      853 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/dynamic/authsetup.tex
--rw-r--r--   0        0        0      290 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/dynamic/authsetupshort.tex
--rw-r--r--   0        0        0      572 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/dynamic/dblfloatsetup.tex
--rw-r--r--   0        0        0      482 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/static/bibnonatsetup.tex
--rw-r--r--   0        0        0     2602 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/static/bibsupersetup.tex
--rw-r--r--   0        0        0     3359 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/static/floatsetup.tex
--rw-r--r--   0        0        0    19901 2023-04-19 06:07:37.177622 shiny_mdc-1.4.0/shinymdc/resources/static/iccv/bibstyle.bst
--rw-r--r--   0        0        0     9433 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/iccv/esopic.sty
--rw-r--r--   0        0        0     3869 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/iccv/everyshi.sty
--rw-r--r--   0        0        0     8276 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/iccv/iccv.sty
--rw-r--r--   0        0        0    26973 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/iclr/bibstyle.bst
--rw-r--r--   0        0        0     9153 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/iclr/iclr.sty
--rw-r--r--   0        0        0    12284 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/iclr/mathcommands.tex
--rw-r--r--   0        0        0    27146 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/icml/bibstyle.bst
--rw-r--r--   0        0        0    27887 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/icml/icml.sty
--rw-r--r--   0        0        0      735 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/mathsetup.tex
--rw-r--r--   0        0        0      848 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/miscsetup.tex
--rw-r--r--   0        0        0    11306 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/neurips/neurips.sty
--rw-r--r--   0        0        0      406 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/resources/static/reqsetup.tex
--rw-r--r--   0        0        0    19149 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/shinymdc.py
--rw-r--r--   0        0        0      935 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/basic.tex
--rw-r--r--   0        0        0     1302 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/iccv.tex
--rw-r--r--   0        0        0     1397 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/iclr.tex
--rw-r--r--   0        0        0     2144 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/icml.tex
--rw-r--r--   0        0        0      890 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/neurips.tex
--rw-r--r--   0        0        0     2057 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/spacious.tex
--rw-r--r--   0        0        0      469 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/standalone.tex
--rw-r--r--   0        0        0     2286 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/shinymdc/templates/stylish.tex
--rw-r--r--   0        0        0    15953 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/test/figures/anscombe.pdf
--rw-r--r--   0        0        0    40892 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/test/figures/densities.pdf
--rw-r--r--   0        0        0    10736 2023-04-19 06:07:37.181622 shiny_mdc-1.4.0/test/figures/diamonds.pdf
--rw-r--r--   0        0        0   197017 2023-04-19 06:07:37.185623 shiny_mdc-1.4.0/test/figures/gaussian2d.pdf
--rw-r--r--   0        0        0    28282 2023-04-19 06:07:37.185623 shiny_mdc-1.4.0/test/figures/lines.png
--rw-r--r--   0        0        0     2972 2023-04-19 06:07:37.185623 shiny_mdc-1.4.0/test/main.md
--rwxr-xr-x   0        0        0      315 2023-04-19 06:07:37.185623 shiny_mdc-1.4.0/test/make.sh
--rw-r--r--   0        0        0     1166 2023-04-19 06:07:37.185623 shiny_mdc-1.4.0/test/references.bib
--rw-r--r--   0        0        0   683424 2023-04-19 06:07:37.185623 shiny_mdc-1.4.0/test/samples/basic.pdf
--rw-r--r--   0        0        0   412896 2023-04-19 06:07:37.189623 shiny_mdc-1.4.0/test/samples/iccv.pdf
--rw-r--r--   0        0        0   406337 2023-04-19 06:07:37.189623 shiny_mdc-1.4.0/test/samples/iclr.pdf
--rw-r--r--   0        0        0   446430 2023-04-19 06:07:37.193623 shiny_mdc-1.4.0/test/samples/icml.pdf
--rw-r--r--   0        0        0   450734 2023-04-19 06:07:37.197623 shiny_mdc-1.4.0/test/samples/neurips.pdf
--rw-r--r--   0        0        0   601766 2023-04-19 06:07:37.197623 shiny_mdc-1.4.0/test/samples/spacious.pdf
--rw-r--r--   0        0        0   553251 2023-04-19 06:07:37.201624 shiny_mdc-1.4.0/test/samples/standalone.pdf
--rw-r--r--   0        0        0   424279 2023-04-19 06:07:37.201624 shiny_mdc-1.4.0/test/samples/stylish.pdf
--rw-r--r--   0        0        0     1535 2023-04-19 06:07:37.205624 shiny_mdc-1.4.0/test/sections/appendix1.md
--rw-r--r--   0        0        0     1625 2023-04-19 06:07:37.205624 shiny_mdc-1.4.0/test/sections/appendix2.md
--rw-r--r--   0        0        0        0 2023-04-19 06:07:37.205624 shiny_mdc-1.4.0/test/sections/empty.md
--rw-r--r--   0        0        0     2100 2023-04-19 06:07:37.205624 shiny_mdc-1.4.0/test/sections/main1.md
--rw-r--r--   0        0        0     1353 2023-04-19 06:07:37.205624 shiny_mdc-1.4.0/test/sections/main2.md
--rw-r--r--   0        0        0      992 2023-04-19 06:07:37.205624 shiny_mdc-1.4.0/test/utils/commands.md
--rw-r--r--   0        0        0       41 2023-04-19 06:07:37.205624 shiny_mdc-1.4.0/test/utils/ext.md
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 shiny_mdc-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3595 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/LICENSE
+-rw-r--r--   0        0        0       78 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/README.md
+-rw-r--r--   0        0        0     2297 2023-04-19 23:33:53.086398 shiny_mdc-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/__init__.py
+-rw-r--r--   0        0        0     1061 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/_latexmk.py
+-rw-r--r--   0        0        0     1867 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/_liquid.py
+-rw-r--r--   0        0        0     4643 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/_pandoc.py
+-rw-r--r--   0        0        0     4936 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/_templates.py
+-rw-r--r--   0        0        0       64 2023-04-19 23:33:53.090397 shiny_mdc-1.4.1/shinymdc/_version.py
+-rw-r--r--   0        0        0      337 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/dynamic/addappendices.tex
+-rw-r--r--   0        0        0      853 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/dynamic/authsetup.tex
+-rw-r--r--   0        0        0      290 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/dynamic/authsetupshort.tex
+-rw-r--r--   0        0        0      572 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/dynamic/dblfloatsetup.tex
+-rw-r--r--   0        0        0      482 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/static/bibnonatsetup.tex
+-rw-r--r--   0        0        0     2602 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/static/bibsupersetup.tex
+-rw-r--r--   0        0        0     3359 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/static/floatsetup.tex
+-rw-r--r--   0        0        0    19901 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/static/iccv/bibstyle.bst
+-rw-r--r--   0        0        0     9433 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/static/iccv/esopic.sty
+-rw-r--r--   0        0        0     3869 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/static/iccv/everyshi.sty
+-rw-r--r--   0        0        0     8276 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/static/iccv/iccv.sty
+-rw-r--r--   0        0        0    26973 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/iclr/bibstyle.bst
+-rw-r--r--   0        0        0     9153 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/iclr/iclr.sty
+-rw-r--r--   0        0        0    12284 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/iclr/mathcommands.tex
+-rw-r--r--   0        0        0    27146 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/icml/bibstyle.bst
+-rw-r--r--   0        0        0    27887 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/icml/icml.sty
+-rw-r--r--   0        0        0      735 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/mathsetup.tex
+-rw-r--r--   0        0        0      848 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/miscsetup.tex
+-rw-r--r--   0        0        0    11306 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/neurips/neurips.sty
+-rw-r--r--   0        0        0      406 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/reqsetup.tex
+-rw-r--r--   0        0        0    19149 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/shinymdc.py
+-rw-r--r--   0        0        0      930 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/basic.tex
+-rw-r--r--   0        0        0     1302 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/iccv.tex
+-rw-r--r--   0        0        0     1397 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/iclr.tex
+-rw-r--r--   0        0        0     2144 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/icml.tex
+-rw-r--r--   0        0        0      890 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/neurips.tex
+-rw-r--r--   0        0        0     2052 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/spacious.tex
+-rw-r--r--   0        0        0      464 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/standalone.tex
+-rw-r--r--   0        0        0     2281 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/stylish.tex
+-rw-r--r--   0        0        0    15953 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/test/figures/anscombe.pdf
+-rw-r--r--   0        0        0    40892 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/test/figures/densities.pdf
+-rw-r--r--   0        0        0    10736 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/test/figures/diamonds.pdf
+-rw-r--r--   0        0        0   197017 2023-04-19 23:33:29.722182 shiny_mdc-1.4.1/test/figures/gaussian2d.pdf
+-rw-r--r--   0        0        0    28282 2023-04-19 23:33:29.722182 shiny_mdc-1.4.1/test/figures/lines.png
+-rw-r--r--   0        0        0     2972 2023-04-19 23:33:29.722182 shiny_mdc-1.4.1/test/main.md
+-rwxr-xr-x   0        0        0      315 2023-04-19 23:33:29.722182 shiny_mdc-1.4.1/test/make.sh
+-rw-r--r--   0        0        0     1166 2023-04-19 23:33:29.722182 shiny_mdc-1.4.1/test/references.bib
+-rw-r--r--   0        0        0   683424 2023-04-19 23:33:29.726182 shiny_mdc-1.4.1/test/samples/basic.pdf
+-rw-r--r--   0        0        0   412896 2023-04-19 23:33:29.726182 shiny_mdc-1.4.1/test/samples/iccv.pdf
+-rw-r--r--   0        0        0   406337 2023-04-19 23:33:29.730182 shiny_mdc-1.4.1/test/samples/iclr.pdf
+-rw-r--r--   0        0        0   446430 2023-04-19 23:33:29.730182 shiny_mdc-1.4.1/test/samples/icml.pdf
+-rw-r--r--   0        0        0   450734 2023-04-19 23:33:29.734182 shiny_mdc-1.4.1/test/samples/neurips.pdf
+-rw-r--r--   0        0        0   601766 2023-04-19 23:33:29.738182 shiny_mdc-1.4.1/test/samples/spacious.pdf
+-rw-r--r--   0        0        0   553251 2023-04-19 23:33:29.738182 shiny_mdc-1.4.1/test/samples/standalone.pdf
+-rw-r--r--   0        0        0   424279 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/samples/stylish.pdf
+-rw-r--r--   0        0        0     1535 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/sections/appendix1.md
+-rw-r--r--   0        0        0     1625 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/sections/appendix2.md
+-rw-r--r--   0        0        0        0 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/sections/empty.md
+-rw-r--r--   0        0        0     2100 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/sections/main1.md
+-rw-r--r--   0        0        0     1353 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/sections/main2.md
+-rw-r--r--   0        0        0      992 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/utils/commands.md
+-rw-r--r--   0        0        0       41 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/utils/ext.md
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 shiny_mdc-1.4.1/PKG-INFO
```

### Comparing `shiny_mdc-1.4.0/CHANGELOG.md` & `shiny_mdc-1.4.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+### [1.4.1](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.4.0...v1.4.1) (2023-04-19)
+
+
+### Bug Fixes
+
+* fix `hidelinks` argument passed to `hyperref` ([5007034](https://github.com/jayanthkoushik/shiny-mdc/commit/500703429ac92f233caf309f1f6b3f22d88c6ef8))
+
 ## [1.4.0](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.3.1...v1.4.0) (2023-04-19)
 
 
 ### Features
 
 * make small tables in stylish template opt-in ([24cdca5](https://github.com/jayanthkoushik/shiny-mdc/commit/24cdca56f336ee69b178a89420c3fe1560be3c94))
```

### Comparing `shiny_mdc-1.4.0/LICENSE` & `shiny_mdc-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/pyproject.toml` & `shiny_mdc-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shiny-mdc"
-version = "1.4.0"  # managed by `poetry-dynamic-versioning`
+version = "1.4.1"  # managed by `poetry-dynamic-versioning`
 description = "Tool to compile markdown files to tex/pdf using pandoc, latexmk"
 readme = "README.md"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 repository = "https://github.com/jayanthkoushik/shinymdc"
 packages = [
   { include = "shinymdc" }
```

### Comparing `shiny_mdc-1.4.0/shinymdc/_latexmk.py` & `shiny_mdc-1.4.1/shinymdc/_latexmk.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/_liquid.py` & `shiny_mdc-1.4.1/shinymdc/_liquid.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/_pandoc.py` & `shiny_mdc-1.4.1/shinymdc/_pandoc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/_templates.py` & `shiny_mdc-1.4.1/shinymdc/_templates.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/dynamic/authsetup.tex` & `shiny_mdc-1.4.1/shinymdc/resources/dynamic/authsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/dynamic/dblfloatsetup.tex` & `shiny_mdc-1.4.1/shinymdc/resources/dynamic/dblfloatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/static/bibsupersetup.tex` & `shiny_mdc-1.4.1/shinymdc/resources/static/bibsupersetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/static/floatsetup.tex` & `shiny_mdc-1.4.1/shinymdc/resources/static/floatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/static/iccv/bibstyle.bst` & `shiny_mdc-1.4.1/shinymdc/resources/static/iccv/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/static/iccv/esopic.sty` & `shiny_mdc-1.4.1/shinymdc/resources/static/iccv/esopic.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/static/iccv/everyshi.sty` & `shiny_mdc-1.4.1/shinymdc/resources/static/iccv/everyshi.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/static/iccv/iccv.sty` & `shiny_mdc-1.4.1/shinymdc/resources/static/iccv/iccv.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/static/iclr/bibstyle.bst` & `shiny_mdc-1.4.1/shinymdc/resources/static/iclr/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/static/iclr/iclr.sty` & `shiny_mdc-1.4.1/shinymdc/resources/static/iclr/iclr.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/static/iclr/mathcommands.tex` & `shiny_mdc-1.4.1/shinymdc/resources/static/iclr/mathcommands.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/static/icml/bibstyle.bst` & `shiny_mdc-1.4.1/shinymdc/resources/static/icml/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/static/icml/icml.sty` & `shiny_mdc-1.4.1/shinymdc/resources/static/icml/icml.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/static/mathsetup.tex` & `shiny_mdc-1.4.1/shinymdc/resources/static/mathsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/static/miscsetup.tex` & `shiny_mdc-1.4.1/shinymdc/resources/static/miscsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/resources/static/neurips/neurips.sty` & `shiny_mdc-1.4.1/shinymdc/resources/static/neurips/neurips.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/shinymdc.py` & `shiny_mdc-1.4.1/shinymdc/shinymdc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/templates/basic.tex` & `shiny_mdc-1.4.1/shinymdc/templates/basic.tex`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\PassOptionsToPackage{hidelinks=true}{hyperref}
+\PassOptionsToPackage{hidelinks}{hyperref}
 
 \documentclass[%
   letterpaper,%
   $if(lang)$$lang$$else$english$endif$%
 ]{article}
 
 \usepackage[margin=1.5in,footskip=0.75in]{geometry}
```

### Comparing `shiny_mdc-1.4.0/shinymdc/templates/iccv.tex` & `shiny_mdc-1.4.1/shinymdc/templates/iccv.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/templates/iclr.tex` & `shiny_mdc-1.4.1/shinymdc/templates/iclr.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/templates/icml.tex` & `shiny_mdc-1.4.1/shinymdc/templates/icml.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/templates/neurips.tex` & `shiny_mdc-1.4.1/shinymdc/templates/neurips.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/shinymdc/templates/spacious.tex` & `shiny_mdc-1.4.1/shinymdc/templates/spacious.tex`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\PassOptionsToPackage{hidelinks=true}{hyperref}
+\PassOptionsToPackage{hidelinks}{hyperref}
 
 \documentclass[%
   letterpaper,%
   12pt,%
   $if(lang)$$lang$$else$english$endif$%
 ]{article}
```

### Comparing `shiny_mdc-1.4.0/shinymdc/templates/stylish.tex` & `shiny_mdc-1.4.1/shinymdc/templates/stylish.tex`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\PassOptionsToPackage{hidelinks=true}{hyperref}
+\PassOptionsToPackage{hidelinks}{hyperref}
 
 \documentclass[%
   letterpaper,%
   twocolumn,%
   $if(lang)$$lang$$else$english$endif$%
 ]{article}
```

### Comparing `shiny_mdc-1.4.0/test/figures/anscombe.pdf` & `shiny_mdc-1.4.1/test/figures/anscombe.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/test/figures/densities.pdf` & `shiny_mdc-1.4.1/test/figures/densities.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/test/figures/diamonds.pdf` & `shiny_mdc-1.4.1/test/figures/diamonds.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/test/figures/gaussian2d.pdf` & `shiny_mdc-1.4.1/test/figures/gaussian2d.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/test/figures/lines.png` & `shiny_mdc-1.4.1/test/figures/lines.png`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/test/main.md` & `shiny_mdc-1.4.1/test/main.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/test/references.bib` & `shiny_mdc-1.4.1/test/references.bib`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/test/samples/basic.pdf` & `shiny_mdc-1.4.1/test/samples/basic.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 0% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'681982'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'681982'*

 * *DEBUG:pdfminer.psparser:seek: 681982*

 * *DEBUG:pdfminer.psparser:nexttoken: (681982, 463)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=681982, token=463*

 * *DEBUG:pdfminer.psparser:seek: 681982*

 * *DEBUG:pdfminer.psparser:nexttoken: (681982, 463)*

 * *DEBUG:pdfminer.psparser:nexttoken: (681986, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (681988, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (681992, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=681992, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (681995, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (682001, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (682007, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (682014, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=682014, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (682016, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (682018, 464)*

 * *DEBUG:pdfminer.psparser:nexttoken: (682022, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=682014, type='a', objs=[0, 464]*

 * *DEBUG:pdfminer.psparser:nexttoken: (682024, /'Size')*

 * *[ truncated after 25 lines; 19044 ignored ]*

```diff
@@ -10844,17 +10844,17 @@
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>Producer</key>
 <value><string size="13">LuaTeX-1.15.0</string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230419012331-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192906-04&#39;00&#39;</string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230419012331-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192906-04&#39;00&#39;</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.FullBanner</key>
 <value><string size="48">This is LuaHBTeX, Version 1.15.0 &#40;TeX Live 2022&#41;</string></value>
 </dict>
 </object>
 
@@ -10879,16 +10879,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="461" /></value>
 <key>Info</key>
 <value><ref id="462" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">m&#38;H&#181;&#252;&#139;:&#244;h&#207;&#169;W&#182;&#173;&#233;&#12;</string>
-<string size="16">m&#38;H&#181;&#252;&#139;:&#244;h&#207;&#169;W&#182;&#173;&#233;&#12;</string>
+<string size="16">,&#254; &#245;9&#166;&#165;&#162;&#171;&#189;&#216;&#163;&#211;K4%</string>
+<string size="16">,&#254; &#245;9&#166;&#165;&#162;&#171;&#189;&#216;&#163;&#211;K4%</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1179</number></value>
 </dict>
 </props>
@@ -10915,16 +10915,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="461" /></value>
 <key>Info</key>
 <value><ref id="462" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">m&#38;H&#181;&#252;&#139;:&#244;h&#207;&#169;W&#182;&#173;&#233;&#12;</string>
-<string size="16">m&#38;H&#181;&#252;&#139;:&#244;h&#207;&#169;W&#182;&#173;&#233;&#12;</string>
+<string size="16">,&#254; &#245;9&#166;&#165;&#162;&#171;&#189;&#216;&#163;&#211;K4%</string>
+<string size="16">,&#254; &#245;9&#166;&#165;&#162;&#171;&#189;&#216;&#163;&#211;K4%</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1179</number></value>
 </dict>
 </trailer>
```

### Comparing `shiny_mdc-1.4.0/test/samples/iccv.pdf` & `shiny_mdc-1.4.1/test/samples/iccv.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 1% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'411695'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'411695'*

 * *DEBUG:pdfminer.psparser:seek: 411695*

 * *DEBUG:pdfminer.psparser:nexttoken: (411695, 366)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=411695, token=366*

 * *DEBUG:pdfminer.psparser:seek: 411695*

 * *DEBUG:pdfminer.psparser:nexttoken: (411695, 366)*

 * *DEBUG:pdfminer.psparser:nexttoken: (411699, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (411701, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (411705, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=411705, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (411708, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (411714, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (411720, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (411727, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=411727, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (411729, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (411731, 367)*

 * *DEBUG:pdfminer.psparser:nexttoken: (411735, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=411727, type='a', objs=[0, 367]*

 * *DEBUG:pdfminer.psparser:nexttoken: (411737, /'Size')*

 * *[ truncated after 25 lines; 15916 ignored ]*

```diff
@@ -9086,17 +9086,17 @@
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>Producer</key>
 <value><string size="13">LuaTeX-1.15.0</string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230419012338-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192913-04&#39;00&#39;</string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230419012338-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192913-04&#39;00&#39;</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.FullBanner</key>
 <value><string size="48">This is LuaHBTeX, Version 1.15.0 &#40;TeX Live 2022&#41;</string></value>
 </dict>
 </object>
 
@@ -9121,16 +9121,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="364" /></value>
 <key>Info</key>
 <value><ref id="365" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#18;&#18;&#3;&#160;v&#2;v&#183;&#180;&#27;H&#21;1&#25;&#144;&#130;</string>
-<string size="16">&#18;&#18;&#3;&#160;v&#2;v&#183;&#180;&#27;H&#21;1&#25;&#144;&#130;</string>
+<string size="16">&#223;K&#214;&#176;&#251;&#190;]C&#167;&#169;hY&#240;&#30;F&#210;</string>
+<string size="16">&#223;K&#214;&#176;&#251;&#190;]C&#167;&#169;hY&#240;&#30;F&#210;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>938</number></value>
 </dict>
 </props>
@@ -9157,16 +9157,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="364" /></value>
 <key>Info</key>
 <value><ref id="365" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#18;&#18;&#3;&#160;v&#2;v&#183;&#180;&#27;H&#21;1&#25;&#144;&#130;</string>
-<string size="16">&#18;&#18;&#3;&#160;v&#2;v&#183;&#180;&#27;H&#21;1&#25;&#144;&#130;</string>
+<string size="16">&#223;K&#214;&#176;&#251;&#190;]C&#167;&#169;hY&#240;&#30;F&#210;</string>
+<string size="16">&#223;K&#214;&#176;&#251;&#190;]C&#167;&#169;hY&#240;&#30;F&#210;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>938</number></value>
 </dict>
 </trailer>
```

### Comparing `shiny_mdc-1.4.0/test/samples/iclr.pdf` & `shiny_mdc-1.4.1/test/samples/iclr.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 1% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'404892'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'404892'*

 * *DEBUG:pdfminer.psparser:seek: 404892*

 * *DEBUG:pdfminer.psparser:nexttoken: (404892, 465)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=404892, token=465*

 * *DEBUG:pdfminer.psparser:seek: 404892*

 * *DEBUG:pdfminer.psparser:nexttoken: (404892, 465)*

 * *DEBUG:pdfminer.psparser:nexttoken: (404896, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (404898, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (404902, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=404902, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (404905, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (404911, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (404917, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (404924, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=404924, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (404926, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (404928, 466)*

 * *DEBUG:pdfminer.psparser:nexttoken: (404932, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=404924, type='a', objs=[0, 466]*

 * *DEBUG:pdfminer.psparser:nexttoken: (404934, /'Size')*

 * *[ truncated after 25 lines; 19154 ignored ]*

```diff
@@ -10653,17 +10653,17 @@
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>Producer</key>
 <value><string size="13">LuaTeX-1.15.0</string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230419012345-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192921-04&#39;00&#39;</string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230419012345-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192921-04&#39;00&#39;</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.FullBanner</key>
 <value><string size="48">This is LuaHBTeX, Version 1.15.0 &#40;TeX Live 2022&#41;</string></value>
 </dict>
 </object>
 
@@ -10688,16 +10688,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="463" /></value>
 <key>Info</key>
 <value><ref id="464" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#166;ee&#232;&#190;&#137;&#230;q&#198;&#146;Y&#197;&#180;&#244;&#175;/</string>
-<string size="16">&#166;ee&#232;&#190;&#137;&#230;q&#198;&#146;Y&#197;&#180;&#244;&#175;/</string>
+<string size="16">&#184;&#236;&#147;/&#184;&#19;&#127;&#133;&#148;,&#29;H}&#221;&#203;&#191;</string>
+<string size="16">&#184;&#236;&#147;/&#184;&#19;&#127;&#133;&#148;,&#29;H}&#221;&#203;&#191;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1182</number></value>
 </dict>
 </props>
@@ -10724,16 +10724,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="463" /></value>
 <key>Info</key>
 <value><ref id="464" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#166;ee&#232;&#190;&#137;&#230;q&#198;&#146;Y&#197;&#180;&#244;&#175;/</string>
-<string size="16">&#166;ee&#232;&#190;&#137;&#230;q&#198;&#146;Y&#197;&#180;&#244;&#175;/</string>
+<string size="16">&#184;&#236;&#147;/&#184;&#19;&#127;&#133;&#148;,&#29;H}&#221;&#203;&#191;</string>
+<string size="16">&#184;&#236;&#147;/&#184;&#19;&#127;&#133;&#148;,&#29;H}&#221;&#203;&#191;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1182</number></value>
 </dict>
 </trailer>
```

### Comparing `shiny_mdc-1.4.0/test/samples/icml.pdf` & `shiny_mdc-1.4.1/test/samples/icml.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 0% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'445249'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'445249'*

 * *DEBUG:pdfminer.psparser:seek: 445249*

 * *DEBUG:pdfminer.psparser:nexttoken: (445249, 370)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=445249, token=370*

 * *DEBUG:pdfminer.psparser:seek: 445249*

 * *DEBUG:pdfminer.psparser:nexttoken: (445249, 370)*

 * *DEBUG:pdfminer.psparser:nexttoken: (445253, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (445255, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (445259, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=445259, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (445262, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (445268, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (445274, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (445281, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=445281, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (445283, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (445285, 371)*

 * *DEBUG:pdfminer.psparser:nexttoken: (445289, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=445281, type='a', objs=[0, 371]*

 * *DEBUG:pdfminer.psparser:nexttoken: (445291, /'Size')*

 * *[ truncated after 25 lines; 16669 ignored ]*

```diff
@@ -9799,17 +9799,17 @@
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>Producer</key>
 <value><string size="13">LuaTeX-1.15.0</string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230419012350-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192925-04&#39;00&#39;</string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230419012350-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192925-04&#39;00&#39;</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.FullBanner</key>
 <value><string size="48">This is LuaHBTeX, Version 1.15.0 &#40;TeX Live 2022&#41;</string></value>
 </dict>
 </object>
 
@@ -9834,16 +9834,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="368" /></value>
 <key>Info</key>
 <value><ref id="369" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">W#&#172;K&#198;&#193;&#205;&#249;$+&#163;&#255;Z&#245;#&#164;</string>
-<string size="16">W#&#172;K&#198;&#193;&#205;&#249;$+&#163;&#255;Z&#245;#&#164;</string>
+<string size="16">&#19;&#138;&#158;&#213;&#133;&#182;I&#237;R&#214;I&#162;&#1;&#5;&#185;&#41;</string>
+<string size="16">&#19;&#138;&#158;&#213;&#133;&#182;I&#237;R&#214;I&#162;&#1;&#5;&#185;&#41;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>918</number></value>
 </dict>
 </props>
@@ -9870,16 +9870,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="368" /></value>
 <key>Info</key>
 <value><ref id="369" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">W#&#172;K&#198;&#193;&#205;&#249;$+&#163;&#255;Z&#245;#&#164;</string>
-<string size="16">W#&#172;K&#198;&#193;&#205;&#249;$+&#163;&#255;Z&#245;#&#164;</string>
+<string size="16">&#19;&#138;&#158;&#213;&#133;&#182;I&#237;R&#214;I&#162;&#1;&#5;&#185;&#41;</string>
+<string size="16">&#19;&#138;&#158;&#213;&#133;&#182;I&#237;R&#214;I&#162;&#1;&#5;&#185;&#41;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>918</number></value>
 </dict>
 </trailer>
```

### Comparing `shiny_mdc-1.4.0/test/samples/neurips.pdf` & `shiny_mdc-1.4.1/test/samples/neurips.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 1% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'449390'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'449390'*

 * *DEBUG:pdfminer.psparser:seek: 449390*

 * *DEBUG:pdfminer.psparser:nexttoken: (449390, 425)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=449390, token=425*

 * *DEBUG:pdfminer.psparser:seek: 449390*

 * *DEBUG:pdfminer.psparser:nexttoken: (449390, 425)*

 * *DEBUG:pdfminer.psparser:nexttoken: (449394, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (449396, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (449400, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=449400, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (449403, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (449409, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (449415, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (449422, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=449422, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (449424, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (449426, 426)*

 * *DEBUG:pdfminer.psparser:nexttoken: (449430, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=449422, type='a', objs=[0, 426]*

 * *DEBUG:pdfminer.psparser:nexttoken: (449432, /'Size')*

 * *[ truncated after 25 lines; 17134 ignored ]*

```diff
@@ -9585,17 +9585,17 @@
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>Producer</key>
 <value><string size="13">LuaTeX-1.15.0</string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230419012355-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192929-04&#39;00&#39;</string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230419012355-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192929-04&#39;00&#39;</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.FullBanner</key>
 <value><string size="48">This is LuaHBTeX, Version 1.15.0 &#40;TeX Live 2022&#41;</string></value>
 </dict>
 </object>
 
@@ -9620,16 +9620,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="423" /></value>
 <key>Info</key>
 <value><ref id="424" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#16;&#249;&#145;m&#225;&#230;@U&#239;[&#212;&#232;&#245;z&#143;&#30;</string>
-<string size="16">&#16;&#249;&#145;m&#225;&#230;@U&#239;[&#212;&#232;&#245;z&#143;&#30;</string>
+<string size="16">&#232;i8M&#7;&#153;&#243;&#167;&#191;&#164;h .&#178;&#213;&#218;</string>
+<string size="16">&#232;i8M&#7;&#153;&#243;&#167;&#191;&#164;h .&#178;&#213;&#218;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1081</number></value>
 </dict>
 </props>
@@ -9656,16 +9656,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="423" /></value>
 <key>Info</key>
 <value><ref id="424" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#16;&#249;&#145;m&#225;&#230;@U&#239;[&#212;&#232;&#245;z&#143;&#30;</string>
-<string size="16">&#16;&#249;&#145;m&#225;&#230;@U&#239;[&#212;&#232;&#245;z&#143;&#30;</string>
+<string size="16">&#232;i8M&#7;&#153;&#243;&#167;&#191;&#164;h .&#178;&#213;&#218;</string>
+<string size="16">&#232;i8M&#7;&#153;&#243;&#167;&#191;&#164;h .&#178;&#213;&#218;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1081</number></value>
 </dict>
 </trailer>
```

### Comparing `shiny_mdc-1.4.0/test/samples/spacious.pdf` & `shiny_mdc-1.4.1/test/samples/spacious.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 0% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'600317'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'600317'*

 * *DEBUG:pdfminer.psparser:seek: 600317*

 * *DEBUG:pdfminer.psparser:nexttoken: (600317, 470)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=600317, token=470*

 * *DEBUG:pdfminer.psparser:seek: 600317*

 * *DEBUG:pdfminer.psparser:nexttoken: (600317, 470)*

 * *DEBUG:pdfminer.psparser:nexttoken: (600321, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (600323, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (600327, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=600327, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (600330, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (600336, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (600342, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (600349, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=600349, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (600351, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (600353, 471)*

 * *DEBUG:pdfminer.psparser:nexttoken: (600357, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=600349, type='a', objs=[0, 471]*

 * *DEBUG:pdfminer.psparser:nexttoken: (600359, /'Size')*

 * *[ truncated after 25 lines; 19171 ignored ]*

```diff
@@ -10772,17 +10772,17 @@
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>Producer</key>
 <value><string size="13">LuaTeX-1.15.0</string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230419012358-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192933-04&#39;00&#39;</string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230419012358-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192933-04&#39;00&#39;</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.FullBanner</key>
 <value><string size="48">This is LuaHBTeX, Version 1.15.0 &#40;TeX Live 2022&#41;</string></value>
 </dict>
 </object>
 
@@ -10807,16 +10807,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="468" /></value>
 <key>Info</key>
 <value><ref id="469" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#34;&#210;&#19;&#237;k&#216;&#152;&#203;&#41;`Q&#137;&#31;[&#195;&#182;</string>
-<string size="16">&#34;&#210;&#19;&#237;k&#216;&#152;&#203;&#41;`Q&#137;&#31;[&#195;&#182;</string>
+<string size="16">&#39;KL&#243;&#27;&#5;&#25;&#210;&#135;L&#151;&#228;u&#7;&#138;!</string>
+<string size="16">&#39;KL&#243;&#27;&#5;&#25;&#210;&#135;L&#151;&#228;u&#7;&#138;!</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1186</number></value>
 </dict>
 </props>
@@ -10843,16 +10843,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="468" /></value>
 <key>Info</key>
 <value><ref id="469" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#34;&#210;&#19;&#237;k&#216;&#152;&#203;&#41;`Q&#137;&#31;[&#195;&#182;</string>
-<string size="16">&#34;&#210;&#19;&#237;k&#216;&#152;&#203;&#41;`Q&#137;&#31;[&#195;&#182;</string>
+<string size="16">&#39;KL&#243;&#27;&#5;&#25;&#210;&#135;L&#151;&#228;u&#7;&#138;!</string>
+<string size="16">&#39;KL&#243;&#27;&#5;&#25;&#210;&#135;L&#151;&#228;u&#7;&#138;!</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1186</number></value>
 </dict>
 </trailer>
```

### Comparing `shiny_mdc-1.4.0/test/samples/standalone.pdf` & `shiny_mdc-1.4.1/test/samples/standalone.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 0% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'552184'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'552184'*

 * *DEBUG:pdfminer.psparser:seek: 552184*

 * *DEBUG:pdfminer.psparser:nexttoken: (552184, 313)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=552184, token=313*

 * *DEBUG:pdfminer.psparser:seek: 552184*

 * *DEBUG:pdfminer.psparser:nexttoken: (552184, 313)*

 * *DEBUG:pdfminer.psparser:nexttoken: (552188, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (552190, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (552194, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=552194, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (552197, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (552203, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (552209, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (552216, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=552216, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (552218, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (552220, 314)*

 * *DEBUG:pdfminer.psparser:nexttoken: (552224, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=552216, type='a', objs=[0, 314]*

 * *DEBUG:pdfminer.psparser:nexttoken: (552226, /'Size')*

 * *[ truncated after 25 lines; 12970 ignored ]*

```diff
@@ -7601,17 +7601,17 @@
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>Producer</key>
 <value><string size="13">LuaTeX-1.15.0</string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230419012403-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192937-04&#39;00&#39;</string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230419012403-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192937-04&#39;00&#39;</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.FullBanner</key>
 <value><string size="48">This is LuaHBTeX, Version 1.15.0 &#40;TeX Live 2022&#41;</string></value>
 </dict>
 </object>
 
@@ -7636,16 +7636,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="311" /></value>
 <key>Info</key>
 <value><ref id="312" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#156;&#224;_&#62;&#252;Ha&#237;&#208;&#138;&#239;&#13;&#13;Q&#134;&#231;</string>
-<string size="16">&#156;&#224;_&#62;&#252;Ha&#237;&#208;&#138;&#239;&#13;&#13;Q&#134;&#231;</string>
+<string size="16">N&#203;&#213;N&#2;&#180;&#195;&#243;&#62;!&#41;,&#167;eJ&#10;</string>
+<string size="16">N&#203;&#213;N&#2;&#180;&#195;&#243;&#62;!&#41;,&#167;eJ&#10;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>804</number></value>
 </dict>
 </props>
@@ -7672,16 +7672,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="311" /></value>
 <key>Info</key>
 <value><ref id="312" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#156;&#224;_&#62;&#252;Ha&#237;&#208;&#138;&#239;&#13;&#13;Q&#134;&#231;</string>
-<string size="16">&#156;&#224;_&#62;&#252;Ha&#237;&#208;&#138;&#239;&#13;&#13;Q&#134;&#231;</string>
+<string size="16">N&#203;&#213;N&#2;&#180;&#195;&#243;&#62;!&#41;,&#167;eJ&#10;</string>
+<string size="16">N&#203;&#213;N&#2;&#180;&#195;&#243;&#62;!&#41;,&#167;eJ&#10;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>804</number></value>
 </dict>
 </trailer>
```

### Comparing `shiny_mdc-1.4.0/test/samples/stylish.pdf` & `shiny_mdc-1.4.1/test/samples/stylish.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 0% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'422756'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'422756'*

 * *DEBUG:pdfminer.psparser:seek: 422756*

 * *DEBUG:pdfminer.psparser:nexttoken: (422756, 487)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=422756, token=487*

 * *DEBUG:pdfminer.psparser:seek: 422756*

 * *DEBUG:pdfminer.psparser:nexttoken: (422756, 487)*

 * *DEBUG:pdfminer.psparser:nexttoken: (422760, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (422762, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (422766, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=422766, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (422769, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (422775, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (422781, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (422788, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=422788, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (422790, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (422792, 488)*

 * *DEBUG:pdfminer.psparser:nexttoken: (422796, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=422788, type='a', objs=[0, 488]*

 * *DEBUG:pdfminer.psparser:nexttoken: (422798, /'Size')*

 * *[ truncated after 25 lines; 19950 ignored ]*

```diff
@@ -11039,17 +11039,17 @@
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>Producer</key>
 <value><string size="13">LuaTeX-1.15.0</string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230419020515-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192942-04&#39;00&#39;</string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230419020515-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230419192942-04&#39;00&#39;</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.FullBanner</key>
 <value><string size="48">This is LuaHBTeX, Version 1.15.0 &#40;TeX Live 2022&#41;</string></value>
 </dict>
 </object>
 
@@ -11074,16 +11074,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="485" /></value>
 <key>Info</key>
 <value><ref id="486" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#193;+&#0;&#236;&#221;&#155;i&#220;&#127;&#150;&#171;&#139;&#230;&#129;&#170;F</string>
-<string size="16">&#193;+&#0;&#236;&#221;&#155;i&#220;&#127;&#150;&#171;&#139;&#230;&#129;&#170;F</string>
+<string size="16">&#4;a&#62;D&#197;&#227;`T@$&#193;&#212;&#62;z&#148;{</string>
+<string size="16">&#4;a&#62;D&#197;&#227;`T@$&#193;&#212;&#62;z&#148;{</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1260</number></value>
 </dict>
 </props>
@@ -11110,16 +11110,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="485" /></value>
 <key>Info</key>
 <value><ref id="486" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#193;+&#0;&#236;&#221;&#155;i&#220;&#127;&#150;&#171;&#139;&#230;&#129;&#170;F</string>
-<string size="16">&#193;+&#0;&#236;&#221;&#155;i&#220;&#127;&#150;&#171;&#139;&#230;&#129;&#170;F</string>
+<string size="16">&#4;a&#62;D&#197;&#227;`T@$&#193;&#212;&#62;z&#148;{</string>
+<string size="16">&#4;a&#62;D&#197;&#227;`T@$&#193;&#212;&#62;z&#148;{</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1260</number></value>
 </dict>
 </trailer>
```

### Comparing `shiny_mdc-1.4.0/test/sections/appendix1.md` & `shiny_mdc-1.4.1/test/sections/appendix1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/test/sections/appendix2.md` & `shiny_mdc-1.4.1/test/sections/appendix2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/test/sections/main1.md` & `shiny_mdc-1.4.1/test/sections/main1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/test/sections/main2.md` & `shiny_mdc-1.4.1/test/sections/main2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/test/utils/commands.md` & `shiny_mdc-1.4.1/test/utils/commands.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.0/PKG-INFO` & `shiny_mdc-1.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny-mdc
-Version: 1.4.0
+Version: 1.4.1
 Summary: Tool to compile markdown files to tex/pdf using pandoc, latexmk
 Home-page: https://github.com/jayanthkoushik/shinymdc
 License: MIT
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

