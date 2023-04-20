# Comparing `tmp/addsshkeys-0.4.0.tar.gz` & `tmp/addsshkeys-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/addsshkeys-0.4.0.tar", last modified: Mon Oct 19 18:55:47 2020, max compression
+gzip compressed data, was "addsshkeys-0.5.tar", last modified: Thu Apr 20 20:47:13 2023, max compression
```

## Comparing `addsshkeys-0.4.0.tar` & `addsshkeys-0.5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 ken       (1000) ken        (502)        0 2020-10-19 18:55:47.165583 addsshkeys-0.4.0/
--rw-rw-r--   0 ken       (1000) ken        (502)     5270 2020-10-19 18:55:47.163583 addsshkeys-0.4.0/PKG-INFO
--rw-rw-r--   0 ken       (1000) ken        (502)     3479 2020-10-19 18:54:02.000000 addsshkeys-0.4.0/README.rst
--rwxrwxr-x   0 ken       (1000) ken        (502)     5850 2020-10-19 18:54:02.000000 addsshkeys-0.4.0/addsshkeys
-drwxrwxr-x   0 ken       (1000) ken        (502)        0 2020-10-19 18:55:47.162583 addsshkeys-0.4.0/addsshkeys.egg-info/
--rw-rw-r--   0 ken       (1000) ken        (502)     5270 2020-10-19 18:55:46.000000 addsshkeys-0.4.0/addsshkeys.egg-info/PKG-INFO
--rw-rw-r--   0 ken       (1000) ken        (502)      199 2020-10-19 18:55:46.000000 addsshkeys-0.4.0/addsshkeys.egg-info/SOURCES.txt
--rw-rw-r--   0 ken       (1000) ken        (502)        1 2020-10-19 18:55:46.000000 addsshkeys-0.4.0/addsshkeys.egg-info/dependency_links.txt
--rw-rw-r--   0 ken       (1000) ken        (502)       69 2020-10-19 18:55:46.000000 addsshkeys-0.4.0/addsshkeys.egg-info/requires.txt
--rw-rw-r--   0 ken       (1000) ken        (502)        1 2020-10-19 18:55:46.000000 addsshkeys-0.4.0/addsshkeys.egg-info/top_level.txt
--rw-rw-r--   0 ken       (1000) ken        (502)       38 2020-10-19 18:55:47.165583 addsshkeys-0.4.0/setup.cfg
--rw-rw-r--   0 ken       (1000) ken        (502)     1274 2020-10-19 18:54:02.000000 addsshkeys-0.4.0/setup.py
+drwx------   0 ken       (1000) ken       (1001)        0 2023-04-20 20:47:13.092361 addsshkeys-0.5/
+-rw-------   0 ken       (1000) ken       (1001)     5062 2023-04-20 20:47:13.092361 addsshkeys-0.5/PKG-INFO
+-rw-rw-r--   0 ken       (1000) ken       (1001)     4300 2023-04-20 20:44:11.000000 addsshkeys-0.5/README.rst
+-rwxrwxr-x   0 ken       (1000) ken       (1001)     6575 2023-04-20 20:44:11.000000 addsshkeys-0.5/addsshkeys
+drwx------   0 ken       (1000) ken       (1001)        0 2023-04-20 20:47:13.092361 addsshkeys-0.5/addsshkeys.egg-info/
+-rw-------   0 ken       (1000) ken       (1001)     5062 2023-04-20 20:47:13.000000 addsshkeys-0.5/addsshkeys.egg-info/PKG-INFO
+-rw-------   0 ken       (1000) ken       (1001)      228 2023-04-20 20:47:13.000000 addsshkeys-0.5/addsshkeys.egg-info/SOURCES.txt
+-rw-------   0 ken       (1000) ken       (1001)        1 2023-04-20 20:47:13.000000 addsshkeys-0.5/addsshkeys.egg-info/dependency_links.txt
+-rw-------   0 ken       (1000) ken       (1001)       69 2023-04-20 20:47:13.000000 addsshkeys-0.5/addsshkeys.egg-info/requires.txt
+-rw-------   0 ken       (1000) ken       (1001)        1 2023-04-20 20:47:13.000000 addsshkeys-0.5/addsshkeys.egg-info/top_level.txt
+-rw-------   0 ken       (1000) ken       (1001)        1 2023-04-20 20:47:12.000000 addsshkeys-0.5/addsshkeys.egg-info/zip-safe
+-rw-------   0 ken       (1000) ken       (1001)       38 2023-04-20 20:47:13.092361 addsshkeys-0.5/setup.cfg
+-rw-rw-r--   0 ken       (1000) ken       (1001)     1272 2023-04-20 20:44:11.000000 addsshkeys-0.5/setup.py
```

### Comparing `addsshkeys-0.4.0/PKG-INFO` & `addsshkeys-0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,141 +1,170 @@
 Metadata-Version: 2.1
 Name: addsshkeys
-Version: 0.4.0
+Version: 0.5
 Summary: Add keys to SSH Agent
 Home-page: https://github.com/kenkundert/addsshkeys
