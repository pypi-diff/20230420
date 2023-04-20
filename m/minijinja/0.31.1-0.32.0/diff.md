# Comparing `tmp/minijinja-0.31.1.tar.gz` & `tmp/minijinja-0.32.0.tar.gz`

## Comparing `minijinja-0.31.1.tar` & `minijinja-0.32.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
--rw-r--r--   0        0        0     1808 1970-01-01 00:00:00.000000 minijinja-0.31.1/local_dependencies/minijinja/Cargo.toml
--rw-r--r--   0     1001      123    10847 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/LICENSE
--rw-r--r--   0     1001      123     5444 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/README.md
--rw-r--r--   0     1001      123      598 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/doc-header.html
--rw-r--r--   0     1001      123    17588 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/ast.rs
--rw-r--r--   0     1001      123    30962 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/codegen.rs
--rw-r--r--   0     1001      123    11867 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/instructions.rs
--rw-r--r--   0     1001      123    18011 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/lexer.rs
--rw-r--r--   0     1001      123     7038 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/meta.rs
--rw-r--r--   0     1001      123      220 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/mod.rs
--rw-r--r--   0     1001      123    40316 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/parser.rs
--rw-r--r--   0     1001      123     4099 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/tokens.rs
--rw-r--r--   0     1001      123     2722 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/debug.rs
--rw-r--r--   0     1001      123     7292 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/defaults.rs
--rw-r--r--   0     1001      123    21455 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/environment.rs
--rw-r--r--   0     1001      123    10576 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/error.rs
--rw-r--r--   0     1001      123     2337 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/expression.rs
--rw-r--r--   0     1001      123    42561 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/filters.rs
--rw-r--r--   0     1001      123    10073 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/functions.rs
--rw-r--r--   0     1001      123     1822 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/key/deserialize.rs
--rw-r--r--   0     1001      123     9223 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/key/mod.rs
--rw-r--r--   0     1001      123     5980 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/key/serialize.rs
--rw-r--r--   0     1001      123    10220 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/lib.rs
--rw-r--r--   0     1001      123     5689 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/macros.rs
--rw-r--r--   0     1001      123     4186 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/output.rs
--rw-r--r--   0     1001      123     9329 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/source.rs
--rw-r--r--   0     1001      123    24382 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/syntax.rs
--rw-r--r--   0     1001      123     7333 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/template.rs
--rw-r--r--   0     1001      123    13302 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/tests.rs
--rw-r--r--   0     1001      123     3809 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/testutils.rs
--rw-r--r--   0     1001      123    11730 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/utils.rs
--rw-r--r--   0     1001      123    19916 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/value/argtypes.rs
--rw-r--r--   0     1001      123     2864 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/value/deserialize.rs
--rw-r--r--   0     1001      123    44469 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/value/mod.rs
--rw-r--r--   0     1001      123    18349 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/value/object.rs
--rw-r--r--   0     1001      123    11170 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/value/ops.rs
--rw-r--r--   0     1001      123    11516 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/value/serialize.rs
--rw-r--r--   0     1001      123     1685 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/vm/closure_object.rs
--rw-r--r--   0     1001      123     9844 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/vm/context.rs
--rw-r--r--   0     1001      123     1862 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/vm/fuel.rs
--rw-r--r--   0     1001      123     4433 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/vm/loop_object.rs
--rw-r--r--   0     1001      123     5550 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/vm/macro_object.rs
--rw-r--r--   0     1001      123    39339 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/vm/mod.rs
--rw-r--r--   0     1001      123     6127 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/vm/state.rs
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 minijinja-0.31.1/Cargo.toml
--rw-r--r--   0     1001      123       47 2023-04-13 19:56:21.000000 minijinja-0.31.1/.gitignore
--rw-r--r--   0     1001      123       45 2023-04-13 19:56:21.000000 minijinja-0.31.1/.vscode/settings.json
--rw-r--r--   0     1001      123    10847 2023-04-13 19:56:21.000000 minijinja-0.31.1/LICENSE
--rw-r--r--   0     1001      123      415 2023-04-13 19:56:21.000000 minijinja-0.31.1/Makefile
--rw-r--r--   0     1001      123     7544 2023-04-13 19:56:21.000000 minijinja-0.31.1/README.md
--rw-r--r--   0     1001      123      571 2023-04-13 19:56:21.000000 minijinja-0.31.1/hello.py
--rw-r--r--   0     1001      123     1110 2023-04-13 19:56:21.000000 minijinja-0.31.1/pyproject.toml
--rw-r--r--   0     1001      123     3604 2023-04-13 19:56:21.000000 minijinja-0.31.1/python/minijinja/__init__.py
--rw-r--r--   0     1001      123      558 2023-04-13 19:56:21.000000 minijinja-0.31.1/python/minijinja/_internal.py
--rw-r--r--   0     1001      123    17747 2023-04-13 19:56:21.000000 minijinja-0.31.1/src/environment.rs
--rw-r--r--   0     1001      123     2406 2023-04-13 19:56:21.000000 minijinja-0.31.1/src/error_support.rs
--rw-r--r--   0     1001      123      303 2023-04-13 19:56:21.000000 minijinja-0.31.1/src/lib.rs
--rw-r--r--   0     1001      123     2935 2023-04-13 19:56:21.000000 minijinja-0.31.1/src/state.rs
--rw-r--r--   0     1001      123    11218 2023-04-13 19:56:21.000000 minijinja-0.31.1/src/typeconv.rs
--rw-r--r--   0     1001      123     6437 2023-04-13 19:56:21.000000 minijinja-0.31.1/tests/test_basic.py
--rw-r--r--   0     1001      123      541 2023-04-13 19:56:21.000000 minijinja-0.31.1/tests/test_security.py
--rw-r--r--   0     1001      123     2492 2023-04-13 19:56:21.000000 minijinja-0.31.1/tests/test_state.py
--rw-r--r--   0     1001      123    66577 2023-04-13 19:57:01.000000 minijinja-0.31.1/Cargo.lock
--rw-r--r--   0        0        0     8547 1970-01-01 00:00:00.000000 minijinja-0.31.1/PKG-INFO
+-rw-r--r--   0        0        0     1940 1970-01-01 00:00:00.000000 minijinja-0.32.0/local_dependencies/minijinja/Cargo.toml
+-rw-r--r--   0     1001      123    10847 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/LICENSE
+-rw-r--r--   0     1001      123     5593 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/README.md
+-rw-r--r--   0     1001      123      598 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/doc-header.html
+-rw-r--r--   0     1001      123    17588 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/ast.rs
+-rw-r--r--   0     1001      123    30962 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/codegen.rs
+-rw-r--r--   0     1001      123    11867 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/instructions.rs
+-rw-r--r--   0     1001      123    23650 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/lexer.rs
+-rw-r--r--   0     1001      123     7038 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/meta.rs
+-rw-r--r--   0     1001      123      220 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/mod.rs
+-rw-r--r--   0     1001      123    40725 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/parser.rs
+-rw-r--r--   0     1001      123     4099 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/tokens.rs
+-rw-r--r--   0     1001      123     5460 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/custom_syntax.rs
+-rw-r--r--   0     1001      123     2722 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/debug.rs
+-rw-r--r--   0     1001      123     7292 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/defaults.rs
+-rw-r--r--   0     1001      123    23025 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/environment.rs
+-rw-r--r--   0     1001      123    10801 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/error.rs
+-rw-r--r--   0     1001      123     2337 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/expression.rs
+-rw-r--r--   0     1001      123    44682 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/filters.rs
+-rw-r--r--   0     1001      123    10177 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/functions.rs
+-rw-r--r--   0     1001      123     1822 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/key/deserialize.rs
+-rw-r--r--   0     1001      123     9223 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/key/mod.rs
+-rw-r--r--   0     1001      123     5980 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/key/serialize.rs
+-rw-r--r--   0     1001      123    10489 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/lib.rs
+-rw-r--r--   0     1001      123     5689 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/macros.rs
+-rw-r--r--   0     1001      123     4186 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/output.rs
+-rw-r--r--   0     1001      123    10960 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/source.rs
+-rw-r--r--   0     1001      123    25393 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/syntax.rs
+-rw-r--r--   0     1001      123     7921 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/template.rs
+-rw-r--r--   0     1001      123    13306 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/tests.rs
+-rw-r--r--   0     1001      123     3809 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/testutils.rs
+-rw-r--r--   0     1001      123    11730 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/utils.rs
+-rw-r--r--   0     1001      123    26412 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/value/argtypes.rs
+-rw-r--r--   0     1001      123     2864 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/value/deserialize.rs
+-rw-r--r--   0     1001      123    44887 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/value/mod.rs
+-rw-r--r--   0     1001      123    18349 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/value/object.rs
+-rw-r--r--   0     1001      123    11170 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/value/ops.rs
+-rw-r--r--   0     1001      123    11516 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/value/serialize.rs
+-rw-r--r--   0     1001      123     1685 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/vm/closure_object.rs
+-rw-r--r--   0     1001      123     9844 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/vm/context.rs
+-rw-r--r--   0     1001      123     1862 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/vm/fuel.rs
+-rw-r--r--   0     1001      123     4433 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/vm/loop_object.rs
+-rw-r--r--   0     1001      123     5550 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/vm/macro_object.rs
+-rw-r--r--   0     1001      123    39339 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/vm/mod.rs
+-rw-r--r--   0     1001      123     6127 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/vm/state.rs
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 minijinja-0.32.0/Cargo.toml
+-rw-r--r--   0     1001      123       47 2023-04-20 15:36:15.000000 minijinja-0.32.0/.gitignore
+-rw-r--r--   0     1001      123       45 2023-04-20 15:36:15.000000 minijinja-0.32.0/.vscode/settings.json
+-rw-r--r--   0     1001      123    10847 2023-04-20 15:36:15.000000 minijinja-0.32.0/LICENSE
+-rw-r--r--   0     1001      123      415 2023-04-20 15:36:15.000000 minijinja-0.32.0/Makefile
+-rw-r--r--   0     1001      123     7544 2023-04-20 15:36:15.000000 minijinja-0.32.0/README.md
+-rw-r--r--   0     1001      123      571 2023-04-20 15:36:15.000000 minijinja-0.32.0/hello.py
+-rw-r--r--   0     1001      123     1110 2023-04-20 15:36:15.000000 minijinja-0.32.0/pyproject.toml
+-rw-r--r--   0     1001      123     4284 2023-04-20 15:36:15.000000 minijinja-0.32.0/python/minijinja/__init__.py
+-rw-r--r--   0     1001      123      558 2023-04-20 15:36:15.000000 minijinja-0.32.0/python/minijinja/_internal.py
+-rw-r--r--   0     1001      123    20491 2023-04-20 15:36:15.000000 minijinja-0.32.0/src/environment.rs
+-rw-r--r--   0     1001      123     2406 2023-04-20 15:36:15.000000 minijinja-0.32.0/src/error_support.rs
+-rw-r--r--   0     1001      123      303 2023-04-20 15:36:15.000000 minijinja-0.32.0/src/lib.rs
+-rw-r--r--   0     1001      123     2935 2023-04-20 15:36:15.000000 minijinja-0.32.0/src/state.rs
+-rw-r--r--   0     1001      123    11218 2023-04-20 15:36:15.000000 minijinja-0.32.0/src/typeconv.rs
+-rw-r--r--   0     1001      123     6798 2023-04-20 15:36:15.000000 minijinja-0.32.0/tests/test_basic.py
+-rw-r--r--   0     1001      123      541 2023-04-20 15:36:15.000000 minijinja-0.32.0/tests/test_security.py
+-rw-r--r--   0     1001      123     2492 2023-04-20 15:36:15.000000 minijinja-0.32.0/tests/test_state.py
+-rw-r--r--   0     1001      123    66922 2023-04-20 15:37:05.000000 minijinja-0.32.0/Cargo.lock
+-rw-r--r--   0        0        0     8547 1970-01-01 00:00:00.000000 minijinja-0.32.0/PKG-INFO
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/Cargo.toml` & `minijinja-0.32.0/local_dependencies/minijinja/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [package]
 name = "minijinja"
