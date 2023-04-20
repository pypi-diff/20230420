# Comparing `tmp/doxysphinx-3.2.3.tar.gz` & `tmp/doxysphinx-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doxysphinx-3.2.3.tar", max compression
+gzip compressed data, was "doxysphinx-3.3.0.tar", max compression
```

## Comparing `doxysphinx-3.2.3.tar` & `doxysphinx-3.3.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1068 2023-04-06 14:29:01.979708 doxysphinx-3.2.3/LICENSE
--rw-r--r--   0        0        0     1078 2023-04-06 14:29:01.979708 doxysphinx-3.2.3/LICENSE.md
--rw-r--r--   0        0        0     2602 2023-04-06 14:29:01.979708 doxysphinx-3.2.3/README.md
--rw-r--r--   0        0        0      926 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/__init__.py
--rw-r--r--   0        0        0      608 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/__main__.py
--rw-r--r--   0        0        0     7409 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/cli.py
--rw-r--r--   0        0        0    12640 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/doxygen.py
--rw-r--r--   0        0        0    19836 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/html_parser.py
--rw-r--r--   0        0        0     7740 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/process.py
--rw-r--r--   0        0        0     5859 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/resources/custom.scss
--rw-r--r--   0        0        0        0 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/resources/toc_template.html.j2
--rw-r--r--   0        0        0     9683 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/resources.py
--rw-r--r--   0        0        0     2943 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/sphinx.py
--rw-r--r--   0        0        0    10875 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/toc.py
--rw-r--r--   0        0        0      527 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/utils/__init__.py
--rw-r--r--   0        0        0     2282 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/utils/contexts.py
--rw-r--r--   0        0        0     1156 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/utils/exceptions.py
--rw-r--r--   0        0        0     4967 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/utils/files.py
--rw-r--r--   0        0        0     1757 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/utils/iterators.py
--rw-r--r--   0        0        0     1431 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/utils/pathlib_fix.py
--rw-r--r--   0        0        0    12216 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/doxysphinx/writer.py
--rw-r--r--   0        0        0     4630 2023-04-06 14:29:01.995709 doxysphinx-3.2.3/pyproject.toml
--rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 doxysphinx-3.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-20 08:34:40.644352 doxysphinx-3.3.0/LICENSE
+-rw-r--r--   0        0        0     1078 2023-04-20 08:34:40.644352 doxysphinx-3.3.0/LICENSE.md
+-rw-r--r--   0        0        0     2602 2023-04-20 08:34:40.644352 doxysphinx-3.3.0/README.md
+-rw-r--r--   0        0        0      926 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/__init__.py
+-rw-r--r--   0        0        0      608 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/__main__.py
+-rw-r--r--   0        0        0     8173 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/cli.py
+-rw-r--r--   0        0        0    12644 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/doxygen.py
+-rw-r--r--   0        0        0    21980 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/html_parser.py
+-rw-r--r--   0        0        0     9102 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/process.py
+-rw-r--r--   0        0        0     5925 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/resources/custom.scss
+-rw-r--r--   0        0        0        0 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/resources/toc_template.html.j2
+-rw-r--r--   0        0        0    11513 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/resources.py
+-rw-r--r--   0        0        0     2943 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/sphinx.py
+-rw-r--r--   0        0        0    10867 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/toc.py
+-rw-r--r--   0        0        0      527 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/utils/__init__.py
+-rw-r--r--   0        0        0     2282 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/utils/contexts.py
+-rw-r--r--   0        0        0     1156 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/utils/exceptions.py
+-rw-r--r--   0        0        0     6235 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/utils/files.py
+-rw-r--r--   0        0        0     1757 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/utils/iterators.py
+-rw-r--r--   0        0        0     1431 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/utils/pathlib_fix.py
+-rw-r--r--   0        0        0      924 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/utils/rst.py
+-rw-r--r--   0        0        0    12187 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/writer.py
+-rw-r--r--   0        0        0     4193 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 doxysphinx-3.3.0/PKG-INFO
```

### Comparing `doxysphinx-3.2.3/LICENSE` & `doxysphinx-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.2.3/LICENSE.md` & `doxysphinx-3.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.2.3/README.md` & `doxysphinx-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.2.3/doxysphinx/__init__.py` & `doxysphinx-3.3.0/doxysphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.2.3/doxysphinx/__main__.py` & `doxysphinx-3.3.0/doxysphinx/__main__.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.2.3/doxysphinx/cli.py` & `doxysphinx-3.3.0/doxysphinx/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -98,18 +98,25 @@
     files. This has the implication, that the doxygen html output directory (where the rst files are generated
     to) has to live inside sphinx's input tree.
     """
     click.secho(f"doxysphinx v{metadata.version('doxysphinx')}", fg="bright_white")
 
 
 @cli.command()
+@click.option(
+    "--parallel/--sequential",
+    default=True,
+    help="parallel will separate the work among all available processor cores where possible while sequential "
+    "won't. The default is 'parallel' - 'sequential' might come in handy when debugging or tracing problems "
+    "because of the linear output.",
+)
 @click.argument("sphinx_source", type=click.Path(file_okay=False, exists=True, path_type=Path))
 @click.argument("sphinx_output", type=click.Path(file_okay=False, path_type=Path))
 @_doxygen_context()
-def build(sphinx_source: Path, sphinx_output: Path, **kwargs):
+def build(parallel: bool, sphinx_source: Path, sphinx_output: Path, **kwargs):
     """
     Build rst and copy related files for doxygen projects.
 
     SPHINX_SOURCE specifies the root of the sphinx source directory tree while SPHINX_OUTPUT specifies the root of the
     sphinx output directory tree.
     \f
 