+Download-URL: https://github.com/kenkundert/addsshkeys/tarball/master
 Author: Ken Kundert
 Author-email: addsshkeys@nurdletech.com
 License: GPLv3+
-Download-URL: https://github.com/kenkundert/addsshkeys/tarball/master
-Description: AddSSHkeys:  Add Keys to SSH Agent
-        ==================================
-        
-        | Version: 0.4.0
-        | Released: 2020-10-19
-        |
-        
-        *AddSSHkeys* adds all of your keys to SSH Agent in one operation. It can work 
-        with `Avendesora <https://avendesora.readthedocs.io>`_ to keep your passphrases 
-        secure.
-        
-        Please report all bugs and suggestions to addsshkeys@nurdletech.com
-        
-        Getting Started
-        ---------------
-        
-        You download and install *AddSSHkeys* with::
-        
-            pip3 install --user addsshkeys
-        
-        Once installed, you will need at least one configuration file.
-        Configurations are placed in: ~/.config/addsshkeys.
-        They are `NestedText <https://nestedtext.readthedocs.io>`_ files.
-        The default configuration is *config*; the default file is *config.nt*.
-        
-        The following settings may be given in your config files.
-        
-        **ssh_add**
-        
-        The name of the command that adds keys to your SSH agent. By default, 'ssh-add' 
-        is used.
-        
-        **ssh_keys**
-        
-        This setting is required.  It contains a dictionary of dictionaries that 
-        contains information about each key.  The primary dictionary contains a name and 
-        the values for each key. The values are held in a dictionary that may contain 
-        three fields:
-        
-        *paths*
-        
-        This is required and contains the paths to one or more SSH private key files.  
-        It may be a list of strings, or a single string that is split.  If a relative 
-        path is given, it is relative to ~/.ssh.
-        
-        *account*
-        
-        This gives the name of the Avendesora account that holds passphrase for the 
-        keys. If present, Avendesora will be queried for the passphrase.
-        
-        *passphrase*
-        
-        This is required if *account* is not given, otherwise it is optional.  If 
-        *account* is given, it is the name of the passphrase field in Avendesora, which 
-        defaults to 'passcode'. If account is not given, it is the passphrase itself. In 
-        this case, the settings file should only be readable by the user.
-        
-        **config_file_mask**
-        
-        An integer that determines if a warning should be printed about the
-        config file permissions being too loose.  The permissions are only checked
-        if the file is found to contain a passphrase. Default is 0o077.  Set to
-        0o000 to disable the warning. Set to 0o077 to generate a warning if the
-        configuration directory is readable or writable by the group or others. Set
-        to 0o007 to generated a warning if the directory is readable or writable by
-        others.
-        
-        Here is an example configuration file::
-        
-            ssh_keys:
-                primary:
-                    paths: primary-ed25519 primary-rsa
-                    account: primary-ssh-key
-                digitalocean:
-                    paths: digitalocean
-                    account: digitalocean-ssh-key
-                github:
-                    paths: github
-                    passphrase: canard apply trousseau forgive
-                backups:
-                    paths: dumper
-                    account: dumper-ssh-key
-        
-        
-        Running AddSSHkeys
-        ------------------
-        
-        Once configured, you can run *AddSSHkeys* with the default configuration using::
-        
-            addsshkeys
-        
-        And you can run it with a particular configuration using::
-        
-            addsshkeys <config>
-        
-        where ``<config>`` is the name of the configuration you wish to use (no need to 
-        give the .nt suffix).  In this way you can have several bundles of keys that you 
-        can load as needed.
-        
-        
-        Releases
-        --------
-        **Latest Development Version**:
-            | Version: 0.4.0
-            | Released: 2020-10-19
-        
-        
-        0.4 (2020-10-19)
-            - fix *config_file_mask*.
-        
-        0.3 (2020-10-19)
-            - allow config file to end with .nt suffix.
-        
-        0.2 (2020-10-14)
-            - update to latest version of NestedText
-        
-        0.1 (2020-08-31)
-            - convert to NestedText for settings file.
-        
 Keywords: avendesora,ssh
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+
+AddSSHkeys — Add Keys to SSH Agent
+==================================
+
+.. image:: https://pepy.tech/badge/addsshkeys/month
+    :target: https://pepy.tech/project/addsshkeys
+
+.. image:: https://img.shields.io/pypi/v/addsshkeys.svg
+    :target: https://pypi.python.org/pypi/addsshkeys
+
+.. image:: https://img.shields.io/pypi/pyversions/addsshkeys.svg
+    :target: https://pypi.python.org/pypi/addsshkeys
+
+| Version: 0.5
+| Released: 2023-04-20
+|
+
+*AddSSHkeys* adds all of your keys to SSH Agent in one operation.
+It is helpful if you routinely add more than one key to your agent.
+It can work with `Avendesora <https://avendesora.readthedocs.io>`_ to keep your 
+passphrases secure.
+
+Please report all bugs and suggestions to addsshkeys@nurdletech.com
+
+Getting Started
+---------------
+
+Download and install *AddSSHkeys* with::
+
+    pip install addsshkeys
+
+Once installed, you will need at least one configuration file.
+Configurations are placed in: ~/.config/addsshkeys.
+They are `NestedText <https://nestedtext.org>`_ files.
+The default configuration is *config*; the default file is *config.nt*.
+
+The following settings may be given in your config files.
+
+**ssh_add**
+
+The name of the command that adds keys to your SSH agent.
+By default, 'ssh-add' is used.
+
+**ssh_keys**
+
+This setting is required.
+It contains a dictionary of dictionaries that contains information about each 
+key.
+The primary dictionary contains a name and the values for each key.
+The values are held in a dictionary that may contain three fields:
+
+*paths*
+
+This is required and contains the paths to one or more SSH private key files.
+It may be a list of strings, or a single string that is split.
+If a relative path is given, it is relative to ~/.ssh.
+
+*account*
+
+This gives the name of the Avendesora account that holds passphrase for the 
+keys.
+If present, Avendesora will be queried for the passphrase.
+
+*passphrase*
+
+This is required if *account* is not given, otherwise it is optional.
+If *account* is given, it is the name of the passphrase field in Avendesora, 
+which defaults to 'passcode'.
+If account is not given, it is the passphrase itself.
+In this case, the settings file should only be readable by the user.
+
+**config_file_mask**
+
+An integer that determines if a warning should be printed about the config file 
+permissions being too loose.
+The permissions are only checked if the file is found to contain a passphrase.
+Default is 077.
+Set to 000 to disable the warning.
+Set to 077 to generate a warning if the configuration directory is readable or 
+writable by the group or others.
+Set to 007 to generated a warning if the directory is readable or writable by 
+others.
+
+**auth_sock_path**
+
+If given, the value of $SSH_AUTH_SOCKET is written to the specified path.
+This can be useful when running SSH related commands in cron and anacron 
+scripts.
+
+
+Here is an example configuration file::
+
+    ssh_keys:
+        primary:
+            paths: primary-ed25519 primary-rsa
+            account: primary-ssh-key
+        digitalocean:
+            paths: digitalocean
+            account: digitalocean-ssh-key
+        github:
+            paths: github
+            passphrase: canard apply trousseau forgive
+        backups:
+            paths: dumper
+            account: dumper-ssh-key
+
+    # assure config file is only readable by me
+    config_file_mask: 077
+
+    # used to provide path to SSH authorization socket to scripts run by cron
+    auth_sock_path: ~/.ssh/auth-sock
+
+Underscores can be replaced by spaces in all keys.
+
+Running AddSSHkeys
+------------------
+
+Once configured, you can run *AddSSHkeys* with the default configuration using::
+
+    addsshkeys
+
+And you can run it with a particular configuration using::
+
+    addsshkeys <config>
+
+where ``<config>`` is the name of the configuration you wish to use (no need to 
+give the .nt suffix).
+In this way you can have several bundles of keys that you can load as needed.
+
+
+Releases
+--------
+**Latest Development Version**:
+    | Version: 0.5
+    | Released: 2023-04-20
+
+0.5 (2023-04-20)
+    - added *auth_sock_path*.
+
+0.4 (2020-10-19)
+    - fix *config_file_mask*.
+
+0.3 (2020-10-19)
+    - allow config file to end with .nt suffix.
+
+0.2 (2020-10-14)
+    - update to latest version of NestedText
+
+0.1 (2020-08-31)
+    - convert to NestedText for settings file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `addsshkeys-0.4.0/README.rst` & `addsshkeys-0.5/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,96 @@
-AddSSHkeys:  Add Keys to SSH Agent
+AddSSHkeys — Add Keys to SSH Agent
 ==================================
 
-| Version: 0.4.0
-| Released: 2020-10-19
+.. image:: https://pepy.tech/badge/addsshkeys/month
+    :target: https://pepy.tech/project/addsshkeys
+
+.. image:: https://img.shields.io/pypi/v/addsshkeys.svg
+    :target: https://pypi.python.org/pypi/addsshkeys
+
+.. image:: https://img.shields.io/pypi/pyversions/addsshkeys.svg
+    :target: https://pypi.python.org/pypi/addsshkeys
+
+| Version: 0.5
+| Released: 2023-04-20
 |
 
-*AddSSHkeys* adds all of your keys to SSH Agent in one operation. It can work 
-with `Avendesora <https://avendesora.readthedocs.io>`_ to keep your passphrases 
-secure.
+*AddSSHkeys* adds all of your keys to SSH Agent in one operation.
+It is helpful if you routinely add more than one key to your agent.
+It can work with `Avendesora <https://avendesora.readthedocs.io>`_ to keep your 
+passphrases secure.
 
 Please report all bugs and suggestions to addsshkeys@nurdletech.com
 
 Getting Started
 ---------------
 
