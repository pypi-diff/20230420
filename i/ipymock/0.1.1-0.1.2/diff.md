# Comparing `tmp/ipymock-0.1.1.tar.gz` & `tmp/ipymock-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-0.1.1.tar", last modified: Thu Apr 20 07:58:46 2023, max compression
+gzip compressed data, was "ipymock-0.1.2.tar", last modified: Thu Apr 20 13:46:23 2023, max compression
```

## Comparing `ipymock-0.1.1.tar` & `ipymock-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 07:58:46.713326 ipymock-0.1.1/
--rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.1.1/LICENSE
--rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.1.1/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-20 07:58:46.713080 ipymock-0.1.1/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     6783 2023-04-20 07:58:34.000000 ipymock-0.1.1/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 07:58:46.709849 ipymock-0.1.1/ipymock/
--rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-20 07:58:25.000000 ipymock-0.1.1/ipymock/__init__.py
--rw-r--r--   0 saintway   (501) staff       (20)     1196 2023-04-20 07:58:25.000000 ipymock-0.1.1/ipymock/_nbdev.py
--rw-r--r--   0 saintway   (501) staff       (20)     9545 2023-04-20 07:58:25.000000 ipymock-0.1.1/ipymock/mock.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 07:58:46.711583 ipymock-0.1.1/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 07:58:46.712470 ipymock-0.1.1/ipymock.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.1.1/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.1.1/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-20 07:58:46.000000 ipymock-0.1.1/ipymock.egg-info/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-20 07:58:46.000000 ipymock-0.1.1/ipymock.egg-info/SOURCES.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-20 07:58:46.000000 ipymock-0.1.1/ipymock.egg-info/dependency_links.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.1.1/ipymock.egg-info/not-zip-safe
--rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-20 07:58:46.000000 ipymock-0.1.1/ipymock.egg-info/requires.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-20 07:58:46.000000 ipymock-0.1.1/ipymock.egg-info/top_level.txt
--rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-20 07:58:44.000000 ipymock-0.1.1/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-20 07:58:46.713414 ipymock-0.1.1/setup.cfg
--rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.1.1/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 13:46:23.317186 ipymock-0.1.2/
+-rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.1.2/LICENSE
+-rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.1.2/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-20 13:46:23.316864 ipymock-0.1.2/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)     6837 2023-04-20 13:46:09.000000 ipymock-0.1.2/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 13:46:23.314069 ipymock-0.1.2/ipymock/
+-rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-20 13:44:18.000000 ipymock-0.1.2/ipymock/__init__.py
+-rw-r--r--   0 saintway   (501) staff       (20)     1196 2023-04-20 13:44:18.000000 ipymock-0.1.2/ipymock/_nbdev.py
+-rw-r--r--   0 saintway   (501) staff       (20)     9733 2023-04-20 13:44:18.000000 ipymock-0.1.2/ipymock/mock.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 13:46:23.315836 ipymock-0.1.2/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 13:46:23.316425 ipymock-0.1.2/ipymock.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.1.2/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.1.2/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-20 13:46:23.000000 ipymock-0.1.2/ipymock.egg-info/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-20 13:46:23.000000 ipymock-0.1.2/ipymock.egg-info/SOURCES.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-20 13:46:23.000000 ipymock-0.1.2/ipymock.egg-info/dependency_links.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.1.2/ipymock.egg-info/not-zip-safe
+-rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-20 13:46:23.000000 ipymock-0.1.2/ipymock.egg-info/requires.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-20 13:46:23.000000 ipymock-0.1.2/ipymock.egg-info/top_level.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-20 13:45:19.000000 ipymock-0.1.2/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-20 13:46:23.317342 ipymock-0.1.2/setup.cfg
+-rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.1.2/setup.py
```

### Comparing `ipymock-0.1.1/LICENSE` & `ipymock-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-0.1.1/PKG-INFO` & `ipymock-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.1.1
+Version: 0.1.2
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
@@ -28,15 +28,15 @@
 -  If you are using an older version of this template, see the instructions above on how to upgrade your template. 
 -  It is important for you to spell the name of your user and repo correctly in `settings.ini` or the website will not have the correct address from which to source assets like CSS for your site.  When in doubt, you can open your browser's developer console and see if there are any errors related to fetching assets for your website due to an incorrect URL generated by misspelled values from `settings.ini`.
 -  If you change the name of your repo, you have to make the appropriate changes in `settings.ini`
 -  After you make changes to `settings.ini`, run `nbdev_build_lib && nbdev_clean_nbs && nbdev_build_docs` to make sure all changes are propagated appropriately.
 
 ## Pytest the Python Testfiles
 
-```
+```python
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -44,24 +44,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```
+```python
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ## Pytest the Python Testcases within IPyNb Runtimes
 
-```
+```python
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -107,15 +107,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```
+```python
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -124,22 +124,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```
+```python
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```
+```python
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -184,34 +184,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to use the do-pytest?
 
-```
+```python
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```
+```python
 from ipymock import do
 ```
 
-```
+```python
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
```

