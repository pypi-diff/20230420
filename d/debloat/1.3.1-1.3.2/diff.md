# Comparing `tmp/debloat-1.3.1.tar.gz` & `tmp/debloat-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debloat-1.3.1.tar", last modified: Sun Mar 26 21:51:43 2023, max compression
+gzip compressed data, was "debloat-1.3.2.tar", last modified: Wed Apr 19 22:52:33 2023, max compression
```

## Comparing `debloat-1.3.1.tar` & `debloat-1.3.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 21:51:43.522647 debloat-1.3.1/
--rw-rw-rw-   0        0        0     7101 2023-03-26 21:51:43.523147 debloat-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     6572 2023-03-26 21:44:28.000000 debloat-1.3.1/README.md
--rw-rw-rw-   0        0        0      788 2023-03-26 21:51:22.000000 debloat-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0      166 2023-03-26 21:51:43.524146 debloat-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-26 16:24:06.000000 debloat-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-26 21:51:43.500644 debloat-1.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-26 21:51:43.512147 debloat-1.3.1/src/debloat/
--rw-rw-rw-   0        0        0        0 2023-03-26 15:50:45.000000 debloat-1.3.1/src/debloat/__init__.py
--rw-rw-rw-   0        0        0     3547 2023-03-26 21:24:00.000000 debloat-1.3.1/src/debloat/gui.py
--rw-rw-rw-   0        0        0     1199 2023-03-26 21:13:00.000000 debloat-1.3.1/src/debloat/main.py
--rw-rw-rw-   0        0        0    12716 2023-03-26 21:27:01.000000 debloat-1.3.1/src/debloat/processor.py
-drwxrwxrwx   0        0        0        0 2023-03-26 21:51:43.521646 debloat-1.3.1/src/debloat.egg-info/
--rw-rw-rw-   0        0        0     7101 2023-03-26 21:51:43.000000 debloat-1.3.1/src/debloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-03-26 21:51:43.000000 debloat-1.3.1/src/debloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 21:51:43.000000 debloat-1.3.1/src/debloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-03-26 21:51:43.000000 debloat-1.3.1/src/debloat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-03-26 21:51:43.000000 debloat-1.3.1/src/debloat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-26 21:51:43.000000 debloat-1.3.1/src/debloat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 22:52:33.048739 debloat-1.3.2/
+-rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     7405 2023-04-19 22:52:33.049240 debloat-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6851 2023-04-19 22:52:19.000000 debloat-1.3.2/README.md
+-rw-rw-rw-   0        0        0      788 2023-04-19 22:43:38.000000 debloat-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0      166 2023-04-19 22:52:33.054239 debloat-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 22:52:33.016239 debloat-1.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 22:52:33.028738 debloat-1.3.2/src/debloat/
+-rw-rw-rw-   0        0        0        0 2023-04-19 22:39:21.000000 debloat-1.3.2/src/debloat/__init__.py
+-rw-rw-rw-   0        0        0      510 2023-03-27 10:51:40.000000 debloat-1.3.2/src/debloat/auxiliary.py
+-rw-rw-rw-   0        0        0     3817 2023-04-19 22:39:35.000000 debloat-1.3.2/src/debloat/gui.py
+-rw-rw-rw-   0        0        0     1556 2023-04-19 22:39:30.000000 debloat-1.3.2/src/debloat/main.py
+-rw-rw-rw-   0        0        0    19474 2023-04-16 12:04:38.000000 debloat-1.3.2/src/debloat/processor.py
+drwxrwxrwx   0        0        0        0 2023-04-19 22:52:33.047738 debloat-1.3.2/src/debloat.egg-info/
+-rw-rw-rw-   0        0        0     7405 2023-04-19 22:52:32.000000 debloat-1.3.2/src/debloat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-04-19 22:52:33.000000 debloat-1.3.2/src/debloat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 22:52:32.000000 debloat-1.3.2/src/debloat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-04-19 22:52:32.000000 debloat-1.3.2/src/debloat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-04-19 22:52:32.000000 debloat-1.3.2/src/debloat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 22:52:32.000000 debloat-1.3.2/src/debloat.egg-info/top_level.txt
```

### Comparing `debloat-1.3.1/PKG-INFO` & `debloat-1.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,78 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.3.1
+Version: 1.3.2
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ![debloat](https://user-images.githubusercontent.com/77356206/215351855-9f89c298-36b4-4234-89b5-dc3f26d1f8b0.png)
 
 # Debloat
 Debloat is a GUI and CLI tool to remove excess garbage from bloated executables.
 
 By excess garbage, I mean 300 - 800MB of junk bytes added to a binary to keep it from going into a sandbox.
 
 Being built with Python, the code and logic is easily accessible for others to take the concepts and apply them to their own tools. The program can be compiled for Windows, MacOS, Linux. The GUI removes any need for remembering commandline options and reading through CLI manuals: it is intended to be as simple as possible. The logic within the program handles the different use cases automatically.
 
 Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
 
-The CLI version can be installed using `pip install debloat`. 
+The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
 
 For advanced users, Debloat can also be imported into other scripts and the processing functions can be called individually.
 
 ## How to use the GUI?
 The GUI of Debloat intends to be as intuitive as possible.
 When launched, you can drag and drop bloated file onto the text bar and press the "Process file" button.
 Some technical information will be printed to the scrolling textbox and the file without bloat will be written to the directory the file was pulled from.
 Sound easy? It is!
 
-Running the program should debloat the binary in 30-40 second on average; as long as 120 seconds for more complicated obfuscation methods.
+Running the program should debloat the binary in 30-40 second on average.
 
 <img width="602" alt="Screenshot 2023-01-29 at 2 52 13 PM" src="https://user-images.githubusercontent.com/77356206/215352245-b37091ce-4d58-415c-a7ba-44a9c45bd6f1.png">
 
 ## How to use the CLI?
 After installing using `pip install debloat` use the command `debloat`.<br>
 `debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
 
 The gui can also be launched from the CLI using the command `debloat-gui`.
 
 ## Does it always work?
 Not yet.
-My unscientific guess is that it should work for every 5 of 6 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. In situations where it does not work, it may remove too much content from the binary and the binary will return malformed.
+My unscientific guess is that it should work for every 7 of 8 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
+In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "-unsafe" switch. If you ever need this switch, consider sharing the sample for additional analysis.
 
 ## Use Cases (Images from [Malcat](https://malcat.fr/))
 ### Full support
 - [x] Bloat appended to the end of a Signed PE.<br>
 In the image below, the bloat has been appended to the end of the executable. <br>
 ![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
 
-- [X] Signed executable packed with UPX.<br>
+- [X] Signed or Unsigned Packed executable.<br>
 In the image below, the bloat has been appended to the executable after packing. <br>
 ![Screenshot 2023-02-11 at 3 44 10 PM](https://user-images.githubusercontent.com/77356206/218280433-6dbcf51a-68c8-48e1-a89a-ad0b818a0afc.png)
 
 - [X] Signed executable includes bloat in the .rsrc section of the PE.<br>
 In the image below, the bloat is identified as in the .rsrc section and is removed from the PE.<br>
 ![Screenshot 2023-02-11 at 3 35 21 PM](https://user-images.githubusercontent.com/77356206/218280086-7cd548f8-e16b-4290-9283-a8a848de1419.png)
 
-### Partial Support
-- [ ] Some cases where bloat is added inside a PE Section.<br>
+- [X] Cases where bloat is added inside a PE Section.<br>
 In the image below, the bloat has been included in a PE section named [0]. <br>
 ![Screenshot 2023-02-11 at 3 26 52 PM](https://user-images.githubusercontent.com/77356206/218279753-ed2c9102-482a-4639-aeb1-df8efc9c4e2e.png)
 
-- [ ] Some packer detection
+# Partial Support
+
+- [X] Some packer detection for instances where the binary simply cannot be debloated. For example, NullSoft installers. These can be unpacked with UniExtract2 and do not need debloated.
 
 ### Other use cases
 There are use cases where the tool does not work. However, I plan to solve for them before publishing too much about them.
 
 ## Why?
 There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
 
@@ -81,18 +84,22 @@
 
 \* Note: If automation is desired, I recommend re-writing these concepts in C/C++ and not Python.
 
 ## How to build? 
 Follow the build commands appropriate to your platform. The main difference between build commands is the format of the icon.
 <br>
 MacOS<br>
-`pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns debloat.py`
+`pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
 
 Windows<br>
-`pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico debloat.py`
+`pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico gui.py`
 
 Linux<br> 
-`~/.local/bin/pyinstaller --onefile --noconsole --icon=debloat.ico --additional-hooks-dir=./hook --add-binary "/home/redacted/.local/lib/python3.10/site-packages/:." debloat.py`
+`~/.local/bin/pyinstaller --onefile --noconsole --icon=debloat.ico --additional-hooks-dir=./hook --add-binary "/home/redacted/.local/lib/python3.10/site-packages/:." gui.py`
 - I'm not sure why the same hook didn't work on Linux and pointing to the site-packages directory is not preferred. For some unknown reason, it would not find the binary if I pointed to the specific tkinterdnd2 or tkdnd directories.
 
 ## Where is this project going next?
-The current plan is to build in CLI functionality to handle batch jobs. At that stage, it will process all the files in a directory and output a report.
+Batch processing: process all files in a directory and produce a report.
+
+Better support for using processing methods outside of debloat.
+
+Support for debloating without unzipping.
```

### Comparing `debloat-1.3.1/README.md` & `debloat-1.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,58 +5,60 @@
 
 By excess garbage, I mean 300 - 800MB of junk bytes added to a binary to keep it from going into a sandbox.
 
 Being built with Python, the code and logic is easily accessible for others to take the concepts and apply them to their own tools. The program can be compiled for Windows, MacOS, Linux. The GUI removes any need for remembering commandline options and reading through CLI manuals: it is intended to be as simple as possible. The logic within the program handles the different use cases automatically.
 
 Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
 
-The CLI version can be installed using `pip install debloat`. 
+The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
 
 For advanced users, Debloat can also be imported into other scripts and the processing functions can be called individually.
 
 ## How to use the GUI?
 The GUI of Debloat intends to be as intuitive as possible.
 When launched, you can drag and drop bloated file onto the text bar and press the "Process file" button.
 Some technical information will be printed to the scrolling textbox and the file without bloat will be written to the directory the file was pulled from.
 Sound easy? It is!
 
-Running the program should debloat the binary in 30-40 second on average; as long as 120 seconds for more complicated obfuscation methods.
+Running the program should debloat the binary in 30-40 second on average.
 
 <img width="602" alt="Screenshot 2023-01-29 at 2 52 13 PM" src="https://user-images.githubusercontent.com/77356206/215352245-b37091ce-4d58-415c-a7ba-44a9c45bd6f1.png">
 
 ## How to use the CLI?
 After installing using `pip install debloat` use the command `debloat`.<br>
 `debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
 
 The gui can also be launched from the CLI using the command `debloat-gui`.
 
 ## Does it always work?
 Not yet.
-My unscientific guess is that it should work for every 5 of 6 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. In situations where it does not work, it may remove too much content from the binary and the binary will return malformed.
+My unscientific guess is that it should work for every 7 of 8 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
+In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "-unsafe" switch. If you ever need this switch, consider sharing the sample for additional analysis.
 
 ## Use Cases (Images from [Malcat](https://malcat.fr/))
 ### Full support
 - [x] Bloat appended to the end of a Signed PE.<br>
 In the image below, the bloat has been appended to the end of the executable. <br>
 ![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
 
-- [X] Signed executable packed with UPX.<br>
+- [X] Signed or Unsigned Packed executable.<br>
 In the image below, the bloat has been appended to the executable after packing. <br>
 ![Screenshot 2023-02-11 at 3 44 10 PM](https://user-images.githubusercontent.com/77356206/218280433-6dbcf51a-68c8-48e1-a89a-ad0b818a0afc.png)
 
 - [X] Signed executable includes bloat in the .rsrc section of the PE.<br>
 In the image below, the bloat is identified as in the .rsrc section and is removed from the PE.<br>
 ![Screenshot 2023-02-11 at 3 35 21 PM](https://user-images.githubusercontent.com/77356206/218280086-7cd548f8-e16b-4290-9283-a8a848de1419.png)
 
-### Partial Support
-- [ ] Some cases where bloat is added inside a PE Section.<br>
+- [X] Cases where bloat is added inside a PE Section.<br>
 In the image below, the bloat has been included in a PE section named [0]. <br>
 ![Screenshot 2023-02-11 at 3 26 52 PM](https://user-images.githubusercontent.com/77356206/218279753-ed2c9102-482a-4639-aeb1-df8efc9c4e2e.png)
 
-- [ ] Some packer detection
+# Partial Support
+
+- [X] Some packer detection for instances where the binary simply cannot be debloated. For example, NullSoft installers. These can be unpacked with UniExtract2 and do not need debloated.
 
 ### Other use cases
 There are use cases where the tool does not work. However, I plan to solve for them before publishing too much about them.
 
 ## Why?
 There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
 
@@ -68,18 +70,22 @@
 
 \* Note: If automation is desired, I recommend re-writing these concepts in C/C++ and not Python.
 
 ## How to build? 
 Follow the build commands appropriate to your platform. The main difference between build commands is the format of the icon.
 <br>
 MacOS<br>
-`pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns debloat.py`
+`pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
 
 Windows<br>
-`pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico debloat.py`
+`pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico gui.py`
 
 Linux<br> 
-`~/.local/bin/pyinstaller --onefile --noconsole --icon=debloat.ico --additional-hooks-dir=./hook --add-binary "/home/redacted/.local/lib/python3.10/site-packages/:." debloat.py`
+`~/.local/bin/pyinstaller --onefile --noconsole --icon=debloat.ico --additional-hooks-dir=./hook --add-binary "/home/redacted/.local/lib/python3.10/site-packages/:." gui.py`
 - I'm not sure why the same hook didn't work on Linux and pointing to the site-packages directory is not preferred. For some unknown reason, it would not find the binary if I pointed to the specific tkinterdnd2 or tkdnd directories.
 
 ## Where is this project going next?
-The current plan is to build in CLI functionality to handle batch jobs. At that stage, it will process all the files in a directory and output a report.
+Batch processing: process all files in a directory and produce a report.
+
+Better support for using processing methods outside of debloat.
+
+Support for debloating without unzipping.
```

### Comparing `debloat-1.3.1/pyproject.toml` & `debloat-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "debloat"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
   { name="Squiblydoo", email="Squiblydoo@pm.me" },
 ]
 description = "Debloat is an tool to remove excess garbage from bloated executables."
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
```

### Comparing `debloat-1.3.1/src/debloat/gui.py` & `debloat-1.3.2/src/debloat/gui.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """This file handles all GUI components."""
 
 import time
