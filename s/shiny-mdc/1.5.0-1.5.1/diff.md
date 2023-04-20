# Comparing `tmp/shiny_mdc-1.5.0.tar.gz` & `tmp/shiny_mdc-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiny_mdc-1.5.0.tar", max compression
+gzip compressed data, was "shiny_mdc-1.5.1.tar", max compression
```

## Comparing `shiny_mdc-1.5.0.tar` & `shiny_mdc-1.5.1.tar`

### file list

```diff
@@ -1,63 +1,64 @@
--rw-r--r--   0        0        0     4775 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/LICENSE
--rw-r--r--   0        0        0       78 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/README.md
--rw-r--r--   0        0        0     2297 2023-04-20 03:20:46.755515 shiny_mdc-1.5.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/__init__.py
--rw-r--r--   0        0        0     1061 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/_latexmk.py
--rw-r--r--   0        0        0     1867 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/_liquid.py
--rw-r--r--   0        0        0     4643 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/_pandoc.py
--rw-r--r--   0        0        0     4936 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/_templates.py
--rw-r--r--   0        0        0       64 2023-04-20 03:20:46.755515 shiny_mdc-1.5.0/shinymdc/_version.py
--rw-r--r--   0        0        0      410 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/dynamic/addappendices.tex
--rw-r--r--   0        0        0      881 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/dynamic/authsetup.tex
--rw-r--r--   0        0        0      317 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/dynamic/authsetupshort.tex
--rw-r--r--   0        0        0      572 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/dynamic/dblfloatsetup.tex
--rw-r--r--   0        0        0      482 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/bibnonatsetup.tex
--rw-r--r--   0        0        0     2475 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/bibsupersetup.tex
--rw-r--r--   0        0        0     3359 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/floatsetup.tex
--rw-r--r--   0        0        0    19901 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/iccv/bibstyle.bst
--rw-r--r--   0        0        0     9433 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/iccv/esopic.sty
--rw-r--r--   0        0        0     3869 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/iccv/everyshi.sty
--rw-r--r--   0        0        0     8276 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/iccv/iccv.sty
--rw-r--r--   0        0        0    26973 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/iclr/bibstyle.bst
--rw-r--r--   0        0        0     9153 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/iclr/iclr.sty
--rw-r--r--   0        0        0    12284 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/iclr/mathcommands.tex
--rw-r--r--   0        0        0    27146 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/resources/static/icml/bibstyle.bst
--rw-r--r--   0        0        0    27887 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/resources/static/icml/icml.sty
--rw-r--r--   0        0        0      735 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/resources/static/mathsetup.tex
--rw-r--r--   0        0        0     1153 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/resources/static/miscsetup.tex
--rw-r--r--   0        0        0    11306 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/resources/static/neurips/neurips.sty
--rw-r--r--   0        0        0      406 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/resources/static/reqsetup.tex
--rw-r--r--   0        0        0    19149 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/shinymdc.py
--rw-r--r--   0        0        0      945 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/basic.tex
--rw-r--r--   0        0        0     1302 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/iccv.tex
--rw-r--r--   0        0        0     1397 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/iclr.tex
--rw-r--r--   0        0        0     2144 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/icml.tex
--rw-r--r--   0        0        0      890 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/neurips.tex
--rw-r--r--   0        0        0     3064 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/spacious.tex
--rw-r--r--   0        0        0      464 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/standalone.tex
--rw-r--r--   0        0        0     2281 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/stylish.tex
--rw-r--r--   0        0        0    15953 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/figures/anscombe.pdf
--rw-r--r--   0        0        0    40892 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/figures/densities.pdf
--rw-r--r--   0        0        0    10736 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/figures/diamonds.pdf
--rw-r--r--   0        0        0   197017 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/figures/gaussian2d.pdf
--rw-r--r--   0        0        0    28282 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/figures/lines.png
--rw-r--r--   0        0        0     2973 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/main.md
--rwxr-xr-x   0        0        0      315 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/make.sh
--rw-r--r--   0        0        0     1166 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/references.bib
--rw-r--r--   0        0        0   690444 2023-04-20 03:20:21.785405 shiny_mdc-1.5.0/test/samples/basic.pdf
--rw-r--r--   0        0        0   413659 2023-04-20 03:20:21.789405 shiny_mdc-1.5.0/test/samples/iccv.pdf
--rw-r--r--   0        0        0   406993 2023-04-20 03:20:21.789405 shiny_mdc-1.5.0/test/samples/iclr.pdf
--rw-r--r--   0        0        0   446722 2023-04-20 03:20:21.793406 shiny_mdc-1.5.0/test/samples/icml.pdf
--rw-r--r--   0        0        0   451263 2023-04-20 03:20:21.797406 shiny_mdc-1.5.0/test/samples/neurips.pdf
--rw-r--r--   0        0        0   600203 2023-04-20 03:20:21.797406 shiny_mdc-1.5.0/test/samples/spacious.pdf
--rw-r--r--   0        0        0   554977 2023-04-20 03:20:21.801406 shiny_mdc-1.5.0/test/samples/standalone.pdf
--rw-r--r--   0        0        0   425121 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/samples/stylish.pdf
--rw-r--r--   0        0        0     1535 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/sections/appendix1.md
--rw-r--r--   0        0        0     1626 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/sections/appendix2.md
--rw-r--r--   0        0        0        0 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/sections/empty.md
--rw-r--r--   0        0        0     2320 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/sections/main1.md
--rw-r--r--   0        0        0     1354 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/sections/main2.md
--rw-r--r--   0        0        0      992 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/utils/commands.md
--rw-r--r--   0        0        0       41 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/utils/ext.md
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 shiny_mdc-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     5210 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/LICENSE
+-rw-r--r--   0        0        0       78 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/README.md
+-rw-r--r--   0        0        0     2297 2023-04-20 04:57:43.432761 shiny_mdc-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/__init__.py
+-rw-r--r--   0        0        0     1061 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/_latexmk.py
+-rw-r--r--   0        0        0     1867 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/_liquid.py
+-rw-r--r--   0        0        0     4643 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/_pandoc.py
+-rw-r--r--   0        0        0     5084 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/_templates.py
+-rw-r--r--   0        0        0       64 2023-04-20 04:57:43.432761 shiny_mdc-1.5.1/shinymdc/_version.py
+-rw-r--r--   0        0        0      410 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/dynamic/addappendices.tex
+-rw-r--r--   0        0        0      879 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/dynamic/authsetup.tex
+-rw-r--r--   0        0        0      316 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/dynamic/authsetupshort.tex
+-rw-r--r--   0        0        0      572 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/dynamic/dblfloatsetup.tex
+-rw-r--r--   0        0        0      491 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/bibnonatsetup.tex
+-rw-r--r--   0        0        0      324 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/bibnosupersetup.tex
+-rw-r--r--   0        0        0      745 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/bibsupersetup.tex
+-rw-r--r--   0        0        0     3359 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/floatsetup.tex
+-rw-r--r--   0        0        0    19901 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/iccv/bibstyle.bst
+-rw-r--r--   0        0        0     9433 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/iccv/esopic.sty
+-rw-r--r--   0        0        0     3869 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/iccv/everyshi.sty
+-rw-r--r--   0        0        0     8276 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/iccv/iccv.sty
+-rw-r--r--   0        0        0    26973 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/iclr/bibstyle.bst
+-rw-r--r--   0        0        0     9153 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/iclr/iclr.sty
+-rw-r--r--   0        0        0    12284 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/iclr/mathcommands.tex
+-rw-r--r--   0        0        0    27146 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/icml/bibstyle.bst
+-rw-r--r--   0        0        0    27887 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/icml/icml.sty
+-rw-r--r--   0        0        0      735 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/mathsetup.tex
+-rw-r--r--   0        0        0     1237 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/miscsetup.tex
+-rw-r--r--   0        0        0    11306 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/neurips/neurips.sty
+-rw-r--r--   0        0        0      406 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/reqsetup.tex
+-rw-r--r--   0        0        0    19208 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/shinymdc.py
+-rw-r--r--   0        0        0      945 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/basic.tex
+-rw-r--r--   0        0        0     1302 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/iccv.tex
+-rw-r--r--   0        0        0     1423 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/iclr.tex
+-rw-r--r--   0        0        0     2170 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/icml.tex
+-rw-r--r--   0        0        0      916 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/neurips.tex
+-rw-r--r--   0        0        0     3064 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/spacious.tex
+-rw-r--r--   0        0        0      464 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/standalone.tex
+-rw-r--r--   0        0        0     2281 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/stylish.tex
+-rw-r--r--   0        0        0    15953 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/figures/anscombe.pdf
+-rw-r--r--   0        0        0    40892 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/figures/densities.pdf
+-rw-r--r--   0        0        0    10736 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/figures/diamonds.pdf
+-rw-r--r--   0        0        0   197017 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/figures/gaussian2d.pdf
+-rw-r--r--   0        0        0    28282 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/figures/lines.png
+-rw-r--r--   0        0        0     2971 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/main.md
+-rwxr-xr-x   0        0        0      315 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/make.sh
+-rw-r--r--   0        0        0     1166 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/references.bib
+-rw-r--r--   0        0        0   690901 2023-04-20 04:57:19.092681 shiny_mdc-1.5.1/test/samples/basic.pdf
+-rw-r--r--   0        0        0   414185 2023-04-20 04:57:19.096681 shiny_mdc-1.5.1/test/samples/iccv.pdf
+-rw-r--r--   0        0        0   407653 2023-04-20 04:57:19.096681 shiny_mdc-1.5.1/test/samples/iclr.pdf
+-rw-r--r--   0        0        0   446740 2023-04-20 04:57:19.100681 shiny_mdc-1.5.1/test/samples/icml.pdf
+-rw-r--r--   0        0        0   451322 2023-04-20 04:57:19.100681 shiny_mdc-1.5.1/test/samples/neurips.pdf
+-rw-r--r--   0        0        0   600276 2023-04-20 04:57:19.104681 shiny_mdc-1.5.1/test/samples/spacious.pdf
+-rw-r--r--   0        0        0   555527 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/samples/standalone.pdf
+-rw-r--r--   0        0        0   425326 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/samples/stylish.pdf
+-rw-r--r--   0        0        0     1535 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/sections/appendix1.md
+-rw-r--r--   0        0        0     1624 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/sections/appendix2.md
+-rw-r--r--   0        0        0        0 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/sections/empty.md
+-rw-r--r--   0        0        0     2326 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/sections/main1.md
+-rw-r--r--   0        0        0     1351 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/sections/main2.md
+-rw-r--r--   0        0        0      992 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/utils/commands.md
+-rw-r--r--   0        0        0       41 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/utils/ext.md
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 shiny_mdc-1.5.1/PKG-INFO
```

### Comparing `shiny_mdc-1.5.0/CHANGELOG.md` & `shiny_mdc-1.5.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+### [1.5.1](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.5.0...v1.5.1) (2023-04-20)
+
+
+### Bug Fixes
+
+* fix spacing for citations, footnotes, and super/sub-scripts ([db84c5d](https://github.com/jayanthkoushik/shiny-mdc/commit/db84c5de40db26594876f6b83293ea6149aad10a))
+* prevent output during cleanup when in quiet mode ([d1193f0](https://github.com/jayanthkoushik/shiny-mdc/commit/d1193f06255165db99fd430836a631f7dadd2b12))
+
 ## [1.5.0](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.4.1...v1.5.0) (2023-04-20)
 
 
 ### Features
 
 * add appendix labels to footnotes ([8279712](https://github.com/jayanthkoushik/shiny-mdc/commit/8279712031ef4a36cc22720248a63cb22ffc6103))
 * add space before superscripts in author lists ([b0db384](https://github.com/jayanthkoushik/shiny-mdc/commit/b0db3843ebca5a68428f275517d3fefce280f45f))
```

### Comparing `shiny_mdc-1.5.0/LICENSE` & `shiny_mdc-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/pyproject.toml` & `shiny_mdc-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shiny-mdc"
-version = "1.5.0"  # managed by `poetry-dynamic-versioning`
+version = "1.5.1"  # managed by `poetry-dynamic-versioning`
 description = "Tool to compile markdown files to tex/pdf using pandoc, latexmk"
 readme = "README.md"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 repository = "https://github.com/jayanthkoushik/shinymdc"
 packages = [
   { include = "shinymdc" }
```

### Comparing `shiny_mdc-1.5.0/shinymdc/_latexmk.py` & `shiny_mdc-1.5.1/shinymdc/_latexmk.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/_liquid.py` & `shiny_mdc-1.5.1/shinymdc/_liquid.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/_pandoc.py` & `shiny_mdc-1.5.1/shinymdc/_pandoc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/_templates.py` & `shiny_mdc-1.5.1/shinymdc/_templates.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,17 +51,22 @@
             "iccv": [
                 "iccv/iccv.sty",
                 "iccv/esopic.sty",
                 "iccv/everyshi.sty",
                 "iccv/bibstyle.bst",
                 "bibnonatsetup.tex",
             ],
-            "iclr": ["iclr/iclr.sty", "iclr/bibstyle.bst", "iclr/mathcommands.tex"],
-            "icml": ["icml/icml.sty", "icml/bibstyle.bst"],
-            "neurips": ["neurips/neurips.sty"],
+            "iclr": [
+                "iclr/iclr.sty",
+                "iclr/bibstyle.bst",
+                "iclr/mathcommands.tex",
+                "bibnosupersetup.tex",
+            ],
+            "icml": ["icml/icml.sty", "icml/bibstyle.bst", "bibnosupersetup.tex"],
+            "neurips": ["neurips/neurips.sty", "bibnosupersetup.tex"],
         },
     )
     _dynamic_resources = defaultdict(
         list,
         {
             # Dynamic resources, defined similarly to static resources.
             "*": ["addappendices.tex"],
```

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/dynamic/authsetup.tex` & `shiny_mdc-1.5.1/shinymdc/resources/dynamic/authsetup.tex`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 \newlength{\maxnamelen}
 \newlength{\maxemlen}
 \newlength{\maxinstlen}
 
 % Use the longest name, email, and institute to get box sizes for the author list.
 \newbox\tempbox
-\savebox{\tempbox}{\hbox{$longest_author_name$~\textsuperscript{*}}}
+\savebox{\tempbox}{\hbox{$longest_author_name$\textsuperscript{*}}}
 \setlength{\maxnamelen}{\wd\tempbox}
 \savebox{\tempbox}{\hbox{\texttt{\textsmaller{$longest_email$}}}}
 \setlength{\maxemlen}{\wd\tempbox}
 \savebox{\tempbox}{\hbox{\textsmaller{$longest_inst_name$}}}
 \setlength{\maxinstlen}{\wd\tempbox}
 
 \author{%
   $for(author)$
-  \makebox[\maxnamelen][c]{$it.name$$if(it.equalcontrib)$$if(skipequal)$$else$~\textsuperscript{*}$endif$$endif$}$if(it.institute)$\\%
+  \makebox[\maxnamelen][c]{$it.name$$if(it.equalcontrib)$$if(skipequal)$$else$\textsuperscript{*}$endif$$endif$}$if(it.institute)$\\%
     $for(it.institute)$\makebox[\maxinstlen]{{\textsmaller{$it$}}}$sep$\\%
     $endfor$$endif$$if(it.email)$\\%
     \makebox[\maxemlen]{\href{mailto:$it.email$}{\texttt{\textsmaller{$it.email$}}}}$endif$%
   $sep$\vspace{1ex}\and%
   $endfor$%
 }
```

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/dynamic/dblfloatsetup.tex` & `shiny_mdc-1.5.1/shinymdc/resources/dynamic/dblfloatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/static/floatsetup.tex` & `shiny_mdc-1.5.1/shinymdc/resources/static/floatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/static/iccv/bibstyle.bst` & `shiny_mdc-1.5.1/shinymdc/resources/static/iccv/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/static/iccv/esopic.sty` & `shiny_mdc-1.5.1/shinymdc/resources/static/iccv/esopic.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/static/iccv/everyshi.sty` & `shiny_mdc-1.5.1/shinymdc/resources/static/iccv/everyshi.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/static/iccv/iccv.sty` & `shiny_mdc-1.5.1/shinymdc/resources/static/iccv/iccv.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/static/iclr/bibstyle.bst` & `shiny_mdc-1.5.1/shinymdc/resources/static/iclr/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/static/iclr/iclr.sty` & `shiny_mdc-1.5.1/shinymdc/resources/static/iclr/iclr.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/static/iclr/mathcommands.tex` & `shiny_mdc-1.5.1/shinymdc/resources/static/iclr/mathcommands.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/static/icml/bibstyle.bst` & `shiny_mdc-1.5.1/shinymdc/resources/static/icml/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/static/icml/icml.sty` & `shiny_mdc-1.5.1/shinymdc/resources/static/icml/icml.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/static/mathsetup.tex` & `shiny_mdc-1.5.1/shinymdc/resources/static/mathsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/static/miscsetup.tex` & `shiny_mdc-1.5.1/shinymdc/resources/static/miscsetup.tex`

 * *Files 7% similar despite different names*

```diff
@@ -22,25 +22,27 @@
 \makeatletter
 \renewcommand\@makefntext[1]{%
   \parindent 1em%
   \noindent
   \hb@xt@1.8em{\hss\@makefnmark}\,#1}
 \makeatother
 
+% Add small space before super/sub-scripts and footnotes.
+\let\origsup\textsuperscript
+\renewcommand{\textsuperscript}[1]{\,\origsup{#1}}
+\let\origsub\textsubscript
+\renewcommand{\textsubscript}[1]{\,\origsub{#1}}
+\let\origfootnote\footnote
+\renewcommand{\footnote}[1]{\,\origfootnote{#1}}
+
 % Create command for footnote without marker.
 \newcommand\blfootnote[1]{%
   \begingroup
   \begin{NoHyper}
   \renewcommand\thefootnote{}\footnote{\raggedright\hspace{-2em} #1}%
   \addtocounter{footnote}{-1}%
   \end{NoHyper}
   \endgroup
 }
 
 % Configure acronym font.
 \renewcommand*{\acsfont}[1]{{\scshape\textsmaller{#1}}}
-
-% Reduce space before superscripts and footnotes.
-\let\origts\textsuperscript
-\renewcommand{\textsuperscript}[1]{{\!\origts{#1}}}
-\let\origfootnote\footnote
-\renewcommand{\footnote}[1]{\!\origfootnote{#1}}
```

### Comparing `shiny_mdc-1.5.0/shinymdc/resources/static/neurips/neurips.sty` & `shiny_mdc-1.5.1/shinymdc/resources/static/neurips/neurips.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/shinymdc.py` & `shiny_mdc-1.5.1/shinymdc/shinymdc.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,23 +147,14 @@
         super().__init__(**kwargs)
         if not hasattr(self, "tex_files_dir"):
             self.tex_files_dir = self.build_dir / "main"
             self.tex_files_dir.mkdir(exist_ok=True)
         if not hasattr(self, "main_tex_path"):
             self.main_tex_path = self.tex_files_dir / "main.tex"
             self.main_tex_path.touch()
-        if hasattr(self, "clean"):
-            for _f in self.tex_files_dir.glob("*.tex"):
-                if _f.is_file():
-                    print(f"+ rm '{_f}'")
-                    _f.unlink()
-            _rescs_dir = self.tex_files_dir / "resources"
-            if _rescs_dir.is_dir():
-                print(f"+ rm -rf '{_rescs_dir}'")
-                shutil.rmtree(_rescs_dir, ignore_errors=True)
         if not hasattr(self, "meta"):
             self.meta = KeyValuePairs("")
 
     def __call__(self) -> int:
         # Wrap the actual call with stdout/stderr redirections.
         # If 'output_path' is not specified, output has to be written to stdout.
         # So, redirect stdout to stderr to prevent subprocesses from writing
@@ -202,14 +193,25 @@
             if ret != 0 and temp_file is not None:
                 # Print stderr output from temp file.
                 temp_file.seek(0)
                 print(temp_file.read(), file=true_stderr)
         return ret
 
     def _call(self, stdout) -> None:
+        ## 0. Clean up.
+        if hasattr(self, "clean"):
+            for _f in self.tex_files_dir.glob("*.tex"):
+                if _f.is_file():
+                    print(f"+ rm '{_f}'", file=sys.stderr)
+                    _f.unlink()
+            _rescs_dir = self.tex_files_dir / "resources"
+            if _rescs_dir.is_dir():
+                print(f"+ rm -rf '{_rescs_dir}'", file=sys.stderr)
+                shutil.rmtree(_rescs_dir, ignore_errors=True)
+
         ## 1. Load input and parse metadata.
 
         # Read input from the input file or stdin.
         if hasattr(self, "input_path"):
             print(f"+ read '{self.input_path}'", file=sys.stderr)
             input_data = self.input_path.read_text()
         else:
```

### Comparing `shiny_mdc-1.5.0/shinymdc/templates/basic.tex` & `shiny_mdc-1.5.1/shinymdc/templates/basic.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/templates/iccv.tex` & `shiny_mdc-1.5.1/shinymdc/templates/iccv.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/templates/iclr.tex` & `shiny_mdc-1.5.1/shinymdc/templates/iclr.tex`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 \usepackage{$iclr$,newtxtext}
 \usepackage{url}
 
 \input{$reqsetup$}
 \input{$floatsetup$}
 \input{$mathsetup$}
 \input{$miscsetup$}
+\input{$bibnosupersetup$}
 
 % Optional math commands from https://github.com/goodfeli/dlbook_notation.
 % \input{$mathcommands$.tex}
 
 \title{$title$}
 
 % The \author macro works with any number of authors. There are two commands
```

### Comparing `shiny_mdc-1.5.0/shinymdc/templates/icml.tex` & `shiny_mdc-1.5.1/shinymdc/templates/icml.tex`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 \usepackage$if(submission)$$else$[accepted]$endif${$icml$}
 
 \input{$floatsetup$}
 \input{$dblfloatsetup$}
 \input{$mathsetup$}
 \input{$miscsetup$}
+\input{$bibnosupersetup$}
 
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 % THEOREMS
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 \theoremstyle{plain}
 \newtheorem{theorem}{Theorem}[section]
 \newtheorem{proposition}[theorem]{Proposition}
```

### Comparing `shiny_mdc-1.5.0/shinymdc/templates/neurips.tex` & `shiny_mdc-1.5.1/shinymdc/templates/neurips.tex`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 \PassOptionsToPackage{numbers,sort&compress}{natbib}
 \usepackage$if(submission)$$else$$if(preprint)$[preprint]$else$[final]$endif$$endif${$neurips$}
 
 \input{$reqsetup$}
 \input{$floatsetup$}
 \input{$mathsetup$}
 \input{$miscsetup$}
+\input{$bibnosupersetup$}
 
 \title{$title$}
 
 \input{$authsetup$}
 
 $for(includes)$
 $it$
```

### Comparing `shiny_mdc-1.5.0/shinymdc/templates/spacious.tex` & `shiny_mdc-1.5.1/shinymdc/templates/spacious.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/shinymdc/templates/stylish.tex` & `shiny_mdc-1.5.1/shinymdc/templates/stylish.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/test/figures/anscombe.pdf` & `shiny_mdc-1.5.1/test/figures/anscombe.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/test/figures/densities.pdf` & `shiny_mdc-1.5.1/test/figures/densities.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/test/figures/diamonds.pdf` & `shiny_mdc-1.5.1/test/figures/diamonds.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/test/figures/gaussian2d.pdf` & `shiny_mdc-1.5.1/test/figures/gaussian2d.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/test/figures/lines.png` & `shiny_mdc-1.5.1/test/figures/lines.png`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/test/main.md` & `shiny_mdc-1.5.1/test/main.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   affiliation:
   - 2
 institute:
 - id: 1
   name: Institute One
 - id: 2
   name: Institute Two at City, State
-abstract: _Markdown_ **in** **_abstract_**. $x+2$. @sec:ex1. Reference\ [@texbook].
+abstract: _Markdown_ **in** **_abstract_**. $x+2$. @sec:ex1. Reference[@texbook].
 bibliography: references.bib
 sections:
 - sections/main1.md
 - sections/main2.md
 - sections/empty.md
 appendices:
 - sections/appendix1.md
```

### Comparing `shiny_mdc-1.5.0/test/references.bib` & `shiny_mdc-1.5.1/test/references.bib`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/test/samples/basic.pdf` & `shiny_mdc-1.5.1/test/samples/basic.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 8% similar despite different names*

#### pdftotext {} -

```diff
@@ -120,14 +120,16 @@
 
 2
 
 Typography
 • Bold
 • Italic
 • Bold italic.
+• Super script
+• Sub script
 
 3
 
 Numbers
 • Normal: 0123456789
 • Math: 0123456789
```

### Comparing `shiny_mdc-1.5.0/test/samples/iccv.pdf` & `shiny_mdc-1.5.1/test/samples/iccv.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 5% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,20 +1,20 @@
 shinymdc-test
-Author One*
+Author One *
 
-Author MiddleName Two*
+Author MiddleName Two *
 
 Institute One
 author1@institute1.edu
 
 Institute One
 Institute Two at City, State
 authortwo@institute1.edu
 
-Author*
+Author *
 
 Author Four
 
 Author Number Five
 
 author4@author4.com
 
@@ -104,18 +104,24 @@
 
 15
 
 (c) Sub-figure with ‘width=2in’
 
 Aliquam at ultrices libero. Nulla facilisi. Fusce sed est
 placerat, fringilla augue at, pretium nisl.
+
+x=1
+x + y = 10
+
 1.2.2
 
 Subsubsection 2
 
+x + y + z = 100
+
 In ut nunc libero. Duis eu elementum purus. Etiam dictum,
 ipsum nec aliquam lobortis, magna magna pellentesque
 ligula, sed ultricies odio ligula vitae orci. Fusce bibendum
 maximus ligula, id gravida felis dictum a. In dapibus nulla
 eget volutpat vulputate. Quisque congue erat quis nibh
 molestie, eget varius eros ultrices.
 Subsubsubsection Proin eleifend lorem semper, commodo
@@ -123,25 +129,47 @@
 consequat maximus lorem faucibus in. Nam purus eros,
 rutrum in sapien et, condimentum lacinia nibh.
 
 2. Typography
 • Bold
 • Italic
 • Bold italic.
+• Super ˢᶜʳⁱᵖᵗ
+• Sub script
 
 3. Numbers
 • Normal: 0123456789
 • Math: 0123456789
 
+4. Acronyms
+• Default (short+long): Carnegie Mellon University
+(CMU)
+• Repeated (short): CMU
+• Forced short: USA
+• Repeated after forced short (short+long): United States
+of America (USA)
+• Plural: social security numbers (SSNs)
+
+5. Math
+Z ∞
+0
+
+2
+
+exp−x dx
+
+(1)
+
+6. Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
-• Pointer to footnote¹² text
+• Pointer to footnote ¹ ² text
 
 7. Citations
 • Short citation [4]
 • Short citation with pre note [4]
 • Short citation with locator [4, p. 1]
 • Short citation with post note [4, for more]
 • Short citation with locators and pre/post notes [4,
@@ -153,29 +181,14 @@
 • Multi citation with pre note [3, 1, 4]
 • Multi citation with locators ([3, sec. 1]; [1]; [4, p. 1-3])
 • Multi citation with post note [3, 1, 4, for more]
 • Multi citation with locators and pre/post notes ([3, p. 1];
 [1]; [4, chap. 1-2, for more])
 
 8. Tables
-
-4. Acronyms
-• Default (short+long): Carnegie Mellon University
-(CMU)
-• Repeated (short): CMU
-• Forced short: USA
-• Repeated after forced short (short+long): United States
-of America (USA)
-• Plural: social security numbers (SSNs)
-
-5. Math
-Z ∞
-
-6. Links
-
 • Table 1
 • Table 2
 
 Col1
 
 Col2
 
@@ -196,47 +209,27 @@
 333
 
 4
 44
 444
 
 Table 1: Short table
-−x2
-
-exp
-
-dx
-
-(1)
-
-0
 
-9.2,Figures
-a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1,
-3, 4, 5, 6, 7, 8, 9
+a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
 (2)
-• Figure 2
+9. Figures
 R∞
 2
-• Figure 3
 • Inline: 0 exp−x dx
-• Figure 4, Figure 4a, Figure 4b
+• Figure 2
 • Block: Equation 1, Equation 2
+• Figure 3
 • Commands defined in body (P[x in X]): P[x ∈ X ]
+• Figure 4, Figure 4a, Figure 4b
 • Aligned:
-x=1
-x + y = 10
-x + y + z = 100
-
-¹ Example footnote text.
-² Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum,
-at tempor nisl. Vivamus vitae pulvinar leo, at pharetra massa. Ut lobortis
-odio non nulla tincidunt pulvinar.
-³ Footnote in sub-figure caption.
-⁴ Footnote in figure caption.
 
 A
 B
 C
 D
 E
 F
@@ -297,17 +290,17 @@
 
 x
 
 15
 
 5
 
-(b) Figure with ‘width=3.5in’³
+(b) Figure with ‘width=3.5in’ ³
 
-Figure 4: Sub-figures⁴
+Figure 4: Sub-figures ⁴
 
 10
 
 x
 
 15
 
@@ -379,14 +372,18 @@
 4
 
 5
 
 6
 
 Table 2: Wide table
+[4] Frank Mittelbach, Michel Gossens, Johannes Braams, David
+Carlisle, and Chris Rowley. The LATEX Companion. AddisonWesley Professional, 2 edition, 2004.
+
+Figure 2: Narrow figure
 
 10. Includes
 • Commands from metadata include: arg min R
 • Include command in body (there should be text after
 this):
 Content added through include statement.
 
@@ -395,18 +392,20 @@
 Journal, 27(2):97–111, 1984.
 [2] Donald E. Knuth. The TEX Book. Addison-Wesley Professional,
 1986.
 [3] Michael Lesk and Brian Kernighan. Computer typesetting
 of technical journals on UNIX. In Proceedings of American
 Federation of Information Processing Societies: 1977 National
 Computer Conference, pages 879–888, Dallas, Texas, 1977.
-[4] Frank Mittelbach, Michel Gossens, Johannes Braams, David
-Carlisle, and Chris Rowley. The LATEX Companion. AddisonWesley Professional, 2 edition, 2004.
-
-Figure 2: Narrow figure
+¹ Example footnote text.
+² Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum,
+at tempor nisl. Vivamus vitae pulvinar leo, at pharetra massa. Ut lobortis
+odio non nulla tincidunt pulvinar.
+³ Footnote in sub-figure caption.
+⁴ Footnote in figure caption.
 
 A
 B
 C
 D
 E
 F
@@ -454,24 +453,30 @@
 Proin eleifend lorem semper, commodo tellus nec, porta
 purus. Nullam commodo lectus nibh, consequat maximus
 lorem faucibus in. Nam purus eros, rutrum in sapien et,
 condimentum lacinia nibh.
 
 A.2. Appendix figures
 • Figure A1
+
 • Figure A2
 
 A.3. Appendix includes
 • Commands from metadata include (argmin R):
 • Include command in body (there should be text after
 this):
 Content added through include statement.
 
 A.4. Appendix links
 • Appendix section: Section A.1.1, Section B
+• Main body section: Section 1
+• Main body figure: Figure 2
+• Main body table: Table 1
+• Main body equation: Equation 1
+• Citation: [1]
 
 (a) Figure with non-default extension
 
 (b) Sub-figure
 
 dataset = I
 
@@ -514,20 +519,14 @@
 
 (c) Sub-figure
 
 Figure A2: Sub-figures with large combined size.
 
 15
 
-• Main body section: Section 1
-• Main body figure: Figure 2
-• Main body table: Table 1
-• Main body equation: Equation 1
-• Citation: [1]
-
 Col1
 
 Col2
 
 Col3
 
 Col4
@@ -586,15 +585,15 @@
 
 1234
 567
 89
 
 444
 44
-4ᴮ²
+4 ᴮ²
 
 a
 aa
 aaa
 
 bbb
 bb
@@ -628,15 +627,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1: Extra wide tableᴮ³
+Table B1: Extra wide table ᴮ³
 
 Appendix B. Appendix 2
 Lorem ipsum dolor sit amet, consectetur adipiscing elit.
 Aliquam nisi purus, bibendum non neque sed, lacinia tristique
 tortor. Vestibulum eu lectus sed velit luctus varius. Sed
 sollicitudin ligula ante. Integer porta a erat commodo
 dignissim. Duis et lectus diam. Nulla id erat vestibulum
```

### Comparing `shiny_mdc-1.5.0/test/samples/iclr.pdf` & `shiny_mdc-1.5.1/test/samples/iclr.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,22 +1,22 @@
 sh inymdc-test
-Author One*
+Author One *
 
-Author MiddleName Two*
+Author MiddleName Two *
 
 Institute One
 
 Institute One
 Institute Two at City, State
 
 author1@institute1.edu
 
 authortwo@institute1.edu
 
-Author*
+Author *
 
 Author Four
 author4@author4.com
 
 Author Number Five
 Institute Two at City, State
 authornumberfive@institutetwo.edu
@@ -95,18 +95,18 @@
 8
 6
 4
 5
 
 10
 
-15
-
 x
 
+15
+
 5
 
 10
 
 x
 
 15
@@ -117,14 +117,16 @@
 
 2
 
 Typography
 • Bold
 • Italic
 • Bold italic.
+• Super ˢᶜʳⁱᵖᵗ
+• Sub script
 
 3
 
 Numbers
 • Normal: 0123456789
 • Math: 0123456789
 
@@ -132,31 +134,30 @@
 
 Acronyms
 • Default (short+long): Carnegie Mellon University (CMU)
 • Repeated (short): CMU
 • Forced short: USA
 • Repeated after forced short (short+long): United States of America (USA)
 • Plural: social security numbers (SSNs)
+2
 
-5
+5
 
 Math
 Z ∞
 
 2
 
 exp−x dx
 
-0
-
-2
-
 (1)
 
-a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
+0
+
+a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
 
 (2)
 
 R∞
 2
 • Inline: 0 exp−x dx
 • Block: Equation 1, Equation 2
@@ -170,15 +171,15 @@
 
 Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
-• Pointer to footnote¹² text
+• Pointer to footnote ¹ ² text
 
 7
 
 Citations
 • Short citation (Mittelbach et al., 2004)
 • Short citation with pre note (see Mittelbach et al., 2004)
 • Short citation with locator (Mittelbach et al., 2004, p. 1)
@@ -200,20 +201,14 @@
 
 8
 
 Tables
 • Table 1
 • Table 2
 
-9
-
-Figures
-• Figure 2
-• Figure 3
-
 ¹ Example footnote text.
 ² Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum, at tempor nisl. Vivamus vitae
 pulvinar leo, at pharetra massa. Ut lobortis odio non nulla tincidunt pulvinar.
 
 3
 
 Col1
@@ -309,29 +304,32 @@
 4
 
 5
 
 6
 
 Table 2: Wide table
+
+9
+
+Figures
+
+Figure 2: Narrow figure
+
+• Figure 2
+• Figure 3
 • Figure 4, Figure 4a, Figure 4b
 
 10
 
 Includes
 • Commands from metadata include: arg min R
 • Include command in body (there should be text after this):
 
 Content added through include statement.
-
-References
-Donald E. Knuth. Literate programming. The Computer Journal, 27(2):97–111, 1984.
-Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
-
-Figure 2: Narrow figure
 ³ Footnote in sub-figure caption.
 ⁴ Footnote in figure caption.
 
 4
 
 A
 B
@@ -359,14 +357,18 @@
 72
 
 74
 
 76
 
 Figure 3: Wide figure
+
+References
+Donald E. Knuth. Literate programming. The Computer Journal, 27(2):97–111, 1984.
+Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
 Michael Lesk and Brian Kernighan. Computer typesetting of technical journals on UNIX. In
 Proceedings of American Federation of Information Processing Societies: 1977 National Computer
 Conference, pp. 879–888, Dallas, Texas, 1977.
 Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle, and Chris Rowley. The LATEX
 Companion. Addison-Wesley Professional, 2 edition, 2004.
 
 5
@@ -404,17 +406,17 @@
 
 x
 
 15
 
 5
 
-(b) Figure with ‘width=3.5in’³
+(b) Figure with ‘width=3.5in’ ³
 
-Figure 4: Sub-figures⁴
+Figure 4: Sub-figures ⁴
 
 6
 
 10
 
 x
 
@@ -609,15 +611,15 @@
 
 1234
 567
 89
 
 444
 44
-4ᴮ²
+4 ᴮ²
 
 a
 aa
 aaa
 
 bbb
 bb
@@ -651,15 +653,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1: Extra wide tableᴮ³
+Table B1: Extra wide table ᴮ³
 
 Appendix B
 
 Appendix 2
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi purus, bibendum non neque
 sed, lacinia tristique tortor. Vestibulum eu lectus sed velit luctus varius. Sed sollicitudin ligula ante.
```

### Comparing `shiny_mdc-1.5.0/test/samples/icml.pdf` & `shiny_mdc-1.5.1/test/samples/icml.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,10 +1,10 @@
 shinymdc-test
 
-Author One*1 Author MiddleName Two*12 Author* Author Four Author Number Five2
+Author One * 1 Author MiddleName Two * 1 2 Author * Author Four Author Number Five 2
 
 Abstract
 Markdown in abstract. x + 2.
 Reference (Knuth, 1986).
 
 1.1. Subsection 1
 Section 1.
@@ -109,18 +109,25 @@
 (c) Sub-figure with ‘width=2in’
 
 Subsubsubsection Proin eleifend lorem semper,
 commodo tellus nec, porta purus. Nullam commodo lectus
 nibh, consequat maximus lorem faucibus in. Nam purus
 eros, rutrum in sapien et, condimentum lacinia nibh.
 
+• Appendix math: Equation 4
+• Pointer to footnote 1 2 text
+
+7. Citations
+
 2. Typography
 • Bold
 • Italic
 • Bold italic.
+• Super script
+• Sub script
 
 3. Numbers
 • Normal: 0123456789
 • Math: 0123456789
 
 4. Acronyms
 • Default (short+long): Carnegie Mellon University
@@ -136,19 +143,17 @@
 
 2
 
 exp−x dx
 
 (1)
 
-• Pointer to footnote 1 2 text
-
-7. Citations
 • Short citation (Mittelbach et al., 2004)
-• Short citation with pre note (see Mittelbach et al., 2004)
+• Short citation with pre note (see Mittelbach et al.,
+2004)
 • Short citation with locator (Mittelbach et al., 2004,
 p. 1)
 • Short citation with post note (Mittelbach et al., 2004,
 for more)
 • Short citation with locators and pre/post notes (see
 Mittelbach et al., 2004, chap. 1-4, for more)
 • Long citation: Lesk & Kernighan (1977)
@@ -164,72 +169,64 @@
 sec. 1; Knuth, 1984; Mittelbach et al., 2004, p. 1-3)
 • Multi citation with post note (Lesk & Kernighan, 1977;
 Knuth, 1984; Mittelbach et al., 2004, for more)
 • Multi citation with locators and pre/post notes (see
 Lesk & Kernighan, 1977, p. 1; Knuth, 1984; Mittelbach
 et al., 2004, chap. 1-2, for more)
 
-8. Tables
-
 0
 
-• Table 1
-• Table 2
+8. Tables
+
 a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
 (2)
-Col1 Col2
+• Table 1
+• Table 2
 R∞
-−x2
-• Inline: 0 exp
-dx
-1
 2
+• Inline: 0 exp−x dx
 • Block: Equation 1, Equation 2
-11
-22
 • Commands defined in body (P[x in X]): P[x ∈ X ]
-111
-222
 • Aligned:
 
+x=1
+x + y = 10
+x + y + z = 100
+
+Col1
+
+Col2
+
 Col3
 
 Col4
 
+1
+11
+111
+
+2
+22
+222
+
 3
 33
 333
 
 4
 44
 444
 
-Table 1. Short table
-
-x=1
-x + y = 10
-x + y + z = 100
-
-9. Figures
-• Figure 2
-
 6. Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
-• Appendix math: Equation 4
-
-1
 
-Example footnote text.
-Integer at enim eu tellus malesuada scelerisque. Ut sed
-rhoncus ipsum, at tempor nisl. Vivamus vitae pulvinar leo, at
-pharetra massa. Ut lobortis odio non nulla tincidunt pulvinar.
-2
+Table 1. Short table
 
 Col1
 
 Col2
 
 Col3
 
@@ -327,32 +324,39 @@
 
 74
 
 76
 
 Figure 3. Wide figure
 
+9. Figures
+• Figure 2
 • Figure 3
 • Figure 4, Figure 4a, Figure 4b
 
 10. Includes
 • Commands from metadata include: arg min R
 • Include command in body (there should be text after
 this):
-Content added through include statement.
 
-Figure 2. Narrow figure
+1
 
+Example footnote text.
+Integer at enim eu tellus malesuada scelerisque. Ut sed
+rhoncus ipsum, at tempor nisl. Vivamus vitae pulvinar leo, at
+pharetra massa. Ut lobortis odio non nulla tincidunt pulvinar.
 3
-
 Footnote in sub-figure caption.
+4
 Footnote in figure caption.
 5
 Footnote in figure caption.
-4
+2
+
+Figure 2. Narrow figure
 
 dataset = I
 
 dataset = II
 
 dataset = III
 
@@ -376,24 +380,26 @@
 6
 4
 5
 (a) Figure with ‘width=2.5in’
 
 10
 
-x
-
 15
 
 5
 
 (b) Figure with ‘width=3.5in’ 3
 
 Figure 4. Sub-figures 5
 
+Content added through include statement.
+
+x
+
 10
 
 x
 
 15
 
 References
```

### Comparing `shiny_mdc-1.5.0/test/samples/neurips.pdf` & `shiny_mdc-1.5.1/test/samples/neurips.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 4% similar despite different names*

#### pdftotext {} -

```diff
@@ -107,25 +107,26 @@
 x
 
 15
 
 (c) Sub-figure with ‘width=2in’
 
 Figure 1: Sub-figures
-
 Subsubsubsection Proin eleifend lorem semper, commodo tellus nec, porta purus. Nullam
 commodo lectus nibh, consequat maximus lorem faucibus in. Nam purus eros, rutrum in sapien et,
 condimentum lacinia nibh.
 
 2
 
 Typography
 • Bold
 • Italic
 • Bold italic.
+• Super script
+• Sub script
 
 3
 
 Numbers
 • Normal: 0123456789
 • Math: 0123456789
```

### Comparing `shiny_mdc-1.5.0/test/samples/spacious.pdf` & `shiny_mdc-1.5.1/test/samples/spacious.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -106,14 +106,16 @@
 faucibus in. Nam purus eros, rutrum in sapien et, condimentum lacinia
 nibh.
 
 2. Typography
 • Bold
 • Italic
 • Bold italic.
+• Super script
+• Sub script
 
 3. Numbers
 • Normal: 0123456789
 • Math: 0123456789
 
 4. Acronyms
 • Default (short+long): Carnegie Mellon University (C M U )
@@ -133,21 +135,21 @@
 (1)
 
 a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
 (2)
 • Inline: 0∞ exp−x dx
 • Block: Equation 1, Equation 2
 • Commands defined in body (P[x in X]): P[x ∈ X ]
-• Aligned:
 R
 
 2
 
 4
 
+• Aligned:
 x=1
 x + y = 10
 x + y + z = 100
 
 6. Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B 2, Section A 1.1.1
```

### Comparing `shiny_mdc-1.5.0/test/samples/standalone.pdf` & `shiny_mdc-1.5.1/test/samples/standalone.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 9% similar despite different names*

#### pdftotext {} -

```diff
@@ -98,14 +98,16 @@
 
 2
 
 Typography
 • Bold
 • Italic
 • Bold italic.
+• Super script
+• Sub script
 
 3
 
 Numbers
 • Normal: 0123456789
 • Math: 0123456789
```

### Comparing `shiny_mdc-1.5.0/test/samples/stylish.pdf` & `shiny_mdc-1.5.1/test/samples/stylish.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -113,107 +113,121 @@
 quat maximus lorem faucibus in. Nam purus eros, rutrum in
 sapien et, condimentum lacinia nibh.
 
 2. Typography
 • Bold
 • Italic
 • Bold italic.
+• Super ˢᶜʳⁱᵖᵗ
+• Sub script
 
 3. Numbers
 • Normal: 0123456789
 • Math: 0123456789
 
 4. Acronyms
 • Default (short+long): Carnegie Mellon University
 (CMU)
 • Repeated (short): CMU
 • Forced short: USA
 • Repeated after forced short (short+long): United States
 of America (USA)
 • Plural: social security numbers (SSNs)
 
+5. Math
+Z ∞
+
+• Pointer to footnote ¹ ² text
+
 7. Citations
-• Short citation[²]
-• Short citation with pre note[ˢᵉᵉ ²]
-• Short citation with locator[²𝄒 ᵖ⋅ ¹]
-• Short citation with post note[²𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
-• Short citation with locators and pre/post notes[ˢᵉᵉ ²𝄒 ᶜʰᵃᵖ⋅ ¹⁻
+• Short citation [²]
+• Short citation with pre note [ˢᵉᵉ ²]
+• Short citation with locator [²𝄒 ᵖ⋅ ¹]
+• Short citation with post note [²𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
+• Short citation with locators and pre/post notes [ˢᵉᵉ ²𝄒 ᶜʰᵃᵖ⋅ ¹⁻
 ⁴𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
-• Long citation: Lesk and Kernighan (1977)[³]
-• Long citation with locator: Lesk and Kernighan (1977)[³𝄒
+• Long citation: Lesk and Kernighan (1977) [³]
+• Long citation with locator: Lesk and Kernighan (1977) [³𝄒
 ᶜʰᵃᵖ⋅ ¹]
-• Long citation with note: Lesk and Kernighan (1977)[³𝄒
+• Long citation with note: Lesk and Kernighan (1977) [³𝄒
 ᶠᵒʳ ᵐᵒʳᵉ]
-• Multi citation[²𝄒 ³𝄒 ⁴]
-• Multi citation with pre note[ˢᵉᵉ ²𝄒 ³𝄒 ⁴]
-• Multi citation with locators[³𝄒 ˢᵉᶜ⋅ ¹; ⁴; ²𝄒 ᵖ⋅ ¹⁻³]
-• Multi citation with post note[²𝄒 ³𝄒 ⁴𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
-• Multi citation with locators and pre/post notes[ˢᵉᵉ ³𝄒 ᵖ⋅ ¹;
+• Multi citation [²𝄒 ³𝄒 ⁴]
+• Multi citation with pre note [ˢᵉᵉ ²𝄒 ³𝄒 ⁴]
+• Multi citation with locators [³𝄒 ˢᵉᶜ⋅ ¹; ⁴; ²𝄒 ᵖ⋅ ¹⁻³]
+• Multi citation with post note [²𝄒 ³𝄒 ⁴𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
+• Multi citation with locators and pre/post notes [ˢᵉᵉ ³𝄒 ᵖ⋅ ¹;
 ⁴; ²𝄒 ᶜʰᵃᵖ⋅ ¹⁻²𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
 
 8. Tables
 • Table 1
 • Table 2
 
-5. Math
-Z ∞
+Col1
 
-2
+Col2
 
-exp−x dx
+Col3
 
-(1)
+Col4
 
-0
+1
+11
+111
+a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
+(2)
 
-Col1 Col2 Col3 Col4
-a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 17, 8, 9
 2
-3
-4
-(2)
-11
 22
-33
-44
-R∞
-−x2
-111
 222
+
+3
+33
 333
+
+4
+44
 444
-• Inline: 0 exp
-dx
-• Block: Equation 1, Equation 2
+
+2
+
+exp−x dx
+
+(1)
+
+0
+
 Table 1: Short table
+
+R∞
+
+• Inline: 0 exp−x dx
+• Block: Equation 1, Equation 2
 • Commands defined in body (P[x in X]): P[x ∈ X ]
 • Aligned:
+2
+
 x=1
+
+9. Figures
+• Figure 2
+• Figure 3
+• Figure 4, Figure 4a, Figure 4b
+
 x + y = 10
 x + y + z = 100
 
 6. Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
-• Pointer to footnote¹² text
 
 ¹ Example footnote text.
 ² Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum,
-
-9. Figures
-• Figure 2
-• Figure 3
-• Figure 4, Figure 4a, Figure 4b
-
-10. Includes
-• Commands from metadata include: arg min R
-
 at tempor nisl. Vivamus vitae pulvinar leo, at pharetra massa. Ut lobortis
 odio non nulla tincidunt pulvinar.
 ³ Footnote in sub-figure caption.
 ⁴ Footnote in figure caption.
 
 2
 
@@ -286,17 +300,17 @@
 
 10
 
 x
 
 15
 
-(b) Figure with ‘width=3.5in’³
+(b) Figure with ‘width=3.5in’ ³
 
-Figure 4: Sub-figures⁴
+Figure 4: Sub-figures ⁴
 
 3
 
 Col1
 
 Col2
 
@@ -365,14 +379,16 @@
 
 5
 
 6
 
 Table 2: Wide table
 
+10. Includes
+• Commands from metadata include: arg min R
 • Include command in body (there should be text after
 this):
 Content added through include statement.
 
 References
 [1] Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
 [2] Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle,
@@ -502,15 +518,15 @@
 
 A.4 Appendix links
 • Appendix section: Section A.1.1, Section B
 • Main body section: Section 1
 • Main body figure: Figure 2
 • Main body table: Table 1
 • Main body equation: Equation 1
-• Citation: Knuth (1984)[⁴]
+• Citation: Knuth (1984) [⁴]
 
 7
 
 Col1
 
 Col2
 
@@ -572,15 +588,15 @@
 
 1234
 567
 89
 
 444
 44
-4ᴮ²
+4 ᴮ²
 
 a
 aa
 aaa
 
 bbb
 bb
@@ -614,15 +630,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1: Extra wide tableᴮ³
+Table B1: Extra wide table ᴮ³
 
 Appendix B
 
 Appendix 2
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi purus, bibendum non neque sed, lacinia tristique
 tortor. Vestibulum eu lectus sed velit luctus varius. Sed sollicitudin ligula ante. Integer porta a erat commodo dignissim.
```

### Comparing `shiny_mdc-1.5.0/test/sections/appendix1.md` & `shiny_mdc-1.5.1/test/sections/appendix1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/test/sections/appendix2.md` & `shiny_mdc-1.5.1/test/sections/appendix2.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 * @tbl:app2ex1
 
 Col1       Col2     Col3     Col4     Col5     Col6     Col7      Col8     Col9     Col10     Col11     Col12     Col13     Col14     Col15     Col16     Col17   Col17
 ------   ------   ------   ------   ------   ------   ------   -------   ------   -------   -------   -------   -------   -------   -------   -------   -------   -------
 a             1        2        3      123     abcd     1234       444        a       bbb      cccc       ddd      eeee       fff      gggg      abcd      1234   9876
 b            11       22       33      456     efgh      567        44       aa        bb      cccc        dd      eeee        ff      gggg      efgh       567   543
-c           111      222      333      789     ijkl       89   4\ [^t]      aaa         b      cccc         d      eeee         f      gggg      ijkl        89   21
+c           111      222      333      789     ijkl       89     4[^t]      aaa         b      cccc         d      eeee         f      gggg      ijkl        89   21
 
-: Extra wide table\ [^u] {#tbl:app2ex1}
+: Extra wide table[^u] {#tbl:app2ex1}
 
 [^t]: Footnote in table.
 [^u]: Footnote in table caption.
 
 ## Appendix math
 
 $$
```

### Comparing `shiny_mdc-1.5.0/test/sections/main1.md` & `shiny_mdc-1.5.1/test/sections/main1.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Typography
 
 * **Bold**
 * _Italic_
 * **_Bold italic_**.
-
+* Super^script^
+* Sub~script~
 
 # Numbers
 
 * Normal: 0123456789
 * Math: $0123456789$
 
 
@@ -56,29 +57,29 @@
 # Links
 
 * Section: @sec:ex1, @sec:ex1.2
 * Appendix section: @sec:app2ex1, @sec:app1ex1.1.1
 * Appendix figure: @fig:app1ex1
 * Appendix table: @tbl:app2ex1
 * Appendix math: @eq:app2ex2
-* Pointer to footnote\ [^1] [^2] text
+* Pointer to footnote[^1][^2] text
 
 [^1]: Example footnote text.
 [^2]: Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum, at tempor
       nisl. Vivamus vitae pulvinar leo, at pharetra massa. Ut lobortis odio non nulla
       tincidunt pulvinar.
 
 # Citations
 
-* Short citation\ [@latex:companion]
-* Short citation with pre note\ [see @latex:companion]
-* Short citation with locator\ [@latex:companion, p. 1]
-* Short citation with post note\ [@latex:companion, for more]
-* Short citation with locators and pre/post notes\ [see @latex:companion, chap. 1-4, for more]
+* Short citation[@latex:companion]
+* Short citation with pre note[see @latex:companion]
+* Short citation with locator[@latex:companion, p. 1]
+* Short citation with post note[@latex:companion, for more]
+* Short citation with locators and pre/post notes[see @latex:companion, chap. 1-4, for more]
 * Long citation: @lesk:1977
 * Long citation with locator: @lesk:1977 [chap. 1]
 * Long citation with note: @lesk:1977 [for more]
-* Multi citation\ [@lesk:1977; @knuth:1984; @latex:companion]
-* Multi citation with pre note\ [see @lesk:1977; @knuth:1984; @latex:companion]
-* Multi citation with locators\ [@lesk:1977, sec. 1; @knuth:1984; @latex:companion, p. 1-3]
-* Multi citation with post note\ [@lesk:1977; @knuth:1984; @latex:companion, for more]
-* Multi citation with locators and pre/post notes\ [see @lesk:1977, p. 1; @knuth:1984; @latex:companion, chap. 1-2, for more]
+* Multi citation[@lesk:1977; @knuth:1984; @latex:companion]
+* Multi citation with pre note[see @lesk:1977; @knuth:1984; @latex:companion]
+* Multi citation with locators[@lesk:1977, sec. 1; @knuth:1984; @latex:companion, p. 1-3]
+* Multi citation with post note[@lesk:1977; @knuth:1984; @latex:companion, for more]
+* Multi citation with locators and pre/post notes[see @lesk:1977, p. 1; @knuth:1984; @latex:companion, chap. 1-2, for more]
```

### Comparing `shiny_mdc-1.5.0/test/sections/main2.md` & `shiny_mdc-1.5.1/test/sections/main2.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 * @fig:ex2
 * @fig:ex3, @fig:ex3a, @fig:ex3b
 
 <div id="fig:ex3">
 
 ![Figure with 'width=2.5in'](figures/gaussian2d){#fig:ex3a width=2.5in}
 
-![Figure with 'width=3.5in'\ [^f]](figures/anscombe){#fig:ex3b width=3.5in}
+![Figure with 'width=3.5in'[^f]](figures/anscombe){#fig:ex3b width=3.5in}
 
-Sub-figures [^g]
+Sub-figures[^g]
 </div>
 
 [^f]: Footnote in sub-figure caption.
 [^g]: Footnote in figure caption.
 
 
 # Includes {#sec:includes}
```

### Comparing `shiny_mdc-1.5.0/test/utils/commands.md` & `shiny_mdc-1.5.1/test/utils/commands.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.0/PKG-INFO` & `shiny_mdc-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny-mdc
-Version: 1.5.0
+Version: 1.5.1
 Summary: Tool to compile markdown files to tex/pdf using pandoc, latexmk
 Home-page: https://github.com/jayanthkoushik/shinymdc
 License: MIT
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

