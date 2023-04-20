# Comparing `tmp/pygame_texteditor-0.7.0.tar.gz` & `tmp/pygame_texteditor-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_texteditor-0.7.0.tar", max compression
+gzip compressed data, was "pygame_texteditor-0.7.1.tar", max compression
```

## Comparing `pygame_texteditor-0.7.0.tar` & `pygame_texteditor-0.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1092 2023-04-20 09:30:36.501202 pygame_texteditor-0.7.0/LICENSE
--rw-r--r--   0        0        0     1558 2023-04-20 09:41:04.570589 pygame_texteditor-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7159 2023-04-20 09:37:05.939641 pygame_texteditor-0.7.0/README.md
--rw-r--r--   0        0        0       36 2023-04-20 09:30:36.506702 pygame_texteditor-0.7.0/src/pygame_texteditor/__init__.py
--rw-r--r--   0        0        0     3924 2023-04-20 09:30:36.507705 pygame_texteditor-0.7.0/src/pygame_texteditor/_caret.py
--rw-r--r--   0        0        0     5964 2023-04-20 09:30:36.508791 pygame_texteditor-0.7.0/src/pygame_texteditor/_customization.py
--rw-r--r--   0        0        0     1783 2023-04-20 09:30:36.509810 pygame_texteditor-0.7.0/src/pygame_texteditor/_editor_getters.py
--rw-r--r--   0        0        0    17455 2023-04-20 09:30:36.511139 pygame_texteditor-0.7.0/src/pygame_texteditor/_input_handling_keyboard.py
--rw-r--r--   0        0        0     9639 2023-04-20 09:30:36.512448 pygame_texteditor-0.7.0/src/pygame_texteditor/_input_handling_keyboard_highlight.py
--rw-r--r--   0        0        0     8518 2023-04-20 09:30:36.513236 pygame_texteditor-0.7.0/src/pygame_texteditor/_input_handling_mouse.py
--rw-r--r--   0        0        0     1428 2023-04-20 09:30:36.513738 pygame_texteditor-0.7.0/src/pygame_texteditor/_letter_operations.py
--rw-r--r--   0        0        0     1503 2023-04-20 09:30:36.514737 pygame_texteditor-0.7.0/src/pygame_texteditor/_other.py
--rw-r--r--   0        0        0     8041 2023-04-20 09:30:36.515239 pygame_texteditor-0.7.0/src/pygame_texteditor/_rendering.py
--rw-r--r--   0        0        0     5117 2023-04-20 09:30:36.516239 pygame_texteditor-0.7.0/src/pygame_texteditor/_rendering_highlighting.py
--rw-r--r--   0        0        0     1072 2023-04-20 09:30:36.517237 pygame_texteditor-0.7.0/src/pygame_texteditor/_rendering_syntax_coloring.py
--rw-r--r--   0        0        0     1852 2023-04-20 09:30:36.518237 pygame_texteditor-0.7.0/src/pygame_texteditor/_scrollbar_vertical.py
--rw-r--r--   0        0        0     2094 2023-04-20 09:30:36.518741 pygame_texteditor-0.7.0/src/pygame_texteditor/_usage.py
--rw-r--r--   0        0        0     3428 2023-04-20 09:30:36.505702 pygame_texteditor-0.7.0/src/pygame_texteditor/ColorFormatter.py
--rw-r--r--   0        0        0      468 2023-04-20 09:30:36.519971 pygame_texteditor-0.7.0/src/pygame_texteditor/elements/colorstyles/bright.yml
--rw-r--r--   0        0        0      469 2023-04-20 09:30:36.519971 pygame_texteditor-0.7.0/src/pygame_texteditor/elements/colorstyles/dark.yml
--rw-r--r--   0        0        0    59516 2023-04-20 09:30:36.520986 pygame_texteditor-0.7.0/src/pygame_texteditor/elements/fonts/Courier.ttf
--rw-r--r--   0        0        0      211 2023-04-20 09:30:36.521992 pygame_texteditor-0.7.0/src/pygame_texteditor/elements/graphics/Scroll_Bar.png
--rw-r--r--   0        0        0    10313 2023-04-20 09:40:04.131701 pygame_texteditor-0.7.0/src/pygame_texteditor/TextEditor.py
--rw-r--r--   0        0        0     8069 1970-01-01 00:00:00.000000 pygame_texteditor-0.7.0/setup.py
--rw-r--r--   0        0        0     8089 1970-01-01 00:00:00.000000 pygame_texteditor-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-20 09:30:36.501202 pygame_texteditor-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1539 2023-04-20 09:58:02.905719 pygame_texteditor-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6933 2023-04-20 09:55:36.909461 pygame_texteditor-0.7.1/README.md
+-rw-r--r--   0        0        0       36 2023-04-20 09:30:36.506702 pygame_texteditor-0.7.1/src/pygame_texteditor/__init__.py
+-rw-r--r--   0        0        0     3924 2023-04-20 09:30:36.507705 pygame_texteditor-0.7.1/src/pygame_texteditor/_caret.py
+-rw-r--r--   0        0        0     5444 2023-04-20 09:57:05.199680 pygame_texteditor-0.7.1/src/pygame_texteditor/_customization.py
+-rw-r--r--   0        0        0     1783 2023-04-20 09:30:36.509810 pygame_texteditor-0.7.1/src/pygame_texteditor/_editor_getters.py
+-rw-r--r--   0        0        0    17455 2023-04-20 09:30:36.511139 pygame_texteditor-0.7.1/src/pygame_texteditor/_input_handling_keyboard.py
+-rw-r--r--   0        0        0     9639 2023-04-20 09:30:36.512448 pygame_texteditor-0.7.1/src/pygame_texteditor/_input_handling_keyboard_highlight.py
+-rw-r--r--   0        0        0     8518 2023-04-20 09:30:36.513236 pygame_texteditor-0.7.1/src/pygame_texteditor/_input_handling_mouse.py
+-rw-r--r--   0        0        0     1428 2023-04-20 09:30:36.513738 pygame_texteditor-0.7.1/src/pygame_texteditor/_letter_operations.py
+-rw-r--r--   0        0        0     1503 2023-04-20 09:30:36.514737 pygame_texteditor-0.7.1/src/pygame_texteditor/_other.py
+-rw-r--r--   0        0        0     8041 2023-04-20 09:30:36.515239 pygame_texteditor-0.7.1/src/pygame_texteditor/_rendering.py
+-rw-r--r--   0        0        0     5117 2023-04-20 09:30:36.516239 pygame_texteditor-0.7.1/src/pygame_texteditor/_rendering_highlighting.py
+-rw-r--r--   0        0        0     1072 2023-04-20 09:30:36.517237 pygame_texteditor-0.7.1/src/pygame_texteditor/_rendering_syntax_coloring.py
+-rw-r--r--   0        0        0     1852 2023-04-20 09:30:36.518237 pygame_texteditor-0.7.1/src/pygame_texteditor/_scrollbar_vertical.py
+-rw-r--r--   0        0        0     2094 2023-04-20 09:30:36.518741 pygame_texteditor-0.7.1/src/pygame_texteditor/_usage.py
+-rw-r--r--   0        0        0     3428 2023-04-20 09:30:36.505702 pygame_texteditor-0.7.1/src/pygame_texteditor/ColorFormatter.py
+-rw-r--r--   0        0        0      468 2023-04-20 09:30:36.519971 pygame_texteditor-0.7.1/src/pygame_texteditor/elements/colorstyles/bright.yml
+-rw-r--r--   0        0        0      469 2023-04-20 09:30:36.519971 pygame_texteditor-0.7.1/src/pygame_texteditor/elements/colorstyles/dark.yml
+-rw-r--r--   0        0        0    59516 2023-04-20 09:30:36.520986 pygame_texteditor-0.7.1/src/pygame_texteditor/elements/fonts/Courier.ttf
+-rw-r--r--   0        0        0      211 2023-04-20 09:30:36.521992 pygame_texteditor-0.7.1/src/pygame_texteditor/elements/graphics/Scroll_Bar.png
+-rw-r--r--   0        0        0    10313 2023-04-20 09:49:10.509400 pygame_texteditor-0.7.1/src/pygame_texteditor/TextEditor.py
+-rw-r--r--   0        0        0     7843 1970-01-01 00:00:00.000000 pygame_texteditor-0.7.1/setup.py
+-rw-r--r--   0        0        0     7875 1970-01-01 00:00:00.000000 pygame_texteditor-0.7.1/PKG-INFO
```

### Comparing `pygame_texteditor-0.7.0/LICENSE` & `pygame_texteditor-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/pyproject.toml` & `pygame_texteditor-0.7.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygame-texteditor"
-version = "0.7.0"
+version = "0.7.1"
 description = "A WYSIWYG-texteditor based on pygame."
 authors = ["Victor Seifert <seifert.victor@web.de>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pygame_texteditor", from="src"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -38,15 +38,14 @@
 pyperclip = ">=1.8.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 pytest = "^7.3.1"
-wheel = "^0.40.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `pygame_texteditor-0.7.0/README.md` & `pygame_texteditor-0.7.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,60 +34,48 @@
 - ```style``` - a String setting the color scheme of editor and syntax highlighting
     > Default: ```'dark'```
 - ```syntax_highlighting_python``` - a boolean enabling syntax highlighting for Python code
     > Default: ```False```
 - ```font_size``` - an integer to set for the font size.
     > Default: ```16```
 
-## Setup
+## Setup and configuration
 
-##### Minimal pygame setup
+##### Minimal texteditor setup example
 
 ```python
 import pygame
+from pygame_texteditor import TextEditor
 
+# minimal pygame setup
 pygame.init()
-screenHeight = 600
-screenWidth = 900
-screen = pygame.display.set_mode((screenWidth, screenHeight))
+screen = pygame.display.set_mode((500, 600))
 pygame.display.set_caption("Pygame")
 pygame.display.get_surface().fill((200, 200, 200))  # background coloring
-```
-
-##### Minimal texteditor setup
-
-```python
-import pygame
-from pygame_texteditor import TextEditor
-
-# parameters
-screen = pygame.display.get_surface()  # get existing pygame window/screen
-offset_X = 50  # offset from the left border of the pygame window
-offset_Y = 50  # offset from the top border of the pygame window
-editor_height = 800
-editor_width = 500
-
-
-# Instantiation
-TX = TextEditor(offset_X, offset_Y, editor_width, editor_height, screen)
-TX.set_line_numbers(True)  # optional
-TX.set_syntax_highlighting(True)  # optional
 
-while True:  # pygame-loop
-    # capture input
+# Instantiation & customization of the text editor
+TX = TextEditor(
+    offset_x=50, offset_y=50, editor_width=500, editor_height=400, screen=pygame.display.get_surface()
+)
+TX.set_line_numbers(True)
+TX.set_syntax_highlighting(True)
+TX.set_font_size(18)
+
+# TextEditor in the pygame-loop
+while True:
+    # INPUT - Mouse + Keyboard
     pygame_events = pygame.event.get()
     pressed_keys = pygame.key.get_pressed()
     mouse_x, mouse_y = pygame.mouse.get_pos()
     mouse_pressed = pygame.mouse.get_pressed()
 
-    # display editor functionality once per loop
+    # displays editor functionality once per loop
     TX.display_editor(pygame_events, pressed_keys, mouse_x, mouse_y, mouse_pressed)
+    pygame.display.flip()  # updates pygame window
 
-    # update pygame window
-    pygame.display.flip()
 ```
 
 ##### Retrieving text from the editor
 
 The editor offers the function `get_text_as_string()` to retrieve the entire text
 as a String from the editor. Lines are separated by the new line character ```\n```.
```

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/_caret.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/_caret.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/_customization.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/_customization.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import math
 import os
 import pathlib
 import re
-
 import pygame
 import yaml
 
 current_dir = os.path.dirname(__file__)
 
 
 def set_key_repetition(self, delay=300, interval=30) -> None:
@@ -35,30 +34,28 @@
 
 def set_font_size(self, size=16) -> None:
     """Sets the given size as font size and re-calculates necessary changes."""
     self.editor_font = pygame.font.Font(self.ttf_path, size=size)
     self.letter_height = size
     self.letter_width = self.editor_font.render(" ", 1, (0, 0, 0)).get_width()
     self.line_height_including_margin = self.letter_height + self.line_margin
-    self.showable_line_numbers_in_editor = int(
-        math.floor(self.editor_height / self.line_height_including_margin)
-    )
+    self.showable_line_numbers_in_editor = int(math.floor(self.editor_height / self.line_height_including_margin))
     # As the font size also influences the size of the line numbers, we need to recalculate some their spacing
-    self.line_number_width = self.editor_font.render(" ", 1, (0, 0, 0)).get_width() * 2
-    self.line_start_x = self.editor_offset_x + self.line_number_width
+    self.max_line_number_rendered = -1
+    self.update_line_number_display()
 
 
 def set_line_numbers(self, b) -> None:
     """
     Activates/deactivates showing the line numbers in the editor
     """
     self.display_line_numbers = b
     if self.display_line_numbers:
-        self.line_number_width = self.editor_font.render(" ", 1, (0, 0, 0)).get_width()
-        self.line_start_x = self.editor_offset_x + self.line_number_width
+        self.max_line_number_rendered = -1
+        self.update_line_number_display()
     else:
         self.line_number_width = 0
         self.line_start_x = self.editor_offset_x
 
 
 def set_syntax_highlighting(self, b) -> None:
     """
@@ -72,47 +69,27 @@
     def get_rgb_by_key(dict, key):
         return tuple([int(x) for x in re.findall(r"(\d{1,3})", dict[key])])
 
     try:
         with open(path_to_yaml) as file:
             color_dict = yaml.load(file, Loader=yaml.FullLoader)
 
-            self.color_coding_background = get_rgb_by_key(
-                color_dict, "codingBackgroundColor"
-            )
-            self.color_scrollbar_background = get_rgb_by_key(
-                color_dict, "codingScrollBarBackgroundColor"
-            )
+            self.color_coding_background = get_rgb_by_key(color_dict, "codingBackgroundColor")
+            self.color_scrollbar_background = get_rgb_by_key(color_dict, "codingScrollBarBackgroundColor")
             self.color_line_number_font = get_rgb_by_key(color_dict, "lineNumberColor")
-            self.color_line_number_background = get_rgb_by_key(
-                color_dict, "lineNumberBackgroundColor"
-            )
+            self.color_line_number_background = get_rgb_by_key(color_dict, "lineNumberBackgroundColor")
             self.color_text = get_rgb_by_key(color_dict, "textColor")
 
-            self.color_formatter.textColor_normal = get_rgb_by_key(
-                color_dict, "textColor_normal"
-            )
-            self.color_formatter.textColor_comments = get_rgb_by_key(
-                color_dict, "textColor_comments"
-            )
-            self.color_formatter.textColor_quotes = get_rgb_by_key(
-                color_dict, "textColor_quotes"
-            )
-            self.color_formatter.textColor_operators = get_rgb_by_key(
-                color_dict, "textColor_operators"
-            )
-            self.color_formatter.textColor_keywords = get_rgb_by_key(
-                color_dict, "textColor_keywords"
-            )
-            self.color_formatter.textColor_function = get_rgb_by_key(
-                color_dict, "textColor_function"
-            )
-            self.color_formatter.textColor_builtin = get_rgb_by_key(
-                color_dict, "textColor_builtin"
-            )
+            self.color_formatter.textColor_normal = get_rgb_by_key(color_dict, "textColor_normal")
+            self.color_formatter.textColor_comments = get_rgb_by_key(color_dict, "textColor_comments")
+            self.color_formatter.textColor_quotes = get_rgb_by_key(color_dict, "textColor_quotes")
+            self.color_formatter.textColor_operators = get_rgb_by_key(color_dict, "textColor_operators")
+            self.color_formatter.textColor_keywords = get_rgb_by_key(color_dict, "textColor_keywords")
+            self.color_formatter.textColor_function = get_rgb_by_key(color_dict, "textColor_function")
+            self.color_formatter.textColor_builtin = get_rgb_by_key(color_dict, "textColor_builtin")
 
     except FileNotFoundError:
         raise FileNotFoundError("Could not find the style file '" + path_to_yaml + "'.")
     except KeyError as e:
         raise KeyError(
             "Could not find all necessary color-keys in the style file '"
             + path_to_yaml
@@ -148,10 +125,8 @@
 
 def set_cursor_mode(self, mode: str = "blinking"):
     if mode == "blinking":
         self.static_cursor = False
     elif mode == "static":
         self.static_cursor = True
     else:
-        raise ValueError(
-            f"Value '{mode}' is not a valid cursor mode. Set either to 'blinking' or 'static'."
-        )
+        raise ValueError(f"Value '{mode}' is not a valid cursor mode. Set either to 'blinking' or 'static'.")
```

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/_editor_getters.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/_editor_getters.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/_input_handling_keyboard.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/_input_handling_keyboard.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/_input_handling_keyboard_highlight.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/_input_handling_keyboard_highlight.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/_input_handling_mouse.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/_input_handling_mouse.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/_letter_operations.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/_letter_operations.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/_other.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/_other.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/_rendering.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/_rendering.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/_rendering_highlighting.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/_rendering_highlighting.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/_rendering_syntax_coloring.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/_rendering_syntax_coloring.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/_scrollbar_vertical.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/_scrollbar_vertical.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/_usage.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/_usage.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/ColorFormatter.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/ColorFormatter.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/elements/fonts/Courier.ttf` & `pygame_texteditor-0.7.1/src/pygame_texteditor/elements/fonts/Courier.ttf`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/src/pygame_texteditor/TextEditor.py` & `pygame_texteditor-0.7.1/src/pygame_texteditor/TextEditor.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.0/setup.py` & `pygame_texteditor-0.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
                        'elements/graphics/*']}
 
 install_requires = \
 ['PyYAML>=5.3.1', 'Pygments>=2.6.1', 'pygame>=1.9.6', 'pyperclip>=1.8.1']
 
 setup_kwargs = {
     'name': 'pygame-texteditor',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': 'A WYSIWYG-texteditor based on pygame.',
-    'long_description': '# A WYSIWYG-texteditor based on pygame for pygame\n\n![PyPI](https://img.shields.io/pypi/v/pygame-texteditor?color=%233775A9&label=pypi%20package&style=plastic)\n![GitHub](https://img.shields.io/github/license/CribberSix/pygame-texteditor?style=plastic)\n\n## Introduction & examples\n\nThe text editor can be inserted into any existing pygame window.\nA minimal code example of it being activated within an existing pygame window can be found below.\n\nThe code editor comes with line numbers and syntax highlighting for python if enabled:\n\n![](./resources/example_one.png)\n\nExample with default configuration:\n\n![](./resources/example_two.png)\n\n## Usage\n\nThe texteditor takes 5 obligatory parameters and 4 optional parameters.\n\n##### Obligatory parameters\n- ```offset_X``` : integer - the offset from the left border of the pygame screen\n- ```offset_y``` : integer - the offset from the top border of the pygame screen\n- ```editor_width``` : integer - the width of texteditor\n- ```editor_height``` : integer - the height of texteditor\n- ```screen``` : pygame display surface - on which the texteditor is to be displayed\n\n##### Optional Parameters with default values\n\n- ```display_line_numbers``` - a boolean enabling showing line numbers\n    > Default: ```False```\n- ```style``` - a String setting the color scheme of editor and syntax highlighting\n    > Default: ```\'dark\'```\n- ```syntax_highlighting_python``` - a boolean enabling syntax highlighting for Python code\n    > Default: ```False```\n- ```font_size``` - an integer to set for the font size.\n    > Default: ```16```\n\n## Setup\n\n##### Minimal pygame setup\n\n```python\nimport pygame\n\npygame.init()\nscreenHeight = 600\nscreenWidth = 900\nscreen = pygame.display.set_mode((screenWidth, screenHeight))\npygame.display.set_caption("Pygame")\npygame.display.get_surface().fill((200, 200, 200))  # background coloring\n```\n\n##### Minimal texteditor setup\n\n```python\nimport pygame\nfrom pygame_texteditor import TextEditor\n\n# parameters\nscreen = pygame.display.get_surface()  # get existing pygame window/screen\noffset_X = 50  # offset from the left border of the pygame window\noffset_Y = 50  # offset from the top border of the pygame window\neditor_height = 800\neditor_width = 500\n\n\n# Instantiation\nTX = TextEditor(offset_X, offset_Y, editor_width, editor_height, screen)\nTX.set_line_numbers(True)  # optional\nTX.set_syntax_highlighting(True)  # optional\n\nwhile True:  # pygame-loop\n    # capture input\n    pygame_events = pygame.event.get()\n    pressed_keys = pygame.key.get_pressed()\n    mouse_x, mouse_y = pygame.mouse.get_pos()\n    mouse_pressed = pygame.mouse.get_pressed()\n\n    # display editor functionality once per loop\n    TX.display_editor(pygame_events, pressed_keys, mouse_x, mouse_y, mouse_pressed)\n\n    # update pygame window\n    pygame.display.flip()\n```\n\n##### Retrieving text from the editor\n\nThe editor offers the function `get_text_as_string()` to retrieve the entire text\nas a String from the editor. Lines are separated by the new line character ```\\n```.\n\nThe editor offers the function `get_text_as_list()` to retrieve the entire text as a list from the editor.\nEach String-item in the list represents one line from the editor.\n\n##### Removing text from the editor\n\nThe editor offers the function `clear_text()` to clear the editor of any text.\n\n##### Inserting text into the editor\n\nInserting text can be done by using one of the two available functions:\n1. With a list of strings in which each string represents one line, or\n2. With a string which includes linebreak characters which get parsed.\n\n```\nset_text_from_list(["First line", "Second Line.", "Third Line."]\nset_text_from_string("First line.\\nSecond line.\\nThird Line")\n```\n\n## Customization\n\n#### Cursor mode\n\nCursor mode can either be `static` or `blinking` (=default).\n\n```python\nTX = TextEditor(...)\nTX.set_cursor_mode("static")\nTX.set_cursor_mode("blinking")\n```\n\n#### Key repetition speeds\n\nWhile a key is being held, multiple key events are being triggered.\nThe delay of the first repetition as well as the interval between all sequential key triggers can be\ncustomized by using the function `set_key_repetition(delay=300, intervall=30)`.\n\nFrom the [official documentation](http://www.pygame.org/docs/ref/key.html#pygame.key.set_repeat):\n> The delay parameter is the number of milliseconds before the first repeated pygame.KEYDOWN event will be sent.\n> After that, another pygame.KEYDOWN event will be sent every interval milliseconds.\n\n\n#### Font Customization\n\nThe editor uses a ttf file to set the font for the editor. By default, the Courier monospace font is used.\n\nA custom font can be loaded with the following method, passing an *absolute* path:\n- `set_font_from_ttf("X:\\path\\to\\custom\\font.ttf")`\n\nDISCLAIMER: As the width of a letter (space) is only calculated once after setting the font_size, any fonts that are not monospace will lead to the editor not working correctly anymore, as it cannot be determined correctly between which letters the user clicked.\n\n#### Font size\n\nFont size can be customized with the command `set_font_size(size)` - the parameter is an integer\nwith the default value `16` to be able to reset it.\n\n#### Line Numbers\nLine numbers can be shown on the left side of the editor. Line numbers begin with 0 as is the Pythonian way.\n\nLine numbers can be enabled and disabled with ```set_line_numbers(Boolean)```.\n\n\n#### Syntax Highlighting\n\nThe editor comes with syntax highlighting for Python code. Tokenization is based on the ```pygment``` package.\n\nSyntax highlighting can be enabled/disabled with ```set_syntax_coloring(boolean_value)```.\n\nThe syntax colors being used are also specified in the yml style file.\n\n\n#### Color-scheme customization\n\nThe editor uses a yml file to set the color-scheme for the editor itself and for the syntax coloring.\n\nTwo styles are delivered with the editor, they can be activated respectively by:\n- `set_colorscheme("dark")`\n- `set_colorscheme("bright")`\n\nA custom style can be loaded with the following method from a created yml file:\n- `set_colorscheme_from_yaml("X:\\path\\to\\custom\\filename.yml")`\n\nAll keys must be present with values. Acceptable values are\nRGB colors in the following format: ```(255, 255, 255)``` or ```255, 255, 255```.\n\nThe following keys are required in the ```stylename.yml``` file, syntax colors are only used if syntax\nhighlighting is enabled, but are still required to be included.\n\n**Editor colors** (source: bright.yml)\n\n- `codingBackgroundColor: (255, 255, 255)`\n- `codingScrollBarBackgroundColor: (49, 50, 50)`\n- `lineNumberColor: (255, 255, 255)`\n- `lineNumberBackgroundColor: (60, 61, 61)`\n- `textColor: (255, 255, 255)`\n\n** Syntax colors** (source: bright.yml)\n\n- `textColor_normal: (0, 255, 255)`\n- `textColor_comments: (119, 115, 115)`\n- `textColor_quotes: (227, 215, 115)`\n- `textColor_operators: (237, 36, 36)`\n- `textColor_keywords: (237, 36, 36)`\n- `textColor_function: (50, 150, 36)`\n- `textColor_builtin: (50, 50, 136)`\n',
+    'long_description': '# A WYSIWYG-texteditor based on pygame for pygame\n\n![PyPI](https://img.shields.io/pypi/v/pygame-texteditor?color=%233775A9&label=pypi%20package&style=plastic)\n![GitHub](https://img.shields.io/github/license/CribberSix/pygame-texteditor?style=plastic)\n\n## Introduction & examples\n\nThe text editor can be inserted into any existing pygame window.\nA minimal code example of it being activated within an existing pygame window can be found below.\n\nThe code editor comes with line numbers and syntax highlighting for python if enabled:\n\n![](./resources/example_one.png)\n\nExample with default configuration:\n\n![](./resources/example_two.png)\n\n## Usage\n\nThe texteditor takes 5 obligatory parameters and 4 optional parameters.\n\n##### Obligatory parameters\n- ```offset_X``` : integer - the offset from the left border of the pygame screen\n- ```offset_y``` : integer - the offset from the top border of the pygame screen\n- ```editor_width``` : integer - the width of texteditor\n- ```editor_height``` : integer - the height of texteditor\n- ```screen``` : pygame display surface - on which the texteditor is to be displayed\n\n##### Optional Parameters with default values\n\n- ```display_line_numbers``` - a boolean enabling showing line numbers\n    > Default: ```False```\n- ```style``` - a String setting the color scheme of editor and syntax highlighting\n    > Default: ```\'dark\'```\n- ```syntax_highlighting_python``` - a boolean enabling syntax highlighting for Python code\n    > Default: ```False```\n- ```font_size``` - an integer to set for the font size.\n    > Default: ```16```\n\n## Setup and configuration\n\n##### Minimal texteditor setup example\n\n```python\nimport pygame\nfrom pygame_texteditor import TextEditor\n\n# minimal pygame setup\npygame.init()\nscreen = pygame.display.set_mode((500, 600))\npygame.display.set_caption("Pygame")\npygame.display.get_surface().fill((200, 200, 200))  # background coloring\n\n# Instantiation & customization of the text editor\nTX = TextEditor(\n    offset_x=50, offset_y=50, editor_width=500, editor_height=400, screen=pygame.display.get_surface()\n)\nTX.set_line_numbers(True)\nTX.set_syntax_highlighting(True)\nTX.set_font_size(18)\n\n# TextEditor in the pygame-loop\nwhile True:\n    # INPUT - Mouse + Keyboard\n    pygame_events = pygame.event.get()\n    pressed_keys = pygame.key.get_pressed()\n    mouse_x, mouse_y = pygame.mouse.get_pos()\n    mouse_pressed = pygame.mouse.get_pressed()\n\n    # displays editor functionality once per loop\n    TX.display_editor(pygame_events, pressed_keys, mouse_x, mouse_y, mouse_pressed)\n    pygame.display.flip()  # updates pygame window\n\n```\n\n##### Retrieving text from the editor\n\nThe editor offers the function `get_text_as_string()` to retrieve the entire text\nas a String from the editor. Lines are separated by the new line character ```\\n```.\n\nThe editor offers the function `get_text_as_list()` to retrieve the entire text as a list from the editor.\nEach String-item in the list represents one line from the editor.\n\n##### Removing text from the editor\n\nThe editor offers the function `clear_text()` to clear the editor of any text.\n\n##### Inserting text into the editor\n\nInserting text can be done by using one of the two available functions:\n1. With a list of strings in which each string represents one line, or\n2. With a string which includes linebreak characters which get parsed.\n\n```\nset_text_from_list(["First line", "Second Line.", "Third Line."]\nset_text_from_string("First line.\\nSecond line.\\nThird Line")\n```\n\n## Customization\n\n#### Cursor mode\n\nCursor mode can either be `static` or `blinking` (=default).\n\n```python\nTX = TextEditor(...)\nTX.set_cursor_mode("static")\nTX.set_cursor_mode("blinking")\n```\n\n#### Key repetition speeds\n\nWhile a key is being held, multiple key events are being triggered.\nThe delay of the first repetition as well as the interval between all sequential key triggers can be\ncustomized by using the function `set_key_repetition(delay=300, intervall=30)`.\n\nFrom the [official documentation](http://www.pygame.org/docs/ref/key.html#pygame.key.set_repeat):\n> The delay parameter is the number of milliseconds before the first repeated pygame.KEYDOWN event will be sent.\n> After that, another pygame.KEYDOWN event will be sent every interval milliseconds.\n\n\n#### Font Customization\n\nThe editor uses a ttf file to set the font for the editor. By default, the Courier monospace font is used.\n\nA custom font can be loaded with the following method, passing an *absolute* path:\n- `set_font_from_ttf("X:\\path\\to\\custom\\font.ttf")`\n\nDISCLAIMER: As the width of a letter (space) is only calculated once after setting the font_size, any fonts that are not monospace will lead to the editor not working correctly anymore, as it cannot be determined correctly between which letters the user clicked.\n\n#### Font size\n\nFont size can be customized with the command `set_font_size(size)` - the parameter is an integer\nwith the default value `16` to be able to reset it.\n\n#### Line Numbers\nLine numbers can be shown on the left side of the editor. Line numbers begin with 0 as is the Pythonian way.\n\nLine numbers can be enabled and disabled with ```set_line_numbers(Boolean)```.\n\n\n#### Syntax Highlighting\n\nThe editor comes with syntax highlighting for Python code. Tokenization is based on the ```pygment``` package.\n\nSyntax highlighting can be enabled/disabled with ```set_syntax_coloring(boolean_value)```.\n\nThe syntax colors being used are also specified in the yml style file.\n\n\n#### Color-scheme customization\n\nThe editor uses a yml file to set the color-scheme for the editor itself and for the syntax coloring.\n\nTwo styles are delivered with the editor, they can be activated respectively by:\n- `set_colorscheme("dark")`\n- `set_colorscheme("bright")`\n\nA custom style can be loaded with the following method from a created yml file:\n- `set_colorscheme_from_yaml("X:\\path\\to\\custom\\filename.yml")`\n\nAll keys must be present with values. Acceptable values are\nRGB colors in the following format: ```(255, 255, 255)``` or ```255, 255, 255```.\n\nThe following keys are required in the ```stylename.yml``` file, syntax colors are only used if syntax\nhighlighting is enabled, but are still required to be included.\n\n**Editor colors** (source: bright.yml)\n\n- `codingBackgroundColor: (255, 255, 255)`\n- `codingScrollBarBackgroundColor: (49, 50, 50)`\n- `lineNumberColor: (255, 255, 255)`\n- `lineNumberBackgroundColor: (60, 61, 61)`\n- `textColor: (255, 255, 255)`\n\n** Syntax colors** (source: bright.yml)\n\n- `textColor_normal: (0, 255, 255)`\n- `textColor_comments: (119, 115, 115)`\n- `textColor_quotes: (227, 215, 115)`\n- `textColor_operators: (237, 36, 36)`\n- `textColor_keywords: (237, 36, 36)`\n- `textColor_function: (50, 150, 36)`\n- `textColor_builtin: (50, 50, 136)`\n',
     'author': 'Victor Seifert',
     'author_email': 'seifert.victor@web.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pygame_texteditor-0.7.0/PKG-INFO` & `pygame_texteditor-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-texteditor
-Version: 0.7.0
+Version: 0.7.1
 Summary: A WYSIWYG-texteditor based on pygame.
 License: MIT
 Keywords: pygame,texteditor,text,editor
 Author: Victor Seifert
 Author-email: seifert.victor@web.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -63,60 +63,48 @@
 - ```style``` - a String setting the color scheme of editor and syntax highlighting
     > Default: ```'dark'```
 - ```syntax_highlighting_python``` - a boolean enabling syntax highlighting for Python code
     > Default: ```False```
 - ```font_size``` - an integer to set for the font size.
     > Default: ```16```
 
-## Setup
+## Setup and configuration
 
-##### Minimal pygame setup
+##### Minimal texteditor setup example
 
 ```python
 import pygame
+from pygame_texteditor import TextEditor
 
+# minimal pygame setup
 pygame.init()
-screenHeight = 600
-screenWidth = 900
-screen = pygame.display.set_mode((screenWidth, screenHeight))
+screen = pygame.display.set_mode((500, 600))
 pygame.display.set_caption("Pygame")
 pygame.display.get_surface().fill((200, 200, 200))  # background coloring
-```
-
-##### Minimal texteditor setup
-
-```python
-import pygame
-from pygame_texteditor import TextEditor
-
-# parameters
-screen = pygame.display.get_surface()  # get existing pygame window/screen
-offset_X = 50  # offset from the left border of the pygame window
-offset_Y = 50  # offset from the top border of the pygame window
-editor_height = 800
-editor_width = 500
-
-
-# Instantiation
-TX = TextEditor(offset_X, offset_Y, editor_width, editor_height, screen)
-TX.set_line_numbers(True)  # optional
-TX.set_syntax_highlighting(True)  # optional
 
-while True:  # pygame-loop
-    # capture input
+# Instantiation & customization of the text editor
+TX = TextEditor(
+    offset_x=50, offset_y=50, editor_width=500, editor_height=400, screen=pygame.display.get_surface()
+)
+TX.set_line_numbers(True)
+TX.set_syntax_highlighting(True)
+TX.set_font_size(18)
+
+# TextEditor in the pygame-loop
+while True:
+    # INPUT - Mouse + Keyboard
     pygame_events = pygame.event.get()
     pressed_keys = pygame.key.get_pressed()
     mouse_x, mouse_y = pygame.mouse.get_pos()
     mouse_pressed = pygame.mouse.get_pressed()
 
-    # display editor functionality once per loop
+    # displays editor functionality once per loop
     TX.display_editor(pygame_events, pressed_keys, mouse_x, mouse_y, mouse_pressed)
+    pygame.display.flip()  # updates pygame window
 
-    # update pygame window
-    pygame.display.flip()
 ```
 
 ##### Retrieving text from the editor
 
 The editor offers the function `get_text_as_string()` to retrieve the entire text
 as a String from the editor. Lines are separated by the new line character ```\n```.
```

