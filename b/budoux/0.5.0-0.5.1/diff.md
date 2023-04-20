# Comparing `tmp/budoux-0.5.0.tar.gz` & `tmp/budoux-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budoux-0.5.0.tar", last modified: Wed Mar  1 03:09:47 2023, max compression
+gzip compressed data, was "budoux-0.5.1.tar", last modified: Thu Apr 20 03:11:23 2023, max compression
```

## Comparing `budoux-0.5.0.tar` & `budoux-0.5.1.tar`

### file list

```diff
@@ -1,29 +1,38 @@
-drwxr-xr-x   0 tushuhei  (1000) tushuhei  (1000)        0 2023-03-01 03:09:47.017094 budoux-0.5.0/
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)    11357 2023-03-01 03:08:05.000000 budoux-0.5.0/LICENSE
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)      129 2023-03-01 03:08:05.000000 budoux-0.5.0/MANIFEST.in
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)     9437 2023-03-01 03:09:47.017094 budoux-0.5.0/PKG-INFO
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)     8807 2023-03-01 03:08:05.000000 budoux-0.5.0/README.md
-drwxr-xr-x   0 tushuhei  (1000) tushuhei  (1000)        0 2023-03-01 03:09:47.016094 budoux-0.5.0/budoux/
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)      908 2023-03-01 03:08:05.000000 budoux-0.5.0/budoux/__init__.py
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)     4977 2023-03-01 03:08:05.000000 budoux-0.5.0/budoux/main.py
-drwxr-xr-x   0 tushuhei  (1000) tushuhei  (1000)        0 2023-03-01 03:09:47.017094 budoux-0.5.0/budoux/models/
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)    14434 2023-03-01 03:08:05.000000 budoux-0.5.0/budoux/models/ja.json
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)    64385 2023-03-01 03:08:05.000000 budoux-0.5.0/budoux/models/zh-hans.json
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)    64671 2023-03-01 03:08:05.000000 budoux-0.5.0/budoux/models/zh-hant.json
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)     6550 2023-03-01 03:08:05.000000 budoux-0.5.0/budoux/parser.py
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)        0 2023-03-01 03:08:05.000000 budoux-0.5.0/budoux/py.typed
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)      124 2023-03-01 03:08:05.000000 budoux-0.5.0/budoux/skip_nodes.json
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)      667 2023-03-01 03:08:05.000000 budoux-0.5.0/budoux/utils.py
-drwxr-xr-x   0 tushuhei  (1000) tushuhei  (1000)        0 2023-03-01 03:09:47.016094 budoux-0.5.0/budoux.egg-info/
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)     9437 2023-03-01 03:09:47.000000 budoux-0.5.0/budoux.egg-info/PKG-INFO
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)      467 2023-03-01 03:09:47.000000 budoux-0.5.0/budoux.egg-info/SOURCES.txt
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)        1 2023-03-01 03:09:47.000000 budoux-0.5.0/budoux.egg-info/dependency_links.txt
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)       44 2023-03-01 03:09:47.000000 budoux-0.5.0/budoux.egg-info/entry_points.txt
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)      108 2023-03-01 03:09:47.000000 budoux-0.5.0/budoux.egg-info/requires.txt
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)        7 2023-03-01 03:09:47.000000 budoux-0.5.0/budoux.egg-info/top_level.txt
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)       90 2023-03-01 03:08:05.000000 budoux-0.5.0/pyproject.toml
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)     1096 2023-03-01 03:09:47.017094 budoux-0.5.0/setup.cfg
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)      614 2023-03-01 03:08:05.000000 budoux-0.5.0/setup.py
-drwxr-xr-x   0 tushuhei  (1000) tushuhei  (1000)        0 2023-03-01 03:09:47.017094 budoux-0.5.0/tests/
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)     5603 2023-03-01 03:08:05.000000 budoux-0.5.0/tests/test_main.py
--rw-r--r--   0 tushuhei  (1000) tushuhei  (1000)     6512 2023-03-01 03:08:05.000000 budoux-0.5.0/tests/test_parser.py
+drwxr-xr-x   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 03:11:23.915552 budoux-0.5.1/
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)    11357 2023-04-20 02:57:14.000000 budoux-0.5.1/LICENSE
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)      129 2023-04-20 02:57:14.000000 budoux-0.5.1/MANIFEST.in
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)     9355 2023-04-20 03:11:23.915848 budoux-0.5.1/PKG-INFO
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)     8725 2023-04-20 02:57:14.000000 budoux-0.5.1/README.md
+drwxr-xr-x   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 03:11:23.904467 budoux-0.5.1/budoux/
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)      908 2023-04-20 03:11:07.000000 budoux-0.5.1/budoux/__init__.py
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)     3218 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/html_processor.py
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)     4977 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/main.py
+drwxr-xr-x   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 03:11:23.909391 budoux-0.5.1/budoux/models/
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)    14434 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/models/ja.json
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)    64385 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/models/zh-hans.json
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)    64671 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/models/zh-hant.json
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)     4282 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/parser.py
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/py.typed
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)      124 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/skip_nodes.json
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)      667 2023-04-20 02:57:14.000000 budoux-0.5.1/budoux/utils.py
+drwxr-xr-x   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 03:11:23.907347 budoux-0.5.1/budoux.egg-info/
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)     9355 2023-04-20 03:11:23.000000 budoux-0.5.1/budoux.egg-info/PKG-INFO
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)      655 2023-04-20 03:11:23.000000 budoux-0.5.1/budoux.egg-info/SOURCES.txt
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)        1 2023-04-20 03:11:23.000000 budoux-0.5.1/budoux.egg-info/dependency_links.txt
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)       44 2023-04-20 03:11:23.000000 budoux-0.5.1/budoux.egg-info/entry_points.txt
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)       77 2023-04-20 03:11:23.000000 budoux-0.5.1/budoux.egg-info/requires.txt
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)       15 2023-04-20 03:11:23.000000 budoux-0.5.1/budoux.egg-info/top_level.txt
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)       90 2023-04-20 02:57:14.000000 budoux-0.5.1/pyproject.toml
+drwxr-xr-x   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 03:11:23.913177 budoux-0.5.1/scripts/
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 02:57:14.000000 budoux-0.5.1/scripts/__init__.py
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)     3157 2023-04-20 02:57:14.000000 budoux-0.5.1/scripts/build_model.py
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)     4946 2023-04-20 02:57:14.000000 budoux-0.5.1/scripts/encode_data.py
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)     4854 2023-04-20 02:57:14.000000 budoux-0.5.1/scripts/prepare_knbc.py
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)    13818 2023-04-20 02:57:14.000000 budoux-0.5.1/scripts/train.py
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)     3612 2023-04-20 02:57:14.000000 budoux-0.5.1/scripts/translate_model.py
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)     1063 2023-04-20 03:11:23.917767 budoux-0.5.1/setup.cfg
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)      614 2023-04-20 02:57:14.000000 budoux-0.5.1/setup.py
+drwxr-xr-x   0 tushuhei (175101) primarygroup (89939)        0 2023-04-20 03:11:23.915032 budoux-0.5.1/tests/
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)     2841 2023-04-20 02:57:14.000000 budoux-0.5.1/tests/test_html_processor.py
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)     5601 2023-04-20 02:57:14.000000 budoux-0.5.1/tests/test_main.py
+-rw-r--r--   0 tushuhei (175101) primarygroup (89939)     5369 2023-04-20 02:57:14.000000 budoux-0.5.1/tests/test_parser.py
```

### Comparing `budoux-0.5.0/LICENSE` & `budoux-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `budoux-0.5.0/PKG-INFO` & `budoux-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budoux
-Version: 0.5.0
+Version: 0.5.1
 Summary: BudouX is the successor of Budou
 Author: Shuhei Iitsuka
 Author-email: tushuhei@google.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -46,16 +46,15 @@
 - Simplified Chinese
 - Traditional Chinese
 
 ## Supported Programming languages
 
 - Python
 - [JavaScript](https://github.com/google/budoux/tree/main/javascript/)
-
-For details about the JavaScript module, please visit [JavaScript README](https://github.com/google/budoux/tree/main/javascript/README.md).
+- [Java](https://github.com/google/budoux/tree/main/java/)
 
 ## Python module
 
 ### Install
 
 ```shellsession
 $ pip install budoux