-version = "0.31.1"
+version = "0.32.0"
 edition = "2021"
 license = "Apache-2.0"
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 description = "a powerful template engine for Rust with minimal dependencies"
 homepage = "https://github.com/mitsuhiko/minijinja"
 repository = "https://github.com/mitsuhiko/minijinja"
 keywords = ["jinja", "jinja2", "templates"]
 readme = "README.md"
 rust-version = "1.61"
 exclude = ["tests"]
 
 [package.metadata.docs.rs]
-features = ["source", "json", "urlencode", "testutils"]
+features = ["source", "json", "urlencode", "testutils", "custom_syntax"]
 rustdoc-args = ["--cfg", "docsrs", "--html-in-header", "doc-header.html"]
 
 [features]
 default = ["builtins", "debug", "deserialization", "macros", "multi_template", "adjacent_loop_items"]
 
 # API features
 preserve_order = ["indexmap"]
 deserialization = []
 debug = []
 source = ["self_cell", "memo-map"]
 unicode = ["unicode-ident"]
 testutils = []
+custom_syntax = ["dep:aho-corasick"]
 
 # Speedups
 key_interning = []
 speedups = ["v_htmlescape"]
 
 # Engine Features
 builtins = []
@@ -48,14 +49,15 @@
 unstable_machinery_serde = ["unstable_machinery", "serde/derive"]
 
 # Incorrectly named features to be removed in 1.x
 multi-template = ["multi_template"]
 adjacent-loop-items = ["adjacent_loop_items"]
 
 [dependencies]
+aho-corasick = { version = "1.0", default-features = false, optional = true }
 serde = "1.0.130"
 v_htmlescape = { version = "0.15.8", optional = true }
 self_cell = { version = "0.10.1", optional = true }
 serde_json = { version = "1.0.68", optional = true }
 percent-encoding = { version = "2.1.0", optional = true }
 indexmap = { version = "1.9.0", optional = true }
 memo-map = { version = "0.3.1", optional = true }
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/LICENSE` & `minijinja-0.32.0/local_dependencies/minijinja/LICENSE`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/README.md` & `minijinja-0.32.0/local_dependencies/minijinja/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 dependencies for a small problem.  Additionally it tries not to re-invent
 something but stay in line with prior art to leverage an already existing
 ecosystem of editor integrations.
 
 ```
 $ cargo tree
 minimal v0.1.0 (examples/minimal)
-└── minijinja v0.31.1 (minijinja)
+└── minijinja v0.32.0 (minijinja)
     └── serde v1.0.144
 ```
 
 You can play with MiniJinja online [in the browser playground](https://mitsuhiko.github.io/minijinja-playground/)
 powered by a WASM build of MiniJinja.
 
 **Goals:**
@@ -81,14 +81,16 @@
 code that is compatible with both 0.20 and newer versions of MiniJinja which
 should make it possible to defer the upgrade to later.
 
 ## Related Crates
 
 * [minijinja-autoreload](https://github.com/mitsuhiko/minijinja/tree/main/minijinja-autoreload): provides
   auto reloading functionality of environments
+* [minijinja-contrib](https://github.com/mitsuhiko/minijinja/tree/main/minijinja-contrib): provides
+  additional utilities too specific for the core
 * [minijinja-stack-ref](https://github.com/mitsuhiko/minijinja/tree/main/minijinja-stack-ref): provides
   functionality to pass values from the stack
 * [minijinja-py](https://github.com/mitsuhiko/minijinja/tree/main/minijinja-py): makes MiniJinja
   available to Python
 
 ## Similar Projects
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/doc-header.html` & `minijinja-0.32.0/local_dependencies/minijinja/doc-header.html`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/compiler/ast.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/compiler/ast.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/compiler/codegen.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/compiler/codegen.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/compiler/instructions.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/compiler/instructions.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/compiler/meta.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/compiler/meta.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/compiler/parser.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/compiler/parser.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use std::collections::BTreeSet;
 use std::fmt;
 
 use crate::compiler::ast::{self, Spanned};
-use crate::compiler::lexer::tokenize;
+use crate::compiler::lexer::{tokenize, SyntaxConfig};
 use crate::compiler::tokens::{Span, Token};
 use crate::error::{Error, ErrorKind};
 use crate::value::Value;
 
 const MAX_RECURSION: usize = 150;
 const RESERVED_NAMES: [&str; 8] = [
     "true", "True", "false", "False", "none", "None", "loop", "self",
@@ -91,16 +91,16 @@
     iter: Box<dyn Iterator<Item = Result<(Token<'a>, Span), Error>> + 'a>,
     current: Option<Result<(Token<'a>, Span), Error>>,
     last_span: Span,
 }
 
 impl<'a> TokenStream<'a> {
     /// Tokenize a template
-    pub fn new(source: &'a str, in_expr: bool) -> TokenStream<'a> {
-        let mut iter = Box::new(tokenize(source, in_expr)) as Box<dyn Iterator<Item = _>>;
+    pub fn new(source: &'a str, in_expr: bool, syntax: SyntaxConfig) -> TokenStream<'a> {
+        let mut iter = Box::new(tokenize(source, in_expr, syntax)) as Box<dyn Iterator<Item = _>>;
         let current = iter.next();
         TokenStream {
             iter,
             current,
             last_span: Span::default(),
         }
     }
@@ -212,17 +212,17 @@
         let rv = $expr;
         $parser.depth -= 1;
         rv
     }};
 }
 
 impl<'a> Parser<'a> {
-    pub fn new(source: &'a str, in_expr: bool) -> Parser<'a> {
+    pub fn new(source: &'a str, in_expr: bool, syntax: SyntaxConfig) -> Parser<'a> {
         Parser {
-            stream: TokenStream::new(source, in_expr),
+            stream: TokenStream::new(source, in_expr, syntax),
             in_macro: false,
             blocks: BTreeSet::new(),
             depth: 0,
         }
     }
 
     fn parse_ifexpr(&mut self) -> Result<ast::Expr<'a>, Error> {
@@ -1087,39 +1087,49 @@
             },
             self.stream.expand_span(span),
         )))
     }
 }
 
 /// Parses a template
+#[cfg(feature = "unstable_machinery")]
 pub fn parse<'source>(source: &'source str, filename: &str) -> Result<ast::Stmt<'source>, Error> {
+    parse_with_syntax(source, filename, Default::default())
+}
+
+/// Parses a template with a specific syntax
+pub fn parse_with_syntax<'source>(
+    source: &'source str,
+    filename: &str,
+    syntax: SyntaxConfig,
+) -> Result<ast::Stmt<'source>, Error> {
     // we want to chop off a single newline at the end.  This means that a template
     // by default does not end in a newline which is a useful property to allow
     // inline templates to work.  If someone wants a trailing newline the expectation
     // is that the user adds it themselves for achieve consistency.
     let mut source = source;
     if source.ends_with('\n') {
         source = &source[..source.len() - 1];
     }
     if source.ends_with('\r') {
         source = &source[..source.len() - 1];
     }
 
-    let mut parser = Parser::new(source, false);
+    let mut parser = Parser::new(source, false, syntax);
     parser.parse().map_err(|mut err| {
         if err.line().is_none() {
             err.set_filename_and_span(filename, parser.stream.last_span())
         }
         err
     })
 }
 
 /// Parses an expression