@@ -118,37 +125,44 @@
        * when using ``sphinx-build -b html SOURCE_DIR OUTPUT_DIR ...`` the html output will be put to ``OUTPUT_DIR`` so
          so doxysphinx's ``SPHINX_OUTPUT`` should be ``OUTPUT_DIR``.
        * when using ``sphinx-build -M html`` the html output will be put to ``OUTPUT_DIR/html`` so doxysphinx's
          ``SPHINX_OUTPUT`` should be ``OUTPUT_DIR/html``.
     """
     doxy_context = DoxygenContext(**kwargs)
     _logger.info("starting build command...")
-    with TimedContext() as tc:
-        builder = Builder(sphinx_source, sphinx_output)
+    with TimedContext() as timed_scope:
+        builder = Builder(sphinx_source, sphinx_output, parallel=parallel)
         for doxy_output in _get_doxygen_outdirs(doxy_context, sphinx_source):
             builder.build(doxy_output)
-    _logger.info(f"build command done in {tc.elapsed_humanized()}.")
+    _logger.info(f"build command done in {timed_scope.elapsed_humanized()} ({timed_scope.elapsed()}).")
 
 
 @cli.command()
+@click.option(
+    "--parallel/--sequential",
+    default=True,
+    help="parallel will separate the work among all available processor cores where possible while sequential "
+    "won't. The default is 'parallel' - 'sequential' might come in handy when debugging or tracing problems "
+    "because of the linear output.",
+)
 @click.argument("sphinx_source", type=click.Path(file_okay=False, exists=True, path_type=Path))
 @click.argument("sphinx_output", type=click.Path(file_okay=False, path_type=Path))
 @_doxygen_context()
-def clean(sphinx_source: Path, sphinx_output: Path, **kwargs):
+def clean(parallel: bool, sphinx_source: Path, sphinx_output: Path, **kwargs):
     r"""
     Clean up files created by doxysphinx.
 
     SPHINX_SOURCE specifies the root of the sphinx source directory tree while SPHINX_OUTPUT specifies the root of the
     sphinx output directory tree. The doxygen html outputs are specified through INPUT (multiple possible) either
     by pointing to the doxygen html output directory or by pointing to the doxygen config file (doxyfile).
     """
     doxy_context = DoxygenContext(**kwargs)
     _logger.info("starting clean command...")
     with TimedContext() as tc:
-        cleaner = Cleaner(sphinx_source, sphinx_output)
+        cleaner = Cleaner(sphinx_source, sphinx_output, parallel=parallel)
         for doxy_output in _get_doxygen_outdirs(doxy_context, sphinx_source):
             cleaner.cleanup(doxy_output)
     _logger.info(f"clean command done in {tc.elapsed_humanized()}.")
 
 
 def _get_doxygen_outdirs(doxy_context: DoxygenContext, sphinx_source: Path) -> Iterator[Path]:
     for i in doxy_context.input:
```

### Comparing `doxysphinx-3.2.3/doxysphinx/doxygen.py` & `doxysphinx-3.3.0/doxysphinx/doxygen.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import os
 import re
 import shutil
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, List, Union
 
-import json5
+import pyjson5
 
 from doxysphinx.utils.pathlib_fix import path_is_relative_to, path_resolve
 
 ConfigDict = Dict[str, Union[str, List[str]]]
 
 
 @dataclass(frozen=True)
@@ -126,15 +126,14 @@
     if normalized_line.startswith("#"):
         return False
 
     return True
 
 
 def _parse_stderr(text: str) -> List[str]:
-
     lines = text.split(os.linesep)
     return [line.replace("warning", "Hint") for line in lines if line]
 
 
 class DoxygenSettingsValidator:
     """
     Validate doxygen settings for compatibility with doxysphinx.
@@ -171,15 +170,15 @@
     """Validation errors merged in one string."""
 
     def validate(self, config: ConfigDict, sphinx_source_dir: Path, doxygen_cwd: Path) -> bool:
         """Validate the doxygen configuration regarding the output directory, mandatory and optional settings.
 
         :param config: the imported doxyfile.
         :param sphinx_source_dir: the sphinx directory (necessary for output directory validation).
-        :param doxygen_cwd the directory for doxygen, paths from doxyfile are relative from here
+        :param doxygen_cwd: the directory for doxygen, paths from doxyfile are relative from here
         :return: False, if there is a deviation to the defined mandatory or optional settings.
         """
         if "WARNINGS" in config:
             self.validation_errors.extend(config["WARNINGS"])
 
         out_dir_validated = self._validate_doxygen_out_dirs(config, sphinx_source_dir, doxygen_cwd)
         recommended_settings_validated = self._validate_doxygen_recommended_settings(config)
@@ -285,15 +284,15 @@
     Read a doxygen javascript data file (e.g. menudata.js) and returns the data as json structure.
 
     :param js_data_file: The doxygen js data file to use.
     :return: a json like dict of the data.
     """
     data = js_data_file.read_text(encoding="utf-8")
     sanitized = re.sub(r"var .*=", "", data)
-    result: Any = json5.loads(sanitized)
+    result: Any = pyjson5.loads(sanitized)
     return result
 
 
 class DoxygenOutputPathValidator:
     """Validates doxygen html output paths."""
 
     def __init__(self) -> None:
```

### Comparing `doxysphinx-3.2.3/doxysphinx/html_parser.py` & `doxysphinx-3.3.0/doxysphinx/html_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,21 @@
 
 import logging
 import re
 from dataclasses import dataclass
 from functools import lru_cache
 from pathlib import Path
 from textwrap import dedent
-from typing import List, Optional, Protocol, Set
+from typing import Iterable, List, Optional, Protocol, Set, Tuple
 
 from lxml import html as etree  # nosec: B410
 from lxml.etree import _Element, _ElementTree  # nosec: B410
 
+from doxysphinx.utils.exceptions import ApplicationError
+
 
 @dataclass
 class HtmlParseResult:
     """Capsules a parsed and processed html tree with meta information."""
 
     html_input_file: Path
     """The html file that was parsed.
@@ -41,18 +43,19 @@
        If not just set to document title
     """
     document_title: str
     """The document title. This is the title that is visible e.g.
        in sphinx menu structure.
     """
     used_snippet_formats: Optional[Set[str]]
-    """The list of snippet format that are used inside the html tree if any.
+    """The list of snippet formats that are used inside the html tree if any.
     """
-    tree: _ElementTree
-    """The html/xml element tree.
+    tree: Optional[_ElementTree]
+    """The html/xml element tree or None if nothing was parsed because the html shouldn't be handled as mixed
+       mode content.
     """
 
 
 # noinspection PyMethodMayBeStatic,PyUnusedLocal
 class HtmlParser(Protocol):
     """Html Parser Protocol for parsing html files into a neutral format (that can be then processed further).
 
@@ -101,14 +104,19 @@
        With a "final processor" (is_final == True) processing of an element stops (no other processors considered)
        once the try_process method returns True.
     """
 
     format: str = "None"
     """The format this element processor processes... like 'rst', 'md' etc."""
 
+    # can_process_regex: str = ""
+    # """A regex that, when used on an html file checks whether the current element processor
+    #    can process that file (finds elements). This is (as optimiziation) for a quick check before loading the
+    #    complete dom (and for eventually skipping it)."""
+
     def try_process(self, element: _Element) -> bool:
         """Try to process an element.
 
         :param element: The element to check and process
         :return: Whether the "processor did it's thing"/"processing was applied" (True) or not (False)
         """
         return False
@@ -118,30 +126,31 @@
     """Element Processor for inline rst elements."""
 
     elements = ["code"]
     format = "rst"
     is_final = True
 
     rst_role_regex = re.compile(
-        r":(?P<role_name>[A-Za-z0-9-_:]*?):[`'\"](?P<role_content>.*?)[`'\"]", re.MULTILINE | re.DOTALL
+        r"\s*?:(?P<role_name>[A-Za-z0-9-_:]*?):[`'\"](?P<role_content>.*?)[`'\"]\s*?", re.MULTILINE | re.DOTALL
     )
 
     def try_process(self, element: _Element) -> bool:
         """Try to process an rst inline element into a neutralized format.
 
         :param element: The html element to process
         :return: True if the element was processed else False
         """
         # check for content
         if not element.text:
             return False
 
         # check if syntax matches sphinx/rst role
