# Comparing `tmp/jupyter_ai_magics-0.5.0.tar.gz` & `tmp/jupyter_ai_magics-0.6.0.tar.gz`

## Comparing `jupyter_ai_magics-0.5.0.tar` & `jupyter_ai_magics-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.5.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.5.0/setup.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.5.0/jupyter_ai_magics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.5.0/jupyter_ai_magics/_version.py
--rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.5.0/jupyter_ai_magics/magics.py
--rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.5.0/jupyter_ai_magics/providers.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.5.0/jupyter_ai_magics/tests/__init__.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.5.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.5.0/LICENSE
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.5.0/README.md
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/setup.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/jupyter_ai_magics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/jupyter_ai_magics/_version.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/jupyter_ai_magics/exception.py
+-rw-r--r--   0        0        0     8841 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/jupyter_ai_magics/magics.py
+-rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/jupyter_ai_magics/providers.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/jupyter_ai_magics/tests/__init__.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/LICENSE
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/README.md
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/PKG-INFO
```

### Comparing `jupyter_ai_magics-0.5.0/package.json` & `jupyter_ai_magics-0.6.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.6.0'"}*

```diff
@@ -16,9 +16,9 @@
         "type": "git",
         "url": "https://github.com/jupyterlab/jupyter-ai.git"
     },
     "scripts": {
         "dev-install": "pip install -e \".[all]\"",
         "dev-uninstall": "pip uninstall jupyter_ai_magics -y"
     },
-    "version": "0.5.0"
+    "version": "0.6.0"
 }
```

### Comparing `jupyter_ai_magics-0.5.0/jupyter_ai_magics/magics.py` & `jupyter_ai_magics-0.6.0/jupyter_ai_magics/magics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import os
 import json
+import os
 import warnings
 from typing import Optional
 
 from importlib_metadata import entry_points
 from IPython import get_ipython
 from IPython.core.magic import Magics, magics_class, line_cell_magic
 from IPython.core.magic_arguments import magic_arguments, argument, parse_argstring
@@ -15,23 +15,47 @@
 MODEL_ID_ALIASES = {
     "gpt2": "huggingface_hub:gpt2",
     "gpt3": "openai:text-davinci-003",
     "chatgpt": "openai-chat:gpt-3.5-turbo",
     "gpt4": "openai-chat:gpt-4",
 }
 
+class TextWithMetadata(object):
+
+    def __init__(self, text, metadata):
+        self.text = text
+        self.metadata = metadata
+
+    def _repr_mimebundle_(self, include=None, exclude=None):
+        return ({'text/plain': self.text}, self.metadata)
+
 DISPLAYS_BY_FORMAT = {
+    "code": None,
     "html": HTML,
     "markdown": Markdown,
     "math": Math,
     "md": Markdown,
     "json": JSON,
-    "raw": None
+    "text": TextWithMetadata
 }
 
+MARKDOWN_PROMPT_TEMPLATE = '{prompt}\n\nProduce output in markdown format only.'
+
+PROMPT_TEMPLATES_BY_FORMAT = {
+    "code": '{prompt}\n\nProduce output as source code only, with no text or explanation before or after it.',
+    "html": '{prompt}\n\nProduce output in HTML format only, with no markup before or afterward.',
+    "markdown": MARKDOWN_PROMPT_TEMPLATE,
+    "md": MARKDOWN_PROMPT_TEMPLATE,
+    "math": '{prompt}\n\nProduce output in LaTeX format only, with $$ at the beginning and end.',
+    "json": '{prompt}\n\nProduce output in JSON format only, with nothing before or after it.',
+    "text": '{prompt}' # No customization
+}
+
+
+
 class FormatDict(dict):
     """Subclass of dict to be passed to str#format(). Suppresses KeyError and
     leaves replacement field unchanged if replacement field is not associated
     with a value."""
     def __missing__(self, key): 
         return key.join("{}")
 
