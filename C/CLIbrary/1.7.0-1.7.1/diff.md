# Comparing `tmp/clibrary-1.7.0.tar.gz` & `tmp/clibrary-1.7.1.tar.gz`

## Comparing `clibrary-1.7.0.tar` & `clibrary-1.7.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 clibrary-1.7.0/Makefile
--rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 clibrary-1.7.0/docs.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 clibrary-1.7.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clibrary-1.7.0/src/CLIbrary/__init__.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 clibrary-1.7.0/src/CLIbrary/__main__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 clibrary-1.7.0/src/CLIbrary/files.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 clibrary-1.7.0/src/CLIbrary/inputs.py
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 clibrary-1.7.0/src/CLIbrary/interface.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 clibrary-1.7.0/src/CLIbrary/outputs.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 clibrary-1.7.0/src/CLIbrary/settings.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 clibrary-1.7.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 clibrary-1.7.0/LICENSE
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 clibrary-1.7.0/README.md
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 clibrary-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 clibrary-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 clibrary-1.7.1/Makefile
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 clibrary-1.7.1/docs.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 clibrary-1.7.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 clibrary-1.7.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 clibrary-1.7.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clibrary-1.7.1/src/CLIbrary/__init__.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 clibrary-1.7.1/src/CLIbrary/__main__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 clibrary-1.7.1/src/CLIbrary/files.py
+-rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 clibrary-1.7.1/src/CLIbrary/inputs.py
+-rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 clibrary-1.7.1/src/CLIbrary/interface.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 clibrary-1.7.1/src/CLIbrary/outputs.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 clibrary-1.7.1/src/CLIbrary/settings.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 clibrary-1.7.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 clibrary-1.7.1/LICENSE
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 clibrary-1.7.1/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 clibrary-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 clibrary-1.7.1/PKG-INFO
```

### Comparing `clibrary-1.7.0/docs.md` & `clibrary-1.7.1/docs.md`

 * *Files 10% similar despite different names*

```diff
@@ -71,56 +71,64 @@
 
 verified by:
 
 	python3 -m CLIbrary
 	
 imported by:
 
-	import CLIbrary
+``` python
+import CLIbrary
+```
 
 and all the functions can be accessed by:
 