-        normalized_content = element.text.strip()
-        match = self.rst_role_regex.match(normalized_content)
+        # normalized_content = element.text.strip()
+        # match = self.rst_role_regex.match(normalized_content)
+        match = self.rst_role_regex.match(element.text)
         if match is None:
             return False
 
         role = match.group("role_name")
         content = match.group("role_content")
 
         element.tag = "snippet"
@@ -191,15 +200,14 @@
         :return: True if the element was processed else False
         """
         text = _flattened_element_text(element)
         if not text:
             return False
 
         if content := _try_parse_rst_block_content(text):
-
             # add newlines around the element tags to have the beginning and closing tags at the beginning of line each
             _ensure_newline_before_element(element)
             _ensure_newline_after_element(element)
 
             # add newlines around the content if necessary to have the content in new lines
             content = "\n" + content if not _starts_with_newline(content) else content
             content = content + "\n" if not _ends_with_newline(content) else content
@@ -218,16 +226,15 @@
 class PreToDivProcessor:
     """This Element Processor will change <pre>-tags to <div class="fragments"> tags.
 
     We do this because doxysphinx will linearize html output in the writer to have it in one line in
     the raw html directive. However this will destroy the newlines in pre tags. To overcome that
     We change the pre output here to a div with inner line divs (which is also supported by doxygen).
 
-    This should be the last processor applied (when everything else is done).
-    The reason is that it gets really hard to debug if we change the structure inbetween processors.
+    This processor is special because it should only run when any other processor has done something.
     """
 
     elements = ["pre"]
     format = ""
     is_final = True
 
     def try_process(self, element: _Element) -> bool:
@@ -309,15 +316,14 @@
             return False
 
         lines = [_flattened_element_text(e) for e in element if e.tag == "div" and e.get("class") == "line"]
 
         text = "\n".join(lines)
 
         if content := _try_parse_rst_block_content(text):
-
             # add newlines around the element tags to have the beginning and closing tags at the beginning of line each
             _ensure_newline_before_element(element)
             _ensure_newline_after_element(element)
 
             # add newlines around the content if necessary to have the content in new lines
             content = "\n" + content if not _starts_with_newline(content) else content
             content = content + "\n" if not _ends_with_newline(content) else content
@@ -450,101 +456,131 @@
 
     _logger = logging.getLogger(__name__)
 
     _processors: List[ElementProcessor] = [
         RstInlineProcessor(),
         RstBlockProcessor(),
         MarkdownRstBlockProcessor(),
-        PreToDivProcessor(),
     ]
+    """ Processors can transform/normalize the tree."""
+
+    _post_processors: List[ElementProcessor] = [PreToDivProcessor()]
+    """ Post processors are only executed when any other processor changed the tree before."""
+
+    _title_regex = re.compile(r"<title>(.*?)</title>")
 
     def __init__(self, source_directory: Path):
         """
         Create an instance of a doxygen html parser.
 
         :param source_directory:  the directory where the html files are located.
         """
         self._source_directory = source_directory
-        # self._parser = etree.HTMLParser(huge_tree=True, recover=False)
 
     def parse(self, file: Path) -> HtmlParseResult:
         """Parse a doxygen HTML file into an ElementTree and normalize its inner data to contain <rst>-tags.
 
         :param file: The html file to parse
         :type file: Path
         :return: The result of the parsing
         :rtype: ParseResult
         """
-        tree = etree.parse(file.as_posix())  # type: ignore # nosec B320
+        buffer = file.read_text()
+        tree = etree.document_fromstring(buffer).getroottree()
 
-        meta_title: str = tree.find("//title").text  # type: ignore
+        meta_title, project, title = self._read_project_and_title(buffer, file)
+
+        if self._should_parse(buffer, file):
+            used_snippet_formats = self._normalize_tree(tree)
+
+            if used_snippet_formats:
+                return HtmlParseResult(file, project, meta_title, title, used_snippet_formats, tree)
+
+        return HtmlParseResult(file, project, meta_title, title, None, None)
+
+    @staticmethod
+    def _read_project_and_title(source: str, file: Path) -> Tuple[str, str, str]:
+        title_match = DoxygenHtmlParser._title_regex.search(source)
+        if not title_match:
+            raise ApplicationError(f"html file {file} seems to have no <title>-element.")
+        meta_title: str = title_match.group(1)
         first, *_, last = meta_title.split(":")
         project = first.strip()
         title = last.strip()
+        return meta_title, project, title
 
-        used_snippet_formats = self._normalize_tree_and_get_used_formats(tree)
-
-        return HtmlParseResult(file, project, meta_title, title, used_snippet_formats, tree)
-
-    def _should_parse(self, source: str) -> bool:
-        # if no supported element (identified by closing tag) is in the file...
-        if not any(f"</{element}>" in source for element in self._all_supported_elements()):
-            # fast exit
+    def _should_parse(self, source: str, file: Path) -> bool:
+        # fail fast for doxygen htmls were no docs could be present:
+        filename = file.stem
+        if filename.endswith("_source"):  # source code listings shouldn't be parsed by us
+            return False
+        # elif filename.startswith("dir_"): # in fact dirs can have comments via @dir special command
+        #    return False
+        elif filename.startswith("functions_"):
+            return False
+        elif filename.startswith("globals_"):
+            return False
+        elif filename in ["classes", "functions", "modules", "globals", "files"]:
             return False
 
-        # get content of each element and
-
-        return True
+        # check for doxygen verbatim elements we are interested in (if none are present we can skip the file)
+        if any(s in source for s in ["<code", "<pre", '<div class="fragment"']):
+            return True
+        else:
+            return False
 
     @staticmethod
     @lru_cache(maxsize=2)
     def _all_supported_elements() -> Set[str]:
         return {e for p in DoxygenHtmlParser._processors for e in p.elements}
 
-    def _normalize_tree_and_get_used_formats(self, tree) -> Set[str]:
+    def _normalize_tree(self, tree) -> Set[str]:
         """Normalize a doxygen html tree.
 
         Searches for pre and code tags, re-formats them and creates different <snippet-*>-tags out of it.
         Will also put a newline behind the closing tag because it's necessary to have lines that can be clearly
         assigned to either html-content or snippet content (and in the un-normalized source html we've got them mixed
         at the closing tag).
         """
-        used_snipped_formats = set()
+        found_snippet_formats = set()
 
         # prefetch element candidates.
         # We do that because if there are bugs in a processor which will change the tree one might get strange
         # behaviors here (processors not applied because the elements where changed during iteration).
         # So this is just a means to make debugging easier...
         element_candidates = list(tree.iter(*self._all_supported_elements()))
 
-        # search for all supported elements in element tree
+        # search for all supported elements in element tree and apply the processors
         for element in element_candidates:
+            # apply the processors on the element
+            applied_processors = self._apply_processors(element, self._processors)
+            detected_formats = [p.format for p in applied_processors if p.format]
+            found_snippet_formats.update(detected_formats)
+
+        # if the tree was normalized (= snippets were found) apply the post-
+        if found_snippet_formats:
+            for element in element_candidates:
+                applied_post_processors = self._apply_processors(element, self._post_processors)
+                detected_formats = [p.format for p in applied_post_processors if p.format]
+                found_snippet_formats.update(detected_formats)
 
-            # try to apply each processor...
-            for processor in self._processors:
+        return found_snippet_formats
 
-                # if the current element isn't supported by the current processor skip to the next one
-                if element.tag not in processor.elements:
-                    continue
-
-                # try to process the element
-                if not self._try_process(element, processor):
-                    continue
-
-                # if it was processed add the used format to the output...
-                if processor.format:
-                    used_snipped_formats.add(processor.format)
-
-                # if the processor is final (no further processors considered) -> break the loop
-                if processor.is_final:
-                    break
-
-        return used_snipped_formats
-
-    def _try_process(self, element: _Element, processor: ElementProcessor) -> bool:
-        # fail if element isn't supported by processor
-        if element.tag not in processor.elements:
-            return False
-
-        # fail if processing returns
-        processed = processor.try_process(element)
-        return processed
+    @staticmethod
+    def _apply_processors(element: _Element, processors: List[ElementProcessor]) -> Iterable[ElementProcessor]:
+        # try to apply each processor...
+        for processor in processors:
+            # if the current element isn't supported by the current processor skip to the next one
+            if element.tag not in processor.elements:
+                continue
+
+            # process element
+            processed = processor.try_process(element)
+            if not processed:
+                continue
+
+            # return the processor because it could process the element
+            yield processor
+
+            # if the processor is final stop moving over processors...
+            if processor.is_final:
+                break
```

### Comparing `doxysphinx-3.2.3/doxysphinx/process.py` & `doxysphinx-3.3.0/doxysphinx/process.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 # =====================================================================================
 
 """
 The process module contains the :class:`Builder` and :class:`Cleaner` classes.
 
 These represent the main functionality of doxysphinx.
 """
-import hashlib
 import logging
 from pathlib import Path
-from typing import List, Type
+from typing import Iterable, List, Optional, Tuple, Type
+
+from mpire import WorkerPool
 
 from doxysphinx.html_parser import DoxygenHtmlParser, HtmlParser
 from doxysphinx.resources import DoxygenResourceProvider, ResourceProvider
 from doxysphinx.sphinx import DirectoryMapper, SphinxHtmlBuilderDirectoryMapper
+from doxysphinx.utils.files import hash_blake2b
 from doxysphinx.writer import RstWriter, Writer
 
 
 class Builder:
     """
     The Builder builds target docs-as-code files out of an existing html documentation.
 
