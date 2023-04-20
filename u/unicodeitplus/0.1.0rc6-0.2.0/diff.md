# Comparing `tmp/unicodeitplus-0.1.0rc6.tar.gz` & `tmp/unicodeitplus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicodeitplus-0.1.0rc6.tar", last modified: Thu Apr 20 10:35:18 2023, max compression
+gzip compressed data, was "unicodeitplus-0.2.0.tar", last modified: Thu Apr 20 14:20:53 2023, max compression
```

## Comparing `unicodeitplus-0.1.0rc6.tar` & `unicodeitplus-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:18.092018 unicodeitplus-0.1.0rc6/
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-20 10:35:03.107915 unicodeitplus-0.1.0rc6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 10:35:03.107915 unicodeitplus-0.1.0rc6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-20 10:35:18.052017 unicodeitplus-0.1.0rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-20 10:35:03.107915 unicodeitplus-0.1.0rc6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-20 10:35:18.092018 unicodeitplus-0.1.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-20 10:35:03.107915 unicodeitplus-0.1.0rc6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:18.092018 unicodeitplus-0.1.0rc6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-20 10:35:03.107915 unicodeitplus-0.1.0rc6/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)     3441 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:18.092018 unicodeitplus-0.1.0rc6/extern/
--rw-r--r--   0 runner    (1001) docker     (123)    19035 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/extern/LICENSE.LPPL
--rw-r--r--   0 runner    (1001) docker     (123)   216332 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/extern/unimathsymbols.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:18.088018 unicodeitplus-0.1.0rc6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:18.092018 unicodeitplus-0.1.0rc6/src/unicodeitplus/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/src/unicodeitplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/src/unicodeitplus/_make_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/src/unicodeitplus/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    69374 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/src/unicodeitplus/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/src/unicodeitplus/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/src/unicodeitplus/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:18.092018 unicodeitplus-0.1.0rc6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/tests/test_latex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:18.092018 unicodeitplus-0.1.0rc6/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/tools/generate_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:53.908615 unicodeitplus-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-20 14:20:53.872614 unicodeitplus-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-04-20 14:20:53.908615 unicodeitplus-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:53.908615 unicodeitplus-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3441 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:53.908615 unicodeitplus-0.2.0/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)    19035 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/extern/LICENSE.LPPL
+-rw-r--r--   0 runner    (1001) docker     (123)   216332 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/extern/unimathsymbols.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:53.908615 unicodeitplus-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:53.908615 unicodeitplus-0.2.0/src/unicodeitplus/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/src/unicodeitplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/src/unicodeitplus/_make_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/src/unicodeitplus/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69424 2023-04-20 14:20:41.632575 unicodeitplus-0.2.0/src/unicodeitplus/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-20 14:20:41.636575 unicodeitplus-0.2.0/src/unicodeitplus/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-20 14:20:41.636575 unicodeitplus-0.2.0/src/unicodeitplus/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:53.908615 unicodeitplus-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-20 14:20:41.636575 unicodeitplus-0.2.0/tests/test_latex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:53.908615 unicodeitplus-0.2.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-20 14:20:41.636575 unicodeitplus-0.2.0/tools/generate_examples.py
```

### Comparing `unicodeitplus-0.1.0rc6/CONTRIBUTING.rst` & `unicodeitplus-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc6/LICENSE` & `unicodeitplus-0.2.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-
-
-BSD License
-
 Copyright (c) 2023, Hans Dembinski
 All rights reserved.
 
-Redistribution and use in source and binary forms, with or without modification,
-are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice, this
-  list of conditions and the following disclaimer in the documentation and/or
-  other materials provided with the distribution.
-
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from this
-  software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
-IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
-INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
-BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
-OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
-OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
-OF THE POSSIBILITY OF SUCH DAMAGE.
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions
+are met:
+
+1. Redistributions of source code must retain the above copyright
+   notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above
+   copyright notice, this list of conditions and the following
+   disclaimer in the documentation and/or other materials provided
+   with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived
+   from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
+LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
+THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 The unicodeitplus repository and source distributions bundles a file which is compatibly licensed.
 
 Name: Unicode characters and corresponding LaTeX math mode commands
 Files: extern/unimathsymbols.txt
 License: LaTeX Project Public License 1.3
