# Comparing `tmp/shiny_mdc-1.4.1.tar.gz` & `tmp/shiny_mdc-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiny_mdc-1.4.1.tar", max compression
+gzip compressed data, was "shiny_mdc-1.5.0.tar", max compression
```

## Comparing `shiny_mdc-1.4.1.tar` & `shiny_mdc-1.5.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     3595 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/LICENSE
--rw-r--r--   0        0        0       78 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/README.md
--rw-r--r--   0        0        0     2297 2023-04-19 23:33:53.086398 shiny_mdc-1.4.1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/__init__.py
--rw-r--r--   0        0        0     1061 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/_latexmk.py
--rw-r--r--   0        0        0     1867 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/_liquid.py
--rw-r--r--   0        0        0     4643 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/_pandoc.py
--rw-r--r--   0        0        0     4936 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/_templates.py
--rw-r--r--   0        0        0       64 2023-04-19 23:33:53.090397 shiny_mdc-1.4.1/shinymdc/_version.py
--rw-r--r--   0        0        0      337 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/dynamic/addappendices.tex
--rw-r--r--   0        0        0      853 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/dynamic/authsetup.tex
--rw-r--r--   0        0        0      290 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/dynamic/authsetupshort.tex
--rw-r--r--   0        0        0      572 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/dynamic/dblfloatsetup.tex
--rw-r--r--   0        0        0      482 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/static/bibnonatsetup.tex
--rw-r--r--   0        0        0     2602 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/static/bibsupersetup.tex
--rw-r--r--   0        0        0     3359 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/static/floatsetup.tex
--rw-r--r--   0        0        0    19901 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/static/iccv/bibstyle.bst
--rw-r--r--   0        0        0     9433 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/static/iccv/esopic.sty
--rw-r--r--   0        0        0     3869 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/static/iccv/everyshi.sty
--rw-r--r--   0        0        0     8276 2023-04-19 23:33:29.714182 shiny_mdc-1.4.1/shinymdc/resources/static/iccv/iccv.sty
--rw-r--r--   0        0        0    26973 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/iclr/bibstyle.bst
--rw-r--r--   0        0        0     9153 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/iclr/iclr.sty
--rw-r--r--   0        0        0    12284 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/iclr/mathcommands.tex
--rw-r--r--   0        0        0    27146 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/icml/bibstyle.bst
--rw-r--r--   0        0        0    27887 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/icml/icml.sty
--rw-r--r--   0        0        0      735 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/mathsetup.tex
--rw-r--r--   0        0        0      848 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/miscsetup.tex
--rw-r--r--   0        0        0    11306 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/neurips/neurips.sty
--rw-r--r--   0        0        0      406 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/resources/static/reqsetup.tex
--rw-r--r--   0        0        0    19149 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/shinymdc.py
--rw-r--r--   0        0        0      930 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/basic.tex
--rw-r--r--   0        0        0     1302 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/iccv.tex
--rw-r--r--   0        0        0     1397 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/iclr.tex
--rw-r--r--   0        0        0     2144 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/icml.tex
--rw-r--r--   0        0        0      890 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/neurips.tex
--rw-r--r--   0        0        0     2052 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/spacious.tex
--rw-r--r--   0        0        0      464 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/standalone.tex
--rw-r--r--   0        0        0     2281 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/shinymdc/templates/stylish.tex
--rw-r--r--   0        0        0    15953 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/test/figures/anscombe.pdf
--rw-r--r--   0        0        0    40892 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/test/figures/densities.pdf
--rw-r--r--   0        0        0    10736 2023-04-19 23:33:29.718182 shiny_mdc-1.4.1/test/figures/diamonds.pdf
--rw-r--r--   0        0        0   197017 2023-04-19 23:33:29.722182 shiny_mdc-1.4.1/test/figures/gaussian2d.pdf
--rw-r--r--   0        0        0    28282 2023-04-19 23:33:29.722182 shiny_mdc-1.4.1/test/figures/lines.png
--rw-r--r--   0        0        0     2972 2023-04-19 23:33:29.722182 shiny_mdc-1.4.1/test/main.md
--rwxr-xr-x   0        0        0      315 2023-04-19 23:33:29.722182 shiny_mdc-1.4.1/test/make.sh
--rw-r--r--   0        0        0     1166 2023-04-19 23:33:29.722182 shiny_mdc-1.4.1/test/references.bib
--rw-r--r--   0        0        0   683424 2023-04-19 23:33:29.726182 shiny_mdc-1.4.1/test/samples/basic.pdf
--rw-r--r--   0        0        0   412896 2023-04-19 23:33:29.726182 shiny_mdc-1.4.1/test/samples/iccv.pdf
--rw-r--r--   0        0        0   406337 2023-04-19 23:33:29.730182 shiny_mdc-1.4.1/test/samples/iclr.pdf
--rw-r--r--   0        0        0   446430 2023-04-19 23:33:29.730182 shiny_mdc-1.4.1/test/samples/icml.pdf
--rw-r--r--   0        0        0   450734 2023-04-19 23:33:29.734182 shiny_mdc-1.4.1/test/samples/neurips.pdf
--rw-r--r--   0        0        0   601766 2023-04-19 23:33:29.738182 shiny_mdc-1.4.1/test/samples/spacious.pdf
--rw-r--r--   0        0        0   553251 2023-04-19 23:33:29.738182 shiny_mdc-1.4.1/test/samples/standalone.pdf
--rw-r--r--   0        0        0   424279 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/samples/stylish.pdf
--rw-r--r--   0        0        0     1535 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/sections/appendix1.md
--rw-r--r--   0        0        0     1625 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/sections/appendix2.md
--rw-r--r--   0        0        0        0 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/sections/empty.md
--rw-r--r--   0        0        0     2100 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/sections/main1.md
--rw-r--r--   0        0        0     1353 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/sections/main2.md
--rw-r--r--   0        0        0      992 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/utils/commands.md
--rw-r--r--   0        0        0       41 2023-04-19 23:33:29.742182 shiny_mdc-1.4.1/test/utils/ext.md
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 shiny_mdc-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4775 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/LICENSE
+-rw-r--r--   0        0        0       78 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/README.md
+-rw-r--r--   0        0        0     2297 2023-04-20 03:20:46.755515 shiny_mdc-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/__init__.py
+-rw-r--r--   0        0        0     1061 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/_latexmk.py
+-rw-r--r--   0        0        0     1867 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/_liquid.py
+-rw-r--r--   0        0        0     4643 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/_pandoc.py
+-rw-r--r--   0        0        0     4936 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/_templates.py
+-rw-r--r--   0        0        0       64 2023-04-20 03:20:46.755515 shiny_mdc-1.5.0/shinymdc/_version.py
+-rw-r--r--   0        0        0      410 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/dynamic/addappendices.tex
+-rw-r--r--   0        0        0      881 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/dynamic/authsetup.tex
+-rw-r--r--   0        0        0      317 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/dynamic/authsetupshort.tex
+-rw-r--r--   0        0        0      572 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/dynamic/dblfloatsetup.tex
+-rw-r--r--   0        0        0      482 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/bibnonatsetup.tex
+-rw-r--r--   0        0        0     2475 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/bibsupersetup.tex
+-rw-r--r--   0        0        0     3359 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/floatsetup.tex
+-rw-r--r--   0        0        0    19901 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/iccv/bibstyle.bst
+-rw-r--r--   0        0        0     9433 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/iccv/esopic.sty
+-rw-r--r--   0        0        0     3869 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/iccv/everyshi.sty
+-rw-r--r--   0        0        0     8276 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/iccv/iccv.sty
+-rw-r--r--   0        0        0    26973 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/iclr/bibstyle.bst
+-rw-r--r--   0        0        0     9153 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/iclr/iclr.sty
+-rw-r--r--   0        0        0    12284 2023-04-20 03:20:21.777404 shiny_mdc-1.5.0/shinymdc/resources/static/iclr/mathcommands.tex
+-rw-r--r--   0        0        0    27146 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/resources/static/icml/bibstyle.bst
+-rw-r--r--   0        0        0    27887 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/resources/static/icml/icml.sty
+-rw-r--r--   0        0        0      735 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/resources/static/mathsetup.tex
+-rw-r--r--   0        0        0     1153 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/resources/static/miscsetup.tex
+-rw-r--r--   0        0        0    11306 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/resources/static/neurips/neurips.sty
+-rw-r--r--   0        0        0      406 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/resources/static/reqsetup.tex
+-rw-r--r--   0        0        0    19149 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/shinymdc.py
+-rw-r--r--   0        0        0      945 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/basic.tex
+-rw-r--r--   0        0        0     1302 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/iccv.tex
+-rw-r--r--   0        0        0     1397 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/iclr.tex
+-rw-r--r--   0        0        0     2144 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/icml.tex
+-rw-r--r--   0        0        0      890 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/neurips.tex
+-rw-r--r--   0        0        0     3064 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/spacious.tex
+-rw-r--r--   0        0        0      464 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/standalone.tex
+-rw-r--r--   0        0        0     2281 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/shinymdc/templates/stylish.tex
+-rw-r--r--   0        0        0    15953 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/figures/anscombe.pdf
+-rw-r--r--   0        0        0    40892 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/figures/densities.pdf
+-rw-r--r--   0        0        0    10736 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/figures/diamonds.pdf
+-rw-r--r--   0        0        0   197017 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/figures/gaussian2d.pdf
+-rw-r--r--   0        0        0    28282 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/figures/lines.png
+-rw-r--r--   0        0        0     2973 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/main.md
+-rwxr-xr-x   0        0        0      315 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/make.sh
+-rw-r--r--   0        0        0     1166 2023-04-20 03:20:21.781405 shiny_mdc-1.5.0/test/references.bib
+-rw-r--r--   0        0        0   690444 2023-04-20 03:20:21.785405 shiny_mdc-1.5.0/test/samples/basic.pdf
+-rw-r--r--   0        0        0   413659 2023-04-20 03:20:21.789405 shiny_mdc-1.5.0/test/samples/iccv.pdf
+-rw-r--r--   0        0        0   406993 2023-04-20 03:20:21.789405 shiny_mdc-1.5.0/test/samples/iclr.pdf
+-rw-r--r--   0        0        0   446722 2023-04-20 03:20:21.793406 shiny_mdc-1.5.0/test/samples/icml.pdf
+-rw-r--r--   0        0        0   451263 2023-04-20 03:20:21.797406 shiny_mdc-1.5.0/test/samples/neurips.pdf
+-rw-r--r--   0        0        0   600203 2023-04-20 03:20:21.797406 shiny_mdc-1.5.0/test/samples/spacious.pdf
+-rw-r--r--   0        0        0   554977 2023-04-20 03:20:21.801406 shiny_mdc-1.5.0/test/samples/standalone.pdf
+-rw-r--r--   0        0        0   425121 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/samples/stylish.pdf
+-rw-r--r--   0        0        0     1535 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/sections/appendix1.md
+-rw-r--r--   0        0        0     1626 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/sections/appendix2.md
+-rw-r--r--   0        0        0        0 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/sections/empty.md
+-rw-r--r--   0        0        0     2320 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/sections/main1.md
+-rw-r--r--   0        0        0     1354 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/sections/main2.md
+-rw-r--r--   0        0        0      992 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/utils/commands.md
+-rw-r--r--   0        0        0       41 2023-04-20 03:20:21.805407 shiny_mdc-1.5.0/test/utils/ext.md
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 shiny_mdc-1.5.0/PKG-INFO
```

### Comparing `shiny_mdc-1.4.1/CHANGELOG.md` & `shiny_mdc-1.5.0/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+## [1.5.0](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.4.1...v1.5.0) (2023-04-20)
+
+
+### Features
+
+* add appendix labels to footnotes ([8279712](https://github.com/jayanthkoushik/shiny-mdc/commit/8279712031ef4a36cc22720248a63cb22ffc6103))
+* add space before superscripts in author lists ([b0db384](https://github.com/jayanthkoushik/shiny-mdc/commit/b0db3843ebca5a68428f275517d3fefce280f45f))
+* convert emails into links ([380670c](https://github.com/jayanthkoushik/shiny-mdc/commit/380670c51565789c6ced8c13278cfbd03f79790e))
+* in the stylish template, use lining numbers where appropriate ([8b7c643](https://github.com/jayanthkoushik/shiny-mdc/commit/8b7c64339f9b54ae5a6f4168c8ffa73f2c0b5df8))
+* make spacing for footnotes and superscripts consistent ([921058f](https://github.com/jayanthkoushik/shiny-mdc/commit/921058fb021805ce4da93151831703cfcbc38fda))
+* use `nowidow` for basic/spacious templates ([53fd916](https://github.com/jayanthkoushik/shiny-mdc/commit/53fd9163d8f5f72cd86b311f18d4bdac428a9a9b))
+* use small caps for appendix labels in spacious template ([240fa66](https://github.com/jayanthkoushik/shiny-mdc/commit/240fa66fc1f30ddace242a5261c4811ca9302de5))
+
 ### [1.4.1](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.4.0...v1.4.1) (2023-04-19)
 
 
 ### Bug Fixes
 
 * fix `hidelinks` argument passed to `hyperref` ([5007034](https://github.com/jayanthkoushik/shiny-mdc/commit/500703429ac92f233caf309f1f6b3f22d88c6ef8))
```

### Comparing `shiny_mdc-1.4.1/LICENSE` & `shiny_mdc-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/pyproject.toml` & `shiny_mdc-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shiny-mdc"
-version = "1.4.1"  # managed by `poetry-dynamic-versioning`
+version = "1.5.0"  # managed by `poetry-dynamic-versioning`
 description = "Tool to compile markdown files to tex/pdf using pandoc, latexmk"
 readme = "README.md"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 repository = "https://github.com/jayanthkoushik/shinymdc"
 packages = [
   { include = "shinymdc" }
```

### Comparing `shiny_mdc-1.4.1/shinymdc/_latexmk.py` & `shiny_mdc-1.5.0/shinymdc/_latexmk.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/_liquid.py` & `shiny_mdc-1.5.0/shinymdc/_liquid.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/_pandoc.py` & `shiny_mdc-1.5.0/shinymdc/_pandoc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/_templates.py` & `shiny_mdc-1.5.0/shinymdc/_templates.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/dynamic/authsetup.tex` & `shiny_mdc-1.5.0/shinymdc/resources/dynamic/authsetup.tex`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 \newlength{\maxnamelen}
 \newlength{\maxemlen}
 \newlength{\maxinstlen}
 
 % Use the longest name, email, and institute to get box sizes for the author list.
 \newbox\tempbox
-\savebox{\tempbox}{\hbox{$longest_author_name$\textsuperscript{*}}}
+\savebox{\tempbox}{\hbox{$longest_author_name$~\textsuperscript{*}}}
 \setlength{\maxnamelen}{\wd\tempbox}
 \savebox{\tempbox}{\hbox{\texttt{\textsmaller{$longest_email$}}}}
 \setlength{\maxemlen}{\wd\tempbox}
 \savebox{\tempbox}{\hbox{\textsmaller{$longest_inst_name$}}}
 \setlength{\maxinstlen}{\wd\tempbox}
 
 \author{%
   $for(author)$
-  \makebox[\maxnamelen][c]{$it.name$$if(it.equalcontrib)$$if(skipequal)$$else$\textsuperscript{*}$endif$$endif$}$if(it.institute)$\\%
+  \makebox[\maxnamelen][c]{$it.name$$if(it.equalcontrib)$$if(skipequal)$$else$~\textsuperscript{*}$endif$$endif$}$if(it.institute)$\\%
     $for(it.institute)$\makebox[\maxinstlen]{{\textsmaller{$it$}}}$sep$\\%
     $endfor$$endif$$if(it.email)$\\%
-    \makebox[\maxemlen]{\texttt{\textsmaller{$it.email$}}}$endif$%
+    \makebox[\maxemlen]{\href{mailto:$it.email$}{\texttt{\textsmaller{$it.email$}}}}$endif$%
   $sep$\vspace{1ex}\and%
   $endfor$%
 }
```

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/dynamic/dblfloatsetup.tex` & `shiny_mdc-1.5.0/shinymdc/resources/dynamic/dblfloatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/static/bibsupersetup.tex` & `shiny_mdc-1.5.0/shinymdc/resources/static/bibsupersetup.tex`

 * *Files 8% similar despite different names*

```diff
@@ -5,37 +5,36 @@
 \fi
 \usepackage{xparse}
 \usepackage{letltxmacro}
 % \usepackage{etoolbox}
 
 \LetLtxMacro\oldcitep\citep
 \RenewDocumentCommand\citep{o o m}{%
-  \IfNoValueTF{#1}{%
-    \textsuperscript{\!\mbox{\oldcitep{#3}}}%
-  }{%
-    \IfNoValueTF{#2}{%
-      \textsuperscript{\!\mbox{\oldcitep[#1]{#3}}}%
+  \textsuperscript{%
+    \IfNoValueTF{#1}{%
+      \oldcitep{#3}%
     }{%
-      \textsuperscript{\!\oldcitep[#1][#2]{#3}}%
+      \IfNoValueTF{#2}{%
+        \oldcitep[#1]{#3}%
+      }{%
+        \oldcitep[#1][#2]{#3}%
+      }%
     }%
   }%
 }
 
 % Put year in citet.
 \newcommand*{\nolink}[1]{{\protect\NoHyper#1\protect\endNoHyper}}
 \let\origcitet\citet
 \renewcommand{\citet}[2][]{%
-  % \nolink{\citeauthor{#2} (\citeyear{#2})}~\textsuperscript{\!\mbox{\oldcitep[#1]{#2}}}%
   \nolink{\citeauthor{#2} (\citeyear{#2})}~\citep[#1]{#2}%
 }
 
 \let\origcitetext\citetext
-\renewcommand{\citetext}[1]{%
-  \textsuperscript{\origcitetext{#1}}%
-}
+\renewcommand{\citetext}[1]{\textsuperscript{\origcitetext{#1}}}
 
 % \newtoggle{HasArgOne}
 % \newtoggle{HasArgTwo}
 % \LetLtxMacro\oldcitep\citep
 % \RenewDocumentCommand\citep{o o m}{%
 %   % First, check if the two optional arguments have values.
 %   % This involves checking for presence, as well as checking
```

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/static/floatsetup.tex` & `shiny_mdc-1.5.0/shinymdc/resources/static/floatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/static/iccv/bibstyle.bst` & `shiny_mdc-1.5.0/shinymdc/resources/static/iccv/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/static/iccv/esopic.sty` & `shiny_mdc-1.5.0/shinymdc/resources/static/iccv/esopic.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/static/iccv/everyshi.sty` & `shiny_mdc-1.5.0/shinymdc/resources/static/iccv/everyshi.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/static/iccv/iccv.sty` & `shiny_mdc-1.5.0/shinymdc/resources/static/iccv/iccv.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/static/iclr/bibstyle.bst` & `shiny_mdc-1.5.0/shinymdc/resources/static/iclr/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/static/iclr/iclr.sty` & `shiny_mdc-1.5.0/shinymdc/resources/static/iclr/iclr.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/static/iclr/mathcommands.tex` & `shiny_mdc-1.5.0/shinymdc/resources/static/iclr/mathcommands.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/static/icml/bibstyle.bst` & `shiny_mdc-1.5.0/shinymdc/resources/static/icml/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/static/icml/icml.sty` & `shiny_mdc-1.5.0/shinymdc/resources/static/icml/icml.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/static/mathsetup.tex` & `shiny_mdc-1.5.0/shinymdc/resources/static/mathsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/static/miscsetup.tex` & `shiny_mdc-1.5.0/shinymdc/resources/static/miscsetup.tex`

 * *Files 25% similar despite different names*

```diff
@@ -6,29 +6,41 @@
 \usepackage{footnote}
 \usepackage{acronym}
 \usepackage{relsize}
 \usepackage{xcolor}
 \usepackage{tikz}
 \usepackage{fancyvrb}
 \usepackage{pgf}
+\usepackage{nowidow}
 
 % Handle footnotes inside tables, figures.
 \makesavenoteenv{table}
 \makesavenoteenv{table*}
 \makesavenoteenv{figure}
 \makesavenoteenv{figure*}
 
 % Add small space after footnote label.
-\renewcommand{\thefootnote}{\arabic{footnote}\,}
+\makeatletter
+\renewcommand\@makefntext[1]{%
+  \parindent 1em%
+  \noindent
+  \hb@xt@1.8em{\hss\@makefnmark}\,#1}
+\makeatother
 
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
+
+% Reduce space before superscripts and footnotes.
+\let\origts\textsuperscript
+\renewcommand{\textsuperscript}[1]{{\!\origts{#1}}}
+\let\origfootnote\footnote
+\renewcommand{\footnote}[1]{\!\origfootnote{#1}}
```

### Comparing `shiny_mdc-1.4.1/shinymdc/resources/static/neurips/neurips.sty` & `shiny_mdc-1.5.0/shinymdc/resources/static/neurips/neurips.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/shinymdc.py` & `shiny_mdc-1.5.0/shinymdc/shinymdc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/templates/basic.tex` & `shiny_mdc-1.5.0/shinymdc/templates/basic.tex`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 $for(includes)$
 $it$
 $endfor$
 
 \begin{document}
 
+\setnowidow[2]
 \maketitle
 
 % Add equal-contrib footnote.
 $if(skipequal)$
 $else$
 \blfootnote{\textsuperscript{*}\,Equal contribution.}
 $endif$
```

### Comparing `shiny_mdc-1.4.1/shinymdc/templates/iccv.tex` & `shiny_mdc-1.5.0/shinymdc/templates/iccv.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/templates/iclr.tex` & `shiny_mdc-1.5.0/shinymdc/templates/iclr.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/templates/icml.tex` & `shiny_mdc-1.5.0/shinymdc/templates/icml.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/templates/neurips.tex` & `shiny_mdc-1.5.0/shinymdc/templates/neurips.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/shinymdc/templates/spacious.tex` & `shiny_mdc-1.5.0/shinymdc/templates/stylish.tex`

 * *Files 19% similar despite different names*

```diff
@@ -1,110 +1,123 @@
 \PassOptionsToPackage{hidelinks}{hyperref}
 
 \documentclass[%
   letterpaper,%
-  12pt,%
+  twocolumn,%
   $if(lang)$$lang$$else$english$endif$%
 ]{article}
 
-\usepackage[textwidth=360pt,textheight=600pt,footnotesep=60pt]{geometry}
-\usepackage[rm,up,big,raggedright]{titlesec}
+\usepackage[%
+  textwidth=492pt,%
+  textheight=624pt,%
+  columnsep=12pt,%
+  footskip=50pt,%
+  footnotesep=50pt%
+]{geometry}
+\usepackage[sf,big,raggedright,compact]{titlesec}
 \usepackage{fancyhdr}
-\usepackage{cfr-lm}
-% \usepackage{ebgaramond}
+\usepackage{newtxtext}
+\usepackage{etoolbox}
 
+\def\nobibcompress{TRUE}
 \input{$reqsetup$}
 \input{$floatsetup$}
+\input{$dblfloatsetup$}
 \input{$mathsetup$}
 \input{$bibsupersetup$}
 \input{$miscsetup$}
 
-% Increase maximum figure/table sizes.
-\renewcommand{\maxfigwidth}{6.5in}
-\renewcommand{\maxfigheight}{10in}
-\renewcommand{\maxtabwidth}{6.5in}
-\renewcommand{\maxtabheight}{10in}
-
-% Configure paragraph title font.
-\titleformat*{\paragraph}{\itshape}
+$if(smalltabs)$
+% Use small font for tables.
+\AtBeginEnvironment{tabular}{\smaller}
+$else$
+$endif$
 
 % Configure caption font.
-\captionsetup{justification=raggedright,font={small}}
+\captionsetup{justification=raggedright,font={sf,small}}
 
 % Add periods after section numbers.
 \titlelabel{\thetitle.\enskip}
 
 % Configure page no.
 \pagestyle{fancy}
 \fancyhf{}
-\fancyhead[R]{{\normalfont\footnotesize\thepage}}
+\renewcommand{\headrulewidth}{0pt}
+\fancyfoot[R]{{\normalfont\sffamily\scriptsize\thepage}}
 
 % Configure title format.
 \makeatletter
 \def\@maketitle{%
   \newpage
-  \vskip 3ex%
   \begin{flushleft}%
-    \normalfont%
-    {\Huge \@title \par}%
-    \vskip 3ex%
+    \normalfont\sffamily%
+    {\LARGE \@title \par}%
+    \vskip 1.5em%
     {\large
-      \lineskip 2ex%
-      \@author
-      \par}%
+      \lineskip .5em%
+      \begin{tabular}[t]{@{}l@{}}%
+          \@author
+      \end{tabular}\par}%
     {\normalsize \@date}%
   \end{flushleft}%
-  \par}
+  \par
+  \vskip 1.5em}
 \makeatother
 
-% Change '\and' to add vertical space.
+% Change '\and' to left align contents.
 \makeatletter
-\def\and{\vskip 2ex}
+\def\and{%
+  \end{tabular}%
+  \hskip 1em \@plus.17fil%
+  \begin{tabular}[t]{@{}l@{}}}%
 \makeatother
 
 \title{$title$}
-\date{$if(date)$\vspace*{3ex}$date$$endif$}
+\date{$if(date)$\vspace*{1em} $date$$endif$}
 
 \input{$authsetupshort$}
 
 $for(includes)$
 $it$
 $endfor$
 
 \begin{document}
 
 \maketitle
 
-\thispagestyle{empty}
-\parindent=3em
+\thispagestyle{fancy}
+\parindent=2em
 
 % Add author-info footnote.
 \blfootnote{%
   {%
-    \normalfont\scriptsize\raggedright%
+    \normalfont\sffamily\scriptsize%
     $if(skipequal)$$else$\mbox{\textsuperscript{*}\,Equal contribution.}\enskip$endif$%
     $for(institute)$\mbox{\textsuperscript{$institute.id$}\,$institute.name$.}\enskip$endfor$%
   }%
 }
 
 $if(abstract)$
-\section*{Abstract}
-$abstract$
+\hrule height 1pt
+\vspace{1ex}%
+{\parindent=0pt \normalfont\sffamily\normalsize $abstract$}
+\vspace{1ex}%
+\hrule height 1pt
+\vspace{1ex}
 $endif$
 
 $if(body)$
 $body$
 $endif$
 
 $for(sections)$
 $it$
 $endfor$
 
 $if(bibliography)$
-\clearpage
 \footnotesize
 \bibliographystyle{unsrtnat}
 \bibliography{$bibliography$}
 \normalsize
 $endif$
 
 \input{$addappendices$}
```

### Comparing `shiny_mdc-1.4.1/shinymdc/templates/stylish.tex` & `shiny_mdc-1.5.0/shinymdc/templates/spacious.tex`

 * *Files 25% similar despite different names*

```diff
@@ -1,125 +1,143 @@
 \PassOptionsToPackage{hidelinks}{hyperref}
 
 \documentclass[%
   letterpaper,%
-  twocolumn,%
+  12pt,%
   $if(lang)$$lang$$else$english$endif$%
 ]{article}
 
-\usepackage[%
-  textwidth=492pt,%
-  textheight=624pt,%
-  columnsep=12pt,%
-  footskip=50pt,%
-  footnotesep=50pt%
-]{geometry}
-\usepackage[sf,big,raggedright,compact]{titlesec}
+\usepackage[textwidth=360pt,textheight=600pt,footnotesep=60pt]{geometry}
+\usepackage[rm,up,big,raggedright]{titlesec}
 \usepackage{fancyhdr}
-\usepackage{newtxtext}
-\usepackage{etoolbox}
+\usepackage{cfr-lm}
+% \usepackage{ebgaramond}
 
-\def\nobibcompress{TRUE}
 \input{$reqsetup$}
 \input{$floatsetup$}
-\input{$dblfloatsetup$}
 \input{$mathsetup$}
 \input{$bibsupersetup$}
 \input{$miscsetup$}
 
-$if(smalltabs)$
-% Use small font for tables.
-\AtBeginEnvironment{tabular}{\smaller}
-$else$
-$endif$
+% Increase maximum figure/table sizes.
+\renewcommand{\maxfigwidth}{6.5in}
+\renewcommand{\maxfigheight}{10in}
+\renewcommand{\maxtabwidth}{6.5in}
+\renewcommand{\maxtabheight}{10in}
+
+% Use proportional, lining digits for footnotes and superscripts.
+\makeatletter
+\renewcommand{\@makefnmark}{\hbox{\@textsuperscript{\normalfont\plstyle\@thefnmark}}}
+\makeatother
+\let\oldts\textsuperscript
+\renewcommand{\textsuperscript}[1]{\oldts{\textpl{#1}}}
+
+% Use proportional, lining digits for bibliography labels.
+\renewcommand{\bibnumfmt}[1]{[\textpl{#1}]}
+
+% Use tabular, lining digits in tables.
+\AtBeginEnvironment{tabular}{\tlstyle}
+
+% Configure paragraph title font.
+\titleformat*{\paragraph}{\itshape}
 
 % Configure caption font.
-\captionsetup{justification=raggedright,font={sf,small}}
+\captionsetup{justification=raggedright,font={small}}
 
 % Add periods after section numbers.
 \titlelabel{\thetitle.\enskip}
 
 % Configure page no.
 \pagestyle{fancy}
 \fancyhf{}
-\renewcommand{\headrulewidth}{0pt}
-\fancyfoot[R]{{\normalfont\sffamily\scriptsize\thepage}}
+\fancyhead[R]{{\normalfont\footnotesize\thepage}}
 
 % Configure title format.
 \makeatletter
 \def\@maketitle{%
   \newpage
+  \vskip 3ex%
   \begin{flushleft}%
-    \normalfont\sffamily%
-    {\LARGE \@title \par}%
-    \vskip 1.5em%
+    \normalfont%
+    {\Huge \@title \par}%
+    \vskip 3ex%
     {\large
-      \lineskip .5em%
-      \begin{tabular}[t]{@{}l@{}}%
-          \@author
-      \end{tabular}\par}%
+      \lineskip 2ex%
+      \@author
+      \par}%
     {\normalsize \@date}%
   \end{flushleft}%
-  \par
-  \vskip 1.5em}
+  \par}
 \makeatother
 
-% Change '\and' to left align contents.
+% Change '\and' to add vertical space.
 \makeatletter
-\def\and{%
-  \end{tabular}%
-  \hskip 1em \@plus.17fil%
-  \begin{tabular}[t]{@{}l@{}}}%
+\def\and{\vskip 2ex}
 \makeatother
 
 \title{$title$}
-\date{$if(date)$\vspace*{1em} $date$$endif$}
+\date{$if(date)$\vspace*{3ex}$date$$endif$}
 
 \input{$authsetupshort$}
 
 $for(includes)$
 $it$
 $endfor$
 
 \begin{document}
 
+\setnowidow[2]
 \maketitle
 
-\thispagestyle{fancy}
-\parindent=2em
+\thispagestyle{empty}
+\parindent=3em
 
 % Add author-info footnote.
 \blfootnote{%
   {%
-    \normalfont\sffamily\scriptsize%
+    \normalfont\scriptsize\raggedright%
     $if(skipequal)$$else$\mbox{\textsuperscript{*}\,Equal contribution.}\enskip$endif$%
     $for(institute)$\mbox{\textsuperscript{$institute.id$}\,$institute.name$.}\enskip$endfor$%
   }%
 }
 
 $if(abstract)$
-\hrule height 1pt
-\vspace{1ex}%
-{\parindent=0pt \normalfont\sffamily\normalsize $abstract$}
-\vspace{1ex}%
-\hrule height 1pt
-\vspace{1ex}
+\section*{Abstract}
+$abstract$
 $endif$
 
 $if(body)$
 $body$
 $endif$
 
 $for(sections)$
 $it$
 $endfor$
 
 $if(bibliography)$
+\clearpage
 \footnotesize
 \bibliographystyle{unsrtnat}
 \bibliography{$bibliography$}
 \normalsize
 $endif$
 
-\input{$addappendices$}
+$if(appendices)$
+$for(appendices/pairs)$
+\clearpage
+\begin{appendices}
+  \renewcommand{\thesection}{\textsmaller{\textsc{$it.key/alpha/uppercase$}}\arabic{section}}
+  \renewcommand{\thefigure}{\textsmaller{\textsc{$it.key/alpha/uppercase$}}\arabic{figure}}
+  \renewcommand{\thetable}{\textsmaller{\textsc{$it.key/alpha/uppercase$}}\arabic{table}}
+  \renewcommand{\thefootnote}{\textsmaller{\textsc{$it.key/alpha/uppercase$}}\arabic{footnote}}
+  \setcounter{table}{0}
+  \setcounter{figure}{0}
+  \setcounter{footnote}{0}
+  $it.value$
+\end{appendices}
+$sep$
+
+$endfor$
+$endif$
+
 
 \end{document}
```

### Comparing `shiny_mdc-1.4.1/test/figures/anscombe.pdf` & `shiny_mdc-1.5.0/test/figures/anscombe.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/test/figures/densities.pdf` & `shiny_mdc-1.5.0/test/figures/densities.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/test/figures/diamonds.pdf` & `shiny_mdc-1.5.0/test/figures/diamonds.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/test/figures/gaussian2d.pdf` & `shiny_mdc-1.5.0/test/figures/gaussian2d.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/test/figures/lines.png` & `shiny_mdc-1.5.0/test/figures/lines.png`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/test/main.md` & `shiny_mdc-1.5.0/test/main.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   affiliation:
   - 2
 institute:
 - id: 1
   name: Institute One
 - id: 2
   name: Institute Two at City, State
-abstract: _Markdown_ **in** **_abstract_**. $x+2$. @sec:ex1. Reference [@texbook].
+abstract: _Markdown_ **in** **_abstract_**. $x+2$. @sec:ex1. Reference\ [@texbook].
 bibliography: references.bib
 sections:
 - sections/main1.md
 - sections/main2.md
 - sections/empty.md
 appendices:
 - sections/appendix1.md
```

### Comparing `shiny_mdc-1.4.1/test/references.bib` & `shiny_mdc-1.5.0/test/references.bib`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/test/samples/basic.pdf` & `shiny_mdc-1.5.0/test/samples/basic.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 11% similar despite different names*

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
 author4@author4.com
 
 Author Number Five
 Institute Two at City, State
 authornumberfive@institutetwo.edu
@@ -160,48 +160,52 @@
 a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
 R∞
 2
 • Inline: 0 exp−x dx
 • Block: Equation 1, Equation 2
 • Commands defined in body (P[x in X]): P[x ∈ X ]
 • Aligned:
+
+(2)
+
 x=1
 x + y = 10
 x + y + z = 100
 
 6
 
 Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
-• Pointer to footnote 1
+• Pointer to footnote 1 2 text
 
 7
 
 Citations
 • Short citation [2]
 • Short citation with pre note [see 2]
 • Short citation with locator [2, p. 1]
 • Short citation with post note [2, for more]
 • Short citation with locators and pre/post notes [see 2, chap. 1-4, for more]
 • Long citation: Lesk and Kernighan (1977) [3]
 • Long citation with locator: Lesk and Kernighan (1977) [3, chap. 1]
 • Long citation with note: Lesk and Kernighan (1977) [3, for more]
-• Multi citation [2–4]
-• Multi citation with pre note [see 2–4]
 1 Example footnote text.
+2 Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum, at tempor nisl. Vivamus vitae
 
-3
+pulvinar leo, at pharetra massa. Ut lobortis odio non nulla tincidunt pulvinar.
 
-(2)
+3
 
-• Multi citation with locators [3, sec. 1; 4; 2, p. 1-3]
+• Multi citation [2–4]
+• Multi citation with pre note [see 2–4]
+• Multi citation with locators [3, sec. 1; 4; 2, p. 1-3]
 • Multi citation with post note [2–4, for more]
 • Multi citation with locators and pre/post notes [see 3, p. 1; 4; 2, chap. 1-2, for more]
 
 8
 
 Tables
 • Table 1
@@ -315,17 +319,16 @@
 10
 
 Includes
 
 • Commands from metadata include: arg min R
 • Include command in body (there should be text after this):
 Content added through include statement.
-
-2 Footnote in sub-figure caption.
-3 Footnote in figure caption.
+3 Footnote in sub-figure caption.
+4 Footnote in figure caption.
 
 4
 
 Figure 2: Narrow figure
 
 A
 B
@@ -393,19 +396,19 @@
 
 15
 
 5
 
 10
 
-(b) Figure with ‘width=3.5in’ 2
+(b) Figure with ‘width=3.5in’ 3
 
 (a) Figure with ‘width=2.5in’
 
-Figure 4: Sub-figures 3
+Figure 4: Sub-figures 4
 
 6
 
 x
 
 15
 
@@ -617,15 +620,15 @@
 
 1234
 567
 89
 
 444
 44
-42
+4 B2
 
 a
 aa
 aaa
 
 bbb
 bb
@@ -659,15 +662,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1: Extra wide table 3
+Table B1: Extra wide table B3
 
 Appendix B
 
 Appendix 2
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi purus, bibendum
 non neque sed, lacinia tristique tortor. Vestibulum eu lectus sed velit luctus varius. Sed
@@ -698,16 +701,16 @@
 0
 
 • Equation 3
 • Equation 4
 • Block without tag:
 x + y + z = 100
 
-1 Footnote in table.
-2 Footnote in table.
-3 Footnote in table caption.
+B1 Footnote in table.
+B2 Footnote in table.
+B3 Footnote in table caption.
 
 11
 
 (4)
```

### Comparing `shiny_mdc-1.4.1/test/samples/iccv.pdf` & `shiny_mdc-1.5.0/test/samples/iccv.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -133,15 +133,15 @@
 • Math: 0123456789
 
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
-• Pointer to footnote ¹
+• Pointer to footnote¹² text
 
 7. Citations
 • Short citation [4]
 • Short citation with pre note [4]
 • Short citation with locator [4, p. 1]
 • Short citation with post note [4, for more]
 • Short citation with locators and pre/post notes [4,
@@ -224,16 +224,19 @@
 • Commands defined in body (P[x in X]): P[x ∈ X ]
 • Aligned:
 x=1
 x + y = 10
 x + y + z = 100
 
 ¹ Example footnote text.
-² Footnote in sub-figure caption.
-³ Footnote in figure caption.
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
@@ -294,17 +297,17 @@
 
 x
 
 15
 
 5
 
-(b) Figure with ‘width=3.5in’ ²
+(b) Figure with ‘width=3.5in’³
 
-Figure 4: Sub-figures ³
+Figure 4: Sub-figures⁴
 
 10
 
 x
 
 15
 
@@ -583,15 +586,15 @@
 
 1234
 567
 89
 
 444
 44
-4²
+4ᴮ²
 
 a
 aa
 aaa
 
 bbb
 bb
@@ -625,15 +628,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1: Extra wide table ³
+Table B1: Extra wide tableᴮ³
 
 Appendix B. Appendix 2
 Lorem ipsum dolor sit amet, consectetur adipiscing elit.
 Aliquam nisi purus, bibendum non neque sed, lacinia tristique
 tortor. Vestibulum eu lectus sed velit luctus varius. Sed
 sollicitudin ligula ante. Integer porta a erat commodo
 dignissim. Duis et lectus diam. Nulla id erat vestibulum
@@ -655,15 +658,15 @@
 0
 
 • Equation 3
 • Equation 4
 • Block without tag:
 x + y + z = 100
 
-¹ Footnote in table.
-² Footnote in table.
-³ Footnote in table caption.
+ᴮ¹ Footnote in table.
+ᴮ² Footnote in table.
+ᴮ³ Footnote in table caption.
 
 (3)
 (4)
```

### Comparing `shiny_mdc-1.4.1/test/samples/iclr.pdf` & `shiny_mdc-1.5.0/test/samples/iclr.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 4% similar despite different names*

#### pdftotext {} -

```diff
@@ -149,36 +149,36 @@
 0
 
 2
 
 (1)
 
 a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
+
+(2)
+
 R∞
 2
 • Inline: 0 exp−x dx
 • Block: Equation 1, Equation 2
 • Commands defined in body (P[x in X]): P[x ∈ X ]
 • Aligned:
-
-(2)
-
 x=1
 x + y = 10
 x + y + z = 100
 
 6
 
 Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
-• Pointer to footnote ¹
+• Pointer to footnote¹² text
 
 7
 
 Citations
 • Short citation (Mittelbach et al., 2004)
 • Short citation with pre note (see Mittelbach et al., 2004)
 • Short citation with locator (Mittelbach et al., 2004, p. 1)
@@ -205,17 +205,18 @@
 • Table 2
 
 9
 
 Figures
 • Figure 2
 • Figure 3
-• Figure 4, Figure 4a, Figure 4b
+
 ¹ Example footnote text.
-² Footnote in sub-figure caption.
+² Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum, at tempor nisl. Vivamus vitae
+pulvinar leo, at pharetra massa. Ut lobortis odio non nulla tincidunt pulvinar.
 
 3
 
 Col1
 
 Col2
 
@@ -308,32 +309,31 @@
 4
 
 5
 
 6
 
 Table 2: Wide table
+• Figure 4, Figure 4a, Figure 4b
 
 10
 
 Includes
 • Commands from metadata include: arg min R
 • Include command in body (there should be text after this):
 
 Content added through include statement.
 
 References
 Donald E. Knuth. Literate programming. The Computer Journal, 27(2):97–111, 1984.
 Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
-Michael Lesk and Brian Kernighan. Computer typesetting of technical journals on UNIX. In
-Proceedings of American Federation of Information Processing Societies: 1977 National Computer
-Conference, pp. 879–888, Dallas, Texas, 1977.
 
 Figure 2: Narrow figure
-³ Footnote in figure caption.
+³ Footnote in sub-figure caption.
+⁴ Footnote in figure caption.
 
 4
 
 A
 B
 C
 D
@@ -359,14 +359,17 @@
 72
 
 74
 
 76
 
 Figure 3: Wide figure
+Michael Lesk and Brian Kernighan. Computer typesetting of technical journals on UNIX. In
+Proceedings of American Federation of Information Processing Societies: 1977 National Computer
+Conference, pp. 879–888, Dallas, Texas, 1977.
 Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle, and Chris Rowley. The LATEX
 Companion. Addison-Wesley Professional, 2 edition, 2004.
 
 5
 
 (a) Figure with ‘width=2.5in’
 
@@ -401,17 +404,17 @@
 
 x
 
 15
 
 5
 
-(b) Figure with ‘width=3.5in’ ²
+(b) Figure with ‘width=3.5in’³
 
-Figure 4: Sub-figures ³
+Figure 4: Sub-figures⁴
 
 6
 
 10
 
 x
 
@@ -606,15 +609,15 @@
 
 1234
 567
 89
 
 444
 44
-4²
+4ᴮ²
 
 a
 aa
 aaa
 
 bbb
 bb
@@ -648,15 +651,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1: Extra wide table ³
+Table B1: Extra wide tableᴮ³
 
 Appendix B
 
 Appendix 2
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi purus, bibendum non neque
 sed, lacinia tristique tortor. Vestibulum eu lectus sed velit luctus varius. Sed sollicitudin ligula ante.
@@ -685,16 +688,16 @@
 0
 
 • Equation 3
 • Equation 4
 • Block without tag:
 x + y + z = 100
 
-¹ Footnote in table.
-² Footnote in table.
-³ Footnote in table caption.
+ᴮ¹ Footnote in table.
+ᴮ² Footnote in table.
+ᴮ³ Footnote in table caption.
 
 10
 
 (4)
```

### Comparing `shiny_mdc-1.4.1/test/samples/icml.pdf` & `shiny_mdc-1.5.0/test/samples/icml.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,10 +1,10 @@
 shinymdc-test
 
-Author One * 1 Author MiddleName Two * 1 2 Author * Author Four Author Number Five 2
+Author One*1 Author MiddleName Two*12 Author* Author Four Author Number Five2
 
 Abstract
 Markdown in abstract. x + 2.
 Reference (Knuth, 1986).
 
 1.1. Subsection 1
 Section 1.
@@ -134,19 +134,17 @@
 5. Math
 Z ∞
 
 2
 
 exp−x dx
 
-0
-
 (1)
 
-• Pointer to footnote 1
+• Pointer to footnote 1 2 text
 
 7. Citations
 • Short citation (Mittelbach et al., 2004)
 • Short citation with pre note (see Mittelbach et al., 2004)
 • Short citation with locator (Mittelbach et al., 2004,
 p. 1)
 • Short citation with post note (Mittelbach et al., 2004,
@@ -167,45 +165,35 @@
 • Multi citation with post note (Lesk & Kernighan, 1977;
 Knuth, 1984; Mittelbach et al., 2004, for more)
 • Multi citation with locators and pre/post notes (see
 Lesk & Kernighan, 1977, p. 1; Knuth, 1984; Mittelbach
 et al., 2004, chap. 1-2, for more)
 
 8. Tables
+
+0
+
 • Table 1
 • Table 2
-
 a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
 (2)
 Col1 Col2
-1
-11
-111
-
 R∞
+−x2
+• Inline: 0 exp
+dx
+1
 2
-• Inline: 0 exp−x dx
 • Block: Equation 1, Equation 2
-• Commands defined in body (P[x in X]): P[x ∈ X ]
-• Aligned:
-
-x=1
-x + y = 10
-x + y + z = 100
-
-6. Links
-• Section: Section 1, Section 1.2
-• Appendix section: Section B, Section A.1.1
-• Appendix figure: Figure A1
-• Appendix table: Table B1
-• Appendix math: Equation 4
-
-2
+11
 22
+• Commands defined in body (P[x in X]): P[x ∈ X ]
+111
 222
+• Aligned:
 
 Col3
 
 Col4
 
 3
 33
@@ -213,101 +201,35 @@
 
 4
 44
 444
 
 Table 1. Short table
 
+x=1
+x + y = 10
+x + y + z = 100
+
 9. Figures
 • Figure 2
-• Figure 3
-• Figure 4, Figure 4a, Figure 4b
+
+6. Links
+• Section: Section 1, Section 1.2
+• Appendix section: Section B, Section A.1.1
+• Appendix figure: Figure A1
+• Appendix table: Table B1
+• Appendix math: Equation 4
 
 1
-2
 
 Example footnote text.
-Footnote in sub-figure caption.
-
-A
-B
-C
-D
-E
-F
-G
-H
-I
-J
-
-62
-
-64
-
-66
-
-68
-
-x
-
-70
-
-72
-
-74
-
-76
-
-Figure 3. Wide figure
-
-dataset = I
-
-dataset = II
-
-dataset = III
-
-dataset = IV
-
-12
-
-y
-
-10
-8
-6
-4
-
-12
-
-y
-
-10
-8
-6
-4
-5
-(a) Figure with ‘width=2.5in’
-
-10
-
-x
-
-15
-
-5
-
-(b) Figure with ‘width=3.5in’ 2
-
-Figure 4. Sub-figures 4
-
-10
-
-x
-
-15
+Integer at enim eu tellus malesuada scelerisque. Ut sed
+rhoncus ipsum, at tempor nisl. Vivamus vitae pulvinar leo, at
+pharetra massa. Ut lobortis odio non nulla tincidunt pulvinar.
+2
 
 Col1
 
 Col2
 
 Col3
 
@@ -374,27 +296,109 @@
 
 5
 
 6
 
 Table 2. Wide table
 
+A
+B
+C
+D
+E
+F
+G
+H
+I
+J
+
+62
+
+64
+
+66
+
+68
+
+x
+
+70
+
+72
+
+74
+
+76
+
+Figure 3. Wide figure
+
+• Figure 3
+• Figure 4, Figure 4a, Figure 4b
+
 10. Includes
 • Commands from metadata include: arg min R
 • Include command in body (there should be text after
 this):
 Content added through include statement.
 
 Figure 2. Narrow figure
 
 3
-4
 
+Footnote in sub-figure caption.
 Footnote in figure caption.
+5
 Footnote in figure caption.
+4
+
+dataset = I
+
+dataset = II
+
+dataset = III
+
+dataset = IV
+
+12
+
+y
+
+10
+8
+6
+4
+
+12
+
+y
+
+10
+8
+6
+4
+5
+(a) Figure with ‘width=2.5in’
+
+10
+
+x
+
+15
+
+5
+
+(b) Figure with ‘width=3.5in’ 3
+
+Figure 4. Sub-figures 5
+
+10
+
+x
+
+15
 
 References
 Knuth, D. E. Literate programming. The Computer Journal,
 27(2):97–111, 1984.
 Knuth, D. E. The TEX Book. Addison-Wesley Professional,
 1986.
 Lesk, M. and Kernighan, B. Computer typesetting of
@@ -581,15 +585,15 @@
 
 1234
 567
 89
 
 444
 44
-42
+4 B2
 
 a
 aa
 aaa
 
 bbb
 bb
@@ -623,15 +627,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1. Extra wide table 4
+Table B1. Extra wide table B4
 
 B. Appendix 2
 Lorem ipsum dolor sit amet, consectetur adipiscing elit.
 Aliquam nisi purus, bibendum non neque sed, lacinia
 tristique tortor. Vestibulum eu lectus sed velit luctus varius.
 Sed sollicitudin ligula ante. Integer porta a erat commodo
 dignissim. Duis et lectus diam. Nulla id erat vestibulum nisi
@@ -654,22 +658,22 @@
 
 • Equation 3
 • Equation 4
 • Block without tag:
 
 x + y + z = 100
 
-1
+B1
 
 Footnote in table.
 Footnote in table.
-3
+B3
 Footnote in table caption.
-4
+B4
 Footnote in table caption.
-2
+B2
 
 (3)
 
 (4)
```

### Comparing `shiny_mdc-1.4.1/test/samples/neurips.pdf` & `shiny_mdc-1.5.0/test/samples/neurips.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 5% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,21 +1,21 @@
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
 author4@author4.com
 
 Author Number Five
 Institute Two at City, State
 authornumberfive@institutetwo.edu
@@ -155,27 +155,30 @@
 a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
 R∞
 2
 • Inline: 0 exp−x dx
 • Block: Equation 1, Equation 2
 • Commands defined in body (P[x in X]): P[x ∈ X ]
 • Aligned:
+
+(2)
+
 x=1
 x + y = 10
 x + y + z = 100
 
 6
 
 Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
-• Pointer to footnote 1
+• Pointer to footnote 1 2 text
 
 7
 
 Citations
 • Short citation [2]
 • Short citation with pre note [see 2]
 • Short citation with locator [2, p. 1]
@@ -201,23 +204,22 @@
 Figures
 • Figure 2
 • Figure 3
 • Figure 4, Figure 4a, Figure 4b
 1
 
 Example footnote text.
-Footnote in sub-figure caption.
+Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum, at tempor nisl. Vivamus vitae
+pulvinar leo, at pharetra massa. Ut lobortis odio non nulla tincidunt pulvinar.
 3
-Footnote in figure caption.
+Footnote in sub-figure caption.
 2
 
 3
 
-(2)
-
 Col1
 1
 11
 111
 
 10
 
@@ -309,14 +311,19 @@
 Includes
 • Commands from metadata include: arg min R
 • Include command in body (there should be text after this):
 
 Content added through include statement.
 
 Figure 2: Narrow figure
+
+4
+
+Footnote in figure caption.
+
 4
 
 A
 B
 C
 D
 E
@@ -381,17 +388,17 @@
 
 x
 
 15
 
 5
 
-(b) Figure with ‘width=3.5in’ 2
+(b) Figure with ‘width=3.5in’ 3
 
-Figure 4: Sub-figures 3
+Figure 4: Sub-figures 4
 
 6
 
 10
 
 x
 
@@ -597,15 +604,15 @@
 
 1234
 567
 89
 
 444
 44
-42
+4 B2
 
 a
 aa
 aaa
 
 bbb
 bb
@@ -639,15 +646,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1: Extra wide table 3
+Table B1: Extra wide table B3
 
 Appendix B
 
 Appendix 2
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi purus, bibendum non neque
 sed, lacinia tristique tortor. Vestibulum eu lectus sed velit luctus varius. Sed sollicitudin ligula ante.
@@ -676,20 +683,20 @@
 0
 
 • Equation 3
 • Equation 4
 • Block without tag:
 x + y + z = 100
 
-1
+B1
 
 Footnote in table.
 Footnote in table.
-3
+B3
 Footnote in table caption.
-2
+B2
 
 11
 
 (4)
```

### Comparing `shiny_mdc-1.4.1/test/samples/spacious.pdf` & `shiny_mdc-1.5.0/test/samples/spacious.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 15% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,19 +1,19 @@
 shinymdc-test
-Author One1,*
+Author One 1,*
 author1@institute1.edu
 
-Author MiddleName Two1,2,*
+Author MiddleName Two 1,2,*
 authortwo@institute1.edu
 
-Author*
+Author *
 Author Four
 author4@author4.com
 
-Author Number Five2
+Author Number Five 2
 authornumberfive@institutetwo.edu
 
 Abstract
 Markdown in abstract. x + 2. Section 1. Reference [1] .
 
 1. Section
 Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum,
@@ -146,19 +146,19 @@
 
 x=1
 x + y = 10
 x + y + z = 100
 
 6. Links
 • Section: Section 1, Section 1.2
-• Appendix section: Section B, Section A.1.1
-• Appendix figure: Figure A1
-• Appendix table: Table B1
+• Appendix section: Section B 2, Section A 1.1.1
+• Appendix figure: Figure A 1
+• Appendix table: Table B 1
 • Appendix math: Equation 4
-• Pointer to footnote 1
+• Pointer to footnote 1 2 text
 
 7. Citations
 • Short citation [2]
 • Short citation with pre note [see 2]
 • Short citation with locator [2, p. 1]
 • Short citation with post note [2, for more]
 • Short citation with locators and pre/post notes [see 2, chap. 1-4, for more]
@@ -167,29 +167,35 @@
 • Long citation with note: Lesk and Kernighan (1977) [3, for more]
 • Multi citation [2–4]
 • Multi citation with pre note [see 2–4]
 • Multi citation with locators [3, sec. 1; 4; 2, p. 1-3]
 • Multi citation with post note [2–4, for more]
 • Multi citation with locators and pre/post notes [see 3, p. 1; 4; 2, chap. 1-2, for more]
 
-8. Tables
-• Table 1
-• Table 2
-
 1
 
 Example footnote text.
+Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum, at
+tempor nisl. Vivamus vitae pulvinar leo, at pharetra massa. Ut lobortis odio non
+nulla tincidunt pulvinar.
+2
 
 5
 
+8. Tables
+• Table 1
+• Table 2
+
 Col1
 
 Col2
 
-Col3 Col4
+Col3
+
+Col4
 
 1
 11
 111
 
 2
 22
@@ -201,62 +207,68 @@
 
 4
 44
 444
 
 Table 1: Short table
 
-Col1 Col2
+Col1
 
-Col3
+Col2
 
-Col4 Col5
+Col3
 
-Col6
+Col4
 
 a
 b
 
 1
 11
 
 2
 22
 
-3
-33
-
-123 abcd
-456 efgh
-
 Mid
 c
 
 111
 
 222
 
-333
+Col5
 
-789
+Col6
 
-Col7 Col8 Col9 Col10
-1234
-567
+Col7
+
+Col8
+
+Col9
+
+Col10
+
+3
+33
+
+123 abcd 1234
+456 efgh 567
 
 444
 44
 
 555
 55
 
 666
 66
 
-89
+333
+
+789
 
 4
 
 5
 
 6
 
@@ -265,25 +277,22 @@
 Table 2: Wide table
 
 9. Figures
 • Figure 2
 • Figure 3
 • Figure 4, Figure 4a, Figure 4b
 
-10. Includes
-• Commands from metadata include: arg min R
-• Include command in body (there should be text after this):
-Content added through include statement.
-
-2
 3
+4
 
 Footnote in sub-figure caption.
 Footnote in figure caption.
 
+89
+
 6
 
 Figure 2: Narrow figure
 
 A
 B
 C
@@ -352,17 +361,22 @@
 
 15
 
 5
 
 10
 
-(b) Figure with ‘width=3.5in’ 2
+(b) Figure with ‘width=3.5in’ 3
 
-Figure 4: Sub-figures 3
+Figure 4: Sub-figures 4
+
+10. Includes
+• Commands from metadata include: arg min R
+• Include command in body (there should be text after this):
+Content added through include statement.
 
 x
 
 15
 
 8
 
@@ -375,41 +389,52 @@
 Societies: 1977 National Computer Conference, pages 879–888, Dallas, Texas,
 1977.
 [4] Donald E. Knuth. Literate programming. The Computer Journal, 27(2):97–111,
 1984.
 
 9
 
-Appendix A Appendix 1
+Appendix A 1 Appendix 1
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi
 purus, bibendum non neque sed, lacinia tristique tortor. Vestibulum
 eu lectus sed velit luctus varius. Sed sollicitudin ligula ante. Integer
 porta a erat commodo dignissim. Duis et lectus diam. Nulla id erat
 vestibulum nisi placerat efficitur. Nulla a semper libero. Praesent
 pharetra ullamcorper massa vel tincidunt. Sed dignissim magna et
 tellus efficitur, vitae sollicitudin lorem tincidunt. Nam non velit et enim
 rutrum euismod.
+A 1.1
+
+Appendix subsection
+
+A 1.1.1
+
+Appendix subsubsection
 
-A.1 Appendix subsection
-A.1.1 Appendix subsubsection
 Proin eleifend lorem semper, commodo tellus nec, porta purus. Nullam
 commodo lectus nibh, consequat maximus lorem faucibus in. Nam
 purus eros, rutrum in sapien et, condimentum lacinia nibh.
+A 1.2
 
-A.2 Appendix figures
-• Figure A1
-• Figure A2
+Appendix figures
+
+• Figure A 1
+• Figure A 2
+A 1.3
+
+Appendix includes
 
-A.3 Appendix includes
 • Commands from metadata include (argmin R):
 • Include command in body (there should be text after this):
 Content added through include statement.
+A 1.4
+
+Appendix links
 
-A.4 Appendix links
-• Appendix section: Section A.1.1, Section B
+• Appendix section: Section A 1.1.1, Section B 2
 • Main body section: Section 1
 • Main body figure: Figure 2
 • Main body table: Table 1
 • Main body equation: Equation 1
 • Citation: Knuth (1984) [4]
 
 10
@@ -435,15 +460,15 @@
 
 x
 
 70
 
 72
 
-Figure A1: Extra wide figure
+Figure A 1: Extra wide figure
 
 74
 
 76
 
 11
 
@@ -491,115 +516,116 @@
 
 x
 
 15
 
 (c) Sub-figure
 
-Figure A2: Sub-figures with large combined size.
+Figure A 2: Sub-figures with large combined size.
 
 12
 
 Col1 Col2
 
 Col3
 
-Col4 Col5
+Col4
+
+Col5
+
+Col6
+
+Col7
+
+Col8
+
+Col9
+
+Col10
 
 a
 b
 c
 
 2
 22
 222
 
 3
 33
 333
 
-1
-11
-111
-
-Col6
-
-Col7 Col8 Col9
-
-123 abcd 1234
-456 efgh 567
+123 abcd
+456 efgh
 789
 ijkl
+
+1234
+567
 89
 
 444
 44
-42
-
-Col10
+4 B2
 
 a
 aa
 aaa
 
-Col11 Col12 Col13
-
 bbb
 bb
 b
 
+1
+11
+111
+
+Col11 Col12
 cccc
 cccc
 cccc
 
+Col13 Col14 Col15 Col16 Col17
+
 ddd
 dd
 d
 
 eeee
 eeee
 eeee
 
-Col14
-
-Col15
-
-Col16
-
-Col17
-
 fff
 ff
 f
 
 gggg
 gggg
 gggg
 
 abcd
 efgh
 ijkl
 
-1234 9876
-567 543
-89 21
+Table B 1: Extra wide table B 3
 
-Table B1: Extra wide table 3
-
-Appendix B Appendix 2
+Appendix B 2 Appendix 2
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi
 purus, bibendum non neque sed, lacinia tristique tortor. Vestibulum
 eu lectus sed velit luctus varius. Sed sollicitudin ligula ante. Integer
 porta a erat commodo dignissim. Duis et lectus diam. Nulla id erat
 vestibulum nisi placerat efficitur. Nulla a semper libero.
+B 2.1
+
+Appendix tables
 
-B.1 Appendix tables
-• Table B1
+• Table B 1
+B 2.2
 
-B.2 Appendix math
+Appendix math
 x=1
 x + y = 10
 R∞
 0
 
 exp−x dx
 2
@@ -611,21 +637,25 @@
 sin2 (x) dx
 
 • Equation 3
 • Equation 4
 • Block without tag:
 x + y + z = 100
 
-1
+B1
 
 Footnote in table.
 Footnote in table.
-3
+B3
 Footnote in table caption.
-2
+B2
 
 (3)
 (4)
 
 Col17
 
+1234 9876
+567 543
+89 21
+
```

### Comparing `shiny_mdc-1.4.1/test/samples/standalone.pdf` & `shiny_mdc-1.5.0/test/samples/standalone.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 7% similar despite different names*

#### pdftotext {} -

```diff
@@ -148,19 +148,20 @@
 
 Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section ??, Section ??
 • Appendix figure: Figure ??
 • Appendix table: Table ??
 • Appendix math: Equation ??
-• Pointer to footnote a
+• Pointer to footnote a b text
 
 7
 
 Citations
+
 • Short citation [1]
 • Short citation with pre note [see 1]
 • Short citation with locator [1, p. 1]
 • Short citation with post note [1, for more]
 • Short citation with locators and pre/post notes [see 1, chap. 1-4, for more]
 • Long citation: Lesk and Kernighan (1977) [2]
 • Long citation with locator: Lesk and Kernighan (1977) [2, chap. 1]
@@ -171,16 +172,15 @@
 • Multi citation with post note [1–3, for more]
 • Multi
 citation
 with
 locators
 and
 pre/post
-notes
-[see 2, p. 1; 3; 1, chap. 1-2, for more]
+notes [see 2, p. 1; 3; 1, chap. 1-2, for more]
 
 8
 
 Tables
 • Table 1
 • Table 2
 Col1
@@ -275,26 +275,25 @@
 
 4
 
 5
 
 6
 
-70
-
-72
-
 Table 2: Wide table
 
 9
 
 Figures
 
 a Example footnote text.
 
+b Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum, at tempor nisl.
+Vivamus vitae pulvinar leo, at pharetra massa. Ut lobortis odio non nulla tincidunt pulvinar.
+
 Figure 2: Narrow figure
 
 A
 B
 C
 D
 E
@@ -310,14 +309,18 @@
 
 66
 
 68
 
 x
 
+70
+
+72
+
 74
 
 76
 
 Figure 3: Wide figure
 • Figure 2
 • Figure 3
```

### Comparing `shiny_mdc-1.4.1/test/samples/stylish.pdf` & `shiny_mdc-1.5.0/test/samples/stylish.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 7% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,22 +1,22 @@
 shinymdc-test
-Author One1,*
+Author One 1,*
 
-Author MiddleName Two1,2,*
+Author MiddleName Two 1,2,*
 
 author1@institute1.edu
 
 authortwo@institute1.edu
 
-Author*
+Author *
 
 Author Four
 author4@author4.com
 
-Author Number Five2
+Author Number Five 2
 authornumberfive@institutetwo.edu
 
 Markdown in abstract. x + 2. Section 1. Reference
 
 [1]
 
 .
@@ -127,104 +127,97 @@
 (CMU)
 • Repeated (short): CMU
 • Forced short: USA
 • Repeated after forced short (short+long): United States
 of America (USA)
 • Plural: social security numbers (SSNs)
 
-5. Math
-Z ∞
-
-2
-
-exp−x dx
-
 7. Citations
 • Short citation[²]
 • Short citation with pre note[ˢᵉᵉ ²]
 • Short citation with locator[²𝄒 ᵖ⋅ ¹]
 • Short citation with post note[²𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
 • Short citation with locators and pre/post notes[ˢᵉᵉ ²𝄒 ᶜʰᵃᵖ⋅ ¹⁻
 ⁴𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
 • Long citation: Lesk and Kernighan (1977)[³]
-• Long citation with locator: Lesk and Kernighan
-(1977)[³𝄒 ᶜʰᵃᵖ⋅ ¹]
-• Long citation with note: Lesk and Kernighan
-(1977)[³𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
+• Long citation with locator: Lesk and Kernighan (1977)[³𝄒
+ᶜʰᵃᵖ⋅ ¹]
+• Long citation with note: Lesk and Kernighan (1977)[³𝄒
+ᶠᵒʳ ᵐᵒʳᵉ]
 • Multi citation[²𝄒 ³𝄒 ⁴]
 • Multi citation with pre note[ˢᵉᵉ ²𝄒 ³𝄒 ⁴]
-• Multi citation with locators [³𝄒 ˢᵉᶜ⋅ ¹; ⁴; ²𝄒 ᵖ⋅ ¹⁻³]
+• Multi citation with locators[³𝄒 ˢᵉᶜ⋅ ¹; ⁴; ²𝄒 ᵖ⋅ ¹⁻³]
 • Multi citation with post note[²𝄒 ³𝄒 ⁴𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
-• Multi citation with locators and pre/post notes [ˢᵉᵉ ³𝄒 ᵖ⋅ ¹;
+• Multi citation with locators and pre/post notes[ˢᵉᵉ ³𝄒 ᵖ⋅ ¹;
 ⁴; ²𝄒 ᶜʰᵃᵖ⋅ ¹⁻²𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
 
 8. Tables
 • Table 1
 • Table 2
 
-(1)
-
-Col1
+5. Math
+Z ∞
 
-0
+2
 
-Col2
+exp−x dx
 
-Col3
+(1)
 
-Col4
+0
 
-1
+Col1 Col2 Col3 Col4
+a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 17, 8, 9
 2
 3
 4
-a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 11
-7, 8, 9
+(2)
+11
 22
 33
 44
-(2)
-111
-222 333 444
 R∞
-2
-• Inline: 0 exp−x dx
-Table 1: Short table
+−x2
+111
+222
+333
+444
+• Inline: 0 exp
+dx
 • Block: Equation 1, Equation 2
+Table 1: Short table
 • Commands defined in body (P[x in X]): P[x ∈ X ]
 • Aligned:
-
-9. Figures
-
 x=1
 x + y = 10
 x + y + z = 100
 
 6. Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
-• Pointer to footnote ¹
+• Pointer to footnote¹² text
 
 ¹ Example footnote text.
+² Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum,
 
+9. Figures
 • Figure 2
 • Figure 3
 • Figure 4, Figure 4a, Figure 4b
 
 10. Includes
 • Commands from metadata include: arg min R
-• Include command in body (there should be text after
-this):
-Content added through include statement.
 
-² Footnote in sub-figure caption.
-³ Footnote in figure caption.
+at tempor nisl. Vivamus vitae pulvinar leo, at pharetra massa. Ut lobortis
+odio non nulla tincidunt pulvinar.
+³ Footnote in sub-figure caption.
+⁴ Footnote in figure caption.
 
 2
 
 A
 B
 C
 D
@@ -293,17 +286,17 @@
 
 10
 
 x
 
 15
 
-(b) Figure with ‘width=3.5in’ ²
+(b) Figure with ‘width=3.5in’³
 
-Figure 4: Sub-figures ³
+Figure 4: Sub-figures⁴
 
 3
 
 Col1
 
 Col2
 
@@ -372,14 +365,18 @@
 
 5
 
 6
 
 Table 2: Wide table
 
+• Include command in body (there should be text after
+this):
+Content added through include statement.
+
 References
 [1] Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
 [2] Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle,
 and Chris Rowley. The LATEX Companion. Addison-Wesley Professional,
 2 edition, 2004.
 [3] Michael Lesk and Brian Kernighan. Computer typesetting of technical
 journals on UNIX. In Proceedings of American Federation of Information Processing Societies: 1977 National Computer Conference, pages
@@ -575,15 +572,15 @@
 
 1234
 567
 89
 
 444
 44
-4²
+4ᴮ²
 
 a
 aa
 aaa
 
 bbb
 bb
@@ -617,15 +614,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1: Extra wide table ³
+Table B1: Extra wide tableᴮ³
 
 Appendix B
 
 Appendix 2
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi purus, bibendum non neque sed, lacinia tristique
 tortor. Vestibulum eu lectus sed velit luctus varius. Sed sollicitudin ligula ante. Integer porta a erat commodo dignissim.
@@ -659,14 +656,14 @@
 0
 
 • Equation 3
 • Equation 4
 • Block without tag:
 x + y + z = 100
 
-¹ Footnote in table.
-² Footnote in table.
-³ Footnote in table caption.
+ᴮ¹ Footnote in table.
+ᴮ² Footnote in table.
+ᴮ³ Footnote in table caption.
 
 8
```

### Comparing `shiny_mdc-1.4.1/test/sections/appendix1.md` & `shiny_mdc-1.5.0/test/sections/appendix1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/test/sections/appendix2.md` & `shiny_mdc-1.5.0/test/sections/appendix2.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 * @tbl:app2ex1
 
 Col1       Col2     Col3     Col4     Col5     Col6     Col7      Col8     Col9     Col10     Col11     Col12     Col13     Col14     Col15     Col16     Col17   Col17
 ------   ------   ------   ------   ------   ------   ------   -------   ------   -------   -------   -------   -------   -------   -------   -------   -------   -------
 a             1        2        3      123     abcd     1234       444        a       bbb      cccc       ddd      eeee       fff      gggg      abcd      1234   9876
 b            11       22       33      456     efgh      567        44       aa        bb      cccc        dd      eeee        ff      gggg      efgh       567   543
-c           111      222      333      789     ijkl       89    4 [^t]      aaa         b      cccc         d      eeee         f      gggg      ijkl        89   21
+c           111      222      333      789     ijkl       89   4\ [^t]      aaa         b      cccc         d      eeee         f      gggg      ijkl        89   21
 
-: Extra wide table [^u] {#tbl:app2ex1}
+: Extra wide table\ [^u] {#tbl:app2ex1}
 
 [^t]: Footnote in table.
 [^u]: Footnote in table caption.
 
 ## Appendix math
 
 $$
```

### Comparing `shiny_mdc-1.4.1/test/sections/main1.md` & `shiny_mdc-1.5.0/test/sections/main1.md`

 * *Files 7% similar despite different names*

```diff
@@ -56,26 +56,29 @@
 # Links
 
 * Section: @sec:ex1, @sec:ex1.2
 * Appendix section: @sec:app2ex1, @sec:app1ex1.1.1
 * Appendix figure: @fig:app1ex1
 * Appendix table: @tbl:app2ex1
 * Appendix math: @eq:app2ex2
-* Pointer to footnote [^1]
+* Pointer to footnote\ [^1] [^2] text
 
 [^1]: Example footnote text.
+[^2]: Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum, at tempor
+      nisl. Vivamus vitae pulvinar leo, at pharetra massa. Ut lobortis odio non nulla
+      tincidunt pulvinar.
 
 # Citations
 
-* Short citation [@latex:companion]
-* Short citation with pre note [see @latex:companion]
-* Short citation with locator [@latex:companion, p. 1]
-* Short citation with post note [@latex:companion, for more]
-* Short citation with locators and pre/post notes [see @latex:companion, chap. 1-4, for more]
+* Short citation\ [@latex:companion]
+* Short citation with pre note\ [see @latex:companion]
+* Short citation with locator\ [@latex:companion, p. 1]
+* Short citation with post note\ [@latex:companion, for more]
+* Short citation with locators and pre/post notes\ [see @latex:companion, chap. 1-4, for more]
 * Long citation: @lesk:1977
 * Long citation with locator: @lesk:1977 [chap. 1]
 * Long citation with note: @lesk:1977 [for more]
-* Multi citation [@lesk:1977; @knuth:1984; @latex:companion]
-* Multi citation with pre note [see @lesk:1977; @knuth:1984; @latex:companion]
-* Multi citation with locators [@lesk:1977, sec. 1; @knuth:1984; @latex:companion, p. 1-3]
-* Multi citation with post note [@lesk:1977; @knuth:1984; @latex:companion, for more]
-* Multi citation with locators and pre/post notes [see @lesk:1977, p. 1; @knuth:1984; @latex:companion, chap. 1-2, for more]
+* Multi citation\ [@lesk:1977; @knuth:1984; @latex:companion]
+* Multi citation with pre note\ [see @lesk:1977; @knuth:1984; @latex:companion]
+* Multi citation with locators\ [@lesk:1977, sec. 1; @knuth:1984; @latex:companion, p. 1-3]
+* Multi citation with post note\ [@lesk:1977; @knuth:1984; @latex:companion, for more]
+* Multi citation with locators and pre/post notes\ [see @lesk:1977, p. 1; @knuth:1984; @latex:companion, chap. 1-2, for more]
```

### Comparing `shiny_mdc-1.4.1/test/sections/main2.md` & `shiny_mdc-1.5.0/test/sections/main2.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 * @fig:ex2
 * @fig:ex3, @fig:ex3a, @fig:ex3b
 
 <div id="fig:ex3">
 
 ![Figure with 'width=2.5in'](figures/gaussian2d){#fig:ex3a width=2.5in}
 
-![Figure with 'width=3.5in' [^f]](figures/anscombe){#fig:ex3b width=3.5in}
+![Figure with 'width=3.5in'\ [^f]](figures/anscombe){#fig:ex3b width=3.5in}
 
 Sub-figures [^g]
 </div>
 
 [^f]: Footnote in sub-figure caption.
 [^g]: Footnote in figure caption.
```

### Comparing `shiny_mdc-1.4.1/test/utils/commands.md` & `shiny_mdc-1.5.0/test/utils/commands.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.4.1/PKG-INFO` & `shiny_mdc-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny-mdc
-Version: 1.4.1
+Version: 1.5.0
 Summary: Tool to compile markdown files to tex/pdf using pandoc, latexmk
 Home-page: https://github.com/jayanthkoushik/shinymdc
 License: MIT
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