@@ -43,14 +45,15 @@
         sphinx_source_dir: Path,
         sphinx_output_dir: Path,
         dir_mapper_type: Type[DirectoryMapper] = SphinxHtmlBuilderDirectoryMapper,
         resource_provider_type: Type[ResourceProvider] = DoxygenResourceProvider,
         parser_type: Type[HtmlParser] = DoxygenHtmlParser,
         writer_type: Type[Writer] = RstWriter,
         force_recreation: bool = False,
+        parallel=True,
     ):
         """
         Create a Builder that builds rsts for doxygen html files.
 
         :param sphinx_source_dir: The sphinx source directory where the rst files are
                                   located (most of the time something like "docs")
         :param sphinx_output_dir: The sphinx output directory where the final
@@ -64,15 +67,17 @@
         """
         self._dir_mapper = dir_mapper_type(sphinx_source_dir, sphinx_output_dir)
         self._resource_provider = resource_provider_type(self._dir_mapper)
 
         # these will be used later lazily
         self._parser_type = parser_type
         self._writer_type = writer_type
+
         self._force_recreation = force_recreation
+        self._parallel = parallel
 
     def build(self, doxygen_html_dir: Path):
         """
         Generate a rst file for each doxygen html file.
 
         Also copies necessary resources.
 
@@ -84,71 +89,94 @@
             f"copied {len(copied_resources)} resource-files " f"to {self._dir_mapper.map(doxygen_html_dir)}"
         )
 
         created_rsts = self._build(doxygen_html_dir)
         self._logger.info(f"created {len(created_rsts)} rst-files in {doxygen_html_dir}")
 
     def _build(self, doxygen_html_dir: Path) -> List[Path]:
-        result_list: List[Path] = []
         parser = self._parser_type(doxygen_html_dir)
         writer = self._writer_type(doxygen_html_dir)
+        task_args: Tuple[HtmlParser, Writer] = (parser, writer)
 
-        for html_file in doxygen_html_dir.glob("*.html"):
-            parse_result = parser.parse(html_file)
+        files_with_hashes = list(self._get_doxy_htmls_to_process_with_hashes(doxygen_html_dir))
+
+        if self._parallel:
+            with WorkerPool() as pool:
+                pool.set_shared_objects(task_args)
+                result = pool.map(self._run, files_with_hashes)
+                return result
+        else:
+            return [self._run((parser, writer), f[0], f[1]) for f in files_with_hashes]
 
-            # for now, we just write the rst parallel to the html file
+    def _get_doxy_htmls_to_process_with_hashes(self, doxygen_html_dir: Path) -> Iterable[Tuple[Path, str]]:
+        """Get all doxygen html files to process with their hashes (blake2b).
+
+        The hashes are used to implement incremental behavior. So only files which aren't the same are
+        processed.
+        """
+        for html_file in doxygen_html_dir.glob("*.html"):
             rst_file = html_file.with_suffix(".rst")
 
-            # get hash of the html file
-            html_text = html_file.read_text()
-            html_hash = hashlib.blake2b(html_text.encode("utf-8")).hexdigest()
+            hash_from_html = hash_blake2b(html_file)
 
-            # if the rst file is either not existing or the html file is not changed...
-            if self._should_build_rst(rst_file, html_hash):
-                result_list.append(writer.write(parse_result, rst_file, html_hash))
+            if not rst_file.exists():
+                yield html_file, hash_from_html
+                continue
 
-        return result_list
+            hash_from_rst = self._get_html_hash_from_rst(rst_file)
 
-    def _should_build_rst(self, rst_file: Path, html_hash: str) -> bool:
+            if hash_from_rst == hash_from_html:
+                self._logger.debug(f"skipping {html_file} as the rst was created before.")
+                continue
 
-        # always build if force mode is on
-        if self._force_recreation:
-            return True
+            yield html_file, hash_from_html
 
-        # always build if rst file is not existing
+    def _get_html_hash_from_rst(self, rst_file: Path) -> Optional[str]:
         if not rst_file.exists():
-            return True
+            return None
 
-        # read the line first line of RST file
-        with open(rst_file, encoding="utf-8") as myfile:
-            rst_content = [next(myfile) for x in range(1)]
+        with rst_file.open(encoding="utf-8") as file:
+            rst_content = [next(file) for x in range(1)]
+
+        if not rst_content:
+            return None
 
-        # return false if meta data is not found in first line
         if not rst_content[0].startswith(".. meta::"):
-            return False
+            return None
 
-        # return true if hash matches with the meta data
+        # take everything from the last ":" onwards and return it (=the hash)
         hash_from_rst = rst_content[0].split(":")[-1].rstrip()
-        if hash_from_rst != html_hash:
-            return True
+        return hash_from_rst
+
+    def _run(self, task_args: Tuple[HtmlParser, Writer], html_file: Path, html_hash: str) -> Path:
+        parser, writer = task_args
+
+        # parse the doxygen html file
+        parse_result = parser.parse(html_file)
 
-        return False
+        rst_file = html_file.with_suffix(".rst")
+
+        # write the corresponding rst file
+        result = writer.write(parse_result, rst_file, html_hash)
+
+        return result
 
 
 class Cleaner:
     """The cleaner cleans files created and copied by the builder."""
 
     _logger = logging.getLogger(__name__)
 
     def __init__(
         self,
         sphinx_source_dir: Path,
         sphinx_output_dir: Path,
         dir_mapper_type: Type[DirectoryMapper] = SphinxHtmlBuilderDirectoryMapper,
         resource_provider_type: Type[ResourceProvider] = DoxygenResourceProvider,
+        parallel: bool = True,
     ):
         """
         Create a Cleaner that will cleanup things that the :class:`Builder` created.
 
         :param sphinx_source_dir: The sphinx source directory where the rst files are
                                   located (most of the time something like "docs")
         :param sphinx_output_dir: The sphinx output directory where the final