```

### Comparing `unicodeitplus-0.1.0rc6/Makefile` & `unicodeitplus-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc6/PKG-INFO` & `unicodeitplus-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodeitplus
-Version: 0.1.0rc6
+Version: 0.2.0
 Summary: Converts simple LaTeX to an unicode approximation
 Maintainer: Hans Dembinski
 Maintainer-email: hans.dembinski@gmail.com
 License: BSD 3-Clause License
 Project-URL: repository, https://github.com/HDembinski/unicodeitplus
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
@@ -23,69 +23,50 @@
 =============
 
 .. image:: https://img.shields.io/pypi/v/unicodeitplus.svg
         :target: https://pypi.python.org/pypi/unicodeitplus
 
 Convert simple LaTeX into an unicode approximation and paste it anywhere.
 
-This package provides a more complete LaTeX to Unicode converter than `unicodeit <https://github.com/svenkreiss/unicodeit/>`_. unicodeitplus uses a better parser (generated from EBNF with the fantastic `Lark library <https://github.com/lark-parser/lark>`_) than ``unicodeit``, which handles some code on which ``unicodeit`` fails, and allows one to parse a mix of text and math code, like ``$p_T$ / GeV $c^{-1}$``.
+This package provides a more complete LaTeX to Unicode converter than `unicodeit <https://github.com/svenkreiss/unicodeit/>`_. unicodeitplus uses a better parser (generated from EBNF with the fantastic `Lark library <https://github.com/lark-parser/lark>`_) than ``unicodeit``, which handles some code on which ``unicodeit`` fails, and allows one to parse a mix of text and math code, like::
+
+    $p_T$ / GeV $c^{-1}$
 
 LaTeX to Unicode: How does this even work?
 ------------------------------------------
 Unicode contains many subscript and superscript characters. It also font variations of characters of both latin and greek characters, including italic, boldface, bold italic, and more. It contains a lot of special mathematical characters and diacritical marks, which we use to approximate LaTeX renderings using just unicode characters.
 
 Like ``unicodeit``, ``unicodeitplus`` is largely based on ``unimathsymbols.txt`` from Günter Milde, which is maps LaTeX macros to Unicode symbols.
 
 Caveats
 -------
-- Only a subset of all LaTeX code can be converted to Unicode. Some Unicode characters simply don't exist. For example, subscript characters exist only for a subset of all lowercase latin characters, and there are no subscript characters for uppercase latin characters.
+- Only a subset of all LaTeX code can be converted to Unicode. Some Unicode characters simply don't exist. For example, subscript characters exist only for a subset of all lowercase latin characters, there are no subscript characters for uppercase latin characters, and all subscript or superscript characters are in roman font (upright).
+- Some code is rendered the best best approximation, for example, ``p_T`` as ``𝑝ₜ``, assuming that a reasonable approximation is preferred over a failed conversion.
 - Your font needs to contain glyphs for the Unicode characters, otherwise you will typically see a little box with the unicode character index.
 - The visually best results seem to be obtained with monospace fonts.
-- Some conversions are deliberate approximations, for example, ``$p_T$`` is rendered as ``𝑝ₜ``.
 
 Examples
 --------
 