-import threading
 from pathlib import Path 
 from tkinter import *
 import tkinter.scrolledtext as st
 from typing import Tuple, Optional, Any
 from tkinterdnd2 import DND_FILES, TkinterDnD
 import pefile
-from debloat.processor import process_pe
+import debloat.processor
 
 
 class MainWindow(TkinterDnD.Tk):
     def __init__(self) -> None:
         '''Define main GUI window.'''
         TkinterDnD.Tk.__init__(self)
         self.title("Debloat")
@@ -21,65 +20,73 @@
         self.geometry("600x600")
 
         # Label and PathBox for the main function of program.
         self.pathbox_Label = Label(self, \
                                    text="Drag and drop file onto text bar.")
         self.pathbox_Label.pack()
         self.pathbox = Entry(self, width=150)
-        self.pathbox.pack(padx=20, pady=20)
+        self.pathbox.pack(padx=20)
         self.pathbox.drop_target_register(DND_FILES)
         self.pathbox.dnd_bind("<<Drop>>", self.process_entry)
 
         # Define button that will be used to the process file.
         self.process_button = Button(self, \
                                      text="Process file", \
                                      command=self.process)
         self.process_button.pack(pady=10)
 
+        # Safe processing value and checkbox: Maybe not even needed?
+        self.safe_processing = BooleanVar(value=True)
+        #self.safe_checkbox = Checkbutton(self,
+        #                                text="Only remove bloat when certain (safe)",
+        #                                 variable=self.safe_processing)
+        #self.safe_checkbox.pack()
+
         # Define Scrollbox for output of program.