@@ -157,14 +185,15 @@
         :param resource_provider_type: The resource provider to use.
         :param parser_type: The html parser to use.
         :param writer_type: The writer type to use.
 
         """
         self._dir_mapper = dir_mapper_type(sphinx_source_dir, sphinx_output_dir)
         self._resource_provider = resource_provider_type(self._dir_mapper)
+        self._parallel = parallel
 
     def cleanup(self, doxygen_html_dir: Path):
         """
         Clean up files that were generated by the build method.
 
         :param doxygen_html_dir: The html output directory of doxygen where the
             generated documentation is.
@@ -173,15 +202,24 @@
         deleted_resources = self._resource_provider.cleanup_resources(resource_target_dir)
         self._logger.info(f"deleted {len(deleted_resources)} resource-files from {resource_target_dir}")
 
         deleted_rsts = self._cleanup(doxygen_html_dir)
         self._logger.info(f"deleted {len(deleted_rsts)} rst-files from {doxygen_html_dir}")
 
     def _cleanup(self, doxygen_html_dir: Path) -> List[Path]:
-        result_list: List[Path] = []
-        for file_path in doxygen_html_dir.glob("*.html"):
-            target_rst_path = file_path.with_suffix(".rst")
-            if target_rst_path.exists():
-                target_rst_path.unlink()
-                result_list.append(target_rst_path)
-                self._logger.debug(f"deleted {target_rst_path}")
-        return result_list
+        files = list(doxygen_html_dir.glob("*.html"))
+
+        if self._parallel:
+            with WorkerPool() as pool:
+                pool.set_shared_objects(self._logger)
+                return pool.map(self._delete_corresponding_file, files)
+        else:
+            return [result for file in files if (result := self._delete_corresponding_file(self._logger, file))]
+
+    @staticmethod
+    def _delete_corresponding_file(logger: logging.Logger, html_file: Path) -> Optional[Path]:
+        target_rst_path = html_file.with_suffix(".rst")
+        if target_rst_path.exists():
+            target_rst_path.unlink()
+            logger.debug(f"deleted {target_rst_path}")
+            return target_rst_path
+        return None
```

### Comparing `doxysphinx-3.2.3/doxysphinx/resources/custom.scss` & `doxysphinx-3.3.0/doxysphinx/resources/custom.scss`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,18 @@
         /* left align header area + headings */
         #titlearea {
             padding-left: 0;
 
             #projectalign {
                 padding-left: 0 !important;
             }
+
+            table {
+                display: table
+            }
         }
 
         /* fix breadcrumb separator icon scaling */
         #nav-path li.navelem:before {
             transform: translateY(-1px);
         }
```

### Comparing `doxysphinx-3.2.3/doxysphinx/resources.py` & `doxysphinx-3.3.0/doxysphinx/resources.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,32 +8,27 @@
 # =====================================================================================
 """
 The resources module contains classes will do resource provisioning and patching.
 
 Resources are stylesheets, images, javascripts etc. that contemplate the html files.
 """
 
+import hashlib
 import logging
 import pkgutil
 from pathlib import Path
-from subprocess import run  # nosec: B404
-from typing import Callable, List, Optional, Protocol, Union
+from typing import Any, Callable, List, Optional, Protocol, Union
+
+import sass
 
 from doxysphinx.sphinx import DirectoryMapper
 
 # noinspection PyMethodMayBeStatic,PyUnusedLocal
-from doxysphinx.utils.exceptions import ApplicationError, PrerequisiteNotMetError
-from doxysphinx.utils.files import (
-    copy_if_different,
-    multi_glob,
-    replace_in_file,
-    stringify_paths,
-    write_file,
-)
-from doxysphinx.utils.iterators import apply_if_first
+from doxysphinx.utils.exceptions import ApplicationError
+from doxysphinx.utils.files import copy_if_different, multi_glob, stringify_paths
 
 
 class ResourceProvider(Protocol):
     """A resource provider copies/adapts necessary resources (images, stylesheets, etc.) to output."""
 
     def __init__(self, directory_mapper: DirectoryMapper):
         """
@@ -95,18 +90,18 @@
 
         :param directory_mapper: a directory mapper to use.
         """
         self._dir_mapper = directory_mapper
         self._css_scoper = CssScoper(".doxygen-content")
         self._custom_styles = self._load_custom_styles()
 
-    def _load_custom_styles(self) -> List[str]:
+    def _load_custom_styles(self) -> str:
         data: Union[bytes, None] = pkgutil.get_data(__name__, "resources/custom.scss")
         if data:
-            return data.decode("utf-8").split("\n")
+            return "\n" + data.decode("utf-8") + "\n"
         else:
             self._logger.critical("could not read custom styles out of package. Exiting.... sorry! :-(")
             exit()
 
     def provide_resources(self, resource_root: Path) -> List[Path]:
         """
         Copy doxygen html resource files (see GLOB_PATTERN below) to sphinx output.
@@ -115,19 +110,44 @@
 
         :type resource_root: the root of the resources (= usually the same folder where
             the html file are located).
         """
         target = self._dir_mapper.map(resource_root)
         target.mkdir(parents=True, exist_ok=True)
 