-You download and install *AddSSHkeys* with::
+Download and install *AddSSHkeys* with::
 
-    pip3 install --user addsshkeys
+    pip install addsshkeys
 
 Once installed, you will need at least one configuration file.
 Configurations are placed in: ~/.config/addsshkeys.
-They are `NestedText <https://nestedtext.readthedocs.io>`_ files.
+They are `NestedText <https://nestedtext.org>`_ files.
 The default configuration is *config*; the default file is *config.nt*.
 
 The following settings may be given in your config files.
 
 **ssh_add**
 
-The name of the command that adds keys to your SSH agent. By default, 'ssh-add' 
-is used.
+The name of the command that adds keys to your SSH agent.
+By default, 'ssh-add' is used.
 
 **ssh_keys**
 
-This setting is required.  It contains a dictionary of dictionaries that 
-contains information about each key.  The primary dictionary contains a name and 
-the values for each key. The values are held in a dictionary that may contain 
-three fields:
+This setting is required.
+It contains a dictionary of dictionaries that contains information about each 
+key.
+The primary dictionary contains a name and the values for each key.
+The values are held in a dictionary that may contain three fields:
 
 *paths*
 
-This is required and contains the paths to one or more SSH private key files.  
-It may be a list of strings, or a single string that is split.  If a relative 
-path is given, it is relative to ~/.ssh.
+This is required and contains the paths to one or more SSH private key files.
+It may be a list of strings, or a single string that is split.
+If a relative path is given, it is relative to ~/.ssh.
 
 *account*
 
 This gives the name of the Avendesora account that holds passphrase for the 