-pub fn parse_expr(source: &str) -> Result<ast::Expr<'_>, Error> {
-    let mut parser = Parser::new(source, true);
+pub fn parse_expr(source: &str, syntax: SyntaxConfig) -> Result<ast::Expr<'_>, Error> {
+    let mut parser = Parser::new(source, true, syntax);
     parser
         .parse_expr()
         .and_then(|result| {
             if ok!(parser.stream.next()).is_some() {
                 syntax_error!("unexpected input after expression")
             } else {
                 Ok(result)
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/compiler/tokens.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/compiler/tokens.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/debug.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/debug.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/defaults.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/defaults.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/environment.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/environment.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 use std::collections::BTreeMap;
 use std::fmt;
 use std::sync::Arc;
 
 use serde::Serialize;
 
 use crate::compiler::codegen::CodeGenerator;
+use crate::compiler::lexer::SyntaxConfig;
 use crate::compiler::parser::parse_expr;
 use crate::error::{attach_basic_debug_info, Error, ErrorKind};
 use crate::expression::Expression;
 use crate::output::Output;
 use crate::template::{CompiledTemplate, Template};
 use crate::utils::{AutoEscape, BTreeMapKeysDebug, UndefinedBehavior};
 use crate::value::{FunctionArgs, FunctionResult, Value};
 use crate::vm::{State, Vm};
 use crate::{defaults, filters, functions, tests};
 
 type TemplateMap<'source> = BTreeMap<&'source str, Arc<CompiledTemplate<'source>>>;
 
 #[derive(Clone)]
 enum Source<'source> {
-    Borrowed(TemplateMap<'source>),
+    Borrowed(TemplateMap<'source>, SyntaxConfig),
     #[cfg(feature = "source")]
     Owned(crate::source::Source),
 }
 
 impl<'source> fmt::Debug for Source<'source> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         match self {
-            Self::Borrowed(tmpls) => fmt::Debug::fmt(&BTreeMapKeysDebug(tmpls), f),
+            Self::Borrowed(tmpls, _) => fmt::Debug::fmt(&BTreeMapKeysDebug(tmpls), f),
             #[cfg(feature = "source")]
             Self::Owned(arg0) => fmt::Debug::fmt(arg0, f),
         }
     }
 }
 
 type AutoEscapeFunc = dyn Fn(&str) -> AutoEscape + Sync + Send;
@@ -97,15 +98,15 @@
     ///
     /// This environment does not yet contain any templates but it will have all
     /// the default filters, tests and globals loaded.  If you do not want any
     /// default configuration you can use the alternative
     /// [`empty`](Environment::empty) method.
     pub fn new() -> Environment<'source> {
         Environment {
-            templates: Source::Borrowed(Default::default()),
+            templates: Source::Borrowed(Default::default(), Default::default()),
             filters: defaults::get_builtin_filters(),
             tests: defaults::get_builtin_tests(),
             globals: defaults::get_globals(),
             default_auto_escape: Arc::new(defaults::default_auto_escape_callback),
             undefined_behavior: UndefinedBehavior::default(),
             formatter: Arc::new(defaults::escape_formatter),
             #[cfg(feature = "debug")]
@@ -117,15 +118,15 @@
 
     /// Creates a completely empty environment.
     ///
     /// This environment has no filters, no templates, no globals and no default
     /// logic for auto escaping configured.
     pub fn empty() -> Environment<'source> {
         Environment {
-            templates: Source::Borrowed(Default::default()),
+            templates: Source::Borrowed(Default::default(), Default::default()),
             filters: Default::default(),
             tests: Default::default(),
             globals: Default::default(),
             default_auto_escape: Arc::new(defaults::no_auto_escape),
             undefined_behavior: UndefinedBehavior::default(),
             formatter: Arc::new(defaults::escape_formatter),
             #[cfg(feature = "debug")]
@@ -146,28 +147,32 @@
     /// any form of sensible dynamic template loading.
     #[cfg_attr(
         feature = "source",
         doc = "To address this restriction use [`set_source`](Self::set_source)."
     )]
     pub fn add_template(&mut self, name: &'source str, source: &'source str) -> Result<(), Error> {
         match self.templates {
-            Source::Borrowed(ref mut map) => {
-                let compiled_template = ok!(CompiledTemplate::from_name_and_source(name, source));
+            Source::Borrowed(ref mut map, ref syntax) => {
+                let compiled_template = ok!(CompiledTemplate::from_name_and_source_with_syntax(
+                    name,
+                    source,
+                    syntax.clone()
+                ));
                 map.insert(name, Arc::new(compiled_template));
                 Ok(())
             }
             #[cfg(feature = "source")]
             Source::Owned(ref mut src) => src.add_template(name, source),
         }
     }
 
     /// Removes a template by name.
     pub fn remove_template(&mut self, name: &str) {
         match self.templates {
-            Source::Borrowed(ref mut map) => {
+            Source::Borrowed(ref mut map, _) => {
                 map.remove(name);
             }
             #[cfg(feature = "source")]
             Source::Owned(ref mut source) => {
                 source.remove_template(name);
             }
         }
@@ -184,15 +189,15 @@
     /// let mut env = Environment::new();
     /// env.add_template("hello.txt", "Hello {{ name }}!").unwrap();
     /// let tmpl = env.get_template("hello.txt").unwrap();
     /// println!("{}", tmpl.render(context!{ name => "World" }).unwrap());
     /// ```
     pub fn get_template(&self, name: &str) -> Result<Template<'_>, Error> {
         let compiled = match &self.templates {
-            Source::Borrowed(ref map) => {
+            Source::Borrowed(ref map, _) => {
                 ok!(map.get(name).ok_or_else(|| Error::new_not_found(name)))
             }
             #[cfg(feature = "source")]
             Source::Owned(source) => ok!(source.get_compiled_template(name)),
         };
         Ok(Template::new(
             self,
@@ -247,15 +252,19 @@
     ) -> Result<String, Error> {
         // reduce total amount of code faling under mono morphization into
         // this function, and share the rest in _eval.
         self._render_str(name, source, Value::from_serializable(&ctx))
     }
 
     fn _render_str(&self, name: &str, source: &str, root: Value) -> Result<String, Error> {
-        let compiled = ok!(CompiledTemplate::from_name_and_source(name, source));
+        let compiled = ok!(CompiledTemplate::from_name_and_source_with_syntax(
+            name,
+            source,
+            self._syntax_config().clone()
+        ));
         let mut rv = String::with_capacity(compiled.buffer_size_hint);
         Vm::new(self)
             .eval(
                 &compiled.instructions,
                 root,
                 &compiled.blocks,
                 &mut Output::with_string(&mut rv),
@@ -392,14 +401,46 @@
     /// Returns the configured fuel.
     #[cfg(feature = "fuel")]
     #[cfg_attr(docsrs, doc(cfg(feature = "fuel")))]
     pub fn fuel(&self) -> Option<u64> {
         self.fuel
     }
 
+    /// Sets the syntax for the environment.
+    ///
+    /// Note that when `source` is used, the syntax is held on the underlying source
+    /// which means that the actual source needs to have it's syntax changed.
+    ///
+    /// See [`Syntax`](crate::Syntax) for more information.
+    #[cfg(feature = "custom_syntax")]
+    #[cfg_attr(docsrs, doc(cfg(feature = "custom_syntax")))]
+    pub fn set_syntax(&mut self, syntax: crate::custom_syntax::Syntax) -> Result<(), Error> {
+        match self.templates {
+            Source::Borrowed(_, ref mut syn) => *syn = ok!(syntax.compile()),
+            #[cfg(feature = "source")]
+            Source::Owned(ref mut source) => ok!(source.set_syntax(syntax)),
+        };
+        Ok(())
+    }
+
+    /// Returns the current syntax.
+    #[cfg(feature = "custom_syntax")]
+    #[cfg_attr(docsrs, doc(cfg(feature = "custom_syntax")))]
+    pub fn syntax(&self) -> &crate::custom_syntax::Syntax {
+        &self._syntax_config().syntax
+    }
+
+    fn _syntax_config(&self) -> &SyntaxConfig {
+        match self.templates {
+            Source::Borrowed(_, ref syn) => syn,
+            #[cfg(feature = "source")]
+            Source::Owned(ref source) => source._syntax_config(),
+        }
+    }
+
     /// Sets the template source for the environment.
     ///
     /// This helps when working with dynamically loaded templates.  The
     /// [`Source`](crate::source::Source) is consulted by the environment to
     /// look up templates that are requested.  The source has the capabilities
     /// to load templates with fewer lifetime restrictions and can also
     /// load templates dynamically at runtime as requested.
@@ -415,25 +456,25 @@
     }
 
     /// Returns the currently set source.
     #[cfg(feature = "source")]
     #[cfg_attr(docsrs, doc(cfg(feature = "source")))]
     pub fn source(&self) -> Option<&crate::source::Source> {
         match self.templates {
-            Source::Borrowed(_) => None,
+            Source::Borrowed(..) => None,
             Source::Owned(ref source) => Some(source),
         }
     }
 
     /// Returns the currently set source as mutable reference.
     #[cfg(feature = "source")]
     #[cfg_attr(docsrs, doc(cfg(feature = "source")))]
     pub fn source_mut(&mut self) -> Option<&mut crate::source::Source> {
         match self.templates {
-            Source::Borrowed(_) => None,
+            Source::Borrowed(..) => None,
             Source::Owned(ref mut source) => Some(source),
         }
     }
 
     /// Compiles an expression.
     ///
     /// This lets one compile an expression in the template language and
@@ -441,15 +482,15 @@
     /// be used as a minimal scripting language.  For more information and an
     /// example see [`Expression`].
     pub fn compile_expression(&self, expr: &'source str) -> Result<Expression<'_, 'source>, Error> {
         attach_basic_debug_info(self._compile_expression(expr), expr)
     }
 
     fn _compile_expression(&self, expr: &'source str) -> Result<Expression<'_, 'source>, Error> {
-        let ast = ok!(parse_expr(expr));
+        let ast = ok!(parse_expr(expr, self._syntax_config().clone()));
         let mut gen = CodeGenerator::new("<expression>", expr);
         gen.compile_expr(&ast);
         let (instructions, _) = gen.finish();
         Ok(Expression::new(self, instructions))
     }
 
     /// Adds a new filter function.
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/error.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,17 @@
     /// Unable to unpack a value.
     CannotUnpack,
     /// Failed writing output.
     WriteFailure,
     /// Engine ran out of fuel
     #[cfg(feature = "fuel")]
     OutOfFuel,
+    #[cfg(feature = "custom_syntax")]
+    /// Error creating aho-corasick delimiters
+    InvalidDelimiter,
 }
 
 impl ErrorKind {
     fn description(self) -> &'static str {
         match self {
             ErrorKind::NonPrimitive => "not a primitive",
             ErrorKind::NonKey => "not a key type",
@@ -158,14 +161,16 @@
             ErrorKind::BadSerialization => "could not serialize to value",
             ErrorKind::BadInclude => "could not render include",
             ErrorKind::EvalBlock => "could not render block",
             ErrorKind::CannotUnpack => "cannot unpack",
             ErrorKind::WriteFailure => "failed to write output",
             #[cfg(feature = "fuel")]
             ErrorKind::OutOfFuel => "engine ran out of fuel",
+            #[cfg(feature = "custom_syntax")]
+            ErrorKind::InvalidDelimiter => "invalid custom delimiters",
         }
     }
 }
 
 impl fmt::Display for ErrorKind {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         write!(f, "{}", self.description())
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/expression.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/expression.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/filters.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/filters.rs`

 * *Files 5% similar despite different names*

```diff
@@ -250,15 +250,15 @@
 
 #[cfg(feature = "builtins")]
 mod builtins {
     use super::*;
 
     use crate::error::ErrorKind;
     use crate::key::Key;
-    use crate::value::{ValueKind, ValueRepr};
+    use crate::value::{Kwargs, ValueKind, ValueRepr};
     use std::borrow::Cow;
     use std::cmp::Ordering;
     use std::fmt::Write;
     use std::mem;
 
     #[cfg(test)]
     use {crate::testutils::apply_filter, similar_asserts::assert_eq};
@@ -352,31 +352,60 @@
             Error::new(
                 ErrorKind::InvalidOperation,
                 format!("cannot calculate length of value of type {}", v.kind()),
             )
         })
     }
 
+    fn sort_helper(a: &Value, b: &Value, case_sensitive: bool) -> Ordering {
+        if !case_sensitive && (a.kind() == ValueKind::String || b.kind() == ValueKind::String) {
+            // TODO: optional unicode support
+            return a
+                .to_string()
+                .to_ascii_lowercase()
+                .cmp(&b.to_string().to_ascii_lowercase());
+        }
+        match (Key::from_borrowed_value(a), Key::from_borrowed_value(b)) {
+            (Ok(a), Ok(b)) => a.partial_cmp(&b),
+            _ => a.partial_cmp(b),
+        }
+        .unwrap_or(Ordering::Less)
+    }
+
     /// Dict sorting functionality.
     ///
     /// This filter works like `|items` but sorts the pairs by key first.
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
-    pub fn dictsort(v: Value) -> Result<Value, Error> {
+    pub fn dictsort(v: Value, kwargs: Kwargs) -> Result<Value, Error> {
         if v.kind() == ValueKind::Map {
             let mut rv = Vec::with_capacity(v.len().unwrap_or(0));
             let iter = ok!(v.try_iter());
             for key in iter {
                 let value = v.get_item(&key).unwrap_or(Value::UNDEFINED);
                 rv.push((key, value));
             }
+            let by_value = match ok!(kwargs.get("by")) {
+                None | Some("key") => false,
+                Some("value") => true,
+                Some(invalid) => {
+                    return Err(Error::new(
+                        ErrorKind::InvalidOperation,
+                        format!("invalid value '{}' for 'by' parameter", invalid),
+                    ))
+                }
+            };
+            let case_sensitive = ok!(kwargs.get::<Option<bool>>("case_sensitive")).unwrap_or(false);
             rv.sort_by(|a, b| {
-                Key::from_borrowed_value(&a.0)
-                    .unwrap()
-                    .cmp(&Key::from_borrowed_value(&b.0).unwrap())
+                let (a, b) = if by_value { (&a.1, &b.1) } else { (&a.0, &b.0) };
+                sort_helper(a, b, case_sensitive)
             });
+            if let Some(true) = ok!(kwargs.get("reverse")) {
+                rv.reverse();
+            }
+            ok!(kwargs.assert_all_used());
             Ok(Value::from(
                 rv.into_iter()
                     .map(|(k, v)| Value::from(vec![k, v]))
                     .collect::<Vec<_>>(),
             ))
         } else {
             Err(Error::new(
@@ -637,24 +666,41 @@
         }));
         Ok(iter
             .max_by(|a, b| a.partial_cmp(b).unwrap_or(Ordering::Less))
             .unwrap_or(Value::UNDEFINED))
     }
 
     /// Returns the sorted version of the given list.
+    /// ```jinja
+    /// {{ [1, 3, 2, 4]|sort }} -> [4, 3, 2, 1]
+    /// {{ [1, 3, 2, 4]|sort(reverse=true) }} -> [1, 2, 3, 4]
+    /// # Sort users by age attribute in descending order.
+    /// {{ users|sort(attribute="age") }}
+    /// # Sort users by age attribute in ascending order.
+    /// {{ users|sort(attribute="age", reverse=true) }}
+    /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
-    pub fn sort(state: &State, value: Value, reverse: Option<bool>) -> Result<Value, Error> {
+    pub fn sort(state: &State, value: Value, kwargs: Kwargs) -> Result<Value, Error> {
         let mut items = ok!(state.undefined_behavior().try_iter(value).map_err(|err| {
             Error::new(ErrorKind::InvalidOperation, "cannot convert value to list").with_source(err)
         }))
         .collect::<Vec<_>>();
-        items.sort_by(|a, b| a.partial_cmp(b).unwrap_or(Ordering::Less));
-        if reverse.unwrap_or(false) {
+        let case_sensitive = ok!(kwargs.get::<Option<bool>>("case_sensitive")).unwrap_or(false);
+        if let Some(attr) = ok!(kwargs.get::<Option<&str>>("attribute")) {
+            items.sort_by(|a, b| match (a.get_path(attr), b.get_path(attr)) {
+                (Ok(a), Ok(b)) => sort_helper(&a, &b, case_sensitive),
+                _ => Ordering::Equal,
+            });
+        } else {
+            items.sort_by(|a, b| sort_helper(a, b, case_sensitive))
+        }
+        if let Some(true) = ok!(kwargs.get("reverse")) {
             items.reverse();
         }
+        ok!(kwargs.assert_all_used());
         Ok(Value::from(items))
     }
 
     /// Converts the input value into a list.
     ///
     /// If the value is already a list, then it's returned unchanged.
     /// Applied to a map this returns the list of keys, applied to a
@@ -1079,61 +1125,61 @@
         state: &State,
         value: Value,
         args: crate::value::Rest<Value>,
     ) -> Result<Vec<Value>, Error> {
         let mut rv = Vec::with_capacity(value.len().unwrap_or(0));
 
         // attribute mapping
-        if args.last().map_or(false, |x| x.is_kwargs()) {
-            let kwargs = args.last().unwrap();
-            if let Some(attr) = kwargs
-                .get_attr("attribute")
-                .ok()
-                .filter(|x| !x.is_undefined())
-            {
-                // TODO: extra arguments shouldn't be ignored
-                if args.len() > 1 {
-                    return Err(Error::new(
-                        ErrorKind::InvalidOperation,
-                        "too many arguments",
-                    ));
-                }
-                let default = kwargs.get_attr("default").ok();
-                for value in ok!(state.undefined_behavior().try_iter(value)) {
-                    let sub_val = match attr.as_str() {
-                        Some(path) => value.get_path(path),
-                        None => value.get_item(&attr),
-                    };
-                    rv.push(match (sub_val, &default) {
-                        (Ok(attr), _) => attr,
-                        (Err(err), None) => return Err(err),
-                        (Err(_), Some(default)) => default.clone(),
-                    });
-                }
-                return Ok(rv);
+        let (args, kwargs) = Kwargs::from_args(&args);
+        if let Some(attr) = ok!(kwargs.get::<Option<Value>>("attribute")) {
+            if !args.is_empty() {
+                return Err(Error::from(ErrorKind::TooManyArguments));
+            }
+            let default = ok!(kwargs.get::<Option<Value>>("default"));
+            for value in ok!(state.undefined_behavior().try_iter(value)) {
+                let sub_val = match attr.as_str() {
+                    Some(path) => value.get_path(path),
+                    None => value.get_item(&attr),
+                };
+                rv.push(match (sub_val, &default) {
+                    (Ok(attr), _) => {
+                        if attr.is_undefined() {
+                            if let Some(ref default) = default {
+                                default.clone()
+                            } else {
+                                Value::UNDEFINED
+                            }
+                        } else {
+                            attr
+                        }
+                    }
+                    (Err(_), Some(default)) => default.clone(),
+                    (Err(err), None) => return Err(err),
+                });
             }
+            ok!(kwargs.assert_all_used());
+            return Ok(rv);
         }
 
         // filter mapping
         let filter_name = ok!(args
-            .0
             .first()
             .ok_or_else(|| Error::new(ErrorKind::InvalidOperation, "filter name is required")));
         let filter_name = ok!(filter_name.as_str().ok_or_else(|| {
             Error::new(ErrorKind::InvalidOperation, "filter name must be a string")
         }));
 
         let filter = ok!(state
             .env
             .get_filter(filter_name)
             .ok_or_else(|| Error::from(ErrorKind::UnknownFilter)));
         for value in ok!(state.undefined_behavior().try_iter(value)) {
             let new_args = Some(value.clone())
                 .into_iter()
-                .chain(args.0.iter().skip(1).cloned())
+                .chain(args.iter().skip(1).cloned())
                 .collect::<Vec<_>>();
             rv.push(ok!(filter.apply_to(state, &new_args)));
         }
         Ok(rv)
     }
 
     #[test]
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/functions.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/functions.rs`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,16 @@
 //!
 //! ```json
 //! [1, 2, {"three": 3, "four": 4}]
 //! ```
 //!
 //! If a function wants to disambiugate between a value passed as keyword argument or not,
 //! the the [`Value::is_kwargs`] can be used which returns `true` if a value represents
-//! keyword arguments as opposed to just a map.
+//! keyword arguments as opposed to just a map.  A more convenient way to work with keyword
+//! arguments is the [`Kwargs`](crate::value::Kwargs) type.
 //!
 //! # Built-in Functions
 //!
 //! When the `builtins` feature is enabled a range of built-in functions are
 //! automatically added to the environment.  These are also all provided in
 //! this module.  Note though that these functions are not to be
 //! called from Rust code as their exact interface (arguments and return types)
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/key/deserialize.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/key/deserialize.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/key/mod.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/key/mod.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/key/serialize.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/key/serialize.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/lib.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -169,14 +169,16 @@
 //!   which preserves the original order of maps and structs.
 //! - `key_interning`: if this feature is enabled the automatic string interning in
 //!   the value type is enabled.  This feature used to be turned on by default but
 //!   has negative performance effects in newer versions of MiniJinja since a lot of
 //!   the previous uses of key interning are no longer needed.  Enabling it however
 //!   cuts down on memory usage slightly in certain scenarios by interning all string
 //!   keys used in dynamic map values.
+//! - `custom_syntax`: when this feature is enabled, custom delimiters are supported by
+//!   the parser.
 //!
 //! </details>
 #![allow(clippy::cognitive_complexity)]
 #![allow(clippy::get_first)]
 #![cfg_attr(docsrs, feature(doc_cfg))]
 #![deny(missing_docs)]
 #![doc(html_logo_url = "https://github.com/mitsuhiko/minijinja/raw/main/artwork/logo-square.png")]
@@ -204,25 +206,31 @@
 #[cfg(any(test, feature = "testutils"))]
 #[cfg_attr(docsrs, doc(cfg(feature = "testutils")))]
 pub mod testutils;
 
 #[cfg(feature = "source")]
 mod source;
 
+#[cfg(feature = "custom_syntax")]
+mod custom_syntax;
+
 #[cfg(feature = "debug")]
 mod debug;
 
 pub use self::defaults::{default_auto_escape_callback, escape_formatter};
 pub use self::environment::Environment;
 pub use self::error::{Error, ErrorKind};
 pub use self::expression::Expression;
 pub use self::output::Output;
 pub use self::template::Template;
 pub use self::utils::{AutoEscape, HtmlEscape, UndefinedBehavior};
 
+#[cfg(feature = "custom_syntax")]
+pub use self::custom_syntax::Syntax;
+
 #[cfg(feature = "source")]
 pub use self::source::Source;
 
 pub use self::macros::__context;
 pub use self::vm::State;
 
 /// This module gives access to the low level machinery.
@@ -233,16 +241,16 @@
 #[cfg(feature = "unstable_machinery")]
 #[cfg_attr(docsrs, doc(cfg(feature = "unstable_machinery")))]
 pub mod machinery {
     #![allow(missing_docs)]
     pub use crate::compiler::ast;
     pub use crate::compiler::codegen::CodeGenerator;
     pub use crate::compiler::instructions::{Instruction, Instructions};
-    pub use crate::compiler::lexer::tokenize;
-    pub use crate::compiler::parser::parse;
+    pub use crate::compiler::lexer::{tokenize, SyntaxConfig};
+    pub use crate::compiler::parser::{parse, parse_with_syntax};
     pub use crate::compiler::tokens::{Span, Token};
     pub use crate::template::CompiledTemplate;
     pub use crate::vm::Vm;
 
     use crate::Output;
 
     /// Creates an [`Output`] that writes into a string.
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/macros.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/macros.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/output.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/output.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/source.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/source.rs`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 use std::path::Path;
 use std::path::PathBuf;
 use std::sync::Arc;
 
 use memo_map::MemoMap;
 use self_cell::self_cell;
 
+use crate::compiler::lexer::SyntaxConfig;
 use crate::error::{Error, ErrorKind};
 use crate::template::CompiledTemplate;
 
 #[cfg(test)]
 use similar_asserts::assert_eq;
 
 type LoadFunc = dyn for<'a> Fn(&'a str) -> Result<String, Error> + Send + Sync;
@@ -38,17 +39,19 @@
 }
 
 #[derive(Clone)]
 enum SourceBacking {
     Dynamic {
         templates: MemoMap<String, Arc<LoadedTemplate>>,
         loader: Arc<LoadFunc>,
+        syntax: SyntaxConfig,
     },
     Static {
         templates: HashMap<String, Arc<LoadedTemplate>>,
+        syntax: SyntaxConfig,
     },
 }
 
 impl Default for Source {
     fn default() -> Source {
         Source::new()
     }
@@ -57,15 +60,15 @@
 impl fmt::Debug for Source {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         match &self.backing {
             SourceBacking::Dynamic { templates, .. } => f
                 .debug_list()
                 .entries(templates.iter().map(|x| x.0))
                 .finish(),
-            SourceBacking::Static { templates } => f
+            SourceBacking::Static { templates, .. } => f
                 .debug_list()
                 .entries(templates.iter().map(|x| x.0))
                 .finish(),
         }
     }
 }
 
@@ -96,18 +99,48 @@
     ///     env
     /// }
     /// ```
     pub fn new() -> Source {
         Source {
             backing: SourceBacking::Static {
                 templates: HashMap::new(),
+                syntax: Default::default(),
             },
         }
     }
 
+    /// Sets the syntax for the source.
+    ///
+    /// See [`Syntax`](crate::Syntax) for more information.
+    #[cfg(feature = "custom_syntax")]
+    #[cfg_attr(docsrs, doc(cfg(feature = "custom_syntax")))]
+    pub fn set_syntax(&mut self, new_syntax: crate::custom_syntax::Syntax) -> Result<(), Error> {
+        match self.backing {
+            SourceBacking::Dynamic { ref mut syntax, .. }
+            | SourceBacking::Static { ref mut syntax, .. } => {
+                *syntax = ok!(new_syntax.compile());
+            }
+        }
+        Ok(())
+    }
+
+    /// Returns the current syntax.
+    #[cfg(feature = "custom_syntax")]
+    #[cfg_attr(docsrs, doc(cfg(feature = "custom_syntax")))]
+    pub fn syntax(&self) -> &crate::custom_syntax::Syntax {
+        &self._syntax_config().syntax
+    }
+
+    pub(crate) fn _syntax_config(&self) -> &SyntaxConfig {
+        match &self.backing {
+            SourceBacking::Dynamic { ref syntax, .. }
+            | SourceBacking::Static { ref syntax, .. } => syntax,
+        }
+    }
+
     /// Creates a source with a dynamic loader.
     ///
     /// When a source was created with the loader, the source gains the ability
     /// to dynamically load templates.  The loader is invoked with the name of
     /// the template.  If this template exists `Ok(Some(template_source))` has
     /// to be returned, otherwise `Ok(None)`.
     ///
@@ -134,14 +167,15 @@
         Source {
             backing: SourceBacking::Dynamic {
                 templates: MemoMap::new(),
                 loader: Arc::new(move |name| match ok!(f(name)) {
                     Some(rv) => Ok(rv),
                     None => Err(Error::new_not_found(name)),
                 }),
+                syntax: Default::default(),
             },
         }
     }
 
     /// Creates a source that loads on demand from a given directory.
     ///
     /// This creates a source with a dynamic loader which looks up templates in the
@@ -188,58 +222,72 @@
     ) -> Result<(), Error> {
         let source = source.into();
         let name = name.into();
         let owner = (name.clone(), source);
         let tmpl = ok!(LoadedTemplate::try_new(
             owner,
             |(name, source)| -> Result<_, Error> {
-                CompiledTemplate::from_name_and_source(name.as_str(), source)
+                CompiledTemplate::from_name_and_source_with_syntax(
+                    name.as_str(),
+                    source,
+                    self._syntax_config().clone(),
+                )
             }
         ));
 
         match self.backing {
             SourceBacking::Dynamic {
                 ref mut templates, ..
             } => {
                 templates.replace(name, Arc::new(tmpl));
             }
-            SourceBacking::Static { ref mut templates } => {
+            SourceBacking::Static {
+                ref mut templates, ..
+            } => {
                 templates.insert(name, Arc::new(tmpl));
             }
         }
         Ok(())
     }
 
     /// Removes an already loaded template from the source.
     pub fn remove_template(&mut self, name: &str) {
         match &mut self.backing {
             SourceBacking::Dynamic { templates, .. } => templates.remove(name),
-            SourceBacking::Static { templates } => templates.remove(name),
+            SourceBacking::Static { templates, .. } => templates.remove(name),
         };
     }
 
     /// Gets a compiled template from the source.
     pub(crate) fn get_compiled_template(&self, name: &str) -> Result<&CompiledTemplate<'_>, Error> {
         match &self.backing {
-            SourceBacking::Dynamic { templates, loader } => Ok(ok!(templates.get_or_try_insert(
-                name,
-                || -> Result<_, Error> {
+            SourceBacking::Dynamic {
+                templates,
+                loader,
+                syntax,
+            } => Ok(
+                ok!(templates.get_or_try_insert(name, || -> Result<_, Error> {
+                    let syntax = syntax.clone();
                     let source = ok!(loader(name));
                     let owner = (name.to_owned(), source);
                     let tmpl = ok!(LoadedTemplate::try_new(
                         owner,
                         |(name, source)| -> Result<_, Error> {
-                            CompiledTemplate::from_name_and_source(name.as_str(), source)
+                            CompiledTemplate::from_name_and_source_with_syntax(
+                                name.as_str(),
+                                source,
+                                syntax,
+                            )
                         }
                     ));
                     Ok(Arc::new(tmpl))
-                }
-            ))
-            .borrow_dependent()),
-            SourceBacking::Static { templates } => templates
+                }))
+                .borrow_dependent(),
+            ),
+            SourceBacking::Static { templates, .. } => templates
                 .get(name)
                 .map(|value| value.borrow_dependent())
                 .ok_or_else(|| Error::new_not_found(name)),
         }
     }
 }
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/syntax.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/syntax.rs`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 //!   - [`{% set %}`](#-set-)
 //!   - [`{% filter %}`](#-filter-)
 //!   - [`{% macro %}`](#-macro-)
 //!   - [`{% call %}`](#-call-)
 //!   - [`{% do %}`](#-do-)
 //!   - [`{% autoescape %}`](#-autoescape-)
 //!   - [`{% raw %}`](#-raw-)
+//! - [Custom Delimiters](#custom-delimiters)
 //!
 //! </details>
 //!
 //! # Synopsis
 //!
 //! A MiniJinja template is simply a text file.  MiniJinja can generate any text-based
 //! format (HTML, XML, CSV, LaTeX, etc.).  A template doesn’t need to have a specific extension
@@ -678,9 +679,44 @@
 //! <ul>
 //! {% for item in seq %}
 //!     <li>{{ item }}</li>
 //! {% endfor %}
 //! </ul>
 //! {% endraw %}
 //! ```
+//!
+#![cfg_attr(
+    feature = "custom_syntax",
+    doc = r#"
+# Custom Delimiters
+
+When MiniJinja has been compiled with the `custom_syntax` feature (see
+[`Syntax`](crate::Syntax)), it's possible to reconfigure the delimiters of the
+templates.  This is generally not recommended but it's useful for situations
+where Jinja templates are used to generate files with a syntax that would be
+conflicting for Jinja.  With custom delimiters it can for instance be more
+convenient to generate LaTeX files:
+
+```
+# use minijinja::{Environment, Syntax};
+let mut environment = Environment::new();
+environment.set_syntax(Syntax {
+    block_start: "\\BLOCK{".into(),
+    block_end: "}".into(),
+    variable_start: "\\VAR{".into(),
+    variable_end: "}".into(),
+    comment_start: "\\#{".into(),
+    comment_end: "}".into(),
+}).unwrap();
+```
+
+And then a template might look like this instead:
 
-// this is just for docs
+```latex
+\begin{itemize}
+\BLOCK{for item in sequence}
+  \item \VAR{item}
+\BLOCK{endfor}
+\end{itemize}
+```
+"#
+)]
```

#### html2text {}

```diff
@@ -4,26 +4,27 @@
 ! - [Comparisons](#comparisons) //! - [Logic](#logic) //! - [Other Operators]
 (#other-operators) //! - [If Expressions](#if-expressions) //! - [Tags](#tags)
 //! - [`{% for %}`](#-for-) //! - [`{% if %}`](#-if-) //! - [`{% extends %}`]
 (#-extends-) //! - [`{% block %}`](#-block-) //! - [`{% include %}`](#-include-
 ) //! - [`{% import %}`](#-import-) //! - [`{% with %}`](#-with-) //! - [`{%
 set %}`](#-set-) //! - [`{% filter %}`](#-filter-) //! - [`{% macro %}`](#-
 macro-) //! - [`{% call %}`](#-call-) //! - [`{% do %}`](#-do-) //! - [`{%
-autoescape %}`](#-autoescape-) //! - [`{% raw %}`](#-raw-) //! //!  //! //! #
-Synopsis //! //! A MiniJinja template is simply a text file. MiniJinja can
-generate any text-based //! format (HTML, XML, CSV, LaTeX, etc.). A template
-doesnât need to have a specific extension //! and in fact MiniJinja does not
-understand much about the file system. However the default //! configuration
-for [auto escaping](crate::Environment::set_auto_escape_callback) uses file //
-! extensions to configure the initial behavior. //! //! A template contains
-[**expressions**](#expressions), which get replaced with values when a //
-! template is rendered; and [**tags**](#tags), which control the logic of the
-template. The //! template syntax is heavily inspired by Jinja2, Django and
-Python. //! //! This is a minimal template that illustrates a few basics: //! /
-/! ```jinja //!
+autoescape %}`](#-autoescape-) //! - [`{% raw %}`](#-raw-) //! - [Custom
+Delimiters](#custom-delimiters) //! //!  //! //! # Synopsis //! //! A MiniJinja
+template is simply a text file. MiniJinja can generate any text-based //
+! format (HTML, XML, CSV, LaTeX, etc.). A template doesnât need to have a
+specific extension //! and in fact MiniJinja does not understand much about the
+file system. However the default //! configuration for [auto escaping](crate::
+Environment::set_auto_escape_callback) uses file //! extensions to configure
+the initial behavior. //! //! A template contains [**expressions**]
+(#expressions), which get replaced with values when a //! template is rendered;
+and [**tags**](#tags), which control the logic of the template. The //
+! template syntax is heavily inspired by Jinja2, Django and Python. //! //
+! This is a minimal template that illustrates a few basics: //! //! ```jinja //
+!
  //!
 //!
     * //! {% for item in navigation %} //!
     * {{_item.caption_}}
     * //! {% endfor %} //!
 //! //!
 ****** My Webpage ******
@@ -349,8 +350,20 @@
 %}` //! //! A raw block is a special construct that lets you ignore the
 embedded template //! syntax. This is particularly useful if a segment of
 template code would //! otherwise require constant escaping with things like `{
 { "{{" }}`: //! //! Example: //! //! ```jinja //! {% raw %} //!
     * //! {% for item in seq %} //!
     * {{ item }}
     * //! {% endfor %} //!
-//! {% endraw %} //! ``` // this is just for docs
+//! {% endraw %} //! ``` //! #![cfg_attr( feature = "custom_syntax", doc = r#"
+# Custom Delimiters When MiniJinja has been compiled with the `custom_syntax`
+feature (see [`Syntax`](crate::Syntax)), it's possible to reconfigure the
+delimiters of the templates. This is generally not recommended but it's useful
+for situations where Jinja templates are used to generate files with a syntax
+that would be conflicting for Jinja. With custom delimiters it can for instance
+be more convenient to generate LaTeX files: ``` # use minijinja::{Environment,
+Syntax}; let mut environment = Environment::new(); environment.set_syntax
+(Syntax { block_start: "\\BLOCK{".into(), block_end: "}".into(),
+variable_start: "\\VAR{".into(), variable_end: "}".into(), comment_start: "\\#
+{".into(), comment_end: "}".into(), }).unwrap(); ``` And then a template might
+look like this instead: ```latex \begin{itemize} \BLOCK{for item in sequence}
+\item \VAR{item} \BLOCK{endfor} \end{itemize} ``` "# )]
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/template.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/template.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 use std::collections::BTreeMap;
 use std::{fmt, io};
 
 use serde::Serialize;
 
 use crate::compiler::codegen::CodeGenerator;
 use crate::compiler::instructions::Instructions;
-use crate::compiler::parser::parse;
+use crate::compiler::lexer::SyntaxConfig;
+use crate::compiler::parser::parse_with_syntax;
 use crate::environment::Environment;
 use crate::error::{attach_basic_debug_info, Error, ErrorKind};
 use crate::output::{Output, WriteWrapper};
 use crate::utils::AutoEscape;
 use crate::value::{self, Value};
 use crate::vm::Vm;
 
@@ -178,29 +179,43 @@
         }
         ds.finish()
     }
 }
 
 impl<'source> CompiledTemplate<'source> {
     /// Creates a compiled template from name and source.
+    #[cfg(feature = "unstable_machinery")]
     pub fn from_name_and_source(
         name: &'source str,
         source: &'source str,
     ) -> Result<CompiledTemplate<'source>, Error> {
-        attach_basic_debug_info(Self::_from_name_and_source_impl(name, source), source)
+        Self::from_name_and_source_with_syntax(name, source, Default::default())
     }
 
-    fn _from_name_and_source_impl(
+    /// Creates a compiled template from name and source using the given settings.
+    pub fn from_name_and_source_with_syntax(
         name: &'source str,
         source: &'source str,
+        syntax: SyntaxConfig,
+    ) -> Result<CompiledTemplate<'source>, Error> {
+        attach_basic_debug_info(
+            Self::_from_name_settings_and_source_with_syntax_impl(name, source, syntax),
+            source,
+        )
+    }
+
+    fn _from_name_settings_and_source_with_syntax_impl(
+        name: &'source str,
+        source: &'source str,
+        syntax: SyntaxConfig,
     ) -> Result<CompiledTemplate<'source>, Error> {
         // the parser/compiler combination can create constants in which case
         // we can probably benefit from the value optimization a bit.
         let _guard = value::value_optimization();
-        let ast = ok!(parse(source, name));
+        let ast = ok!(parse_with_syntax(source, name, syntax));
         let mut gen = CodeGenerator::new(name, source);
         gen.compile_stmt(&ast);
         let buffer_size_hint = gen.buffer_size_hint();
         let (instructions, blocks) = gen.finish();
         Ok(CompiledTemplate {
             instructions,
             blocks,
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/tests.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/tests.rs`

 * *Files 0% similar despite different names*

```diff
@@ -307,27 +307,27 @@
     pub fn is_mapping(v: Value) -> bool {
         matches!(v.kind(), ValueKind::Map)
     }
 
     /// Checks if the value is starting with a string.
     ///
     /// ```jinja
-    /// {{ "foobar" is startingwith "foo" }} -> true
-    /// {{ "foobar" is startingwith "bar" }} -> false
+    /// {{ "foobar" is startingwith("foo") }} -> true
+    /// {{ "foobar" is startingwith("bar") }} -> false
     /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn is_startingwith(v: Cow<'_, str>, other: Cow<'_, str>) -> bool {
         v.starts_with(&other as &str)
     }
 
     /// Checks if the value is ending with a string.
     ///
     /// ```jinja
-    /// {{ "foobar" is endingwith "bar" }} -> true
-    /// {{ "foobar" is endingwith "foo" }} -> false
+    /// {{ "foobar" is endingwith("bar") }} -> true
+    /// {{ "foobar" is endingwith("foo") }} -> false
     /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn is_endingwith(v: Cow<'_, str>, other: Cow<'_, str>) -> bool {
         v.ends_with(&other as &str)
     }
 
     /// Test version of `==`.
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/testutils.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/testutils.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/utils.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/utils.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/value/argtypes.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/value/argtypes.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 use std::borrow::Cow;
-use std::collections::{BTreeMap, HashMap};
+use std::cell::RefCell;
+use std::collections::{BTreeMap, HashMap, HashSet};
 use std::convert::TryFrom;
 use std::ops::{Deref, DerefMut};
 
 use crate::error::{Error, ErrorKind};
 use crate::key::{Key, StaticKey};
 use crate::utils::UndefinedBehavior;
 use crate::value::{
-    Arc, MapType, Object, Packed, SeqObject, StringType, Value, ValueKind, ValueRepr,
+    Arc, MapType, Object, Packed, SeqObject, StringType, Value, ValueKind, ValueMap, ValueRepr,
 };
 use crate::vm::State;
 
 /// A utility trait that represents the return value of functions and filters.
 ///
 /// It's implemented for the following types:
 ///
@@ -424,17 +425,25 @@
 primitive_try_from!(bool, {
     ValueRepr::Bool(val) => val,
 });
 primitive_try_from!(char, {
     ValueRepr::Char(val) => val,
 });
 primitive_try_from!(f32, {
+    ValueRepr::U64(val) => val as f32,
+    ValueRepr::I64(val) => val as f32,
+    ValueRepr::U128(val) => val.0 as f32,
+    ValueRepr::I128(val) => val.0 as f32,
     ValueRepr::F64(val) => val as f32,
 });
 primitive_try_from!(f64, {
+    ValueRepr::U64(val) => val as f64,
+    ValueRepr::I64(val) => val as f64,
+    ValueRepr::U128(val) => val.0 as f64,
+    ValueRepr::I128(val) => val.0 as f64,
     ValueRepr::F64(val) => val,
 });
 
 impl<'a> ArgType<'a> for &str {
     type Output = &'a str;
 
     fn from_value(value: Option<&'a Value>) -> Result<Self::Output, Error> {
@@ -475,15 +484,15 @@
 
 impl<'a, T: ArgType<'a>> ArgType<'a> for Option<T> {
     type Output = Option<T::Output>;
 
     fn from_value(value: Option<&'a Value>) -> Result<Self::Output, Error> {
         match value {
             Some(value) => {
-                if value.is_undefined() || value.is_none() {
+                if value.is_undefined() {
                     Ok(None)
                 } else {
                     T::from_value(Some(value)).map(Some)
                 }
             }
             None => Ok(None),
         }
@@ -583,14 +592,197 @@
                 .map(|v| T::from_value(Some(v)))
                 .collect::<Result<_, _>>())),
             args.len(),
         ))
     }
 }
 
+/// Utility to accept keyword arguments.
+///
+/// Keyword arguments are represented as regular values as the last argument
+/// in an argument list.  This can be quite complex to use manually so this
+/// type is added as a utility.  You can use [`get`](Self::get) to fetch a
+/// single keyword argument and then use [`assert_all_used`](Self::assert_all_used)
+/// to make sure extra arguments create an error.
+///
+/// Here an example of a function modifying values in different ways.
+///
+/// ```
+/// use minijinja::value::{Value, Kwargs};
+/// use minijinja::Error;
+///
+/// fn modify(mut values: Vec<Value>, options: Kwargs) -> Result<Vec<Value>, Error> {
+///     // get pulls a parameter of any type.  Same as from_args.  For optional
+///     // boolean values the type inference is particularly convenient.
+///     if let Some(true) = options.get("reverse")? {
+///         values.reverse();
+///     }
+///     if let Some(limit) = options.get("limit")? {
+///         values.truncate(limit);
+///     }
+///     options.assert_all_used()?;
+///     Ok(values)
+/// }
+/// ```
+///
+/// If for whatever reason you need a value again you can use [`Into`] to
+/// convert it back into a [`Value`].
+#[derive(Debug, Clone)]
+pub struct Kwargs {
+    values: Arc<ValueMap>,
+    used: RefCell<HashSet<String>>,
+}
+
+impl<'a> ArgType<'a> for Kwargs {
+    type Output = Self;
+
+    fn from_value(value: Option<&'a Value>) -> Result<Self, Error> {
+        match value {
+            Some(value) => {
+                if let ValueRepr::Map(ref map, MapType::Kwargs) = value.0 {
+                    Ok(Kwargs::new(map.clone()))
+                } else {
+                    Err(Error::from(ErrorKind::MissingArgument))
+                }
+            }
+            None => Ok(Kwargs::new(Default::default())),
+        }
+    }
+
+    fn from_state_and_values(
+        _state: Option<&'a State>,
+        values: &'a [Value],
+        offset: usize,
+    ) -> Result<(Self, usize), Error> {
+        if let Some(value) = values.get(offset) {
+            if let ValueRepr::Map(ref map, MapType::Kwargs) = value.0 {
+                return Ok((Kwargs::new(map.clone()), 1));
+            }
+        }
+        Ok((Kwargs::new(Default::default()), 0))
+    }
+}
+
+impl Kwargs {
+    fn new(map: Arc<ValueMap>) -> Kwargs {
+        Kwargs {
+            values: map,
+            used: RefCell::new(HashSet::new()),
+        }
+    }
+
+    /// Split off kwargs from args.
+    ///
+    /// This is useful when [`Rest`] is used to consume all arguments:
+    ///
+    /// ```rust
+    /// # use minijinja::value::{Value, Rest, Kwargs};
+    /// fn my_func(args: Rest<Value>) -> Value {
+    ///     let (args, kwargs) = Kwargs::from_args(&args);
+    ///     // do something with args and kwargs
+    /// # todo!()
+    /// }
+    /// ```
+    pub fn from_args(args: &[Value]) -> (&[Value], Kwargs) {
+        if let Some(value) = args.last() {
+            if let ValueRepr::Map(ref map, MapType::Kwargs) = value.0 {
+                return (&args[..args.len() - 1], Kwargs::new(map.clone()));
+            }
+        }
+        (args, Kwargs::new(Default::default()))
+    }
+
+    /// Get a single argument from the kwargs but don't mark it as used.
+    pub fn peek<'a, T>(&'a self, key: &'a str) -> Result<T, Error>
+    where
+        T: ArgType<'a, Output = T>,
+    {
+        T::from_value(self.values.get(&Key::Str(key)))
+    }
+
+    /// Gets a single argument from the kwargs and marks it as used.
+    ///
+    /// This method works pretty much like [`from_args`] and marks any parameter
+    /// used internally.  For optional arguments you would typically use
+    /// `Option<T>` and for non optional ones directly `T`.
+    ///
+    /// Examples:
+    ///
+    /// ```
+    /// # use minijinja::Error;
+    /// # use minijinja::value::Kwargs; fn f(kwargs: Kwargs) -> Result<(), Error> {
+    /// // f(int=42) -> Some(42)
+    /// // f() -> None
+    /// let optional_int: Option<u32> = kwargs.get("int")?;
+    /// // f(int=42) -> 42
+    /// // f() -> Error
+    /// let required_int: u32 = kwargs.get("int")?;
+    /// # Ok(()) }
+    /// ```
+    ///
+    /// If you don't want to mark it as used, us [`peek`](Self::peek) instead.
+    pub fn get<'a, T>(&'a self, key: &'a str) -> Result<T, Error>
+    where
+        T: ArgType<'a, Output = T>,
+    {
+        let rv = ok!(self.peek::<T>(key));
+        self.used.borrow_mut().insert(key.to_string());
+        Ok(rv)
+    }
+
+    /// Checks if a keyword argument exists.
+    pub fn has(&self, key: &str) -> bool {
+        self.values.contains_key(&Key::Str(key))
+    }
+
+    /// Iterates over all passed keyword arguments.
+    pub fn args(&self) -> impl Iterator<Item = &str> {
+        self.values.iter().filter_map(|x| x.0.as_str())
+    }
+
+    /// Asserts that all kwargs were used.
+    pub fn assert_all_used(&self) -> Result<(), Error> {
+        let used = self.used.borrow();
+        for key in self.values.keys() {
+            if let Some(key) = key.as_str() {
+                if !used.contains(key) {
+                    return Err(Error::new(
+                        ErrorKind::TooManyArguments,
+                        format!("unknown keyword argument '{}'", key),
+                    ));
+                }
+            } else {
+                return Err(Error::new(
+                    ErrorKind::InvalidOperation,
+                    "non string keys passed to kwargs",
+                ));
+            }
+        }
+        Ok(())
+    }
+}
+
+impl From<Kwargs> for Value {
+    fn from(value: Kwargs) -> Self {
+        Value(ValueRepr::Map(value.values, MapType::Kwargs))
+    }
+}
+
+impl TryFrom<Value> for Kwargs {
+    type Error = Error;
+
+    fn try_from(value: Value) -> Result<Self, Self::Error> {
+        match value.0 {
+            ValueRepr::Undefined => Ok(Kwargs::new(Default::default())),
+            ValueRepr::Map(ref val, MapType::Kwargs) => Ok(Kwargs::new(val.clone())),
+            _ => Err(Error::from(ErrorKind::InvalidOperation)),
+        }
+    }
+}
+
 impl<'a> ArgType<'a> for Value {
     type Output = Self;
 
     fn from_state_and_value(
         _state: Option<&'a State>,
         value: Option<&'a Value>,
     ) -> Result<(Self::Output, usize), Error> {
@@ -662,7 +854,17 @@
 }
 
 impl From<usize> for Value {
     fn from(val: usize) -> Self {
         Value::from(val as u64)
     }
 }
+
+#[test]
+fn test_as_f64() {
+    let v = Value::from(42u32);
+    let f: f64 = v.try_into().unwrap();
+    assert_eq!(f, 42.0);
+    let v = Value::from(42.5);
+    let f: f64 = v.try_into().unwrap();
+    assert_eq!(f, 42.5);
+}
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/value/deserialize.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/value/deserialize.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/value/mod.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/value/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 use crate::functions;
 use crate::key::{Key, StaticKey};
 use crate::utils::OnDrop;
 use crate::value::object::{SimpleSeqObject, SimpleStructObject};
 use crate::value::serialize::transform;
 use crate::vm::State;
 
-pub use crate::value::argtypes::{from_args, ArgType, FunctionArgs, FunctionResult, Rest};
+pub use crate::value::argtypes::{from_args, ArgType, FunctionArgs, FunctionResult, Kwargs, Rest};
 pub use crate::value::object::{Object, ObjectKind, SeqObject, SeqObjectIter, StructObject};
 
 mod argtypes;
 #[cfg(feature = "deserialization")]
 mod deserialize;
 mod object;
 pub(crate) mod ops;
@@ -604,14 +604,28 @@
                 ObjectKind::Plain => ValueKind::Map,
                 ObjectKind::Seq(_) => ValueKind::Seq,
                 ObjectKind::Struct(_) => ValueKind::Map,
             },
         }
     }
 