-==================================  =============
-LaTeX                               Unicode
-==================================  =============
-``\alpha``                          ``𝛼``
-``\beta``                           ``𝛽``
-``\gamma``                          ``𝛾``
-``\Gamma``                          ``𝛤``
-``\infty``                          ``∞``
-``e^+``                             ``𝑒⁺``
-``\mu^-``                           ``𝜇⁻``
-``\exists``                         ``∃``
-``\in``                             ``∈``
-``\int``                            ``∫``
-``\sum``                            ``∑``
-``\partial``                        ``∂``
-``\slash{\partial}``                ``∂̸``
-``\longrightarrow``                 ``⟶``
-``\to``                             ``→``
-``p\bar{p}``                        ``𝑝𝑝̄``
-``\mathrm{t}\bar{\mathrm{t}}``      ``tt̄``
-``\mathcal{H}``                     ``ℋ``
-``\mathbb{R}``                      ``ℝ``
-``\underline{x}``                   ``𝑥̲``
-``\phone``                          ``☎``
-``\checkmark``                      ``✓``
-``\dot{x}``                         ``𝑥̇``
-``\ddot{x}``                        ``𝑥̈``
-``\vec{x}``                         ``𝑥⃗``
-``A^6``                             ``𝐴⁶``
-``m_0``                             ``𝑚₀``
-``\Im``                             ``ℑ``
-``\Re``                             ``ℜ``
-``\hbar``                           ``ℏ``
-``\perp``                           ``⟂``
-``\parallel``                       ``∥``
-``\therefore``                      ``∴``
-``\because``                        ``∵``
-``\subset``                         ``⊂``
-``\supset``                         ``⊃``
-``p_T / \mathrm{GeV} c^{-1}``       ``𝑝ₜ/GeV𝑐⁻¹``
-``K^0_S``                           ``𝐾⁰ₛ``
-``D^{\ast\ast} \to hhee``           ``𝐷**→ℎℎ𝑒𝑒``
-``A \mathbf{x} \simeq \mathbf{b}``  ``𝐴𝐱≃𝐛``
-==================================  =============
+==========================================  ===============
+LaTeX                                       Unicode
+==========================================  ===============
+``\alpha \beta \gamma \Gamma``              ``𝛼 𝛽 𝛾 𝛤``
+``e^+ \mu^-``                               ``𝑒⁺ 𝜇⁻``
+``\exists \in \int \sum \partial \infty``   ``∃ ∈ ∫ ∑ ∂ ∞``
+``\slash{\partial}``                        ``∂̸``
+``\to \longrightarrow``                     ``→ ⟶``
+``p\bar{p} \mathrm{t}\bar{\mathrm{t}}``     ``𝑝𝑝̄ tt̄``
+``\mathcal{H} \mathbb{R}``                  ``ℋ ℝ``
+``\phone \checkmark``                       ``☎ ✓``
+``\underline{x} \dot{x} \ddot{x} \vec{x}``  ``𝑥̲ 𝑥̇ 𝑥̈ 𝑥⃗``
+``A^6 m_0``                                 ``𝐴⁶ 𝑚₀``
+``1.2 \times 10^{23}``                      ``1.2 × 10²³``
+``\Im \Re``                                 ``ℑ ℜ``
+``\hbar``                                   ``ℏ``
+``\perp \parallel``                         ``⟂ ∥``
+``\therefore \because \subset \supset``     ``∴ ∵ ⊂ ⊃``
+``p_T / \mathrm{GeV} c^{-1}``               ``𝑝ₜ/GeV𝑐⁻¹``
+``K^0_S``                                   ``𝐾⁰ₛ``
+``D^{\ast\ast} \to hhee``                   ``𝐷**→ℎℎ𝑒𝑒``
+``A \cdot \mathbf{x} \simeq \mathbf{b}``    ``𝐴⋅𝐱≃𝐛``
+==========================================  ===============
```

### Comparing `unicodeitplus-0.1.0rc6/README.rst` & `unicodeitplus-0.2.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -3,69 +3,50 @@
 =============
 
 .. image:: https://img.shields.io/pypi/v/unicodeitplus.svg
         :target: https://pypi.python.org/pypi/unicodeitplus
 
 Convert simple LaTeX into an unicode approximation and paste it anywhere.
 
-This package provides a more complete LaTeX to Unicode converter than `unicodeit <https://github.com/svenkreiss/unicodeit/>`_. unicodeitplus uses a better parser (generated from EBNF with the fantastic `Lark library <https://github.com/lark-parser/lark>`_) than ``unicodeit``, which handles some code on which ``unicodeit`` fails, and allows one to parse a mix of text and math code, like ``$p_T$ / GeV $c^{-1}$``.
+This package provides a more complete LaTeX to Unicode converter than `unicodeit <https://github.com/svenkreiss/unicodeit/>`_. unicodeitplus uses a better parser (generated from EBNF with the fantastic `Lark library <https://github.com/lark-parser/lark>`_) than ``unicodeit``, which handles some code on which ``unicodeit`` fails, and allows one to parse a mix of text and math code, like::
+
+    $p_T$ / GeV $c^{-1}$
 
 LaTeX to Unicode: How does this even work?
 ------------------------------------------
 Unicode contains many subscript and superscript characters. It also font variations of characters of both latin and greek characters, including italic, boldface, bold italic, and more. It contains a lot of special mathematical characters and diacritical marks, which we use to approximate LaTeX renderings using just unicode characters.
 
 Like ``unicodeit``, ``unicodeitplus`` is largely based on ``unimathsymbols.txt`` from Günter Milde, which is maps LaTeX macros to Unicode symbols.
 
 Caveats
 -------