-keys. If present, Avendesora will be queried for the passphrase.
+keys.
+If present, Avendesora will be queried for the passphrase.
 
 *passphrase*
 
-This is required if *account* is not given, otherwise it is optional.  If 
-*account* is given, it is the name of the passphrase field in Avendesora, which 
-defaults to 'passcode'. If account is not given, it is the passphrase itself. In 
-this case, the settings file should only be readable by the user.
+This is required if *account* is not given, otherwise it is optional.
+If *account* is given, it is the name of the passphrase field in Avendesora, 
+which defaults to 'passcode'.
+If account is not given, it is the passphrase itself.
+In this case, the settings file should only be readable by the user.
 
 **config_file_mask**
 
-An integer that determines if a warning should be printed about the
-config file permissions being too loose.  The permissions are only checked
-if the file is found to contain a passphrase. Default is 0o077.  Set to
-0o000 to disable the warning. Set to 0o077 to generate a warning if the
-configuration directory is readable or writable by the group or others. Set
-to 0o007 to generated a warning if the directory is readable or writable by
+An integer that determines if a warning should be printed about the config file 
+permissions being too loose.
+The permissions are only checked if the file is found to contain a passphrase.
+Default is 077.
+Set to 000 to disable the warning.
+Set to 077 to generate a warning if the configuration directory is readable or 
+writable by the group or others.
+Set to 007 to generated a warning if the directory is readable or writable by 
 others.
 
+**auth_sock_path**
+
+If given, the value of $SSH_AUTH_SOCKET is written to the specified path.
+This can be useful when running SSH related commands in cron and anacron 
+scripts.
+
+
 Here is an example configuration file::
 
     ssh_keys:
         primary:
             paths: primary-ed25519 primary-rsa
             account: primary-ssh-key
         digitalocean:
@@ -77,37 +99,46 @@
         github:
             paths: github
             passphrase: canard apply trousseau forgive
         backups:
             paths: dumper
             account: dumper-ssh-key
 
+    # assure config file is only readable by me
+    config_file_mask: 077
+
+    # used to provide path to SSH authorization socket to scripts run by cron
+    auth_sock_path: ~/.ssh/auth-sock
+
+Underscores can be replaced by spaces in all keys.
 
 Running AddSSHkeys
 ------------------
 
 Once configured, you can run *AddSSHkeys* with the default configuration using::
 
     addsshkeys
 
 And you can run it with a particular configuration using::
 
     addsshkeys <config>
 
 where ``<config>`` is the name of the configuration you wish to use (no need to 
-give the .nt suffix).  In this way you can have several bundles of keys that you 
-can load as needed.
+give the .nt suffix).
+In this way you can have several bundles of keys that you can load as needed.
 
 
 Releases
 --------
 **Latest Development Version**:
-    | Version: 0.4.0
-    | Released: 2020-10-19
+    | Version: 0.5
+    | Released: 2023-04-20
 
+0.5 (2023-04-20)
+    - added *auth_sock_path*.
 
 0.4 (2020-10-19)
     - fix *config_file_mask*.
 
 0.3 (2020-10-19)
     - allow config file to end with .nt suffix.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `addsshkeys-0.4.0/addsshkeys` & `addsshkeys-0.5/addsshkeys`

 * *Files 15% similar despite different names*