@@ -101,15 +125,15 @@
 
     @magic_arguments()
     @argument('model_id',
                 help="""Model to run, specified as a model ID that may be
                 optionally prefixed with the ID of the model provider, delimited
                 by a colon.""")
     @argument('-f', '--format',
-                choices=["markdown", "html", "json", "math", "md", "raw"],
+                choices=["code", "markdown", "html", "json", "math", "md", "text"],
                 nargs="?",
                 default="markdown",
                 help="""IPython display to use when rendering output. [default="markdown"]""")
     @argument('-r', '--reset',
                 action="store_true",
                 help="""Clears the conversation transcript used when interacting
                 with an OpenAI chat model provider. Does nothing with other
@@ -124,14 +148,17 @@
         # parse arguments
         args = parse_argstring(self.ai, line)
         if cell is None:
             prompt = ' '.join(args.prompt)
         else:
             prompt = cell
         
+        # Apply a prompt template.
+        prompt = PROMPT_TEMPLATES_BY_FORMAT[args.format].format(prompt = prompt)
+
         # determine provider and local model IDs
         provider_id, local_model_id = self._decompose_model_id(args.model_id)
         Provider = self._get_provider(provider_id)
         if Provider is None:
             return f"Cannot determine model provider from model ID {args.model_id}."
 
         # if `--reset` is specified, reset transcript and return early
@@ -166,16 +193,36 @@
 
         # if openai-chat, append exchange to transcript
         if provider_id == "openai-chat":
             self._append_exchange_openai(prompt, output)
 
         # build output display
         DisplayClass = DISPLAYS_BY_FORMAT[args.format]
+
+        md = {
+            "jupyter_ai": {
+                "provider_id": provider_id,
+                "model_id": local_model_id
+            }
+        }
+
+        # if the user wants code, add another cell with the output.
+        if args.format == 'code':
+            # Strip leading and trailing triple-backticks
+            output = output.removeprefix('```\n').removesuffix('\n```')
+            new_cell_payload = dict(
+                source='set_next_input',
+                text=output,
+                replace=False,
+            )
+            ip.payload_manager.write_payload(new_cell_payload)
+            return HTML('AI generated code inserted below &#11015;&#65039;', metadata=md); # No output from the AI cell
+
         if DisplayClass is None:
             return output
         if args.format == 'json':
             # JSON display expects a dict, not a JSON string
             output = json.loads(output)
-        output_display = DisplayClass(output)
+        output_display = DisplayClass(output, metadata=md)
 
         # finally, display output display
         return output_display
```

### Comparing `jupyter_ai_magics-0.5.0/jupyter_ai_magics/providers.py` & `jupyter_ai_magics-0.6.0/jupyter_ai_magics/providers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.5.0/.gitignore` & `jupyter_ai_magics-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.5.0/LICENSE` & `jupyter_ai_magics-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.5.0/pyproject.toml` & `jupyter_ai_magics-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 dependencies = [
     "ipython",
     "pydantic",
     "importlib_metadata~=5.2.0",
-    "langchain~=0.0.115"
+    "langchain~=0.0.144"
 ]
 
 [project.optional-dependencies]
 test = [
     "coverage",
     "pytest",
     "pytest-asyncio",
```

### Comparing `jupyter_ai_magics-0.5.0/PKG-INFO` & `jupyter_ai_magics-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai_magics
-Version: 0.5.0
+Version: 0.6.0
 Summary: Jupyter AI magics Python package. Not published on NPM.
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -44,15 +44,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata~=5.2.0
 Requires-Dist: ipython
-Requires-Dist: langchain~=0.0.115
+Requires-Dist: langchain~=0.0.144
 Requires-Dist: pydantic
 Provides-Extra: all
 Requires-Dist: ai21; extra == 'all'
 Requires-Dist: anthropic; extra == 'all'
 Requires-Dist: boto3; extra == 'all'
 Requires-Dist: cohere; extra == 'all'
 Requires-Dist: huggingface-hub; extra == 'all'
```