```

### Comparing `budoux-0.5.0/README.md` & `budoux-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 - Simplified Chinese
 - Traditional Chinese
 
 ## Supported Programming languages
 
 - Python
 - [JavaScript](https://github.com/google/budoux/tree/main/javascript/)
-
-For details about the JavaScript module, please visit [JavaScript README](https://github.com/google/budoux/tree/main/javascript/README.md).
+- [Java](https://github.com/google/budoux/tree/main/java/)
 
 ## Python module
 
 ### Install
 
 ```shellsession
 $ pip install budoux
```

### Comparing `budoux-0.5.0/budoux/__init__.py` & `budoux-0.5.1/budoux/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """BudouX module."""
 
 from . import parser
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 Parser = parser.Parser
 load_default_japanese_parser = parser.load_default_japanese_parser
 load_default_simplified_chinese_parser = parser.load_default_simplified_chinese_parser
 load_default_traditional_chinese_parser = parser.load_default_traditional_chinese_parser
```

### Comparing `budoux-0.5.0/budoux/main.py` & `budoux-0.5.1/budoux/main.py`

 * *Files identical despite different names*

### Comparing `budoux-0.5.0/budoux/models/ja.json` & `budoux-0.5.1/budoux/models/ja.json`

 * *Files identical despite different names*

### Comparing `budoux-0.5.0/budoux/models/zh-hans.json` & `budoux-0.5.1/budoux/models/zh-hans.json`

 * *Files identical despite different names*

### Comparing `budoux-0.5.0/budoux/models/zh-hant.json` & `budoux-0.5.1/budoux/models/zh-hant.json`

 * *Files identical despite different names*

### Comparing `budoux-0.5.0/budoux/utils.py` & `budoux-0.5.1/budoux/utils.py`

 * *Files identical despite different names*

### Comparing `budoux-0.5.0/budoux.egg-info/PKG-INFO` & `budoux-0.5.1/budoux.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budoux
-Version: 0.5.0
+Version: 0.5.1
 Summary: BudouX is the successor of Budou
 Author: Shuhei Iitsuka
 Author-email: tushuhei@google.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -46,16 +46,15 @@
 - Simplified Chinese
 - Traditional Chinese
 
 ## Supported Programming languages
 
 - Python
 - [JavaScript](https://github.com/google/budoux/tree/main/javascript/)
-
-For details about the JavaScript module, please visit [JavaScript README](https://github.com/google/budoux/tree/main/javascript/README.md).
+- [Java](https://github.com/google/budoux/tree/main/java/)
 
 ## Python module
 
 ### Install
 
 ```shellsession
 $ pip install budoux
```

### Comparing `budoux-0.5.0/setup.cfg` & `budoux-0.5.1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -22,22 +22,20 @@
 include_package_data = True
 test_suite = tests
 
 [options.extras_require]
 dev = 
 	build
 	flake8
-	html5lib
 	isort
 	numpy
-	mypy==0.971
+	mypy
 	pytest
 	toml
 	twine
-	types-html5lib
 	types-setuptools
 	yapf
 
 [options.entry_points]
 console_scripts = 
 	budoux = budoux.main:main
```

### Comparing `budoux-0.5.0/setup.py` & `budoux-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `budoux-0.5.0/tests/test_main.py` & `budoux-0.5.1/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
   def test_cmdargs_single_html(self) -> None:
     cmdargs = ['-H', '今日は<b>とても天気</b>です。']
     output = main._main(cmdargs)
 
     self.assertEqual(
         output,
         '<span style="word-break: keep-all; overflow-wrap: break-word;">'
-        '今日は<b ><wbr>とても<wbr>天気</b>です。</span>')
+        '今日は<b><wbr>とても<wbr>天気</b>です。</span>')
 
   def test_cmdargs_multi_html(self) -> None:
     cmdargs = ['-H', '今日は<b>とても天気</b>です。', 'これは<b>テスト</b>です。']
     with self.assertRaises(SystemExit) as cm:
       main._main(cmdargs)
 
     self.assertEqual(cm.exception.code, 2)
@@ -170,13 +170,13 @@
         encoding=sys.getdefaultencoding()) as f:
       sys.stdin = f
       output = main._main(["-H"])
 
     self.assertEqual(
         output,
         '<span style="word-break: keep-all; overflow-wrap: break-word;">'
-        'これは<b ><wbr>テスト</b>です。<wbr>\n'
+        'これは<b><wbr>テスト</b>です。<wbr>\n'
         '</span>')
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `budoux-0.5.0/tests/test_parser.py` & `budoux-0.5.1/tests/test_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,56 +12,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests the BudouX parser."""
 
 import os
 import sys
 import unittest
-import xml.etree.ElementTree as ET
-
-import html5lib
 
 # module hack
 LIB_PATH = os.path.join(os.path.dirname(__file__), '..')
 sys.path.insert(0, os.path.abspath(LIB_PATH))
 
 from budoux import parser  # noqa (module hack)
 
-html_parser = html5lib.HTMLParser()
-
-
-def compare_html_string(a: str, b: str) -> bool:
-  a_normalized = ET.tostring(html_parser.parse(a))
-  b_normalized = ET.tostring(html_parser.parse(b))
-  return a_normalized == b_normalized
-
-
-class TestTextContentExtractor(unittest.TestCase):
-
-  def test_output(self) -> None:
-    input = '<p><a href="#">Hello</a>, <b>World</b></p>'
-    expected = 'Hello, World'
-    extractor = parser.TextContentExtractor()
-    extractor.feed(input)
-    self.assertEqual(
-        extractor.output, expected,
-        'Text content should be extacted from the given HTML string.')
-
-
-class TestHTMLChunkResolver(unittest.TestCase):
-
-  def test_output(self) -> None:
-    input = '<p>ab<b>cde</b>f</p>'
-    expected = '<p>ab<b>c<wbr>de</b>f</p>'
-    resolver = parser.HTMLChunkResolver(['abc', 'def'])
-    resolver.feed(input)
-    self.assertTrue(
-        compare_html_string(resolver.output, expected),
-        'WBR tags should be inserted as specified by chunks.')
-
 
 class TestParser(unittest.TestCase):
   TEST_SENTENCE = 'abcdeabcd'
 
   def test_parse(self) -> None:
     p = parser.Parser({
         'UW4': {
@@ -95,54 +60,49 @@
     })
 
     input_html = 'xyzabcd'
     expected_html = (
         '<span style="word-break: keep-all; overflow-wrap: break-word;">'
         'xyz<wbr>abcd</span>')
     output_html = p.translate_html_string(input_html)
-    self.assertTrue(
-        compare_html_string(output_html, expected_html),
+    self.assertEqual(
+        output_html, expected_html,
         'Should output a html string with a SPAN parent with proper style attributes.'
     )
 
     input_html = 'xyz<script>alert(1);</script>xyzabc'
     expected_html = (
         '<span style="word-break: keep-all; overflow-wrap: break-word;">'
         'xyz<script>alert(1);</script>xyz<wbr>abc</span>')
     output_html = p.translate_html_string(input_html)
-    self.assertTrue(
-        compare_html_string(output_html, expected_html),
-        'Should pass script tags as is.')
+    self.assertEqual(output_html, expected_html,
+                     'Should pass script tags as is.')
 
     input_html = 'xyz<code>abc</code>abc'
     expected_html = (
         '<span style="word-break: keep-all; overflow-wrap: break-word;">'
         'xyz<code>abc</code><wbr>abc</span>')
     output_html = p.translate_html_string(input_html)
-    self.assertTrue(
-        compare_html_string(output_html, expected_html),
-        'Should skip some specific tags.')
+    self.assertEqual(output_html, expected_html,
+                     'Should skip some specific tags.')
 
     input_html = 'xyza<a href="#" hidden>bc</a>abc'
     expected_html = (
         '<span style="word-break: keep-all; overflow-wrap: break-word;">'
         'xyz<wbr>a<a href="#" hidden>bc</a><wbr>abc</span>')
     output_html = p.translate_html_string(input_html)
-    self.assertTrue(
-        compare_html_string(output_html, expected_html),
-        'Should not ruin attributes of child elements.')
+    self.assertEqual(output_html, expected_html,
+                     'Should not ruin attributes of child elements.')
 
     input_html = 'xyza🇯🇵🇵🇹abc'
     expected_html = (
         '<span style="word-break: keep-all; overflow-wrap: break-word;">'
         'xyz<wbr>a🇯🇵🇵🇹<wbr>abc</span>')
     output_html = p.translate_html_string(input_html)
-    self.assertTrue(
-        compare_html_string(output_html, expected_html),
-        'Should work with emojis.')
+    self.assertEqual(output_html, expected_html, 'Should work with emojis.')
 
 
 class TestDefaultParser(unittest.TestCase):
 
   def test_load_default_japanese_parser(self) -> None:
     p_ja = parser.load_default_japanese_parser()
     phrases = p_ja.parse('Google の使命は、世界中の情報を整理し、世界中の人がアクセスできて使えるようにすることです。')
```