-- Only a subset of all LaTeX code can be converted to Unicode. Some Unicode characters simply don't exist. For example, subscript characters exist only for a subset of all lowercase latin characters, and there are no subscript characters for uppercase latin characters.
+- Only a subset of all LaTeX code can be converted to Unicode. Some Unicode characters simply don't exist. For example, subscript characters exist only for a subset of all lowercase latin characters, there are no subscript characters for uppercase latin characters, and all subscript or superscript characters are in roman font (upright).
+- Some code is rendered the best best approximation, for example, ``p_T`` as ``𝑝ₜ``, assuming that a reasonable approximation is preferred over a failed conversion.
 - Your font needs to contain glyphs for the Unicode characters, otherwise you will typically see a little box with the unicode character index.
 - The visually best results seem to be obtained with monospace fonts.
-- Some conversions are deliberate approximations, for example, ``$p_T$`` is rendered as ``𝑝ₜ``.
 
 Examples
 --------
 
-==================================  =============
-LaTeX                               Unicode
-==================================  =============
-``\alpha``                          ``𝛼``
-``\beta``                           ``𝛽``
-``\gamma``                          ``𝛾``
-``\Gamma``                          ``𝛤``
-``\infty``                          ``∞``
-``e^+``                             ``𝑒⁺``
-``\mu^-``                           ``𝜇⁻``
-``\exists``                         ``∃``
-``\in``                             ``∈``
-``\int``                            ``∫``
-``\sum``                            ``∑``
-``\partial``                        ``∂``
-``\slash{\partial}``                ``∂̸``
-``\longrightarrow``                 ``⟶``
-``\to``                             ``→``
-``p\bar{p}``                        ``𝑝𝑝̄``
-``\mathrm{t}\bar{\mathrm{t}}``      ``tt̄``
-``\mathcal{H}``                     ``ℋ``
-``\mathbb{R}``                      ``ℝ``
-``\underline{x}``                   ``𝑥̲``
-``\phone``                          ``☎``
-``\checkmark``                      ``✓``
-``\dot{x}``                         ``𝑥̇``
-``\ddot{x}``                        ``𝑥̈``
-``\vec{x}``                         ``𝑥⃗``
-``A^6``                             ``𝐴⁶``
-``m_0``                             ``𝑚₀``
-``\Im``                             ``ℑ``
-``\Re``                             ``ℜ``
-``\hbar``                           ``ℏ``
-``\perp``                           ``⟂``
-``\parallel``                       ``∥``
-``\therefore``                      ``∴``
-``\because``                        ``∵``
-``\subset``                         ``⊂``
-``\supset``                         ``⊃``
-``p_T / \mathrm{GeV} c^{-1}``       ``𝑝ₜ/GeV𝑐⁻¹``
-``K^0_S``                           ``𝐾⁰ₛ``
-``D^{\ast\ast} \to hhee``           ``𝐷**→ℎℎ𝑒𝑒``
-``A \mathbf{x} \simeq \mathbf{b}``  ``𝐴𝐱≃𝐛``
-==================================  =============
+==========================================  ===============
+LaTeX                                       Unicode
+==========================================  ===============
+``\alpha \beta \gamma \Gamma``              ``𝛼 𝛽 𝛾 𝛤``
+``e^+ \mu^-``                               ``𝑒⁺ 𝜇⁻``
+``\exists \in \int \sum \partial \infty``   ``∃ ∈ ∫ ∑ ∂ ∞``
+``\slash{\partial}``                        ``∂̸``
+``\to \longrightarrow``                     ``→ ⟶``
+``p\bar{p} \mathrm{t}\bar{\mathrm{t}}``     ``𝑝𝑝̄ tt̄``
+``\mathcal{H} \mathbb{R}``                  ``ℋ ℝ``
+``\phone \checkmark``                       ``☎ ✓``
+``\underline{x} \dot{x} \ddot{x} \vec{x}``  ``𝑥̲ 𝑥̇ 𝑥̈ 𝑥⃗``
+``A^6 m_0``                                 ``𝐴⁶ 𝑚₀``
+``1.2 \times 10^{23}``                      ``1.2 × 10²³``
+``\Im \Re``                                 ``ℑ ℜ``
+``\hbar``                                   ``ℏ``
+``\perp \parallel``                         ``⟂ ∥``
+``\therefore \because \subset \supset``     ``∴ ∵ ⊂ ⊃``
+``p_T / \mathrm{GeV} c^{-1}``               ``𝑝ₜ/GeV𝑐⁻¹``
+``K^0_S``                                   ``𝐾⁰ₛ``
+``D^{\ast\ast} \to hhee``                   ``𝐷**→ℎℎ𝑒𝑒``
+``A \cdot \mathbf{x} \simeq \mathbf{b}``    ``𝐴⋅𝐱≃𝐛``
+==========================================  ===============
```

### Comparing `unicodeitplus-0.1.0rc6/docs/Makefile` & `unicodeitplus-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc6/docs/conf.py` & `unicodeitplus-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc6/extern/LICENSE.LPPL` & `unicodeitplus-0.2.0/extern/LICENSE.LPPL`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc6/extern/unimathsymbols.txt` & `unicodeitplus-0.2.0/extern/unimathsymbols.txt`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc6/pyproject.toml` & `unicodeitplus-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc6/setup.py` & `unicodeitplus-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc6/src/unicodeitplus/__init__.py` & `unicodeitplus-0.2.0/src/unicodeitplus/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 """Top-level package for unicodeitplus."""
 from importlib.metadata import version
 from .parser import parser
 from .transform import transform