-        copied_files = copy_if_different(resource_root, target, *self._provisioning_glob_pattern)
+        # copy file that are different in target, except for css files that we post process later (the
+        # difference check would fail for them anyway)
+        doxygen_css = resource_root / "doxygen.css"
+        doxygen_awesome_css = resource_root / "doxygen-awesome.css"
+        css_files_for_postprocessing = [doxygen_css, doxygen_awesome_css]
+        copied_files = copy_if_different(
+            resource_root, target, *self._provisioning_glob_pattern, ignore_files=css_files_for_postprocessing
+        )
 
         self._logger.debug(f"copied files:\n{stringify_paths(copied_files)}")
 
-        self._post_process(copied_files)
+        # postprocessing (patching + sass)
+        # ... for doxygen.css
+        written_doxygen_css = self._css_scoper.scope(
+            stylesheet=doxygen_css,
+            target=target / doxygen_css.name,
+            additional_css_rules=self._custom_styles,
+            content_patch_callback=lambda s: str.replace(s, "code.JavaDocCode\n", "code.JavaDocCode {\n"),
+        )
+        if written_doxygen_css:
+            copied_files.append(written_doxygen_css)
+        # ... for doxygen_awesome.css if existing
+        if doxygen_awesome_css.exists():
+            written_doxygen_awesome_css = self._css_scoper.scope(
+                stylesheet=doxygen_awesome_css,
+                target=target / doxygen_awesome_css.name,
+                content_patch_callback=lambda s: str.replace(s, "invert()", '#{"invert()"}'),
+            )
+            if written_doxygen_awesome_css:
+                copied_files.append(written_doxygen_awesome_css)
 
         return copied_files
 
     def cleanup_resources(self, resource_root: Path) -> List[Path]:
         """Clean up any provisioned resources that were copied to sphinx output."""
         target = self._dir_mapper.map(resource_root)
         target.mkdir(parents=True, exist_ok=True)
@@ -139,45 +159,32 @@
             if target_file.exists():
                 target_file.unlink()
                 self._logger.debug(f"deleted {target_file}")
                 files_deleted.append(target_file)
 
         return files_deleted
 
-    def _post_process(self, copied_files: List[Path]):
-        # stylesheet scoping
-        apply_if_first(
-            copied_files,
-            lambda p: p.name == "doxygen.css",
-            self._patch_doxygen_stylesheet,
-        )
-        apply_if_first(
-            copied_files,
-            lambda p: p.name == "doxygen-awesome.css",
-            self._patch_doxygen_awesome_stylesheet,
-        )
-
-    def _patch_doxygen_stylesheet(self, doxygen_css_file: Path):
-        self._css_scoper.scope(
-            doxygen_css_file,
-            self._custom_styles,
-            scss_patch_callback=lambda file: replace_in_file(file, "code.JavaDocCode\n", "code.JavaDocCode {\n"),
-        )
-
-    def _patch_doxygen_awesome_stylesheet(self, doxygen_awesome_css_file: Path):
-        self._css_scoper.scope(
-            doxygen_awesome_css_file,
-            scss_patch_callback=lambda file: replace_in_file(file, "invert()", '#{"invert()"}'),
-        )
-
 
 class CssScoper:
     """Scopes css-stylesheets to a special selector.
 
-    This is done with the help of dartsass (a sass processor).
+    This is done with the help of libsass (as the sass-syntax extends css with nesting).
+
+    Our original problem was that the doxygen stylesheet and the sphinx theme stylesheets collide in some
+    ways (e.g. global styles like heading-styles etc...). We therefore needed to have a mechanism to apply
+    doxygen stylesheets only to doxygen content (not to the outer sphinx theme shell). We do this via sass,
+    because sass is css compatible but adds some nice features to it. You can for example nest styles.
+    We use that here to define an outer class and nest the whole doxygen stylesheet below it in a temporary
+    sass stylesheet which then gets compiled back to css. With this
+    we kill 2 birds with one stone:
+    * all doxygen rules are now scoped so they are not applied to the sphinx bits shell anymore....
+    * all doxygen rules now are more specialized than any of the outer sphinx style rules (they will win in browser).
+
+    In the end that means that sphinx styles are applied to sphinx bits and doxygen styles are applied to
+    doxygen bits. We still need to fix some minor issues with a custom stylesheet (which we also apply here).
     """
 
     _logger = logging.getLogger(__name__)
 
     def __init__(self, css_selector: str):
         """
         Create a new CssScoper.
@@ -185,80 +192,96 @@
         :param css_selector: The selector where the stylesheets should be scoped under.
         """
         self._selector = css_selector
 
     def scope(
         self,
         stylesheet: Path,
-        additional_css_rules: Optional[List[str]] = None,
-        scss_patch_callback: Optional[Callable[[Path], None]] = None,
-    ) -> Path:
-        """
-        Scopes a stylesheet to given selector.
-
-        The process is as follows: The original stylesheet will be moved to .original.scss.
-        Then an scss file (same name like stylesheet) that will import that .original.scss
-        file will be created. This will be compiled to the same filename as the original
-        stylesheet with the help of dartsass.
+        target: Path,
+        additional_css_rules: Optional[str] = None,
+        content_patch_callback: Optional[Callable[[str], str]] = None,
+    ) -> Optional[Path]:
+        """Scope a stylesheet to given selector.
+
+        The process is as follows: The original stylesheet is read, processed, hashed and compiled to the
+        target. If a target already exists and the hash is identical nothing is compiled and written.
 
-        :param stylesheet: The stylesheet to scope.
+        :param stylesheet: The path to a stylesheet to scope.
+        :param: target: The path to a stylesheet where the results are written to.
         :param additional_css_rules: Additional css rules to inject.