+    /// Returns `true` if the value is a number.
+    ///
+    /// To convert a value into a primitive number, use [`TryFrom`] or [`TryInto`].
+    pub fn is_number(&self) -> bool {
+        matches!(
+            self.0,
+            ValueRepr::U64(_)
+                | ValueRepr::I64(_)
+                | ValueRepr::F64(_)
+                | ValueRepr::I128(_)
+                | ValueRepr::U128(_)
+        )
+    }
+
     /// Returns `true` if the map represents keyword arguments.
     pub fn is_kwargs(&self) -> bool {
         matches!(self.0, ValueRepr::Map(_, MapType::Kwargs))
     }
 
     /// Is this value true?
     pub fn is_true(&self) -> bool {
```

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/value/object.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/value/object.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/value/ops.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/value/ops.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/value/serialize.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/value/serialize.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/vm/closure_object.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/vm/closure_object.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/vm/context.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/vm/context.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/vm/fuel.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/vm/fuel.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/vm/loop_object.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/vm/loop_object.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/vm/macro_object.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/vm/macro_object.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/vm/mod.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/vm/mod.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/local_dependencies/minijinja/src/vm/state.rs` & `minijinja-0.32.0/local_dependencies/minijinja/src/vm/state.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/LICENSE` & `minijinja-0.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/README.md` & `minijinja-0.32.0/README.md`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/hello.py` & `minijinja-0.32.0/hello.py`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/pyproject.toml` & `minijinja-0.32.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "minijinja"
-version = "0.31.1"
+version = "0.32.0"
 description = "An experimental Python binding of the Rust MiniJinja template engine."
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
     { name = "Armin Ronacher", email = "armin.ronacher@active-4.com" }
 ]
 maintainers = [
```

### Comparing `minijinja-0.31.1/python/minijinja/__init__.py` & `minijinja-0.32.0/python/minijinja/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,14 +27,20 @@
         globals=None,
         debug=True,
         fuel=None,
         undefined_behavior=None,
         auto_escape_callback=None,
         finalizer=None,
         reload_before_render=False,
+        block_start_string="{%",
+        block_end_string="%}",
+        variable_start_string="{{",
+        variable_end_string="}}",
+        comment_start_string="{#",
+        comment_end_string="#}",
     ):
         super().__init__()
         if loader is not None:
             if templates:
                 raise TypeError("Cannot set loader and templates at the same time")
             self.loader = loader
         elif templates is not None:
@@ -55,14 +61,23 @@
             self.auto_escape_callback = auto_escape_callback
         if finalizer is not None:
             self.finalizer = finalizer
         if undefined_behavior is not None:
             self.undefined_behavior = undefined_behavior
         self.reload_before_render = reload_before_render
 
+        # XXX: because this is not an atomic reconfigure if you set one of
+        # the values to a conflicting set, it will immediately error out :(
+        self.block_start_string = block_start_string
+        self.block_end_string = block_end_string
+        self.variable_start_string = variable_start_string
+        self.variable_end_string = variable_end_string
+        self.comment_start_string = comment_start_string
+        self.comment_end_string = comment_end_string
+
 
 DEFAULT_ENVIRONMENT = Environment()
 
 
 def render_str(*args, **context):
     """Shortcut to render a string with the default environment."""
     return DEFAULT_ENVIRONMENT.render_str(*args, **context)
```

### Comparing `minijinja-0.31.1/python/minijinja/_internal.py` & `minijinja-0.32.0/python/minijinja/_internal.py`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/src/environment.rs` & `minijinja-0.32.0/src/environment.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 use std::ffi::c_void;
 use std::sync::atomic::{AtomicBool, AtomicPtr, Ordering};
 use std::sync::Mutex;
 
 use minijinja::value::{Rest, Value};
-use minijinja::{context, escape_formatter, AutoEscape, Error, Source, State, UndefinedBehavior};
+use minijinja::{
+    context, escape_formatter, AutoEscape, Error, Source, State, Syntax, UndefinedBehavior,
+};
 use pyo3::conversion::AsPyPointer;
 use pyo3::exceptions::PyRuntimeError;
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyTuple};
 
 use crate::error_support::{report_unraisable, to_minijinja_error, to_py_error};
 use crate::state::bind_state;
@@ -15,19 +17,53 @@
     get_custom_autoescape, to_minijinja_value, to_python_args, to_python_value, DictLikeObject,
 };
 
 thread_local! {
     static CURRENT_ENV: AtomicPtr<c_void> = AtomicPtr::new(std::ptr::null_mut());
 }
 
+macro_rules! syntax_setter {
+    ($slf:expr, $value:expr, $field:ident, $default:expr) => {{
+        let value = $value;
+        let mut inner = $slf.inner.lock().unwrap();
+        if inner.syntax.is_none() {
+            if value == $default {
+                return Ok(());
+            }
+            inner.syntax = Some(Syntax::default());
+        }
+        if let Some(ref mut syntax) = inner.syntax {
+            if syntax.$field != value {
+                syntax.$field = value.into();
+                let new_syntax = syntax.clone();
+                inner.env.set_syntax(new_syntax).map_err(to_py_error)?;
+            }
+        }
+        Ok(())
+    }};
+}
+
+macro_rules! syntax_getter {
+    ($slf:expr, $field:ident, $default:expr) => {{
+        $slf.inner
+            .lock()
+            .unwrap()
+            .syntax
+            .as_ref()
+            .map_or($default, |x| &x.$field)
+            .into()
+    }};
+}
+
 struct Inner {
     env: minijinja::Environment<'static>,
     loader: Option<Py<PyAny>>,
     auto_escape_callback: Option<Py<PyAny>>,
     finalizer_callback: Option<Py<PyAny>>,
+    syntax: Option<Syntax>,
 }
 
 /// Represents a MiniJinja environment.
 #[pyclass(subclass, module = "minijinja._lowlevel")]
 pub struct Environment {
     inner: Mutex<Inner>,
     reload_before_render: AtomicBool,
@@ -39,14 +75,15 @@
     fn py_new() -> PyResult<Self> {
         Ok(Environment {
             inner: Mutex::new(Inner {
                 env: minijinja::Environment::new(),
                 loader: None,
                 auto_escape_callback: None,
                 finalizer_callback: None,
+                syntax: None,
             }),
             reload_before_render: AtomicBool::new(false),
         })
     }
 
     /// Enables or disables debug mode.
     #[setter]
@@ -324,15 +361,16 @@
                     return Err(PyRuntimeError::new_err("expected callback"));
                 }
                 Some(callback.into())
             }
         };
         let mut inner = self.inner.lock().unwrap();
         inner.loader = callback.clone();
-        inner.env.set_source(if let Some(callback) = callback {
+
+        let mut source = if let Some(callback) = callback {
             Source::with_loader(move |name| {
                 Python::with_gil(|py| {
                     let callback = callback.as_ref(py);
                     let rv = callback
                         .call1(PyTuple::new(py, [name]))
                         .map_err(to_minijinja_error)?;
                     if rv.is_none() {
@@ -340,15 +378,18 @@
                     } else {
                         Ok(Some(rv.to_string()))
                     }
                 })
             })
         } else {
             Source::new()
-        });
+        };
+        source.set_syntax(Syntax::default()).map_err(to_py_error)?;
+        inner.env.set_source(source);
+
         Ok(())
     }
 
     /// Returns the current loader.
     #[getter]
     pub fn get_loader(&self) -> Option<Py<PyAny>> {
         self.inner.lock().unwrap().loader.clone()
@@ -372,14 +413,74 @@
     }
 
     #[getter]
     pub fn get_reload_before_render(&self) -> bool {
         self.reload_before_render.load(Ordering::Relaxed)
     }
 
+    #[setter]
+    pub fn set_variable_start_string(&self, value: String) -> PyResult<()> {
+        syntax_setter!(self, value, variable_start, "{{")
+    }
+
+    #[getter]
+    pub fn get_variable_start_string(&self) -> String {
+        syntax_getter!(self, variable_start, "{{")
+    }
+
+    #[setter]
+    pub fn set_block_start_string(&self, value: String) -> PyResult<()> {
+        syntax_setter!(self, value, block_start, "{%")
+    }
+
+    #[getter]
+    pub fn get_block_start_string(&self) -> String {
+        syntax_getter!(self, block_start, "{%")
+    }
+
+    #[setter]
+    pub fn set_comment_start_string(&self, value: String) -> PyResult<()> {
+        syntax_setter!(self, value, comment_start, "{#")
+    }
+
+    #[getter]
+    pub fn get_comment_start_string(&self) -> String {
+        syntax_getter!(self, comment_start, "{#")
+    }
+
+    #[setter]
+    pub fn set_variable_end_string(&self, value: String) -> PyResult<()> {
+        syntax_setter!(self, value, variable_end, "}}")
+    }
+
+    #[getter]
+    pub fn get_variable_end_string(&self) -> String {
+        syntax_getter!(self, variable_end, "}}")
+    }
+
+    #[setter]
+    pub fn set_block_end_string(&self, value: String) -> PyResult<()> {
+        syntax_setter!(self, value, block_end, "%}")
+    }
+
+    #[getter]
+    pub fn get_block_end_string(&self) -> String {
+        syntax_getter!(self, block_end, "%}")
+    }
+
+    #[setter]
+    pub fn set_comment_end_string(&self, value: String) -> PyResult<()> {
+        syntax_setter!(self, value, comment_end, "#}")
+    }
+
+    #[getter]
+    pub fn get_comment_end_string(&self) -> String {
+        syntax_getter!(self, comment_end, "#}")
+    }
+
     /// Manually adds a template to the environment.
     pub fn add_template(&self, name: &str, source: &str) -> PyResult<()> {
         let mut inner = self.inner.lock().unwrap();
         if inner.env.source().is_none() {
             inner.env.set_source(Source::new());
         }
         inner
```

