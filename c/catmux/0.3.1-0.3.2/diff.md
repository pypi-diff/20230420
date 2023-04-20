# Comparing `tmp/catmux-0.3.1.tar.gz` & `tmp/catmux-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catmux-0.3.1.tar", last modified: Sun Aug 28 13:28:13 2022, max compression
+gzip compressed data, was "catmux-0.3.2.tar", last modified: Thu Apr 20 12:02:47 2023, max compression
```

## Comparing `catmux-0.3.1.tar` & `catmux-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2022-08-28 13:28:13.684558 catmux-0.3.1/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     7026 2022-08-28 13:28:13.684558 catmux-0.3.1/PKG-INFO
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     5698 2022-04-29 13:11:28.000000 catmux-0.3.1/README.md
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2022-08-28 13:28:13.684558 catmux-0.3.1/catmux/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        0 2022-04-29 13:11:28.000000 catmux-0.3.1/catmux/__init__.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1477 2022-04-29 13:11:28.000000 catmux-0.3.1/catmux/prefix.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     8388 2022-08-28 13:27:00.000000 catmux-0.3.1/catmux/session.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     2172 2022-08-28 13:27:00.000000 catmux-0.3.1/catmux/split.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     2426 2022-08-28 13:27:00.000000 catmux-0.3.1/catmux/tmux_wrapper.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     3812 2022-08-28 13:27:00.000000 catmux-0.3.1/catmux/window.py
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2022-08-28 13:28:13.684558 catmux-0.3.1/catmux.egg-info/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     7026 2022-08-28 13:28:13.000000 catmux-0.3.1/catmux.egg-info/PKG-INFO
--rw-rw-r--   0 mauch     (1000) mauch     (1000)      373 2022-08-28 13:28:13.000000 catmux-0.3.1/catmux.egg-info/SOURCES.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        1 2022-08-28 13:28:13.000000 catmux-0.3.1/catmux.egg-info/dependency_links.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        7 2022-08-28 13:28:13.000000 catmux-0.3.1/catmux.egg-info/requires.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        7 2022-08-28 13:28:13.000000 catmux-0.3.1/catmux.egg-info/top_level.txt
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2022-08-28 13:28:13.684558 catmux-0.3.1/etc/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1984 2022-04-29 13:11:28.000000 catmux-0.3.1/etc/example_session.yaml
--rw-rw-r--   0 mauch     (1000) mauch     (1000)      810 2022-04-29 13:11:28.000000 catmux-0.3.1/etc/readme_tmux.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1489 2022-04-29 13:11:28.000000 catmux-0.3.1/etc/tmux_default.conf
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2022-08-28 13:28:13.684558 catmux-0.3.1/script/
--rwxrwxr-x   0 mauch     (1000) mauch     (1000)     4673 2022-08-28 13:27:00.000000 catmux-0.3.1/script/catmux_create_session
--rw-rw-r--   0 mauch     (1000) mauch     (1000)       38 2022-08-28 13:28:13.684558 catmux-0.3.1/setup.cfg
--rw-rw-r--   0 mauch     (1000) mauch     (1000)      964 2022-08-28 13:27:12.000000 catmux-0.3.1/setup.py
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-04-20 12:02:47.075002 catmux-0.3.2/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1068 2023-04-04 19:35:47.000000 catmux-0.3.2/LICENSE
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     6129 2023-04-20 12:02:47.075002 catmux-0.3.2/PKG-INFO
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     5698 2023-04-04 19:35:47.000000 catmux-0.3.2/README.md
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-04-20 12:02:47.075002 catmux-0.3.2/catmux/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)        0 2023-04-04 19:35:47.000000 catmux-0.3.2/catmux/__init__.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1477 2023-04-04 19:35:47.000000 catmux-0.3.2/catmux/prefix.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     8388 2023-04-04 19:35:47.000000 catmux-0.3.2/catmux/session.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     2172 2023-04-04 19:35:47.000000 catmux-0.3.2/catmux/split.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     2426 2023-04-04 19:35:47.000000 catmux-0.3.2/catmux/tmux_wrapper.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     3812 2023-04-04 19:35:47.000000 catmux-0.3.2/catmux/window.py
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-04-20 12:02:47.075002 catmux-0.3.2/catmux.egg-info/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     6129 2023-04-20 12:02:47.000000 catmux-0.3.2/catmux.egg-info/PKG-INFO
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)      381 2023-04-20 12:02:47.000000 catmux-0.3.2/catmux.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)        1 2023-04-20 12:02:47.000000 catmux-0.3.2/catmux.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)        7 2023-04-20 12:02:47.000000 catmux-0.3.2/catmux.egg-info/requires.txt
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)        7 2023-04-20 12:02:47.000000 catmux-0.3.2/catmux.egg-info/top_level.txt
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-04-20 12:02:47.075002 catmux-0.3.2/etc/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1984 2023-04-04 19:35:47.000000 catmux-0.3.2/etc/example_session.yaml
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)      810 2023-04-04 19:35:47.000000 catmux-0.3.2/etc/readme_tmux.txt
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1593 2023-04-04 19:35:47.000000 catmux-0.3.2/etc/tmux_default.conf
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-04-20 12:02:47.075002 catmux-0.3.2/script/
+-rwxrwxr-x   0 mauch     (1000) mauch     (1000)     4646 2023-04-04 19:35:47.000000 catmux-0.3.2/script/catmux_create_session
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)       38 2023-04-20 12:02:47.075002 catmux-0.3.2/setup.cfg
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)      964 2023-04-20 12:00:07.000000 catmux-0.3.2/setup.py
```

### Comparing `catmux-0.3.1/PKG-INFO` & `catmux-0.3.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,111 @@
-Metadata-Version: 2.1
-Name: catmux
-Version: 0.3.1
-Summary: A tmux orchestration package.
-Home-page: https://github.com/fmauch/catmux
-Author: Felix Exner
-Author-email: felix_mauch@web.de
-License: MIT
-Description: # Catmux
-        
-        ## About
-        Catmux is a little helper to run a tmux session with multiple windows and panes with just one
-        command. It is inspired and functionally very similar to
-        [tmuxinator](https://github.com/tmuxinator/tmuxinator), but without the project management feature
-        which is in my opinion kind of an overhead.
-        
-        Session configs can be stored anywhere and have to be given as an argument.
-        
-        ## Motivation
-        In most of our ROS projects at work we use shell output for almost all nodes to get log information
-        during runtime. Having all this in one window where you start your "Start it all"-launchfile makes
-        it very hard to follow the log of a specific node. Starting everything in separate windows is quite
-        a lot of work and requires documentation overhead in sense of documenting which launchfiles or nodes
-        have to be started.
-        
-        At a conference I caught the idea to use tmux scripting to orchestrate all this in one tmux session.
-        However, quickly I noticed that creating these scripts is a daunting task as you'll have to type in
-        a lot of commands over and over again and as soon as you wanted to do things a little different such
-        as not starting a particular launchfile if a certain parameter was set, things got complicated.
-        
-        I liked the yaml-syntax of [tmuxinator](https://github.com/tmuxinator/tmuxinator), but that tool
-        didn't quite hit the spot. I wanted to have something that can be easily integrated into a ROS
-        project and I definitely wanted something that saves the config per project and not all configs at
-        one central spot on a particular machine.
-        
-        ## Installation
-        Catmux is a pure python package and the installation via `pip3 install --user catmux` is recommended.
-        
-        You can also install it by cloning this repository and calling `pip3 install --user .` in the
-        repository's root directory. If you use this option, please be aware that some examples behave
-        differently if you have installed catmux this way and are calling it from the repository directory.
-        Calling them from outside the directory (e.g. after leaving via `cd`) is fine and should result in
-        the same behavior as with the recommended installation method.
-        
-        ## Usage
-        Currently, there is no full-blown documentation, but the example config file in
-        `etc/example_session.yaml` gives a detailed insight on possible commands.
-        
-        ### Running the example the most simple way
-        After installation, you can run a simple example by calling the following command:
-        ```
-        catmux_create_session $(python3 -m catmux.prefix)/share/catmux/example_session.yaml
-        ```
-        
-        To see further options, simply run it with argument `-h`:
-        ```
-        $ catmux_create_session -h
-        usage: catmux_create_session [-h] [-n SESSION_NAME] [-t TMUX_CONFIG] [-d] [--overwrite OVERWRITE]
-                                     session_config
-        
-        Create a new catmux session
-        
-        positional arguments:
-          session_config        Session configuration. Should be a yaml-file.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -n SESSION_NAME, --session_name SESSION_NAME
-                                Name used for the tmux session
-          -t TMUX_CONFIG, --tmux_config TMUX_CONFIG
-                                This config will be used for the tmux session
-          -d, --detach          Start session in detached mode
-          --overwrite OVERWRITE
-                                Overwrite a parameter from the session config. Parameters can be specified
-                                using a comma-separated list such as '--overwrite param_a=1,param_b=2'.
-        ```
-        
-        ### Full blown example
-        To make use of all catmux features, run the following example command:
-        ```
-        catmux_create_session $(python3 -m catmux.prefix)/share/catmux/example_session.yaml \
-          --tmux_config $(python3 -m catmux.prefix)/share/catmux/tmux_default.conf \
-          --session_name example_session \
-          --overwrite show_layouts=True,replacement_param="new catmux user"
-        ```
-        
-        ### Killing a catmux session
-        If you are not that familiar with tmux: To kill a session, simply type `tmux kill-session` in any
-        terminal window. In the `etc/tmux_default.conf` there is a key-binding for that, see
-        `etc/readme_tmux.txt` for details.
-        
-        ### Tmux server to be used
-        By default, catmux spawns its own tmux server called `catmux`. Therefore, a simple
-        `tmux list-sessions` (or `tmux ls`) will not list the `catmux` session. To list the `catmux`
-        session, use `tmux -L catmux list-sessions`. You can change the server's name by specifying the
-        `-L <server_name>` parameter to `catmux_create_session`. That mechanism ensures that the environment
-        in which `catmux_create_session` is started, will be used inside the catmux session (as long as no
-        other session previously exists on that particular tmux server).
-        
-        ## Migrating from the catkin version of catmux
-        With the spread of ROS2, the need for a catkin-independent catmux has emerged.
-        Catmux is now a plain python package without the ROS integration.
-        Therefore, it is installed via pip and no longer needs to be part of a catkin workspace.
-        This opens the possibility to easily use catmux outside of robotics application, e.g. for server
-        administration or other development tasks.
-        
-        Catmux no longer has the `package://<your_package_name>` lookup capabilities.
-        To achieve the same outcome, simply use rospack:
-        ```
-        catmux_create_session $(rospack find <your_package_name>)/path/to/<your_catmux_session_config.yaml>
-        ```
-        
-        For ROS2, the same is achievable with `ros2 pkg prefix` but the yaml has to be installed (similar
-        to, for example, a launch file) and the installation path has to be specified:
-        ```
-        catmux_create_session $(ros2 pkg prefix <your_package_name>)/path/to/the/installed/<your_catmux_session_config.yaml>
-        
-        # for example: $ catmux_create_session $(ros2 pkg prefix catmux_test_pkg)/share/catmux_test_pkg/catmux_session.yaml
-        ```
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# Catmux
+
+## About
+Catmux is a little helper to run a tmux session with multiple windows and panes with just one
+command. It is inspired and functionally very similar to
+[tmuxinator](https://github.com/tmuxinator/tmuxinator), but without the project management feature
+which is in my opinion kind of an overhead.
+
+Session configs can be stored anywhere and have to be given as an argument.
+
+## Motivation
+In most of our ROS projects at work we use shell output for almost all nodes to get log information
+during runtime. Having all this in one window where you start your "Start it all"-launchfile makes
+it very hard to follow the log of a specific node. Starting everything in separate windows is quite
+a lot of work and requires documentation overhead in sense of documenting which launchfiles or nodes
+have to be started.
+
+At a conference I caught the idea to use tmux scripting to orchestrate all this in one tmux session.
+However, quickly I noticed that creating these scripts is a daunting task as you'll have to type in
+a lot of commands over and over again and as soon as you wanted to do things a little different such
+as not starting a particular launchfile if a certain parameter was set, things got complicated.
+
+I liked the yaml-syntax of [tmuxinator](https://github.com/tmuxinator/tmuxinator), but that tool
+didn't quite hit the spot. I wanted to have something that can be easily integrated into a ROS
+project and I definitely wanted something that saves the config per project and not all configs at
+one central spot on a particular machine.
+
+## Installation
+Catmux is a pure python package and the installation via `pip3 install --user catmux` is recommended.
+
+You can also install it by cloning this repository and calling `pip3 install --user .` in the
+repository's root directory. If you use this option, please be aware that some examples behave
+differently if you have installed catmux this way and are calling it from the repository directory.
+Calling them from outside the directory (e.g. after leaving via `cd`) is fine and should result in
+the same behavior as with the recommended installation method.
+
+## Usage
+Currently, there is no full-blown documentation, but the example config file in
+`etc/example_session.yaml` gives a detailed insight on possible commands.
+
+### Running the example the most simple way
+After installation, you can run a simple example by calling the following command:
+```
+catmux_create_session $(python3 -m catmux.prefix)/share/catmux/example_session.yaml
+```
+
+To see further options, simply run it with argument `-h`:
+```
+$ catmux_create_session -h
+usage: catmux_create_session [-h] [-n SESSION_NAME] [-t TMUX_CONFIG] [-d] [--overwrite OVERWRITE]
+                             session_config
+
+Create a new catmux session
+
+positional arguments:
+  session_config        Session configuration. Should be a yaml-file.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -n SESSION_NAME, --session_name SESSION_NAME
+                        Name used for the tmux session
+  -t TMUX_CONFIG, --tmux_config TMUX_CONFIG
+                        This config will be used for the tmux session
+  -d, --detach          Start session in detached mode
+  --overwrite OVERWRITE
+                        Overwrite a parameter from the session config. Parameters can be specified
+                        using a comma-separated list such as '--overwrite param_a=1,param_b=2'.
+```
+
+### Full blown example
+To make use of all catmux features, run the following example command:
+```
+catmux_create_session $(python3 -m catmux.prefix)/share/catmux/example_session.yaml \
+  --tmux_config $(python3 -m catmux.prefix)/share/catmux/tmux_default.conf \
+  --session_name example_session \
+  --overwrite show_layouts=True,replacement_param="new catmux user"
+```
+
+### Killing a catmux session
+If you are not that familiar with tmux: To kill a session, simply type `tmux kill-session` in any
+terminal window. In the `etc/tmux_default.conf` there is a key-binding for that, see
+`etc/readme_tmux.txt` for details.
+
+### Tmux server to be used
+By default, catmux spawns its own tmux server called `catmux`. Therefore, a simple
+`tmux list-sessions` (or `tmux ls`) will not list the `catmux` session. To list the `catmux`
+session, use `tmux -L catmux list-sessions`. You can change the server's name by specifying the
+`-L <server_name>` parameter to `catmux_create_session`. That mechanism ensures that the environment
+in which `catmux_create_session` is started, will be used inside the catmux session (as long as no
+other session previously exists on that particular tmux server).
+
+## Migrating from the catkin version of catmux
+With the spread of ROS2, the need for a catkin-independent catmux has emerged.
+Catmux is now a plain python package without the ROS integration.
+Therefore, it is installed via pip and no longer needs to be part of a catkin workspace.
+This opens the possibility to easily use catmux outside of robotics application, e.g. for server
+administration or other development tasks.
+
+Catmux no longer has the `package://<your_package_name>` lookup capabilities.
+To achieve the same outcome, simply use rospack:
+```
+catmux_create_session $(rospack find <your_package_name>)/path/to/<your_catmux_session_config.yaml>
+```
+
+For ROS2, the same is achievable with `ros2 pkg prefix` but the yaml has to be installed (similar
+to, for example, a launch file) and the installation path has to be specified:
+```
+catmux_create_session $(ros2 pkg prefix <your_package_name>)/path/to/the/installed/<your_catmux_session_config.yaml>
+
+# for example: $ catmux_create_session $(ros2 pkg prefix catmux_test_pkg)/share/catmux_test_pkg/catmux_session.yaml
+```
```

### Comparing `catmux-0.3.1/README.md` & `catmux-0.3.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: catmux
+Version: 0.3.2
+Summary: A tmux orchestration package.
+Home-page: https://github.com/fmauch/catmux
+Author: Felix Exner
+Author-email: felix_mauch@web.de
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Catmux
 
 ## About
 Catmux is a little helper to run a tmux session with multiple windows and panes with just one
 command. It is inspired and functionally very similar to
 [tmuxinator](https://github.com/tmuxinator/tmuxinator), but without the project management feature
 which is in my opinion kind of an overhead.
```

### Comparing `catmux-0.3.1/catmux/prefix.py` & `catmux-0.3.2/catmux/prefix.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.1/catmux/session.py` & `catmux-0.3.2/catmux/session.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.1/catmux/split.py` & `catmux-0.3.2/catmux/split.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.1/catmux/tmux_wrapper.py` & `catmux-0.3.2/catmux/tmux_wrapper.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.1/catmux/window.py` & `catmux-0.3.2/catmux/window.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.1/catmux.egg-info/PKG-INFO` & `catmux-0.3.2/catmux.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,126 +1,126 @@
 Metadata-Version: 2.1
 Name: catmux
-Version: 0.3.1
+Version: 0.3.2
 Summary: A tmux orchestration package.
 Home-page: https://github.com/fmauch/catmux
 Author: Felix Exner
 Author-email: felix_mauch@web.de
 License: MIT
-Description: # Catmux
-        
-        ## About
-        Catmux is a little helper to run a tmux session with multiple windows and panes with just one
-        command. It is inspired and functionally very similar to
-        [tmuxinator](https://github.com/tmuxinator/tmuxinator), but without the project management feature
-        which is in my opinion kind of an overhead.
-        
-        Session configs can be stored anywhere and have to be given as an argument.
-        
-        ## Motivation
-        In most of our ROS projects at work we use shell output for almost all nodes to get log information
-        during runtime. Having all this in one window where you start your "Start it all"-launchfile makes
-        it very hard to follow the log of a specific node. Starting everything in separate windows is quite
-        a lot of work and requires documentation overhead in sense of documenting which launchfiles or nodes
-        have to be started.
-        
-        At a conference I caught the idea to use tmux scripting to orchestrate all this in one tmux session.
-        However, quickly I noticed that creating these scripts is a daunting task as you'll have to type in
-        a lot of commands over and over again and as soon as you wanted to do things a little different such
-        as not starting a particular launchfile if a certain parameter was set, things got complicated.
-        
-        I liked the yaml-syntax of [tmuxinator](https://github.com/tmuxinator/tmuxinator), but that tool
-        didn't quite hit the spot. I wanted to have something that can be easily integrated into a ROS
-        project and I definitely wanted something that saves the config per project and not all configs at
-        one central spot on a particular machine.
-        
-        ## Installation
-        Catmux is a pure python package and the installation via `pip3 install --user catmux` is recommended.
-        
-        You can also install it by cloning this repository and calling `pip3 install --user .` in the
-        repository's root directory. If you use this option, please be aware that some examples behave
-        differently if you have installed catmux this way and are calling it from the repository directory.
-        Calling them from outside the directory (e.g. after leaving via `cd`) is fine and should result in
-        the same behavior as with the recommended installation method.
-        
-        ## Usage
-        Currently, there is no full-blown documentation, but the example config file in
-        `etc/example_session.yaml` gives a detailed insight on possible commands.
-        
-        ### Running the example the most simple way
-        After installation, you can run a simple example by calling the following command:
-        ```
-        catmux_create_session $(python3 -m catmux.prefix)/share/catmux/example_session.yaml
-        ```
-        
-        To see further options, simply run it with argument `-h`:
-        ```
-        $ catmux_create_session -h
-        usage: catmux_create_session [-h] [-n SESSION_NAME] [-t TMUX_CONFIG] [-d] [--overwrite OVERWRITE]
-                                     session_config
-        
-        Create a new catmux session
-        
-        positional arguments:
-          session_config        Session configuration. Should be a yaml-file.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -n SESSION_NAME, --session_name SESSION_NAME
-                                Name used for the tmux session
-          -t TMUX_CONFIG, --tmux_config TMUX_CONFIG
-                                This config will be used for the tmux session
-          -d, --detach          Start session in detached mode
-          --overwrite OVERWRITE
-                                Overwrite a parameter from the session config. Parameters can be specified
-                                using a comma-separated list such as '--overwrite param_a=1,param_b=2'.
-        ```
-        
-        ### Full blown example
-        To make use of all catmux features, run the following example command:
-        ```
-        catmux_create_session $(python3 -m catmux.prefix)/share/catmux/example_session.yaml \
-          --tmux_config $(python3 -m catmux.prefix)/share/catmux/tmux_default.conf \
-          --session_name example_session \
-          --overwrite show_layouts=True,replacement_param="new catmux user"
-        ```
-        
-        ### Killing a catmux session
-        If you are not that familiar with tmux: To kill a session, simply type `tmux kill-session` in any
-        terminal window. In the `etc/tmux_default.conf` there is a key-binding for that, see
-        `etc/readme_tmux.txt` for details.
-        
-        ### Tmux server to be used
-        By default, catmux spawns its own tmux server called `catmux`. Therefore, a simple
-        `tmux list-sessions` (or `tmux ls`) will not list the `catmux` session. To list the `catmux`
-        session, use `tmux -L catmux list-sessions`. You can change the server's name by specifying the
-        `-L <server_name>` parameter to `catmux_create_session`. That mechanism ensures that the environment
-        in which `catmux_create_session` is started, will be used inside the catmux session (as long as no
-        other session previously exists on that particular tmux server).
-        
-        ## Migrating from the catkin version of catmux
-        With the spread of ROS2, the need for a catkin-independent catmux has emerged.
-        Catmux is now a plain python package without the ROS integration.
-        Therefore, it is installed via pip and no longer needs to be part of a catkin workspace.
-        This opens the possibility to easily use catmux outside of robotics application, e.g. for server
-        administration or other development tasks.
-        
-        Catmux no longer has the `package://<your_package_name>` lookup capabilities.
-        To achieve the same outcome, simply use rospack:
-        ```
-        catmux_create_session $(rospack find <your_package_name>)/path/to/<your_catmux_session_config.yaml>
-        ```
-        
-        For ROS2, the same is achievable with `ros2 pkg prefix` but the yaml has to be installed (similar
-        to, for example, a launch file) and the installation path has to be specified:
-        ```
-        catmux_create_session $(ros2 pkg prefix <your_package_name>)/path/to/the/installed/<your_catmux_session_config.yaml>
-        
-        # for example: $ catmux_create_session $(ros2 pkg prefix catmux_test_pkg)/share/catmux_test_pkg/catmux_session.yaml
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Catmux
+
+## About
+Catmux is a little helper to run a tmux session with multiple windows and panes with just one
+command. It is inspired and functionally very similar to
+[tmuxinator](https://github.com/tmuxinator/tmuxinator), but without the project management feature
+which is in my opinion kind of an overhead.
+
+Session configs can be stored anywhere and have to be given as an argument.
+
+## Motivation
+In most of our ROS projects at work we use shell output for almost all nodes to get log information
+during runtime. Having all this in one window where you start your "Start it all"-launchfile makes
+it very hard to follow the log of a specific node. Starting everything in separate windows is quite
+a lot of work and requires documentation overhead in sense of documenting which launchfiles or nodes
+have to be started.
+
+At a conference I caught the idea to use tmux scripting to orchestrate all this in one tmux session.
+However, quickly I noticed that creating these scripts is a daunting task as you'll have to type in
+a lot of commands over and over again and as soon as you wanted to do things a little different such
+as not starting a particular launchfile if a certain parameter was set, things got complicated.
+
+I liked the yaml-syntax of [tmuxinator](https://github.com/tmuxinator/tmuxinator), but that tool
+didn't quite hit the spot. I wanted to have something that can be easily integrated into a ROS
+project and I definitely wanted something that saves the config per project and not all configs at
+one central spot on a particular machine.
+
+## Installation
+Catmux is a pure python package and the installation via `pip3 install --user catmux` is recommended.
+
+You can also install it by cloning this repository and calling `pip3 install --user .` in the
+repository's root directory. If you use this option, please be aware that some examples behave
+differently if you have installed catmux this way and are calling it from the repository directory.
+Calling them from outside the directory (e.g. after leaving via `cd`) is fine and should result in
+the same behavior as with the recommended installation method.
+
+## Usage
+Currently, there is no full-blown documentation, but the example config file in
+`etc/example_session.yaml` gives a detailed insight on possible commands.
+
+### Running the example the most simple way
+After installation, you can run a simple example by calling the following command:
+```
+catmux_create_session $(python3 -m catmux.prefix)/share/catmux/example_session.yaml
+```
+
+To see further options, simply run it with argument `-h`:
+```
+$ catmux_create_session -h
+usage: catmux_create_session [-h] [-n SESSION_NAME] [-t TMUX_CONFIG] [-d] [--overwrite OVERWRITE]
+                             session_config
+
+Create a new catmux session
+
+positional arguments:
+  session_config        Session configuration. Should be a yaml-file.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -n SESSION_NAME, --session_name SESSION_NAME
+                        Name used for the tmux session
+  -t TMUX_CONFIG, --tmux_config TMUX_CONFIG
+                        This config will be used for the tmux session
+  -d, --detach          Start session in detached mode
+  --overwrite OVERWRITE
+                        Overwrite a parameter from the session config. Parameters can be specified
+                        using a comma-separated list such as '--overwrite param_a=1,param_b=2'.
+```
+
+### Full blown example
+To make use of all catmux features, run the following example command:
+```
+catmux_create_session $(python3 -m catmux.prefix)/share/catmux/example_session.yaml \
+  --tmux_config $(python3 -m catmux.prefix)/share/catmux/tmux_default.conf \
+  --session_name example_session \
+  --overwrite show_layouts=True,replacement_param="new catmux user"
+```
+
+### Killing a catmux session
+If you are not that familiar with tmux: To kill a session, simply type `tmux kill-session` in any
+terminal window. In the `etc/tmux_default.conf` there is a key-binding for that, see
+`etc/readme_tmux.txt` for details.
+
+### Tmux server to be used
+By default, catmux spawns its own tmux server called `catmux`. Therefore, a simple
+`tmux list-sessions` (or `tmux ls`) will not list the `catmux` session. To list the `catmux`
+session, use `tmux -L catmux list-sessions`. You can change the server's name by specifying the
+`-L <server_name>` parameter to `catmux_create_session`. That mechanism ensures that the environment
+in which `catmux_create_session` is started, will be used inside the catmux session (as long as no
+other session previously exists on that particular tmux server).
+
+## Migrating from the catkin version of catmux
+With the spread of ROS2, the need for a catkin-independent catmux has emerged.
+Catmux is now a plain python package without the ROS integration.
+Therefore, it is installed via pip and no longer needs to be part of a catkin workspace.
+This opens the possibility to easily use catmux outside of robotics application, e.g. for server
+administration or other development tasks.
+
+Catmux no longer has the `package://<your_package_name>` lookup capabilities.
+To achieve the same outcome, simply use rospack:
+```
+catmux_create_session $(rospack find <your_package_name>)/path/to/<your_catmux_session_config.yaml>
+```
+
+For ROS2, the same is achievable with `ros2 pkg prefix` but the yaml has to be installed (similar
+to, for example, a launch file) and the installation path has to be specified:
+```
+catmux_create_session $(ros2 pkg prefix <your_package_name>)/path/to/the/installed/<your_catmux_session_config.yaml>
+
+# for example: $ catmux_create_session $(ros2 pkg prefix catmux_test_pkg)/share/catmux_test_pkg/catmux_session.yaml
+```
```

### Comparing `catmux-0.3.1/etc/example_session.yaml` & `catmux-0.3.2/etc/example_session.yaml`

 * *Files identical despite different names*

### Comparing `catmux-0.3.1/etc/readme_tmux.txt` & `catmux-0.3.2/etc/readme_tmux.txt`

 * *Files identical despite different names*

### Comparing `catmux-0.3.1/etc/tmux_default.conf` & `catmux-0.3.2/etc/tmux_default.conf`

 * *Files 26% similar despite different names*

```diff
@@ -28,7 +28,11 @@
 bind-key h select-pane -L
 bind-key l select-pane -R
 bind-key j select-pane -D
 bind-key k select-pane -U
 bind-key K confirm-before kill-session
 
 set -g history-limit 99999
+
+# tmux colors
+set -g default-terminal "xterm-256color"
+set -ag terminal-overrides ",xterm-256color:Tc"
```

### Comparing `catmux-0.3.1/script/catmux_create_session` & `catmux-0.3.2/script/catmux_create_session`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # -- END LICENSE BLOCK ------------------------------------------------
 
 from __future__ import print_function
 import os
 import subprocess
-import site
 import sys
 
-import rospkg
-
 import argparse
 
 from catmux.session import Session as CatmuxSession
 from catmux.prefix import get_prefix
 
 
 def safe_call(cmd_list):
```

### Comparing `catmux-0.3.1/setup.py` & `catmux-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="catmux",
-    version="0.3.1",
+    version="0.3.2",
     license="MIT",
     author="Felix Exner",
     author_email="felix_mauch@web.de",
     description="A tmux orchestration package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fmauch/catmux",
```