-        self.output_scrollbox = st.ScrolledText(self, width=100, height=100)
+        self.output_scrollbox = st.ScrolledText(self, 
+                                                width=100, 
+                                                height=100,
+                                                wrap=WORD)
         self.output_scrollbox.pack(padx=20, pady=20)
 
     def clear_pathbox(self) -> None:
         '''Clear any text in the pathbox.'''
         self.pathbox.delete(0,"end")
 
-    def output_scrollbox_handler(self, message: str) -> None:
+    def output_scrollbox_handler(self, message: str, end = "\n", flush=True) -> None:
         '''Insert messages in the textbox.'''
-        output_thread = threading.Thread(self.output_scrollbox.insert(INSERT,\
-                                                                      message))
-        output_thread.start()
+        self.output_scrollbox.insert(INSERT, message + end)
+        self.update()
 
     def process_entry(self, event: Any) -> None:
         '''Check and update user provided file path.'''
         self.pathbox.insert("end", event.data)
         file_path = self.pathbox.get()
         if file_path[0] == '{' and file_path[-1] == '}':
             file_path = file_path[1:-1]
             self.pathbox.delete(0,"end")
             self.pathbox.insert(0, file_path) 
 
     def process(self) -> None:
         '''Process the file at the user provided path.'''
         start_time = time.time()
         file_path = Path(self.pathbox.get())