```diff
@@ -1,157 +1,218 @@
 #!/usr/bin/env python3
+# DESCRIPTION {{{1
 """
 Add keys to SSH agent
 
 Usage:
     addsshkeys [options] [<config>]
 
 Options:
-    -v, --verbose    list the keys as they are being added to ssh agent
-    -l, --list       list the keys without adding them to ssh agent
+    -v, --verbose          list the keys as they are being added to ssh agent
+    -l, --list             list the keys without adding them to ssh agent
 
 Configurations can be found in: {settings_dir}.
-They are Python files.  The default configuration is {config_filename}.
-
-Currently there is only one setting available: ssh_keys.  It contains
-a dictionary of dictionaries that contains information about each key.  The
-primary dictionary contains a name and the values for each key. The values are
-held in a dictionary that may contain three fields: paths, account, and
-passphrase.  The first, paths, is required and contains the paths to one or more
-SSH private key files.  It may be a list of strings, or a single string that is
-split.  If a relative path is given, it is relative to ~/.ssh.  The second,
-account, gives the name of the avendesora account that holds passphrase for the
-keys. If present, Avendesora will be queried for the passphrase. The third,
-passphrase is required if account is not given, otherwise it is optional.  If
-account is given, it is the name of the passphrase field in Avendesora, which
-defaults to 'passcode'. If account is not given, it is the passphrase itself. In
-this case, the settings file should only be readable by the user.
+The default configuration is {config_filename}.
 
 A description of how to configure and use this program can be found at
 `<https://avendesora.readthedocs.io/en/latest/api.html#example-add-ssh-keys>_.
 """
 
-from pathlib import Path
 
+# IMPORTS {{{1
+from pathlib import Path
 import pexpect
 from appdirs import user_config_dir
 from avendesora import PasswordError, PasswordGenerator
 from docopt import docopt
 from inform import (
-    Error, Inform, codicil, comment, display, error, warn, os_error
+    Error, Inform, codicil, comment, display, error, full_stop, os_error, warn
 )
+from voluptuous import Schema, Invalid, MultipleInvalid
 import nestedtext as nt
+import os
+
 
-__version__ = "0.4.0"
-__released__ = "2020-10-19"
+# GLOBALS {{{1
+__version__ = "0.5"
+__released__ = "2023-04-20"
 
 # Settings
 # These cannot be overridden in ~/.config/addsshkeys/config
 prog_name = "addsshkeys"
 config_filename = "config"
 settings_dir = user_config_dir(prog_name)
 
 # These can be overridden in ~/.config/addsshkeys/config
 ssh_add = "ssh-add"
 ssh_keys = {}
 config_file_mask = 0o077
+auth_sock_path = None
 
-# read command line
+# UTILITIES {{{1
+def to_list(arg):
+    if isinstance(arg, str):
+        return arg.replace(',', ' ').split()
+    if isinstance(arg, dict):
+        raise Invalid('expected a list')
+    return arg
+
+def to_path(path):
+    if isinstance(path, str):
+        return Path(path).expanduser()
+    raise Invalid('expected a path')
+
+def to_octal(arg):
+    try:
+        return int(arg, base=8)
+    except (ValueError, TypeError):
+        raise Invalid('expected an octal integer')
+
+def to_gpg_ids(arg):
+    return [to_gpg_id(i) for i in to_list(arg)]
+
+def normalize_key(key, parent_keys):
+    return '_'.join(key.lower().split())
+
+def get_auth_sock():
+    auth_sock = os.environ.get('SSH_AUTH_SOCK')
+    if not auth_sock:
+        raise Error(
+            'cannot access ssh-agent ($SSH_AUTH_SOCK not set or empty).'
+        )
+    return auth_sock
+
+
+# CONFIGURATION SCHEMA {{{1
+config_validator = Schema(dict(
+    ssh_keys = {
+        str: dict(paths=to_list, account=str, passphrase=str)
+    },
+    config_file_mask = to_octal,
+    auth_sock_path = to_path,
+))
+
+# READ COMMAND LINE {{{1
 cmdline = docopt(__doc__.format(**locals()))
 verbose = cmdline["--verbose"]
 list_keys = cmdline["--list"]
 config = cmdline["<config>"]
 if not config:
     config = config_filename
 
+
+# READ CONFIGURATION FILE {{{1
 try:
     # initialization
     Inform(verbose=verbose)
     settings_dir = Path(settings_dir)
     pw = None
 
     # read settings file
     config_filepath = Path(settings_dir, config)
-    if config_filepath.exists():
-        settings = nt.load(config_filepath, top='dict')
-    else:
-        # try again, this time with a .nt suffix
+    if not config_filepath.exists():
         config_filepath = config_filepath.with_suffix('.nt')
-        if config_filepath.exists():
-            settings = nt.load(config_filepath, top='dict')
-        else:
-            raise Error("config file not found.", culprit=config_filepath)
-    settings['config_file_mask'] = int(
-        settings.get('config_file_mask', config_file_mask),
-        base = 8
+    if not config_filepath.exists():
+        raise Error("config file not found.", culprit=config_filepath)
+
+    settings = nt.load(
+        config_filepath,
+        top = 'dict',
+        keymap = (keymap:={}),
+        normalize_key = normalize_key
     )
+    settings = config_validator(settings)
     locals().update(settings)
 
     if not ssh_keys:
         raise Error("no keys found.", culprit=config_filepath)
 
-    # load keys
+
+    # LOAD KEYS {{{1
     for key, values in ssh_keys.items():
+        comment(f"{key}:")
         try:
             paths = values["paths"].split()
         except AttributeError:
             paths = values["paths"]
         except KeyError:
             raise Error("missing paths.", culprit=key)
         account_name = values.get("account")
         passphrase = values.get("passphrase")
         if list_keys:
             display(f"{key}:")
             for path in paths:
                 display(f"    {path}")
             continue
-        try:
-            if account_name:
-                if not pw:
-                    pw = PasswordGenerator()
-                account = pw.get_account(account_name)
-                if passphrase:
-                    passphrase = str(account.get_value(passphrase).value)
-                else:
-                    passphrase = str(account.get_passcode().value)
-            elif not passphrase:
-                raise Error("missing passphrase.", culprit=key)
+
+        if account_name:
+            if not pw:
+                pw = PasswordGenerator()
+            account = pw.get_account(account_name)
+            if passphrase:
+                passphrase = str(account.get_value(passphrase).value)
             else:
-                # config file contains the passphrase, check its permissions
-                permissions = config_filepath.stat().st_mode & 0o777
-                violation = permissions & config_file_mask
-                if violation:
-                    recommended = permissions & ~config_file_mask
-                    warn("file permissions are too loose.", culprit=config_filepath)
-                    codicil(
-                        "Recommend running: chmod {:o} {}".format(
-                            recommended, config_filepath
-                        )
+                passphrase = str(account.get_passcode().value)
+        elif not passphrase:
+            raise Error("missing passphrase.", culprit=key)
+        else:
+            # config file contains the passphrase, check its permissions
+            permissions = config_filepath.stat().st_mode & 0o777
+            violation = permissions & config_file_mask
+            if violation:
+                recommended = permissions & ~config_file_mask
+                warn("file permissions are too loose.", culprit=config_filepath)
+                codicil(
+                    "Recommend running: chmod {:o} {}".format(
+                        recommended, config_filepath
                     )
+                )
 
-            for path in paths:
-                comment(f"{key:>15}: adding {path}")
-                path = Path(path).expanduser()
-                path = Path("~/.ssh", path).expanduser()
-                try:
-                    sshadd = pexpect.spawn(ssh_add, [str(path)])
-                    sshadd.expect("Enter passphrase for %s: " % (path), timeout=4)
-                    sshadd.sendline(passphrase)
-                    sshadd.expect(pexpect.EOF)
-                    sshadd.close()
-                    response = sshadd.before.decode("utf-8")
-                    if "identity added" in response.lower():
-                        continue
-                except (pexpect.EOF, pexpect.TIMEOUT):
-                    pass
-                error("failed.", culprit=key)
-                codicil("response:", sshadd.before.decode("utf8"), culprit=ssh_add)
-                codicil("exit status:", sshadd.exitstatus, culprit=ssh_add)
-        except PasswordError as e:
-            e.report(culprit=key)
+        # issue error if ssh-agent is not available
+        get_auth_sock()
+
+        for path in paths:
+            comment(f"    adding {path}")
+            path = Path(path).expanduser()
+            path = Path("~/.ssh", path).expanduser()
+            try:
+                sshadd = pexpect.spawn(ssh_add, [str(path)])
+                sshadd.expect("Enter passphrase for %s: " % (path), timeout=4)
+                sshadd.sendline(passphrase)
+                sshadd.expect(pexpect.EOF)
+                sshadd.close()
+                response = sshadd.before.decode("utf-8")
+                if "identity added" in response.lower():
+                    continue
+            except (pexpect.EOF, pexpect.TIMEOUT):
+                pass
+            error("failed.", culprit=key)
+            codicil("response:", sshadd.before.decode("utf8"), culprit=ssh_add)
+            codicil("exit status:", sshadd.exitstatus, culprit=ssh_add)
+
+    if auth_sock_path:
+        comment(f"writing $SSH_AUTH_SOCK to {auth_sock_path!s}")
+        auth_sock_path.write_text(get_auth_sock())
 
-except (Error, PasswordError) as e:
+# HANDLE EXCEPTIONS {{{1
+except (Error, PasswordError, nt.NestedTextError) as e:
     e.report()
+except MultipleInvalid as exception:  # report schema violations
+    voluptuous_error_msg_mappings = {
+        "extra keys not allowed": ("unknown key", "key"),
+    }
+    for e in exception.errors:
+        msg, flag = voluptuous_error_msg_mappings.get(
+            e.msg, (e.msg, 'value')
+        )
+        loc = keymap.get(tuple(e.path))
+        codicil = loc.as_line(flag) if loc else None
+        keys = nt.join_keys(e.path, keymap=keymap)
+        error(
+            full_stop(msg),
+            culprit = (config_filepath, keys),
+            codicil = codicil
+        )
 except OSError as e:
     error(os_error(e))
 except KeyboardInterrupt:
     comment("Killed by user.")
```

### Comparing `addsshkeys-0.4.0/addsshkeys.egg-info/PKG-INFO` & `addsshkeys-0.5/addsshkeys.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,141 +1,170 @@
 Metadata-Version: 2.1
 Name: addsshkeys
-Version: 0.4.0
+Version: 0.5
 Summary: Add keys to SSH Agent
 Home-page: https://github.com/kenkundert/addsshkeys
+Download-URL: https://github.com/kenkundert/addsshkeys/tarball/master
 Author: Ken Kundert
 Author-email: addsshkeys@nurdletech.com
 License: GPLv3+
-Download-URL: https://github.com/kenkundert/addsshkeys/tarball/master
-Description: AddSSHkeys:  Add Keys to SSH Agent
-        ==================================
-        
-        | Version: 0.4.0
-        | Released: 2020-10-19
-        |
-        
-        *AddSSHkeys* adds all of your keys to SSH Agent in one operation. It can work 
-        with `Avendesora <https://avendesora.readthedocs.io>`_ to keep your passphrases 
-        secure.
-        
-        Please report all bugs and suggestions to addsshkeys@nurdletech.com
-        
-        Getting Started
-        ---------------
-        
-        You download and install *AddSSHkeys* with::
-        
-            pip3 install --user addsshkeys
-        
-        Once installed, you will need at least one configuration file.
-        Configurations are placed in: ~/.config/addsshkeys.
-        They are `NestedText <https://nestedtext.readthedocs.io>`_ files.
-        The default configuration is *config*; the default file is *config.nt*.
-        
-        The following settings may be given in your config files.
-        
-        **ssh_add**
-        
-        The name of the command that adds keys to your SSH agent. By default, 'ssh-add' 
-        is used.
-        
-        **ssh_keys**
-        
-        This setting is required.  It contains a dictionary of dictionaries that 
-        contains information about each key.  The primary dictionary contains a name and 
-        the values for each key. The values are held in a dictionary that may contain 
-        three fields:
-        
-        *paths*
-        
-        This is required and contains the paths to one or more SSH private key files.  
-        It may be a list of strings, or a single string that is split.  If a relative 
-        path is given, it is relative to ~/.ssh.
-        
-        *account*
-        
-        This gives the name of the Avendesora account that holds passphrase for the 
-        keys. If present, Avendesora will be queried for the passphrase.
-        
-        *passphrase*
-        
-        This is required if *account* is not given, otherwise it is optional.  If 
-        *account* is given, it is the name of the passphrase field in Avendesora, which 
-        defaults to 'passcode'. If account is not given, it is the passphrase itself. In 
-        this case, the settings file should only be readable by the user.
-        
-        **config_file_mask**
-        
-        An integer that determines if a warning should be printed about the
-        config file permissions being too loose.  The permissions are only checked
-        if the file is found to contain a passphrase. Default is 0o077.  Set to
-        0o000 to disable the warning. Set to 0o077 to generate a warning if the
-        configuration directory is readable or writable by the group or others. Set
-        to 0o007 to generated a warning if the directory is readable or writable by
-        others.
-        
-        Here is an example configuration file::
-        
-            ssh_keys:
-                primary:
-                    paths: primary-ed25519 primary-rsa
-                    account: primary-ssh-key
-                digitalocean:
-                    paths: digitalocean
-                    account: digitalocean-ssh-key
-                github:
-                    paths: github
-                    passphrase: canard apply trousseau forgive
-                backups:
-                    paths: dumper
-                    account: dumper-ssh-key
-        
-        
-        Running AddSSHkeys
-        ------------------
-        
-        Once configured, you can run *AddSSHkeys* with the default configuration using::
-        
-            addsshkeys
-        
-        And you can run it with a particular configuration using::
-        
-            addsshkeys <config>
-        
-        where ``<config>`` is the name of the configuration you wish to use (no need to 
-        give the .nt suffix).  In this way you can have several bundles of keys that you 
-        can load as needed.
-        
-        
-        Releases
-        --------
-        **Latest Development Version**:
-            | Version: 0.4.0
-            | Released: 2020-10-19
-        
-        
-        0.4 (2020-10-19)
-            - fix *config_file_mask*.
-        
-        0.3 (2020-10-19)
-            - allow config file to end with .nt suffix.
-        
-        0.2 (2020-10-14)
-            - update to latest version of NestedText
-        
-        0.1 (2020-08-31)
-            - convert to NestedText for settings file.
-        
 Keywords: avendesora,ssh
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+
+AddSSHkeys — Add Keys to SSH Agent
+==================================
+
+.. image:: https://pepy.tech/badge/addsshkeys/month
+    :target: https://pepy.tech/project/addsshkeys
+
+.. image:: https://img.shields.io/pypi/v/addsshkeys.svg
+    :target: https://pypi.python.org/pypi/addsshkeys
+
+.. image:: https://img.shields.io/pypi/pyversions/addsshkeys.svg
+    :target: https://pypi.python.org/pypi/addsshkeys
+
+| Version: 0.5
+| Released: 2023-04-20
+|
+
+*AddSSHkeys* adds all of your keys to SSH Agent in one operation.
+It is helpful if you routinely add more than one key to your agent.
+It can work with `Avendesora <https://avendesora.readthedocs.io>`_ to keep your 
+passphrases secure.
+
+Please report all bugs and suggestions to addsshkeys@nurdletech.com
+
+Getting Started
+---------------
+
+Download and install *AddSSHkeys* with::
+
+    pip install addsshkeys
+
+Once installed, you will need at least one configuration file.
+Configurations are placed in: ~/.config/addsshkeys.
+They are `NestedText <https://nestedtext.org>`_ files.
+The default configuration is *config*; the default file is *config.nt*.
+
+The following settings may be given in your config files.
+
+**ssh_add**
+
+The name of the command that adds keys to your SSH agent.
+By default, 'ssh-add' is used.
+
+**ssh_keys**
+
+This setting is required.
+It contains a dictionary of dictionaries that contains information about each 
+key.
+The primary dictionary contains a name and the values for each key.
+The values are held in a dictionary that may contain three fields:
+
+*paths*
+
+This is required and contains the paths to one or more SSH private key files.
+It may be a list of strings, or a single string that is split.
+If a relative path is given, it is relative to ~/.ssh.
+
+*account*
+
+This gives the name of the Avendesora account that holds passphrase for the 
+keys.
+If present, Avendesora will be queried for the passphrase.
+
+*passphrase*
+
+This is required if *account* is not given, otherwise it is optional.
+If *account* is given, it is the name of the passphrase field in Avendesora, 
+which defaults to 'passcode'.
+If account is not given, it is the passphrase itself.
+In this case, the settings file should only be readable by the user.
+
+**config_file_mask**
+
+An integer that determines if a warning should be printed about the config file 
+permissions being too loose.
+The permissions are only checked if the file is found to contain a passphrase.
+Default is 077.
+Set to 000 to disable the warning.
+Set to 077 to generate a warning if the configuration directory is readable or 
+writable by the group or others.
+Set to 007 to generated a warning if the directory is readable or writable by 
+others.
+
+**auth_sock_path**
+
+If given, the value of $SSH_AUTH_SOCKET is written to the specified path.
+This can be useful when running SSH related commands in cron and anacron 
+scripts.
+
+
+Here is an example configuration file::
+
+    ssh_keys:
+        primary:
+            paths: primary-ed25519 primary-rsa
+            account: primary-ssh-key
+        digitalocean:
+            paths: digitalocean
+            account: digitalocean-ssh-key
+        github:
+            paths: github
+            passphrase: canard apply trousseau forgive
+        backups:
+            paths: dumper
+            account: dumper-ssh-key
+
+    # assure config file is only readable by me
+    config_file_mask: 077
+
+    # used to provide path to SSH authorization socket to scripts run by cron
+    auth_sock_path: ~/.ssh/auth-sock
+
+Underscores can be replaced by spaces in all keys.
+
+Running AddSSHkeys
+------------------
+
+Once configured, you can run *AddSSHkeys* with the default configuration using::
+
+    addsshkeys
+
+And you can run it with a particular configuration using::
+
+    addsshkeys <config>
+
+where ``<config>`` is the name of the configuration you wish to use (no need to 
+give the .nt suffix).
+In this way you can have several bundles of keys that you can load as needed.
+
+
+Releases
+--------
+**Latest Development Version**:
+    | Version: 0.5
+    | Released: 2023-04-20
+
+0.5 (2023-04-20)
+    - added *auth_sock_path*.
+
+0.4 (2020-10-19)
+    - fix *config_file_mask*.
+
+0.3 (2020-10-19)
+    - allow config file to end with .nt suffix.
+
+0.2 (2020-10-14)
+    - update to latest version of NestedText
+
+0.1 (2020-08-31)
+    - convert to NestedText for settings file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `addsshkeys-0.4.0/setup.py` & `addsshkeys-0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,40 +4,40 @@
 
 from setuptools import setup
 
 with open("README.rst", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
-    name="addsshkeys",
-    version="0.4.0",
-    author="Ken Kundert",
-    author_email="addsshkeys@nurdletech.com",
-    description="Add keys to SSH Agent",
-    long_description=readme,
-    long_description_content_type = 'text/x-rst',
-    url="https://github.com/kenkundert/addsshkeys",
-    download_url="https://github.com/kenkundert/addsshkeys/tarball/master",
-    license="GPLv3+",
-    scripts="addsshkeys".split(),
-    install_requires=[
+    name = "addsshkeys",
+    version = "0.5",
+    author = "Ken Kundert",
+    author_email = "addsshkeys@nurdletech.com",
+    description = "Add keys to SSH Agent",
+    long_description = readme,
+    long_description_content_type  =  'text/x-rst',
+    url = "https://github.com/kenkundert/addsshkeys",
+    download_url = "https://github.com/kenkundert/addsshkeys/tarball/master",
+    license = "GPLv3+",
+    scripts = "addsshkeys".split(),
+    install_requires = [
         "appdirs",
         "avendesora>=1.12",
         "docopt",
         "inform>=1.14",
         "nestedtext>=1.1",
         "pexpect",
     ],
-    python_requires=">=3.6",
-    keywords="avendesora ssh".split(),
-    classifiers=[
+    python_requires = ">=3.8",
+    zip_safe = True,
+    keywords = "avendesora ssh".split(),
+    classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3",
         "Topic :: Utilities",
     ],
 )
```

