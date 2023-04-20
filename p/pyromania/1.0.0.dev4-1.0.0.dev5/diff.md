# Comparing `tmp/pyromania-1.0.0.dev4.tar.gz` & `tmp/pyromania-1.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/var/www-dev/tallen/pyromania/dist/.tmp-gvhiel1_/pyromania-1.0.0.dev4.tar", last modified: Mon Apr  3 14:54:16 2023, max compression
+gzip compressed data, was "pyromania-1.0.0.dev5.tar", last modified: Thu Apr 20 17:02:12 2023, max compression
```

## Comparing `pyromania-1.0.0.dev4.tar` & `pyromania-1.0.0.dev5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwx------   0 tallen   (86646) wrds     (60359)        0 2023-04-03 14:54:16.941351 pyromania-1.0.0.dev4/
--rw-------   0 tallen   (86646) wrds     (60359)     3209 2023-04-03 14:54:16.940351 pyromania-1.0.0.dev4/PKG-INFO
--rw-------   0 tallen   (86646) wrds     (60359)     2069 2023-04-03 14:39:17.000000 pyromania-1.0.0.dev4/README.md
-drwx------   0 tallen   (86646) wrds     (60359)        0 2023-04-03 14:54:16.936351 pyromania-1.0.0.dev4/ansible-role-install/
--rw-------   0 tallen   (86646) wrds     (60359)      142 2023-03-02 15:12:08.000000 pyromania-1.0.0.dev4/ansible-role-install/README.md
-drwx------   0 tallen   (86646) wrds     (60359)        0 2023-04-03 14:54:16.939351 pyromania-1.0.0.dev4/ansible-role-install/tasks/
--rw-------   0 tallen   (86646) wrds     (60359)      855 2023-03-02 15:12:08.000000 pyromania-1.0.0.dev4/ansible-role-install/tasks/main.yml
--rw-------   0 tallen   (86646) wrds     (60359)     1198 2023-03-02 15:14:53.000000 pyromania-1.0.0.dev4/install-sudo.sh
--rw-------   0 tallen   (86646) wrds     (60359)      952 2023-03-02 15:14:53.000000 pyromania-1.0.0.dev4/install.sh
--rw-------   0 tallen   (86646) wrds     (60359)     1272 2023-02-22 00:17:19.000000 pyromania-1.0.0.dev4/pyproject.toml
--rw-------   0 tallen   (86646) wrds     (60359)     8652 2023-04-03 14:39:17.000000 pyromania-1.0.0.dev4/pyro.sh
--rw-------   0 tallen   (86646) wrds     (60359)      944 2023-04-03 14:46:46.000000 pyromania-1.0.0.dev4/pyro_test.sh
-drwx------   0 tallen   (86646) wrds     (60359)        0 2023-04-03 14:54:16.940351 pyromania-1.0.0.dev4/pyromania.egg-info/
--rw-------   0 tallen   (86646) wrds     (60359)     3209 2023-04-03 14:54:16.000000 pyromania-1.0.0.dev4/pyromania.egg-info/PKG-INFO
--rw-------   0 tallen   (86646) wrds     (60359)      271 2023-04-03 14:54:16.000000 pyromania-1.0.0.dev4/pyromania.egg-info/SOURCES.txt
--rw-------   0 tallen   (86646) wrds     (60359)        1 2023-04-03 14:54:16.000000 pyromania-1.0.0.dev4/pyromania.egg-info/dependency_links.txt
--rw-------   0 tallen   (86646) wrds     (60359)        1 2023-04-03 14:54:16.000000 pyromania-1.0.0.dev4/pyromania.egg-info/top_level.txt
--rw-------   0 tallen   (86646) wrds     (60359)       38 2023-04-03 14:54:16.941351 pyromania-1.0.0.dev4/setup.cfg
+drwxr-xr-x   0 tallen     (503) staff       (20)        0 2023-04-20 17:02:12.839606 pyromania-1.0.0.dev5/
+-rw-r--r--   0 tallen     (503) staff       (20)     3209 2023-04-20 17:02:12.839465 pyromania-1.0.0.dev5/PKG-INFO
+-rw-r--r--   0 tallen     (503) staff       (20)     2069 2023-04-20 16:46:58.000000 pyromania-1.0.0.dev5/README.md
+drwxr-xr-x   0 tallen     (503) staff       (20)        0 2023-04-20 17:02:12.838682 pyromania-1.0.0.dev5/ansible-role-install/
+-rw-r--r--   0 tallen     (503) staff       (20)      142 2023-04-20 16:46:58.000000 pyromania-1.0.0.dev5/ansible-role-install/README.md
+drwxr-xr-x   0 tallen     (503) staff       (20)        0 2023-04-20 17:02:12.838800 pyromania-1.0.0.dev5/ansible-role-install/tasks/
+-rw-r--r--   0 tallen     (503) staff       (20)      855 2023-04-20 16:46:58.000000 pyromania-1.0.0.dev5/ansible-role-install/tasks/main.yml
+-rw-r--r--   0 tallen     (503) staff       (20)     1198 2023-04-20 16:46:58.000000 pyromania-1.0.0.dev5/install-sudo.sh
+-rw-r--r--   0 tallen     (503) staff       (20)      952 2023-02-28 14:35:16.000000 pyromania-1.0.0.dev5/install.sh
+-rw-r--r--   0 tallen     (503) staff       (20)     1272 2023-02-28 14:21:14.000000 pyromania-1.0.0.dev5/pyproject.toml
+-rw-r--r--   0 tallen     (503) staff       (20)     8781 2023-04-20 16:52:19.000000 pyromania-1.0.0.dev5/pyro.sh
+-rw-r--r--   0 tallen     (503) staff       (20)      944 2023-04-20 16:46:58.000000 pyromania-1.0.0.dev5/pyro_test.sh
+drwxr-xr-x   0 tallen     (503) staff       (20)        0 2023-04-20 17:02:12.839276 pyromania-1.0.0.dev5/pyromania.egg-info/
+-rw-r--r--   0 tallen     (503) staff       (20)     3209 2023-04-20 17:02:12.000000 pyromania-1.0.0.dev5/pyromania.egg-info/PKG-INFO
+-rw-r--r--   0 tallen     (503) staff       (20)      271 2023-04-20 17:02:12.000000 pyromania-1.0.0.dev5/pyromania.egg-info/SOURCES.txt
+-rw-r--r--   0 tallen     (503) staff       (20)        1 2023-04-20 17:02:12.000000 pyromania-1.0.0.dev5/pyromania.egg-info/dependency_links.txt
+-rw-r--r--   0 tallen     (503) staff       (20)        1 2023-04-20 17:02:12.000000 pyromania-1.0.0.dev5/pyromania.egg-info/top_level.txt
+-rw-r--r--   0 tallen     (503) staff       (20)       38 2023-04-20 17:02:12.839637 pyromania-1.0.0.dev5/setup.cfg
```

### Comparing `pyromania-1.0.0.dev4/PKG-INFO` & `pyromania-1.0.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyromania
-Version: 1.0.0.dev4
+Version: 1.0.0.dev5
 Summary: Pyromania creates and manages Python 3 venvs, inspired by virtualenvwrapper.
 Author-email: Tim Allen <tallen@wharton.upenn.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/FlipperPA/pyromania/
 Project-URL: Repository, https://github.com/FlipperPA/pyromania/
 Project-URL: Documentation, https://github.com/FlipperPA/pyromania/
 Project-URL: Bug Tracker, https://github.com/FlipperPA/pyromania/issues