### Comparing `minijinja-0.31.1/src/error_support.rs` & `minijinja-0.32.0/src/error_support.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/src/state.rs` & `minijinja-0.32.0/src/state.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/src/typeconv.rs` & `minijinja-0.32.0/src/typeconv.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/tests/test_basic.py` & `minijinja-0.32.0/tests/test_basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -235,7 +235,20 @@
         assert "unexpected end of input" in e.message
         assert "1 > 1 +" not in e.message
         assert "1 > 1 +" in str(e)
         assert e.line == 1
         assert e.kind == "SyntaxError"
     else:
         assert False, "expected error"
+
+
+def test_custom_syntax():
+    env = Environment(
+        block_start_string="[%",
+        block_end_string="%]",
+        variable_start_string="{",
+        variable_end_string="}",
+        comment_start_string="/*",
+        comment_end_string="*/",
+    )
+    rv = env.render_str('[% if true %]{value}[% endif %]/* nothing */', value=42)
+    assert rv == '42'
```

### Comparing `minijinja-0.31.1/tests/test_security.py` & `minijinja-0.32.0/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/tests/test_state.py` & `minijinja-0.32.0/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.1/Cargo.lock` & `minijinja-0.32.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "aho-corasick"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e5bce8d450891e3b36f85a2230cec441fddd60e0c455b61b15bb3ffba955ca85"
+
+[[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
@@ -711,15 +717,15 @@
 
 [[package]]
 name = "globset"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "029d74589adefde59de1a0c4f4732695c32805624aec7b68d91503d4dba79afc"
 dependencies = [
- "aho-corasick",
+ "aho-corasick 0.7.20",
  "bstr 1.4.0",
  "fnv",
  "log",
  "regex",
 ]
 
 [[package]]
@@ -1141,17 +1147,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
@@ -1311,56 +1317,65 @@
 dependencies = [
  "mime",
  "unicase",
 ]
 
 [[package]]
 name = "minijinja"
-version = "0.31.1"
+version = "0.32.0"
 dependencies = [
+ "aho-corasick 1.0.0",
  "indexmap",
  "insta",
  "memo-map",
  "percent-encoding",
  "self_cell",
  "serde",
  "serde_json",
  "similar-asserts",
  "unicode-ident",
  "v_htmlescape",
 ]
 
 [[package]]
 name = "minijinja-autoreload"
-version = "0.31.1"
+version = "0.32.0"
 dependencies = [
  "minijinja",
  "notify",
 ]
 
 [[package]]
+name = "minijinja-contrib"
+version = "0.32.0"
+dependencies = [
+ "minijinja",
+ "similar-asserts",
+]
+
+[[package]]
 name = "minijinja-dis"
 version = "0.1.0"
 dependencies = [
  "argh",
  "minijinja",
 ]
 
 [[package]]
 name = "minijinja-py"
-version = "0.31.1"
+version = "0.32.0"
 dependencies = [
  "minijinja",
  "once_cell",
  "pyo3",
 ]
 
 [[package]]
 name = "minijinja-stack-ref"
-version = "0.31.1"
+version = "0.32.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
 name = "minimal"
 version = "0.1.0"
@@ -1746,17 +1761,17 @@
  "tokio",
  "tokio-stream",
  "wasm-bindgen-futures",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
@@ -1764,49 +1779,49 @@
  "pyo3-macros",
  "serde",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -1889,15 +1904,15 @@
 
 [[package]]
 name = "regex"
 version = "1.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
 dependencies = [
- "aho-corasick",
+ "aho-corasick 0.7.20",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
```

### Comparing `minijinja-0.31.1/PKG-INFO` & `minijinja-0.32.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: minijinja
-Version: 0.31.1
+Version: 0.32.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 License-File: LICENSE
 Summary: An experimental Python binding of the Rust MiniJinja template engine.
 Keywords: jinja,template-engine
 Author-email: Armin Ronacher <armin.ronacher@active-4.com>
 Maintainer-email: Armin Ronacher <armin.ronacher@active-4.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Donate, https://github.com/sponsors/mitsuhiko
-Project-URL: Issue Tracker, https://github.com/mitsuhiko/minijinja/issues
 Project-URL: Repository, https://github.com/mitsuhiko/minijinja
+Project-URL: Issue Tracker, https://github.com/mitsuhiko/minijinja/issues
+Project-URL: Donate, https://github.com/sponsors/mitsuhiko
 
 <div align="center">
   <img src="https://github.com/mitsuhiko/minijinja/raw/main/artwork/logo.png" alt="" width=320>
   <p><strong>MiniJinja for Python: a powerful template engine for Rust and Python</strong></p>
 
 [![Build Status](https://github.com/mitsuhiko/minijinja/workflows/Tests/badge.svg?branch=main)](https://github.com/mitsuhiko/minijinja/actions?query=workflow%3ATests)
 [![License](https://img.shields.io/github/license/mitsuhiko/minijinja)](https://github.com/mitsuhiko/minijinja/blob/main/LICENSE)
```

