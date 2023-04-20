# Comparing `tmp/pygame-texteditor-0.6.7.tar.gz` & `tmp/pygame_texteditor-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pygame-texteditor-0.6.7.tar", last modified: Tue Jun 14 13:52:18 2022, max compression
+gzip compressed data, was "pygame_texteditor-0.7.0.tar", max compression
```

## Comparing `pygame-texteditor-0.6.7.tar` & `pygame_texteditor-0.7.0.tar`

### file list

```diff
@@ -1,39 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-06-14 13:52:18.517904 pygame-texteditor-0.6.7/
--rw-rw-rw-   0        0        0     1090 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/LICENSE
--rw-rw-rw-   0        0        0      176 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/MANIFEST.in
--rw-rw-rw-   0        0        0     7044 2022-06-14 13:52:18.517404 pygame-texteditor-0.6.7/PKG-INFO
--rw-rw-rw-   0        0        0     6268 2022-06-14 13:50:35.000000 pygame-texteditor-0.6.7/README.md
-drwxrwxrwx   0        0        0        0 2022-06-14 13:52:18.488903 pygame-texteditor-0.6.7/pygame_texteditor/
--rw-rw-rw-   0        0        0     2678 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/ColorFormatter.py
--rw-rw-rw-   0        0        0     9309 2022-06-14 13:45:22.000000 pygame-texteditor-0.6.7/pygame_texteditor/TextEditor.py
--rw-rw-rw-   0        0        0       34 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/__init__.py
--rw-rw-rw-   0        0        0     3545 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/_caret.py
--rw-rw-rw-   0        0        0     4820 2022-06-14 13:44:06.000000 pygame-texteditor-0.6.7/pygame_texteditor/_customization.py
--rw-rw-rw-   0        0        0     1622 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/_editor_getters.py
--rw-rw-rw-   0        0        0    15572 2022-06-14 13:44:48.000000 pygame-texteditor-0.6.7/pygame_texteditor/_input_handling_keyboard.py
--rw-rw-rw-   0        0        0     8732 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/_input_handling_keyboard_highlight.py
--rw-rw-rw-   0        0        0     7266 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/_input_handling_mouse.py
--rw-rw-rw-   0        0        0     1501 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/_letter_operations.py
--rw-rw-rw-   0        0        0     1484 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/_other.py
--rw-rw-rw-   0        0        0     5437 2022-06-14 13:41:15.000000 pygame-texteditor-0.6.7/pygame_texteditor/_rendering.py
--rw-rw-rw-   0        0        0     4583 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/_rendering_highlighting.py
--rw-rw-rw-   0        0        0     1198 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/_rendering_syntax_coloring.py
--rw-rw-rw-   0        0        0     1387 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/_scrollbar_vertical.py
--rw-rw-rw-   0        0        0     2290 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/_usage.py
-drwxrwxrwx   0        0        0        0 2022-06-14 13:52:18.468904 pygame-texteditor-0.6.7/pygame_texteditor/elements/
-drwxrwxrwx   0        0        0        0 2022-06-14 13:52:18.512405 pygame-texteditor-0.6.7/pygame_texteditor/elements/colorstyles/
--rw-rw-rw-   0        0        0      468 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/elements/colorstyles/bright.yml
--rw-rw-rw-   0        0        0      469 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/elements/colorstyles/dark.yml
-drwxrwxrwx   0        0        0        0 2022-06-14 13:52:18.513405 pygame-texteditor-0.6.7/pygame_texteditor/elements/fonts/
--rw-rw-rw-   0        0        0    59516 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/elements/fonts/Courier.ttf
-drwxrwxrwx   0        0        0        0 2022-06-14 13:52:18.516405 pygame-texteditor-0.6.7/pygame_texteditor/elements/graphics/
--rw-rw-rw-   0        0        0      211 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/elements/graphics/Scroll_Bar.png
--rw-rw-rw-   0        0        0      151 2022-06-14 11:55:11.000000 pygame-texteditor-0.6.7/pygame_texteditor/elements/graphics/Trennzeichen.png
-drwxrwxrwx   0        0        0        0 2022-06-14 13:52:18.510404 pygame-texteditor-0.6.7/pygame_texteditor.egg-info/
--rw-rw-rw-   0        0        0     7044 2022-06-14 13:52:17.000000 pygame-texteditor-0.6.7/pygame_texteditor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2022-06-14 13:52:18.000000 pygame-texteditor-0.6.7/pygame_texteditor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-14 13:52:17.000000 pygame-texteditor-0.6.7/pygame_texteditor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2022-06-14 13:52:18.000000 pygame-texteditor-0.6.7/pygame_texteditor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2022-06-14 13:52:18.000000 pygame-texteditor-0.6.7/pygame_texteditor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-14 13:52:18.517904 pygame-texteditor-0.6.7/setup.cfg
--rw-rw-rw-   0        0        0     1414 2022-06-14 13:48:25.000000 pygame-texteditor-0.6.7/setup.py
+-rw-r--r--   0        0        0     1092 2023-04-20 09:30:36.501202 pygame_texteditor-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1558 2023-04-20 09:41:04.570589 pygame_texteditor-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7159 2023-04-20 09:37:05.939641 pygame_texteditor-0.7.0/README.md
+-rw-r--r--   0        0        0       36 2023-04-20 09:30:36.506702 pygame_texteditor-0.7.0/src/pygame_texteditor/__init__.py
+-rw-r--r--   0        0        0     3924 2023-04-20 09:30:36.507705 pygame_texteditor-0.7.0/src/pygame_texteditor/_caret.py
+-rw-r--r--   0        0        0     5964 2023-04-20 09:30:36.508791 pygame_texteditor-0.7.0/src/pygame_texteditor/_customization.py
+-rw-r--r--   0        0        0     1783 2023-04-20 09:30:36.509810 pygame_texteditor-0.7.0/src/pygame_texteditor/_editor_getters.py
+-rw-r--r--   0        0        0    17455 2023-04-20 09:30:36.511139 pygame_texteditor-0.7.0/src/pygame_texteditor/_input_handling_keyboard.py
+-rw-r--r--   0        0        0     9639 2023-04-20 09:30:36.512448 pygame_texteditor-0.7.0/src/pygame_texteditor/_input_handling_keyboard_highlight.py
+-rw-r--r--   0        0        0     8518 2023-04-20 09:30:36.513236 pygame_texteditor-0.7.0/src/pygame_texteditor/_input_handling_mouse.py
+-rw-r--r--   0        0        0     1428 2023-04-20 09:30:36.513738 pygame_texteditor-0.7.0/src/pygame_texteditor/_letter_operations.py
+-rw-r--r--   0        0        0     1503 2023-04-20 09:30:36.514737 pygame_texteditor-0.7.0/src/pygame_texteditor/_other.py
+-rw-r--r--   0        0        0     8041 2023-04-20 09:30:36.515239 pygame_texteditor-0.7.0/src/pygame_texteditor/_rendering.py
+-rw-r--r--   0        0        0     5117 2023-04-20 09:30:36.516239 pygame_texteditor-0.7.0/src/pygame_texteditor/_rendering_highlighting.py
+-rw-r--r--   0        0        0     1072 2023-04-20 09:30:36.517237 pygame_texteditor-0.7.0/src/pygame_texteditor/_rendering_syntax_coloring.py
+-rw-r--r--   0        0        0     1852 2023-04-20 09:30:36.518237 pygame_texteditor-0.7.0/src/pygame_texteditor/_scrollbar_vertical.py
+-rw-r--r--   0        0        0     2094 2023-04-20 09:30:36.518741 pygame_texteditor-0.7.0/src/pygame_texteditor/_usage.py
+-rw-r--r--   0        0        0     3428 2023-04-20 09:30:36.505702 pygame_texteditor-0.7.0/src/pygame_texteditor/ColorFormatter.py
+-rw-r--r--   0        0        0      468 2023-04-20 09:30:36.519971 pygame_texteditor-0.7.0/src/pygame_texteditor/elements/colorstyles/bright.yml
+-rw-r--r--   0        0        0      469 2023-04-20 09:30:36.519971 pygame_texteditor-0.7.0/src/pygame_texteditor/elements/colorstyles/dark.yml
+-rw-r--r--   0        0        0    59516 2023-04-20 09:30:36.520986 pygame_texteditor-0.7.0/src/pygame_texteditor/elements/fonts/Courier.ttf
+-rw-r--r--   0        0        0      211 2023-04-20 09:30:36.521992 pygame_texteditor-0.7.0/src/pygame_texteditor/elements/graphics/Scroll_Bar.png
+-rw-r--r--   0        0        0    10313 2023-04-20 09:40:04.131701 pygame_texteditor-0.7.0/src/pygame_texteditor/TextEditor.py
+-rw-r--r--   0        0        0     8069 1970-01-01 00:00:00.000000 pygame_texteditor-0.7.0/setup.py
+-rw-r--r--   0        0        0     8089 1970-01-01 00:00:00.000000 pygame_texteditor-0.7.0/PKG-INFO
```

### Comparing `pygame-texteditor-0.6.7/LICENSE` & `pygame_texteditor-0.7.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `pygame-texteditor-0.6.7/PKG-INFO` & `pygame_texteditor-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,204 +1,227 @@
-Metadata-Version: 2.1
-Name: pygame-texteditor
-Version: 0.6.7
-Summary: A WYSIWYG-texteditor based on pygame.
-Author: CribberSix
-Author-email: cribbersix@gmail.com
-License: MIT
-Keywords: pygame,texteditor,text,editor
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# A WYSIWYG-texteditor based on pygame for pygame
-
-![PyPI](https://img.shields.io/pypi/v/pygame-texteditor?color=%233775A9&label=pypi%20package&style=plastic)
-![GitHub](https://img.shields.io/github/license/CribberSix/pygame-texteditor?style=plastic)
-
-## Introduction & examples
-
-The text editor can be inserted into any existing pygame window. 
-A minimal code example of it being activated within an existing pygame window can be found below.
-
-The code editor comes with line numbers and syntax highlighting for python if enabled:
-
-![](./resources/example_one.png)
-
-Example with default configuration:
-
-![](./resources/example_two.png)
-
-## Usage
-
-The texteditor takes 5 obligatory parameters and 3 optional parameters.
-
-##### Obligatory parameters
-- ```offset_X``` : integer - the offset from the left border of the pygame screen
-- ```offset_y``` : integer - the offset from the top border of the pygame screen
-- ```textAreaWidth``` : integer - the width of texteditor
-- ```textAreaHeight``` : integer - the height of texteditor
-- ```screen``` : pygame display surface - on which the texteditor is to be displayed
-
-##### Optional Parameters with default values
-
-- ```line_numbers_flag``` - a boolean enabling showing line numbers 
-    > Default: ```False```
-- ```style``` - a String setting the color scheme of editor and syntax highlighting 
-    > Default: ```'dark'```
-- ```syntax_highlighting_flag``` - a boolean enabling syntax highlighting for Python code 
-    > Default: ```False```
-
-## Setup
-
-##### Minimal pygame setup
-
-```
-import pygame
-from pygame_texteditor import TextEditor
-
-pygame.init()
-screenHeight = 600
-screenWidth = 900
-screen = pygame.display.set_mode((screenWidth, screenHeight))
-pygame.display.set_caption("Pygame")
-pygame.display.get_surface().fill((200, 200, 200))  # background coloring
-
-```
-##### Minimal texteditor setup
-```
-# parameters
-screen = pygame.display.get_surface()  # get existing pygame window/screen
-offset_X = 50  # offset from the left border of the pygame window
-offset_Y = 50  # offset from the top border of the pygame window
-textAreaHeight = 500
-textAreaWidth = 800
-
-
-# Instantiation
-TX = TextEditor(offset_X, offset_Y, textAreaWidth, textAreaHeight, screen)
-TX.set_line_numbers(True)  # optional 
-TX.set_syntax_highlighting(True)  # optional
-
-while True:  # pygame-loop
-    # capture input
-    pygame_events = pygame.event.get()
-    pressed_keys = pygame.key.get_pressed()
-    mouse_x, mouse_y = pygame.mouse.get_pos()
-    mouse_pressed = pygame.mouse.get_pressed()
-
-    # display editor functionality once per loop
-    TX.display_editor(pygame_events, pressed_keys, mouse_x, mouse_y, mouse_pressed)
-
-    # update pygame window
-    pygame.display.flip()  
-
-
-```
-
-##### Retrieving text from the editor
-
-The editor offers the function `get_text_as_string()` to retrieve the entire text 
-as a String from the editor. Lines are separated by the new line character ```\n```.
-
-The editor offers the function `get_text_as_list()` to retrieve the entire text as a list from the editor. 
-Each String-item in the list represents one line from the editor.
-
-##### Removing text from the editor
-
-The editor offers the function `clear_text()` to clear the editor of any text.
-
-
-##### Inserting text into the editor
-
-Inserting text can be done by using one of the two available functions: 
-1. With a list of strings in which each string represents one line, or
-2. With a string which includes linebreak characters which get parsed. 
-
-```
-set_text_from_list(["First line", "Second Line.", "Third Line."]
-set_text_from_string("First line.\nSecond line.\nThird Line")
-```
-
-## Customization
-
-#### Cursor mode 
-
-Cursor mode can either be `static` or `blinking` (=default). 
-
-```python
-set_cursor_mode("static")
-set_cursor_mode("blinking")
-```
-
-#### Key repetition speeds
-
-While a key is being held, multiple key events are being triggered. 
-The delay of the first repetition as well as the interval between all sequential key triggers can be 
-customized by using the function `set_key_repetition(delay=300, intervall=30)`. 
-
-From the [official documentation](http://www.pygame.org/docs/ref/key.html#pygame.key.set_repeat): 
-> The delay parameter is the number of milliseconds before the first repeated pygame.KEYDOWN event will be sent.
-> After that, another pygame.KEYDOWN event will be sent every interval milliseconds.
-
-#### Font size
-
-Font size can be customized with the command `set_font_size(size)` - the parameter is an integer 
-with the default value `12` to be able to reset it. 
-
-#### Line Numbers 
-Line numbers can be shown on the left side of the editor. Line numbers begin with 0 as is the Pythonian way. 
-
-Line numbers can be enabled and disabled with ```set_line_numbers(Boolean)```.
-
-
-#### Syntax Highlighting
-
-The editor comes with syntax highlighting for Python code. Tokenization is based on the ```pygment``` package. 
-
-Syntax highlighting can be enabled/disabled with ```set_syntax_coloring(boolean_value)```.
-
-The syntax colors being used are also specified in the yml style file.
-
-
-#### Color-scheme customization
-
-The editor uses a yml file to set the color-scheme for the editor itself and for the syntax coloring. 
-
-Two styles are delivered with the editor, they can be activated respectively by:
-- `set_colorscheme("dark")`
-- `set_colorscheme("bright")`
-
-A custom style can be loaded with the following method from a created yml file: 
-- `set_colorscheme_from_yaml("X:\path\to\custom\filename.yml")`
-
-All keys must be present with values. Acceptable values are 
-RGB colors in the following format: ```(255, 255, 255)``` or ```255, 255, 255```.
-
-The following keys are required in the ```stylename.yml``` file, syntax colors are only used if syntax
-highlighting is enabled, but are still required to be included.
-
-*Editor colors*
-- `codingBackgroundColor`
-- `codingScrollBarBackgroundColor`
-- `lineNumberColor`
-- `lineNumberBackgroundColor`
-- `textColor`
-
-*Syntax colors*
-- `textColor_normal`
-- `textColor_comments`
-- `textColor_quotes`
-- `textColor_operators`
-- `textColor_keywords`
-- `textColor_function`
-- `textColor_builtin`
-
+Metadata-Version: 2.1
+Name: pygame-texteditor
+Version: 0.7.0
+Summary: A WYSIWYG-texteditor based on pygame.
+License: MIT
+Keywords: pygame,texteditor,text,editor
+Author: Victor Seifert
+Author-email: seifert.victor@web.de
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: PyYAML (>=5.3.1)
+Requires-Dist: Pygments (>=2.6.1)
+Requires-Dist: pygame (>=1.9.6)
+Requires-Dist: pyperclip (>=1.8.1)
+Description-Content-Type: text/markdown
+
+# A WYSIWYG-texteditor based on pygame for pygame
+
+![PyPI](https://img.shields.io/pypi/v/pygame-texteditor?color=%233775A9&label=pypi%20package&style=plastic)
+![GitHub](https://img.shields.io/github/license/CribberSix/pygame-texteditor?style=plastic)
+
+## Introduction & examples
+
+The text editor can be inserted into any existing pygame window.
+A minimal code example of it being activated within an existing pygame window can be found below.
+
+The code editor comes with line numbers and syntax highlighting for python if enabled:
+
+![](./resources/example_one.png)
+
+Example with default configuration:
+
+![](./resources/example_two.png)
+
+## Usage
+
+The texteditor takes 5 obligatory parameters and 4 optional parameters.
+
+##### Obligatory parameters
+- ```offset_X``` : integer - the offset from the left border of the pygame screen
+- ```offset_y``` : integer - the offset from the top border of the pygame screen
+- ```editor_width``` : integer - the width of texteditor
+- ```editor_height``` : integer - the height of texteditor
+- ```screen``` : pygame display surface - on which the texteditor is to be displayed
+
+##### Optional Parameters with default values
+
+- ```display_line_numbers``` - a boolean enabling showing line numbers
+    > Default: ```False```
+- ```style``` - a String setting the color scheme of editor and syntax highlighting
+    > Default: ```'dark'```
+- ```syntax_highlighting_python``` - a boolean enabling syntax highlighting for Python code
+    > Default: ```False```
+- ```font_size``` - an integer to set for the font size.
+    > Default: ```16```
+
+## Setup
+
+##### Minimal pygame setup
+
+```python
+import pygame
+
+pygame.init()
+screenHeight = 600
+screenWidth = 900
+screen = pygame.display.set_mode((screenWidth, screenHeight))
+pygame.display.set_caption("Pygame")
+pygame.display.get_surface().fill((200, 200, 200))  # background coloring
+```
+
+##### Minimal texteditor setup
+
+```python
+import pygame
+from pygame_texteditor import TextEditor
+
+# parameters
+screen = pygame.display.get_surface()  # get existing pygame window/screen
+offset_X = 50  # offset from the left border of the pygame window
+offset_Y = 50  # offset from the top border of the pygame window
+editor_height = 800
+editor_width = 500
+
+
+# Instantiation
+TX = TextEditor(offset_X, offset_Y, editor_width, editor_height, screen)
+TX.set_line_numbers(True)  # optional
+TX.set_syntax_highlighting(True)  # optional
+
+while True:  # pygame-loop
+    # capture input
+    pygame_events = pygame.event.get()
+    pressed_keys = pygame.key.get_pressed()
+    mouse_x, mouse_y = pygame.mouse.get_pos()
+    mouse_pressed = pygame.mouse.get_pressed()
+
+    # display editor functionality once per loop
+    TX.display_editor(pygame_events, pressed_keys, mouse_x, mouse_y, mouse_pressed)
+
+    # update pygame window
+    pygame.display.flip()
+```
+
+##### Retrieving text from the editor
+
+The editor offers the function `get_text_as_string()` to retrieve the entire text
+as a String from the editor. Lines are separated by the new line character ```\n```.
+
+The editor offers the function `get_text_as_list()` to retrieve the entire text as a list from the editor.
+Each String-item in the list represents one line from the editor.
+
+##### Removing text from the editor
+
+The editor offers the function `clear_text()` to clear the editor of any text.
+
+##### Inserting text into the editor
+
+Inserting text can be done by using one of the two available functions:
+1. With a list of strings in which each string represents one line, or
+2. With a string which includes linebreak characters which get parsed.
+
+```
+set_text_from_list(["First line", "Second Line.", "Third Line."]
+set_text_from_string("First line.\nSecond line.\nThird Line")
+```
+
+## Customization
+
+#### Cursor mode
+
+Cursor mode can either be `static` or `blinking` (=default).
+
+```python
+TX = TextEditor(...)
+TX.set_cursor_mode("static")
+TX.set_cursor_mode("blinking")
+```
+
+#### Key repetition speeds
+
+While a key is being held, multiple key events are being triggered.
+The delay of the first repetition as well as the interval between all sequential key triggers can be
+customized by using the function `set_key_repetition(delay=300, intervall=30)`.
+
+From the [official documentation](http://www.pygame.org/docs/ref/key.html#pygame.key.set_repeat):
+> The delay parameter is the number of milliseconds before the first repeated pygame.KEYDOWN event will be sent.
+> After that, another pygame.KEYDOWN event will be sent every interval milliseconds.
+
+
+#### Font Customization
+
+The editor uses a ttf file to set the font for the editor. By default, the Courier monospace font is used.
+
+A custom font can be loaded with the following method, passing an *absolute* path:
+- `set_font_from_ttf("X:\path\to\custom\font.ttf")`
+
+DISCLAIMER: As the width of a letter (space) is only calculated once after setting the font_size, any fonts that are not monospace will lead to the editor not working correctly anymore, as it cannot be determined correctly between which letters the user clicked.
+
+#### Font size
+
+Font size can be customized with the command `set_font_size(size)` - the parameter is an integer
+with the default value `16` to be able to reset it.
+
+#### Line Numbers
+Line numbers can be shown on the left side of the editor. Line numbers begin with 0 as is the Pythonian way.
+
+Line numbers can be enabled and disabled with ```set_line_numbers(Boolean)```.
+
+
+#### Syntax Highlighting
+
+The editor comes with syntax highlighting for Python code. Tokenization is based on the ```pygment``` package.
+
+Syntax highlighting can be enabled/disabled with ```set_syntax_coloring(boolean_value)```.
+
+The syntax colors being used are also specified in the yml style file.
+
+
+#### Color-scheme customization
+
+The editor uses a yml file to set the color-scheme for the editor itself and for the syntax coloring.
+
+Two styles are delivered with the editor, they can be activated respectively by:
+- `set_colorscheme("dark")`
+- `set_colorscheme("bright")`
+
+A custom style can be loaded with the following method from a created yml file:
+- `set_colorscheme_from_yaml("X:\path\to\custom\filename.yml")`
+
+All keys must be present with values. Acceptable values are
+RGB colors in the following format: ```(255, 255, 255)``` or ```255, 255, 255```.
+
+The following keys are required in the ```stylename.yml``` file, syntax colors are only used if syntax
+highlighting is enabled, but are still required to be included.
+
+**Editor colors** (source: bright.yml)
+
+- `codingBackgroundColor: (255, 255, 255)`
+- `codingScrollBarBackgroundColor: (49, 50, 50)`
+- `lineNumberColor: (255, 255, 255)`
+- `lineNumberBackgroundColor: (60, 61, 61)`
+- `textColor: (255, 255, 255)`
+
+** Syntax colors** (source: bright.yml)
+
+- `textColor_normal: (0, 255, 255)`
+- `textColor_comments: (119, 115, 115)`
+- `textColor_quotes: (227, 215, 115)`
+- `textColor_operators: (237, 36, 36)`
+- `textColor_keywords: (237, 36, 36)`
+- `textColor_function: (50, 150, 36)`
+- `textColor_builtin: (50, 50, 136)`
+
```

### Comparing `pygame-texteditor-0.6.7/README.md` & `pygame_texteditor-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,183 +1,197 @@
 # A WYSIWYG-texteditor based on pygame for pygame
 
 ![PyPI](https://img.shields.io/pypi/v/pygame-texteditor?color=%233775A9&label=pypi%20package&style=plastic)
 ![GitHub](https://img.shields.io/github/license/CribberSix/pygame-texteditor?style=plastic)
 
 ## Introduction & examples
 
-The text editor can be inserted into any existing pygame window. 
+The text editor can be inserted into any existing pygame window.
 A minimal code example of it being activated within an existing pygame window can be found below.
 
 The code editor comes with line numbers and syntax highlighting for python if enabled:
 
 ![](./resources/example_one.png)
 
 Example with default configuration:
 
 ![](./resources/example_two.png)
 
 ## Usage
 
-The texteditor takes 5 obligatory parameters and 3 optional parameters.
+The texteditor takes 5 obligatory parameters and 4 optional parameters.
 
 ##### Obligatory parameters
 - ```offset_X``` : integer - the offset from the left border of the pygame screen
 - ```offset_y``` : integer - the offset from the top border of the pygame screen
-- ```textAreaWidth``` : integer - the width of texteditor
-- ```textAreaHeight``` : integer - the height of texteditor
+- ```editor_width``` : integer - the width of texteditor
+- ```editor_height``` : integer - the height of texteditor
 - ```screen``` : pygame display surface - on which the texteditor is to be displayed
 
 ##### Optional Parameters with default values
 
-- ```line_numbers_flag``` - a boolean enabling showing line numbers 
+- ```display_line_numbers``` - a boolean enabling showing line numbers
     > Default: ```False```
-- ```style``` - a String setting the color scheme of editor and syntax highlighting 
+- ```style``` - a String setting the color scheme of editor and syntax highlighting
     > Default: ```'dark'```
-- ```syntax_highlighting_flag``` - a boolean enabling syntax highlighting for Python code 
+- ```syntax_highlighting_python``` - a boolean enabling syntax highlighting for Python code
     > Default: ```False```
+- ```font_size``` - an integer to set for the font size.
+    > Default: ```16```
 
 ## Setup
 
 ##### Minimal pygame setup
 
-```
+```python
 import pygame
-from pygame_texteditor import TextEditor
 
 pygame.init()
 screenHeight = 600
 screenWidth = 900
 screen = pygame.display.set_mode((screenWidth, screenHeight))
 pygame.display.set_caption("Pygame")
 pygame.display.get_surface().fill((200, 200, 200))  # background coloring
-
 ```
+
 ##### Minimal texteditor setup
-```
+
+```python
+import pygame
+from pygame_texteditor import TextEditor
+
 # parameters
 screen = pygame.display.get_surface()  # get existing pygame window/screen
 offset_X = 50  # offset from the left border of the pygame window
 offset_Y = 50  # offset from the top border of the pygame window
-textAreaHeight = 500
-textAreaWidth = 800
+editor_height = 800
+editor_width = 500
 
 
 # Instantiation
-TX = TextEditor(offset_X, offset_Y, textAreaWidth, textAreaHeight, screen)
-TX.set_line_numbers(True)  # optional 
+TX = TextEditor(offset_X, offset_Y, editor_width, editor_height, screen)
+TX.set_line_numbers(True)  # optional
 TX.set_syntax_highlighting(True)  # optional
 
 while True:  # pygame-loop
     # capture input
     pygame_events = pygame.event.get()
     pressed_keys = pygame.key.get_pressed()
     mouse_x, mouse_y = pygame.mouse.get_pos()
     mouse_pressed = pygame.mouse.get_pressed()
 
     # display editor functionality once per loop
     TX.display_editor(pygame_events, pressed_keys, mouse_x, mouse_y, mouse_pressed)
 
     # update pygame window
-    pygame.display.flip()  
-
-
+    pygame.display.flip()
 ```
 
 ##### Retrieving text from the editor
 
-The editor offers the function `get_text_as_string()` to retrieve the entire text 
+The editor offers the function `get_text_as_string()` to retrieve the entire text
 as a String from the editor. Lines are separated by the new line character ```\n```.
 
-The editor offers the function `get_text_as_list()` to retrieve the entire text as a list from the editor. 
+The editor offers the function `get_text_as_list()` to retrieve the entire text as a list from the editor.
 Each String-item in the list represents one line from the editor.
 
 ##### Removing text from the editor
 
 The editor offers the function `clear_text()` to clear the editor of any text.
 
-
 ##### Inserting text into the editor
 
-Inserting text can be done by using one of the two available functions: 
+Inserting text can be done by using one of the two available functions:
 1. With a list of strings in which each string represents one line, or
-2. With a string which includes linebreak characters which get parsed. 
+2. With a string which includes linebreak characters which get parsed.
 
 ```
 set_text_from_list(["First line", "Second Line.", "Third Line."]
 set_text_from_string("First line.\nSecond line.\nThird Line")
 ```
 
 ## Customization
 
-#### Cursor mode 
+#### Cursor mode
 
-Cursor mode can either be `static` or `blinking` (=default). 
+Cursor mode can either be `static` or `blinking` (=default).
 
 ```python
-set_cursor_mode("static")
-set_cursor_mode("blinking")
+TX = TextEditor(...)
+TX.set_cursor_mode("static")
+TX.set_cursor_mode("blinking")
 ```
 
 #### Key repetition speeds
 
-While a key is being held, multiple key events are being triggered. 
-The delay of the first repetition as well as the interval between all sequential key triggers can be 
-customized by using the function `set_key_repetition(delay=300, intervall=30)`. 
+While a key is being held, multiple key events are being triggered.
+The delay of the first repetition as well as the interval between all sequential key triggers can be
+customized by using the function `set_key_repetition(delay=300, intervall=30)`.
 
-From the [official documentation](http://www.pygame.org/docs/ref/key.html#pygame.key.set_repeat): 
+From the [official documentation](http://www.pygame.org/docs/ref/key.html#pygame.key.set_repeat):
 > The delay parameter is the number of milliseconds before the first repeated pygame.KEYDOWN event will be sent.
 > After that, another pygame.KEYDOWN event will be sent every interval milliseconds.
 
+
+#### Font Customization
+
+The editor uses a ttf file to set the font for the editor. By default, the Courier monospace font is used.
+
+A custom font can be loaded with the following method, passing an *absolute* path:
+- `set_font_from_ttf("X:\path\to\custom\font.ttf")`
+
+DISCLAIMER: As the width of a letter (space) is only calculated once after setting the font_size, any fonts that are not monospace will lead to the editor not working correctly anymore, as it cannot be determined correctly between which letters the user clicked.
+
 #### Font size
 
-Font size can be customized with the command `set_font_size(size)` - the parameter is an integer 
-with the default value `12` to be able to reset it. 
+Font size can be customized with the command `set_font_size(size)` - the parameter is an integer
+with the default value `16` to be able to reset it.
 
-#### Line Numbers 
-Line numbers can be shown on the left side of the editor. Line numbers begin with 0 as is the Pythonian way. 
+#### Line Numbers
+Line numbers can be shown on the left side of the editor. Line numbers begin with 0 as is the Pythonian way.
 
 Line numbers can be enabled and disabled with ```set_line_numbers(Boolean)```.
 
 
 #### Syntax Highlighting
 
-The editor comes with syntax highlighting for Python code. Tokenization is based on the ```pygment``` package. 
+The editor comes with syntax highlighting for Python code. Tokenization is based on the ```pygment``` package.
 
 Syntax highlighting can be enabled/disabled with ```set_syntax_coloring(boolean_value)```.
 
 The syntax colors being used are also specified in the yml style file.
 
 
 #### Color-scheme customization
 
-The editor uses a yml file to set the color-scheme for the editor itself and for the syntax coloring. 
+The editor uses a yml file to set the color-scheme for the editor itself and for the syntax coloring.
 
 Two styles are delivered with the editor, they can be activated respectively by:
 - `set_colorscheme("dark")`
 - `set_colorscheme("bright")`
 
-A custom style can be loaded with the following method from a created yml file: 
+A custom style can be loaded with the following method from a created yml file:
 - `set_colorscheme_from_yaml("X:\path\to\custom\filename.yml")`
 
-All keys must be present with values. Acceptable values are 
+All keys must be present with values. Acceptable values are
 RGB colors in the following format: ```(255, 255, 255)``` or ```255, 255, 255```.
 
 The following keys are required in the ```stylename.yml``` file, syntax colors are only used if syntax
 highlighting is enabled, but are still required to be included.
 
-*Editor colors*
-- `codingBackgroundColor`
-- `codingScrollBarBackgroundColor`
-- `lineNumberColor`
-- `lineNumberBackgroundColor`
-- `textColor`
-
-*Syntax colors*
-- `textColor_normal`
-- `textColor_comments`
-- `textColor_quotes`
-- `textColor_operators`
-- `textColor_keywords`
-- `textColor_function`
-- `textColor_builtin`
+**Editor colors** (source: bright.yml)
 
+- `codingBackgroundColor: (255, 255, 255)`
+- `codingScrollBarBackgroundColor: (49, 50, 50)`
+- `lineNumberColor: (255, 255, 255)`
+- `lineNumberBackgroundColor: (60, 61, 61)`
+- `textColor: (255, 255, 255)`
+
+** Syntax colors** (source: bright.yml)
+
+- `textColor_normal: (0, 255, 255)`
+- `textColor_comments: (119, 115, 115)`
+- `textColor_quotes: (227, 215, 115)`
+- `textColor_operators: (237, 36, 36)`
+- `textColor_keywords: (237, 36, 36)`
+- `textColor_function: (50, 150, 36)`
+- `textColor_builtin: (50, 50, 136)`
```

### Comparing `pygame-texteditor-0.6.7/pygame_texteditor/ColorFormatter.py` & `pygame_texteditor-0.7.0/src/pygame_texteditor/ColorFormatter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+import os
+import re
+from typing import Dict, List, Tuple
+
+import yaml
 from pygments import highlight
-from pygments.lexers import PythonLexer
 from pygments.formatter import Formatter
+from pygments.lexers import PythonLexer
 from pygments.token import Token, is_token_subtype
-from typing import List, Dict, Tuple
-import os
-import yaml
-import re
 
 
 class ColorFormatter:
-
     def __init__(self):
         self.textColor_normal = (0, 0, 0)
         self.textColor_comments = (0, 0, 0)
         self.textColor_quotes = (0, 0, 0)
         self.textColor_operators = (0, 0, 0)
         self.textColor_keywords = (0, 0, 0)
         self.textColor_function = (0, 0, 0)
@@ -29,39 +29,73 @@
         Depending on the type of token a color is assigned.
         """
 
         dicts = []
         for ttype, value in tokensource:
             # NAME.FUNCTION
             if ttype == Token.Name.Function:
-                dicts.append({'chars': value, 'type': 'function', 'color': self.textColor_function})
+                dicts.append(
+                    {
+                        "chars": value,
+                        "type": "function",
+                        "color": self.textColor_function,
+                    }
+                )
 
             # BUILTIN
             elif ttype == Token.Name.Builtin:
-                dicts.append({'chars': value, 'type': 'builtin', 'color': self.textColor_builtin})
+                dicts.append(
+                    {"chars": value, "type": "builtin", "color": self.textColor_builtin}
+                )
 
             # LITERAL.STRING(.*)
             elif ttype == Token.Literal.String.Affix:
-                dicts.append({'chars': value, 'type': 'builtin', 'color': self.textColor_builtin})
+                dicts.append(
+                    {"chars": value, "type": "builtin", "color": self.textColor_builtin}
+                )
             elif is_token_subtype(ttype, Token.Literal.String):
-                dicts.append({'chars': value, 'type': 'quotes', 'color': self.textColor_quotes})
+                dicts.append(
+                    {"chars": value, "type": "quotes", "color": self.textColor_quotes}
+                )
 
             # OPERATOR.*
             elif is_token_subtype(ttype, Token.Operator):
-                dicts.append({'chars': value, 'type': 'operators', 'color': self.textColor_operators})
+                dicts.append(
+                    {
+                        "chars": value,
+                        "type": "operators",
+                        "color": self.textColor_operators,
+                    }
+                )
 
             # KEYWORD.*
             elif is_token_subtype(ttype, Token.Keyword):
-                dicts.append({'chars': value, 'type': 'keywords', 'color': self.textColor_keywords})
+                dicts.append(
+                    {
+                        "chars": value,
+                        "type": "keywords",
+                        "color": self.textColor_keywords,
+                    }
+                )
 
             # COMMENT.*
             elif is_token_subtype(ttype, Token.Comment):
-                dicts.append({'chars': value, 'type': 'comments', 'color': self.textColor_comments})
-
-            elif value == '\n':  # since we parse line-by-line, we need to exclude the linebreak character
+                dicts.append(
+                    {
+                        "chars": value,
+                        "type": "comments",
+                        "color": self.textColor_comments,
+                    }
+                )
+
+            elif (
+                value == "\n"
+            ):  # since we parse line-by-line, we need to exclude the linebreak character
                 pass
 
             # REST
             else:
-                dicts.append({'chars': value, 'type': 'text', 'color': self.textColor_normal})
+                dicts.append(
+                    {"chars": value, "type": "text", "color": self.textColor_normal}
+                )
 
         return dicts
```

### Comparing `pygame-texteditor-0.6.7/pygame_texteditor/TextEditor.py` & `pygame_texteditor-0.7.0/src/pygame_texteditor/TextEditor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,201 +1,277 @@
-from pygments.lexers import PythonLexer
-import pygame
 import math
 import os
-import yaml
-import re
+from typing import Optional
+import pygame
+from pygments.lexers import PythonLexer
 
 from .ColorFormatter import ColorFormatter
 
+current_dir = os.path.dirname(__file__)
+
 
 class TextEditor:
+    """A WYSIWYG-texteditor for pygame."""
+
     # Scroll functionality
-    from ._scrollbar_vertical import render_scrollbar_vertical, display_scrollbar, scrollbar_up, \
-        scrollbar_down
+    # caret
+    from ._caret import (
+        set_drag_end_after_last_line,
+        set_drag_end_by_mouse,
+        set_drag_end_letter_by_mouse,
+        set_drag_end_line_by_mouse,
+        set_drag_start_after_last_line,
+        set_drag_start_before_first_line,
+        set_drag_start_by_mouse,
+        update_caret_position,
+        update_caret_position_by_drag_end,
+        update_caret_position_by_drag_start,
+    )
 
-    # input handling KEYBOARD
-    from ._input_handling_keyboard import handle_keyboard_input, handle_keyboard_delete, handle_keyboard_backspace, \
-        handle_keyboard_return, handle_keyboard_space, handle_keyboard_tab, insert_unicode, \
-        handle_keyboard_arrow_left, handle_keyboard_arrow_right, handle_keyboard_arrow_up, handle_keyboard_arrow_down
+    # files for customization of the editor:
+    from ._customization import (
+        set_colorscheme,
+        set_colorscheme_from_yaml,
+        set_cursor_mode,
+        set_font_from_ttf,
+        set_font_size,
+        set_line_numbers,
+        set_syntax_highlighting,
+    )
+    from ._editor_getters import (
+        get_letter_index,
+        get_line_index,
+        get_number_of_letters_in_line_by_index,
+        get_number_of_letters_in_line_by_mouse,
+        get_showable_lines,
+        line_is_visible,
+    )
 
-    from ._input_handling_keyboard_highlight import handle_input_with_highlight, handle_highlight_and_copy, \
-        handle_highlight_and_paste, handle_highlight_and_cut, highlight_all, get_highlighted_characters
+    # input handling KEYBOARD
+    from ._input_handling_keyboard import (
+        handle_keyboard_arrow_down,
+        handle_keyboard_arrow_left,
+        handle_keyboard_arrow_right,
+        handle_keyboard_arrow_up,
+        handle_keyboard_backspace,
+        handle_keyboard_delete,
+        handle_keyboard_input,
+        handle_keyboard_return,
+        handle_keyboard_space,
+        handle_keyboard_tab,
+        insert_unicode,
+    )
+    from ._input_handling_keyboard_highlight import (
+        get_highlighted_characters,
+        handle_highlight_and_copy,
+        handle_highlight_and_cut,
+        handle_highlight_and_paste,
+        handle_input_with_highlight,
+        highlight_all,
+    )
 
     # input handling MOUSE
-    from ._input_handling_mouse import handle_mouse_input, mouse_within_texteditor, mouse_within_existing_lines
-
-    # caret
-    from ._caret import update_caret_position, update_caret_position_by_drag_end, update_caret_position_by_drag_start, \
-        set_drag_start_after_last_line, set_drag_end_after_last_line, set_drag_start_by_mouse, \
-        set_drag_end_by_mouse, set_drag_end_line_by_mouse, set_drag_end_letter_by_mouse, \
-        set_drag_start_before_first_line
+    from ._input_handling_mouse import handle_mouse_input, mouse_within_existing_lines, mouse_within_texteditor
 
     # letter operations (delete, get)
-    from ._letter_operations import \
-        delete_entire_line, delete_start_to_letter, delete_letter_to_end, delete_letter_to_letter, \
-        get_entire_line, get_line_from_start_to_char, get_line_from_char_to_end, get_line_from_char_to_char
+    from ._letter_operations import (
+        delete_entire_line,
+        delete_letter_to_end,
+        delete_letter_to_letter,
+        delete_start_to_letter,
+        get_entire_line,
+        get_line_from_char_to_char,
+        get_line_from_char_to_end,
+        get_line_from_start_to_char,
+    )
+    from ._other import jump_to_end, jump_to_start, reset_after_highlight
 
     # rendering (basic, highlighting, syntax coloring)
-    from ._rendering import render_line_contents_by_dicts, \
-        render_caret, caret_within_texteditor, render_background_coloring, render_line_numbers, \
-        reset_text_area_to_caret, get_rect_coord_from_indizes, get_rect_coord_from_mouse
-    from ._rendering_highlighting import render_highlight, highlight_lines, highlight_entire_line, \
-        highlight_from_letter_to_letter, highlight_from_start_to_letter, highlight_from_letter_to_end
-    from ._rendering_syntax_coloring import get_syntax_coloring_dicts, get_single_color_dicts
-
-    from ._editor_getters import get_line_index, get_letter_index, line_is_visible, get_showable_lines, \
-        get_number_of_letters_in_line_by_mouse, get_number_of_letters_in_line_by_index
-
-    from ._other import jump_to_start, jump_to_end, reset_after_highlight
-
-    # files for customization of the editor:
-    from ._customization import set_line_numbers, set_syntax_highlighting, set_colorscheme, \
-                                set_colorscheme_from_yaml, set_font_size, set_cursor_mode
-    from ._usage import get_text_as_list, get_text_as_string, clear_text, set_text_from_list, set_text_from_string
-
-    def __init__(self, offset_x, offset_y, text_area_width, text_area_height, screen,
-                 line_numbers_flag=False, style='dark', syntax_highlighting_flag=False):
+    from ._rendering import (
+        caret_within_texteditor,
+        get_rect_coord_from_indizes,
+        get_rect_coord_from_mouse,
+        render_background_coloring,
+        render_caret,
+        render_line_contents,
+        render_line_numbers,
+        reset_text_area_to_caret,
+        update_line_number_display,
+    )
+    from ._rendering_highlighting import (
+        highlight_entire_line,
+        highlight_from_letter_to_end,
+        highlight_from_letter_to_letter,
+        highlight_from_start_to_letter,
+        highlight_lines,
+        render_highlight,
+    )
+    from ._rendering_syntax_coloring import get_single_color_dicts, get_syntax_coloring_dicts
+    from ._scrollbar_vertical import display_scrollbar, render_scrollbar_vertical, scrollbar_down, scrollbar_up
+    from ._usage import clear_text, get_text_as_list, get_text_as_string, set_text_from_list, set_text_from_string
+
+    def __init__(
+        self,
+        offset_x,
+        offset_y,
+        editor_width,
+        editor_height,
+        screen,
+        display_line_numbers=False,
+        style="dark",
+        syntax_highlighting_python=False,
+        font_size=16,
+    ):
+        """Initialize the class."""
         self.screen = screen
 
         # VISUALS
-        self.editor_offset_X = offset_x
-        self.editor_offset_Y = offset_y
-        self.textAreaWidth = text_area_width
-        self.textAreaHeight = text_area_height
-
-        self.conclusionBarHeight = 18
-        self.letter_size_Y = 16
-        current_dir = os.path.dirname(__file__)
-        self.courier_font = pygame.font.Font(os.path.join(current_dir, "elements/fonts/Courier.ttf"),
-                                             self.letter_size_Y)
-
-        letter_width = self.courier_font.render(" ", 1, (0, 0, 0)).get_width()
-        self.letter_size_X = letter_width
-
-        self.trennzeichen_image = pygame.image.load(
-            os.path.join(current_dir, "elements/graphics/Trennzeichen.png")).convert_alpha()
-        self.syntax_coloring = syntax_highlighting_flag
-
-        # LINES
-        self.Trenn_counter = 0
-        self.MaxLinecounter = 0
-        self.line_string_list = []  # LOGIC: Array of actual Strings
-        self.lineHeight = self.letter_size_Y
-
-        # self.maxLines is the variable keeping count how many lines we currently have -
-        # in the beginning we fill the entire editor with empty lines.
-        self.maxLines = int(math.floor(self.textAreaHeight / self.lineHeight))
-        self.showStartLine = 0  # first line (shown at the top of the editor) <- must be zero during init!
-        self.line_gap = 3 + self.letter_size_Y
-        self.showable_line_numbers_in_editor = int(math.floor(self.textAreaHeight / self.line_gap))
-
-        for i in range(self.maxLines):  # from 0 to maxLines:
-            self.line_string_list.append("")  # Add a line
+        self.editor_offset_x = offset_x
+        self.editor_offset_y = offset_y
+        self.editor_width = editor_width
+        self.editor_height = editor_height
+        self.conclusion_bar_height = 18
+        self.ttf_path = os.path.join(current_dir, "elements/fonts/Courier.ttf")
+        self.editor_font = pygame.font.Font(self.ttf_path, size=font_size)
+        self.letter_height = font_size
+        self.letter_width = self.editor_font.render(" ", 1, (0, 0, 0)).get_width()
+        self.syntax_highlighting_python = syntax_highlighting_python
+
+        # LINES (line height equals the letter height).
+        self.max_line_counter = 0
+        # Fill the entire editor with empty lines in the beginning
+        self.editor_lines = ["" for _ in range(int(math.floor(self.editor_height / self.letter_height)))]
+        self.first_showable_line_index = 0  # first line, shown at the top of the editor
+        self.line_margin = 3
+        self.line_height_including_margin = self.letter_height + self.line_margin
+        self.showable_line_numbers_in_editor = int(math.floor(self.editor_height / self.line_height_including_margin))
 
         # SCROLLBAR
-        self.scrollBarImg = pygame.image.load(os.path.join(current_dir, "elements/graphics/Scroll_Bar.png")).convert()
-        self.scrollBarWidth = 8  # must be an even number
-
-        self.scrollbar: pygame.Rect = None
-        self.scroll_start_y: int = None
-        self.scroll_dragging: bool = False
+        # TODO: replace image with PyGame drawn rect
+        self.scrollbar_image = pygame.image.load(
+            os.path.join(current_dir, "elements/graphics/Scroll_Bar.png")
+        ).convert()
+        self.scrollbar_width = 8  # must be an even number
+        self.padding_between_edge_and_scrollbar = 2
+
+        self.scrollbar: Optional[pygame.Rect] = None
+        self.scrollbar_start_y: Optional[int] = None
+        self.scrollbar_is_being_dragged: bool = False
 
         # LINE NUMBERS
-        self.displayLineNumbers = line_numbers_flag
-        if self.displayLineNumbers:
-            self.lineNumberWidth = 27  # line number background width and also offset for text!
-        else:
-            self.lineNumberWidth = 0
-        self.line_numbers_Y = self.editor_offset_Y
+        self.display_line_numbers = display_line_numbers
+        self.line_number_width = 0
+        if self.display_line_numbers:
+            self.line_number_width = self.editor_font.render(" ", 1, (0, 0, 0)).get_width() * 2
+        self.line_numbers_y = self.editor_offset_y
 
         # TEXT COORDINATES
-        self.chosen_LineIndex = 0
-        self.chosen_LetterIndex = 0
-        self.yline_start = self.editor_offset_Y + 3
-        self.yline = self.editor_offset_Y
-        self.xline_start_offset = 28
-        if self.displayLineNumbers:
-            self.xline_start = self.editor_offset_X + self.xline_start_offset
-            self.xline = self.editor_offset_X + self.xline_start_offset
-        else:
-            self.xline_start = self.editor_offset_X
-            self.xline = self.editor_offset_X
+        self.chosen_line_index = 0
+        self.chosen_letter_index = 0
+        self.line_start_y = self.editor_offset_y + self.line_margin  # add initial margin to offset
+        self.line_start_x = self.editor_offset_x
+        if self.display_line_numbers:
+            self.line_start_x += self.line_number_width
 
         # CURSOR - coordinates for displaying the caret while typing
+        self.caret_display_counter = 0
+        self.caret_display_intervals_per_second = 5
         self.static_cursor = False
-        self.cursor_Y = self.yline_start - 3
-        self.cursor_X = self.xline_start
+        self.caret_y = self.editor_offset_y
+        self.caret_x = self.line_start_x
 
         # click down - coordinates used to identify start-point of drag
         self.dragged_active = False
         self.dragged_finished = True
-        self.drag_chosen_LineIndex_start = 0
-        self.drag_chosen_LetterIndex_start = 0
+        self.drag_chosen_line_index_start = 0
+        self.drag_chosen_letter_index_start = 0
         self.last_clickdown_cycle = 0
 
         # click up  - coordinates used to identify end-point of drag
-        self.drag_chosen_LineIndex_end = 0
-        self.drag_chosen_LetterIndex_end = 0
+        self.drag_chosen_line_index_end = 0
+        self.drag_chosen_letter_index_end = 0
         self.last_clickup_cycle = 0
 
         # Colors
-        self.codingBackgroundColor = (40, 41, 41)
-        self.codingScrollBarBackgroundColor = (49, 50, 50)
-        self.lineNumberColor = (255, 255, 255)
-        self.lineNumberBackgroundColor = (60, 61, 61)
-        self.textColor = (255, 255, 255)
+        self.color_coding_background = (40, 41, 41)
         self.color_scrollbar = (60, 61, 61)
+        self.color_scrollbar_background = (49, 50, 50)
+        self.color_line_number_font = (255, 255, 255)
+        self.color_line_number_background = (60, 61, 61)
+        self.color_text = (255, 255, 255)
+        self.color_caret = (255, 255, 255)
 
         self.lexer = PythonLexer()
-        self.formatter = ColorFormatter()
+        self.color_formatter = ColorFormatter()
         self.set_colorscheme(style)
 
         # Key input variables+
         self.key_initial_delay = 300
-        self.key_continued_intervall = 30
-        pygame.key.set_repeat(self.key_initial_delay, self.key_continued_intervall) 
+        self.key_continued_interval = 30
+        pygame.key.set_repeat(self.key_initial_delay, self.key_continued_interval)
 
         # Performance enhancing variables
-        self.firstiteration_boolean = True
-        self.rerenderLineNumbers = True
-        self.click_hold = False
+        self.first_iteration_boolean = True
+        self.render_line_numbers_flag = True
+        self.click_hold_flag = False
         self.cycleCounter = 0  # Used to be able to tell whether a mouse-drag action has been handled already or not.
 
         self.clock = pygame.time.Clock()
         self.FPS = 60  # we need to limit the FPS so we don't trigger the same actions too often (e.g. deletions)
+        self.max_line_number_rendered = len(self.editor_lines)  # TODO: move to a fitting location.
 
     def display_editor(self, pygame_events, pressed_keys, mouse_x, mouse_y, mouse_pressed):
+        """Display the editor.
+
+        The function should be called once within every pygame loop.
+
+        :param pygame_events:
+        :param pressed_keys:
+        :param mouse_x:
+        :param mouse_y:
+        :param mouse_pressed:
+        """
         # needs to be called within a while loop to be able to catch key/mouse input and update visuals throughout use.
         self.cycleCounter = self.cycleCounter + 1
         # first iteration
-        if self.firstiteration_boolean:
+        if self.first_iteration_boolean:
             # paint entire area to avoid pixel error beneath line numbers
-            pygame.draw.rect(self.screen, self.codingBackgroundColor,
-                             (self.editor_offset_X, self.editor_offset_Y, self.textAreaWidth, self.textAreaHeight))
-            self.firstiteration_boolean = False
+            pygame.draw.rect(
+                self.screen,
+                self.color_coding_background,
+                (
+                    self.editor_offset_x,
+                    self.editor_offset_y,
+                    self.editor_width,
+                    self.editor_height,
+                ),
+            )
+            self.first_iteration_boolean = False
 
         for event in pygame_events:  # handle QUIT operation
             if event.type == pygame.QUIT:
                 pygame.quit()
                 exit()
 
         self.handle_keyboard_input(pygame_events, pressed_keys)
         self.handle_mouse_input(pygame_events, mouse_x, mouse_y, mouse_pressed)
 
+        self.update_line_number_display()
+
         # RENDERING 1 - Background objects
         self.render_background_coloring()
         self.render_line_numbers()
 
-        # RENDERING 2 - Lines
+        # RENDERING 2 - Line contents, caret
         self.render_highlight(mouse_x, mouse_y)
-
-        if self.syntax_coloring:  # syntax highlighting for code
-            list_of_dicts = self.get_syntax_coloring_dicts()
-        else:  # single-color text
-            list_of_dicts = self.get_single_color_dicts()
-        self.render_line_contents_by_dicts(list_of_dicts)
-
+        if self.syntax_highlighting_python:
+            # syntax highlighting for code
+            line_contents = self.get_syntax_coloring_dicts()
+        else:
+            # single-color text
+            line_contents = self.get_single_color_dicts()
+        self.render_line_contents(line_contents)
         self.render_caret()
 
+        # RENDERING 3 - scrollbar
         self.render_scrollbar_vertical()
         self.clock.tick(self.FPS)
```

### Comparing `pygame-texteditor-0.6.7/pygame_texteditor/_caret.py` & `pygame_texteditor-0.7.0/src/pygame_texteditor/_caret.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-
-
 def set_drag_start_by_mouse(self, mouse_x, mouse_y) -> None:
     # get line
-    self.drag_chosen_LineIndex_start = self.get_line_index(mouse_y)
+    self.drag_chosen_line_index_start = self.get_line_index(mouse_y)
 
     # end of line
-    if self.get_number_of_letters_in_line_by_mouse(mouse_y) < self.get_letter_index(mouse_x):
-        self.drag_chosen_LetterIndex_start = len(self.line_string_list[self.drag_chosen_LineIndex_start])
+    if self.get_number_of_letters_in_line_by_mouse(mouse_y) < self.get_letter_index(
+        mouse_x
+    ):
+        self.drag_chosen_letter_index_start = len(
+            self.editor_lines[self.drag_chosen_line_index_start]
+        )
 
     else:  # within existing line
-        self.drag_chosen_LetterIndex_start = self.get_letter_index(mouse_x)
+        self.drag_chosen_letter_index_start = self.get_letter_index(mouse_x)
 
 
 def set_drag_end_by_mouse(self, mouse_x, mouse_y) -> None:
     """
     Compact method to set both line and letter of drag_end based on mouse coordinates.
     """
     # set line
@@ -22,71 +24,93 @@
     self.set_drag_end_letter_by_mouse(mouse_x)
 
 
 def set_drag_end_line_by_mouse(self, mouse_y) -> None:
     """
     Sets self.drag_chosen_LineIndex_end by mouse_y.
     """
-    self.drag_chosen_LineIndex_end = self.get_line_index(mouse_y)
+    self.drag_chosen_line_index_end = self.get_line_index(mouse_y)
 
 
 def set_drag_end_letter_by_mouse(self, mouse_x) -> None:
     """
     Sets self.drag_chosen_LetterIndex_end by mouse_x.
     Dependent on self.drag_chosen_LineIndex_end.
     """
     # end of line
-    if self.get_letter_index(mouse_x) > self.get_number_of_letters_in_line_by_index(self.drag_chosen_LineIndex_end):
-        self.drag_chosen_LetterIndex_end = len(self.line_string_list[self.drag_chosen_LineIndex_end])
+    if self.get_letter_index(mouse_x) > self.get_number_of_letters_in_line_by_index(
+        self.drag_chosen_line_index_end
+    ):
+        self.drag_chosen_letter_index_end = len(
+            self.editor_lines[self.drag_chosen_line_index_end]
+        )
     else:  # within existing line
-        self.drag_chosen_LetterIndex_end = self.get_letter_index(mouse_x)
+        self.drag_chosen_letter_index_end = self.get_letter_index(mouse_x)
 
 
 def set_drag_start_after_last_line(self) -> None:
     # select last line
-    self.drag_chosen_LineIndex_start = self.maxLines - 1
+    self.drag_chosen_line_index_start = len(self.editor_lines) - 1
     # select last letter of the line
-    self.drag_chosen_LetterIndex_start = len(self.line_string_list[self.drag_chosen_LineIndex_start])
+    self.drag_chosen_letter_index_start = len(
+        self.editor_lines[self.drag_chosen_line_index_start]
+    )
 
 
 def set_drag_start_before_first_line(self) -> None:
-    self.drag_chosen_LineIndex_start = 0
-    self.drag_chosen_LetterIndex_start = 0
+    self.drag_chosen_line_index_start = 0
+    self.drag_chosen_letter_index_start = 0
 
 
 def set_drag_end_after_last_line(self) -> None:
     # select last line
-    self.drag_chosen_LineIndex_end = self.maxLines - 1
+    self.drag_chosen_line_index_end = len(self.editor_lines) - 1
     # select last letter of the line
-    self.drag_chosen_LetterIndex_end = len(self.line_string_list[self.drag_chosen_LineIndex_end])
+    self.drag_chosen_letter_index_end = len(
+        self.editor_lines[self.drag_chosen_line_index_end]
+    )
 
 
 def update_caret_position_by_drag_start(self) -> None:
     """
     # Updates cursor_X and cursor_Y positions based on the start position of a dragging operation.
     """
     # X Position
-    self.cursor_X = self.xline_start + (self.drag_chosen_LetterIndex_start * self.letter_size_X)
+    self.caret_x = self.line_start_x + (
+        self.drag_chosen_letter_index_start * self.letter_width
+    )
     # Y Position
-    self.cursor_Y = self.editor_offset_Y + (self.drag_chosen_LineIndex_start * self.line_gap) - \
-                    (self.showStartLine * self.lineHeight)
+    self.caret_y = (
+        self.editor_offset_y
+        + (self.drag_chosen_line_index_start * self.line_height_including_margin)
+        - (self.first_showable_line_index * self.letter_height)
+    )
 
 
 def update_caret_position_by_drag_end(self) -> None:
     """
     # Updates cursor_X and cursor_Y positions based on the end position of a dragging operation.
     """
     # X Position
-    self.cursor_X = self.xline_start + (self.drag_chosen_LetterIndex_end * self.letter_size_X)
+    self.caret_x = self.line_start_x + (
+        self.drag_chosen_letter_index_end * self.letter_width
+    )
     # Y Position
-    self.cursor_Y = self.editor_offset_Y + (self.drag_chosen_LineIndex_end * self.line_gap) - \
-                    (self.showStartLine * self.lineHeight)
+    self.caret_y = (
+        self.editor_offset_y
+        + (self.drag_chosen_line_index_end * self.line_height_including_margin)
+        - (self.first_showable_line_index * self.letter_height)
+    )
 
 
 def update_caret_position(self) -> None:
-    """
-    # Updates cursor_X and cursor_Y positions based on current position by line and letter indices
-    """
-    self.cursor_X = self.xline_start + (self.chosen_LetterIndex * self.letter_size_X)
+    """Update the caret position based on current position by line and letter indices.
 
-    self.cursor_Y = self.editor_offset_Y + (self.chosen_LineIndex * self.line_gap) - \
-                    (self.showStartLine * self.lineHeight)
+    We add one pixel to the x coordinate so the caret is fully visible if it is at the start of the line.
+    """
+    self.caret_x = (
+        self.line_start_x + (self.chosen_letter_index * self.letter_width) + 1
+    )
+    self.caret_y = self.editor_offset_y + (
+        (self.chosen_line_index - self.first_showable_line_index)
+        * self.line_height_including_margin
+    )
```

### Comparing `pygame-texteditor-0.6.7/pygame_texteditor/_customization.py` & `pygame_texteditor-0.7.0/src/pygame_texteditor/_customization.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,108 +1,157 @@
-import os
-import re
 import math
+import os
 import pathlib
-import yaml
+import re
+
 import pygame
+import yaml
+
+current_dir = os.path.dirname(__file__)
 
 
-def set_key_repetition(self, delay=300, intervall=30) -> None:
+def set_key_repetition(self, delay=300, interval=30) -> None:
     """
     The delay parameter is the number of milliseconds before the first repeated pygame.KEYDOWN event will be sent.
     After that, another pygame.KEYDOWN event will be sent every interval milliseconds.
     """
     self.key_initial_delay = delay
-    self.key_continued_intervall = intervall 
-    pygame.key.set_repeat(self.key_initial_delay, self.key_continued_intervall) 
+    self.key_continued_interval = interval
+    pygame.key.set_repeat(self.key_initial_delay, self.key_continued_interval)
 
 
-def set_font_size(self, size=16) -> None:
+def set_font_from_ttf(self, absolute_path_to_ttf: str) -> None:
     """
-    Sets the given size as font size and re-calculates necessary changes.
+    Sets the font given a ttf file.
+
+    Disclaimer: As the width of a letter (space) is only calculated once after setting the font_size, any fonts that are not
+    monospace will lead to the editor not working correctly anymore, as it cannot be determined anymore, between which
+    letters the user clicked.
     """
-    self.letter_size_Y = size
-    current_dir = os.path.dirname(__file__)
-    self.courier_font = pygame.font.Font(os.path.join(current_dir, "elements/fonts/Courier.ttf"),
-                                         self.letter_size_Y)
-    letter_width = self.courier_font.render(" ", 1, (0, 0, 0)).get_width()
-    self.letter_size_X = letter_width
-    self.line_gap = 3 + self.letter_size_Y
-    self.showable_line_numbers_in_editor = int(math.floor(self.textAreaHeight / self.line_gap))
+    self.ttf_path = absolute_path_to_ttf
+
+    # force all the font settings to re-render
+    set_font_size(self, self.letter_height)
+
+
+def set_font_size(self, size=16) -> None:
+    """Sets the given size as font size and re-calculates necessary changes."""
+    self.editor_font = pygame.font.Font(self.ttf_path, size=size)
+    self.letter_height = size
+    self.letter_width = self.editor_font.render(" ", 1, (0, 0, 0)).get_width()
+    self.line_height_including_margin = self.letter_height + self.line_margin
+    self.showable_line_numbers_in_editor = int(
+        math.floor(self.editor_height / self.line_height_including_margin)
+    )
+    # As the font size also influences the size of the line numbers, we need to recalculate some their spacing
+    self.line_number_width = self.editor_font.render(" ", 1, (0, 0, 0)).get_width() * 2
+    self.line_start_x = self.editor_offset_x + self.line_number_width
 
 
 def set_line_numbers(self, b) -> None:
     """
     Activates/deactivates showing the line numbers in the editor
     """
-    self.displayLineNumbers = b
-    if self.displayLineNumbers:
-        self.lineNumberWidth = 27  # line number background width and also offset for text!
-        self.xline_start = self.editor_offset_X + self.xline_start_offset
-        self.xline = self.editor_offset_X + self.xline_start_offset
+    self.display_line_numbers = b
+    if self.display_line_numbers:
+        self.line_number_width = self.editor_font.render(" ", 1, (0, 0, 0)).get_width()
+        self.line_start_x = self.editor_offset_x + self.line_number_width
     else:
-        self.lineNumberWidth = 0
-        self.xline_start = self.editor_offset_X
-        self.xline = self.editor_offset_X
+        self.line_number_width = 0
+        self.line_start_x = self.editor_offset_x
 
 
 def set_syntax_highlighting(self, b) -> None:
     """
     Activates / deactivates syntax highlighting.
     If activated, creates the lexer and formatter and sets the formatter's style.
     """
-    self.syntax_coloring = b
+    self.syntax_highlighting_python = b
 
 
 def set_colorscheme_from_yaml(self, path_to_yaml) -> None:
-
     def get_rgb_by_key(dict, key):
-        return tuple([int(x) for x in re.findall(r'(\d{1,3})', dict[key])])
+        return tuple([int(x) for x in re.findall(r"(\d{1,3})", dict[key])])
 
     try:
         with open(path_to_yaml) as file:
             color_dict = yaml.load(file, Loader=yaml.FullLoader)
 
-            self.codingBackgroundColor = get_rgb_by_key(color_dict, 'codingBackgroundColor')
-            self.codingScrollBarBackgroundColor = get_rgb_by_key(color_dict, 'codingScrollBarBackgroundColor')
-            self.lineNumberColor = get_rgb_by_key(color_dict, 'lineNumberColor')
-            self.lineNumberBackgroundColor = get_rgb_by_key(color_dict, 'lineNumberBackgroundColor')
-            self.textColor = get_rgb_by_key(color_dict, 'textColor')
-
-            self.formatter.textColor_normal = get_rgb_by_key(color_dict, 'textColor_normal')
-            self.formatter.textColor_comments = get_rgb_by_key(color_dict, 'textColor_comments')
-            self.formatter.textColor_quotes = get_rgb_by_key(color_dict, 'textColor_quotes')
-            self.formatter.textColor_operators = get_rgb_by_key(color_dict, 'textColor_operators')
-            self.formatter.textColor_keywords = get_rgb_by_key(color_dict, 'textColor_keywords')
-            self.formatter.textColor_function = get_rgb_by_key(color_dict, 'textColor_function')
-            self.formatter.textColor_builtin = get_rgb_by_key(color_dict, 'textColor_builtin')
+            self.color_coding_background = get_rgb_by_key(
+                color_dict, "codingBackgroundColor"
+            )
+            self.color_scrollbar_background = get_rgb_by_key(
+                color_dict, "codingScrollBarBackgroundColor"
+            )
+            self.color_line_number_font = get_rgb_by_key(color_dict, "lineNumberColor")
+            self.color_line_number_background = get_rgb_by_key(
+                color_dict, "lineNumberBackgroundColor"
+            )
+            self.color_text = get_rgb_by_key(color_dict, "textColor")
+
+            self.color_formatter.textColor_normal = get_rgb_by_key(
+                color_dict, "textColor_normal"
+            )
+            self.color_formatter.textColor_comments = get_rgb_by_key(
+                color_dict, "textColor_comments"
+            )
+            self.color_formatter.textColor_quotes = get_rgb_by_key(
+                color_dict, "textColor_quotes"
+            )
+            self.color_formatter.textColor_operators = get_rgb_by_key(
+                color_dict, "textColor_operators"
+            )
+            self.color_formatter.textColor_keywords = get_rgb_by_key(
+                color_dict, "textColor_keywords"
+            )
+            self.color_formatter.textColor_function = get_rgb_by_key(
+                color_dict, "textColor_function"
+            )
+            self.color_formatter.textColor_builtin = get_rgb_by_key(
+                color_dict, "textColor_builtin"
+            )
 
     except FileNotFoundError:
         raise FileNotFoundError("Could not find the style file '" + path_to_yaml + "'.")
     except KeyError as e:
-        raise KeyError("Could not find all necessary color-keys in the style file '" + path_to_yaml + "'. " +
-                       "Missing key: " + str(e))
+        raise KeyError(
+            "Could not find all necessary color-keys in the style file '"
+            + path_to_yaml
+            + "'. "
+            + "Missing key: "
+            + str(e)
+        )
 
 
 def set_colorscheme(self, style) -> None:
     """
     Sets the color scheme for the editor and for syntax highlighting if the latter is enabled based on
     one of the editor's default styles.
     """
     if style in ("bright", "dark"):
-        default_path = os.path.join(str(pathlib.Path(__file__).parent.absolute()),
-            'elements', 'colorstyles', style + ".yml")
+        default_path = os.path.join(
+            str(pathlib.Path(__file__).parent.absolute()),
+            "elements",
+            "colorstyles",
+            style + ".yml",
+        )
         self.set_colorscheme_from_yaml(default_path)
     else:
-        raise ValueError("No default style with the name '" + style + "' available. " +
-                         "\n\tAvailable styles are 'dark' and 'bright'. \n\tFor your " +
-                         "own custom styles, use the method 'set_colorscheme_from_yaml(path_to_yaml)' " +
-                         "and have a look at the docs.")
+        raise ValueError(
+            "No default style with the name '"
+            + style
+            + "' available. "
+            + "\n\tAvailable styles are 'dark' and 'bright'. \n\tFor your "
+            + "own custom styles, use the method 'set_colorscheme_from_yaml(path_to_yaml)' "
+            + "and have a look at the docs."
+        )
 
 
 def set_cursor_mode(self, mode: str = "blinking"):
     if mode == "blinking":
         self.static_cursor = False
     elif mode == "static":
         self.static_cursor = True
     else:
-        raise ValueError(f"Value '{mode}' is not a valid cursor mode. Set either to 'blinking' or 'static'.")
+        raise ValueError(
+            f"Value '{mode}' is not a valid cursor mode. Set either to 'blinking' or 'static'."
+        )
```

### Comparing `pygame-texteditor-0.6.7/pygame_texteditor/_editor_getters.py` & `pygame_texteditor-0.7.0/src/pygame_texteditor/_editor_getters.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,54 @@
-
-
 def get_line_index(self, mouse_y) -> int:
     """
     Returns possible line-position of mouse -> does not take into account
     how many lines there actually are!
     """
-    return int(((mouse_y - self.editor_offset_Y) / self.line_gap) + (self.showStartLine))
+    return int(
+        ((mouse_y - self.editor_offset_y) / self.line_height_including_margin)
+        + self.first_showable_line_index
+    )
 
 
 def get_letter_index(self, mouse_x) -> int:
     """
     Returns possible letter-position of mouse.
 
-    The function is independent from any specific line, so we could possible return a letter_index which
+    The function is independent of any specific line, so we could possibly return a letter_index which
     is bigger than the letters in the line.
     Returns at least 0 to make sure it is possibly a valid index.
     """
-    letter = int((mouse_x - self.xline_start) / self.letter_size_X)
+    letter = int((mouse_x - self.line_start_x) / self.letter_width)
     letter = 0 if letter < 0 else letter
     return letter
 
 
 def get_number_of_letters_in_line_by_mouse(self, mouse_y) -> int:
     line_index = get_line_index(self, mouse_y)
     return get_number_of_letters_in_line_by_index(self, line_index)
 
 
 def get_number_of_letters_in_line_by_index(self, index) -> int:
-    return len(self.line_string_list[index])
+    return len(self.editor_lines[index])
 
 
 def get_showable_lines(self) -> int:
     """
     Return the number of lines which are shown. Less than maximum if less lines are in the array.
     """
-    if self.showable_line_numbers_in_editor + self.showStartLine < self.maxLines:
-        return self.showable_line_numbers_in_editor + self.showStartLine
+    if self.showable_line_numbers_in_editor + self.first_showable_line_index < len(
+        self.editor_lines
+    ):
+        return self.showable_line_numbers_in_editor + self.first_showable_line_index
     else:
-        return self.maxLines
+        return len(self.editor_lines)
 
 
 def line_is_visible(self, line) -> bool:
     """
     Calculate whether the line is being shown in the editor
     """
-    return self.showStartLine <= line < self.showStartLine + self.showable_line_numbers_in_editor
-
+    return (
+        self.first_showable_line_index
+        <= line
+        < self.first_showable_line_index + self.showable_line_numbers_in_editor
+    )
```

### Comparing `pygame-texteditor-0.6.7/pygame_texteditor/_other.py` & `pygame_texteditor-0.7.0/src/pygame_texteditor/_other.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-
 def jump_to_start(self, line_start, line_end, letter_start, letter_end) -> None:
     """
     Chosen LineIndex set to start of highlighted area
     """
     if line_start <= line_end:
         # downward highlight or the same line
-        self.chosen_LineIndex = line_start
-        self.chosen_LetterIndex = letter_start
+        self.chosen_line_index = line_start
+        self.chosen_letter_index = letter_start
     else:  # upward highlight
-        self.chosen_LineIndex = line_end
-        self.chosen_LetterIndex = letter_end
+        self.chosen_line_index = line_end
+        self.chosen_letter_index = letter_end
 
 
 def jump_to_end(self, line_start, line_end, letter_start, letter_end) -> None:
     """
     Chosen LineIndex set to end of highlighted area
     """
     if line_start <= line_end:
         # downward highlight or the same line
-        self.chosen_LineIndex = line_end
-        self.chosen_LetterIndex = letter_end
+        self.chosen_line_index = line_end
+        self.chosen_letter_index = letter_end
     else:  # upward highlight
-        self.chosen_LineIndex = line_start
-        self.chosen_LetterIndex = letter_start
+        self.chosen_line_index = line_start
+        self.chosen_letter_index = letter_start
 
 
 def reset_after_highlight(self) -> None:
     """
     Reset caret, clickdown_cycles and dragged booleans.
     """
     self.dragged_active = False  # deactivate highlight
     self.dragged_finished = True  # highlight is finished
     self.update_caret_position()  # update caret position to chosen_Index (Line+Letter)
     self.last_clickdown_cycle = 0  # reset drag-cycle
     self.last_clickup_cycle = -1
-    self.rerenderLineNumbers = True
+    self.render_line_numbers_flag = True
 
-    if len(self.line_string_list) <= self.showable_line_numbers_in_editor:
-        self.showStartLine = 0  # update first showable line
+    if len(self.editor_lines) <= self.showable_line_numbers_in_editor:
+        self.first_showable_line_index = 0  # update first showable line
```

### Comparing `pygame-texteditor-0.6.7/pygame_texteditor/_rendering_highlighting.py` & `pygame_texteditor-0.7.0/src/pygame_texteditor/_rendering_highlighting.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,91 +5,123 @@
     """
     Renders highlighted area:
     1. During drag-action -> area starts at drag_start and follows mouse
     2. After drag-action -> area stays confined to selected area by drag_start and drag_end
     """
 
     if self.dragged_active:  # some text is highlighted or being highlighted
-        line_start = self.drag_chosen_LineIndex_start
-        letter_start = self.drag_chosen_LetterIndex_start
+        line_start = self.drag_chosen_line_index_start
+        letter_start = self.drag_chosen_letter_index_start
 
-        if self.dragged_finished:  # highlighting operation is done, user "clicked-up" with the left mouse button
-            line_end = self.drag_chosen_LineIndex_end
-            letter_end = self.drag_chosen_LetterIndex_end
+        if (
+            self.dragged_finished
+        ):  # highlighting operation is done, user "clicked-up" with the left mouse button
+            line_end = self.drag_chosen_line_index_end
+            letter_end = self.drag_chosen_letter_index_end
             if letter_end < 0:
                 letter_end = 0
-            self.highlight_lines(line_start, letter_start, line_end, letter_end)  # Actual highlighting
+            self.highlight_lines(
+                line_start, letter_start, line_end, letter_end
+            )  # Actual highlighting
 
         else:  # active highlighting -> highlighted area follows mouse movements
             line_end = self.get_line_index(mouse_y)
             letter_end = self.get_letter_index(mouse_x)
             # adapt line_end: if mouse_y below showable area / existing lines,
             if line_end >= self.get_showable_lines():
-                line_end = self.get_showable_lines() - 1  # select last showable/existing line as line_end
+                line_end = (
+                    self.get_showable_lines() - 1
+                )  # select last showable/existing line as line_end
 
             # Correct letter_end based on cursor position / letters in the cursor's line
             if letter_end < 0:  # cursor is left of the line
                 letter_end = 0
-            elif letter_end > len(self.line_string_list[line_end]):
-                letter_end = len(self.line_string_list[line_end])
+            elif letter_end > len(self.editor_lines[line_end]):
+                letter_end = len(self.editor_lines[line_end])
 
-            self.highlight_lines(line_start, letter_start, line_end, letter_end)  # Actual highlighting
+            self.highlight_lines(
+                line_start, letter_start, line_end, letter_end
+            )  # Actual highlighting
 
 
 def highlight_lines(self, line_start, letter_start, line_end, letter_end) -> None:
     """
     Highlights multiple lines based on indizies of starting & ending lines and letters.
     """
     if line_start == line_end:  # single-line highlight
         self.highlight_from_letter_to_letter(line_start, letter_start, letter_end)
     else:  # multi-line highlighting
-        if line_start > line_end:  # swap variables based on up/downward highlight to make code more readable
+        if (
+            line_start > line_end
+        ):  # swap variables based on up/downward highlight to make code more readable
             line_start, line_end = line_end, line_start
             letter_start, letter_end = letter_end, letter_start
 
-        for i, line_number in enumerate(range(line_start, line_end + 1)):  # for each line
+        for i, line_number in enumerate(
+            range(line_start, line_end + 1)
+        ):  # for each line
             if i == 0:  # first line
-                self.highlight_from_letter_to_end(line_number, letter_start)  # right leaning highlight
+                self.highlight_from_letter_to_end(
+                    line_number, letter_start
+                )  # right leaning highlight
             elif i < len(range(line_start, line_end)):  # middle line
                 self.highlight_entire_line(line_number)
             else:  # last line
-                self.highlight_from_start_to_letter(line_number, letter_end)  # left leaning highlight
+                self.highlight_from_start_to_letter(
+                    line_number, letter_end
+                )  # left leaning highlight
 
 
 def highlight_from_letter_to_end(self, line, letter) -> None:
     """
     Highlight from a specific letter by index to the end of a line.
     """
     if self.line_is_visible(line):
         x1, y1 = self.get_rect_coord_from_indizes(line, letter)
-        x2, y2 = self.get_rect_coord_from_indizes(line, len(self.line_string_list[line]))
-        pygame.draw.rect(self.screen, (0, 0, 0), pygame.Rect(x1, y1, x2 - x1, self.line_gap))
+        x2, y2 = self.get_rect_coord_from_indizes(line, len(self.editor_lines[line]))
+        pygame.draw.rect(
+            self.screen,
+            (0, 0, 0),
+            pygame.Rect(x1, y1, x2 - x1, self.line_height_including_margin),
+        )
 
 
 def highlight_from_start_to_letter(self, line, letter) -> None:
     """
     Highlight from the beginning of a line to a specific letter by index.
     """
     if self.line_is_visible(line):
         x1, y1 = self.get_rect_coord_from_indizes(line, 0)
         x2, y2 = self.get_rect_coord_from_indizes(line, letter)
-        pygame.draw.rect(self.screen, (0, 0, 0), pygame.Rect(x1, y1, x2 - x1, self.line_gap))
+        pygame.draw.rect(
+            self.screen,
+            (0, 0, 0),
+            pygame.Rect(x1, y1, x2 - x1, self.line_height_including_margin),
+        )
 
 
 def highlight_entire_line(self, line) -> None:
     """
     Full highlight of the entire line - first until last letter.
     """
     if self.line_is_visible(line):
         x1, y1 = self.get_rect_coord_from_indizes(line, 0)
-        x2, y2 = self.get_rect_coord_from_indizes(line, len(self.line_string_list[line]))
-        pygame.draw.rect(self.screen, (0, 0, 0), pygame.Rect(x1, y1, x2 - x1, self.line_gap))
+        x2, y2 = self.get_rect_coord_from_indizes(line, len(self.editor_lines[line]))
+        pygame.draw.rect(
+            self.screen,
+            (0, 0, 0),
+            pygame.Rect(x1, y1, x2 - x1, self.line_height_including_margin),
+        )
 
 
 def highlight_from_letter_to_letter(self, line, letter_start, letter_end) -> None:
     """
     Highlights within a single line from letter to letter by indizes.
     """
     if self.line_is_visible(line):
         x1, y1 = self.get_rect_coord_from_indizes(line, letter_start)
         x2, y2 = self.get_rect_coord_from_indizes(line, letter_end)
-        pygame.draw.rect(self.screen, (0, 0, 0), pygame.Rect(x1, y1, x2 - x1, self.line_gap))
+        pygame.draw.rect(
+            self.screen,
+            (0, 0, 0),
+            pygame.Rect(x1, y1, x2 - x1, self.line_height_including_margin),
+        )
```

### Comparing `pygame-texteditor-0.6.7/pygame_texteditor/_scrollbar_vertical.py` & `pygame_texteditor-0.7.0/src/pygame_texteditor/_scrollbar_vertical.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,37 +3,55 @@
 
 def render_scrollbar_vertical(self) -> None:
     self.display_scrollbar()
 
 
 def display_scrollbar(self):
     # Scroll Bar
-
-    if len(self.line_string_list) <= self.showable_line_numbers_in_editor:
+    if len(self.editor_lines) <= self.showable_line_numbers_in_editor:
         self.scrollbar = None
         return  # if scrollbar is not needed, don't show.
 
     # scroll bar is a fraction of the space
-    w = self.scrollBarWidth 
-    x = self.editor_offset_X + self.textAreaWidth - self.scrollBarWidth - 2  # -2 for space between edge & scrollbar
-    y = int(self.editor_offset_Y + (w/2) + (self.textAreaHeight * ((self.showStartLine * 1.0) / self.maxLines)))
-    h = int((self.textAreaHeight - w) * ((self.showable_line_numbers_in_editor * 1.0) / self.maxLines))
+    w = self.scrollbar_width
+    x = (
+        self.editor_offset_x
+        + self.editor_width
+        - self.scrollbar_width
+        - self.padding_between_edge_and_scrollbar
+    )
+    y = int(
+        self.editor_offset_y
+        + (self.scrollbar_width / 2)
+        + (
+            (self.editor_height - self.scrollbar_width)
+            * ((self.first_showable_line_index * 1.0) / len(self.editor_lines))
+        )
+    )
+    # Entire height minus the diameter as the ends are rounded. Multiplied with the fraction of displayable lines.
+    h = int(
+        (self.editor_height - (2 * self.scrollbar_width))
+        * ((self.showable_line_numbers_in_editor * 1.0) / len(self.editor_lines))
+    )
     self.scrollbar = pygame.Rect(x, y, w, h)
 
-    pygame.draw.circle(self.screen, self.color_scrollbar, (int(x + (w/2)), y), int(w/2))  # top round corner
-    pygame.draw.rect(self.screen, self.color_scrollbar, self.scrollbar)  # actual scrollbar
-    pygame.draw.circle(self.screen, self.color_scrollbar, (int(x + (w/2)), y + h), int(w/2))  # bottom round corner
+    pygame.draw.circle(
+        self.screen, self.color_scrollbar, (int(x + (w / 2)), y), int(w / 2)
+    )  # top round corner
+    pygame.draw.rect(
+        self.screen, self.color_scrollbar, self.scrollbar
+    )  # actual scrollbar
+    pygame.draw.circle(
+        self.screen, self.color_scrollbar, (int(x + (w / 2)), y + h), int(w / 2)
+    )  # bottom round corner
 
 
 def scrollbar_up(self) -> None:
-    self.showStartLine -= 1
-    self.cursor_Y += self.line_gap
-    self.rerenderLineNumbers = True
-    
+    self.first_showable_line_index -= 1
+    self.caret_y += self.line_height_including_margin
+    self.render_line_numbers_flag = True
 
 
 def scrollbar_down(self) -> None:
-    self.showStartLine += 1
-    self.cursor_Y -= self.line_gap
-    self.rerenderLineNumbers = True
-
-
+    self.first_showable_line_index += 1
+    self.caret_y -= self.line_height_including_margin
+    self.render_line_numbers_flag = True
```

### Comparing `pygame-texteditor-0.6.7/pygame_texteditor/_usage.py` & `pygame_texteditor-0.7.0/src/pygame_texteditor/_usage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,72 @@
-import pygame
 import math
 from typing import List
 
+import pygame
+
 
 def get_text_as_string(self) -> str:
     """
     Returns the entire text of the editor as a single string.
     Linebreak characters are used to differentiate between lines.
     :param self:  Texteditor-Class
     :return: String
     """
-    return "\n".join(self.line_string_list)
+    return "\n".join(self.editor_lines)
 
 
 def get_text_as_list(self) -> List:
     """
     Returns the text in it's logical form as a list of lines.
     :param self:  Texteditor-Class
     :return: List of lines containing the text. Lines cane be empty Strings.
     """
-    return self.line_string_list
+    return self.editor_lines
 
 
 def clear_text(self) -> None:
     """
     Clears the textarea.
     :param self: Texteditor-Class
     :return: None
     """
-    self.line_string_list = []  # LOGIC: List of actual Strings for each line
-    self.maxLines = int(math.floor(self.textAreaHeight / self.lineHeight))
-    self.showStartLine = 0
-    for i in range(self.maxLines):  # from 0 to maxLines:
-        self.line_string_list.append("")  # Add a line
+    # Create lines
+    self.editor_lines = [
+        "" for _ in range(int(math.floor(self.editor_height / self.letter_height)))
+    ]
+    self.first_showable_line_index = 0
 
     # reset caret
-    self.firstiteration_boolean = True  # redraws background
-    self.rerenderLineNumbers = True
-    self.chosen_LineIndex = 0
-    self.chosen_LetterIndex = 0
+    self.first_iteration_boolean = True  # redraws background
+    self.render_line_numbers_flag = True
+    self.chosen_line_index = 0
+    self.chosen_letter_index = 0
     self.dragged_active = False
     self.dragged_finished = True
-    self.scroll_dragging = False
-    self.drag_chosen_LineIndex_start = 0
-    self.drag_chosen_LetterIndex_start = 0
-    self.drag_chosen_LineIndex_end = 0
-    self.drag_chosen_LetterIndex_end = 0
+    self.scrollbar_is_being_dragged = False
+    self.drag_chosen_line_index_start = 0
+    self.drag_chosen_letter_index_start = 0
+    self.drag_chosen_line_index_end = 0
+    self.drag_chosen_letter_index_end = 0
     self.last_clickdown_cycle = 0
     self.last_clickup_cycle = 0
     self.cycleCounter = 0
     self.update_caret_position()
     self.cycleCounter = 0
 
 
 def set_text_from_list(self, text_list) -> None:
     """
     Sets the text of the editor based on a list of strings. Each item in the list represents one line.
     """
     self.clear_text()
-    self.line_string_list = text_list
-    self.maxLines = len(self.line_string_list)
-    self.rerenderLineNumbers = True
+    self.editor_lines = text_list
+    self.render_line_numbers_flag = True
 
 
 def set_text_from_string(self, string) -> None:
     """
     Sets the text of the editor based on a string. Linebreak characters are parsed.
     """
     self.clear_text()
-    self.line_string_list = string.split('\n')
-    self.maxLines = len(self.line_string_list)
-    self.rerenderLineNumbers = True
+    self.editor_lines = string.split("\n")
+    self.render_line_numbers_flag = True
```

### Comparing `pygame-texteditor-0.6.7/pygame_texteditor/elements/fonts/Courier.ttf` & `pygame_texteditor-0.7.0/src/pygame_texteditor/elements/fonts/Courier.ttf`

 * *Files identical despite different names*

### Comparing `pygame-texteditor-0.6.7/pygame_texteditor.egg-info/PKG-INFO` & `pygame_texteditor-0.7.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,204 +1,37 @@
-Metadata-Version: 2.1
-Name: pygame-texteditor
-Version: 0.6.7
-Summary: A WYSIWYG-texteditor based on pygame.
-Author: CribberSix
-Author-email: cribbersix@gmail.com
-License: MIT
-Keywords: pygame,texteditor,text,editor
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# A WYSIWYG-texteditor based on pygame for pygame
-
-![PyPI](https://img.shields.io/pypi/v/pygame-texteditor?color=%233775A9&label=pypi%20package&style=plastic)
-![GitHub](https://img.shields.io/github/license/CribberSix/pygame-texteditor?style=plastic)
-
-## Introduction & examples
-
-The text editor can be inserted into any existing pygame window. 
-A minimal code example of it being activated within an existing pygame window can be found below.
-
-The code editor comes with line numbers and syntax highlighting for python if enabled:
-
-![](./resources/example_one.png)
-
-Example with default configuration:
-
-![](./resources/example_two.png)
-
-## Usage
-
-The texteditor takes 5 obligatory parameters and 3 optional parameters.
-
-##### Obligatory parameters
-- ```offset_X``` : integer - the offset from the left border of the pygame screen
-- ```offset_y``` : integer - the offset from the top border of the pygame screen
-- ```textAreaWidth``` : integer - the width of texteditor
-- ```textAreaHeight``` : integer - the height of texteditor
-- ```screen``` : pygame display surface - on which the texteditor is to be displayed
-
-##### Optional Parameters with default values
-
-- ```line_numbers_flag``` - a boolean enabling showing line numbers 
-    > Default: ```False```
-- ```style``` - a String setting the color scheme of editor and syntax highlighting 
-    > Default: ```'dark'```
-- ```syntax_highlighting_flag``` - a boolean enabling syntax highlighting for Python code 
-    > Default: ```False```
-
-## Setup
-
-##### Minimal pygame setup
-
-```
-import pygame
-from pygame_texteditor import TextEditor
-
-pygame.init()
-screenHeight = 600
-screenWidth = 900
-screen = pygame.display.set_mode((screenWidth, screenHeight))
-pygame.display.set_caption("Pygame")
-pygame.display.get_surface().fill((200, 200, 200))  # background coloring
-
-```
-##### Minimal texteditor setup
-```
-# parameters
-screen = pygame.display.get_surface()  # get existing pygame window/screen
-offset_X = 50  # offset from the left border of the pygame window
-offset_Y = 50  # offset from the top border of the pygame window
-textAreaHeight = 500
-textAreaWidth = 800
-
-
-# Instantiation
-TX = TextEditor(offset_X, offset_Y, textAreaWidth, textAreaHeight, screen)
-TX.set_line_numbers(True)  # optional 
-TX.set_syntax_highlighting(True)  # optional
-
-while True:  # pygame-loop
-    # capture input
-    pygame_events = pygame.event.get()
-    pressed_keys = pygame.key.get_pressed()
-    mouse_x, mouse_y = pygame.mouse.get_pos()
-    mouse_pressed = pygame.mouse.get_pressed()
-
-    # display editor functionality once per loop
-    TX.display_editor(pygame_events, pressed_keys, mouse_x, mouse_y, mouse_pressed)
-
-    # update pygame window
-    pygame.display.flip()  
-
-
-```
-
-##### Retrieving text from the editor
-
-The editor offers the function `get_text_as_string()` to retrieve the entire text 
-as a String from the editor. Lines are separated by the new line character ```\n```.
-
-The editor offers the function `get_text_as_list()` to retrieve the entire text as a list from the editor. 
-Each String-item in the list represents one line from the editor.
-
-##### Removing text from the editor
-
-The editor offers the function `clear_text()` to clear the editor of any text.
-
-
-##### Inserting text into the editor
-
-Inserting text can be done by using one of the two available functions: 
-1. With a list of strings in which each string represents one line, or
-2. With a string which includes linebreak characters which get parsed. 
-
-```
-set_text_from_list(["First line", "Second Line.", "Third Line."]
-set_text_from_string("First line.\nSecond line.\nThird Line")
-```
-
-## Customization
-
-#### Cursor mode 
-
-Cursor mode can either be `static` or `blinking` (=default). 
-
-```python
-set_cursor_mode("static")
-set_cursor_mode("blinking")
-```
-
-#### Key repetition speeds
-
-While a key is being held, multiple key events are being triggered. 
-The delay of the first repetition as well as the interval between all sequential key triggers can be 
-customized by using the function `set_key_repetition(delay=300, intervall=30)`. 
-
-From the [official documentation](http://www.pygame.org/docs/ref/key.html#pygame.key.set_repeat): 
-> The delay parameter is the number of milliseconds before the first repeated pygame.KEYDOWN event will be sent.
-> After that, another pygame.KEYDOWN event will be sent every interval milliseconds.
-
-#### Font size
-
-Font size can be customized with the command `set_font_size(size)` - the parameter is an integer 
-with the default value `12` to be able to reset it. 
-
-#### Line Numbers 
-Line numbers can be shown on the left side of the editor. Line numbers begin with 0 as is the Pythonian way. 
-
-Line numbers can be enabled and disabled with ```set_line_numbers(Boolean)```.
-
-
-#### Syntax Highlighting
-
-The editor comes with syntax highlighting for Python code. Tokenization is based on the ```pygment``` package. 
-
-Syntax highlighting can be enabled/disabled with ```set_syntax_coloring(boolean_value)```.
-
-The syntax colors being used are also specified in the yml style file.
-
-
-#### Color-scheme customization
-
-The editor uses a yml file to set the color-scheme for the editor itself and for the syntax coloring. 
-
-Two styles are delivered with the editor, they can be activated respectively by:
-- `set_colorscheme("dark")`
-- `set_colorscheme("bright")`
-
-A custom style can be loaded with the following method from a created yml file: 
-- `set_colorscheme_from_yaml("X:\path\to\custom\filename.yml")`
-
-All keys must be present with values. Acceptable values are 
-RGB colors in the following format: ```(255, 255, 255)``` or ```255, 255, 255```.
-
-The following keys are required in the ```stylename.yml``` file, syntax colors are only used if syntax
-highlighting is enabled, but are still required to be included.
-
-*Editor colors*
-- `codingBackgroundColor`
-- `codingScrollBarBackgroundColor`
-- `lineNumberColor`
-- `lineNumberBackgroundColor`
-- `textColor`
-
-*Syntax colors*
-- `textColor_normal`
-- `textColor_comments`
-- `textColor_quotes`
-- `textColor_operators`
-- `textColor_keywords`
-- `textColor_function`
-- `textColor_builtin`
-
+# -*- coding: utf-8 -*-
+from setuptools import setup
+
+package_dir = \
+{'': 'src'}
+
+packages = \
+['pygame_texteditor']
+
+package_data = \
+{'': ['*'],
+ 'pygame_texteditor': ['elements/colorstyles/*',
+                       'elements/fonts/*',
+                       'elements/graphics/*']}
+
+install_requires = \
+['PyYAML>=5.3.1', 'Pygments>=2.6.1', 'pygame>=1.9.6', 'pyperclip>=1.8.1']
+
+setup_kwargs = {
+    'name': 'pygame-texteditor',
+    'version': '0.7.0',
+    'description': 'A WYSIWYG-texteditor based on pygame.',
+    'long_description': '# A WYSIWYG-texteditor based on pygame for pygame\n\n![PyPI](https://img.shields.io/pypi/v/pygame-texteditor?color=%233775A9&label=pypi%20package&style=plastic)\n![GitHub](https://img.shields.io/github/license/CribberSix/pygame-texteditor?style=plastic)\n\n## Introduction & examples\n\nThe text editor can be inserted into any existing pygame window.\nA minimal code example of it being activated within an existing pygame window can be found below.\n\nThe code editor comes with line numbers and syntax highlighting for python if enabled:\n\n![](./resources/example_one.png)\n\nExample with default configuration:\n\n![](./resources/example_two.png)\n\n## Usage\n\nThe texteditor takes 5 obligatory parameters and 4 optional parameters.\n\n##### Obligatory parameters\n- ```offset_X``` : integer - the offset from the left border of the pygame screen\n- ```offset_y``` : integer - the offset from the top border of the pygame screen\n- ```editor_width``` : integer - the width of texteditor\n- ```editor_height``` : integer - the height of texteditor\n- ```screen``` : pygame display surface - on which the texteditor is to be displayed\n\n##### Optional Parameters with default values\n\n- ```display_line_numbers``` - a boolean enabling showing line numbers\n    > Default: ```False```\n- ```style``` - a String setting the color scheme of editor and syntax highlighting\n    > Default: ```\'dark\'```\n- ```syntax_highlighting_python``` - a boolean enabling syntax highlighting for Python code\n    > Default: ```False```\n- ```font_size``` - an integer to set for the font size.\n    > Default: ```16```\n\n## Setup\n\n##### Minimal pygame setup\n\n```python\nimport pygame\n\npygame.init()\nscreenHeight = 600\nscreenWidth = 900\nscreen = pygame.display.set_mode((screenWidth, screenHeight))\npygame.display.set_caption("Pygame")\npygame.display.get_surface().fill((200, 200, 200))  # background coloring\n```\n\n##### Minimal texteditor setup\n\n```python\nimport pygame\nfrom pygame_texteditor import TextEditor\n\n# parameters\nscreen = pygame.display.get_surface()  # get existing pygame window/screen\noffset_X = 50  # offset from the left border of the pygame window\noffset_Y = 50  # offset from the top border of the pygame window\neditor_height = 800\neditor_width = 500\n\n\n# Instantiation\nTX = TextEditor(offset_X, offset_Y, editor_width, editor_height, screen)\nTX.set_line_numbers(True)  # optional\nTX.set_syntax_highlighting(True)  # optional\n\nwhile True:  # pygame-loop\n    # capture input\n    pygame_events = pygame.event.get()\n    pressed_keys = pygame.key.get_pressed()\n    mouse_x, mouse_y = pygame.mouse.get_pos()\n    mouse_pressed = pygame.mouse.get_pressed()\n\n    # display editor functionality once per loop\n    TX.display_editor(pygame_events, pressed_keys, mouse_x, mouse_y, mouse_pressed)\n\n    # update pygame window\n    pygame.display.flip()\n```\n\n##### Retrieving text from the editor\n\nThe editor offers the function `get_text_as_string()` to retrieve the entire text\nas a String from the editor. Lines are separated by the new line character ```\\n```.\n\nThe editor offers the function `get_text_as_list()` to retrieve the entire text as a list from the editor.\nEach String-item in the list represents one line from the editor.\n\n##### Removing text from the editor\n\nThe editor offers the function `clear_text()` to clear the editor of any text.\n\n##### Inserting text into the editor\n\nInserting text can be done by using one of the two available functions:\n1. With a list of strings in which each string represents one line, or\n2. With a string which includes linebreak characters which get parsed.\n\n```\nset_text_from_list(["First line", "Second Line.", "Third Line."]\nset_text_from_string("First line.\\nSecond line.\\nThird Line")\n```\n\n## Customization\n\n#### Cursor mode\n\nCursor mode can either be `static` or `blinking` (=default).\n\n```python\nTX = TextEditor(...)\nTX.set_cursor_mode("static")\nTX.set_cursor_mode("blinking")\n```\n\n#### Key repetition speeds\n\nWhile a key is being held, multiple key events are being triggered.\nThe delay of the first repetition as well as the interval between all sequential key triggers can be\ncustomized by using the function `set_key_repetition(delay=300, intervall=30)`.\n\nFrom the [official documentation](http://www.pygame.org/docs/ref/key.html#pygame.key.set_repeat):\n> The delay parameter is the number of milliseconds before the first repeated pygame.KEYDOWN event will be sent.\n> After that, another pygame.KEYDOWN event will be sent every interval milliseconds.\n\n\n#### Font Customization\n\nThe editor uses a ttf file to set the font for the editor. By default, the Courier monospace font is used.\n\nA custom font can be loaded with the following method, passing an *absolute* path:\n- `set_font_from_ttf("X:\\path\\to\\custom\\font.ttf")`\n\nDISCLAIMER: As the width of a letter (space) is only calculated once after setting the font_size, any fonts that are not monospace will lead to the editor not working correctly anymore, as it cannot be determined correctly between which letters the user clicked.\n\n#### Font size\n\nFont size can be customized with the command `set_font_size(size)` - the parameter is an integer\nwith the default value `16` to be able to reset it.\n\n#### Line Numbers\nLine numbers can be shown on the left side of the editor. Line numbers begin with 0 as is the Pythonian way.\n\nLine numbers can be enabled and disabled with ```set_line_numbers(Boolean)```.\n\n\n#### Syntax Highlighting\n\nThe editor comes with syntax highlighting for Python code. Tokenization is based on the ```pygment``` package.\n\nSyntax highlighting can be enabled/disabled with ```set_syntax_coloring(boolean_value)```.\n\nThe syntax colors being used are also specified in the yml style file.\n\n\n#### Color-scheme customization\n\nThe editor uses a yml file to set the color-scheme for the editor itself and for the syntax coloring.\n\nTwo styles are delivered with the editor, they can be activated respectively by:\n- `set_colorscheme("dark")`\n- `set_colorscheme("bright")`\n\nA custom style can be loaded with the following method from a created yml file:\n- `set_colorscheme_from_yaml("X:\\path\\to\\custom\\filename.yml")`\n\nAll keys must be present with values. Acceptable values are\nRGB colors in the following format: ```(255, 255, 255)``` or ```255, 255, 255```.\n\nThe following keys are required in the ```stylename.yml``` file, syntax colors are only used if syntax\nhighlighting is enabled, but are still required to be included.\n\n**Editor colors** (source: bright.yml)\n\n- `codingBackgroundColor: (255, 255, 255)`\n- `codingScrollBarBackgroundColor: (49, 50, 50)`\n- `lineNumberColor: (255, 255, 255)`\n- `lineNumberBackgroundColor: (60, 61, 61)`\n- `textColor: (255, 255, 255)`\n\n** Syntax colors** (source: bright.yml)\n\n- `textColor_normal: (0, 255, 255)`\n- `textColor_comments: (119, 115, 115)`\n- `textColor_quotes: (227, 215, 115)`\n- `textColor_operators: (237, 36, 36)`\n- `textColor_keywords: (237, 36, 36)`\n- `textColor_function: (50, 150, 36)`\n- `textColor_builtin: (50, 50, 136)`\n',
+    'author': 'Victor Seifert',
+    'author_email': 'seifert.victor@web.de',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
+    'package_dir': package_dir,
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'python_requires': '>=3.8,<4.0',
+}
+
+
+setup(**setup_kwargs)
```

