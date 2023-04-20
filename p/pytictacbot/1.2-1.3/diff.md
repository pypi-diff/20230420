# Comparing `tmp/pytictacbot-1.2.tar.gz` & `tmp/pytictacbot-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytictacbot-1.2.tar", last modified: Wed Apr 19 22:35:27 2023, max compression
+gzip compressed data, was "pytictacbot-1.3.tar", last modified: Thu Apr 20 07:55:55 2023, max compression
```

## Comparing `pytictacbot-1.2.tar` & `pytictacbot-1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 22:35:27.472997 pytictacbot-1.2/
--rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 pytictacbot-1.2/MANIFEST.in
--rw-r--r--   0 edgarcresson   (501) staff       (20)     2954 2023-04-19 22:35:27.472784 pytictacbot-1.2/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)     2801 2023-04-19 22:34:45.000000 pytictacbot-1.2/README.md
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 22:35:27.468362 pytictacbot-1.2/pytictacbot.egg-info/
--rw-r--r--   0 edgarcresson   (501) staff       (20)     2954 2023-04-19 22:35:27.000000 pytictacbot-1.2/pytictacbot.egg-info/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)      286 2023-04-19 22:35:27.000000 pytictacbot-1.2/pytictacbot.egg-info/SOURCES.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-19 22:35:27.000000 pytictacbot-1.2/pytictacbot.egg-info/dependency_links.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-19 22:35:27.000000 pytictacbot-1.2/pytictacbot.egg-info/entry_points.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-19 22:35:27.000000 pytictacbot-1.2/pytictacbot.egg-info/requires.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-19 22:35:27.000000 pytictacbot-1.2/pytictacbot.egg-info/top_level.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-19 22:35:27.473043 pytictacbot-1.2/setup.cfg
--rw-r--r--   0 edgarcresson   (501) staff       (20)      604 2023-04-19 22:35:22.000000 pytictacbot-1.2/setup.py
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 22:35:27.471985 pytictacbot-1.2/tictacbot/
--rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-14 12:45:16.000000 pytictacbot-1.2/tictacbot/gutenberg.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)     6363 2023-04-19 19:37:00.000000 pytictacbot-1.2/tictacbot/listen.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 07:55:55.382261 pytictacbot-1.3/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 pytictacbot-1.3/MANIFEST.in
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     2954 2023-04-20 07:55:55.382119 pytictacbot-1.3/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     2801 2023-04-19 22:34:45.000000 pytictacbot-1.3/README.md
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 07:55:55.378322 pytictacbot-1.3/pytictacbot.egg-info/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     2954 2023-04-20 07:55:55.000000 pytictacbot-1.3/pytictacbot.egg-info/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      286 2023-04-20 07:55:55.000000 pytictacbot-1.3/pytictacbot.egg-info/SOURCES.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-20 07:55:55.000000 pytictacbot-1.3/pytictacbot.egg-info/dependency_links.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-20 07:55:55.000000 pytictacbot-1.3/pytictacbot.egg-info/entry_points.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-20 07:55:55.000000 pytictacbot-1.3/pytictacbot.egg-info/requires.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-20 07:55:55.000000 pytictacbot-1.3/pytictacbot.egg-info/top_level.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-20 07:55:55.382298 pytictacbot-1.3/setup.cfg
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      604 2023-04-20 07:55:33.000000 pytictacbot-1.3/setup.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-20 07:55:55.381902 pytictacbot-1.3/tictacbot/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-14 12:45:16.000000 pytictacbot-1.3/tictacbot/gutenberg.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     6163 2023-04-20 07:55:26.000000 pytictacbot-1.3/tictacbot/listen.py
```

### Comparing `pytictacbot-1.2/PKG-INFO` & `pytictacbot-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytictacbot
-Version: 1.2
+Version: 1.3
 Summary: A program that makes you unbeatable at BombParty
 Description-Content-Type: text/markdown
 
 # Tictacbot
 
 A program that makes you unbeatable at [BombParty](https://jklm.fun/) (in french).
```

### Comparing `pytictacbot-1.2/README.md` & `pytictacbot-1.3/README.md`

 * *Files identical despite different names*

### Comparing `pytictacbot-1.2/pytictacbot.egg-info/PKG-INFO` & `pytictacbot-1.3/pytictacbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytictacbot
-Version: 1.2
+Version: 1.3
 Summary: A program that makes you unbeatable at BombParty
 Description-Content-Type: text/markdown
 
 # Tictacbot
 
 A program that makes you unbeatable at [BombParty](https://jklm.fun/) (in french).
```

### Comparing `pytictacbot-1.2/setup.py` & `pytictacbot-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pytictacbot",
-    version="1.2",
+    version="1.3",
     packages=["tictacbot"],
     include_package_data=True,
     description="A program that makes you unbeatable at BombParty",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "pynput",
```

### Comparing `pytictacbot-1.2/tictacbot/gutenberg.txt` & `pytictacbot-1.3/tictacbot/gutenberg.txt`

 * *Files identical despite different names*

### Comparing `pytictacbot-1.2/tictacbot/listen.py` & `pytictacbot-1.3/tictacbot/listen.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+import os
 from pynput import keyboard
 import pyperclip
 import pyautogui
 from art import text2art
 from colorama import init, Fore, Style
-import os
-
-this_file_path = os.path.dirname(os.path.abspath(__file__))
-gutenberg = os.path.join(this_file_path, "gutenberg.txt")
 
 init()
 
 keys_pressed = []
 remaining_letters = list("abcdefghijklmnopqrstuvwxyz")
 
 
 def retrieve_best_word(
     str_to_search: str, remaining_letters: list[str]
 ) -> dict["word":str, "score":int] | None:
     if str_to_search.isalpha():
         str_to_search = str_to_search.lower()
 
+        this_file_path = os.path.dirname(os.path.abspath(__file__))
+        gutenberg = os.path.join(this_file_path, "gutenberg.txt")
+
         best_word = {"word": None, "score": -1}
         with open(gutenberg, "r", encoding="utf-8") as f:
             for word in f:
                 if str_to_search in word:
                     score = len(set(word) & set(remaining_letters))
                     word_found = {"word": word.strip(), "score": score}
                     if best_word["score"] < word_found["score"]:
@@ -107,38 +107,37 @@
         # Colorization start (really annoying to read)
         word_found_label_colored = Fore.YELLOW + "Found: " + Style.RESET_ALL
 
         word_found_colored = ""
         remaining_letters_found = ""
 
         word_found = word_found.replace(str_to_search, str_to_search.upper())
+        underlined = "\033[4m"
+
         for letter in word_found:
             if letter.isupper():
-                underlined = "\033[4m"
-                if letter.lower() in remaining_letters:
-                    if letter.lower() not in remaining_letters_found:
-                        word_found_colored += (
-                            Fore.LIGHTBLUE_EX
-                            + underlined
-                            + letter.lower()
-                            + Style.RESET_ALL
-                        )
-                        remaining_letters_found += letter.lower()
-                    else:
-                        word_found_colored += (
-                            underlined + letter.lower() + Style.RESET_ALL
-                        )
-                else:
-                    word_found_colored += underlined + letter.lower() + Style.RESET_ALL
-            elif letter.lower() in remaining_letters:
-                if letter.lower() not in remaining_letters_found:
-                    word_found_colored += Fore.LIGHTBLUE_EX + letter + Style.RESET_ALL
+                if (
+                    letter.lower() in remaining_letters
+                    and letter.lower() not in remaining_letters_found
+                ):
+                    word_found_colored += (
+                        Fore.LIGHTBLUE_EX
+                        + underlined
+                        + letter.lower()
+                        + Style.RESET_ALL
+                    )
                     remaining_letters_found += letter.lower()
                 else:
-                    word_found_colored += letter
+                    word_found_colored += underlined + letter.lower() + Style.RESET_ALL
+            elif (
+                letter.lower() in remaining_letters
+                and letter.lower() not in remaining_letters_found
+            ):
+                word_found_colored += Fore.LIGHTBLUE_EX + letter + Style.RESET_ALL
+                remaining_letters_found += letter.lower()
             else:
                 word_found_colored += letter
 
         score_label_colored = Fore.YELLOW + "Score: " + Style.RESET_ALL
         if word_score > 0:
             score_colored = Fore.LIGHTBLUE_EX + str(word_score) + Style.RESET_ALL
         else:
```