-from pathlib import Path
 
 __version__ = version("unicodeitplus")
-__all__ = ["replace"]
-
-_cdir = Path(__file__).parent
-_make_data = _cdir / "_make_data.py"
-if _make_data.stat().st_mtime > (_cdir / "data.py").stat().st_mtime:
-    from importlib import import_module
-
-    import_module("unicodeitplus._make_data").write_data()
+__all__ = ["replace", "parse"]
 
 
 def parse(s: str) -> str:
     """
     Parse simple LaTeX code and replace it by an unicode approximation.
     """
     tree = parser.parse(s)
```

### Comparing `unicodeitplus-0.1.0rc6/src/unicodeitplus/_make_data.py` & `unicodeitplus-0.2.0/src/unicodeitplus/_make_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import pathlib
+from pathlib import Path
 from typing import Dict
 
-project_dir = pathlib.Path(__file__).parent.parent.parent
-
 
 def _generate_sub_and_super_scripts() -> Dict[str, str]:
     import string
 
     # Wikipedia: https://en.wikipedia.org/wiki/Unicode_subscripts_and_superscripts
 
     cmds = {}
@@ -69,14 +67,23 @@
         if sub != " ":
             cmds[f"_{{{latex}}}"] = sub
 
     return cmds
 
 
 def _generate_from_unimathsymbols_txt() -> Dict[str, str]:
+    d = Path(__file__).parent
+    fn = None
+    while d.parent is not None:
+        d = d.parent
+        if (d / "extern").exists():
+            fn = d / "extern" / "unimathsymbols.txt"
+            break
+    assert fn is not None
+
     # Symbols extracted from extern/unimathsymbols.txt, which is under Copyright 2011 by
     # Günter Milde and licensed under the LaTeX Project Public License (LPPL)
     def match(comments: str) -> str:
         matches = [
             ("PLUS", "+"),
             ("MINUS", "-"),
             ("EQUALS", "="),
@@ -85,15 +92,15 @@
         ]
         for match, latex in matches:
             if match in comments:
                 return latex
         assert False, f"unmatched: {comments}"  # nosec, never arrive here
 
     cmds = {}
-    with open(project_dir / "extern" / "unimathsymbols.txt") as f:
+    with open(fn) as f:
         for line in f:
             if line.startswith("#"):
                 continue
             items = line.split("^")
             _, ch, latex, latex2, clas, category, requirements, comments = items
             comments = comments[:-1]
             if latex:
@@ -111,40 +118,63 @@
                 cmds[latex] = ch
             else:
                 pass
 
     return cmds
 
 
-def write_data() -> None:
-    """Write data.py with database of known LaTeX commands."""
-    cmds = _generate_sub_and_super_scripts()
-    cmds.update(_generate_from_unimathsymbols_txt())
-
-    # enhancements and aliases
-    cmds[r"\to"] = cmds[r"\rightarrow"]
+def _corrections_and_enhancements() -> Dict[str, str]:
+    cmds = {}
     cmds[r"^{\ast}"] = "*"
-    cmds[r"\hbar"] = cmds[r"\hslash"]
     cmds["h"] = "ℎ"
     cmds[r"\partial"] = "∂"
     cmds[r"\slash"] = "\u0338"
     cmds[r"\phone"] = "☎"
+    cmds[r"\thinspace"] = "\u2009"
+    return cmds
 
