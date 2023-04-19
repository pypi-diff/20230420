# Comparing `tmp/carter-py-0.1.2.tar.gz` & `tmp/carter-py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carter-py-0.1.2.tar", last modified: Sat Apr 15 14:42:11 2023, max compression
+gzip compressed data, was "carter-py-0.1.3.tar", last modified: Wed Apr 19 23:07:44 2023, max compression
```

## Comparing `carter-py-0.1.2.tar` & `carter-py-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 14:42:11.606955 carter-py-0.1.2/
--rw-rw-rw-   0        0        0     6530 2023-04-15 14:42:11.606955 carter-py-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5862 2023-04-15 14:16:25.000000 carter-py-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 14:42:11.599948 carter-py-0.1.2/carter_py.egg-info/
--rw-rw-rw-   0        0        0     6530 2023-04-15 14:42:11.000000 carter-py-0.1.2/carter_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-04-15 14:42:11.000000 carter-py-0.1.2/carter_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 14:42:11.000000 carter-py-0.1.2/carter_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2023-04-15 14:42:11.000000 carter-py-0.1.2/carter_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 14:42:11.000000 carter-py-0.1.2/carter_py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 14:42:11.604952 carter-py-0.1.2/carterpy/
--rw-rw-rw-   0        0        0       67 2023-04-15 11:17:48.000000 carter-py-0.1.2/carterpy/__init__.py
--rw-rw-rw-   0        0        0     2789 2023-04-15 14:40:07.000000 carter-py-0.1.2/carterpy/async_carter.py
--rw-rw-rw-   0        0        0     2703 2023-04-15 14:34:54.000000 carter-py-0.1.2/carterpy/carter.py
--rw-rw-rw-   0        0        0     3069 2023-04-15 14:40:40.000000 carter-py-0.1.2/carterpy/classes.py
--rw-rw-rw-   0        0        0      455 2023-04-12 20:13:09.000000 carter-py-0.1.2/carterpy/utils.py
--rw-rw-rw-   0        0        0     1075 2023-04-12 19:53:47.000000 carter-py-0.1.2/license.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 14:42:11.606955 carter-py-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1034 2023-04-15 14:42:07.000000 carter-py-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 23:07:44.186867 carter-py-0.1.3/
+-rw-rw-rw-   0        0        0     7684 2023-04-19 23:07:44.185866 carter-py-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7015 2023-04-19 22:48:31.000000 carter-py-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 23:07:44.171853 carter-py-0.1.3/carter_py.egg-info/
+-rw-rw-rw-   0        0        0     7684 2023-04-19 23:07:43.000000 carter-py-0.1.3/carter_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-04-19 23:07:43.000000 carter-py-0.1.3/carter_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 23:07:43.000000 carter-py-0.1.3/carter_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2023-04-19 23:07:43.000000 carter-py-0.1.3/carter_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 23:07:43.000000 carter-py-0.1.3/carter_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 23:07:44.183864 carter-py-0.1.3/carterpy/
+-rw-rw-rw-   0        0        0       67 2023-04-15 11:17:48.000000 carter-py-0.1.3/carterpy/__init__.py
+-rw-rw-rw-   0        0        0     3195 2023-04-19 22:34:49.000000 carter-py-0.1.3/carterpy/async_carter.py
+-rw-rw-rw-   0        0        0     3109 2023-04-16 23:54:59.000000 carter-py-0.1.3/carterpy/carter.py
+-rw-rw-rw-   0        0        0     2767 2023-04-16 20:48:06.000000 carter-py-0.1.3/carterpy/classes.py
+-rw-rw-rw-   0        0        0      455 2023-04-12 20:13:09.000000 carter-py-0.1.3/carterpy/utils.py
+-rw-rw-rw-   0        0        0     1075 2023-04-12 19:53:47.000000 carter-py-0.1.3/license.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 23:07:44.186867 carter-py-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2023-04-19 22:14:49.000000 carter-py-0.1.3/setup.py
```

### Comparing `carter-py-0.1.2/PKG-INFO` & `carter-py-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: carter-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: A wrapper for the Carter API
-Home-page: https://github.com/LazyLyrics/carterpy
+Home-page: https://github.com/LazyLyrics/carter-py
 Author: LazyLyrics
 Author-email: lazylyrics@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 # carter-py: A Python Wrapper for the Carter API
 
