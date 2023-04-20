# Comparing `tmp/pysetns-0.2.3.1.tar.gz` & `tmp/pysetns-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysetns-0.2.3.1.tar", last modified: Tue Apr 18 16:18:54 2023, max compression
+gzip compressed data, was "pysetns-0.3.0.tar", last modified: Thu Apr 20 19:22:03 2023, max compression
```

## Comparing `pysetns-0.2.3.1.tar` & `pysetns-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:18:54.611884 pysetns-0.2.3.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-04-18 16:18:40.000000 pysetns-0.2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-18 16:18:54.611884 pysetns-0.2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-18 16:18:40.000000 pysetns-0.2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:18:54.611884 pysetns-0.2.3.1/pysetns/
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-04-18 16:18:40.000000 pysetns-0.2.3.1/pysetns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:18:54.611884 pysetns-0.2.3.1/pysetns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-18 16:18:54.000000 pysetns-0.2.3.1/pysetns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-18 16:18:54.000000 pysetns-0.2.3.1/pysetns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:18:54.000000 pysetns-0.2.3.1/pysetns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 16:18:54.000000 pysetns-0.2.3.1/pysetns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:18:54.611884 pysetns-0.2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-18 16:18:40.000000 pysetns-0.2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:18:54.611884 pysetns-0.2.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-18 16:18:40.000000 pysetns-0.2.3.1/src/ext.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:22:03.715916 pysetns-0.3.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-04-20 19:21:51.000000 pysetns-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-20 19:22:03.715916 pysetns-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-20 19:21:51.000000 pysetns-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:22:03.715916 pysetns-0.3.0/pysetns/
+-rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-04-20 19:21:51.000000 pysetns-0.3.0/pysetns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:22:03.715916 pysetns-0.3.0/pysetns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-20 19:22:03.000000 pysetns-0.3.0/pysetns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-20 19:22:03.000000 pysetns-0.3.0/pysetns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:22:03.000000 pysetns-0.3.0/pysetns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 19:22:03.000000 pysetns-0.3.0/pysetns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:22:03.715916 pysetns-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-20 19:21:51.000000 pysetns-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:22:03.715916 pysetns-0.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-20 19:21:51.000000 pysetns-0.3.0/src/ext.c
```

### Comparing `pysetns-0.2.3.1/LICENSE` & `pysetns-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysetns-0.2.3.1/PKG-INFO` & `pysetns-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pysetns
-Version: 0.2.3.1
+Version: 0.3.0
 Summary: Python wrapper for setns Linux syscall.
 Home-page: https://github.com/baskiton/pysetns
 Author: Alexander Baskikh
 Author-email: baskiton@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/baskiton/pysetns
 Project-URL: Bug Tracker, https://github.com/baskiton/pysetns/issues
 Keywords: linux kernel namespace setns
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: System :: Operating System Kernels :: Linux
-Requires-Python: >=3.8
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysetns
 [![pypi](https://img.shields.io/pypi/v/pysetns?logo=python&logoColor=white)](https://pypi.org/project/pysetns/)
 [![downloads](https://img.shields.io/pypi/dm/pysetns?logo=python&logoColor=white)](https://pypi.org/project/pysetns/)
 [![license](https://img.shields.io/pypi/l/pysetns?logo=open-source-initiative&logoColor=white)](https://github.com/baskiton/pysetns/blob/main/LICENSE)
@@ -31,15 +31,16 @@
 
 To detail see the [documentation][documentation]
 
 ### IMPORTANT!
 `setns` required execution from **ROOT**!
 
 ## Requirements
- * Python 3.8+
+ * Linux 3.0+
+ * Python 3
 
 ## Installing
 ### Using PIP
 ```sh
 $ pip install pysetns
 ```
```

### Comparing `pysetns-0.2.3.1/README.md` & `pysetns-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 To detail see the [documentation][documentation]
 
 ### IMPORTANT!
 `setns` required execution from **ROOT**!
 
 ## Requirements
- * Python 3.8+
+ * Linux 3.0+
+ * Python 3
 
 ## Installing
 ### Using PIP
 ```sh
 $ pip install pysetns
 ```
```

### Comparing `pysetns-0.2.3.1/pysetns/__init__.py` & `pysetns-0.3.0/pysetns/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,139 +1,150 @@
 # coding: utf-8
 
-__all__ = ('__version__', 'NS_TIME', 'NS_MNT', 'NS_CGROUP', 'NS_UTS',
+__all__ = ('NS_TIME', 'NS_MNT', 'NS_CGROUP', 'NS_UTS',
            'NS_IPC', 'NS_USER', 'NS_PID', 'NS_NET', 'NS_ALL',
            'UserNamespaceWarning', 'Namespace', 'get_ns_string')
 
 import errno
 import os
 
-from typing import Callable, Union, Iterable
+from collections import OrderedDict as OD
 
 from . import ext
 
-__version__ = '0.2.3.1'
 
+NS_INVALID = ext.NS_INVALID
 NS_TIME = ext.CLONE_NEWTIME     # time namespace (since Linux 5.8)
 NS_MNT = ext.CLONE_NEWNS        # mount namespace group (since Linux 3.8)
 NS_CGROUP = ext.CLONE_NEWCGROUP # cgroup namespace (since Linux 4.6)
 NS_UTS = ext.CLONE_NEWUTS       # utsname namespace (since Linux 3.0)
 NS_IPC = ext.CLONE_NEWIPC       # ipc namespace (since Linux 3.0)
 NS_USER = ext.CLONE_NEWUSER     # user namespace (since Linux 3.8)
 NS_PID = ext.CLONE_NEWPID       # pid namespace (since Linux 3.8)
 NS_NET = ext.CLONE_NEWNET       # network namespace (since Linux 3.0)
 NS_ALL = NS_MNT | NS_USER | NS_PID | NS_NET | NS_UTS | NS_IPC | NS_CGROUP | NS_TIME
 
-_NS_NAMES = {
+_NS_NAMES = OD((
     # Order is very important here! NS_USER should always be last!
-    NS_CGROUP: 'cgroup',
-    NS_IPC: 'ipc',
-    NS_UTS: 'uts',
-    NS_NET: 'net',
-    NS_PID: 'pid',
-    NS_MNT: 'mnt',
-    NS_TIME: 'time',
-    NS_USER: 'user',
-}
+    (NS_CGROUP, 'cgroup'),
+    (NS_IPC, 'ipc'),
+    (NS_UTS, 'uts'),
+    (NS_NET, 'net'),
+    (NS_PID, 'pid'),
+    (NS_MNT, 'mnt'),
+    (NS_TIME, 'time'),
+    (NS_USER, 'user'),
+))
+if NS_INVALID in _NS_NAMES:
+    _NS_NAMES.pop(NS_INVALID)
 
-_OFLAGS = os.O_RDONLY | os.O_NONBLOCK | os.O_NOCTTY | getattr(os, 'O_CLOEXEC', 0o2000000)
+_OFLAGS = os.O_RDONLY | os.O_NONBLOCK | os.O_NOCTTY | ext.O_CLOEXEC
 
 
-def get_ns_string(ns_types: int) -> str:
+def get_ns_string(ns_types):
     """
     Represents namespace types `ns_types` in string view
+    :type ns_types: int
+    :rtype: str
     """
 
     return '|'.join(v for k, v in _NS_NAMES.items() if k & ns_types)
 
 
 class UserNamespaceWarning(Warning):
-    def __init__(self, gid: int, uid: int, pid: Union[int, str]):
-        self.message = (f'Further work will be under the *USER* namespace '
-                        f'with rights of the user {gid}:{uid} of pid {pid}!')
+    def __init__(self, gid, uid, pid):
+        self.message = ('Further work will be under the *USER* namespace '
+                        'with rights of the user %s:%s of pid %s!' % (gid, uid, pid))
         super(UserNamespaceWarning, self).__init__(self.message)
 
 
 class Namespace:
     """
     Namespace object
     """
 
-    def __init__(self, target_pid: Union[int, str], ns_types: int = NS_ALL,
-                 target_gid: int = None, target_uid: int = None,
-                 do_fork: bool = False, true_user: bool = False,
-                 keep_caps: bool = False):
+    def __init__(self, target_pid, ns_types=NS_ALL, target_gid=None, target_uid=None,
+                 do_fork=False, true_user=False, keep_caps=False):
         """
+        :type target_pid: int | str
         :param target_pid: The pid of the process whose namespace you want to access
+        :type ns_types: int
         :param ns_types: Namespace types to be accessed. These are bitwise. :const:`NS_ALL` included all of this:
 
             - :const:`NS_TIME` - time namespace (since Linux 5.8)
             - :const:`NS_MNT` - mount namespace group (since Linux 3.8)
             - :const:`NS_CGROUP` - cgroup namespace (since Linux 4.6)
             - :const:`NS_UTS` - utsname namespace (since Linux 3.0)
             - :const:`NS_IPC` - ipc namespace (since Linux 3.0)
             - :const:`NS_USER` - user namespace (since Linux 3.8)
             - :const:`NS_PID` - pid namespace (since Linux 3.8)
             - :const:`NS_NET` - network namespace (since Linux 3.0)
 
+        :type target_gid: int | None
         :param target_gid:
+        :type target_uid: int | None
         :param target_uid: The GID and UID of the user you want to access in :const:`NS_USER` as.
             If None, the GID and UID of the process owner will be used
+        :type do_fork: bool
         :param do_fork: Enter into the namespace in a separate process. If `ns_types` includes :const:`NS_USER`
             or :const:`NS_PID`, entering into the namespace will be done in a separate process
             and `do_fork` value is ignored
+        :type true_user: bool
         :param true_user: If False (default), entering into :const:`NS_USER` will be done by simply switching
             to target GID and UID (`target_gid`, `target_uid`), otherwise through a system call,
             but then returning from the namespace will not be possible and the program will need to be terminated,
             and in this case the :class:`UserNamespaceWarning` exception will be raised
+        :type keep_caps: bool
         :param keep_caps: Preserve root capabilities if you need to perform an action on behalf of a user
             with administrator rights. Only relevant if `ns_types` includes :const:`NS_USER`
 
         :raises FileNotFoundError, OSError: if `target_pid` is not valid
         :raises TypeError: if `ns_types` is not valid
         """
 
         if not (NS_ALL & ns_types):
             raise TypeError('Invalid namespace types')
 
         self.errors = {}
         self.retry = False
         self.target_pid = target_pid
-        proc_st = os.stat(f'/proc/{self.target_pid}')
+        proc_st = os.stat('/proc/%s' % self.target_pid)
         self.target_gid = proc_st.st_gid if (target_gid is None) else target_gid
         self.target_uid = proc_st.st_uid if (target_uid is None) else target_uid
         self.true_user = true_user
         self.keep_caps = keep_caps
 
-        self.parent_ns_files = {nstype: self._get_nsfd('self', name)
-                                for nstype, name in _NS_NAMES.items()
-                                if nstype & ns_types}
+        self.parent_ns_files = OD((nstype, self._get_nsfd('self', name))
+                                  for nstype, name in _NS_NAMES.items()
+                                  if nstype & ns_types)
         if ns_types & NS_USER and self._disallow_user_ns(target_pid):
             self._close_fds(self.parent_ns_files.pop(NS_USER))
-        self.target_ns_files = {nstype: self._get_nsfd(target_pid, name)
-                                for nstype, name in _NS_NAMES.items()
-                                if self.parent_ns_files.get(nstype, -1) != -1}
+        self.target_ns_files = OD((nstype, self._get_nsfd(target_pid, name))
+                                  for nstype, name in _NS_NAMES.items()
+                                  if self.parent_ns_files.get(nstype, -1) != -1)
         self.namespaces = ns_types & NS_USER
         for t_nstype, t_fd in self.target_ns_files.items():
             if t_fd != -1:
                 self.namespaces |= t_nstype
             else:
                 self._close_fds(self.parent_ns_files.setdefault(t_nstype, -1))
         self.do_fork = do_fork or self.namespaces & (NS_USER | NS_PID)
         self.fork = -1
 
-    def enter(self, target: Callable, *args, **kwargs) -> None:
+    def enter(self, target, *args, **kwargs):
         """
         Enter into **namespace** and execute `target` function with its `args` and `kwargs`.
         Exiting namespaces will happen automatically. But if this needs to be done inside the `target` function,
         pass the **namespace** object as one of the parameters to it and call the :func:`Namespace.exit` method.
         If an error occurs while entering into **namespace**, it will be written to the ``Namespace.errors`` attribute
         in the format ``{ns_type: error}``, and if it was not the only `ns_type`, work will continue.
         Errors caused by the operation of the `target` function will be ignored, so take care of them yourself.
 
+        :type target: Callable
+        :rtype: None
         :raise: :class:`UserNamespaceWarning` on exiting when `true_user` parameter of the
             :class:`Namespace` is ``True``
         """
 
         if not callable(target):
             raise TypeError('`target` is not callable')
 
@@ -174,20 +185,22 @@
                     os.setuid(self.target_uid)
         exitcode = 0
         try:
             exitcode = target(*args, **kwargs)
         finally:
             self.exit(exitcode)
 
-    def exit(self, errcode: int = 0) -> None:
+    def exit(self, errcode=0):
         """
         Exit from **namespace** and set the `errcode` if required. You usually don't need to call this method
         yourself. If the `errcode` is set to 11 (:const:`EAGAIN`), the ``Namespace.retry`` attribute
         will be set to ``True``.
 
+        :type errcode: int
+        :rtype: None
         :raise: :class:`UserNamespaceWarning` when `true_user` parameter of the :class:`Namespace` is ``True``
         """
 
         uerr = 0
         if self.do_fork and self.fork != -1:
             if self.fork:
                 _, status = os.wait()
@@ -207,53 +220,50 @@
                         ext.setns(fd, ns)
                 except OSError as e:
                     # further work is strictly prohibited!
                     # the entire parent process must be terminated!
                     self._close_fds(fd)
                     self.parent_ns_files[ns] = -1
                     self.namespaces &= ~ns
-                    e.strerror = f'{e.strerror} when exiting from "{_NS_NAMES[ns]}" namespace. ' \
-                                 f'Further work is impossible!'
+                    e.strerror = '%s when exiting from "%s" namespace. ' \
+                                 'Further work is impossible!' % (e.strerror, _NS_NAMES[ns])
                     raise
-        self._close_fds(self.parent_ns_files.values())
-        self._close_fds(self.target_ns_files.values())
+        self._close_fds(*self.parent_ns_files.values())
+        self._close_fds(*self.target_ns_files.values())
         if uerr:
             self.parent_ns_files.clear()
             self.target_ns_files.clear()
             raise UserNamespaceWarning(self.target_gid, self.target_uid, self.target_pid)
         else:
             self.parent_ns_files = dict.fromkeys(self.parent_ns_files, -1)
             self.target_ns_files = dict.fromkeys(self.target_ns_files, -1)
 
     @staticmethod
-    def _get_nsfd(pid: Union[int, str], ns_str: str) -> int:
+    def _get_nsfd(pid, ns_str):
         try:
-            return os.open(f'/proc/{pid}/ns/{ns_str}', _OFLAGS)
+            return os.open('/proc/%s/ns/%s' % (pid, ns_str), _OFLAGS)
         except OSError:
             return -1
 
     @staticmethod
-    def _disallow_user_ns(target_pid) -> bool:
+    def _disallow_user_ns(target_pid):
         # It is not permitted to use setns(2) to reenter the caller's current user namespace
-        pp = f'/proc/{os.getpid()}'
-        tp = f'/proc/{target_pid}'
+        pp = '/proc/%s' % os.getpid()
+        tp = '/proc/%s' % target_pid
         if os.path.isdir(pp) and os.path.isdir(tp):
             try:
                 parent_ino = os.stat(os.path.join(pp, 'ns/user')).st_ino
                 target_ino = os.stat(os.path.join(tp, 'ns/user')).st_ino
                 return parent_ino == target_ino
             except OSError:
                 # user namespace is not exist. disallow
                 return True
         else:
             raise OSError(errno.ESRCH, os.strerror(errno.ESRCH))
 
     @staticmethod
-    def _close_fds(fds: Union[int, Iterable]) -> None:
-        if isinstance(fds, Iterable):
-            for fd in fds:
-                Namespace._close_fds(fd)
-        else:
+    def _close_fds(*fds):
+        for fd in fds:
             try:
-                os.close(fds)
+                os.close(fd)
             except OSError:
                 pass
```

### Comparing `pysetns-0.2.3.1/pysetns.egg-info/PKG-INFO` & `pysetns-0.3.0/pysetns.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pysetns
-Version: 0.2.3.1
+Version: 0.3.0
 Summary: Python wrapper for setns Linux syscall.
 Home-page: https://github.com/baskiton/pysetns
 Author: Alexander Baskikh
 Author-email: baskiton@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/baskiton/pysetns
 Project-URL: Bug Tracker, https://github.com/baskiton/pysetns/issues
 Keywords: linux kernel namespace setns
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: System :: Operating System Kernels :: Linux
-Requires-Python: >=3.8
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysetns
 [![pypi](https://img.shields.io/pypi/v/pysetns?logo=python&logoColor=white)](https://pypi.org/project/pysetns/)
 [![downloads](https://img.shields.io/pypi/dm/pysetns?logo=python&logoColor=white)](https://pypi.org/project/pysetns/)
 [![license](https://img.shields.io/pypi/l/pysetns?logo=open-source-initiative&logoColor=white)](https://github.com/baskiton/pysetns/blob/main/LICENSE)
@@ -31,15 +31,16 @@
 
 To detail see the [documentation][documentation]
 
 ### IMPORTANT!
 `setns` required execution from **ROOT**!
 
 ## Requirements
- * Python 3.8+
+ * Linux 3.0+
+ * Python 3
 
 ## Installing
 ### Using PIP
 ```sh
 $ pip install pysetns
 ```
```

### Comparing `pysetns-0.2.3.1/src/ext.c` & `pysetns-0.3.0/src/ext.c`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 #define _GNU_SOURCE
+#define Py_LIMITED_API 3
 #include <Python.h>
-#include <sched.h>
+#include <fcntl.h>
 #include <linux/sched.h>
 #include <linux/capability.h>
+#include <sched.h>
 #include <sys/prctl.h>
 #include <syscall.h>
 
 
 PyDoc_STRVAR(ext__doc__,
 "Wrapper for setns syscall.\n");
 
-#define EXT_ADD_ZERO_MACRO(name) PyModule_AddIntConstant(module, #name, 0)
+#define NS_INVALID 0
+#define EXT_SET_INVALID_MACRO(name) PyModule_AddIntConstant(module, #name, NS_INVALID)
 #define EXT_ADD_INT_MACRO(name) PyModule_AddIntConstant(module, #name, name)
 
 PyDoc_STRVAR(setns__doc__,
 "setns(fd, nstype=0) -> None\n"
 "\n"
 "Wrapper for setns syscall.\n"
 "See the manpage for setns for more details:\n"
@@ -119,41 +122,44 @@
 PyInit_ext(void)
 {
     PyObject *module = PyModule_Create(&moduledef);
     if (module == NULL) {
         return NULL;
     }
 
+    EXT_ADD_INT_MACRO(O_CLOEXEC);
+    EXT_ADD_INT_MACRO(NS_INVALID);
+
 #ifdef CLONE_NEWIPC     // since Linux 3.0
     EXT_ADD_INT_MACRO(CLONE_NEWIPC);
     EXT_ADD_INT_MACRO(CLONE_NEWNET);
     EXT_ADD_INT_MACRO(CLONE_NEWUTS);
 #else
-    EXT_ADD_ZERO_MACRO(CLONE_NEWIPC);
-    EXT_ADD_ZERO_MACRO(CLONE_NEWNET);
-    EXT_ADD_ZERO_MACRO(CLONE_NEWUTS);
+    EXT_SET_INVALID_MACRO(CLONE_NEWIPC);
+    EXT_SET_INVALID_MACRO(CLONE_NEWNET);
+    EXT_SET_INVALID_MACRO(CLONE_NEWUTS);
 #endif // CLONE_NEWIPC (since Linux 3.0)
 
 #ifdef CLONE_NEWNS      // since Linux 3.8
     EXT_ADD_INT_MACRO(CLONE_NEWNS);
     EXT_ADD_INT_MACRO(CLONE_NEWPID);
     EXT_ADD_INT_MACRO(CLONE_NEWUSER);
 #else
-    EXT_ADD_ZERO_MACRO(CLONE_NEWNS);
-    EXT_ADD_ZERO_MACRO(CLONE_NEWPID);
-    EXT_ADD_ZERO_MACRO(CLONE_NEWUSER);
+    EXT_SET_INVALID_MACRO(CLONE_NEWNS);
+    EXT_SET_INVALID_MACRO(CLONE_NEWPID);
+    EXT_SET_INVALID_MACRO(CLONE_NEWUSER);
 #endif // CLONE_NEWNS (since Linux 3.8)
 
 #ifdef CLONE_NEWCGROUP  // since Linux 4.6
     EXT_ADD_INT_MACRO(CLONE_NEWCGROUP);
 #else
-    EXT_ADD_ZERO_MACRO(CLONE_NEWCGROUP);
+    EXT_SET_INVALID_MACRO(CLONE_NEWCGROUP);
 #endif // CLONE_NEWCGROUP (since Linux 4.6)
 
 #ifdef CLONE_NEWTIME    // since Linux 5.8
     EXT_ADD_INT_MACRO(CLONE_NEWTIME);
 #else
-    EXT_ADD_ZERO_MACRO(CLONE_NEWTIME);
+    EXT_SET_INVALID_MACRO(CLONE_NEWTIME);
 #endif // CLONE_NEWTIME (since Linux 5.8)
 
     return module;
 }
```

