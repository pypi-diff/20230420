# Comparing `tmp/pytictacbot-1.3.tar.gz` & `tmp/pytictacbot-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytictacbot-1.3.tar", last modified: Thu Apr 20 07:55:55 2023, max compression
+gzip compressed data, was "pytictacbot-1.4.tar", last modified: Thu Apr 20 09:46:22 2023, max compression
```

## Comparing `pytictacbot-1.3.tar` & `pytictacbot-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 07:55:55.382261 pytictacbot-1.3/
--rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 pytictacbot-1.3/MANIFEST.in
--rw-r--r--   0 edgarcresson   (501) staff       (20)     2954 2023-04-20 07:55:55.382119 pytictacbot-1.3/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)     2801 2023-04-19 22:34:45.000000 pytictacbot-1.3/README.md
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 07:55:55.378322 pytictacbot-1.3/pytictacbot.egg-info/
--rw-r--r--   0 edgarcresson   (501) staff       (20)     2954 2023-04-20 07:55:55.000000 pytictacbot-1.3/pytictacbot.egg-info/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)      286 2023-04-20 07:55:55.000000 pytictacbot-1.3/pytictacbot.egg-info/SOURCES.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-20 07:55:55.000000 pytictacbot-1.3/pytictacbot.egg-info/dependency_links.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-20 07:55:55.000000 pytictacbot-1.3/pytictacbot.egg-info/entry_points.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-20 07:55:55.000000 pytictacbot-1.3/pytictacbot.egg-info/requires.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-20 07:55:55.000000 pytictacbot-1.3/pytictacbot.egg-info/top_level.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-20 07:55:55.382298 pytictacbot-1.3/setup.cfg
--rw-r--r--   0 edgarcresson   (501) staff       (20)      604 2023-04-20 07:55:33.000000 pytictacbot-1.3/setup.py
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 07:55:55.381902 pytictacbot-1.3/tictacbot/
--rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-14 12:45:16.000000 pytictacbot-1.3/tictacbot/gutenberg.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)     6163 2023-04-20 07:55:26.000000 pytictacbot-1.3/tictacbot/listen.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 09:46:22.630764 pytictacbot-1.4/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 pytictacbot-1.4/MANIFEST.in
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     3116 2023-04-20 09:46:22.630622 pytictacbot-1.4/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     2963 2023-04-20 09:45:54.000000 pytictacbot-1.4/README.md
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 09:46:22.626617 pytictacbot-1.4/pytictacbot.egg-info/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     3116 2023-04-20 09:46:22.000000 pytictacbot-1.4/pytictacbot.egg-info/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      286 2023-04-20 09:46:22.000000 pytictacbot-1.4/pytictacbot.egg-info/SOURCES.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-20 09:46:22.000000 pytictacbot-1.4/pytictacbot.egg-info/dependency_links.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-20 09:46:22.000000 pytictacbot-1.4/pytictacbot.egg-info/entry_points.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-20 09:46:22.000000 pytictacbot-1.4/pytictacbot.egg-info/requires.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-20 09:46:22.000000 pytictacbot-1.4/pytictacbot.egg-info/top_level.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-20 09:46:22.630814 pytictacbot-1.4/setup.cfg
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      604 2023-04-20 09:46:00.000000 pytictacbot-1.4/setup.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 09:46:22.630276 pytictacbot-1.4/tictacbot/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-14 12:45:16.000000 pytictacbot-1.4/tictacbot/gutenberg.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     6477 2023-04-20 08:47:39.000000 pytictacbot-1.4/tictacbot/listen.py
```

### Comparing `pytictacbot-1.3/PKG-INFO` & `pytictacbot-1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: pytictacbot
-Version: 1.3
+Version: 1.4
 Summary: A program that makes you unbeatable at BombParty
 Description-Content-Type: text/markdown
 
 # Tictacbot
 
 A program that makes you unbeatable at [BombParty](https://jklm.fun/) (in french).
 
+![Demo](tictacbot-demo.gif)
+
 ## Installation
 
-⚠️ This program requires a version of **Python** >= 3 installed on your machine.
+⚠️ This program requires a version of [python](https://www.python.org/) >= 3 installed on your machine.
 
-Install the [pytictacbot](https://pypi.org/project/pytictacbot/) module using *pip*:
+Install the [pytictacbot](https://pypi.org/project/pytictacbot/) module using *pip* (it is included with python):
 ```zsh
 pip install pytictacbot
 ```
 
 ## Usage
 
 *Note: this program will only work on MacOS since it uses "Command + V" keys to paste. You can edit the code yourself if you want to adapt it to your environment.*
 
-In order for this program to work, you must allow "Accessibility" settings to the application that will run the script. Indeed, you need access to the input monitorig to listen to the keys you type.
+In order for this program to work, you must allow "Accessibility" settings to the application that will run the script. Indeed, you need access to the input monitoring to listen to the keys you type.
 
-- On your Mac, open *System settings*,
-- Open the *Privacy & Security* section,
-- Open the *Accessibility* section,
-- Allow the application in which you will run the script (ex: iTerm).
+On Mac:
+- Open *System settings*,
+- Navigate into the *Privacy & Security* section,
+- Click on *Accessibility*,
+- Allow the application(s) in which you will run the script (ex: iTerm, Visual Studio Code...),
+- Go back, then do the same thing for *Input Monitoring*.
 
 Once this is done, it is ready to use !
 
 In your terminal, run:
 ```zsh
 tictacbot
 ```
```

### Comparing `pytictacbot-1.3/README.md` & `pytictacbot-1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # Tictacbot
 
 A program that makes you unbeatable at [BombParty](https://jklm.fun/) (in french).
 
+![Demo](tictacbot-demo.gif)
+
 ## Installation
 
-⚠️ This program requires a version of **Python** >= 3 installed on your machine.
+⚠️ This program requires a version of [python](https://www.python.org/) >= 3 installed on your machine.
 
-Install the [pytictacbot](https://pypi.org/project/pytictacbot/) module using *pip*:
+Install the [pytictacbot](https://pypi.org/project/pytictacbot/) module using *pip* (it is included with python):
 ```zsh
 pip install pytictacbot
 ```
 
 ## Usage
 
 *Note: this program will only work on MacOS since it uses "Command + V" keys to paste. You can edit the code yourself if you want to adapt it to your environment.*
 
-In order for this program to work, you must allow "Accessibility" settings to the application that will run the script. Indeed, you need access to the input monitorig to listen to the keys you type.
+In order for this program to work, you must allow "Accessibility" settings to the application that will run the script. Indeed, you need access to the input monitoring to listen to the keys you type.
 
-- On your Mac, open *System settings*,
-- Open the *Privacy & Security* section,
-- Open the *Accessibility* section,
-- Allow the application in which you will run the script (ex: iTerm).
+On Mac:
+- Open *System settings*,
+- Navigate into the *Privacy & Security* section,
+- Click on *Accessibility*,
+- Allow the application(s) in which you will run the script (ex: iTerm, Visual Studio Code...),
+- Go back, then do the same thing for *Input Monitoring*.
 
 Once this is done, it is ready to use !
 
 In your terminal, run:
 ```zsh
 tictacbot
 ```
```

### Comparing `pytictacbot-1.3/pytictacbot.egg-info/PKG-INFO` & `pytictacbot-1.4/pytictacbot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: pytictacbot
-Version: 1.3
+Version: 1.4
 Summary: A program that makes you unbeatable at BombParty
 Description-Content-Type: text/markdown
 
 # Tictacbot
 
 A program that makes you unbeatable at [BombParty](https://jklm.fun/) (in french).
 
+![Demo](tictacbot-demo.gif)
+
 ## Installation
 
-⚠️ This program requires a version of **Python** >= 3 installed on your machine.
+⚠️ This program requires a version of [python](https://www.python.org/) >= 3 installed on your machine.
 
-Install the [pytictacbot](https://pypi.org/project/pytictacbot/) module using *pip*:
+Install the [pytictacbot](https://pypi.org/project/pytictacbot/) module using *pip* (it is included with python):
 ```zsh
 pip install pytictacbot
 ```
 
 ## Usage
 
 *Note: this program will only work on MacOS since it uses "Command + V" keys to paste. You can edit the code yourself if you want to adapt it to your environment.*
 
-In order for this program to work, you must allow "Accessibility" settings to the application that will run the script. Indeed, you need access to the input monitorig to listen to the keys you type.
+In order for this program to work, you must allow "Accessibility" settings to the application that will run the script. Indeed, you need access to the input monitoring to listen to the keys you type.
 
-- On your Mac, open *System settings*,
-- Open the *Privacy & Security* section,
-- Open the *Accessibility* section,
-- Allow the application in which you will run the script (ex: iTerm).
+On Mac:
+- Open *System settings*,
+- Navigate into the *Privacy & Security* section,
+- Click on *Accessibility*,
+- Allow the application(s) in which you will run the script (ex: iTerm, Visual Studio Code...),
+- Go back, then do the same thing for *Input Monitoring*.
 
 Once this is done, it is ready to use !
 
 In your terminal, run:
 ```zsh
 tictacbot
 ```
```

### Comparing `pytictacbot-1.3/setup.py` & `pytictacbot-1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pytictacbot",
-    version="1.3",
+    version="1.4",
     packages=["tictacbot"],
     include_package_data=True,
     description="A program that makes you unbeatable at BombParty",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "pynput",
```

### Comparing `pytictacbot-1.3/tictacbot/gutenberg.txt` & `pytictacbot-1.4/tictacbot/gutenberg.txt`

 * *Files identical despite different names*

### Comparing `pytictacbot-1.3/tictacbot/listen.py` & `pytictacbot-1.4/tictacbot/listen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import os
 from pynput import keyboard
 import pyperclip
 import pyautogui
 from art import text2art
 from colorama import init, Fore, Style
+import unicodedata
 
 init()
 
 keys_pressed = []
 remaining_letters = list("abcdefghijklmnopqrstuvwxyz")
 
+def remove_accent(word: str) -> str:
+    return unicodedata.normalize('NFD', word).encode('ascii', 'ignore').decode('utf-8')
 
 def retrieve_best_word(
     str_to_search: str, remaining_letters: list[str]
 ) -> dict["word":str, "score":int] | None:
     if str_to_search.isalpha():
         str_to_search = str_to_search.lower()
 
         this_file_path = os.path.dirname(os.path.abspath(__file__))
         gutenberg = os.path.join(this_file_path, "gutenberg.txt")
 
         best_word = {"word": None, "score": -1}
         with open(gutenberg, "r", encoding="utf-8") as f:
             for word in f:
-                if str_to_search in word:
-                    score = len(set(word) & set(remaining_letters))
+                if str_to_search in word: 
+                    score = len(set(remove_accent(word)) & set(remaining_letters))
                     word_found = {"word": word.strip(), "score": score}
                     if best_word["score"] < word_found["score"]:
                         best_word = word_found
             return best_word
 
 
 def print_new_section(init: bool):
@@ -69,15 +72,15 @@
 
     print(Style.RESET_ALL)
 
 
 def update_remaining_letters(word_found: str):
     global remaining_letters
     remaining_letters = [
-        letter for letter in remaining_letters if letter not in word_found
+        letter for letter in remaining_letters if letter not in remove_accent(word_found)
     ]
     if len(remaining_letters) == 0:
         print_success_message()
         remaining_letters = list("abcdefghijklmnopqrstuvwxyz")
 
 
 def paste_word(word: str):
@@ -110,34 +113,35 @@
         word_found_colored = ""
         remaining_letters_found = ""
 
         word_found = word_found.replace(str_to_search, str_to_search.upper())
         underlined = "\033[4m"
 
         for letter in word_found:
-            if letter.isupper():
+            letter_without_accent = remove_accent(letter)
+            if letter_without_accent.isupper():
                 if (
-                    letter.lower() in remaining_letters
-                    and letter.lower() not in remaining_letters_found
+                    letter_without_accent.lower() in remaining_letters
+                    and letter_without_accent.lower() not in remaining_letters_found
                 ):
                     word_found_colored += (
                         Fore.LIGHTBLUE_EX
                         + underlined
                         + letter.lower()
                         + Style.RESET_ALL
                     )
-                    remaining_letters_found += letter.lower()
+                    remaining_letters_found += letter_without_accent.lower()
                 else:
                     word_found_colored += underlined + letter.lower() + Style.RESET_ALL
             elif (
-                letter.lower() in remaining_letters
-                and letter.lower() not in remaining_letters_found
+                letter_without_accent in remaining_letters
+                and letter_without_accent not in remaining_letters_found
             ):
                 word_found_colored += Fore.LIGHTBLUE_EX + letter + Style.RESET_ALL
-                remaining_letters_found += letter.lower()
+                remaining_letters_found += letter_without_accent
             else:
                 word_found_colored += letter
 
         score_label_colored = Fore.YELLOW + "Score: " + Style.RESET_ALL
         if word_score > 0:
             score_colored = Fore.LIGHTBLUE_EX + str(word_score) + Style.RESET_ALL
         else:
```