-    with open(project_dir / "src" / "unicodeitplus" / "data.py", "w") as f:
-        f.write(
-            """\"\"\"
+
+def _aliases(cmds: Dict[str, str]) -> None:
+    alias = {
+        r"\rightarrow": r"\to",
+        r"\hslash": r"\hbar",
+        r"\thinspace": r"\,",
+    }
+    for old, new in alias.items():
+        cmds[new] = cmds[old]
+
+
+def generate_data() -> str:
+    """Generate source code for Python module with database of known LaTeX commands."""
+    cmds = _generate_sub_and_super_scripts()
+    cmds.update(_generate_from_unimathsymbols_txt())
+    cmds.update(_corrections_and_enhancements())
+    _aliases(cmds)
+
+    chunks = [
+        """\"\"\"
 Symbols extracted from extern/unimathsymbols.txt.
 
 extern/unimathsymbols.txt is under Copyright 2011 by Günter Milde and licensed under the
 LaTeX Project Public License (LPPL).
 
 As a Derived Work, this file is licensed under LaTeX Project Public License (LPPL).
 \"\"\"
 
+COMMANDS = {
 """
-        )
-
-        f.write("COMMANDS = {\n")
-        for key in sorted(cmds):
-            val = cmds[key]
-            f.write(f"    {key!r}: {val!r},\n")
-        f.write("}\n")
+    ]
+    for key in sorted(cmds):
+        val = cmds[key]
+        chunks.append(f"    {key!r}: {val!r},\n".replace("'", '"'))
+    chunks.append("}\n")
+
+    return "".join(chunks)
+
+
+if __name__ == "__main__":
+    print(generate_data())
+else:
+    fn_data = Path(__file__).parent / "data.py"
+    if fn_data.stat().st_mtime < Path(__file__).stat().st_mtime:
+        with open(fn_data, "w") as f:
+            f.write(generate_data())
```

### Comparing `unicodeitplus-0.1.0rc6/src/unicodeitplus/data.py` & `unicodeitplus-0.2.0/src/unicodeitplus/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     "X": "𝑋",
     "Y": "𝑌",
     "Z": "𝑍",
     "\\#": "#",
     "\\$": "$",
     "\\%": "%",
     "\\&": "&",
+    "\\,": "\u2009",
     "\\:": "\u205f",
     "\\AC": "∿",
     "\\APLboxquestion": "⍰",
     "\\APLboxupcaret": "⍓",
     "\\APLcomment": "⍝",
     "\\APLdownarrowbox": "⍗",
     "\\APLinput": "⍞",
@@ -2237,14 +2238,15 @@
     "\\talloblong": "⫾",
     "\\tau": "𝜏",
     "\\taurus": "♉",
     "\\tcohm": "Ω",
     "\\therefore": "∴",
     "\\thermod": "⧧",
     "\\theta": "𝜃",
+    "\\thinspace": "\u2009",
     "\\third": "‴",
     "\\threedangle": "⟀",
     "\\threedotcolon": "⫶",
     "\\threeunderdot": "x⃨",
     "\\tieinfty": "⧝",
     "\\tilde": "̃",
     "\\times": "×",
```

### Comparing `unicodeitplus-0.1.0rc6/src/unicodeitplus/parser.py` & `unicodeitplus-0.2.0/src/unicodeitplus/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     | COMMAND
 
 ?item: atom
     | WS+
     | group
 
 CHARACTER: /[^%#&\{\}^_]/ | ESCAPED
-ESCAPED: "\\\\" | "\\#" | "\\%" | "\\&"  | "\\{" | "\\}" | "\\_"
+ESCAPED: "\\\\" | "\\#" | "\\%" | "\\&"  | "\\{" | "\\}" | "\\_" | "\\,"
 group: "{" item* "}"
 math: "$" item* "$"
 SUBSCRIPT: "_"
 SUPERSCRIPT: "^"
 COMMAND: (("\\" WORD WS*) | SUBSCRIPT | SUPERSCRIPT)
 
 %import common.WS
```

### Comparing `unicodeitplus-0.1.0rc6/src/unicodeitplus/transform.py` & `unicodeitplus-0.2.0/src/unicodeitplus/transform.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tools to transform LaTeX tree into unicode."""
+from . import _make_data  # noqa, imported for side-effects
 from .data import COMMANDS
 from lark import Tree, Token
 from typing import Optional, List, Union
 from dataclasses import dataclass
 
 
 HAS_ARG = {
```

### Comparing `unicodeitplus-0.1.0rc6/tests/test_latex.py` & `unicodeitplus-0.2.0/tests/test_latex.py`

 * *Files identical despite different names*