-	CLIbrary.FUNCTION_NAME()
+``` python
+CLIbrary.FUNCTION_NAME()
+```
 
 ## Interface
 
 [Go back to ToC](#table-of-contents)
 
 ### CLI
 
-	CLIbrary.cmdIn(commandHandler={}) -> dict
+``` python
+CLIbrary.cmdIn(commandHandler={}) -> dict
+```
 
 *cmdIn* stands for *Command Input* as this function allows the user to input command as in a CLI interface.
 
 The handler for this function makes use of the following parameters:
 * request, str: The prompt to the user.
 * added, str: A set of characters to be automatically added to the prompt. Default is ": ".
 * style, str[^1]: A particular colour style to be applied to the prompt.
 * verbose, bool.
 * allowedCommands, list: A list of all the allowed commands for the CLI interface.
 * helpPath, str: The path to the help JSON. This enables the *help* command.
 
 This function returns a dictionary with the following keys:
 * command, str: The command.
 * sdOpts, dict: A dictionary containing single-dash options as {"opts1": "value1", "opts2": "value2", ...}[^2].
-* ddOpts, list: A list containing double-dash options as [opts1, opts2, ...].
+* ddOpts, list: A list containing double-dash options as [opts1, opts2, ...][^2].
 
 Commands are always structured as:
 
 	command -sdOpt value --ddOpt
 
 with no more than a single word for the command itself.
 
 [^1]: Colorama styling works best for styling inside **CLIbrary**.
 
-[^2]: The options get returned without the dash.
+[^2]: The options get returned without the dashes.
 
 ### Help
 
-	CLIbrary.helpPrint(handler={}) -> None
+``` python
+CLIbrary.helpPrint(handler={}) -> None
+```
 
 *helpPrint* is a function that reads and print the help JSON whose path gets passed to *cmdIn*.
 This function cannot be called manually as its calls are embedded inside *cmdIn*.
 
 ### Help entries
 
 A help entry must be formatted this way:
@@ -167,39 +175,45 @@
 
 [Go back to ToC](#table-of-contents)
 
 **CLIbrary** provides two functions to handle files loading and dumping: *aLoad* and *aDump*. These functions make a great use of the Python module Pickle.
 
 ### Loading
 
-	CLIbrary.aLoad(fileHandler: dict)
+``` python
+CLIbrary.aLoad(fileHandler: dict)
+``` 
 
 *aLoad* stands for *Automatic Loading* as this function loads informations from files without user confirmation.
 
 The handler for this function makes use of the following parameters:
 * path, str: The path to the file.
 * ignoreMissing, bool: Whether to display an error on missing files.
 
 ### Dumping
 
-	CLIbrary.aDump(fileHandler: dict) -> None
+``` python
+CLIbrary.aDump(fileHandler: dict) -> None
+```
 
 *aDump* stands for *Automatic Dumping* as this function dumps informations to files without user confirmation.
 
 The handler for this function makes use of the following parameters:
 * path, str: The path to the file.
 * data: The data to be dumped.
 
 ## Inputs
 
 [Go back to ToC](#table-of-contents)
 
 ### Strings
 
-	CLIbrary.strIn(stringHandler={}) -> str
+``` python
+CLIbrary.strIn(stringHandler={}) -> str
+```
 
 *strIn* stands for *String Input* as this function's purpose is receiving string inputs.
 
 The handler for this function makes use of the following parameters:
 * Strings.
 	* request: The prompt to the user.
 	* added: A set of characters to be automatically added to the prompt.
@@ -215,15 +229,17 @@
 * Integers.
 	* fixedLength: The length of the accepted answer, if different from zero.
 
 The returned value isn't case sensitive.
 
 ### Numbers
 
-	CLIbrary.numIn(numberHandler={}) -> "int, float"
+``` python
+CLIbrary.numIn(numberHandler={}) -> "int, float"
+```
 
 *numIn* stands for *Number Input* as this function's purpose is receiving numeric inputs.
 
 The handler for this function makes use of the following parameters:
 * Strings.
 	* request: The prompt to the user.
 	* added: A set of characters to be automatically added to the prompt.
@@ -233,28 +249,32 @@
 * Bools.
 	* verbose.
 * Integers.
 	* round: The number of decimal to round to, if different from -1.
 
 ### Booleans
 
-	CLIbrary.boolIn(boolHandler={}) -> bool
+``` python
+CLIbrary.boolIn(boolHandler={}) -> bool
+```
 
 *boolIn* stands for *Boolean Input* as this function's purpose is receiving boolean inputs.
 
 The handler for this function makes use of the following parameters:
 * Strings.
 	* request: The prompt to the user.
 	* added: A set of characters to be automatically added to the prompt.
 * Bools.
 	* verbose.
 
 ### Dates
 
-	CLIbrary.dateIn(dateHandler={}) -> str
+``` python
+CLIbrary.dateIn(dateHandler={}) -> str
+```
 
 *dateIn* stands for *Date Input* as this function's purpose is receiving date[^4] inputs.
 
 The handler for this function makes use of the following parameters:
 * Strings.
 	* request: The prompt to the user.
 	* added: A set of characters to be automatically added to the prompt.
@@ -262,15 +282,17 @@
 	* placeholders: Enables the use of "x"s as placeholders for not fully known dates.
 	* verbose.
 
 [^4]: Dates have to be passed in respect to the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) standard. 
 
 ### List handling
 
-	CLIbrary.listCh(listHandler={})
+``` python
+CLIbrary.listCh(listHandler={})
+```
 
 *listCh* stands for *List Choice* as this function returns the choosen element from a list.
 
 The handler for this function makes use of the following parameters:
 * Strings.
 	* request: The prompt to the user.
 	* added: A set of characters to be automatically added to the prompt.
@@ -279,19 +301,21 @@
 
 ## Outputs
 
 [Go back to ToC](#table-of-contents)
 
 ### Output function
 
-	CLIbrary.output(outputHandler: dict) -> None
+``` python
+CLIbrary.output(outputHandler: dict) -> None
+```
 
 The handler for this function makes use of the following parameters:
 * Strings.
 	* string: The output string.
 	* type: The output type, to be choosen from:
 		* `"error"`,
 		* `"warning"`,
 		* `"verbose"`,
 		* `""`: A plain style, similar to that of `CLIbrary.style.setting_plainMode`.
 	* before: A string that gets printed before the output and is unaffected by the output styling.
-	* after: A string that gets printed after the output and is unaffected by the output styling.
+	* after: A string that gets printed after the output and is unaffected by the output styling.
```

### Comparing `clibrary-1.7.0/.github/workflows/python-publish.yml` & `clibrary-1.7.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `clibrary-1.7.0/src/CLIbrary/files.py` & `clibrary-1.7.1/src/CLIbrary/files.py`

 * *Files identical despite different names*

### Comparing `clibrary-1.7.0/src/CLIbrary/inputs.py` & `clibrary-1.7.1/src/CLIbrary/inputs.py`

 * *Files identical despite different names*

### Comparing `clibrary-1.7.0/src/CLIbrary/interface.py` & `clibrary-1.7.1/src/CLIbrary/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,14 @@
 			font = Fore.BLACK
 			back = Back.BLACK
 
 		else:
 			font = Fore.WHITE
 			back = Back.WHITE
 
-
 		if not style.setting_plainMode:
 			for key in helpJson:
 				helpString = ""
 
 				if key not in handler["allowedCommands"]:
 					helpString += Back.YELLOW + font + " UNAVAILABLE " + Style.RESET_ALL
```

### Comparing `clibrary-1.7.0/src/CLIbrary/outputs.py` & `clibrary-1.7.1/src/CLIbrary/outputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 	handler = {}
 
 	# Strings.
 	handler["string"] = "" # Output string.
 	handler["type"] = "" # Output type.
 	handler["before"] = "" # Prints this style-unaffected string before the main string.
-	handler["after"] = "" # Prints this style-unaffected string afteer the main string.
+	handler["after"] = "" # Prints this style-unaffected string after the main string.
 
 	handler.update(outputHandler)
 
 	# Checks types and values.
 	if not type(handler["type"]) == str:
 		handler["type"] = ""
 	if not type(handler["before"]) == str:
@@ -44,15 +44,15 @@
 	elif handler["type"] == "verbose":
 		outputStyle = verboseStyle
 
 	elif handler["type"] == "":
 		outputStyle = ""
 	
 	else:
-		output({"type": "warning", "string": "OUTPUT MISCONFIGURED. PLEASE REFER TO THE DOCUMENTATION.", "before": handler["before"], "after": handler["after"]})
+		output({"type": "warning", "string": "OUTPUT MISCONFIGURED. PLEASE REFER TO THE DOCUMENTATION.", "before": "\n", "after": "\n"})
 		outputStyle = ""
 
 	if style.setting_plainMode: # Checks plain mode.
 		if handler["type"] in ["error", "warning", "verbose"]:
 			outputStyle = "[" + handler["type"].upper() + "] "
 
 		else:
```

### Comparing `clibrary-1.7.0/LICENSE` & `clibrary-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clibrary-1.7.0/pyproject.toml` & `clibrary-1.7.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling", "colorama", "datetime"]
+requires = ["hatchling", "colorama", "datetime", "setuptools"]
 build-backend = "hatchling.build"
 
 [project]
 name = "CLIbrary"
-version = "1.7.0"
+version = "1.7.1"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "A standardized collection of CLI utilities written in Python to handle commands, I/O and files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