+[GitHub](https://github.com/LazyLyrics/carter-py) | [PyPI](https://pypi.org/project/carter-py/) | [Change Log](https://github.com/LazyLyrics/carter-py/blob/main/CHANGELOG.md)
+
 `carter-py` is a Python package that provides a simple wrapper for the Carter API. It allows you to easily send text messages to the API and receive responses with minimal setup, and with the ability to add more complex functionality in upcoming releases.
 
 ## Installation
 
 ```bash
 pip install `carter-py`
 ```
@@ -32,15 +34,15 @@
 
 ## Usage
 
 To use `carter-py`, you will need to obtain an API key from the Carter website. Once you have your API key, you can use it to create a Carter object and start sending messages. Here's an example:
 
 ```python
 
-from `carter-py` import Carter
+from `carterpy` import Carter
 
 
 # Replace YOUR_API_KEY with your actual API key
 
 carter = Carter("YOUR_API_KEY")
 
 # Send a message to the API
@@ -73,24 +75,37 @@
 ```python
 # with carter object already created
 
 interaction = carter.personalise("Hello, world!")
 print(interaction.output_text)
 ```
 
+### Speak
+
+When using any of the methods above, the output audio will be returned by default. This currently introduces significant latency on the API end. If you don't want to receive the audio you have two options. You can set the `speak` parameter to `False` when creating the Carter object, or you can set it to `False` when calling the method. When calling a function `carter-py` will first check if the `speak` parameter is set on the Class. If it is not set, it will then check if the `speak` parameter is set on the method. The default on both is `True`.
+
+```python
+    carter = Carter('your-api-key', speak=False) # True by default
+
+    interaction = carter.say("Hello, world!", "player123") # No audio will be returned, because you have not overridden the default on the class
+
+    interaction = carter.say("Hello, world!", "player123", speak=True) # Audio will be returned, because you have overridden the default on the class
+```
+
 ### Interactions
 
 Each request to carter returns an instance of the Interaction class. This contains information about the interaction, including the input text, output text, and forced behaviours. It also contains the status code and message, and the time taken to receive the response. Both the `opener()` and `personalise()` methods return an Interaction object, with the redundant properties removed. Here's an example of the Interaction class:
 
 ```text
+# Represents a single interaction with the Carter API.
+
 class Interaction():
-    # Represents a single interaction with the Carter API.
     input_text (str): The input text that was sent to the API. # Not present in opener()
     output_text (str): The output text that was received from the API.
-    output_audio (str): The output audio url that was received from the API.
+    output_audio (str): The output audio url that was received from the API (only if speak is True)
     forced_behaviours (array): The forced behaviours that were applied by the API. # Not present in opener() or personalise()
     id (uuid.UUID): The unique identifier of the interaction.
     time_taken (int): The time taken to receive the response, in milliseconds.
     timestamp (string): The timestamp of the interaction in isoformat.
     ok (bool): Whether the response was successful or not.
     status_code (int): The status code of the response.
     status_message (str): The status message of the response.
```

### Comparing `carter-py-0.1.2/README.md` & `carter-py-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # carter-py: A Python Wrapper for the Carter API
 
+[GitHub](https://github.com/LazyLyrics/carter-py) | [PyPI](https://pypi.org/project/carter-py/) | [Change Log](https://github.com/LazyLyrics/carter-py/blob/main/CHANGELOG.md)
+
 `carter-py` is a Python package that provides a simple wrapper for the Carter API. It allows you to easily send text messages to the API and receive responses with minimal setup, and with the ability to add more complex functionality in upcoming releases.
 
 ## Installation
 
 ```bash
 pip install `carter-py`
 ```
@@ -14,15 +16,15 @@
 
 ## Usage
 
 To use `carter-py`, you will need to obtain an API key from the Carter website. Once you have your API key, you can use it to create a Carter object and start sending messages. Here's an example:
 
 ```python
 
-from `carter-py` import Carter
+from `carterpy` import Carter
 
 
 # Replace YOUR_API_KEY with your actual API key
 
 carter = Carter("YOUR_API_KEY")
 
 # Send a message to the API
@@ -55,24 +57,37 @@
 ```python
 # with carter object already created
 
 interaction = carter.personalise("Hello, world!")
 print(interaction.output_text)
 ```
 
+### Speak
+
+When using any of the methods above, the output audio will be returned by default. This currently introduces significant latency on the API end. If you don't want to receive the audio you have two options. You can set the `speak` parameter to `False` when creating the Carter object, or you can set it to `False` when calling the method. When calling a function `carter-py` will first check if the `speak` parameter is set on the Class. If it is not set, it will then check if the `speak` parameter is set on the method. The default on both is `True`.
+
+```python
+    carter = Carter('your-api-key', speak=False) # True by default
+
+    interaction = carter.say("Hello, world!", "player123") # No audio will be returned, because you have not overridden the default on the class
+
+    interaction = carter.say("Hello, world!", "player123", speak=True) # Audio will be returned, because you have overridden the default on the class
+```
+
 ### Interactions
 
 Each request to carter returns an instance of the Interaction class. This contains information about the interaction, including the input text, output text, and forced behaviours. It also contains the status code and message, and the time taken to receive the response. Both the `opener()` and `personalise()` methods return an Interaction object, with the redundant properties removed. Here's an example of the Interaction class:
 
 ```text
+# Represents a single interaction with the Carter API.
+
 class Interaction():
-    # Represents a single interaction with the Carter API.
     input_text (str): The input text that was sent to the API. # Not present in opener()
     output_text (str): The output text that was received from the API.
-    output_audio (str): The output audio url that was received from the API.
+    output_audio (str): The output audio url that was received from the API (only if speak is True)
     forced_behaviours (array): The forced behaviours that were applied by the API. # Not present in opener() or personalise()
     id (uuid.UUID): The unique identifier of the interaction.
     time_taken (int): The time taken to receive the response, in milliseconds.
     timestamp (string): The timestamp of the interaction in isoformat.
     ok (bool): Whether the response was successful or not.
     status_code (int): The status code of the response.
     status_message (str): The status message of the response.
```

### Comparing `carter-py-0.1.2/carter_py.egg-info/PKG-INFO` & `carter-py-0.1.3/carter_py.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: carter-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: A wrapper for the Carter API
-Home-page: https://github.com/LazyLyrics/carterpy
+Home-page: https://github.com/LazyLyrics/carter-py
 Author: LazyLyrics
 Author-email: lazylyrics@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 # carter-py: A Python Wrapper for the Carter API
 
+[GitHub](https://github.com/LazyLyrics/carter-py) | [PyPI](https://pypi.org/project/carter-py/) | [Change Log](https://github.com/LazyLyrics/carter-py/blob/main/CHANGELOG.md)
+
 `carter-py` is a Python package that provides a simple wrapper for the Carter API. It allows you to easily send text messages to the API and receive responses with minimal setup, and with the ability to add more complex functionality in upcoming releases.
 
 ## Installation
 
 ```bash
 pip install `carter-py`
 ```
@@ -32,15 +34,15 @@
 
 ## Usage
 
 To use `carter-py`, you will need to obtain an API key from the Carter website. Once you have your API key, you can use it to create a Carter object and start sending messages. Here's an example:
 
 ```python
 
-from `carter-py` import Carter
+from `carterpy` import Carter
 
 
 # Replace YOUR_API_KEY with your actual API key
 
 carter = Carter("YOUR_API_KEY")
 
 # Send a message to the API
@@ -73,24 +75,37 @@
 ```python
 # with carter object already created
 
 interaction = carter.personalise("Hello, world!")
 print(interaction.output_text)
 ```
 
+### Speak
+
+When using any of the methods above, the output audio will be returned by default. This currently introduces significant latency on the API end. If you don't want to receive the audio you have two options. You can set the `speak` parameter to `False` when creating the Carter object, or you can set it to `False` when calling the method. When calling a function `carter-py` will first check if the `speak` parameter is set on the Class. If it is not set, it will then check if the `speak` parameter is set on the method. The default on both is `True`.
+
+```python
+    carter = Carter('your-api-key', speak=False) # True by default
+
+    interaction = carter.say("Hello, world!", "player123") # No audio will be returned, because you have not overridden the default on the class
+
+    interaction = carter.say("Hello, world!", "player123", speak=True) # Audio will be returned, because you have overridden the default on the class
+```
+
 ### Interactions
 
 Each request to carter returns an instance of the Interaction class. This contains information about the interaction, including the input text, output text, and forced behaviours. It also contains the status code and message, and the time taken to receive the response. Both the `opener()` and `personalise()` methods return an Interaction object, with the redundant properties removed. Here's an example of the Interaction class:
 
 ```text
+# Represents a single interaction with the Carter API.
+
 class Interaction():
-    # Represents a single interaction with the Carter API.
     input_text (str): The input text that was sent to the API. # Not present in opener()
     output_text (str): The output text that was received from the API.
-    output_audio (str): The output audio url that was received from the API.
+    output_audio (str): The output audio url that was received from the API (only if speak is True)
     forced_behaviours (array): The forced behaviours that were applied by the API. # Not present in opener() or personalise()
     id (uuid.UUID): The unique identifier of the interaction.
     time_taken (int): The time taken to receive the response, in milliseconds.
     timestamp (string): The timestamp of the interaction in isoformat.
     ok (bool): Whether the response was successful or not.
     status_code (int): The status code of the response.
     status_message (str): The status message of the response.
```

### Comparing `carter-py-0.1.2/carterpy/carter.py` & `carter-py-0.1.3/carterpy/carter.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,65 +12,72 @@
         carter_data = response.json()
         return {"carter_data": carter_data, "status_code": response.status_code, "status_message": response.reason, "ok": response.ok, "url": response.url}
     except (requests.exceptions.RequestException, json.JSONDecodeError) as e:
         return None
 
 
 class Carter:
-    def __init__(self, api_key):
+    def __init__(self, api_key, speak=True):
         self.api_key = api_key
         self.history = []
+        self.speak_default = speak
 
-    def say(self, text, player_id):
+    def say(self, text, player_id, speak=None):
         text = convert_to_string("text", text)
         player_id = convert_to_string("player_id", player_id)
         start = time.perf_counter()
+        speak_now = speak if speak is not None else self.speak_default
         data = {
             "text": text,
             "playerId": player_id,
             "key": self.api_key,
+            "speak": speak_now
         }
 
         headersList = {
             "Accept": "*/*",
             "Content-Type": "application/json"
         }
 
-        response = carterRequest(URLS["say"], data, headers=headersList)
+        response_data = carterRequest(URLS["say"], data, headers=headersList)
         time_taken = int((time.perf_counter() - start) * 1000)
-        interaction = Interaction("say", data, response, time_taken)
+        interaction = Interaction("say", data, response_data, time_taken)
         if interaction.ok:
             self.history.insert(0, interaction)
         return interaction
 
-    def opener(self, player_id):
+    def opener(self, player_id, speak=None):
         player_id = convert_to_string("player_id", player_id)
         start = time.perf_counter()
+        speak_now = speak if speak is not None else self.speak_default
         data = {
             "playerId": player_id,
             "key": self.api_key,
+            "speak": speak_now
         }
         headersList = {
             "Accept": "*/*",
             "Content-Type": "application/json"
         }
         response = carterRequest(
             URLS["opener"], headers=headersList, data=data)
         time_taken = int((time.perf_counter() - start) * 1000)
         interaction = Interaction("opener", data, response, time_taken)
         if interaction.ok:
             self.history.insert(0, interaction)
         return interaction
 
-    def personalise(self, text):
+    def personalise(self, text, speak=None):
         text = convert_to_string("text", text)
         start = time.perf_counter()
+        speak_now = speak if speak is not None else self.speak_default
         data = {
             "text": text,
             "key": self.api_key,
+            "speak": speak_now
         }
         headersList = {
             "Accept": "*/*",
             "Content-Type": "application/json"
         }
         response = carterRequest(
             URLS["personalise"], headers=headersList, data=data)
```

### Comparing `carter-py-0.1.2/license.txt` & `carter-py-0.1.3/license.txt`

 * *Files identical despite different names*

### Comparing `carter-py-0.1.2/setup.py` & `carter-py-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="carter-py",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires = [
     "aiohttp==3.8.4",
     "aioresponses==0.7.4",
     "asynctest==0.13.0",
     "python-dotenv==1.0.0",
     "Requests==2.28.2",
@@ -14,15 +14,15 @@
     "setuptools==65.5.0"
     ],
     author="LazyLyrics",
     author_email="lazylyrics@icloud.com",
     description="A wrapper for the Carter API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    url="https://github.com/LazyLyrics/carterpy",
+    url="https://github.com/LazyLyrics/carter-py",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