-        self.output_scrollbox_handler("Processing. Please wait.\n")
+        self.output_scrollbox_handler("Processing. Please wait.")
         try:
             pe = pefile.PE(file_path)
         except Exception:
-            self.output_scrollbox_handler("Provided file is not \
-                                        an executable! Please try again \
-                                        with an executable. Maybe it needs \
-                                        unzipped?\n")
+            self.output_scrollbox_handler('''
+Provided file is not an executable! Please try again 
+with an executable. Maybe it needs unzipped?''')
             self.clear_pathbox()
             return
         out_path = file_path.parent \
             / f"{file_path.stem}_patched{file_path.suffix}"
-        process_pe(pe, out_path=str(out_path), \
-                   log_message=lambda x: self.output_scrollbox_handler(x + "\n"))
+        process_pe(pe,  out_path, self.safe_processing, 
+                   log_message=self.output_scrollbox_handler)
         self.output_scrollbox_handler("-----Processessing took %s seconds ---\n" \
                                     % round((time.time() - start_time), 2))
         self.clear_pathbox()
 
 def main() -> None:
     root = MainWindow()
     root.mainloop()
```

### Comparing `debloat-1.3.1/src/debloat.egg-info/PKG-INFO` & `debloat-1.3.2/src/debloat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,78 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.3.1
+Version: 1.3.2
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ![debloat](https://user-images.githubusercontent.com/77356206/215351855-9f89c298-36b4-4234-89b5-dc3f26d1f8b0.png)
 
 # Debloat
 Debloat is a GUI and CLI tool to remove excess garbage from bloated executables.
 
 By excess garbage, I mean 300 - 800MB of junk bytes added to a binary to keep it from going into a sandbox.
 
 Being built with Python, the code and logic is easily accessible for others to take the concepts and apply them to their own tools. The program can be compiled for Windows, MacOS, Linux. The GUI removes any need for remembering commandline options and reading through CLI manuals: it is intended to be as simple as possible. The logic within the program handles the different use cases automatically.
 
 Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
 
-The CLI version can be installed using `pip install debloat`. 
+The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
 
 For advanced users, Debloat can also be imported into other scripts and the processing functions can be called individually.
 
 ## How to use the GUI?
 The GUI of Debloat intends to be as intuitive as possible.
 When launched, you can drag and drop bloated file onto the text bar and press the "Process file" button.
 Some technical information will be printed to the scrolling textbox and the file without bloat will be written to the directory the file was pulled from.
 Sound easy? It is!
 
-Running the program should debloat the binary in 30-40 second on average; as long as 120 seconds for more complicated obfuscation methods.
+Running the program should debloat the binary in 30-40 second on average.
 
 <img width="602" alt="Screenshot 2023-01-29 at 2 52 13 PM" src="https://user-images.githubusercontent.com/77356206/215352245-b37091ce-4d58-415c-a7ba-44a9c45bd6f1.png">
 
 ## How to use the CLI?
 After installing using `pip install debloat` use the command `debloat`.<br>
 `debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
 
 The gui can also be launched from the CLI using the command `debloat-gui`.
 
 ## Does it always work?
 Not yet.
-My unscientific guess is that it should work for every 5 of 6 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. In situations where it does not work, it may remove too much content from the binary and the binary will return malformed.
+My unscientific guess is that it should work for every 7 of 8 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
+In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "-unsafe" switch. If you ever need this switch, consider sharing the sample for additional analysis.
 
 ## Use Cases (Images from [Malcat](https://malcat.fr/))
 ### Full support
 - [x] Bloat appended to the end of a Signed PE.<br>
 In the image below, the bloat has been appended to the end of the executable. <br>
 ![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
 
-- [X] Signed executable packed with UPX.<br>
+- [X] Signed or Unsigned Packed executable.<br>
 In the image below, the bloat has been appended to the executable after packing. <br>
 ![Screenshot 2023-02-11 at 3 44 10 PM](https://user-images.githubusercontent.com/77356206/218280433-6dbcf51a-68c8-48e1-a89a-ad0b818a0afc.png)
 
 - [X] Signed executable includes bloat in the .rsrc section of the PE.<br>
 In the image below, the bloat is identified as in the .rsrc section and is removed from the PE.<br>
 ![Screenshot 2023-02-11 at 3 35 21 PM](https://user-images.githubusercontent.com/77356206/218280086-7cd548f8-e16b-4290-9283-a8a848de1419.png)
 
-### Partial Support
-- [ ] Some cases where bloat is added inside a PE Section.<br>
+- [X] Cases where bloat is added inside a PE Section.<br>
 In the image below, the bloat has been included in a PE section named [0]. <br>
 ![Screenshot 2023-02-11 at 3 26 52 PM](https://user-images.githubusercontent.com/77356206/218279753-ed2c9102-482a-4639-aeb1-df8efc9c4e2e.png)
 
-- [ ] Some packer detection
+# Partial Support
+
+- [X] Some packer detection for instances where the binary simply cannot be debloated. For example, NullSoft installers. These can be unpacked with UniExtract2 and do not need debloated.
 
 ### Other use cases
 There are use cases where the tool does not work. However, I plan to solve for them before publishing too much about them.
 
 ## Why?
 There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
 
@@ -81,18 +84,22 @@
 
 \* Note: If automation is desired, I recommend re-writing these concepts in C/C++ and not Python.
 
 ## How to build? 
 Follow the build commands appropriate to your platform. The main difference between build commands is the format of the icon.
 <br>
 MacOS<br>
-`pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns debloat.py`
+`pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
 
 Windows<br>
-`pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico debloat.py`
+`pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico gui.py`
 
 Linux<br> 
-`~/.local/bin/pyinstaller --onefile --noconsole --icon=debloat.ico --additional-hooks-dir=./hook --add-binary "/home/redacted/.local/lib/python3.10/site-packages/:." debloat.py`
+`~/.local/bin/pyinstaller --onefile --noconsole --icon=debloat.ico --additional-hooks-dir=./hook --add-binary "/home/redacted/.local/lib/python3.10/site-packages/:." gui.py`
 - I'm not sure why the same hook didn't work on Linux and pointing to the site-packages directory is not preferred. For some unknown reason, it would not find the binary if I pointed to the specific tkinterdnd2 or tkdnd directories.
 
 ## Where is this project going next?
-The current plan is to build in CLI functionality to handle batch jobs. At that stage, it will process all the files in a directory and output a report.
+Batch processing: process all files in a directory and produce a report.
+
+Better support for using processing methods outside of debloat.
+
+Support for debloating without unzipping.
```