```

### Comparing `pyromania-1.0.0.dev4/README.md` & `pyromania-1.0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `pyromania-1.0.0.dev4/ansible-role-install/tasks/main.yml` & `pyromania-1.0.0.dev5/ansible-role-install/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pyromania-1.0.0.dev4/install-sudo.sh` & `pyromania-1.0.0.dev5/install-sudo.sh`

 * *Files identical despite different names*

### Comparing `pyromania-1.0.0.dev4/install.sh` & `pyromania-1.0.0.dev5/install.sh`

 * *Files identical despite different names*

### Comparing `pyromania-1.0.0.dev4/pyproject.toml` & `pyromania-1.0.0.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyromania-1.0.0.dev4/pyro.sh` & `pyromania-1.0.0.dev5/pyro.sh`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,19 @@
     ACTIVE_NAME=$1
     ACTIVE_DIR=`pwd`
     ACTIVE_VENV="${VENV_DIR}"
 
     if [ $2 = "--auto-create" ]; then
         echo "There is no venv called '${ACTIVE_NAME}'. Do you want to create it? (y/N) "
         read yes_no
+
+	# Uppercase the first character of the input
         yes_no=${yes_no:0:1}
-        yes_no=${yes_no^^}
+        yes_no=`echo $yes_no | tr a-z A-Z`
+
         if [ "$yes_no" != "Y" ]; then
             echo "Not creating the new venv '${ACTIVE_NAME}'."
             return
         fi
     fi
 
     if [ -f "${ACTIVE_DIR}/${ACTIVE_VENV}/bin/activate" ]; then
@@ -245,14 +248,15 @@
         else
             pyro_activate
         fi
     fi
 }
 alias pyro=fn_pyro
 
+# complete is a bash built-in, so it should always be available.
 pyro_autocomplete() 
 {
     local cur prev opts
     COMPREPLY=()
     cur="${COMP_WORDS[COMP_CWORD]}"
     prev="${COMP_WORDS[COMP_CWORD-1]}"
```

### Comparing `pyromania-1.0.0.dev4/pyro_test.sh` & `pyromania-1.0.0.dev5/pyro_test.sh`

 * *Files identical despite different names*

### Comparing `pyromania-1.0.0.dev4/pyromania.egg-info/PKG-INFO` & `pyromania-1.0.0.dev5/pyromania.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyromania
-Version: 1.0.0.dev4
+Version: 1.0.0.dev5
 Summary: Pyromania creates and manages Python 3 venvs, inspired by virtualenvwrapper.
 Author-email: Tim Allen <tallen@wharton.upenn.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/FlipperPA/pyromania/
 Project-URL: Repository, https://github.com/FlipperPA/pyromania/
 Project-URL: Documentation, https://github.com/FlipperPA/pyromania/
 Project-URL: Bug Tracker, https://github.com/FlipperPA/pyromania/issues
```