### Comparing `ipymock-0.1.1/README.md` & `ipymock-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 -  If you are using an older version of this template, see the instructions above on how to upgrade your template. 
 -  It is important for you to spell the name of your user and repo correctly in `settings.ini` or the website will not have the correct address from which to source assets like CSS for your site.  When in doubt, you can open your browser's developer console and see if there are any errors related to fetching assets for your website due to an incorrect URL generated by misspelled values from `settings.ini`.
 -  If you change the name of your repo, you have to make the appropriate changes in `settings.ini`
 -  After you make changes to `settings.ini`, run `nbdev_build_lib && nbdev_clean_nbs && nbdev_build_docs` to make sure all changes are propagated appropriately.
 
 ## Pytest the Python Testfiles
 
-```
+```python
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -24,24 +24,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```
+```python
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ## Pytest the Python Testcases within IPyNb Runtimes
 
-```
+```python
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -87,15 +87,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```
+```python
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -104,22 +104,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```
+```python
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```
+```python
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -164,34 +164,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to use the do-pytest?
 
-```
+```python
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```
+```python
 from ipymock import do
 ```
 
-```
+```python
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
```

### Comparing `ipymock-0.1.1/ipymock/__init__.py` & `ipymock-0.1.2/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-0.1.1/ipymock/_nbdev.py` & `ipymock-0.1.2/ipymock/_nbdev.py`

 * *Files identical despite different names*

### Comparing `ipymock-0.1.1/ipymock/mock.py` & `ipymock-0.1.2/ipymock/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     response_text_channel = Queue()
     conversation_done_channel = Queue()
     parent_message_id = ''
     conversation_id = ''
     reload_conversations_channel = Queue()
 
 # Internal Cell
-import json, os, requests, uuid
+import json, os, requests, sys, uuid
 
 # Cell
 chat_gpt_base_url = 'http://127.0.0.1:8080'
 
 # open the JSON file and read the access_token
 with open(os.path.expanduser('~/.config/revChatGPT/config.json'), 'r') as f:
     access_token = json.load(f).get('access_token', None)
@@ -98,15 +98,19 @@
         if not line.startswith(b'data: '):
             continue
 
         if line.endswith(b'[DONE]'):
             common.conversation_done_channel.put(True)
             continue
 
-        make_conversation_response = json.loads(line.decode('utf-8')[len('data: '):])
+        try:
+            make_conversation_response = json.loads(line.decode('utf-8')[len('data: '):])
+        except json.decoder.JSONDecodeError as err:
+            sys.stderr.write(f'Error JSON Decoding: {line}\n')
+            continue
         if make_conversation_response is None:
             continue
         parts = make_conversation_response['message']['content']['parts']
         if len(parts) > 0:
             common.response_text_channel.put(parts[0])
             yield parts[0]
         if common.conversation_id == '':
@@ -183,17 +187,17 @@
     conversation_id = json.load(f).get('conversation_id', None)
 
 # Internal Cell
 try:
     common.conversation_id = conversation_id
     get_conversation(conversation_id)
 except requests.exceptions.ConnectionError as errc:
-    print('Error Connecting:', errc)
+    sys.stderr.write(f'Error Connecting: {errc}\n')
 except RecursionError as errr:
-    print('Error Recursion:', errr)
+    sys.stderr.write(f'Error Recursion: {errr}\n')
 
 # Cell
 class attrdict(dict):
     def __getattr__(self, attr):
         return self.get(attr)
 
 def attributize(obj):
```

### Comparing `ipymock-0.1.1/ipymock.egg-info/PKG-INFO` & `ipymock-0.1.2/ipymock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.1.1
+Version: 0.1.2
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
@@ -28,15 +28,15 @@
 -  If you are using an older version of this template, see the instructions above on how to upgrade your template. 
 -  It is important for you to spell the name of your user and repo correctly in `settings.ini` or the website will not have the correct address from which to source assets like CSS for your site.  When in doubt, you can open your browser's developer console and see if there are any errors related to fetching assets for your website due to an incorrect URL generated by misspelled values from `settings.ini`.
 -  If you change the name of your repo, you have to make the appropriate changes in `settings.ini`
 -  After you make changes to `settings.ini`, run `nbdev_build_lib && nbdev_clean_nbs && nbdev_build_docs` to make sure all changes are propagated appropriately.
 
 ## Pytest the Python Testfiles
 
-```
+```python
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -44,24 +44,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```
+```python
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ## Pytest the Python Testcases within IPyNb Runtimes
 
-```
+```python
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -107,15 +107,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```
+```python
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -124,22 +124,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```
+```python
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```
+```python
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -184,34 +184,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to use the do-pytest?
 
-```
+```python
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```
+```python
 from ipymock import do
 ```
 
-```
+```python
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
```

### Comparing `ipymock-0.1.1/settings.ini` & `ipymock-0.1.2/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 user = seii-saintway
 description = A pytest plugin that let you run pytest within Jupyter Notebook cells.
 keywords = pytest interactive jupyter
 author = andrew
 author_email = andrew.saintway@gmail.com
 copyright = Neuro Spirit, DAO.
 branch = main
-version = 0.1.1
+version = 0.1.2
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `ipymock-0.1.1/setup.py` & `ipymock-0.1.2/setup.py`

 * *Files identical despite different names*