-        :param scss_patch_callback: A callback that will be called on the original file
+        :param scss_patch_callback: A callback that will be called on the original file.
+               Note: we had a bug in doxygen.css and a sass compatibility fix for doxygen-awesome that made
+               this mechanism necessary. With one of the recent doxygen versions the doxygen.css bug was fixed
+               however we still keep it here some time.
         :return: The path to the written stylesheet (should be identical to stylesheet).
         """
-        # move original stylesheet to .original.scss
-        original = stylesheet.with_suffix(".original.scss")
-        self._move(stylesheet, original)
+        if stylesheet == target:
+            raise ApplicationError(f"source ({stylesheet}) and target ({target}) stylesheets cannot be identical.")
 
-        # execute patch callback if any
-        if scss_patch_callback:
-            scss_patch_callback(original)
+        # load stylesheet and apply patches
+        css_content = stylesheet.read_text()
 
-        # create .scss (sass) file that will import the .original.scss but scoped to
-        # the selector
-        content = [f"{self._selector} {{", f'   @import "{original.name}";', "}", ""]
+        if content_patch_callback:
+            css_content = content_patch_callback(css_content)
 
-        if additional_css_rules:  # add additional styles if any
-            content.extend(additional_css_rules)
+        # create .scss (sass) content scoped to the selector
+        content = f"{self._selector} {{\n{css_content}\n}}\n"  # here we scope the content to a given css selector
 
-        sass_stylesheet = stylesheet.with_suffix(".scss")
-        write_file(sass_stylesheet, content)
+        if additional_css_rules:
+            content += additional_css_rules
 
-        # compile scoped scss to css (thereby retaining original file)
-        self._call_sass(sass_stylesheet, stylesheet)
+        new_hash_digest = hashlib.blake2b(content.encode("utf-8")).hexdigest()
 
-        # remove scoping from html element (if any) where typically variables are
-        # stored, because this will only work globally.
-        replace_in_file(stylesheet, f"{self._selector} html {{", "html {")
+        old_hash_digest = self._read_hash_digest(target)
+        if new_hash_digest == old_hash_digest:
+            return None
 
-        self._logger.debug(f"scoped stylesheet '{stylesheet}' to selector '{self._selector}'.")
-        return stylesheet
+        # add hash digest to content
+        content = (
+            f"/* {new_hash_digest} <- doxysphinx hash digest for the original input css that leads"
+            f"to the css below */\n{content}"
+        )
+
+        # compile the scss to a css
+        compiled_css: Any = sass.compile(
+            string=content,
+            output_style="expanded",
+            indented=False,
+            include_paths=[str(stylesheet.parent)],
+        )
+
+        # the sass compiler does also scope the html element (where typically css variables are
+        # stored). We need to remove that scoping again because it will only work if it's in global scope.
+        compiled_css = compiled_css.replace(f"{self._selector} html {{", "html {")
+
+        # write stylesheet
+        target.write_text(compiled_css)
+
+        self._logger.debug(
+            f"scoped original stylesheet '{stylesheet}' to selector '{self._selector}' in target '{target}'."
+        )
+        return target
+
+    @staticmethod
+    def _read_hash_digest(file: Path) -> str:
+        if not file.exists():
+            return ""
+
+        digest_line: str
+        with open(file, mode="r", encoding="utf") as f:
+            digest_line = f.readline()
+            # sometimes sass renders an @charset css directive which has to be on the first line (by css spec)
+            # so in that case our hash digest is on the second line and we need to adapt to that...
+            if digest_line.startswith("@charset"):
+                digest_line = f.readline()
+
+        if not digest_line.startswith("/* "):
+            return ""
+
+        digest = digest_line[3:].split(" <- ")[0]
+        return digest
 
     @staticmethod
     def _move(original: Path, new: Path):
         if new.exists():
             new.unlink()
         original.rename(new)
-
-    @staticmethod
-    def _call_sass(sass_file: Path, output_css_file: Path):
-        try:
-            result = run(["sass", sass_file, output_css_file])  # nosec: B607, B603
-            result.check_returncode()
-
-            if result.stderr:
-                message = (
-                    "Sass Compiler had errors "
-                    f"(call: sass {sass_file}"  # type: ignore [str-bytes-safe]
-                    f"{output_css_file}): \n{result.stderr}"
-                )
-
-                raise ApplicationError(message)
-        except FileNotFoundError:
-            raise PrerequisiteNotMetError(
-                "The dart-sass-compiler 'sass' wasn't found. This is a prerequisite "
-                "for us to fix stylesheet issues when integrating doxygen html "
-                "documentation with sphinx. Please install it either by using the "
-                "official guide (https://sass-lang.com/install) or by downloading the "
-                "binary directly and putting it on your $PATH "
-                "(https://github.com/sass/dart-sass/releases)."
-            )
```

### Comparing `doxysphinx-3.2.3/doxysphinx/sphinx.py` & `doxysphinx-3.3.0/doxysphinx/sphinx.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.2.3/doxysphinx/toc.py` & `doxysphinx-3.3.0/doxysphinx/toc.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,17 +149,17 @@
         self._doxy_html_template: Tuple[str, str] = self._parse_template()
 
         # create rst files for those structural dummies doxygen is using...
         structural_dummies = [e for e in self._flatten_tree(self._menu) if e.is_structural_dummy]
         apply(structural_dummies, self._prepare_structural_dummy)
         apply(structural_dummies, self._create_toc_file_for_structural_dummy)
 
-        self._menu_lookup: Dict[str, _MenuEntry] = dict(
-            {e.docname: e for e in self._flatten_tree(self._menu) if not e.is_leaf}
-        )
+        self._menu_lookup: Dict[str, _MenuEntry] = {
+            e.docname: e for e in self._flatten_tree(self._menu) if not e.is_leaf
+        }
 
     def _parse_template(self) -> Tuple[str, str]:
         """Parse a "doxygen html template shell" out of the index.html file.
 
         :return: A Tuple containing the doxygen html before the content area and the content after the content area.
         """
         # load html file as string and remove the newline chars
@@ -190,15 +190,14 @@
 
     def _prepare_structural_dummy(self, structural_dummy: _MenuEntry):
         clean_title = structural_dummy.title.replace(" ", "_").lower()
         toc_docname = f"{structural_dummy.docname}_{clean_title}"
         structural_dummy.docname = toc_docname
 
     def _create_toc_file_for_structural_dummy(self, structural_dummy: _MenuEntry):
-
         prefix, suffix = self._doxy_html_template
 
         content = [
             f".. title:: {structural_dummy.title}",
             "",
             f"{structural_dummy.title}",
             f"{'-' * len(structural_dummy.title)}",
```

### Comparing `doxysphinx-3.2.3/doxysphinx/utils/__init__.py` & `doxysphinx-3.3.0/doxysphinx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.2.3/doxysphinx/utils/contexts.py` & `doxysphinx-3.3.0/doxysphinx/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.2.3/doxysphinx/utils/exceptions.py` & `doxysphinx-3.3.0/doxysphinx/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.2.3/doxysphinx/utils/iterators.py` & `doxysphinx-3.3.0/doxysphinx/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.2.3/doxysphinx/utils/pathlib_fix.py` & `doxysphinx-3.3.0/doxysphinx/utils/pathlib_fix.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.2.3/doxysphinx/writer.py` & `doxysphinx-3.3.0/doxysphinx/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         html_file = parse_result.html_input_file
 
         preamble = self._preamble(title, meta_title)
 
         toc = self._toc_gen.generate_toc_for(html_file)
         content = []
 
-        if parse_result.used_snippet_formats:
+        if tree:
             # for rst containing htmls we create a mixed (raw html + rst block) rst
             self._logger.debug(f"writing mixed rst for {parse_result.html_input_file}")
             content.extend(self._mixed_rst(tree))
         else:
             # for normal (non-rst-containing) htmls we create a raw html import rst
             self._logger.debug(f"writing raw placeholder rst for {parse_result.html_input_file}")
             content.extend(self._raw_placeholder_rst(html_file))
```

### Comparing `doxysphinx-3.2.3/pyproject.toml` & `doxysphinx-3.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ##
 ##  Author(s):
 ##  - Markus Braun, :em engineering methods AG (contracted by Robert Bosch GmbH)
 ## =====================================================================================
 
 [tool.poetry]
 name = "doxysphinx"
-version = "3.2.3"
+version = "3.3.0"
 description = "Integrates doxygen html documentation with sphinx."
 authors = [
     "Nirmal Sasidharan <nirmal.sasidharan@de.bosch.com>",
     "Markus Braun <markus.braun@em.ag>",
     "Aniket Salve <aniketdilip.salve@bosch.com>",
 ]
 maintainers = ["Nirmal Sasidharan <nirmal.sasidharan@de.bosch.com>"]
@@ -32,67 +32,63 @@
     "Topic :: Text Processing :: Markup :: reStructuredText",
     "Topic :: Documentation :: Sphinx",
     "Topic :: Documentation",
 ]
 packages = [{ include = "doxysphinx" }]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-lxml = "^4.9.1"
-json5 = "^0.9.8"
-colorama = { version = "^0.4.5", platform = "windows" }
+python = ">=3.8,<3.12"
+lxml = "^4.9.2"
+colorama = { version = "^0.4.6", platform = "windows" }
 click = "^8.1.3"
 click-log = "^0.4.0"
 pyparsing = "^3.0.9"
+mpire = "^2.6.0"
+pyjson5 = "^1.6.2"
+libsass = "^0.22.0"
 
-[tool.poetry.group.dev.dependencies]
-lxml-stubs = "^0.3.1"
-pytest = "^7.1.2"
+[tool.poetry.group.sphinx.dependencies]
 sphinx = "^4.5.0"
-Pillow = "^9.2.0"
-sphinx-rtd-theme = "^1.0.0"
+Pillow = "^9.3.0"
+sphinx-rtd-theme = "^1.1.1"
 sphinxcontrib-needs = "^0.7.9"
 sphinxcontrib-plantuml = "^0.22"
-sphinxcontrib-doxylink = "^1.12.0"
+sphinxcontrib-doxylink = "^1.12.2"
 sphinx-test-reports = "^0.3.7"
 sphinx-theme = "^1.0"
-sphinx-copybutton = "^0.5.0"
-pex = "^2.1.99"
+sphinx-copybutton = "^0.5.1"
 sphinx-book-theme = "^0.2.0"
-snakeviz = "^2.1.1"
 myst-parser = "^0.17.2"
-pytest-cov = "^3.0.0"
-pre-commit = "^2.20.0"
-flake8 = "^4.0.1"
-flake8-bugbear = "^22.7.1"
-black = "^22.6.0"
-isort = "^5.12.0"
-bandit = "^1.7.4"
-safety = "^1.10.3"
-flake8-comprehensions = "^3.10.0"
-flake8-simplify = "^0.19.2"
-mypy = "^0.942"
 toml = "^0.10.2"
-types-PyYAML = "^6.0.10"
-cohesion = "^1.0.0"
-pydocstyle = "^6.1.1"
 sphinx_design = "^0.1.0"
-sphinx-toolbox = "^3.1.2"
-flake8-docstrings = "^1.6.0"
+sphinx-toolbox = "^3.2.0"
+sphinx-autoapi = "^2.0.0"
+
+[tool.poetry.group.typedefs.dependencies]
+lxml-stubs = "^0.4.0"
+types-pyyaml = "^6.0.12.2"
+
+# ci build dependencies
+[tool.poetry.group.ci]
+optional = true
+[tool.poetry.group.ci.dependencies]
+pytest = "^7.2.2"
+pytest-cov = "^4.0.0"
 pytest-emoji = "^0.2.0"
 pytest-md = "^0.2.0"
-commitizen = "^2.29.0"
-sphinx-autoapi = "^2.0.0"
+pex = "^2.1.131"
+pre-commit = "^3.2.2"
+commitizen = "^2.42.1"
 
 [tool.poetry.scripts]
 doxysphinx = "doxysphinx.cli:cli"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "3.2.3"
+version = "3.3.0"
 tag_format = "v$version"
 version_files = ["pyproject.toml:^version"]
 bump_message = """chore(release): release $current_version → $new_version by commitizen [skip-ci]
 
 Signed-off-by: github-actions <actions@github.com>
 """
 
@@ -103,30 +99,14 @@
 [tool.pytest.ini_options]
 log_level = "DEBUG"
 testpaths = ["tests"]
 junit_logging = "out-err"
 markers = ["speed: manual speed tests"]
 addopts = "-m 'not speed'"
 
-[tool.semantic_release]
-version_source = "commit"
-version_variable = ["pyproject.toml:version"]
-changelog_file = "CHANGELOG.md"
-branch = "main"
-commit_message = """chore(release): release {version} published by python-semantic-release [skip ci]
-
-Signed-off-by: github-actions <actions@github.com>
-"""
-commit_author = "github-actions <actions@github.com>"
-# everything following is deactivated: we only want python-semantic-release to create the changelog and the version tags (because everything else is quite buggy)
-upload_to_pypi = false
-upload_to_release = false
-build_command = false
-remove_dist = false
-
 [tool.black]
 line-length = 120
 target-version = ['py38']
 # black doesn't need further excludes because it honors the .gitignore file
 extend-exclude = "(docs/)|(demo/)|(\\.vscode)|(\\.idea)|(\\.devcontainer)"
 
 [tool.isort]
@@ -160,10 +140,28 @@
 
 [tool.pydocstyle]
 match_dir = "doxysphinx"
 ignore = "D301,D213,D212,D203"
 
 [tool.pylint]
 disable = ["logging-fstring-interpolation"]
+extension-pkg-allow-list = ["lxml", "mpire"]
 
 [tool.pylint.FORMAT]
 max-line-length = 120
+
+[tool.pyright]
+exclude = [
+    ".build",
+    ".cache",
+    ".devcontainer",
+    ".github",
+    ".idea",
+    ".mypy_cache",
+    ".pytest_cache",
+    ".venv",
+    ".vscode",
+    "demo",
+    "dist",
+    "docs",
+    "external",
+]
```

### Comparing `doxysphinx-3.2.3/PKG-INFO` & `doxysphinx-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: doxysphinx
-Version: 3.2.3
+Version: 3.3.0
 Summary: Integrates doxygen html documentation with sphinx.
 Home-page: https://github.com/boschglobal/doxysphinx
 License: MIT
 Keywords: DaC,docs-as-code,doxygen,sphinx
 Author: Nirmal Sasidharan
 Author-email: nirmal.sasidharan@de.bosch.com
 Maintainer: Nirmal Sasidharan
 Maintainer-email: nirmal.sasidharan@de.bosch.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
-Requires-Dist: colorama (>=0.4.5,<0.5.0) ; sys_platform == "windows"
-Requires-Dist: json5 (>=0.9.8,<0.10.0)
-Requires-Dist: lxml (>=4.9.1,<5.0.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0) ; sys_platform == "windows"
+Requires-Dist: libsass (>=0.22.0,<0.23.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: mpire (>=2.6.0,<3.0.0)
+Requires-Dist: pyjson5 (>=1.6.2,<2.0.0)
 Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
 Project-URL: Documentation, https://boschglobal.github.io/doxysphinx/
 Project-URL: Repository, https://github.com/boschglobal/doxysphinx
 Description-Content-Type: text/markdown
 
 <!--
 =====================================================================================
```

